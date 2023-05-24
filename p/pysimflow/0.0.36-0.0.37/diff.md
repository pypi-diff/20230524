# Comparing `tmp/pysimflow-0.0.36.tar.gz` & `tmp/pysimflow-0.0.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysimflow-0.0.36.tar", last modified: Wed May 24 04:06:04 2023, max compression
+gzip compressed data, was "pysimflow-0.0.37.tar", last modified: Wed May 24 06:06:55 2023, max compression
```

## Comparing `pysimflow-0.0.36.tar` & `pysimflow-0.0.37.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 04:06:04.094897 pysimflow-0.0.36/
--rw-r--r--   0 root         (0) root         (0)      197 2023-05-24 04:06:04.095897 pysimflow-0.0.36/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    29434 2023-04-21 09:19:09.000000 pysimflow-0.0.36/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 04:06:04.094897 pysimflow-0.0.36/digitaltwin/
--rw-r--r--   0 root         (0) root         (0)      273 2023-05-12 07:57:26.000000 pysimflow-0.0.36/digitaltwin/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2178 2023-05-24 03:33:42.000000 pysimflow-0.0.36/digitaltwin/active_obj.py
--rw-r--r--   0 root         (0) root         (0)    16452 2023-05-24 03:11:27.000000 pysimflow-0.0.36/digitaltwin/camera.py
--rw-r--r--   0 root         (0) root         (0)     4007 2023-05-19 08:07:17.000000 pysimflow-0.0.36/digitaltwin/editor.py
--rw-r--r--   0 root         (0) root         (0)     2713 2023-05-24 03:51:04.000000 pysimflow-0.0.36/digitaltwin/placer.py
--rw-r--r--   0 root         (0) root         (0)    10083 2023-03-15 13:18:59.000000 pysimflow-0.0.36/digitaltwin/printer.py
--rw-r--r--   0 root         (0) root         (0)     3554 2023-05-12 09:18:14.000000 pysimflow-0.0.36/digitaltwin/render.py
--rw-r--r--   0 root         (0) root         (0)    20113 2023-05-24 02:57:29.000000 pysimflow-0.0.36/digitaltwin/robot.py
--rw-r--r--   0 root         (0) root         (0)     6109 2023-05-24 03:57:14.000000 pysimflow-0.0.36/digitaltwin/scene.py
--rw-r--r--   0 root         (0) root         (0)     2235 2023-05-11 02:13:41.000000 pysimflow-0.0.36/digitaltwin/stacker.py
--rw-r--r--   0 root         (0) root         (0)     6296 2023-05-24 01:54:30.000000 pysimflow-0.0.36/digitaltwin/workflow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 04:06:04.094897 pysimflow-0.0.36/pysimflow.egg-info/
--rw-r--r--   0 root         (0) root         (0)      197 2023-05-24 04:06:04.000000 pysimflow-0.0.36/pysimflow.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      442 2023-05-24 04:06:04.000000 pysimflow-0.0.36/pysimflow.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 04:06:04.000000 pysimflow-0.0.36/pysimflow.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-24 04:06:04.000000 pysimflow-0.0.36/pysimflow.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-05-24 04:06:04.000000 pysimflow-0.0.36/pysimflow.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       78 2023-05-24 04:06:04.095897 pysimflow-0.0.36/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      399 2023-05-24 04:05:38.000000 pysimflow-0.0.36/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 06:06:55.855747 pysimflow-0.0.37/
+-rw-r--r--   0 root         (0) root         (0)      197 2023-05-24 06:06:55.855747 pysimflow-0.0.37/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    29351 2023-05-24 04:24:44.000000 pysimflow-0.0.37/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 06:06:55.855747 pysimflow-0.0.37/digitaltwin/
+-rw-r--r--   0 root         (0) root         (0)      273 2023-05-12 07:57:26.000000 pysimflow-0.0.37/digitaltwin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2178 2023-05-24 03:33:42.000000 pysimflow-0.0.37/digitaltwin/active_obj.py
+-rw-r--r--   0 root         (0) root         (0)    16452 2023-05-24 03:11:27.000000 pysimflow-0.0.37/digitaltwin/camera.py
+-rw-r--r--   0 root         (0) root         (0)     4007 2023-05-19 08:07:17.000000 pysimflow-0.0.37/digitaltwin/editor.py
+-rw-r--r--   0 root         (0) root         (0)     2713 2023-05-24 03:51:04.000000 pysimflow-0.0.37/digitaltwin/placer.py
+-rw-r--r--   0 root         (0) root         (0)    10083 2023-03-15 13:18:59.000000 pysimflow-0.0.37/digitaltwin/printer.py
+-rw-r--r--   0 root         (0) root         (0)     3554 2023-05-12 09:18:14.000000 pysimflow-0.0.37/digitaltwin/render.py
+-rw-r--r--   0 root         (0) root         (0)    20135 2023-05-24 06:06:28.000000 pysimflow-0.0.37/digitaltwin/robot.py
+-rw-r--r--   0 root         (0) root         (0)     6109 2023-05-24 03:57:14.000000 pysimflow-0.0.37/digitaltwin/scene.py
+-rw-r--r--   0 root         (0) root         (0)     2235 2023-05-11 02:13:41.000000 pysimflow-0.0.37/digitaltwin/stacker.py
+-rw-r--r--   0 root         (0) root         (0)     6296 2023-05-24 01:54:30.000000 pysimflow-0.0.37/digitaltwin/workflow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 06:06:55.855747 pysimflow-0.0.37/pysimflow.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      197 2023-05-24 06:06:55.000000 pysimflow-0.0.37/pysimflow.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      442 2023-05-24 06:06:55.000000 pysimflow-0.0.37/pysimflow.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 06:06:55.000000 pysimflow-0.0.37/pysimflow.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-24 06:06:55.000000 pysimflow-0.0.37/pysimflow.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-05-24 06:06:55.000000 pysimflow-0.0.37/pysimflow.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       78 2023-05-24 06:06:55.856747 pysimflow-0.0.37/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      330 2023-05-24 06:06:50.000000 pysimflow-0.0.37/setup.py
```

### Comparing `pysimflow-0.0.36/README.md` & `pysimflow-0.0.37/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-<h1 align="center">Digital-Twin</h1>
+<h1 align="center">Simflow</h1>
 
 [TOC]
 
 <div style="page-break-after: always;" ></div>
 
 # 1 概述
 
         本文的目标在于梳理并定义前端业务接口规范，用于避免SDK开发者在不完全了解前端业务的情况下开发出不兼容的接口。 
 
 ## 1.1 安装
 
