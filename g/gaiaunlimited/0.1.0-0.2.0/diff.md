# Comparing `tmp/gaiaunlimited-0.1.0.tar.gz` & `tmp/gaiaunlimited-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaiaunlimited-0.1.0.tar", last modified: Wed Aug 31 20:57:31 2022, max compression
+gzip compressed data, was "gaiaunlimited-0.2.0.tar", last modified: Wed May 24 11:53:17 2023, max compression
```

## Comparing `gaiaunlimited-0.1.0.tar` & `gaiaunlimited-0.2.0.tar`

### file list

```diff
@@ -1,33 +1,41 @@
-drwxr-xr-x   0 soh        (501) staff       (20)        0 2022-08-31 20:57:31.372535 gaiaunlimited-0.1.0/
--rw-r--r--   0 soh        (501) staff       (20)     1521 2022-08-31 20:54:45.000000 gaiaunlimited-0.1.0/LICENSE
--rw-r--r--   0 soh        (501) staff       (20)     1754 2022-08-31 20:57:31.372626 gaiaunlimited-0.1.0/PKG-INFO
--rw-r--r--   0 soh        (501) staff       (20)      959 2022-08-30 00:05:11.000000 gaiaunlimited-0.1.0/README.md
--rw-r--r--   0 soh        (501) staff       (20)       80 2022-05-03 19:32:05.000000 gaiaunlimited-0.1.0/pyproject.toml
--rw-r--r--   0 soh        (501) staff       (20)     1135 2022-08-31 20:57:31.373120 gaiaunlimited-0.1.0/setup.cfg
-drwxr-xr-x   0 soh        (501) staff       (20)        0 2022-08-31 20:57:31.351500 gaiaunlimited-0.1.0/src/
-drwxr-xr-x   0 soh        (501) staff       (20)        0 2022-08-31 20:57:31.353607 gaiaunlimited-0.1.0/src/gaiaunlimited/
--rw-r--r--   0 soh        (501) staff       (20)       78 2022-08-31 20:54:45.000000 gaiaunlimited-0.1.0/src/gaiaunlimited/__init__.py
-drwxr-xr-x   0 soh        (501) staff       (20)        0 2022-08-31 20:57:31.354864 gaiaunlimited-0.1.0/src/gaiaunlimited/data/
-drwxr-xr-x   0 soh        (501) staff       (20)        0 2022-08-31 20:57:31.370443 gaiaunlimited-0.1.0/src/gaiaunlimited/data/dr2/
--rw-r--r--   0 soh        (501) staff       (20)    15083 2022-08-30 00:05:11.000000 gaiaunlimited-0.1.0/src/gaiaunlimited/data/dr2/Astrometry.csv
--rw-r--r--   0 soh        (501) staff       (20)      723 2022-08-30 00:05:11.000000 gaiaunlimited-0.1.0/src/gaiaunlimited/data/dr2/Photometry.csv
--rw-r--r--   0 soh        (501) staff       (20)    15776 2022-08-30 00:05:11.000000 gaiaunlimited-0.1.0/src/gaiaunlimited/data/dr2/Spectroscopy.csv
-drwxr-xr-x   0 soh        (501) staff       (20)        0 2022-08-31 20:57:31.370954 gaiaunlimited-0.1.0/src/gaiaunlimited/data/dr3/
--rw-r--r--   0 soh        (501) staff       (20)     6881 2022-08-31 20:54:45.000000 gaiaunlimited-0.1.0/src/gaiaunlimited/data/dr3/Astrometry.csv
--rw-r--r--   0 soh        (501) staff       (20)     7755 2022-08-31 20:54:45.000000 gaiaunlimited-0.1.0/src/gaiaunlimited/data/dr3/Photometry.csv
--rw-r--r--   0 soh        (501) staff       (20)   193444 2022-08-31 20:54:45.000000 gaiaunlimited-0.1.0/src/gaiaunlimited/data/dr3/Spectroscopy.csv
--rw-r--r--   0 soh        (501) staff       (20) 16649513 2022-08-30 00:05:11.000000 gaiaunlimited-0.1.0/src/gaiaunlimited/data/horizons_results_gaia.txt
--rw-r--r--   0 soh        (501) staff       (20)     5752 2022-08-30 00:05:11.000000 gaiaunlimited-0.1.0/src/gaiaunlimited/fetch_utils.py
--rw-r--r--   0 soh        (501) staff       (20)    10356 2022-08-31 20:54:45.000000 gaiaunlimited-0.1.0/src/gaiaunlimited/scanninglaw.py
-drwxr-xr-x   0 soh        (501) staff       (20)        0 2022-08-31 20:57:31.372365 gaiaunlimited-0.1.0/src/gaiaunlimited/selectionfunctions/
--rw-r--r--   0 soh        (501) staff       (20)       72 2022-08-30 00:05:11.000000 gaiaunlimited-0.1.0/src/gaiaunlimited/selectionfunctions/__init__.py
--rw-r--r--   0 soh        (501) staff       (20)     6981 2022-08-30 00:05:11.000000 gaiaunlimited-0.1.0/src/gaiaunlimited/selectionfunctions/subsample.py
--rw-r--r--   0 soh        (501) staff       (20)     6844 2022-08-30 00:05:11.000000 gaiaunlimited-0.1.0/src/gaiaunlimited/selectionfunctions/survey.py
--rw-r--r--   0 soh        (501) staff       (20)    10147 2022-08-30 00:05:11.000000 gaiaunlimited-0.1.0/src/gaiaunlimited/selectionfunctions/surveyTCG.py
--rw-r--r--   0 soh        (501) staff       (20)     2427 2022-08-30 00:05:11.000000 gaiaunlimited-0.1.0/src/gaiaunlimited/utils.py
-drwxr-xr-x   0 soh        (501) staff       (20)        0 2022-08-31 20:57:31.354744 gaiaunlimited-0.1.0/src/gaiaunlimited.egg-info/
--rw-r--r--   0 soh        (501) staff       (20)     1754 2022-08-31 20:57:31.000000 gaiaunlimited-0.1.0/src/gaiaunlimited.egg-info/PKG-INFO
--rw-r--r--   0 soh        (501) staff       (20)      870 2022-08-31 20:57:31.000000 gaiaunlimited-0.1.0/src/gaiaunlimited.egg-info/SOURCES.txt
--rw-r--r--   0 soh        (501) staff       (20)        1 2022-08-31 20:57:31.000000 gaiaunlimited-0.1.0/src/gaiaunlimited.egg-info/dependency_links.txt
--rw-r--r--   0 soh        (501) staff       (20)       71 2022-08-31 20:57:31.000000 gaiaunlimited-0.1.0/src/gaiaunlimited.egg-info/requires.txt
--rw-r--r--   0 soh        (501) staff       (20)       14 2022-08-31 20:57:31.000000 gaiaunlimited-0.1.0/src/gaiaunlimited.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:53:17.281977 gaiaunlimited-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-24 11:53:04.000000 gaiaunlimited-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-05-24 11:53:17.281977 gaiaunlimited-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-24 11:53:04.000000 gaiaunlimited-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-24 11:53:04.000000 gaiaunlimited-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-24 11:53:17.281977 gaiaunlimited-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:53:17.261977 gaiaunlimited-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:53:17.265977 gaiaunlimited-0.2.0/src/gaiaunlimited/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-24 11:53:04.000000 gaiaunlimited-0.2.0/src/gaiaunlimited/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:53:17.265977 gaiaunlimited-0.2.0/src/gaiaunlimited/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   218094 2023-05-24 11:53:04.000000 gaiaunlimited-0.2.0/src/gaiaunlimited/data/apogee_sampling_fractions.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:53:17.281977 gaiaunlimited-0.2.0/src/gaiaunlimited/data/dr2/
+-rw-r--r--   0 runner    (1001) docker     (123)    15083 2023-05-24 11:53:04.000000 gaiaunlimited-0.2.0/src/gaiaunlimited/data/dr2/Astrometry.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-24 11:53:04.000000 gaiaunlimited-0.2.0/src/gaiaunlimited/data/dr2/Photometry.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    15776 2023-05-24 11:53:04.000000 gaiaunlimited-0.2.0/src/gaiaunlimited/data/dr2/Spectroscopy.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:53:17.281977 gaiaunlimited-0.2.0/src/gaiaunlimited/data/dr3/
+-rw-r--r--   0 runner    (1001) docker     (123)     6881 2023-05-24 11:53:04.000000 gaiaunlimited-0.2.0/src/gaiaunlimited/data/dr3/Astrometry.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7755 2023-05-24 11:53:04.000000 gaiaunlimited-0.2.0/src/gaiaunlimited/data/dr3/Photometry.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   193444 2023-05-24 11:53:04.000000 gaiaunlimited-0.2.0/src/gaiaunlimited/data/dr3/Spectroscopy.csv
+-rw-r--r--   0 runner    (1001) docker     (123) 16649513 2023-05-24 11:53:04.000000 gaiaunlimited-0.2.0/src/gaiaunlimited/data/horizons_results_gaia.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-05-24 11:53:04.000000 gaiaunlimited-0.2.0/src/gaiaunlimited/fetch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10750 2023-05-24 11:53:04.000000 gaiaunlimited-0.2.0/src/gaiaunlimited/scanninglaw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:53:17.281977 gaiaunlimited-0.2.0/src/gaiaunlimited/selectionfunctions/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-24 11:53:04.000000 gaiaunlimited-0.2.0/src/gaiaunlimited/selectionfunctions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-05-24 11:53:04.000000 gaiaunlimited-0.2.0/src/gaiaunlimited/selectionfunctions/apogee.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12137 2023-05-24 11:53:04.000000 gaiaunlimited-0.2.0/src/gaiaunlimited/selectionfunctions/subsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6832 2023-05-24 11:53:04.000000 gaiaunlimited-0.2.0/src/gaiaunlimited/selectionfunctions/survey.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13545 2023-05-24 11:53:04.000000 gaiaunlimited-0.2.0/src/gaiaunlimited/selectionfunctions/surveyTCG.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-05-24 11:53:04.000000 gaiaunlimited-0.2.0/src/gaiaunlimited/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:53:17.265977 gaiaunlimited-0.2.0/src/gaiaunlimited.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-05-24 11:53:17.000000 gaiaunlimited-0.2.0/src/gaiaunlimited.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-24 11:53:17.000000 gaiaunlimited-0.2.0/src/gaiaunlimited.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 11:53:17.000000 gaiaunlimited-0.2.0/src/gaiaunlimited.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-24 11:53:17.000000 gaiaunlimited-0.2.0/src/gaiaunlimited.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-24 11:53:17.000000 gaiaunlimited-0.2.0/src/gaiaunlimited.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:53:17.281977 gaiaunlimited-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-24 11:53:04.000000 gaiaunlimited-0.2.0/tests/test_apogee.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-24 11:53:04.000000 gaiaunlimited-0.2.0/tests/test_scanninglaw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-24 11:53:04.000000 gaiaunlimited-0.2.0/tests/test_subsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-05-24 11:53:04.000000 gaiaunlimited-0.2.0/tests/test_survey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-24 11:53:04.000000 gaiaunlimited-0.2.0/tests/test_surveyTCG.py
```

### Comparing `gaiaunlimited-0.1.0/LICENSE` & `gaiaunlimited-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gaiaunlimited-0.1.0/PKG-INFO` & `gaiaunlimited-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaiaunlimited
-Version: 0.1.0
+Version: 0.2.0
 Summary: Tools for manipulating Gaia selection functions.
 Home-page: https://github.com/GaiaUnlimited/gaiaunlimited
 Author: GaiaUnlimited
 Maintainer: Alfred Castro-Ginard, Tristan Cantat-Gaudin
 Maintainer-email: acastro@strw.leidenuniv.nl, cantat@mpia-hd.mpg.de
 Project-URL: Bug Tracker, https://github.com/GaiaUnlimited/gaiaunlimited/issues
 Keywords: astronomy,Gaia,selection function,scanning law
