# Comparing `tmp/cfr-0.4.6.tar.gz` & `tmp/cfr-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfr-0.4.6.tar", last modified: Sat Apr 22 18:56:26 2023, max compression
+gzip compressed data, was "cfr-0.5.0.tar", last modified: Tue May 23 23:17:35 2023, max compression
```

## Comparing `cfr-0.4.6.tar` & `cfr-0.5.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-04-22 18:56:26.570985 cfr-0.4.6/
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1516 2023-03-03 14:30:05.000000 cfr-0.4.6/LICENSE
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1676 2023-04-22 18:56:26.570465 cfr-0.4.6/PKG-INFO
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1112 2023-04-18 00:48:45.000000 cfr-0.4.6/README.rst
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-04-22 18:56:26.554034 cfr-0.4.6/bin/
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     3905 2023-03-03 14:30:05.000000 cfr-0.4.6/bin/cfr
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-04-22 18:56:26.563558 cfr-0.4.6/cfr/
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)      640 2023-03-24 19:14:09.000000 cfr-0.4.6/cfr/__init__.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    18148 2023-04-14 08:22:21.000000 cfr-0.4.6/cfr/climate.py
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-04-22 18:56:26.569798 cfr-0.4.6/cfr/da/
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)       22 2023-03-03 14:30:05.000000 cfr-0.4.6/cfr/da/__init__.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    16319 2023-03-26 05:47:23.000000 cfr-0.4.6/cfr/da/enkf.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    22484 2023-04-17 17:43:24.000000 cfr-0.4.6/cfr/gcm.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     7623 2023-03-03 14:30:05.000000 cfr-0.4.6/cfr/ml.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    61428 2023-04-22 04:02:32.000000 cfr-0.4.6/cfr/proxy.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    44996 2023-04-22 03:20:57.000000 cfr-0.4.6/cfr/psm.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    49933 2023-04-09 06:47:02.000000 cfr-0.4.6/cfr/reconjob.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     2311 2023-03-26 06:27:24.000000 cfr-0.4.6/cfr/reconres.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    17830 2023-04-06 07:20:24.000000 cfr-0.4.6/cfr/ts.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    20957 2023-04-22 04:02:16.000000 cfr-0.4.6/cfr/utils.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    54810 2023-04-06 07:30:44.000000 cfr-0.4.6/cfr/visual.py
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-04-22 18:56:26.568539 cfr-0.4.6/cfr.egg-info/
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1676 2023-04-22 18:56:26.565061 cfr-0.4.6/cfr.egg-info/PKG-INFO
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)      374 2023-04-22 18:56:26.565563 cfr-0.4.6/cfr.egg-info/SOURCES.txt
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)        1 2023-04-22 18:56:26.566306 cfr-0.4.6/cfr.egg-info/dependency_links.txt
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)        1 2023-03-03 14:35:18.000000 cfr-0.4.6/cfr.egg-info/not-zip-safe
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)      203 2023-04-22 18:56:26.567925 cfr-0.4.6/cfr.egg-info/requires.txt
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)        4 2023-04-22 18:56:26.568630 cfr-0.4.6/cfr.egg-info/top_level.txt
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)       38 2023-04-22 18:56:26.571084 cfr-0.4.6/setup.cfg
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1415 2023-04-22 07:25:43.000000 cfr-0.4.6/setup.py
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-05-23 23:17:35.548694 cfr-0.5.0/
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1516 2023-03-03 14:30:05.000000 cfr-0.5.0/LICENSE
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1771 2023-05-23 23:17:35.548393 cfr-0.5.0/PKG-INFO
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1207 2023-04-22 19:12:46.000000 cfr-0.5.0/README.md
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-05-23 23:17:35.527142 cfr-0.5.0/bin/
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     3905 2023-03-03 14:30:05.000000 cfr-0.5.0/bin/cfr
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-05-23 23:17:35.541168 cfr-0.5.0/cfr/
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)      640 2023-03-24 19:14:09.000000 cfr-0.5.0/cfr/__init__.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    18155 2023-04-26 03:15:40.000000 cfr-0.5.0/cfr/climate.py
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-05-23 23:17:35.547167 cfr-0.5.0/cfr/da/
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)       22 2023-03-03 14:30:05.000000 cfr-0.5.0/cfr/da/__init__.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    16319 2023-03-26 05:47:23.000000 cfr-0.5.0/cfr/da/enkf.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    22484 2023-04-17 17:43:24.000000 cfr-0.5.0/cfr/gcm.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     7623 2023-03-03 14:30:05.000000 cfr-0.5.0/cfr/ml.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    61644 2023-05-23 23:10:44.000000 cfr-0.5.0/cfr/proxy.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    44996 2023-04-22 03:20:57.000000 cfr-0.5.0/cfr/psm.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    49933 2023-04-09 06:47:02.000000 cfr-0.5.0/cfr/reconjob.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     2311 2023-03-26 06:27:24.000000 cfr-0.5.0/cfr/reconres.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    17993 2023-04-26 03:13:51.000000 cfr-0.5.0/cfr/ts.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    21303 2023-05-23 23:14:30.000000 cfr-0.5.0/cfr/utils.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    54810 2023-04-06 07:30:44.000000 cfr-0.5.0/cfr/visual.py
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-05-23 23:17:35.545739 cfr-0.5.0/cfr.egg-info/
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1771 2023-05-23 23:17:34.000000 cfr-0.5.0/cfr.egg-info/PKG-INFO
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)      373 2023-05-23 23:17:34.000000 cfr-0.5.0/cfr.egg-info/SOURCES.txt
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)        1 2023-05-23 23:17:34.000000 cfr-0.5.0/cfr.egg-info/dependency_links.txt
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)        1 2023-03-03 14:35:18.000000 cfr-0.5.0/cfr.egg-info/not-zip-safe
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)      203 2023-05-23 23:17:34.000000 cfr-0.5.0/cfr.egg-info/requires.txt
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)        4 2023-05-23 23:17:34.000000 cfr-0.5.0/cfr.egg-info/top_level.txt
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)       38 2023-05-23 23:17:35.548807 cfr-0.5.0/setup.cfg
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1414 2023-05-23 22:58:12.000000 cfr-0.5.0/setup.py
```

### Comparing `cfr-0.4.6/LICENSE` & `cfr-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cfr-0.4.6/PKG-INFO` & `cfr-0.5.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfr
-Version: 0.4.6
+Version: 0.5.0
 Summary: cfr: the Python package for Climate Field Reconstruction
 Home-page: https://github.com/fzhu2e/cfr
 Author: Feng Zhu, Julien Emile-Geay
 Author-email: fengzhu@ucar.edu, julieneg@usc.edu
 License: BSD 3-Clause
 Keywords: paleocliamte reconstruction
 Classifier: Natural Language :: English
