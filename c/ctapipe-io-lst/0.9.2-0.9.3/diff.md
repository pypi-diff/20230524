# Comparing `tmp/ctapipe_io_lst-0.9.2.tar.gz` & `tmp/ctapipe_io_lst-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctapipe_io_lst-0.9.2.tar", last modified: Fri Apr  9 13:23:48 2021, max compression
+gzip compressed data, was "ctapipe_io_lst-0.9.3.tar", last modified: Thu Apr 22 09:41:20 2021, max compression
```

## Comparing `ctapipe_io_lst-0.9.2.tar` & `ctapipe_io_lst-0.9.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-09 13:23:48.271993 ctapipe_io_lst-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (121)      151 2021-04-09 13:23:43.000000 ctapipe_io_lst-0.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1237 2021-04-09 13:23:48.271993 ctapipe_io_lst-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      725 2021-04-09 13:23:43.000000 ctapipe_io_lst-0.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-09 13:23:48.263992 ctapipe_io_lst-0.9.2/ctapipe_io_lst/
--rw-r--r--   0 runner    (1001) docker     (121)    27587 2021-04-09 13:23:43.000000 ctapipe_io_lst-0.9.2/ctapipe_io_lst/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      142 2021-04-09 13:23:48.000000 ctapipe_io_lst-0.9.2/ctapipe_io_lst/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     1547 2021-04-09 13:23:43.000000 ctapipe_io_lst-0.9.2/ctapipe_io_lst/anyarray_dtypes.py
--rw-r--r--   0 runner    (1001) docker     (121)    30450 2021-04-09 13:23:43.000000 ctapipe_io_lst-0.9.2/ctapipe_io_lst/calibration.py
--rw-r--r--   0 runner    (1001) docker     (121)      546 2021-04-09 13:23:43.000000 ctapipe_io_lst-0.9.2/ctapipe_io_lst/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     5741 2021-04-09 13:23:43.000000 ctapipe_io_lst-0.9.2/ctapipe_io_lst/containers.py
--rw-r--r--   0 runner    (1001) docker     (121)    15625 2021-04-09 13:23:43.000000 ctapipe_io_lst-0.9.2/ctapipe_io_lst/event_time.py
--rw-r--r--   0 runner    (1001) docker     (121)     3955 2021-04-09 13:23:43.000000 ctapipe_io_lst-0.9.2/ctapipe_io_lst/pointing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-09 13:23:48.263992 ctapipe_io_lst-0.9.2/ctapipe_io_lst/resources/
--rw-r--r--   0 runner    (1001) docker     (121)    12434 2021-04-09 13:23:43.000000 ctapipe_io_lst-0.9.2/ctapipe_io_lst/resources/LSTCam-003.camgeom.fits.gz
--rw-r--r--   0 runner    (1001) docker     (121)    12434 2021-04-09 13:23:43.000000 ctapipe_io_lst-0.9.2/ctapipe_io_lst/resources/LSTCam-004.camgeom.fits.gz
--rw-r--r--   0 runner    (1001) docker     (121)      251 2021-04-09 13:23:43.000000 ctapipe_io_lst-0.9.2/ctapipe_io_lst/resources/no_corrections_pulse_LST.dat
--rw-r--r--   0 runner    (1001) docker     (121)    55795 2021-04-09 13:23:43.000000 ctapipe_io_lst-0.9.2/ctapipe_io_lst/resources/oversampled_pulse_LST_8dynode_pix6_20200204.dat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-09 13:23:48.263992 ctapipe_io_lst-0.9.2/ctapipe_io_lst/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-09 13:23:48.271993 ctapipe_io_lst-0.9.2/ctapipe_io_lst/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (121)   462441 2021-04-09 13:23:43.000000 ctapipe_io_lst-0.9.2/ctapipe_io_lst/tests/resources/calibration.Run2462.0000.hdf5
--rw-r--r--   0 runner    (1001) docker     (121)  4854156 2021-04-09 13:23:43.000000 ctapipe_io_lst-0.9.2/ctapipe_io_lst/tests/resources/drs4_pedestal.Run2460.0000.fits.gz
--rw-r--r--   0 runner    (1001) docker     (121)    35968 2021-04-09 13:23:43.000000 ctapipe_io_lst-0.9.2/ctapipe_io_lst/tests/resources/first_caps.hdf5
--rw-r--r--   0 runner    (1001) docker     (121)     8773 2021-04-09 13:23:43.000000 ctapipe_io_lst-0.9.2/ctapipe_io_lst/tests/test_calib.py
--rw-r--r--   0 runner    (1001) docker     (121)     7931 2021-04-09 13:23:43.000000 ctapipe_io_lst-0.9.2/ctapipe_io_lst/tests/test_event_time.py
--rw-r--r--   0 runner    (1001) docker     (121)     3327 2021-04-09 13:23:43.000000 ctapipe_io_lst-0.9.2/ctapipe_io_lst/tests/test_lsteventsource.py
--rw-r--r--   0 runner    (1001) docker     (121)     1644 2021-04-09 13:23:43.000000 ctapipe_io_lst-0.9.2/ctapipe_io_lst/tests/test_pointing.py
--rw-r--r--   0 runner    (1001) docker     (121)     3242 2021-04-09 13:23:43.000000 ctapipe_io_lst-0.9.2/ctapipe_io_lst/tests/test_stage1.py
--rw-r--r--   0 runner    (1001) docker     (121)      100 2021-04-09 13:23:43.000000 ctapipe_io_lst-0.9.2/ctapipe_io_lst/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (121)      814 2021-04-09 13:23:43.000000 ctapipe_io_lst-0.9.2/ctapipe_io_lst/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-09 13:23:48.263992 ctapipe_io_lst-0.9.2/ctapipe_io_lst.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1237 2021-04-09 13:23:48.000000 ctapipe_io_lst-0.9.2/ctapipe_io_lst.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1201 2021-04-09 13:23:48.000000 ctapipe_io_lst-0.9.2/ctapipe_io_lst.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-09 13:23:48.000000 ctapipe_io_lst-0.9.2/ctapipe_io_lst.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       62 2021-04-09 13:23:48.000000 ctapipe_io_lst-0.9.2/ctapipe_io_lst.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2021-04-09 13:23:48.000000 ctapipe_io_lst-0.9.2/ctapipe_io_lst.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)      535 2021-04-09 13:23:43.000000 ctapipe_io_lst-0.9.2/download_test_data.sh
--rw-r--r--   0 runner    (1001) docker     (121)      395 2021-04-09 13:23:43.000000 ctapipe_io_lst-0.9.2/environment.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1227 2021-04-09 13:23:43.000000 ctapipe_io_lst-0.9.2/example_stage1_config.json
--rw-r--r--   0 runner    (1001) docker     (121)      129 2021-04-09 13:23:43.000000 ctapipe_io_lst-0.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      417 2021-04-09 13:23:48.271993 ctapipe_io_lst-0.9.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)      448 2021-04-09 13:23:43.000000 ctapipe_io_lst-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-22 09:41:20.981211 ctapipe_io_lst-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (121)      151 2021-04-22 09:41:11.000000 ctapipe_io_lst-0.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1237 2021-04-22 09:41:20.981211 ctapipe_io_lst-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      725 2021-04-22 09:41:11.000000 ctapipe_io_lst-0.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-22 09:41:20.969211 ctapipe_io_lst-0.9.3/ctapipe_io_lst/
+-rw-r--r--   0 runner    (1001) docker     (121)    27587 2021-04-22 09:41:11.000000 ctapipe_io_lst-0.9.3/ctapipe_io_lst/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      142 2021-04-22 09:41:20.000000 ctapipe_io_lst-0.9.3/ctapipe_io_lst/_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1547 2021-04-22 09:41:11.000000 ctapipe_io_lst-0.9.3/ctapipe_io_lst/anyarray_dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30444 2021-04-22 09:41:11.000000 ctapipe_io_lst-0.9.3/ctapipe_io_lst/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (121)      546 2021-04-22 09:41:11.000000 ctapipe_io_lst-0.9.3/ctapipe_io_lst/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5741 2021-04-22 09:41:11.000000 ctapipe_io_lst-0.9.3/ctapipe_io_lst/containers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15625 2021-04-22 09:41:11.000000 ctapipe_io_lst-0.9.3/ctapipe_io_lst/event_time.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3955 2021-04-22 09:41:11.000000 ctapipe_io_lst-0.9.3/ctapipe_io_lst/pointing.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-22 09:41:20.969211 ctapipe_io_lst-0.9.3/ctapipe_io_lst/resources/
+-rw-r--r--   0 runner    (1001) docker     (121)    12434 2021-04-22 09:41:11.000000 ctapipe_io_lst-0.9.3/ctapipe_io_lst/resources/LSTCam-003.camgeom.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (121)    12434 2021-04-22 09:41:11.000000 ctapipe_io_lst-0.9.3/ctapipe_io_lst/resources/LSTCam-004.camgeom.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (121)      251 2021-04-22 09:41:11.000000 ctapipe_io_lst-0.9.3/ctapipe_io_lst/resources/no_corrections_pulse_LST.dat
+-rw-r--r--   0 runner    (1001) docker     (121)    55795 2021-04-22 09:41:11.000000 ctapipe_io_lst-0.9.3/ctapipe_io_lst/resources/oversampled_pulse_LST_8dynode_pix6_20200204.dat
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-22 09:41:20.969211 ctapipe_io_lst-0.9.3/ctapipe_io_lst/tests/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-22 09:41:20.981211 ctapipe_io_lst-0.9.3/ctapipe_io_lst/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (121)   462441 2021-04-22 09:41:11.000000 ctapipe_io_lst-0.9.3/ctapipe_io_lst/tests/resources/calibration.Run2462.0000.hdf5
+-rw-r--r--   0 runner    (1001) docker     (121)  4854156 2021-04-22 09:41:11.000000 ctapipe_io_lst-0.9.3/ctapipe_io_lst/tests/resources/drs4_pedestal.Run2460.0000.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (121)    35968 2021-04-22 09:41:11.000000 ctapipe_io_lst-0.9.3/ctapipe_io_lst/tests/resources/first_caps.hdf5
+-rw-r--r--   0 runner    (1001) docker     (121)     9183 2021-04-22 09:41:11.000000 ctapipe_io_lst-0.9.3/ctapipe_io_lst/tests/test_calib.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7931 2021-04-22 09:41:11.000000 ctapipe_io_lst-0.9.3/ctapipe_io_lst/tests/test_event_time.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3327 2021-04-22 09:41:11.000000 ctapipe_io_lst-0.9.3/ctapipe_io_lst/tests/test_lsteventsource.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1644 2021-04-22 09:41:11.000000 ctapipe_io_lst-0.9.3/ctapipe_io_lst/tests/test_pointing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3242 2021-04-22 09:41:11.000000 ctapipe_io_lst-0.9.3/ctapipe_io_lst/tests/test_stage1.py
+-rw-r--r--   0 runner    (1001) docker     (121)      100 2021-04-22 09:41:11.000000 ctapipe_io_lst-0.9.3/ctapipe_io_lst/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)      814 2021-04-22 09:41:11.000000 ctapipe_io_lst-0.9.3/ctapipe_io_lst/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-22 09:41:20.969211 ctapipe_io_lst-0.9.3/ctapipe_io_lst.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1237 2021-04-22 09:41:20.000000 ctapipe_io_lst-0.9.3/ctapipe_io_lst.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1201 2021-04-22 09:41:20.000000 ctapipe_io_lst-0.9.3/ctapipe_io_lst.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-22 09:41:20.000000 ctapipe_io_lst-0.9.3/ctapipe_io_lst.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       62 2021-04-22 09:41:20.000000 ctapipe_io_lst-0.9.3/ctapipe_io_lst.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2021-04-22 09:41:20.000000 ctapipe_io_lst-0.9.3/ctapipe_io_lst.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (121)      535 2021-04-22 09:41:11.000000 ctapipe_io_lst-0.9.3/download_test_data.sh
+-rw-r--r--   0 runner    (1001) docker     (121)      395 2021-04-22 09:41:11.000000 ctapipe_io_lst-0.9.3/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1227 2021-04-22 09:41:11.000000 ctapipe_io_lst-0.9.3/example_stage1_config.json
+-rw-r--r--   0 runner    (1001) docker     (121)      129 2021-04-22 09:41:11.000000 ctapipe_io_lst-0.9.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      417 2021-04-22 09:41:20.981211 ctapipe_io_lst-0.9.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (121)      448 2021-04-22 09:41:11.000000 ctapipe_io_lst-0.9.3/setup.py
```

### Comparing `ctapipe_io_lst-0.9.2/PKG-INFO` & `ctapipe_io_lst-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctapipe_io_lst
-Version: 0.9.2
+Version: 0.9.3
 Summary: ctapipe plugin for reading LST prototype files
 Home-page: UNKNOWN
 Author: LST Consortium
 Author-email: cassol@cppm.in2p3.fr
 License: MIT
 Description: # ctapipe_io_lst [![Build Status](https://github.com/cta-observatory/ctapipe_io_lst/workflows/CI/badge.svg?branch=master)](https://github.com/cta-observatory/ctapipe_io_lst/actions?query=workflow%3ACI+branch%3Amaster)
