# Comparing `tmp/dapr-ext-workflow-dev-0.0.1rc1.dev1574.tar.gz` & `tmp/dapr-ext-workflow-dev-0.0.1rc1.dev1577.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dapr-ext-workflow-dev-0.0.1rc1.dev1574.tar", last modified: Wed May 24 16:41:16 2023, max compression
+gzip compressed data, was "dist/dapr-ext-workflow-dev-0.0.1rc1.dev1577.tar", last modified: Wed May 24 16:43:37 2023, max compression
```

## Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1574.tar` & `dapr-ext-workflow-dev-0.0.1rc1.dev1577.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:41:16.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1574/
--rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-05-24 16:40:55.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1574/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-24 16:41:16.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1574/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-24 16:40:55.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1574/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:41:16.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1574/dapr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:41:16.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1574/dapr/ext/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:41:16.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1574/dapr/ext/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-24 16:40:55.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1574/dapr/ext/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10662 2023-05-24 16:40:55.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1574/dapr/ext/workflow/dapr_workflow_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-05-24 16:40:55.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1574/dapr/ext/workflow/dapr_workflow_context.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-24 16:40:55.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1574/dapr/ext/workflow/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-24 16:40:55.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1574/dapr/ext/workflow/workflow_activity_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-05-24 16:40:55.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1574/dapr/ext/workflow/workflow_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-05-24 16:40:55.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1574/dapr/ext/workflow/workflow_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-05-24 16:40:55.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1574/dapr/ext/workflow/workflow_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:41:16.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1574/dapr_ext_workflow_dev.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-24 16:41:16.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1574/dapr_ext_workflow_dev.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-24 16:41:16.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1574/dapr_ext_workflow_dev.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 16:41:16.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1574/dapr_ext_workflow_dev.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-24 16:41:16.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1574/dapr_ext_workflow_dev.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-24 16:41:16.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1574/dapr_ext_workflow_dev.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-24 16:41:16.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1574/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-24 16:40:55.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1574/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:43:37.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1577/
+-rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-05-24 16:43:18.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1577/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-24 16:43:37.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1577/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-24 16:43:18.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1577/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:43:37.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1577/dapr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:43:37.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1577/dapr/ext/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:43:37.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1577/dapr/ext/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-24 16:43:18.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1577/dapr/ext/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10662 2023-05-24 16:43:18.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1577/dapr/ext/workflow/dapr_workflow_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-05-24 16:43:18.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1577/dapr/ext/workflow/dapr_workflow_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-24 16:43:18.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1577/dapr/ext/workflow/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-24 16:43:18.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1577/dapr/ext/workflow/workflow_activity_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-05-24 16:43:18.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1577/dapr/ext/workflow/workflow_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-05-24 16:43:18.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1577/dapr/ext/workflow/workflow_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-05-24 16:43:18.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1577/dapr/ext/workflow/workflow_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:43:37.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1577/dapr_ext_workflow_dev.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-24 16:43:37.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1577/dapr_ext_workflow_dev.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-24 16:43:37.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1577/dapr_ext_workflow_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 16:43:37.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1577/dapr_ext_workflow_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-24 16:43:37.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1577/dapr_ext_workflow_dev.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-24 16:43:37.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1577/dapr_ext_workflow_dev.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-24 16:43:37.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1577/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-24 16:43:18.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1577/setup.py
```

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1574/LICENSE` & `dapr-ext-workflow-dev-0.0.1rc1.dev1577/LICENSE`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1574/PKG-INFO` & `dapr-ext-workflow-dev-0.0.1rc1.dev1577/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: dapr-ext-workflow-dev
-Version: 0.0.1rc1.dev1574
+Version: 0.0.1rc1.dev1577
 Summary: The developmental release for Dapr Workflow Authoring.
 Home-page: https://dapr.io/
 Author: Dapr Authors
 Author-email: daprweb@microsoft.com
 License: Apache
 Project-URL: Documentation, https://github.com/dapr/docs
 Project-URL: Source, https://github.com/dapr/python-sdk
```

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1574/dapr/ext/workflow/__init__.py` & `dapr-ext-workflow-dev-0.0.1rc1.dev1577/dapr/ext/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1574/dapr/ext/workflow/dapr_workflow_client.py` & `dapr-ext-workflow-dev-0.0.1rc1.dev1577/dapr/ext/workflow/dapr_workflow_client.py`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1574/dapr/ext/workflow/dapr_workflow_context.py` & `dapr-ext-workflow-dev-0.0.1rc1.dev1577/dapr/ext/workflow/dapr_workflow_context.py`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1574/dapr/ext/workflow/version.py` & `dapr-ext-workflow-dev-0.0.1rc1.dev1577/dapr/ext/workflow/version.py`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1574/dapr/ext/workflow/workflow_activity_context.py` & `dapr-ext-workflow-dev-0.0.1rc1.dev1577/dapr/ext/workflow/workflow_activity_context.py`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1574/dapr/ext/workflow/workflow_context.py` & `dapr-ext-workflow-dev-0.0.1rc1.dev1577/dapr/ext/workflow/workflow_context.py`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1574/dapr/ext/workflow/workflow_runtime.py` & `dapr-ext-workflow-dev-0.0.1rc1.dev1577/dapr/ext/workflow/workflow_runtime.py`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1574/dapr/ext/workflow/workflow_state.py` & `dapr-ext-workflow-dev-0.0.1rc1.dev1577/dapr/ext/workflow/workflow_state.py`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1574/dapr_ext_workflow_dev.egg-info/PKG-INFO` & `dapr-ext-workflow-dev-0.0.1rc1.dev1577/dapr_ext_workflow_dev.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: dapr-ext-workflow-dev
-Version: 0.0.1rc1.dev1574
+Version: 0.0.1rc1.dev1577
 Summary: The developmental release for Dapr Workflow Authoring.
 Home-page: https://dapr.io/
 Author: Dapr Authors
 Author-email: daprweb@microsoft.com
 License: Apache
 Project-URL: Documentation, https://github.com/dapr/docs
 Project-URL: Source, https://github.com/dapr/python-sdk
```

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1574/dapr_ext_workflow_dev.egg-info/SOURCES.txt` & `dapr-ext-workflow-dev-0.0.1rc1.dev1577/dapr_ext_workflow_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1574/setup.cfg` & `dapr-ext-workflow-dev-0.0.1rc1.dev1577/setup.cfg`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1574/setup.py` & `dapr-ext-workflow-dev-0.0.1rc1.dev1577/setup.py`

 * *Files identical despite different names*

