# Comparing `tmp/serverhttpy-0.0.2.tar.gz` & `tmp/serverhttpy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serverhttpy-0.0.2.tar", last modified: Tue May 23 21:47:43 2023, max compression
+gzip compressed data, was "serverhttpy-0.0.3.tar", last modified: Tue May 23 22:03:02 2023, max compression
```

## Comparing `serverhttpy-0.0.2.tar` & `serverhttpy-0.0.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:47:43.397045 serverhttpy-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-23 21:47:43.397045 serverhttpy-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-23 21:47:32.000000 serverhttpy-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-23 21:47:32.000000 serverhttpy-0.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:47:43.393045 serverhttpy-0.0.2/serverhttpy/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-23 21:47:32.000000 serverhttpy-0.0.2/serverhttpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-23 21:47:32.000000 serverhttpy-0.0.2/serverhttpy/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:47:43.393045 serverhttpy-0.0.2/serverhttpy/enums/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 21:47:32.000000 serverhttpy-0.0.2/serverhttpy/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-23 21:47:32.000000 serverhttpy-0.0.2/serverhttpy/enums/http_method.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-23 21:47:32.000000 serverhttpy-0.0.2/serverhttpy/enums/status_code.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:47:43.393045 serverhttpy-0.0.2/serverhttpy/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-05-23 21:47:32.000000 serverhttpy-0.0.2/serverhttpy/examples/example_clients_managment.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-23 21:47:32.000000 serverhttpy-0.0.2/serverhttpy/examples/sample_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:47:43.397045 serverhttpy-0.0.2/serverhttpy/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 21:47:32.000000 serverhttpy-0.0.2/serverhttpy/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-23 21:47:32.000000 serverhttpy-0.0.2/serverhttpy/exceptions/invalid_header_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-23 21:47:32.000000 serverhttpy-0.0.2/serverhttpy/exceptions/invalid_path_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-23 21:47:32.000000 serverhttpy-0.0.2/serverhttpy/exceptions/invalid_query_param_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-23 21:47:32.000000 serverhttpy-0.0.2/serverhttpy/exceptions/invalid_request_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-23 21:47:32.000000 serverhttpy-0.0.2/serverhttpy/exceptions/no_action_registered_in_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-23 21:47:32.000000 serverhttpy-0.0.2/serverhttpy/exceptions/unsupported_method_specified.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:47:43.397045 serverhttpy-0.0.2/serverhttpy/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 21:47:32.000000 serverhttpy-0.0.2/serverhttpy/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-23 21:47:32.000000 serverhttpy-0.0.2/serverhttpy/models/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-23 21:47:32.000000 serverhttpy-0.0.2/serverhttpy/models/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-23 21:47:32.000000 serverhttpy-0.0.2/serverhttpy/models/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-23 21:47:32.000000 serverhttpy-0.0.2/serverhttpy/models/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-23 21:47:32.000000 serverhttpy-0.0.2/serverhttpy/models/uri.py
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-05-23 21:47:32.000000 serverhttpy-0.0.2/serverhttpy/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:47:43.393045 serverhttpy-0.0.2/serverhttpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-23 21:47:43.000000 serverhttpy-0.0.2/serverhttpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-23 21:47:43.000000 serverhttpy-0.0.2/serverhttpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 21:47:43.000000 serverhttpy-0.0.2/serverhttpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-23 21:47:43.000000 serverhttpy-0.0.2/serverhttpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 21:47:43.397045 serverhttpy-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-23 21:47:32.000000 serverhttpy-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:03:02.268815 serverhttpy-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-23 22:03:02.268815 serverhttpy-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-23 22:02:53.000000 serverhttpy-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-23 22:02:53.000000 serverhttpy-0.0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:03:02.268815 serverhttpy-0.0.3/serverhttpy/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-23 22:02:53.000000 serverhttpy-0.0.3/serverhttpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-23 22:02:53.000000 serverhttpy-0.0.3/serverhttpy/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:03:02.268815 serverhttpy-0.0.3/serverhttpy/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 22:02:53.000000 serverhttpy-0.0.3/serverhttpy/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-23 22:02:53.000000 serverhttpy-0.0.3/serverhttpy/enums/http_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-23 22:02:53.000000 serverhttpy-0.0.3/serverhttpy/enums/status_code.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:03:02.268815 serverhttpy-0.0.3/serverhttpy/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-05-23 22:02:53.000000 serverhttpy-0.0.3/serverhttpy/examples/example_clients_managment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-23 22:02:53.000000 serverhttpy-0.0.3/serverhttpy/examples/sample_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:03:02.268815 serverhttpy-0.0.3/serverhttpy/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 22:02:53.000000 serverhttpy-0.0.3/serverhttpy/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-23 22:02:53.000000 serverhttpy-0.0.3/serverhttpy/exceptions/invalid_header_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-23 22:02:53.000000 serverhttpy-0.0.3/serverhttpy/exceptions/invalid_path_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-23 22:02:53.000000 serverhttpy-0.0.3/serverhttpy/exceptions/invalid_query_param_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-23 22:02:53.000000 serverhttpy-0.0.3/serverhttpy/exceptions/invalid_request_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-23 22:02:53.000000 serverhttpy-0.0.3/serverhttpy/exceptions/no_action_registered_in_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-23 22:02:53.000000 serverhttpy-0.0.3/serverhttpy/exceptions/unsupported_method_specified.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:03:02.268815 serverhttpy-0.0.3/serverhttpy/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 22:02:53.000000 serverhttpy-0.0.3/serverhttpy/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-23 22:02:53.000000 serverhttpy-0.0.3/serverhttpy/models/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-23 22:02:53.000000 serverhttpy-0.0.3/serverhttpy/models/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-23 22:02:53.000000 serverhttpy-0.0.3/serverhttpy/models/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-23 22:02:53.000000 serverhttpy-0.0.3/serverhttpy/models/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-23 22:02:53.000000 serverhttpy-0.0.3/serverhttpy/models/uri.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-05-23 22:02:53.000000 serverhttpy-0.0.3/serverhttpy/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:03:02.268815 serverhttpy-0.0.3/serverhttpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-23 22:03:02.000000 serverhttpy-0.0.3/serverhttpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-23 22:03:02.000000 serverhttpy-0.0.3/serverhttpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 22:03:02.000000 serverhttpy-0.0.3/serverhttpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-23 22:03:02.000000 serverhttpy-0.0.3/serverhttpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 22:03:02.268815 serverhttpy-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-23 22:02:53.000000 serverhttpy-0.0.3/setup.py
```

### Comparing `serverhttpy-0.0.2/serverhttpy/enums/status_code.py` & `serverhttpy-0.0.3/serverhttpy/enums/status_code.py`

 * *Files identical despite different names*

### Comparing `serverhttpy-0.0.2/serverhttpy/examples/example_clients_managment.py` & `serverhttpy-0.0.3/serverhttpy/examples/example_clients_managment.py`

 * *Files identical despite different names*

### Comparing `serverhttpy-0.0.2/serverhttpy/examples/sample_data.py` & `serverhttpy-0.0.3/serverhttpy/examples/sample_data.py`

 * *Files identical despite different names*

### Comparing `serverhttpy-0.0.2/serverhttpy/models/endpoint.py` & `serverhttpy-0.0.3/serverhttpy/models/endpoint.py`

 * *Files identical despite different names*

### Comparing `serverhttpy-0.0.2/serverhttpy/models/path.py` & `serverhttpy-0.0.3/serverhttpy/models/path.py`

 * *Files identical despite different names*

### Comparing `serverhttpy-0.0.2/serverhttpy/models/request.py` & `serverhttpy-0.0.3/serverhttpy/models/request.py`

 * *Files identical despite different names*

### Comparing `serverhttpy-0.0.2/serverhttpy/models/response.py` & `serverhttpy-0.0.3/serverhttpy/models/response.py`

 * *Files identical despite different names*

### Comparing `serverhttpy-0.0.2/serverhttpy/models/uri.py` & `serverhttpy-0.0.3/serverhttpy/models/uri.py`

 * *Files identical despite different names*

### Comparing `serverhttpy-0.0.2/serverhttpy/server.py` & `serverhttpy-0.0.3/serverhttpy/server.py`

 * *Files identical despite different names*

### Comparing `serverhttpy-0.0.2/serverhttpy.egg-info/SOURCES.txt` & `serverhttpy-0.0.3/serverhttpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

