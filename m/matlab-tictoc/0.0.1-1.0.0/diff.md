# Comparing `tmp/matlab-tictoc-0.0.1.tar.gz` & `tmp/matlab-tictoc-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matlab-tictoc-0.0.1.tar", last modified: Wed May 24 16:19:59 2023, max compression
+gzip compressed data, was "matlab-tictoc-1.0.0.tar", last modified: Wed May 24 16:27:27 2023, max compression
```

## Comparing `matlab-tictoc-0.0.1.tar` & `matlab-tictoc-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-05-24 16:19:59.852425 matlab-tictoc-0.0.1/
--rw-r--r--   0 matt       (501) staff       (20)    11357 2023-05-24 16:03:01.000000 matlab-tictoc-0.0.1/LICENSE
--rw-r--r--   0 matt       (501) staff       (20)     1547 2023-05-24 16:19:59.852302 matlab-tictoc-0.0.1/PKG-INFO
--rw-r--r--   0 matt       (501) staff       (20)     1301 2023-04-14 14:13:31.000000 matlab-tictoc-0.0.1/README.md
--rw-r--r--   0 matt       (501) staff       (20)      395 2023-05-24 16:19:45.000000 matlab-tictoc-0.0.1/pyproject.toml
--rw-r--r--   0 matt       (501) staff       (20)       38 2023-05-24 16:19:59.852460 matlab-tictoc-0.0.1/setup.cfg
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-05-24 16:19:59.850679 matlab-tictoc-0.0.1/src/
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-05-24 16:19:59.851838 matlab-tictoc-0.0.1/src/matlab_tictoc.egg-info/
--rw-r--r--   0 matt       (501) staff       (20)     1547 2023-05-24 16:19:59.000000 matlab-tictoc-0.0.1/src/matlab_tictoc.egg-info/PKG-INFO
--rw-r--r--   0 matt       (501) staff       (20)      240 2023-05-24 16:19:59.000000 matlab-tictoc-0.0.1/src/matlab_tictoc.egg-info/SOURCES.txt
--rw-r--r--   0 matt       (501) staff       (20)        1 2023-05-24 16:19:59.000000 matlab-tictoc-0.0.1/src/matlab_tictoc.egg-info/dependency_links.txt
--rw-r--r--   0 matt       (501) staff       (20)        7 2023-05-24 16:19:59.000000 matlab-tictoc-0.0.1/src/matlab_tictoc.egg-info/top_level.txt
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-05-24 16:19:59.852051 matlab-tictoc-0.0.1/src/tictoc/
--rw-r--r--   0 matt       (501) staff       (20)       64 2023-04-14 13:49:52.000000 matlab-tictoc-0.0.1/src/tictoc/__init__.py
--rw-r--r--   0 matt       (501) staff       (20)     2347 2023-04-14 14:09:06.000000 matlab-tictoc-0.0.1/src/tictoc/tictoc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:27:27.719520 matlab-tictoc-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-24 16:27:18.000000 matlab-tictoc-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-24 16:27:27.719520 matlab-tictoc-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-24 16:27:18.000000 matlab-tictoc-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-24 16:27:18.000000 matlab-tictoc-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 16:27:27.719520 matlab-tictoc-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:27:27.719520 matlab-tictoc-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:27:27.719520 matlab-tictoc-1.0.0/src/matlab_tictoc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-24 16:27:27.000000 matlab-tictoc-1.0.0/src/matlab_tictoc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-24 16:27:27.000000 matlab-tictoc-1.0.0/src/matlab_tictoc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 16:27:27.000000 matlab-tictoc-1.0.0/src/matlab_tictoc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-24 16:27:27.000000 matlab-tictoc-1.0.0/src/matlab_tictoc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:27:27.719520 matlab-tictoc-1.0.0/src/tictoc/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-24 16:27:18.000000 matlab-tictoc-1.0.0/src/tictoc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-05-24 16:27:18.000000 matlab-tictoc-1.0.0/src/tictoc/tictoc.py
```

### Comparing `matlab-tictoc-0.0.1/LICENSE` & `matlab-tictoc-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `matlab-tictoc-0.0.1/PKG-INFO` & `matlab-tictoc-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matlab-tictoc
-Version: 0.0.1
+Version: 1.0.0
 Summary: A timing package that mimics MATLAB's tic and toc functionality
 Author: Matthew Altberg
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Tic Toc
```

### Comparing `matlab-tictoc-0.0.1/README.md` & `matlab-tictoc-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `matlab-tictoc-0.0.1/src/matlab_tictoc.egg-info/PKG-INFO` & `matlab-tictoc-1.0.0/src/matlab_tictoc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matlab-tictoc
-Version: 0.0.1
+Version: 1.0.0
 Summary: A timing package that mimics MATLAB's tic and toc functionality
 Author: Matthew Altberg
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Tic Toc
```

### Comparing `matlab-tictoc-0.0.1/src/tictoc/tictoc.py` & `matlab-tictoc-1.0.0/src/tictoc/tictoc.py`

 * *Files identical despite different names*

