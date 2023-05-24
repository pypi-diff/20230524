# Comparing `tmp/pybuilder-integration-91.tar.gz` & `tmp/pybuilder-integration-92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybuilder-integration-91.tar", last modified: Tue May 23 23:54:54 2023, max compression
+gzip compressed data, was "pybuilder-integration-92.tar", last modified: Tue May 23 23:55:33 2023, max compression
```

## Comparing `pybuilder-integration-91.tar` & `pybuilder-integration-92.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:54:54.535851 pybuilder-integration-91/
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-23 23:54:54.531851 pybuilder-integration-91/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:54:54.531851 pybuilder-integration-91/pybuilder_integration/
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-23 23:54:10.000000 pybuilder-integration-91/pybuilder_integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9718 2023-05-23 23:54:10.000000 pybuilder-integration-91/pybuilder_integration/artifact_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-23 23:54:10.000000 pybuilder-integration-91/pybuilder_integration/cloudwatchlogs_utility.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-05-23 23:54:10.000000 pybuilder-integration-91/pybuilder_integration/directory_utility.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-05-23 23:54:10.000000 pybuilder-integration-91/pybuilder_integration/exec_utility.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-23 23:54:10.000000 pybuilder-integration-91/pybuilder_integration/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    12026 2023-05-23 23:54:10.000000 pybuilder-integration-91/pybuilder_integration/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-23 23:54:10.000000 pybuilder-integration-91/pybuilder_integration/tool_utility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:54:54.531851 pybuilder-integration-91/pybuilder_integration.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-23 23:54:54.000000 pybuilder-integration-91/pybuilder_integration.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-23 23:54:54.000000 pybuilder-integration-91/pybuilder_integration.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 23:54:54.000000 pybuilder-integration-91/pybuilder_integration.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 23:54:54.000000 pybuilder-integration-91/pybuilder_integration.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-23 23:54:54.000000 pybuilder-integration-91/pybuilder_integration.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-23 23:54:54.000000 pybuilder-integration-91/pybuilder_integration.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 23:54:54.000000 pybuilder-integration-91/pybuilder_integration.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 23:54:54.535851 pybuilder-integration-91/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1682 2023-05-23 23:54:51.000000 pybuilder-integration-91/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:55:33.987875 pybuilder-integration-92/
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-23 23:55:33.987875 pybuilder-integration-92/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:55:33.987875 pybuilder-integration-92/pybuilder_integration/
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-23 23:54:57.000000 pybuilder-integration-92/pybuilder_integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9718 2023-05-23 23:54:57.000000 pybuilder-integration-92/pybuilder_integration/artifact_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-23 23:54:57.000000 pybuilder-integration-92/pybuilder_integration/cloudwatchlogs_utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-05-23 23:54:57.000000 pybuilder-integration-92/pybuilder_integration/directory_utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-05-23 23:54:57.000000 pybuilder-integration-92/pybuilder_integration/exec_utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-23 23:54:57.000000 pybuilder-integration-92/pybuilder_integration/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12078 2023-05-23 23:54:57.000000 pybuilder-integration-92/pybuilder_integration/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-23 23:54:57.000000 pybuilder-integration-92/pybuilder_integration/tool_utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:55:33.987875 pybuilder-integration-92/pybuilder_integration.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-23 23:55:33.000000 pybuilder-integration-92/pybuilder_integration.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-23 23:55:33.000000 pybuilder-integration-92/pybuilder_integration.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 23:55:33.000000 pybuilder-integration-92/pybuilder_integration.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 23:55:33.000000 pybuilder-integration-92/pybuilder_integration.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-23 23:55:33.000000 pybuilder-integration-92/pybuilder_integration.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-23 23:55:33.000000 pybuilder-integration-92/pybuilder_integration.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 23:55:33.000000 pybuilder-integration-92/pybuilder_integration.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 23:55:33.987875 pybuilder-integration-92/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1682 2023-05-23 23:55:32.000000 pybuilder-integration-92/setup.py
```

### Comparing `pybuilder-integration-91/PKG-INFO` & `pybuilder-integration-92/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybuilder-integration
-Version: 91
+Version: 92
 Summary: A pybuilder plugin that runs integration tests (Tavern & Cypress) against a target.
 Home-page: https://github.com/rspitler/pybuilder-integration
 Author: 
 Author-email: 
 Maintainer: 
 Maintainer-email: 
 License: Apache 2.0
