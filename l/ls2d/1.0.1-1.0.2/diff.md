# Comparing `tmp/ls2d-1.0.1.tar.gz` & `tmp/ls2d-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ls2d-1.0.1.tar", last modified: Mon May  1 11:47:16 2023, max compression
+gzip compressed data, was "ls2d-1.0.2.tar", last modified: Wed May 24 12:13:37 2023, max compression
```

## Comparing `ls2d-1.0.1.tar` & `ls2d-1.0.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-01 11:47:16.795487 ls2d-1.0.1/
--rw-r--r--   0 bart      (1000) bart      (1000)    35147 2021-05-26 07:47:37.000000 ls2d-1.0.1/LICENSE.txt
--rw-r--r--   0 bart      (1000) bart      (1000)      153 2023-04-04 10:39:10.000000 ls2d-1.0.1/MANIFEST.in
--rw-r--r--   0 bart      (1000) bart      (1000)    44246 2023-05-01 11:47:16.795487 ls2d-1.0.1/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)     3044 2023-04-04 11:24:03.000000 ls2d-1.0.1/README.md
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-01 11:47:16.792154 ls2d-1.0.1/examples/
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-01 11:47:16.792154 ls2d-1.0.1/examples/microhh/
--rw-r--r--   0 bart      (1000) bart      (1000)     1823 2021-05-26 07:47:37.000000 ls2d-1.0.1/examples/microhh/cabauw.ini.base
--rwxr-xr-x   0 bart      (1000) bart      (1000)      577 2023-04-04 09:43:40.000000 ls2d-1.0.1/examples/microhh/link_lookup_tables.sh
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-01 11:47:16.792154 ls2d-1.0.1/ls2d/
--rw-r--r--   0 bart      (1000) bart      (1000)     1083 2023-04-01 13:15:27.000000 ls2d-1.0.1/ls2d/__init__.py
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-01 11:47:16.792154 ls2d-1.0.1/ls2d/ecmwf/
--rw-r--r--   0 bart      (1000) bart      (1000)     7644 2023-04-01 13:15:27.000000 ls2d-1.0.1/ls2d/ecmwf/IFS_tools.py
--rw-r--r--   0 bart      (1000) bart      (1000)    11723 2021-05-03 14:13:15.000000 ls2d-1.0.1/ls2d/ecmwf/L137_grid.txt
--rw-r--r--   0 bart      (1000) bart      (1000)     5300 2021-09-16 10:54:45.000000 ls2d-1.0.1/ls2d/ecmwf/L60_grid.txt
--rw-r--r--   0 bart      (1000) bart      (1000)      814 2023-04-01 13:15:27.000000 ls2d-1.0.1/ls2d/ecmwf/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1000)    16446 2023-04-01 13:15:27.000000 ls2d-1.0.1/ls2d/ecmwf/download_era5.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2846 2023-04-01 13:15:27.000000 ls2d-1.0.1/ls2d/ecmwf/era_tools.py
--rw-r--r--   0 bart      (1000) bart      (1000)    30347 2023-05-01 09:45:03.000000 ls2d-1.0.1/ls2d/ecmwf/read_era5.py
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-01 11:47:16.795487 ls2d-1.0.1/ls2d/src/
--rw-r--r--   0 bart      (1000) bart      (1000)        0 2023-04-01 13:15:27.000000 ls2d-1.0.1/ls2d/src/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1603 2023-04-01 13:15:27.000000 ls2d-1.0.1/ls2d/src/finite_difference.py
--rw-r--r--   0 bart      (1000) bart      (1000)     4108 2023-04-01 13:15:27.000000 ls2d-1.0.1/ls2d/src/grid.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1822 2023-04-01 13:15:27.000000 ls2d-1.0.1/ls2d/src/messages.py
--rw-r--r--   0 bart      (1000) bart      (1000)     7512 2023-04-01 13:15:27.000000 ls2d-1.0.1/ls2d/src/slurm.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2672 2023-04-01 13:15:27.000000 ls2d-1.0.1/ls2d/src/spatial_tools.py
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-01 11:47:16.792154 ls2d-1.0.1/ls2d.egg-info/
--rw-r--r--   0 bart      (1000) bart      (1000)    44246 2023-05-01 11:47:16.000000 ls2d-1.0.1/ls2d.egg-info/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)      581 2023-05-01 11:47:16.000000 ls2d-1.0.1/ls2d.egg-info/SOURCES.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        1 2023-05-01 11:47:16.000000 ls2d-1.0.1/ls2d.egg-info/dependency_links.txt
--rw-r--r--   0 bart      (1000) bart      (1000)       61 2023-05-01 11:47:16.000000 ls2d-1.0.1/ls2d.egg-info/requires.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        5 2023-05-01 11:47:16.000000 ls2d-1.0.1/ls2d.egg-info/top_level.txt
--rw-r--r--   0 bart      (1000) bart      (1000)      990 2023-05-01 11:46:30.000000 ls2d-1.0.1/pyproject.toml
--rw-r--r--   0 bart      (1000) bart      (1000)       38 2023-05-01 11:47:16.795487 ls2d-1.0.1/setup.cfg
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-24 12:13:37.299243 ls2d-1.0.2/
+-rw-r--r--   0 bart      (1000) bart      (1000)    35147 2021-05-26 07:47:37.000000 ls2d-1.0.2/LICENSE.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)      153 2023-04-04 10:39:10.000000 ls2d-1.0.2/MANIFEST.in
+-rw-r--r--   0 bart      (1000) bart      (1000)    44246 2023-05-24 12:13:37.299243 ls2d-1.0.2/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)     3044 2023-04-04 11:24:03.000000 ls2d-1.0.2/README.md
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-24 12:13:37.295910 ls2d-1.0.2/examples/
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-24 12:13:37.295910 ls2d-1.0.2/examples/microhh/
+-rw-r--r--   0 bart      (1000) bart      (1000)     1823 2021-05-26 07:47:37.000000 ls2d-1.0.2/examples/microhh/cabauw.ini.base
+-rwxr-xr-x   0 bart      (1000) bart      (1000)      577 2023-04-04 09:43:40.000000 ls2d-1.0.2/examples/microhh/link_lookup_tables.sh
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-24 12:13:37.295910 ls2d-1.0.2/ls2d/
+-rw-r--r--   0 bart      (1000) bart      (1000)     1083 2023-04-01 13:15:27.000000 ls2d-1.0.2/ls2d/__init__.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-24 12:13:37.299243 ls2d-1.0.2/ls2d/ecmwf/
+-rw-r--r--   0 bart      (1000) bart      (1000)     7644 2023-04-01 13:15:27.000000 ls2d-1.0.2/ls2d/ecmwf/IFS_tools.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    11723 2021-05-03 14:13:15.000000 ls2d-1.0.2/ls2d/ecmwf/L137_grid.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)     5300 2021-09-16 10:54:45.000000 ls2d-1.0.2/ls2d/ecmwf/L60_grid.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)      814 2023-04-01 13:15:27.000000 ls2d-1.0.2/ls2d/ecmwf/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    16446 2023-04-01 13:15:27.000000 ls2d-1.0.2/ls2d/ecmwf/download_era5.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2846 2023-04-01 13:15:27.000000 ls2d-1.0.2/ls2d/ecmwf/era_tools.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    30353 2023-05-24 12:11:48.000000 ls2d-1.0.2/ls2d/ecmwf/read_era5.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-24 12:13:37.299243 ls2d-1.0.2/ls2d/src/
+-rw-r--r--   0 bart      (1000) bart      (1000)        0 2023-04-01 13:15:27.000000 ls2d-1.0.2/ls2d/src/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1603 2023-04-01 13:15:27.000000 ls2d-1.0.2/ls2d/src/finite_difference.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     4108 2023-04-01 13:15:27.000000 ls2d-1.0.2/ls2d/src/grid.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1822 2023-04-01 13:15:27.000000 ls2d-1.0.2/ls2d/src/messages.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     7512 2023-04-01 13:15:27.000000 ls2d-1.0.2/ls2d/src/slurm.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2672 2023-04-01 13:15:27.000000 ls2d-1.0.2/ls2d/src/spatial_tools.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-24 12:13:37.299243 ls2d-1.0.2/ls2d.egg-info/
+-rw-r--r--   0 bart      (1000) bart      (1000)    44246 2023-05-24 12:13:37.000000 ls2d-1.0.2/ls2d.egg-info/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)      581 2023-05-24 12:13:37.000000 ls2d-1.0.2/ls2d.egg-info/SOURCES.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        1 2023-05-24 12:13:37.000000 ls2d-1.0.2/ls2d.egg-info/dependency_links.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)       61 2023-05-24 12:13:37.000000 ls2d-1.0.2/ls2d.egg-info/requires.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        5 2023-05-24 12:13:37.000000 ls2d-1.0.2/ls2d.egg-info/top_level.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)      990 2023-05-24 12:13:14.000000 ls2d-1.0.2/pyproject.toml
+-rw-r--r--   0 bart      (1000) bart      (1000)       38 2023-05-24 12:13:37.299243 ls2d-1.0.2/setup.cfg
```

### Comparing `ls2d-1.0.1/LICENSE.txt` & `ls2d-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ls2d-1.0.1/PKG-INFO` & `ls2d-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ls2d
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python toolkit to downscale ERA5 with doubly-periodic large-eddy simulation
 Author-email: Bart van Stratum <bart.vanstratum@wur.nl>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ls2d-1.0.1/README.md` & `ls2d-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ls2d-1.0.1/examples/microhh/cabauw.ini.base` & `ls2d-1.0.2/examples/microhh/cabauw.ini.base`

 * *Files identical despite different names*

### Comparing `ls2d-1.0.1/examples/microhh/link_lookup_tables.sh` & `ls2d-1.0.2/examples/microhh/link_lookup_tables.sh`

 * *Files identical despite different names*

### Comparing `ls2d-1.0.1/ls2d/__init__.py` & `ls2d-1.0.2/ls2d/__init__.py`

 * *Files identical despite different names*

### Comparing `ls2d-1.0.1/ls2d/ecmwf/IFS_tools.py` & `ls2d-1.0.2/ls2d/ecmwf/IFS_tools.py`

 * *Files identical despite different names*

### Comparing `ls2d-1.0.1/ls2d/ecmwf/L137_grid.txt` & `ls2d-1.0.2/ls2d/ecmwf/L137_grid.txt`

 * *Files identical despite different names*

### Comparing `ls2d-1.0.1/ls2d/ecmwf/L60_grid.txt` & `ls2d-1.0.2/ls2d/ecmwf/L60_grid.txt`

 * *Files identical despite different names*

### Comparing `ls2d-1.0.1/ls2d/ecmwf/__init__.py` & `ls2d-1.0.2/ls2d/ecmwf/__init__.py`

 * *Files identical despite different names*

### Comparing `ls2d-1.0.1/ls2d/ecmwf/download_era5.py` & `ls2d-1.0.2/ls2d/ecmwf/download_era5.py`

 * *Files identical despite different names*

### Comparing `ls2d-1.0.1/ls2d/ecmwf/era_tools.py` & `ls2d-1.0.2/ls2d/ecmwf/era_tools.py`

 * *Files identical despite different names*

### Comparing `ls2d-1.0.1/ls2d/ecmwf/read_era5.py` & `ls2d-1.0.2/ls2d/ecmwf/read_era5.py`

 * *Files 0% similar despite different names*

```diff
@@ -227,17 +227,17 @@
         self.Ts  =  get_variable(self.fsa, 'skt',  s2d)  # Skin temperature (K)
         self.H   = -get_variable(self.fsa, 'ishf', s2d)  # Surface sensible heat flux (W m-2)
         self.wqs = -get_variable(self.fsa, 'ie',   s2d)  # Surface kinematic moisture flux (g kg-1)
         self.z0m =  get_variable(self.fsa, 'fsr',  s2d)  # Surface roughness length (m)
         self.z0h =  get_variable(self.fsa, 'flsr', s2d, np.exp)  # Surface roughness length heat (m)
         self.ps  =  get_variable(self.fsa, 'sp',   s2d)  # Surface pressure (Pa)
 
