# Comparing `tmp/np_codeocean-0.1.2.tar.gz` & `tmp/np_codeocean-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "np_codeocean-0.1.2.tar", last modified: Wed May 10 23:19:01 2023, max compression
+gzip compressed data, was "np_codeocean-0.1.3.tar", last modified: Wed May 24 20:16:14 2023, max compression
```

## Comparing `np_codeocean-0.1.2.tar` & `np_codeocean-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      107 2023-05-02 03:16:59.498618 np_codeocean-0.1.2/README.md
--rw-r--r--   0        0        0     1834 2023-05-10 23:19:01.620657 np_codeocean-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-02 03:16:59.500618 np_codeocean-0.1.2/src/np_codeocean/__init__.py
--rw-r--r--   0        0        0     5377 2023-05-10 23:18:08.279782 np_codeocean-0.1.2/src/np_codeocean/upload.py
--rw-r--r--   0        0        0     3375 2023-05-10 23:12:49.826589 np_codeocean-0.1.2/src/np_codeocean/utils.py
--rw-r--r--   0        0        0     1239 1970-01-01 00:00:00.000000 np_codeocean-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      107 2023-05-02 03:16:59.498618 np_codeocean-0.1.3/README.md
+-rw-r--r--   0        0        0     1834 2023-05-24 20:16:14.825779 np_codeocean-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       66 2023-05-24 20:01:38.495205 np_codeocean-0.1.3/src/np_codeocean/__init__.py
+-rw-r--r--   0        0        0     5377 2023-05-10 23:18:08.279782 np_codeocean-0.1.3/src/np_codeocean/upload.py
+-rw-r--r--   0        0        0     3375 2023-05-10 23:12:49.826589 np_codeocean-0.1.3/src/np_codeocean/utils.py
+-rw-r--r--   0        0        0     1239 1970-01-01 00:00:00.000000 np_codeocean-0.1.3/PKG-INFO
```

### Comparing `np_codeocean-0.1.2/pyproject.toml` & `np_codeocean-0.1.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 composite = [
     "bump",
     "pdm publish",
 ]
 
 [project]
 name = "np_codeocean"
-version = "0.1.2"
+version = "0.1.3"
 description = "Tools for uploading and interacting with Mindscope Neuropixels experiments on Code Ocean"
 authors = [
     { name = "Ben Hardcastle", email = "ben.hardcastle@alleninstitute.org" },
 ]
 dependencies = [
     "np_session>=0.6.4",
     "np_tools>=0.1.12",
```

### Comparing `np_codeocean-0.1.2/src/np_codeocean/upload.py` & `np_codeocean-0.1.3/src/np_codeocean/upload.py`

 * *Files identical despite different names*

### Comparing `np_codeocean-0.1.2/src/np_codeocean/utils.py` & `np_codeocean-0.1.3/src/np_codeocean/utils.py`

 * *Files identical despite different names*

### Comparing `np_codeocean-0.1.2/PKG-INFO` & `np_codeocean-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: np-codeocean
-Version: 0.1.2
+Version: 0.1.3
 Summary: Tools for uploading and interacting with Mindscope Neuropixels experiments on Code Ocean
 Author-Email: Ben Hardcastle <ben.hardcastle@alleninstitute.org>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

