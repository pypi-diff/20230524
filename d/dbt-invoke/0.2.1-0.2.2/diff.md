# Comparing `tmp/dbt-invoke-0.2.1.tar.gz` & `tmp/dbt-invoke-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-invoke-0.2.1.tar", last modified: Wed Feb 22 18:33:29 2023, max compression
+gzip compressed data, was "dbt-invoke-0.2.2.tar", last modified: Wed May 24 00:47:42 2023, max compression
```

## Comparing `dbt-invoke-0.2.1.tar` & `dbt-invoke-0.2.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 18:33:29.375645 dbt-invoke-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-22 18:33:19.000000 dbt-invoke-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10361 2023-02-22 18:33:29.375645 dbt-invoke-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8188 2023-02-22 18:33:19.000000 dbt-invoke-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 18:33:29.371646 dbt-invoke-0.2.1/dbt_invoke/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 18:33:19.000000 dbt-invoke-0.2.1/dbt_invoke/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 18:33:29.375645 dbt-invoke-0.2.1/dbt_invoke/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 18:33:19.000000 dbt-invoke-0.2.1/dbt_invoke/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14975 2023-02-22 18:33:19.000000 dbt-invoke-0.2.1/dbt_invoke/internal/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-22 18:33:19.000000 dbt-invoke-0.2.1/dbt_invoke/internal/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-02-22 18:33:19.000000 dbt-invoke-0.2.1/dbt_invoke/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    33712 2023-02-22 18:33:19.000000 dbt-invoke-0.2.1/dbt_invoke/properties.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 18:33:29.371646 dbt-invoke-0.2.1/dbt_invoke.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10361 2023-02-22 18:33:29.000000 dbt-invoke-0.2.1/dbt_invoke.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-02-22 18:33:29.000000 dbt-invoke-0.2.1/dbt_invoke.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 18:33:29.000000 dbt-invoke-0.2.1/dbt_invoke.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-02-22 18:33:29.000000 dbt-invoke-0.2.1/dbt_invoke.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-02-22 18:33:29.000000 dbt-invoke-0.2.1/dbt_invoke.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-22 18:33:29.000000 dbt-invoke-0.2.1/dbt_invoke.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-22 18:33:29.375645 dbt-invoke-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-02-22 18:33:19.000000 dbt-invoke-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 00:47:42.184163 dbt-invoke-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-24 00:47:27.000000 dbt-invoke-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10361 2023-05-24 00:47:42.184163 dbt-invoke-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8188 2023-05-24 00:47:27.000000 dbt-invoke-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 00:47:42.180163 dbt-invoke-0.2.2/dbt_invoke/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 00:47:27.000000 dbt-invoke-0.2.2/dbt_invoke/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 00:47:42.184163 dbt-invoke-0.2.2/dbt_invoke/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 00:47:27.000000 dbt-invoke-0.2.2/dbt_invoke/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15292 2023-05-24 00:47:27.000000 dbt-invoke-0.2.2/dbt_invoke/internal/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-24 00:47:27.000000 dbt-invoke-0.2.2/dbt_invoke/internal/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-24 00:47:27.000000 dbt-invoke-0.2.2/dbt_invoke/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33712 2023-05-24 00:47:27.000000 dbt-invoke-0.2.2/dbt_invoke/properties.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 00:47:42.184163 dbt-invoke-0.2.2/dbt_invoke.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10361 2023-05-24 00:47:41.000000 dbt-invoke-0.2.2/dbt_invoke.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-24 00:47:42.000000 dbt-invoke-0.2.2/dbt_invoke.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 00:47:41.000000 dbt-invoke-0.2.2/dbt_invoke.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-24 00:47:41.000000 dbt-invoke-0.2.2/dbt_invoke.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-24 00:47:41.000000 dbt-invoke-0.2.2/dbt_invoke.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-24 00:47:41.000000 dbt-invoke-0.2.2/dbt_invoke.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 00:47:42.184163 dbt-invoke-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-24 00:47:27.000000 dbt-invoke-0.2.2/setup.py
```

### Comparing `dbt-invoke-0.2.1/LICENSE` & `dbt-invoke-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-invoke-0.2.1/PKG-INFO` & `dbt-invoke-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-invoke
-Version: 0.2.1
+Version: 0.2.2
 Summary: dbt-invoke is a CLI for creating, updating, and deleting dbt property files.
 Home-page: https://github.com/Dashlane/dbt-invoke
 Author: Robert Astel, Jennifer Zhan, Vincent Dragonette
 Author-email: rob.astel@gmail.com
 License: Apache License 2.0
 Description: # dbt-invoke
```

### Comparing `dbt-invoke-0.2.1/README.md` & `dbt-invoke-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `dbt-invoke-0.2.1/dbt_invoke/internal/_utils.py` & `dbt-invoke-0.2.2/dbt_invoke/internal/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,25 @@
 import json
 import logging
 from pathlib import Path
 import sys
 import platform
 import re
 from dbt.task.base import get_nearest_project_dir
+
+try:
+    from importlib.metadata import version
+
+    DBT_VERSION = version('dbt-core')
+
+except ImportError:
+    import pkg_resources
+
+    DBT_VERSION = pkg_resources.get_distribution('dbt-core').version
+
 from ruamel.yaml import YAML, YAMLError
 
 MACROS = {
     '_log_columns_list': (
         "\n{# This macro is intended for use by dbt-invoke #}"
         "\n{% macro _log_columns_list(sql=none, resource_name=none) %}"
         "\n    {% if sql is none %}"
@@ -103,15 +114,18 @@
     and store them in ctx (an Invoke context object)
 
     :param ctx: An Invoke context object
     :param project_dir: A directory containing a dbt_project.yml file
     :return: None
     """
     project = Project(project_dir)
-    project_path = get_nearest_project_dir(project)
+    if DBT_VERSION < '1.5.0':
+        project_path = get_nearest_project_dir(project)
+    else:
+        project_path = get_nearest_project_dir(project.project_dir)
     project_yml_path = Path(project_path, 'dbt_project.yml')
     # Get project configuration values from dbt_project.yml
     # (or use dbt defaults)
     project_yml = parse_yaml(project_yml_path)
     project_name = project_yml.get('name')
     target_path = Path(project_path, project_yml.get('target-path', 'target'))
     compiled_path = Path(target_path, 'compiled', project_name)
```

### Comparing `dbt-invoke-0.2.1/dbt_invoke/properties.py` & `dbt-invoke-0.2.2/dbt_invoke/properties.py`

 * *Files identical despite different names*

### Comparing `dbt-invoke-0.2.1/dbt_invoke.egg-info/PKG-INFO` & `dbt-invoke-0.2.2/dbt_invoke.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-invoke
-Version: 0.2.1
+Version: 0.2.2
 Summary: dbt-invoke is a CLI for creating, updating, and deleting dbt property files.
 Home-page: https://github.com/Dashlane/dbt-invoke
 Author: Robert Astel, Jennifer Zhan, Vincent Dragonette
 Author-email: rob.astel@gmail.com
 License: Apache License 2.0
 Description: # dbt-invoke
```

### Comparing `dbt-invoke-0.2.1/setup.py` & `dbt-invoke-0.2.2/setup.py`

 * *Files identical despite different names*

