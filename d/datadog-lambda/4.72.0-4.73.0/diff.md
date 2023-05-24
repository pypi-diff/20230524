# Comparing `tmp/datadog_lambda-4.72.0.tar.gz` & `tmp/datadog_lambda-4.73.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datadog_lambda-4.72.0.tar", max compression
+gzip compressed data, was "datadog_lambda-4.73.0.tar", max compression
```

## Comparing `datadog_lambda-4.72.0.tar` & `datadog_lambda-4.73.0.tar`

### file list

```diff
@@ -1,25 +1,24 @@
--rw-r--r--   0        0        0    11379 2022-08-04 20:47:28.483033 datadog_lambda-4.72.0/LICENSE
--rw-r--r--   0        0        0      394 2023-02-13 18:56:36.618770 datadog_lambda-4.72.0/LICENSE-3rdparty.csv
--rw-r--r--   0        0        0     3422 2023-04-21 16:54:22.800300 datadog_lambda-4.72.0/README.md
--rw-r--r--   0        0        0      538 2023-02-17 16:21:55.265937 datadog_lambda-4.72.0/datadog_lambda/__init__.py
--rw-r--r--   0        0        0     3653 2023-02-13 18:56:36.619460 datadog_lambda-4.72.0/datadog_lambda/api.py
--rw-r--r--   0        0        0     7232 2023-04-21 16:53:43.883638 datadog_lambda-4.72.0/datadog_lambda/cold_start.py
--rw-r--r--   0        0        0     1669 2023-02-13 18:56:36.620125 datadog_lambda-4.72.0/datadog_lambda/constants.py
--rw-r--r--   0        0        0     4769 2023-02-13 18:56:36.620241 datadog_lambda-4.72.0/datadog_lambda/dogstatsd.py
--rw-r--r--   0        0        0     1199 2023-02-13 18:56:36.620396 datadog_lambda-4.72.0/datadog_lambda/extension.py
--rw-r--r--   0        0        0      994 2022-08-04 20:47:28.483885 datadog_lambda-4.72.0/datadog_lambda/handler.py
--rw-r--r--   0        0        0     4707 2023-03-15 15:25:33.105333 datadog_lambda-4.72.0/datadog_lambda/metric.py
--rw-r--r--   0        0        0      139 2023-02-13 18:56:36.620660 datadog_lambda-4.72.0/datadog_lambda/module_name.py
--rw-r--r--   0        0        0     4641 2023-02-13 18:56:36.620808 datadog_lambda-4.72.0/datadog_lambda/patch.py
--rw-r--r--   0        0        0      243 2023-02-13 18:56:36.620890 datadog_lambda-4.72.0/datadog_lambda/stats_writer.py
--rw-r--r--   0        0        0      403 2023-02-13 18:56:36.620968 datadog_lambda-4.72.0/datadog_lambda/statsd_writer.py
--rw-r--r--   0        0        0     1751 2023-02-13 18:56:36.621061 datadog_lambda-4.72.0/datadog_lambda/tag_object.py
--rw-r--r--   0        0        0     3240 2023-02-13 18:56:36.621201 datadog_lambda-4.72.0/datadog_lambda/tags.py
--rw-r--r--   0        0        0     2522 2023-02-13 18:56:36.621290 datadog_lambda-4.72.0/datadog_lambda/thread_stats_writer.py
--rw-r--r--   0        0        0    45292 2023-04-12 18:23:27.981500 datadog_lambda-4.72.0/datadog_lambda/tracing.py
--rw-r--r--   0        0        0    12082 2023-04-12 18:23:27.981977 datadog_lambda-4.72.0/datadog_lambda/trigger.py
--rw-r--r--   0        0        0    14126 2023-04-25 15:31:19.068502 datadog_lambda-4.72.0/datadog_lambda/wrapper.py
--rw-r--r--   0        0        0     3449 2023-04-24 17:49:26.625012 datadog_lambda-4.72.0/datadog_lambda/xray.py
--rw-r--r--   0        0        0     1251 2023-04-27 18:36:42.931504 datadog_lambda-4.72.0/pyproject.toml
--rw-r--r--   0        0        0     4555 1970-01-01 00:00:00.000000 datadog_lambda-4.72.0/setup.py
--rw-r--r--   0        0        0     4969 1970-01-01 00:00:00.000000 datadog_lambda-4.72.0/PKG-INFO
+-rw-r--r--   0        0        0    11379 2022-09-22 18:30:00.504292 datadog_lambda-4.73.0/LICENSE
+-rw-r--r--   0        0        0      394 2022-09-22 18:30:00.504380 datadog_lambda-4.73.0/LICENSE-3rdparty.csv
+-rw-r--r--   0        0        0     3422 2023-04-18 14:29:41.172896 datadog_lambda-4.73.0/README.md
+-rw-r--r--   0        0        0      538 2023-02-13 20:46:09.160997 datadog_lambda-4.73.0/datadog_lambda/__init__.py
+-rw-r--r--   0        0        0     3653 2022-09-22 18:30:00.504778 datadog_lambda-4.73.0/datadog_lambda/api.py
+-rw-r--r--   0        0        0     7232 2023-04-18 14:29:41.173911 datadog_lambda-4.73.0/datadog_lambda/cold_start.py
+-rw-r--r--   0        0        0     1669 2023-01-25 19:31:51.675529 datadog_lambda-4.73.0/datadog_lambda/constants.py
+-rw-r--r--   0        0        0     4769 2022-09-22 18:30:00.505031 datadog_lambda-4.73.0/datadog_lambda/dogstatsd.py
+-rw-r--r--   0        0        0     1199 2022-09-22 18:30:00.505121 datadog_lambda-4.73.0/datadog_lambda/extension.py
+-rw-r--r--   0        0        0      994 2022-09-22 18:30:00.505207 datadog_lambda-4.73.0/datadog_lambda/handler.py
+-rw-r--r--   0        0        0     4707 2022-09-22 18:30:00.505343 datadog_lambda-4.73.0/datadog_lambda/metric.py
+-rw-r--r--   0        0        0      139 2022-09-22 18:30:00.505417 datadog_lambda-4.73.0/datadog_lambda/module_name.py
+-rw-r--r--   0        0        0     4641 2022-09-22 18:30:00.505516 datadog_lambda-4.73.0/datadog_lambda/patch.py
+-rw-r--r--   0        0        0      243 2022-09-22 18:30:00.505686 datadog_lambda-4.73.0/datadog_lambda/stats_writer.py
+-rw-r--r--   0        0        0      403 2022-09-22 18:30:00.505792 datadog_lambda-4.73.0/datadog_lambda/statsd_writer.py
+-rw-r--r--   0        0        0     1751 2022-09-22 18:30:00.505884 datadog_lambda-4.73.0/datadog_lambda/tag_object.py
+-rw-r--r--   0        0        0     3240 2022-09-22 18:30:00.505984 datadog_lambda-4.73.0/datadog_lambda/tags.py
+-rw-r--r--   0        0        0     2522 2022-09-22 18:30:00.506089 datadog_lambda-4.73.0/datadog_lambda/thread_stats_writer.py
+-rw-r--r--   0        0        0    45245 2023-05-24 20:17:42.363176 datadog_lambda-4.73.0/datadog_lambda/tracing.py
+-rw-r--r--   0        0        0    12082 2023-04-12 17:19:32.172228 datadog_lambda-4.73.0/datadog_lambda/trigger.py
+-rw-r--r--   0        0        0    14126 2023-05-24 20:17:42.363590 datadog_lambda-4.73.0/datadog_lambda/wrapper.py
+-rw-r--r--   0        0        0     3449 2023-03-22 12:07:02.672991 datadog_lambda-4.73.0/datadog_lambda/xray.py
+-rw-r--r--   0        0        0     1270 2023-05-24 21:34:10.837930 datadog_lambda-4.73.0/pyproject.toml
+-rw-r--r--   0        0        0     4800 1970-01-01 00:00:00.000000 datadog_lambda-4.73.0/PKG-INFO
```

### Comparing `datadog_lambda-4.72.0/LICENSE` & `datadog_lambda-4.73.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.72.0/README.md` & `datadog_lambda-4.73.0/README.md`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.72.0/datadog_lambda/__init__.py` & `datadog_lambda-4.73.0/datadog_lambda/__init__.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.72.0/datadog_lambda/api.py` & `datadog_lambda-4.73.0/datadog_lambda/api.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.72.0/datadog_lambda/cold_start.py` & `datadog_lambda-4.73.0/datadog_lambda/cold_start.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.72.0/datadog_lambda/constants.py` & `datadog_lambda-4.73.0/datadog_lambda/constants.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.72.0/datadog_lambda/dogstatsd.py` & `datadog_lambda-4.73.0/datadog_lambda/dogstatsd.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.72.0/datadog_lambda/extension.py` & `datadog_lambda-4.73.0/datadog_lambda/extension.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.72.0/datadog_lambda/handler.py` & `datadog_lambda-4.73.0/datadog_lambda/handler.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.72.0/datadog_lambda/metric.py` & `datadog_lambda-4.73.0/datadog_lambda/metric.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.72.0/datadog_lambda/patch.py` & `datadog_lambda-4.73.0/datadog_lambda/patch.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.72.0/datadog_lambda/tag_object.py` & `datadog_lambda-4.73.0/datadog_lambda/tag_object.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.72.0/datadog_lambda/tags.py` & `datadog_lambda-4.73.0/datadog_lambda/tags.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.72.0/datadog_lambda/thread_stats_writer.py` & `datadog_lambda-4.73.0/datadog_lambda/thread_stats_writer.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.72.0/datadog_lambda/tracing.py` & `datadog_lambda-4.73.0/datadog_lambda/tracing.py`

 * *Files 2% similar despite different names*

