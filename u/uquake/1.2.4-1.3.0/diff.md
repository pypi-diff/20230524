# Comparing `tmp/uquake-1.2.4.tar.gz` & `tmp/uquake-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uquake-1.2.4.tar", max compression
+gzip compressed data, was "uquake-1.3.0.tar", max compression
```

## Comparing `uquake-1.2.4.tar` & `uquake-1.3.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     2345 2023-01-30 13:40:20.174805 uquake-1.2.4/pyproject.toml
--rw-r--r--   0        0        0      158 2023-01-25 01:11:29.666160 uquake-1.2.4/uquake/__init__.py
--rw-r--r--   0        0        0      191 2023-01-15 00:23:22.715786 uquake-1.2.4/uquake/core/__init__.py
--rw-r--r--   0        0        0      658 2023-01-15 00:23:22.715786 uquake-1.2.4/uquake/core/decorators.py
--rw-r--r--   0        0        0    31807 2023-04-17 12:59:33.326538 uquake-1.2.4/uquake/core/event.py
--rw-r--r--   0        0        0     6233 2023-01-15 00:23:22.715786 uquake-1.2.4/uquake/core/focal_mechanism.py
--rw-r--r--   0        0        0    38774 2023-04-16 18:22:31.094780 uquake-1.2.4/uquake/core/inventory.py
--rw-r--r--   0        0        0      239 2023-01-15 00:23:22.715786 uquake-1.2.4/uquake/core/logging.py
--rw-r--r--   0        0        0    13782 2023-01-25 01:08:23.561456 uquake-1.2.4/uquake/core/stream.py
--rw-r--r--   0        0        0     5308 2023-01-15 00:23:22.715786 uquake-1.2.4/uquake/core/trace.py
--rw-r--r--   0        0        0       67 2023-01-15 00:23:22.715786 uquake-1.2.4/uquake/core/util/__init__.py
--rw-r--r--   0        0        0     4206 2023-01-15 00:23:22.715786 uquake-1.2.4/uquake/core/util/base.py
--rw-r--r--   0        0        0     5713 2023-01-15 00:23:22.715786 uquake-1.2.4/uquake/core/util/decorator.py
--rw-r--r--   0        0        0      620 2023-04-16 18:19:34.782672 uquake-1.2.4/uquake/core/util/requests.py
--rw-r--r--   0        0        0    13768 2023-01-15 00:23:22.715786 uquake-1.2.4/uquake/core/util/tools.py
--rw-r--r--   0        0        0       28 2023-01-15 00:23:22.715786 uquake-1.2.4/uquake/grid/__init__.py
--rw-r--r--   0        0        0    22963 2023-04-13 23:59:04.661740 uquake-1.2.4/uquake/grid/base.py
--rw-r--r--   0        0        0     4658 2023-01-15 00:23:22.715786 uquake-1.2.4/uquake/grid/hdf5.py
--rw-r--r--   0        0        0    47247 2023-04-14 00:12:47.864202 uquake-1.2.4/uquake/grid/nlloc.py
--rw-r--r--   0        0        0        0 2023-01-15 00:23:22.715786 uquake-1.2.4/uquake/imaging/__init__.py
--rw-r--r--   0        0        0    10043 2023-03-08 09:37:25.089762 uquake-1.2.4/uquake/imaging/plot.py
--rw-r--r--   0        0        0     2474 2023-01-15 00:23:22.715786 uquake-1.2.4/uquake/imaging/stereonet.py
--rw-r--r--   0        0        0    59743 2023-01-15 00:23:22.719786 uquake-1.2.4/uquake/imaging/waveform.py
--rw-r--r--   0        0        0      423 2023-01-15 00:23:22.719786 uquake-1.2.4/uquake/io/__init__.py
--rw-r--r--   0        0        0        0 2023-01-15 00:23:22.719786 uquake-1.2.4/uquake/io/event/__init__.py
--rw-r--r--   0        0        0     3417 2023-01-15 00:23:22.719786 uquake-1.2.4/uquake/io/event/core.py
--rw-r--r--   0        0        0       20 2023-01-15 00:23:22.719786 uquake-1.2.4/uquake/io/grid/__init__.py
--rw-r--r--   0        0        0     8496 2023-01-15 00:23:22.719786 uquake-1.2.4/uquake/io/grid/core.py
--rw-r--r--   0        0        0       21 2023-01-15 00:23:22.719786 uquake-1.2.4/uquake/io/inventory/__init__.py
--rw-r--r--   0        0        0     6531 2023-01-15 00:23:22.719786 uquake-1.2.4/uquake/io/inventory/core.py
--rw-r--r--   0        0        0       20 2023-01-15 00:23:22.719786 uquake-1.2.4/uquake/io/waveform/__init__.py
--rw-r--r--   0        0        0     9262 2023-01-15 00:23:22.719786 uquake-1.2.4/uquake/io/waveform/core.py
--rw-r--r--   0        0        0       21 2023-01-15 00:23:22.719786 uquake-1.2.4/uquake/nlloc/__init__.py
--rw-r--r--   0        0        0    48293 2023-01-15 00:23:22.719786 uquake-1.2.4/uquake/nlloc/nlloc.py
--rw-r--r--   0        0        0        0 2023-01-15 00:23:22.719786 uquake-1.2.4/uquake/waveform/__init__.py
--rw-r--r--   0        0        0    34528 2023-01-15 00:23:22.719786 uquake-1.2.4/uquake/waveform/amp_measures.py
--rw-r--r--   0        0        0    15799 2023-01-15 00:23:22.719786 uquake-1.2.4/uquake/waveform/mag.py
--rw-r--r--   0        0        0     5354 2023-01-15 00:23:22.719786 uquake-1.2.4/uquake/waveform/mag_utils.py
--rw-r--r--   0        0        0     2827 2023-01-15 00:23:22.719786 uquake-1.2.4/uquake/waveform/parseval_utils.py
--rw-r--r--   0        0        0    23179 2023-01-15 00:23:22.719786 uquake-1.2.4/uquake/waveform/pick.py
--rw-r--r--   0        0        0    45461 2023-04-04 17:02:48.691928 uquake-1.2.4/uquake/waveform/simple_mag.py
--rw-r--r--   0        0        0    32225 2023-01-15 00:23:22.719786 uquake-1.2.4/uquake/waveform/smom_measure.py
--rw-r--r--   0        0        0    33065 2023-01-15 00:23:22.719786 uquake-1.2.4/uquake/waveform/smom_measure_legacy.py
--rw-r--r--   0        0        0     4456 2023-01-15 00:23:22.719786 uquake-1.2.4/uquake/waveform/transforms.py
--rw-r--r--   0        0        0     2849 1970-01-01 00:00:00.000000 uquake-1.2.4/setup.py
--rw-r--r--   0        0        0     1054 1970-01-01 00:00:00.000000 uquake-1.2.4/PKG-INFO
+-rw-r--r--   0        0        0     2399 2023-05-24 00:23:29.689902 uquake-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      158 2023-01-25 01:11:29.666160 uquake-1.3.0/uquake/__init__.py
+-rw-r--r--   0        0        0      191 2023-01-15 00:23:22.715786 uquake-1.3.0/uquake/core/__init__.py
+-rw-r--r--   0        0        0      658 2023-01-15 00:23:22.715786 uquake-1.3.0/uquake/core/decorators.py
+-rw-r--r--   0        0        0    31807 2023-04-17 12:59:33.326538 uquake-1.3.0/uquake/core/event.py
+-rw-r--r--   0        0        0     6233 2023-01-15 00:23:22.715786 uquake-1.3.0/uquake/core/focal_mechanism.py
+-rw-r--r--   0        0        0    38774 2023-04-16 18:22:31.094780 uquake-1.3.0/uquake/core/inventory.py
+-rw-r--r--   0        0        0      239 2023-01-15 00:23:22.715786 uquake-1.3.0/uquake/core/logging.py
+-rw-r--r--   0        0        0    13782 2023-01-25 01:08:23.561456 uquake-1.3.0/uquake/core/stream.py
+-rw-r--r--   0        0        0     5308 2023-01-15 00:23:22.715786 uquake-1.3.0/uquake/core/trace.py
+-rw-r--r--   0        0        0       67 2023-01-15 00:23:22.715786 uquake-1.3.0/uquake/core/util/__init__.py
+-rw-r--r--   0        0        0     4206 2023-01-15 00:23:22.715786 uquake-1.3.0/uquake/core/util/base.py
+-rw-r--r--   0        0        0     5713 2023-01-15 00:23:22.715786 uquake-1.3.0/uquake/core/util/decorator.py
+-rw-r--r--   0        0        0      620 2023-04-16 18:19:34.782672 uquake-1.3.0/uquake/core/util/requests.py
+-rw-r--r--   0        0        0    13768 2023-01-15 00:23:22.715786 uquake-1.3.0/uquake/core/util/tools.py
+-rw-r--r--   0        0        0       28 2023-01-15 00:23:22.715786 uquake-1.3.0/uquake/grid/__init__.py
+-rw-r--r--   0        0        0    22173 2023-04-27 00:23:45.744173 uquake-1.3.0/uquake/grid/base.py
+-rw-r--r--   0        0        0     4660 2023-05-06 10:03:22.429231 uquake-1.3.0/uquake/grid/hdf5.py
+-rw-r--r--   0        0        0    47247 2023-04-27 00:26:03.338550 uquake-1.3.0/uquake/grid/nlloc.py
+-rw-r--r--   0        0        0        0 2023-01-15 00:23:22.715786 uquake-1.3.0/uquake/imaging/__init__.py
+-rw-r--r--   0        0        0    10043 2023-03-08 09:37:25.089762 uquake-1.3.0/uquake/imaging/plot.py
+-rw-r--r--   0        0        0     2474 2023-01-15 00:23:22.715786 uquake-1.3.0/uquake/imaging/stereonet.py
+-rw-r--r--   0        0        0    59743 2023-01-15 00:23:22.719786 uquake-1.3.0/uquake/imaging/waveform.py
+-rw-r--r--   0        0        0      423 2023-01-15 00:23:22.719786 uquake-1.3.0/uquake/io/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-15 00:23:22.719786 uquake-1.3.0/uquake/io/event/__init__.py
+-rw-r--r--   0        0        0     3417 2023-01-15 00:23:22.719786 uquake-1.3.0/uquake/io/event/core.py
+-rw-r--r--   0        0        0       20 2023-01-15 00:23:22.719786 uquake-1.3.0/uquake/io/grid/__init__.py
+-rw-r--r--   0        0        0     8496 2023-01-15 00:23:22.719786 uquake-1.3.0/uquake/io/grid/core.py
+-rw-r--r--   0        0        0       21 2023-01-15 00:23:22.719786 uquake-1.3.0/uquake/io/inventory/__init__.py
+-rw-r--r--   0        0        0     6531 2023-01-15 00:23:22.719786 uquake-1.3.0/uquake/io/inventory/core.py
+-rw-r--r--   0        0        0       20 2023-01-15 00:23:22.719786 uquake-1.3.0/uquake/io/waveform/__init__.py
+-rw-r--r--   0        0        0     9262 2023-01-15 00:23:22.719786 uquake-1.3.0/uquake/io/waveform/core.py
+-rw-r--r--   0        0        0       21 2023-01-15 00:23:22.719786 uquake-1.3.0/uquake/nlloc/__init__.py
+-rw-r--r--   0        0        0    48293 2023-01-15 00:23:22.719786 uquake-1.3.0/uquake/nlloc/nlloc.py
+-rw-r--r--   0        0        0        0 2023-01-15 00:23:22.719786 uquake-1.3.0/uquake/waveform/__init__.py
+-rw-r--r--   0        0        0    34528 2023-01-15 00:23:22.719786 uquake-1.3.0/uquake/waveform/amp_measures.py
+-rw-r--r--   0        0        0    15799 2023-01-15 00:23:22.719786 uquake-1.3.0/uquake/waveform/mag.py
+-rw-r--r--   0        0        0     5354 2023-01-15 00:23:22.719786 uquake-1.3.0/uquake/waveform/mag_utils.py
+-rw-r--r--   0        0        0     2827 2023-01-15 00:23:22.719786 uquake-1.3.0/uquake/waveform/parseval_utils.py
+-rw-r--r--   0        0        0    21331 2023-05-16 01:15:39.357070 uquake-1.3.0/uquake/waveform/pick.py
+-rw-r--r--   0        0        0    45461 2023-04-04 17:02:48.691928 uquake-1.3.0/uquake/waveform/simple_mag.py
+-rw-r--r--   0        0        0    32225 2023-01-15 00:23:22.719786 uquake-1.3.0/uquake/waveform/smom_measure.py
+-rw-r--r--   0        0        0    33065 2023-01-15 00:23:22.719786 uquake-1.3.0/uquake/waveform/smom_measure_legacy.py
+-rw-r--r--   0        0        0     4456 2023-01-15 00:23:22.719786 uquake-1.3.0/uquake/waveform/transforms.py
+-rw-r--r--   0        0        0     2919 1970-01-01 00:00:00.000000 uquake-1.3.0/setup.py
+-rw-r--r--   0        0        0     1152 1970-01-01 00:00:00.000000 uquake-1.3.0/PKG-INFO
```

### Comparing `uquake-1.2.4/pyproject.toml` & `uquake-1.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 [tool.poetry]
 name = "uquake"
