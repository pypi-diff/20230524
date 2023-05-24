# Comparing `tmp/pingertron-0.1.0.tar.gz` & `tmp/pingertron-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pingertron-0.1.0.tar", max compression
+gzip compressed data, was "pingertron-0.2.0.tar", max compression
```

## Comparing `pingertron-0.1.0.tar` & `pingertron-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1071 2023-05-22 15:17:56.890459 pingertron-0.1.0/LICENSE
--rw-r--r--   0        0        0     1597 2023-05-22 18:14:44.481413 pingertron-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-19 20:54:31.460873 pingertron-0.1.0/pingertron/__init__.py
--rw-r--r--   0        0        0     4655 2023-05-22 21:43:47.176680 pingertron-0.1.0/pingertron/main.py
--rw-r--r--   0        0        0     1594 2023-05-22 14:45:31.372782 pingertron-0.1.0/pingertron/metrics.py
--rw-r--r--   0        0        0      531 2023-05-22 15:52:21.557725 pingertron-0.1.0/pingertron/probes_config.py
--rw-r--r--   0        0        0      855 2023-05-22 18:52:50.106748 pingertron-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2395 1970-01-01 00:00:00.000000 pingertron-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-22 15:17:56.890459 pingertron-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1597 2023-05-22 18:14:44.481413 pingertron-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-19 20:54:31.460873 pingertron-0.2.0/pingertron/__init__.py
+-rw-r--r--   0        0        0     5295 2023-05-24 16:09:11.792797 pingertron-0.2.0/pingertron/main.py
+-rw-r--r--   0        0        0     1594 2023-05-22 14:45:31.372782 pingertron-0.2.0/pingertron/metrics.py
+-rw-r--r--   0        0        0      531 2023-05-22 15:52:21.557725 pingertron-0.2.0/pingertron/probes_config.py
+-rw-r--r--   0        0        0      884 2023-05-24 17:47:03.276720 pingertron-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2395 1970-01-01 00:00:00.000000 pingertron-0.2.0/PKG-INFO
```

### Comparing `pingertron-0.1.0/LICENSE` & `pingertron-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pingertron-0.1.0/README.md` & `pingertron-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pingertron-0.1.0/pingertron/main.py` & `pingertron-0.2.0/pingertron/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import asyncio
+import logging
 import pathlib
 from typing import Annotated
 
 import httpx
 import rich.traceback
 import structlog
+import structlog.contextvars
+import structlog.processors
 import typer
 from icmplib import async_ping
 from pydantic_yaml import parse_yaml_file_as
 
 from . import metrics
 from .probes_config import HTTPProbe, ICMPProbe, Probe, ProbesConfig
 
@@ -26,21 +29,21 @@
     )
     metrics.http_request_count.labels(
         method=probe.method,
         url=probe.url,
         expected_status_code=probe.expected_status_code,
     ).inc()
 
-    log.debug("Sending HTTP request")
+    log.debug("ping")
     async with httpx.AsyncClient() as client:
         with metrics.http_response_duration_histogram.labels(
             method=probe.method, url=probe.url
         ).time():
             response = await client.request(method=probe.method, url=probe.url)