```diff
@@ -511,42 +511,39 @@
     trace context may already exist, and it should be used. Otherwise, use the
     current X-Ray trace entity, or the dd-trace-py context if DD_TRACE_ENABLED is true.
 
     Most of widely-used HTTP clients are patched to inject the context
     automatically, but this function can be used to manually inject the trace
     context to an outgoing request.
     """
-    global dd_trace_context
+    if dd_tracing_enabled:
+        dd_trace_py_context = _get_dd_trace_py_context()
+        if dd_trace_py_context is not None:
+            return _context_obj_to_headers(dd_trace_py_context)
 
-    context = None
-    xray_context = None
+    global dd_trace_context
 
     try:
         xray_context = _get_xray_trace_context()  # xray (sub)segment
     except Exception as e:
         logger.debug(
             "get_dd_trace_context couldn't read from segment from x-ray, with error %s"
             % e
         )
+    if not xray_context:
+        return {}
 
-    if xray_context and not dd_trace_context:
-        context = xray_context
-    elif xray_context and dd_trace_context:
-        context = dd_trace_context.copy()
-        context["parent-id"] = xray_context.get("parent-id")
-        logger.debug(
-            "Set parent id from xray trace context: %s", context.get("parent-id")
-        )
+    if not dd_trace_context:
+        return _context_obj_to_headers(xray_context)
 
-    if dd_tracing_enabled:
-        dd_trace_py_context = _get_dd_trace_py_context()
-        if dd_trace_py_context is not None:
-            context = dd_trace_py_context
+    context = dd_trace_context.copy()
+    context["parent-id"] = xray_context.get("parent-id")
+    logger.debug("Set parent id from xray trace context: %s", context.get("parent-id"))
 
-    return _context_obj_to_headers(context) if context is not None else {}
+    return _context_obj_to_headers(context)
 
 
 def set_correlation_ids():
     """
     Create a dummy span, and overrides its trace_id and span_id, to make
     ddtrace.helpers.get_log_correlation_context() return a dict containing the correct ids for both
     auto and manual log correlations.
@@ -557,14 +554,16 @@
         logger.debug("set_correlation_ids is only supported in LambdaContext")
         return
     if dd_tracing_enabled:
         logger.debug("using ddtrace implementation for spans")
         return
 
     context = get_dd_trace_context()
+    if not context:
+        return
 
     span = tracer.trace("dummy.span")
     span.trace_id = int(context[TraceHeader.TRACE_ID])
     span.span_id = int(context[TraceHeader.PARENT_ID])
 
     logger.debug("correlation ids set")
```

