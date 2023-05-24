# Comparing `tmp/crosslab_soa_service_electrical-0.2.3.tar.gz` & `tmp/crosslab_soa_service_electrical-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crosslab_soa_service_electrical-0.2.3.tar", last modified: Fri May 19 08:17:37 2023, max compression
+gzip compressed data, was "crosslab_soa_service_electrical-0.2.4.tar", last modified: Wed May 24 18:57:11 2023, max compression
```

## Comparing `crosslab_soa_service_electrical-0.2.3.tar` & `crosslab_soa_service_electrical-0.2.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:17:37.823256 crosslab_soa_service_electrical-0.2.3/
--rw-r--r--   0 dev       (1000) docker-host   (967)      355 2023-05-19 08:17:37.823256 crosslab_soa_service_electrical-0.2.3/PKG-INFO
--rw-r--r--   0 dev       (1000) docker-host   (967)       87 2023-02-10 09:58:35.000000 crosslab_soa_service_electrical-0.2.3/pyproject.toml
--rw-r--r--   0 dev       (1000) docker-host   (967)      585 2023-05-19 08:17:37.823256 crosslab_soa_service_electrical-0.2.3/setup.cfg
--rw-r--r--   0 dev       (1000) docker-host   (967)       37 2023-02-10 09:58:35.000000 crosslab_soa_service_electrical-0.2.3/setup.py
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:17:37.813256 crosslab_soa_service_electrical-0.2.3/src/
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:17:37.813256 crosslab_soa_service_electrical-0.2.3/src/crosslab/
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:17:37.813256 crosslab_soa_service_electrical-0.2.3/src/crosslab/soa_services/
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:17:37.816589 crosslab_soa_service_electrical-0.2.3/src/crosslab/soa_services/electrical/
--rw-r--r--   0 dev       (1000) docker-host   (967)      256 2023-02-10 09:58:35.000000 crosslab_soa_service_electrical-0.2.3/src/crosslab/soa_services/electrical/__init__.py
--rw-r--r--   0 dev       (1000) docker-host   (967)     5204 2023-04-26 09:19:14.000000 crosslab_soa_service_electrical-0.2.3/src/crosslab/soa_services/electrical/electrical_connection_service.py
--rw-r--r--   0 dev       (1000) docker-host   (967)      745 2023-02-10 10:19:30.000000 crosslab_soa_service_electrical-0.2.3/src/crosslab/soa_services/electrical/messages.py
--rw-r--r--   0 dev       (1000) docker-host   (967)        0 2023-02-10 09:58:35.000000 crosslab_soa_service_electrical-0.2.3/src/crosslab/soa_services/electrical/py.typed
--rw-r--r--   0 dev       (1000) docker-host   (967)      614 2023-04-12 09:26:55.000000 crosslab_soa_service_electrical-0.2.3/src/crosslab/soa_services/electrical/signal_interface.py
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:17:37.819923 crosslab_soa_service_electrical-0.2.3/src/crosslab/soa_services/electrical/signal_interfaces/
--rw-r--r--   0 dev       (1000) docker-host   (967)        0 2023-02-10 09:58:35.000000 crosslab_soa_service_electrical-0.2.3/src/crosslab/soa_services/electrical/signal_interfaces/__init__.py
--rw-r--r--   0 dev       (1000) docker-host   (967)     2876 2023-04-26 09:19:14.000000 crosslab_soa_service_electrical-0.2.3/src/crosslab/soa_services/electrical/signal_interfaces/gpio.py
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:17:37.819923 crosslab_soa_service_electrical-0.2.3/src/crosslab_soa_service_electrical.egg-info/
--rw-r--r--   0 dev       (1000) docker-host   (967)      355 2023-05-19 08:17:37.000000 crosslab_soa_service_electrical-0.2.3/src/crosslab_soa_service_electrical.egg-info/PKG-INFO
--rw-r--r--   0 dev       (1000) docker-host   (967)      770 2023-05-19 08:17:37.000000 crosslab_soa_service_electrical-0.2.3/src/crosslab_soa_service_electrical.egg-info/SOURCES.txt
--rw-r--r--   0 dev       (1000) docker-host   (967)        1 2023-05-19 08:17:37.000000 crosslab_soa_service_electrical-0.2.3/src/crosslab_soa_service_electrical.egg-info/dependency_links.txt
--rw-r--r--   0 dev       (1000) docker-host   (967)       25 2023-05-19 08:17:37.000000 crosslab_soa_service_electrical-0.2.3/src/crosslab_soa_service_electrical.egg-info/requires.txt
--rw-r--r--   0 dev       (1000) docker-host   (967)        9 2023-05-19 08:17:37.000000 crosslab_soa_service_electrical-0.2.3/src/crosslab_soa_service_electrical.egg-info/top_level.txt
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:17:37.823256 crosslab_soa_service_electrical-0.2.3/tests/
--rw-r--r--   0 dev       (1000) docker-host   (967)     4076 2023-04-26 09:19:14.000000 crosslab_soa_service_electrical-0.2.3/tests/test_gpio.py
--rw-r--r--   0 dev       (1000) docker-host   (967)      810 2023-04-26 09:19:14.000000 crosslab_soa_service_electrical-0.2.3/tests/test_standard.py
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-24 18:57:11.510491 crosslab_soa_service_electrical-0.2.4/
+-rw-r--r--   0 dev       (1000) docker-host   (967)      355 2023-05-24 18:57:11.510491 crosslab_soa_service_electrical-0.2.4/PKG-INFO
+-rw-r--r--   0 dev       (1000) docker-host   (967)       87 2023-01-10 14:53:51.000000 crosslab_soa_service_electrical-0.2.4/pyproject.toml
+-rw-r--r--   0 dev       (1000) docker-host   (967)      585 2023-05-24 18:57:11.510491 crosslab_soa_service_electrical-0.2.4/setup.cfg
+-rw-r--r--   0 dev       (1000) docker-host   (967)       37 2023-01-10 14:52:40.000000 crosslab_soa_service_electrical-0.2.4/setup.py
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-24 18:57:11.507158 crosslab_soa_service_electrical-0.2.4/src/
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-24 18:57:11.507158 crosslab_soa_service_electrical-0.2.4/src/crosslab/
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-24 18:57:11.507158 crosslab_soa_service_electrical-0.2.4/src/crosslab/soa_services/
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-24 18:57:11.507158 crosslab_soa_service_electrical-0.2.4/src/crosslab/soa_services/electrical/
+-rw-r--r--   0 dev       (1000) docker-host   (967)      256 2022-12-20 17:27:48.000000 crosslab_soa_service_electrical-0.2.4/src/crosslab/soa_services/electrical/__init__.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)     5236 2023-05-22 07:55:59.000000 crosslab_soa_service_electrical-0.2.4/src/crosslab/soa_services/electrical/electrical_connection_service.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)      745 2023-04-23 10:11:43.000000 crosslab_soa_service_electrical-0.2.4/src/crosslab/soa_services/electrical/messages.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)        0 2023-01-16 16:15:44.000000 crosslab_soa_service_electrical-0.2.4/src/crosslab/soa_services/electrical/py.typed
+-rw-r--r--   0 dev       (1000) docker-host   (967)      614 2023-02-13 11:08:58.000000 crosslab_soa_service_electrical-0.2.4/src/crosslab/soa_services/electrical/signal_interface.py
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-24 18:57:11.507158 crosslab_soa_service_electrical-0.2.4/src/crosslab/soa_services/electrical/signal_interfaces/
+-rw-r--r--   0 dev       (1000) docker-host   (967)        0 2022-12-20 16:55:25.000000 crosslab_soa_service_electrical-0.2.4/src/crosslab/soa_services/electrical/signal_interfaces/__init__.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)     3001 2023-05-23 12:48:52.000000 crosslab_soa_service_electrical-0.2.4/src/crosslab/soa_services/electrical/signal_interfaces/gpio.py
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-24 18:57:11.510491 crosslab_soa_service_electrical-0.2.4/src/crosslab_soa_service_electrical.egg-info/
+-rw-r--r--   0 dev       (1000) docker-host   (967)      355 2023-05-24 18:57:11.000000 crosslab_soa_service_electrical-0.2.4/src/crosslab_soa_service_electrical.egg-info/PKG-INFO
+-rw-r--r--   0 dev       (1000) docker-host   (967)      770 2023-05-24 18:57:11.000000 crosslab_soa_service_electrical-0.2.4/src/crosslab_soa_service_electrical.egg-info/SOURCES.txt
+-rw-r--r--   0 dev       (1000) docker-host   (967)        1 2023-05-24 18:57:11.000000 crosslab_soa_service_electrical-0.2.4/src/crosslab_soa_service_electrical.egg-info/dependency_links.txt
+-rw-r--r--   0 dev       (1000) docker-host   (967)       25 2023-05-24 18:57:11.000000 crosslab_soa_service_electrical-0.2.4/src/crosslab_soa_service_electrical.egg-info/requires.txt
+-rw-r--r--   0 dev       (1000) docker-host   (967)        9 2023-05-24 18:57:11.000000 crosslab_soa_service_electrical-0.2.4/src/crosslab_soa_service_electrical.egg-info/top_level.txt
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-24 18:57:11.510491 crosslab_soa_service_electrical-0.2.4/tests/
+-rw-r--r--   0 dev       (1000) docker-host   (967)     4098 2023-05-23 20:29:08.000000 crosslab_soa_service_electrical-0.2.4/tests/test_gpio.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)      810 2023-04-20 09:47:47.000000 crosslab_soa_service_electrical-0.2.4/tests/test_standard.py
```

### Comparing `crosslab_soa_service_electrical-0.2.3/setup.cfg` & `crosslab_soa_service_electrical-0.2.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = crosslab_soa_service_electrical
-version = 0.2.3
+version = 0.2.4
 author = Johannes Nau
 author_email = johannes.nau@tu-ilmenau.de
 description = The CrossLab SOA Electrical Service
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: Other/Proprietary License
 	Operating System :: OS Independent
