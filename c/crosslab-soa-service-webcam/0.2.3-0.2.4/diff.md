# Comparing `tmp/crosslab_soa_service_webcam-0.2.3.tar.gz` & `tmp/crosslab_soa_service_webcam-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crosslab_soa_service_webcam-0.2.3.tar", last modified: Fri May 19 08:19:53 2023, max compression
+gzip compressed data, was "crosslab_soa_service_webcam-0.2.4.tar", last modified: Wed May 24 18:58:49 2023, max compression
```

## Comparing `crosslab_soa_service_webcam-0.2.3.tar` & `crosslab_soa_service_webcam-0.2.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:19:53.467347 crosslab_soa_service_webcam-0.2.3/
--rw-r--r--   0 dev       (1000) docker-host   (967)      348 2023-05-19 08:19:53.467347 crosslab_soa_service_webcam-0.2.3/PKG-INFO
--rw-r--r--   0 dev       (1000) docker-host   (967)       87 2023-04-03 16:08:17.000000 crosslab_soa_service_webcam-0.2.3/pyproject.toml
--rw-r--r--   0 dev       (1000) docker-host   (967)      578 2023-05-19 08:19:53.467347 crosslab_soa_service_webcam-0.2.3/setup.cfg
--rw-r--r--   0 dev       (1000) docker-host   (967)       37 2023-04-03 16:08:17.000000 crosslab_soa_service_webcam-0.2.3/setup.py
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:19:53.467347 crosslab_soa_service_webcam-0.2.3/src/
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:19:53.467347 crosslab_soa_service_webcam-0.2.3/src/crosslab/
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:19:53.467347 crosslab_soa_service_webcam-0.2.3/src/crosslab/soa_services/
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:19:53.467347 crosslab_soa_service_webcam-0.2.3/src/crosslab/soa_services/webcam/
--rw-r--r--   0 dev       (1000) docker-host   (967)      153 2023-04-03 16:08:17.000000 crosslab_soa_service_webcam-0.2.3/src/crosslab/soa_services/webcam/__init__.py
--rw-r--r--   0 dev       (1000) docker-host   (967)     1165 2023-05-19 07:55:53.000000 crosslab_soa_service_webcam-0.2.3/src/crosslab/soa_services/webcam/media.py
--rw-r--r--   0 dev       (1000) docker-host   (967)      151 2023-04-26 09:19:14.000000 crosslab_soa_service_webcam-0.2.3/src/crosslab/soa_services/webcam/messages.py
--rw-r--r--   0 dev       (1000) docker-host   (967)        0 2023-04-03 16:08:17.000000 crosslab_soa_service_webcam-0.2.3/src/crosslab/soa_services/webcam/py.typed
--rw-r--r--   0 dev       (1000) docker-host   (967)     1051 2023-04-26 09:19:14.000000 crosslab_soa_service_webcam-0.2.3/src/crosslab/soa_services/webcam/webcam_service.py
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:19:53.467347 crosslab_soa_service_webcam-0.2.3/src/crosslab_soa_service_webcam.egg-info/
--rw-r--r--   0 dev       (1000) docker-host   (967)      348 2023-05-19 08:19:53.000000 crosslab_soa_service_webcam-0.2.3/src/crosslab_soa_service_webcam.egg-info/PKG-INFO
--rw-r--r--   0 dev       (1000) docker-host   (967)      555 2023-05-19 08:19:53.000000 crosslab_soa_service_webcam-0.2.3/src/crosslab_soa_service_webcam.egg-info/SOURCES.txt
--rw-r--r--   0 dev       (1000) docker-host   (967)        1 2023-05-19 08:19:53.000000 crosslab_soa_service_webcam-0.2.3/src/crosslab_soa_service_webcam.egg-info/dependency_links.txt
--rw-r--r--   0 dev       (1000) docker-host   (967)       25 2023-05-19 08:19:53.000000 crosslab_soa_service_webcam-0.2.3/src/crosslab_soa_service_webcam.egg-info/requires.txt
--rw-r--r--   0 dev       (1000) docker-host   (967)        9 2023-05-19 08:19:53.000000 crosslab_soa_service_webcam-0.2.3/src/crosslab_soa_service_webcam.egg-info/top_level.txt
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:19:53.467347 crosslab_soa_service_webcam-0.2.3/tests/
--rw-r--r--   0 dev       (1000) docker-host   (967)      641 2023-05-19 07:55:53.000000 crosslab_soa_service_webcam-0.2.3/tests/test_standard.py
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-24 18:58:49.736116 crosslab_soa_service_webcam-0.2.4/
+-rw-r--r--   0 dev       (1000) docker-host   (967)      348 2023-05-24 18:58:49.736116 crosslab_soa_service_webcam-0.2.4/PKG-INFO
+-rw-r--r--   0 dev       (1000) docker-host   (967)       87 2023-02-22 10:18:01.000000 crosslab_soa_service_webcam-0.2.4/pyproject.toml
+-rw-r--r--   0 dev       (1000) docker-host   (967)      578 2023-05-24 18:58:49.736116 crosslab_soa_service_webcam-0.2.4/setup.cfg
+-rw-r--r--   0 dev       (1000) docker-host   (967)       37 2023-02-22 10:18:01.000000 crosslab_soa_service_webcam-0.2.4/setup.py
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-24 18:58:49.732783 crosslab_soa_service_webcam-0.2.4/src/
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-24 18:58:49.732783 crosslab_soa_service_webcam-0.2.4/src/crosslab/
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-24 18:58:49.732783 crosslab_soa_service_webcam-0.2.4/src/crosslab/soa_services/
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-24 18:58:49.736116 crosslab_soa_service_webcam-0.2.4/src/crosslab/soa_services/webcam/
+-rw-r--r--   0 dev       (1000) docker-host   (967)      153 2023-02-22 10:18:01.000000 crosslab_soa_service_webcam-0.2.4/src/crosslab/soa_services/webcam/__init__.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)     1165 2023-05-02 06:17:30.000000 crosslab_soa_service_webcam-0.2.4/src/crosslab/soa_services/webcam/media.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)      151 2023-04-20 09:47:47.000000 crosslab_soa_service_webcam-0.2.4/src/crosslab/soa_services/webcam/messages.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)        0 2023-02-22 10:18:01.000000 crosslab_soa_service_webcam-0.2.4/src/crosslab/soa_services/webcam/py.typed
+-rw-r--r--   0 dev       (1000) docker-host   (967)     1056 2023-05-22 07:55:59.000000 crosslab_soa_service_webcam-0.2.4/src/crosslab/soa_services/webcam/webcam_service.py
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-24 18:58:49.736116 crosslab_soa_service_webcam-0.2.4/src/crosslab_soa_service_webcam.egg-info/
+-rw-r--r--   0 dev       (1000) docker-host   (967)      348 2023-05-24 18:58:49.000000 crosslab_soa_service_webcam-0.2.4/src/crosslab_soa_service_webcam.egg-info/PKG-INFO
+-rw-r--r--   0 dev       (1000) docker-host   (967)      555 2023-05-24 18:58:49.000000 crosslab_soa_service_webcam-0.2.4/src/crosslab_soa_service_webcam.egg-info/SOURCES.txt
+-rw-r--r--   0 dev       (1000) docker-host   (967)        1 2023-05-24 18:58:49.000000 crosslab_soa_service_webcam-0.2.4/src/crosslab_soa_service_webcam.egg-info/dependency_links.txt
+-rw-r--r--   0 dev       (1000) docker-host   (967)       25 2023-05-24 18:58:49.000000 crosslab_soa_service_webcam-0.2.4/src/crosslab_soa_service_webcam.egg-info/requires.txt
+-rw-r--r--   0 dev       (1000) docker-host   (967)        9 2023-05-24 18:58:49.000000 crosslab_soa_service_webcam-0.2.4/src/crosslab_soa_service_webcam.egg-info/top_level.txt
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-24 18:58:49.736116 crosslab_soa_service_webcam-0.2.4/tests/
+-rw-r--r--   0 dev       (1000) docker-host   (967)      641 2023-05-02 06:17:30.000000 crosslab_soa_service_webcam-0.2.4/tests/test_standard.py
```

### Comparing `crosslab_soa_service_webcam-0.2.3/setup.cfg` & `crosslab_soa_service_webcam-0.2.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = crosslab_soa_service_webcam
-version = 0.2.3
+version = 0.2.4
 author = Johannes Nau
 author_email = johannes.nau@tu-ilmenau.de
 description = The CrossLab SOA Webcam Service.
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: Other/Proprietary License
 	Operating System :: OS Independent
