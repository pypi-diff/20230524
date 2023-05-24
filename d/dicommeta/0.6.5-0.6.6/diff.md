# Comparing `tmp/dicommeta-0.6.5.tar.gz` & `tmp/dicommeta-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dicommeta-0.6.5.tar", max compression
+gzip compressed data, was "dicommeta-0.6.6.tar", max compression
```

## Comparing `dicommeta-0.6.5.tar` & `dicommeta-0.6.6.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0    11356 2023-05-09 13:28:51.971341 dicommeta-0.6.5/LICENSE
--rw-r--r--   0        0        0     2666 2023-05-23 15:47:43.845985 dicommeta-0.6.5/README.md
--rw-r--r--   0        0        0      514 2023-05-23 15:58:27.858380 dicommeta-0.6.5/pyproject.toml
--rw-r--r--   0        0        0     3673 2023-05-23 11:56:02.053987 dicommeta-0.6.5/src/dicommeta/Struct.py
--rw-r--r--   0        0        0     2342 2023-05-23 11:49:03.746665 dicommeta-0.6.5/src/dicommeta/Utils.py
--rw-r--r--   0        0        0        0 2023-05-22 22:10:29.709188 dicommeta-0.6.5/src/dicommeta/__init__.py
--rw-r--r--   0        0        0     3126 1970-01-01 00:00:00.000000 dicommeta-0.6.5/PKG-INFO
+-rw-r--r--   0        0        0       57 2023-05-22 22:52:50.650896 dicommeta-0.6.6/CHANGELOG.md
+-rw-r--r--   0        0        0    11356 2023-05-09 13:28:51.971341 dicommeta-0.6.6/LICENSE
+-rw-r--r--   0        0        0     2666 2023-05-23 15:47:43.845985 dicommeta-0.6.6/README.md
+-rw-r--r--   0        0        0      673 2023-05-24 01:01:34.199258 dicommeta-0.6.6/pyproject.toml
+-rw-r--r--   0        0        0     3673 2023-05-23 11:56:02.053987 dicommeta-0.6.6/src/dicommeta/Struct.py
+-rw-r--r--   0        0        0     2342 2023-05-23 11:49:03.746665 dicommeta-0.6.6/src/dicommeta/Utils.py
+-rw-r--r--   0        0        0        0 2023-05-22 22:10:29.709188 dicommeta-0.6.6/src/dicommeta/__init__.py
+-rw-r--r--   0        0        0     3341 1970-01-01 00:00:00.000000 dicommeta-0.6.6/PKG-INFO
```

### Comparing `dicommeta-0.6.5/LICENSE` & `dicommeta-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dicommeta-0.6.5/README.md` & `dicommeta-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `dicommeta-0.6.5/pyproject.toml` & `dicommeta-0.6.6/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 [tool.poetry]
 name = "dicommeta"
-version = "0.6.5"
+version = "0.6.6"
 description = "Dicom Metadata structures"
-authors = ["Kevin Long <longke@pennmedicine.upenn.edu>"]
+authors = ["Kevin Long <longke@pennmedicine.upenn.edu>",]
+maintainers = ["Kevin Long <longke@pennmedicine.upenn.edu>",]
+repository = "https://dev.azure.com/longke/Radiology/_git/DicomMeta"
 readme = "README.md"
+include = ["CHANGELOG.md"]
 packages = [
     { include = "dicommeta", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 attrs = "^23.1.0"
```

### Comparing `dicommeta-0.6.5/src/dicommeta/Struct.py` & `dicommeta-0.6.6/src/dicommeta/Struct.py`

 * *Files identical despite different names*

### Comparing `dicommeta-0.6.5/src/dicommeta/Utils.py` & `dicommeta-0.6.6/src/dicommeta/Utils.py`

 * *Files identical despite different names*

### Comparing `dicommeta-0.6.5/PKG-INFO` & `dicommeta-0.6.6/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 Metadata-Version: 2.1
 Name: dicommeta
-Version: 0.6.5
+Version: 0.6.6
 Summary: Dicom Metadata structures
+Home-page: https://dev.azure.com/longke/Radiology/_git/DicomMeta
 Author: Kevin Long
 Author-email: longke@pennmedicine.upenn.edu
+Maintainer: Kevin Long
+Maintainer-email: longke@pennmedicine.upenn.edu
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: attrs (>=23.1.0,<24.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
+Project-URL: Repository, https://dev.azure.com/longke/Radiology/_git/DicomMeta
 Description-Content-Type: text/markdown
 
 # DicomMeta
 
 dicommeta is a Python library for efficiently storing large amounts of Dicom Metadata
 
 ## Installation
```

