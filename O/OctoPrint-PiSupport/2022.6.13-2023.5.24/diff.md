# Comparing `tmp/OctoPrint-PiSupport-2022.6.13.tar.gz` & `tmp/OctoPrint-PiSupport-2023.5.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/OctoPrint-PiSupport-2022.6.13.tar", last modified: Mon Jun 13 09:36:07 2022, max compression
+gzip compressed data, was "dist/OctoPrint-PiSupport-2023.5.24.tar", last modified: Wed May 24 16:11:57 2023, max compression
```

## Comparing `OctoPrint-PiSupport-2022.6.13.tar` & `OctoPrint-PiSupport-2023.5.24.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-13 09:36:07.000000 OctoPrint-PiSupport-2022.6.13/
--rw-r--r--   0 runner    (1001) docker     (121)    34520 2022-06-13 09:36:03.000000 OctoPrint-PiSupport-2022.6.13/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      171 2022-06-13 09:36:03.000000 OctoPrint-PiSupport-2022.6.13/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-13 09:36:07.000000 OctoPrint-PiSupport-2022.6.13/OctoPrint_PiSupport.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3237 2022-06-13 09:36:07.000000 OctoPrint-PiSupport-2022.6.13/OctoPrint_PiSupport.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      824 2022-06-13 09:36:07.000000 OctoPrint-PiSupport-2022.6.13/OctoPrint_PiSupport.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-13 09:36:07.000000 OctoPrint-PiSupport-2022.6.13/OctoPrint_PiSupport.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-06-13 09:36:07.000000 OctoPrint-PiSupport-2022.6.13/OctoPrint_PiSupport.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-13 09:36:07.000000 OctoPrint-PiSupport-2022.6.13/OctoPrint_PiSupport.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-13 09:36:07.000000 OctoPrint-PiSupport-2022.6.13/OctoPrint_PiSupport.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-06-13 09:36:07.000000 OctoPrint-PiSupport-2022.6.13/OctoPrint_PiSupport.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3237 2022-06-13 09:36:07.000000 OctoPrint-PiSupport-2022.6.13/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2406 2022-06-13 09:36:03.000000 OctoPrint-PiSupport-2022.6.13/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-13 09:36:07.000000 OctoPrint-PiSupport-2022.6.13/octoprint_pi_support/
--rw-r--r--   0 runner    (1001) docker     (121)    18353 2022-06-13 09:36:03.000000 OctoPrint-PiSupport-2022.6.13/octoprint_pi_support/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-13 09:36:07.000000 OctoPrint-PiSupport-2022.6.13/octoprint_pi_support/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-13 09:36:07.000000 OctoPrint-PiSupport-2022.6.13/octoprint_pi_support/static/clientjs/
--rw-r--r--   0 runner    (1001) docker     (121)      583 2022-06-13 09:36:03.000000 OctoPrint-PiSupport-2022.6.13/octoprint_pi_support/static/clientjs/pi_support.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-13 09:36:07.000000 OctoPrint-PiSupport-2022.6.13/octoprint_pi_support/static/css/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-06-13 09:36:03.000000 OctoPrint-PiSupport-2022.6.13/octoprint_pi_support/static/css/pi_support.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-13 09:36:07.000000 OctoPrint-PiSupport-2022.6.13/octoprint_pi_support/static/js/
--rw-r--r--   0 runner    (1001) docker     (121)    13541 2022-06-13 09:36:03.000000 OctoPrint-PiSupport-2022.6.13/octoprint_pi_support/static/js/pi_support.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-13 09:36:07.000000 OctoPrint-PiSupport-2022.6.13/octoprint_pi_support/templates/
--rw-r--r--   0 runner    (1001) docker     (121)     1475 2022-06-13 09:36:03.000000 OctoPrint-PiSupport-2022.6.13/octoprint_pi_support/templates/pi_support_about_octopi.jinja2
--rw-r--r--   0 runner    (1001) docker     (121)      775 2022-06-13 09:36:03.000000 OctoPrint-PiSupport-2022.6.13/octoprint_pi_support/templates/pi_support_navbar.jinja2
--rw-r--r--   0 runner    (1001) docker     (121)     3772 2022-06-13 09:36:03.000000 OctoPrint-PiSupport-2022.6.13/octoprint_pi_support/templates/pi_support_settings.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-13 09:36:07.000000 OctoPrint-PiSupport-2022.6.13/octoprint_pi_support/translations/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-13 09:36:07.000000 OctoPrint-PiSupport-2022.6.13/octoprint_pi_support/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-13 09:36:07.000000 OctoPrint-PiSupport-2022.6.13/octoprint_pi_support/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     7031 2022-06-13 09:36:03.000000 OctoPrint-PiSupport-2022.6.13/octoprint_pi_support/translations/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (121)    11164 2022-06-13 09:36:03.000000 OctoPrint-PiSupport-2022.6.13/octoprint_pi_support/translations/de/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (121)      374 2022-06-13 09:36:07.000000 OctoPrint-PiSupport-2022.6.13/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)    25124 2022-06-13 09:36:03.000000 OctoPrint-PiSupport-2022.6.13/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:11:57.000000 OctoPrint-PiSupport-2023.5.24/
+-rw-r--r--   0 runner    (1001) docker     (123)    34520 2023-05-24 16:11:51.000000 OctoPrint-PiSupport-2023.5.24/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-24 16:11:51.000000 OctoPrint-PiSupport-2023.5.24/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:11:57.000000 OctoPrint-PiSupport-2023.5.24/OctoPrint_PiSupport.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-05-24 16:11:56.000000 OctoPrint-PiSupport-2023.5.24/OctoPrint_PiSupport.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-24 16:11:57.000000 OctoPrint-PiSupport-2023.5.24/OctoPrint_PiSupport.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 16:11:56.000000 OctoPrint-PiSupport-2023.5.24/OctoPrint_PiSupport.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-24 16:11:56.000000 OctoPrint-PiSupport-2023.5.24/OctoPrint_PiSupport.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 16:11:56.000000 OctoPrint-PiSupport-2023.5.24/OctoPrint_PiSupport.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 16:11:56.000000 OctoPrint-PiSupport-2023.5.24/OctoPrint_PiSupport.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-24 16:11:56.000000 OctoPrint-PiSupport-2023.5.24/OctoPrint_PiSupport.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-05-24 16:11:57.000000 OctoPrint-PiSupport-2023.5.24/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-05-24 16:11:51.000000 OctoPrint-PiSupport-2023.5.24/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:11:57.000000 OctoPrint-PiSupport-2023.5.24/octoprint_pi_support/
+-rw-r--r--   0 runner    (1001) docker     (123)    20030 2023-05-24 16:11:51.000000 OctoPrint-PiSupport-2023.5.24/octoprint_pi_support/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:11:57.000000 OctoPrint-PiSupport-2023.5.24/octoprint_pi_support/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:11:57.000000 OctoPrint-PiSupport-2023.5.24/octoprint_pi_support/static/clientjs/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-24 16:11:51.000000 OctoPrint-PiSupport-2023.5.24/octoprint_pi_support/static/clientjs/pi_support.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:11:57.000000 OctoPrint-PiSupport-2023.5.24/octoprint_pi_support/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-24 16:11:51.000000 OctoPrint-PiSupport-2023.5.24/octoprint_pi_support/static/css/pi_support.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:11:57.000000 OctoPrint-PiSupport-2023.5.24/octoprint_pi_support/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    13609 2023-05-24 16:11:51.000000 OctoPrint-PiSupport-2023.5.24/octoprint_pi_support/static/js/pi_support.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:11:57.000000 OctoPrint-PiSupport-2023.5.24/octoprint_pi_support/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-24 16:11:51.000000 OctoPrint-PiSupport-2023.5.24/octoprint_pi_support/templates/pi_support_about_octopi.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-24 16:11:51.000000 OctoPrint-PiSupport-2023.5.24/octoprint_pi_support/templates/pi_support_navbar.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-05-24 16:11:51.000000 OctoPrint-PiSupport-2023.5.24/octoprint_pi_support/templates/pi_support_settings.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:11:57.000000 OctoPrint-PiSupport-2023.5.24/octoprint_pi_support/translations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:11:57.000000 OctoPrint-PiSupport-2023.5.24/octoprint_pi_support/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:11:57.000000 OctoPrint-PiSupport-2023.5.24/octoprint_pi_support/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     7031 2023-05-24 16:11:51.000000 OctoPrint-PiSupport-2023.5.24/octoprint_pi_support/translations/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11164 2023-05-24 16:11:51.000000 OctoPrint-PiSupport-2023.5.24/octoprint_pi_support/translations/de/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-24 16:11:57.000000 OctoPrint-PiSupport-2023.5.24/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    24824 2023-05-24 16:11:51.000000 OctoPrint-PiSupport-2023.5.24/setup.py
```

### Comparing `OctoPrint-PiSupport-2022.6.13/LICENSE` & `OctoPrint-PiSupport-2023.5.24/LICENSE`

 * *Files identical despite different names*

### Comparing `OctoPrint-PiSupport-2022.6.13/OctoPrint_PiSupport.egg-info/PKG-INFO` & `OctoPrint-PiSupport-2023.5.24/OctoPrint_PiSupport.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OctoPrint-PiSupport
-Version: 2022.6.13
+Version: 2023.5.24
 Summary: Provides additional information about your Pi in the UI
 Home-page: https://github.com/OctoPrint/OctoPrint-PiSupport
 Author: Gina Häußge
 Author-email: gina@octoprint.org
 License: AGPLv3
 Description: # Pi Support
