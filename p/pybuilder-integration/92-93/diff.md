# Comparing `tmp/pybuilder-integration-92.tar.gz` & `tmp/pybuilder-integration-93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybuilder-integration-92.tar", last modified: Tue May 23 23:55:33 2023, max compression
+gzip compressed data, was "pybuilder-integration-93.tar", last modified: Wed May 24 12:59:57 2023, max compression
```

## Comparing `pybuilder-integration-92.tar` & `pybuilder-integration-93.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:55:33.987875 pybuilder-integration-92/
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-23 23:55:33.987875 pybuilder-integration-92/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:55:33.987875 pybuilder-integration-92/pybuilder_integration/
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-23 23:54:57.000000 pybuilder-integration-92/pybuilder_integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9718 2023-05-23 23:54:57.000000 pybuilder-integration-92/pybuilder_integration/artifact_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-23 23:54:57.000000 pybuilder-integration-92/pybuilder_integration/cloudwatchlogs_utility.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-05-23 23:54:57.000000 pybuilder-integration-92/pybuilder_integration/directory_utility.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-05-23 23:54:57.000000 pybuilder-integration-92/pybuilder_integration/exec_utility.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-23 23:54:57.000000 pybuilder-integration-92/pybuilder_integration/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    12078 2023-05-23 23:54:57.000000 pybuilder-integration-92/pybuilder_integration/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-23 23:54:57.000000 pybuilder-integration-92/pybuilder_integration/tool_utility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:55:33.987875 pybuilder-integration-92/pybuilder_integration.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-23 23:55:33.000000 pybuilder-integration-92/pybuilder_integration.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-23 23:55:33.000000 pybuilder-integration-92/pybuilder_integration.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 23:55:33.000000 pybuilder-integration-92/pybuilder_integration.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 23:55:33.000000 pybuilder-integration-92/pybuilder_integration.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-23 23:55:33.000000 pybuilder-integration-92/pybuilder_integration.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-23 23:55:33.000000 pybuilder-integration-92/pybuilder_integration.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 23:55:33.000000 pybuilder-integration-92/pybuilder_integration.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 23:55:33.987875 pybuilder-integration-92/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1682 2023-05-23 23:55:32.000000 pybuilder-integration-92/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:59:57.550470 pybuilder-integration-93/
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-24 12:59:57.550470 pybuilder-integration-93/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:59:57.550470 pybuilder-integration-93/pybuilder_integration/
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-24 12:59:24.000000 pybuilder-integration-93/pybuilder_integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9660 2023-05-24 12:59:24.000000 pybuilder-integration-93/pybuilder_integration/artifact_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-24 12:59:24.000000 pybuilder-integration-93/pybuilder_integration/cloudwatchlogs_utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-05-24 12:59:24.000000 pybuilder-integration-93/pybuilder_integration/directory_utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-05-24 12:59:24.000000 pybuilder-integration-93/pybuilder_integration/exec_utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-24 12:59:24.000000 pybuilder-integration-93/pybuilder_integration/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12557 2023-05-24 12:59:24.000000 pybuilder-integration-93/pybuilder_integration/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-24 12:59:24.000000 pybuilder-integration-93/pybuilder_integration/tool_utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:59:57.550470 pybuilder-integration-93/pybuilder_integration.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-24 12:59:57.000000 pybuilder-integration-93/pybuilder_integration.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-24 12:59:57.000000 pybuilder-integration-93/pybuilder_integration.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 12:59:57.000000 pybuilder-integration-93/pybuilder_integration.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 12:59:57.000000 pybuilder-integration-93/pybuilder_integration.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-24 12:59:57.000000 pybuilder-integration-93/pybuilder_integration.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-24 12:59:57.000000 pybuilder-integration-93/pybuilder_integration.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 12:59:57.000000 pybuilder-integration-93/pybuilder_integration.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 12:59:57.550470 pybuilder-integration-93/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1682 2023-05-24 12:59:55.000000 pybuilder-integration-93/setup.py
```

### Comparing `pybuilder-integration-92/PKG-INFO` & `pybuilder-integration-93/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybuilder-integration
-Version: 92
+Version: 93
 Summary: A pybuilder plugin that runs integration tests (Tavern & Cypress) against a target.
 Home-page: https://github.com/rspitler/pybuilder-integration
 Author: 
 Author-email: 
 Maintainer: 
 Maintainer-email: 
 License: Apache 2.0
```

### Comparing `pybuilder-integration-92/pybuilder_integration/__init__.py` & `pybuilder-integration-93/pybuilder_integration/__init__.py`

 * *Files identical despite different names*

### Comparing `pybuilder-integration-92/pybuilder_integration/artifact_manager.py` & `pybuilder-integration-93/pybuilder_integration/artifact_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,21 +100,25 @@
                                   project=project,
                                   reactor=reactor,
                                   logger=logger,
                                   report=False)
 
     def does_bucket_exist(self, logger, project, reactor):
         app_group, app_name, bucket, environment, role = get_project_metadata(logger, project)
+
+        args = [
+            's3api',
+            'head-bucket',
+            '--bucket',
+            bucket
+        ]
+        if project.get_property("verbose", False):
+            args.append('--debug')
         return exec_utility.exec_command(command_name='aws',
-                                         args=[
-                                             's3api',
-                                             'head-bucket',
-                                             '--bucket',
-                                             bucket
-                                         ],
+                                         args=args,
                                          failure_message=f"Failed to find bucket",
                                          log_file_name='s3-head-bucket',
                                          project=project,
                                          reactor=reactor,
                                          logger=logger,
                                          raise_exception=True,
                                          report=True)
