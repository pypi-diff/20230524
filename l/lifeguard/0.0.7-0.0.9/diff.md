# Comparing `tmp/lifeguard-0.0.7.tar.gz` & `tmp/lifeguard-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifeguard-0.0.7.tar", last modified: Thu Jan  7 18:48:02 2021, max compression
+gzip compressed data, was "lifeguard-0.0.9.tar", last modified: Fri Jan 15 19:17:59 2021, max compression
```

## Comparing `lifeguard-0.0.7.tar` & `lifeguard-0.0.9.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-07 18:48:02.235910 lifeguard-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (116)      363 2021-01-07 18:48:02.235910 lifeguard-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      404 2021-01-07 18:47:48.000000 lifeguard-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-07 18:48:02.231910 lifeguard-0.0.7/bin/
--rwxr-xr-x   0 runner    (1001) docker     (116)      106 2021-01-07 18:47:48.000000 lifeguard-0.0.7/bin/lifeguard
--rwxr-xr-x   0 runner    (1001) docker     (116)      944 2021-01-07 18:47:48.000000 lifeguard-0.0.7/bin/lifeguard-scheduler
--rwxr-xr-x   0 runner    (1001) docker     (116)      217 2021-01-07 18:47:48.000000 lifeguard-0.0.7/bin/lifeguard-server
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-07 18:48:02.235910 lifeguard-0.0.7/lifeguard/
--rw-r--r--   0 runner    (1001) docker     (116)     1243 2021-01-07 18:47:48.000000 lifeguard-0.0.7/lifeguard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-07 18:48:02.235910 lifeguard-0.0.7/lifeguard/actions/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-07 18:47:48.000000 lifeguard-0.0.7/lifeguard/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      457 2021-01-07 18:47:48.000000 lifeguard-0.0.7/lifeguard/actions/database.py
--rw-r--r--   0 runner    (1001) docker     (116)     2994 2021-01-07 18:47:48.000000 lifeguard-0.0.7/lifeguard/actions/notifications.py
--rw-r--r--   0 runner    (1001) docker     (116)      778 2021-01-07 18:47:48.000000 lifeguard-0.0.7/lifeguard/http_client.py
--rw-r--r--   0 runner    (1001) docker     (116)     1662 2021-01-07 18:47:48.000000 lifeguard-0.0.7/lifeguard/logger.py
--rw-r--r--   0 runner    (1001) docker     (116)     3584 2021-01-07 18:47:48.000000 lifeguard-0.0.7/lifeguard/notifications.py
--rw-r--r--   0 runner    (1001) docker     (116)     1600 2021-01-07 18:47:48.000000 lifeguard-0.0.7/lifeguard/repositories.py
--rw-r--r--   0 runner    (1001) docker     (116)     1279 2021-01-07 18:47:48.000000 lifeguard-0.0.7/lifeguard/server.py
--rw-r--r--   0 runner    (1001) docker     (116)     1596 2021-01-07 18:47:48.000000 lifeguard-0.0.7/lifeguard/settings.py
--rw-r--r--   0 runner    (1001) docker     (116)     3927 2021-01-07 18:47:48.000000 lifeguard-0.0.7/lifeguard/validations.py
--rw-r--r--   0 runner    (1001) docker     (116)      126 2021-01-07 18:47:48.000000 lifeguard-0.0.7/lifeguard/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-07 18:48:02.235910 lifeguard-0.0.7/lifeguard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      363 2021-01-07 18:48:01.000000 lifeguard-0.0.7/lifeguard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      950 2021-01-07 18:48:02.000000 lifeguard-0.0.7/lifeguard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-07 18:48:01.000000 lifeguard-0.0.7/lifeguard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       33 2021-01-07 18:48:01.000000 lifeguard-0.0.7/lifeguard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       16 2021-01-07 18:48:01.000000 lifeguard-0.0.7/lifeguard.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      125 2021-01-07 18:48:02.235910 lifeguard-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      646 2021-01-07 18:47:48.000000 lifeguard-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-07 18:48:02.235910 lifeguard-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-07 18:47:48.000000 lifeguard-0.0.7/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-07 18:48:02.235910 lifeguard-0.0.7/tests/actions/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-07 18:47:48.000000 lifeguard-0.0.7/tests/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      661 2021-01-07 18:47:48.000000 lifeguard-0.0.7/tests/actions/test_database.py
--rw-r--r--   0 runner    (1001) docker     (116)     6465 2021-01-07 18:47:48.000000 lifeguard-0.0.7/tests/actions/test_notification.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-07 18:48:02.235910 lifeguard-0.0.7/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-07 18:47:48.000000 lifeguard-0.0.7/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)       41 2021-01-07 18:47:48.000000 lifeguard-0.0.7/tests/fixtures/fixtures_repositories.py
--rw-r--r--   0 runner    (1001) docker     (116)      138 2021-01-07 18:47:48.000000 lifeguard-0.0.7/tests/fixtures/mock_lifeguard_settings.py
--rw-r--r--   0 runner    (1001) docker     (116)     1107 2021-01-07 18:47:48.000000 lifeguard-0.0.7/tests/test_http_client.py
--rw-r--r--   0 runner    (1001) docker     (116)     1143 2021-01-07 18:47:48.000000 lifeguard-0.0.7/tests/test_lifeguard_core.py
--rw-r--r--   0 runner    (1001) docker     (116)     1307 2021-01-07 18:47:48.000000 lifeguard-0.0.7/tests/test_notifications.py
--rw-r--r--   0 runner    (1001) docker     (116)     3873 2021-01-07 18:47:48.000000 lifeguard-0.0.7/tests/test_repositories.py
--rw-r--r--   0 runner    (1001) docker     (116)     2283 2021-01-07 18:47:48.000000 lifeguard-0.0.7/tests/test_server.py
--rw-r--r--   0 runner    (1001) docker     (116)      947 2021-01-07 18:47:48.000000 lifeguard-0.0.7/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (116)     2770 2021-01-07 18:47:48.000000 lifeguard-0.0.7/tests/test_validations.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 19:17:59.591395 lifeguard-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (116)      363 2021-01-15 19:17:59.591395 lifeguard-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      404 2021-01-15 19:17:49.000000 lifeguard-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 19:17:59.587395 lifeguard-0.0.9/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (116)     1190 2021-01-15 19:17:49.000000 lifeguard-0.0.9/bin/lifeguard
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 19:17:59.591395 lifeguard-0.0.9/lifeguard/
+-rw-r--r--   0 runner    (1001) docker     (116)     1312 2021-01-15 19:17:49.000000 lifeguard-0.0.9/lifeguard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 19:17:59.591395 lifeguard-0.0.9/lifeguard/actions/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-15 19:17:49.000000 lifeguard-0.0.9/lifeguard/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      457 2021-01-15 19:17:49.000000 lifeguard-0.0.9/lifeguard/actions/database.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2994 2021-01-15 19:17:49.000000 lifeguard-0.0.9/lifeguard/actions/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1466 2021-01-15 19:17:49.000000 lifeguard-0.0.9/lifeguard/controllers.py
+-rw-r--r--   0 runner    (1001) docker     (116)      778 2021-01-15 19:17:49.000000 lifeguard-0.0.9/lifeguard/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1662 2021-01-15 19:17:49.000000 lifeguard-0.0.9/lifeguard/logger.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3584 2021-01-15 19:17:49.000000 lifeguard-0.0.9/lifeguard/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1600 2021-01-15 19:17:49.000000 lifeguard-0.0.9/lifeguard/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (116)      854 2021-01-15 19:17:49.000000 lifeguard-0.0.9/lifeguard/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1377 2021-01-15 19:17:49.000000 lifeguard-0.0.9/lifeguard/server.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1596 2021-01-15 19:17:49.000000 lifeguard-0.0.9/lifeguard/settings.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3927 2021-01-15 19:17:49.000000 lifeguard-0.0.9/lifeguard/validations.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 19:17:59.591395 lifeguard-0.0.9/lifeguard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)      363 2021-01-15 19:17:59.000000 lifeguard-0.0.9/lifeguard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      985 2021-01-15 19:17:59.000000 lifeguard-0.0.9/lifeguard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-15 19:17:59.000000 lifeguard-0.0.9/lifeguard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       33 2021-01-15 19:17:59.000000 lifeguard-0.0.9/lifeguard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       16 2021-01-15 19:17:59.000000 lifeguard-0.0.9/lifeguard.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      125 2021-01-15 19:17:59.595395 lifeguard-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)      565 2021-01-15 19:17:49.000000 lifeguard-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 19:17:59.591395 lifeguard-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-15 19:17:49.000000 lifeguard-0.0.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 19:17:59.591395 lifeguard-0.0.9/tests/actions/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-15 19:17:49.000000 lifeguard-0.0.9/tests/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      661 2021-01-15 19:17:49.000000 lifeguard-0.0.9/tests/actions/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6465 2021-01-15 19:17:49.000000 lifeguard-0.0.9/tests/actions/test_notification.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 19:17:59.591395 lifeguard-0.0.9/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-15 19:17:49.000000 lifeguard-0.0.9/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)       41 2021-01-15 19:17:49.000000 lifeguard-0.0.9/tests/fixtures/fixtures_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (116)      138 2021-01-15 19:17:49.000000 lifeguard-0.0.9/tests/fixtures/mock_lifeguard_settings.py
+-rw-r--r--   0 runner    (1001) docker     (116)      764 2021-01-15 19:17:49.000000 lifeguard-0.0.9/tests/test_controllers.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1107 2021-01-15 19:17:49.000000 lifeguard-0.0.9/tests/test_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1050 2021-01-15 19:17:49.000000 lifeguard-0.0.9/tests/test_lifeguard_core.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1307 2021-01-15 19:17:49.000000 lifeguard-0.0.9/tests/test_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3873 2021-01-15 19:17:49.000000 lifeguard-0.0.9/tests/test_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (116)      526 2021-01-15 19:17:49.000000 lifeguard-0.0.9/tests/test_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2283 2021-01-15 19:17:49.000000 lifeguard-0.0.9/tests/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (116)      947 2021-01-15 19:17:49.000000 lifeguard-0.0.9/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2770 2021-01-15 19:17:49.000000 lifeguard-0.0.9/tests/test_validations.py
```

### Comparing `lifeguard-0.0.7/bin/lifeguard-scheduler` & `lifeguard-0.0.9/lifeguard/scheduler.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,30 @@
-#!/usr/bin/env python3
 import time
