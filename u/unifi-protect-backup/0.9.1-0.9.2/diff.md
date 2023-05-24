# Comparing `tmp/unifi_protect_backup-0.9.1.tar.gz` & `tmp/unifi_protect_backup-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unifi_protect_backup-0.9.1.tar", max compression
+gzip compressed data, was "unifi_protect_backup-0.9.2.tar", max compression
```

## Comparing `unifi_protect_backup-0.9.1.tar` & `unifi_protect_backup-0.9.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1074 2023-04-29 08:52:44.952642 unifi_protect_backup-0.9.1/LICENSE
--rw-r--r--   0        0        0    17222 2023-04-29 08:52:44.952642 unifi_protect_backup-0.9.1/README.md
--rw-r--r--   0        0        0     2110 2023-04-29 08:52:44.952642 unifi_protect_backup-0.9.1/pyproject.toml
--rw-r--r--   0        0        0       50 2023-04-29 08:52:44.952642 unifi_protect_backup-0.9.1/tests/__init__.py
--rw-r--r--   0        0        0     1031 2023-04-29 08:52:44.952642 unifi_protect_backup-0.9.1/tests/test_unifi_protect_backup.py
--rw-r--r--   0        0        0      359 2023-04-29 08:52:44.952642 unifi_protect_backup-0.9.1/unifi_protect_backup/__init__.py
--rw-r--r--   0        0        0     6416 2023-04-29 08:52:44.952642 unifi_protect_backup-0.9.1/unifi_protect_backup/cli.py
--rw-r--r--   0        0        0     8972 2023-04-29 08:52:44.952642 unifi_protect_backup-0.9.1/unifi_protect_backup/downloader.py
--rw-r--r--   0        0        0     5277 2023-04-29 08:52:44.956642 unifi_protect_backup-0.9.1/unifi_protect_backup/event_listener.py
--rw-r--r--   0        0        0     6505 2023-04-29 08:52:44.956642 unifi_protect_backup-0.9.1/unifi_protect_backup/missing_event_checker.py
--rw-r--r--   0        0        0      540 2023-04-29 08:52:44.956642 unifi_protect_backup-0.9.1/unifi_protect_backup/notifications.py
--rw-r--r--   0        0        0     3682 2023-04-29 08:52:44.956642 unifi_protect_backup-0.9.1/unifi_protect_backup/purge.py
--rw-r--r--   0        0        0    12499 2023-04-29 08:52:44.956642 unifi_protect_backup-0.9.1/unifi_protect_backup/unifi_protect_backup_core.py
--rw-r--r--   0        0        0     6365 2023-04-29 08:52:44.956642 unifi_protect_backup-0.9.1/unifi_protect_backup/uploader.py
--rw-r--r--   0        0        0    16583 2023-04-29 08:52:44.956642 unifi_protect_backup-0.9.1/unifi_protect_backup/utils.py
--rw-r--r--   0        0        0    18356 1970-01-01 00:00:00.000000 unifi_protect_backup-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-23 23:45:52.955222 unifi_protect_backup-0.9.2/LICENSE
+-rw-r--r--   0        0        0    17222 2023-05-23 23:45:52.955222 unifi_protect_backup-0.9.2/README.md
+-rw-r--r--   0        0        0     2110 2023-05-23 23:45:52.959222 unifi_protect_backup-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0       50 2023-05-23 23:45:52.959222 unifi_protect_backup-0.9.2/tests/__init__.py
+-rw-r--r--   0        0        0     1031 2023-05-23 23:45:52.959222 unifi_protect_backup-0.9.2/tests/test_unifi_protect_backup.py
+-rw-r--r--   0        0        0      359 2023-05-23 23:45:52.959222 unifi_protect_backup-0.9.2/unifi_protect_backup/__init__.py
+-rw-r--r--   0        0        0     6416 2023-05-23 23:45:52.959222 unifi_protect_backup-0.9.2/unifi_protect_backup/cli.py
+-rw-r--r--   0        0        0     8972 2023-05-23 23:45:52.959222 unifi_protect_backup-0.9.2/unifi_protect_backup/downloader.py
+-rw-r--r--   0        0        0     5277 2023-05-23 23:45:52.959222 unifi_protect_backup-0.9.2/unifi_protect_backup/event_listener.py
+-rw-r--r--   0        0        0     6589 2023-05-23 23:45:52.959222 unifi_protect_backup-0.9.2/unifi_protect_backup/missing_event_checker.py
+-rw-r--r--   0        0        0      540 2023-05-23 23:45:52.959222 unifi_protect_backup-0.9.2/unifi_protect_backup/notifications.py
+-rw-r--r--   0        0        0     3682 2023-05-23 23:45:52.959222 unifi_protect_backup-0.9.2/unifi_protect_backup/purge.py
+-rw-r--r--   0        0        0    12499 2023-05-23 23:45:52.959222 unifi_protect_backup-0.9.2/unifi_protect_backup/unifi_protect_backup_core.py
+-rw-r--r--   0        0        0     6365 2023-05-23 23:45:52.959222 unifi_protect_backup-0.9.2/unifi_protect_backup/uploader.py
+-rw-r--r--   0        0        0    16583 2023-05-23 23:45:52.959222 unifi_protect_backup-0.9.2/unifi_protect_backup/utils.py
+-rw-r--r--   0        0        0    18258 1970-01-01 00:00:00.000000 unifi_protect_backup-0.9.2/PKG-INFO
```

### Comparing `unifi_protect_backup-0.9.1/LICENSE` & `unifi_protect_backup-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `unifi_protect_backup-0.9.1/README.md` & `unifi_protect_backup-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `unifi_protect_backup-0.9.1/pyproject.toml` & `unifi_protect_backup-0.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "unifi_protect_backup"
-version = "0.9.1"
+version = "0.9.2"
 homepage = "https://github.com/ep1cman/unifi-protect-backup"
 description = "Python tool to backup unifi event clips in realtime."
 authors = ["sebastian.goscik <sebastian@goscik.com>"]
 readme = "README.md"
 license =  "MIT"
 classifiers=[
     'Development Status :: 5 - Production/Stable',
```

### Comparing `unifi_protect_backup-0.9.1/tests/test_unifi_protect_backup.py` & `unifi_protect_backup-0.9.2/tests/test_unifi_protect_backup.py`

 * *Files identical despite different names*

### Comparing `unifi_protect_backup-0.9.1/unifi_protect_backup/cli.py` & `unifi_protect_backup-0.9.2/unifi_protect_backup/cli.py`

 * *Files identical despite different names*

### Comparing `unifi_protect_backup-0.9.1/unifi_protect_backup/downloader.py` & `unifi_protect_backup-0.9.2/unifi_protect_backup/downloader.py`

 * *Files identical despite different names*

### Comparing `unifi_protect_backup-0.9.1/unifi_protect_backup/event_listener.py` & `unifi_protect_backup-0.9.2/unifi_protect_backup/event_listener.py`

 * *Files identical despite different names*

### Comparing `unifi_protect_backup-0.9.1/unifi_protect_backup/missing_event_checker.py` & `unifi_protect_backup-0.9.2/unifi_protect_backup/missing_event_checker.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,16 @@
 
         missing_event_ids = set(unifi_events.keys()) - (db_event_ids | downloading_event_ids | uploading_event_ids)
 
         def wanted_event_type(event_id):
             event = unifi_events[event_id]
             if event.start is None or event.end is None:
                 return False  # This event is still on-going
+            if event.camera_id in self.ignore_cameras:
+                return False
             if event.type is EventType.MOTION and "motion" not in self.detection_types:
                 return False
             if event.type is EventType.RING and "ring" not in self.detection_types:
                 return False
             elif event.type is EventType.SMART_DETECT:
                 for event_smart_detection_type in event.smart_detect_types:
                     if event_smart_detection_type not in self.detection_types:
```

### Comparing `unifi_protect_backup-0.9.1/unifi_protect_backup/notifications.py` & `unifi_protect_backup-0.9.2/unifi_protect_backup/notifications.py`

 * *Files identical despite different names*

### Comparing `unifi_protect_backup-0.9.1/unifi_protect_backup/purge.py` & `unifi_protect_backup-0.9.2/unifi_protect_backup/purge.py`

 * *Files identical despite different names*

### Comparing `unifi_protect_backup-0.9.1/unifi_protect_backup/unifi_protect_backup_core.py` & `unifi_protect_backup-0.9.2/unifi_protect_backup/unifi_protect_backup_core.py`

 * *Files identical despite different names*

### Comparing `unifi_protect_backup-0.9.1/unifi_protect_backup/uploader.py` & `unifi_protect_backup-0.9.2/unifi_protect_backup/uploader.py`

 * *Files identical despite different names*

### Comparing `unifi_protect_backup-0.9.1/unifi_protect_backup/utils.py` & `unifi_protect_backup-0.9.2/unifi_protect_backup/utils.py`

 * *Files identical despite different names*

### Comparing `unifi_protect_backup-0.9.1/PKG-INFO` & `unifi_protect_backup-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 Metadata-Version: 2.1
 Name: unifi-protect-backup
-Version: 0.9.1
+Version: 0.9.2
 Summary: Python tool to backup unifi event clips in realtime.
 Home-page: https://github.com/ep1cman/unifi-protect-backup
 License: MIT
 Author: sebastian.goscik
 Author-email: sebastian@goscik.com
 Requires-Python: >=3.9.0,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: aiorun (>=2022.11.1,<2023.0.0)
 Requires-Dist: aiosqlite (>=0.17.0,<0.18.0)
 Requires-Dist: apprise (>=1.3.0,<2.0.0)
 Requires-Dist: click (==8.0.1)
 Requires-Dist: expiring-dict (>=1.1.0,<2.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: pyunifiprotect (>=4.0.11,<5.0.0)
```

