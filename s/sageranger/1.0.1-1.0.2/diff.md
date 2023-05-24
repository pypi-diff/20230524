# Comparing `tmp/sageranger-1.0.1.tar.gz` & `tmp/sageranger-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sageranger-1.0.1.tar", last modified: Wed May 24 18:49:34 2023, max compression
+gzip compressed data, was "sageranger-1.0.2.tar", last modified: Wed May 24 19:01:22 2023, max compression
```

## Comparing `sageranger-1.0.1.tar` & `sageranger-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 katie     (1000) katie     (1000)        0 2023-05-24 18:49:34.933669 sageranger-1.0.1/
--rw-rw-r--   0 katie     (1000) katie     (1000)     1084 2023-05-24 18:18:08.000000 sageranger-1.0.1/LICENSE
--rw-rw-r--   0 katie     (1000) katie     (1000)     1928 2023-05-24 18:49:34.933669 sageranger-1.0.1/PKG-INFO
--rw-rw-r--   0 katie     (1000) katie     (1000)      156 2023-05-24 18:22:24.000000 sageranger-1.0.1/README.md
--rw-rw-r--   0 katie     (1000) katie     (1000)      757 2023-05-24 18:48:45.000000 sageranger-1.0.1/pyproject.toml
-drwxrwxr-x   0 katie     (1000) katie     (1000)        0 2023-05-24 18:49:34.933669 sageranger-1.0.1/sageranger/
--rw-rw-r--   0 katie     (1000) katie     (1000)      220 2023-05-24 18:42:52.000000 sageranger-1.0.1/sageranger/__init__.py
--rw-rw-r--   0 katie     (1000) katie     (1000)     1573 2023-05-04 16:02:14.000000 sageranger-1.0.1/sageranger/attach_image_er.py
--rw-rw-r--   0 katie     (1000) katie     (1000)     1395 2023-05-04 16:02:14.000000 sageranger-1.0.1/sageranger/get_cam_location.py
--rw-rw-r--   0 katie     (1000) katie     (1000)     2031 2023-05-22 18:27:58.000000 sageranger-1.0.1/sageranger/post_cougar_log.py
--rw-rw-r--   0 katie     (1000) katie     (1000)     2334 2023-05-22 18:28:14.000000 sageranger-1.0.1/sageranger/post_event_er.py
-drwxrwxr-x   0 katie     (1000) katie     (1000)        0 2023-05-24 18:49:34.933669 sageranger-1.0.1/sageranger.egg-info/
--rw-rw-r--   0 katie     (1000) katie     (1000)     1928 2023-05-24 18:49:34.000000 sageranger-1.0.1/sageranger.egg-info/PKG-INFO
--rw-rw-r--   0 katie     (1000) katie     (1000)      343 2023-05-24 18:49:34.000000 sageranger-1.0.1/sageranger.egg-info/SOURCES.txt
--rw-rw-r--   0 katie     (1000) katie     (1000)        1 2023-05-24 18:49:34.000000 sageranger-1.0.1/sageranger.egg-info/dependency_links.txt
--rw-rw-r--   0 katie     (1000) katie     (1000)       25 2023-05-24 18:49:34.000000 sageranger-1.0.1/sageranger.egg-info/requires.txt
--rw-rw-r--   0 katie     (1000) katie     (1000)       11 2023-05-24 18:49:34.000000 sageranger-1.0.1/sageranger.egg-info/top_level.txt
--rw-rw-r--   0 katie     (1000) katie     (1000)       38 2023-05-24 18:49:34.933669 sageranger-1.0.1/setup.cfg
+drwxrwxr-x   0 katie     (1000) katie     (1000)        0 2023-05-24 19:01:22.720730 sageranger-1.0.2/
+-rw-rw-r--   0 katie     (1000) katie     (1000)     1084 2023-05-24 18:18:08.000000 sageranger-1.0.2/LICENSE
+-rw-rw-r--   0 katie     (1000) katie     (1000)     1964 2023-05-24 19:01:22.720730 sageranger-1.0.2/PKG-INFO
+-rw-rw-r--   0 katie     (1000) katie     (1000)      192 2023-05-24 18:55:09.000000 sageranger-1.0.2/README.md
+-rw-rw-r--   0 katie     (1000) katie     (1000)      757 2023-05-24 19:00:29.000000 sageranger-1.0.2/pyproject.toml
+drwxrwxr-x   0 katie     (1000) katie     (1000)        0 2023-05-24 19:01:22.720730 sageranger-1.0.2/sageranger/
+-rw-rw-r--   0 katie     (1000) katie     (1000)      202 2023-05-24 18:55:09.000000 sageranger-1.0.2/sageranger/__init__.py
+-rw-rw-r--   0 katie     (1000) katie     (1000)     1573 2023-05-24 18:55:09.000000 sageranger-1.0.2/sageranger/attach_image_er.py
+-rw-rw-r--   0 katie     (1000) katie     (1000)     1395 2023-05-24 18:55:09.000000 sageranger-1.0.2/sageranger/get_cam_location.py
+-rw-rw-r--   0 katie     (1000) katie     (1000)     2031 2023-05-24 18:55:09.000000 sageranger-1.0.2/sageranger/post_cougar_log.py
+-rw-rw-r--   0 katie     (1000) katie     (1000)     2334 2023-05-24 18:55:09.000000 sageranger-1.0.2/sageranger/post_event_er.py
+drwxrwxr-x   0 katie     (1000) katie     (1000)        0 2023-05-24 19:01:22.720730 sageranger-1.0.2/sageranger.egg-info/
+-rw-rw-r--   0 katie     (1000) katie     (1000)     1964 2023-05-24 19:01:22.000000 sageranger-1.0.2/sageranger.egg-info/PKG-INFO
+-rw-rw-r--   0 katie     (1000) katie     (1000)      343 2023-05-24 19:01:22.000000 sageranger-1.0.2/sageranger.egg-info/SOURCES.txt
+-rw-rw-r--   0 katie     (1000) katie     (1000)        1 2023-05-24 19:01:22.000000 sageranger-1.0.2/sageranger.egg-info/dependency_links.txt
+-rw-rw-r--   0 katie     (1000) katie     (1000)       25 2023-05-24 19:01:22.000000 sageranger-1.0.2/sageranger.egg-info/requires.txt
+-rw-rw-r--   0 katie     (1000) katie     (1000)       11 2023-05-24 19:01:22.000000 sageranger-1.0.2/sageranger.egg-info/top_level.txt
+-rw-rw-r--   0 katie     (1000) katie     (1000)       38 2023-05-24 19:01:22.720730 sageranger-1.0.2/setup.cfg
```

### Comparing `sageranger-1.0.1/LICENSE` & `sageranger-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sageranger-1.0.1/PKG-INFO` & `sageranger-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sageranger
-Version: 1.0.1
+Version: 1.0.2
 Summary: Package to aide in utilization of Earthranger
 Author-email: Katie Garwood <kgarwood@sdzwa.org>
 License: MIT License
         
         Copyright (c) 2023 Conservation Technology Lab
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -33,7 +33,9 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # sageranger
 A package to aide in the utilization of Earthranger as a way to capture and display data of interest from camera traps and other data loggers.
