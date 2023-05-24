# Comparing `tmp/grrif_tools-0.6.1.tar.gz` & `tmp/grrif_tools-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grrif_tools-0.6.1.tar", last modified: Sun May  7 21:12:53 2023, max compression
+gzip compressed data, was "grrif_tools-0.6.2.tar", last modified: Wed May 24 20:45:41 2023, max compression
```

## Comparing `grrif_tools-0.6.1.tar` & `grrif_tools-0.6.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:12:53.754684 grrif_tools-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-07 21:12:48.000000 grrif_tools-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-07 21:12:48.000000 grrif_tools-0.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-05-07 21:12:53.754684 grrif_tools-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-07 21:12:48.000000 grrif_tools-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:12:53.754684 grrif_tools-0.6.1/grrif_tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 21:12:48.000000 grrif_tools-0.6.1/grrif_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-05-07 21:12:48.000000 grrif_tools-0.6.1/grrif_tools/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-05-07 21:12:48.000000 grrif_tools-0.6.1/grrif_tools/grrif_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-07 21:12:48.000000 grrif_tools-0.6.1/grrif_tools/grrif_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:12:53.754684 grrif_tools-0.6.1/grrif_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-05-07 21:12:53.000000 grrif_tools-0.6.1/grrif_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-07 21:12:53.000000 grrif_tools-0.6.1/grrif_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 21:12:53.000000 grrif_tools-0.6.1/grrif_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-07 21:12:53.000000 grrif_tools-0.6.1/grrif_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-07 21:12:53.000000 grrif_tools-0.6.1/grrif_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-07 21:12:53.000000 grrif_tools-0.6.1/grrif_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-07 21:12:48.000000 grrif_tools-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 21:12:53.754684 grrif_tools-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-07 21:12:48.000000 grrif_tools-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:45:41.974254 grrif_tools-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-24 20:45:36.000000 grrif_tools-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-24 20:45:36.000000 grrif_tools-0.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-05-24 20:45:41.974254 grrif_tools-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-24 20:45:36.000000 grrif_tools-0.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:45:41.974254 grrif_tools-0.6.2/grrif_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:45:36.000000 grrif_tools-0.6.2/grrif_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-05-24 20:45:36.000000 grrif_tools-0.6.2/grrif_tools/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-05-24 20:45:36.000000 grrif_tools-0.6.2/grrif_tools/grrif_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-24 20:45:36.000000 grrif_tools-0.6.2/grrif_tools/grrif_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:45:41.974254 grrif_tools-0.6.2/grrif_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-05-24 20:45:41.000000 grrif_tools-0.6.2/grrif_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-24 20:45:41.000000 grrif_tools-0.6.2/grrif_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 20:45:41.000000 grrif_tools-0.6.2/grrif_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-24 20:45:41.000000 grrif_tools-0.6.2/grrif_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-24 20:45:41.000000 grrif_tools-0.6.2/grrif_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-24 20:45:41.000000 grrif_tools-0.6.2/grrif_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-24 20:45:36.000000 grrif_tools-0.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 20:45:41.974254 grrif_tools-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-24 20:45:36.000000 grrif_tools-0.6.2/setup.py
```

### Comparing `grrif_tools-0.6.1/LICENSE` & `grrif_tools-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `grrif_tools-0.6.1/PKG-INFO` & `grrif_tools-0.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: grrif_tools
-Version: 0.6.1
+Version: 0.6.2
 Summary: An unofficial set of tools for Cool Cats™.
-Home-page: https://github.com/fetzu/grrif_tools
-Download-URL: https://github.com/fetzu/grrif_tools/releases/latest
+Home-page: https://github.com/fetzu/grrif-tools
+Download-URL: https://github.com/fetzu/grrif-tools/releases/latest
 Author: Julien 'fetzu' Bono
 License: MIT License
         
         Copyright (c) 2023 Julien 'fetzu' Bono
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -23,16 +23,16 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: Homepage, https://github.com/fetzu/grrif_tools
-Project-URL: Bug Tracker, https://github.com/fetzu/grrif_tools/issues
+Project-URL: Homepage, https://github.com/fetzu/grrif-tools
+Project-URL: Bug Tracker, https://github.com/fetzu/grrif-tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `grrif_tools-0.6.1/README.md` & `grrif_tools-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `grrif_tools-0.6.1/grrif_tools/cli.py` & `grrif_tools-0.6.2/grrif_tools/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ### [ GRRIF Tools by Julien 'fetzu' Bono ]
 ## [ IMPORTS ]
 import sys
 import argparse
 from datetime import date, datetime
 
 ## [ CONFIGURATION ]
-__version__ = "0.6.1"
+__version__ = "0.6.2"
 
 ## [ Is CLI even cooler with argparse? ]
 parser = argparse.ArgumentParser(
     description="A set of tools for Cool Cats™. Allows you to archive GRRIF's play history and scrobble it to last.fm (upcoming)."
 )
 
 subparsers = parser.add_subparsers(dest="command")
```

### Comparing `grrif_tools-0.6.1/grrif_tools/grrif_archiver.py` & `grrif_tools-0.6.2/grrif_tools/grrif_archiver.py`

 * *Files identical despite different names*

### Comparing `grrif_tools-0.6.1/grrif_tools/grrif_stats.py` & `grrif_tools-0.6.2/grrif_tools/grrif_stats.py`

 * *Files identical despite different names*

### Comparing `grrif_tools-0.6.1/grrif_tools.egg-info/PKG-INFO` & `grrif_tools-0.6.2/grrif_tools.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: grrif-tools
-Version: 0.6.1
+Version: 0.6.2
 Summary: An unofficial set of tools for Cool Cats™.
-Home-page: https://github.com/fetzu/grrif_tools
-Download-URL: https://github.com/fetzu/grrif_tools/releases/latest
+Home-page: https://github.com/fetzu/grrif-tools
+Download-URL: https://github.com/fetzu/grrif-tools/releases/latest
 Author: Julien 'fetzu' Bono
 License: MIT License
         
         Copyright (c) 2023 Julien 'fetzu' Bono
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -23,16 +23,16 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: Homepage, https://github.com/fetzu/grrif_tools
-Project-URL: Bug Tracker, https://github.com/fetzu/grrif_tools/issues
+Project-URL: Homepage, https://github.com/fetzu/grrif-tools
+Project-URL: Bug Tracker, https://github.com/fetzu/grrif-tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `grrif_tools-0.6.1/pyproject.toml` & `grrif_tools-0.6.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "grrif_tools"
-version = "0.6.1"
+version = "0.6.2"
 authors = [
   { name="Julien 'fetzu' Bono" },
 ]
 description = "An unofficial set of tools for Cool Cats™."
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.9"
@@ -19,9 +19,9 @@
     "titlecase==2.4",
 ]
 
 [project.entry-points.'console_scripts']
 grrif_tools = "grrif_tools.cli:main"
 
 [project.urls]
-"Homepage" = "https://github.com/fetzu/grrif_tools"
-"Bug Tracker" = "https://github.com/fetzu/grrif_tools/issues"
+"Homepage" = "https://github.com/fetzu/grrif-tools"
+"Bug Tracker" = "https://github.com/fetzu/grrif-tools/issues"
```

