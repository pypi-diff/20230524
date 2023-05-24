# Comparing `tmp/graiax-shortcut-0.2.0.tar.gz` & `tmp/graiax-shortcut-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graiax-shortcut-0.2.0.tar", last modified: Mon Nov 14 13:00:22 2022, max compression
+gzip compressed data, was "graiax-shortcut-0.2.1.tar", last modified: Mon Dec 12 15:00:38 2022, max compression
```

## Comparing `graiax-shortcut-0.2.0.tar` & `graiax-shortcut-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 13:00:22.113777 graiax-shortcut-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1063 2022-11-14 12:59:59.000000 graiax-shortcut-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1174 2022-11-14 13:00:22.113777 graiax-shortcut-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      794 2022-11-14 12:59:59.000000 graiax-shortcut-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1253 2022-11-14 12:59:59.000000 graiax-shortcut-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-14 13:00:22.113777 graiax-shortcut-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 13:00:22.113777 graiax-shortcut-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 13:00:22.113777 graiax-shortcut-0.2.0/src/graiax/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 13:00:22.113777 graiax-shortcut-0.2.0/src/graiax/shortcut/
--rw-r--r--   0 runner    (1001) docker     (121)      480 2022-11-14 12:59:59.000000 graiax-shortcut-0.2.0/src/graiax/shortcut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      330 2022-11-14 12:59:59.000000 graiax-shortcut-0.2.0/src/graiax/shortcut/_util.py
--rw-r--r--   0 runner    (1001) docker     (121)     4225 2022-11-14 12:59:59.000000 graiax-shortcut-0.2.0/src/graiax/shortcut/formatter.py
--rw-r--r--   0 runner    (1001) docker     (121)     6712 2022-11-14 12:59:59.000000 graiax-shortcut-0.2.0/src/graiax/shortcut/interrupt.py
--rw-r--r--   0 runner    (1001) docker     (121)     7110 2022-11-14 12:59:59.000000 graiax-shortcut-0.2.0/src/graiax/shortcut/saya.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 13:00:22.113777 graiax-shortcut-0.2.0/src/graiax_shortcut.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1174 2022-11-14 13:00:22.000000 graiax-shortcut-0.2.0/src/graiax_shortcut.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      401 2022-11-14 13:00:22.000000 graiax-shortcut-0.2.0/src/graiax_shortcut.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-14 13:00:22.000000 graiax-shortcut-0.2.0/src/graiax_shortcut.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-11-14 13:00:22.000000 graiax-shortcut-0.2.0/src/graiax_shortcut.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-11-14 13:00:22.000000 graiax-shortcut-0.2.0/src/graiax_shortcut.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 15:00:38.993995 graiax-shortcut-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2022-12-12 15:00:13.000000 graiax-shortcut-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2022-12-12 15:00:38.993995 graiax-shortcut-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2022-12-12 15:00:13.000000 graiax-shortcut-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2022-12-12 15:00:13.000000 graiax-shortcut-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-12 15:00:38.993995 graiax-shortcut-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 15:00:38.993995 graiax-shortcut-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 15:00:38.993995 graiax-shortcut-0.2.1/src/graiax/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 15:00:38.993995 graiax-shortcut-0.2.1/src/graiax/shortcut/
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2022-12-12 15:00:13.000000 graiax-shortcut-0.2.1/src/graiax/shortcut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2022-12-12 15:00:13.000000 graiax-shortcut-0.2.1/src/graiax/shortcut/_typing_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2022-12-12 15:00:13.000000 graiax-shortcut-0.2.1/src/graiax/shortcut/_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2022-12-12 15:00:13.000000 graiax-shortcut-0.2.1/src/graiax/shortcut/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6712 2022-12-12 15:00:13.000000 graiax-shortcut-0.2.1/src/graiax/shortcut/interrupt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7110 2022-12-12 15:00:13.000000 graiax-shortcut-0.2.1/src/graiax/shortcut/saya.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12213 2022-12-12 15:00:13.000000 graiax-shortcut-0.2.1/src/graiax/shortcut/text_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 15:00:38.993995 graiax-shortcut-0.2.1/src/graiax_shortcut.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2022-12-12 15:00:38.000000 graiax-shortcut-0.2.1/src/graiax_shortcut.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2022-12-12 15:00:38.000000 graiax-shortcut-0.2.1/src/graiax_shortcut.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-12 15:00:38.000000 graiax-shortcut-0.2.1/src/graiax_shortcut.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2022-12-12 15:00:38.000000 graiax-shortcut-0.2.1/src/graiax_shortcut.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2022-12-12 15:00:38.000000 graiax-shortcut-0.2.1/src/graiax_shortcut.egg-info/top_level.txt
```

### Comparing `graiax-shortcut-0.2.0/LICENSE` & `graiax-shortcut-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `graiax-shortcut-0.2.0/PKG-INFO` & `graiax-shortcut-0.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: graiax-shortcut
-Version: 0.2.0
+Version: 0.2.1
 Summary: Utilities for Graia Framework Community.
 Author-email: BlueGlassBlock <blueglassblock@outlook.com>, RF-Tar-Railt <rf_tar_railt@qq.com>
 License: MIT
-Project-URL: Repository, https://github.com/GraiaProject/graiax-shortcut
+Project-URL: Repository, https://github.com/GraiaCommunity/Shortcut
 Requires-Python: <4.0,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
 
 # GraiaX Shortcut
```

