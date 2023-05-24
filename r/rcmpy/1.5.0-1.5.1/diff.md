# Comparing `tmp/rcmpy-1.5.0.tar.gz` & `tmp/rcmpy-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcmpy-1.5.0.tar", last modified: Tue May 16 02:31:56 2023, max compression
+gzip compressed data, was "rcmpy-1.5.1.tar", last modified: Wed May 24 19:53:23 2023, max compression
```

## Comparing `rcmpy-1.5.0.tar` & `rcmpy-1.5.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:31:56.965894 rcmpy-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-16 02:30:46.000000 rcmpy-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8647 2023-05-16 02:31:56.965894 rcmpy-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-05-16 02:30:46.000000 rcmpy-1.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-16 02:30:46.000000 rcmpy-1.5.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:31:56.961894 rcmpy-1.5.0/rcmpy/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-16 02:30:46.000000 rcmpy-1.5.0/rcmpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-16 02:30:46.000000 rcmpy-1.5.0/rcmpy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-16 02:30:46.000000 rcmpy-1.5.0/rcmpy/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:31:56.961894 rcmpy-1.5.0/rcmpy/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 02:30:46.000000 rcmpy-1.5.0/rcmpy/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-16 02:30:46.000000 rcmpy-1.5.0/rcmpy/commands/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-05-16 02:30:46.000000 rcmpy-1.5.0/rcmpy/commands/apply.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-16 02:30:46.000000 rcmpy-1.5.0/rcmpy/commands/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-16 02:30:46.000000 rcmpy-1.5.0/rcmpy/commands/dump.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-16 02:30:46.000000 rcmpy-1.5.0/rcmpy/commands/use.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-16 02:30:46.000000 rcmpy-1.5.0/rcmpy/commands/variant.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-16 02:30:46.000000 rcmpy-1.5.0/rcmpy/commands/watch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:31:56.961894 rcmpy-1.5.0/rcmpy/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-16 02:30:46.000000 rcmpy-1.5.0/rcmpy/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-05-16 02:30:46.000000 rcmpy-1.5.0/rcmpy/config/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:31:56.957893 rcmpy-1.5.0/rcmpy/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:31:56.965894 rcmpy-1.5.0/rcmpy/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-16 02:30:46.000000 rcmpy-1.5.0/rcmpy/data/schemas/Config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-16 02:30:46.000000 rcmpy-1.5.0/rcmpy/data/schemas/ManagedFile.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-16 02:30:46.000000 rcmpy-1.5.0/rcmpy/data/schemas/State.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-16 02:30:46.000000 rcmpy-1.5.0/rcmpy/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-16 02:30:46.000000 rcmpy-1.5.0/rcmpy/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:31:56.965894 rcmpy-1.5.0/rcmpy/environment/
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-16 02:30:46.000000 rcmpy-1.5.0/rcmpy/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-05-16 02:30:46.000000 rcmpy-1.5.0/rcmpy/environment/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-16 02:30:46.000000 rcmpy-1.5.0/rcmpy/environment/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-05-16 02:30:46.000000 rcmpy-1.5.0/rcmpy/environment/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:31:56.965894 rcmpy-1.5.0/rcmpy/paths/
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-16 02:30:46.000000 rcmpy-1.5.0/rcmpy/paths/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 02:30:46.000000 rcmpy-1.5.0/rcmpy/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 02:30:46.000000 rcmpy-1.5.0/rcmpy/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-16 02:30:46.000000 rcmpy-1.5.0/rcmpy/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:31:56.965894 rcmpy-1.5.0/rcmpy/state/
--rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-05-16 02:30:46.000000 rcmpy-1.5.0/rcmpy/state/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:31:56.965894 rcmpy-1.5.0/rcmpy/watch/
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-05-16 02:30:46.000000 rcmpy-1.5.0/rcmpy/watch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-16 02:30:46.000000 rcmpy-1.5.0/rcmpy/watch/params.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:31:56.965894 rcmpy-1.5.0/rcmpy/xdg/
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-05-16 02:30:46.000000 rcmpy-1.5.0/rcmpy/xdg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:31:56.961894 rcmpy-1.5.0/rcmpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8647 2023-05-16 02:31:56.000000 rcmpy-1.5.0/rcmpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-16 02:31:56.000000 rcmpy-1.5.0/rcmpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 02:31:56.000000 rcmpy-1.5.0/rcmpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-16 02:31:56.000000 rcmpy-1.5.0/rcmpy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-16 02:31:56.000000 rcmpy-1.5.0/rcmpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-16 02:31:56.000000 rcmpy-1.5.0/rcmpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 02:31:56.965894 rcmpy-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-16 02:30:46.000000 rcmpy-1.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:31:56.965894 rcmpy-1.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-16 02:30:46.000000 rcmpy-1.5.0/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-16 02:30:46.000000 rcmpy-1.5.0/tests/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-16 02:30:46.000000 rcmpy-1.5.0/tests/test_xdg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:53:23.830553 rcmpy-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-24 19:51:59.000000 rcmpy-1.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8647 2023-05-24 19:53:23.830553 rcmpy-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-05-24 19:51:59.000000 rcmpy-1.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-24 19:51:59.000000 rcmpy-1.5.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:53:23.826553 rcmpy-1.5.1/rcmpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-24 19:51:59.000000 rcmpy-1.5.1/rcmpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-24 19:51:59.000000 rcmpy-1.5.1/rcmpy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-24 19:51:59.000000 rcmpy-1.5.1/rcmpy/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:53:23.830553 rcmpy-1.5.1/rcmpy/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 19:51:59.000000 rcmpy-1.5.1/rcmpy/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-24 19:51:59.000000 rcmpy-1.5.1/rcmpy/commands/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-05-24 19:51:59.000000 rcmpy-1.5.1/rcmpy/commands/apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-24 19:51:59.000000 rcmpy-1.5.1/rcmpy/commands/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-24 19:51:59.000000 rcmpy-1.5.1/rcmpy/commands/dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-24 19:51:59.000000 rcmpy-1.5.1/rcmpy/commands/use.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-24 19:51:59.000000 rcmpy-1.5.1/rcmpy/commands/variant.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-24 19:51:59.000000 rcmpy-1.5.1/rcmpy/commands/watch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:53:23.830553 rcmpy-1.5.1/rcmpy/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-24 19:51:59.000000 rcmpy-1.5.1/rcmpy/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-05-24 19:51:59.000000 rcmpy-1.5.1/rcmpy/config/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:53:23.826553 rcmpy-1.5.1/rcmpy/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:53:23.830553 rcmpy-1.5.1/rcmpy/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-24 19:51:59.000000 rcmpy-1.5.1/rcmpy/data/schemas/Config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-24 19:51:59.000000 rcmpy-1.5.1/rcmpy/data/schemas/ManagedFile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-24 19:51:59.000000 rcmpy-1.5.1/rcmpy/data/schemas/State.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-24 19:51:59.000000 rcmpy-1.5.1/rcmpy/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-24 19:51:59.000000 rcmpy-1.5.1/rcmpy/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:53:23.830553 rcmpy-1.5.1/rcmpy/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-24 19:51:59.000000 rcmpy-1.5.1/rcmpy/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-05-24 19:51:59.000000 rcmpy-1.5.1/rcmpy/environment/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-24 19:51:59.000000 rcmpy-1.5.1/rcmpy/environment/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-05-24 19:51:59.000000 rcmpy-1.5.1/rcmpy/environment/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:53:23.830553 rcmpy-1.5.1/rcmpy/paths/
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-24 19:51:59.000000 rcmpy-1.5.1/rcmpy/paths/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 19:51:59.000000 rcmpy-1.5.1/rcmpy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-24 19:51:59.000000 rcmpy-1.5.1/rcmpy/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-24 19:51:59.000000 rcmpy-1.5.1/rcmpy/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:53:23.830553 rcmpy-1.5.1/rcmpy/state/
+-rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-05-24 19:51:59.000000 rcmpy-1.5.1/rcmpy/state/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:53:23.830553 rcmpy-1.5.1/rcmpy/watch/
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-05-24 19:51:59.000000 rcmpy-1.5.1/rcmpy/watch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-24 19:51:59.000000 rcmpy-1.5.1/rcmpy/watch/params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:53:23.830553 rcmpy-1.5.1/rcmpy/xdg/
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-05-24 19:51:59.000000 rcmpy-1.5.1/rcmpy/xdg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:53:23.826553 rcmpy-1.5.1/rcmpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8647 2023-05-24 19:53:23.000000 rcmpy-1.5.1/rcmpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-24 19:53:23.000000 rcmpy-1.5.1/rcmpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 19:53:23.000000 rcmpy-1.5.1/rcmpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-24 19:53:23.000000 rcmpy-1.5.1/rcmpy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-24 19:53:23.000000 rcmpy-1.5.1/rcmpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-24 19:53:23.000000 rcmpy-1.5.1/rcmpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 19:53:23.830553 rcmpy-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-24 19:51:59.000000 rcmpy-1.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:53:23.830553 rcmpy-1.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-24 19:51:59.000000 rcmpy-1.5.1/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-24 19:51:59.000000 rcmpy-1.5.1/tests/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-24 19:51:59.000000 rcmpy-1.5.1/tests/test_xdg.py
```

### Comparing `rcmpy-1.5.0/LICENSE` & `rcmpy-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.0/PKG-INFO` & `rcmpy-1.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcmpy
-Version: 1.5.0
+Version: 1.5.1
 Summary: A configuration-file management system.
 Home-page: https://github.com/vkottler/rcmpy
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=8bb20a7e710e9071d4cf11a5f065e18e
+    hash=744ace272d6f05ecee63ea172bf1a6bd
     =====================================
 -->
 
