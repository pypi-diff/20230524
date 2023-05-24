# Comparing `tmp/srsinst.uga-0.0.1.tar.gz` & `tmp/srsinst.uga-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\PyPI\instrument_library\uga100\dist\.tmp-56qdkxsg\srsinst.uga-0.0.1.tar", last modified: Fri May 12 21:57:05 2023, max compression
+gzip compressed data, was "C:\PyPI\instrument drivers to GIT\uga100\dist\.tmp-6qykfqwj\srsinst.uga-0.0.2.tar", last modified: Wed May 24 20:48:23 2023, max compression
```

## Comparing `srsinst.uga-0.0.1.tar` & `srsinst.uga-0.0.2.tar`

### file list

```diff
@@ -1,53 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 21:57:05.562775 srsinst.uga-0.0.1/
--rw-rw-rw-   0        0        0    35823 2022-11-23 00:41:06.000000 srsinst.uga-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     6868 2023-05-12 21:57:05.562775 srsinst.uga-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     6083 2023-05-12 21:41:17.000000 srsinst.uga-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-12 21:57:05.532777 srsinst.uga-0.0.1/docs/
--rw-rw-rw-   0        0        0      658 2022-10-10 15:59:35.000000 srsinst.uga-0.0.1/docs/Makefile
--rwxrwxrwx   0        0        0       35 2022-11-08 00:43:04.000000 srsinst.uga-0.0.1/docs/autodoc.bat
--rwxrwxrwx   0        0        0      804 2022-10-10 15:59:35.000000 srsinst.uga-0.0.1/docs/make.bat
--rw-rw-rw-   0        0        0       32 2022-10-21 20:04:54.000000 srsinst.uga-0.0.1/docs/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-05-12 21:57:05.542775 srsinst.uga-0.0.1/docs/source/
--rw-rw-rw-   0        0        0     5458 2022-11-01 00:07:51.000000 srsinst.uga-0.0.1/docs/source/basic_operation.rst
--rw-rw-rw-   0        0        0     1944 2022-11-10 00:15:48.000000 srsinst.uga-0.0.1/docs/source/conf.py
--rw-rw-rw-   0        0        0     1168 2022-10-17 18:12:05.000000 srsinst.uga-0.0.1/docs/source/connection.rst
--rw-rw-rw-   0        0        0     1306 2022-11-08 00:20:36.000000 srsinst.uga-0.0.1/docs/source/index.rst
--rw-rw-rw-   0        0        0     1246 2022-10-17 18:01:59.000000 srsinst.uga-0.0.1/docs/source/installation.rst
--rw-rw-rw-   0        0        0     1145 2022-10-21 20:04:55.000000 srsinst.uga-0.0.1/docs/source/license.rst
--rw-rw-rw-   0        0        0       62 2022-11-08 01:01:26.000000 srsinst.uga-0.0.1/docs/source/modules.rst
--rw-rw-rw-   0        0        0       60 2022-10-14 01:09:18.000000 srsinst.uga-0.0.1/docs/source/rga120_operation.rst
--rw-rw-rw-   0        0        0     1010 2022-11-01 00:07:51.000000 srsinst.uga-0.0.1/docs/source/scan_operation.rst
--rw-rw-rw-   0        0        0     1474 2022-10-17 18:12:34.000000 srsinst.uga-0.0.1/docs/source/troubleshooting.rst
--rw-rw-rw-   0        0        0      443 2022-11-10 00:51:51.000000 srsinst.uga-0.0.1/docs/source/uga100.instruments.rst
--rw-rw-rw-   0        0        0      576 2022-11-10 00:33:46.000000 srsinst.uga-0.0.1/docs/source/uga100.instruments.uga100.rst
--rw-rw-rw-   0        0        0      113 2022-11-10 00:29:22.000000 srsinst.uga-0.0.1/docs/source/uga100.rst
--rw-rw-rw-   0        0        0      162 2022-11-10 00:19:45.000000 srsinst.uga-0.0.1/docs/source/uga100.tasks.rst
--rw-rw-rw-   0        0        0     1181 2023-05-12 21:56:47.000000 srsinst.uga-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-12 21:57:05.562775 srsinst.uga-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-02-09 00:46:42.000000 srsinst.uga-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-12 21:57:05.499422 srsinst.uga-0.0.1/srsinst/
-drwxrwxrwx   0        0        0        0 2023-05-12 21:57:05.552775 srsinst.uga-0.0.1/srsinst/uga/
--rw-rw-rw-   0        0        0      229 2023-02-14 01:31:57.000000 srsinst.uga-0.0.1/srsinst/uga/__init__.py
--rw-rw-rw-   0        0        0      483 2022-12-12 16:43:23.000000 srsinst.uga-0.0.1/srsinst/uga/__main__.py
--rw-rw-rw-   0        0        0    10600 2023-05-10 19:39:21.000000 srsinst.uga-0.0.1/srsinst/uga/gaslib.dat
-drwxrwxrwx   0        0        0        0 2023-05-12 21:57:05.552775 srsinst.uga-0.0.1/srsinst/uga/instruments/
--rw-rw-rw-   0        0        0       47 2023-03-16 17:02:33.000000 srsinst.uga-0.0.1/srsinst/uga/instruments/__init__.py
--rw-rw-rw-   0        0        0     1212 2023-04-06 22:21:55.000000 srsinst.uga-0.0.1/srsinst/uga/instruments/get_instruments.py
-drwxrwxrwx   0        0        0        0 2023-05-12 21:57:05.552775 srsinst.uga-0.0.1/srsinst/uga/instruments/uga100/
--rw-rw-rw-   0        0        0        0 2022-11-22 22:50:25.000000 srsinst.uga-0.0.1/srsinst/uga/instruments/uga100/__init__.py
--rw-rw-rw-   0        0        0    10443 2023-05-12 17:44:46.000000 srsinst.uga-0.0.1/srsinst/uga/instruments/uga100/components.py
--rw-rw-rw-   0        0        0     4489 2023-05-10 23:48:01.000000 srsinst.uga-0.0.1/srsinst/uga/instruments/uga100/keys.py
--rw-rw-rw-   0        0        0     5431 2023-05-11 17:09:11.000000 srsinst.uga-0.0.1/srsinst/uga/instruments/uga100/uga.py
-drwxrwxrwx   0        0        0        0 2023-05-12 21:57:05.562775 srsinst.uga-0.0.1/srsinst/uga/tasks/
--rw-rw-rw-   0        0        0        0 2022-11-22 20:35:39.000000 srsinst.uga-0.0.1/srsinst/uga/tasks/__init__.py
--rw-rw-rw-   0        0        0     4289 2023-04-06 22:22:14.000000 srsinst.uga-0.0.1/srsinst/uga/tasks/ugamodecontroltask.py
--rw-rw-rw-   0        0        0     3766 2023-04-06 22:22:33.000000 srsinst.uga-0.0.1/srsinst/uga/tasks/ugamultiplottask.py
--rw-rw-rw-   0        0        0     1892 2023-04-06 22:48:39.000000 srsinst.uga-0.0.1/srsinst/uga/tasks/ugastatemonitortask.py
--rw-rw-rw-   0        0        0     2354 2023-05-10 00:04:38.000000 srsinst.uga-0.0.1/srsinst/uga/uga.taskconfig
-drwxrwxrwx   0        0        0        0 2023-05-12 21:57:05.542775 srsinst.uga-0.0.1/srsinst.uga.egg-info/
--rw-rw-rw-   0        0        0     6868 2023-05-12 21:57:05.000000 srsinst.uga-0.0.1/srsinst.uga.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1218 2023-05-12 21:57:05.000000 srsinst.uga-0.0.1/srsinst.uga.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 21:57:05.000000 srsinst.uga-0.0.1/srsinst.uga.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-12 21:57:05.000000 srsinst.uga-0.0.1/srsinst.uga.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       81 2023-05-12 21:57:05.000000 srsinst.uga-0.0.1/srsinst.uga.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-12 21:57:05.000000 srsinst.uga-0.0.1/srsinst.uga.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-24 20:48:23.927017 srsinst.uga-0.0.2/
+-rw-rw-rw-   0        0        0     1356 2023-05-15 17:35:24.000000 srsinst.uga-0.0.2/.gitignore
+-rw-rw-rw-   0        0        0     1103 2023-05-19 19:35:50.000000 srsinst.uga-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     7000 2023-05-24 20:48:23.927017 srsinst.uga-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6219 2023-05-19 20:11:28.000000 srsinst.uga-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-24 20:48:23.897064 srsinst.uga-0.0.2/docs/
+drwxrwxrwx   0        0        0        0 2023-05-24 20:48:23.897064 srsinst.uga-0.0.2/docs/_static/
+drwxrwxrwx   0        0        0        0 2023-05-24 20:48:23.907027 srsinst.uga-0.0.2/docs/_static/image/
+-rw-rw-rw-   0        0        0   174299 2023-05-16 16:03:57.000000 srsinst.uga-0.0.2/docs/_static/image/UGA100_composition_analysis_screenshot.png
+-rw-rw-rw-   0        0        0     1181 2023-05-12 21:56:47.000000 srsinst.uga-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-24 20:48:23.927017 srsinst.uga-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-02-09 00:46:42.000000 srsinst.uga-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 20:48:23.897064 srsinst.uga-0.0.2/srsinst/
+drwxrwxrwx   0        0        0        0 2023-05-24 20:48:23.917023 srsinst.uga-0.0.2/srsinst/uga/
+-rw-rw-rw-   0        0        0      229 2023-05-24 20:48:10.000000 srsinst.uga-0.0.2/srsinst/uga/__init__.py
+-rw-rw-rw-   0        0        0      483 2023-05-19 21:22:28.000000 srsinst.uga-0.0.2/srsinst/uga/__main__.py
+-rw-rw-rw-   0        0        0    10600 2023-05-19 21:22:27.000000 srsinst.uga-0.0.2/srsinst/uga/gaslib.dat
+drwxrwxrwx   0        0        0        0 2023-05-24 20:48:23.917023 srsinst.uga-0.0.2/srsinst/uga/instruments/
+-rw-rw-rw-   0        0        0       47 2023-05-19 21:22:28.000000 srsinst.uga-0.0.2/srsinst/uga/instruments/__init__.py
+-rw-rw-rw-   0        0        0     1327 2023-05-19 21:32:52.000000 srsinst.uga-0.0.2/srsinst/uga/instruments/get_instruments.py
+drwxrwxrwx   0        0        0        0 2023-05-24 20:48:23.917023 srsinst.uga-0.0.2/srsinst/uga/instruments/uga100/
+-rw-rw-rw-   0        0        0        0 2023-05-19 21:22:28.000000 srsinst.uga-0.0.2/srsinst/uga/instruments/uga100/__init__.py
+-rw-rw-rw-   0        0        0    10643 2023-05-24 18:25:35.000000 srsinst.uga-0.0.2/srsinst/uga/instruments/uga100/components.py
+-rw-rw-rw-   0        0        0     4643 2023-05-24 17:51:21.000000 srsinst.uga-0.0.2/srsinst/uga/instruments/uga100/keys.py
+-rw-rw-rw-   0        0        0     5544 2023-05-19 21:34:11.000000 srsinst.uga-0.0.2/srsinst/uga/instruments/uga100/uga.py
+drwxrwxrwx   0        0        0        0 2023-05-24 20:48:23.927017 srsinst.uga-0.0.2/srsinst/uga/tasks/
+-rw-rw-rw-   0        0        0        0 2023-05-19 21:22:28.000000 srsinst.uga-0.0.2/srsinst/uga/tasks/__init__.py
+-rw-rw-rw-   0        0        0     4415 2023-05-24 17:26:46.000000 srsinst.uga-0.0.2/srsinst/uga/tasks/ugamodecontroltask.py
+-rw-rw-rw-   0        0        0     3881 2023-05-19 21:34:42.000000 srsinst.uga-0.0.2/srsinst/uga/tasks/ugamultiplottask.py
+-rw-rw-rw-   0        0        0     1949 2023-05-24 18:32:16.000000 srsinst.uga-0.0.2/srsinst/uga/tasks/ugastatemonitortask.py
+-rw-rw-rw-   0        0        0     2339 2023-05-24 16:25:05.000000 srsinst.uga-0.0.2/srsinst/uga/uga.taskconfig
+drwxrwxrwx   0        0        0        0 2023-05-24 20:48:23.917023 srsinst.uga-0.0.2/srsinst.uga.egg-info/
+-rw-rw-rw-   0        0        0     7000 2023-05-24 20:48:23.000000 srsinst.uga-0.0.2/srsinst.uga.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      817 2023-05-24 20:48:23.000000 srsinst.uga-0.0.2/srsinst.uga.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 20:48:23.000000 srsinst.uga-0.0.2/srsinst.uga.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-24 20:48:23.000000 srsinst.uga-0.0.2/srsinst.uga.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       81 2023-05-24 20:48:23.000000 srsinst.uga-0.0.2/srsinst.uga.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-24 20:48:23.000000 srsinst.uga-0.0.2/srsinst.uga.egg-info/top_level.txt
```

### Comparing `srsinst.uga-0.0.1/PKG-INFO` & `srsinst.uga-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srsinst.uga
-Version: 0.0.1
+Version: 0.0.2
 Summary: Instrument driver package for Universal Gas Analyzers (UGA) from Stanford Research Systems
 Author: Chulhoon Kim
 License: MIT license
 Keywords: UGA,universal gas analyzer,SRS,Stanford Research Systems
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -12,24 +12,26 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: full
-License-File: LICENSE.txt
+License-File: LICENSE
 
 # `srsinst.uga`
 
 `srsinst.uga` contains a Python instrument driver to control and acquire 
 mass spectra of atmospheric gas samples from 
 [Stanford Research Systems (SRS) Universal Gas Analyzer (UGA)](https://thinksrs.com/products/uga.html). It also has a collection of Python scripts 
-that runs on a graphic user interface (GUI) based on [srsgui](https://pypi.org/project/srsgui/).
+that runs on a graphic user interface (GUI) based on [srsgui](https://thinksrs.github.io/srsgui/).
 
 
+![screenshot](https://github.com/thinkSRS/srsinst.uga/blob/main/docs/_static/image/UGA100_composition_analysis_screenshot.png " ")
+
 ## Installation
 You need a working Python with `pip` (Python package installer) installed. If you don't,
 [install Python 3](https://realpython.com/installing-python/) to your system.
 
 To install `srsinst.uga` as an instrument driver only, use Python package installer `pip` 
 from the command line.
```

### Comparing `srsinst.uga-0.0.1/README.md` & `srsinst.uga-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # `srsinst.uga`
 
 `srsinst.uga` contains a Python instrument driver to control and acquire 
 mass spectra of atmospheric gas samples from 
 [Stanford Research Systems (SRS) Universal Gas Analyzer (UGA)](https://thinksrs.com/products/uga.html). It also has a collection of Python scripts 
-that runs on a graphic user interface (GUI) based on [srsgui](https://pypi.org/project/srsgui/).
+that runs on a graphic user interface (GUI) based on [srsgui](https://thinksrs.github.io/srsgui/).
 
 
+![screenshot](https://github.com/thinkSRS/srsinst.uga/blob/main/docs/_static/image/UGA100_composition_analysis_screenshot.png " ")
+
 ## Installation
 You need a working Python with `pip` (Python package installer) installed. If you don't,
 [install Python 3](https://realpython.com/installing-python/) to your system.
 
 To install `srsinst.uga` as an instrument driver only, use Python package installer `pip` 
 from the command line.
```

### Comparing `srsinst.uga-0.0.1/docs/source/license.rst` & `srsinst.uga-0.0.2/LICENSE`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,17 @@
-.. _license:
+MIT License
 
-License
-=========
+Copyright (c) 2023 Stanford Research Systems
 
-The MIT License
-
-Copyright (c) 2022 Stanford Research Systems
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of
-this software and associated documentation files (the "Software"), to deal in
-the Software without restriction, including without limitation the rights to
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
-of the Software, and to permit persons to whom the Software is furnished to do
-so, subject to the following conditions:
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all
 copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
```

### Comparing `srsinst.uga-0.0.1/pyproject.toml` & `srsinst.uga-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `srsinst.uga-0.0.1/srsinst/uga/gaslib.dat` & `srsinst.uga-0.0.2/srsinst/uga/gaslib.dat`

 * *Files identical despite different names*

### Comparing `srsinst.uga-0.0.1/srsinst/uga/instruments/get_instruments.py` & `srsinst.uga-0.0.2/srsinst/uga/instruments/get_instruments.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+##! 
+##! Coptright(c) 2023 Stanford Research Systems, All right reserved
+##! Subject to the MIT License
+##! 
+
 import logging
 from srsgui import Task
 from srsinst.rga import RGA100
 
 from srsinst.uga.instruments.uga100.uga import UGA100
 
 """
```

### Comparing `srsinst.uga-0.0.1/srsinst/uga/instruments/uga100/components.py` & `srsinst.uga-0.0.2/srsinst/uga/instruments/uga100/components.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+##! 
+##! Coptright(c) 2023 Stanford Research Systems, All right reserved
+##! Subject to the MIT License
+##! 
 
 from srsgui import Component, Instrument
 
 from srsgui import Command, GetCommand,\
                    BoolCommand, BoolGetCommand,\
                    IntCommand, IntGetCommand, IntSetCommand,\
                    FloatCommand, FloatSetCommand, FloatGetCommand, \
@@ -36,14 +40,15 @@
         Keys.TurningOn4: 4,
         Keys.TurningOn5: 5,
         Keys.TurningOff6: 6,
         Keys.TurningOff7: 7,
         Keys.TurningIdle8: 8,
         Keys.TurningIdle9: 9,
         Keys.TurningIdle10: 10,
+        Keys.TurningIdle11: 11,
         Keys.Error: 12,
     }
 
     OffOnDict = {
         Keys.Off: 0,
         Keys.On:  1,
     }
@@ -133,20 +138,20 @@
                 self.check_id()
    
 
 class IonGauge(Component):
     """
     IonGauge component has two commands and one method:
 
-    The state command turn on and off the ion gauge.
-    The ion gauge can be turned on, only when the turbo pump is on or idle.
+    * Command 'state' turns on and off the ion gauge.
+      Ion gauge can be turned on, only when the turbo pump is on or idle.
 
-    The ion gauge has two filaments and if one is broken, you can select the other one.
+    * Ion gauge has two filaments and if one is broken, you can select the other one.
 
-    The method get_pressure() return the ion gauge pressure reading in Torr.
+    * Method get_pressure() returns the ion gauge pressure reading in Torr.
     """
     StateDict = {
         Keys.Off: 0,
         Keys.On: 1,
         Keys.Degas: 2
     }
     FilamentDict = {
@@ -185,15 +190,15 @@
     bake_temperature = IntIndexCommand('ZPTB', 1, 0, BakeHeaterDict, '°C')
     sample_temperature = IntIndexCommand('ZPTH', 3, 0, HeaterDict, '°C')
 
 
 class Temperature(Component):
     """
     Temperature component contains temperature measurements from 5 sensors.
-    If the temperature calue us 255, the sensor is not working properly.
+    If the temperature value is 255, the sensor is not working properly.
     """
     turbo_pump = IntGetCommand('ZQTT', '°C')
     elbow = IntGetCommand('ZQTA', '°C')
     chamber = IntGetCommand('ZQTB', '°C')
     sample_inlet = IntGetCommand('ZQTC', '°C')
     capillary = IntGetCommand('ZQTD', '°C')
 
@@ -202,20 +207,21 @@
     channel = IntCommand('ZCMI')
 
 
 class Pressure(Component):
     """
     Pressure component has two commands:
 
-         Values are pressure measured with gauges:
+        * Values are pressure measured with gauges:
 
             Pressure from Pirani and CM gauges are in the unit of uTorr (1e-6 Torr).
             pressure from IG is in the unit of pTorr (1e-12 Torr) regardless of the display unit
 
-         Display_unit is to select the pressure unit for the front panel display.
+
+        * Display_unit is to select the pressure unit for the front panel display.
 
             Reply from values command always in the unit of Torr.
     """
     GaugeDict = {
         Keys.Pirani: 0,
         Keys.Roughting: 0,
         Keys.CM: 2,
@@ -230,15 +236,14 @@
         Keys.MilliBar: 2,
         Keys.Bar: 3
     }
     values = IntIndexGetCommand('ZQAD', 3, 0, GaugeDict)
     display_unit = DictCommand('ZPPU', UnitDict)
 
 
-
 class Ethernet(Component):
     mac_address = GetCommand('ZQMC')
     ip_address = Command('ZPIP')
     gateway = Command('ZPGW')
     subnet_mask = Command('ZPSM')
     login = Command('ZPNM')
     password = Command('ZPPW')
@@ -277,17 +282,18 @@
     serial_number = GetCommand('ZQSN')
     baud_rate = IntCommand('ZPBA')
 
     states = IntGetCommand('ZBST')
     changed = IntGetCommand('ZBCT')
     changing = IntGetCommand('ZBTT')
     error = DictGetCommand('ZERR', Keys.ErrorMessageDict)
+    error_number = IntGetCommand('ZERR')
     error_message = IndexGetCommand('ZEDS', index_max=126)
 
-    exclude_capture = [error_message]
+    exclude_capture = [error_number, error_message]
 
     def get_status_text(self):
         out_buffer = ''
         error_buffer = 'Errors: '
         item_line_format = '{}: {} \n'
         
         states = self.states
```

### Comparing `srsinst.uga-0.0.1/srsinst/uga/instruments/uga100/keys.py` & `srsinst.uga-0.0.2/srsinst/uga/instruments/uga100/keys.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+##! 
+##! Coptright(c) 2023 Stanford Research Systems, All right reserved
+##! Subject to the MIT License
+##! 
 
 class Keys:
     OK = 'OK'
     # Mode component
     Off = 'Off'
     On = 'On'
     Idle = 'Idle'
@@ -21,14 +25,15 @@
 
     TurningOff6 = 'Turning off (6)'
     TurningOff7 = 'Turning off (7)'
 
     TurningIdle8 = 'Turning idle (8)'
     TurningIdle9 = 'Turning idle (9)'
     TurningIdle10 = 'Turning idle (10)'
+    TurningIdle11 = 'Turning idle (11)'
 
     Error = 'Error'
 
     Degas = 'Degas'
 
     Filament1 = 'Fil. 1'
     Filament2 = 'Fil. 2'
```

### Comparing `srsinst.uga-0.0.1/srsinst/uga/instruments/uga100/uga.py` & `srsinst.uga-0.0.2/srsinst/uga/instruments/uga100/uga.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,340 +1,347 @@
-00000000: 0d0a 6672 6f6d 2073 7273 6775 692e 696e  ..from srsgui.in
-00000010: 7374 2e63 6f6d 706f 6e65 6e74 2069 6d70  st.component imp
-00000020: 6f72 7420 436f 6d70 6f6e 656e 740d 0a66  ort Component..f
-00000030: 726f 6d20 7372 7367 7569 2e69 6e73 742e  rom srsgui.inst.
-00000040: 696e 7374 7275 6d65 6e74 2069 6d70 6f72  instrument impor
-00000050: 7420 496e 7374 7275 6d65 6e74 2c20 5365  t Instrument, Se
-00000060: 7269 616c 496e 7465 7266 6163 652c 2054  rialInterface, T
-00000070: 6370 6970 496e 7465 7266 6163 650d 0a66  cpipInterface..f
-00000080: 726f 6d20 7372 7367 7569 2e69 6e73 742e  rom srsgui.inst.
-00000090: 6578 6365 7074 696f 6e73 2069 6d70 6f72  exceptions impor
-000000a0: 7420 496e 7374 4964 4572 726f 720d 0a0d  t InstIdError...
-000000b0: 0a66 726f 6d20 7372 7367 7569 2e74 6173  .from srsgui.tas
-000000c0: 6b2e 696e 7075 7473 2069 6d70 6f72 7420  k.inputs import 
-000000d0: 4669 6e64 4c69 7374 496e 7075 742c 2049  FindListInput, I
-000000e0: 6e74 6567 6572 4c69 7374 496e 7075 742c  ntegerListInput,
-000000f0: 2049 7034 496e 7075 742c 2053 7472 696e   Ip4Input, Strin
-00000100: 6749 6e70 7574 2c20 5061 7373 776f 7264  gInput, Password
-00000110: 496e 7075 740d 0a0d 0a66 726f 6d20 2e63  Input....from .c
-00000120: 6f6d 706f 6e65 6e74 7320 696d 706f 7274  omponents import
-00000130: 2042 7970 6173 7350 756d 702c 2052 6f75   BypassPump, Rou
-00000140: 6768 696e 6750 756d 702c 2054 7572 626f  ghingPump, Turbo
-00000150: 5075 6d70 2c20 5c0d 0a20 2020 2020 2020  Pump, \..       
-00000160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000170: 2042 7970 6173 7356 616c 7665 2c20 5361   BypassValve, Sa
-00000180: 6d70 6c65 5661 6c76 652c 2056 656e 7456  mpleValve, VentV
-00000190: 616c 7665 2c20 5c0d 0a20 2020 2020 2020  alve, \..       
-000001a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000001b0: 2052 4741 2c20 496f 6e47 6175 6765 2c20   RGA, IonGauge, 
-000001c0: 204d 756c 7469 706c 6549 6e6c 6574 2c20   MultipleInlet, 
-000001d0: 5c0d 0a20 2020 2020 2020 2020 2020 2020  \..             
-000001e0: 2020 2020 2020 2020 2020 2050 7265 7373             Press
-000001f0: 7572 652c 2048 6561 7465 7273 2c20 5465  ure, Heaters, Te
-00000200: 6d70 6572 6174 7572 652c 205c 0d0a 2020  mperature, \..  
+00000000: 2323 2120 0d0a 2323 2120 436f 7074 7269  ##! ..##! Coptri
+00000010: 6768 7428 6329 2032 3032 3320 5374 616e  ght(c) 2023 Stan
+00000020: 666f 7264 2052 6573 6561 7263 6820 5379  ford Research Sy
+00000030: 7374 656d 732c 2041 6c6c 2072 6967 6874  stems, All right
+00000040: 2072 6573 6572 7665 640d 0a23 2321 2053   reserved..##! S
+00000050: 7562 6a65 6374 2074 6f20 7468 6520 4d49  ubject to the MI
+00000060: 5420 4c69 6365 6e73 650d 0a23 2321 200d  T License..##! .
+00000070: 0a0d 0a66 726f 6d20 7372 7367 7569 2e69  ...from srsgui.i
+00000080: 6e73 742e 636f 6d70 6f6e 656e 7420 696d  nst.component im
+00000090: 706f 7274 2043 6f6d 706f 6e65 6e74 0d0a  port Component..
+000000a0: 6672 6f6d 2073 7273 6775 692e 696e 7374  from srsgui.inst
+000000b0: 2e69 6e73 7472 756d 656e 7420 696d 706f  .instrument impo
+000000c0: 7274 2049 6e73 7472 756d 656e 742c 2053  rt Instrument, S
+000000d0: 6572 6961 6c49 6e74 6572 6661 6365 2c20  erialInterface, 
+000000e0: 5463 7069 7049 6e74 6572 6661 6365 0d0a  TcpipInterface..
+000000f0: 6672 6f6d 2073 7273 6775 692e 696e 7374  from srsgui.inst
+00000100: 2e65 7863 6570 7469 6f6e 7320 696d 706f  .exceptions impo
+00000110: 7274 2049 6e73 7449 6445 7272 6f72 0d0a  rt InstIdError..
+00000120: 0d0a 6672 6f6d 2073 7273 6775 692e 7461  ..from srsgui.ta
+00000130: 736b 2e69 6e70 7574 7320 696d 706f 7274  sk.inputs import
+00000140: 2046 696e 644c 6973 7449 6e70 7574 2c20   FindListInput, 
+00000150: 496e 7465 6765 724c 6973 7449 6e70 7574  IntegerListInput
+00000160: 2c20 4970 3449 6e70 7574 2c20 5374 7269  , Ip4Input, Stri
+00000170: 6e67 496e 7075 742c 2050 6173 7377 6f72  ngInput, Passwor
+00000180: 6449 6e70 7574 0d0a 0d0a 6672 6f6d 202e  dInput....from .
+00000190: 636f 6d70 6f6e 656e 7473 2069 6d70 6f72  components impor
+000001a0: 7420 4279 7061 7373 5075 6d70 2c20 526f  t BypassPump, Ro
+000001b0: 7567 6869 6e67 5075 6d70 2c20 5475 7262  ughingPump, Turb
+000001c0: 6f50 756d 702c 205c 0d0a 2020 2020 2020  oPump, \..      
+000001d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000001e0: 2020 4279 7061 7373 5661 6c76 652c 2053    BypassValve, S
+000001f0: 616d 706c 6556 616c 7665 2c20 5665 6e74  ampleValve, Vent
+00000200: 5661 6c76 652c 205c 0d0a 2020 2020 2020  Valve, \..      
 00000210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000220: 2020 2020 2020 4574 6865 726e 6574 2c20        Ethernet, 
-00000230: 5374 6174 7573 2c20 4d6f 6465 0d0a 6672  Status, Mode..fr
-00000240: 6f6d 202e 6b65 7973 2069 6d70 6f72 7420  om .keys import 
-00000250: 4b65 7973 0d0a 0d0a 0d0a 636c 6173 7320  Keys......class 
-00000260: 5547 4131 3030 2849 6e73 7472 756d 656e  UGA100(Instrumen
-00000270: 7429 3a0d 0a20 2020 205f 4964 5374 7269  t):..    _IdStri
-00000280: 6e67 203d 2027 5352 535f 5547 4127 0d0a  ng = 'SRS_UGA'..
-00000290: 2020 2020 5f74 6572 6d5f 6368 6172 203d      _term_char =
-000002a0: 2062 275c 7227 0d0a 0d0a 2020 2020 6176   b'\r'....    av
-000002b0: 6169 6c61 626c 655f 696e 7465 7266 6163  ailable_interfac
-000002c0: 6573 203d 205b 0d0a 2020 2020 2020 2020  es = [..        
-000002d0: 5b20 2020 5365 7269 616c 496e 7465 7266  [   SerialInterf
-000002e0: 6163 652c 0d0a 2020 2020 2020 2020 2020  ace,..          
-000002f0: 2020 7b0d 0a20 2020 2020 2020 2020 2020    {..           
-00000300: 2020 2020 2027 706f 7274 273a 2046 696e       'port': Fin
-00000310: 644c 6973 7449 6e70 7574 2829 2c0d 0a20  dListInput(),.. 
-00000320: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00000330: 6261 7564 5f72 6174 6527 3a20 496e 7465  baud_rate': Inte
-00000340: 6765 724c 6973 7449 6e70 7574 285b 3238  gerListInput([28
-00000350: 3830 302c 2033 3834 3030 5d29 2c0d 0a20  800, 38400]),.. 
-00000360: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00000370: 6861 7264 7761 7265 5f66 6c6f 775f 636f  hardware_flow_co
-00000380: 6e74 726f 6c27 3a20 5472 7565 0d0a 2020  ntrol': True..  
-00000390: 2020 2020 2020 2020 2020 7d0d 0a20 2020            }..   
-000003a0: 2020 2020 205d 2c0d 0a20 2020 2020 2020       ],..       
-000003b0: 205b 2020 2054 6370 6970 496e 7465 7266   [   TcpipInterf
-000003c0: 6163 652c 0d0a 2020 2020 2020 2020 2020  ace,..          
-000003d0: 2020 7b0d 0a20 2020 2020 2020 2020 2020    {..           
-000003e0: 2020 2020 2027 6970 5f61 6464 7265 7373       'ip_address
-000003f0: 273a 2049 7034 496e 7075 7428 2731 3932  ': Ip4Input('192
-00000400: 2e31 3638 2e31 2e31 3027 292c 0d0a 2020  .168.1.10'),..  
-00000410: 2020 2020 2020 2020 2020 2020 2020 2775                'u
-00000420: 7365 725f 6964 273a 2053 7472 696e 6749  ser_id': StringI
-00000430: 6e70 7574 2827 7372 7375 6761 2729 2c0d  nput('srsuga'),.
-00000440: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000450: 2027 7061 7373 776f 7264 273a 2050 6173   'password': Pas
-00000460: 7377 6f72 6449 6e70 7574 2827 7372 7375  swordInput('srsu
-00000470: 6761 2729 2c0d 0a20 2020 2020 2020 2020  ga'),..         
-00000480: 2020 2020 2020 2027 706f 7274 273a 2038         'port': 8
-00000490: 3138 0d0a 2020 2020 2020 2020 2020 2020  18..            
-000004a0: 7d0d 0a20 2020 2020 2020 205d 0d0a 2020  }..        ]..  
-000004b0: 2020 5d0d 0a0d 0a20 2020 2064 6566 205f    ]....    def _
-000004c0: 5f69 6e69 745f 5f28 7365 6c66 2c20 696e  _init__(self, in
-000004d0: 7465 7266 6163 655f 7479 7065 3d4e 6f6e  terface_type=Non
-000004e0: 652c 202a 6172 6773 293a 0d0a 2020 2020  e, *args):..    
-000004f0: 2020 2020 7375 7065 7228 292e 5f5f 696e      super().__in
-00000500: 6974 5f5f 2869 6e74 6572 6661 6365 5f74  it__(interface_t
-00000510: 7970 652c 202a 6172 6773 290d 0a0d 0a20  ype, *args).... 
-00000520: 2020 2020 2020 2073 656c 662e 6d6f 6465         self.mode
-00000530: 203d 204d 6f64 6528 7365 6c66 290d 0a20   = Mode(self).. 
-00000540: 2020 2020 2020 2073 656c 662e 6270 203d         self.bp =
-00000550: 2042 7970 6173 7350 756d 7028 7365 6c66   BypassPump(self
-00000560: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00000570: 7270 203d 2052 6f75 6768 696e 6750 756d  rp = RoughingPum
-00000580: 7028 7365 6c66 290d 0a20 2020 2020 2020  p(self)..       
-00000590: 2073 656c 662e 7470 203d 2054 7572 626f   self.tp = Turbo
-000005a0: 5075 6d70 2873 656c 6629 0d0a 2020 2020  Pump(self)..    
-000005b0: 2020 2020 7365 6c66 2e62 7620 3d20 4279      self.bv = By
-000005c0: 7061 7373 5661 6c76 6528 7365 6c66 290d  passValve(self).
-000005d0: 0a20 2020 2020 2020 2073 656c 662e 7376  .        self.sv
-000005e0: 203d 2053 616d 706c 6556 616c 7665 2873   = SampleValve(s
-000005f0: 656c 6629 0d0a 2020 2020 2020 2020 7365  elf)..        se
-00000600: 6c66 2e76 7620 3d20 5665 6e74 5661 6c76  lf.vv = VentValv
-00000610: 6528 7365 6c66 290d 0a20 2020 2020 2020  e(self)..       
-00000620: 2073 656c 662e 7267 6120 3d20 5247 4128   self.rga = RGA(
-00000630: 7365 6c66 290d 0a20 2020 2020 2020 2073  self)..        s
-00000640: 656c 662e 6967 203d 2049 6f6e 4761 7567  elf.ig = IonGaug
-00000650: 6528 7365 6c66 290d 0a20 2020 2020 2020  e(self)..       
-00000660: 2073 656c 662e 6d69 203d 204d 756c 7469   self.mi = Multi
-00000670: 706c 6549 6e6c 6574 2873 656c 6629 0d0a  pleInlet(self)..
-00000680: 2020 2020 2020 2020 7365 6c66 2e68 7420          self.ht 
-00000690: 3d20 4865 6174 6572 7328 7365 6c66 290d  = Heaters(self).
-000006a0: 0a0d 0a20 2020 2020 2020 2073 656c 662e  ...        self.
-000006b0: 7465 6d70 6572 6174 7572 6520 3d20 5465  temperature = Te
-000006c0: 6d70 6572 6174 7572 6528 7365 6c66 290d  mperature(self).
-000006d0: 0a20 2020 2020 2020 2073 656c 662e 7072  .        self.pr
-000006e0: 6573 7375 7265 203d 2050 7265 7373 7572  essure = Pressur
-000006f0: 6528 7365 6c66 290d 0a20 2020 2020 2020  e(self)..       
-00000700: 2073 656c 662e 6574 6865 726e 6574 203d   self.ethernet =
-00000710: 2045 7468 6572 6e65 7428 7365 6c66 290d   Ethernet(self).
-00000720: 0a20 2020 2020 2020 2073 656c 662e 7374  .        self.st
-00000730: 6174 7573 203d 2053 7461 7475 7328 7365  atus = Status(se
-00000740: 6c66 290d 0a0d 0a20 2020 2064 6566 2063  lf)....    def c
-00000750: 6865 636b 5f69 6428 7365 6c66 293a 0d0a  heck_id(self):..
-00000760: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
-00000770: 656c 662e 6973 5f63 6f6e 6e65 6374 6564  elf.is_connected
-00000780: 2829 3a0d 0a20 2020 2020 2020 2020 2020  ():..           
-00000790: 2072 6574 7572 6e20 4e6f 6e65 2c20 4e6f   return None, No
-000007a0: 6e65 2c20 4e6f 6e65 0d0a 0d0a 2020 2020  ne, None....    
-000007b0: 2020 2020 7265 706c 7920 3d20 7365 6c66      reply = self
-000007c0: 2e71 7565 7279 5f74 6578 7428 275a 5149  .query_text('ZQI
-000007d0: 443f 2729 2e73 7472 6970 2829 0d0a 2020  D?').strip()..  
-000007e0: 2020 2020 2020 7374 7269 6e67 7320 3d20        strings = 
-000007f0: 7265 706c 792e 7370 6c69 7428 272c 2729  reply.split(',')
-00000800: 0d0a 0d0a 2020 2020 2020 2020 6966 206c  ....        if l
-00000810: 656e 2873 7472 696e 6773 2920 213d 2033  en(strings) != 3
-00000820: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-00000830: 6574 7572 6e20 4e6f 6e65 2c20 4e6f 6e65  eturn None, None
-00000840: 2c20 4e6f 6e65 0d0a 0d0a 2020 2020 2020  , None....      
-00000850: 2020 6d6f 6465 6c5f 6e61 6d65 203d 2073    model_name = s
-00000860: 7472 696e 6773 5b30 5d2e 7374 7269 7028  trings[0].strip(
-00000870: 290d 0a20 2020 2020 2020 2073 6572 6961  )..        seria
-00000880: 6c5f 6e75 6d62 6572 203d 2073 7472 696e  l_number = strin
-00000890: 6773 5b31 5d2e 7374 7269 7028 295b 343a  gs[1].strip()[4:
-000008a0: 5d0d 0a20 2020 2020 2020 2066 6972 6d77  ]..        firmw
-000008b0: 6172 655f 7665 7273 696f 6e20 3d20 7374  are_version = st
-000008c0: 7269 6e67 735b 325d 2e73 7472 6970 2829  rings[2].strip()
-000008d0: 5b32 3a5d 0d0a 0d0a 2020 2020 2020 2020  [2:]....        
-000008e0: 6966 2073 656c 662e 5f49 6453 7472 696e  if self._IdStrin
-000008f0: 6720 6e6f 7420 696e 2072 6570 6c79 3a0d  g not in reply:.
-00000900: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-00000910: 7365 2049 6e73 7449 6445 7272 6f72 2822  se InstIdError("
-00000920: 496e 7661 6c69 6420 696e 7374 7275 6d65  Invalid instrume
-00000930: 6e74 3a20 7b7d 206e 6f74 2069 6e20 7b7d  nt: {} not in {}
-00000940: 220d 0a20 2020 2020 2020 2020 2020 2020  "..             
-00000950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000960: 202e 666f 726d 6174 2873 656c 662e 5f49   .format(self._I
-00000970: 6453 7472 696e 672c 2072 6570 6c79 2929  dString, reply))
-00000980: 0d0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
-00000990: 662e 7267 612e 7374 6174 6520 3d3d 204b  f.rga.state == K
-000009a0: 6579 732e 4f6e 3a0d 0a20 2020 2020 2020  eys.On:..       
-000009b0: 2020 2020 2073 656c 662e 7267 612e 6368       self.rga.ch
-000009c0: 6563 6b5f 6964 2829 2020 2320 636f 6e66  eck_id()  # conf
-000009d0: 6967 7572 6520 5247 410d 0a0d 0a20 2020  igure RGA....   
-000009e0: 2020 2020 2069 6620 2755 4741 5f48 5427       if 'UGA_HT'
-000009f0: 2069 6e20 6d6f 6465 6c5f 6e61 6d65 3a0d   in model_name:.
-00000a00: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00000a10: 6861 7361 7474 7228 7365 6c66 2c20 2762  hasattr(self, 'b
-00000a20: 7627 293a 0d0a 2020 2020 2020 2020 2020  v'):..          
-00000a30: 2020 2020 2020 6465 6c20 7365 6c66 2e62        del self.b
-00000a40: 760d 0a20 2020 2020 2020 2020 2020 2069  v..            i
-00000a50: 6620 6861 7361 7474 7228 7365 6c66 2c20  f hasattr(self, 
-00000a60: 2773 7627 293a 0d0a 2020 2020 2020 2020  'sv'):..        
-00000a70: 2020 2020 2020 2020 6465 6c20 7365 6c66          del self
-00000a80: 2e73 760d 0a20 2020 2020 2020 2020 2020  .sv..           
-00000a90: 2069 6620 6861 7361 7474 7228 7365 6c66   if hasattr(self
-00000aa0: 2c20 276d 6927 293a 0d0a 2020 2020 2020  , 'mi'):..      
-00000ab0: 2020 2020 2020 2020 2020 6465 6c20 7365            del se
-00000ac0: 6c66 2e6d 690d 0a20 2020 2020 2020 2020  lf.mi..         
-00000ad0: 2020 2069 6620 6e6f 7420 6861 7361 7474     if not hasatt
-00000ae0: 7228 7365 6c66 2c20 2762 7027 293a 0d0a  r(self, 'bp'):..
-00000af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b00: 7365 6c66 2e62 7020 3d20 4279 7061 7373  self.bp = Bypass
-00000b10: 5075 6d70 2873 656c 6629 0d0a 2020 2020  Pump(self)..    
-00000b20: 2020 2020 656c 6966 2027 5547 415f 4c54      elif 'UGA_LT
-00000b30: 2720 696e 206d 6f64 656c 5f6e 616d 653a  ' in model_name:
-00000b40: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00000b50: 206e 6f74 2068 6173 6174 7472 2873 656c   not hasattr(sel
-00000b60: 662c 2027 6276 2729 3a0d 0a20 2020 2020  f, 'bv'):..     
-00000b70: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00000b80: 6276 203d 2042 7970 6173 7356 616c 7665  bv = BypassValve
-00000b90: 2873 656c 6629 0d0a 2020 2020 2020 2020  (self)..        
-00000ba0: 2020 2020 6966 206e 6f74 2068 6173 6174      if not hasat
-00000bb0: 7472 2873 656c 662c 2027 7376 2729 3a0d  tr(self, 'sv'):.
-00000bc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000bd0: 2073 656c 662e 7376 203d 2053 616d 706c   self.sv = Sampl
-00000be0: 6556 616c 7665 2873 656c 6629 0d0a 2020  eValve(self)..  
-00000bf0: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-00000c00: 2068 6173 6174 7472 2873 656c 662c 2027   hasattr(self, '
-00000c10: 6d69 2729 3a0d 0a20 2020 2020 2020 2020  mi'):..         
-00000c20: 2020 2020 2020 2073 656c 662e 6d69 203d         self.mi =
-00000c30: 204d 756c 7469 706c 6549 6e6c 6574 2873   MultipleInlet(s
-00000c40: 656c 6629 0d0a 2020 2020 2020 2020 2020  elf)..          
-00000c50: 2020 6966 2068 6173 6174 7472 2873 656c    if hasattr(sel
-00000c60: 662c 2027 6270 2729 3a0d 0a20 2020 2020  f, 'bp'):..     
-00000c70: 2020 2020 2020 2020 2020 2064 656c 2073             del s
-00000c80: 656c 662e 6270 0d0a 2020 2020 2020 2020  elf.bp..        
-00000c90: 656c 6966 2027 5547 415f 504d 2720 696e  elif 'UGA_PM' in
-00000ca0: 206d 6f64 656c 5f6e 616d 653a 0d0a 2020   model_name:..  
-00000cb0: 2020 2020 2020 2020 2020 6966 2068 6173            if has
-00000cc0: 6174 7472 2873 656c 662c 2027 6276 2729  attr(self, 'bv')
-00000cd0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00000ce0: 2020 2064 656c 2073 656c 662e 6276 0d0a     del self.bv..
-00000cf0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-00000d00: 6f74 2068 6173 6174 7472 2873 656c 662c  ot hasattr(self,
-00000d10: 2027 7376 2729 3a0d 0a20 2020 2020 2020   'sv'):..       
-00000d20: 2020 2020 2020 2020 2073 656c 662e 7376           self.sv
-00000d30: 203d 2053 616d 706c 6556 616c 7665 2873   = SampleValve(s
-00000d40: 656c 6629 0d0a 2020 2020 2020 2020 2020  elf)..          
-00000d50: 2020 6966 206e 6f74 2068 6173 6174 7472    if not hasattr
-00000d60: 2873 656c 662c 2027 6d69 2729 3a0d 0a20  (self, 'mi'):.. 
-00000d70: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00000d80: 656c 662e 6d69 203d 204d 756c 7469 706c  elf.mi = Multipl
-00000d90: 6549 6e6c 6574 2873 656c 6629 0d0a 2020  eInlet(self)..  
-00000da0: 2020 2020 2020 2020 2020 6966 2068 6173            if has
-00000db0: 6174 7472 2873 656c 662c 2027 6270 2729  attr(self, 'bp')
-00000dc0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00000dd0: 2020 2064 656c 2073 656c 662e 6270 0d0a     del self.bp..
-00000de0: 2020 2020 2020 2020 656c 6966 2027 5547          elif 'UG
-00000df0: 4127 2069 6e20 6d6f 6465 6c5f 6e61 6d65  A' in model_name
-00000e00: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
-00000e10: 6620 6e6f 7420 6861 7361 7474 7228 7365  f not hasattr(se
-00000e20: 6c66 2c20 2762 7627 293a 0d0a 2020 2020  lf, 'bv'):..    
-00000e30: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00000e40: 2e62 7620 3d20 4279 7061 7373 5661 6c76  .bv = BypassValv
-00000e50: 6528 7365 6c66 290d 0a20 2020 2020 2020  e(self)..       
-00000e60: 2020 2020 2069 6620 6e6f 7420 6861 7361       if not hasa
-00000e70: 7474 7228 7365 6c66 2c20 2773 7627 293a  ttr(self, 'sv'):
-00000e80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000e90: 2020 7365 6c66 2e73 7620 3d20 5361 6d70    self.sv = Samp
-00000ea0: 6c65 5661 6c76 6528 7365 6c66 290d 0a20  leValve(self).. 
-00000eb0: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-00000ec0: 7420 6861 7361 7474 7228 7365 6c66 2c20  t hasattr(self, 
-00000ed0: 276d 6927 293a 0d0a 2020 2020 2020 2020  'mi'):..        
-00000ee0: 2020 2020 2020 2020 7365 6c66 2e6d 6920          self.mi 
-00000ef0: 3d20 4d75 6c74 6970 6c65 496e 6c65 7428  = MultipleInlet(
-00000f00: 7365 6c66 290d 0a20 2020 2020 2020 2020  self)..         
-00000f10: 2020 2069 6620 6e6f 7420 6861 7361 7474     if not hasatt
-00000f20: 7228 7365 6c66 2c20 2762 7027 293a 0d0a  r(self, 'bp'):..
-00000f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f40: 7365 6c66 2e62 7020 3d20 4279 7061 7373  self.bp = Bypass
-00000f50: 5075 6d70 2873 656c 6629 0d0a 0d0a 2020  Pump(self)....  
-00000f60: 2020 2020 2020 7365 6c66 2e5f 6964 5f73        self._id_s
-00000f70: 7472 696e 6720 3d20 7265 706c 790d 0a20  tring = reply.. 
-00000f80: 2020 2020 2020 2073 656c 662e 5f6d 6f64         self._mod
-00000f90: 656c 5f6e 616d 6520 3d20 6d6f 6465 6c5f  el_name = model_
-00000fa0: 6e61 6d65 0d0a 2020 2020 2020 2020 7365  name..        se
-00000fb0: 6c66 2e5f 7365 7269 616c 5f6e 756d 6265  lf._serial_numbe
-00000fc0: 7220 3d20 7365 7269 616c 5f6e 756d 6265  r = serial_numbe
-00000fd0: 720d 0a20 2020 2020 2020 2073 656c 662e  r..        self.
-00000fe0: 5f66 6972 6d77 6172 655f 7665 7273 696f  _firmware_versio
-00000ff0: 6e20 3d20 6669 726d 7761 7265 5f76 6572  n = firmware_ver
-00001000: 7369 6f6e 0d0a 2020 2020 2020 2020 7265  sion..        re
-00001010: 7475 726e 2073 656c 662e 5f6d 6f64 656c  turn self._model
-00001020: 5f6e 616d 652c 2073 656c 662e 5f73 6572  _name, self._ser
-00001030: 6961 6c5f 6e75 6d62 6572 2c20 7365 6c66  ial_number, self
-00001040: 2e5f 6669 726d 7761 7265 5f76 6572 7369  ._firmware_versi
-00001050: 6f6e 0d0a 2020 2020 2020 2020 0d0a 2020  on..        ..  
-00001060: 2020 6465 6620 6765 745f 7374 6174 7573    def get_status
-00001070: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
-00001080: 2072 6574 7572 6e20 7365 6c66 2e73 7461   return self.sta
-00001090: 7475 732e 6765 745f 7374 6174 7573 5f74  tus.get_status_t
-000010a0: 6578 7428 290d 0a0d 0a20 2020 2064 6566  ext()....    def
-000010b0: 2072 6573 6574 2873 656c 6629 3a0d 0a20   reset(self):.. 
-000010c0: 2020 2020 2020 2073 656c 662e 636f 6d6d         self.comm
-000010d0: 2e73 656e 6428 275a 5253 5427 290d 0a0d  .send('ZRST')...
-000010e0: 0a20 2020 2064 6566 2068 616e 646c 655f  .    def handle_
-000010f0: 636f 6d6d 616e 6428 7365 6c66 2c20 636d  command(self, cm
-00001100: 645f 7374 7269 6e67 3a20 7374 7229 3a0d  d_string: str):.
-00001110: 0a20 2020 2020 2020 2063 6d64 203d 2063  .        cmd = c
-00001120: 6d64 5f73 7472 696e 672e 7570 7065 7228  md_string.upper(
-00001130: 290d 0a20 2020 2020 2020 2072 6570 6c79  )..        reply
-00001140: 203d 2027 270d 0a20 2020 2020 2020 2069   = ''..        i
-00001150: 6620 273f 2720 696e 2063 6d64 206f 7220  f '?' in cmd or 
-00001160: 636d 642e 7374 6172 7473 7769 7468 2822  cmd.startswith("
-00001170: 464c 2229 206f 7220 636d 642e 7374 6172  FL") or cmd.star
-00001180: 7473 7769 7468 2822 4856 2229 206f 7220  tswith("HV") or 
-00001190: 5c0d 0a20 2020 2020 2020 2020 2020 2020  \..             
-000011a0: 2020 2063 6d64 2e73 7461 7274 7377 6974     cmd.startswit
-000011b0: 6828 2256 4622 2920 6f72 2063 6d64 2e73  h("VF") or cmd.s
-000011c0: 7461 7274 7377 6974 6828 2245 4522 2920  tartswith("EE") 
-000011d0: 6f72 205c 0d0a 2020 2020 2020 2020 2020  or \..          
-000011e0: 2020 2020 2020 636d 642e 7374 6172 7473        cmd.starts
-000011f0: 7769 7468 2822 4945 2229 206f 7220 636d  with("IE") or cm
-00001200: 642e 7374 6172 7473 7769 7468 2822 494e  d.startswith("IN
-00001210: 2229 3a0d 0a20 2020 2020 2020 2020 2020  "):..           
-00001220: 2072 6570 6c79 203d 2073 656c 662e 7175   reply = self.qu
-00001230: 6572 795f 7465 7874 2863 6d64 292e 7374  ery_text(cmd).st
-00001240: 7269 7028 290d 0a20 2020 2020 2020 2065  rip()..        e
-00001250: 6c69 6620 636d 642e 7374 6172 7473 7769  lif cmd.startswi
-00001260: 7468 2822 4d52 2229 3a0d 0a20 2020 2020  th("MR"):..     
-00001270: 2020 2020 2020 2023 2073 656c 662e 7365         # self.se
-00001280: 6e64 2863 6d64 290d 0a20 2020 2020 2020  nd(cmd)..       
-00001290: 2020 2020 2074 7279 3a0d 0a20 2020 2020       try:..     
-000012a0: 2020 2020 2020 2020 2020 206d 6173 7320             mass 
-000012b0: 3d20 696e 7428 636d 645b 323a 5d2e 7374  = int(cmd[2:].st
-000012c0: 7269 7028 2929 0d0a 2020 2020 2020 2020  rip())..        
-000012d0: 2020 2020 2020 2020 696e 7465 6e73 6974          intensit
-000012e0: 7920 3d20 7365 6c66 2e72 6761 2e73 6361  y = self.rga.sca
-000012f0: 6e2e 6765 745f 7369 6e67 6c65 5f6d 6173  n.get_single_mas
-00001300: 735f 7363 616e 286d 6173 7329 2020 2320  s_scan(mass)  # 
-00001310: 7265 6164 5f6c 6f6e 6728 290d 0a20 2020  read_long()..   
-00001320: 2020 2020 2020 2020 2020 2020 2072 6570               rep
-00001330: 6c79 203d 2073 7472 2869 6e74 656e 7369  ly = str(intensi
-00001340: 7479 290d 0a20 2020 2020 2020 2020 2020  ty)..           
-00001350: 2065 7863 6570 743a 0d0a 2020 2020 2020   except:..      
-00001360: 2020 2020 2020 2020 2020 7061 7373 0d0a            pass..
-00001370: 2020 2020 2020 2020 656c 6966 2063 6d64          elif cmd
-00001380: 2e73 7461 7274 7377 6974 6828 2253 4322  .startswith("SC"
-00001390: 2920 616e 6420 6c65 6e28 636d 6429 203c  ) and len(cmd) <
-000013a0: 2031 303a 0d0a 2020 2020 2020 2020 2020   10:..          
-000013b0: 2020 7365 6c66 2e72 6761 2e73 6361 6e2e    self.rga.scan.
-000013c0: 6765 745f 616e 616c 6f67 5f73 6361 6e28  get_analog_scan(
-000013d0: 290d 0a20 2020 2020 2020 2020 2020 2072  )..            r
-000013e0: 6570 6c79 203d 2022 5363 616e 2043 6f6d  eply = "Scan Com
-000013f0: 706c 6574 6564 220d 0a20 2020 2020 2020  pleted"..       
-00001400: 2065 6c69 6620 636d 642e 7374 6172 7473   elif cmd.starts
-00001410: 7769 7468 2822 4853 2229 3a0d 0a20 2020  with("HS"):..   
-00001420: 2020 2020 2020 2020 2073 656c 662e 7267           self.rg
-00001430: 612e 7363 616e 2e67 6574 5f68 6973 746f  a.scan.get_histo
-00001440: 6772 616d 5f73 6361 6e28 290d 0a20 2020  gram_scan()..   
-00001450: 2020 2020 2020 2020 2072 6570 6c79 203d           reply =
-00001460: 2022 5363 616e 2043 6f6d 706c 6574 6564   "Scan Completed
-00001470: 220d 0a20 2020 2020 2020 2065 6c73 653a  "..        else:
-00001480: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00001490: 6c66 2e73 656e 6428 636d 6429 0d0a 2020  lf.send(cmd)..  
-000014a0: 2020 2020 2020 7265 7475 726e 2072 6570        return rep
-000014b0: 6c79 0d0a 0d0a 0d0a 6966 205f 5f6e 616d  ly......if __nam
-000014c0: 655f 5f20 3d3d 2027 5f5f 6d61 696e 5f5f  e__ == '__main__
-000014d0: 273a 0d0a 2020 2020 7567 6120 3d20 5547  ':..    uga = UG
-000014e0: 4131 3030 2827 7463 7069 7027 2c20 2731  A100('tcpip', '1
-000014f0: 3732 2e32 352e 3132 382e 3133 272c 2027  72.25.128.13', '
-00001500: 7372 7375 6761 272c 2027 7372 7375 6761  srsuga', 'srsuga
-00001510: 2729 0d0a 2020 2020 7072 696e 7428 7567  ')..    print(ug
-00001520: 612e 7374 6174 7573 2e69 645f 7374 7269  a.status.id_stri
-00001530: 6e67 290d 0a0d 0a                        ng)....
+00000220: 2020 5247 412c 2049 6f6e 4761 7567 652c    RGA, IonGauge,
+00000230: 2020 4d75 6c74 6970 6c65 496e 6c65 742c    MultipleInlet,
+00000240: 205c 0d0a 2020 2020 2020 2020 2020 2020   \..            
+00000250: 2020 2020 2020 2020 2020 2020 5072 6573              Pres
+00000260: 7375 7265 2c20 4865 6174 6572 732c 2054  sure, Heaters, T
+00000270: 656d 7065 7261 7475 7265 2c20 5c0d 0a20  emperature, \.. 
+00000280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000290: 2020 2020 2020 2045 7468 6572 6e65 742c         Ethernet,
+000002a0: 2053 7461 7475 732c 204d 6f64 650d 0a66   Status, Mode..f
+000002b0: 726f 6d20 2e6b 6579 7320 696d 706f 7274  rom .keys import
+000002c0: 204b 6579 730d 0a0d 0a0d 0a63 6c61 7373   Keys......class
+000002d0: 2055 4741 3130 3028 496e 7374 7275 6d65   UGA100(Instrume
+000002e0: 6e74 293a 0d0a 2020 2020 5f49 6453 7472  nt):..    _IdStr
+000002f0: 696e 6720 3d20 2753 5253 5f55 4741 270d  ing = 'SRS_UGA'.
+00000300: 0a20 2020 205f 7465 726d 5f63 6861 7220  .    _term_char 
+00000310: 3d20 6227 5c72 270d 0a0d 0a20 2020 2061  = b'\r'....    a
+00000320: 7661 696c 6162 6c65 5f69 6e74 6572 6661  vailable_interfa
+00000330: 6365 7320 3d20 5b0d 0a20 2020 2020 2020  ces = [..       
+00000340: 205b 2020 2053 6572 6961 6c49 6e74 6572   [   SerialInter
+00000350: 6661 6365 2c0d 0a20 2020 2020 2020 2020  face,..         
+00000360: 2020 207b 0d0a 2020 2020 2020 2020 2020     {..          
+00000370: 2020 2020 2020 2770 6f72 7427 3a20 4669        'port': Fi
+00000380: 6e64 4c69 7374 496e 7075 7428 292c 0d0a  ndListInput(),..
+00000390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000003a0: 2762 6175 645f 7261 7465 273a 2049 6e74  'baud_rate': Int
+000003b0: 6567 6572 4c69 7374 496e 7075 7428 5b32  egerListInput([2
+000003c0: 3838 3030 2c20 3338 3430 305d 292c 0d0a  8800, 38400]),..
+000003d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000003e0: 2768 6172 6477 6172 655f 666c 6f77 5f63  'hardware_flow_c
+000003f0: 6f6e 7472 6f6c 273a 2054 7275 650d 0a20  ontrol': True.. 
+00000400: 2020 2020 2020 2020 2020 207d 0d0a 2020             }..  
+00000410: 2020 2020 2020 5d2c 0d0a 2020 2020 2020        ],..      
+00000420: 2020 5b20 2020 5463 7069 7049 6e74 6572    [   TcpipInter
+00000430: 6661 6365 2c0d 0a20 2020 2020 2020 2020  face,..         
+00000440: 2020 207b 0d0a 2020 2020 2020 2020 2020     {..          
+00000450: 2020 2020 2020 2769 705f 6164 6472 6573        'ip_addres
+00000460: 7327 3a20 4970 3449 6e70 7574 2827 3139  s': Ip4Input('19
+00000470: 322e 3136 382e 312e 3130 2729 2c0d 0a20  2.168.1.10'),.. 
+00000480: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00000490: 7573 6572 5f69 6427 3a20 5374 7269 6e67  user_id': String
+000004a0: 496e 7075 7428 2773 7273 7567 6127 292c  Input('srsuga'),
+000004b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000004c0: 2020 2770 6173 7377 6f72 6427 3a20 5061    'password': Pa
+000004d0: 7373 776f 7264 496e 7075 7428 2773 7273  sswordInput('srs
+000004e0: 7567 6127 292c 0d0a 2020 2020 2020 2020  uga'),..        
+000004f0: 2020 2020 2020 2020 2770 6f72 7427 3a20          'port': 
+00000500: 3831 380d 0a20 2020 2020 2020 2020 2020  818..           
+00000510: 207d 0d0a 2020 2020 2020 2020 5d0d 0a20   }..        ].. 
+00000520: 2020 205d 0d0a 0d0a 2020 2020 6465 6620     ]....    def 
+00000530: 5f5f 696e 6974 5f5f 2873 656c 662c 2069  __init__(self, i
+00000540: 6e74 6572 6661 6365 5f74 7970 653d 4e6f  nterface_type=No
+00000550: 6e65 2c20 2a61 7267 7329 3a0d 0a20 2020  ne, *args):..   
+00000560: 2020 2020 2073 7570 6572 2829 2e5f 5f69       super().__i
+00000570: 6e69 745f 5f28 696e 7465 7266 6163 655f  nit__(interface_
+00000580: 7479 7065 2c20 2a61 7267 7329 0d0a 0d0a  type, *args)....
+00000590: 2020 2020 2020 2020 7365 6c66 2e6d 6f64          self.mod
+000005a0: 6520 3d20 4d6f 6465 2873 656c 6629 0d0a  e = Mode(self)..
+000005b0: 2020 2020 2020 2020 7365 6c66 2e62 7020          self.bp 
+000005c0: 3d20 4279 7061 7373 5075 6d70 2873 656c  = BypassPump(sel
+000005d0: 6629 0d0a 2020 2020 2020 2020 7365 6c66  f)..        self
+000005e0: 2e72 7020 3d20 526f 7567 6869 6e67 5075  .rp = RoughingPu
+000005f0: 6d70 2873 656c 6629 0d0a 2020 2020 2020  mp(self)..      
+00000600: 2020 7365 6c66 2e74 7020 3d20 5475 7262    self.tp = Turb
+00000610: 6f50 756d 7028 7365 6c66 290d 0a20 2020  oPump(self)..   
+00000620: 2020 2020 2073 656c 662e 6276 203d 2042       self.bv = B
+00000630: 7970 6173 7356 616c 7665 2873 656c 6629  ypassValve(self)
+00000640: 0d0a 2020 2020 2020 2020 7365 6c66 2e73  ..        self.s
+00000650: 7620 3d20 5361 6d70 6c65 5661 6c76 6528  v = SampleValve(
+00000660: 7365 6c66 290d 0a20 2020 2020 2020 2073  self)..        s
+00000670: 656c 662e 7676 203d 2056 656e 7456 616c  elf.vv = VentVal
+00000680: 7665 2873 656c 6629 0d0a 2020 2020 2020  ve(self)..      
+00000690: 2020 7365 6c66 2e72 6761 203d 2052 4741    self.rga = RGA
+000006a0: 2873 656c 6629 0d0a 2020 2020 2020 2020  (self)..        
+000006b0: 7365 6c66 2e69 6720 3d20 496f 6e47 6175  self.ig = IonGau
+000006c0: 6765 2873 656c 6629 0d0a 2020 2020 2020  ge(self)..      
+000006d0: 2020 7365 6c66 2e6d 6920 3d20 4d75 6c74    self.mi = Mult
+000006e0: 6970 6c65 496e 6c65 7428 7365 6c66 290d  ipleInlet(self).
+000006f0: 0a20 2020 2020 2020 2073 656c 662e 6874  .        self.ht
+00000700: 203d 2048 6561 7465 7273 2873 656c 6629   = Heaters(self)
+00000710: 0d0a 0d0a 2020 2020 2020 2020 7365 6c66  ....        self
+00000720: 2e74 656d 7065 7261 7475 7265 203d 2054  .temperature = T
+00000730: 656d 7065 7261 7475 7265 2873 656c 6629  emperature(self)
+00000740: 0d0a 2020 2020 2020 2020 7365 6c66 2e70  ..        self.p
+00000750: 7265 7373 7572 6520 3d20 5072 6573 7375  ressure = Pressu
+00000760: 7265 2873 656c 6629 0d0a 2020 2020 2020  re(self)..      
+00000770: 2020 7365 6c66 2e65 7468 6572 6e65 7420    self.ethernet 
+00000780: 3d20 4574 6865 726e 6574 2873 656c 6629  = Ethernet(self)
+00000790: 0d0a 2020 2020 2020 2020 7365 6c66 2e73  ..        self.s
+000007a0: 7461 7475 7320 3d20 5374 6174 7573 2873  tatus = Status(s
+000007b0: 656c 6629 0d0a 0d0a 2020 2020 6465 6620  elf)....    def 
+000007c0: 6368 6563 6b5f 6964 2873 656c 6629 3a0d  check_id(self):.
+000007d0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+000007e0: 7365 6c66 2e69 735f 636f 6e6e 6563 7465  self.is_connecte
+000007f0: 6428 293a 0d0a 2020 2020 2020 2020 2020  d():..          
+00000800: 2020 7265 7475 726e 204e 6f6e 652c 204e    return None, N
+00000810: 6f6e 652c 204e 6f6e 650d 0a0d 0a20 2020  one, None....   
+00000820: 2020 2020 2072 6570 6c79 203d 2073 656c       reply = sel
+00000830: 662e 7175 6572 795f 7465 7874 2827 5a51  f.query_text('ZQ
+00000840: 4944 3f27 292e 7374 7269 7028 290d 0a20  ID?').strip().. 
+00000850: 2020 2020 2020 2073 7472 696e 6773 203d         strings =
+00000860: 2072 6570 6c79 2e73 706c 6974 2827 2c27   reply.split(','
+00000870: 290d 0a0d 0a20 2020 2020 2020 2069 6620  )....        if 
+00000880: 6c65 6e28 7374 7269 6e67 7329 2021 3d20  len(strings) != 
+00000890: 333a 0d0a 2020 2020 2020 2020 2020 2020  3:..            
+000008a0: 7265 7475 726e 204e 6f6e 652c 204e 6f6e  return None, Non
+000008b0: 652c 204e 6f6e 650d 0a0d 0a20 2020 2020  e, None....     
+000008c0: 2020 206d 6f64 656c 5f6e 616d 6520 3d20     model_name = 
+000008d0: 7374 7269 6e67 735b 305d 2e73 7472 6970  strings[0].strip
+000008e0: 2829 0d0a 2020 2020 2020 2020 7365 7269  ()..        seri
+000008f0: 616c 5f6e 756d 6265 7220 3d20 7374 7269  al_number = stri
+00000900: 6e67 735b 315d 2e73 7472 6970 2829 5b34  ngs[1].strip()[4
+00000910: 3a5d 0d0a 2020 2020 2020 2020 6669 726d  :]..        firm
+00000920: 7761 7265 5f76 6572 7369 6f6e 203d 2073  ware_version = s
+00000930: 7472 696e 6773 5b32 5d2e 7374 7269 7028  trings[2].strip(
+00000940: 295b 323a 5d0d 0a0d 0a20 2020 2020 2020  )[2:]....       
+00000950: 2069 6620 7365 6c66 2e5f 4964 5374 7269   if self._IdStri
+00000960: 6e67 206e 6f74 2069 6e20 7265 706c 793a  ng not in reply:
+00000970: 0d0a 2020 2020 2020 2020 2020 2020 7261  ..            ra
+00000980: 6973 6520 496e 7374 4964 4572 726f 7228  ise InstIdError(
+00000990: 2249 6e76 616c 6964 2069 6e73 7472 756d  "Invalid instrum
+000009a0: 656e 743a 207b 7d20 6e6f 7420 696e 207b  ent: {} not in {
+000009b0: 7d22 0d0a 2020 2020 2020 2020 2020 2020  }"..            
+000009c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000009d0: 2020 2e66 6f72 6d61 7428 7365 6c66 2e5f    .format(self._
+000009e0: 4964 5374 7269 6e67 2c20 7265 706c 7929  IdString, reply)
+000009f0: 290d 0a20 2020 2020 2020 2069 6620 7365  )..        if se
+00000a00: 6c66 2e72 6761 2e73 7461 7465 203d 3d20  lf.rga.state == 
+00000a10: 4b65 7973 2e4f 6e3a 0d0a 2020 2020 2020  Keys.On:..      
+00000a20: 2020 2020 2020 7365 6c66 2e72 6761 2e63        self.rga.c
+00000a30: 6865 636b 5f69 6428 2920 2023 2063 6f6e  heck_id()  # con
+00000a40: 6669 6775 7265 2052 4741 0d0a 0d0a 2020  figure RGA....  
+00000a50: 2020 2020 2020 6966 2027 5547 415f 4854        if 'UGA_HT
+00000a60: 2720 696e 206d 6f64 656c 5f6e 616d 653a  ' in model_name:
+00000a70: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00000a80: 2068 6173 6174 7472 2873 656c 662c 2027   hasattr(self, '
+00000a90: 6276 2729 3a0d 0a20 2020 2020 2020 2020  bv'):..         
+00000aa0: 2020 2020 2020 2064 656c 2073 656c 662e         del self.
+00000ab0: 6276 0d0a 2020 2020 2020 2020 2020 2020  bv..            
+00000ac0: 6966 2068 6173 6174 7472 2873 656c 662c  if hasattr(self,
+00000ad0: 2027 7376 2729 3a0d 0a20 2020 2020 2020   'sv'):..       
+00000ae0: 2020 2020 2020 2020 2064 656c 2073 656c           del sel
+00000af0: 662e 7376 0d0a 2020 2020 2020 2020 2020  f.sv..          
+00000b00: 2020 6966 2068 6173 6174 7472 2873 656c    if hasattr(sel
+00000b10: 662c 2027 6d69 2729 3a0d 0a20 2020 2020  f, 'mi'):..     
+00000b20: 2020 2020 2020 2020 2020 2064 656c 2073             del s
+00000b30: 656c 662e 6d69 0d0a 2020 2020 2020 2020  elf.mi..        
+00000b40: 2020 2020 6966 206e 6f74 2068 6173 6174      if not hasat
+00000b50: 7472 2873 656c 662c 2027 6270 2729 3a0d  tr(self, 'bp'):.
+00000b60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000b70: 2073 656c 662e 6270 203d 2042 7970 6173   self.bp = Bypas
+00000b80: 7350 756d 7028 7365 6c66 290d 0a20 2020  sPump(self)..   
+00000b90: 2020 2020 2065 6c69 6620 2755 4741 5f4c       elif 'UGA_L
+00000ba0: 5427 2069 6e20 6d6f 6465 6c5f 6e61 6d65  T' in model_name
+00000bb0: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
+00000bc0: 6620 6e6f 7420 6861 7361 7474 7228 7365  f not hasattr(se
+00000bd0: 6c66 2c20 2762 7627 293a 0d0a 2020 2020  lf, 'bv'):..    
+00000be0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00000bf0: 2e62 7620 3d20 4279 7061 7373 5661 6c76  .bv = BypassValv
+00000c00: 6528 7365 6c66 290d 0a20 2020 2020 2020  e(self)..       
+00000c10: 2020 2020 2069 6620 6e6f 7420 6861 7361       if not hasa
+00000c20: 7474 7228 7365 6c66 2c20 2773 7627 293a  ttr(self, 'sv'):
+00000c30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000c40: 2020 7365 6c66 2e73 7620 3d20 5361 6d70    self.sv = Samp
+00000c50: 6c65 5661 6c76 6528 7365 6c66 290d 0a20  leValve(self).. 
+00000c60: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+00000c70: 7420 6861 7361 7474 7228 7365 6c66 2c20  t hasattr(self, 
+00000c80: 276d 6927 293a 0d0a 2020 2020 2020 2020  'mi'):..        
+00000c90: 2020 2020 2020 2020 7365 6c66 2e6d 6920          self.mi 
+00000ca0: 3d20 4d75 6c74 6970 6c65 496e 6c65 7428  = MultipleInlet(
+00000cb0: 7365 6c66 290d 0a20 2020 2020 2020 2020  self)..         
+00000cc0: 2020 2069 6620 6861 7361 7474 7228 7365     if hasattr(se
+00000cd0: 6c66 2c20 2762 7027 293a 0d0a 2020 2020  lf, 'bp'):..    
+00000ce0: 2020 2020 2020 2020 2020 2020 6465 6c20              del 
+00000cf0: 7365 6c66 2e62 700d 0a20 2020 2020 2020  self.bp..       
+00000d00: 2065 6c69 6620 2755 4741 5f50 4d27 2069   elif 'UGA_PM' i
+00000d10: 6e20 6d6f 6465 6c5f 6e61 6d65 3a0d 0a20  n model_name:.. 
+00000d20: 2020 2020 2020 2020 2020 2069 6620 6861             if ha
+00000d30: 7361 7474 7228 7365 6c66 2c20 2762 7627  sattr(self, 'bv'
+00000d40: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00000d50: 2020 2020 6465 6c20 7365 6c66 2e62 760d      del self.bv.
+00000d60: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00000d70: 6e6f 7420 6861 7361 7474 7228 7365 6c66  not hasattr(self
+00000d80: 2c20 2773 7627 293a 0d0a 2020 2020 2020  , 'sv'):..      
+00000d90: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+00000da0: 7620 3d20 5361 6d70 6c65 5661 6c76 6528  v = SampleValve(
+00000db0: 7365 6c66 290d 0a20 2020 2020 2020 2020  self)..         
+00000dc0: 2020 2069 6620 6e6f 7420 6861 7361 7474     if not hasatt
+00000dd0: 7228 7365 6c66 2c20 276d 6927 293a 0d0a  r(self, 'mi'):..
+00000de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000df0: 7365 6c66 2e6d 6920 3d20 4d75 6c74 6970  self.mi = Multip
+00000e00: 6c65 496e 6c65 7428 7365 6c66 290d 0a20  leInlet(self).. 
+00000e10: 2020 2020 2020 2020 2020 2069 6620 6861             if ha
+00000e20: 7361 7474 7228 7365 6c66 2c20 2762 7027  sattr(self, 'bp'
+00000e30: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00000e40: 2020 2020 6465 6c20 7365 6c66 2e62 700d      del self.bp.
+00000e50: 0a20 2020 2020 2020 2065 6c69 6620 2755  .        elif 'U
+00000e60: 4741 2720 696e 206d 6f64 656c 5f6e 616d  GA' in model_nam
+00000e70: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00000e80: 6966 206e 6f74 2068 6173 6174 7472 2873  if not hasattr(s
+00000e90: 656c 662c 2027 6276 2729 3a0d 0a20 2020  elf, 'bv'):..   
+00000ea0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00000eb0: 662e 6276 203d 2042 7970 6173 7356 616c  f.bv = BypassVal
+00000ec0: 7665 2873 656c 6629 0d0a 2020 2020 2020  ve(self)..      
+00000ed0: 2020 2020 2020 6966 206e 6f74 2068 6173        if not has
+00000ee0: 6174 7472 2873 656c 662c 2027 7376 2729  attr(self, 'sv')
+00000ef0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00000f00: 2020 2073 656c 662e 7376 203d 2053 616d     self.sv = Sam
+00000f10: 706c 6556 616c 7665 2873 656c 6629 0d0a  pleValve(self)..
+00000f20: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+00000f30: 6f74 2068 6173 6174 7472 2873 656c 662c  ot hasattr(self,
+00000f40: 2027 6d69 2729 3a0d 0a20 2020 2020 2020   'mi'):..       
+00000f50: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
+00000f60: 203d 204d 756c 7469 706c 6549 6e6c 6574   = MultipleInlet
+00000f70: 2873 656c 6629 0d0a 2020 2020 2020 2020  (self)..        
+00000f80: 2020 2020 6966 206e 6f74 2068 6173 6174      if not hasat
+00000f90: 7472 2873 656c 662c 2027 6270 2729 3a0d  tr(self, 'bp'):.
+00000fa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000fb0: 2073 656c 662e 6270 203d 2042 7970 6173   self.bp = Bypas
+00000fc0: 7350 756d 7028 7365 6c66 290d 0a0d 0a20  sPump(self).... 
+00000fd0: 2020 2020 2020 2073 656c 662e 5f69 645f         self._id_
+00000fe0: 7374 7269 6e67 203d 2072 6570 6c79 0d0a  string = reply..
+00000ff0: 2020 2020 2020 2020 7365 6c66 2e5f 6d6f          self._mo
+00001000: 6465 6c5f 6e61 6d65 203d 206d 6f64 656c  del_name = model
+00001010: 5f6e 616d 650d 0a20 2020 2020 2020 2073  _name..        s
+00001020: 656c 662e 5f73 6572 6961 6c5f 6e75 6d62  elf._serial_numb
+00001030: 6572 203d 2073 6572 6961 6c5f 6e75 6d62  er = serial_numb
+00001040: 6572 0d0a 2020 2020 2020 2020 7365 6c66  er..        self
+00001050: 2e5f 6669 726d 7761 7265 5f76 6572 7369  ._firmware_versi
+00001060: 6f6e 203d 2066 6972 6d77 6172 655f 7665  on = firmware_ve
+00001070: 7273 696f 6e0d 0a20 2020 2020 2020 2072  rsion..        r
+00001080: 6574 7572 6e20 7365 6c66 2e5f 6d6f 6465  eturn self._mode
+00001090: 6c5f 6e61 6d65 2c20 7365 6c66 2e5f 7365  l_name, self._se
+000010a0: 7269 616c 5f6e 756d 6265 722c 2073 656c  rial_number, sel
+000010b0: 662e 5f66 6972 6d77 6172 655f 7665 7273  f._firmware_vers
+000010c0: 696f 6e0d 0a20 2020 2020 2020 200d 0a20  ion..        .. 
+000010d0: 2020 2064 6566 2067 6574 5f73 7461 7475     def get_statu
+000010e0: 7328 7365 6c66 293a 0d0a 2020 2020 2020  s(self):..      
+000010f0: 2020 7265 7475 726e 2073 656c 662e 7374    return self.st
+00001100: 6174 7573 2e67 6574 5f73 7461 7475 735f  atus.get_status_
+00001110: 7465 7874 2829 0d0a 0d0a 2020 2020 6465  text()....    de
+00001120: 6620 7265 7365 7428 7365 6c66 293a 0d0a  f reset(self):..
+00001130: 2020 2020 2020 2020 7365 6c66 2e63 6f6d          self.com
+00001140: 6d2e 7365 6e64 2827 5a52 5354 2729 0d0a  m.send('ZRST')..
+00001150: 0d0a 2020 2020 6465 6620 6861 6e64 6c65  ..    def handle
+00001160: 5f63 6f6d 6d61 6e64 2873 656c 662c 2063  _command(self, c
+00001170: 6d64 5f73 7472 696e 673a 2073 7472 293a  md_string: str):
+00001180: 0d0a 2020 2020 2020 2020 636d 6420 3d20  ..        cmd = 
+00001190: 636d 645f 7374 7269 6e67 2e75 7070 6572  cmd_string.upper
+000011a0: 2829 0d0a 2020 2020 2020 2020 7265 706c  ()..        repl
+000011b0: 7920 3d20 2727 0d0a 2020 2020 2020 2020  y = ''..        
+000011c0: 6966 2027 3f27 2069 6e20 636d 6420 6f72  if '?' in cmd or
+000011d0: 2063 6d64 2e73 7461 7274 7377 6974 6828   cmd.startswith(
+000011e0: 2246 4c22 2920 6f72 2063 6d64 2e73 7461  "FL") or cmd.sta
+000011f0: 7274 7377 6974 6828 2248 5622 2920 6f72  rtswith("HV") or
+00001200: 205c 0d0a 2020 2020 2020 2020 2020 2020   \..            
+00001210: 2020 2020 636d 642e 7374 6172 7473 7769      cmd.startswi
+00001220: 7468 2822 5646 2229 206f 7220 636d 642e  th("VF") or cmd.
+00001230: 7374 6172 7473 7769 7468 2822 4545 2229  startswith("EE")
+00001240: 206f 7220 5c0d 0a20 2020 2020 2020 2020   or \..         
+00001250: 2020 2020 2020 2063 6d64 2e73 7461 7274         cmd.start
+00001260: 7377 6974 6828 2249 4522 2920 6f72 2063  swith("IE") or c
+00001270: 6d64 2e73 7461 7274 7377 6974 6828 2249  md.startswith("I
+00001280: 4e22 293a 0d0a 2020 2020 2020 2020 2020  N"):..          
+00001290: 2020 7265 706c 7920 3d20 7365 6c66 2e71    reply = self.q
+000012a0: 7565 7279 5f74 6578 7428 636d 6429 2e73  uery_text(cmd).s
+000012b0: 7472 6970 2829 0d0a 2020 2020 2020 2020  trip()..        
+000012c0: 656c 6966 2063 6d64 2e73 7461 7274 7377  elif cmd.startsw
+000012d0: 6974 6828 224d 5222 293a 0d0a 2020 2020  ith("MR"):..    
+000012e0: 2020 2020 2020 2020 2320 7365 6c66 2e73          # self.s
+000012f0: 656e 6428 636d 6429 0d0a 2020 2020 2020  end(cmd)..      
+00001300: 2020 2020 2020 7472 793a 0d0a 2020 2020        try:..    
+00001310: 2020 2020 2020 2020 2020 2020 6d61 7373              mass
+00001320: 203d 2069 6e74 2863 6d64 5b32 3a5d 2e73   = int(cmd[2:].s
+00001330: 7472 6970 2829 290d 0a20 2020 2020 2020  trip())..       
+00001340: 2020 2020 2020 2020 2069 6e74 656e 7369           intensi
+00001350: 7479 203d 2073 656c 662e 7267 612e 7363  ty = self.rga.sc
+00001360: 616e 2e67 6574 5f73 696e 676c 655f 6d61  an.get_single_ma
+00001370: 7373 5f73 6361 6e28 6d61 7373 2920 2023  ss_scan(mass)  #
+00001380: 2072 6561 645f 6c6f 6e67 2829 0d0a 2020   read_long()..  
+00001390: 2020 2020 2020 2020 2020 2020 2020 7265                re
+000013a0: 706c 7920 3d20 7374 7228 696e 7465 6e73  ply = str(intens
+000013b0: 6974 7929 0d0a 2020 2020 2020 2020 2020  ity)..          
+000013c0: 2020 6578 6365 7074 3a0d 0a20 2020 2020    except:..     
+000013d0: 2020 2020 2020 2020 2020 2070 6173 730d             pass.
+000013e0: 0a20 2020 2020 2020 2065 6c69 6620 636d  .        elif cm
+000013f0: 642e 7374 6172 7473 7769 7468 2822 5343  d.startswith("SC
+00001400: 2229 2061 6e64 206c 656e 2863 6d64 2920  ") and len(cmd) 
+00001410: 3c20 3130 3a0d 0a20 2020 2020 2020 2020  < 10:..         
+00001420: 2020 2073 656c 662e 7267 612e 7363 616e     self.rga.scan
+00001430: 2e67 6574 5f61 6e61 6c6f 675f 7363 616e  .get_analog_scan
+00001440: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
+00001450: 7265 706c 7920 3d20 2253 6361 6e20 436f  reply = "Scan Co
+00001460: 6d70 6c65 7465 6422 0d0a 2020 2020 2020  mpleted"..      
+00001470: 2020 656c 6966 2063 6d64 2e73 7461 7274    elif cmd.start
+00001480: 7377 6974 6828 2248 5322 293a 0d0a 2020  swith("HS"):..  
+00001490: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
+000014a0: 6761 2e73 6361 6e2e 6765 745f 6869 7374  ga.scan.get_hist
+000014b0: 6f67 7261 6d5f 7363 616e 2829 0d0a 2020  ogram_scan()..  
+000014c0: 2020 2020 2020 2020 2020 7265 706c 7920            reply 
+000014d0: 3d20 2253 6361 6e20 436f 6d70 6c65 7465  = "Scan Complete
+000014e0: 6422 0d0a 2020 2020 2020 2020 656c 7365  d"..        else
+000014f0: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
+00001500: 656c 662e 7365 6e64 2863 6d64 290d 0a20  elf.send(cmd).. 
+00001510: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+00001520: 706c 790d 0a0d 0a0d 0a69 6620 5f5f 6e61  ply......if __na
+00001530: 6d65 5f5f 203d 3d20 275f 5f6d 6169 6e5f  me__ == '__main_
+00001540: 5f27 3a0d 0a20 2020 2075 6761 203d 2055  _':..    uga = U
+00001550: 4741 3130 3028 2774 6370 6970 272c 2027  GA100('tcpip', '
+00001560: 3137 322e 3235 2e31 3238 2e31 3327 2c20  172.25.128.13', 
+00001570: 2773 7273 7567 6127 2c20 2773 7273 7567  'srsuga', 'srsug
+00001580: 6127 290d 0a20 2020 2070 7269 6e74 2875  a')..    print(u
+00001590: 6761 2e73 7461 7475 732e 6964 5f73 7472  ga.status.id_str
+000015a0: 696e 6729 0d0a 0d0a                      ing)....
```

### Comparing `srsinst.uga-0.0.1/srsinst/uga/tasks/ugamodecontroltask.py` & `srsinst.uga-0.0.2/srsinst/uga/tasks/ugamodecontroltask.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+##! 
+##! Coptright(c) 2023 Stanford Research Systems, All right reserved
+##! Subject to the MIT License
+##! 
 
 import time
 from srsinst.uga import Keys
 
 from srsgui import Task
 from srsgui.task.inputs import InstrumentInput, ListInput, IntegerInput
 from srsinst.uga import get_uga
@@ -27,15 +31,15 @@
 
     def setup(self):
         self.logger = self.get_logger(__name__)
         self.params = self.get_all_input_parameters()
 
         self.uga = get_uga(self, self.params[self.InstrumentName])
         print(self.uga.status.id_string)
-        while self.uga.status.error != 0:
+        while self.uga.status.error != Keys.OK:
             pass
 
         self.immediate_state = self.uga.mode.state
         self.final_state = self.immediate_state
         self.logger.info('Current mode before changing: {}'.format(self.immediate_state))
 
     def test(self):
@@ -78,15 +82,15 @@
         elif self.params[self.ModeName] == Keys.SystemBakeOff:
             if self.uga.mode.state != Keys.SystemBake:
                 raise ValueError('SYSTEM BAKE is not on')
             self.uga.mode.bake = False
             self.immediate_state = Keys.Start
             self.final_state = Keys.Ready
 
-        error_code = self.uga.status.error
+        error_code = self.uga.status.error_number
         if error_code > 10:
             raise ValueError('Error "{}" when trying to change to  {}'
                              .format(self.uga.status.error_message[error_code], self.final_state))
         else:
             self.logger.info('UGA mode changing to {}'.format(self.final_state))
 
         self.display_device_info(device_name=self.params[self.InstrumentName], update=True)
```

### Comparing `srsinst.uga-0.0.1/srsinst/uga/tasks/ugamultiplottask.py` & `srsinst.uga-0.0.2/srsinst/uga/tasks/ugamultiplottask.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+##! 
+##! Coptright(c) 2023 Stanford Research Systems, All right reserved
+##! Subject to the MIT License
+##! 
+
 import time
 import numpy as np
 from srsgui import Task
 from srsgui.task.inputs import InstrumentInput, IntegerInput
 
 from srsinst.rga.plots.timeplot import TimePlot
 from srsinst.rga.plots.analogscanplot import AnalogScanPlot
```

### Comparing `srsinst.uga-0.0.1/srsinst/uga/tasks/ugastatemonitortask.py` & `srsinst.uga-0.0.2/srsinst/uga/tasks/ugastatemonitortask.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+##! 
+##! Coptright(c) 2023 Stanford Research Systems, All right reserved
+##! Subject to the MIT License
+##! 
+
 import time
 import numpy as np
 from srsgui import Task
 from srsgui import InstrumentInput, IntegerInput
 from srsinst.rga.plots.timeplot import TimePlot
 
 from srsinst.uga import get_uga
@@ -21,30 +26,30 @@
         self.logger = self.get_logger(__name__)
         self.params = self.get_all_input_parameters()
         self.uga = get_uga(self, self.params[self.InstrumentName])
 
         self.ax = self.figure.subplots(nrows=1, ncols=2, sharex=True)
 
         self.pressure_plot = TimePlot(self, self.ax[0], 'Pressure',
-            ['IG pressure', 'PG pressure', 'CM pressure'])
+            ['Ion Gauge', 'Pirani Gauge', 'CM Gauge'])
         self.pressure_plot.ax.set_yscale('log')
 
         self.temperature_plot = TimePlot(self, self.ax[1], 'Temperature',
-            ['Chamber Temperature', 'Elbow Temperature', 'Sample Inlet Temperature',
-             'Capillary Temperature', 'Turbo Pump Temperature'])
+            ['Chamber', 'Elbow', 'Sample Inlet',
+             'Capillary', 'Turbo Pump'])
 
     def test(self):
         while True:
             if not self.is_running():
                 break
 
             self.display_device_info(device_name=self.params[self.InstrumentName], update=True)
 
             self.pressure_plot.add_data([self.uga.ig.get_pressure(), self.uga.rp.get_pressure(),
-                         self.uga.bp.get_pressure()])
+                         self.uga.bp.get_pressure()], True)
 
             self.temperature_plot.add_data([self.uga.temperature.chamber, self.uga.temperature.elbow,
                          self.uga.temperature.sample_inlet, self.uga.temperature.capillary,
                          self.uga.temperature.turbo_pump], True)
 
             time.sleep(self.params[self.UpdatePeriod])
```

### Comparing `srsinst.uga-0.0.1/srsinst/uga/uga.taskconfig` & `srsinst.uga-0.0.2/srsinst/uga/uga.taskconfig`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 # Line that starts with '#' is a comment line
-# MyRGA Task list for srsgui
+# UGA Task list for srsgui
 
 # The name is used for the main window title
 
 Name: UGA Tasks
 
 # Specify Instruments used in the task suite
-# A line that starts with 'inst' adds an instrument to be used in the following tasks
-# an instrument is a subclass derived from Instrument class in 'rga' package
-# The second column is the Python module or package that contains the instrument class.
+# A line that starts with 'inst' adds an instrument to be used in the following tasks.
+# An instrument is a subclass derived from Instrument class in 'srsgui' package.
+# The second column is the name of the Python module or package that contains the instrument class.
 # The third column is a instrument class in the module
 # The fourth column is connection parameters.
-# if given, the instrument will be connected using the parameters when the config file is loaded.
+# If the fourth item is given, the instrument will be connected using the parameters 
+# when the config file is loaded.
 
 inst: uga,     srsinst.uga,    UGA100
 
-# inst: rga,     srsinst.rga,    RGA100
-# inst: uga2,   srsinst.uga,    UGA100,    tcpip:172.25.40.37:srsuga:srsuga:818
-# inst: uga3,  srsinst.uga,     UGA100,    serial:com3:28800:True
+# inst: rga,   srsinst.rga,    RGA100
+# inst: uga2,  srsinst.uga,    UGA100,    tcpip:172.25.40.37:srsuga:srsuga:818
+# inst: uga3,  srsinst.uga,    UGA100,    serial:com3:28800:True
 
 
-# A line that starts with 'task: ' adds a task to the task config file.
+# A line that starts with 'task: ' adds a task to the srsgui application.
 # The first column is the task name that will be used as a dictionary key
-# of the task, displayed in GUI Tak menu for selection, and used in task result data file.
-# The Second column is the Python module that contains the task class with relative path from the Task config file.
-# The third column is a task class  that is a Task subclass in the module.
-
-task: UGA State Monitor,       tasks.ugastatemonitortask,                UGAStateMonitorTask
-task: UGA Mode Control,        tasks.ugamodecontroltask,                 UGAModeControlTask
-# task: UGA Multi Plot,          tasks.ugamultiplottask,                   UGAMultiplotTask
+# of the task, displayed in GUI Tasks menu for selection, and used in task result data file.
+# The Second column is the name of the Python module that contains the task class 
+# with relative path from the Task config file.
+# The third column is the name of a Task subclass in the module.
 
+task: UGA State Monitor,         srsinst.uga.tasks.ugastatemonitortask,     UGAStateMonitorTask
+task: UGA Mode Control,          srsinst.uga.tasks.ugamodecontroltask,      UGAModeControlTask
+
+# Tasks from srsinst.rga
 task: Filament Control,          srsinst.rga.tasks.filamentcontroltask,     FilamentControlTask
 task: CEM Control,               srsinst.rga.tasks.cemcontroltask,          CEMControlTask
+task: CEM Gain Tuning,           srsinst.rga.tasks.cemgaintask,             CEMGainTask
 task: Analog Scan,               srsinst.rga.tasks.analogscantask,          AnalogScanTask
 task: Histogram Scan,            srsinst.rga.tasks.histogramscantask,       HistogramScanTask
 task: Pressure vs. Time Scan,    srsinst.rga.tasks.pvstscantask,            PvsTScanTask
 task: Derived P vs. T Scan,      srsinst.rga.tasks.derivedpvstscantask,     DerivedPvsTScanTask
 task: Composition analysis scan, srsinst.rga.tasks.compositionanalysistask, CompositionAnalysisTask
-task: CEM Gain Tuning,           srsinst.rga.tasks.cemgaintask,             CEMGainTask
+
```

### Comparing `srsinst.uga-0.0.1/srsinst.uga.egg-info/PKG-INFO` & `srsinst.uga-0.0.2/srsinst.uga.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srsinst.uga
-Version: 0.0.1
+Version: 0.0.2
 Summary: Instrument driver package for Universal Gas Analyzers (UGA) from Stanford Research Systems
 Author: Chulhoon Kim
 License: MIT license
 Keywords: UGA,universal gas analyzer,SRS,Stanford Research Systems
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -12,24 +12,26 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: full
-License-File: LICENSE.txt
+License-File: LICENSE
 
 # `srsinst.uga`
 
 `srsinst.uga` contains a Python instrument driver to control and acquire 
 mass spectra of atmospheric gas samples from 
 [Stanford Research Systems (SRS) Universal Gas Analyzer (UGA)](https://thinksrs.com/products/uga.html). It also has a collection of Python scripts 
-that runs on a graphic user interface (GUI) based on [srsgui](https://pypi.org/project/srsgui/).
+that runs on a graphic user interface (GUI) based on [srsgui](https://thinksrs.github.io/srsgui/).
 
 
+![screenshot](https://github.com/thinkSRS/srsinst.uga/blob/main/docs/_static/image/UGA100_composition_analysis_screenshot.png " ")
+
 ## Installation
 You need a working Python with `pip` (Python package installer) installed. If you don't,
 [install Python 3](https://realpython.com/installing-python/) to your system.
 
 To install `srsinst.uga` as an instrument driver only, use Python package installer `pip` 
 from the command line.
```