-version = "1.2.4"
+version = "1.3.0"
 description = "extension of the ObsPy library for local seismicity"
 authors = ["uQuake development team <dev@uQuake.org>"]
 license = "MIT"
 
 # poetry config virtualenvs.create false; poetry env info
 
 [tool.poetry.dependencies]
 python = "^3.9"
 numpy = "^1.18.0"
 loguru = "^0.5.3"
 pandas = "^1.2.1"
 jedi = "0.17.2"
-pytest = "^6.2.1"
 openpyxl = "^3.0.6"
 obspy = "^1.2.2"
 vtk = "^9.0.1"
 dynaconf = "^3.1.4"
 h5py = "^3.2.1"
 pydantic = "^1.8.2"
 pyproj = "^3.2.1"
 tqdm = "^4.62.3"
 scikit-fmm = "^2022.3.26"
 future = "^0.18.2"
+pytest = "^7.3.1"
+pytest-asyncio = "^0.21.0"
+pyproject-toml = "^0.0.10"
 
 [tool.poetry.dev-dependencies]
 ipdb = "^0.13.9"
 ipython = "^8.1.0"
 
 [tool.poetry.plugins] # Optional super table
```

### Comparing `uquake-1.2.4/uquake/core/decorators.py` & `uquake-1.3.0/uquake/core/decorators.py`

 * *Files identical despite different names*

### Comparing `uquake-1.2.4/uquake/core/event.py` & `uquake-1.3.0/uquake/core/event.py`

 * *Files identical despite different names*

### Comparing `uquake-1.2.4/uquake/core/focal_mechanism.py` & `uquake-1.3.0/uquake/core/focal_mechanism.py`

 * *Files identical despite different names*

### Comparing `uquake-1.2.4/uquake/core/inventory.py` & `uquake-1.3.0/uquake/core/inventory.py`

 * *Files identical despite different names*

### Comparing `uquake-1.2.4/uquake/core/stream.py` & `uquake-1.3.0/uquake/core/stream.py`

 * *Files identical despite different names*

### Comparing `uquake-1.2.4/uquake/core/trace.py` & `uquake-1.3.0/uquake/core/trace.py`

 * *Files identical despite different names*

### Comparing `uquake-1.2.4/uquake/core/util/base.py` & `uquake-1.3.0/uquake/core/util/base.py`

 * *Files identical despite different names*

### Comparing `uquake-1.2.4/uquake/core/util/decorator.py` & `uquake-1.3.0/uquake/core/util/decorator.py`

 * *Files identical despite different names*

### Comparing `uquake-1.2.4/uquake/core/util/requests.py` & `uquake-1.3.0/uquake/core/util/requests.py`

 * *Files identical despite different names*

### Comparing `uquake-1.2.4/uquake/core/util/tools.py` & `uquake-1.3.0/uquake/core/util/tools.py`

 * *Files identical despite different names*

### Comparing `uquake-1.2.4/uquake/grid/base.py` & `uquake-1.3.0/uquake/grid/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -369,35 +369,14 @@
             points[i] = points[i] * self.dimensions
 
         if not grid_space:
             return self.transform_from_grid(points)
 
         return points
 