-# rcmpy ([1.5.0](https://pypi.org/project/rcmpy/))
+# rcmpy ([1.5.1](https://pypi.org/project/rcmpy/))
 
 [![python](https://img.shields.io/pypi/pyversions/rcmpy.svg)](https://pypi.org/project/rcmpy/)
 ![Build Status](https://github.com/vkottler/rcmpy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/rcmpy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/rcmpy)
 ![PyPI - Status](https://img.shields.io/pypi/status/rcmpy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/rcmpy)
```

### Comparing `rcmpy-1.5.0/README.md` & `rcmpy-1.5.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=8bb20a7e710e9071d4cf11a5f065e18e
+    hash=744ace272d6f05ecee63ea172bf1a6bd
     =====================================
 -->
 
-# rcmpy ([1.5.0](https://pypi.org/project/rcmpy/))
+# rcmpy ([1.5.1](https://pypi.org/project/rcmpy/))
 
 [![python](https://img.shields.io/pypi/pyversions/rcmpy.svg)](https://pypi.org/project/rcmpy/)
 ![Build Status](https://github.com/vkottler/rcmpy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/rcmpy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/rcmpy)
 ![PyPI - Status](https://img.shields.io/pypi/status/rcmpy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/rcmpy)
```

### Comparing `rcmpy-1.5.0/pyproject.toml` & `rcmpy-1.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "rcmpy"
-version = "1.5.0"
+version = "1.5.1"
 description = "A configuration-file management system."
 readme = "README.md"
 requires-python = ">=3.7"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `rcmpy-1.5.0/rcmpy/app.py` & `rcmpy-1.5.1/rcmpy/app.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.0/rcmpy/commands/all.py` & `rcmpy-1.5.1/rcmpy/commands/all.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.0/rcmpy/commands/apply.py` & `rcmpy-1.5.1/rcmpy/commands/apply.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.0/rcmpy/commands/common.py` & `rcmpy-1.5.1/rcmpy/commands/common.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.0/rcmpy/commands/dump.py` & `rcmpy-1.5.1/rcmpy/commands/dump.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.0/rcmpy/commands/use.py` & `rcmpy-1.5.1/rcmpy/commands/use.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.0/rcmpy/commands/variant.py` & `rcmpy-1.5.1/rcmpy/commands/variant.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.0/rcmpy/commands/watch.py` & `rcmpy-1.5.1/rcmpy/commands/watch.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.0/rcmpy/config/__init__.py` & `rcmpy-1.5.1/rcmpy/config/__init__.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.0/rcmpy/config/file.py` & `rcmpy-1.5.1/rcmpy/config/file.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,21 +8,15 @@
 from pathlib import Path
 from shutil import copyfile
 import sys
 from typing import Any, Dict, Set
 
 # third-party
 from vcorelib.logging import LoggerType
-from vcorelib.paths import rel
-
-
-def set_exec_flags(path: Path) -> None:
-    """Set the executable bits, but respect the 'read' bits."""
-    mode = path.stat().st_mode
-    path.chmod(mode | ((mode & 0o444) >> 2))
+from vcorelib.paths import rel, set_exec_flags
 
 
 @dataclass
 class ManagedFile:
     """
     A data structure for managed files specified in the configuration data.
     """
```

### Comparing `rcmpy-1.5.0/rcmpy/data/schemas/ManagedFile.yaml` & `rcmpy-1.5.1/rcmpy/data/schemas/ManagedFile.yaml`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.0/rcmpy/entry.py` & `rcmpy-1.5.1/rcmpy/entry.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.0/rcmpy/environment/__init__.py` & `rcmpy-1.5.1/rcmpy/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.0/rcmpy/environment/base.py` & `rcmpy-1.5.1/rcmpy/environment/base.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.0/rcmpy/environment/data.py` & `rcmpy-1.5.1/rcmpy/environment/data.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.0/rcmpy/environment/template.py` & `rcmpy-1.5.1/rcmpy/environment/template.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.0/rcmpy/paths/__init__.py` & `rcmpy-1.5.1/rcmpy/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.0/rcmpy/schemas.py` & `rcmpy-1.5.1/rcmpy/schemas.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.0/rcmpy/state/__init__.py` & `rcmpy-1.5.1/rcmpy/state/__init__.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.0/rcmpy/watch/__init__.py` & `rcmpy-1.5.1/rcmpy/watch/__init__.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.0/rcmpy/watch/params.py` & `rcmpy-1.5.1/rcmpy/watch/params.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.0/rcmpy/xdg/__init__.py` & `rcmpy-1.5.1/rcmpy/xdg/__init__.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.0/rcmpy.egg-info/PKG-INFO` & `rcmpy-1.5.1/rcmpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcmpy
-Version: 1.5.0
+Version: 1.5.1
 Summary: A configuration-file management system.
 Home-page: https://github.com/vkottler/rcmpy
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=8bb20a7e710e9071d4cf11a5f065e18e
+    hash=744ace272d6f05ecee63ea172bf1a6bd
     =====================================
 -->
 
-# rcmpy ([1.5.0](https://pypi.org/project/rcmpy/))
+# rcmpy ([1.5.1](https://pypi.org/project/rcmpy/))
 
 [![python](https://img.shields.io/pypi/pyversions/rcmpy.svg)](https://pypi.org/project/rcmpy/)
 ![Build Status](https://github.com/vkottler/rcmpy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/rcmpy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/rcmpy)
 ![PyPI - Status](https://img.shields.io/pypi/status/rcmpy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/rcmpy)
```

### Comparing `rcmpy-1.5.0/rcmpy.egg-info/SOURCES.txt` & `rcmpy-1.5.1/rcmpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.0/setup.py` & `rcmpy-1.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.0/tests/test_entry.py` & `rcmpy-1.5.1/tests/test_entry.py`

 * *Files identical despite different names*