### Comparing `datadog_lambda-4.72.0/datadog_lambda/trigger.py` & `datadog_lambda-4.73.0/datadog_lambda/trigger.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.72.0/datadog_lambda/wrapper.py` & `datadog_lambda-4.73.0/datadog_lambda/wrapper.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.72.0/datadog_lambda/xray.py` & `datadog_lambda-4.73.0/datadog_lambda/xray.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.72.0/pyproject.toml` & `datadog_lambda-4.73.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datadog_lambda"
-version = "4.72.0"
+version = "4.73.0"
 description = "The Datadog AWS Lambda Library"
 authors = ["Datadog, Inc. <dev@datadoghq.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/DataDog/datadog-lambda-python"
 keywords = [
     "datadog",
@@ -23,14 +23,15 @@
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.7.0,<4"
 datadog = ">=0.41.0,<1.0.0"
 wrapt = "^1.11.2"
 ddtrace = "^1.6.4"
+urllib3 = "<2.0.0"
 importlib_metadata = {version = "^1.0", python = "<3.8"}
 boto3 = { version = "^1.10.33", optional = true }
 typing_extensions = {version = "^4.0", python = "<3.8"}
 requests = { version ="^2.22.0", optional = true }
 nose2 = { version= "^0.9.1", optional = true }
 flake8 = { version = "^3.7.9", optional = true }
 httpretty = {version = "^0.9.7", optional = true }
```

### Comparing `datadog_lambda-4.72.0/setup.py` & `datadog_lambda-4.73.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,86 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: datadog-lambda
+Version: 4.73.0
+Summary: The Datadog AWS Lambda Library
+Home-page: https://github.com/DataDog/datadog-lambda-python
+License: Apache-2.0
+Keywords: datadog,aws,lambda,layer
+Author: Datadog, Inc.
+Author-email: dev@datadoghq.com
+Requires-Python: >=3.7.0,<4
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: dev
+Requires-Dist: boto3 (>=1.10.33,<2.0.0) ; extra == "dev"
+Requires-Dist: datadog (>=0.41.0,<1.0.0)
+Requires-Dist: ddtrace (>=1.6.4,<2.0.0)
+Requires-Dist: flake8 (>=3.7.9,<4.0.0) ; extra == "dev"
+Requires-Dist: httpretty (>=0.9.7,<0.10.0) ; extra == "dev"
+Requires-Dist: importlib_metadata (>=1.0,<2.0) ; python_version < "3.8"
+Requires-Dist: nose2 (>=0.9.1,<0.10.0) ; extra == "dev"
+Requires-Dist: requests (>=2.22.0,<3.0.0) ; extra == "dev"
+Requires-Dist: typing_extensions (>=4.0,<5.0) ; python_version < "3.8"
+Requires-Dist: urllib3 (<2.0.0)
+Requires-Dist: wrapt (>=1.11.2,<2.0.0)
+Project-URL: Repository, https://github.com/DataDog/datadog-lambda-python
+Description-Content-Type: text/markdown
 
-packages = \
-['datadog_lambda']
+# datadog-lambda-python
 
-package_data = \
-{'': ['*']}
+![build](https://github.com/DataDog/datadog-lambda-python/workflows/build/badge.svg)
+[![PyPI](https://img.shields.io/pypi/v/datadog-lambda)](https://pypi.org/project/datadog-lambda/)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/datadog-lambda)
+[![Slack](https://chat.datadoghq.com/badge.svg?bg=632CA6)](https://chat.datadoghq.com/)
+[![License](https://img.shields.io/badge/license-Apache--2.0-blue)](https://github.com/DataDog/datadog-lambda-python/blob/main/LICENSE)
 
-install_requires = \
-['datadog>=0.41.0,<1.0.0', 'ddtrace>=1.6.4,<2.0.0', 'wrapt>=1.11.2,<2.0.0']
-
-extras_require = \
-{':python_version < "3.8"': ['importlib_metadata>=1.0,<2.0',
-                             'typing_extensions>=4.0,<5.0'],
- 'dev': ['boto3>=1.10.33,<2.0.0',
-         'requests>=2.22.0,<3.0.0',
-         'nose2>=0.9.1,<0.10.0',
-         'flake8>=3.7.9,<4.0.0',
-         'httpretty>=0.9.7,<0.10.0']}
-
-setup_kwargs = {
-    'name': 'datadog-lambda',
-    'version': '4.72.0',
-    'description': 'The Datadog AWS Lambda Library',
-    'long_description': "# datadog-lambda-python\n\n![build](https://github.com/DataDog/datadog-lambda-python/workflows/build/badge.svg)\n[![PyPI](https://img.shields.io/pypi/v/datadog-lambda)](https://pypi.org/project/datadog-lambda/)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/datadog-lambda)\n[![Slack](https://chat.datadoghq.com/badge.svg?bg=632CA6)](https://chat.datadoghq.com/)\n[![License](https://img.shields.io/badge/license-Apache--2.0-blue)](https://github.com/DataDog/datadog-lambda-python/blob/main/LICENSE)\n\nDatadog Lambda Library for Python (3.7, 3.8, 3.9, and 3.10) enables [enhanced Lambda metrics](https://docs.datadoghq.com/serverless/enhanced_lambda_metrics), [distributed tracing](https://docs.datadoghq.com/serverless/distributed_tracing), and [custom metric submission](https://docs.datadoghq.com/serverless/custom_metrics) from AWS Lambda functions.\n\n## Installation\n\nFollow the [installation instructions](https://docs.datadoghq.com/serverless/installation/python/), and view your function's enhanced metrics, traces and logs in Datadog.\n\n## Configuration\n\nFollow the [configuration instructions](https://docs.datadoghq.com/serverless/configuration) to tag your telemetry, capture request/response payloads, filter or scrub sensitive information from logs or traces, and more.\n\n## Opening Issues\n\nIf you encounter a bug with this package, we want to hear about it. Before opening a new issue, search the existing issues to avoid duplicates.\n\nWhen opening an issue, include the Datadog Lambda Library version, Python version, and stack trace if available. In addition, include the steps to reproduce when appropriate.\n\nYou can also open an issue for a feature request.\n\n## Lambda Profiling Beta\n\nDatadog's [Continuous Profiler](https://www.datadoghq.com/product/code-profiling/) is now available in beta for Python in version 4.62.0 and layer version 62 and above. This optional feature is enabled by setting the `DD_PROFILING_ENABLED` environment variable to `true`. During the beta period, profiling is available at no additional cost.\n\nThe Continuous Profiler works by spawning a thread which periodically wakes up and takes a snapshot of the CPU and Heap of all running python code. This can include the profiler itself. If you want the Profiler to ignore itself, set `DD_PROFILING_IGNORE_PROFILER` to `true`.\n\n## Major Version Notes\n\n### 4.x / Layer version 61+\n\n- Python3.6 support has been [deprecated](https://docs.aws.amazon.com/lambda/latest/dg/lambda-runtimes.html) by AWS, and support removed from this library.\n- `dd-trace` upgraded from 0.61 to 1.4, full release notes are available [here](https://ddtrace.readthedocs.io/en/stable/release_notes.html#v1-0-0)\n  - `get_correlation_ids()` has been changed to `get_log_correlation_context()`, which now returns a dictionary containing the active `span_id`, `trace_id`, as well as `service` and `env`.\n\n## Contributing\n\nIf you find an issue with this package and have a fix, please feel free to open a pull request following the [procedures](CONTRIBUTING.md).\n\n## Community\n\nFor product feedback and questions, join the `#serverless` channel in the [Datadog community on Slack](https://chat.datadoghq.com/).\n\n## License\n\nUnless explicitly stated otherwise all files in this repository are licensed under the Apache License Version 2.0.\n\nThis product includes software developed at Datadog (https://www.datadoghq.com/). Copyright 2019 Datadog, Inc.\n",
-    'author': 'Datadog, Inc.',
-    'author_email': 'dev@datadoghq.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/DataDog/datadog-lambda-python',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.7.0,<4',
-}
+Datadog Lambda Library for Python (3.7, 3.8, 3.9, and 3.10) enables [enhanced Lambda metrics](https://docs.datadoghq.com/serverless/enhanced_lambda_metrics), [distributed tracing](https://docs.datadoghq.com/serverless/distributed_tracing), and [custom metric submission](https://docs.datadoghq.com/serverless/custom_metrics) from AWS Lambda functions.
 
+## Installation
+
+Follow the [installation instructions](https://docs.datadoghq.com/serverless/installation/python/), and view your function's enhanced metrics, traces and logs in Datadog.
+
+## Configuration
+
+Follow the [configuration instructions](https://docs.datadoghq.com/serverless/configuration) to tag your telemetry, capture request/response payloads, filter or scrub sensitive information from logs or traces, and more.
+
+## Opening Issues
+
+If you encounter a bug with this package, we want to hear about it. Before opening a new issue, search the existing issues to avoid duplicates.
+
+When opening an issue, include the Datadog Lambda Library version, Python version, and stack trace if available. In addition, include the steps to reproduce when appropriate.
+
+You can also open an issue for a feature request.
+
+## Lambda Profiling Beta
+
+Datadog's [Continuous Profiler](https://www.datadoghq.com/product/code-profiling/) is now available in beta for Python in version 4.62.0 and layer version 62 and above. This optional feature is enabled by setting the `DD_PROFILING_ENABLED` environment variable to `true`. During the beta period, profiling is available at no additional cost.
+
+The Continuous Profiler works by spawning a thread which periodically wakes up and takes a snapshot of the CPU and Heap of all running python code. This can include the profiler itself. If you want the Profiler to ignore itself, set `DD_PROFILING_IGNORE_PROFILER` to `true`.
+
+## Major Version Notes
+
+### 4.x / Layer version 61+
+
+- Python3.6 support has been [deprecated](https://docs.aws.amazon.com/lambda/latest/dg/lambda-runtimes.html) by AWS, and support removed from this library.
+- `dd-trace` upgraded from 0.61 to 1.4, full release notes are available [here](https://ddtrace.readthedocs.io/en/stable/release_notes.html#v1-0-0)
+  - `get_correlation_ids()` has been changed to `get_log_correlation_context()`, which now returns a dictionary containing the active `span_id`, `trace_id`, as well as `service` and `env`.
+
+## Contributing
+
+If you find an issue with this package and have a fix, please feel free to open a pull request following the [procedures](CONTRIBUTING.md).
+
+## Community
+
+For product feedback and questions, join the `#serverless` channel in the [Datadog community on Slack](https://chat.datadoghq.com/).
+
+## License
+
+Unless explicitly stated otherwise all files in this repository are licensed under the Apache License Version 2.0.
+
+This product includes software developed at Datadog (https://www.datadoghq.com/). Copyright 2019 Datadog, Inc.
 
-setup(**setup_kwargs)
```

