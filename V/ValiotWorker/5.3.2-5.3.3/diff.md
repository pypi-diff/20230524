# Comparing `tmp/ValiotWorker-5.3.2.tar.gz` & `tmp/ValiotWorker-5.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ValiotWorker-5.3.2.tar", last modified: Fri Apr 21 16:57:50 2023, max compression
+gzip compressed data, was "ValiotWorker-5.3.3.tar", last modified: Wed May 24 15:22:20 2023, max compression
```

## Comparing `ValiotWorker-5.3.2.tar` & `ValiotWorker-5.3.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-04-21 16:57:50.409291 ValiotWorker-5.3.2/
--rw-r--r--   0 baruc      (501) staff       (20)     1074 2021-04-26 22:17:35.000000 ValiotWorker-5.3.2/LICENCE
--rw-r--r--   0 baruc      (501) staff       (20)       37 2023-02-24 03:38:26.000000 ValiotWorker-5.3.2/MANIFEST.in
--rw-r--r--   0 baruc      (501) staff       (20)     2158 2023-04-21 16:57:50.409042 ValiotWorker-5.3.2/PKG-INFO
--rw-r--r--   0 baruc      (501) staff       (20)     1811 2021-04-26 22:17:35.000000 ValiotWorker-5.3.2/README.md
-drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-04-21 16:57:50.402067 ValiotWorker-5.3.2/ValiotWorker/
--rw-r--r--   0 baruc      (501) staff       (20)     3486 2023-04-19 23:58:36.000000 ValiotWorker-5.3.2/ValiotWorker/Logging.py
--rw-r--r--   0 baruc      (501) staff       (20)    13430 2021-12-23 22:44:57.000000 ValiotWorker-5.3.2/ValiotWorker/Notifications.py
--rw-r--r--   0 baruc      (501) staff       (20)      294 2023-03-27 19:36:21.000000 ValiotWorker-5.3.2/ValiotWorker/__init__.py
--rw-r--r--   0 baruc      (501) staff       (20)     3450 2023-04-21 16:31:49.000000 ValiotWorker-5.3.2/ValiotWorker/__main__.py
--rw-r--r--   0 baruc      (501) staff       (20)       22 2023-04-21 16:56:56.000000 ValiotWorker-5.3.2/ValiotWorker/__version__.py
--rw-r--r--   0 baruc      (501) staff       (20)      276 2023-02-21 21:58:52.000000 ValiotWorker-5.3.2/ValiotWorker/croniterHelpers.py
--rw-r--r--   0 baruc      (501) staff       (20)      218 2023-02-21 21:58:52.000000 ValiotWorker-5.3.2/ValiotWorker/dateHelpers.py
-drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-04-21 16:57:50.405773 ValiotWorker-5.3.2/ValiotWorker/healthCheckProbe/
--rw-r--r--   0 baruc      (501) staff       (20)       41 2023-02-24 03:33:56.000000 ValiotWorker-5.3.2/ValiotWorker/healthCheckProbe/__init__.py
--rw-r--r--   0 baruc      (501) staff       (20)      963 2023-03-07 23:36:56.000000 ValiotWorker-5.3.2/ValiotWorker/healthCheckProbe/__main__.py
-drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-04-21 16:57:50.406159 ValiotWorker-5.3.2/ValiotWorker/healthCheckProbe/modules/
--rw-r--r--   0 baruc      (501) staff       (20)     1593 2023-02-24 03:33:56.000000 ValiotWorker-5.3.2/ValiotWorker/healthCheckProbe/modules/http_server.py
--rw-r--r--   0 baruc      (501) staff       (20)     7003 2023-03-07 22:03:01.000000 ValiotWorker-5.3.2/ValiotWorker/mutations.py
--rw-r--r--   0 baruc      (501) staff       (20)     4394 2023-03-07 23:36:56.000000 ValiotWorker-5.3.2/ValiotWorker/queries.py
--rw-r--r--   0 baruc      (501) staff       (20)     5885 2023-04-21 16:56:56.000000 ValiotWorker-5.3.2/ValiotWorker/redis.py
--rw-r--r--   0 baruc      (501) staff       (20)     1244 2023-03-27 19:36:21.000000 ValiotWorker-5.3.2/ValiotWorker/subscriptions.py
--rw-r--r--   0 baruc      (501) staff       (20)      182 2021-12-23 22:44:57.000000 ValiotWorker-5.3.2/ValiotWorker/uploaders.py
--rw-r--r--   0 baruc      (501) staff       (20)    69745 2023-04-21 16:51:33.000000 ValiotWorker-5.3.2/ValiotWorker/worker.py
-drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-04-21 16:57:50.405136 ValiotWorker-5.3.2/ValiotWorker.egg-info/
--rw-r--r--   0 baruc      (501) staff       (20)     2158 2023-04-21 16:57:50.000000 ValiotWorker-5.3.2/ValiotWorker.egg-info/PKG-INFO
--rw-r--r--   0 baruc      (501) staff       (20)      791 2023-04-21 16:57:50.000000 ValiotWorker-5.3.2/ValiotWorker.egg-info/SOURCES.txt
--rw-r--r--   0 baruc      (501) staff       (20)        1 2023-04-21 16:57:50.000000 ValiotWorker-5.3.2/ValiotWorker.egg-info/dependency_links.txt
--rw-r--r--   0 baruc      (501) staff       (20)       60 2023-04-21 16:57:50.000000 ValiotWorker-5.3.2/ValiotWorker.egg-info/entry_points.txt
--rw-r--r--   0 baruc      (501) staff       (20)        1 2023-02-17 23:30:14.000000 ValiotWorker-5.3.2/ValiotWorker.egg-info/not-zip-safe
--rw-r--r--   0 baruc      (501) staff       (20)      237 2023-04-21 16:57:50.000000 ValiotWorker-5.3.2/ValiotWorker.egg-info/requires.txt
--rw-r--r--   0 baruc      (501) staff       (20)       13 2023-04-21 16:57:50.000000 ValiotWorker-5.3.2/ValiotWorker.egg-info/top_level.txt
--rw-r--r--   0 baruc      (501) staff       (20)       38 2023-04-21 16:57:50.409360 ValiotWorker-5.3.2/setup.cfg
--rw-r--r--   0 baruc      (501) staff       (20)     2289 2023-02-22 19:57:08.000000 ValiotWorker-5.3.2/setup.py
-drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-04-21 16:57:50.408592 ValiotWorker-5.3.2/tests/
--rw-r--r--   0 baruc      (501) staff       (20)      106 2023-04-21 16:31:49.000000 ValiotWorker-5.3.2/tests/test_dummy.py
+drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-05-24 15:22:20.741697 ValiotWorker-5.3.3/
+-rw-r--r--   0 baruc      (501) staff       (20)     1074 2021-04-26 22:17:35.000000 ValiotWorker-5.3.3/LICENCE
+-rw-r--r--   0 baruc      (501) staff       (20)       37 2023-02-24 03:38:26.000000 ValiotWorker-5.3.3/MANIFEST.in
+-rw-r--r--   0 baruc      (501) staff       (20)     2158 2023-05-24 15:22:20.741476 ValiotWorker-5.3.3/PKG-INFO
+-rw-r--r--   0 baruc      (501) staff       (20)     1811 2021-04-26 22:17:35.000000 ValiotWorker-5.3.3/README.md
+drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-05-24 15:22:20.737334 ValiotWorker-5.3.3/ValiotWorker/
+-rw-r--r--   0 baruc      (501) staff       (20)     3486 2023-04-19 23:58:36.000000 ValiotWorker-5.3.3/ValiotWorker/Logging.py
+-rw-r--r--   0 baruc      (501) staff       (20)    13430 2021-12-23 22:44:57.000000 ValiotWorker-5.3.3/ValiotWorker/Notifications.py
+-rw-r--r--   0 baruc      (501) staff       (20)      294 2023-03-27 19:36:21.000000 ValiotWorker-5.3.3/ValiotWorker/__init__.py
+-rw-r--r--   0 baruc      (501) staff       (20)     3450 2023-05-24 13:52:21.000000 ValiotWorker-5.3.3/ValiotWorker/__main__.py
+-rw-r--r--   0 baruc      (501) staff       (20)       22 2023-05-24 15:20:48.000000 ValiotWorker-5.3.3/ValiotWorker/__version__.py
+-rw-r--r--   0 baruc      (501) staff       (20)      276 2023-02-21 21:58:52.000000 ValiotWorker-5.3.3/ValiotWorker/croniterHelpers.py
+-rw-r--r--   0 baruc      (501) staff       (20)      218 2023-02-21 21:58:52.000000 ValiotWorker-5.3.3/ValiotWorker/dateHelpers.py
+drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-05-24 15:22:20.740429 ValiotWorker-5.3.3/ValiotWorker/healthCheckProbe/
+-rw-r--r--   0 baruc      (501) staff       (20)       41 2023-02-24 03:33:56.000000 ValiotWorker-5.3.3/ValiotWorker/healthCheckProbe/__init__.py
+-rw-r--r--   0 baruc      (501) staff       (20)      963 2023-03-07 23:36:56.000000 ValiotWorker-5.3.3/ValiotWorker/healthCheckProbe/__main__.py
+drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-05-24 15:22:20.740743 ValiotWorker-5.3.3/ValiotWorker/healthCheckProbe/modules/
+-rw-r--r--   0 baruc      (501) staff       (20)     1593 2023-02-24 03:33:56.000000 ValiotWorker-5.3.3/ValiotWorker/healthCheckProbe/modules/http_server.py
+-rw-r--r--   0 baruc      (501) staff       (20)     7003 2023-03-07 22:03:01.000000 ValiotWorker-5.3.3/ValiotWorker/mutations.py
+-rw-r--r--   0 baruc      (501) staff       (20)     4394 2023-03-07 23:36:56.000000 ValiotWorker-5.3.3/ValiotWorker/queries.py
+-rw-r--r--   0 baruc      (501) staff       (20)     5885 2023-05-24 13:52:21.000000 ValiotWorker-5.3.3/ValiotWorker/redis.py
+-rw-r--r--   0 baruc      (501) staff       (20)     1244 2023-03-27 19:36:21.000000 ValiotWorker-5.3.3/ValiotWorker/subscriptions.py
+-rw-r--r--   0 baruc      (501) staff       (20)      182 2021-12-23 22:44:57.000000 ValiotWorker-5.3.3/ValiotWorker/uploaders.py
+-rw-r--r--   0 baruc      (501) staff       (20)    69941 2023-05-24 15:20:39.000000 ValiotWorker-5.3.3/ValiotWorker/worker.py
+drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-05-24 15:22:20.739865 ValiotWorker-5.3.3/ValiotWorker.egg-info/
+-rw-r--r--   0 baruc      (501) staff       (20)     2158 2023-05-24 15:22:20.000000 ValiotWorker-5.3.3/ValiotWorker.egg-info/PKG-INFO
+-rw-r--r--   0 baruc      (501) staff       (20)      791 2023-05-24 15:22:20.000000 ValiotWorker-5.3.3/ValiotWorker.egg-info/SOURCES.txt
+-rw-r--r--   0 baruc      (501) staff       (20)        1 2023-05-24 15:22:20.000000 ValiotWorker-5.3.3/ValiotWorker.egg-info/dependency_links.txt
+-rw-r--r--   0 baruc      (501) staff       (20)       60 2023-05-24 15:22:20.000000 ValiotWorker-5.3.3/ValiotWorker.egg-info/entry_points.txt
+-rw-r--r--   0 baruc      (501) staff       (20)        1 2023-02-17 23:30:14.000000 ValiotWorker-5.3.3/ValiotWorker.egg-info/not-zip-safe
+-rw-r--r--   0 baruc      (501) staff       (20)      237 2023-05-24 15:22:20.000000 ValiotWorker-5.3.3/ValiotWorker.egg-info/requires.txt
+-rw-r--r--   0 baruc      (501) staff       (20)       13 2023-05-24 15:22:20.000000 ValiotWorker-5.3.3/ValiotWorker.egg-info/top_level.txt
+-rw-r--r--   0 baruc      (501) staff       (20)       38 2023-05-24 15:22:20.741755 ValiotWorker-5.3.3/setup.cfg
+-rw-r--r--   0 baruc      (501) staff       (20)     2289 2023-02-22 19:57:08.000000 ValiotWorker-5.3.3/setup.py
+drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-05-24 15:22:20.741066 ValiotWorker-5.3.3/tests/
+-rw-r--r--   0 baruc      (501) staff       (20)      106 2023-05-24 13:52:21.000000 ValiotWorker-5.3.3/tests/test_dummy.py
```

### Comparing `ValiotWorker-5.3.2/LICENCE` & `ValiotWorker-5.3.3/LICENCE`

 * *Files identical despite different names*

### Comparing `ValiotWorker-5.3.2/PKG-INFO` & `ValiotWorker-5.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ValiotWorker
-Version: 5.3.2
+Version: 5.3.3
 Summary: Enables running Python functions as standalone jobs based on interaction with valiot-jobs API
 Home-page: https://github.com/valiot/python-gql-worker
 Author: Valiot
 Author-email: hiring@valiot.io
 Keywords: ValiotWorker
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `ValiotWorker-5.3.2/README.md` & `ValiotWorker-5.3.3/README.md`

 * *Files identical despite different names*

