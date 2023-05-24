# Comparing `tmp/furiosa-common-0.9.0rc3.tar.gz` & `tmp/furiosa_common-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "furiosa-common-0.9.0rc3.tar", last modified: Fri Apr 14 21:24:53 2023, max compression
+gzip compressed data, was "furiosa_common-0.9.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `furiosa-common-0.9.0rc3.tar` & `furiosa_common-0.9.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      353 2023-04-14 21:20:22.712571 furiosa-common-0.9.0rc3/Makefile
--rw-r--r--   0        0        0      144 2023-04-14 21:20:22.712571 furiosa-common-0.9.0rc3/README.md
--rw-r--r--   0        0        0      142 2023-04-14 21:20:22.712571 furiosa-common-0.9.0rc3/furiosa/common/__init__.py
--rw-r--r--   0        0        0      523 2023-04-14 21:20:22.712571 furiosa-common-0.9.0rc3/furiosa/common/error.py
--rw-r--r--   0        0        0       17 2023-04-14 21:21:26.595991 furiosa-common-0.9.0rc3/furiosa/common/git_version.txt
--rw-r--r--   0        0        0     3184 2023-04-14 21:20:22.712571 furiosa-common-0.9.0rc3/furiosa/common/native.py
--rw-r--r--   0        0        0     1552 2023-04-14 21:20:22.712571 furiosa-common-0.9.0rc3/furiosa/common/thread.py
--rw-r--r--   0        0        0     1110 2023-04-14 21:20:22.712571 furiosa-common-0.9.0rc3/furiosa/common/utils.py
--rw-r--r--   0        0        0     2301 2023-04-14 21:20:22.712571 furiosa-common-0.9.0rc3/pyproject.toml
--rw-r--r--   0        0        0     1228 1970-01-01 00:00:00.000000 furiosa-common-0.9.0rc3/PKG-INFO
+-rw-r--r--   0        0        0      353 2023-05-24 05:34:31.216840 furiosa_common-0.9.1/Makefile
+-rw-r--r--   0        0        0      144 2023-05-24 05:34:31.216840 furiosa_common-0.9.1/README.md
+-rw-r--r--   0        0        0      142 2023-05-24 05:34:31.216840 furiosa_common-0.9.1/furiosa/common/__init__.py
+-rw-r--r--   0        0        0      523 2023-05-24 05:34:31.216840 furiosa_common-0.9.1/furiosa/common/error.py
+-rw-r--r--   0        0        0       14 2023-05-24 05:35:51.860300 furiosa_common-0.9.1/furiosa/common/git_version.txt
+-rw-r--r--   0        0        0     3184 2023-05-24 05:34:31.220841 furiosa_common-0.9.1/furiosa/common/native.py
+-rw-r--r--   0        0        0     1552 2023-05-24 05:34:31.220841 furiosa_common-0.9.1/furiosa/common/thread.py
+-rw-r--r--   0        0        0     1110 2023-05-24 05:34:31.220841 furiosa_common-0.9.1/furiosa/common/utils.py
+-rw-r--r--   0        0        0     2297 2023-05-24 05:34:31.220841 furiosa_common-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     1225 1970-01-01 00:00:00.000000 furiosa_common-0.9.1/PKG-INFO
```

### Comparing `furiosa-common-0.9.0rc3/furiosa/common/error.py` & `furiosa_common-0.9.1/furiosa/common/error.py`

 * *Files identical despite different names*

### Comparing `furiosa-common-0.9.0rc3/furiosa/common/native.py` & `furiosa_common-0.9.1/furiosa/common/native.py`

 * *Files identical despite different names*

### Comparing `furiosa-common-0.9.0rc3/furiosa/common/thread.py` & `furiosa_common-0.9.1/furiosa/common/thread.py`

 * *Files identical despite different names*

### Comparing `furiosa-common-0.9.0rc3/furiosa/common/utils.py` & `furiosa_common-0.9.1/furiosa/common/utils.py`

 * *Files identical despite different names*

### Comparing `furiosa-common-0.9.0rc3/pyproject.toml` & `furiosa_common-0.9.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Custom backend from https://gitlab.com/ileixe/flit_ext to use setuptools-scm
 # Upstream flit does not support it. See https://github.com/pypa/flit/issues/257
 requires = ["flit_ext"]
 build-backend = "flit_ext:buildapi"
 
 [project]
 name = "furiosa-common"
-version = "0.9.0.rc3"
+version = "0.9.1"
 authors = [{ name = "FurioaAI, Inc.", email = "pkg@furiosa.ai" }]
 readme = "README.md"
 license = { text = "Apache License 2.0" }
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Intended Audience :: Developers",
```

### Comparing `furiosa-common-0.9.0rc3/PKG-INFO` & `furiosa_common-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: furiosa-common
-Version: 0.9.0rc3
+Version: 0.9.1
 Summary: Furiosa SDK common utilities
 Author-email: "FurioaAI, Inc." <pkg@furiosa.ai>
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

