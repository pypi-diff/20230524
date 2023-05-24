# Comparing `tmp/arkitema_config-0.1.0.tar.gz` & `tmp/arkitema_config-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arkitema_config-0.1.0.tar", max compression
+gzip compressed data, was "arkitema_config-0.1.1.tar", max compression
```

## Comparing `arkitema_config-0.1.0.tar` & `arkitema_config-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    10173 2023-05-22 14:23:03.085819 arkitema_config-0.1.0/LICENSE
--rw-r--r--   0        0        0     1124 2023-05-22 14:23:03.085819 arkitema_config-0.1.0/README.md
--rw-r--r--   0        0        0     2275 2023-05-22 14:23:03.085819 arkitema_config-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      189 2023-05-22 14:23:03.085819 arkitema_config-0.1.0/src/arkitema_config/__init__.py
--rw-r--r--   0        0        0     2308 2023-05-22 14:23:03.085819 arkitema_config-0.1.0/src/arkitema_config/config.py
--rw-r--r--   0        0        0     1001 2023-05-22 14:23:03.085819 arkitema_config-0.1.0/src/arkitema_config/connection.py
--rw-r--r--   0        0        0      372 2023-05-22 14:23:03.085819 arkitema_config-0.1.0/src/arkitema_config/context.py
--rw-r--r--   0        0        0     1154 2023-05-22 14:23:03.085819 arkitema_config-0.1.0/src/arkitema_config/email.py
--rw-r--r--   0        0        0      263 2023-05-22 14:23:03.085819 arkitema_config-0.1.0/src/arkitema_config/exceptions.py
--rw-r--r--   0        0        0      631 2023-05-22 14:23:03.085819 arkitema_config-0.1.0/src/arkitema_config/fastapi.py
--rw-r--r--   0        0        0       69 2023-05-22 14:23:03.085819 arkitema_config-0.1.0/src/arkitema_config/formatting.py
--rw-r--r--   0        0        0        0 2023-05-22 14:23:03.085819 arkitema_config-0.1.0/src/arkitema_config/graphql/__init__.py
--rw-r--r--   0        0        0     2772 2023-05-22 14:23:03.085819 arkitema_config-0.1.0/src/arkitema_config/graphql/input_filters.py
--rw-r--r--   0        0        0     1270 2023-05-22 14:23:03.085819 arkitema_config-0.1.0/src/arkitema_config/graphql/pagination.py
--rw-r--r--   0        0        0     4856 2023-05-22 14:23:03.085819 arkitema_config-0.1.0/src/arkitema_config/monitoring.py
--rw-r--r--   0        0        0      400 2023-05-22 14:23:03.085819 arkitema_config-0.1.0/src/arkitema_config/permissions.py
--rw-r--r--   0        0        0      992 2023-05-22 14:23:03.085819 arkitema_config-0.1.0/src/arkitema_config/router.py
--rw-r--r--   0        0        0      533 2023-05-22 14:23:03.085819 arkitema_config-0.1.0/src/arkitema_config/security.py
--rw-r--r--   0        0        0     5075 2023-05-22 14:23:03.085819 arkitema_config-0.1.0/src/arkitema_config/user.py
--rw-r--r--   0        0        0     2353 1970-01-01 00:00:00.000000 arkitema_config-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    10173 2023-05-24 08:25:39.708466 arkitema_config-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1124 2023-05-24 08:25:39.708466 arkitema_config-0.1.1/README.md
+-rw-r--r--   0        0        0     2275 2023-05-24 08:25:39.712466 arkitema_config-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      189 2023-05-24 08:25:39.712466 arkitema_config-0.1.1/src/arkitema_config/__init__.py
+-rw-r--r--   0        0        0     2308 2023-05-24 08:25:39.712466 arkitema_config-0.1.1/src/arkitema_config/config.py
+-rw-r--r--   0        0        0     1001 2023-05-24 08:25:39.712466 arkitema_config-0.1.1/src/arkitema_config/connection.py
+-rw-r--r--   0        0        0      372 2023-05-24 08:25:39.712466 arkitema_config-0.1.1/src/arkitema_config/context.py
+-rw-r--r--   0        0        0     1154 2023-05-24 08:25:39.712466 arkitema_config-0.1.1/src/arkitema_config/email.py
+-rw-r--r--   0        0        0      263 2023-05-24 08:25:39.712466 arkitema_config-0.1.1/src/arkitema_config/exceptions.py
+-rw-r--r--   0        0        0      631 2023-05-24 08:25:39.712466 arkitema_config-0.1.1/src/arkitema_config/fastapi.py
+-rw-r--r--   0        0        0       69 2023-05-24 08:25:39.712466 arkitema_config-0.1.1/src/arkitema_config/formatting.py
+-rw-r--r--   0        0        0        0 2023-05-24 08:25:39.712466 arkitema_config-0.1.1/src/arkitema_config/graphql/__init__.py
+-rw-r--r--   0        0        0     2772 2023-05-24 08:25:39.712466 arkitema_config-0.1.1/src/arkitema_config/graphql/input_filters.py
+-rw-r--r--   0        0        0     1270 2023-05-24 08:25:39.712466 arkitema_config-0.1.1/src/arkitema_config/graphql/pagination.py
+-rw-r--r--   0        0        0     4856 2023-05-24 08:25:39.712466 arkitema_config-0.1.1/src/arkitema_config/monitoring.py
+-rw-r--r--   0        0        0      400 2023-05-24 08:25:39.712466 arkitema_config-0.1.1/src/arkitema_config/permissions.py
+-rw-r--r--   0        0        0      992 2023-05-24 08:25:39.712466 arkitema_config-0.1.1/src/arkitema_config/router.py
+-rw-r--r--   0        0        0      533 2023-05-24 08:25:39.712466 arkitema_config-0.1.1/src/arkitema_config/security.py
+-rw-r--r--   0        0        0     5075 2023-05-24 08:25:39.712466 arkitema_config-0.1.1/src/arkitema_config/user.py
+-rw-r--r--   0        0        0     2353 1970-01-01 00:00:00.000000 arkitema_config-0.1.1/PKG-INFO
```

### Comparing `arkitema_config-0.1.0/LICENSE` & `arkitema_config-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `arkitema_config-0.1.0/README.md` & `arkitema_config-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `arkitema_config-0.1.0/pyproject.toml` & `arkitema_config-0.1.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "arkitema-config"
-version = "0.1.0"
+version = "0.1.1"
 description = "Configurations for Arkitema FastAPI apps"
 authors = ["Christian Kongsgaard <chrk@arkitema.com>"]
 repository = "https://github.com/Arkitema/backend-config"
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `arkitema_config-0.1.0/src/arkitema_config/config.py` & `arkitema_config-0.1.1/src/arkitema_config/config.py`

 * *Files identical despite different names*

