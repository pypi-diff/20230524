# Comparing `tmp/autoAmbient-0.3.1.tar.gz` & `tmp/autoAmbient-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoAmbient-0.3.1.tar", last modified: Sun May  7 20:21:10 2023, max compression
+gzip compressed data, was "autoAmbient-0.3.3.tar", last modified: Wed May 24 00:53:43 2023, max compression
```

## Comparing `autoAmbient-0.3.1.tar` & `autoAmbient-0.3.3.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2023-05-07 20:21:10.678269 autoAmbient-0.3.1/
--rw-rw-r--   0 luis      (1000) luis      (1000)      185 2023-05-07 20:21:10.678269 autoAmbient-0.3.1/PKG-INFO
-drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2023-05-07 20:21:10.674269 autoAmbient-0.3.1/ambient/
--rw-rw-r--   0 luis      (1000) luis      (1000)       73 2023-04-17 21:37:09.000000 autoAmbient-0.3.1/ambient/__init__.py
--rw-rw-r--   0 luis      (1000) luis      (1000)      897 2023-04-25 14:38:15.000000 autoAmbient-0.3.1/ambient/createAutoAmbient.py
--rw-rw-r--   0 luis      (1000) luis      (1000)      785 2023-04-25 15:08:35.000000 autoAmbient-0.3.1/ambient/createTagsFile.py
--rw-rw-r--   0 luis      (1000) luis      (1000)      721 2023-04-11 15:44:13.000000 autoAmbient-0.3.1/ambient/getFile.py
-drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2023-05-07 20:21:10.674269 autoAmbient-0.3.1/ambient/models/
--rw-rw-r--   0 luis      (1000) luis      (1000)      165 2023-04-25 14:32:48.000000 autoAmbient-0.3.1/ambient/models/blocksModel.py
--rw-rw-r--   0 luis      (1000) luis      (1000)       47 2023-04-17 21:10:55.000000 autoAmbient-0.3.1/ambient/models/mainModel.py
--rw-rw-r--   0 luis      (1000) luis      (1000)      476 2023-04-25 14:56:13.000000 autoAmbient-0.3.1/ambient/models/runModel.py
-drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2023-05-07 20:21:10.674269 autoAmbient-0.3.1/ambient/tolls/
--rw-rw-r--   0 luis      (1000) luis      (1000)     1916 2023-04-25 14:46:31.000000 autoAmbient-0.3.1/ambient/tolls/clicks.py
--rw-rw-r--   0 luis      (1000) luis      (1000)     4826 2023-04-17 22:02:18.000000 autoAmbient-0.3.1/ambient/tolls/gui.py
--rw-rw-r--   0 luis      (1000) luis      (1000)      834 2023-04-25 14:59:25.000000 autoAmbient-0.3.1/ambient/tolls/utils.py
-drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2023-05-07 20:21:10.678269 autoAmbient-0.3.1/autoAmbient.egg-info/
--rw-rw-r--   0 luis      (1000) luis      (1000)      185 2023-05-07 20:21:10.000000 autoAmbient-0.3.1/autoAmbient.egg-info/PKG-INFO
--rw-rw-r--   0 luis      (1000) luis      (1000)      458 2023-05-07 20:21:10.000000 autoAmbient-0.3.1/autoAmbient.egg-info/SOURCES.txt
--rw-rw-r--   0 luis      (1000) luis      (1000)        1 2023-05-07 20:21:10.000000 autoAmbient-0.3.1/autoAmbient.egg-info/dependency_links.txt
--rw-rw-r--   0 luis      (1000) luis      (1000)      142 2023-05-07 20:21:10.000000 autoAmbient-0.3.1/autoAmbient.egg-info/entry_points.txt
--rw-rw-r--   0 luis      (1000) luis      (1000)        8 2023-05-07 20:21:10.000000 autoAmbient-0.3.1/autoAmbient.egg-info/top_level.txt
--rw-rw-r--   0 luis      (1000) luis      (1000)        0 2023-04-11 14:47:07.000000 autoAmbient-0.3.1/pyproject.toml
--rw-rw-r--   0 luis      (1000) luis      (1000)      149 2023-05-07 20:21:10.678269 autoAmbient-0.3.1/setup.cfg
--rw-rw-r--   0 luis      (1000) luis      (1000)      373 2023-05-07 20:15:04.000000 autoAmbient-0.3.1/setup.py
+drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2023-05-24 00:53:43.865197 autoAmbient-0.3.3/
+-rw-rw-r--   0 luis      (1000) luis      (1000)      348 2023-05-24 00:53:43.865197 autoAmbient-0.3.3/PKG-INFO
+-rw-rw-r--   0 luis      (1000) luis      (1000)        0 2023-05-24 00:51:08.000000 autoAmbient-0.3.3/README.md
+drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2023-05-24 00:53:43.865197 autoAmbient-0.3.3/ambient/
+-rw-rw-r--   0 luis      (1000) luis      (1000)       73 2023-04-17 21:37:09.000000 autoAmbient-0.3.3/ambient/__init__.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)      897 2023-04-25 14:38:15.000000 autoAmbient-0.3.3/ambient/createAutoAmbient.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)      785 2023-04-25 15:08:35.000000 autoAmbient-0.3.3/ambient/createTagsFile.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)      721 2023-04-11 15:44:13.000000 autoAmbient-0.3.3/ambient/getFile.py
+drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2023-05-24 00:53:43.865197 autoAmbient-0.3.3/ambient/models/
+-rw-rw-r--   0 luis      (1000) luis      (1000)      165 2023-04-25 14:32:48.000000 autoAmbient-0.3.3/ambient/models/blocksModel.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)       47 2023-04-17 21:10:55.000000 autoAmbient-0.3.3/ambient/models/mainModel.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)      476 2023-04-25 14:56:13.000000 autoAmbient-0.3.3/ambient/models/runModel.py
+drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2023-05-24 00:53:43.865197 autoAmbient-0.3.3/ambient/tolls/
+-rw-rw-r--   0 luis      (1000) luis      (1000)     1892 2023-05-07 20:31:23.000000 autoAmbient-0.3.3/ambient/tolls/clicks.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)     4826 2023-04-17 22:02:18.000000 autoAmbient-0.3.3/ambient/tolls/gui.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)      822 2023-05-07 20:31:23.000000 autoAmbient-0.3.3/ambient/tolls/utils.py
+drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2023-05-24 00:53:43.865197 autoAmbient-0.3.3/autoAmbient.egg-info/
+-rw-rw-r--   0 luis      (1000) luis      (1000)      348 2023-05-24 00:53:43.000000 autoAmbient-0.3.3/autoAmbient.egg-info/PKG-INFO
+-rw-rw-r--   0 luis      (1000) luis      (1000)      502 2023-05-24 00:53:43.000000 autoAmbient-0.3.3/autoAmbient.egg-info/SOURCES.txt
+-rw-rw-r--   0 luis      (1000) luis      (1000)        1 2023-05-24 00:53:43.000000 autoAmbient-0.3.3/autoAmbient.egg-info/dependency_links.txt
+-rw-rw-r--   0 luis      (1000) luis      (1000)      142 2023-05-24 00:53:43.000000 autoAmbient-0.3.3/autoAmbient.egg-info/entry_points.txt
+-rw-rw-r--   0 luis      (1000) luis      (1000)       52 2023-05-24 00:53:43.000000 autoAmbient-0.3.3/autoAmbient.egg-info/requires.txt
+-rw-rw-r--   0 luis      (1000) luis      (1000)        8 2023-05-24 00:53:43.000000 autoAmbient-0.3.3/autoAmbient.egg-info/top_level.txt
+-rw-rw-r--   0 luis      (1000) luis      (1000)        0 2023-04-11 14:47:07.000000 autoAmbient-0.3.3/pyproject.toml
+-rw-rw-r--   0 luis      (1000) luis      (1000)      149 2023-05-24 00:53:43.869197 autoAmbient-0.3.3/setup.cfg
+-rw-rw-r--   0 luis      (1000) luis      (1000)      868 2023-05-24 00:52:24.000000 autoAmbient-0.3.3/setup.py
```

### Comparing `autoAmbient-0.3.1/ambient/createAutoAmbient.py` & `autoAmbient-0.3.3/ambient/createAutoAmbient.py`

 * *Files identical despite different names*

### Comparing `autoAmbient-0.3.1/ambient/createTagsFile.py` & `autoAmbient-0.3.3/ambient/createTagsFile.py`

 * *Files identical despite different names*

### Comparing `autoAmbient-0.3.1/ambient/getFile.py` & `autoAmbient-0.3.3/ambient/getFile.py`

 * *Files identical despite different names*

### Comparing `autoAmbient-0.3.1/ambient/tolls/clicks.py` & `autoAmbient-0.3.3/ambient/tolls/clicks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from . import gui
 import pyautogui