-        self.soil_type     = get_variable(self.fsa, 'slt', s2d, np.round, np.int)  # Soil type (-)
-        self.veg_type_low  = get_variable(self.fsa, 'tvl', s2d, np.round, np.int)  # Low vegetation type (-)
-        self.veg_type_high = get_variable(self.fsa, 'tvh', s2d, np.round, np.int)  # High vegetation type (-)
+        self.soil_type     = get_variable(self.fsa, 'slt', s2d, np.round, np.int32)  # Soil type (-)
+        self.veg_type_low  = get_variable(self.fsa, 'tvl', s2d, np.round, np.int32)  # Low vegetation type (-)
+        self.veg_type_high = get_variable(self.fsa, 'tvh', s2d, np.round, np.int32)  # High vegetation type (-)
 
         self.lai_low  = get_variable(self.fsa, 'lai_lv', s2d)  # LAI low veg (-)
         self.lai_high = get_variable(self.fsa, 'lai_hv', s2d)  # LAI high veg (-)
 
         self.cveg_low  = get_variable(self.fsa, 'cvl', s2d)  # Low vegetation cover (-)
         self.cveg_high = get_variable(self.fsa, 'cvh', s2d)  # High vegetation cover (-)
```

### Comparing `ls2d-1.0.1/ls2d/src/finite_difference.py` & `ls2d-1.0.2/ls2d/src/finite_difference.py`

 * *Files identical despite different names*

### Comparing `ls2d-1.0.1/ls2d/src/grid.py` & `ls2d-1.0.2/ls2d/src/grid.py`

 * *Files identical despite different names*

### Comparing `ls2d-1.0.1/ls2d/src/messages.py` & `ls2d-1.0.2/ls2d/src/messages.py`

 * *Files identical despite different names*

### Comparing `ls2d-1.0.1/ls2d/src/slurm.py` & `ls2d-1.0.2/ls2d/src/slurm.py`

 * *Files identical despite different names*

### Comparing `ls2d-1.0.1/ls2d/src/spatial_tools.py` & `ls2d-1.0.2/ls2d/src/spatial_tools.py`

 * *Files identical despite different names*

### Comparing `ls2d-1.0.1/ls2d.egg-info/PKG-INFO` & `ls2d-1.0.2/ls2d.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ls2d
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python toolkit to downscale ERA5 with doubly-periodic large-eddy simulation
 Author-email: Bart van Stratum <bart.vanstratum@wur.nl>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ls2d-1.0.1/ls2d.egg-info/SOURCES.txt` & `ls2d-1.0.2/ls2d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ls2d-1.0.1/pyproject.toml` & `ls2d-1.0.2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 packages = [
     "ls2d",
     "ls2d.ecmwf",
     "ls2d.src"]
 
 [project]
 name = "ls2d"
-version = "1.0.1"
+version = "1.0.2"
 description = "Python toolkit to downscale ERA5 with doubly-periodic large-eddy simulation"
 readme = "README.md"
 authors = [{ name = "Bart van Stratum", email = "bart.vanstratum@wur.nl" }]
 license = { file = "LICENSE.txt" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python",
```

