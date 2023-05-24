# Comparing `tmp/birdhouse-birdy-0.8.3.tar.gz` & `tmp/birdhouse-birdy-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "birdhouse-birdy-0.8.3.tar", last modified: Fri May  5 15:06:37 2023, max compression
+gzip compressed data, was "birdhouse-birdy-0.8.4.tar", last modified: Wed May 24 15:23:08 2023, max compression
```

## Comparing `birdhouse-birdy-0.8.3.tar` & `birdhouse-birdy-0.8.4.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:06:37.506090 birdhouse-birdy-0.8.3/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6600 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9959 2023-05-05 15:06:37.506090 birdhouse-birdy-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:06:37.502090 birdhouse-birdy-0.8.3/birdhouse_birdy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9959 2023-05-05 15:06:37.000000 birdhouse-birdy-0.8.3/birdhouse_birdy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-05 15:06:37.000000 birdhouse-birdy-0.8.3/birdhouse_birdy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 15:06:37.000000 birdhouse-birdy-0.8.3/birdhouse_birdy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-05 15:06:37.000000 birdhouse-birdy-0.8.3/birdhouse_birdy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-05 15:06:37.000000 birdhouse-birdy-0.8.3/birdhouse_birdy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 15:06:37.000000 birdhouse-birdy-0.8.3/birdhouse_birdy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:06:37.502090 birdhouse-birdy-0.8.3/birdy/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/birdy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:06:37.502090 birdhouse-birdy-0.8.3/birdy/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/birdy/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/birdy/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/birdy/cli/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/birdy/cli/run.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/birdy/cli/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:06:37.502090 birdhouse-birdy-0.8.3/birdy/client/
--rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/birdy/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15876 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/birdy/client/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10685 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/birdy/client/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/birdy/client/notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/birdy/client/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/birdy/client/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/birdy/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/birdy/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:06:37.502090 birdhouse-birdy-0.8.3/birdy/ipyleafletwfs/
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/birdy/ipyleafletwfs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/birdy/ipyleafletwfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15076 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/birdy/ipyleafletwfs/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:06:37.502090 birdhouse-birdy-0.8.3/birdy/ipyleafletwfs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/birdy/ipyleafletwfs/examples/ipyleafletwfs_guide.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/birdy/ipyleafletwfs/examples/quickstart-template.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/birdy/ipyleafletwfs/examples/wfs_constructor.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:06:37.502090 birdhouse-birdy-0.8.3/birdy/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/birdy/templates/cmd.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/birdy/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/requirements_extra.txt
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-05 15:06:37.506090 birdhouse-birdy-0.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:06:37.506090 birdhouse-birdy-0.8.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/tests/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    11959 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/tests/test_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/tests/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/tests/test_notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:23:08.651214 birdhouse-birdy-0.8.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-24 15:23:04.000000 birdhouse-birdy-0.8.4/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-05-24 15:23:04.000000 birdhouse-birdy-0.8.4/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-24 15:23:04.000000 birdhouse-birdy-0.8.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-24 15:23:04.000000 birdhouse-birdy-0.8.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10235 2023-05-24 15:23:08.651214 birdhouse-birdy-0.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-24 15:23:04.000000 birdhouse-birdy-0.8.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:23:08.647214 birdhouse-birdy-0.8.4/birdhouse_birdy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10235 2023-05-24 15:23:08.000000 birdhouse-birdy-0.8.4/birdhouse_birdy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-24 15:23:08.000000 birdhouse-birdy-0.8.4/birdhouse_birdy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:23:08.000000 birdhouse-birdy-0.8.4/birdhouse_birdy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-24 15:23:08.000000 birdhouse-birdy-0.8.4/birdhouse_birdy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-24 15:23:08.000000 birdhouse-birdy-0.8.4/birdhouse_birdy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-24 15:23:08.000000 birdhouse-birdy-0.8.4/birdhouse_birdy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:23:08.647214 birdhouse-birdy-0.8.4/birdy/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-24 15:23:04.000000 birdhouse-birdy-0.8.4/birdy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:23:08.647214 birdhouse-birdy-0.8.4/birdy/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-05-24 15:23:04.000000 birdhouse-birdy-0.8.4/birdy/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-05-24 15:23:04.000000 birdhouse-birdy-0.8.4/birdy/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-24 15:23:04.000000 birdhouse-birdy-0.8.4/birdy/cli/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-05-24 15:23:04.000000 birdhouse-birdy-0.8.4/birdy/cli/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-24 15:23:04.000000 birdhouse-birdy-0.8.4/birdy/cli/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:23:08.647214 birdhouse-birdy-0.8.4/birdy/client/
+-rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-05-24 15:23:04.000000 birdhouse-birdy-0.8.4/birdy/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15857 2023-05-24 15:23:04.000000 birdhouse-birdy-0.8.4/birdy/client/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10679 2023-05-24 15:23:04.000000 birdhouse-birdy-0.8.4/birdy/client/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9416 2023-05-24 15:23:04.000000 birdhouse-birdy-0.8.4/birdy/client/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-24 15:23:04.000000 birdhouse-birdy-0.8.4/birdy/client/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9540 2023-05-24 15:23:04.000000 birdhouse-birdy-0.8.4/birdy/client/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-24 15:23:04.000000 birdhouse-birdy-0.8.4/birdy/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-24 15:23:04.000000 birdhouse-birdy-0.8.4/birdy/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:23:08.647214 birdhouse-birdy-0.8.4/birdy/ipyleafletwfs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-24 15:23:04.000000 birdhouse-birdy-0.8.4/birdy/ipyleafletwfs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-24 15:23:04.000000 birdhouse-birdy-0.8.4/birdy/ipyleafletwfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15068 2023-05-24 15:23:04.000000 birdhouse-birdy-0.8.4/birdy/ipyleafletwfs/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:23:08.647214 birdhouse-birdy-0.8.4/birdy/ipyleafletwfs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-05-24 15:23:04.000000 birdhouse-birdy-0.8.4/birdy/ipyleafletwfs/examples/ipyleafletwfs_guide.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-24 15:23:04.000000 birdhouse-birdy-0.8.4/birdy/ipyleafletwfs/examples/quickstart-template.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-05-24 15:23:04.000000 birdhouse-birdy-0.8.4/birdy/ipyleafletwfs/examples/wfs_constructor.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:23:08.651214 birdhouse-birdy-0.8.4/birdy/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-05-24 15:23:04.000000 birdhouse-birdy-0.8.4/birdy/templates/cmd.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-05-24 15:23:04.000000 birdhouse-birdy-0.8.4/birdy/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-24 15:23:04.000000 birdhouse-birdy-0.8.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-24 15:23:04.000000 birdhouse-birdy-0.8.4/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-24 15:23:04.000000 birdhouse-birdy-0.8.4/requirements_extra.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-24 15:23:08.651214 birdhouse-birdy-0.8.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-05-24 15:23:04.000000 birdhouse-birdy-0.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:23:08.651214 birdhouse-birdy-0.8.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-24 15:23:04.000000 birdhouse-birdy-0.8.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-24 15:23:04.000000 birdhouse-birdy-0.8.4/tests/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-24 15:23:04.000000 birdhouse-birdy-0.8.4/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11959 2023-05-24 15:23:04.000000 birdhouse-birdy-0.8.4/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-05-24 15:23:04.000000 birdhouse-birdy-0.8.4/tests/test_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-24 15:23:04.000000 birdhouse-birdy-0.8.4/tests/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-24 15:23:04.000000 birdhouse-birdy-0.8.4/tests/test_notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-05-24 15:23:04.000000 birdhouse-birdy-0.8.4/tests/test_utils.py
```

### Comparing `birdhouse-birdy-0.8.3/CHANGES.rst` & `birdhouse-birdy-0.8.4/CHANGES.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Change History
 **************
 
