# Comparing `tmp/cenao-0.9.1.tar.gz` & `tmp/cenao-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cenao-0.9.1.tar", last modified: Mon Apr 17 23:12:58 2023, max compression
+gzip compressed data, was "cenao-0.9.2.tar", last modified: Thu May  4 23:49:07 2023, max compression
```

## Comparing `cenao-0.9.1.tar` & `cenao-0.9.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 23:12:58.014031 cenao-0.9.1/
--rw-rw-rw-   0 root         (0) root         (0)     1071 2022-04-03 12:51:06.000000 cenao-0.9.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      723 2023-04-17 23:12:58.014031 cenao-0.9.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       57 2022-04-03 12:51:06.000000 cenao-0.9.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)       85 2022-04-03 12:51:06.000000 cenao-0.9.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 23:12:58.014031 cenao-0.9.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1487 2023-01-31 14:58:38.000000 cenao-0.9.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 23:12:58.010031 cenao-0.9.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 23:12:58.014031 cenao-0.9.1/src/cenao/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 23:12:47.000000 cenao-0.9.1/src/cenao/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4653 2023-04-17 22:55:11.000000 cenao-0.9.1/src/cenao/app.py
--rw-rw-rw-   0 root         (0) root         (0)     1863 2023-01-23 19:46:22.000000 cenao-0.9.1/src/cenao/config.py
--rw-rw-rw-   0 root         (0) root         (0)     1278 2023-04-06 20:52:12.000000 cenao-0.9.1/src/cenao/errors.py
--rw-rw-rw-   0 root         (0) root         (0)      159 2022-04-03 12:51:06.000000 cenao-0.9.1/src/cenao/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 23:12:58.014031 cenao-0.9.1/src/cenao/features/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 23:12:47.000000 cenao-0.9.1/src/cenao/features/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      480 2022-04-13 21:27:34.000000 cenao-0.9.1/src/cenao/features/health.py
--rw-rw-rw-   0 root         (0) root         (0)     4264 2022-04-03 12:51:06.000000 cenao-0.9.1/src/cenao/features/redis.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 23:12:58.014031 cenao-0.9.1/src/cenao/features/redis_storage/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 23:12:47.000000 cenao-0.9.1/src/cenao/features/redis_storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      341 2022-04-03 12:51:06.000000 cenao-0.9.1/src/cenao/features/redis_storage/app_feature.py
--rw-rw-rw-   0 root         (0) root         (0)       30 2022-04-03 12:51:06.000000 cenao-0.9.1/src/cenao/features/redis_storage/model.py
--rw-rw-rw-   0 root         (0) root         (0)     4750 2023-04-06 20:52:12.000000 cenao-0.9.1/src/cenao/features/s3.py
--rw-rw-rw-   0 root         (0) root         (0)     3877 2023-04-17 23:12:47.000000 cenao-0.9.1/src/cenao/features/web.py
--rw-rw-rw-   0 root         (0) root         (0)     1996 2023-01-23 19:46:22.000000 cenao-0.9.1/src/cenao/runner.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-17 23:12:52.000000 cenao-0.9.1/src/cenao/version.py
--rw-rw-rw-   0 root         (0) root         (0)     1953 2023-04-06 20:52:12.000000 cenao-0.9.1/src/cenao/view.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 23:12:58.014031 cenao-0.9.1/src/cenao.egg-info/
--rw-r--r--   0 root         (0) root         (0)      723 2023-04-17 23:12:58.000000 cenao-0.9.1/src/cenao.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      641 2023-04-17 23:12:58.000000 cenao-0.9.1/src/cenao.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 23:12:58.000000 cenao-0.9.1/src/cenao.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      178 2023-04-17 23:12:58.000000 cenao-0.9.1/src/cenao.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-04-17 23:12:58.000000 cenao-0.9.1/src/cenao.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 23:49:07.394655 cenao-0.9.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1071 2022-04-03 12:51:06.000000 cenao-0.9.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      723 2023-05-04 23:49:07.394655 cenao-0.9.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       57 2022-04-03 12:51:06.000000 cenao-0.9.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       85 2022-04-03 12:51:06.000000 cenao-0.9.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-04 23:49:07.394655 cenao-0.9.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1487 2023-01-31 14:56:23.000000 cenao-0.9.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 23:49:07.390655 cenao-0.9.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 23:49:07.394655 cenao-0.9.2/src/cenao/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-04 23:48:57.000000 cenao-0.9.2/src/cenao/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4653 2023-04-17 22:55:07.000000 cenao-0.9.2/src/cenao/app.py
+-rw-rw-rw-   0 root         (0) root         (0)     1863 2022-12-10 13:52:25.000000 cenao-0.9.2/src/cenao/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1278 2023-03-07 22:50:32.000000 cenao-0.9.2/src/cenao/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)      159 2022-04-03 12:51:06.000000 cenao-0.9.2/src/cenao/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 23:49:07.394655 cenao-0.9.2/src/cenao/features/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-04 23:48:57.000000 cenao-0.9.2/src/cenao/features/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      480 2022-04-13 20:43:45.000000 cenao-0.9.2/src/cenao/features/health.py
+-rw-rw-rw-   0 root         (0) root         (0)     4264 2022-04-03 12:51:06.000000 cenao-0.9.2/src/cenao/features/redis.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 23:49:07.394655 cenao-0.9.2/src/cenao/features/redis_storage/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-04 23:48:57.000000 cenao-0.9.2/src/cenao/features/redis_storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      341 2022-04-03 12:51:06.000000 cenao-0.9.2/src/cenao/features/redis_storage/app_feature.py
+-rw-rw-rw-   0 root         (0) root         (0)       30 2022-04-03 12:51:06.000000 cenao-0.9.2/src/cenao/features/redis_storage/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     4750 2023-04-03 12:41:52.000000 cenao-0.9.2/src/cenao/features/s3.py
+-rw-rw-rw-   0 root         (0) root         (0)     3837 2023-05-04 23:48:56.000000 cenao-0.9.2/src/cenao/features/web.py
+-rw-rw-rw-   0 root         (0) root         (0)     1996 2022-12-10 13:52:25.000000 cenao-0.9.2/src/cenao/runner.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-05-04 23:49:01.000000 cenao-0.9.2/src/cenao/version.py
+-rw-rw-rw-   0 root         (0) root         (0)     1953 2023-04-06 20:52:07.000000 cenao-0.9.2/src/cenao/view.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 23:49:07.394655 cenao-0.9.2/src/cenao.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      723 2023-05-04 23:49:07.000000 cenao-0.9.2/src/cenao.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      641 2023-05-04 23:49:07.000000 cenao-0.9.2/src/cenao.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 23:49:07.000000 cenao-0.9.2/src/cenao.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      178 2023-05-04 23:49:07.000000 cenao-0.9.2/src/cenao.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-04 23:49:07.000000 cenao-0.9.2/src/cenao.egg-info/top_level.txt
```

### Comparing `cenao-0.9.1/LICENSE` & `cenao-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cenao-0.9.1/PKG-INFO` & `cenao-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cenao
-Version: 0.9.1
+Version: 0.9.2
 Summary: Python framework for fast and async applications
 Home-page: https://gitlab.uwtech.org/uwtech/cenao
 Author: Roman Shishkin
 Author-email: spark@uwtech.org
 License: MIT
 Project-URL: Source, https://gitlab.uwtech.org/uwtech/cenao
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cenao-0.9.1/setup.py` & `cenao-0.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `cenao-0.9.1/src/cenao/app.py` & `cenao-0.9.2/src/cenao/app.py`

 * *Files identical despite different names*