-import sys
-import schedule
 import traceback
+import schedule
 
-sys.path.append(".")
-
-from lifeguard import setup
 from lifeguard.validations import VALIDATIONS
 from lifeguard.logger import lifeguard_logger as logger
 
 
-def start_scheduler():
-
+def configure_validations():
     for validation in VALIDATIONS:
         content = VALIDATIONS[validation]
         if "every" in content["schedule"]:
             if "minutes" in content["schedule"]["every"]:
                 schedule.every(content["schedule"]["every"]["minutes"]).minutes.do(
                     content["ref"]
                 )
 
+
+def start_scheduler():
+    configure_validations()
     while True:
         time.sleep(1)
         try:
             schedule.run_pending()
         except Exception as exception:
             logger.error(
                 "error on execute scheduler %s",
                 str(exception),
                 extra={"traceback": traceback.format_exc()},
             )
-
-
-if __name__ == "__main__":
-    setup()
-    start_scheduler()
```

### Comparing `lifeguard-0.0.7/lifeguard/__init__.py` & `lifeguard-0.0.9/lifeguard/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,18 +3,17 @@
 """
 import os
 import sys
 
 from lifeguard.logger import lifeguard_logger as logger
 from lifeguard.repositories import declare_implementation
 from lifeguard.settings import LIFEGUARD_DIRECTORY
+from lifeguard.controllers import load_custom_controllers
 from lifeguard.validations import load_validations
 
-VERSION = "0.0.7"
-
 NORMAL = "NORMAL"
 WARNING = "WARNING"
 PROBLEM = "PROBLEM"
 
 ACTION_STATUSES = [NORMAL, WARNING, PROBLEM]
 LIFEGUARD_CONTEXT = {}
 
@@ -54,10 +53,11 @@
 
     # init plugins
     lifeguard_settings = recover_settings()
 
     for plugin in lifeguard_settings.PLUGINS:
         plugin.init(lifeguard_context)
 
+    load_custom_controllers()
     load_validations()
 
     lifeguard_settings.setup(lifeguard_context)
```

### Comparing `lifeguard-0.0.7/lifeguard/actions/notifications.py` & `lifeguard-0.0.9/lifeguard/actions/notifications.py`

 * *Files identical despite different names*

### Comparing `lifeguard-0.0.7/lifeguard/http_client.py` & `lifeguard-0.0.9/lifeguard/http_client.py`

 * *Files identical despite different names*

### Comparing `lifeguard-0.0.7/lifeguard/logger.py` & `lifeguard-0.0.9/lifeguard/logger.py`

 * *Files identical despite different names*

### Comparing `lifeguard-0.0.7/lifeguard/notifications.py` & `lifeguard-0.0.9/lifeguard/notifications.py`

 * *Files identical despite different names*

### Comparing `lifeguard-0.0.7/lifeguard/repositories.py` & `lifeguard-0.0.9/lifeguard/repositories.py`

 * *Files identical despite different names*

### Comparing `lifeguard-0.0.7/lifeguard/server.py` & `lifeguard-0.0.9/lifeguard/server.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-from datetime import datetime
 import json
 import traceback
+from datetime import datetime
 
 from flask import Flask, make_response
 
+from lifeguard.controllers import custom_controllers
+from lifeguard.logger import lifeguard_logger as logger
 from lifeguard.repositories import ValidationRepository
 from lifeguard.validations import VALIDATIONS, ValidationResponseEncoder
-from lifeguard.logger import lifeguard_logger as logger
 
 APP = Flask(__name__)
 
 
 def make_json_response(content):
     response = make_response(content)
     response.headers["Content-Type"] = "application/json"
@@ -33,7 +34,10 @@
     except Exception:
         logger.error(
             "error on execute validation %s",
             validation,
             extra={"traceback": traceback.format_exc()},
         )
         return json.dumps({"error": traceback.format_exc()})
+
+
+APP.register_blueprint(custom_controllers)
```

### Comparing `lifeguard-0.0.7/lifeguard/settings.py` & `lifeguard-0.0.9/lifeguard/settings.py`

 * *Files identical despite different names*

### Comparing `lifeguard-0.0.7/lifeguard/validations.py` & `lifeguard-0.0.9/lifeguard/validations.py`

 * *Files identical despite different names*

### Comparing `lifeguard-0.0.7/lifeguard.egg-info/SOURCES.txt` & `lifeguard-0.0.9/lifeguard.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 README.md
 setup.cfg
 setup.py
 bin/lifeguard
-bin/lifeguard-scheduler
-bin/lifeguard-server
 lifeguard/__init__.py
+lifeguard/controllers.py
 lifeguard/http_client.py
 lifeguard/logger.py
 lifeguard/notifications.py
 lifeguard/repositories.py
+lifeguard/scheduler.py
 lifeguard/server.py
 lifeguard/settings.py
 lifeguard/validations.py
-lifeguard/wsgi.py
 lifeguard.egg-info/PKG-INFO
 lifeguard.egg-info/SOURCES.txt
 lifeguard.egg-info/dependency_links.txt
 lifeguard.egg-info/requires.txt
 lifeguard.egg-info/top_level.txt
 lifeguard/actions/__init__.py
 lifeguard/actions/database.py
 lifeguard/actions/notifications.py
 tests/__init__.py
+tests/test_controllers.py
 tests/test_http_client.py
 tests/test_lifeguard_core.py
 tests/test_notifications.py
 tests/test_repositories.py
+tests/test_scheduler.py
 tests/test_server.py
 tests/test_settings.py
 tests/test_validations.py
 tests/actions/__init__.py
 tests/actions/test_database.py
 tests/actions/test_notification.py
 tests/fixtures/__init__.py
```

### Comparing `lifeguard-0.0.7/tests/actions/test_database.py` & `lifeguard-0.0.9/tests/actions/test_database.py`

 * *Files identical despite different names*

### Comparing `lifeguard-0.0.7/tests/actions/test_notification.py` & `lifeguard-0.0.9/tests/actions/test_notification.py`

 * *Files identical despite different names*

### Comparing `lifeguard-0.0.7/tests/test_http_client.py` & `lifeguard-0.0.9/tests/test_http_client.py`

 * *Files identical despite different names*

### Comparing `lifeguard-0.0.7/tests/test_lifeguard_core.py` & `lifeguard-0.0.9/tests/test_lifeguard_core.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,25 +4,21 @@
 
 from lifeguard import (
     change_status,
     setup,
     NORMAL,
     WARNING,
     PROBLEM,
-    VERSION,
     ACTION_STATUSES,
 )
 
 from tests.fixtures import mock_lifeguard_settings
 
 
 class TestLifeguardCore(unittest.TestCase):
-    def test_current_version(self):
-        self.assertEqual(VERSION, "0.0.6")
-
     def test_statuses(self):
         self.assertEqual(NORMAL, "NORMAL")
         self.assertEqual(WARNING, "WARNING")
         self.assertEqual(PROBLEM, "PROBLEM")
         self.assertEqual(ACTION_STATUSES, [NORMAL, WARNING, PROBLEM])
 
     def test_change_status(self):
```

### Comparing `lifeguard-0.0.7/tests/test_notifications.py` & `lifeguard-0.0.9/tests/test_notifications.py`

 * *Files identical despite different names*

### Comparing `lifeguard-0.0.7/tests/test_repositories.py` & `lifeguard-0.0.9/tests/test_repositories.py`

 * *Files identical despite different names*

### Comparing `lifeguard-0.0.7/tests/test_server.py` & `lifeguard-0.0.9/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `lifeguard-0.0.7/tests/test_settings.py` & `lifeguard-0.0.9/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `lifeguard-0.0.7/tests/test_validations.py` & `lifeguard-0.0.9/tests/test_validations.py`

 * *Files identical despite different names*

