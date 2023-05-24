# Comparing `tmp/crosslab_soa_service_message-0.2.3.tar.gz` & `tmp/crosslab_soa_service_message-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crosslab_soa_service_message-0.2.3.tar", last modified: Fri May 19 08:24:10 2023, max compression
+gzip compressed data, was "crosslab_soa_service_message-0.2.4.tar", last modified: Wed May 24 19:02:29 2023, max compression
```

## Comparing `crosslab_soa_service_message-0.2.3.tar` & `crosslab_soa_service_message-0.2.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:24:10.148730 crosslab_soa_service_message-0.2.3/
--rw-r--r--   0 dev       (1000) docker-host   (967)      350 2023-05-19 08:24:10.148730 crosslab_soa_service_message-0.2.3/PKG-INFO
--rw-r--r--   0 dev       (1000) docker-host   (967)       87 2023-04-03 16:08:17.000000 crosslab_soa_service_message-0.2.3/pyproject.toml
--rw-r--r--   0 dev       (1000) docker-host   (967)      580 2023-05-19 08:24:10.148730 crosslab_soa_service_message-0.2.3/setup.cfg
--rw-r--r--   0 dev       (1000) docker-host   (967)       37 2023-04-03 16:08:17.000000 crosslab_soa_service_message-0.2.3/setup.py
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:24:10.145397 crosslab_soa_service_message-0.2.3/src/
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:24:10.145397 crosslab_soa_service_message-0.2.3/src/crosslab/
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:24:10.145397 crosslab_soa_service_message-0.2.3/src/crosslab/soa_services/
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:24:10.145397 crosslab_soa_service_message-0.2.3/src/crosslab/soa_services/message/
--rw-r--r--   0 dev       (1000) docker-host   (967)      213 2023-04-03 16:08:17.000000 crosslab_soa_service_message-0.2.3/src/crosslab/soa_services/message/__init__.py
--rw-r--r--   0 dev       (1000) docker-host   (967)     2607 2023-04-26 09:19:14.000000 crosslab_soa_service_message-0.2.3/src/crosslab/soa_services/message/message_service.py
--rw-r--r--   0 dev       (1000) docker-host   (967)      232 2023-04-03 16:08:17.000000 crosslab_soa_service_message-0.2.3/src/crosslab/soa_services/message/messages.py
--rw-r--r--   0 dev       (1000) docker-host   (967)        0 2023-04-03 16:08:17.000000 crosslab_soa_service_message-0.2.3/src/crosslab/soa_services/message/py.typed
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:24:10.145397 crosslab_soa_service_message-0.2.3/src/crosslab_soa_service_message.egg-info/
--rw-r--r--   0 dev       (1000) docker-host   (967)      350 2023-05-19 08:24:10.000000 crosslab_soa_service_message-0.2.3/src/crosslab_soa_service_message.egg-info/PKG-INFO
--rw-r--r--   0 dev       (1000) docker-host   (967)      523 2023-05-19 08:24:10.000000 crosslab_soa_service_message-0.2.3/src/crosslab_soa_service_message.egg-info/SOURCES.txt
--rw-r--r--   0 dev       (1000) docker-host   (967)        1 2023-05-19 08:24:10.000000 crosslab_soa_service_message-0.2.3/src/crosslab_soa_service_message.egg-info/dependency_links.txt
--rw-r--r--   0 dev       (1000) docker-host   (967)       25 2023-05-19 08:24:10.000000 crosslab_soa_service_message-0.2.3/src/crosslab_soa_service_message.egg-info/requires.txt
--rw-r--r--   0 dev       (1000) docker-host   (967)        9 2023-05-19 08:24:10.000000 crosslab_soa_service_message-0.2.3/src/crosslab_soa_service_message.egg-info/top_level.txt
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:24:10.148730 crosslab_soa_service_message-0.2.3/tests/
--rw-r--r--   0 dev       (1000) docker-host   (967)      916 2023-04-26 09:19:14.000000 crosslab_soa_service_message-0.2.3/tests/test_standard.py
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-24 19:02:29.299892 crosslab_soa_service_message-0.2.4/
+-rw-r--r--   0 dev       (1000) docker-host   (967)      350 2023-05-24 19:02:29.299892 crosslab_soa_service_message-0.2.4/PKG-INFO
+-rw-r--r--   0 dev       (1000) docker-host   (967)       87 2023-02-22 10:18:01.000000 crosslab_soa_service_message-0.2.4/pyproject.toml
+-rw-r--r--   0 dev       (1000) docker-host   (967)      580 2023-05-24 19:02:29.299892 crosslab_soa_service_message-0.2.4/setup.cfg
+-rw-r--r--   0 dev       (1000) docker-host   (967)       37 2023-02-22 10:18:01.000000 crosslab_soa_service_message-0.2.4/setup.py
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-24 19:02:29.296558 crosslab_soa_service_message-0.2.4/src/
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-24 19:02:29.296558 crosslab_soa_service_message-0.2.4/src/crosslab/
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-24 19:02:29.296558 crosslab_soa_service_message-0.2.4/src/crosslab/soa_services/
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-24 19:02:29.299892 crosslab_soa_service_message-0.2.4/src/crosslab/soa_services/message/
+-rw-r--r--   0 dev       (1000) docker-host   (967)      213 2023-02-22 10:18:01.000000 crosslab_soa_service_message-0.2.4/src/crosslab/soa_services/message/__init__.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)     2618 2023-05-22 07:55:59.000000 crosslab_soa_service_message-0.2.4/src/crosslab/soa_services/message/message_service.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)      232 2023-02-22 10:18:01.000000 crosslab_soa_service_message-0.2.4/src/crosslab/soa_services/message/messages.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)        0 2023-02-22 10:18:01.000000 crosslab_soa_service_message-0.2.4/src/crosslab/soa_services/message/py.typed
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-24 19:02:29.299892 crosslab_soa_service_message-0.2.4/src/crosslab_soa_service_message.egg-info/
+-rw-r--r--   0 dev       (1000) docker-host   (967)      350 2023-05-24 19:02:29.000000 crosslab_soa_service_message-0.2.4/src/crosslab_soa_service_message.egg-info/PKG-INFO
+-rw-r--r--   0 dev       (1000) docker-host   (967)      523 2023-05-24 19:02:29.000000 crosslab_soa_service_message-0.2.4/src/crosslab_soa_service_message.egg-info/SOURCES.txt
+-rw-r--r--   0 dev       (1000) docker-host   (967)        1 2023-05-24 19:02:29.000000 crosslab_soa_service_message-0.2.4/src/crosslab_soa_service_message.egg-info/dependency_links.txt
+-rw-r--r--   0 dev       (1000) docker-host   (967)       25 2023-05-24 19:02:29.000000 crosslab_soa_service_message-0.2.4/src/crosslab_soa_service_message.egg-info/requires.txt
+-rw-r--r--   0 dev       (1000) docker-host   (967)        9 2023-05-24 19:02:29.000000 crosslab_soa_service_message-0.2.4/src/crosslab_soa_service_message.egg-info/top_level.txt
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-24 19:02:29.299892 crosslab_soa_service_message-0.2.4/tests/
+-rw-r--r--   0 dev       (1000) docker-host   (967)      916 2023-04-20 09:47:47.000000 crosslab_soa_service_message-0.2.4/tests/test_standard.py
```

### Comparing `crosslab_soa_service_message-0.2.3/setup.cfg` & `crosslab_soa_service_message-0.2.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = crosslab_soa_service_message
-version = 0.2.3
+version = 0.2.4
 author = Johannes Nau
 author_email = johannes.nau@tu-ilmenau.de
 description = The CrossLab SOA message Service.
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: Other/Proprietary License
 	Operating System :: OS Independent