### Comparing `cenao-0.9.1/src/cenao/config.py` & `cenao-0.9.2/src/cenao/config.py`

 * *Files identical despite different names*

### Comparing `cenao-0.9.1/src/cenao/errors.py` & `cenao-0.9.2/src/cenao/errors.py`

 * *Files identical despite different names*

### Comparing `cenao-0.9.1/src/cenao/features/redis.py` & `cenao-0.9.2/src/cenao/features/redis.py`

 * *Files identical despite different names*

### Comparing `cenao-0.9.1/src/cenao/features/s3.py` & `cenao-0.9.2/src/cenao/features/s3.py`

 * *Files identical despite different names*

### Comparing `cenao-0.9.1/src/cenao/features/web.py` & `cenao-0.9.2/src/cenao/features/web.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
                     status_code = error_resp.status
                     raise
                 except BaseException:
                     status_code = 500
                     raise
                 finally:
                     self.PROMETHEUS_REQUEST_METRIC.labels(
-                        path=request.match_info.route.resource.canonical,
+                        path=uri,
                         method=request.method,
                         status=str(status_code),
                     ).inc()
 
             return resp
 
         self.aiohttp_app = web.Application(
```

### Comparing `cenao-0.9.1/src/cenao/runner.py` & `cenao-0.9.2/src/cenao/runner.py`

 * *Files identical despite different names*

### Comparing `cenao-0.9.1/src/cenao/view.py` & `cenao-0.9.2/src/cenao/view.py`

 * *Files identical despite different names*

### Comparing `cenao-0.9.1/src/cenao.egg-info/PKG-INFO` & `cenao-0.9.2/src/cenao.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cenao
-Version: 0.9.1
+Version: 0.9.2
 Summary: Python framework for fast and async applications
 Home-page: https://gitlab.uwtech.org/uwtech/cenao
 Author: Roman Shishkin
 Author-email: spark@uwtech.org
 License: MIT
 Project-URL: Source, https://gitlab.uwtech.org/uwtech/cenao
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cenao-0.9.1/src/cenao.egg-info/SOURCES.txt` & `cenao-0.9.2/src/cenao.egg-info/SOURCES.txt`

 * *Files identical despite different names*