```

### Comparing `OctoPrint-PiSupport-2022.6.13/OctoPrint_PiSupport.egg-info/SOURCES.txt` & `OctoPrint-PiSupport-2023.5.24/OctoPrint_PiSupport.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OctoPrint-PiSupport-2022.6.13/PKG-INFO` & `OctoPrint-PiSupport-2023.5.24/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OctoPrint-PiSupport
-Version: 2022.6.13
+Version: 2023.5.24
 Summary: Provides additional information about your Pi in the UI
 Home-page: https://github.com/OctoPrint/OctoPrint-PiSupport
 Author: Gina Häußge
 Author-email: gina@octoprint.org
 License: AGPLv3
 Description: # Pi Support
```

### Comparing `OctoPrint-PiSupport-2022.6.13/README.md` & `OctoPrint-PiSupport-2023.5.24/README.md`

 * *Files identical despite different names*

### Comparing `OctoPrint-PiSupport-2022.6.13/octoprint_pi_support/__init__.py` & `OctoPrint-PiSupport-2023.5.24/octoprint_pi_support/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,10 @@
-# -*- coding: utf-8 -*-
-from __future__ import absolute_import, division, print_function, unicode_literals
-
 __license__ = "GNU Affero General Public License http://www.gnu.org/licenses/agpl.html"
 __copyright__ = "Copyright (C) 2017 The OctoPrint Project - Released under terms of the AGPLv3 License"
 
