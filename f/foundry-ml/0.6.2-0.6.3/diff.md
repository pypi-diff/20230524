# Comparing `tmp/foundry_ml-0.6.2.tar.gz` & `tmp/foundry_ml-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foundry_ml-0.6.2.tar", last modified: Thu May 11 22:07:08 2023, max compression
+gzip compressed data, was "foundry_ml-0.6.3.tar", last modified: Wed May 24 21:13:23 2023, max compression
```

## Comparing `foundry_ml-0.6.2.tar` & `foundry_ml-0.6.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 22:07:08.601895 foundry_ml-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-11 22:06:55.000000 foundry_ml-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-05-11 22:07:08.601895 foundry_ml-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-05-11 22:06:55.000000 foundry_ml-0.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 22:07:08.597895 foundry_ml-0.6.2/foundry/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-11 22:06:55.000000 foundry_ml-0.6.2/foundry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-11 22:06:55.000000 foundry_ml-0.6.2/foundry/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    33352 2023-05-11 22:06:55.000000 foundry_ml-0.6.2/foundry/foundry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-05-11 22:06:55.000000 foundry_ml-0.6.2/foundry/https_download.py
--rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-05-11 22:06:55.000000 foundry_ml-0.6.2/foundry/https_upload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 22:07:08.597895 foundry_ml-0.6.2/foundry/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 22:06:55.000000 foundry_ml-0.6.2/foundry/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-11 22:06:55.000000 foundry_ml-0.6.2/foundry/loaders/tf_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-11 22:06:55.000000 foundry_ml-0.6.2/foundry/loaders/torch_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-05-11 22:06:55.000000 foundry_ml-0.6.2/foundry/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-11 22:06:55.000000 foundry_ml-0.6.2/foundry/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 22:07:08.597895 foundry_ml-0.6.2/foundry_ml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-05-11 22:07:08.000000 foundry_ml-0.6.2/foundry_ml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-11 22:07:08.000000 foundry_ml-0.6.2/foundry_ml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 22:07:08.000000 foundry_ml-0.6.2/foundry_ml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-11 22:07:08.000000 foundry_ml-0.6.2/foundry_ml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-11 22:07:08.000000 foundry_ml-0.6.2/foundry_ml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-11 22:07:08.601895 foundry_ml-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-05-11 22:06:55.000000 foundry_ml-0.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 22:07:08.601895 foundry_ml-0.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 22:06:55.000000 foundry_ml-0.6.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13966 2023-05-11 22:06:55.000000 foundry_ml-0.6.2/tests/test_foundry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:13:23.451231 foundry_ml-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-24 21:13:10.000000 foundry_ml-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-05-24 21:13:23.451231 foundry_ml-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-05-24 21:13:10.000000 foundry_ml-0.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:13:23.451231 foundry_ml-0.6.3/foundry/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-24 21:13:10.000000 foundry_ml-0.6.3/foundry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-24 21:13:10.000000 foundry_ml-0.6.3/foundry/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33352 2023-05-24 21:13:10.000000 foundry_ml-0.6.3/foundry/foundry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-05-24 21:13:10.000000 foundry_ml-0.6.3/foundry/https_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-05-24 21:13:10.000000 foundry_ml-0.6.3/foundry/https_upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:13:23.451231 foundry_ml-0.6.3/foundry/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 21:13:10.000000 foundry_ml-0.6.3/foundry/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-24 21:13:10.000000 foundry_ml-0.6.3/foundry/loaders/tf_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-24 21:13:10.000000 foundry_ml-0.6.3/foundry/loaders/torch_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-05-24 21:13:10.000000 foundry_ml-0.6.3/foundry/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-24 21:13:10.000000 foundry_ml-0.6.3/foundry/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:13:23.451231 foundry_ml-0.6.3/foundry_ml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-05-24 21:13:23.000000 foundry_ml-0.6.3/foundry_ml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-24 21:13:23.000000 foundry_ml-0.6.3/foundry_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 21:13:23.000000 foundry_ml-0.6.3/foundry_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-24 21:13:23.000000 foundry_ml-0.6.3/foundry_ml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-24 21:13:23.000000 foundry_ml-0.6.3/foundry_ml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-24 21:13:23.451231 foundry_ml-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-05-24 21:13:10.000000 foundry_ml-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:13:23.451231 foundry_ml-0.6.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 21:13:10.000000 foundry_ml-0.6.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13966 2023-05-24 21:13:10.000000 foundry_ml-0.6.3/tests/test_foundry.py
```

### Comparing `foundry_ml-0.6.2/LICENSE` & `foundry_ml-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `foundry_ml-0.6.2/PKG-INFO` & `foundry_ml-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foundry_ml
-Version: 0.6.2
+Version: 0.6.3
 Summary: Package to support simplified application of machine learning models to datasets in materials science
 Home-page: https://github.com/MLMI2-CSSI/foundry
 Author: Aristana Scourtas, KJ Schmidt, Isaac Darling, Aadit Ambadkar, Braeden Cullen,
             Imogen Foster, Ribhav Bose, Zoa Katok, Ethan Truelove, Ian Foster, Ben Blaiszik
 Author-email: blaiszik@uchicago.edu
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `foundry_ml-0.6.2/README.md` & `foundry_ml-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `foundry_ml-0.6.2/foundry/auth.py` & `foundry_ml-0.6.3/foundry/auth.py`

 * *Files identical despite different names*

