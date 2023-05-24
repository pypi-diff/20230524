# Comparing `tmp/pickled_carrots-0.1.5.tar.gz` & `tmp/pickled_carrots-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pickled_carrots-0.1.5.tar", max compression
+gzip compressed data, was "pickled_carrots-0.1.6.tar", max compression
```

## Comparing `pickled_carrots-0.1.5.tar` & `pickled_carrots-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1309 2023-05-19 17:43:26.854143 pickled_carrots-0.1.5/README.md
--rw-r--r--   0        0        0    43329 2023-05-19 18:09:07.525014 pickled_carrots-0.1.5/pickled_carrots/DPData.py
--rw-r--r--   0        0        0    89223 2023-05-19 18:09:07.461011 pickled_carrots-0.1.5/pickled_carrots/DPPlot.py
--rw-r--r--   0        0        0    44076 2023-05-19 18:09:07.521014 pickled_carrots-0.1.5/pickled_carrots/DPUtil.py
--rw-r--r--   0        0        0      464 2023-05-19 18:09:07.477012 pickled_carrots-0.1.5/pickled_carrots/__init__.py
--rw-r--r--   0        0        0    90206 2023-05-19 18:09:07.517014 pickled_carrots-0.1.5/pickled_carrots/database.py
--rw-r--r--   0        0        0    22267 2023-05-19 18:09:07.549015 pickled_carrots-0.1.5/pickled_carrots/dataclass.py
--rw-r--r--   0        0        0    32719 2023-05-19 18:09:07.541015 pickled_carrots-0.1.5/pickled_carrots/mathutil.py
--rw-r--r--   0        0        0    36342 2023-05-19 18:09:07.473012 pickled_carrots-0.1.5/pickled_carrots/plot.py
--rw-r--r--   0        0        0       19 2023-05-20 10:55:16.214096 pickled_carrots-0.1.5/pickled_carrots/vinegar/__init__.py
--rw-r--r--   0        0        0    15989 2023-05-23 20:57:57.969769 pickled_carrots-0.1.5/pickled_carrots/vinegar/core.py
--rw-r--r--   0        0        0     5547 2023-05-23 21:08:20.226797 pickled_carrots-0.1.5/pickled_carrots/vinegar/event.py
--rw-r--r--   0        0        0     1016 2023-05-19 18:44:55.447828 pickled_carrots-0.1.5/pickled_carrots/vinegar/inventory.py
--rw-r--r--   0        0        0      691 2023-05-23 21:03:16.276618 pickled_carrots-0.1.5/pickled_carrots/vinegar/tests/test_read_hsf.py
--rw-r--r--   0        0        0   138961 2023-05-23 21:02:01.777143 pickled_carrots-0.1.5/pickled_carrots/waveforms.py
--rw-r--r--   0        0        0      678 2023-05-23 22:51:24.428568 pickled_carrots-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2469 1970-01-01 00:00:00.000000 pickled_carrots-0.1.5/setup.py
--rw-r--r--   0        0        0     2413 1970-01-01 00:00:00.000000 pickled_carrots-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1309 2023-05-19 17:43:26.854143 pickled_carrots-0.1.6/README.md
+-rw-r--r--   0        0        0    43329 2023-05-19 18:09:07.525014 pickled_carrots-0.1.6/pickled_carrots/DPData.py
+-rw-r--r--   0        0        0    89223 2023-05-19 18:09:07.461011 pickled_carrots-0.1.6/pickled_carrots/DPPlot.py
+-rw-r--r--   0        0        0    44076 2023-05-19 18:09:07.521014 pickled_carrots-0.1.6/pickled_carrots/DPUtil.py
+-rw-r--r--   0        0        0      464 2023-05-19 18:09:07.477012 pickled_carrots-0.1.6/pickled_carrots/__init__.py
+-rw-r--r--   0        0        0    90206 2023-05-19 18:09:07.517014 pickled_carrots-0.1.6/pickled_carrots/database.py
+-rw-r--r--   0        0        0    22267 2023-05-19 18:09:07.549015 pickled_carrots-0.1.6/pickled_carrots/dataclass.py
+-rw-r--r--   0        0        0    32719 2023-05-19 18:09:07.541015 pickled_carrots-0.1.6/pickled_carrots/mathutil.py
+-rw-r--r--   0        0        0    36342 2023-05-19 18:09:07.473012 pickled_carrots-0.1.6/pickled_carrots/plot.py
+-rw-r--r--   0        0        0       19 2023-05-20 10:55:16.214096 pickled_carrots-0.1.6/pickled_carrots/vinegar/__init__.py
+-rw-r--r--   0        0        0    16132 2023-05-23 22:54:44.753901 pickled_carrots-0.1.6/pickled_carrots/vinegar/core.py
+-rw-r--r--   0        0        0     5547 2023-05-23 21:08:20.226797 pickled_carrots-0.1.6/pickled_carrots/vinegar/event.py
+-rw-r--r--   0        0        0     1016 2023-05-19 18:44:55.447828 pickled_carrots-0.1.6/pickled_carrots/vinegar/inventory.py
+-rw-r--r--   0        0        0      691 2023-05-23 21:03:16.276618 pickled_carrots-0.1.6/pickled_carrots/vinegar/tests/test_read_hsf.py
+-rw-r--r--   0        0        0   138961 2023-05-23 21:02:01.777143 pickled_carrots-0.1.6/pickled_carrots/waveforms.py
+-rw-r--r--   0        0        0      678 2023-05-23 22:59:23.302878 pickled_carrots-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2469 1970-01-01 00:00:00.000000 pickled_carrots-0.1.6/setup.py
+-rw-r--r--   0        0        0     2413 1970-01-01 00:00:00.000000 pickled_carrots-0.1.6/PKG-INFO
```

### Comparing `pickled_carrots-0.1.5/README.md` & `pickled_carrots-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `pickled_carrots-0.1.5/pickled_carrots/DPData.py` & `pickled_carrots-0.1.6/pickled_carrots/DPData.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-0.1.5/pickled_carrots/DPPlot.py` & `pickled_carrots-0.1.6/pickled_carrots/DPPlot.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-0.1.5/pickled_carrots/DPUtil.py` & `pickled_carrots-0.1.6/pickled_carrots/DPUtil.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-0.1.5/pickled_carrots/database.py` & `pickled_carrots-0.1.6/pickled_carrots/database.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-0.1.5/pickled_carrots/dataclass.py` & `pickled_carrots-0.1.6/pickled_carrots/dataclass.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-0.1.5/pickled_carrots/mathutil.py` & `pickled_carrots-0.1.6/pickled_carrots/mathutil.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-0.1.5/pickled_carrots/plot.py` & `pickled_carrots-0.1.6/pickled_carrots/plot.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-0.1.5/pickled_carrots/vinegar/core.py` & `pickled_carrots-0.1.6/pickled_carrots/vinegar/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,24 +22,26 @@
 from ipdb import set_trace
 reload(event)
 
 lookups = HeaderLookups()
 
 
 class HSFHandler(object):
-    def __init__(self, st, header, network):
+    def __init__(self, st, header, network, experimental=False):
         self.st = Stream(st)
         self.header = header
         self.network_code = network
+        self.experimental = experimental
 
     @classmethod
     def from_hsf_file(cls, hsf_path, network):
-        st, header = hsf_to_obspy(hsf_path, print_out=False, experimental=True,
+        st, header = hsf_to_obspy(hsf_path, print_out=False,
+                                  experimental=False,
                                   groundmotion=False, return_head=True)
-        return cls(st, header, network)
+        return cls(st, header, network, experimental=False)
 
     @property
     def event_type(self):
         ev_type = self.header['evtype']
         if ev_type < 12:
             return self.event_type_look_up[ev_type]
         else:
@@ -281,19 +283,19 @@
         return Catalog(events=[self.event])
 
     @property
     def file_bundle(self):
         return FileBundleHandler(self.stream, self.catalog, self.inventory)
 
     @classmethod
-    def read(cls, file_path, network):
+    def read(cls, file_path, network, experimental=False):
         with tempfile.NamedTemporaryFile(delete=True) as tmpfile:
             st, head = waveforms.hsf_to_obspy(file_path, print_out=False,
                                               groundmotion=False, return_head=True,
-                                              experimental=False)
+                                              experimental=experimental)
 
         # convert voltage into 32 bits integer (ADC counts)
         volt_ranges = expand_list(head['volt_range'], head['ch_descr'])
         previous_stations = []
         i = 0
         for tr, volt_range in zip(st, volt_ranges):
             if tr.stats.station not in previous_stations:
```