### Comparing `arkitema_config-0.1.0/src/arkitema_config/connection.py` & `arkitema_config-0.1.1/src/arkitema_config/connection.py`

 * *Files identical despite different names*

### Comparing `arkitema_config-0.1.0/src/arkitema_config/email.py` & `arkitema_config-0.1.1/src/arkitema_config/email.py`

 * *Files identical despite different names*

### Comparing `arkitema_config-0.1.0/src/arkitema_config/fastapi.py` & `arkitema_config-0.1.1/src/arkitema_config/fastapi.py`

 * *Files identical despite different names*

### Comparing `arkitema_config-0.1.0/src/arkitema_config/graphql/input_filters.py` & `arkitema_config-0.1.1/src/arkitema_config/graphql/input_filters.py`

 * *Files identical despite different names*

### Comparing `arkitema_config-0.1.0/src/arkitema_config/graphql/pagination.py` & `arkitema_config-0.1.1/src/arkitema_config/graphql/pagination.py`

 * *Files identical despite different names*

### Comparing `arkitema_config-0.1.0/src/arkitema_config/monitoring.py` & `arkitema_config-0.1.1/src/arkitema_config/monitoring.py`

 * *Files identical despite different names*

### Comparing `arkitema_config-0.1.0/src/arkitema_config/router.py` & `arkitema_config-0.1.1/src/arkitema_config/router.py`

 * *Files identical despite different names*

### Comparing `arkitema_config-0.1.0/src/arkitema_config/security.py` & `arkitema_config-0.1.1/src/arkitema_config/security.py`

 * *Files identical despite different names*

### Comparing `arkitema_config-0.1.0/src/arkitema_config/user.py` & `arkitema_config-0.1.1/src/arkitema_config/user.py`

 * *Files identical despite different names*

### Comparing `arkitema_config-0.1.0/PKG-INFO` & `arkitema_config-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arkitema-config
-Version: 0.1.0
+Version: 0.1.1
 Summary: Configurations for Arkitema FastAPI apps
 Home-page: https://github.com/Arkitema/backend-config
 License: Apache-2.0
 Author: Christian Kongsgaard
 Author-email: chrk@arkitema.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

