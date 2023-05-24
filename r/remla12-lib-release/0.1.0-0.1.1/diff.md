# Comparing `tmp/remla12-lib-release-0.1.0.tar.gz` & `tmp/remla12-lib-release-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remla12-lib-release-0.1.0.tar", last modified: Wed May 24 14:29:19 2023, max compression
+gzip compressed data, was "remla12-lib-release-0.1.1.tar", last modified: Wed May 24 15:15:25 2023, max compression
```

## Comparing `remla12-lib-release-0.1.0.tar` & `remla12-lib-release-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:29:19.012816 remla12-lib-release-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-24 14:29:19.012816 remla12-lib-release-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-24 14:29:07.000000 remla12-lib-release-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:29:19.012816 remla12-lib-release-0.1.0/remla12_lib_release.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-24 14:29:18.000000 remla12-lib-release-0.1.0/remla12_lib_release.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-24 14:29:18.000000 remla12-lib-release-0.1.0/remla12_lib_release.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 14:29:18.000000 remla12-lib-release-0.1.0/remla12_lib_release.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 14:29:18.000000 remla12-lib-release-0.1.0/remla12_lib_release.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 14:29:19.012816 remla12-lib-release-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-24 14:29:07.000000 remla12-lib-release-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:15:25.224907 remla12-lib-release-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-24 15:15:25.224907 remla12-lib-release-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-24 15:15:14.000000 remla12-lib-release-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:15:25.224907 remla12-lib-release-0.1.1/remla12_lib_release.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-24 15:15:25.000000 remla12-lib-release-0.1.1/remla12_lib_release.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-24 15:15:25.000000 remla12-lib-release-0.1.1/remla12_lib_release.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:15:25.000000 remla12-lib-release-0.1.1/remla12_lib_release.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:15:25.000000 remla12-lib-release-0.1.1/remla12_lib_release.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 15:15:25.224907 remla12-lib-release-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-24 15:15:14.000000 remla12-lib-release-0.1.1/setup.py
```

### Comparing `remla12-lib-release-0.1.0/PKG-INFO` & `remla12-lib-release-0.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: remla12-lib-release
-Version: 0.1.0
+Version: 0.1.1
 Summary: A version-aware library for REMLA12 project
 Home-page: https://github.com/remla23-team12/lib
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # Library
 
 The lib repository requires a library that the app repository will depend on. The app repository will intall the lib through a package manager (PyPI). The library has to be published as a package in the same programming language as the app repository.
 
 Changing the below number by incrementing the PATCH version + 1 will trigger the automated workflow (e.g., 0.0.5 --> 0.0.6)
 Note: you need to change init.py,readme,setup 
 
-Release 0.1.0
+Release 0.1.1
```

### Comparing `remla12-lib-release-0.1.0/remla12_lib_release.egg-info/PKG-INFO` & `remla12-lib-release-0.1.1/remla12_lib_release.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: remla12-lib-release
-Version: 0.1.0
+Version: 0.1.1
 Summary: A version-aware library for REMLA12 project
 Home-page: https://github.com/remla23-team12/lib
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # Library
 
 The lib repository requires a library that the app repository will depend on. The app repository will intall the lib through a package manager (PyPI). The library has to be published as a package in the same programming language as the app repository.
 
 Changing the below number by incrementing the PATCH version + 1 will trigger the automated workflow (e.g., 0.0.5 --> 0.0.6)
 Note: you need to change init.py,readme,setup 
 
-Release 0.1.0
+Release 0.1.1
```