@@ -12,26 +12,29 @@
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/x-rst
 Provides-Extra: psm
 Provides-Extra: ml
 Provides-Extra: graphem
 License-File: LICENSE
 
-***********************************************************
-`cfr`: a Python package for Climate Field Reconstruction
-***********************************************************
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7855587.svg)](https://doi.org/10.5281/zenodo.7855587)
+
+# `cfr`: a Python package for Climate Field Reconstruction
 
 `cfr` aims to provide a universal framework for climate field reconstruction (CFR).
 It provides a toolkit for
 
 + the processing and visualization of the proxy records, climate model simulations, and instrumental observations,
-+ the calibration and running of the proxy system models (PSMs, `Evans et al., 2013 <https://doi.org/10.1016/j.quascirev.2013.05.024>`_),
-+ the preparation and running of the multiple reconstruction frameworks/algorithms, such as LMR (`Hakim et al., 2016 <https://doi.org/10.1002/2016JD024751>`_; `Tardif et al., 2019 <https://doi.org/https://doi.org/10.5194/cp-15-1251-2019>`_) and GraphEM (`Guillot et al., 2015 <https://doi.org/10.1214/14-AOAS794>`_), and
++ the calibration and running of the proxy system models (PSMs, [Evans et al., 2013](https://doi.org/10.1016/j.quascirev.2013.05.024)),
++ the preparation and running of the multiple reconstruction frameworks/algorithms, such as LMR ([Hakim et al., 2016](https://doi.org/10.1002/2016JD024751); [Tardif et al., 2019](https://doi.org/https://doi.org/10.5194/cp-15-1251-2019)) and GraphEM ([Guillot et al., 2015](https://doi.org/10.1214/14-AOAS794)), and
 + the validation of the reconstructions, etc.
 
 For more details, please refer to the documentation linked below.
 
-Documentation
-=============
+## Documentation
 
 + Homepage: https://fzhu2e.github.io/cfr
 + Installation: https://fzhu2e.github.io/cfr/ug-installation.html
+
+## How to cite this repo
+
+This repo can be cited with DOI: [10.5281/zenodo.7855587](https://doi.org/10.5281/zenodo.7855587)
```

### Comparing `cfr-0.4.6/README.rst` & `cfr-0.5.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,22 @@
-***********************************************************
-`cfr`: a Python package for Climate Field Reconstruction
-***********************************************************
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7855587.svg)](https://doi.org/10.5281/zenodo.7855587)
+
+# `cfr`: a Python package for Climate Field Reconstruction
 
 `cfr` aims to provide a universal framework for climate field reconstruction (CFR).
 It provides a toolkit for
 
 + the processing and visualization of the proxy records, climate model simulations, and instrumental observations,
-+ the calibration and running of the proxy system models (PSMs, `Evans et al., 2013 <https://doi.org/10.1016/j.quascirev.2013.05.024>`_),
-+ the preparation and running of the multiple reconstruction frameworks/algorithms, such as LMR (`Hakim et al., 2016 <https://doi.org/10.1002/2016JD024751>`_; `Tardif et al., 2019 <https://doi.org/https://doi.org/10.5194/cp-15-1251-2019>`_) and GraphEM (`Guillot et al., 2015 <https://doi.org/10.1214/14-AOAS794>`_), and
++ the calibration and running of the proxy system models (PSMs, [Evans et al., 2013](https://doi.org/10.1016/j.quascirev.2013.05.024)),
++ the preparation and running of the multiple reconstruction frameworks/algorithms, such as LMR ([Hakim et al., 2016](https://doi.org/10.1002/2016JD024751); [Tardif et al., 2019](https://doi.org/https://doi.org/10.5194/cp-15-1251-2019)) and GraphEM ([Guillot et al., 2015](https://doi.org/10.1214/14-AOAS794)), and
 + the validation of the reconstructions, etc.
 
 For more details, please refer to the documentation linked below.
 
-Documentation
-=============
+## Documentation
 
 + Homepage: https://fzhu2e.github.io/cfr
-+ Installation: https://fzhu2e.github.io/cfr/ug-installation.html
++ Installation: https://fzhu2e.github.io/cfr/ug-installation.html
+
+## How to cite this repo
+
+This repo can be cited with DOI: [10.5281/zenodo.7855587](https://doi.org/10.5281/zenodo.7855587)
```

### Comparing `cfr-0.4.6/bin/cfr` & `cfr-0.5.0/bin/cfr`

 * *Files identical despite different names*

### Comparing `cfr-0.4.6/cfr/__init__.py` & `cfr-0.5.0/cfr/__init__.py`

 * *Files identical despite different names*

### Comparing `cfr-0.4.6/cfr/climate.py` & `cfr-0.5.0/cfr/climate.py`

 * *Files 0% similar despite different names*

```diff
@@ -531,9 +531,9 @@
         fd = ClimateField(da)
 
         return  fd
 
     def geo_mean(self, lat_min=-90, lat_max=90, lon_min=0, lon_max=360):
         ''' Calculate the geographical mean value of the climate field. '''
         m = utils.geo_mean(self.da, lat_min=lat_min, lat_max=lat_max, lon_min=lon_min, lon_max=lon_max)
-        ts = EnsTS(time=m['time'], value=m.values)
+        ts = EnsTS(time=m['time'].values, value=m.values)
         return ts
```

### Comparing `cfr-0.4.6/cfr/da/enkf.py` & `cfr-0.5.0/cfr/da/enkf.py`

 * *Files identical despite different names*

### Comparing `cfr-0.4.6/cfr/gcm.py` & `cfr-0.5.0/cfr/gcm.py`

 * *Files identical despite different names*

### Comparing `cfr-0.4.6/cfr/ml.py` & `cfr-0.5.0/cfr/ml.py`

 * *Files identical despite different names*

### Comparing `cfr-0.4.6/cfr/proxy.py` & `cfr-0.5.0/cfr/proxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,30 +132,30 @@
         lat (float): latitude
         lon (float): longitude
         time (numpy.array): time axis in unit of year CE 
         value (numpy.array): proxy value axis
         ptype (str): the label of proxy type according to archive and proxy information;
             some examples:
 
-            * 'tree.trw' : TRW
-            * 'tree.mxd' : MXD
+            * 'tree.trw' : tree-ring width (TRW)
+            * 'tree.mxd' : maximum latewood density (MXD)
             * 'coral.d18O' : Coral d18O isotopes
             * 'coral.SrCa' : Coral Sr/Ca ratios
-            * 'ice.d18O' : Ice d18O isotopes
+            * 'ice.d18O' : Ice core d18O isotopes
         tags (a set of str):
             the tags for the record, to enable tag filtering
     '''
     def __init__(self, pid=None, time=None, value=None, lat=None, lon=None, elev=None, ptype=None, tags=None,
         value_name=None, value_unit=None, time_name=None, time_unit=None, seasonality=None):
         self.pid = pid
         if time is not None:
-            if len(time) == 1:
-                time = [time]
-            if not utils.is_numeric(time):
+            try:
                 time = utils.datetime2year_float(time)
+            except:
+                pass
         self.time = time
         self.value = value
         self.lat = lat
         self.lon = np.mod(lon, 360) if lon is not None else None
         self.elev = elev
         self.ptype = ptype
         self.tags = set() if tags is None else tags
@@ -878,14 +878,15 @@
 
     def refresh(self):
         ''' Refresh a bunch of attributes. '''
         self.nrec = len(self.records)
         self.pids = [pobj.pid for pid, pobj in self.records.items()]
         self.lats = [pobj.lat for pid, pobj in self.records.items()]
         self.lons = [pobj.lon for pid, pobj in self.records.items()]
+        self.elevs = [pobj.elev for pid, pobj in self.records.items()]
         self.type_list = [pobj.ptype for pid, pobj in self.records.items()]
         self.type_dict = {}
         for t in self.type_list:
             if t not in self.type_dict:
                 self.type_dict[t] = 1
             else:
                 self.type_dict[t] += 1
@@ -994,14 +995,15 @@
             by (str): filter by a keyword {'ptype', 'pid', 'lat', 'lon', 'loc', 'tag'}
             keys (set): a set of keywords
 
                 * For `by = 'ptype' or 'pid'`, keys take a fuzzy match
                 * For `by = 'lat' or 'lon'`, keys = (lat_min, lat_max) or (lon_min, lon_max)
                 * For `by = 'loc-squre'`, keys = (lat_min, lat_max, lon_min, lon_max)
                 * For `by = 'loc-circle'`, keys = (center_lat, center_lon, distance)
+                * For `by = 'tag'`, keys should be a list of tags
 
             mode (str): 'fuzzy' or 'exact' search when `by = 'ptype' or 'pid'`
 
         '''
         if isinstance(keys, str): keys = [keys]
 
         new_db = ProxyDatabase()
@@ -1184,15 +1186,16 @@
                 df_proxy = ts_proxy.to_frame()
             else:
                 df_proxy = pd.merge(df_proxy, ts_proxy, left_index=True, right_index=True, how='outer')
 
             if obs is not None:
                 pobj.get_clim(obs, tag='obs')
                 pobj.clim[f'obs.{vn}'].center(ref_period=anom_period)
-                obs_time, obs_value, _ = utils.smooth_ts(pobj.clim[f'obs.{vn}'].time, pobj.clim[f'obs.{vn}'].da.values, bin_width=bin_width)
+                clim_time = utils.datetime2year_float(pobj.clim[f'obs.{vn}'].da.time.values)
+                obs_time, obs_value, _ = utils.smooth_ts(clim_time, pobj.clim[f'obs.{vn}'].da.values, bin_width=bin_width)
                 ts_obs = pd.Series(index=obs_time, data=obs_value, name=pid)
 
                 if 'df_obs' not in locals():
                     df_obs = ts_obs.to_frame()
                 else:
                     df_obs = pd.merge(df_obs, ts_obs, left_index=True, right_index=True, how='outer')
             else:
```

### Comparing `cfr-0.4.6/cfr/psm.py` & `cfr-0.5.0/cfr/psm.py`

 * *Files identical despite different names*

### Comparing `cfr-0.4.6/cfr/reconjob.py` & `cfr-0.5.0/cfr/reconjob.py`

 * *Files identical despite different names*

### Comparing `cfr-0.4.6/cfr/reconres.py` & `cfr-0.5.0/cfr/reconres.py`

 * *Files identical despite different names*

### Comparing `cfr-0.4.6/cfr/ts.py` & `cfr-0.5.0/cfr/ts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 from matplotlib.colors import LogNorm
 from scipy.stats import pearsonr
 import copy
+from . import utils
 from .utils import (
     coefficient_efficiency,
     p_header,
     p_hint,
     p_success,
     p_fail,
     p_warning,
@@ -32,14 +33,20 @@
         median (numpy.array): the median of the ensemble timeseries
 
     '''
     def __init__(self, time=None, value=None, value_name=None):
         if np.ndim(value) == 1:
             value = value[:, np.newaxis]
 
+        if time is not None:
+            try:
+                time = utils.datetime2year_float(time)
+            except:
+                pass
+
         self.time = time
         self.value = value
         self.value_name = value_name
 
         if self.value is not None:
             self.refresh()
```

### Comparing `cfr-0.4.6/cfr/utils.py` & `cfr-0.5.0/cfr/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,18 +194,18 @@
     ts = np.array(ts)
     ys = np.array(ys)
 
     return ts, ys
 
 
 def overlap_ts(ts_proxy, ys_proxy, ts_obs, ys_obs):
-    ys_proxy = np.array(ys_proxy, dtype=np.float)
-    ts_proxy = np.array(ts_proxy, dtype=np.float)
-    ys_obs = np.array(ys_obs, dtype=np.float)
-    ts_obs = np.array(ts_obs, dtype=np.float)
+    ys_proxy = np.array(ys_proxy, dtype=float)
+    ts_proxy = np.array(ts_proxy, dtype=float)
+    ys_obs = np.array(ys_obs, dtype=float)
+    ts_obs = np.array(ts_obs, dtype=float)
 
     overlap_proxy = (ts_proxy >= np.min(ts_obs)) & (ts_proxy <= np.max(ts_obs))
     overlap_obs = (ts_obs >= np.min(ts_proxy)) & (ts_obs <= np.max(ts_proxy))
 
     ys_proxy_overlap, ts_proxy_overlap = ys_proxy[overlap_proxy], ts_proxy[overlap_proxy]
     ys_obs_overlap, ts_obs_overlap = ys_obs[overlap_obs], ts_obs[overlap_obs]
 
@@ -214,18 +214,18 @@
     ind_obs = list(i for i, t in enumerate(ts_obs_overlap) if t in time_overlap)
     ys_proxy_overlap = ys_proxy_overlap[ind_proxy]
     ys_obs_overlap = ys_obs_overlap[ind_obs]
 
     return time_overlap, ys_proxy_overlap, ys_obs_overlap
 
 def ols_ts(ts_proxy, ys_proxy, ts_obs, ys_obs):
-    ys_proxy = np.asarray(ys_proxy, dtype=np.float)
-    ts_proxy = np.asarray(ts_proxy, dtype=np.float)
-    ys_obs = np.asarray(ys_obs, dtype=np.float)
-    ts_obs = np.asarray(ts_obs, dtype=np.float)
+    ys_proxy = np.array(ys_proxy, dtype=float)
+    ts_proxy = np.array(ts_proxy, dtype=float)
+    ys_obs = np.array(ys_obs, dtype=float)
+    ts_obs = np.array(ts_obs, dtype=float)
 
     time_overlap, ys_proxy_overlap, ys_obs_overlap = overlap_ts(ts_proxy, ys_proxy, ts_obs, ys_obs)
 
     # calculate the linear regression
     X = sm.add_constant(ys_proxy_overlap)
     ols_model = sm.OLS(ys_obs_overlap, X, missing='drop')
 
@@ -648,8 +648,22 @@
         sin_func = np.sin(2*np.pi*k*f0*t[j] + theta)
         y[j] = np.sum(coeff*sin_func)
 
     return y
 
 def is_numeric(obj):
     attrs = ['__add__', '__sub__', '__mul__', '__truediv__', '__pow__']
-    return all(hasattr(obj, attr) for attr in attrs)
+    return all(hasattr(obj, attr) for attr in attrs)
+
+def replace_str(fpath, d):
+    ''' Replace the string in a given text file according
+    to the dictionary `d`
+    '''
+    with open(fpath, 'r') as f:
+        text = f.read()
+        for k, v in d.items():
+            search_text = k
+            replace_text = v
+            text = text.replace(search_text, replace_text)
+
+    with open(fpath, 'w') as f:
+        f.write(text)
```

### Comparing `cfr-0.4.6/cfr/visual.py` & `cfr-0.5.0/cfr/visual.py`

 * *Files identical despite different names*

### Comparing `cfr-0.4.6/cfr.egg-info/PKG-INFO` & `cfr-0.5.0/cfr.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfr
-Version: 0.4.6
+Version: 0.5.0
 Summary: cfr: the Python package for Climate Field Reconstruction
 Home-page: https://github.com/fzhu2e/cfr
 Author: Feng Zhu, Julien Emile-Geay
 Author-email: fengzhu@ucar.edu, julieneg@usc.edu
 License: BSD 3-Clause
 Keywords: paleocliamte reconstruction
 Classifier: Natural Language :: English
@@ -12,26 +12,29 @@
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/x-rst
 Provides-Extra: psm
 Provides-Extra: ml
 Provides-Extra: graphem
 License-File: LICENSE
 
-***********************************************************
-`cfr`: a Python package for Climate Field Reconstruction
-***********************************************************
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7855587.svg)](https://doi.org/10.5281/zenodo.7855587)
+
+# `cfr`: a Python package for Climate Field Reconstruction
 
 `cfr` aims to provide a universal framework for climate field reconstruction (CFR).
 It provides a toolkit for
 
 + the processing and visualization of the proxy records, climate model simulations, and instrumental observations,
-+ the calibration and running of the proxy system models (PSMs, `Evans et al., 2013 <https://doi.org/10.1016/j.quascirev.2013.05.024>`_),
-+ the preparation and running of the multiple reconstruction frameworks/algorithms, such as LMR (`Hakim et al., 2016 <https://doi.org/10.1002/2016JD024751>`_; `Tardif et al., 2019 <https://doi.org/https://doi.org/10.5194/cp-15-1251-2019>`_) and GraphEM (`Guillot et al., 2015 <https://doi.org/10.1214/14-AOAS794>`_), and
++ the calibration and running of the proxy system models (PSMs, [Evans et al., 2013](https://doi.org/10.1016/j.quascirev.2013.05.024)),
++ the preparation and running of the multiple reconstruction frameworks/algorithms, such as LMR ([Hakim et al., 2016](https://doi.org/10.1002/2016JD024751); [Tardif et al., 2019](https://doi.org/https://doi.org/10.5194/cp-15-1251-2019)) and GraphEM ([Guillot et al., 2015](https://doi.org/10.1214/14-AOAS794)), and
 + the validation of the reconstructions, etc.
 
 For more details, please refer to the documentation linked below.
 
-Documentation
-=============
+## Documentation
 
 + Homepage: https://fzhu2e.github.io/cfr
 + Installation: https://fzhu2e.github.io/cfr/ug-installation.html
+
+## How to cite this repo
+
+This repo can be cited with DOI: [10.5281/zenodo.7855587](https://doi.org/10.5281/zenodo.7855587)
```

### Comparing `cfr-0.4.6/setup.py` & `cfr-0.5.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
-with open('README.rst', 'r') as fh:
+with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='cfr',  # required
-    version='0.4.6',
+    version='0.5.0',
     description='cfr: the Python package for Climate Field Reconstruction',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     author='Feng Zhu, Julien Emile-Geay',
     author_email='fengzhu@ucar.edu, julieneg@usc.edu',
     url='https://github.com/fzhu2e/cfr',
     packages=find_packages(),
```