+0.8.4 (2023-05-24)
+==================
+
+Changes:
+
+* Fix docstring creation error occurring when the server identification abstract is None. See issue `228`.
+* Handle case where the server `describeProcess` does not understand "ALL" as the process identifier. See issue `229`.
+
 0.8.3 (2023-05-03)
 ==================
 
 Changes:
 
 * Added the `packaging` library to the list of requirements.
```

### Comparing `birdhouse-birdy-0.8.3/LICENSE.txt` & `birdhouse-birdy-0.8.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.3/PKG-INFO` & `birdhouse-birdy-0.8.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: birdhouse-birdy
-Version: 0.8.3
+Version: 0.8.4
 Summary: Birdy provides a command-line tool to work with Web Processing Services.
 Home-page: https://github.com/bird-house/birdy
 Author: Carsten Ehbrecht
 Author-email: ehbrecht@dkrz.de
 License: Apache License v2.0
 Keywords: wps pywps owslib geopython birdy birdhouse
 Classifier: Development Status :: 4 - Beta
@@ -67,19 +67,19 @@
         :alt: GitHub license
 
 .. |Gitter| image:: https://badges.gitter.im/bird-house/birdhouse.svg
         :target: https://gitter.im/bird-house/birdhouse?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
         :alt: Join the chat at https://gitter.im/bird-house/birdhouse
 
 .. |Binder| image:: https://mybinder.org/badge_logo.svg
