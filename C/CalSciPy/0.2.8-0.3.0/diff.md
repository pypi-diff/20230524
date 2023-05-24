# Comparing `tmp/CalSciPy-0.2.8.tar.gz` & `tmp/CalSciPy-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CalSciPy-0.2.8.tar", last modified: Wed May 24 14:27:40 2023, max compression
+gzip compressed data, was "CalSciPy-0.3.0.tar", last modified: Wed May 24 14:31:11 2023, max compression
```

## Comparing `CalSciPy-0.2.8.tar` & `CalSciPy-0.3.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 14:27:40.474300 CalSciPy-0.2.8/
--rw-rw-rw-   0        0        0     1094 2023-02-20 20:08:47.000000 CalSciPy-0.2.8/LICENSE
--rw-rw-rw-   0        0        0     4947 2023-05-24 14:27:40.464300 CalSciPy-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0     2840 2023-04-03 15:47:56.000000 CalSciPy-0.2.8/README.md
--rw-rw-rw-   0        0        0     2305 2023-05-24 14:05:26.000000 CalSciPy-0.2.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-24 14:27:40.474300 CalSciPy-0.2.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-24 14:27:40.332230 CalSciPy-0.2.8/src/
-drwxrwxrwx   0        0        0        0 2023-05-24 14:27:40.394161 CalSciPy-0.2.8/src/CalSciPy/
--rw-rw-rw-   0        0        0      368 2023-05-24 14:06:12.000000 CalSciPy-0.2.8/src/CalSciPy/__init__.py
--rw-rw-rw-   0        0        0    11488 2023-05-24 14:10:25.000000 CalSciPy-0.2.8/src/CalSciPy/bruker.py
--rw-rw-rw-   0        0        0     3270 2023-05-24 14:25:43.000000 CalSciPy-0.2.8/src/CalSciPy/coloring.py
--rw-rw-rw-   0        0        0     9766 2023-05-24 14:18:29.000000 CalSciPy-0.2.8/src/CalSciPy/event_processing.py
--rw-rw-rw-   0        0        0     4603 2023-05-24 14:11:21.000000 CalSciPy-0.2.8/src/CalSciPy/image_processing.py
--rw-rw-rw-   0        0        0     8973 2023-05-24 14:26:47.000000 CalSciPy-0.2.8/src/CalSciPy/interactive_visuals.py
--rw-rw-rw-   0        0        0     9653 2023-04-26 15:19:07.000000 CalSciPy-0.2.8/src/CalSciPy/io_tools.py
--rw-rw-rw-   0        0        0     7557 2023-05-03 19:58:49.000000 CalSciPy-0.2.8/src/CalSciPy/misc.py
--rw-rw-rw-   0        0        0     3444 2023-03-29 17:06:08.000000 CalSciPy-0.2.8/src/CalSciPy/reorganization.py
--rw-rw-rw-   0        0        0    10311 2023-05-24 14:19:33.000000 CalSciPy-0.2.8/src/CalSciPy/trace_processing.py
--rw-rw-rw-   0        0        0      199 2023-02-20 22:24:54.000000 CalSciPy-0.2.8/src/CalSciPy/version.py
-drwxrwxrwx   0        0        0        0 2023-05-24 14:27:40.414037 CalSciPy-0.2.8/src/CalSciPy.egg-info/
--rw-rw-rw-   0        0        0     4947 2023-05-24 14:27:40.000000 CalSciPy-0.2.8/src/CalSciPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      737 2023-05-24 14:27:40.000000 CalSciPy-0.2.8/src/CalSciPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 14:27:40.000000 CalSciPy-0.2.8/src/CalSciPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      378 2023-05-24 14:27:40.000000 CalSciPy-0.2.8/src/CalSciPy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-24 14:27:40.000000 CalSciPy-0.2.8/src/CalSciPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-02-20 20:08:47.000000 CalSciPy-0.2.8/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-24 14:27:40.464300 CalSciPy-0.2.8/tests/
--rw-rw-rw-   0        0        0     1933 2023-04-03 13:04:29.000000 CalSciPy-0.2.8/tests/test_a_install.py
--rw-rw-rw-   0        0        0     3074 2023-04-05 17:07:30.000000 CalSciPy-0.2.8/tests/test_bruker.py
--rw-rw-rw-   0        0        0      492 2023-05-24 14:14:23.000000 CalSciPy-0.2.8/tests/test_coloring.py
--rw-rw-rw-   0        0        0     1218 2023-04-03 15:39:20.000000 CalSciPy-0.2.8/tests/test_event_processing.py
--rw-rw-rw-   0        0        0    12735 2023-04-05 16:39:27.000000 CalSciPy-0.2.8/tests/test_io_tools.py
--rw-rw-rw-   0        0        0     2373 2023-04-05 15:55:20.000000 CalSciPy-0.2.8/tests/test_misc.py
--rw-rw-rw-   0        0        0     5124 2023-03-29 19:08:15.000000 CalSciPy-0.2.8/tests/test_reorganization.py
--rw-rw-rw-   0        0        0     3250 2023-03-29 21:11:25.000000 CalSciPy-0.2.8/tests/test_trace_processing.py
+drwxrwxrwx   0        0        0        0 2023-05-24 14:31:11.846920 CalSciPy-0.3.0/
+-rw-rw-rw-   0        0        0     1094 2023-02-20 20:08:47.000000 CalSciPy-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0     4947 2023-05-24 14:31:11.844948 CalSciPy-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2840 2023-04-03 15:47:56.000000 CalSciPy-0.3.0/README.md
+-rw-rw-rw-   0        0        0     2303 2023-05-24 14:30:46.000000 CalSciPy-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-24 14:31:11.847954 CalSciPy-0.3.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-24 14:31:11.711637 CalSciPy-0.3.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-24 14:31:11.769629 CalSciPy-0.3.0/src/CalSciPy/
+-rw-rw-rw-   0        0        0      368 2023-05-24 14:06:12.000000 CalSciPy-0.3.0/src/CalSciPy/__init__.py
+-rw-rw-rw-   0        0        0    11488 2023-05-24 14:10:25.000000 CalSciPy-0.3.0/src/CalSciPy/bruker.py
+-rw-rw-rw-   0        0        0     3270 2023-05-24 14:25:43.000000 CalSciPy-0.3.0/src/CalSciPy/coloring.py
+-rw-rw-rw-   0        0        0     9766 2023-05-24 14:18:29.000000 CalSciPy-0.3.0/src/CalSciPy/event_processing.py
+-rw-rw-rw-   0        0        0     4603 2023-05-24 14:11:21.000000 CalSciPy-0.3.0/src/CalSciPy/image_processing.py
+-rw-rw-rw-   0        0        0     8973 2023-05-24 14:26:47.000000 CalSciPy-0.3.0/src/CalSciPy/interactive_visuals.py
+-rw-rw-rw-   0        0        0     9653 2023-04-26 15:19:07.000000 CalSciPy-0.3.0/src/CalSciPy/io_tools.py
+-rw-rw-rw-   0        0        0     7557 2023-05-03 19:58:49.000000 CalSciPy-0.3.0/src/CalSciPy/misc.py
+-rw-rw-rw-   0        0        0     3444 2023-03-29 17:06:08.000000 CalSciPy-0.3.0/src/CalSciPy/reorganization.py
+-rw-rw-rw-   0        0        0    10311 2023-05-24 14:19:33.000000 CalSciPy-0.3.0/src/CalSciPy/trace_processing.py
+-rw-rw-rw-   0        0        0      199 2023-02-20 22:24:54.000000 CalSciPy-0.3.0/src/CalSciPy/version.py
+drwxrwxrwx   0        0        0        0 2023-05-24 14:31:11.794633 CalSciPy-0.3.0/src/CalSciPy.egg-info/
+-rw-rw-rw-   0        0        0     4947 2023-05-24 14:31:11.000000 CalSciPy-0.3.0/src/CalSciPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      737 2023-05-24 14:31:11.000000 CalSciPy-0.3.0/src/CalSciPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 14:31:11.000000 CalSciPy-0.3.0/src/CalSciPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      376 2023-05-24 14:31:11.000000 CalSciPy-0.3.0/src/CalSciPy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-24 14:31:11.000000 CalSciPy-0.3.0/src/CalSciPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-02-20 20:08:47.000000 CalSciPy-0.3.0/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 14:31:11.839926 CalSciPy-0.3.0/tests/
+-rw-rw-rw-   0        0        0     1933 2023-04-03 13:04:29.000000 CalSciPy-0.3.0/tests/test_a_install.py
+-rw-rw-rw-   0        0        0     3074 2023-04-05 17:07:30.000000 CalSciPy-0.3.0/tests/test_bruker.py
+-rw-rw-rw-   0        0        0      492 2023-05-24 14:14:23.000000 CalSciPy-0.3.0/tests/test_coloring.py
+-rw-rw-rw-   0        0        0     1218 2023-04-03 15:39:20.000000 CalSciPy-0.3.0/tests/test_event_processing.py
+-rw-rw-rw-   0        0        0    12735 2023-04-05 16:39:27.000000 CalSciPy-0.3.0/tests/test_io_tools.py
+-rw-rw-rw-   0        0        0     2373 2023-04-05 15:55:20.000000 CalSciPy-0.3.0/tests/test_misc.py
+-rw-rw-rw-   0        0        0     5124 2023-03-29 19:08:15.000000 CalSciPy-0.3.0/tests/test_reorganization.py
+-rw-rw-rw-   0        0        0     3250 2023-03-29 21:11:25.000000 CalSciPy-0.3.0/tests/test_trace_processing.py
```

### Comparing `CalSciPy-0.2.8/LICENSE` & `CalSciPy-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.8/PKG-INFO` & `CalSciPy-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CalSciPy
-Version: 0.2.8
+Version: 0.3.0
 Summary: A collection
 Author: Darik A. O'Neil
 Maintainer: Darik A. O'Neil
 License: MIT License
         
         Copyright (c) 2023 Darik A O’Neil
