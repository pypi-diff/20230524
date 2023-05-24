# Comparing `tmp/crosslab_soa_service_file-0.2.3.tar.gz` & `tmp/crosslab_soa_service_file-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crosslab_soa_service_file-0.2.3.tar", last modified: Fri May 19 08:21:56 2023, max compression
+gzip compressed data, was "crosslab_soa_service_file-0.2.4.tar", last modified: Wed May 24 19:00:24 2023, max compression
```

## Comparing `crosslab_soa_service_file-0.2.3.tar` & `crosslab_soa_service_file-0.2.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:21:56.798019 crosslab_soa_service_file-0.2.3/
--rw-r--r--   0 dev       (1000) docker-host   (967)      344 2023-05-19 08:21:56.798019 crosslab_soa_service_file-0.2.3/PKG-INFO
--rw-r--r--   0 dev       (1000) docker-host   (967)       87 2023-04-03 16:08:17.000000 crosslab_soa_service_file-0.2.3/pyproject.toml
--rw-r--r--   0 dev       (1000) docker-host   (967)      574 2023-05-19 08:21:56.801353 crosslab_soa_service_file-0.2.3/setup.cfg
--rw-r--r--   0 dev       (1000) docker-host   (967)       37 2023-04-03 16:08:17.000000 crosslab_soa_service_file-0.2.3/setup.py
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:21:56.798019 crosslab_soa_service_file-0.2.3/src/
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:21:56.798019 crosslab_soa_service_file-0.2.3/src/crosslab/
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:21:56.798019 crosslab_soa_service_file-0.2.3/src/crosslab/soa_services/
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:21:56.798019 crosslab_soa_service_file-0.2.3/src/crosslab/soa_services/file/
--rw-r--r--   0 dev       (1000) docker-host   (967)      192 2023-04-03 16:08:17.000000 crosslab_soa_service_file-0.2.3/src/crosslab/soa_services/file/__init__.py
--rw-r--r--   0 dev       (1000) docker-host   (967)     2541 2023-04-26 09:19:14.000000 crosslab_soa_service_file-0.2.3/src/crosslab/soa_services/file/file_service.py
--rw-r--r--   0 dev       (1000) docker-host   (967)      222 2023-04-03 16:08:17.000000 crosslab_soa_service_file-0.2.3/src/crosslab/soa_services/file/messages.py
--rw-r--r--   0 dev       (1000) docker-host   (967)        0 2023-04-03 16:08:17.000000 crosslab_soa_service_file-0.2.3/src/crosslab/soa_services/file/py.typed
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:21:56.798019 crosslab_soa_service_file-0.2.3/src/crosslab_soa_service_file.egg-info/
--rw-r--r--   0 dev       (1000) docker-host   (967)      344 2023-05-19 08:21:56.000000 crosslab_soa_service_file-0.2.3/src/crosslab_soa_service_file.egg-info/PKG-INFO
--rw-r--r--   0 dev       (1000) docker-host   (967)      493 2023-05-19 08:21:56.000000 crosslab_soa_service_file-0.2.3/src/crosslab_soa_service_file.egg-info/SOURCES.txt
--rw-r--r--   0 dev       (1000) docker-host   (967)        1 2023-05-19 08:21:56.000000 crosslab_soa_service_file-0.2.3/src/crosslab_soa_service_file.egg-info/dependency_links.txt
--rw-r--r--   0 dev       (1000) docker-host   (967)       25 2023-05-19 08:21:56.000000 crosslab_soa_service_file-0.2.3/src/crosslab_soa_service_file.egg-info/requires.txt
--rw-r--r--   0 dev       (1000) docker-host   (967)        9 2023-05-19 08:21:56.000000 crosslab_soa_service_file-0.2.3/src/crosslab_soa_service_file.egg-info/top_level.txt
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:21:56.798019 crosslab_soa_service_file-0.2.3/tests/
--rw-r--r--   0 dev       (1000) docker-host   (967)      898 2023-04-26 09:19:14.000000 crosslab_soa_service_file-0.2.3/tests/test_standard.py
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-24 19:00:24.100051 crosslab_soa_service_file-0.2.4/
+-rw-r--r--   0 dev       (1000) docker-host   (967)      344 2023-05-24 19:00:24.100051 crosslab_soa_service_file-0.2.4/PKG-INFO
+-rw-r--r--   0 dev       (1000) docker-host   (967)       87 2023-02-22 10:18:01.000000 crosslab_soa_service_file-0.2.4/pyproject.toml
+-rw-r--r--   0 dev       (1000) docker-host   (967)      574 2023-05-24 19:00:24.100051 crosslab_soa_service_file-0.2.4/setup.cfg
+-rw-r--r--   0 dev       (1000) docker-host   (967)       37 2023-02-22 10:18:01.000000 crosslab_soa_service_file-0.2.4/setup.py
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-24 19:00:24.100051 crosslab_soa_service_file-0.2.4/src/
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-24 19:00:24.100051 crosslab_soa_service_file-0.2.4/src/crosslab/
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-24 19:00:24.100051 crosslab_soa_service_file-0.2.4/src/crosslab/soa_services/
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-24 19:00:24.100051 crosslab_soa_service_file-0.2.4/src/crosslab/soa_services/file/
+-rw-r--r--   0 dev       (1000) docker-host   (967)      192 2023-02-22 10:18:01.000000 crosslab_soa_service_file-0.2.4/src/crosslab/soa_services/file/__init__.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)     2551 2023-05-22 07:55:59.000000 crosslab_soa_service_file-0.2.4/src/crosslab/soa_services/file/file_service.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)      222 2023-02-22 10:18:01.000000 crosslab_soa_service_file-0.2.4/src/crosslab/soa_services/file/messages.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)        0 2023-02-22 10:18:01.000000 crosslab_soa_service_file-0.2.4/src/crosslab/soa_services/file/py.typed
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-24 19:00:24.100051 crosslab_soa_service_file-0.2.4/src/crosslab_soa_service_file.egg-info/
+-rw-r--r--   0 dev       (1000) docker-host   (967)      344 2023-05-24 19:00:24.000000 crosslab_soa_service_file-0.2.4/src/crosslab_soa_service_file.egg-info/PKG-INFO
+-rw-r--r--   0 dev       (1000) docker-host   (967)      493 2023-05-24 19:00:24.000000 crosslab_soa_service_file-0.2.4/src/crosslab_soa_service_file.egg-info/SOURCES.txt
+-rw-r--r--   0 dev       (1000) docker-host   (967)        1 2023-05-24 19:00:24.000000 crosslab_soa_service_file-0.2.4/src/crosslab_soa_service_file.egg-info/dependency_links.txt
+-rw-r--r--   0 dev       (1000) docker-host   (967)       25 2023-05-24 19:00:24.000000 crosslab_soa_service_file-0.2.4/src/crosslab_soa_service_file.egg-info/requires.txt
+-rw-r--r--   0 dev       (1000) docker-host   (967)        9 2023-05-24 19:00:24.000000 crosslab_soa_service_file-0.2.4/src/crosslab_soa_service_file.egg-info/top_level.txt
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-24 19:00:24.100051 crosslab_soa_service_file-0.2.4/tests/
+-rw-r--r--   0 dev       (1000) docker-host   (967)      898 2023-04-20 09:47:47.000000 crosslab_soa_service_file-0.2.4/tests/test_standard.py
```

### Comparing `crosslab_soa_service_file-0.2.3/setup.cfg` & `crosslab_soa_service_file-0.2.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = crosslab_soa_service_file
-version = 0.2.3
+version = 0.2.4
 author = Johannes Nau
 author_email = johannes.nau@tu-ilmenau.de
 description = The CrossLab SOA file Service.
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: Other/Proprietary License
 	Operating System :: OS Independent