-        :target: https://mybinder.org/v2/gh/bird-house/birdy.git/v0.8.3?filepath=notebooks
+        :target: https://mybinder.org/v2/gh/bird-house/birdy.git/v0.8.4?filepath=notebooks
         :alt: Binder Launcher
 
 .. |NBViewer| image:: https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg
-        :target: https://nbviewer.jupyter.org/github/bird-house/birdy/tree/v0.8.3/notebooks/
+        :target: https://nbviewer.jupyter.org/github/bird-house/birdy/tree/v0.8.4/notebooks/
         :alt: NBViewer
         :height: 20
 
 Authors
 *******
 
 * David Huard <huard.david@ouranos.ca>
@@ -89,14 +89,22 @@
 ************
 
 * Trevor James Smith <smith.trevorj@ouranos.ca> `@Zeitsperre <https://www.github.com/Zeitsperre>`_
 
 Change History
 **************
 
+0.8.4 (2023-05-24)
+==================
+
+Changes:
+
+* Fix docstring creation error occurring when the server identification abstract is None. See issue `228`.
+* Handle case where the server `describeProcess` does not understand "ALL" as the process identifier. See issue `229`.
+
 0.8.3 (2023-05-03)
 ==================
 
 Changes:
 
 * Added the `packaging` library to the list of requirements.
```

### Comparing `birdhouse-birdy-0.8.3/README.rst` & `birdhouse-birdy-0.8.4/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,14 @@
         :alt: GitHub license
 
 .. |Gitter| image:: https://badges.gitter.im/bird-house/birdhouse.svg
         :target: https://gitter.im/bird-house/birdhouse?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
         :alt: Join the chat at https://gitter.im/bird-house/birdhouse
 
 .. |Binder| image:: https://mybinder.org/badge_logo.svg
-        :target: https://mybinder.org/v2/gh/bird-house/birdy.git/v0.8.3?filepath=notebooks
+        :target: https://mybinder.org/v2/gh/bird-house/birdy.git/v0.8.4?filepath=notebooks
         :alt: Binder Launcher
 
 .. |NBViewer| image:: https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg
-        :target: https://nbviewer.jupyter.org/github/bird-house/birdy/tree/v0.8.3/notebooks/
+        :target: https://nbviewer.jupyter.org/github/bird-house/birdy/tree/v0.8.4/notebooks/
         :alt: NBViewer
         :height: 20
