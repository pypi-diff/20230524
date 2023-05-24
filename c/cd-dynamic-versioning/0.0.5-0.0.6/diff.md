# Comparing `tmp/cd_dynamic_versioning-0.0.5.tar.gz` & `tmp/cd_dynamic_versioning-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cd_dynamic_versioning-0.0.5.tar", max compression
+gzip compressed data, was "cd_dynamic_versioning-0.0.6.tar", max compression
```

## Comparing `cd_dynamic_versioning-0.0.5.tar` & `cd_dynamic_versioning-0.0.6.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      554 2023-05-24 07:56:19.460082 cd_dynamic_versioning-0.0.5/README.md
--rw-r--r--   0        0        0       56 2023-05-24 07:57:00.126212 cd_dynamic_versioning-0.0.5/cd_dynamic_versioning/__init__.py
--rw-r--r--   0        0        0     1129 2023-05-24 07:57:00.126212 cd_dynamic_versioning-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1053 1970-01-01 00:00:00.000000 cd_dynamic_versioning-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      554 2023-05-24 10:43:08.988165 cd_dynamic_versioning-0.0.6/README.md
+-rw-r--r--   0        0        0       56 2023-05-24 10:43:41.428800 cd_dynamic_versioning-0.0.6/cd_dynamic_versioning/__init__.py
+-rw-r--r--   0        0        0     1129 2023-05-24 10:43:41.424800 cd_dynamic_versioning-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1053 1970-01-01 00:00:00.000000 cd_dynamic_versioning-0.0.6/PKG-INFO
```

### Comparing `cd_dynamic_versioning-0.0.5/README.md` & `cd_dynamic_versioning-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `cd_dynamic_versioning-0.0.5/pyproject.toml` & `cd_dynamic_versioning-0.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cd-dynamic-versioning"
-version = "0.0.5"
+version = "0.0.6"
 description = "Testpackage for dynamic versioning"
 authors = ["Yngve Moe <yngve.m.moe@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "cd_dynamic_versioning"}]
 
 [tool.poetry.dependencies]
```

### Comparing `cd_dynamic_versioning-0.0.5/PKG-INFO` & `cd_dynamic_versioning-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cd-dynamic-versioning
-Version: 0.0.5
+Version: 0.0.6
 Summary: Testpackage for dynamic versioning
 License: MIT
 Author: Yngve Moe
 Author-email: yngve.m.moe@gmail.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

