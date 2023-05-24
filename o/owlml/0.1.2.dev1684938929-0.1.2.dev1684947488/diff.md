# Comparing `tmp/owlml-0.1.2.dev1684938929.tar.gz` & `tmp/owlml-0.1.2.dev1684947488.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "owlml-0.1.2.dev1684938929.tar", last modified: Wed May 24 14:35:42 2023, max compression
+gzip compressed data, was "owlml-0.1.2.dev1684947488.tar", last modified: Wed May 24 16:58:20 2023, max compression
```

## Comparing `owlml-0.1.2.dev1684938929.tar` & `owlml-0.1.2.dev1684947488.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:35:42.125939 owlml-0.1.2.dev1684938929/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-24 14:34:01.000000 owlml-0.1.2.dev1684938929/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-24 14:35:42.125939 owlml-0.1.2.dev1684938929/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-24 14:34:01.000000 owlml-0.1.2.dev1684938929/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:35:42.125939 owlml-0.1.2.dev1684938929/owlml/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-24 14:34:01.000000 owlml-0.1.2.dev1684938929/owlml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-24 14:34:01.000000 owlml-0.1.2.dev1684938929/owlml/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-24 14:34:01.000000 owlml-0.1.2.dev1684938929/owlml/annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-24 14:34:01.000000 owlml-0.1.2.dev1684938929/owlml/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-24 14:34:01.000000 owlml-0.1.2.dev1684938929/owlml/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-05-24 14:34:01.000000 owlml-0.1.2.dev1684938929/owlml/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-24 14:34:01.000000 owlml-0.1.2.dev1684938929/owlml/experiments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-24 14:34:01.000000 owlml-0.1.2.dev1684938929/owlml/images.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:35:42.125939 owlml-0.1.2.dev1684938929/owlml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-24 14:35:42.000000 owlml-0.1.2.dev1684938929/owlml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-24 14:35:42.000000 owlml-0.1.2.dev1684938929/owlml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 14:35:42.000000 owlml-0.1.2.dev1684938929/owlml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-24 14:35:42.000000 owlml-0.1.2.dev1684938929/owlml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-24 14:35:42.000000 owlml-0.1.2.dev1684938929/owlml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-24 14:35:42.000000 owlml-0.1.2.dev1684938929/owlml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-24 14:35:42.129940 owlml-0.1.2.dev1684938929/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 14:34:01.000000 owlml-0.1.2.dev1684938929/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:58:20.953276 owlml-0.1.2.dev1684947488/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-24 16:56:49.000000 owlml-0.1.2.dev1684947488/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-24 16:58:20.953276 owlml-0.1.2.dev1684947488/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-24 16:56:49.000000 owlml-0.1.2.dev1684947488/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:58:20.953276 owlml-0.1.2.dev1684947488/owlml/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-24 16:56:49.000000 owlml-0.1.2.dev1684947488/owlml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-24 16:56:49.000000 owlml-0.1.2.dev1684947488/owlml/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-24 16:56:49.000000 owlml-0.1.2.dev1684947488/owlml/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-24 16:56:49.000000 owlml-0.1.2.dev1684947488/owlml/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-24 16:56:49.000000 owlml-0.1.2.dev1684947488/owlml/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-05-24 16:56:49.000000 owlml-0.1.2.dev1684947488/owlml/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-24 16:56:49.000000 owlml-0.1.2.dev1684947488/owlml/experiments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-24 16:56:49.000000 owlml-0.1.2.dev1684947488/owlml/images.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:58:20.953276 owlml-0.1.2.dev1684947488/owlml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-24 16:58:20.000000 owlml-0.1.2.dev1684947488/owlml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-24 16:58:20.000000 owlml-0.1.2.dev1684947488/owlml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 16:58:20.000000 owlml-0.1.2.dev1684947488/owlml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-24 16:58:20.000000 owlml-0.1.2.dev1684947488/owlml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-24 16:58:20.000000 owlml-0.1.2.dev1684947488/owlml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-24 16:58:20.000000 owlml-0.1.2.dev1684947488/owlml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-24 16:58:20.957276 owlml-0.1.2.dev1684947488/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 16:56:49.000000 owlml-0.1.2.dev1684947488/setup.py
```

### Comparing `owlml-0.1.2.dev1684938929/LICENSE` & `owlml-0.1.2.dev1684947488/LICENSE`

 * *Files identical despite different names*

### Comparing `owlml-0.1.2.dev1684938929/README.md` & `owlml-0.1.2.dev1684947488/README.md`

 * *Files identical despite different names*

### Comparing `owlml-0.1.2.dev1684938929/owlml/__main__.py` & `owlml-0.1.2.dev1684947488/owlml/__main__.py`

 * *Files identical despite different names*

### Comparing `owlml-0.1.2.dev1684938929/owlml/annotations.py` & `owlml-0.1.2.dev1684947488/owlml/annotations.py`

 * *Files identical despite different names*

### Comparing `owlml-0.1.2.dev1684938929/owlml/api.py` & `owlml-0.1.2.dev1684947488/owlml/api.py`

 * *Files identical despite different names*

### Comparing `owlml-0.1.2.dev1684938929/owlml/auth.py` & `owlml-0.1.2.dev1684947488/owlml/auth.py`

 * *Files identical despite different names*

### Comparing `owlml-0.1.2.dev1684938929/owlml/datasets.py` & `owlml-0.1.2.dev1684947488/owlml/datasets.py`

 * *Files identical despite different names*

### Comparing `owlml-0.1.2.dev1684938929/owlml/images.py` & `owlml-0.1.2.dev1684947488/owlml/images.py`

 * *Files identical despite different names*