-from typing import Callable, Self
+from typing import Callable
 
 gui = gui.gui
 
 
 def alertImageNotFound(imgName):
     raise Exception(f"{imgName} não foi encontrado")
 
 
 def doNothing(x=1, y=2):
     pass
 
 
 def find(
-    self: Self,
+    self,
     imgName: str,
     waiting_time: int = 500,
     afterAction: Callable = lambda: pyautogui.press("enter"),
     notFoundAction: alertImageNotFound = alertImageNotFound,
 ):
     try:
         if not self.find(imgName, matching=0.93, waiting_time=waiting_time):
@@ -33,26 +33,26 @@
                 imgName,
                 waiting_time=waiting_time,
                 afterAction=afterAction,
                 notFoundAction=notFoundAction,
             )
 
 
-def tryToClick(self: Self, btnName: str, waiting_time: int = 2000):
+def tryToClick(self, btnName: str, waiting_time: int = 2000):
     if not self.find(btnName, matching=0.93, waiting_time=waiting_time):
         try:
             self.find(f"{btnName}_r", matching=0.93, waiting_time=waiting_time)
             self.click()
         except Exception:
             raise Exception(f'o botão "{btnName}" não foi encontrado')
     else:
         self.click()
 
 
-def click(self: Self, btnName: str, waiting_time: int = 2000, error=False):
+def click(self, btnName: str, waiting_time: int = 2000, error=False):
     if error:
         self.tab()
     btn = btnName
     try:
         tryToClick(self, btn, waiting_time=waiting_time)
     except Exception as e:
         if gui.wrong(text=f"({btn})[{e}]")["tryAgain"]:
```

### Comparing `autoAmbient-0.3.1/ambient/tolls/gui.py` & `autoAmbient-0.3.3/ambient/tolls/gui.py`

 * *Files identical despite different names*

### Comparing `autoAmbient-0.3.1/ambient/tolls/utils.py` & `autoAmbient-0.3.3/ambient/tolls/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 from . import clicks as cl
-from typing import Self, TypeVar
+from typing import TypeVar
 
 
 def notify(text):
 
     logging.basicConfig(
         handlers=[
             logging.FileHandler(
@@ -19,15 +19,15 @@
     logging.info(text)
 
 
 C = TypeVar("C")
 
 
 def remove_self_necessity(
-    self: Self,
+    self,
     func: C,
 ) -> C:
     def wrapper(*args, **kwargs):
         return func(self, *args, **kwargs)
 
     return wrapper
```