### Comparing `pickled_carrots-0.1.5/pickled_carrots/vinegar/event.py` & `pickled_carrots-0.1.6/pickled_carrots/vinegar/event.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-0.1.5/pickled_carrots/vinegar/inventory.py` & `pickled_carrots-0.1.6/pickled_carrots/vinegar/inventory.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-0.1.5/pickled_carrots/vinegar/tests/test_read_hsf.py` & `pickled_carrots-0.1.6/pickled_carrots/vinegar/tests/test_read_hsf.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-0.1.5/pickled_carrots/waveforms.py` & `pickled_carrots-0.1.6/pickled_carrots/waveforms.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-0.1.5/pyproject.toml` & `pickled_carrots-0.1.6/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pickled_carrots"
-version = "0.1.5"
+version = "0.1.6"
 description = ""
 authors = ["pickled cattots team"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 plotly = "^5.14.1"
```

### Comparing `pickled_carrots-0.1.5/setup.py` & `pickled_carrots-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
  'pytz>=2023.3,<2024.0',
  'shapely>=2.0.1,<3.0.0',
  'statsmodels>=0.14.0,<0.15.0',
  'uquake>=1.2.4,<2.0.0']
 
 setup_kwargs = {
     'name': 'pickled-carrots',
-    'version': '0.1.5',
+    'version': '0.1.6',
     'description': '',
     'long_description': "# ESG_Research\n\nThis repository contains Python and C# code which is used for various different functions. In this document we will go through what each folder contains.\n\n__Analytics_Notebooks__\n\nThis folder contains Jupyter notebooks which have various different functionalities. More notebooks can be found on the DataShare, under Frac4/Notebooks.\n\n&nbsp;\n\n\n__ESG-dash__\n\nA dash-based dashboard for evaluating sensor quality for mining sites.\n\n&nbsp;\n\n\n__ESG__\n\nThe main module folder for our Python codes. The files within this folder are used in most of our jupyter notebooks. More details on what each file contains can be found in the folder.\n\n&nbsp;\n\n__ITG-FMC__\n\nContains the tiltmeter processing dashboard written in Python, a Fiber processing C# app, a DPA and DPA-RTA C# app, and a copy of the Stress Inversion python package (which has since been merged into the main ESG repo.\n\n&nbsp;\n\n__Scripts__\n\nContains various Python scripts which are used to automated processes such as HypoDD or noise analysis.\n\n&nbsp;\n\n__build/lib, dist, esg_das, esg_dts__\n\nPython code for processing Fiber data. \n\n&nbsp;\n\n__Miscellaneous__\n\nThere are some additional files in this folder which are related to replicated anaconda environments. The requirements.txt file can be used to create ESG's default environment.\n",
     'author': 'pickled cattots team',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pickled_carrots-0.1.5/PKG-INFO` & `pickled_carrots-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pickled-carrots
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Author: pickled cattots team
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

