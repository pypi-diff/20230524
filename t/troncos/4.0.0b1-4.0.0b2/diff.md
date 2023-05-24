# Comparing `tmp/troncos-4.0.0b1.tar.gz` & `tmp/troncos-4.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "troncos-4.0.0b1.tar", max compression
+gzip compressed data, was "troncos-4.0.0b2.tar", max compression
```

## Comparing `troncos-4.0.0b1.tar` & `troncos-4.0.0b2.tar`

### file list

```diff
@@ -1,30 +1,32 @@
--rw-r--r--   0        0        0     1077 2023-05-23 13:42:18.030371 troncos-4.0.0b1/LICENSE
--rw-r--r--   0        0        0     6047 2023-05-23 13:42:18.030371 troncos-4.0.0b1/README.md
--rw-r--r--   0        0        0     2195 2023-05-23 13:42:18.030371 troncos-4.0.0b1/pyproject.toml
--rw-r--r--   0        0        0      291 2023-05-23 13:42:18.034371 troncos-4.0.0b1/troncos/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 13:42:18.034371 troncos-4.0.0b1/troncos/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 13:42:18.034371 troncos-4.0.0b1/troncos/contrib/asgi/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 13:42:18.034371 troncos-4.0.0b1/troncos/contrib/asgi/logging/__init__.py
--rw-r--r--   0        0        0     2606 2023-05-23 13:42:18.034371 troncos-4.0.0b1/troncos/contrib/asgi/logging/middleware.py
--rw-r--r--   0        0        0        0 2023-05-23 13:42:18.034371 troncos-4.0.0b1/troncos/contrib/asgi/profiling/__init__.py
--rw-r--r--   0        0        0      576 2023-05-23 13:42:18.034371 troncos-4.0.0b1/troncos/contrib/asgi/profiling/app.py
--rw-r--r--   0        0        0        0 2023-05-23 13:42:18.034371 troncos-4.0.0b1/troncos/contrib/django/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 13:42:18.034371 troncos-4.0.0b1/troncos/contrib/django/profiling/__init__.py
--rw-r--r--   0        0        0      265 2023-05-23 13:42:18.034371 troncos-4.0.0b1/troncos/contrib/django/profiling/views.py
--rw-r--r--   0        0        0        0 2023-05-23 13:42:18.034371 troncos-4.0.0b1/troncos/contrib/starlette/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 13:42:18.034371 troncos-4.0.0b1/troncos/contrib/starlette/profiling/__init__.py
--rw-r--r--   0        0        0      291 2023-05-23 13:42:18.034371 troncos-4.0.0b1/troncos/contrib/starlette/profiling/views.py
--rw-r--r--   0        0        0        0 2023-05-23 13:42:18.034371 troncos-4.0.0b1/troncos/contrib/structlog/__init__.py
--rw-r--r--   0        0        0      705 2023-05-23 13:42:18.034371 troncos-4.0.0b1/troncos/contrib/structlog/processors.py
--rw-r--r--   0        0        0        0 2023-05-23 13:42:18.034371 troncos-4.0.0b1/troncos/profiling/__init__.py
--rw-r--r--   0        0        0      192 2023-05-23 13:42:18.034371 troncos-4.0.0b1/troncos/profiling/auto.py
--rw-r--r--   0        0        0        0 2023-05-23 13:42:18.034371 troncos-4.0.0b1/troncos/profiling/bootstrap/__init__.py
--rw-r--r--   0        0        0      439 2023-05-23 13:42:18.034371 troncos-4.0.0b1/troncos/profiling/bootstrap/profile.py
--rw-r--r--   0        0        0      343 2023-05-23 13:42:18.034371 troncos-4.0.0b1/troncos/profiling/bootstrap/start.py
--rw-r--r--   0        0        0     1814 2023-05-23 13:42:18.034371 troncos-4.0.0b1/troncos/profiling/profiler.py
--rw-r--r--   0        0        0        0 2023-05-23 13:42:18.034371 troncos-4.0.0b1/troncos/py.typed
--rw-r--r--   0        0        0      570 2023-05-23 13:42:18.034371 troncos-4.0.0b1/troncos/tracing/__init__.py
--rw-r--r--   0        0        0     1298 2023-05-23 13:42:18.034371 troncos-4.0.0b1/troncos/tracing/_otel.py
--rw-r--r--   0        0        0     4062 2023-05-23 13:42:18.034371 troncos-4.0.0b1/troncos/tracing/_span.py
--rw-r--r--   0        0        0     1672 2023-05-23 13:42:18.034371 troncos-4.0.0b1/troncos/tracing/_writer.py
--rw-r--r--   0        0        0     6887 1970-01-01 00:00:00.000000 troncos-4.0.0b1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-24 09:45:35.272978 troncos-4.0.0b2/LICENSE
+-rw-r--r--   0        0        0     6282 2023-05-24 09:45:35.272978 troncos-4.0.0b2/README.md
+-rw-r--r--   0        0        0     2220 2023-05-24 09:45:35.272978 troncos-4.0.0b2/pyproject.toml
+-rw-r--r--   0        0        0      291 2023-05-24 09:45:35.272978 troncos-4.0.0b2/troncos/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 09:45:35.272978 troncos-4.0.0b2/troncos/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 09:45:35.272978 troncos-4.0.0b2/troncos/contrib/asgi/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 09:45:35.272978 troncos-4.0.0b2/troncos/contrib/asgi/logging/__init__.py
+-rw-r--r--   0        0        0     5042 2023-05-24 09:45:35.272978 troncos-4.0.0b2/troncos/contrib/asgi/logging/middleware.py
+-rw-r--r--   0        0        0        0 2023-05-24 09:45:35.272978 troncos-4.0.0b2/troncos/contrib/asgi/profiling/__init__.py
+-rw-r--r--   0        0        0      576 2023-05-24 09:45:35.272978 troncos-4.0.0b2/troncos/contrib/asgi/profiling/app.py
+-rw-r--r--   0        0        0        0 2023-05-24 09:45:35.272978 troncos-4.0.0b2/troncos/contrib/django/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 09:45:35.272978 troncos-4.0.0b2/troncos/contrib/django/logging/__init__.py
+-rw-r--r--   0        0        0     2318 2023-05-24 09:45:35.272978 troncos-4.0.0b2/troncos/contrib/django/logging/middleware.py
+-rw-r--r--   0        0        0        0 2023-05-24 09:45:35.272978 troncos-4.0.0b2/troncos/contrib/django/profiling/__init__.py
+-rw-r--r--   0        0        0      265 2023-05-24 09:45:35.272978 troncos-4.0.0b2/troncos/contrib/django/profiling/views.py
+-rw-r--r--   0        0        0        0 2023-05-24 09:45:35.272978 troncos-4.0.0b2/troncos/contrib/starlette/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 09:45:35.272978 troncos-4.0.0b2/troncos/contrib/starlette/profiling/__init__.py
+-rw-r--r--   0        0        0      291 2023-05-24 09:45:35.272978 troncos-4.0.0b2/troncos/contrib/starlette/profiling/views.py
+-rw-r--r--   0        0        0        0 2023-05-24 09:45:35.272978 troncos-4.0.0b2/troncos/contrib/structlog/__init__.py
+-rw-r--r--   0        0        0      705 2023-05-24 09:45:35.272978 troncos-4.0.0b2/troncos/contrib/structlog/processors.py
+-rw-r--r--   0        0        0        0 2023-05-24 09:45:35.272978 troncos-4.0.0b2/troncos/profiling/__init__.py
+-rw-r--r--   0        0        0      192 2023-05-24 09:45:35.272978 troncos-4.0.0b2/troncos/profiling/auto.py
+-rw-r--r--   0        0        0        0 2023-05-24 09:45:35.272978 troncos-4.0.0b2/troncos/profiling/bootstrap/__init__.py
+-rw-r--r--   0        0        0      439 2023-05-24 09:45:35.272978 troncos-4.0.0b2/troncos/profiling/bootstrap/profile.py
+-rw-r--r--   0        0        0      343 2023-05-24 09:45:35.272978 troncos-4.0.0b2/troncos/profiling/bootstrap/start.py
+-rw-r--r--   0        0        0     1814 2023-05-24 09:45:35.272978 troncos-4.0.0b2/troncos/profiling/profiler.py
+-rw-r--r--   0        0        0        0 2023-05-24 09:45:35.272978 troncos-4.0.0b2/troncos/py.typed
+-rw-r--r--   0        0        0      570 2023-05-24 09:45:35.272978 troncos-4.0.0b2/troncos/tracing/__init__.py
+-rw-r--r--   0        0        0     1298 2023-05-24 09:45:35.272978 troncos-4.0.0b2/troncos/tracing/_otel.py
+-rw-r--r--   0        0        0     4062 2023-05-24 09:45:35.272978 troncos-4.0.0b2/troncos/tracing/_span.py
+-rw-r--r--   0        0        0     1672 2023-05-24 09:45:35.272978 troncos-4.0.0b2/troncos/tracing/_writer.py
+-rw-r--r--   0        0        0     7169 1970-01-01 00:00:00.000000 troncos-4.0.0b2/PKG-INFO
```

### Comparing `troncos-4.0.0b1/LICENSE` & `troncos-4.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b1/README.md` & `troncos-4.0.0b2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -132,14 +132,26 @@
 from starlette.applications import Starlette
 
 from troncos.contrib.asgi.logging.middleware import AsgiLoggingMiddleware
 
 application = AsgiLoggingMiddleware(Starlette())
 ```
 
+#### Django middleware
+
+Log Django requests. This is not needed if you run Django with ASGI and use the
+ASGI middleware.
+
+```python
+MIDDLEWARE = [
+    "troncos.contrib.django.logging.middleware.DjangoLoggingMiddleware",
+    ...
+]
+```
+
 ## Profiling
 
 ### Enabling the profiler
 
 Start the profiler by importing the profiler module early in your application. This is
 typically done in `settings.py` of you want to profile a Django application, or in `__init__.py`
 in the root project package.
```

