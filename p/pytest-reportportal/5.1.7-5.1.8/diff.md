# Comparing `tmp/pytest-reportportal-5.1.7.tar.gz` & `tmp/pytest-reportportal-5.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-reportportal-5.1.7.tar", last modified: Fri Apr 21 13:10:27 2023, max compression
+gzip compressed data, was "pytest-reportportal-5.1.8.tar", last modified: Wed May 24 15:16:41 2023, max compression
```

## Comparing `pytest-reportportal-5.1.7.tar` & `pytest-reportportal-5.1.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:10:27.150581 pytest-reportportal-5.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-04-21 13:10:20.000000 pytest-reportportal-5.1.7/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-21 13:10:20.000000 pytest-reportportal-5.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-21 13:10:20.000000 pytest-reportportal-5.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10467 2023-04-21 13:10:27.150581 pytest-reportportal-5.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9742 2023-04-21 13:10:20.000000 pytest-reportportal-5.1.7/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-21 13:10:20.000000 pytest-reportportal-5.1.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:10:27.150581 pytest-reportportal-5.1.7/pytest_reportportal/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-21 13:10:20.000000 pytest-reportportal-5.1.7/pytest_reportportal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-04-21 13:10:20.000000 pytest-reportportal-5.1.7/pytest_reportportal/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-21 13:10:20.000000 pytest-reportportal-5.1.7/pytest_reportportal/config.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-21 13:10:20.000000 pytest-reportportal-5.1.7/pytest_reportportal/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    15597 2023-04-21 13:10:20.000000 pytest-reportportal-5.1.7/pytest_reportportal/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-21 13:10:20.000000 pytest-reportportal-5.1.7/pytest_reportportal/plugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-04-21 13:10:20.000000 pytest-reportportal-5.1.7/pytest_reportportal/rp_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    31887 2023-04-21 13:10:20.000000 pytest-reportportal-5.1.7/pytest_reportportal/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-21 13:10:20.000000 pytest-reportportal-5.1.7/pytest_reportportal/service.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:10:27.150581 pytest-reportportal-5.1.7/pytest_reportportal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10467 2023-04-21 13:10:27.000000 pytest-reportportal-5.1.7/pytest_reportportal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-21 13:10:27.000000 pytest-reportportal-5.1.7/pytest_reportportal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 13:10:27.000000 pytest-reportportal-5.1.7/pytest_reportportal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-21 13:10:27.000000 pytest-reportportal-5.1.7/pytest_reportportal.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-21 13:10:27.000000 pytest-reportportal-5.1.7/pytest_reportportal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-21 13:10:27.000000 pytest-reportportal-5.1.7/pytest_reportportal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-21 13:10:20.000000 pytest-reportportal-5.1.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-21 13:10:27.154582 pytest-reportportal-5.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-04-21 13:10:20.000000 pytest-reportportal-5.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:16:41.027979 pytest-reportportal-5.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-05-24 15:16:33.000000 pytest-reportportal-5.1.8/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-24 15:16:33.000000 pytest-reportportal-5.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-24 15:16:33.000000 pytest-reportportal-5.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10467 2023-05-24 15:16:41.027979 pytest-reportportal-5.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9742 2023-05-24 15:16:33.000000 pytest-reportportal-5.1.8/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-24 15:16:33.000000 pytest-reportportal-5.1.8/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:16:41.023979 pytest-reportportal-5.1.8/pytest_reportportal/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-24 15:16:33.000000 pytest-reportportal-5.1.8/pytest_reportportal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-05-24 15:16:33.000000 pytest-reportportal-5.1.8/pytest_reportportal/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-24 15:16:33.000000 pytest-reportportal-5.1.8/pytest_reportportal/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-24 15:16:33.000000 pytest-reportportal-5.1.8/pytest_reportportal/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15607 2023-05-24 15:16:33.000000 pytest-reportportal-5.1.8/pytest_reportportal/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-24 15:16:33.000000 pytest-reportportal-5.1.8/pytest_reportportal/plugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-05-24 15:16:33.000000 pytest-reportportal-5.1.8/pytest_reportportal/rp_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31887 2023-05-24 15:16:33.000000 pytest-reportportal-5.1.8/pytest_reportportal/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-24 15:16:33.000000 pytest-reportportal-5.1.8/pytest_reportportal/service.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:16:41.027979 pytest-reportportal-5.1.8/pytest_reportportal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10467 2023-05-24 15:16:41.000000 pytest-reportportal-5.1.8/pytest_reportportal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-24 15:16:41.000000 pytest-reportportal-5.1.8/pytest_reportportal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:16:41.000000 pytest-reportportal-5.1.8/pytest_reportportal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-24 15:16:41.000000 pytest-reportportal-5.1.8/pytest_reportportal.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-24 15:16:41.000000 pytest-reportportal-5.1.8/pytest_reportportal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-24 15:16:41.000000 pytest-reportportal-5.1.8/pytest_reportportal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-24 15:16:33.000000 pytest-reportportal-5.1.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-24 15:16:41.027979 pytest-reportportal-5.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-05-24 15:16:33.000000 pytest-reportportal-5.1.8/setup.py
```

### Comparing `pytest-reportportal-5.1.7/CONTRIBUTING.rst` & `pytest-reportportal-5.1.8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pytest-reportportal-5.1.7/LICENSE` & `pytest-reportportal-5.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-reportportal-5.1.7/PKG-INFO` & `pytest-reportportal-5.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-reportportal
-Version: 5.1.7
+Version: 5.1.8
 Summary: Agent for Reporting results of tests to the Report Portal
 Home-page: https://github.com/reportportal/agent-python-pytest
 Author: Report Portal Team
 Author-email: support@reportportal.io
 License: Apache 2.0
 Keywords: testing,reporting,reportportal,pytest,agent
 Classifier: Framework :: Pytest
