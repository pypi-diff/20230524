# Comparing `tmp/pyflipper-0.15.tar.gz` & `tmp/pyflipper-0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyflipper-0.15.tar", last modified: Wed May 24 09:11:45 2023, max compression
+gzip compressed data, was "pyflipper-0.16.tar", last modified: Wed May 24 09:14:57 2023, max compression
```

## Comparing `pyflipper-0.15.tar` & `pyflipper-0.16.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 wh        (1000) users      (984)        0 2023-05-24 09:11:45.442517 pyflipper-0.15/
--rw-r--r--   0 wh        (1000) users      (984)     1063 2023-05-24 08:32:10.000000 pyflipper-0.15/LICENSE
--rw-r--r--   0 wh        (1000) users      (984)      900 2023-05-24 09:11:45.442517 pyflipper-0.15/PKG-INFO
--rw-r--r--   0 wh        (1000) users      (984)     8172 2023-05-24 08:32:10.000000 pyflipper-0.15/README.md
--rw-r--r--   0 wh        (1000) users      (984)      112 2023-05-24 09:11:45.442517 pyflipper-0.15/setup.cfg
--rw-r--r--   0 wh        (1000) users      (984)     1538 2023-05-24 09:11:40.000000 pyflipper-0.15/setup.py
-drwxr-xr-x   0 wh        (1000) users      (984)        0 2023-05-24 09:11:45.439183 pyflipper-0.15/src/
-drwxr-xr-x   0 wh        (1000) users      (984)        0 2023-05-24 09:11:45.439183 pyflipper-0.15/src/pyflipper/
--rw-r--r--   0 wh        (1000) users      (984)        0 2023-05-24 09:11:01.000000 pyflipper-0.15/src/pyflipper/__init__.py
-drwxr-xr-x   0 wh        (1000) users      (984)        0 2023-05-24 09:11:45.442517 pyflipper-0.15/src/pyflipper/lib/
--rw-r--r--   0 wh        (1000) users      (984)        0 2023-05-24 08:32:10.000000 pyflipper-0.15/src/pyflipper/lib/__init__.py
--rw-r--r--   0 wh        (1000) users      (984)      310 2023-05-24 08:32:10.000000 pyflipper-0.15/src/pyflipper/lib/bt.py
--rw-r--r--   0 wh        (1000) users      (984)      479 2023-05-24 08:32:10.000000 pyflipper-0.15/src/pyflipper/lib/date.py
--rw-r--r--   0 wh        (1000) users      (984)      251 2023-05-24 08:32:10.000000 pyflipper-0.15/src/pyflipper/lib/debug.py
--rw-r--r--   0 wh        (1000) users      (984)      557 2023-05-24 08:32:10.000000 pyflipper-0.15/src/pyflipper/lib/device_info.py
--rw-r--r--   0 wh        (1000) users      (984)      428 2023-05-24 08:32:10.000000 pyflipper-0.15/src/pyflipper/lib/free.py
--rw-r--r--   0 wh        (1000) users      (984)      511 2023-05-24 08:32:10.000000 pyflipper-0.15/src/pyflipper/lib/gpio.py
--rw-r--r--   0 wh        (1000) users      (984)      179 2023-05-24 08:32:10.000000 pyflipper-0.15/src/pyflipper/lib/i2c.py
--rw-r--r--   0 wh        (1000) users      (984)     1494 2023-05-24 08:32:10.000000 pyflipper-0.15/src/pyflipper/lib/ikey.py
--rw-r--r--   0 wh        (1000) users      (984)      672 2023-05-24 08:32:10.000000 pyflipper-0.15/src/pyflipper/lib/input.py
--rw-r--r--   0 wh        (1000) users      (984)     1912 2023-05-24 08:32:10.000000 pyflipper-0.15/src/pyflipper/lib/ir.py
--rw-r--r--   0 wh        (1000) users      (984)      908 2023-05-24 08:32:10.000000 pyflipper-0.15/src/pyflipper/lib/led.py
--rw-r--r--   0 wh        (1000) users      (984)      742 2023-05-24 08:32:10.000000 pyflipper-0.15/src/pyflipper/lib/loader.py
--rw-r--r--   0 wh        (1000) users      (984)      306 2023-05-24 08:32:10.000000 pyflipper-0.15/src/pyflipper/lib/log.py
--rw-r--r--   0 wh        (1000) users      (984)      485 2023-05-24 08:32:10.000000 pyflipper-0.15/src/pyflipper/lib/music_player.py
--rw-r--r--   0 wh        (1000) users      (984)     1136 2023-05-24 08:32:10.000000 pyflipper-0.15/src/pyflipper/lib/nfc.py
--rw-r--r--   0 wh        (1000) users      (984)      197 2023-05-24 08:32:10.000000 pyflipper-0.15/src/pyflipper/lib/onewire.py
--rw-r--r--   0 wh        (1000) users      (984)      628 2023-05-24 08:32:10.000000 pyflipper-0.15/src/pyflipper/lib/power.py
--rw-r--r--   0 wh        (1000) users      (984)      526 2023-05-24 08:32:10.000000 pyflipper-0.15/src/pyflipper/lib/ps.py
--rw-r--r--   0 wh        (1000) users      (984)     1604 2023-05-24 08:32:10.000000 pyflipper-0.15/src/pyflipper/lib/rfid.py
--rw-r--r--   0 wh        (1000) users      (984)     1535 2023-05-24 09:01:07.000000 pyflipper-0.15/src/pyflipper/lib/serial_wrapper.py
--rw-r--r--   0 wh        (1000) users      (984)     3039 2023-05-24 09:00:31.000000 pyflipper-0.15/src/pyflipper/lib/storage.py
--rw-r--r--   0 wh        (1000) users      (984)     1069 2023-05-24 08:32:10.000000 pyflipper-0.15/src/pyflipper/lib/subghz.py
--rw-r--r--   0 wh        (1000) users      (984)      766 2023-05-24 08:32:10.000000 pyflipper-0.15/src/pyflipper/lib/threaded.py
--rw-r--r--   0 wh        (1000) users      (984)      621 2023-05-24 08:32:10.000000 pyflipper-0.15/src/pyflipper/lib/update.py
--rw-r--r--   0 wh        (1000) users      (984)      150 2023-05-24 08:32:10.000000 pyflipper-0.15/src/pyflipper/lib/utils.py
--rw-r--r--   0 wh        (1000) users      (984)      428 2023-05-24 08:32:10.000000 pyflipper-0.15/src/pyflipper/lib/vibro.py
--rw-r--r--   0 wh        (1000) users      (984)     2540 2023-05-24 08:57:26.000000 pyflipper-0.15/src/pyflipper/pyflipper.py
-drwxr-xr-x   0 wh        (1000) users      (984)        0 2023-05-24 09:11:45.439183 pyflipper-0.15/src/pyflipper.egg-info/
--rw-r--r--   0 wh        (1000) users      (984)      900 2023-05-24 09:11:45.000000 pyflipper-0.15/src/pyflipper.egg-info/PKG-INFO
--rw-r--r--   0 wh        (1000) users      (984)     1015 2023-05-24 09:11:45.000000 pyflipper-0.15/src/pyflipper.egg-info/SOURCES.txt
--rw-r--r--   0 wh        (1000) users      (984)        1 2023-05-24 09:11:45.000000 pyflipper-0.15/src/pyflipper.egg-info/dependency_links.txt
--rw-r--r--   0 wh        (1000) users      (984)       26 2023-05-24 09:11:45.000000 pyflipper-0.15/src/pyflipper.egg-info/requires.txt
--rw-r--r--   0 wh        (1000) users      (984)       10 2023-05-24 09:11:45.000000 pyflipper-0.15/src/pyflipper.egg-info/top_level.txt
+drwxr-xr-x   0 wh        (1000) users      (984)        0 2023-05-24 09:14:57.479229 pyflipper-0.16/
+-rw-r--r--   0 wh        (1000) users      (984)     1063 2023-05-24 08:32:10.000000 pyflipper-0.16/LICENSE
+-rw-r--r--   0 wh        (1000) users      (984)      900 2023-05-24 09:14:57.479229 pyflipper-0.16/PKG-INFO
+-rw-r--r--   0 wh        (1000) users      (984)     8172 2023-05-24 08:32:10.000000 pyflipper-0.16/README.md
+-rw-r--r--   0 wh        (1000) users      (984)      112 2023-05-24 09:14:57.482562 pyflipper-0.16/setup.cfg
+-rw-r--r--   0 wh        (1000) users      (984)     1239 2023-05-24 09:14:47.000000 pyflipper-0.16/setup.py
+drwxr-xr-x   0 wh        (1000) users      (984)        0 2023-05-24 09:14:57.475896 pyflipper-0.16/src/
+drwxr-xr-x   0 wh        (1000) users      (984)        0 2023-05-24 09:14:57.475896 pyflipper-0.16/src/pyflipper/
+-rw-r--r--   0 wh        (1000) users      (984)        0 2023-05-24 09:11:01.000000 pyflipper-0.16/src/pyflipper/__init__.py
+drwxr-xr-x   0 wh        (1000) users      (984)        0 2023-05-24 09:14:57.479229 pyflipper-0.16/src/pyflipper/lib/
+-rw-r--r--   0 wh        (1000) users      (984)        0 2023-05-24 08:32:10.000000 pyflipper-0.16/src/pyflipper/lib/__init__.py
+-rw-r--r--   0 wh        (1000) users      (984)      310 2023-05-24 08:32:10.000000 pyflipper-0.16/src/pyflipper/lib/bt.py
+-rw-r--r--   0 wh        (1000) users      (984)      479 2023-05-24 08:32:10.000000 pyflipper-0.16/src/pyflipper/lib/date.py
+-rw-r--r--   0 wh        (1000) users      (984)      251 2023-05-24 08:32:10.000000 pyflipper-0.16/src/pyflipper/lib/debug.py
+-rw-r--r--   0 wh        (1000) users      (984)      557 2023-05-24 08:32:10.000000 pyflipper-0.16/src/pyflipper/lib/device_info.py
+-rw-r--r--   0 wh        (1000) users      (984)      428 2023-05-24 08:32:10.000000 pyflipper-0.16/src/pyflipper/lib/free.py
+-rw-r--r--   0 wh        (1000) users      (984)      511 2023-05-24 08:32:10.000000 pyflipper-0.16/src/pyflipper/lib/gpio.py
+-rw-r--r--   0 wh        (1000) users      (984)      179 2023-05-24 08:32:10.000000 pyflipper-0.16/src/pyflipper/lib/i2c.py
+-rw-r--r--   0 wh        (1000) users      (984)     1494 2023-05-24 08:32:10.000000 pyflipper-0.16/src/pyflipper/lib/ikey.py
+-rw-r--r--   0 wh        (1000) users      (984)      672 2023-05-24 08:32:10.000000 pyflipper-0.16/src/pyflipper/lib/input.py
+-rw-r--r--   0 wh        (1000) users      (984)     1912 2023-05-24 08:32:10.000000 pyflipper-0.16/src/pyflipper/lib/ir.py
+-rw-r--r--   0 wh        (1000) users      (984)      908 2023-05-24 08:32:10.000000 pyflipper-0.16/src/pyflipper/lib/led.py
+-rw-r--r--   0 wh        (1000) users      (984)      742 2023-05-24 08:32:10.000000 pyflipper-0.16/src/pyflipper/lib/loader.py
+-rw-r--r--   0 wh        (1000) users      (984)      306 2023-05-24 08:32:10.000000 pyflipper-0.16/src/pyflipper/lib/log.py
+-rw-r--r--   0 wh        (1000) users      (984)      485 2023-05-24 08:32:10.000000 pyflipper-0.16/src/pyflipper/lib/music_player.py
+-rw-r--r--   0 wh        (1000) users      (984)     1136 2023-05-24 08:32:10.000000 pyflipper-0.16/src/pyflipper/lib/nfc.py
+-rw-r--r--   0 wh        (1000) users      (984)      197 2023-05-24 08:32:10.000000 pyflipper-0.16/src/pyflipper/lib/onewire.py
+-rw-r--r--   0 wh        (1000) users      (984)      628 2023-05-24 08:32:10.000000 pyflipper-0.16/src/pyflipper/lib/power.py
+-rw-r--r--   0 wh        (1000) users      (984)      526 2023-05-24 08:32:10.000000 pyflipper-0.16/src/pyflipper/lib/ps.py
+-rw-r--r--   0 wh        (1000) users      (984)     1604 2023-05-24 08:32:10.000000 pyflipper-0.16/src/pyflipper/lib/rfid.py
+-rw-r--r--   0 wh        (1000) users      (984)     1535 2023-05-24 09:01:07.000000 pyflipper-0.16/src/pyflipper/lib/serial_wrapper.py
+-rw-r--r--   0 wh        (1000) users      (984)     3039 2023-05-24 09:00:31.000000 pyflipper-0.16/src/pyflipper/lib/storage.py
+-rw-r--r--   0 wh        (1000) users      (984)     1069 2023-05-24 08:32:10.000000 pyflipper-0.16/src/pyflipper/lib/subghz.py
+-rw-r--r--   0 wh        (1000) users      (984)      766 2023-05-24 08:32:10.000000 pyflipper-0.16/src/pyflipper/lib/threaded.py
+-rw-r--r--   0 wh        (1000) users      (984)      621 2023-05-24 08:32:10.000000 pyflipper-0.16/src/pyflipper/lib/update.py
+-rw-r--r--   0 wh        (1000) users      (984)      150 2023-05-24 08:32:10.000000 pyflipper-0.16/src/pyflipper/lib/utils.py
+-rw-r--r--   0 wh        (1000) users      (984)      428 2023-05-24 08:32:10.000000 pyflipper-0.16/src/pyflipper/lib/vibro.py
+-rw-r--r--   0 wh        (1000) users      (984)     2540 2023-05-24 08:57:26.000000 pyflipper-0.16/src/pyflipper/pyflipper.py
+drwxr-xr-x   0 wh        (1000) users      (984)        0 2023-05-24 09:14:57.475896 pyflipper-0.16/src/pyflipper.egg-info/
+-rw-r--r--   0 wh        (1000) users      (984)      900 2023-05-24 09:14:57.000000 pyflipper-0.16/src/pyflipper.egg-info/PKG-INFO
+-rw-r--r--   0 wh        (1000) users      (984)     1015 2023-05-24 09:14:57.000000 pyflipper-0.16/src/pyflipper.egg-info/SOURCES.txt
+-rw-r--r--   0 wh        (1000) users      (984)        1 2023-05-24 09:14:57.000000 pyflipper-0.16/src/pyflipper.egg-info/dependency_links.txt
+-rw-r--r--   0 wh        (1000) users      (984)       26 2023-05-24 09:14:57.000000 pyflipper-0.16/src/pyflipper.egg-info/requires.txt
+-rw-r--r--   0 wh        (1000) users      (984)       10 2023-05-24 09:14:57.000000 pyflipper-0.16/src/pyflipper.egg-info/top_level.txt
```

### Comparing `pyflipper-0.15/LICENSE` & `pyflipper-0.16/LICENSE`

 * *Files identical despite different names*

### Comparing `pyflipper-0.15/PKG-INFO` & `pyflipper-0.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyflipper
-Version: 0.15
+Version: 0.16
 Summary: Unoffical Flipper Zero cli wrapper
 Home-page: https://github.com/wh00hw/pyFlipper
 Author: wh00hw
 Author-email: white_rabbit@autistici.org
 License: MIT
 Project-URL: Documentation, https://github.com/wh00hw/pyFlipper/blob/master/README.md
 Project-URL: Bug Reports, https://github.com/wh00hw/pyFlipper/issues