-import io
 import os
 from getpass import getuser
 
 import flask
 import octoprint.events
 import octoprint.plugin
 import sarge
@@ -17,20 +13,56 @@
 from octoprint.access.permissions import Permissions
 from octoprint.util import RepeatedTimer
 from octoprint.util.platform import CLOSE_FDS
 
 _PROC_DT_MODEL_PATH = "/proc/device-tree/model"
 _OCTOPI_VERSION_PATH = "/etc/octopi_version"
 _OCTOPIUPTODATE_BUILD_PATH = "/etc/octopiuptodate_build"
+_NEW_CAMERA_STACK_PATH = "/etc/systemd/system/camera-streamer-usb@.service"
 _VCGENCMD_THROTTLE = "/usr/bin/vcgencmd get_throttled"
 _SSHWARN_PATH = "/run/sshwarn"
 
 _CHECK_INTERVAL_OK = 300
 _CHECK_INTERVAL_THROTTLED = 30
 
+
+def _gather_new_camerastack_files():
+    import logging
+
+    files = {}
+
+    try:
+        os.system(
+            "journalctl --boot -u 'camera-streamer*' > /tmp/camerastack-journal.log"
+        )
+        files["camerastack-journal.log"] = "/tmp/camerastack-journal.log"
+    except Exception:
+        logging.getLogger(__name__).exception(
+            "Failed to create camerastack-journal.log file"
+        )
+
+    try:
+        os.system(
+            "/usr/bin/libcamera-hello --list-cameras > /tmp/camerastack-libcamera.log"
+        )
+        files["camerastack-libcamera.log"] = "/tmp/camerastack-libcamera.log"
+    except Exception:
+        logging.getLogger(__name__).exception(
+            "Failed to create camerastack-libcamera.log file"
+        )
+
+    try:
+        os.system("/usr/bin/list-usb-cameras > /tmp/camerastack-usb.log")
+        files["camerastack-usb.log"] = "/tmp/camerastack-usb.log"
+    except Exception:
+        logging.getLogger(__name__).exception("Failed to create camerastack-usb.log file")
+
+    return files
+
+
 __LOCAL_DEBUG = os.path.exists(
     os.path.realpath(os.path.join(os.path.dirname(__file__), "..", ".local_debug"))
 )
 
 if __LOCAL_DEBUG:
     ### mocks & settings for local debugging
     base = os.path.realpath(
@@ -43,20 +75,28 @@
     )
     debug = os.path.realpath(
         os.path.join(os.path.dirname(__file__), "..", ".local_debug")
     )
     _PROC_DT_MODEL_PATH = os.path.join(base, "fake_model.txt")
     _OCTOPI_VERSION_PATH = os.path.join(base, "fake_octopi.txt")
     _OCTOPIUPTODATE_BUILD_PATH = os.path.join(base, "fake_octopiuptodate.txt")
