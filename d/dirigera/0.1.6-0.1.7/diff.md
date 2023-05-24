# Comparing `tmp/dirigera-0.1.6.tar.gz` & `tmp/dirigera-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dirigera-0.1.6.tar", last modified: Thu May 11 14:49:16 2023, max compression
+gzip compressed data, was "dirigera-0.1.7.tar", last modified: Wed May 24 15:14:53 2023, max compression
```

## Comparing `dirigera-0.1.6.tar` & `dirigera-0.1.7.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:49:16.779026 dirigera-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-11 14:49:03.000000 dirigera-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-05-11 14:49:16.779026 dirigera-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-05-11 14:49:03.000000 dirigera-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-11 14:49:03.000000 dirigera-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 14:49:16.779026 dirigera-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 14:49:03.000000 dirigera-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:49:16.775026 dirigera-0.1.6/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 14:49:03.000000 dirigera-0.1.6/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:49:16.775026 dirigera-0.1.6/src/dirigera/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-11 14:49:03.000000 dirigera-0.1.6/src/dirigera/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:49:16.775026 dirigera-0.1.6/src/dirigera/devices/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 14:49:03.000000 dirigera-0.1.6/src/dirigera/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-05-11 14:49:03.000000 dirigera-0.1.6/src/dirigera/devices/blinds.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-11 14:49:03.000000 dirigera-0.1.6/src/dirigera/devices/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-05-11 14:49:03.000000 dirigera-0.1.6/src/dirigera/devices/environment_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-05-11 14:49:03.000000 dirigera-0.1.6/src/dirigera/devices/light.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-11 14:49:03.000000 dirigera-0.1.6/src/dirigera/devices/open_close_sensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:49:16.779026 dirigera-0.1.6/src/dirigera/hub/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 14:49:03.000000 dirigera-0.1.6/src/dirigera/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-11 14:49:03.000000 dirigera-0.1.6/src/dirigera/hub/abstract_smart_home_hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-11 14:49:03.000000 dirigera-0.1.6/src/dirigera/hub/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-05-11 14:49:03.000000 dirigera-0.1.6/src/dirigera/hub/hub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:49:16.775026 dirigera-0.1.6/src/dirigera.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-05-11 14:49:16.000000 dirigera-0.1.6/src/dirigera.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-11 14:49:16.000000 dirigera-0.1.6/src/dirigera.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 14:49:16.000000 dirigera-0.1.6/src/dirigera.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-11 14:49:16.000000 dirigera-0.1.6/src/dirigera.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-11 14:49:16.000000 dirigera-0.1.6/src/dirigera.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-11 14:49:16.000000 dirigera-0.1.6/src/dirigera.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:49:16.779026 dirigera-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-05-11 14:49:03.000000 dirigera-0.1.6/tests/test_blinds.py
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-05-11 14:49:03.000000 dirigera-0.1.6/tests/test_environment_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-05-11 14:49:03.000000 dirigera-0.1.6/tests/test_light.py
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-11 14:49:03.000000 dirigera-0.1.6/tests/test_open_close_sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:14:53.422249 dirigera-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-24 15:14:44.000000 dirigera-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9429 2023-05-24 15:14:53.422249 dirigera-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-05-24 15:14:44.000000 dirigera-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-24 15:14:44.000000 dirigera-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 15:14:53.422249 dirigera-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 15:14:44.000000 dirigera-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:14:53.418249 dirigera-0.1.7/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:14:44.000000 dirigera-0.1.7/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:14:53.418249 dirigera-0.1.7/src/dirigera/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-24 15:14:44.000000 dirigera-0.1.7/src/dirigera/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:14:53.422249 dirigera-0.1.7/src/dirigera/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:14:44.000000 dirigera-0.1.7/src/dirigera/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-05-24 15:14:44.000000 dirigera-0.1.7/src/dirigera/devices/blinds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-24 15:14:44.000000 dirigera-0.1.7/src/dirigera/devices/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-05-24 15:14:44.000000 dirigera-0.1.7/src/dirigera/devices/environment_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-05-24 15:14:44.000000 dirigera-0.1.7/src/dirigera/devices/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-24 15:14:44.000000 dirigera-0.1.7/src/dirigera/devices/open_close_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-05-24 15:14:44.000000 dirigera-0.1.7/src/dirigera/devices/outlet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:14:53.422249 dirigera-0.1.7/src/dirigera/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:14:44.000000 dirigera-0.1.7/src/dirigera/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-24 15:14:44.000000 dirigera-0.1.7/src/dirigera/hub/abstract_smart_home_hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-24 15:14:44.000000 dirigera-0.1.7/src/dirigera/hub/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-05-24 15:14:44.000000 dirigera-0.1.7/src/dirigera/hub/hub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:14:53.418249 dirigera-0.1.7/src/dirigera.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9429 2023-05-24 15:14:53.000000 dirigera-0.1.7/src/dirigera.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-24 15:14:53.000000 dirigera-0.1.7/src/dirigera.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:14:53.000000 dirigera-0.1.7/src/dirigera.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-24 15:14:53.000000 dirigera-0.1.7/src/dirigera.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-24 15:14:53.000000 dirigera-0.1.7/src/dirigera.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-24 15:14:53.000000 dirigera-0.1.7/src/dirigera.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:14:53.422249 dirigera-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-05-24 15:14:44.000000 dirigera-0.1.7/tests/test_blinds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-05-24 15:14:44.000000 dirigera-0.1.7/tests/test_environment_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11554 2023-05-24 15:14:44.000000 dirigera-0.1.7/tests/test_light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-24 15:14:44.000000 dirigera-0.1.7/tests/test_open_close_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-05-24 15:14:44.000000 dirigera-0.1.7/tests/test_outlet.py
```

### Comparing `dirigera-0.1.6/LICENSE` & `dirigera-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.6/PKG-INFO` & `dirigera-0.1.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dirigera
-Version: 0.1.6
+Version: 0.1.7
 Summary: An unofficial Python client for controlling the IKEA Dirigera Smart Home Hub
 Author-email: Leggin <legginsun@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Leggin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -44,14 +44,15 @@
 ![Test](https://github.com/Leggin/dirigera/actions/workflows/tests.yml/badge.svg)
 ![Pypi](https://img.shields.io/pypi/v/dirigera)
 [![Downloads](https://static.pepy.tech/badge/dirigera/month)](https://pepy.tech/project/dirigera)
 ![Downloads](https://img.shields.io/pypi/pyversions/dirigera)
 
 This repository provides an unofficial Python client for controlling the IKEA Dirigera Smart Home Hub. Current features:
  - [light control](#controlling-lights)
+ - [outlet control](#controlling-outlets)
  - [blinds control](#controlling-blinds)
  - [environment sensor](#environment-sensor) (tested with VINDSTYRKA)
  - [event listener](#event-listener) for hub events
 
 Support for other features will be added in the future and your input in form of issues and PRs is greatly appreciated.
 
 ## Installation
@@ -135,14 +136,45 @@
 light.set_color_temperature(color_temp=3000)
 
 light.set_light_color(hue=128, saturation=0.5)
 
 light.set_startup_behaviour(behaviour=StartupEnum.START_OFF)
 ```
 
+## [Controlling Outlets](./src/dirigera/devices/outlet.py)
+
+To get information about the available outlets, you can use the `get_outlets()` method:
+
+```python
+outlets = dirigera_hub.get_outlets()
+```
+
+The outlet object has the following attributes:
+
+```python
+device_id: str
+is_reachable: bool
+custom_name: str
+is_on: bool
+startup_on_off: StartupEnum | None
+room_id: str
+room_name: str
+can_receive: List[str]  # list of all available commands ["customName", "isOn", "lightLevel", ...]
+```
+
+Available methods for outlet are:
+
+```python
+outlet.set_name(name="kitchen socket 1")
+
+outlet.set_on(outlet_on=True)
+
+outlet.set_startup_behaviour(behaviour=StartupEnum.START_OFF)
+```
+
 ## [Controlling Blinds](./src/dirigera/devices/blinds.py)
 
 To get information about the available blinds, you can use the `get_blinds()` method:
 
 ```python
 blinds = dirigera_hub.get_blinds()
 ```
```

### Comparing `dirigera-0.1.6/README.md` & `dirigera-0.1.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 ![Test](https://github.com/Leggin/dirigera/actions/workflows/tests.yml/badge.svg)
 ![Pypi](https://img.shields.io/pypi/v/dirigera)
 [![Downloads](https://static.pepy.tech/badge/dirigera/month)](https://pepy.tech/project/dirigera)
 ![Downloads](https://img.shields.io/pypi/pyversions/dirigera)
 
 This repository provides an unofficial Python client for controlling the IKEA Dirigera Smart Home Hub. Current features:
  - [light control](#controlling-lights)
+ - [outlet control](#controlling-outlets)
  - [blinds control](#controlling-blinds)
  - [environment sensor](#environment-sensor) (tested with VINDSTYRKA)
  - [event listener](#event-listener) for hub events
 
 Support for other features will be added in the future and your input in form of issues and PRs is greatly appreciated.
 
 ## Installation
@@ -93,14 +94,45 @@
 light.set_color_temperature(color_temp=3000)
 
 light.set_light_color(hue=128, saturation=0.5)
 
 light.set_startup_behaviour(behaviour=StartupEnum.START_OFF)
 ```
 
+## [Controlling Outlets](./src/dirigera/devices/outlet.py)
+
+To get information about the available outlets, you can use the `get_outlets()` method:
+
+```python
+outlets = dirigera_hub.get_outlets()
+```
+
+The outlet object has the following attributes:
+
+```python
+device_id: str
+is_reachable: bool
+custom_name: str
+is_on: bool
+startup_on_off: StartupEnum | None
+room_id: str
+room_name: str
+can_receive: List[str]  # list of all available commands ["customName", "isOn", "lightLevel", ...]
+```
+
+Available methods for outlet are:
+
+```python
+outlet.set_name(name="kitchen socket 1")
+
+outlet.set_on(outlet_on=True)
+
+outlet.set_startup_behaviour(behaviour=StartupEnum.START_OFF)
+```
+
 ## [Controlling Blinds](./src/dirigera/devices/blinds.py)
 
 To get information about the available blinds, you can use the `get_blinds()` method:
 
 ```python
 blinds = dirigera_hub.get_blinds()
 ```
@@ -189,8 +221,8 @@
 
 Contributions are welcome! If you have an idea for a new feature or a bug fix, please post and issue or submit a pull request.
 
 ## License
 
 The MIT License (MIT)
 
-Copyright (c) 2023 Leggin
+Copyright (c) 2023 Leggin
```

### Comparing `dirigera-0.1.6/pyproject.toml` & `dirigera-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
    "setuptools",
    "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dirigera"
-version = "0.1.6"
+version = "0.1.7"
 description = "An unofficial Python client for controlling the IKEA Dirigera Smart Home Hub"
 readme = "README.md"
 authors = [{ name = "Leggin", email = "legginsun@gmail.com" }]
 license = { file = "LICENSE" }
 keywords = ["python", "iot", "smarthome", "hub", "lighting", "ikea", "tradfri", "dirigera"]
 dependencies = [
     "requests >= 2.22.0",
```

### Comparing `dirigera-0.1.6/src/dirigera/devices/blinds.py` & `dirigera-0.1.7/src/dirigera/devices/blinds.py`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.6/src/dirigera/devices/environment_sensor.py` & `dirigera-0.1.7/src/dirigera/devices/environment_sensor.py`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.6/src/dirigera/devices/light.py` & `dirigera-0.1.7/src/dirigera/devices/light.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,15 @@
 from dataclasses import dataclass
-from enum import Enum
 from typing import Any, Optional, Dict
 
-from .device import Device
+from .device import Device, StartupEnum
 
 from ..hub.abstract_smart_home_hub import AbstractSmartHomeHub
 
 
-class StartupEnum(Enum):
-    START_ON = "startOn"
-    START_OFF = "startOff"
-    START_PREVIOUS = "startPrevious"
-    START_TOGGLE = "startToggle"
-
-
 @dataclass
 class Light(Device):
     dirigera_client: AbstractSmartHomeHub
     is_reachable: bool
     is_on: bool
     startup_on_off: Optional[StartupEnum]
     light_level: Optional[int]
@@ -26,29 +18,39 @@
     color_temp_max: Optional[int]
     color_hue: Optional[int]
     color_saturation: Optional[float]
 
     def refresh(self) -> None:
         data = self.dirigera_client.get(route=f"/devices/{self.device_id}")
         attributes: Dict[str, Any] = data["attributes"]
+
+        if "startupOnOff" in attributes:
+            startup_on_off = StartupEnum(attributes.get("startupOnOff"))
+        else:
+            startup_on_off = None
+
         self.device_id = data["id"]
         self.is_reachable = data["isReachable"]
         self.custom_name = attributes["customName"]
         self.is_on = attributes["isOn"]
-        self.startup_on_off = attributes.get("startupOnOff")
+        self.startup_on_off = startup_on_off
         self.light_level = attributes.get("lightLevel")
         self.color_temp = attributes.get("colorTemperature")
         self.color_temp_min = attributes.get("colorTemperatureMin")
         self.color_temp_max = attributes.get("colorTemperatureMax")
         self.color_hue = attributes.get("colorHue")
         self.color_saturation = attributes.get("colorSaturation")
         self.firmware_version = attributes.get("firmwareVersion")
+        self.hardware_version = attributes.get("hardwareVersion")
         self.room_id = data["room"]["id"]
         self.room_name = data["room"]["name"]
         self.can_receive = data["capabilities"]["canReceive"]
+        self.model = attributes.get("model")
+        self.manufacturer=attributes.get("manufacturer")
+        self.serial_number=attributes.get("serialNumber")
 
     def set_name(self, name: str) -> None:
         if "customName" not in self.can_receive:
             raise AssertionError("This lamp does not support the swith-off function")
 
         data = [{"attributes": {"customName": name}}]
         self.dirigera_client.patch(route=f"/devices/{self.device_id}", data=data)
@@ -110,29 +112,34 @@
         """
         Sets the behaviour of the lamp in case of a power outage.
         When set to START_ON the lamp will turn on once the power is back.
         When set to START_OFF the lamp will stay off once the power is back.
         When set to START_PREVIOUS the lamp will resume its state at power outage.
         When set to START_TOGGLE, a sequence of power-off -> power-on, will toggle the lamp state
         """
-        data = [{"attributes": {"startupOnOff": behaviour}}]
+        data = [{"attributes": {"startupOnOff": behaviour.value}}]
         self.dirigera_client.patch(route=f"/devices/{self.device_id}", data=data)
         self.startup_on_off = behaviour
 
 
 def dict_to_light(data: Dict[str, Any], dirigera_client: AbstractSmartHomeHub):
     attributes: Dict[str, Any] = data["attributes"]
 
+    if "startupOnOff" in attributes:
+        startup_on_off = StartupEnum(attributes.get("startupOnOff"))
+    else:
+        startup_on_off = None
+
     return Light(
         dirigera_client=dirigera_client,
         device_id=data["id"],
         is_reachable=data["isReachable"],
         custom_name=attributes["customName"],
         is_on=attributes["isOn"],
-        startup_on_off=attributes.get("startupOnOff"),
+        startup_on_off=startup_on_off,
         light_level=attributes.get("lightLevel"),
         color_temp=attributes.get("colorTemperature"),
         color_temp_min=attributes.get("colorTemperatureMin"),
         color_temp_max=attributes.get("colorTemperatureMax"),
         color_hue=attributes.get("colorHue"),
         color_saturation=attributes.get("colorSaturation"),
         can_receive=data["capabilities"]["canReceive"],
```

### Comparing `dirigera-0.1.6/src/dirigera/devices/open_close_sensor.py` & `dirigera-0.1.7/src/dirigera/devices/open_close_sensor.py`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.6/src/dirigera/hub/abstract_smart_home_hub.py` & `dirigera-0.1.7/src/dirigera/hub/abstract_smart_home_hub.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,13 +12,15 @@
         raise NotImplementedError
 
 
 class FakeDirigeraHub(AbstractSmartHomeHub):
     def __init__(self) -> None:
         self.patch_actions: List = []
         self.get_actions: List = []
+        self.get_action_replys: Dict = {}
 
     def patch(self, route: str, data: Dict[str, Any]) -> Dict[str, Any]:
         self.patch_actions.append({"route": route, "data": data})
 
     def get(self, route: str) -> Dict[str, Any]:
         self.get_actions.append({"route": route})
+        return self.get_action_replys[route]
```

### Comparing `dirigera-0.1.6/src/dirigera/hub/auth.py` & `dirigera-0.1.7/src/dirigera/hub/auth.py`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.6/src/dirigera/hub/hub.py` & `dirigera-0.1.7/src/dirigera/hub/hub.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import requests
 import websocket
 from urllib3.exceptions import InsecureRequestWarning
 
 from .abstract_smart_home_hub import AbstractSmartHomeHub
 from ..devices.light import Light, dict_to_light
 from ..devices.blinds import Blind, dict_to_blind
+from ..devices.outlet import Outlet, dict_to_outlet
 from ..devices.environment_sensor import EnvironmentSensor, dict_to_environment_sensor
 from ..devices.open_close_sensor import OpenCloseSensor, dict_to_open_close_sensor
 
 requests.packages.urllib3.disable_warnings(  # pylint: disable=no-member
     category=InsecureRequestWarning
 )
 
@@ -100,14 +101,22 @@
         """
         lights = self.get_lights()
         lights = list(filter(lambda x: x.custom_name == lamp_name, lights))
         if len(lights) == 0:
             raise AssertionError(f"No light found with name {lamp_name}")
         return lights[0]
 
+    def get_outlets(self) -> List[Outlet]:
+        """
+        Fetches all outlets registered in the Hub
+        """
+        devices = self.get("/devices")
+        outlets = list(filter(lambda x: x["type"] == "outlet", devices))
+        return [dict_to_outlet(outlet, self) for outlet in outlets]
+
     def get_environment_sensors(self) -> List[EnvironmentSensor]:
         """
         Fetches all environment sensors registered in the Hub
         """
         devices = self.get("/devices")
         sensors = list(
             filter(lambda x: x["deviceType"] == "environmentSensor", devices)
```

### Comparing `dirigera-0.1.6/src/dirigera.egg-info/PKG-INFO` & `dirigera-0.1.7/src/dirigera.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dirigera
-Version: 0.1.6
+Version: 0.1.7
 Summary: An unofficial Python client for controlling the IKEA Dirigera Smart Home Hub
 Author-email: Leggin <legginsun@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Leggin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -44,14 +44,15 @@
 ![Test](https://github.com/Leggin/dirigera/actions/workflows/tests.yml/badge.svg)
 ![Pypi](https://img.shields.io/pypi/v/dirigera)
 [![Downloads](https://static.pepy.tech/badge/dirigera/month)](https://pepy.tech/project/dirigera)
 ![Downloads](https://img.shields.io/pypi/pyversions/dirigera)
 
 This repository provides an unofficial Python client for controlling the IKEA Dirigera Smart Home Hub. Current features:
  - [light control](#controlling-lights)
+ - [outlet control](#controlling-outlets)
  - [blinds control](#controlling-blinds)
  - [environment sensor](#environment-sensor) (tested with VINDSTYRKA)
  - [event listener](#event-listener) for hub events
 
 Support for other features will be added in the future and your input in form of issues and PRs is greatly appreciated.
 
 ## Installation
@@ -135,14 +136,45 @@
 light.set_color_temperature(color_temp=3000)
 
 light.set_light_color(hue=128, saturation=0.5)
 
 light.set_startup_behaviour(behaviour=StartupEnum.START_OFF)
 ```
 
+## [Controlling Outlets](./src/dirigera/devices/outlet.py)
+
+To get information about the available outlets, you can use the `get_outlets()` method:
+
+```python
+outlets = dirigera_hub.get_outlets()
+```
+
+The outlet object has the following attributes:
+
+```python
+device_id: str
+is_reachable: bool
+custom_name: str
+is_on: bool
+startup_on_off: StartupEnum | None
+room_id: str
+room_name: str
+can_receive: List[str]  # list of all available commands ["customName", "isOn", "lightLevel", ...]
+```
+
+Available methods for outlet are:
+
+```python
+outlet.set_name(name="kitchen socket 1")
+
+outlet.set_on(outlet_on=True)
+
+outlet.set_startup_behaviour(behaviour=StartupEnum.START_OFF)
+```
+
 ## [Controlling Blinds](./src/dirigera/devices/blinds.py)
 
 To get information about the available blinds, you can use the `get_blinds()` method:
 
 ```python
 blinds = dirigera_hub.get_blinds()
 ```
```

### Comparing `dirigera-0.1.6/src/dirigera.egg-info/SOURCES.txt` & `dirigera-0.1.7/src/dirigera.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 src/dirigera.egg-info/top_level.txt
 src/dirigera/devices/__init__.py
 src/dirigera/devices/blinds.py
 src/dirigera/devices/device.py
 src/dirigera/devices/environment_sensor.py
 src/dirigera/devices/light.py
 src/dirigera/devices/open_close_sensor.py
+src/dirigera/devices/outlet.py
 src/dirigera/hub/__init__.py
 src/dirigera/hub/abstract_smart_home_hub.py
 src/dirigera/hub/auth.py
 src/dirigera/hub/hub.py
 tests/test_blinds.py
 tests/test_environment_sensor.py
 tests/test_light.py
-tests/test_open_close_sensor.py
+tests/test_open_close_sensor.py
+tests/test_outlet.py
```

### Comparing `dirigera-0.1.6/tests/test_blinds.py` & `dirigera-0.1.7/tests/test_blinds.py`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.6/tests/test_environment_sensor.py` & `dirigera-0.1.7/tests/test_environment_sensor.py`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.6/tests/test_light.py` & `dirigera-0.1.7/tests/test_light.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pytest
 from src.dirigera.hub.abstract_smart_home_hub import FakeDirigeraHub
 from src.dirigera.devices.light import dict_to_light
-from src.dirigera.devices.light import Light, StartupEnum
+from src.dirigera.devices.light import Light
+from src.dirigera.devices.device import StartupEnum
 
 
 @pytest.fixture(name="fake_client")
 def fixture_fake_client():
     return FakeDirigeraHub()
 
 
@@ -38,14 +39,66 @@
             "colorTemperature",
             "colorHue",
             "colorSaturation",
         ],
     )
 
 
+def test_refresh(fake_light: Light, fake_client: FakeDirigeraHub):
+    data = {
+        "id": "1237-343-2dfa",
+        "type": "light",
+        "deviceType": "light",
+        "isReachable": True,
+        "attributes": {
+            "customName": "Light 2",
+            "model": "TRADFRI bulb E27 WW 806lm",
+            "manufacturer": "IKEA of Sweden",
+            "serialNumber": "84",
+            "firmwareVersion": "2.3.093",
+            "hardwareVersion": "2",
+            "isOn": True,
+            "lightLevel": 50,
+            "colorTemperature": 2710,
+            "colorTemperatureMin": 4000,
+            "colorTemperatureMax": 2202,
+            "colorMode": "temperature",
+        },
+        "capabilities": {
+            "canSend": [],
+            "canReceive": ["customName", "isOn", "lightLevel"],
+        },
+        "room": {
+            "id": "19aa77553369",
+            "name": "Living room",
+        },
+    }
+    fake_client.get_action_replys[f"/devices/{fake_light.device_id}"] = data
+    fake_light.refresh()
+    fake_client.get_actions.pop()
+    assert fake_light.dirigera_client == fake_client
+    assert fake_light.device_id == data["id"]
+    assert fake_light.is_reachable == data["isReachable"]
+    assert fake_light.custom_name == data["attributes"]["customName"]
+    assert fake_light.is_on == data["attributes"]["isOn"]
+    assert fake_light.startup_on_off is None
+    assert fake_light.light_level == data["attributes"]["lightLevel"]
+    assert fake_light.color_temp == data["attributes"]["colorTemperature"]
+    assert fake_light.color_temp_min == data["attributes"]["colorTemperatureMin"]
+    assert fake_light.color_temp_max == data["attributes"]["colorTemperatureMax"]
+    assert fake_light.can_receive == data["capabilities"]["canReceive"]
+    assert fake_light.room_id == data["room"]["id"]
+    assert fake_light.room_name == data["room"]["name"]
+    assert fake_light.firmware_version == data["attributes"]["firmwareVersion"]
+    assert fake_light.hardware_version == data["attributes"]["hardwareVersion"]
+    assert fake_light.model == data["attributes"]["model"]
+    assert fake_light.manufacturer == data["attributes"]["manufacturer"]
+    assert fake_light.serial_number == data["attributes"]["serialNumber"]
+
+
 def test_set_name(fake_light: Light, fake_client: FakeDirigeraHub):
     new_name = "stadtlampefluss"
     fake_light.set_name(new_name)
     action = fake_client.patch_actions.pop()
     assert action["route"] == f"/devices/{fake_light.device_id}"
     assert action["data"] == [{"attributes": {"customName": new_name}}]
     assert fake_light.custom_name == new_name
@@ -101,58 +154,59 @@
 def test_set_startup_behaviour_off(
     fake_light: Light, fake_client: FakeDirigeraHub
 ) -> None:
     behaviour = StartupEnum.START_OFF
     fake_light.set_startup_behaviour(behaviour)
     action = fake_client.patch_actions.pop()
     assert action["route"] == f"/devices/{fake_light.device_id}"
-    assert action["data"] == [{"attributes": {"startupOnOff": behaviour}}]
+    assert action["data"] == [{"attributes": {"startupOnOff": behaviour.value}}]
     assert fake_light.startup_on_off == behaviour
 
 
 def test_set_startup_behaviour_on(
     fake_light: Light, fake_client: FakeDirigeraHub
 ) -> None:
     behaviour = StartupEnum.START_ON
     fake_light.set_startup_behaviour(behaviour)
     action = fake_client.patch_actions.pop()
     assert action["route"] == f"/devices/{fake_light.device_id}"
-    assert action["data"] == [{"attributes": {"startupOnOff": behaviour}}]
+    assert action["data"] == [{"attributes": {"startupOnOff": behaviour.value}}]
     assert fake_light.startup_on_off == behaviour
 
 def test_set_startup_behaviour_previous(
     fake_light: Light, fake_client: FakeDirigeraHub
 ) -> None:
     behaviour = StartupEnum.START_PREVIOUS
     fake_light.set_startup_behaviour(behaviour)
     action = fake_client.patch_actions.pop()
     assert action["route"] == f"/devices/{fake_light.device_id}"
-    assert action["data"] == [{"attributes": {"startupOnOff": behaviour}}]
+    assert action["data"] == [{"attributes": {"startupOnOff": behaviour.value}}]
     assert fake_light.startup_on_off == behaviour
 
 def test_set_startup_behaviour_toggle(
     fake_light: Light, fake_client: FakeDirigeraHub
 ) -> None:
     behaviour = StartupEnum.START_TOGGLE
     fake_light.set_startup_behaviour(behaviour)
     action = fake_client.patch_actions.pop()
     assert action["route"] == f"/devices/{fake_light.device_id}"
-    assert action["data"] == [{"attributes": {"startupOnOff": behaviour}}]
+    assert action["data"] == [{"attributes": {"startupOnOff": behaviour.value}}]
     assert fake_light.startup_on_off == behaviour
 
 def test_dict_to_light(fake_client: FakeDirigeraHub):
     data = {
         "id": "1237-343-2dfa",
         "type": "light",
         "deviceType": "light",
         "isReachable": True,
         "attributes": {
             "customName": "Light 2",
             "model": "TRADFRI bulb E27 WW 806lm",
             "manufacturer": "IKEA of Sweden",
+            "serialNumber": "84",
             "firmwareVersion": "2.3.093",
             "hardwareVersion": "2",
             "isOn": False,
             "startupOnOff": "startOn",
             "lightLevel": 100,
             "colorTemperature": 2710,
             "colorTemperatureMin": 4000,
@@ -171,19 +225,70 @@
 
     light = dict_to_light(data, fake_client)
     assert light.dirigera_client == fake_client
     assert light.device_id == data["id"]
     assert light.is_reachable == data["isReachable"]
     assert light.custom_name == data["attributes"]["customName"]
     assert light.is_on == data["attributes"]["isOn"]
-    assert light.startup_on_off == data["attributes"]["startupOnOff"]
+    assert light.startup_on_off == StartupEnum(data["attributes"]["startupOnOff"])
+    assert light.light_level == data["attributes"]["lightLevel"]
+    assert light.color_temp == data["attributes"]["colorTemperature"]
+    assert light.color_temp_min == data["attributes"]["colorTemperatureMin"]
+    assert light.color_temp_max == data["attributes"]["colorTemperatureMax"]
+    assert light.can_receive == data["capabilities"]["canReceive"]
+    assert light.room_id == data["room"]["id"]
+    assert light.room_name == data["room"]["name"]
+    assert light.firmware_version == data["attributes"]["firmwareVersion"]
+    assert light.hardware_version == data["attributes"]["hardwareVersion"]
+    assert light.model == data["attributes"]["model"]
+    assert light.manufacturer == data["attributes"]["manufacturer"]
+    assert light.serial_number == data["attributes"]["serialNumber"]
+
+def test_dict_to_light_3rdparty(fake_client: FakeDirigeraHub):
+    data = {
+        "id": "1237-343-2dfa",
+        "type": "light",
+        "deviceType": "light",
+        "isReachable": True,
+        "attributes": {
+            "customName": "Light 2",
+            "model": "3rd party bulb no startupOnOff",
+            "manufacturer": "3rd party",
+            "serialNumber": "84",
+            "firmwareVersion": "2.3.093",
+            "hardwareVersion": "2",
+            "isOn": False,
+            "lightLevel": 100,
+            "colorTemperature": 2710,
+            "colorTemperatureMin": 4000,
+            "colorTemperatureMax": 2202,
+            "colorMode": "temperature",
+        },
+        "capabilities": {
+            "canSend": [],
+            "canReceive": ["customName", "isOn", "lightLevel"],
+        },
+        "room": {
+            "id": "19aa77553369",
+            "name": "Living room",
+        },
+    }
+
+    light = dict_to_light(data, fake_client)
+    assert light.dirigera_client == fake_client
+    assert light.device_id == data["id"]
+    assert light.is_reachable == data["isReachable"]
+    assert light.custom_name == data["attributes"]["customName"]
+    assert light.is_on == data["attributes"]["isOn"]
+    assert light.startup_on_off is None
     assert light.light_level == data["attributes"]["lightLevel"]
     assert light.color_temp == data["attributes"]["colorTemperature"]
     assert light.color_temp_min == data["attributes"]["colorTemperatureMin"]
     assert light.color_temp_max == data["attributes"]["colorTemperatureMax"]
     assert light.can_receive == data["capabilities"]["canReceive"]
     assert light.room_id == data["room"]["id"]
     assert light.room_name == data["room"]["name"]
     assert light.firmware_version == data["attributes"]["firmwareVersion"]
     assert light.hardware_version == data["attributes"]["hardwareVersion"]
     assert light.model == data["attributes"]["model"]
     assert light.manufacturer == data["attributes"]["manufacturer"]
+    assert light.serial_number == data["attributes"]["serialNumber"]
```

### Comparing `dirigera-0.1.6/tests/test_open_close_sensor.py` & `dirigera-0.1.7/tests/test_open_close_sensor.py`

 * *Files identical despite different names*