@@ -13,29 +13,30 @@
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Gaiaunlimited
+# gaiaunlimited
 
-Gaiaunlimited is a package for querying and constructing selection functions for the Gaia survey. It is developed by the GaiaUnlimited collaboration.
+[![pypi status](https://img.shields.io/pypi/v/dustapprox.svg)](https://pypi.org/project/dustapprox/)
+[![Documentation Status](https://readthedocs.org/projects/gaiaunlimited/badge/?version=latest)](https://gaiaunlimited.readthedocs.io/en/latest/?badge=latest)
+
+gaiaunlimited is a package for querying and constructing selection functions for the Gaia survey. It is developed by the GaiaUnlimited collaboration.
+
+The documentation for gaiaunlimited is hosted on [Read the docs](https://gaiaunlimited.readthedocs.io/en/latest).
+
+*The [GaiaUnlimited](https://gaia-unlimited.org/) project is funded by the European Union’s Horizon 2020 research and innovation program under grant agreement No 101004110.*
 
 ## Features
 
 - Query Gaia scanning laws for when a given sky position is scanned.
 - Query Gaia survey selection functions for the probabilities that sources of given properties are included in the Gaia catalog.
 - Query ready-made Gaia DR3 subsample selection functions for
 	- the astrometry sample
 	- the RVS sample
 
-## Documentation
-
-[![Documentation Status](https://readthedocs.org/projects/gaiaunlimited/badge/?version=latest)](https://gaiaunlimited.readthedocs.io/en/latest/?badge=latest)
-
-The documentation for gaiaunlimited is hosted on [Read the docs](https://gaiaunlimited.readthedocs.io/en/latest).
-
 ## Acknowledgements
 
 This work is part of the GaiaUnlimited project funded by the European Union’s
 Horizon 2020 research and innovation program under grant agreement No 101004110.
```

### Comparing `gaiaunlimited-0.1.0/README.md` & `gaiaunlimited-0.2.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-# Gaiaunlimited
+# gaiaunlimited
 
-Gaiaunlimited is a package for querying and constructing selection functions for the Gaia survey. It is developed by the GaiaUnlimited collaboration.
+[![pypi status](https://img.shields.io/pypi/v/dustapprox.svg)](https://pypi.org/project/dustapprox/)
+[![Documentation Status](https://readthedocs.org/projects/gaiaunlimited/badge/?version=latest)](https://gaiaunlimited.readthedocs.io/en/latest/?badge=latest)
+
+gaiaunlimited is a package for querying and constructing selection functions for the Gaia survey. It is developed by the GaiaUnlimited collaboration.
+
+The documentation for gaiaunlimited is hosted on [Read the docs](https://gaiaunlimited.readthedocs.io/en/latest).
+
+*The [GaiaUnlimited](https://gaia-unlimited.org/) project is funded by the European Union’s Horizon 2020 research and innovation program under grant agreement No 101004110.*
 
 ## Features
 
 - Query Gaia scanning laws for when a given sky position is scanned.
 - Query Gaia survey selection functions for the probabilities that sources of given properties are included in the Gaia catalog.
 - Query ready-made Gaia DR3 subsample selection functions for
 	- the astrometry sample
 	- the RVS sample
 
-## Documentation
-
-[![Documentation Status](https://readthedocs.org/projects/gaiaunlimited/badge/?version=latest)](https://gaiaunlimited.readthedocs.io/en/latest/?badge=latest)
-
-The documentation for gaiaunlimited is hosted on [Read the docs](https://gaiaunlimited.readthedocs.io/en/latest).
-
 ## Acknowledgements
 
 This work is part of the GaiaUnlimited project funded by the European Union’s
 Horizon 2020 research and innovation program under grant agreement No 101004110.
```

### Comparing `gaiaunlimited-0.1.0/setup.cfg` & `gaiaunlimited-0.2.0/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -21,16 +21,17 @@
 [options]
 packages = find_namespace:
 package_dir = 
 	= src
 python_requires = >=3.7
 install_requires = 
 	numpy
-	scipy
+	scipy >= 1.6.0
 	astropy
+	astropy_healpix
 	astroquery
 	pandas
 	xarray
 	healpy
 	h5py
 	tqdm
 	requests
@@ -39,12 +40,13 @@
 where = src
 
 [options.package_data]
 gaiaunlimited.data = 
 	dr2/*.csv
 	dr3/*.csv
 	horizons_results_gaia.txt
+	apogee_sampling_fractions.csv
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `gaiaunlimited-0.1.0/src/gaiaunlimited/data/dr2/Astrometry.csv` & `gaiaunlimited-0.2.0/src/gaiaunlimited/data/dr2/Astrometry.csv`

 * *Files identical despite different names*

### Comparing `gaiaunlimited-0.1.0/src/gaiaunlimited/data/dr2/Photometry.csv` & `gaiaunlimited-0.2.0/src/gaiaunlimited/data/dr2/Photometry.csv`

 * *Files identical despite different names*

### Comparing `gaiaunlimited-0.1.0/src/gaiaunlimited/data/dr2/Spectroscopy.csv` & `gaiaunlimited-0.2.0/src/gaiaunlimited/data/dr2/Spectroscopy.csv`

 * *Files identical despite different names*

### Comparing `gaiaunlimited-0.1.0/src/gaiaunlimited/data/dr3/Astrometry.csv` & `gaiaunlimited-0.2.0/src/gaiaunlimited/data/dr3/Astrometry.csv`

 * *Files identical despite different names*

### Comparing `gaiaunlimited-0.1.0/src/gaiaunlimited/data/dr3/Photometry.csv` & `gaiaunlimited-0.2.0/src/gaiaunlimited/data/dr3/Photometry.csv`

 * *Files identical despite different names*

### Comparing `gaiaunlimited-0.1.0/src/gaiaunlimited/data/dr3/Spectroscopy.csv` & `gaiaunlimited-0.2.0/src/gaiaunlimited/data/dr3/Spectroscopy.csv`

 * *Files identical despite different names*

### Comparing `gaiaunlimited-0.1.0/src/gaiaunlimited/data/horizons_results_gaia.txt` & `gaiaunlimited-0.2.0/src/gaiaunlimited/data/horizons_results_gaia.txt`

 * *Files identical despite different names*

### Comparing `gaiaunlimited-0.1.0/src/gaiaunlimited/fetch_utils.py` & `gaiaunlimited-0.2.0/src/gaiaunlimited/fetch_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,19 @@
 class DownloadError(Exception):
     """
     An exception that occurs while trying to download a file.
     """
 
 
 def get_datadir():
-    """Get gaiasf data directory as Path."""
+    """Get gaiasf data directory as Path.
+    
+    Return type:
+        pathlib.PosixPath object
+    """
     p = (
         Path(os.getenv("GAIAUNLIMITED_DATADIR", "~/.gaiaunlimited"))
         .expanduser()
         .resolve()
     )
     return p
 
@@ -156,13 +160,17 @@
                 path_to_file1 = self._get_data('myfile1')
                 with h5py.File(path_to_file1) as f:
                     ...
     """
 
     def _get_data(self, filename):
         """Download data files specified in datafiles dict class attribute."""
+        savedir = get_datadir()
+        if not savedir.exists():
+            print('Creating directory',savedir)
+            os.makedirs(savedir)
         fullpath = get_datadir() / filename
         if not fullpath.exists():
             url = self.datafiles[filename]
             with open(fullpath, "wb") as f:
                 download(url, f)
         return fullpath
```

### Comparing `gaiaunlimited-0.1.0/src/gaiaunlimited/scanninglaw.py` & `gaiaunlimited-0.2.0/src/gaiaunlimited/scanninglaw.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,16 +37,16 @@
     return (obmt - 1717.6256) / 4 - (2455197.5 - 2457023.5 - 0.25)
 
 
 def make_rotmat(fov1_xyz, fov2_xyz):
     """Make rotational matrix from ICRS to Gaia body frame(ish).
 
     Args:
-    fov1_xyz (array-like): vector pointing to FoV1. Should have shape (..., 3)
-    fov2_xyz (array-like): vector pointing to FoV2. Should have shape (..., 3)
+        fov1_xyz (array-like): vector pointing to FoV1. Should have shape (..., 3)
+        fov2_xyz (array-like): vector pointing to FoV2. Should have shape (..., 3)
 
     Returns:
         rotation matrix (..., 3, 3)
     """
     fov1_xyz, fov2_xyz = np.atleast_2d(fov1_xyz), np.atleast_2d(fov2_xyz)
     _xaxis = fov1_xyz
     _zaxis = np.cross(fov1_xyz, fov2_xyz)
@@ -54,20 +54,37 @@
     _yaxis /= np.linalg.norm(_yaxis, axis=1)[:, np.newaxis]
     _zaxis /= np.linalg.norm(_zaxis, axis=1)[:, np.newaxis]
     _matrix = np.moveaxis(np.stack((_xaxis, _yaxis, _zaxis)), 1, 0)
     return np.squeeze(_matrix)
 
 
 def angle2dist3d(sepangle):
-    """Get equivalent 3d distance of an angle on a unit sphere."""
+    """
+    Get equivalent 3d distance of an angle on a unit sphere.
+    
+    Args:
+        sepangle (float): separation in degree
+        
+    Returns:
+        float: distance corresponding to the angle on a unit sphere
+    """
     r = 2 * np.sin(np.deg2rad(sepangle) / 2.0)
     return r
 
 
 def cartesian_to_spherical(xyz):
+    """
+    Convert cartesian XYZ to (longitude,latitude).
+    
+    Args:
+        xyz ((N,3) array): (X,Y,Z) coordinates for each point
+        
+    Returns:
+        (2,N) array: longitude and latitude of each point
+    """
     lon = np.rad2deg(np.arctan2(xyz[:, 1], xyz[:, 0]))
     lat = np.rad2deg(
         np.arctan2(xyz[:, 2], np.sqrt(xyz[:, 0] ** 2.0 + xyz[:, 1] ** 2.0))
     )
     return lon, lat
```

### Comparing `gaiaunlimited-0.1.0/src/gaiaunlimited/selectionfunctions/subsample.py` & `gaiaunlimited-0.2.0/src/gaiaunlimited/selectionfunctions/survey.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,147 +1,143 @@
 import h5py
-import pandas as pd
 import healpy as hp
 import numpy as np
 import xarray as xr
-from scipy.special import expit, logit
+from scipy import stats
 
-from gaiaunlimited import fetch_utils, utils
+from .. import fetch_utils, utils
 
-__all__ = [
-    "SelectionFunctionBase",
-    "DR3RVSSelectionFunction",
-    "EDR3RVSSelectionFunction",
-]
-
-
-def _validate_ds(ds):
-    """Validate if xarray.Dataset contains the expected selection function data."""
-    if not isinstance(ds, xr.Dataset):
-        raise ValueError("ds must be an xarray.Dataset.")
-    for required_variable in ["logitp"]:
-        if required_variable not in ds:
-            raise ValueError(f"missing required variable {required_variable}.")
-    diff = set(ds["logitp"].dims) - set(["g", "c", "ipix"])
-    if diff:
-        raise ValueError(f"Unrecognized dims of probability array: {diff}")
-
-
-# TODO: spec out base class and op for combining SFs
-class SelectionFunctionBase:
-    """Base class for Gaia selection functions.
-
-    Selection function is defined as the selection probability as a function of
-    Gaia G magnitude and healpix location, and optionally also on G-G_PR color.
-
-    We use xarray.Dataset as the main data structure to contain this
-    multi-dimensional map of probabilities. This Dataset instance should be
-    attach as `.ds` and have the following schema:
-
-        - must contain data variable `p` and `logitp` for selection probability
-          and logit of that selection probability.
-        - must have coodinates
-            - ipix for healpix id in int64 dtype
-            - g for Gaia G magnitude
-            - c for Gaia G - G_RP color
+__all__ = ["DR2SelectionFunction", "DR3SelectionFunction"]
 
-    It is assumed that ipix is the full index array for the given healpix order
-    with no missing index.
-    """
 
-    def __init__(self, ds):
-        _validate_ds(ds)
-        self.ds = ds
+# Selection functions ported from gaiaverse's work ----------------
+class DR2SelectionFunction(fetch_utils.DownloadMixin):
+    """DR2 selection function developed by the Gaiaverse team."""
+
+    __bibtex__ = """
+@ARTICLE{2020MNRAS.497.4246B,
+       author = {{Boubert}, Douglas and {Everall}, Andrew},
+        title = "{Completeness of the Gaia verse II: what are the odds that a star is missing from Gaia DR2?}",
+      journal = {\mnras},
+     keywords = {methods: data analysis, methods: statistical, stars: statistics, Galaxy: kinematics and dynamics, Galaxy: stellar content, Astrophysics - Astrophysics of Galaxies, Astrophysics - Instrumentation and Methods for Astrophysics, Astrophysics - Solar and Stellar Astrophysics},
+         year = 2020,
+        month = oct,
+       volume = {497},
+       number = {4},
+        pages = {4246-4261},
+          doi = {10.1093/mnras/staa2305},
+archivePrefix = {arXiv},
+       eprint = {2005.08983},
+ primaryClass = {astro-ph.GA},
+       adsurl = {https://ui.adsabs.harvard.edu/abs/2020MNRAS.497.4246B},
+      adsnote = {Provided by the SAO/NASA Astrophysics Data System}
+}
+"""
+    datafiles = {
+        "cog_ii_dr2.h5": "https://dataverse.harvard.edu/api/access/datafile/:persistentId?persistentId=doi:10.7910/DVN/PDFOVC/NYV9DM"
+    }
+    nside_n_field = 4096
+    nside_crowding = 1024
 
-    @property
-    def order(self):
-        """Order of the HEALPix."""
-        return hp.npix2order(self.ds["ipix"].size)
-
-    @property
-    def nside(self):
-        """Nside of the HEALPix."""
-        return hp.npix2nside(self.ds["ipix"].size)
-
-    @property
-    def factors(self):
-        """Variables other than HEALPix id that define the selection function."""
-        return set(self.ds["logitp"].dims) - set({"ipix"})
-
-    def __mul__(self, other):
-        # if not isinstance(other, SelectionFunctionBase):
-        #     raise TypeError()
-        # TODO
-        raise NotImplementedError()
-
-    @classmethod
-    def from_conditions(cls, conditions):
-        # potential idea
-        # TODO: query for conditions and make Dataset from result
-        raise NotImplementedError()
+    def __init__(self):
+        with h5py.File(self._get_data("cog_ii_dr2.h5")) as f:
+            # NOTE: HEAL pixelisation is in ICRS in these files!
+            # n_field heal order=12, nside=4096
+            # neighbour_field heal order=10, nside=1024
+            theta = f["t_theta_percentiles"][()]
+            alpha = f["ab_alpha_percentiles"][()]
+            beta = f["ab_beta_percentiles"][()]
+            ds = xr.Dataset(
+                data_vars=dict(
+                    theta=(["logrho", "g", "perc"], theta),
+                    alpha=(["logrho", "g", "perc"], alpha),
+                    beta=(["logrho", "g", "perc"], beta),
+                    n_field=("ipix", f["n_field"][()].astype(np.uint16)),
+                    neighbour_field=(["ipix_logrho"], f["neighbour_field"][()]),
+                ),
+                coords=dict(
+                    logrho=f["log10_rho_grid"][()],
+                    g=f["g_grid"][()],
+                ),
+            )
+        # Add logrho
+        ds["logrho_field"] = np.log10(
+            np.maximum(1.0, ds["neighbour_field"])
+            / hp.nside2pixarea(self.nside_crowding, degrees=True)
+        )
+        self.ds = ds
 
-    def query(self, coords, **kwargs):
-        """Query the selection function at the given coordinates.
+    def query(self, coords, gmag, use_modelT=False):
+        """Query the selection function.
 
         Args:
             coords: sky coordinates as an astropy coordinates instance.
-
-        Other factors that determine this selection function should be given
-        as keyword arguments of the same shape as coords.
+            gmag (float or array): Gaia G magnitudes. Should have the same size as coords.
 
         Returns:
-            np.array: array of internal selection probabilities.
+            np.array : array of selection probabilities.
         """
-        # NOTE: make input atleast_1d for .interp keyword consistency.
-        ipix = utils.coord2healpix(coords, "icrs", self.nside, nest=True)
-        ipix = xr.DataArray(np.atleast_1d(ipix))
-        d = {}
-        for k in self.factors:
-            if k not in kwargs:
-                raise ValueError(f"{k} values are missing.")
-            d[k] = xr.DataArray(np.atleast_1d(kwargs[k]))
-        d["method"] = "nearest"
-        d["kwargs"] = dict(fill_value=None)  # extrapolates
-        out = self.ds["logitp"].interp(ipix=ipix, **d).to_numpy()
-        if len(coords.shape) == 0:
-            out = out.squeeze()
-        return expit(out)
-
-
-class DR3RVSSelectionFunction(SelectionFunctionBase, fetch_utils.DownloadMixin):
-    """Internal selection function for the RVS sample in DR3.
-
-    This function gives the probability
-        P(has RV | has G and G_RP)
-    as a function of G magnitude and G-RP color.
-    """
-
-    datafiles = {
-        "dr3-rvs-nk.h5": "https://dataverse.harvard.edu/api/access/datafile/6424746"
-    }
-
-    def __init__(self):
-        with h5py.File(self._get_data("dr3-rvs-nk.h5")) as f:
-            df = pd.DataFrame.from_records(f["data"][()])
-            df["p"] = (df["k"] + 1) / (df["n"] + 2)
-            df["logitp"] = logit(df["p"])
-            dset_dr3 = xr.Dataset.from_dataframe(df.set_index(["ipix", "i_g", "i_c"]))
-            gcenters, ccenters = f["g_mid"][()], f["c_mid"][()]
-            dset_dr3 = dset_dr3.assign_coords(i_g=gcenters, i_c=ccenters)
-            dset_dr3 = dset_dr3.rename({"i_g": "g", "i_c": "c"})
-            super().__init__(dset_dr3)
-
+        if coords.shape != np.shape(gmag):
+            raise ValueError(f"Input shape mismatch: {coords.shape} != {gmag.shape}")
+        if coords.ndim >= 2:
+            raise ValueError(f"Input must be a scalar or 1d array")
+
+        ipix = utils.coord2healpix(coords, "icrs", self.nside_n_field)
+        ipix_logrho = utils.coord2healpix(coords, "icrs", self.nside_crowding)
+        logrho = self.ds["logrho_field"].sel(ipix_logrho=ipix_logrho).to_numpy()
+
+        # NOTE: xr.DataArray's interp method calls scipy's interp1d or interpnd
+        # depending on the input shape. The two methods do not have a consistent
+        # keyword for `fill_value` when we want to force extrapolation.
+        # For interp1d, it is 'extrapolate', for interpnd it is None.
+        # Let's make input at least 1d array so that we can not worry about this.
+        ipix = np.atleast_1d(ipix)
+        gmag = np.atleast_1d(gmag)
+        logrho = np.atleast_1d(logrho)
+        ns = self.ds["n_field"].sel(ipix=ipix).to_numpy()
+        kwargs = dict(
+            method="nearest",
+            kwargs=dict(fill_value=None),
+        )
+        if use_modelT:
+            ps = (
+                self.ds["theta"]
+                .sel(perc=2)
+                .interp(g=xr.DataArray(gmag), logrho=xr.DataArray(logrho), **kwargs)
+                .to_numpy()
+            )
+            out = stats.binom(ns, ps).sf(4)
+        else:
+            alphas = (
+                self.ds["alpha"]
+                .sel(perc=2)
+                .interp(g=xr.DataArray(gmag), logrho=xr.DataArray(logrho), **kwargs)
+                .to_numpy()
+            )
+            betas = (
+                self.ds["beta"]
+                .sel(perc=2)
+                .interp(g=xr.DataArray(gmag), logrho=xr.DataArray(logrho), **kwargs)
+                .to_numpy()
+            )
+            out = stats.betabinom(ns, alphas, betas).sf(4)
 
-# Selection functions ported from gaiaverse's work ----------------
-class EDR3RVSSelectionFunction(SelectionFunctionBase, fetch_utils.DownloadMixin):
-    """Internal selection function for the RVS sample in EDR3.
+        if len(coords.shape) == 0:
+            return out.squeeze()
+        else:
+            return out
 
-    This has been ported from the selectionfunctions by Gaiaverse team.
 
-    NOTE: The definition of the RVS sample is not the same as DR3RVSSelectionFunction.
+class DR3SelectionFunction(DR2SelectionFunction):
+    """DR3 selection function developed by the Gaiaverse team.
+
+    This selection function assumes the same detection probability and simply
+    swaps the number of scans map (since DR3 covers a longer mission time).  The
+    map resolution also changed from HEAL order 12 (nside=4096) to order 10
+    (nside=1024).
     """
 
     __bibtex__ = """
 @ARTICLE{2022MNRAS.509.6205E,
        author = {{Everall}, Andrew and {Boubert}, Douglas},
         title = "{Completeness of the Gaia verse - V. Astrometry and radial velocity sample selection functions in Gaia EDR3}",
       journal = {\mnras},
@@ -155,33 +151,19 @@
 archivePrefix = {arXiv},
        eprint = {2111.04127},
  primaryClass = {astro-ph.GA},
        adsurl = {https://ui.adsabs.harvard.edu/abs/2022MNRAS.509.6205E},
       adsnote = {Provided by the SAO/NASA Astrophysics Data System}
 }
 """
+    datafiles = DR2SelectionFunction.datafiles.copy()
+    datafiles.update(
+        {"n_field_dr3.h5": "https://dataverse.harvard.edu/api/access/datafile/4204267"}
+    )
+    nside_n_field = 1024
+    nside_crowding = 1024
 
-    datafiles = {
-        "rvs_cogv.h5": "https://dataverse.harvard.edu/api/access/datafile/5203267"
-    }
+    def __init__(self, *args, **kwargs):
+        super(DR3SelectionFunction, self).__init__()
 
-    # frame = ''
-
-    def __init__(self):
-        with h5py.File(self._get_data("rvs_cogv.h5")) as f:
-            # NOTE: HEAL pixelisation is in ICRS in these files!
-            # x is the logit probability evaluated at each (mag, color, ipix)
-            x = f["x"][()]  # dims: (n_mag_bins, n_color_bins, n_healpix_order6)
-            # these are model parameters
-            # b = f['b'][()]
-            # z = f['z'][()]
-            attrs = dict(f["x"].attrs.items())
-            n_gbins, n_cbins, n_pix = x.shape
-            gbins = np.linspace(*attrs["Mlim"], n_gbins + 1)
-            cbins = np.linspace(*attrs["Clim"], n_cbins + 1)
-            edges2centers = lambda x: (x[1:] + x[:-1]) * 0.5
-            gcenters, ccenters = edges2centers(gbins), edges2centers(cbins)
-            ds = xr.Dataset(
-                data_vars=dict(logitp=(["g", "c", "ipix"], x)),
-                coords=dict(g=gcenters, c=ccenters),
-            )
-        super().__init__(ds)
+        with h5py.File(self._get_data("n_field_dr3.h5")) as f:
+            self.ds["n_field"] = ("ipix", f["n_field"][()].astype(np.uint16))
```

### Comparing `gaiaunlimited-0.1.0/src/gaiaunlimited/selectionfunctions/surveyTCG.py` & `gaiaunlimited-0.2.0/src/gaiaunlimited/selectionfunctions/surveyTCG.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,243 +1,287 @@
 import numpy as np
 import healpy as hp
-from gaiaunlimited import fetch_utils, utils
 import h5py
 from astroquery.gaia import Gaia
+from astropy.table import Table
+import astropy_healpix as ah
+import astropy.units as u
+from astropy.coordinates import SkyCoord
+
+from .. import fetch_utils, utils
+
+__all__ = [
+    "DR3SelectionFunctionTCG",
+    "build_patch_map",
+    "sigmoid",
+    "m10_to_completeness",
+]
 
 Gaia.MAIN_GAIA_TABLE = "gaiadr3.gaia_source"
 Gaia.ROW_LIMIT = -1  # default is 50 rows max, -1 for unlimited
 
 
-class DR3SelectionFunctionTCG:
-    """Model of the Gaia DR3 survey selection function calibrated on DECaPS."""
+class DR3SelectionFunctionTCG(fetch_utils.DownloadMixin):
+    """Model of the Gaia DR3 survey selection function calibrated on DECaPS.
 
-    def __init__(self, m10map):
-        # NOTE: HEAL pixelisation is in ICRS in these files!
-        self.m10map = m10map
+    Available in three flavours:
 
-    def query(self, coords, gmag):
-        """Query the selection function.
+    *   mode = 'hpx7' (default)
+        Uses a map precomputed in healpix regions of order 7.
 
-        Args:
-            coords: sky coordinates as an astropy coordinates instance.
-            gmag (float or array): G magnitudes. Should have the same shape as coords.
+    *   mode='multi'
+        Uses a precomputed map of variable resolution,
+        with healpixels as small as order 10, provided they contain at least 20 sources.
 
-        Returns:
-            prob: array of selection probabilities.
-        """
-        if coords.shape != np.shape(gmag):
-            raise ValueError(f"Input shape mismatch: {coords.shape} != {gmag.shape}")
-        order_map = self.m10map[:, 0].astype(np.int64)
-        ipix_map = self.m10map[:, 1].astype(np.int64)
-        m10_map = self.m10map[:, 2]
-        nside = 2 ** order_map[0]
-        ipix = utils.coord2healpix(coords, "icrs", nside)
-        # if using custom maps, the user might query a point outside the map:
-        is_in_map = np.in1d(ipix, ipix_map)
-        if np.all(is_in_map) == False:
-            print("Warning: the following points are outside the map:")
-            print(coords[~is_in_map])
-            # find the missing ipix, temporarily add them with value Nan
-            missingIpix = sorted(set(ipix[~is_in_map]))
-            for mip in missingIpix:
-                ipix_map = np.append(ipix_map, mip)
-                m10_map = np.append(m10_map, np.nan)
-        pointIndices = np.array(
-            [np.where(ipix_map == foo)[0][0] for foo in ipix]
-        )  # horrendous but works, could be clearer with np.in1d?
-        allM10 = m10_map[pointIndices]
-        prob = m10_to_completeness(gmag.astype(float), allM10)
-        return prob
-
-    # @classmethod
-    # def from_patch(cls, *args, **kwargs):
-    #    pass
-    #    # make m10map
-    #    # return cls(m10map)
+    *   mode='patch'
+        The field of view is a circular patch of radius 'radius' centered on (ra,dec).
+        The spatial resolution will vary across the field of view,
+        from healpix order 6 to 12, enforcing that bins must contain
+        at least min_points sources (default 20). A low number makes the map
+        more detailed but also noisier.
+
+    Arguments:
+        mode: 'hpx7' or 'multi' or 'patch' (defaults to 'hpx7')
+
+    In 'patch' mode only:
+        ra: right ascension of centre of field of view, in degrees
+        dec: declination of centre of field of view, in degrees
+        size: width/height of the square field of view, in degrees
+        min_points: minimum number of sources used to compute the map
 
+    If you use this model in a publication please cite::
 
-class DR3SelectionFunctionTCG_hpx7(DR3SelectionFunctionTCG, fetch_utils.DownloadMixin):
-    """Initialises the model from the all-sky map precomputed in healpix order 7 (Nside=128)."""
+        @ARTICLE{2023A&A...669A..55C,
+               author = {{Cantat-Gaudin}, Tristan and {Fouesneau}, Morgan and {Rix}, Hans-Walter and {Brown}, Anthony G.~A. and {Castro-Ginard}, Alfred and {Kostrzewa-Rutkowska}, Zuzanna and {Drimmel}, Ronald and {Hogg}, David W. and {Casey}, Andrew R. and {Khanna}, Shourya and {Oh}, Semyeong and {Price-Whelan}, Adrian M. and {Belokurov}, Vasily and {Saydjari}, Andrew K. and {Green}, G.},
+                title = "{An empirical model of the Gaia DR3 selection function}",
+              journal = {\aap},
+             keywords = {astrometry, catalogs, methods: data analysis, methods: statistical, Astrophysics - Astrophysics of Galaxies, Astrophysics - Instrumentation and Methods for Astrophysics},
+                 year = 2023,
+                month = jan,
+               volume = {669},
+                  eid = {A55},
+                pages = {A55},
+                  doi = {10.1051/0004-6361/202244784},
+        archivePrefix = {arXiv},
+               eprint = {2208.09335},
+         primaryClass = {astro-ph.GA},
+               adsurl = {https://ui.adsabs.harvard.edu/abs/2023A&A...669A..55C},
+              adsnote = {Provided by the SAO/NASA Astrophysics Data System}
+        }
+    """
 
     datafiles = {
-        "allsky_M10_hpx7.hdf5": "https://github.com/TristanCantatGaudin/GaiaCompleteness/blob/main/allsky_M10_hpx7.hdf5?raw=true"
+        "allsky_M10_hpx7.hdf5": "https://github.com/TristanCantatGaudin/GaiaCompleteness/blob/main/allsky_M10_hpx7.hdf5?raw=true",
+        "allsky_uniq_10.fits": "https://keeper.mpdl.mpg.de/f/c4fb744aa7e941928da6/?dl=1",
     }
 
-    def __init__(self):
-        with h5py.File(self._get_data("allsky_M10_hpx7.hdf5"), "r") as f:
-            m10_order7 = f["data"][()]
-        super().__init__(m10_order7)
+    def __init__(self, mode="hpx7", coord=None, radius=None, min_points=20):
+        self.mode = mode
 
+        if self.mode == "multi":
+            self.m10map = Table.read(self._get_data("allsky_uniq_10.fits"))
+            # For every healpixel large or small, represent it with is first order 29 division.
+            # Once ordered, any sky position can quickly be linked to its nearest healpixel
+            # (which will correspond to the one containing it)
+            max_level = 29
+            level, ipix = ah.uniq_to_level_ipix(self.m10map["UNIQ"])
+            self.index = ipix * (2 ** (max_level - level)) ** 2
+            self.sorter = np.argsort(self.index)
+            self.max_nside = ah.level_to_nside(max_level)
+
+        elif self.mode == "patch":
+            self.coord = coord
+            self.radius_patch = radius
+            self.min_points = min_points
+            # The m10map is not read from a file, we have to build it on the fly:
+            self.m10map = build_patch_map(coord, radius, min_points)
 
-class DR3SelectionFunctionTCG_from_patch(DR3SelectionFunctionTCG):
-    """Initialises the model for a requested patch of sky.
-    The field of view is a square of width 'size' centered on (ra,dec).
-    The spatial resolution will vary across the field of view,
-    from healpix order 6 to 12, enforcing that bins must contain
-    at least min_points sources (default 5). A low number makes the map
-    more detailed but also noisier.
+        else:
+            # Any invalid choice of mode defaults to the healpix 7 map.
+            if mode != "hpx7":
+                print("Mode %s unknown, defaulting to 'hpx7'." % (mode))
+            self.mode = "hpx7"
+            with h5py.File(self._get_data("allsky_M10_hpx7.hdf5"), "r") as f:
+                self.m10map = f["data"][()]
 
-    Args:
-        ra: right ascension of centre of field of view, in degrees
-        dec: declination of centre of field of view, in degrees
-        size: width/height of the field of view, in degrees
-        min_points: minimum number of sources used to compute the map"""
+    def query(self, coords, gmag):
+        """Query the selection function.
 
-    def __init__(self, ra, dec, size, min_points=20):
-        self.ra = ra
-        self.dec = dec
-        self.size = size
-        self.min_points = min_points
-
-        scale = 1.0 / np.cos(np.radians(self.dec))
-
-        queryStringGaia = """SELECT ra, dec, source_id,phot_g_mean_mag
-        FROM gaiadr3.gaia_source
-        WHERE ra>%.3f and ra<%.3f
-        and dec>%.3f and dec<%.3f
-        and astrometric_matched_transits<11
-        and phot_g_mean_mag<50""" % (
-            self.ra - scale * self.size / 2,
-            self.ra + scale * self.size / 2,
-            self.dec - self.size / 2,
-            self.dec + self.size / 2,
-        )
-        print("Querying the Gaia archive...")
-        job = Gaia.launch_job_async(queryStringGaia)
-        GaiaT = job.get_results()
-        print(f"{len(GaiaT)} sources downloaded.")
-
-        # find all the potential hpx ids of queried sources:
-        allHpx6 = sorted(set(GaiaT["source_id"] // (2**35 * 4 ** (12 - 6))))
-        allHpx7 = [
-            foo for i in allHpx6 for foo in [4 * i, 4 * i + 1, 4 * i + 2, 4 * i + 3]
-        ]
-        allHpx8 = [
-            foo for i in allHpx7 for foo in [4 * i, 4 * i + 1, 4 * i + 2, 4 * i + 3]
-        ]
-        allHpx9 = [
-            foo for i in allHpx8 for foo in [4 * i, 4 * i + 1, 4 * i + 2, 4 * i + 3]
-        ]
-        allHpx10 = [
-            foo for i in allHpx9 for foo in [4 * i, 4 * i + 1, 4 * i + 2, 4 * i + 3]
-        ]
-        allHpx11 = [
-            foo for i in allHpx10 for foo in [4 * i, 4 * i + 1, 4 * i + 2, 4 * i + 3]
-        ]
-        allHpx12 = [
-            foo for i in allHpx11 for foo in [4 * i, 4 * i + 1, 4 * i + 2, 4 * i + 3]
-        ]
-        # identify which ones have centers inside the user-requested patch:
-        allGoodHpx12 = []
-        for h in allHpx12:
-            rah, dech = hp.pix2ang(2**12, h, nest=True, lonlat=True)
-            # print(rah,dech)
-            if (
-                rah < self.ra + scale * self.size / 2
-                and rah > self.ra - scale * size / 2
-                and dech < self.dec + size / 2
-                and dech > self.dec - size / 2
-            ):
-                allGoodHpx12.append(h)
-
-        fineMap = [np.nan for foo in allGoodHpx12]
-        for stepUp in range(5):
-            print(f"Grouping the stars by hpx level {12-stepUp}...")
-            sourceHpxThisOrder = np.array(GaiaT["source_id"]) // (
-                2**35 * 4 ** (12 - (12 - stepUp))
+        Args:
+            coords: sky coordinates as an astropy coordinates instance.
+            gmag (float or array): G magnitudes. Should have the same shape as coords.
+
+        Returns:
+            prob: array of selection probabilities.
+        """
+        if not isinstance(coords, SkyCoord):
+            print(
+                "*** WARNING: The coordinates do not seem to be an astropy.coord.SkyCoord object."
+            )
+            print(
+                "This could lead to the error:\n     \"object has no attribute 'frame'\""
             )
-            for i, h in enumerate(allGoodHpx12):
-                if np.isnan(fineMap[i]):
-                    gI = GaiaT["phot_g_mean_mag"][
-                        sourceHpxThisOrder == h // 4**stepUp
-                    ]
-                    # print(i,h,gI); input()
-                    if len(gI) >= min_points:
-                        fineMap[i] = np.median(gI)
-                    else:
-                        pass
-        print("Done.")
-        fineMap = np.array(fineMap)
-        allGoodHpx12 = np.array(allGoodHpx12)
-        order = 12 * np.ones_like(allGoodHpx12)
-        m10_map = np.column_stack((order, allGoodHpx12, fineMap))
-        self.allGoodHpx12 = allGoodHpx12
-        self.fineMap = fineMap
-        super().__init__(m10_map)
-
-    def display(self, G=None):
-        """Uses healpy.gnomview to display the map."""
-        # fill the fullsky map
-        npix = hp.nside2npix(2**12)
-        hpx_map = np.zeros(npix, dtype=float) * np.nan
-        idx = self.allGoodHpx12
-        if G is None:
-            cmap = "turbo"
-            hpx_map[idx] = self.fineMap
+            print(
+                "The syntax to query the completeness map is:\n    mapName.query( coordinates , gmags )"
+            )
+        if self.mode == "multi":
+            ra = coords.ra
+            dec = coords.dec
+            # Determine the NESTED pixel index of the target sky location at that max resolution.
+            match_ipix = ah.lonlat_to_healpix(ra, dec, self.max_nside, order="nested")
+            # Do a binary search for that value:
+            i = self.sorter[
+                np.searchsorted(
+                    self.index, match_ipix, side="right", sorter=self.sorter
+                )
+                - 1
+            ]
+            # That pixel contains the target sky position.
+            allM10 = self.m10map[i]["M10"]
+            prob = m10_to_completeness(gmag.astype(float), allM10)
+            return prob
         else:
-            cmap = "viridis"
-            hpx_map[idx] = m10_to_completeness(G, self.fineMap)
-        hp.gnomview(
-            hpx_map,
-            rot=[self.ra, self.dec],
-            nest=True,
-            xsize=2.1 * 60 * self.size,
-            reso=0.5,
-            cmap=cmap,
+            if coords.shape != np.shape(gmag):
+                raise ValueError(
+                    f"Input shape mismatch: {coords.shape} != {gmag.shape}"
+                )
+            order_map = self.m10map[:, 0].astype(np.int64)
+            ipix_map = self.m10map[:, 1].astype(np.int64)
+            m10_map = self.m10map[:, 2]
+            nside = 2 ** order_map[0]
+            ipix = utils.coord2healpix(coords, "icrs", nside)
+            # if using custom maps, the user might query a point outside the map:
+            is_in_map = np.in1d(ipix, ipix_map)
+            if np.all(is_in_map) == False:
+                print("Warning: some requested points are outside the map.")
+                # print(coords[~is_in_map])
+                # find the missing ipix, temporarily add them with value Nan
+                missingIpix = sorted(set(ipix[~is_in_map]))
+                for mip in missingIpix:
+                    ipix_map = np.append(ipix_map, mip)
+                    m10_map = np.append(m10_map, np.nan)
+            pointIndices = np.array(
+                [np.where(ipix_map == foo)[0][0] for foo in ipix]
+            )  # horrendous but works, could be clearer with np.in1d?
+            allM10 = m10_map[pointIndices]
+            prob = m10_to_completeness(gmag.astype(float), allM10)
+            return prob
+
+
+def build_patch_map(coord, radius, min_points=20):
+    """
+    Query the Gaia database and create a high-resolution healpix map of the M_10
+    parameter for a given circular patch of sky.
+    The pixels without a sufficient number of sources will be grouped together.
+
+    Args:
+        coord (:obj:`astropy.coordinates.SkyCoord`): sky coordinates of the center of the patch, as an astropy SkyCoord object
+        radius (float): the radius of the patch, in degrees
+        min_points (int): minimum number of sources used to compute M_10 in a given pixel.
+            A given region will be subdivided into four higher-order regions
+            if all its subdivisions contain more than min_points points.
+
+    Returns:
+        A numpy array of shape (3,N) where the first column is the order of the maximum resolution reached,
+        the second column is the healpixel number, and the third is the M_10 value in that healpixel.
+    """
+    ra_patch = coord.icrs.ra / u.degree
+    dec_patch = coord.icrs.dec / u.degree
+    print("Querying the Gaia archive...")
+    queryStringGaia = """SELECT ra, dec, source_id,phot_g_mean_mag
+    FROM gaiadr3.gaia_source
+    WHERE 1 = CONTAINS(POINT(ra,dec),CIRCLE(%f, %f, %f))
+    and astrometric_matched_transits<11
+    and phot_g_mean_mag<50""" % (
+        ra_patch,
+        dec_patch,
+        radius,
+    )
+    print(queryStringGaia)
+    job = Gaia.launch_job_async(queryStringGaia)
+    GaiaT = job.get_results()
+    print(f"Obtained {len(GaiaT)} sources.")
+
+    # find all the potential hpx ids of queried sources:
+    allHpx6 = sorted(set(GaiaT["source_id"] // (2**35 * 4 ** (12 - 6))))
+    allHpx7 = [foo for i in allHpx6 for foo in [4 * i, 4 * i + 1, 4 * i + 2, 4 * i + 3]]
+    allHpx8 = [foo for i in allHpx7 for foo in [4 * i, 4 * i + 1, 4 * i + 2, 4 * i + 3]]
+    allHpx9 = [foo for i in allHpx8 for foo in [4 * i, 4 * i + 1, 4 * i + 2, 4 * i + 3]]
+    allHpx10 = [
+        foo for i in allHpx9 for foo in [4 * i, 4 * i + 1, 4 * i + 2, 4 * i + 3]
+    ]
+    allHpx11 = [
+        foo for i in allHpx10 for foo in [4 * i, 4 * i + 1, 4 * i + 2, 4 * i + 3]
+    ]
+    allHpx12 = [
+        foo for i in allHpx11 for foo in [4 * i, 4 * i + 1, 4 * i + 2, 4 * i + 3]
+    ]
+    # identify which ones have centers inside the user-requested patch:
+    allGoodHpx12 = []
+    for h in allHpx12:
+        rah, dech = hp.pix2ang(2**12, h, nest=True, lonlat=True)
+        if coord.separation(SkyCoord(ra=rah, dec=dech, unit="deg")) < u.Quantity(
+            radius, u.deg
+        ):
+            allGoodHpx12.append(h)
+
+    fineMap = [np.nan for foo in allGoodHpx12]
+    for stepUp in range(5):
+        print(f"Grouping the stars by hpx level {12-stepUp}...")
+        sourceHpxThisOrder = np.array(GaiaT["source_id"]) // (
+            2**35 * 4 ** (12 - (12 - stepUp))
         )
-        import matplotlib.pyplot as plt
+        for i, h in enumerate(allGoodHpx12):
+            if np.isnan(fineMap[i]):
+                gI = GaiaT["phot_g_mean_mag"][sourceHpxThisOrder == h // 4**stepUp]
+                # print(i,h,gI); input()
+                if len(gI) >= min_points:
+                    fineMap[i] = np.ma.median(gI)
+                else:
+                    pass
+    print("Done.")
+    fineMap = np.array(fineMap)
+    allGoodHpx12 = np.array(allGoodHpx12)
+    order = 12 * np.ones_like(allGoodHpx12)
+    m10_map = np.column_stack((order, allGoodHpx12, fineMap))
+    return m10_map
 
-        plt.show()
 
+def sigmoid(G, G0, invslope, shape):
+    """Generalized sigmoid function.
 
-def sigmoid(
-    G: np.ndarray, G0: np.ndarray, invslope: np.ndarray, shape: np.ndarray
-) -> np.ndarray:
-    """Generalized sigmoid function
-
-    Parameters
-    ----------
-    G: nd.array
-        where to evaluate the function
-    G0: float
-        inflection point
-    invslope: float
-        steepness of the linear part. Shallower for larger values
-    shape: float
-        if shape=1, model is the classical logistic function,
-        shape converges to zero, then the model is a Gompertz function.
-
-    Returns
-    -------
-    f(G) evaluation of the model.
+    Note: this function is not robust to numerical issues but works within the range of values we feed it.
 
-        FIXME: this function is not robust to numerical issues (but works within the range of values we feed it)
+    Args:
+        G (nd.array): where to evaluate the function
+        G0 (float): inflection point
+        invslope (float): steepness of the linear part. Shallower for larger values
+        shape (float): if shape=1, model is the classical logistic function,
+            shape converges to zero, then the model is a Gompertz function.
+
+    Returns:
+        evaluation of the model f(G) = 1 - (0.5 * (np.tanh(delta / invslope) + 1)) ** shape
     """
     delta = G - G0
     return 1 - (0.5 * (np.tanh(delta / invslope) + 1)) ** shape
 
 
 def m10_to_completeness(G, m10):
     """Predicts the completeness at magnitude G, given a value of M_10 read from a precomputed map.
 
-    Parameters
-    ----------
-    G:   float or nd.array
-                    where to evaluate the function
-    m10: float or nd.array
-                    the value of M_10 in a given region
-
-    Returns
-    -------
-    sf(G) between 0 and 1.
-    The shape of the output will match the input:
-            if given an array (i.e. an array of positions) the output is an array
-            if given an array of Gmag and either one position or a matching array of positions, the output is also an array
-            if only given scalars, the output is one number.
+    Args:
+        G (float or nd.array): where to evaluate the function
+        m10 (float or nd.array): the value of M_10 in a given region
+
+    Returns:
+        sf(G) between 0 and 1.
+        The shape of the output will match the input:
+            * if given an array (i.e. an array of positions) the output is an array
+            * if given an array of Gmag and either one position or a matching array of positions, the output is also an array
+            * if only given scalars, the output is one number.
 
     """
     # These are the best-fit value of the free parameters we optimised in our model:
     ax, bx, cx, ay, by, cy, az, bz, cz, lim = dict(
         ax=0.9848761394197864,
         bx=0.6473155510230146,
         cx=0.6929084598209412,
```

### Comparing `gaiaunlimited-0.1.0/src/gaiaunlimited/utils.py` & `gaiaunlimited-0.2.0/src/gaiaunlimited/utils.py`

 * *Files identical despite different names*

### Comparing `gaiaunlimited-0.1.0/src/gaiaunlimited.egg-info/PKG-INFO` & `gaiaunlimited-0.2.0/src/gaiaunlimited.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaiaunlimited
-Version: 0.1.0
+Version: 0.2.0
 Summary: Tools for manipulating Gaia selection functions.
 Home-page: https://github.com/GaiaUnlimited/gaiaunlimited
 Author: GaiaUnlimited
 Maintainer: Alfred Castro-Ginard, Tristan Cantat-Gaudin
 Maintainer-email: acastro@strw.leidenuniv.nl, cantat@mpia-hd.mpg.de
 Project-URL: Bug Tracker, https://github.com/GaiaUnlimited/gaiaunlimited/issues
 Keywords: astronomy,Gaia,selection function,scanning law
@@ -13,29 +13,30 @@
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Gaiaunlimited
+# gaiaunlimited
 
-Gaiaunlimited is a package for querying and constructing selection functions for the Gaia survey. It is developed by the GaiaUnlimited collaboration.
+[![pypi status](https://img.shields.io/pypi/v/dustapprox.svg)](https://pypi.org/project/dustapprox/)
+[![Documentation Status](https://readthedocs.org/projects/gaiaunlimited/badge/?version=latest)](https://gaiaunlimited.readthedocs.io/en/latest/?badge=latest)
+
+gaiaunlimited is a package for querying and constructing selection functions for the Gaia survey. It is developed by the GaiaUnlimited collaboration.
+
+The documentation for gaiaunlimited is hosted on [Read the docs](https://gaiaunlimited.readthedocs.io/en/latest).
+
+*The [GaiaUnlimited](https://gaia-unlimited.org/) project is funded by the European Union’s Horizon 2020 research and innovation program under grant agreement No 101004110.*
 
 ## Features
 
 - Query Gaia scanning laws for when a given sky position is scanned.
 - Query Gaia survey selection functions for the probabilities that sources of given properties are included in the Gaia catalog.
 - Query ready-made Gaia DR3 subsample selection functions for
 	- the astrometry sample
 	- the RVS sample
 
-## Documentation
-
-[![Documentation Status](https://readthedocs.org/projects/gaiaunlimited/badge/?version=latest)](https://gaiaunlimited.readthedocs.io/en/latest/?badge=latest)
-
-The documentation for gaiaunlimited is hosted on [Read the docs](https://gaiaunlimited.readthedocs.io/en/latest).
-
 ## Acknowledgements
 
 This work is part of the GaiaUnlimited project funded by the European Union’s
 Horizon 2020 research and innovation program under grant agreement No 101004110.
```

