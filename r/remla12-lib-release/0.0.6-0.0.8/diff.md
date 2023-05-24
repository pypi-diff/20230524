# Comparing `tmp/remla12-lib-release-0.0.6.tar.gz` & `tmp/remla12-lib-release-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remla12-lib-release-0.0.6.tar", last modified: Wed May 24 13:56:05 2023, max compression
+gzip compressed data, was "remla12-lib-release-0.0.8.tar", last modified: Wed May 24 14:08:06 2023, max compression
```

## Comparing `remla12-lib-release-0.0.6.tar` & `remla12-lib-release-0.0.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:56:05.780969 remla12-lib-release-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-24 13:56:05.780969 remla12-lib-release-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-24 13:55:54.000000 remla12-lib-release-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:56:05.780969 remla12-lib-release-0.0.6/remla12_lib_release.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-24 13:56:05.000000 remla12-lib-release-0.0.6/remla12_lib_release.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-24 13:56:05.000000 remla12-lib-release-0.0.6/remla12_lib_release.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 13:56:05.000000 remla12-lib-release-0.0.6/remla12_lib_release.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 13:56:05.000000 remla12-lib-release-0.0.6/remla12_lib_release.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 13:56:05.780969 remla12-lib-release-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-24 13:55:54.000000 remla12-lib-release-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:08:06.157509 remla12-lib-release-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-24 14:08:06.153509 remla12-lib-release-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-24 14:07:52.000000 remla12-lib-release-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:08:06.153509 remla12-lib-release-0.0.8/remla12_lib_release.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-24 14:08:06.000000 remla12-lib-release-0.0.8/remla12_lib_release.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-24 14:08:06.000000 remla12-lib-release-0.0.8/remla12_lib_release.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 14:08:06.000000 remla12-lib-release-0.0.8/remla12_lib_release.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 14:08:06.000000 remla12-lib-release-0.0.8/remla12_lib_release.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 14:08:06.157509 remla12-lib-release-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-24 14:07:52.000000 remla12-lib-release-0.0.8/setup.py
```

### Comparing `remla12-lib-release-0.0.6/PKG-INFO` & `remla12-lib-release-0.0.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: remla12-lib-release
-Version: 0.0.6
+Version: 0.0.8
 Summary: A version-aware library for REMLA12 project
 Home-page: https://github.com/remla23-team12/lib
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # Library
 
 The lib repository requires a library that the app repository will depend on. The app repository will intall the lib through a package manager (PyPI). The library has to be published as a package in the same programming language as the app repository.
 
 Changing the below number by incrementing the PATCH version + 1 will trigger the automated workflow (e.g., 0.0.5 --> 0.0.6)
 
-Release 0.0.7
+Release 0.0.8
```

### Comparing `remla12-lib-release-0.0.6/remla12_lib_release.egg-info/PKG-INFO` & `remla12-lib-release-0.0.8/remla12_lib_release.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: remla12-lib-release
-Version: 0.0.6
+Version: 0.0.8
 Summary: A version-aware library for REMLA12 project
 Home-page: https://github.com/remla23-team12/lib
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # Library
 
 The lib repository requires a library that the app repository will depend on. The app repository will intall the lib through a package manager (PyPI). The library has to be published as a package in the same programming language as the app repository.
 
 Changing the below number by incrementing the PATCH version + 1 will trigger the automated workflow (e.g., 0.0.5 --> 0.0.6)
 
-Release 0.0.7
+Release 0.0.8
```

