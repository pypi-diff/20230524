# Comparing `tmp/trove-classifiers-2023.5.22.tar.gz` & `tmp/trove-classifiers-2023.5.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trove-classifiers-2023.5.22.tar", last modified: Mon May 22 23:06:28 2023, max compression
+gzip compressed data, was "trove-classifiers-2023.5.24.tar", last modified: Wed May 24 15:35:47 2023, max compression
```

## Comparing `trove-classifiers-2023.5.22.tar` & `trove-classifiers-2023.5.24.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:06:28.730424 trove-classifiers-2023.5.22/
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-22 23:05:50.000000 trove-classifiers-2023.5.22/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-22 23:05:50.000000 trove-classifiers-2023.5.22/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-22 23:05:50.000000 trove-classifiers-2023.5.22/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-22 23:05:50.000000 trove-classifiers-2023.5.22/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-05-22 23:06:28.730424 trove-classifiers-2023.5.22/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-22 23:05:50.000000 trove-classifiers-2023.5.22/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:06:28.726424 trove-classifiers-2023.5.22/bin/
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-22 23:05:50.000000 trove-classifiers-2023.5.22/bin/sort.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-22 23:05:50.000000 trove-classifiers-2023.5.22/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:06:28.726424 trove-classifiers-2023.5.22/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-22 23:05:50.000000 trove-classifiers-2023.5.22/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 23:06:28.730424 trove-classifiers-2023.5.22/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-22 23:05:50.000000 trove-classifiers-2023.5.22/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:06:28.722424 trove-classifiers-2023.5.22/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:06:28.726424 trove-classifiers-2023.5.22/src/trove_classifiers/
--rw-r--r--   0 runner    (1001) docker     (123)    40050 2023-05-22 23:05:50.000000 trove-classifiers-2023.5.22/src/trove_classifiers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-22 23:05:50.000000 trove-classifiers-2023.5.22/src/trove_classifiers/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 23:05:50.000000 trove-classifiers-2023.5.22/src/trove_classifiers/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:06:28.726424 trove-classifiers-2023.5.22/src/trove_classifiers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-05-22 23:06:28.000000 trove-classifiers-2023.5.22/src/trove_classifiers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-22 23:06:28.000000 trove-classifiers-2023.5.22/src/trove_classifiers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 23:06:28.000000 trove-classifiers-2023.5.22/src/trove_classifiers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-22 23:06:28.000000 trove-classifiers-2023.5.22/src/trove_classifiers.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:06:28.726424 trove-classifiers-2023.5.22/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 23:05:50.000000 trove-classifiers-2023.5.22/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:06:28.726424 trove-classifiers-2023.5.22/tests/lib/
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-22 23:05:50.000000 trove-classifiers-2023.5.22/tests/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-22 23:05:50.000000 trove-classifiers-2023.5.22/tests/lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-05-22 23:05:50.000000 trove-classifiers-2023.5.22/tests/test_classifiers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:35:47.236750 trove-classifiers-2023.5.24/
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-24 15:35:19.000000 trove-classifiers-2023.5.24/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-24 15:35:19.000000 trove-classifiers-2023.5.24/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-24 15:35:19.000000 trove-classifiers-2023.5.24/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-24 15:35:19.000000 trove-classifiers-2023.5.24/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-05-24 15:35:47.236750 trove-classifiers-2023.5.24/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-24 15:35:19.000000 trove-classifiers-2023.5.24/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:35:47.232750 trove-classifiers-2023.5.24/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-24 15:35:19.000000 trove-classifiers-2023.5.24/bin/sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-24 15:35:19.000000 trove-classifiers-2023.5.24/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:35:47.232750 trove-classifiers-2023.5.24/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-24 15:35:19.000000 trove-classifiers-2023.5.24/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 15:35:47.236750 trove-classifiers-2023.5.24/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-24 15:35:19.000000 trove-classifiers-2023.5.24/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:35:47.232750 trove-classifiers-2023.5.24/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:35:47.232750 trove-classifiers-2023.5.24/src/trove_classifiers/
+-rw-r--r--   0 runner    (1001) docker     (123)    40085 2023-05-24 15:35:19.000000 trove-classifiers-2023.5.24/src/trove_classifiers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-24 15:35:19.000000 trove-classifiers-2023.5.24/src/trove_classifiers/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:35:19.000000 trove-classifiers-2023.5.24/src/trove_classifiers/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:35:47.232750 trove-classifiers-2023.5.24/src/trove_classifiers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-05-24 15:35:47.000000 trove-classifiers-2023.5.24/src/trove_classifiers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-24 15:35:47.000000 trove-classifiers-2023.5.24/src/trove_classifiers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:35:47.000000 trove-classifiers-2023.5.24/src/trove_classifiers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-24 15:35:47.000000 trove-classifiers-2023.5.24/src/trove_classifiers.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:35:47.232750 trove-classifiers-2023.5.24/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:35:19.000000 trove-classifiers-2023.5.24/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:35:47.236750 trove-classifiers-2023.5.24/tests/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-24 15:35:19.000000 trove-classifiers-2023.5.24/tests/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-24 15:35:19.000000 trove-classifiers-2023.5.24/tests/lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-05-24 15:35:19.000000 trove-classifiers-2023.5.24/tests/test_classifiers.py
```

### Comparing `trove-classifiers-2023.5.22/CONTRIBUTING.md` & `trove-classifiers-2023.5.24/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `trove-classifiers-2023.5.22/LICENSE` & `trove-classifiers-2023.5.24/LICENSE`

 * *Files identical despite different names*