```

### Comparing `crosslab_soa_service_webcam-0.2.3/src/crosslab/soa_services/webcam/media.py` & `crosslab_soa_service_webcam-0.2.4/src/crosslab/soa_services/webcam/media.py`

 * *Files identical despite different names*

### Comparing `crosslab_soa_service_webcam-0.2.3/src/crosslab/soa_services/webcam/webcam_service.py` & `crosslab_soa_service_webcam-0.2.4/src/crosslab/soa_services/webcam/webcam_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from crosslab.soa_client.service import Service
 
 from crosslab.soa_services.webcam.messages import WebcamServiceConfig
 
 
 class WebcamService__Producer(Service):
     service_type = "http://api.goldi-labs.de/serviceTypes/webcam"
-    service_direction = "out"
+    service_direction = "producer"
     service_id: str
 
     _track: MediaStreamTrack
 
     def __init__(self, track: MediaStreamTrack, service_id: str):
         self.service_id = service_id
         self._track = track
```

### Comparing `crosslab_soa_service_webcam-0.2.3/src/crosslab_soa_service_webcam.egg-info/SOURCES.txt` & `crosslab_soa_service_webcam-0.2.4/src/crosslab_soa_service_webcam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crosslab_soa_service_webcam-0.2.3/tests/test_standard.py` & `crosslab_soa_service_webcam-0.2.4/tests/test_standard.py`

 * *Files identical despite different names*

