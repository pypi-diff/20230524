# Comparing `tmp/pickled_carrots-0.1.4.tar.gz` & `tmp/pickled_carrots-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pickled_carrots-0.1.4.tar", max compression
+gzip compressed data, was "pickled_carrots-0.1.5.tar", max compression
```

## Comparing `pickled_carrots-0.1.4.tar` & `pickled_carrots-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1309 2023-05-19 17:43:26.854143 pickled_carrots-0.1.4/README.md
--rw-r--r--   0        0        0    43329 2023-05-19 18:09:07.525014 pickled_carrots-0.1.4/pickled_carrots/DPData.py
--rw-r--r--   0        0        0    89223 2023-05-19 18:09:07.461011 pickled_carrots-0.1.4/pickled_carrots/DPPlot.py
--rw-r--r--   0        0        0    44076 2023-05-19 18:09:07.521014 pickled_carrots-0.1.4/pickled_carrots/DPUtil.py
--rw-r--r--   0        0        0      464 2023-05-19 18:09:07.477012 pickled_carrots-0.1.4/pickled_carrots/__init__.py
--rw-r--r--   0        0        0    90206 2023-05-19 18:09:07.517014 pickled_carrots-0.1.4/pickled_carrots/database.py
--rw-r--r--   0        0        0    22267 2023-05-19 18:09:07.549015 pickled_carrots-0.1.4/pickled_carrots/dataclass.py
--rw-r--r--   0        0        0    32719 2023-05-19 18:09:07.541015 pickled_carrots-0.1.4/pickled_carrots/mathutil.py
--rw-r--r--   0        0        0    36342 2023-05-19 18:09:07.473012 pickled_carrots-0.1.4/pickled_carrots/plot.py
--rw-r--r--   0        0        0       19 2023-05-20 10:55:16.214096 pickled_carrots-0.1.4/pickled_carrots/vinegar/__init__.py
--rw-r--r--   0        0        0    15989 2023-05-20 11:21:14.081943 pickled_carrots-0.1.4/pickled_carrots/vinegar/core.py
--rw-r--r--   0        0        0     5481 2023-05-19 17:53:39.362318 pickled_carrots-0.1.4/pickled_carrots/vinegar/event.py
--rw-r--r--   0        0        0     1016 2023-05-19 18:44:55.447828 pickled_carrots-0.1.4/pickled_carrots/vinegar/inventory.py
--rw-r--r--   0        0        0      650 2023-05-19 21:07:21.294282 pickled_carrots-0.1.4/pickled_carrots/vinegar/tests/read_hsf.py
--rw-r--r--   0        0        0   138903 2023-05-19 21:13:13.562541 pickled_carrots-0.1.4/pickled_carrots/waveforms.py
--rw-r--r--   0        0        0      678 2023-05-23 14:37:50.380891 pickled_carrots-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2469 1970-01-01 00:00:00.000000 pickled_carrots-0.1.4/setup.py
--rw-r--r--   0        0        0     2413 1970-01-01 00:00:00.000000 pickled_carrots-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1309 2023-05-19 17:43:26.854143 pickled_carrots-0.1.5/README.md
+-rw-r--r--   0        0        0    43329 2023-05-19 18:09:07.525014 pickled_carrots-0.1.5/pickled_carrots/DPData.py
+-rw-r--r--   0        0        0    89223 2023-05-19 18:09:07.461011 pickled_carrots-0.1.5/pickled_carrots/DPPlot.py
+-rw-r--r--   0        0        0    44076 2023-05-19 18:09:07.521014 pickled_carrots-0.1.5/pickled_carrots/DPUtil.py
+-rw-r--r--   0        0        0      464 2023-05-19 18:09:07.477012 pickled_carrots-0.1.5/pickled_carrots/__init__.py
+-rw-r--r--   0        0        0    90206 2023-05-19 18:09:07.517014 pickled_carrots-0.1.5/pickled_carrots/database.py
+-rw-r--r--   0        0        0    22267 2023-05-19 18:09:07.549015 pickled_carrots-0.1.5/pickled_carrots/dataclass.py
+-rw-r--r--   0        0        0    32719 2023-05-19 18:09:07.541015 pickled_carrots-0.1.5/pickled_carrots/mathutil.py
+-rw-r--r--   0        0        0    36342 2023-05-19 18:09:07.473012 pickled_carrots-0.1.5/pickled_carrots/plot.py
+-rw-r--r--   0        0        0       19 2023-05-20 10:55:16.214096 pickled_carrots-0.1.5/pickled_carrots/vinegar/__init__.py
+-rw-r--r--   0        0        0    15989 2023-05-23 20:57:57.969769 pickled_carrots-0.1.5/pickled_carrots/vinegar/core.py
+-rw-r--r--   0        0        0     5547 2023-05-23 21:08:20.226797 pickled_carrots-0.1.5/pickled_carrots/vinegar/event.py
+-rw-r--r--   0        0        0     1016 2023-05-19 18:44:55.447828 pickled_carrots-0.1.5/pickled_carrots/vinegar/inventory.py
+-rw-r--r--   0        0        0      691 2023-05-23 21:03:16.276618 pickled_carrots-0.1.5/pickled_carrots/vinegar/tests/test_read_hsf.py
+-rw-r--r--   0        0        0   138961 2023-05-23 21:02:01.777143 pickled_carrots-0.1.5/pickled_carrots/waveforms.py
+-rw-r--r--   0        0        0      678 2023-05-23 22:51:24.428568 pickled_carrots-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2469 1970-01-01 00:00:00.000000 pickled_carrots-0.1.5/setup.py
+-rw-r--r--   0        0        0     2413 1970-01-01 00:00:00.000000 pickled_carrots-0.1.5/PKG-INFO
```

### Comparing `pickled_carrots-0.1.4/README.md` & `pickled_carrots-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pickled_carrots-0.1.4/pickled_carrots/DPData.py` & `pickled_carrots-0.1.5/pickled_carrots/DPData.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-0.1.4/pickled_carrots/DPPlot.py` & `pickled_carrots-0.1.5/pickled_carrots/DPPlot.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-0.1.4/pickled_carrots/DPUtil.py` & `pickled_carrots-0.1.5/pickled_carrots/DPUtil.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-0.1.4/pickled_carrots/database.py` & `pickled_carrots-0.1.5/pickled_carrots/database.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-0.1.4/pickled_carrots/dataclass.py` & `pickled_carrots-0.1.5/pickled_carrots/dataclass.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-0.1.4/pickled_carrots/mathutil.py` & `pickled_carrots-0.1.5/pickled_carrots/mathutil.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-0.1.4/pickled_carrots/plot.py` & `pickled_carrots-0.1.5/pickled_carrots/plot.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-0.1.4/pickled_carrots/vinegar/core.py` & `pickled_carrots-0.1.5/pickled_carrots/vinegar/core.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-0.1.4/pickled_carrots/vinegar/event.py` & `pickled_carrots-0.1.5/pickled_carrots/vinegar/event.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,34 +46,35 @@
 
     return event
 
 
 def magnitudes_from_catalog(head, evaluation_mode, evaluation_status):
     magnitudes = []
 