### Comparing `ValiotWorker-5.3.2/ValiotWorker/Logging.py` & `ValiotWorker-5.3.3/ValiotWorker/Logging.py`

 * *Files identical despite different names*

### Comparing `ValiotWorker-5.3.2/ValiotWorker/Notifications.py` & `ValiotWorker-5.3.3/ValiotWorker/Notifications.py`

 * *Files identical despite different names*

### Comparing `ValiotWorker-5.3.2/ValiotWorker/__main__.py` & `ValiotWorker-5.3.3/ValiotWorker/__main__.py`

 * *Files identical despite different names*

### Comparing `ValiotWorker-5.3.2/ValiotWorker/healthCheckProbe/__main__.py` & `ValiotWorker-5.3.3/ValiotWorker/healthCheckProbe/__main__.py`

 * *Files identical despite different names*

### Comparing `ValiotWorker-5.3.2/ValiotWorker/healthCheckProbe/modules/http_server.py` & `ValiotWorker-5.3.3/ValiotWorker/healthCheckProbe/modules/http_server.py`

 * *Files identical despite different names*

### Comparing `ValiotWorker-5.3.2/ValiotWorker/mutations.py` & `ValiotWorker-5.3.3/ValiotWorker/mutations.py`

 * *Files identical despite different names*