-    def write(self, filename, format='PICKLE', **kwargs):
-        """
-        write the grid to disk
-        :param filename: full path to the file to be written
-        :type filename: str
-        :param format: output file format
-        :type format: str
-        """
-        format = format.upper()
-        if format not in ENTRY_POINTS['grid'].keys():
-            logger.error('format %s is not currently supported for Grid '
-                         'objects' % format)
-            return
-
-        format_ep = ENTRY_POINTS['grid'][format]
-        write_format = load_entry_point(format_ep.dist.key,
-                                        'uquake.plugin.grid.%s'
-                                        % format_ep.name, 'writeFormat')
-
-        write_format(self, filename, **kwargs)
-
     def interpolate(self, coord, grid_space=True, mode='nearest',
                     order=1, **kwargs):
         """
         This function interpolate the values at a given point expressed
         either in grid or absolute coordinates
         :param coord: Coordinate of the point(s) at which to interpolate
         either in grid or absolute coordinates
```

### Comparing `uquake-1.2.4/uquake/grid/hdf5.py` & `uquake-1.3.0/uquake/grid/hdf5.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 from glob import glob
 import numpy as np
 import h5py
 
+
 class H5TTable(object):
     """docstring for H5TTable"""
 
     def __init__(self, path, dset_key=None):
         self.path = path
         self.hf = h5py.File(path, 'r')
         self.keys = list(self.hf.keys())
@@ -84,14 +85,15 @@
         for yv in y:
             for zv in z:
                 points[ix] = [xv, yv, zv]
                 ix += 1
 
     return points
 
+
 def array_from_travel_time_ensemble(tt_grids):
 
     data = {'P': [],
             'S': []}
 
     sites = []
     slocs = []
```

### Comparing `uquake-1.2.4/uquake/grid/nlloc.py` & `uquake-1.3.0/uquake/grid/nlloc.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -914,22 +914,22 @@
 
         else:
             tt_grid_ensemble = TravelTimeEnsemble([])
             for key in self.keys():
                 for seed, seed_labels in zip(seeds, seed_labels):
                     tt_grid_ensemble += self[key].to_time(seed, seed_label)
 
-
     @property
     def p(self):
         return self['p']
 
     def s(self):
         return self['s']
 
+
 class SeededGrid(NLLocGrid):
     """
     container for seeded grids (e.g., travel time, azimuth and take off angle)
     """
     __valid_grid_type__ = ['TIME', 'TIME2D', 'ANGLE', 'ANGLE2D']
 
     def __init__(self, network_code, data_or_dims, origin, spacing, seed,
```

### Comparing `uquake-1.2.4/uquake/imaging/plot.py` & `uquake-1.3.0/uquake/imaging/plot.py`

 * *Files identical despite different names*

### Comparing `uquake-1.2.4/uquake/imaging/stereonet.py` & `uquake-1.3.0/uquake/imaging/stereonet.py`

 * *Files identical despite different names*

### Comparing `uquake-1.2.4/uquake/imaging/waveform.py` & `uquake-1.3.0/uquake/imaging/waveform.py`

 * *Files identical despite different names*

### Comparing `uquake-1.2.4/uquake/io/event/core.py` & `uquake-1.3.0/uquake/io/event/core.py`

 * *Files identical despite different names*

### Comparing `uquake-1.2.4/uquake/io/grid/core.py` & `uquake-1.3.0/uquake/io/grid/core.py`

 * *Files identical despite different names*

### Comparing `uquake-1.2.4/uquake/io/inventory/core.py` & `uquake-1.3.0/uquake/io/inventory/core.py`

 * *Files identical despite different names*

### Comparing `uquake-1.2.4/uquake/io/waveform/core.py` & `uquake-1.3.0/uquake/io/waveform/core.py`

 * *Files identical despite different names*

### Comparing `uquake-1.2.4/uquake/nlloc/nlloc.py` & `uquake-1.3.0/uquake/nlloc/nlloc.py`

 * *Files identical despite different names*

### Comparing `uquake-1.2.4/uquake/waveform/amp_measures.py` & `uquake-1.3.0/uquake/waveform/amp_measures.py`

 * *Files identical despite different names*

### Comparing `uquake-1.2.4/uquake/waveform/mag.py` & `uquake-1.3.0/uquake/waveform/mag.py`

 * *Files identical despite different names*

### Comparing `uquake-1.2.4/uquake/waveform/mag_utils.py` & `uquake-1.3.0/uquake/waveform/mag_utils.py`

 * *Files identical despite different names*

### Comparing `uquake-1.2.4/uquake/waveform/parseval_utils.py` & `uquake-1.3.0/uquake/waveform/parseval_utils.py`

 * *Files identical despite different names*

### Comparing `uquake-1.2.4/uquake/waveform/pick.py` & `uquake-1.3.0/uquake/waveform/pick.py`

 * *Files 9% similar despite different names*

```diff
@@ -268,54 +268,14 @@
                                  method_string=method_string,
                                  resource_id=pick.resource_id))
         snrs.append(snr)
 
     return snrs, o_picks
 
 
-def linearity_ensemble_re_picker(st, picks, start_search_window,
-                                 end_search_window,
-                                 start_refined_search_window,
-                                 end_refinde_search_window,
-                                 refined_window_search_resolution,
-                                 linearity_calc_window_len):
-    """
-        Function to improve the picks based on the linearity or planarity
-        for an ensemble of traces.
-        :param st: waveforms containing a seismic event
-        :type st: :py:class:`uquake.core.stream.Stream`
-        :param picks: list of :class:`uquake.core.event.Pick` object
-        picks
-        :type picks: list of :py:class:`uquake.core.event.Pick`
-        :param start_search_window: start of the search window relative to
-        provided picks in seconds
-        :type start_search_window: float
-        :param end_search_window: end of the search window relative to the
-        provided picks in seconds
-        :param start_refined_search_window: start of the refined search
-        window in seconds
-        :type: float
-        :param end_refined_search_window: end of the refined search window in
-        seconds
-        :type: float
-        :type end_search_window: float
-        :param refined_window_search_resolution: resolution of the search
-        space in seconds
-        :type refined_window_search_resolution: float
-        :param linearity_calc_window_len: length of the window after the
-        presumed pick used to calculate the linearity
-        :param trace_padding: buffer from trace start and end time excluded
-        from search window
-        :returns:  Tuple comprising 1) a :py:class:`uquake.core.event.Catalog`
-        a new catalog containing a single event with a list of picks and 2)
-        the SNR
-        """
-
-
-
 def snr_ensemble_re_picker(st, picks, start_search_window, end_search_window,
                            start_refined_search_window,
                            end_refined_search_window,
                            refined_window_search_resolution,
                            snr_calc_pre_pick_window_len=1e-3,
                            snr_calc_post_pick_window_len=20e-3,
                            trace_padding=30e-3):
@@ -484,32 +444,28 @@
                                         window_length_sample
         waveforms.append(tr.data[start_measurement_window_sample:
                                  end_measurement_window_sample])
 
     return np.array(waveforms)
 
 
-
 def measure_linearity(st: Stream, pick_time: UTCDateTime,
                       window_length: float):
     """
     measure the linearity of the particule motion using PCA
     :param st: waveforms recorded by a particular site
     :type st: :py:class:`uquake.core.stream.Stream`
     :param pick_time: pick time
     :type pick_time: :py:class:uquake.core.UTCDateTime
     :param window_length: length of the window in seconds over which the
     linearity is measured
     :return: the linearity between 0 and 1. 1 representing a perfect linearity
     :rtype: float
     """
 
-
-
-
     pass
 
 
 def measure_planarity():
     """
     measure the planarity of the particule motion using PCA
     :param st: waveforms recorded by a particular site
