# Comparing `tmp/blackarrow-1.0.9.tar.gz` & `tmp/blackarrow-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blackarrow-1.0.9.tar", max compression
+gzip compressed data, was "blackarrow-1.1.tar", max compression
```

## Comparing `blackarrow-1.0.9.tar` & `blackarrow-1.1.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1076 2021-07-13 03:29:55.245792 blackarrow-1.0.9/LICENSE.txt
--rw-r--r--   0        0        0     2843 2021-07-13 03:29:55.245792 blackarrow-1.0.9/blackarrow/__init__.py
--rwxr-xr-x   0        0        0     8287 2021-07-13 03:29:55.245792 blackarrow-1.0.9/blackarrow/blackarrow.py
--rw-r--r--   0        0        0        0 2021-07-13 03:29:55.245792 blackarrow-1.0.9/blackarrow/test/__init__.py
--rw-r--r--   0        0        0     1114 2021-07-13 03:29:55.245792 blackarrow-1.0.9/blackarrow/test/test_indexing.py
--rw-r--r--   0        0        0      399 2021-07-13 03:44:41.285744 blackarrow-1.0.9/pyproject.toml
--rw-r--r--   0        0        0      104 2021-07-13 03:29:55.245792 blackarrow-1.0.9/sample/tester.txt
--rw-r--r--   0        0        0      104 2021-07-13 03:29:55.245792 blackarrow-1.0.9/sample/tester2.txt
--rw-r--r--   0        0        0      739 2021-07-13 03:44:47.182091 blackarrow-1.0.9/setup.py
--rw-r--r--   0        0        0      585 2021-07-13 03:44:47.182357 blackarrow-1.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-05-24 04:30:00.135084 blackarrow-1.1/LICENSE.txt
+-rw-r--r--   0        0        0     3222 2023-05-24 04:30:00.135084 blackarrow-1.1/README.md
+-rw-r--r--   0        0        0     2843 2023-05-24 04:30:00.135084 blackarrow-1.1/blackarrow/__init__.py
+-rwxr-xr-x   0        0        0     8320 2023-05-24 04:36:14.235094 blackarrow-1.1/blackarrow/blackarrow.py
+-rw-r--r--   0        0        0        0 2023-05-24 04:30:00.135084 blackarrow-1.1/blackarrow/test/__init__.py
+-rw-r--r--   0        0        0     1114 2023-05-24 04:30:00.135084 blackarrow-1.1/blackarrow/test/test_indexing.py
+-rw-r--r--   0        0        0     1044 2023-05-24 04:36:14.175094 blackarrow-1.1/pyproject.toml
+-rw-r--r--   0        0        0      104 2023-05-24 04:30:00.135084 blackarrow-1.1/sample/tester.txt
+-rw-r--r--   0        0        0      104 2023-05-24 04:30:00.135084 blackarrow-1.1/sample/tester2.txt
+-rw-r--r--   0        0        0     4110 1970-01-01 00:00:00.000000 blackarrow-1.1/setup.py
+-rw-r--r--   0        0        0     4369 1970-01-01 00:00:00.000000 blackarrow-1.1/PKG-INFO
```

### Comparing `blackarrow-1.0.9/LICENSE.txt` & `blackarrow-1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blackarrow-1.0.9/blackarrow/__init__.py` & `blackarrow-1.1/blackarrow/__init__.py`

 * *Files identical despite different names*

### Comparing `blackarrow-1.0.9/blackarrow/blackarrow.py` & `blackarrow-1.1/blackarrow/blackarrow.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,16 @@
     # default to numcores
     # backup is 6 or specified by user
     try:
         numworkers = mp.cpu_count()
     except NotImplementedError:
         numworkers = args.workers or 6
 
+    mp.set_start_method('fork')
+
     search_queue = mp.Queue()
     output = mp.Queue()
     final_queue = mp.Queue()  # Use final queue for external output
     processes = []
 
     indexer = mp.Process(
         name="indexer",
```

### Comparing `blackarrow-1.0.9/blackarrow/test/test_indexing.py` & `blackarrow-1.1/blackarrow/test/test_indexing.py`

 * *Files identical despite different names*