+    _NEW_CAMERA_STACK_PATH = os.path.join(debug, "new-camera-stack")
     _SSHWARN_PATH = os.path.join(debug, "sshwarn")
 
+    _gather_new_camerastack_files = lambda: {  # noqa: F811
+        "camerastack-journal.log": os.path.join(base, "fake_camerastack_journal.txt"),
+        "camerastack-libcamera.log": os.path.join(base, "fake_camerastack_libcamera.txt"),
+        "camerastack-usb.log": os.path.join(base, "fake_camerastack_usb.txt"),
+    }
+
     import itertools
 
     _VCGENCMD_OUTPUT = itertools.chain(
-        iter(("0x0", "0x0", "0x50005", "0x50000", "0x70007")), itertools.repeat("0x70005")
+        iter(("0x0", "0x0", "0x50005", "0x50000", "0x70007")),
+        itertools.repeat("0x70005"),
     )
     _VCGENCMD_BROKEN = os.path.exists(os.path.join(debug, "vcgencmd_broken"))
 
     _CHECK_INTERVAL_OK = 10
     _CHECK_INTERVAL_THROTTLED = 5
 
 
@@ -67,15 +107,15 @@
 _FLAG_PAST_UNDERVOLTAGE = 1 << 16
 _FLAG_PAST_FREQ_CAPPED = 1 << 17
 _FLAG_PAST_THROTTLED = 1 << 18
 
 _UNRECOMMENDED_MODELS = ("Zero", "Zero W")
 
 
