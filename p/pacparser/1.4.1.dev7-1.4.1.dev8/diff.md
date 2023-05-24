# Comparing `tmp/pacparser-1.4.1.dev7.tar.gz` & `tmp/pacparser-1.4.1.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pacparser-1.4.1.dev7.tar", last modified: Wed May 24 05:24:19 2023, max compression
+gzip compressed data, was "pacparser-1.4.1.dev8.tar", last modified: Wed May 24 05:30:08 2023, max compression
```

## Comparing `pacparser-1.4.1.dev7.tar` & `pacparser-1.4.1.dev8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 05:24:19.905440 pacparser-1.4.1.dev7/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-24 05:23:50.000000 pacparser-1.4.1.dev7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-24 05:24:19.905440 pacparser-1.4.1.dev7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 05:24:19.905440 pacparser-1.4.1.dev7/pacparser/
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-05-24 05:23:50.000000 pacparser-1.4.1.dev7/pacparser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 05:24:19.905440 pacparser-1.4.1.dev7/pacparser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-24 05:24:19.000000 pacparser-1.4.1.dev7/pacparser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-24 05:24:19.000000 pacparser-1.4.1.dev7/pacparser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 05:24:19.000000 pacparser-1.4.1.dev7/pacparser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-24 05:24:19.000000 pacparser-1.4.1.dev7/pacparser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-05-24 05:23:50.000000 pacparser-1.4.1.dev7/pacparser_py.c
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 05:24:19.905440 pacparser-1.4.1.dev7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-05-24 05:23:50.000000 pacparser-1.4.1.dev7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 05:30:08.490475 pacparser-1.4.1.dev8/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-24 05:29:58.000000 pacparser-1.4.1.dev8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-24 05:30:08.490475 pacparser-1.4.1.dev8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 05:30:08.482475 pacparser-1.4.1.dev8/pacparser/
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-05-24 05:29:58.000000 pacparser-1.4.1.dev8/pacparser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 05:30:08.490475 pacparser-1.4.1.dev8/pacparser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-24 05:30:08.000000 pacparser-1.4.1.dev8/pacparser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-24 05:30:08.000000 pacparser-1.4.1.dev8/pacparser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 05:30:08.000000 pacparser-1.4.1.dev8/pacparser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-24 05:30:08.000000 pacparser-1.4.1.dev8/pacparser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-05-24 05:29:58.000000 pacparser-1.4.1.dev8/pacparser_py.c
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 05:30:08.490475 pacparser-1.4.1.dev8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-05-24 05:29:58.000000 pacparser-1.4.1.dev8/setup.py
```

### Comparing `pacparser-1.4.1.dev7/pacparser/__init__.py` & `pacparser-1.4.1.dev8/pacparser/__init__.py`

 * *Files identical despite different names*

### Comparing `pacparser-1.4.1.dev7/pacparser_py.c` & `pacparser-1.4.1.dev8/pacparser_py.c`

 * *Files identical despite different names*

### Comparing `pacparser-1.4.1.dev7/setup.py` & `pacparser-1.4.1.dev8/setup.py`

 * *Files identical despite different names*