```

### Comparing `crosslab_soa_service_electrical-0.2.3/src/crosslab/soa_services/electrical/electrical_connection_service.py` & `crosslab_soa_service_electrical-0.2.4/src/crosslab/soa_services/electrical/electrical_connection_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 @dataclass
 class ConnectionMeta:
     interfaces: Set[SignalInterface]
     interface_meta: Dict[SignalInterface, SignalInterfaceMeta]
 
 
 class ElectricalConnectionService(Service, AsyncIOEventEmitter):
-    service_type = "goldi/electrical"
+    service_type = "http://api.goldi-labs.de/serviceTypes/electrical"
     service_id: str
     _interfaces: Dict[str, SignalInterface]
     _interfaces_constructors: Dict[str, ConstructableSignalInterface]
     _interface_id_ref_counter: Dict[str, int]
     _connection_meta: Dict[Connection, ConnectionMeta]
 
     def __init__(self, serviceId: str):
```

### Comparing `crosslab_soa_service_electrical-0.2.3/src/crosslab/soa_services/electrical/messages.py` & `crosslab_soa_service_electrical-0.2.4/src/crosslab/soa_services/electrical/messages.py`

 * *Files identical despite different names*

### Comparing `crosslab_soa_service_electrical-0.2.3/src/crosslab/soa_services/electrical/signal_interface.py` & `crosslab_soa_service_electrical-0.2.4/src/crosslab/soa_services/electrical/signal_interface.py`

 * *Files identical despite different names*

### Comparing `crosslab_soa_service_electrical-0.2.3/src/crosslab/soa_services/electrical/signal_interfaces/gpio.py` & `crosslab_soa_service_electrical-0.2.4/src/crosslab/soa_services/electrical/signal_interfaces/gpio.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass
-from typing import Dict, List, Optional
+from typing import Dict, List, Literal, Optional
 
 from crosslab.soa_services.electrical import (
     ConstructableSignalInterface,
     SignalInterface,
 )
 from crosslab.soa_services.electrical.messages import (
     GPIOInterfaceConfig,
@@ -82,15 +82,16 @@
             self.signalState = newState
             self.emit("signalChange", data)
 
 
 class ConstractableGPIOInterface(ConstructableSignalInterface):
     interfaceType = "gpio"
 
-    def __init__(self, gpios: List[str]):
+    def __init__(self, gpios: List[str], direction: Literal["in", "out", "inout"] = "inout"):
         self.gpios = gpios
+        self.direction = direction
 
     def getDescription(self):
-        return {"availableSignals": {"gpio": self.gpios}}
+        return {"availableSignals": {"gpio": self.gpios}, "direction": self.direction}
 
     def create(self, interfaceConfig):
         return GPIOInterface(interfaceConfig)
```

### Comparing `crosslab_soa_service_electrical-0.2.3/src/crosslab_soa_service_electrical.egg-info/SOURCES.txt` & `crosslab_soa_service_electrical-0.2.4/src/crosslab_soa_service_electrical.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crosslab_soa_service_electrical-0.2.3/tests/test_gpio.py` & `crosslab_soa_service_electrical-0.2.4/tests/test_gpio.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     ConstractableGPIOInterface,
     GPIOInterface,
 )
 
 
 def test_gpio_meta():
     gci = ConstractableGPIOInterface(["S1", "S2"])
-    assert gci.getDescription() == {"availableSignals": {"gpio": ["S1", "S2"]}}
+    assert gci.getDescription() == {"availableSignals": {"gpio": ["S1", "S2"]}, "direction": "inout"}
 
 
 @pytest.mark.parametrize("tiebreaker", [True, False])
 def test_gpio_interface_creation(tiebreaker):
     con = ConnectionStub(tiebreaker)
     ecs = ElectricalConnectionService("test")
     gci = ConstractableGPIOInterface(["S1", "S2"])
```

### Comparing `crosslab_soa_service_electrical-0.2.3/tests/test_standard.py` & `crosslab_soa_service_electrical-0.2.4/tests/test_standard.py`

 * *Files identical despite different names*

