# Comparing `tmp/py-gutenberg-1.0.1.tar.gz` & `tmp/py-gutenberg-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-gutenberg-1.0.1.tar", last modified: Mon May 22 20:16:35 2023, max compression
+gzip compressed data, was "py-gutenberg-1.0.2.tar", last modified: Wed May 24 14:08:24 2023, max compression
```

## Comparing `py-gutenberg-1.0.1.tar` & `py-gutenberg-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:16:35.787004 py-gutenberg-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-22 20:16:15.000000 py-gutenberg-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-05-22 20:16:35.787004 py-gutenberg-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-05-22 20:16:15.000000 py-gutenberg-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-22 20:16:15.000000 py-gutenberg-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 20:16:35.787004 py-gutenberg-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:16:35.787004 py-gutenberg-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:16:35.787004 py-gutenberg-1.0.1/src/gutenberg/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-22 20:16:15.000000 py-gutenberg-1.0.1/src/gutenberg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-05-22 20:16:15.000000 py-gutenberg-1.0.1/src/gutenberg/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-05-22 20:16:15.000000 py-gutenberg-1.0.1/src/gutenberg/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:16:35.787004 py-gutenberg-1.0.1/src/py_gutenberg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-05-22 20:16:35.000000 py-gutenberg-1.0.1/src/py_gutenberg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-22 20:16:35.000000 py-gutenberg-1.0.1/src/py_gutenberg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 20:16:35.000000 py-gutenberg-1.0.1/src/py_gutenberg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-22 20:16:35.000000 py-gutenberg-1.0.1/src/py_gutenberg.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:16:35.787004 py-gutenberg-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-22 20:16:15.000000 py-gutenberg-1.0.1/tests/test_gutenberg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:08:24.483767 py-gutenberg-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-24 14:08:08.000000 py-gutenberg-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-05-24 14:08:24.483767 py-gutenberg-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-05-24 14:08:08.000000 py-gutenberg-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-24 14:08:08.000000 py-gutenberg-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 14:08:24.483767 py-gutenberg-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:08:24.479767 py-gutenberg-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:08:24.479767 py-gutenberg-1.0.2/src/gutenberg/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-24 14:08:08.000000 py-gutenberg-1.0.2/src/gutenberg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-05-24 14:08:08.000000 py-gutenberg-1.0.2/src/gutenberg/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-05-24 14:08:08.000000 py-gutenberg-1.0.2/src/gutenberg/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:08:24.479767 py-gutenberg-1.0.2/src/py_gutenberg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-05-24 14:08:24.000000 py-gutenberg-1.0.2/src/py_gutenberg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-24 14:08:24.000000 py-gutenberg-1.0.2/src/py_gutenberg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 14:08:24.000000 py-gutenberg-1.0.2/src/py_gutenberg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-24 14:08:24.000000 py-gutenberg-1.0.2/src/py_gutenberg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:08:24.483767 py-gutenberg-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-24 14:08:08.000000 py-gutenberg-1.0.2/tests/test_gutenberg.py
```

### Comparing `py-gutenberg-1.0.1/LICENSE` & `py-gutenberg-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py-gutenberg-1.0.1/PKG-INFO` & `py-gutenberg-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-gutenberg
-Version: 1.0.1
+Version: 1.0.2
 Summary: A library to access the Project Gutenberg API
 Author-email: Peter Rauscher <peterrauscher@protonmail.com>
 Project-URL: Homepage, https://github.com/peterrauscher/gutenberg-py
 Project-URL: Bug Tracker, https://github.com/peterrauscher/gutenberg-py/issues
 Project-URL: Source Code, https://github.com/peterrauscher/gutenberg-py
 Project-URL: Funding, https://ko-fi.com/peterrauscher
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `py-gutenberg-1.0.1/README.md` & `py-gutenberg-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `py-gutenberg-1.0.1/pyproject.toml` & `py-gutenberg-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "requests>=2.28.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "py-gutenberg"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Peter Rauscher", email="peterrauscher@protonmail.com" },
 ]
 description = "A library to access the Project Gutenberg API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `py-gutenberg-1.0.1/src/gutenberg/main.py` & `py-gutenberg-1.0.2/src/gutenberg/main.py`

 * *Files identical despite different names*

### Comparing `py-gutenberg-1.0.1/src/gutenberg/models.py` & `py-gutenberg-1.0.2/src/gutenberg/models.py`

 * *Files identical despite different names*

### Comparing `py-gutenberg-1.0.1/src/py_gutenberg.egg-info/PKG-INFO` & `py-gutenberg-1.0.2/src/py_gutenberg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-gutenberg
-Version: 1.0.1
+Version: 1.0.2
 Summary: A library to access the Project Gutenberg API
 Author-email: Peter Rauscher <peterrauscher@protonmail.com>
 Project-URL: Homepage, https://github.com/peterrauscher/gutenberg-py
 Project-URL: Bug Tracker, https://github.com/peterrauscher/gutenberg-py/issues
 Project-URL: Source Code, https://github.com/peterrauscher/gutenberg-py
 Project-URL: Funding, https://ko-fi.com/peterrauscher
 Classifier: Development Status :: 5 - Production/Stable
```