#### html2text {}

```diff
@@ -40,16 +40,19 @@
 application Finding relevant traces in Grafana can be difficult. One way to
 make finding the relevant traces easier it to log every major action in your
 application. This typically means logging every incoming HTTP request to your
 server or every task executed by your Celery worker. The structlog processor
 above needs to be enabled before logging your major actions is relevant. ####
 ASGI middleware Log ASGI requests. ```python from starlette.applications import
 Starlette from troncos.contrib.asgi.logging.middleware import
-AsgiLoggingMiddleware application = AsgiLoggingMiddleware(Starlette()) ``` ##
-Profiling ### Enabling the profiler Start the profiler by importing the
+AsgiLoggingMiddleware application = AsgiLoggingMiddleware(Starlette()) ``` ####
+Django middleware Log Django requests. This is not needed if you run Django
+with ASGI and use the ASGI middleware. ```python MIDDLEWARE =
+[ "troncos.contrib.django.logging.middleware.DjangoLoggingMiddleware", ... ]
+``` ## Profiling ### Enabling the profiler Start the profiler by importing the
 profiler module early in your application. This is typically done in
 `settings.py` of you want to profile a Django application, or in `__init__.py`
 in the root project package. ```python import troncos.profiling.auto ``` ###
 Setup profile endpoint Use one of the methods bellow based on your selected
 framework. #### Django Add the profile view to the url config. ```python from
 django.urls import path from troncos.contrib.django.profiling.views import
 profiling_view urlpatterns = [ path("/debug/pprof", profiling_view,
```

### Comparing `troncos-4.0.0b1/pyproject.toml` & `troncos-4.0.0b2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "troncos"
-version = "4.0.0b1"
+version = "4.0.0b2"
 description = "Collection of Python logging, tracing and profiling tools"
 authors = [
     "Guðmundur Björn Birkisson <gudmundur.birkisson@oda.com>",
     "Karl Fredrik Haugland <karlfredrik.haugland@oda.com>",
     "Eirik Martiniussen Sylliaas <eirik.sylliaas@oda.com>",
 ]
 license = "MIT"
@@ -15,14 +15,15 @@
 keywords = ["logs", "traces", "opentelemetry"]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
 ddtrace = "1.13.3"
 opentelemetry-sdk = "1.17.0"
 opentelemetry-exporter-otlp-proto-http = "1.17.0"
+python-ipware = "^0.9.0"
 
 [tool.poetry.group.dev.dependencies]
 isort = "^5.12.0"
 black = "^23.1.0"
 flake8 = "^6.0.0"
 mypy = "^1.0.1"
 pytest = "^7.2.1"
```

### Comparing `troncos-4.0.0b1/troncos/contrib/asgi/profiling/app.py` & `troncos-4.0.0b2/troncos/contrib/asgi/profiling/app.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b1/troncos/contrib/structlog/processors.py` & `troncos-4.0.0b2/troncos/contrib/structlog/processors.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b1/troncos/profiling/profiler.py` & `troncos-4.0.0b2/troncos/profiling/profiler.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b1/troncos/tracing/__init__.py` & `troncos-4.0.0b2/troncos/tracing/__init__.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b1/troncos/tracing/_otel.py` & `troncos-4.0.0b2/troncos/tracing/_otel.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b1/troncos/tracing/_span.py` & `troncos-4.0.0b2/troncos/tracing/_span.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b1/troncos/tracing/_writer.py` & `troncos-4.0.0b2/troncos/tracing/_writer.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b1/PKG-INFO` & `troncos-4.0.0b2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: troncos
-Version: 4.0.0b1
+Version: 4.0.0b2
 Summary: Collection of Python logging, tracing and profiling tools
 Home-page: https://github.com/kolonialno/troncos
 License: MIT
 Keywords: logs,traces,opentelemetry
 Author: Guðmundur Björn Birkisson
 Author-email: gudmundur.birkisson@oda.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ddtrace (==1.13.3)
 Requires-Dist: opentelemetry-exporter-otlp-proto-http (==1.17.0)
 Requires-Dist: opentelemetry-sdk (==1.17.0)
+Requires-Dist: python-ipware (>=0.9.0,<0.10.0)
 Project-URL: Documentation, https://github.com/kolonialno/troncos
 Project-URL: Repository, https://github.com/kolonialno/troncos
 Description-Content-Type: text/markdown
 
 <h1 align="center" style="border-bottom: 0">
   🪵<br>
   Troncos <br/>
@@ -153,14 +154,26 @@
 from starlette.applications import Starlette
 
 from troncos.contrib.asgi.logging.middleware import AsgiLoggingMiddleware
 
 application = AsgiLoggingMiddleware(Starlette())
 ```
 
+#### Django middleware
+
+Log Django requests. This is not needed if you run Django with ASGI and use the
+ASGI middleware.
+
+```python
+MIDDLEWARE = [
+    "troncos.contrib.django.logging.middleware.DjangoLoggingMiddleware",
+    ...
+]
+```
+
 ## Profiling
 
 ### Enabling the profiler
 
 Start the profiler by importing the profiler module early in your application. This is
 typically done in `settings.py` of you want to profile a Django application, or in `__init__.py`
 in the root project package.
```

#### html2text {}

```diff
@@ -1,18 +1,19 @@
-Metadata-Version: 2.1 Name: troncos Version: 4.0.0b1 Summary: Collection of
+Metadata-Version: 2.1 Name: troncos Version: 4.0.0b2 Summary: Collection of
 Python logging, tracing and profiling tools Home-page: https://github.com/
 kolonialno/troncos License: MIT Keywords: logs,traces,opentelemetry Author:
 GuÃ°mundur BjÃ¶rn Birkisson Author-email: gudmundur.birkisson@oda.com Requires-
 Python: >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ddtrace (==1.13.3) Requires-Dist: opentelemetry-exporter-otlp-
-proto-http (==1.17.0) Requires-Dist: opentelemetry-sdk (==1.17.0) Project-URL:
-Documentation, https://github.com/kolonialno/troncos Project-URL: Repository,
-https://github.com/kolonialno/troncos Description-Content-Type: text/markdown
+proto-http (==1.17.0) Requires-Dist: opentelemetry-sdk (==1.17.0) Requires-
+Dist: python-ipware (>=0.9.0,<0.10.0) Project-URL: Documentation, https://
+github.com/kolonialno/troncos Project-URL: Repository, https://github.com/
+kolonialno/troncos Description-Content-Type: text/markdown
                                   ****** ðªµ
                                    Troncos
                                      ******
           Collection of Python logging, tracing and profiling tools
        [CI_status] [https://img.shields.io/pypi/v/troncos.svg] [https://
 img.shields.io/pypi/pyversions/troncos] [https://img.shields.io/github/license/
                             kolonialno/troncos.svg]
@@ -51,16 +52,19 @@
 application Finding relevant traces in Grafana can be difficult. One way to
 make finding the relevant traces easier it to log every major action in your
 application. This typically means logging every incoming HTTP request to your
 server or every task executed by your Celery worker. The structlog processor
 above needs to be enabled before logging your major actions is relevant. ####
 ASGI middleware Log ASGI requests. ```python from starlette.applications import
 Starlette from troncos.contrib.asgi.logging.middleware import
-AsgiLoggingMiddleware application = AsgiLoggingMiddleware(Starlette()) ``` ##
-Profiling ### Enabling the profiler Start the profiler by importing the
+AsgiLoggingMiddleware application = AsgiLoggingMiddleware(Starlette()) ``` ####
+Django middleware Log Django requests. This is not needed if you run Django
+with ASGI and use the ASGI middleware. ```python MIDDLEWARE =
+[ "troncos.contrib.django.logging.middleware.DjangoLoggingMiddleware", ... ]
+``` ## Profiling ### Enabling the profiler Start the profiler by importing the
 profiler module early in your application. This is typically done in
 `settings.py` of you want to profile a Django application, or in `__init__.py`
 in the root project package. ```python import troncos.profiling.auto ``` ###
 Setup profile endpoint Use one of the methods bellow based on your selected
 framework. #### Django Add the profile view to the url config. ```python from
 django.urls import path from troncos.contrib.django.profiling.views import
 profiling_view urlpatterns = [ path("/debug/pprof", profiling_view,
```