```

### Comparing `pytest-reportportal-5.1.7/README.rst` & `pytest-reportportal-5.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-reportportal-5.1.7/pytest_reportportal/config.py` & `pytest-reportportal-5.1.8/pytest_reportportal/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,18 +55,18 @@
             pytest_config, 'rp_log_batch_payload_size')
         if batch_payload_size:
             self.rp_log_batch_payload_size = int(batch_payload_size)
         else:
             self.rp_log_batch_payload_size = MAX_LOG_BATCH_PAYLOAD_SIZE
         self.rp_log_level = get_actual_log_level(pytest_config, 'rp_log_level')
         self.rp_log_format = self.find_option(pytest_config, 'rp_log_format')
-        self.rp_mode = self.find_option(pytest_config, 'rp_mode')
-        self.rp_thread_logging = self.find_option(
+        self.rp_thread_logging = bool(strtobool(str(self.find_option(
             pytest_config, 'rp_thread_logging'
-        )
+        ) or False)))
+        self.rp_mode = self.find_option(pytest_config, 'rp_mode')
         self.rp_parent_item_id = self.find_option(pytest_config,
                                                   'rp_parent_item_id')
         self.rp_project = self.find_option(pytest_config,
                                            'rp_project')
         self.rp_rerun_of = self.find_option(pytest_config,
                                             'rp_rerun_of')
         self.rp_retries = int(self.find_option(pytest_config,
```

### Comparing `pytest-reportportal-5.1.7/pytest_reportportal/config.pyi` & `pytest-reportportal-5.1.8/pytest_reportportal/config.pyi`

 * *Files identical despite different names*

### Comparing `pytest-reportportal-5.1.7/pytest_reportportal/plugin.py` & `pytest-reportportal-5.1.8/pytest_reportportal/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     'rp_uuid: {}'
 
 FAILED_LAUNCH_WAIT = 'Failed to initialize reportportal-client service. ' \
                      + 'Waiting for Launch start timed out. ' \
                      + 'Reporting is disabled.'
 
 
-@pytest.mark.optionalhook
+@pytest.hookimpl(optionalhook=True)
 def pytest_configure_node(node):
     """Configure xdist node controller.
 
     :param node: Object of the xdist WorkerController class
     """
     # noinspection PyProtectedMember
     if not node.config._rp_enabled:
```

### Comparing `pytest-reportportal-5.1.7/pytest_reportportal/plugin.pyi` & `pytest-reportportal-5.1.8/pytest_reportportal/plugin.pyi`

 * *Files identical despite different names*

### Comparing `pytest-reportportal-5.1.7/pytest_reportportal/rp_logging.py` & `pytest-reportportal-5.1.8/pytest_reportportal/rp_logging.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,29 @@
 """RPLogger class for low-level logging in tests."""
 
 import logging
 import threading
 from contextlib import contextmanager
 from functools import wraps
 
-from reportportal_client.client import RPClient
-
 from reportportal_client._local import current, set_current
 from reportportal_client import RPLogger
+from reportportal_client.core.worker import APIWorker
+
+
+def is_api_worker(target):
+    """Check if target is an RP worker thread."""
+    if target:
+        method_name = getattr(target, '__name__', None)
+        method_self = getattr(target, '__self__', None)
+        if method_name == '_monitor' and method_self:
+            clazz = getattr(method_self, '__class__', None)
+            if clazz is APIWorker:
+                return True
+    return False
 
 
 @contextmanager
 def patching_thread_class(config):
     """
     Add patch for Thread class.
 
@@ -26,15 +37,16 @@
         original_run = threading.Thread.run
         try:
             def wrap_start(original_func):
                 @wraps(original_func)
                 def _start(self, *args, **kwargs):
                     """Save the invoking thread's client if there is one."""
                     # Prevent an endless loop of workers being spawned
-                    if "_monitor" not in self.name:
+                    target = getattr(self, '_target', None)
+                    if not is_api_worker(self) and not is_api_worker(target):
                         current_client = current()
                         self.parent_rp_client = current_client
                     return original_func(self, *args, **kwargs)
 
                 return _start
 
             def wrap_run(original_func):
@@ -44,28 +56,15 @@
                     client = None
                     if (
                         hasattr(self, "parent_rp_client")
                         and self.parent_rp_client
                         and not current()
                     ):
                         parent = self.parent_rp_client
-                        client = RPClient(
-                            endpoint=parent.endpoint,
-                            project=parent.project,
-                            token=parent.token,
-                            log_batch_size=parent.log_batch_size,
-                            is_skipped_an_issue=parent.is_skipped_an_issue,
-                            verify_ssl=parent.verify_ssl,
-                            retries=config.rp_retries,
-                            launch_id=parent.launch_id
-                        )
-                        if parent.current_item():
-                            client._item_stack.append(
-                                parent.current_item()
-                            )
+                        client = parent.clone()
                         client.start()
                     try:
                         return original_func(self, *args, **kwargs)
                     finally:
                         if client:
                             # Stop the client and remove any references
                             client.terminate()
```

### Comparing `pytest-reportportal-5.1.7/pytest_reportportal/service.py` & `pytest-reportportal-5.1.8/pytest_reportportal/service.py`

 * *Files identical despite different names*

### Comparing `pytest-reportportal-5.1.7/pytest_reportportal/service.pyi` & `pytest-reportportal-5.1.8/pytest_reportportal/service.pyi`

 * *Files identical despite different names*

### Comparing `pytest-reportportal-5.1.7/pytest_reportportal.egg-info/PKG-INFO` & `pytest-reportportal-5.1.8/pytest_reportportal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-reportportal
-Version: 5.1.7
+Version: 5.1.8
 Summary: Agent for Reporting results of tests to the Report Portal
 Home-page: https://github.com/reportportal/agent-python-pytest
 Author: Report Portal Team
 Author-email: support@reportportal.io
 License: Apache 2.0
 Keywords: testing,reporting,reportportal,pytest,agent
 Classifier: Framework :: Pytest
```

### Comparing `pytest-reportportal-5.1.7/pytest_reportportal.egg-info/SOURCES.txt` & `pytest-reportportal-5.1.8/pytest_reportportal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-reportportal-5.1.7/setup.py` & `pytest-reportportal-5.1.8/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Config for setup package pytest agent."""
 
 import os
 
 from setuptools import setup
 
 
-__version__ = '5.1.7'
+__version__ = '5.1.8'
 
 
 def read_file(fname):
     """Read the given file.
 
     :param fname: Filename to be read
     :return:      File content
```

