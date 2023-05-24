# Comparing `tmp/remla12_lib_release-0.1.2.tar.gz` & `tmp/remla12_lib_release-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remla12_lib_release-0.1.2.tar", last modified: Wed May 24 16:57:30 2023, max compression
+gzip compressed data, was "remla12_lib_release-0.1.3.tar", last modified: Wed May 24 16:58:28 2023, max compression
```

## Comparing `remla12_lib_release-0.1.2.tar` & `remla12_lib_release-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:57:30.827403 remla12_lib_release-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-24 16:57:30.827403 remla12_lib_release-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-24 16:57:20.000000 remla12_lib_release-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:57:30.827403 remla12_lib_release-0.1.2/remla12_lib_release.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-24 16:57:30.000000 remla12_lib_release-0.1.2/remla12_lib_release.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-24 16:57:30.000000 remla12_lib_release-0.1.2/remla12_lib_release.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 16:57:30.000000 remla12_lib_release-0.1.2/remla12_lib_release.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 16:57:30.000000 remla12_lib_release-0.1.2/remla12_lib_release.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 16:57:30.827403 remla12_lib_release-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-24 16:57:20.000000 remla12_lib_release-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:58:28.524869 remla12_lib_release-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-24 16:58:28.524869 remla12_lib_release-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-24 16:58:15.000000 remla12_lib_release-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:58:28.524869 remla12_lib_release-0.1.3/remla12_lib_release.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-24 16:58:28.000000 remla12_lib_release-0.1.3/remla12_lib_release.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-24 16:58:28.000000 remla12_lib_release-0.1.3/remla12_lib_release.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 16:58:28.000000 remla12_lib_release-0.1.3/remla12_lib_release.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 16:58:28.000000 remla12_lib_release-0.1.3/remla12_lib_release.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 16:58:28.524869 remla12_lib_release-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-24 16:58:15.000000 remla12_lib_release-0.1.3/setup.py
```

### Comparing `remla12_lib_release-0.1.2/PKG-INFO` & `remla12_lib_release-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: remla12_lib_release
-Version: 0.1.2
+Version: 0.1.3
 Summary: A version-aware library for REMLA12 project
 Home-page: https://github.com/remla23-team12/lib
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # Library
 
 The lib repository requires a library that the app repository will depend on. The app repository will intall the lib through a package manager (PyPI). The library has to be published as a package in the same programming language as the app repository.
 
 Changing the below number by incrementing the PATCH version + 1 will trigger the automated workflow (e.g., 0.0.5 --> 0.0.6)
 Note: you need to change init.py,readme,setup 
 
-Release 0.1.2
+Release 0.1.3
```

### Comparing `remla12_lib_release-0.1.2/remla12_lib_release.egg-info/PKG-INFO` & `remla12_lib_release-0.1.3/remla12_lib_release.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: remla12-lib-release
-Version: 0.1.2
+Version: 0.1.3
 Summary: A version-aware library for REMLA12 project
 Home-page: https://github.com/remla23-team12/lib
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # Library
 
 The lib repository requires a library that the app repository will depend on. The app repository will intall the lib through a package manager (PyPI). The library has to be published as a package in the same programming language as the app repository.
 
 Changing the below number by incrementing the PATCH version + 1 will trigger the automated workflow (e.g., 0.0.5 --> 0.0.6)
 Note: you need to change init.py,readme,setup 
 
-Release 0.1.2
+Release 0.1.3
```

