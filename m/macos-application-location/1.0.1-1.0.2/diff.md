# Comparing `tmp/macos_application_location-1.0.1.tar.gz` & `tmp/macos_application_location-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macos_application_location-1.0.1.tar", max compression
+gzip compressed data, was "macos_application_location-1.0.2.tar", max compression
```

## Comparing `macos_application_location-1.0.1.tar` & `macos_application_location-1.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    16725 2023-05-24 17:18:29.408463 macos_application_location-1.0.1/LICENSE
--rw-r--r--   0        0        0      230 2023-05-24 17:25:00.082578 macos_application_location-1.0.1/README.md
--rw-r--r--   0        0        0       22 2023-05-24 17:18:42.355322 macos_application_location-1.0.1/packages/macos_application_location/__init__.py
--rw-r--r--   0        0        0      373 2023-05-24 17:18:42.355590 macos_application_location-1.0.1/packages/macos_application_location/main.py
--rw-r--r--   0        0        0      554 2023-05-24 17:25:04.161120 macos_application_location-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1070 1970-01-01 00:00:00.000000 macos_application_location-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    16725 2023-05-24 17:18:29.408463 macos_application_location-1.0.2/LICENSE
+-rw-r--r--   0        0        0      312 2023-05-24 17:43:57.563227 macos_application_location-1.0.2/README.md
+-rw-r--r--   0        0        0       22 2023-05-24 17:18:42.355322 macos_application_location-1.0.2/packages/macos_application_location/__init__.py
+-rw-r--r--   0        0        0      326 2023-05-24 17:47:36.091466 macos_application_location-1.0.2/packages/macos_application_location/main.py
+-rw-r--r--   0        0        0      537 2023-05-24 17:49:32.656048 macos_application_location-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1122 1970-01-01 00:00:00.000000 macos_application_location-1.0.2/PKG-INFO
```

### Comparing `macos_application_location-1.0.1/LICENSE` & `macos_application_location-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `macos_application_location-1.0.1/PKG-INFO` & `macos_application_location-1.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macos-application-location
-Version: 1.0.1
+Version: 1.0.2
 Summary: 
 Home-page: https://github.com/changyuheng/macos-application-location
 License: MPL-2.0
 Author: Johann Chang
 Author-email: mr.changyuheng@gmail.com
 Requires-Python: >=3.5
 Classifier: License :: OSI Approved
@@ -12,20 +12,21 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: psutil (>=5.9)
 Project-URL: Repository, https://github.com/changyuheng/macos-application-location
 Description-Content-Type: text/markdown
 
 # macos-application-location.py
 
+This tiny module helps you to obtain the path of an Application (.app) on macOS.
+
 ## Installation
 
 ```sh
 pip install macos-application-location
 ```
 
 ## Usage
```