```

### Comparing `birdhouse-birdy-0.8.3/birdhouse_birdy.egg-info/PKG-INFO` & `birdhouse-birdy-0.8.4/birdhouse_birdy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: birdhouse-birdy
-Version: 0.8.3
+Version: 0.8.4
 Summary: Birdy provides a command-line tool to work with Web Processing Services.
 Home-page: https://github.com/bird-house/birdy
 Author: Carsten Ehbrecht
 Author-email: ehbrecht@dkrz.de
 License: Apache License v2.0
 Keywords: wps pywps owslib geopython birdy birdhouse
 Classifier: Development Status :: 4 - Beta
@@ -67,19 +67,19 @@
         :alt: GitHub license
 
 .. |Gitter| image:: https://badges.gitter.im/bird-house/birdhouse.svg
         :target: https://gitter.im/bird-house/birdhouse?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
         :alt: Join the chat at https://gitter.im/bird-house/birdhouse
 
 .. |Binder| image:: https://mybinder.org/badge_logo.svg
-        :target: https://mybinder.org/v2/gh/bird-house/birdy.git/v0.8.3?filepath=notebooks
+        :target: https://mybinder.org/v2/gh/bird-house/birdy.git/v0.8.4?filepath=notebooks
         :alt: Binder Launcher
 
 .. |NBViewer| image:: https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg
-        :target: https://nbviewer.jupyter.org/github/bird-house/birdy/tree/v0.8.3/notebooks/
+        :target: https://nbviewer.jupyter.org/github/bird-house/birdy/tree/v0.8.4/notebooks/
         :alt: NBViewer
         :height: 20
 
 Authors
 *******
 
 * David Huard <huard.david@ouranos.ca>
@@ -89,14 +89,22 @@
 ************
 
 * Trevor James Smith <smith.trevorj@ouranos.ca> `@Zeitsperre <https://www.github.com/Zeitsperre>`_
 
 Change History
 **************
 
+0.8.4 (2023-05-24)
+==================
+
+Changes:
+
+* Fix docstring creation error occurring when the server identification abstract is None. See issue `228`.
+* Handle case where the server `describeProcess` does not understand "ALL" as the process identifier. See issue `229`.
+
 0.8.3 (2023-05-03)
 ==================
 
 Changes:
 
 * Added the `packaging` library to the list of requirements.