-    energy = head['energy_p'] + head['energy_sh'] + head['energy_sh']
-    energy = energy[np.nonzero(energy)]
+    energy = np.array(head['energy_p'] + head['energy_sh'] + head['energy_sh']).flatten()
+    energy = energy[np.nonzero(energy)[0]]
     energy = np.median(energy)
     # energy = 1
     magnitude = Magnitude()
     magnitude.magnitude_type = 'Mw'
     magnitude.mag = head['mw']
     # magnitude.seismic_moment = catalog_line['SeiMoment']
     e_p = energy / (1 + head['esep'])
     e_s = e_p * head['esep']
     magnitude.energy_s_joule = e_s
     magnitude.energy_p_joule = e_p
     magnitude.energy_joule = e_s + e_p
     magnitude.moment_magnitude_uncertainty = 0
-    magnitude.corner_frequency_p_hz = np.median(head['corner_p'][np.nonzero(
-        head['corner_p'])])
-    magnitude.corner_frequency_s_hz = np.median(head['corner_s'][np.nonzero(
-        head['corner_s'])])
-    magnitude.corner_frequency_hz = np.median(head['corner_p'][np.nonzero(
-        head['corner_p'])])
+    corner_p = np.array(head['corner_p']).flatten()
+    corner_s = np.array(head['corner_p']).flatten()
+    magnitude.corner_frequency_p_hz = np.median(corner_p[np.nonzero(
+        corner_p)[0]])
+    magnitude.corner_frequency_s_hz = np.median(corner_s[np.nonzero(
+        corner_s)[0]])
+    magnitude.corner_frequency_hz = magnitude.corner_frequency_p_hz
     magnitude.evaluation_mode = evaluation_mode
     magnitude.evaluation_status = evaluation_status
 
     magnitudes.append(magnitude)
 
     # local_magnitude = Magnitude()
     # local_magnitude.magnitude_type = 'Ml'