```

### Comparing `ctapipe_io_lst-0.9.2/README.md` & `ctapipe_io_lst-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `ctapipe_io_lst-0.9.2/ctapipe_io_lst/__init__.py` & `ctapipe_io_lst-0.9.3/ctapipe_io_lst/__init__.py`

 * *Files identical despite different names*

### Comparing `ctapipe_io_lst-0.9.2/ctapipe_io_lst/anyarray_dtypes.py` & `ctapipe_io_lst-0.9.3/ctapipe_io_lst/anyarray_dtypes.py`

 * *Files identical despite different names*

### Comparing `ctapipe_io_lst-0.9.2/ctapipe_io_lst/calibration.py` & `ctapipe_io_lst-0.9.3/ctapipe_io_lst/calibration.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,15 +207,15 @@
             end = self.r1_sample_end.tel[tel_id]
             r1.waveform = r1.waveform[..., start:end]
             waveform = r1.waveform
 
             waveform -= self.offset.tel[tel_id]
 
             mon = event.mon.tel[tel_id]
-            waveform[mon.pixel_status.hardware_failing_pixels] = np.nan
+            waveform[mon.pixel_status.hardware_failing_pixels] = 0.0
 
     def update_first_capacitors(self, event: ArrayEventContainer):
         for tel_id in event.r0.tel:
             lst = event.lst.tel[tel_id]
             self.first_cap_old[tel_id] = self.first_cap[tel_id]
             self.first_cap[tel_id] = get_first_capacitors_for_pixels(
                 lst.evt.first_capacitor_id,
@@ -239,15 +239,15 @@
             # subtract pedestal and convert to pe
             if self.mon_data is not None:
                 calibration = self.mon_data.tel[tel_id].calibration
                 waveform -= calibration.pedestal_per_sample[:, :, np.newaxis]
                 waveform *= calibration.dc_to_pe[:, :, np.newaxis]
 
             mon = event.mon.tel[tel_id]
-            waveform[mon.pixel_status.hardware_failing_pixels] = np.nan
+            waveform[mon.pixel_status.hardware_failing_pixels] = 0.0
 
             waveform = waveform.astype(np.float32)
             n_gains, n_pixels, n_samples = waveform.shape
             pixel_index = np.arange(n_pixels)
 
             if selected_gain_channel is not None:
                 r1.waveform = waveform[selected_gain_channel, pixel_index]
```

### Comparing `ctapipe_io_lst-0.9.2/ctapipe_io_lst/constants.py` & `ctapipe_io_lst-0.9.3/ctapipe_io_lst/constants.py`

 * *Files identical despite different names*

### Comparing `ctapipe_io_lst-0.9.2/ctapipe_io_lst/containers.py` & `ctapipe_io_lst-0.9.3/ctapipe_io_lst/containers.py`

 * *Files identical despite different names*

### Comparing `ctapipe_io_lst-0.9.2/ctapipe_io_lst/event_time.py` & `ctapipe_io_lst-0.9.3/ctapipe_io_lst/event_time.py`

 * *Files identical despite different names*

### Comparing `ctapipe_io_lst-0.9.2/ctapipe_io_lst/pointing.py` & `ctapipe_io_lst-0.9.3/ctapipe_io_lst/pointing.py`

 * *Files identical despite different names*

### Comparing `ctapipe_io_lst-0.9.2/ctapipe_io_lst/resources/LSTCam-003.camgeom.fits.gz` & `ctapipe_io_lst-0.9.3/ctapipe_io_lst/resources/LSTCam-003.camgeom.fits.gz`

 * *Files identical despite different names*

### Comparing `ctapipe_io_lst-0.9.2/ctapipe_io_lst/resources/LSTCam-004.camgeom.fits.gz` & `ctapipe_io_lst-0.9.3/ctapipe_io_lst/resources/LSTCam-004.camgeom.fits.gz`

 * *Files identical despite different names*

### Comparing `ctapipe_io_lst-0.9.2/ctapipe_io_lst/resources/oversampled_pulse_LST_8dynode_pix6_20200204.dat` & `ctapipe_io_lst-0.9.3/ctapipe_io_lst/resources/oversampled_pulse_LST_8dynode_pix6_20200204.dat`

 * *Files identical despite different names*

### Comparing `ctapipe_io_lst-0.9.2/ctapipe_io_lst/tests/resources/calibration.Run2462.0000.hdf5` & `ctapipe_io_lst-0.9.3/ctapipe_io_lst/tests/resources/calibration.Run2462.0000.hdf5`

 * *Files identical despite different names*

### Comparing `ctapipe_io_lst-0.9.2/ctapipe_io_lst/tests/resources/drs4_pedestal.Run2460.0000.fits.gz` & `ctapipe_io_lst-0.9.3/ctapipe_io_lst/tests/resources/drs4_pedestal.Run2460.0000.fits.gz`

 * *Files identical despite different names*

### Comparing `ctapipe_io_lst-0.9.2/ctapipe_io_lst/tests/resources/first_caps.hdf5` & `ctapipe_io_lst-0.9.3/ctapipe_io_lst/tests/resources/first_caps.hdf5`

 * *Files identical despite different names*

### Comparing `ctapipe_io_lst-0.9.2/ctapipe_io_lst/tests/test_calib.py` & `ctapipe_io_lst-0.9.3/ctapipe_io_lst/tests/test_calib.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from ctapipe_io_lst.constants import HIGH_GAIN
 import os
 from pathlib import Path
 from traitlets.config import Config
 import numpy as np
 import tables
 import pkg_resources
 
@@ -178,16 +179,26 @@
     )
 
     assert source.r0_r1_calibrator.mon_data is not None
     with source:
         for event in source:
             waveform = event.r1.tel[1].waveform
             assert waveform is not None