```

### Comparing `birdhouse-birdy-0.8.3/birdhouse_birdy.egg-info/SOURCES.txt` & `birdhouse-birdy-0.8.4/birdhouse_birdy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.3/birdy/cli/__init__.py` & `birdhouse-birdy-0.8.4/birdy/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.3/birdy/cli/base.py` & `birdhouse-birdy-0.8.4/birdy/cli/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,15 +57,15 @@
                 self.wps.getcapabilities(xml=self.caps_xml)
             except SSLError:
                 raise ConnectionError(
                     "SSL verfication of server certificate failed. Set WPS_SSL_VERIFY=false."
                 )
             except Exception as e:
                 raise ConnectionError(
-                    "Could not connect to Web Processing Service ({!r})".format(e)
+                    f"Could not connect to Web Processing Service ({e!r})"
                 )
             for process in self.wps.processes:
                 self.commands[process.identifier] = dict(
                     name=process.identifier,
                     url=self.wps.url,
                     version=process.processVersion,
                     help=BirdyCLI.format_command_help(process),
@@ -88,15 +88,15 @@
     def _get_command_info(self, name, ctx):  # noqa: D102
         cmd = self.commands.get(name)
         pp = self.wps.describeprocess(name, xml=self.desc_xml)
         for inp in pp.dataInputs:
             help = inp.title or ""
             default = BirdyCLI.get_param_default(inp)
             if default:
-                help = "{}. Default: {}".format(help, default)
+                help = f"{help}. Default: {default}"
             cmd["options"].append(
                 dict(
                     name=inp.identifier.replace(" ", "-"),
                     # default=BirdyCLI.get_param_default(inp),
                     help=help,
                     type=BirdyCLI.get_param_type(inp),
                     multiple=inp.maxOccurs > 1,
```

### Comparing `birdhouse-birdy-0.8.3/birdy/cli/misc.py` & `birdhouse-birdy-0.8.4/birdy/cli/misc.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,17 +10,15 @@
         while not execution.isComplete():
             execution.checkStatus(sleepSecs=1)
             bar.label = execution.status
             bar.update(max(execution.percentCompleted, 1))
     if execution.isSucceded():
         click.echo("Output:")
         for output in execution.processOutputs:
-            click.echo(
-                "{}={}".format(output.identifier, output.data or output.reference)
-            )
+            click.echo(f"{output.identifier}={output.data or output.reference}")
     else:
         click.echo("Process execution failed.")
 
 
 def get_ssl_verify():  # noqa: D103
     value = os.environ.get("WPS_SSL_VERIFY", "True")
     if value.lower() == "true":
```

### Comparing `birdhouse-birdy-0.8.3/birdy/cli/run.py` & `birdhouse-birdy-0.8.4/birdy/cli/run.py`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.3/birdy/cli/types.py` & `birdhouse-birdy-0.8.4/birdy/cli/types.py`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.3/birdy/client/__init__.py` & `birdhouse-birdy-0.8.4/birdy/client/__init__.py`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.3/birdy/client/base.py` & `birdhouse-birdy-0.8.4/birdy/client/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 # noqa: D100
 
 import logging
 import types
 from collections import OrderedDict
 from textwrap import dedent
+from warnings import warn
 
 import owslib
+import packaging.version
 import requests
 import requests.auth
 from boltons.funcutils import FunctionBuilder
 from owslib.util import ServiceException
 from owslib.wps import (
     ASYNC,
     SYNC,
     WPS_DEFAULT_VERSION,
     ComplexData,
     WebProcessingService,
 )
-from warnings import warn
-import packaging.version
 
 from birdy.client import notebook, utils
 from birdy.client.outputs import WPSResult
 from birdy.exceptions import UnauthorizedException
 from birdy.utils import embed, fix_url, guess_type, sanitize
 
 
 # TODO: Support passing ComplexInput's data using POST.
-class WPSClient(object):
+class WPSClient:
     """Returns a class where every public method is a WPS process available at the given url.
 
     Examples
     --------
     >>> emu = WPSClient(url='<server url>')
     >>> emu.hello('stranger')
     'Hello stranger'
@@ -192,19 +192,20 @@
         -------
         OrderedDict
           A dictionary keyed by the process identifier of process descriptions.
         """
         all_wps_processes = [p.identifier for p in self._wps.processes]
 
         if processes is None:
-            if owslib.__version__ > "0.17.0":
+            try:
                 # Get the description for all processes in one request.
                 ps = self._wps.describeprocess("all", xml=xml)
                 return OrderedDict((p.identifier, p) for p in ps)
-            else:
+
+            except (ServiceException, ValueError):
                 processes = all_wps_processes
 
         # Check for invalid process names, i.e. not matching the getCapabilities response.
 
         process_names, missing = utils.filter_case_insensitive(
             processes, all_wps_processes
         )
@@ -428,17 +429,17 @@
                     execution.process.identifier,
                     execution.percentCompleted,
                     execution.statusMessage[:50],
                 )
             )
 
         if execution.isSucceded():
-            self.logger.info("{} done.".format(execution.process.identifier))
+            self.logger.info(f"{execution.process.identifier} done.")
         else:
-            self.logger.info("{} failed.".format(execution.process.identifier))
+            self.logger.info(f"{execution.process.identifier} failed.")
 
 
 def sort_inputs_key(i):
     """Key function for sorting process inputs.
 
     The order is:
      - Inputs that have minOccurs >= 1 and no default value
```

### Comparing `birdhouse-birdy-0.8.3/birdy/client/converters.py` & `birdhouse-birdy-0.8.4/birdy/client/converters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # noqa: D100
 
 import tempfile
 from distutils.version import StrictVersion
 from importlib import import_module
 from pathlib import Path
 from typing import Sequence, Union
-from birdy.utils import is_opendap_url
+
 from owslib.wps import Output
 
+from birdy.utils import is_opendap_url
+
 from . import notebook as nb
 
 
-class BaseConverter(object):  # noqa: D101
+class BaseConverter:  # noqa: D101
     mimetypes = ()
     extensions = ()
     priority = None
     nested = False
 
     def __init__(self, output=None, path=None, verify=True):
         """Instantiate the conversion class.
```

### Comparing `birdhouse-birdy-0.8.3/birdy/client/notebook.py` & `birdhouse-birdy-0.8.4/birdy/client/notebook.py`

 * *Files 1% similar despite different names*

```diff
@@ -278,15 +278,15 @@
     elif typ.endswith("dateTime"):
         out = widgets.Text(value=default, placeholder="YYYY-MM-DDThh-mm-ss", **kwds)
     elif typ.endswith("angle"):
         out = widgets.BoundedFloatText(min=0, max=360, **kwds)
     elif typ.endswith("ComplexData"):
         out = widgets.Text(description=inpt.title)
     else:
-        raise AttributeError("Data type not recognized {}".format(typ))
+        raise AttributeError(f"Data type not recognized {typ}")
 
     return out
 
 
 def output2widget(output):
     """Return notebook widget based on output mime-type."""
     pass
```

### Comparing `birdhouse-birdy-0.8.3/birdy/client/outputs.py` & `birdhouse-birdy-0.8.4/birdy/client/outputs.py`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.3/birdy/client/utils.py` & `birdhouse-birdy-0.8.4/birdy/client/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,17 +55,15 @@
             return repr(obj)
 
     attributes = []
     indent = "    " if linebreaks else ""
 
     for key, value in items:
         value = pretty_repr(value, linebreaks=False)
-        attributes.append(
-            "{indent}{key}={value}".format(indent=indent, key=key, value=value)
-        )
+        attributes.append(f"{indent}{key}={value}")
 
     attribute_joiner = ",\n" if linebreaks else ", "
     attributes = attribute_joiner.join(attributes)
 
     joiner = "\n" if linebreaks else ""
     return joiner.join([class_name + "(", attributes, ")"])
 
@@ -79,15 +77,15 @@
     processes : Dict[str, owslib.wps.Process]
 
     Returns
     -------
     str
         The formatted docstring for this WPSClient
     """
-    doc = [wps.identification.abstract, "", "Processes", "---------", ""]
+    doc = [wps.identification.abstract or "", "", "Processes", "---------", ""]
 
     for process_name, process in list(processes.items()):
         sanitized_name = sanitize(process_name)
         description = "{name}\n    {abstract}".format(
             name=sanitized_name, abstract=process.abstract or "(No description)"
         )
         doc.append(description)
@@ -106,40 +104,40 @@
     doc = [process.abstract or "", ""]
 
     # Inputs
     if process.dataInputs:
         doc.append("Parameters")
         doc.append("----------")
         for i in process.dataInputs:
-            doc.append("{} : {}".format(sanitize(i.identifier), format_type(i)))
-            doc.append("    {}".format(i.abstract or i.title))
+            doc.append(f"{sanitize(i.identifier)} : {format_type(i)}")
+            doc.append(f"    {i.abstract or i.title}")
             # if i.metadata:
             #    doc[-1] += " ({})".format(', '.join(['`{} <{}>`_'.format(m.title, m.href) for m in i.metadata]))
         doc.append("")
 
     # Outputs
     if process.processOutputs:
         doc.append("Returns")
         doc.append("-------")
         for i in process.processOutputs:
-            doc.append("{} : {}".format(sanitize(i.identifier), format_type(i)))
-            doc.append("    {}".format(i.abstract or i.title))
+            doc.append(f"{sanitize(i.identifier)} : {format_type(i)}")
+            doc.append(f"    {i.abstract or i.title}")
 
     doc.append("")
     return "\n".join(doc)
 
 
 def format_type(obj):
     """Create docstring entry for input parameter from an OWSlib object."""
     nmax = 10
 
     doc = ""
     try:
         if getattr(obj, "allowedValues", None):
-            av = ", ".join(["'{}'".format(i) for i in obj.allowedValues[:nmax]])
+            av = ", ".join([f"'{i}'" for i in obj.allowedValues[:nmax]])
             if len(obj.allowedValues) > nmax:
                 av += ", ..."
             doc += "{" + av + "}"
 
         if getattr(obj, "dataType", None):
             doc += obj.dataType
 
@@ -157,21 +155,21 @@
                 crss += ", ..."
             doc += "[" + crss + "]"
 
         if getattr(obj, "minOccurs", None) and obj.minOccurs == 0:
             doc += ", optional"
 
         if getattr(obj, "default", None):
-            doc += ", default:{}".format(obj.defaultValue)
+            doc += f", default:{obj.defaultValue}"
 
         if getattr(obj, "uoms", None):
             doc += ", units:[{}]".format(", ".join([u.uom for u in obj.uoms]))
 
     except Exception as e:
-        raise type(e)("{} (in {} docstring)".format(e, obj.identifier))
+        raise type(e)(f"{e} (in {obj.identifier} docstring)")
     return doc
 
 
 def is_embedded_in_request(url, value):
     """Whether or not to encode the value as raw data content.
 
     Returns True if
@@ -194,17 +192,15 @@
         p = Path(v.path)
         scheme = v.scheme
 
     if scheme == "file":  # Explicit link to file
         if is_file(p):
             return "localhost" not in u.netloc
         else:
-            raise IOError(
-                "{} should be a local file but was not found on disk.".format(value)
-            )
+            raise OSError(f"{value} should be a local file but was not found on disk.")
     elif scheme == "":  # Could be a local path or just a string
         if is_file(p):
             return "localhost" not in u.netloc
         else:
             return True
     else:  # Other URL (http, https, ftp, ...)
         return False
```

### Comparing `birdhouse-birdy-0.8.3/birdy/dependencies.py` & `birdhouse-birdy-0.8.4/birdy/dependencies.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-
 """
 Module for managing optional dependencies.
 
 Example usage::
 
     from birdy.dependencies import ipywidgets as widgets
 """
```

### Comparing `birdhouse-birdy-0.8.3/birdy/ipyleafletwfs/README.md` & `birdhouse-birdy-0.8.4/birdy/ipyleafletwfs/README.md`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.3/birdy/ipyleafletwfs/base.py` & `birdhouse-birdy-0.8.4/birdy/ipyleafletwfs/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     lon2 = coords[1][1]
     lat2 = coords[1][0]
     formatted_coordinates = (lon1, lat1, lon2, lat2)
 
     return formatted_coordinates
 
 
-class IpyleafletWFS(object):
+class IpyleafletWFS:
     """Create a connection to a WFS service capable of geojson output.
 
     This class is a small wrapper for ipylealet to facilitate the use of
     a WFS service, as well as provide some automation.
 
     Request to the WFS service is done through the owslib module and requires
     a geojson output capable WFS. The geojson data is filtered for the map extent
```

### Comparing `birdhouse-birdy-0.8.3/birdy/ipyleafletwfs/examples/ipyleafletwfs_guide.ipynb` & `birdhouse-birdy-0.8.4/birdy/ipyleafletwfs/examples/ipyleafletwfs_guide.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998697916666667%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(1, '\\n'), (2, 'from birdy import IpyleafletWFS\\n')], "*

 * *            'delete: [0]}}}'}*

```diff
@@ -12,17 +12,18 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from birdy import IpyleafletWFS\n",
                 "from ipyleaflet import Map\n",
                 "\n",
+                "from birdy import IpyleafletWFS\n",
+                "\n",
                 "url = \"http://boreas.ouranos.ca/geoserver/wfs\"\n",
                 "version = \"2.0.0\"\n",
                 "\n",
                 "wfs_connection = IpyleafletWFS(url, version)\n",
                 "\n",
                 "demo_map = Map(center=(46.42, -64.14), zoom=8)\n",
                 "demo_map"
```

### Comparing `birdhouse-birdy-0.8.3/birdy/ipyleafletwfs/examples/quickstart-template.ipynb` & `birdhouse-birdy-0.8.4/birdy/ipyleafletwfs/examples/quickstart-template.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994642857142857%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(1, '\\n'), (2, 'from birdy import IpyleafletWFS\\n')], "*

 * *            'delete: [0]}}}'}*