### Comparing `ValiotWorker-5.3.2/ValiotWorker/queries.py` & `ValiotWorker-5.3.3/ValiotWorker/queries.py`

 * *Files identical despite different names*

### Comparing `ValiotWorker-5.3.2/ValiotWorker/redis.py` & `ValiotWorker-5.3.3/ValiotWorker/redis.py`

 * *Files identical despite different names*

### Comparing `ValiotWorker-5.3.2/ValiotWorker/subscriptions.py` & `ValiotWorker-5.3.3/ValiotWorker/subscriptions.py`

 * *Files identical despite different names*

### Comparing `ValiotWorker-5.3.2/ValiotWorker/worker.py` & `ValiotWorker-5.3.3/ValiotWorker/worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -766,17 +766,20 @@
             self.currentQueues[queue_index]['locks'] = [lock]
         elif action == 'updated':
             log_from_queue(LogLevel.SUCCESS,
                            f'Queue {queue["name"]} lock updated')
             lock_index = __.find_index(
                 current_queue['locks'], lambda l: l['id'] == lock['id'])
             if lock_index == -1:
-                self.currentQueues[queue_index]['locks'].append(lock)
-                self.currentQueues[queue_index]['locks'] = __.sort_by(
-                    self.currentQueues[queue_index]['locks'], 'updatedAt', reverse=True)
+                if lock is not None:
+                    log_from_queue(LogLevel.WARNING,
+                           f'Lock not found in current locks list, appending and sorting...')
+                    self.currentQueues[queue_index]['locks'].append(lock)
+                    self.currentQueues[queue_index]['locks'] = __.sort_by(
+                        self.currentQueues[queue_index]['locks'], 'updatedAt', reverse=True)
             else:
                 self.currentQueues[queue_index]['locks'][lock_index] = lock
         elif action == 'deleted':
             log_from_queue(LogLevel.SUCCESS,
                            f'Queue {queue["name"]} lock released')
             lock_index = __.find_index(
                 current_queue['locks'], lambda l: l['id'] == lock['id'])
```

### Comparing `ValiotWorker-5.3.2/ValiotWorker.egg-info/PKG-INFO` & `ValiotWorker-5.3.3/ValiotWorker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ValiotWorker
-Version: 5.3.2
+Version: 5.3.3
 Summary: Enables running Python functions as standalone jobs based on interaction with valiot-jobs API
 Home-page: https://github.com/valiot/python-gql-worker
 Author: Valiot
 Author-email: hiring@valiot.io
 Keywords: ValiotWorker
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `ValiotWorker-5.3.2/ValiotWorker.egg-info/SOURCES.txt` & `ValiotWorker-5.3.3/ValiotWorker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ValiotWorker-5.3.2/setup.py` & `ValiotWorker-5.3.3/setup.py`

 * *Files identical despite different names*