-class ThrottleState(object):
+class ThrottleState:
     @classmethod
     def from_value(cls, value=0):
         if value == 0:
             return ThrottleState(raw_value=value)
 
         kwargs = {
             "undervoltage": _FLAG_UNDERVOLTAGE & value == _FLAG_UNDERVOLTAGE,
@@ -95,15 +135,15 @@
         self._freq_capped = False
         self._throttled = False
         self._past_undervoltage = False
         self._past_freq_capped = False
         self._past_throttled = False
 
         for key, value in kwargs.items():
-            local_key = "_{}".format(key)
+            local_key = f"_{key}"
             if hasattr(self, local_key) and isinstance(value, bool):
                 setattr(self, local_key, value)
 
     @property
     def undervoltage(self):
         return self.current_undervoltage or self.past_undervoltage
 
@@ -141,15 +181,15 @@
 
     @property
     def raw_value(self):
         return self._raw_value
 
     @property
     def raw_value_hex(self):
-        return "0x{:X}".format(self._raw_value)
+        return f"0x{self._raw_value:X}"
 
     def __eq__(self, other):
         if not isinstance(other, ThrottleState):
             return False
 
         return (
             self._undervoltage == other._undervoltage
@@ -176,15 +216,15 @@
 _proc_dt_model = None
 
 
 def get_proc_dt_model():
     global _proc_dt_model
 
     if _proc_dt_model is None:
-        with io.open(_PROC_DT_MODEL_PATH, "rt", encoding="utf-8") as f:
+        with open(_PROC_DT_MODEL_PATH, encoding="utf-8") as f:
             _proc_dt_model = f.readline().strip(" \t\r\n\0")
 
     return _proc_dt_model
 
 
 def get_vcgencmd_throttled_state(command):
     if __LOCAL_DEBUG:
@@ -196,60 +236,62 @@
                 next(_VCGENCMD_OUTPUT)
             )  # mock for local debugging
             error = ""
     else:
         output, error = sarge.get_both(command, close_fds=CLOSE_FDS)
 
     if "throttled=0x" not in output:
-        raise ValueError(
-            'Cannot parse "{}" output: {}'.format(command, error if error else output)
-        )
+        raise ValueError(f"Cannot parse {command!r} output: {error if error else output}")
 
     value = output[len("throttled=") :].strip(" \t\r\n\0")
     value = int(value, 0)
     return ThrottleState.from_value(value)
 
 
 def is_octopi():
     return os.path.exists(_OCTOPI_VERSION_PATH)
 
 
 def is_octopiuptodate():
     return os.path.exists(_OCTOPIUPTODATE_BUILD_PATH)
 
 
+def is_new_camerastack():
+    return os.path.exists(_NEW_CAMERA_STACK_PATH)
+
+
 def is_model_any_of(model, *args):
     model = model.lower()
     for arg in map(lambda x: x.lower(), args):
-        if "{} rev".format(arg) in model or model.endswith(arg):
+        if f"{arg} rev" in model or model.endswith(arg):
             return True
     return False
 
 
 _octopi_version = None
 
 
 def get_octopi_version():
     global _octopi_version
 
     if _octopi_version is None:
-        with io.open(_OCTOPI_VERSION_PATH, "rt", encoding="utf-8") as f:
+        with open(_OCTOPI_VERSION_PATH, encoding="utf-8") as f:
             _octopi_version = f.readline().strip(" \t\r\n\0")
 
     return _octopi_version
 
 
 _octopiuptodate_build = None
 
 
 def get_octopiuptodate_build():
     global _octopiuptodate_build
 
     if _octopiuptodate_build is None:
-        with io.open(_OCTOPIUPTODATE_BUILD_PATH, "rt", encoding="utf-8") as f:
+        with open(_OCTOPIUPTODATE_BUILD_PATH, encoding="utf-8") as f:
             _octopiuptodate_build = f.readline().strip(" \t\r\n\0")
 
     return _octopiuptodate_build
 
 
 def has_default_password():
     # It would be nicer to actually fetch the hash from /etc/shadow here and verify it
@@ -266,15 +308,14 @@
     octoprint.plugin.EnvironmentDetectionPlugin,
     octoprint.plugin.SimpleApiPlugin,
     octoprint.plugin.AssetPlugin,
     octoprint.plugin.TemplatePlugin,
     octoprint.plugin.StartupPlugin,
     octoprint.plugin.SettingsPlugin,
 ):
-
     # noinspection PyMissingConstructor
     def __init__(self):
         self._throttle_state = ThrottleState()
         self._throttle_check = None
         self._throttle_undervoltage = False
         self._throttle_overheat = False
         self._throttle_check_enabled = True
@@ -304,18 +345,28 @@
             }
         ]
 
     # Additional bundle files hook
 
     def get_additional_bundle_files(self, *args, **kwargs):
         if is_octopi():
-            return {
-                "webcamd.log": "/var/log/webcamd.log",
+            result = {
                 "haproxy.log": "/var/log/haproxy.log",
             }
+
+            if is_new_camerastack():
+                # new camera-streamer based camera stack
+                files = _gather_new_camerastack_files()
+                result.update(**files)
+
+            else:
+                # old mjpg-streamer based camera stack
+                result["webcamd.log"] = "/var/log/webcamd.log"
+
+            return result
         else:
             return {}
 
     # ~~ EnvironmentDetectionPlugin
 
     def get_additional_environment(self):
         result = {"model": get_proc_dt_model()}
@@ -472,15 +523,15 @@
 
     def _check_throttled_state(self):
         if not self._throttle_check_enabled:
             return
 
         command = self._settings.get(["vcgencmd_throttle_check_command"])
 
-        self._logger.debug('Retrieving throttle state via "{}"'.format(command))
+        self._logger.debug(f"Retrieving throttle state via {command!r}")
         try:
             state = get_vcgencmd_throttled_state(command)
         except ValueError as ex:
             error = str(ex)
             self._logger.warning(error)
             if "VCHI initialization failed" in error:
                 self._logger.warning(
```

### Comparing `OctoPrint-PiSupport-2022.6.13/octoprint_pi_support/static/clientjs/pi_support.js` & `OctoPrint-PiSupport-2023.5.24/octoprint_pi_support/static/clientjs/pi_support.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-PiSupport-2022.6.13/octoprint_pi_support/static/js/pi_support.js` & `OctoPrint-PiSupport-2023.5.24/octoprint_pi_support/static/js/pi_support.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -245,17 +245,21 @@
                 "<hr><p><small>" +
                 gettext("Click the navbar icon for more information.") +
                 "</small></p>";
 
             return content;
         });
 
