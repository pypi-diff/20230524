# Comparing `tmp/jina-hubble-sdk-0.9.1.tar.gz` & `tmp/jina-hubble-sdk-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jina-hubble-sdk-0.9.1.tar", last modified: Wed Aug 10 13:45:57 2022, max compression
+gzip compressed data, was "dist/jina-hubble-sdk-0.9.2.tar", last modified: Thu Aug 11 10:23:18 2022, max compression
```

## Comparing `jina-hubble-sdk-0.9.1.tar` & `jina-hubble-sdk-0.9.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 13:45:57.000000 jina-hubble-sdk-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-08-10 13:45:09.000000 jina-hubble-sdk-0.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6158 2022-08-10 13:45:57.000000 jina-hubble-sdk-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4935 2022-08-10 13:45:09.000000 jina-hubble-sdk-0.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 13:45:57.000000 jina-hubble-sdk-0.9.1/hubble/
--rw-r--r--   0 runner    (1001) docker     (121)     2023 2022-08-10 13:45:09.000000 jina-hubble-sdk-0.9.1/hubble/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 13:45:57.000000 jina-hubble-sdk-0.9.1/hubble/client/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-10 13:45:09.000000 jina-hubble-sdk-0.9.1/hubble/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2618 2022-08-10 13:45:09.000000 jina-hubble-sdk-0.9.1/hubble/client/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     8726 2022-08-10 13:45:09.000000 jina-hubble-sdk-0.9.1/hubble/client/client.py
--rw-r--r--   0 runner    (1001) docker     (121)      536 2022-08-10 13:45:09.000000 jina-hubble-sdk-0.9.1/hubble/client/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (121)     1270 2022-08-10 13:45:09.000000 jina-hubble-sdk-0.9.1/hubble/client/session.py
--rw-r--r--   0 runner    (1001) docker     (121)     2976 2022-08-10 13:45:09.000000 jina-hubble-sdk-0.9.1/hubble/excepts.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 13:45:57.000000 jina-hubble-sdk-0.9.1/hubble/utils/
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-08-10 13:45:09.000000 jina-hubble-sdk-0.9.1/hubble/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      315 2022-08-10 13:45:09.000000 jina-hubble-sdk-0.9.1/hubble/utils/api_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3516 2022-08-10 13:45:09.000000 jina-hubble-sdk-0.9.1/hubble/utils/auth.py
--rw-r--r--   0 runner    (1001) docker     (121)     2084 2022-08-10 13:45:09.000000 jina-hubble-sdk-0.9.1/hubble/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     1161 2022-08-10 13:45:09.000000 jina-hubble-sdk-0.9.1/hubble/utils/pbar.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 13:45:57.000000 jina-hubble-sdk-0.9.1/jina_hubble_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6158 2022-08-10 13:45:57.000000 jina-hubble-sdk-0.9.1/jina_hubble_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      602 2022-08-10 13:45:57.000000 jina-hubble-sdk-0.9.1/jina_hubble_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-10 13:45:57.000000 jina-hubble-sdk-0.9.1/jina_hubble_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-10 13:45:57.000000 jina-hubble-sdk-0.9.1/jina_hubble_sdk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      191 2022-08-10 13:45:57.000000 jina-hubble-sdk-0.9.1/jina_hubble_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-08-10 13:45:57.000000 jina-hubble-sdk-0.9.1/jina_hubble_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      200 2022-08-10 13:45:09.000000 jina-hubble-sdk-0.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-08-10 13:45:09.000000 jina-hubble-sdk-0.9.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-08-10 13:45:09.000000 jina-hubble-sdk-0.9.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-08-10 13:45:57.000000 jina-hubble-sdk-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2606 2022-08-10 13:45:09.000000 jina-hubble-sdk-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 10:23:18.000000 jina-hubble-sdk-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (121)       53 2022-08-11 10:22:20.000000 jina-hubble-sdk-0.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     6157 2022-08-11 10:23:18.000000 jina-hubble-sdk-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4934 2022-08-11 10:22:20.000000 jina-hubble-sdk-0.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 10:23:18.000000 jina-hubble-sdk-0.9.2/hubble/
+-rw-r--r--   0 runner    (1001) docker     (121)     2023 2022-08-11 10:22:20.000000 jina-hubble-sdk-0.9.2/hubble/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 10:23:18.000000 jina-hubble-sdk-0.9.2/hubble/client/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-11 10:22:20.000000 jina-hubble-sdk-0.9.2/hubble/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2618 2022-08-11 10:22:20.000000 jina-hubble-sdk-0.9.2/hubble/client/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8726 2022-08-11 10:22:20.000000 jina-hubble-sdk-0.9.2/hubble/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)      536 2022-08-11 10:22:20.000000 jina-hubble-sdk-0.9.2/hubble/client/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1270 2022-08-11 10:22:20.000000 jina-hubble-sdk-0.9.2/hubble/client/session.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2976 2022-08-11 10:22:20.000000 jina-hubble-sdk-0.9.2/hubble/excepts.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 10:23:18.000000 jina-hubble-sdk-0.9.2/hubble/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)       44 2022-08-11 10:22:20.000000 jina-hubble-sdk-0.9.2/hubble/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      315 2022-08-11 10:22:20.000000 jina-hubble-sdk-0.9.2/hubble/utils/api_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3516 2022-08-11 10:22:20.000000 jina-hubble-sdk-0.9.2/hubble/utils/auth.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2084 2022-08-11 10:22:20.000000 jina-hubble-sdk-0.9.2/hubble/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1161 2022-08-11 10:22:20.000000 jina-hubble-sdk-0.9.2/hubble/utils/pbar.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 10:23:18.000000 jina-hubble-sdk-0.9.2/jina_hubble_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     6157 2022-08-11 10:23:18.000000 jina-hubble-sdk-0.9.2/jina_hubble_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      602 2022-08-11 10:23:18.000000 jina-hubble-sdk-0.9.2/jina_hubble_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-11 10:23:18.000000 jina-hubble-sdk-0.9.2/jina_hubble_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-11 10:23:18.000000 jina-hubble-sdk-0.9.2/jina_hubble_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      145 2022-08-11 10:23:18.000000 jina-hubble-sdk-0.9.2/jina_hubble_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2022-08-11 10:23:18.000000 jina-hubble-sdk-0.9.2/jina_hubble_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      200 2022-08-11 10:22:20.000000 jina-hubble-sdk-0.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      112 2022-08-11 10:22:20.000000 jina-hubble-sdk-0.9.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-08-11 10:22:20.000000 jina-hubble-sdk-0.9.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       66 2022-08-11 10:23:18.000000 jina-hubble-sdk-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2606 2022-08-11 10:22:20.000000 jina-hubble-sdk-0.9.2/setup.py
```

### Comparing `jina-hubble-sdk-0.9.1/PKG-INFO` & `jina-hubble-sdk-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jina-hubble-sdk
-Version: 0.9.1
+Version: 0.9.2
 Summary: SDK for Hubble API at Jina AI.
 Home-page: https://github.com/jina-ai/hubble-client-python/
 Download-URL: https://github.com/jina-ai/hubble-client-python/tags
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Proprietary
 Project-URL: Source, https://github.com/jina-ai/hubble-client-python/