```diff
@@ -13,17 +13,18 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from birdy import IpyleafletWFS\n",
                 "from ipyleaflet import Map\n",
                 "\n",
+                "from birdy import IpyleafletWFS\n",
+                "\n",
                 "# Initialize the connection\n",
                 "url = \"http://boreas.ouranos.ca/geoserver/wfs\"\n",
                 "version = \"2.0.0\"\n",
                 "\n",
                 "boreas_wfs = IpyleafletWFS(url, version)\n",
                 "\n",
                 "# Create and render map\n",
```

### Comparing `birdhouse-birdy-0.8.3/birdy/ipyleafletwfs/examples/wfs_constructor.ipynb` & `birdhouse-birdy-0.8.4/birdy/ipyleafletwfs/examples/wfs_constructor.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.99953125%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(1, '\\n'), (2, 'from birdy import IpyleafletWFS\\n')], "*

 * *            'delete: [0]}}}'}*

```diff
@@ -11,17 +11,18 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from birdy import IpyleafletWFS\n",
                 "from ipyleaflet import Map\n",
                 "\n",
+                "from birdy import IpyleafletWFS\n",
+                "\n",
                 "# Create connection\n",
                 "url = \"http://boreas.ouranos.ca/geoserver/wfs\"\n",
                 "version = \"2.0.0\"\n",
                 "\n",
                 "wfs = IpyleafletWFS(url, version)"
             ]
         },
```

