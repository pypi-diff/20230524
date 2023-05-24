# Comparing `tmp/getm-0.0.3.tar.gz` & `tmp/getm-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/getm-0.0.3.tar", last modified: Tue Jun  8 20:19:59 2021, max compression
+gzip compressed data, was "dist/getm-0.0.4.tar", last modified: Tue Jun  8 20:22:58 2021, max compression
```

## Comparing `getm-0.0.3.tar` & `getm-0.0.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2021-06-08 20:19:59.000000 getm-0.0.3/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       88 2021-06-02 15:02:10.000000 getm-0.0.3/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3738 2021-06-08 20:19:59.000000 getm-0.0.3/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2674 2021-06-02 15:02:10.000000 getm-0.0.3/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2021-06-08 20:19:59.000000 getm-0.0.3/getm/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      966 2021-06-02 15:02:10.000000 getm-0.0.3/getm/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5239 2021-06-02 15:02:10.000000 getm-0.0.3/getm/checksum.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11070 2021-06-02 15:02:10.000000 getm-0.0.3/getm/cli.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2021-06-08 20:19:59.000000 getm-0.0.3/getm/concurrent/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      164 2021-06-02 15:02:10.000000 getm-0.0.3/getm/concurrent/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4898 2021-06-02 15:02:10.000000 getm-0.0.3/getm/concurrent/buffers.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5766 2021-06-08 20:03:46.000000 getm-0.0.3/getm/concurrent/collections.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2021-06-08 20:19:59.000000 getm-0.0.3/getm/concurrent/shared_memory_37/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2021-06-02 15:02:10.000000 getm-0.0.3/getm/concurrent/shared_memory_37/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2021-06-08 20:19:59.000000 getm-0.0.3/getm/concurrent/shared_memory_37/clinic/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2353 2021-06-02 15:02:10.000000 getm-0.0.3/getm/concurrent/shared_memory_37/clinic/posixshmem.c.h
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1774 2021-06-02 15:02:10.000000 getm-0.0.3/getm/concurrent/shared_memory_37/posixshmem.c
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18182 2021-06-02 15:02:10.000000 getm-0.0.3/getm/concurrent/shared_memory_37/shared_memory.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5265 2021-06-08 20:00:12.000000 getm-0.0.3/getm/http.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3837 2021-06-02 15:02:10.000000 getm-0.0.3/getm/progress.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11289 2021-06-02 15:02:10.000000 getm-0.0.3/getm/reader.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2483 2021-06-02 15:02:10.000000 getm-0.0.3/getm/utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       22 2021-06-08 20:19:58.000000 getm-0.0.3/getm/version.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2021-06-08 20:19:59.000000 getm-0.0.3/getm.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3738 2021-06-08 20:19:58.000000 getm-0.0.3/getm.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      716 2021-06-08 20:19:59.000000 getm-0.0.3/getm.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2021-06-08 20:19:58.000000 getm-0.0.3/getm.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       40 2021-06-08 20:19:58.000000 getm-0.0.3/getm.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2021-06-08 20:11:25.000000 getm-0.0.3/getm.egg-info/not-zip-safe
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       34 2021-06-08 20:19:58.000000 getm-0.0.3/getm.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       11 2021-06-08 20:19:58.000000 getm-0.0.3/getm.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       34 2021-06-02 15:02:10.000000 getm-0.0.3/requirements.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2021-06-08 20:19:59.000000 getm-0.0.3/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2563 2021-06-02 15:02:10.000000 getm-0.0.3/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2021-06-08 20:19:59.000000 getm-0.0.3/tests/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2021-06-08 20:19:59.000000 getm-0.0.3/tests/infra/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2971 2021-06-02 15:02:10.000000 getm-0.0.3/tests/infra/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      803 2021-06-02 15:02:10.000000 getm-0.0.3/tests/infra/profile.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1298 2021-06-02 15:02:10.000000 getm-0.0.3/tests/infra/server.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2021-06-08 20:22:58.000000 getm-0.0.4/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       88 2021-06-02 15:02:10.000000 getm-0.0.4/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3738 2021-06-08 20:22:58.000000 getm-0.0.4/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2674 2021-06-02 15:02:10.000000 getm-0.0.4/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2021-06-08 20:22:58.000000 getm-0.0.4/getm/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      966 2021-06-02 15:02:10.000000 getm-0.0.4/getm/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5239 2021-06-02 15:02:10.000000 getm-0.0.4/getm/checksum.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11070 2021-06-02 15:02:10.000000 getm-0.0.4/getm/cli.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2021-06-08 20:22:58.000000 getm-0.0.4/getm/concurrent/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      164 2021-06-02 15:02:10.000000 getm-0.0.4/getm/concurrent/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4898 2021-06-02 15:02:10.000000 getm-0.0.4/getm/concurrent/buffers.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5766 2021-06-08 20:03:46.000000 getm-0.0.4/getm/concurrent/collections.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2021-06-08 20:22:58.000000 getm-0.0.4/getm/concurrent/shared_memory_37/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2021-06-02 15:02:10.000000 getm-0.0.4/getm/concurrent/shared_memory_37/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2021-06-08 20:22:58.000000 getm-0.0.4/getm/concurrent/shared_memory_37/clinic/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2353 2021-06-02 15:02:10.000000 getm-0.0.4/getm/concurrent/shared_memory_37/clinic/posixshmem.c.h
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1774 2021-06-02 15:02:10.000000 getm-0.0.4/getm/concurrent/shared_memory_37/posixshmem.c
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18182 2021-06-02 15:02:10.000000 getm-0.0.4/getm/concurrent/shared_memory_37/shared_memory.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5265 2021-06-08 20:00:12.000000 getm-0.0.4/getm/http.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3837 2021-06-02 15:02:10.000000 getm-0.0.4/getm/progress.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11289 2021-06-02 15:02:10.000000 getm-0.0.4/getm/reader.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2483 2021-06-02 15:02:10.000000 getm-0.0.4/getm/utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       22 2021-06-08 20:22:58.000000 getm-0.0.4/getm/version.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2021-06-08 20:22:58.000000 getm-0.0.4/getm.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3738 2021-06-08 20:22:58.000000 getm-0.0.4/getm.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      716 2021-06-08 20:22:58.000000 getm-0.0.4/getm.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2021-06-08 20:22:58.000000 getm-0.0.4/getm.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       40 2021-06-08 20:22:58.000000 getm-0.0.4/getm.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2021-06-08 20:22:58.000000 getm-0.0.4/getm.egg-info/not-zip-safe
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       34 2021-06-08 20:22:58.000000 getm-0.0.4/getm.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       11 2021-06-08 20:22:58.000000 getm-0.0.4/getm.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       34 2021-06-02 15:02:10.000000 getm-0.0.4/requirements.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2021-06-08 20:22:58.000000 getm-0.0.4/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2563 2021-06-02 15:02:10.000000 getm-0.0.4/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2021-06-08 20:22:58.000000 getm-0.0.4/tests/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2021-06-08 20:22:58.000000 getm-0.0.4/tests/infra/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2971 2021-06-02 15:02:10.000000 getm-0.0.4/tests/infra/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      803 2021-06-02 15:02:10.000000 getm-0.0.4/tests/infra/profile.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1298 2021-06-02 15:02:10.000000 getm-0.0.4/tests/infra/server.py
```

### Comparing `getm-0.0.3/PKG-INFO` & `getm-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getm
-Version: 0.0.3
+Version: 0.0.4
 Summary: Download data from URLs quickly, with integrity
 Home-page: https://github.com/xbrianh/getm.git
 Author: Brian Hannafious
 Author-email: bhannafi@ucsc.edu
 License: MIT
 Description: # getm: Fast reads with integrity for data URLs
         _getm_ provides fast binary reads for HTTP URLs using
