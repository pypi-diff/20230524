# Comparing `tmp/elm-messenger-0.1.8.tar.gz` & `tmp/elm-messenger-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elm-messenger-0.1.8.tar", last modified: Tue May 23 09:13:19 2023, max compression
+gzip compressed data, was "elm-messenger-0.1.9.tar", last modified: Wed May 24 04:47:35 2023, max compression
```

## Comparing `elm-messenger-0.1.8.tar` & `elm-messenger-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-23 09:13:19.499624 elm-messenger-0.1.8/
--rw-r--r--   0 linsy     (1000) linsy     (1000)       18 2023-05-04 10:50:53.000000 elm-messenger-0.1.8/MANIFEST.in
--rw-r--r--   0 linsy     (1000) linsy     (1000)      387 2023-05-23 09:13:19.499624 elm-messenger-0.1.8/PKG-INFO
--rw-r--r--   0 linsy     (1000) linsy     (1000)      122 2023-05-04 10:50:53.000000 elm-messenger-0.1.8/Readme.md
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-23 09:13:19.499624 elm-messenger-0.1.8/elm_messenger.egg-info/
--rw-r--r--   0 linsy     (1000) linsy     (1000)      387 2023-05-23 09:13:19.000000 elm-messenger-0.1.8/elm_messenger.egg-info/PKG-INFO
--rw-r--r--   0 linsy     (1000) linsy     (1000)      368 2023-05-23 09:13:19.000000 elm-messenger-0.1.8/elm_messenger.egg-info/SOURCES.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)        1 2023-05-23 09:13:19.000000 elm-messenger-0.1.8/elm_messenger.egg-info/dependency_links.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)       61 2023-05-23 09:13:19.000000 elm-messenger-0.1.8/elm_messenger.egg-info/entry_points.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)        6 2023-05-23 09:13:19.000000 elm-messenger-0.1.8/elm_messenger.egg-info/requires.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)       13 2023-05-23 09:13:19.000000 elm-messenger-0.1.8/elm_messenger.egg-info/top_level.txt
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-23 09:13:19.499624 elm-messenger-0.1.8/messengercli/
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-04 10:50:53.000000 elm-messenger-0.1.8/messengercli/__init__.py
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)      120 2023-05-04 10:50:53.000000 elm-messenger-0.1.8/messengercli/command_line.py
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)    17530 2023-05-22 06:39:53.000000 elm-messenger-0.1.8/messengercli/messenger.py
--rw-r--r--   0 linsy     (1000) linsy     (1000)     1170 2023-05-12 14:41:01.000000 elm-messenger-0.1.8/messengercli/updater.py
--rw-r--r--   0 linsy     (1000) linsy     (1000)      407 2023-05-23 09:13:19.499624 elm-messenger-0.1.8/setup.cfg
--rw-r--r--   0 linsy     (1000) linsy     (1000)      161 2023-05-04 10:50:53.000000 elm-messenger-0.1.8/setup.py
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-24 04:47:35.067003 elm-messenger-0.1.9/
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       18 2023-05-04 10:50:53.000000 elm-messenger-0.1.9/MANIFEST.in
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      387 2023-05-24 04:47:35.067003 elm-messenger-0.1.9/PKG-INFO
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      122 2023-05-04 10:50:53.000000 elm-messenger-0.1.9/Readme.md
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-24 04:47:35.067003 elm-messenger-0.1.9/elm_messenger.egg-info/
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      387 2023-05-24 04:47:35.000000 elm-messenger-0.1.9/elm_messenger.egg-info/PKG-INFO
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      368 2023-05-24 04:47:35.000000 elm-messenger-0.1.9/elm_messenger.egg-info/SOURCES.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)        1 2023-05-24 04:47:35.000000 elm-messenger-0.1.9/elm_messenger.egg-info/dependency_links.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       61 2023-05-24 04:47:35.000000 elm-messenger-0.1.9/elm_messenger.egg-info/entry_points.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)        6 2023-05-24 04:47:35.000000 elm-messenger-0.1.9/elm_messenger.egg-info/requires.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       13 2023-05-24 04:47:35.000000 elm-messenger-0.1.9/elm_messenger.egg-info/top_level.txt
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-24 04:47:35.067003 elm-messenger-0.1.9/messengercli/
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-04 10:50:53.000000 elm-messenger-0.1.9/messengercli/__init__.py
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)      120 2023-05-04 10:50:53.000000 elm-messenger-0.1.9/messengercli/command_line.py
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)    17575 2023-05-24 04:45:46.000000 elm-messenger-0.1.9/messengercli/messenger.py
+-rw-r--r--   0 linsy     (1000) linsy     (1000)     1170 2023-05-12 14:41:01.000000 elm-messenger-0.1.9/messengercli/updater.py
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      407 2023-05-24 04:47:35.067003 elm-messenger-0.1.9/setup.cfg
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      161 2023-05-04 10:50:53.000000 elm-messenger-0.1.9/setup.py
```

### Comparing `elm-messenger-0.1.8/messengercli/messenger.py` & `elm-messenger-0.1.9/messengercli/messenger.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import typer
 import os
 import shutil
 import json
 from .updater import Updater
 
 app = typer.Typer(add_completion=False, help="Messenger CLI")
-API_VERSION = "0.1.8"
+API_VERSION = "0.1.9"
 
 
 class Messenger:
     config = None
 
     def __init__(self) -> None:
         """
@@ -400,14 +400,15 @@
     os.makedirs(name, exist_ok=True)
     os.chdir(name)
     os.system(f"git clone {template_repo} .messenger --depth=1")
     shutil.copytree(".messenger/core/", "./src")
     shutil.copytree(".messenger/public/", "./public")
     shutil.copy(".messenger/.gitignore", "./.gitignore")
     shutil.copy(".messenger/Makefile", "./Makefile")
+    shutil.copy(".messenger/make", "./make")
     shutil.copy(".messenger/elm.json", "./elm.json")
 
     os.makedirs("src/Scenes", exist_ok=True)
     os.makedirs("assets", exist_ok=True)
     os.makedirs("src/Components", exist_ok=True)
     os.makedirs("src/SceneProtos", exist_ok=True)
```

### Comparing `elm-messenger-0.1.8/messengercli/updater.py` & `elm-messenger-0.1.9/messengercli/updater.py`

 * *Files identical despite different names*

