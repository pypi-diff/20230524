# Comparing `tmp/crosslab_soa_client-0.2.2.tar.gz` & `tmp/crosslab_soa_client-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crosslab_soa_client-0.2.2.tar", last modified: Wed Apr 19 18:28:41 2023, max compression
+gzip compressed data, was "crosslab_soa_client-0.2.3.tar", last modified: Fri May 19 08:15:40 2023, max compression
```

## Comparing `crosslab_soa_client-0.2.2.tar` & `crosslab_soa_client-0.2.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:28:41.422602 crosslab_soa_client-0.2.2/
--rw-r--r--   0 dev       (1000) docker-host   (967)      331 2023-04-19 18:28:41.422602 crosslab_soa_client-0.2.2/PKG-INFO
--rw-r--r--   0 dev       (1000) docker-host   (967)     2494 2023-04-19 18:06:55.000000 crosslab_soa_client-0.2.2/README.md
--rw-r--r--   0 dev       (1000) docker-host   (967)       87 2023-02-14 11:45:37.000000 crosslab_soa_client-0.2.2/pyproject.toml
--rw-r--r--   0 dev       (1000) docker-host   (967)      617 2023-04-19 18:28:41.422602 crosslab_soa_client-0.2.2/setup.cfg
--rw-r--r--   0 dev       (1000) docker-host   (967)       37 2023-02-14 11:45:37.000000 crosslab_soa_client-0.2.2/setup.py
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:28:41.419268 crosslab_soa_client-0.2.2/src/
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:28:41.419268 crosslab_soa_client-0.2.2/src/crosslab/
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:28:41.422602 crosslab_soa_client-0.2.2/src/crosslab/soa_client/
--rw-r--r--   0 dev       (1000) docker-host   (967)        0 2023-02-14 11:45:37.000000 crosslab_soa_client-0.2.2/src/crosslab/soa_client/__init__.py
--rw-r--r--   0 dev       (1000) docker-host   (967)     1762 2023-04-19 13:37:16.000000 crosslab_soa_client-0.2.2/src/crosslab/soa_client/connection.py
--rw-r--r--   0 dev       (1000) docker-host   (967)     9539 2023-04-19 13:37:16.000000 crosslab_soa_client-0.2.2/src/crosslab/soa_client/connection_webrtc.py
--rw-r--r--   0 dev       (1000) docker-host   (967)     6244 2023-04-19 13:37:16.000000 crosslab_soa_client-0.2.2/src/crosslab/soa_client/device_handler.py
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:28:41.422602 crosslab_soa_client-0.2.2/src/crosslab/soa_client/media/
--rw-r--r--   0 dev       (1000) docker-host   (967)        0 2023-02-14 11:45:37.000000 crosslab_soa_client-0.2.2/src/crosslab/soa_client/media/__init__.py
--rw-r--r--   0 dev       (1000) docker-host   (967)      395 2023-02-14 11:45:37.000000 crosslab_soa_client-0.2.2/src/crosslab/soa_client/media/gst_track.py
--rw-r--r--   0 dev       (1000) docker-host   (967)      557 2023-02-14 11:45:37.000000 crosslab_soa_client-0.2.2/src/crosslab/soa_client/media/udp_track.py
--rw-r--r--   0 dev       (1000) docker-host   (967)        0 2023-02-14 11:45:37.000000 crosslab_soa_client-0.2.2/src/crosslab/soa_client/message_handling.py
--rw-r--r--   0 dev       (1000) docker-host   (967)     1077 2023-02-14 11:45:37.000000 crosslab_soa_client-0.2.2/src/crosslab/soa_client/messages.py
--rw-r--r--   0 dev       (1000) docker-host   (967)        0 2023-02-14 11:45:37.000000 crosslab_soa_client-0.2.2/src/crosslab/soa_client/py.typed
--rw-r--r--   0 dev       (1000) docker-host   (967)      764 2023-04-19 13:37:16.000000 crosslab_soa_client-0.2.2/src/crosslab/soa_client/service.py
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:28:41.422602 crosslab_soa_client-0.2.2/src/crosslab/soa_client/test_helper/
--rw-r--r--   0 dev       (1000) docker-host   (967)       81 2023-04-19 13:37:16.000000 crosslab_soa_client-0.2.2/src/crosslab/soa_client/test_helper/__init__.py
--rw-r--r--   0 dev       (1000) docker-host   (967)     1051 2023-04-19 13:37:16.000000 crosslab_soa_client-0.2.2/src/crosslab/soa_client/test_helper/connection_stub.py
--rw-r--r--   0 dev       (1000) docker-host   (967)      787 2023-04-19 13:37:16.000000 crosslab_soa_client-0.2.2/src/crosslab/soa_client/test_helper/dummy_track.py
--rw-r--r--   0 dev       (1000) docker-host   (967)     4298 2023-04-19 13:37:16.000000 crosslab_soa_client-0.2.2/src/crosslab/soa_client/test_helper/service_stub.py
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:28:41.422602 crosslab_soa_client-0.2.2/src/crosslab_soa_client.egg-info/
--rw-r--r--   0 dev       (1000) docker-host   (967)      331 2023-04-19 18:28:41.000000 crosslab_soa_client-0.2.2/src/crosslab_soa_client.egg-info/PKG-INFO
--rw-r--r--   0 dev       (1000) docker-host   (967)      981 2023-04-19 18:28:41.000000 crosslab_soa_client-0.2.2/src/crosslab_soa_client.egg-info/SOURCES.txt
--rw-r--r--   0 dev       (1000) docker-host   (967)        1 2023-04-19 18:28:41.000000 crosslab_soa_client-0.2.2/src/crosslab_soa_client.egg-info/dependency_links.txt
--rw-r--r--   0 dev       (1000) docker-host   (967)       36 2023-04-19 18:28:41.000000 crosslab_soa_client-0.2.2/src/crosslab_soa_client.egg-info/requires.txt
--rw-r--r--   0 dev       (1000) docker-host   (967)        9 2023-04-19 18:28:41.000000 crosslab_soa_client-0.2.2/src/crosslab_soa_client.egg-info/top_level.txt
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:28:41.422602 crosslab_soa_client-0.2.2/tests/
--rw-r--r--   0 dev       (1000) docker-host   (967)     1970 2023-04-19 13:37:16.000000 crosslab_soa_client-0.2.2/tests/test_device_handler.py
--rw-r--r--   0 dev       (1000) docker-host   (967)     5239 2023-04-19 13:37:16.000000 crosslab_soa_client-0.2.2/tests/test_webrtc_connection.py
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:15:40.689247 crosslab_soa_client-0.2.3/
+-rw-r--r--   0 dev       (1000) docker-host   (967)      331 2023-05-19 08:15:40.689247 crosslab_soa_client-0.2.3/PKG-INFO
+-rw-r--r--   0 dev       (1000) docker-host   (967)     2494 2023-04-26 09:19:14.000000 crosslab_soa_client-0.2.3/README.md
+-rw-r--r--   0 dev       (1000) docker-host   (967)       87 2023-02-14 11:45:37.000000 crosslab_soa_client-0.2.3/pyproject.toml
+-rw-r--r--   0 dev       (1000) docker-host   (967)      617 2023-05-19 08:15:40.692580 crosslab_soa_client-0.2.3/setup.cfg
+-rw-r--r--   0 dev       (1000) docker-host   (967)       37 2023-02-14 11:45:37.000000 crosslab_soa_client-0.2.3/setup.py
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:15:40.685913 crosslab_soa_client-0.2.3/src/
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:15:40.682580 crosslab_soa_client-0.2.3/src/crosslab/
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:15:40.685913 crosslab_soa_client-0.2.3/src/crosslab/soa_client/
+-rw-r--r--   0 dev       (1000) docker-host   (967)        0 2023-02-14 11:45:37.000000 crosslab_soa_client-0.2.3/src/crosslab/soa_client/__init__.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)     1774 2023-05-19 07:55:53.000000 crosslab_soa_client-0.2.3/src/crosslab/soa_client/connection.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)     9557 2023-05-19 07:55:53.000000 crosslab_soa_client-0.2.3/src/crosslab/soa_client/connection_webrtc.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)     6244 2023-04-26 09:19:14.000000 crosslab_soa_client-0.2.3/src/crosslab/soa_client/device_handler.py
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:15:40.689247 crosslab_soa_client-0.2.3/src/crosslab/soa_client/media/
+-rw-r--r--   0 dev       (1000) docker-host   (967)        0 2023-02-14 11:45:37.000000 crosslab_soa_client-0.2.3/src/crosslab/soa_client/media/__init__.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)      395 2023-02-14 11:45:37.000000 crosslab_soa_client-0.2.3/src/crosslab/soa_client/media/gst_track.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)      557 2023-02-14 11:45:37.000000 crosslab_soa_client-0.2.3/src/crosslab/soa_client/media/udp_track.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)        0 2023-02-14 11:45:37.000000 crosslab_soa_client-0.2.3/src/crosslab/soa_client/message_handling.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)     1077 2023-02-14 11:45:37.000000 crosslab_soa_client-0.2.3/src/crosslab/soa_client/messages.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)        0 2023-02-14 11:45:37.000000 crosslab_soa_client-0.2.3/src/crosslab/soa_client/py.typed
+-rw-r--r--   0 dev       (1000) docker-host   (967)      764 2023-04-26 09:19:14.000000 crosslab_soa_client-0.2.3/src/crosslab/soa_client/service.py
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:15:40.689247 crosslab_soa_client-0.2.3/src/crosslab/soa_client/test_helper/
+-rw-r--r--   0 dev       (1000) docker-host   (967)       81 2023-04-26 09:19:14.000000 crosslab_soa_client-0.2.3/src/crosslab/soa_client/test_helper/__init__.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)     1051 2023-04-26 09:19:14.000000 crosslab_soa_client-0.2.3/src/crosslab/soa_client/test_helper/connection_stub.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)      787 2023-04-26 09:19:14.000000 crosslab_soa_client-0.2.3/src/crosslab/soa_client/test_helper/dummy_track.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)     4298 2023-04-26 09:19:14.000000 crosslab_soa_client-0.2.3/src/crosslab/soa_client/test_helper/service_stub.py
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:15:40.689247 crosslab_soa_client-0.2.3/src/crosslab_soa_client.egg-info/
+-rw-r--r--   0 dev       (1000) docker-host   (967)      331 2023-05-19 08:15:40.000000 crosslab_soa_client-0.2.3/src/crosslab_soa_client.egg-info/PKG-INFO
+-rw-r--r--   0 dev       (1000) docker-host   (967)      981 2023-05-19 08:15:40.000000 crosslab_soa_client-0.2.3/src/crosslab_soa_client.egg-info/SOURCES.txt
+-rw-r--r--   0 dev       (1000) docker-host   (967)        1 2023-05-19 08:15:40.000000 crosslab_soa_client-0.2.3/src/crosslab_soa_client.egg-info/dependency_links.txt
+-rw-r--r--   0 dev       (1000) docker-host   (967)       36 2023-05-19 08:15:40.000000 crosslab_soa_client-0.2.3/src/crosslab_soa_client.egg-info/requires.txt
+-rw-r--r--   0 dev       (1000) docker-host   (967)        9 2023-05-19 08:15:40.000000 crosslab_soa_client-0.2.3/src/crosslab_soa_client.egg-info/top_level.txt
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:15:40.689247 crosslab_soa_client-0.2.3/tests/
+-rw-r--r--   0 dev       (1000) docker-host   (967)     1970 2023-04-26 09:19:14.000000 crosslab_soa_client-0.2.3/tests/test_device_handler.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)     5239 2023-04-26 09:19:14.000000 crosslab_soa_client-0.2.3/tests/test_webrtc_connection.py
```

### Comparing `crosslab_soa_client-0.2.2/README.md` & `crosslab_soa_client-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `crosslab_soa_client-0.2.2/setup.cfg` & `crosslab_soa_client-0.2.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = crosslab_soa_client
-version = 0.2.2
+version = 0.2.3
 author = Johannes Nau
 author_email = johannes.nau@tu-ilmenau.de
 description = The CrossLab SOA Client
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: Other/Proprietary License
 	Operating System :: OS Independent
```