+Installation
+pip install sageranger
```

### Comparing `sageranger-1.0.1/pyproject.toml` & `sageranger-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sageranger"
-version = "1.0.1"
+version = "1.0.2"
 description = "Package to aide in utilization of Earthranger"
 readme = "README.md"
 authors = [{ name = "Katie Garwood", email = "kgarwood@sdzwa.org" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `sageranger-1.0.1/sageranger/attach_image_er.py` & `sageranger-1.0.2/sageranger/attach_image_er.py`

 * *Files identical despite different names*

### Comparing `sageranger-1.0.1/sageranger/get_cam_location.py` & `sageranger-1.0.2/sageranger/get_cam_location.py`

 * *Files identical despite different names*

### Comparing `sageranger-1.0.1/sageranger/post_cougar_log.py` & `sageranger-1.0.2/sageranger/post_cougar_log.py`

 * *Files identical despite different names*

### Comparing `sageranger-1.0.1/sageranger/post_event_er.py` & `sageranger-1.0.2/sageranger/post_event_er.py`

 * *Files identical despite different names*

### Comparing `sageranger-1.0.1/sageranger.egg-info/PKG-INFO` & `sageranger-1.0.2/sageranger.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sageranger
-Version: 1.0.1
+Version: 1.0.2
 Summary: Package to aide in utilization of Earthranger
 Author-email: Katie Garwood <kgarwood@sdzwa.org>
 License: MIT License
         
         Copyright (c) 2023 Conservation Technology Lab
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -33,7 +33,9 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # sageranger
 A package to aide in the utilization of Earthranger as a way to capture and display data of interest from camera traps and other data loggers.
+Installation
+pip install sageranger
```