-        self.onStartup = self.onServerReconnect = self.onUserLoggedIn = self.onUserLoggedOut = function() {
-            self.requestData();
-        };
+        self.onStartup =
+            self.onServerReconnect =
+            self.onUserLoggedIn =
+            self.onUserLoggedOut =
+            function() {
+                self.requestData();
+            };
 
         self.onDataUpdaterPluginMessage = function(plugin, data) {
             if (plugin !== "pi_support") return;
             if (!data.hasOwnProperty("state") || !data.hasOwnProperty("type")) return;
             if (data.type !== "throttle_state") return;
             if (
                 !self.loginState.hasPermission(
```

### Comparing `OctoPrint-PiSupport-2022.6.13/octoprint_pi_support/templates/pi_support_about_octopi.jinja2` & `OctoPrint-PiSupport-2023.5.24/octoprint_pi_support/templates/pi_support_about_octopi.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-PiSupport-2022.6.13/octoprint_pi_support/templates/pi_support_navbar.jinja2` & `OctoPrint-PiSupport-2023.5.24/octoprint_pi_support/templates/pi_support_navbar.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-PiSupport-2022.6.13/octoprint_pi_support/templates/pi_support_settings.jinja2` & `OctoPrint-PiSupport-2023.5.24/octoprint_pi_support/templates/pi_support_settings.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-PiSupport-2022.6.13/octoprint_pi_support/translations/de/LC_MESSAGES/messages.mo` & `OctoPrint-PiSupport-2023.5.24/octoprint_pi_support/translations/de/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `OctoPrint-PiSupport-2022.6.13/octoprint_pi_support/translations/de/LC_MESSAGES/messages.po` & `OctoPrint-PiSupport-2023.5.24/octoprint_pi_support/translations/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `OctoPrint-PiSupport-2022.6.13/setup.py` & `OctoPrint-PiSupport-2023.5.24/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-# -*- coding: utf-8 -*-
-
 ########################################################################################################################
 ### Do not forget to adjust the following variables to your own plugin.
 
 # The plugin's identifier, has to be unique
 plugin_identifier = "pi_support"
 
 # The plugin's python package, should be "octoprint_<plugin identifier>", has to be unique
 plugin_package = "octoprint_pi_support"
 
 # The plugin's human readable name. Can be overwritten within OctoPrint's internal data via __plugin_name__ in the
 # plugin module
 plugin_name = "OctoPrint-PiSupport"
 
 # The plugin's version. Can be overwritten within OctoPrint's internal data via __plugin_version__ in the plugin module
-plugin_version = "2022.6.13"
+plugin_version = "2023.5.24"
 
 # The plugin's description. Can be overwritten within OctoPrint's internal data via __plugin_description__ in the plugin
 # module
 plugin_description = """Provides additional information about your Pi in the UI"""
 
 # The plugin's author. Can be overwritten within OctoPrint's internal data via __plugin_author__ in the plugin module
 plugin_author = "Gina Häußge"
@@ -449,17 +447,15 @@
             if not os.path.isdir(target_path):
                 raise RuntimeError(
                     "target path " + target_path + " exists and is not a directory"
                 )
             shutil.rmtree(target_path)
 
         print(
-            "Copying translations for locale {locale} from {source_path} to {target_path}...".format(
-                **locals()
-            )
+            f"Copying translations for locale {locale} from {source_path} to {target_path}..."
         )
         shutil.copytree(source_path, target_path)
 
 
 class PackTranslation(Command):
     description = "creates language packs for translations"
     user_options = [
@@ -519,41 +515,41 @@
             self.target,
             "{prefix}{locale}_{date}.zip".format(
                 prefix=self.__class__.pack_name_prefix,
                 locale=locale,
                 date=now.strftime("%Y%m%d%H%M%S"),
             ),
         )
-        print("Packing translation to {zip_path}".format(**locals()))
+        print(f"Packing translation to {zip_path}")
 
         def add_recursively(zip, path, prefix):
             if not os.path.isdir(path):
                 return
 
             for entry in os.listdir(path):
                 entry_path = os.path.join(path, entry)
                 new_prefix = prefix + "/" + entry
                 if os.path.isdir(entry_path):
                     add_recursively(zip, entry_path, new_prefix)
                 elif os.path.isfile(entry_path):
-                    print("Adding {entry_path} as {new_prefix}".format(**locals()))
+                    print(f"Adding {entry_path} as {new_prefix}")
                     zip.write(entry_path, new_prefix)
 
-        meta_str = "last_update: {date}\n".format(date=now.isoformat())
+        meta_str = f"last_update: {now.isoformat()}\n"
         if self.author:
-            meta_str += "author: {author}\n".format(author=self.author)
+            meta_str += f"author: {self.author}\n"
 
         zip_locale_root = self.__class__.pack_path_prefix + locale
 
         import zipfile
 
         with zipfile.ZipFile(zip_path, "w") as zip:
             add_recursively(zip, locale_dir, zip_locale_root)
 
-            print("Adding meta.yaml as {zip_locale_root}/meta.yaml".format(**locals()))
+            print(f"Adding meta.yaml as {zip_locale_root}/meta.yaml")
             zip.writestr(zip_locale_root + "/meta.yaml", meta_str)
 
 
 def get_babel_commandclasses(
     pot_file=None,
     mapping_file="babel.cfg",
     input_dirs=".",
@@ -616,15 +612,15 @@
     eggs=None,
     package=None,
     dependency_links=None,
 ):
     import pkg_resources
 
     if package is None:
-        package = "octoprint_{identifier}".format(**locals())
+        package = f"octoprint_{identifier}"
 
     if additional_data is None:
         additional_data = list()
 
     if additional_packages is None:
         additional_packages = list()
 
@@ -672,32 +668,32 @@
     pot_file = os.path.join(translation_dir, "messages.pot")
     bundled_dir = os.path.join(source_folder, package, "translations")
     cmdclass.update(
         get_babel_commandclasses(
             pot_file=pot_file,
             output_dir=translation_dir,
             bundled_dir=bundled_dir,
-            pack_name_prefix="{name}-i18n-".format(**locals()),
-            pack_path_prefix="_plugins/{identifier}/".format(**locals()),
+            pack_name_prefix=f"{name}-i18n-",
+            pack_path_prefix=f"_plugins/{identifier}/",
         )
     )
 
     from setuptools import find_packages
 
     packages = set(
         [package]
         + list(
             filter(
-                lambda x: x.startswith("{package}.".format(package=package)),
+                lambda x: x.startswith(f"{package}."),
                 find_packages(where=source_folder, exclude=ignored_packages),
             )
         )
         + additional_packages
     )
-    print("Found packages: {packages!r}".format(**locals()))
+    print(f"Found packages: {packages!r}")
 
     return dict(
         name=name,
         version=version,
         description=description,
         author=author,
         author_email=mail,
@@ -719,17 +715,15 @@
         # this plugin is not zip_safe.
         zip_safe=False,
         install_requires=requires,
         extras_require=extra_requires,
         dependency_links=dependency_links,
         # Hook the plugin into the "octoprint.plugin" entry point, mapping the plugin_identifier to the plugin_package.
         # That way OctoPrint will be able to find the plugin and load it.
-        entry_points={
-            "octoprint.plugin": ["{identifier} = {package}".format(**locals())]
-        },
+        entry_points={"octoprint.plugin": [f"{identifier} = {package}"]},
     )
 
 
 def read_file_contents(path):
     import codecs
 
     with codecs.open(path, encoding="utf-8") as f:
```