### Comparing `birdhouse-birdy-0.8.3/birdy/templates/cmd.py.j2` & `birdhouse-birdy-0.8.4/birdy/templates/cmd.py.j2`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.3/birdy/utils.py` & `birdhouse-birdy-0.8.4/birdy/utils.py`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.3/setup.cfg` & `birdhouse-birdy-0.8.4/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.8.3
+current_version = 0.8.4
 commit = True
 tag = False
 
 [metadata]
 description-file = README.rst
 
 [bumpversion:file:birdy/__init__.py]
```

### Comparing `birdhouse-birdy-0.8.3/setup.py` & `birdhouse-birdy-0.8.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # noqa: D100
 
 import re
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
@@ -16,15 +15,15 @@
         git_url_match = egg_regex.search(req)
         if git_url_match:
             req = git_url_match.group(1)
         reqs.append(req)
     return reqs
 
 
-with open(Path(__file__).parent / "birdy" / "__init__.py", "r") as f:
+with open(Path(__file__).parent / "birdy" / "__init__.py") as f:
     version = re.search(r'__version__ = [\'"](.+?)[\'"]', f.read()).group(1)
 
 description = "Birdy provides a command-line tool to work with Web Processing Services."
 long_description = (
     open("README.rst").read()
     + "\n"
     + open("AUTHORS.rst").read()
```

### Comparing `birdhouse-birdy-0.8.3/tests/test_cli.py` & `birdhouse-birdy-0.8.4/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.3/tests/test_client.py` & `birdhouse-birdy-0.8.4/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.3/tests/test_converters.py` & `birdhouse-birdy-0.8.4/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.3/tests/test_utils.py` & `birdhouse-birdy-0.8.4/tests/test_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # noqa
 
-import pytest
 from pathlib import Path
 
+import pytest
+
 from birdy import utils
 
 from .common import resource_file
 
 
 def test_is_url():  # noqa: D103
     assert utils.is_url("http://localhost:5000/wps")
```

