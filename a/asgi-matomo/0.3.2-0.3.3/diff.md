# Comparing `tmp/asgi_matomo-0.3.2.tar.gz` & `tmp/asgi_matomo-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asgi_matomo-0.3.2.tar", max compression
+gzip compressed data, was "asgi_matomo-0.3.3.tar", max compression
```

## Comparing `asgi_matomo-0.3.2.tar` & `asgi_matomo-0.3.3.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1069 2023-05-23 11:34:01.134242 asgi_matomo-0.3.2/LICENSE
--rw-r--r--   0        0        0     5278 2023-05-23 11:34:01.134242 asgi_matomo-0.3.2/README.md
--rw-r--r--   0        0        0      186 2023-05-23 11:34:01.134242 asgi_matomo-0.3.2/asgi_matomo/__init__.py
--rw-r--r--   0        0        0     9799 2023-05-23 11:34:01.134242 asgi_matomo-0.3.2/asgi_matomo/middleware.py
--rw-r--r--   0        0        0     1024 2023-05-23 11:34:01.134242 asgi_matomo-0.3.2/asgi_matomo/trackers.py
--rw-r--r--   0        0        0      879 2023-05-23 11:34:01.134242 asgi_matomo-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     6163 1970-01-01 00:00:00.000000 asgi_matomo-0.3.2/setup.py
--rw-r--r--   0        0        0     6011 1970-01-01 00:00:00.000000 asgi_matomo-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-24 11:54:16.478030 asgi_matomo-0.3.3/LICENSE
+-rw-r--r--   0        0        0     5278 2023-05-24 11:54:16.478030 asgi_matomo-0.3.3/README.md
+-rw-r--r--   0        0        0      186 2023-05-24 11:54:16.478030 asgi_matomo-0.3.3/asgi_matomo/__init__.py
+-rw-r--r--   0        0        0     9799 2023-05-24 11:54:16.478030 asgi_matomo-0.3.3/asgi_matomo/middleware.py
+-rw-r--r--   0        0        0        0 2023-05-24 11:54:16.478030 asgi_matomo-0.3.3/asgi_matomo/py.typed
+-rw-r--r--   0        0        0     1024 2023-05-24 11:54:16.478030 asgi_matomo-0.3.3/asgi_matomo/trackers.py
+-rw-r--r--   0        0        0      879 2023-05-24 11:54:16.478030 asgi_matomo-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     6163 1970-01-01 00:00:00.000000 asgi_matomo-0.3.3/setup.py
+-rw-r--r--   0        0        0     6011 1970-01-01 00:00:00.000000 asgi_matomo-0.3.3/PKG-INFO
```

### Comparing `asgi_matomo-0.3.2/LICENSE` & `asgi_matomo-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `asgi_matomo-0.3.2/README.md` & `asgi_matomo-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `asgi_matomo-0.3.2/asgi_matomo/middleware.py` & `asgi_matomo-0.3.3/asgi_matomo/middleware.py`

 * *Files identical despite different names*

### Comparing `asgi_matomo-0.3.2/asgi_matomo/trackers.py` & `asgi_matomo-0.3.3/asgi_matomo/trackers.py`

 * *Files identical despite different names*

### Comparing `asgi_matomo-0.3.2/pyproject.toml` & `asgi_matomo-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asgi-matomo"
-version = "0.3.2"
+version = "0.3.3"
 description = "Middleware for tracking ASGI reqeusts with Matomo"
 authors = ["Kristoffer Andersson <kristoffer.andersson@gu.se>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://spraakbanken.gu.se"
 repository = "https://github.com/spraakbanken/asgi-matomo"
 packages = [{include = "asgi_matomo"}]
```

### Comparing `asgi_matomo-0.3.2/setup.py` & `asgi_matomo-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['asgiref>=3.6.0,<4.0.0', 'httpx>=0.24.0,<0.25.0']
 
 setup_kwargs = {
     'name': 'asgi-matomo',
-    'version': '0.3.2',
+    'version': '0.3.3',
     'description': 'Middleware for tracking ASGI reqeusts with Matomo',
     'long_description': '# asgi-matomo\n[![Packaging status](https://img.shields.io/pypi/v/asgi-matomo?color=%2334D058&label=pypi%20package)](https://pypi.org/project/asgi-matomo)\n[![CI](https://github.com/spraakbanken/asgi-matomo/workflows/CI/badge.svg)](https://github.com/spraakbanken/asgi-matomo/actions?query=workflow%3ACI)\n[![codecov](https://codecov.io/gh/spraakbanken/asgi-matomo/branch/main/graph/badge.svg?token=MRJZVCJQF5)](https://codecov.io/gh/spraakbanken/asgi-matomo)\n\nTracking requests with Matomo from ASGI apps.\n\n`MatomoMiddleware` adds tracking of all requests to Matomo to ASGI applications (Starlette, FastAPI, Quart, etc.). The intended usage is for api tracking (backends).\n\n**Note** If you serve HTML (directly or by templates), it is suggested to track those parts through Matomo\'s javascript tracking.\n\n**Installation**\n\n```bash\npip install asgi-matomo\n```\n\n## What is tracked\n\nCurrently this middleware tracks:\n- `url`\n- `ua`: user_agent\n- `gt_ms`: mesaured as the time before and after this middleware call next in the asgi stack.\n- `send_image=0` for performance issues\n- `cvar` with at least `http_status_code` and `http_method` set.\n- `lang` if `accept-lang` is set\n- `cip` client ip, **requires** `access_token` to be given.\n- `action_name` that defaults to path, but can be specified.\n\nYou can also pass variable to track by adding an `asgi_matomo`  dict in the `state` dict of the ASGI `scope`:\n```python\nscope = {\n  "state": {\n    "asgi_matomo": {\n      "e_a": "Playing",\n      "cvar": {\n        "your": "custom",\n        "data": "here",\n      }\n    }\n  }\n}\n```\n\nThe keys of the `asgi_matomo` dict is expected to be valid parameter for the [Matomo HTTP Tracking API](https://developer.matomo.org/api-reference/tracking-api). `cvar` is serialized with the standard `json` lib.\n\nYou can also track time spent on different tasks with `trackers.PerfMsTracker`.\n```python\nimport asyncio\nfrom starlette.applications import Starlette\nfrom starlette.responses import JSONResponse\nfrom starlette.routing import Route\nfrom starlette.middleware import Middleware\n\nfrom asgi_matomo import MatomoMiddleware\nfrom asgi_matomo.trackers import PerfMsTracker\n\nasync def homepage(request):\n    async with PerfMsTracker(scope=request.scope, key="pf_srv"):\n        # fetch/compute data\n        await asyncio.sleep(1)\n        data = {"data": "a"*4000}\n    return JSONResponse(data)\n\napp = Starlette(\n  routes=[Route("/", homepage)],\n  middleware=[\n    Middleware(\n      MatomoMiddleware,\n      matomo_url="YOUR MATOMO TRACKING URL",\n      idsite=12345, # your service tracking id\n  )],\n)\n```\n\n## Examples\n\n### Starlette\n\n```python\nfrom starlette.applications import Starlette\nfrom starlette.responses import JSONResponse\nfrom starlette.routing import Route\nfrom starlette.middleware import Middleware\n\nfrom asgi_matomo import MatomoMiddleware\n\nasync def homepage(request):\n    return JSONResponse({"data": "a" * 4000})\n\napp = Starlette(\n  routes=[Route("/", homepage)],\n  middleware=[\n    Middleware(\n      MatomoMiddleware,\n      matomo_url="YOUR MATOMO TRACKING URL",\n      idsite=12345, # your service tracking id\n  )],\n)\n```\n\n### FastAPI\n\n```python\nfrom fastapi import FastAPI\nfrom asgi_matomo import MatomoMiddleware\n\napp = FastAPI()\napp.add_middleware(\n  BrotliMiddleware,\n  matomo_url="YOUR MATOMO TRACKING URL",\n  idsite=12345, # your service tracking id\n)\n\n@app.get("/")\ndef home() -> dict:\n    return {"data": "a" * 4000}\n```\n\n## API Reference\n\n**Overview**\n\n```python\napp.add_middleware(\n  MatomoMiddleware,\n  matomo_url="YOUR MATOMO TRACKING URL",\n  idsite=12345, # your service tracking id\n  access_token="SECRETTOKEN",\n  assume_https=True,\n  exclude_paths=["/health"],\n  exclude_patterns=[".*/old.*"],\n  route_details={\n    "route": {\n      "action_name": "Name",\n    }\n  }\n)\n```\n\n**Parameters**:\n\n- **(Required)** `matomo_url`: The URL to make your tracking calls to.\n- **(Required)** `idsite`: The tracking id for your service.\n- _(Optional)_ `access_token`: Access token for Matomo. If this is set `cip` is also tracked. Required for tracking some data.\n- _(Optional)_ `assume_https`: If `True`, set tracked url scheme to `https`, useful when running behind a proxy. Defaults to `True`.\n- _(Optional)_ `exclude_paths`: A list of paths to exclude, only excludes path that is equal to a path in this list. These are tried before `exclude_patterns`. Defaults to `None`.\n- _(Optional)_ `exclude_patterns`: A list of regex patterns that are compiled, and then exclude a path from tracking if any pattern match. Defaults to `None`.\nThese are tried after `exclude_paths`.\n- _(Optional)_ `route_details`: A dict with custom route-specific tracking data. Defaults to `None`.\n\n\n**Notes**:\n\n- Currently only some parts [Matomo Tracking HTTP API](https://developer.matomo.org/api-reference/tracking-api) is supported.\n\n## Ideas for further work:\n- [x] _filtering tracked of urls_\n- [x] _custom extraction of tracked data_\n\n\nThis project keeps a [changelog](https://github.com/spraakbanken/asgi-matomo/CHANGELOG.md).\n\n# Releas Notes\n\n## Latest Changes\n\n## [0.3.2] - 2023-05-23\n\n* feat: add PerfMsTracker. PR [#10](https://github.com/spraakbanken/asgi-matomo/pull/10) by [@kod-kristoff](https://github.com/kod-kristoff).\n\n## [0.3.0] - 2023-05-22\n### Added\n\n- Allow setting route-details\n\n',
     'author': 'Kristoffer Andersson',
     'author_email': 'kristoffer.andersson@gu.se',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://spraakbanken.gu.se',
```

### Comparing `asgi_matomo-0.3.2/PKG-INFO` & `asgi_matomo-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asgi-matomo
-Version: 0.3.2
+Version: 0.3.3
 Summary: Middleware for tracking ASGI reqeusts with Matomo
 Home-page: https://spraakbanken.gu.se
 License: MIT
 Author: Kristoffer Andersson
 Author-email: kristoffer.andersson@gu.se
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