### Comparing `crosslab_soa_client-0.2.2/src/crosslab/soa_client/connection.py` & `crosslab_soa_client-0.2.3/src/crosslab/soa_client/connection.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,20 +43,20 @@
     def close(self):
         self.emit("close")
         self.remove_all_listeners()
 
 
 class Connection(ABC):
     tiebreaker: bool
-    state: Literal["created", "connecting", "connected", "disconnected"]
+    state: Literal["new", "connecting", "connected", "disconnected", "closed", "failed"]
 
     def __init__(self) -> None:
         super().__init__()
         self.tiebreaker = False
-        self.state = "created"
+        self.state = "new"
 
     @abstractmethod
     async def close(self):
         pass
 
     @abstractmethod
     def transmit(
```

### Comparing `crosslab_soa_client-0.2.2/src/crosslab/soa_client/connection_webrtc.py` & `crosslab_soa_client-0.2.3/src/crosslab/soa_client/connection_webrtc.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,17 +47,16 @@
         async def connectionstatechanged():
             print(
                 "connectionstatechanged",
                 self.pc.connectionState,
                 self.pc.iceConnectionState,
                 self.pc.signalingState,
             )
-            if self.pc.connectionState == "connected":
-                self.state = "connected"
-                self.emit("connectionChanged")
+            self.state = self.pc.connectionState
+            self.emit("connectionChanged")
 
         async def datachannel(datachannel):
             channel = self._receivingChannelMap[datachannel.label]
             if channel.channel_type == "DataChannel":
                 dchannel = cast(DataChannel, channel)
 
                 async def upstreamData(data):
@@ -92,14 +91,16 @@
         assert channel is not None  # TODO: handle this
         channel.emit("track", transeiver.receiver.track)
 
     async def close(self):
         await self.pc.close()
         for channel in self._dataChannels:
             channel.close()
+        self.state = "closed"
+        self.emit("connectionChanged")
 
         del self.pc
 
     def _create_label(self, serviceConfig: ServiceConfig, id: str):
         id1 = (
             serviceConfig["serviceId"]
             if self.tiebreaker
```

### Comparing `crosslab_soa_client-0.2.2/src/crosslab/soa_client/device_handler.py` & `crosslab_soa_client-0.2.3/src/crosslab/soa_client/device_handler.py`

 * *Files identical despite different names*

### Comparing `crosslab_soa_client-0.2.2/src/crosslab/soa_client/media/udp_track.py` & `crosslab_soa_client-0.2.3/src/crosslab/soa_client/media/udp_track.py`

 * *Files identical despite different names*

### Comparing `crosslab_soa_client-0.2.2/src/crosslab/soa_client/messages.py` & `crosslab_soa_client-0.2.3/src/crosslab/soa_client/messages.py`

 * *Files identical despite different names*

### Comparing `crosslab_soa_client-0.2.2/src/crosslab/soa_client/service.py` & `crosslab_soa_client-0.2.3/src/crosslab/soa_client/service.py`

 * *Files identical despite different names*

### Comparing `crosslab_soa_client-0.2.2/src/crosslab/soa_client/test_helper/connection_stub.py` & `crosslab_soa_client-0.2.3/src/crosslab/soa_client/test_helper/connection_stub.py`

 * *Files identical despite different names*

### Comparing `crosslab_soa_client-0.2.2/src/crosslab/soa_client/test_helper/dummy_track.py` & `crosslab_soa_client-0.2.3/src/crosslab/soa_client/test_helper/dummy_track.py`

 * *Files identical despite different names*

### Comparing `crosslab_soa_client-0.2.2/src/crosslab/soa_client/test_helper/service_stub.py` & `crosslab_soa_client-0.2.3/src/crosslab/soa_client/test_helper/service_stub.py`

 * *Files identical despite different names*

### Comparing `crosslab_soa_client-0.2.2/src/crosslab_soa_client.egg-info/SOURCES.txt` & `crosslab_soa_client-0.2.3/src/crosslab_soa_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crosslab_soa_client-0.2.2/tests/test_device_handler.py` & `crosslab_soa_client-0.2.3/tests/test_device_handler.py`

 * *Files identical despite different names*

### Comparing `crosslab_soa_client-0.2.2/tests/test_webrtc_connection.py` & `crosslab_soa_client-0.2.3/tests/test_webrtc_connection.py`

 * *Files identical despite different names*