```

### Comparing `pybuilder-integration-91/pybuilder_integration/__init__.py` & `pybuilder-integration-92/pybuilder_integration/__init__.py`

 * *Files identical despite different names*

### Comparing `pybuilder-integration-91/pybuilder_integration/artifact_manager.py` & `pybuilder-integration-92/pybuilder_integration/artifact_manager.py`

 * *Files identical despite different names*

### Comparing `pybuilder-integration-91/pybuilder_integration/cloudwatchlogs_utility.py` & `pybuilder-integration-92/pybuilder_integration/cloudwatchlogs_utility.py`

 * *Files identical despite different names*

### Comparing `pybuilder-integration-91/pybuilder_integration/directory_utility.py` & `pybuilder-integration-92/pybuilder_integration/directory_utility.py`

 * *Files identical despite different names*

### Comparing `pybuilder-integration-91/pybuilder_integration/exec_utility.py` & `pybuilder-integration-92/pybuilder_integration/exec_utility.py`

 * *Files identical despite different names*

### Comparing `pybuilder-integration-91/pybuilder_integration/properties.py` & `pybuilder-integration-92/pybuilder_integration/properties.py`

 * *Files identical despite different names*

### Comparing `pybuilder-integration-91/pybuilder_integration/tasks.py` & `pybuilder-integration-92/pybuilder_integration/tasks.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,14 +109,15 @@
     total_time = Timer.start()
     target_url = project.get_mandatory_property(INTEGRATION_TARGET_URL)
     environment = project.get_mandatory_property(ENVIRONMENT)
     if not os.path.exists(work_dir):
         logger.info("Skipping cypress run: no tests")
         return False
     logger.info(f"Found {len(os.listdir(work_dir))} files in cypress test directory")
+    logger.debug(f"Files: {os.listdir(work_dir)} ")
     # Validate NPM install and Install cypress
     package_json = os.path.join(work_dir, "package.json")
     if os.path.exists(package_json):
         logger.info("Found package.json installing dependencies")
         tool_utility.install_npm_dependencies(work_dir, project=project, logger=logger, reactor=reactor)
     else:
         install_cypress(logger=logger, project=project, reactor=reactor, work_dir=work_dir)
```

### Comparing `pybuilder-integration-91/pybuilder_integration/tool_utility.py` & `pybuilder-integration-92/pybuilder_integration/tool_utility.py`

 * *Files identical despite different names*

### Comparing `pybuilder-integration-91/pybuilder_integration.egg-info/PKG-INFO` & `pybuilder-integration-92/pybuilder_integration.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybuilder-integration
-Version: 91
+Version: 92
 Summary: A pybuilder plugin that runs integration tests (Tavern & Cypress) against a target.
 Home-page: https://github.com/rspitler/pybuilder-integration
 Author: 
 Author-email: 
 Maintainer: 
 Maintainer-email: 
 License: Apache 2.0
```

### Comparing `pybuilder-integration-91/pybuilder_integration.egg-info/SOURCES.txt` & `pybuilder-integration-92/pybuilder_integration.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pybuilder-integration-91/setup.py` & `pybuilder-integration-92/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         _install.run(self)
 
         self.post_install_script()
 
 if __name__ == '__main__':
     setup(
         name = 'pybuilder-integration',
-        version = '91',
+        version = '92',
         description = 'A pybuilder plugin that runs integration tests (Tavern & Cypress) against a target.',
         long_description = 'A pybuilder plugin that runs integration tests against a target.  This is intended to be a broader scope than unit-tests encompassing dependant functionality.',
         long_description_content_type = None,
         classifiers = [
             'Development Status :: 3 - Alpha',
             'Programming Language :: Python'
         ],
```