```

### Comparing `pyflipper-0.15/README.md` & `pyflipper-0.16/README.md`

 * *Files identical despite different names*

### Comparing `pyflipper-0.15/src/pyflipper/lib/device_info.py` & `pyflipper-0.16/src/pyflipper/lib/device_info.py`

 * *Files identical despite different names*

### Comparing `pyflipper-0.15/src/pyflipper/lib/ikey.py` & `pyflipper-0.16/src/pyflipper/lib/ikey.py`

 * *Files identical despite different names*

### Comparing `pyflipper-0.15/src/pyflipper/lib/input.py` & `pyflipper-0.16/src/pyflipper/lib/input.py`

 * *Files identical despite different names*

### Comparing `pyflipper-0.15/src/pyflipper/lib/ir.py` & `pyflipper-0.16/src/pyflipper/lib/ir.py`

 * *Files identical despite different names*

### Comparing `pyflipper-0.15/src/pyflipper/lib/led.py` & `pyflipper-0.16/src/pyflipper/lib/led.py`

 * *Files identical despite different names*

### Comparing `pyflipper-0.15/src/pyflipper/lib/loader.py` & `pyflipper-0.16/src/pyflipper/lib/loader.py`

 * *Files identical despite different names*

### Comparing `pyflipper-0.15/src/pyflipper/lib/nfc.py` & `pyflipper-0.16/src/pyflipper/lib/nfc.py`

 * *Files identical despite different names*

### Comparing `pyflipper-0.15/src/pyflipper/lib/power.py` & `pyflipper-0.16/src/pyflipper/lib/power.py`

 * *Files identical despite different names*

### Comparing `pyflipper-0.15/src/pyflipper/lib/ps.py` & `pyflipper-0.16/src/pyflipper/lib/ps.py`

 * *Files identical despite different names*

### Comparing `pyflipper-0.15/src/pyflipper/lib/rfid.py` & `pyflipper-0.16/src/pyflipper/lib/rfid.py`

 * *Files identical despite different names*

### Comparing `pyflipper-0.15/src/pyflipper/lib/serial_wrapper.py` & `pyflipper-0.16/src/pyflipper/lib/serial_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyflipper-0.15/src/pyflipper/lib/storage.py` & `pyflipper-0.16/src/pyflipper/lib/storage.py`

 * *Files identical despite different names*

### Comparing `pyflipper-0.15/src/pyflipper/lib/subghz.py` & `pyflipper-0.16/src/pyflipper/lib/subghz.py`

 * *Files identical despite different names*

### Comparing `pyflipper-0.15/src/pyflipper/lib/threaded.py` & `pyflipper-0.16/src/pyflipper/lib/threaded.py`

 * *Files identical despite different names*

### Comparing `pyflipper-0.15/src/pyflipper/lib/update.py` & `pyflipper-0.16/src/pyflipper/lib/update.py`

 * *Files identical despite different names*

### Comparing `pyflipper-0.15/src/pyflipper/pyflipper.py` & `pyflipper-0.16/src/pyflipper/pyflipper.py`

 * *Files identical despite different names*

### Comparing `pyflipper-0.15/src/pyflipper.egg-info/PKG-INFO` & `pyflipper-0.16/src/pyflipper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyflipper
-Version: 0.15
+Version: 0.16
 Summary: Unoffical Flipper Zero cli wrapper
 Home-page: https://github.com/wh00hw/pyFlipper
 Author: wh00hw
 Author-email: white_rabbit@autistici.org
 License: MIT
 Project-URL: Documentation, https://github.com/wh00hw/pyFlipper/blob/master/README.md
 Project-URL: Bug Reports, https://github.com/wh00hw/pyFlipper/issues
```

### Comparing `pyflipper-0.15/src/pyflipper.egg-info/SOURCES.txt` & `pyflipper-0.16/src/pyflipper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

