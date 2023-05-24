# Comparing `tmp/macos_application_location-1.0.0.tar.gz` & `tmp/macos_application_location-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macos_application_location-1.0.0.tar", max compression
+gzip compressed data, was "macos_application_location-1.0.1.tar", max compression
```

## Comparing `macos_application_location-1.0.0.tar` & `macos_application_location-1.0.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    16725 2023-05-24 17:18:29.408463 macos_application_location-1.0.0/LICENSE
--rw-r--r--   0        0        0      229 2023-05-24 17:18:42.355107 macos_application_location-1.0.0/README.md
--rw-r--r--   0        0        0       22 2023-05-24 17:18:42.355322 macos_application_location-1.0.0/packages/macos_application_location/__init__.py
--rw-r--r--   0        0        0      373 2023-05-24 17:18:42.355590 macos_application_location-1.0.0/packages/macos_application_location/main.py
--rw-r--r--   0        0        0      554 2023-05-24 17:18:42.356205 macos_application_location-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1069 1970-01-01 00:00:00.000000 macos_application_location-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    16725 2023-05-24 17:18:29.408463 macos_application_location-1.0.1/LICENSE
+-rw-r--r--   0        0        0      230 2023-05-24 17:25:00.082578 macos_application_location-1.0.1/README.md
+-rw-r--r--   0        0        0       22 2023-05-24 17:18:42.355322 macos_application_location-1.0.1/packages/macos_application_location/__init__.py
+-rw-r--r--   0        0        0      373 2023-05-24 17:18:42.355590 macos_application_location-1.0.1/packages/macos_application_location/main.py
+-rw-r--r--   0        0        0      554 2023-05-24 17:25:04.161120 macos_application_location-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1070 1970-01-01 00:00:00.000000 macos_application_location-1.0.1/PKG-INFO
```

### Comparing `macos_application_location-1.0.0/LICENSE` & `macos_application_location-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `macos_application_location-1.0.0/pyproject.toml` & `macos_application_location-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "macos_application_location"
-version = "1.0.0"
+version = "1.0.1"
 description = ""
 authors = ["Johann Chang <mr.changyuheng@gmail.com>"]
 license = "MPL-2.0"
 readme = "README.md"
 homepage = "https://github.com/changyuheng/macos-application-location"
 repository = "https://github.com/changyuheng/macos-application-location"
 packages = [
```

### Comparing `macos_application_location-1.0.0/PKG-INFO` & `macos_application_location-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macos-application-location
-Version: 1.0.0
+Version: 1.0.1
 Summary: 
 Home-page: https://github.com/changyuheng/macos-application-location
 License: MPL-2.0
 Author: Johann Chang
 Author-email: mr.changyuheng@gmail.com
 Requires-Python: >=3.5
 Classifier: License :: OSI Approved
@@ -21,20 +21,21 @@
 Description-Content-Type: text/markdown
 
 # macos-application-location.py
 
 ## Installation
 
 ```sh
-pip install macos_application_location
+pip install macos-application-location
 ```
 
 ## Usage
 
 ```py
 import pathlib
 
 import macos_application_location
 
 
 app_path: pathlib.Path = macos_application_location.get()
 ```
+
```