```

### Comparing `crosslab_soa_service_message-0.2.3/src/crosslab/soa_services/message/message_service.py` & `crosslab_soa_service_message-0.2.4/src/crosslab/soa_services/message/message_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     MessageServiceConfig,
     MessageServiceEvent,
 )
 
 
 class MessageService__Producer(Service):
     service_type = "https://api.goldi-labs.de/serviceTypes/message"
-    service_direction = "out"
+    service_direction = "producer"
     service_id: str
 
     def __init__(self, service_id: str):
         self.service_id = service_id
 
     def getMeta(self):
         return {
@@ -40,15 +40,15 @@
 
     async def sendMessage(self, message: str, message_type: Literal["info", "error"]):
         self.channel.send(json.dumps({"messageType": message_type, "message": message}))
 
 
 class MessageService__Consumer(Service, AsyncIOEventEmitter):
     service_type = "https://api.goldi-labs.de/serviceTypes/message"
-    service_direction = "in"
+    service_direction = "consumer"
     service_id: str
 
     def __init__(self, service_id: str):
         AsyncIOEventEmitter.__init__(self)
         self.service_id = service_id
 
     def getMeta(self):
```

### Comparing `crosslab_soa_service_message-0.2.3/src/crosslab_soa_service_message.egg-info/SOURCES.txt` & `crosslab_soa_service_message-0.2.4/src/crosslab_soa_service_message.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crosslab_soa_service_message-0.2.3/tests/test_standard.py` & `crosslab_soa_service_message-0.2.4/tests/test_standard.py`

 * *Files identical despite different names*

