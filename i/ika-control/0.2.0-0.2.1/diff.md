# Comparing `tmp/ika-control-0.2.0.tar.gz` & `tmp/ika-control-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ika-control-0.2.0.tar", last modified: Fri May 19 19:32:25 2023, max compression
+gzip compressed data, was "ika-control-0.2.1.tar", last modified: Wed May 24 18:31:16 2023, max compression
```

## Comparing `ika-control-0.2.0.tar` & `ika-control-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-05-19 19:32:25.003232 ika-control-0.2.0/
--rw-r--r--   0 a.ruddick   (502) staff       (20)    35149 2023-01-23 17:35:20.000000 ika-control-0.2.0/LICENSE
--rw-r--r--   0 a.ruddick   (502) staff       (20)     2263 2023-05-19 19:32:25.003300 ika-control-0.2.0/PKG-INFO
--rw-r--r--   0 a.ruddick   (502) staff       (20)     1389 2023-03-16 19:17:53.000000 ika-control-0.2.0/README.md
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-05-19 19:32:25.002083 ika-control-0.2.0/ika/
--rw-r--r--   0 a.ruddick   (502) staff       (20)     2232 2023-04-10 23:30:07.000000 ika-control-0.2.0/ika/__init__.py
--rwxr-xr-x   0 a.ruddick   (502) staff       (20)    22553 2023-04-10 23:28:51.000000 ika-control-0.2.0/ika/driver.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)     9814 2023-04-28 19:55:58.000000 ika-control-0.2.0/ika/mock.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)     8627 2023-03-24 21:57:08.000000 ika-control-0.2.0/ika/util.py
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-05-19 19:32:25.003094 ika-control-0.2.0/ika_control.egg-info/
--rw-r--r--   0 a.ruddick   (502) staff       (20)     2263 2023-05-19 19:32:24.000000 ika-control-0.2.0/ika_control.egg-info/PKG-INFO
--rw-r--r--   0 a.ruddick   (502) staff       (20)      302 2023-05-19 19:32:24.000000 ika-control-0.2.0/ika_control.egg-info/SOURCES.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)        1 2023-05-19 19:32:24.000000 ika-control-0.2.0/ika_control.egg-info/dependency_links.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)       41 2023-05-19 19:32:24.000000 ika-control-0.2.0/ika_control.egg-info/entry_points.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)      135 2023-05-19 19:32:24.000000 ika-control-0.2.0/ika_control.egg-info/requires.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)        4 2023-05-19 19:32:24.000000 ika-control-0.2.0/ika_control.egg-info/top_level.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)      216 2023-05-19 19:32:25.003535 ika-control-0.2.0/setup.cfg
--rw-r--r--   0 a.ruddick   (502) staff       (20)     1506 2023-05-19 19:32:20.000000 ika-control-0.2.0/setup.py
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-05-24 18:31:16.837502 ika-control-0.2.1/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)    35149 2023-01-23 17:35:20.000000 ika-control-0.2.1/LICENSE
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     2263 2023-05-24 18:31:16.837576 ika-control-0.2.1/PKG-INFO
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     1389 2023-03-16 19:17:53.000000 ika-control-0.2.1/README.md
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-05-24 18:31:16.836453 ika-control-0.2.1/ika/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     2232 2023-04-10 23:30:07.000000 ika-control-0.2.1/ika/__init__.py
+-rwxr-xr-x   0 a.ruddick   (502) staff       (20)    22386 2023-05-24 18:27:17.000000 ika-control-0.2.1/ika/driver.py
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     9814 2023-04-28 19:55:58.000000 ika-control-0.2.1/ika/mock.py
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     8627 2023-03-24 21:57:08.000000 ika-control-0.2.1/ika/util.py
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-05-24 18:31:16.837307 ika-control-0.2.1/ika_control.egg-info/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     2263 2023-05-24 18:31:16.000000 ika-control-0.2.1/ika_control.egg-info/PKG-INFO
+-rw-r--r--   0 a.ruddick   (502) staff       (20)      302 2023-05-24 18:31:16.000000 ika-control-0.2.1/ika_control.egg-info/SOURCES.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)        1 2023-05-24 18:31:16.000000 ika-control-0.2.1/ika_control.egg-info/dependency_links.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)       41 2023-05-24 18:31:16.000000 ika-control-0.2.1/ika_control.egg-info/entry_points.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)      135 2023-05-24 18:31:16.000000 ika-control-0.2.1/ika_control.egg-info/requires.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)        4 2023-05-24 18:31:16.000000 ika-control-0.2.1/ika_control.egg-info/top_level.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)      216 2023-05-24 18:31:16.837818 ika-control-0.2.1/setup.cfg
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     1506 2023-05-24 18:30:05.000000 ika-control-0.2.1/setup.py
```

### Comparing `ika-control-0.2.0/LICENSE` & `ika-control-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ika-control-0.2.0/PKG-INFO` & `ika-control-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ika-control
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python driver for IKA instruments.
 Home-page: https://github.com/numat/ika/
 Author: Alex Ruddick
 Author-email: a.ruddick@numat-tech.com
 License: GPLv3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ika-control-0.2.0/README.md` & `ika-control-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ika-control-0.2.0/ika/__init__.py` & `ika-control-0.2.1/ika/__init__.py`

 * *Files identical despite different names*

### Comparing `ika-control-0.2.0/ika/driver.py` & `ika-control-0.2.1/ika/driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,18 +191,15 @@
 
 
 class Hotplate(HotplateProtocol, IKADevice):
     """Driver for IKA hotplate stirrer."""
 
     def __init__(self, address, include_surface_control=False):
         """Set up connection parameters, IP address and port."""
-        if address.startswith('/dev') or address.startswith('COM'):  # serial
-            self.hw: Client = SerialClient(address=address)
-        else:
-            self.hw = TcpClient(address=address)
+        super().__init__(address)
         self.include_surface_control = include_surface_control
 
     async def get(self, include_surface_control=False):
         """Get hotplate speed, surface temperature, and process temperature readings."""
         speed = await self.query(self.READ_ACTUAL_SPEED)
         speed_sp = await self.query(self.READ_SPEED_SETPOINT)
         process_temp = await self.query(self.READ_ACTUAL_PROCESS_TEMP)
```

### Comparing `ika-control-0.2.0/ika/mock.py` & `ika-control-0.2.1/ika/mock.py`

 * *Files identical despite different names*

### Comparing `ika-control-0.2.0/ika/util.py` & `ika-control-0.2.1/ika/util.py`

 * *Files identical despite different names*

### Comparing `ika-control-0.2.0/ika_control.egg-info/PKG-INFO` & `ika-control-0.2.1/ika_control.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ika-control
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python driver for IKA instruments.
 Home-page: https://github.com/numat/ika/
 Author: Alex Ruddick
 Author-email: a.ruddick@numat-tech.com
 License: GPLv3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ika-control-0.2.0/setup.py` & `ika-control-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 with open('README.md') as in_file:
     long_description = in_file.read()
 
 setup(
     name="ika-control",
-    version="0.2.0",
+    version="0.2.1",
     description="Python driver for IKA instruments.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/numat/ika/",
     author="Alex Ruddick",
     author_email="a.ruddick@numat-tech.com",
     packages=['ika'],
```