### Comparing `foundry_ml-0.6.2/foundry/foundry.py` & `foundry_ml-0.6.3/foundry/foundry.py`

 * *Files identical despite different names*

### Comparing `foundry_ml-0.6.2/foundry/https_download.py` & `foundry_ml-0.6.3/foundry/https_download.py`

 * *Files identical despite different names*

### Comparing `foundry_ml-0.6.2/foundry/https_upload.py` & `foundry_ml-0.6.3/foundry/https_upload.py`

 * *Files identical despite different names*

### Comparing `foundry_ml-0.6.2/foundry/loaders/tf_wrapper.py` & `foundry_ml-0.6.3/foundry/loaders/tf_wrapper.py`

 * *Files identical despite different names*

### Comparing `foundry_ml-0.6.2/foundry/loaders/torch_wrapper.py` & `foundry_ml-0.6.3/foundry/loaders/torch_wrapper.py`

 * *Files identical despite different names*

### Comparing `foundry_ml-0.6.2/foundry/models.py` & `foundry_ml-0.6.3/foundry/models.py`

 * *Files identical despite different names*

### Comparing `foundry_ml-0.6.2/foundry/utils.py` & `foundry_ml-0.6.3/foundry/utils.py`

 * *Files identical despite different names*

### Comparing `foundry_ml-0.6.2/foundry_ml.egg-info/PKG-INFO` & `foundry_ml-0.6.3/foundry_ml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foundry-ml
-Version: 0.6.2
+Version: 0.6.3
 Summary: Package to support simplified application of machine learning models to datasets in materials science
 Home-page: https://github.com/MLMI2-CSSI/foundry
 Author: Aristana Scourtas, KJ Schmidt, Isaac Darling, Aadit Ambadkar, Braeden Cullen,
             Imogen Foster, Ribhav Bose, Zoa Katok, Ethan Truelove, Ian Foster, Ben Blaiszik
 Author-email: blaiszik@uchicago.edu
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `foundry_ml-0.6.2/setup.py` & `foundry_ml-0.6.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 packages = (setuptools.find_packages(),)
 setuptools.setup(
     name="foundry_ml",
-    version="0.6.2",
+    version="0.6.3",
     author="""Aristana Scourtas, KJ Schmidt, Isaac Darling, Aadit Ambadkar, Braeden Cullen,
             Imogen Foster, Ribhav Bose, Zoa Katok, Ethan Truelove, Ian Foster, Ben Blaiszik""",
     author_email="blaiszik@uchicago.edu",
     packages=setuptools.find_packages(),
     description="Package to support simplified application of machine learning models to datasets in materials science",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `foundry_ml-0.6.2/tests/test_foundry.py` & `foundry_ml-0.6.3/tests/test_foundry.py`

 * *Files identical despite different names*

