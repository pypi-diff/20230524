# Comparing `tmp/pyflipper-0.14.tar.gz` & `tmp/pyflipper-0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyflipper-0.14.tar", last modified: Wed May 24 09:09:54 2023, max compression
+gzip compressed data, was "pyflipper-0.15.tar", last modified: Wed May 24 09:11:45 2023, max compression
```

## Comparing `pyflipper-0.14.tar` & `pyflipper-0.15.tar`

### file list

```diff
@@ -1,41 +1,44 @@
-drwxr-xr-x   0 wh        (1000) users      (984)        0 2023-05-24 09:09:54.725823 pyflipper-0.14/
--rw-r--r--   0 wh        (1000) users      (984)     1063 2023-05-24 08:32:10.000000 pyflipper-0.14/LICENSE
--rw-r--r--   0 wh        (1000) users      (984)      900 2023-05-24 09:09:54.725823 pyflipper-0.14/PKG-INFO
--rw-r--r--   0 wh        (1000) users      (984)     8172 2023-05-24 08:32:10.000000 pyflipper-0.14/README.md
--rw-r--r--   0 wh        (1000) users      (984)      112 2023-05-24 09:09:54.725823 pyflipper-0.14/setup.cfg
--rw-r--r--   0 wh        (1000) users      (984)     1538 2023-05-24 09:09:40.000000 pyflipper-0.14/setup.py
-drwxr-xr-x   0 wh        (1000) users      (984)        0 2023-05-24 09:09:54.722490 pyflipper-0.14/src/
-drwxr-xr-x   0 wh        (1000) users      (984)        0 2023-05-24 09:09:54.722490 pyflipper-0.14/src/lib/
--rw-r--r--   0 wh        (1000) users      (984)        0 2023-05-24 08:32:10.000000 pyflipper-0.14/src/lib/__init__.py
--rw-r--r--   0 wh        (1000) users      (984)      310 2023-05-24 08:32:10.000000 pyflipper-0.14/src/lib/bt.py
--rw-r--r--   0 wh        (1000) users      (984)      479 2023-05-24 08:32:10.000000 pyflipper-0.14/src/lib/date.py
--rw-r--r--   0 wh        (1000) users      (984)      251 2023-05-24 08:32:10.000000 pyflipper-0.14/src/lib/debug.py
--rw-r--r--   0 wh        (1000) users      (984)      557 2023-05-24 08:32:10.000000 pyflipper-0.14/src/lib/device_info.py
--rw-r--r--   0 wh        (1000) users      (984)      428 2023-05-24 08:32:10.000000 pyflipper-0.14/src/lib/free.py
--rw-r--r--   0 wh        (1000) users      (984)      511 2023-05-24 08:32:10.000000 pyflipper-0.14/src/lib/gpio.py
--rw-r--r--   0 wh        (1000) users      (984)      179 2023-05-24 08:32:10.000000 pyflipper-0.14/src/lib/i2c.py
--rw-r--r--   0 wh        (1000) users      (984)     1494 2023-05-24 08:32:10.000000 pyflipper-0.14/src/lib/ikey.py
--rw-r--r--   0 wh        (1000) users      (984)      672 2023-05-24 08:32:10.000000 pyflipper-0.14/src/lib/input.py
--rw-r--r--   0 wh        (1000) users      (984)     1912 2023-05-24 08:32:10.000000 pyflipper-0.14/src/lib/ir.py
--rw-r--r--   0 wh        (1000) users      (984)      908 2023-05-24 08:32:10.000000 pyflipper-0.14/src/lib/led.py
--rw-r--r--   0 wh        (1000) users      (984)      742 2023-05-24 08:32:10.000000 pyflipper-0.14/src/lib/loader.py
--rw-r--r--   0 wh        (1000) users      (984)      306 2023-05-24 08:32:10.000000 pyflipper-0.14/src/lib/log.py
--rw-r--r--   0 wh        (1000) users      (984)      485 2023-05-24 08:32:10.000000 pyflipper-0.14/src/lib/music_player.py
--rw-r--r--   0 wh        (1000) users      (984)     1136 2023-05-24 08:32:10.000000 pyflipper-0.14/src/lib/nfc.py
--rw-r--r--   0 wh        (1000) users      (984)      197 2023-05-24 08:32:10.000000 pyflipper-0.14/src/lib/onewire.py
--rw-r--r--   0 wh        (1000) users      (984)      628 2023-05-24 08:32:10.000000 pyflipper-0.14/src/lib/power.py
--rw-r--r--   0 wh        (1000) users      (984)      526 2023-05-24 08:32:10.000000 pyflipper-0.14/src/lib/ps.py
--rw-r--r--   0 wh        (1000) users      (984)     1604 2023-05-24 08:32:10.000000 pyflipper-0.14/src/lib/rfid.py
--rw-r--r--   0 wh        (1000) users      (984)     1535 2023-05-24 09:01:07.000000 pyflipper-0.14/src/lib/serial_wrapper.py
--rw-r--r--   0 wh        (1000) users      (984)     3039 2023-05-24 09:00:31.000000 pyflipper-0.14/src/lib/storage.py
--rw-r--r--   0 wh        (1000) users      (984)     1069 2023-05-24 08:32:10.000000 pyflipper-0.14/src/lib/subghz.py
--rw-r--r--   0 wh        (1000) users      (984)      766 2023-05-24 08:32:10.000000 pyflipper-0.14/src/lib/threaded.py
--rw-r--r--   0 wh        (1000) users      (984)      621 2023-05-24 08:32:10.000000 pyflipper-0.14/src/lib/update.py
--rw-r--r--   0 wh        (1000) users      (984)      150 2023-05-24 08:32:10.000000 pyflipper-0.14/src/lib/utils.py
--rw-r--r--   0 wh        (1000) users      (984)      428 2023-05-24 08:32:10.000000 pyflipper-0.14/src/lib/vibro.py
-drwxr-xr-x   0 wh        (1000) users      (984)        0 2023-05-24 09:09:54.725823 pyflipper-0.14/src/pyflipper.egg-info/
--rw-r--r--   0 wh        (1000) users      (984)      900 2023-05-24 09:09:54.000000 pyflipper-0.14/src/pyflipper.egg-info/PKG-INFO
--rw-r--r--   0 wh        (1000) users      (984)      692 2023-05-24 09:09:54.000000 pyflipper-0.14/src/pyflipper.egg-info/SOURCES.txt
--rw-r--r--   0 wh        (1000) users      (984)        1 2023-05-24 09:09:54.000000 pyflipper-0.14/src/pyflipper.egg-info/dependency_links.txt
--rw-r--r--   0 wh        (1000) users      (984)       26 2023-05-24 09:09:54.000000 pyflipper-0.14/src/pyflipper.egg-info/requires.txt
--rw-r--r--   0 wh        (1000) users      (984)        4 2023-05-24 09:09:54.000000 pyflipper-0.14/src/pyflipper.egg-info/top_level.txt
+drwxr-xr-x   0 wh        (1000) users      (984)        0 2023-05-24 09:11:45.442517 pyflipper-0.15/
+-rw-r--r--   0 wh        (1000) users      (984)     1063 2023-05-24 08:32:10.000000 pyflipper-0.15/LICENSE
+-rw-r--r--   0 wh        (1000) users      (984)      900 2023-05-24 09:11:45.442517 pyflipper-0.15/PKG-INFO
+-rw-r--r--   0 wh        (1000) users      (984)     8172 2023-05-24 08:32:10.000000 pyflipper-0.15/README.md
+-rw-r--r--   0 wh        (1000) users      (984)      112 2023-05-24 09:11:45.442517 pyflipper-0.15/setup.cfg
+-rw-r--r--   0 wh        (1000) users      (984)     1538 2023-05-24 09:11:40.000000 pyflipper-0.15/setup.py
+drwxr-xr-x   0 wh        (1000) users      (984)        0 2023-05-24 09:11:45.439183 pyflipper-0.15/src/
+drwxr-xr-x   0 wh        (1000) users      (984)        0 2023-05-24 09:11:45.439183 pyflipper-0.15/src/pyflipper/
+-rw-r--r--   0 wh        (1000) users      (984)        0 2023-05-24 09:11:01.000000 pyflipper-0.15/src/pyflipper/__init__.py
+drwxr-xr-x   0 wh        (1000) users      (984)        0 2023-05-24 09:11:45.442517 pyflipper-0.15/src/pyflipper/lib/
+-rw-r--r--   0 wh        (1000) users      (984)        0 2023-05-24 08:32:10.000000 pyflipper-0.15/src/pyflipper/lib/__init__.py
+-rw-r--r--   0 wh        (1000) users      (984)      310 2023-05-24 08:32:10.000000 pyflipper-0.15/src/pyflipper/lib/bt.py
+-rw-r--r--   0 wh        (1000) users      (984)      479 2023-05-24 08:32:10.000000 pyflipper-0.15/src/pyflipper/lib/date.py
+-rw-r--r--   0 wh        (1000) users      (984)      251 2023-05-24 08:32:10.000000 pyflipper-0.15/src/pyflipper/lib/debug.py
+-rw-r--r--   0 wh        (1000) users      (984)      557 2023-05-24 08:32:10.000000 pyflipper-0.15/src/pyflipper/lib/device_info.py
+-rw-r--r--   0 wh        (1000) users      (984)      428 2023-05-24 08:32:10.000000 pyflipper-0.15/src/pyflipper/lib/free.py
+-rw-r--r--   0 wh        (1000) users      (984)      511 2023-05-24 08:32:10.000000 pyflipper-0.15/src/pyflipper/lib/gpio.py
+-rw-r--r--   0 wh        (1000) users      (984)      179 2023-05-24 08:32:10.000000 pyflipper-0.15/src/pyflipper/lib/i2c.py
+-rw-r--r--   0 wh        (1000) users      (984)     1494 2023-05-24 08:32:10.000000 pyflipper-0.15/src/pyflipper/lib/ikey.py
+-rw-r--r--   0 wh        (1000) users      (984)      672 2023-05-24 08:32:10.000000 pyflipper-0.15/src/pyflipper/lib/input.py
+-rw-r--r--   0 wh        (1000) users      (984)     1912 2023-05-24 08:32:10.000000 pyflipper-0.15/src/pyflipper/lib/ir.py
+-rw-r--r--   0 wh        (1000) users      (984)      908 2023-05-24 08:32:10.000000 pyflipper-0.15/src/pyflipper/lib/led.py
+-rw-r--r--   0 wh        (1000) users      (984)      742 2023-05-24 08:32:10.000000 pyflipper-0.15/src/pyflipper/lib/loader.py
+-rw-r--r--   0 wh        (1000) users      (984)      306 2023-05-24 08:32:10.000000 pyflipper-0.15/src/pyflipper/lib/log.py
+-rw-r--r--   0 wh        (1000) users      (984)      485 2023-05-24 08:32:10.000000 pyflipper-0.15/src/pyflipper/lib/music_player.py
+-rw-r--r--   0 wh        (1000) users      (984)     1136 2023-05-24 08:32:10.000000 pyflipper-0.15/src/pyflipper/lib/nfc.py
+-rw-r--r--   0 wh        (1000) users      (984)      197 2023-05-24 08:32:10.000000 pyflipper-0.15/src/pyflipper/lib/onewire.py
+-rw-r--r--   0 wh        (1000) users      (984)      628 2023-05-24 08:32:10.000000 pyflipper-0.15/src/pyflipper/lib/power.py
+-rw-r--r--   0 wh        (1000) users      (984)      526 2023-05-24 08:32:10.000000 pyflipper-0.15/src/pyflipper/lib/ps.py
+-rw-r--r--   0 wh        (1000) users      (984)     1604 2023-05-24 08:32:10.000000 pyflipper-0.15/src/pyflipper/lib/rfid.py
+-rw-r--r--   0 wh        (1000) users      (984)     1535 2023-05-24 09:01:07.000000 pyflipper-0.15/src/pyflipper/lib/serial_wrapper.py
+-rw-r--r--   0 wh        (1000) users      (984)     3039 2023-05-24 09:00:31.000000 pyflipper-0.15/src/pyflipper/lib/storage.py
+-rw-r--r--   0 wh        (1000) users      (984)     1069 2023-05-24 08:32:10.000000 pyflipper-0.15/src/pyflipper/lib/subghz.py
+-rw-r--r--   0 wh        (1000) users      (984)      766 2023-05-24 08:32:10.000000 pyflipper-0.15/src/pyflipper/lib/threaded.py
+-rw-r--r--   0 wh        (1000) users      (984)      621 2023-05-24 08:32:10.000000 pyflipper-0.15/src/pyflipper/lib/update.py
+-rw-r--r--   0 wh        (1000) users      (984)      150 2023-05-24 08:32:10.000000 pyflipper-0.15/src/pyflipper/lib/utils.py
+-rw-r--r--   0 wh        (1000) users      (984)      428 2023-05-24 08:32:10.000000 pyflipper-0.15/src/pyflipper/lib/vibro.py
+-rw-r--r--   0 wh        (1000) users      (984)     2540 2023-05-24 08:57:26.000000 pyflipper-0.15/src/pyflipper/pyflipper.py
+drwxr-xr-x   0 wh        (1000) users      (984)        0 2023-05-24 09:11:45.439183 pyflipper-0.15/src/pyflipper.egg-info/
+-rw-r--r--   0 wh        (1000) users      (984)      900 2023-05-24 09:11:45.000000 pyflipper-0.15/src/pyflipper.egg-info/PKG-INFO
+-rw-r--r--   0 wh        (1000) users      (984)     1015 2023-05-24 09:11:45.000000 pyflipper-0.15/src/pyflipper.egg-info/SOURCES.txt
+-rw-r--r--   0 wh        (1000) users      (984)        1 2023-05-24 09:11:45.000000 pyflipper-0.15/src/pyflipper.egg-info/dependency_links.txt
+-rw-r--r--   0 wh        (1000) users      (984)       26 2023-05-24 09:11:45.000000 pyflipper-0.15/src/pyflipper.egg-info/requires.txt
+-rw-r--r--   0 wh        (1000) users      (984)       10 2023-05-24 09:11:45.000000 pyflipper-0.15/src/pyflipper.egg-info/top_level.txt
```

### Comparing `pyflipper-0.14/LICENSE` & `pyflipper-0.15/LICENSE`

 * *Files identical despite different names*

### Comparing `pyflipper-0.14/PKG-INFO` & `pyflipper-0.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyflipper
-Version: 0.14
+Version: 0.15
 Summary: Unoffical Flipper Zero cli wrapper
 Home-page: https://github.com/wh00hw/pyFlipper
 Author: wh00hw
 Author-email: white_rabbit@autistici.org
 License: MIT
 Project-URL: Documentation, https://github.com/wh00hw/pyFlipper/blob/master/README.md
 Project-URL: Bug Reports, https://github.com/wh00hw/pyFlipper/issues