```

### Comparing `pybuilder-integration-92/pybuilder_integration/cloudwatchlogs_utility.py` & `pybuilder-integration-93/pybuilder_integration/cloudwatchlogs_utility.py`

 * *Files identical despite different names*

### Comparing `pybuilder-integration-92/pybuilder_integration/directory_utility.py` & `pybuilder-integration-93/pybuilder_integration/directory_utility.py`

 * *Files identical despite different names*

### Comparing `pybuilder-integration-92/pybuilder_integration/exec_utility.py` & `pybuilder-integration-93/pybuilder_integration/exec_utility.py`

 * *Files identical despite different names*

### Comparing `pybuilder-integration-92/pybuilder_integration/properties.py` & `pybuilder-integration-93/pybuilder_integration/properties.py`

 * *Files identical despite different names*

### Comparing `pybuilder-integration-92/pybuilder_integration/tasks.py` & `pybuilder-integration-93/pybuilder_integration/tasks.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,22 +44,25 @@
     if project.get_property(SHOULD_SKIP_LATEST, False):
         if project.get_property(ROLE) == test_dir:
             return False
     return True
 
 
 def _run_tests_in_directory(dist_directory, logger, project, reactor, latest=False):
+    logger.debug(f"Run tests in directory: {os.listdir(dist_directory)} ")
     _run_tavern_tests_in_dist_dir(dist_directory, latest, logger, project, reactor)
     _run_cypress_tests_in_dist_dir(dist_directory, latest, logger, project, reactor)
 
 
 def _run_cypress_tests_in_dist_dir(dist_directory, latest, logger, project, reactor):
     total_time = Timer.start()
     cypress_test_path = f"{dist_directory}/cypress"
     if os.path.exists(cypress_test_path):
+        logger.debug(f"Run cypress tests in directory: {cypress_test_path} ")
+        logger.debug(f"Run cypress tests in directory files: {os.listdir(cypress_test_path)} ")
         logger.info(f"Found cypress tests - starting run latest: {latest}")
         if latest:
             for test_dir in os.listdir(cypress_test_path):
                 directory_to_test = f"{cypress_test_path}/{test_dir}"
                 if os.path.isdir(directory_to_test) and _should_run_latest(test_dir, project):
                     logger.info(f"Running {directory_to_test}")
                     _run_cypress_tests_in_directory(work_dir=directory_to_test,
@@ -76,19 +79,22 @@
 
 
 def _run_tavern_tests_in_dist_dir(dist_directory, latest, logger, project, reactor):
     total_time = Timer.start()
     tavern_test_path = f"{dist_directory}/tavern"
     if os.path.exists(tavern_test_path):
         logger.info(f"Found tavern tests - starting run latest: {latest}")
+        logger.debug(f"Run tavern tests in directory: {tavern_test_path} ")
+        logger.debug(f"Run tavern tests in directory files: {os.listdir(tavern_test_path)} ")
         if latest:
             for tavern_dir in os.listdir(tavern_test_path):
-                if os.path.isdir(f"{tavern_test_path}/{tavern_dir}") and _should_run_latest(tavern_dir, project):
-                    logger.info(f"Running {tavern_dir}")
-                    _run_tavern_tests_in_dir(test_dir=f"{tavern_test_path}/{tavern_dir}",
+                tavern_test_direcotry = f"{tavern_test_path}/{tavern_dir}"
+                if os.path.isdir(tavern_test_direcotry) and _should_run_latest(tavern_dir, project):
+                    logger.info(f"Running {tavern_test_direcotry}")
+                    _run_tavern_tests_in_dir(test_dir=tavern_test_direcotry,
                                              logger=logger,
                                              project=project,
                                              reactor=reactor,
                                              role=os.path.basename(tavern_dir))
         else:
             _run_tavern_tests_in_dir(test_dir=f"{tavern_test_path}",
                                      logger=logger,
```

### Comparing `pybuilder-integration-92/pybuilder_integration/tool_utility.py` & `pybuilder-integration-93/pybuilder_integration/tool_utility.py`

 * *Files identical despite different names*

### Comparing `pybuilder-integration-92/pybuilder_integration.egg-info/PKG-INFO` & `pybuilder-integration-93/pybuilder_integration.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybuilder-integration
-Version: 92
+Version: 93
 Summary: A pybuilder plugin that runs integration tests (Tavern & Cypress) against a target.
 Home-page: https://github.com/rspitler/pybuilder-integration
 Author: 
 Author-email: 
 Maintainer: 
 Maintainer-email: 
 License: Apache 2.0
```

### Comparing `pybuilder-integration-92/pybuilder_integration.egg-info/SOURCES.txt` & `pybuilder-integration-93/pybuilder_integration.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pybuilder-integration-92/setup.py` & `pybuilder-integration-93/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         _install.run(self)
 
         self.post_install_script()
 
 if __name__ == '__main__':
     setup(
         name = 'pybuilder-integration',
-        version = '92',
+        version = '93',
         description = 'A pybuilder plugin that runs integration tests (Tavern & Cypress) against a target.',
         long_description = 'A pybuilder plugin that runs integration tests against a target.  This is intended to be a broader scope than unit-tests encompassing dependant functionality.',
         long_description_content_type = None,
         classifiers = [
             'Development Status :: 3 - Alpha',
             'Programming Language :: Python'
         ],
```