-        log.info("Got HTTP response", status_code=response.status_code)
+        log.debug("ack", status_code=response.status_code)
         success = response.status_code == probe.expected_status_code
         metrics.http_response_count.labels(
             method=probe.method,
             url=probe.url,
             expected_status_code=probe.expected_status_code,
             status_code=response.status_code,
             success=success,
@@ -51,22 +54,22 @@
 
 
 async def do_icmp_probe(probe: ICMPProbe):
     log = LOG.bind(
         protocol=probe.protocol,
         hostname=probe.hostname,
     )
-    log.debug("Sending ICMP packet")
+    log.debug("ping")
     metrics.icmp_request_count.labels(hostname=probe.hostname).inc()
     with metrics.icmp_response_duration_histogram.labels(
         hostname=probe.hostname
     ).time():
         ping_host = await async_ping(address=probe.hostname, count=1)
-    log.info(
-        "Got ICMP response",
+    log.debug(
+        "ack",
         rtt=ping_host.max_rtt,
         is_alive=ping_host.is_alive,
     )
     success = ping_host.is_alive
     max_rtt = ping_host.max_rtt / 1000  # ms to seconds
     metrics.icmp_response_count.labels(hostname=probe.hostname, success=success).inc()
     metrics.icmp_max_rtt_histogram.labels(hostname=probe.hostname).observe(max_rtt)
@@ -93,42 +96,54 @@
     while True:
         stat = probes_config_path.stat()
         new_stat = (stat.st_size, stat.st_mtime)
         if probes_config is None or previous_stat != new_stat:
             LOG.debug("Loading probes config", config_path=probes_config_path)
             probes_config = parse_yaml_file_as(ProbesConfig, probes_config_path)
             previous_stat = new_stat
-            LOG.info("Loaded probes config", config=probes_config)
+            LOG.info("Loaded probes config", config=probes_config.dict())
 
         # Start the sleep at the same time as the probes, aiming to start next batch of
         # probes close to exactly the interval time.
         async with asyncio.TaskGroup() as group:
             group.create_task(run_probes(probes_config.probes))
             group.create_task(asyncio.sleep(probes_config.interval_seconds))
 
 
 @app.command()
 def main(
-    config: Annotated[pathlib.Path, typer.Argument()],
-    prometheus_exporter_port: int = 8000,
-    use_json_logging: bool = False,
+    config: Annotated[pathlib.Path, typer.Argument(help="Path to probes.yml config")],
+    prometheus_exporter_port: Annotated[
+        int, typer.Option(help="Port to export prometheus metrics on")
+    ] = 8000,
+    use_json_logging: Annotated[
+        bool, typer.Option(help="Output using JSON logging?")
+    ] = False,
+    verbose: Annotated[bool, typer.Option(help="More verbose log output?")] = False,
 ):
     rich.traceback.install(show_locals=True)
+    log_level = logging.DEBUG if verbose else logging.INFO
     if use_json_logging:
         # Configure same processor stack as default, minus dev bits
         structlog.configure(
             processors=[
                 structlog.contextvars.merge_contextvars,
                 structlog.processors.add_log_level,
                 structlog.processors.StackInfoRenderer(),
                 structlog.processors.TimeStamper(fmt="iso", utc=True),
                 structlog.processors.JSONRenderer(),
-            ]
+            ],
+            wrapper_class=structlog.make_filtering_bound_logger(log_level),
+        )
+    else:
+        structlog.configure(
+            wrapper_class=structlog.make_filtering_bound_logger(log_level),
         )
 
     metrics.setup_metrics(prometheus_exporter_port=prometheus_exporter_port)
+    LOG.debug(f"Prometheus metrics available on port {prometheus_exporter_port}")
 
     asyncio.run(go(probes_config_path=config))
 
 
 if __name__ == "__main__":
     typer.run(app)
```

### Comparing `pingertron-0.1.0/pingertron/metrics.py` & `pingertron-0.2.0/pingertron/metrics.py`

 * *Files identical despite different names*

### Comparing `pingertron-0.1.0/pingertron/probes_config.py` & `pingertron-0.2.0/pingertron/probes_config.py`

 * *Files identical despite different names*

### Comparing `pingertron-0.1.0/pyproject.toml` & `pingertron-0.2.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pingertron"
-version = "0.1.0"
+version = "0.2.0"
 description = "Ping Hosts and URLs and keep stats on successes and failures"
 authors = ["Michael Twomey <mick@twomeylee.name>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
@@ -20,14 +20,15 @@
 
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.3.0"
 ruff = "^0.0.269"
 black = "^23.3.0"
 pytest = "^7.3.1"
+changelog-manager = "^1.3.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
 # Turn on namespaces to support opentelementry
```

### Comparing `pingertron-0.1.0/PKG-INFO` & `pingertron-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pingertron
-Version: 0.1.0
+Version: 0.2.0
 Summary: Ping Hosts and URLs and keep stats on successes and failures
 License: MIT
 Author: Michael Twomey
 Author-email: mick@twomeylee.name
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