```

### Comparing `crosslab_soa_service_file-0.2.3/src/crosslab/soa_services/file/file_service.py` & `crosslab_soa_service_file-0.2.4/src/crosslab/soa_services/file/file_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from pyee.asyncio import AsyncIOEventEmitter
 
 from crosslab.soa_services.file.messages import FileServiceConfig, FileServiceEvent
 
 
 class FileService__Producer(Service):
     service_type = "https://api.goldi-labs.de/serviceTypes/file"
-    service_direction = "out"
+    service_direction = "producer"
     service_id: str
 
     def __init__(self, service_id: str):
         self.service_id = service_id
 
     def getMeta(self):
         return {
@@ -36,15 +36,15 @@
     async def sendFile(self, file_type: str, content: bytes):
         self.channel.send(json.dumps({"fileType": file_type, "length": len(content)}))
         self.channel.send(content)
 
 
 class FileService__Consumer(Service, AsyncIOEventEmitter):
     service_type = "https://api.goldi-labs.de/serviceTypes/file"
-    service_direction = "out"
+    service_direction = "consumer"
     service_id: str
 
     def __init__(self, service_id: str):
         AsyncIOEventEmitter.__init__(self)
         self.service_id = service_id
 
     def getMeta(self):
```

### Comparing `crosslab_soa_service_file-0.2.3/tests/test_standard.py` & `crosslab_soa_service_file-0.2.4/tests/test_standard.py`

 * *Files identical despite different names*