### Comparing `trove-classifiers-2023.5.22/Makefile` & `trove-classifiers-2023.5.24/Makefile`

 * *Files identical despite different names*

### Comparing `trove-classifiers-2023.5.22/PKG-INFO` & `trove-classifiers-2023.5.24/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trove-classifiers
-Version: 2023.5.22
+Version: 2023.5.24
 Summary: Canonical source for classifiers on PyPI (pypi.org).
 Home-page: https://github.com/pypa/trove-classifiers
 Author: The PyPI Admins
 Author-email: admin@pypi.org
 Keywords: classifiers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `trove-classifiers-2023.5.22/README.md` & `trove-classifiers-2023.5.24/README.md`

 * *Files identical despite different names*

### Comparing `trove-classifiers-2023.5.22/bin/sort.py` & `trove-classifiers-2023.5.24/bin/sort.py`

 * *Files identical despite different names*

### Comparing `trove-classifiers-2023.5.22/setup.py` & `trove-classifiers-2023.5.24/setup.py`

 * *Files identical despite different names*

### Comparing `trove-classifiers-2023.5.22/src/trove_classifiers/__init__.py` & `trove-classifiers-2023.5.24/src/trove_classifiers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -452,14 +452,15 @@
     "Programming Language :: Fortran",
     "Programming Language :: Haskell",
     "Programming Language :: Java",
     "Programming Language :: JavaScript",
     "Programming Language :: Kotlin",
     "Programming Language :: Lisp",
     "Programming Language :: Logo",
+    "Programming Language :: Lua",
     "Programming Language :: ML",
     "Programming Language :: Modula",
     "Programming Language :: OCaml",
     "Programming Language :: Object Pascal",
     "Programming Language :: Objective C",
     "Programming Language :: Other",
     "Programming Language :: Other Scripting Engines",
```

### Comparing `trove-classifiers-2023.5.22/src/trove_classifiers.egg-info/PKG-INFO` & `trove-classifiers-2023.5.24/src/trove_classifiers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trove-classifiers
-Version: 2023.5.22
+Version: 2023.5.24
 Summary: Canonical source for classifiers on PyPI (pypi.org).
 Home-page: https://github.com/pypa/trove-classifiers
 Author: The PyPI Admins
 Author-email: admin@pypi.org
 Keywords: classifiers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `trove-classifiers-2023.5.22/tests/lib/__init__.py` & `trove-classifiers-2023.5.24/tests/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `trove-classifiers-2023.5.22/tests/test_classifiers.py` & `trove-classifiers-2023.5.24/tests/test_classifiers.py`

 * *Files identical despite different names*