@@ -38,15 +38,14 @@
 <p align="center">
     <a href="https://codecov.io/gh/jina-ai/hubble-client-python">
         <img src="https://codecov.io/gh/jina-ai/hubble-client-python/branch/main/graph/badge.svg?token=Sttz9HTmDq"/>
     </a>
 </p>
 
 
-
 ## Install
 
 ```shell
 pip install jina-hubble-sdk
 ```
 
 ## Core functionality
```

### Comparing `jina-hubble-sdk-0.9.1/README.md` & `jina-hubble-sdk-0.9.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 <p align="center">
     <a href="https://codecov.io/gh/jina-ai/hubble-client-python">
         <img src="https://codecov.io/gh/jina-ai/hubble-client-python/branch/main/graph/badge.svg?token=Sttz9HTmDq"/>
     </a>
 </p>
 
 
-
 ## Install
 
 ```shell
 pip install jina-hubble-sdk
 ```
 
 ## Core functionality
```

### Comparing `jina-hubble-sdk-0.9.1/hubble/__init__.py` & `jina-hubble-sdk-0.9.2/hubble/__init__.py`

 * *Files identical despite different names*

### Comparing `jina-hubble-sdk-0.9.1/hubble/client/base.py` & `jina-hubble-sdk-0.9.2/hubble/client/base.py`

 * *Files identical despite different names*

### Comparing `jina-hubble-sdk-0.9.1/hubble/client/client.py` & `jina-hubble-sdk-0.9.2/hubble/client/client.py`

 * *Files identical despite different names*

### Comparing `jina-hubble-sdk-0.9.1/hubble/client/endpoints.py` & `jina-hubble-sdk-0.9.2/hubble/client/endpoints.py`

 * *Files identical despite different names*

### Comparing `jina-hubble-sdk-0.9.1/hubble/client/session.py` & `jina-hubble-sdk-0.9.2/hubble/client/session.py`

 * *Files identical despite different names*

### Comparing `jina-hubble-sdk-0.9.1/hubble/excepts.py` & `jina-hubble-sdk-0.9.2/hubble/excepts.py`

 * *Files identical despite different names*

### Comparing `jina-hubble-sdk-0.9.1/hubble/utils/auth.py` & `jina-hubble-sdk-0.9.2/hubble/utils/auth.py`

 * *Files identical despite different names*

### Comparing `jina-hubble-sdk-0.9.1/hubble/utils/config.py` & `jina-hubble-sdk-0.9.2/hubble/utils/config.py`

 * *Files identical despite different names*

### Comparing `jina-hubble-sdk-0.9.1/hubble/utils/pbar.py` & `jina-hubble-sdk-0.9.2/hubble/utils/pbar.py`

 * *Files identical despite different names*

### Comparing `jina-hubble-sdk-0.9.1/jina_hubble_sdk.egg-info/PKG-INFO` & `jina-hubble-sdk-0.9.2/jina_hubble_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jina-hubble-sdk
-Version: 0.9.1
+Version: 0.9.2
 Summary: SDK for Hubble API at Jina AI.
 Home-page: https://github.com/jina-ai/hubble-client-python/
 Download-URL: https://github.com/jina-ai/hubble-client-python/tags
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Proprietary
 Project-URL: Source, https://github.com/jina-ai/hubble-client-python/
@@ -38,15 +38,14 @@
 <p align="center">
     <a href="https://codecov.io/gh/jina-ai/hubble-client-python">
         <img src="https://codecov.io/gh/jina-ai/hubble-client-python/branch/main/graph/badge.svg?token=Sttz9HTmDq"/>
     </a>
 </p>
 
 
-
 ## Install
 
 ```shell
 pip install jina-hubble-sdk
 ```
 
 ## Core functionality
```

### Comparing `jina-hubble-sdk-0.9.1/jina_hubble_sdk.egg-info/SOURCES.txt` & `jina-hubble-sdk-0.9.2/jina_hubble_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jina-hubble-sdk-0.9.1/setup.py` & `jina-hubble-sdk-0.9.2/setup.py`

 * *Files identical despite different names*