-            assert np.count_nonzero(np.isnan(waveform)) == N_PIXELS_MODULE * (N_SAMPLES - 4)
-            assert np.all(np.isnan(waveform[514]))
+
+
+            failing_pixels = event.mon.tel[1].pixel_status.hardware_failing_pixels
+
+            # one module failed, in each gain channel
+            assert np.count_nonzero(failing_pixels) ==  2 * N_PIXELS_MODULE
+
+            # there might be zeros in other pixels than just the broken ones
+            assert np.count_nonzero(waveform == 0) >= N_PIXELS_MODULE * (N_SAMPLES - 4)
+
+            # waveforms in failing pixels must be all 0
+            assert np.all(waveform[failing_pixels[HIGH_GAIN]] == 0)
 
 def test_no_gain_selection():
     from ctapipe_io_lst import LSTEventSource
     from ctapipe_io_lst.constants import N_PIXELS, N_GAINS, N_SAMPLES
 
     config = Config({
         'LSTEventSource': {
```

### Comparing `ctapipe_io_lst-0.9.2/ctapipe_io_lst/tests/test_event_time.py` & `ctapipe_io_lst-0.9.3/ctapipe_io_lst/tests/test_event_time.py`

 * *Files identical despite different names*

### Comparing `ctapipe_io_lst-0.9.2/ctapipe_io_lst/tests/test_lsteventsource.py` & `ctapipe_io_lst-0.9.3/ctapipe_io_lst/tests/test_lsteventsource.py`

 * *Files identical despite different names*

### Comparing `ctapipe_io_lst-0.9.2/ctapipe_io_lst/tests/test_pointing.py` & `ctapipe_io_lst-0.9.3/ctapipe_io_lst/tests/test_pointing.py`

 * *Files identical despite different names*

### Comparing `ctapipe_io_lst-0.9.2/ctapipe_io_lst/tests/test_stage1.py` & `ctapipe_io_lst-0.9.3/ctapipe_io_lst/tests/test_stage1.py`

 * *Files identical despite different names*

### Comparing `ctapipe_io_lst-0.9.2/ctapipe_io_lst/version.py` & `ctapipe_io_lst-0.9.3/ctapipe_io_lst/version.py`

 * *Files identical despite different names*

### Comparing `ctapipe_io_lst-0.9.2/ctapipe_io_lst.egg-info/PKG-INFO` & `ctapipe_io_lst-0.9.3/ctapipe_io_lst.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctapipe-io-lst
-Version: 0.9.2
+Version: 0.9.3
 Summary: ctapipe plugin for reading LST prototype files
 Home-page: UNKNOWN
 Author: LST Consortium
 Author-email: cassol@cppm.in2p3.fr
 License: MIT
 Description: # ctapipe_io_lst [![Build Status](https://github.com/cta-observatory/ctapipe_io_lst/workflows/CI/badge.svg?branch=master)](https://github.com/cta-observatory/ctapipe_io_lst/actions?query=workflow%3ACI+branch%3Amaster)
```

### Comparing `ctapipe_io_lst-0.9.2/ctapipe_io_lst.egg-info/SOURCES.txt` & `ctapipe_io_lst-0.9.3/ctapipe_io_lst.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ctapipe_io_lst-0.9.2/download_test_data.sh` & `ctapipe_io_lst-0.9.3/download_test_data.sh`

 * *Files identical despite different names*

### Comparing `ctapipe_io_lst-0.9.2/example_stage1_config.json` & `ctapipe_io_lst-0.9.3/example_stage1_config.json`

 * *Files identical despite different names*