-下载源代码：`git clone http://120.24.55.96:3000/MixedAI/GraspSim`
-
-安装依赖：`pip3 install -r requirements.txt`
+下载源代码：`pip3 install pysimflow`
 
 ## 1.2 快速开始
 
+
+
 获取一堆工件的深度图：`python3 test.py`
 
 获取一堆工件的姿态数据：`python3 test0.py`
 
 混合拆垛演示：`python3 test1.py`
 
 无序抓取演示：`python3 test2.py`
```

### Comparing `pysimflow-0.0.36/digitaltwin/active_obj.py` & `pysimflow-0.0.37/digitaltwin/active_obj.py`

 * *Files identical despite different names*

### Comparing `pysimflow-0.0.36/digitaltwin/camera.py` & `pysimflow-0.0.37/digitaltwin/camera.py`

 * *Files identical despite different names*

### Comparing `pysimflow-0.0.36/digitaltwin/editor.py` & `pysimflow-0.0.37/digitaltwin/editor.py`

 * *Files identical despite different names*

### Comparing `pysimflow-0.0.36/digitaltwin/placer.py` & `pysimflow-0.0.37/digitaltwin/placer.py`

 * *Files identical despite different names*

### Comparing `pysimflow-0.0.36/digitaltwin/printer.py` & `pysimflow-0.0.37/digitaltwin/printer.py`

 * *Files identical despite different names*

### Comparing `pysimflow-0.0.36/digitaltwin/render.py` & `pysimflow-0.0.37/digitaltwin/render.py`

 * *Files identical despite different names*

### Comparing `pysimflow-0.0.36/digitaltwin/robot.py` & `pysimflow-0.0.37/digitaltwin/robot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pybullet as p
 import numpy as np
 from scipy.spatial.transform import Rotation
 import xml.dom.minidom as xml
 import os 
 
-from .active_obj import ActiveObject
-from .end_effector import Gripper,Suction
+from digitaltwin.active_obj import ActiveObject
+from digitaltwin.end_effector import Gripper,Suction
 
 class Robot(ActiveObject):
     def __init__(self,scene,**kwargs):
         if 'reset_joint_poses' not in kwargs: kwargs['reset_joint_poses'] = []
         if 'joint_damping' not in kwargs: kwargs['joint_damping'] = []
         if 'end_effector' not in kwargs: kwargs['end_effector'] = ''
         if 'speed' not in kwargs:  kwargs['speed'] = 1.0
```

### Comparing `pysimflow-0.0.36/digitaltwin/scene.py` & `pysimflow-0.0.37/digitaltwin/scene.py`

 * *Files identical despite different names*

### Comparing `pysimflow-0.0.36/digitaltwin/stacker.py` & `pysimflow-0.0.37/digitaltwin/stacker.py`

 * *Files identical despite different names*

### Comparing `pysimflow-0.0.36/digitaltwin/workflow.py` & `pysimflow-0.0.37/digitaltwin/workflow.py`

 * *Files identical despite different names*