```

### Comparing `pickled_carrots-0.1.4/pickled_carrots/vinegar/inventory.py` & `pickled_carrots-0.1.5/pickled_carrots/vinegar/inventory.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-0.1.4/pickled_carrots/vinegar/tests/read_hsf.py` & `pickled_carrots-0.1.5/pickled_carrots/vinegar/tests/test_read_hsf.py`

 * *Files 26% similar despite different names*

```diff
@@ -17,8 +17,10 @@
                                          groundmotion=False, return_head=True)
 
     t1 = time()
     logger.info(f'done reading the HSF file in {t1 - t0} seconds')
 
     hsf_handler = core.HSFHandler(st, head, 'GBC')
 
-    krapout
+    file_bundle = hsf_handler.file_bundle
+
+    crash
```

### Comparing `pickled_carrots-0.1.4/pickled_carrots/waveforms.py` & `pickled_carrots-0.1.5/pickled_carrots/waveforms.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,16 +140,16 @@
     
     # making sure that rotate is turned on if rotate_to_zrt is turned on
     if rotate_to_zrt or rotate_to_lqt:
         rotate = True
 
     # setting experimental to True when on posix
 
-    if os.name == 'posix':
-        experimental = True
+    # if os.name == 'posix':
+    #     experimental = True
     
     # whether to run the read_hsf function
     if head is None:
         if experimental is False:
             tm, data, head = read_hsf(file=file, groundmotion=groundmotion, print_out=print_out,
                                       from_hsf_to_obspy=True)
         else:
@@ -1090,14 +1090,15 @@
         if os.name != "nt":
             # if we are on the jupyter server
             # adjusting the path of the hsf compressor call
             hsfcompressor = '/usr/bin/wine /home/share/wine/HSFCompressor.exe'
 
         if stdout:
             # Stdout option exists to directly pass waveform data to python
+            logging.info('decompressing the HSFfile')
             p = Popen(hsfcompressor + ' -none -stdout ' + file, stdout=PIPE, stderr=PIPE, shell=True)
             hbin = ''
             err = ''
             try:
                 hbin, err = p.communicate()
             except IOError:
                 print('IOError: ' + str(IOError))
```

### Comparing `pickled_carrots-0.1.4/pyproject.toml` & `pickled_carrots-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pickled_carrots"
-version = "0.1.4"
+version = "0.1.5"
 description = ""
 authors = ["pickled cattots team"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 plotly = "^5.14.1"
```

### Comparing `pickled_carrots-0.1.4/setup.py` & `pickled_carrots-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
  'pytz>=2023.3,<2024.0',
  'shapely>=2.0.1,<3.0.0',
  'statsmodels>=0.14.0,<0.15.0',
  'uquake>=1.2.4,<2.0.0']
 
 setup_kwargs = {
     'name': 'pickled-carrots',
-    'version': '0.1.4',
+    'version': '0.1.5',
     'description': '',
     'long_description': "# ESG_Research\n\nThis repository contains Python and C# code which is used for various different functions. In this document we will go through what each folder contains.\n\n__Analytics_Notebooks__\n\nThis folder contains Jupyter notebooks which have various different functionalities. More notebooks can be found on the DataShare, under Frac4/Notebooks.\n\n&nbsp;\n\n\n__ESG-dash__\n\nA dash-based dashboard for evaluating sensor quality for mining sites.\n\n&nbsp;\n\n\n__ESG__\n\nThe main module folder for our Python codes. The files within this folder are used in most of our jupyter notebooks. More details on what each file contains can be found in the folder.\n\n&nbsp;\n\n__ITG-FMC__\n\nContains the tiltmeter processing dashboard written in Python, a Fiber processing C# app, a DPA and DPA-RTA C# app, and a copy of the Stress Inversion python package (which has since been merged into the main ESG repo.\n\n&nbsp;\n\n__Scripts__\n\nContains various Python scripts which are used to automated processes such as HypoDD or noise analysis.\n\n&nbsp;\n\n__build/lib, dist, esg_das, esg_dts__\n\nPython code for processing Fiber data. \n\n&nbsp;\n\n__Miscellaneous__\n\nThere are some additional files in this folder which are related to replicated anaconda environments. The requirements.txt file can be used to create ESG's default environment.\n",
     'author': 'pickled cattots team',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pickled_carrots-0.1.4/PKG-INFO` & `pickled_carrots-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pickled-carrots
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Author: pickled cattots team
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