```

### Comparing `pyflipper-0.14/README.md` & `pyflipper-0.15/README.md`

 * *Files identical despite different names*

### Comparing `pyflipper-0.14/setup.py` & `pyflipper-0.15/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 import setuptools
 
 setuptools.setup(
   name = 'pyflipper',      
   package_dir={'': 'src'},
   packages=setuptools.find_packages(where='src'),
-  version = '0.14',      # Start with a small number and increase it with every change you make
+  version = '0.15',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Unoffical Flipper Zero cli wrapper',   # Give a short description about your library
   author = 'wh00hw',                   # Type in your name
   author_email = 'white_rabbit@autistici.org',      # Type in your E-Mail
   url = 'https://github.com/wh00hw/pyFlipper',   # Provide either the link to your github or to your website
   project_urls={
     'Documentation': 'https://github.com/wh00hw/pyFlipper/blob/master/README.md',
```

### Comparing `pyflipper-0.14/src/lib/device_info.py` & `pyflipper-0.15/src/pyflipper/lib/device_info.py`

 * *Files identical despite different names*

### Comparing `pyflipper-0.14/src/lib/ikey.py` & `pyflipper-0.15/src/pyflipper/lib/ikey.py`

 * *Files identical despite different names*

### Comparing `pyflipper-0.14/src/lib/input.py` & `pyflipper-0.15/src/pyflipper/lib/input.py`

 * *Files identical despite different names*

### Comparing `pyflipper-0.14/src/lib/ir.py` & `pyflipper-0.15/src/pyflipper/lib/ir.py`

 * *Files identical despite different names*

### Comparing `pyflipper-0.14/src/lib/led.py` & `pyflipper-0.15/src/pyflipper/lib/led.py`

 * *Files identical despite different names*

### Comparing `pyflipper-0.14/src/lib/loader.py` & `pyflipper-0.15/src/pyflipper/lib/loader.py`

 * *Files identical despite different names*

### Comparing `pyflipper-0.14/src/lib/nfc.py` & `pyflipper-0.15/src/pyflipper/lib/nfc.py`

 * *Files identical despite different names*

### Comparing `pyflipper-0.14/src/lib/power.py` & `pyflipper-0.15/src/pyflipper/lib/power.py`

 * *Files identical despite different names*

### Comparing `pyflipper-0.14/src/lib/ps.py` & `pyflipper-0.15/src/pyflipper/lib/ps.py`

 * *Files identical despite different names*

### Comparing `pyflipper-0.14/src/lib/rfid.py` & `pyflipper-0.15/src/pyflipper/lib/rfid.py`

 * *Files identical despite different names*

### Comparing `pyflipper-0.14/src/lib/serial_wrapper.py` & `pyflipper-0.15/src/pyflipper/lib/serial_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyflipper-0.14/src/lib/storage.py` & `pyflipper-0.15/src/pyflipper/lib/storage.py`

 * *Files identical despite different names*

### Comparing `pyflipper-0.14/src/lib/subghz.py` & `pyflipper-0.15/src/pyflipper/lib/subghz.py`

 * *Files identical despite different names*

### Comparing `pyflipper-0.14/src/lib/threaded.py` & `pyflipper-0.15/src/pyflipper/lib/threaded.py`

 * *Files identical despite different names*

### Comparing `pyflipper-0.14/src/lib/update.py` & `pyflipper-0.15/src/pyflipper/lib/update.py`

 * *Files identical despite different names*

### Comparing `pyflipper-0.14/src/pyflipper.egg-info/PKG-INFO` & `pyflipper-0.15/src/pyflipper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyflipper
-Version: 0.14
+Version: 0.15
 Summary: Unoffical Flipper Zero cli wrapper
 Home-page: https://github.com/wh00hw/pyFlipper
 Author: wh00hw
 Author-email: white_rabbit@autistici.org
 License: MIT
 Project-URL: Documentation, https://github.com/wh00hw/pyFlipper/blob/master/README.md
 Project-URL: Bug Reports, https://github.com/wh00hw/pyFlipper/issues
```

### Comparing `pyflipper-0.14/src/pyflipper.egg-info/SOURCES.txt` & `pyflipper-0.15/src/pyflipper.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
-src/lib/__init__.py
-src/lib/bt.py
-src/lib/date.py
-src/lib/debug.py
-src/lib/device_info.py
-src/lib/free.py
-src/lib/gpio.py
-src/lib/i2c.py
-src/lib/ikey.py
-src/lib/input.py
-src/lib/ir.py
-src/lib/led.py
-src/lib/loader.py
-src/lib/log.py
-src/lib/music_player.py
-src/lib/nfc.py
-src/lib/onewire.py
-src/lib/power.py
-src/lib/ps.py
-src/lib/rfid.py
-src/lib/serial_wrapper.py
-src/lib/storage.py
-src/lib/subghz.py
-src/lib/threaded.py
-src/lib/update.py
-src/lib/utils.py
-src/lib/vibro.py
+src/pyflipper/__init__.py
+src/pyflipper/pyflipper.py
 src/pyflipper.egg-info/PKG-INFO
 src/pyflipper.egg-info/SOURCES.txt
 src/pyflipper.egg-info/dependency_links.txt
 src/pyflipper.egg-info/requires.txt
-src/pyflipper.egg-info/top_level.txt
+src/pyflipper.egg-info/top_level.txt
+src/pyflipper/lib/__init__.py
+src/pyflipper/lib/bt.py
+src/pyflipper/lib/date.py
+src/pyflipper/lib/debug.py
+src/pyflipper/lib/device_info.py
+src/pyflipper/lib/free.py
+src/pyflipper/lib/gpio.py
+src/pyflipper/lib/i2c.py
+src/pyflipper/lib/ikey.py
+src/pyflipper/lib/input.py
+src/pyflipper/lib/ir.py
+src/pyflipper/lib/led.py
+src/pyflipper/lib/loader.py
+src/pyflipper/lib/log.py
+src/pyflipper/lib/music_player.py
+src/pyflipper/lib/nfc.py
+src/pyflipper/lib/onewire.py
+src/pyflipper/lib/power.py
+src/pyflipper/lib/ps.py
+src/pyflipper/lib/rfid.py
+src/pyflipper/lib/serial_wrapper.py
+src/pyflipper/lib/storage.py
+src/pyflipper/lib/subghz.py
+src/pyflipper/lib/threaded.py
+src/pyflipper/lib/update.py
+src/pyflipper/lib/utils.py
+src/pyflipper/lib/vibro.py
```

