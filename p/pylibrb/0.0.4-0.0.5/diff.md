# Comparing `tmp/pylibrb-0.0.4.tar.gz` & `tmp/pylibrb-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylibrb-0.0.4.tar", last modified: Mon May 22 17:41:52 2023, max compression
+gzip compressed data, was "pylibrb-0.0.5.tar", last modified: Wed May 24 10:27:48 2023, max compression
```

## Comparing `pylibrb-0.0.4.tar` & `pylibrb-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:41:52.297926 pylibrb-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    18091 2023-05-22 17:41:38.000000 pylibrb-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-22 17:41:38.000000 pylibrb-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-22 17:41:52.297926 pylibrb-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-22 17:41:38.000000 pylibrb-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-22 17:41:38.000000 pylibrb-0.0.4/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-22 17:41:38.000000 pylibrb-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-22 17:41:52.297926 pylibrb-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-22 17:41:38.000000 pylibrb-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:41:52.297926 pylibrb-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:41:52.297926 pylibrb-0.0.4/src/pylibrb/
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-22 17:41:38.000000 pylibrb-0.0.4/src/pylibrb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:41:38.000000 pylibrb-0.0.4/src/pylibrb/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    36163 2023-05-22 17:41:38.000000 pylibrb-0.0.4/src/pylibrb/pylibrb_ext.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:41:52.297926 pylibrb-0.0.4/src/pylibrb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-22 17:41:52.000000 pylibrb-0.0.4/src/pylibrb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-22 17:41:52.000000 pylibrb-0.0.4/src/pylibrb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 17:41:52.000000 pylibrb-0.0.4/src/pylibrb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-22 17:41:52.000000 pylibrb-0.0.4/src/pylibrb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-22 17:41:52.000000 pylibrb-0.0.4/src/pylibrb.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:41:52.297926 pylibrb-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-05-22 17:41:38.000000 pylibrb-0.0.4/tests/test_stretcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-22 17:41:38.000000 pylibrb-0.0.4/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:27:48.843157 pylibrb-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    18091 2023-05-24 10:27:35.000000 pylibrb-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-24 10:27:35.000000 pylibrb-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-24 10:27:48.843157 pylibrb-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-24 10:27:35.000000 pylibrb-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-24 10:27:35.000000 pylibrb-0.0.5/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-24 10:27:35.000000 pylibrb-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-24 10:27:48.843157 pylibrb-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-24 10:27:35.000000 pylibrb-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:27:48.839156 pylibrb-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:27:48.843157 pylibrb-0.0.5/src/pylibrb/
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-24 10:27:35.000000 pylibrb-0.0.5/src/pylibrb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 10:27:35.000000 pylibrb-0.0.5/src/pylibrb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    36162 2023-05-24 10:27:35.000000 pylibrb-0.0.5/src/pylibrb/pylibrb_ext.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:27:48.843157 pylibrb-0.0.5/src/pylibrb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-24 10:27:48.000000 pylibrb-0.0.5/src/pylibrb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-24 10:27:48.000000 pylibrb-0.0.5/src/pylibrb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 10:27:48.000000 pylibrb-0.0.5/src/pylibrb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-24 10:27:48.000000 pylibrb-0.0.5/src/pylibrb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-24 10:27:48.000000 pylibrb-0.0.5/src/pylibrb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:27:48.843157 pylibrb-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7061 2023-05-24 10:27:35.000000 pylibrb-0.0.5/tests/test_stretcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-24 10:27:35.000000 pylibrb-0.0.5/tests/test_utils.py
```

### Comparing `pylibrb-0.0.4/LICENSE` & `pylibrb-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pylibrb-0.0.4/PKG-INFO` & `pylibrb-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylibrb
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python bindings for the RubberBand library
 Home-page: https://github.com/pawel-glomski/pylibrb
 Author: Paweł Głomski
 Author-email: pglomski.dev@gmail.com
 License: 'GPLv2'
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Intended Audience :: Developers
```

### Comparing `pylibrb-0.0.4/README.md` & `pylibrb-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pylibrb-0.0.4/setup.cfg` & `pylibrb-0.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `pylibrb-0.0.4/src/pylibrb/__init__.py` & `pylibrb-0.0.5/src/pylibrb/__init__.py`

 * *Files identical despite different names*

### Comparing `pylibrb-0.0.4/src/pylibrb/pylibrb_ext.pyi` & `pylibrb-0.0.5/src/pylibrb/pylibrb_ext.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -761,27 +761,27 @@
         De-interleaved audio data with one float array per channel. Sample values are conventionally
         expected to be in the range -1.0f to +1.0f
       final:
         Is this the last block of input data.
     '''
 
 
-def create_audio_array(channels_num: int, samples_num: int) -> np.ndarray:
+def create_audio_array(channels_num: int, samples_num: int, init_value: float = 0.0) -> np.ndarray:
   '''Creates an array for audio with `channels_num` channels and `samples_num` samples.
 
-  Note that the array elements are not assigned to any value, thus they may contain any values.
-
   Args:
     channels_num:
       Number of channels that the audio will have.
     samples_num:
       Number of samples that the audio will have.
+    init_value:
+      Value that assigned to every element of the array. 
 
   Returns:
-    Numpy ndarray with RubberBand-compatible shape and dtype.
+    Numpy ndarray with pylibrb-compatible shape and dtype.
   '''
 
 
 def set_default_logging_level(level: int) -> None:
   '''Set the default level of debug output for subsequently constructed stretchers.
     
   Args:
```

### Comparing `pylibrb-0.0.4/src/pylibrb.egg-info/PKG-INFO` & `pylibrb-0.0.5/src/pylibrb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylibrb
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python bindings for the RubberBand library
 Home-page: https://github.com/pawel-glomski/pylibrb
 Author: Paweł Głomski
 Author-email: pglomski.dev@gmail.com
 License: 'GPLv2'
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Intended Audience :: Developers
```

### Comparing `pylibrb-0.0.4/tests/test_stretcher.py` & `pylibrb-0.0.5/tests/test_stretcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,16 +145,17 @@
     assert stretcher.retrieve(available_samples).size == 0
 
   @pytest.mark.parametrize('time_ratio', [1.0, 0.5])
   def test_retrieve_should_return_expected_number_of_samples_for_given_time_ratio(
       self, time_ratio: float, realtime_stretcher: RubberBandStretcher):
     stretcher = realtime_stretcher
 
-    audio_data = pylibrb.create_audio_array(stretcher.channels, stretcher.get_samples_required())
-    audio_data[:] = 1
+    audio_data = pylibrb.create_audio_array(stretcher.channels,
+                                            stretcher.get_samples_required(),
+                                            init_value=1)
     audio_samples = audio_data.shape[pylibrb.SAMPLES_AXIS]
 
     expected_samples = 0.0
     observed_samples = 0
     iters = 10
 
     stretcher.time_ratio = 1.0
```