```

### Comparing `getm-0.0.3/README.md` & `getm-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `getm-0.0.3/getm/__init__.py` & `getm-0.0.4/getm/__init__.py`

 * *Files identical despite different names*

### Comparing `getm-0.0.3/getm/checksum.py` & `getm-0.0.4/getm/checksum.py`

 * *Files identical despite different names*

### Comparing `getm-0.0.3/getm/cli.py` & `getm-0.0.4/getm/cli.py`

 * *Files identical despite different names*

### Comparing `getm-0.0.3/getm/concurrent/buffers.py` & `getm-0.0.4/getm/concurrent/buffers.py`

 * *Files identical despite different names*

### Comparing `getm-0.0.3/getm/concurrent/collections.py` & `getm-0.0.4/getm/concurrent/collections.py`

 * *Files identical despite different names*

### Comparing `getm-0.0.3/getm/concurrent/shared_memory_37/clinic/posixshmem.c.h` & `getm-0.0.4/getm/concurrent/shared_memory_37/clinic/posixshmem.c.h`

 * *Files identical despite different names*

### Comparing `getm-0.0.3/getm/concurrent/shared_memory_37/posixshmem.c` & `getm-0.0.4/getm/concurrent/shared_memory_37/posixshmem.c`

 * *Files identical despite different names*

### Comparing `getm-0.0.3/getm/concurrent/shared_memory_37/shared_memory.py` & `getm-0.0.4/getm/concurrent/shared_memory_37/shared_memory.py`

 * *Files identical despite different names*

### Comparing `getm-0.0.3/getm/http.py` & `getm-0.0.4/getm/http.py`

 * *Files identical despite different names*

### Comparing `getm-0.0.3/getm/progress.py` & `getm-0.0.4/getm/progress.py`

 * *Files identical despite different names*

### Comparing `getm-0.0.3/getm/reader.py` & `getm-0.0.4/getm/reader.py`

 * *Files identical despite different names*

### Comparing `getm-0.0.3/getm/utils.py` & `getm-0.0.4/getm/utils.py`

 * *Files identical despite different names*

### Comparing `getm-0.0.3/getm.egg-info/PKG-INFO` & `getm-0.0.4/getm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getm
-Version: 0.0.3
+Version: 0.0.4
 Summary: Download data from URLs quickly, with integrity
 Home-page: https://github.com/xbrianh/getm.git
 Author: Brian Hannafious
 Author-email: bhannafi@ucsc.edu
 License: MIT
 Description: # getm: Fast reads with integrity for data URLs
         _getm_ provides fast binary reads for HTTP URLs using
```

### Comparing `getm-0.0.3/getm.egg-info/SOURCES.txt` & `getm-0.0.4/getm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `getm-0.0.3/setup.py` & `getm-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `getm-0.0.3/tests/infra/__init__.py` & `getm-0.0.4/tests/infra/__init__.py`

 * *Files identical despite different names*

### Comparing `getm-0.0.3/tests/infra/profile.py` & `getm-0.0.4/tests/infra/profile.py`

 * *Files identical despite different names*

### Comparing `getm-0.0.3/tests/infra/server.py` & `getm-0.0.4/tests/infra/server.py`

 * *Files identical despite different names*