```

### Comparing `CalSciPy-0.2.8/README.md` & `CalSciPy-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.8/pyproject.toml` & `CalSciPy-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "CalSciPy"
-version = "0.2.8"
+version = "0.3.0"
 description = "A collection"
 readme = "README.md"
 requires-python = ">=3.7, <4"
 license = {file = "LICENSE"}
 keywords = ["CalSciPy", "Calcium Imaging"]
 authors = [
   {name = "Darik A. O'Neil"}
@@ -30,15 +30,15 @@
 dependencies = [
     "matplotlib",
     "numpy",
     "opencv-python",
     "pillow",
     "PPVD",
     "prettytable",
-    "pyside2",
+    "PyQt5",
     "seaborn",
     "scikit-learn",
     "scipy",
     "tqdm"
 ]
 
 [project.urls]
```

### Comparing `CalSciPy-0.2.8/src/CalSciPy/bruker.py` & `CalSciPy-0.3.0/src/CalSciPy/bruker.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.8/src/CalSciPy/coloring.py` & `CalSciPy-0.3.0/src/CalSciPy/coloring.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.8/src/CalSciPy/event_processing.py` & `CalSciPy-0.3.0/src/CalSciPy/event_processing.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.8/src/CalSciPy/image_processing.py` & `CalSciPy-0.3.0/src/CalSciPy/image_processing.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.8/src/CalSciPy/interactive_visuals.py` & `CalSciPy-0.3.0/src/CalSciPy/interactive_visuals.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.8/src/CalSciPy/io_tools.py` & `CalSciPy-0.3.0/src/CalSciPy/io_tools.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.8/src/CalSciPy/misc.py` & `CalSciPy-0.3.0/src/CalSciPy/misc.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.8/src/CalSciPy/reorganization.py` & `CalSciPy-0.3.0/src/CalSciPy/reorganization.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.8/src/CalSciPy/trace_processing.py` & `CalSciPy-0.3.0/src/CalSciPy/trace_processing.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.8/src/CalSciPy.egg-info/PKG-INFO` & `CalSciPy-0.3.0/src/CalSciPy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CalSciPy
-Version: 0.2.8
+Version: 0.3.0
 Summary: A collection
 Author: Darik A. O'Neil
 Maintainer: Darik A. O'Neil
 License: MIT License
         
         Copyright (c) 2023 Darik A O’Neil
```

### Comparing `CalSciPy-0.2.8/src/CalSciPy.egg-info/SOURCES.txt` & `CalSciPy-0.3.0/src/CalSciPy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.8/tests/test_a_install.py` & `CalSciPy-0.3.0/tests/test_a_install.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.8/tests/test_bruker.py` & `CalSciPy-0.3.0/tests/test_bruker.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.8/tests/test_event_processing.py` & `CalSciPy-0.3.0/tests/test_event_processing.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.8/tests/test_io_tools.py` & `CalSciPy-0.3.0/tests/test_io_tools.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.8/tests/test_misc.py` & `CalSciPy-0.3.0/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.8/tests/test_reorganization.py` & `CalSciPy-0.3.0/tests/test_reorganization.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.8/tests/test_trace_processing.py` & `CalSciPy-0.3.0/tests/test_trace_processing.py`

 * *Files identical despite different names*