### Comparing `graiax-shortcut-0.2.0/README.md` & `graiax-shortcut-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `graiax-shortcut-0.2.0/pyproject.toml` & `graiax-shortcut-0.2.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -7,22 +7,23 @@
 ]
 license = {text = "MIT"}
 readme = "README.md"
 requires-python = ">=3.8,<4.0"
 dependencies = [
     "graia-broadcast<1.0.0,>=0.18",
     "creart~=0.2",
-    "graia-amnesia<0.7.0,>=0.6.0",
+    "graia-amnesia~=0.7.0",
     "graia-scheduler>=0.0.8",
     "graia-saya<0.1.0,>=0.0.17",
+    "typing-extensions>=4.4.0",
 ]
-version = "0.2.0"
+version = "0.2.1"
 
 [project.urls]
-Repository = "https://github.com/GraiaProject/graiax-shortcut"
+Repository = "https://github.com/GraiaCommunity/Shortcut"
 
 [project.optional-dependencies]
 [tool.pdm.build]
 package-dir = "src"
 
 [tool.pdm.dev-dependencies]
 dev = [
```

### Comparing `graiax-shortcut-0.2.0/src/graiax/shortcut/formatter.py` & `graiax-shortcut-0.2.1/src/graiax/shortcut/formatter.py`

 * *Files identical despite different names*

### Comparing `graiax-shortcut-0.2.0/src/graiax/shortcut/interrupt.py` & `graiax-shortcut-0.2.1/src/graiax/shortcut/interrupt.py`

 * *Files identical despite different names*

### Comparing `graiax-shortcut-0.2.0/src/graiax/shortcut/saya.py` & `graiax-shortcut-0.2.1/src/graiax/shortcut/saya.py`

 * *Files identical despite different names*

### Comparing `graiax-shortcut-0.2.0/src/graiax_shortcut.egg-info/PKG-INFO` & `graiax-shortcut-0.2.1/src/graiax_shortcut.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: graiax-shortcut
-Version: 0.2.0
+Version: 0.2.1
 Summary: Utilities for Graia Framework Community.
 Author-email: BlueGlassBlock <blueglassblock@outlook.com>, RF-Tar-Railt <rf_tar_railt@qq.com>
 License: MIT
-Project-URL: Repository, https://github.com/GraiaProject/graiax-shortcut
+Project-URL: Repository, https://github.com/GraiaCommunity/Shortcut
 Requires-Python: <4.0,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
 
 # GraiaX Shortcut
```

