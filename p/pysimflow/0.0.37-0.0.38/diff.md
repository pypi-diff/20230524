# Comparing `tmp/pysimflow-0.0.37.tar.gz` & `tmp/pysimflow-0.0.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysimflow-0.0.37.tar", last modified: Wed May 24 06:06:55 2023, max compression
+gzip compressed data, was "pysimflow-0.0.38.tar", last modified: Wed May 24 06:08:56 2023, max compression
```

## Comparing `pysimflow-0.0.37.tar` & `pysimflow-0.0.38.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 06:06:55.855747 pysimflow-0.0.37/
--rw-r--r--   0 root         (0) root         (0)      197 2023-05-24 06:06:55.855747 pysimflow-0.0.37/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    29351 2023-05-24 04:24:44.000000 pysimflow-0.0.37/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 06:06:55.855747 pysimflow-0.0.37/digitaltwin/
--rw-r--r--   0 root         (0) root         (0)      273 2023-05-12 07:57:26.000000 pysimflow-0.0.37/digitaltwin/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2178 2023-05-24 03:33:42.000000 pysimflow-0.0.37/digitaltwin/active_obj.py
--rw-r--r--   0 root         (0) root         (0)    16452 2023-05-24 03:11:27.000000 pysimflow-0.0.37/digitaltwin/camera.py
--rw-r--r--   0 root         (0) root         (0)     4007 2023-05-19 08:07:17.000000 pysimflow-0.0.37/digitaltwin/editor.py
--rw-r--r--   0 root         (0) root         (0)     2713 2023-05-24 03:51:04.000000 pysimflow-0.0.37/digitaltwin/placer.py
--rw-r--r--   0 root         (0) root         (0)    10083 2023-03-15 13:18:59.000000 pysimflow-0.0.37/digitaltwin/printer.py
--rw-r--r--   0 root         (0) root         (0)     3554 2023-05-12 09:18:14.000000 pysimflow-0.0.37/digitaltwin/render.py
--rw-r--r--   0 root         (0) root         (0)    20135 2023-05-24 06:06:28.000000 pysimflow-0.0.37/digitaltwin/robot.py
--rw-r--r--   0 root         (0) root         (0)     6109 2023-05-24 03:57:14.000000 pysimflow-0.0.37/digitaltwin/scene.py
--rw-r--r--   0 root         (0) root         (0)     2235 2023-05-11 02:13:41.000000 pysimflow-0.0.37/digitaltwin/stacker.py
--rw-r--r--   0 root         (0) root         (0)     6296 2023-05-24 01:54:30.000000 pysimflow-0.0.37/digitaltwin/workflow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 06:06:55.855747 pysimflow-0.0.37/pysimflow.egg-info/
--rw-r--r--   0 root         (0) root         (0)      197 2023-05-24 06:06:55.000000 pysimflow-0.0.37/pysimflow.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      442 2023-05-24 06:06:55.000000 pysimflow-0.0.37/pysimflow.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 06:06:55.000000 pysimflow-0.0.37/pysimflow.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-24 06:06:55.000000 pysimflow-0.0.37/pysimflow.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-05-24 06:06:55.000000 pysimflow-0.0.37/pysimflow.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       78 2023-05-24 06:06:55.856747 pysimflow-0.0.37/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      330 2023-05-24 06:06:50.000000 pysimflow-0.0.37/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 06:08:56.928814 pysimflow-0.0.38/
+-rw-r--r--   0 root         (0) root         (0)      197 2023-05-24 06:08:56.928814 pysimflow-0.0.38/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    29351 2023-05-24 04:24:44.000000 pysimflow-0.0.38/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 06:08:56.928814 pysimflow-0.0.38/digitaltwin/
+-rw-r--r--   0 root         (0) root         (0)      361 2023-05-24 06:08:43.000000 pysimflow-0.0.38/digitaltwin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2178 2023-05-24 03:33:42.000000 pysimflow-0.0.38/digitaltwin/active_obj.py
+-rw-r--r--   0 root         (0) root         (0)    16452 2023-05-24 03:11:27.000000 pysimflow-0.0.38/digitaltwin/camera.py
+-rw-r--r--   0 root         (0) root         (0)     4007 2023-05-19 08:07:17.000000 pysimflow-0.0.38/digitaltwin/editor.py
+-rw-r--r--   0 root         (0) root         (0)     2713 2023-05-24 03:51:04.000000 pysimflow-0.0.38/digitaltwin/placer.py
+-rw-r--r--   0 root         (0) root         (0)    10083 2023-03-15 13:18:59.000000 pysimflow-0.0.38/digitaltwin/printer.py
+-rw-r--r--   0 root         (0) root         (0)     3554 2023-05-12 09:18:14.000000 pysimflow-0.0.38/digitaltwin/render.py
+-rw-r--r--   0 root         (0) root         (0)    20135 2023-05-24 06:06:28.000000 pysimflow-0.0.38/digitaltwin/robot.py
+-rw-r--r--   0 root         (0) root         (0)     6109 2023-05-24 03:57:14.000000 pysimflow-0.0.38/digitaltwin/scene.py
+-rw-r--r--   0 root         (0) root         (0)     2235 2023-05-11 02:13:41.000000 pysimflow-0.0.38/digitaltwin/stacker.py
+-rw-r--r--   0 root         (0) root         (0)     6296 2023-05-24 01:54:30.000000 pysimflow-0.0.38/digitaltwin/workflow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 06:08:56.928814 pysimflow-0.0.38/pysimflow.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      197 2023-05-24 06:08:56.000000 pysimflow-0.0.38/pysimflow.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      442 2023-05-24 06:08:56.000000 pysimflow-0.0.38/pysimflow.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 06:08:56.000000 pysimflow-0.0.38/pysimflow.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-24 06:08:56.000000 pysimflow-0.0.38/pysimflow.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-05-24 06:08:56.000000 pysimflow-0.0.38/pysimflow.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       78 2023-05-24 06:08:56.928814 pysimflow-0.0.38/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      330 2023-05-24 06:08:54.000000 pysimflow-0.0.38/setup.py
```

### Comparing `pysimflow-0.0.37/README.md` & `pysimflow-0.0.38/README.md`

 * *Files identical despite different names*

### Comparing `pysimflow-0.0.37/digitaltwin/active_obj.py` & `pysimflow-0.0.38/digitaltwin/active_obj.py`

 * *Files identical despite different names*

### Comparing `pysimflow-0.0.37/digitaltwin/camera.py` & `pysimflow-0.0.38/digitaltwin/camera.py`

 * *Files identical despite different names*

### Comparing `pysimflow-0.0.37/digitaltwin/editor.py` & `pysimflow-0.0.38/digitaltwin/editor.py`

 * *Files identical despite different names*

### Comparing `pysimflow-0.0.37/digitaltwin/placer.py` & `pysimflow-0.0.38/digitaltwin/placer.py`

 * *Files identical despite different names*

### Comparing `pysimflow-0.0.37/digitaltwin/printer.py` & `pysimflow-0.0.38/digitaltwin/printer.py`

 * *Files identical despite different names*

### Comparing `pysimflow-0.0.37/digitaltwin/render.py` & `pysimflow-0.0.38/digitaltwin/render.py`

 * *Files identical despite different names*

### Comparing `pysimflow-0.0.37/digitaltwin/robot.py` & `pysimflow-0.0.38/digitaltwin/robot.py`

 * *Files identical despite different names*

### Comparing `pysimflow-0.0.37/digitaltwin/scene.py` & `pysimflow-0.0.38/digitaltwin/scene.py`

 * *Files identical despite different names*

### Comparing `pysimflow-0.0.37/digitaltwin/stacker.py` & `pysimflow-0.0.38/digitaltwin/stacker.py`

 * *Files identical despite different names*

### Comparing `pysimflow-0.0.37/digitaltwin/workflow.py` & `pysimflow-0.0.38/digitaltwin/workflow.py`

 * *Files identical despite different names*