```

### Comparing `uquake-1.2.4/uquake/waveform/simple_mag.py` & `uquake-1.3.0/uquake/waveform/simple_mag.py`

 * *Files identical despite different names*

### Comparing `uquake-1.2.4/uquake/waveform/smom_measure.py` & `uquake-1.3.0/uquake/waveform/smom_measure.py`

 * *Files identical despite different names*

### Comparing `uquake-1.2.4/uquake/waveform/smom_measure_legacy.py` & `uquake-1.3.0/uquake/waveform/smom_measure_legacy.py`

 * *Files identical despite different names*

### Comparing `uquake-1.2.4/uquake/waveform/transforms.py` & `uquake-1.3.0/uquake/waveform/transforms.py`

 * *Files identical despite different names*

### Comparing `uquake-1.2.4/setup.py` & `uquake-1.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,17 @@
  'loguru>=0.5.3,<0.6.0',
  'numpy>=1.18.0,<2.0.0',
  'obspy>=1.2.2,<2.0.0',
  'openpyxl>=3.0.6,<4.0.0',
  'pandas>=1.2.1,<2.0.0',
  'pydantic>=1.8.2,<2.0.0',
  'pyproj>=3.2.1,<4.0.0',
- 'pytest>=6.2.1,<7.0.0',
+ 'pyproject-toml>=0.0.10,<0.0.11',
+ 'pytest-asyncio>=0.21.0,<0.22.0',
+ 'pytest>=7.3.1,<8.0.0',
  'scikit-fmm>=2022.3.26,<2023.0.0',
  'tqdm>=4.62.3,<5.0.0',
  'vtk>=9.0.1,<10.0.0']
 
 entry_points = \
 {'uquake.io.event': ['NLLOC = uquake.io.nlloc', 'QUAKEML = uquake.io.quakeml'],
  'uquake.io.grid': ['CSV = uquake.io.grid',
@@ -61,15 +63,15 @@
  'uquake.io.waveform.IMS_ASCII': ['readFormat = '
                                   'uquake.io.waveform:read_IMS_ASCII'],
  'uquake.io.waveform.TEXCEL_CSV': ['readFormat = '
                                    'uquake.io.waveform:read_TEXCEL_CSV']}
 
 setup_kwargs = {
     'name': 'uquake',
-    'version': '1.2.4',
+    'version': '1.3.0',
     'description': 'extension of the ObsPy library for local seismicity',
     'long_description': 'None',
     'author': 'uQuake development team',
     'author_email': 'dev@uQuake.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `uquake-1.2.4/PKG-INFO` & `uquake-1.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uquake
-Version: 1.2.4
+Version: 1.3.0
 Summary: extension of the ObsPy library for local seismicity
 License: MIT
 Author: uQuake development team
 Author-email: dev@uQuake.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -18,11 +18,13 @@
 Requires-Dist: loguru (>=0.5.3,<0.6.0)
 Requires-Dist: numpy (>=1.18.0,<2.0.0)
 Requires-Dist: obspy (>=1.2.2,<2.0.0)
 Requires-Dist: openpyxl (>=3.0.6,<4.0.0)
 Requires-Dist: pandas (>=1.2.1,<2.0.0)
 Requires-Dist: pydantic (>=1.8.2,<2.0.0)
 Requires-Dist: pyproj (>=3.2.1,<4.0.0)
-Requires-Dist: pytest (>=6.2.1,<7.0.0)
+Requires-Dist: pyproject-toml (>=0.0.10,<0.0.11)
+Requires-Dist: pytest (>=7.3.1,<8.0.0)
+Requires-Dist: pytest-asyncio (>=0.21.0,<0.22.0)
 Requires-Dist: scikit-fmm (>=2022.3.26,<2023.0.0)
 Requires-Dist: tqdm (>=4.62.3,<5.0.0)
 Requires-Dist: vtk (>=9.0.1,<10.0.0)
```

