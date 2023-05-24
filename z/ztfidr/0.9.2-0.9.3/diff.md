# Comparing `tmp/ztfidr-0.9.2.tar.gz` & `tmp/ztfidr-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ztfidr-0.9.2.tar", last modified: Mon May 22 15:03:34 2023, max compression
+gzip compressed data, was "ztfidr-0.9.3.tar", last modified: Wed May 24 14:01:56 2023, max compression
```

## Comparing `ztfidr-0.9.2.tar` & `ztfidr-0.9.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-22 15:03:34.557697 ztfidr-0.9.2/
--rwxrwxrwx   0 rigault   (2358) staff       (20)    11357 2022-04-07 08:06:46.000000 ztfidr-0.9.2/LICENSE
--rw-r--r--   0 rigault   (2358) staff       (20)      234 2023-05-22 15:03:34.557515 ztfidr-0.9.2/PKG-INFO
--rwxrwxrwx   0 rigault   (2358) staff       (20)     2186 2022-04-30 12:26:28.000000 ztfidr-0.9.2/README.md
--rw-r--r--   0 rigault   (2358) staff       (20)       38 2023-05-22 15:03:34.557746 ztfidr-0.9.2/setup.cfg
--rwxrwxrwx   0 rigault   (2358) staff       (20)      609 2023-05-22 15:03:14.000000 ztfidr-0.9.2/setup.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-22 15:03:34.556571 ztfidr-0.9.2/ztfidr/
--rwxrwxrwx   0 rigault   (2358) staff       (20)      127 2023-05-22 15:03:09.000000 ztfidr-0.9.2/ztfidr/__init__.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    14854 2023-05-19 12:46:56.000000 ztfidr-0.9.2/ztfidr/io.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    22044 2023-03-20 14:23:14.000000 ztfidr-0.9.2/ztfidr/lightcurve.py
--rw-r--r--   0 rigault   (2358) staff       (20)    18659 2022-11-06 15:43:33.000000 ztfidr-0.9.2/ztfidr/linefitter.py
--rw-r--r--   0 rigault   (2358) staff       (20)     3214 2023-05-22 14:53:09.000000 ztfidr-0.9.2/ztfidr/plotting.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)     1893 2022-04-07 08:06:50.000000 ztfidr-0.9.2/ztfidr/salt2.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    31049 2023-05-15 15:49:11.000000 ztfidr-0.9.2/ztfidr/sample.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)      629 2022-05-02 15:53:23.000000 ztfidr-0.9.2/ztfidr/script.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)     1170 2023-05-15 11:47:44.000000 ztfidr-0.9.2/ztfidr/snid.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    21063 2023-05-15 15:36:52.000000 ztfidr-0.9.2/ztfidr/spectroscopy.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    10043 2022-11-19 14:22:02.000000 ztfidr-0.9.2/ztfidr/target.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    23610 2023-05-22 12:14:03.000000 ztfidr-0.9.2/ztfidr/typing.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)     4034 2023-03-24 07:32:25.000000 ztfidr-0.9.2/ztfidr/utils.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-22 15:03:34.557326 ztfidr-0.9.2/ztfidr.egg-info/
--rwxrwxrwx   0 rigault   (2358) staff       (20)      234 2023-05-22 15:03:34.000000 ztfidr-0.9.2/ztfidr.egg-info/PKG-INFO
--rwxrwxrwx   0 rigault   (2358) staff       (20)      377 2023-05-22 15:03:34.000000 ztfidr-0.9.2/ztfidr.egg-info/SOURCES.txt
--rwxrwxrwx   0 rigault   (2358) staff       (20)        1 2023-05-22 15:03:34.000000 ztfidr-0.9.2/ztfidr.egg-info/dependency_links.txt
--rwxrwxrwx   0 rigault   (2358) staff       (20)        7 2023-05-22 15:03:34.000000 ztfidr-0.9.2/ztfidr.egg-info/top_level.txt
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-24 14:01:56.242895 ztfidr-0.9.3/
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    11357 2022-04-07 08:06:46.000000 ztfidr-0.9.3/LICENSE
+-rw-r--r--   0 rigault   (2358) staff       (20)      234 2023-05-24 14:01:56.242761 ztfidr-0.9.3/PKG-INFO
+-rwxrwxrwx   0 rigault   (2358) staff       (20)     2186 2022-04-30 12:26:28.000000 ztfidr-0.9.3/README.md
+-rw-r--r--   0 rigault   (2358) staff       (20)       38 2023-05-24 14:01:56.242938 ztfidr-0.9.3/setup.cfg
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      609 2023-05-24 14:01:27.000000 ztfidr-0.9.3/setup.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-24 14:01:56.242021 ztfidr-0.9.3/ztfidr/
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      127 2023-05-24 14:01:22.000000 ztfidr-0.9.3/ztfidr/__init__.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    14854 2023-05-19 12:46:56.000000 ztfidr-0.9.3/ztfidr/io.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    22044 2023-03-20 14:23:14.000000 ztfidr-0.9.3/ztfidr/lightcurve.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    18672 2023-05-23 08:15:23.000000 ztfidr-0.9.3/ztfidr/linefitter.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     3434 2023-05-24 12:50:01.000000 ztfidr-0.9.3/ztfidr/plotting.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)     1893 2022-04-07 08:06:50.000000 ztfidr-0.9.3/ztfidr/salt2.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    31049 2023-05-15 15:49:11.000000 ztfidr-0.9.3/ztfidr/sample.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      629 2022-05-02 15:53:23.000000 ztfidr-0.9.3/ztfidr/script.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    10255 2023-05-24 11:57:29.000000 ztfidr-0.9.3/ztfidr/snid.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    21063 2023-05-15 15:36:52.000000 ztfidr-0.9.3/ztfidr/spectroscopy.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    10043 2022-11-19 14:22:02.000000 ztfidr-0.9.3/ztfidr/target.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    23610 2023-05-22 12:14:03.000000 ztfidr-0.9.3/ztfidr/typing.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)     4034 2023-03-24 07:32:25.000000 ztfidr-0.9.3/ztfidr/utils.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-24 14:01:56.242612 ztfidr-0.9.3/ztfidr.egg-info/
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      234 2023-05-24 14:01:56.000000 ztfidr-0.9.3/ztfidr.egg-info/PKG-INFO
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      377 2023-05-24 14:01:56.000000 ztfidr-0.9.3/ztfidr.egg-info/SOURCES.txt
+-rwxrwxrwx   0 rigault   (2358) staff       (20)        1 2023-05-24 14:01:56.000000 ztfidr-0.9.3/ztfidr.egg-info/dependency_links.txt
+-rwxrwxrwx   0 rigault   (2358) staff       (20)        7 2023-05-24 14:01:56.000000 ztfidr-0.9.3/ztfidr.egg-info/top_level.txt
```

### Comparing `ztfidr-0.9.2/LICENSE` & `ztfidr-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ztfidr-0.9.2/README.md` & `ztfidr-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `ztfidr-0.9.2/setup.py` & `ztfidr-0.9.3/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 from distutils.core import setup
 from setuptools import setup, find_packages
 
 
 packages = find_packages()
 
-VERSION = '0.9.2'
+VERSION = '0.9.3'
         
 setup(name='ztfidr',
       version=VERSION,
       description='Tools for ZTF Ia *Internal*DataReleases',
       author='Mickael Rigault',
       author_email='m.rigault@ipnl.in2p3.fr',
       url='https://github.com/MickaelRigault/ztfdr',
```

### Comparing `ztfidr-0.9.2/ztfidr/io.py` & `ztfidr-0.9.3/ztfidr/io.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.9.2/ztfidr/lightcurve.py` & `ztfidr-0.9.3/ztfidr/lightcurve.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.9.2/ztfidr/linefitter.py` & `ztfidr-0.9.3/ztfidr/linefitter.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,14 +79,15 @@
         -------
         (pandas.Series, pandas.DataFrame), figure
             metadata table and results (value, error, cov_)
         """
         if type(spectrum) is str:
             from .spectroscopy import Spectrum
             spectrum = Spectrum.from_filename(spectrum)
+            
         # Loads
         this = cls(spectrum, redshift, lbda_window=lbda_window)
         # Fit        
         params = this.fit(**kwargs)
         # Plot
         if figure:
             fig = this.show_data(show_guess=True,
```

### Comparing `ztfidr-0.9.2/ztfidr/plotting.py` & `ztfidr-0.9.3/ztfidr/plotting.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,40 @@
+import pandas
 import numpy as np
 import matplotlib.pyplot as plt
 
 from . import utils
 
-def show_hubble_standardisation(sample, fig=None,
+def show_hubble_standardisation(sample_or_data, fig=None,
                                 param="c", vmin=-0.2, vmax=0.3, cmap="coolwarm", 
-                                clear_axes=False):
+                                clear_axes=False, bins="auto"):
     """ """
     from astropy.cosmology import Planck18
-    data = sample.get_data(x1_range=[-4,4], c_range=[-0.3,0.8], goodcoverage=True)
-    data = data[data["classification"].isin(['snia-norm'])]
-    
+    if not type(sample_or_data) == pandas.DataFrame:
+        data = sample_or_data.get_data(x1_range=[-4,4], c_range=[-0.3,0.8], goodcoverage=True)
+        data = data[data["classification"].isin(['snia-norm'])]
+    else:
+        data = sample_or_data.copy()
+        
     if fig is None:
         fig = plt.figure(figsize=[6,4])
     
     ax = fig.add_axes([0.1,0.15,0.8,0.75])
     cax = fig.add_axes([0.4,0.3,0.4,0.25])
 
-    mag = -2.5 * np.log10(data["x0"])
+    if "mag" not in data:
+        data["mag"] = -2.5 * np.log10(data["x0"])+19*1.58
+        
     sc = ax.scatter(data["redshift"], 
-                    mag+19*1.58, c=data[param], 
+                    data["mag"], c=data[param], 
                     cmap=cmap,
                     s=10, vmin=vmin, vmax=vmax)
 
-
     _ = utils.hist_colorbar(data[param], ax=cax, cmap=cmap, fcolorbar=0.1,
-                           vmin=vmin, vmax=vmax)
+                           vmin=vmin, vmax=vmax, bins=bins)
 
     xx = np.linspace(0.002,0.23,1000)
     ax.plot(xx, Planck18.distmod(xx), color="k", lw=2)
 
     ax.set_ylabel("distance modulus + cst", fontsize="large")
     ax.set_xlabel("redshift", fontsize="large")
     cax.set_xlabel(f"{param}", fontsize="small", color="0.5")
```

### Comparing `ztfidr-0.9.2/ztfidr/salt2.py` & `ztfidr-0.9.3/ztfidr/salt2.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.9.2/ztfidr/sample.py` & `ztfidr-0.9.3/ztfidr/sample.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.9.2/ztfidr/script.py` & `ztfidr-0.9.3/ztfidr/script.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.9.2/ztfidr/spectroscopy.py` & `ztfidr-0.9.3/ztfidr/spectroscopy.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.9.2/ztfidr/target.py` & `ztfidr-0.9.3/ztfidr/target.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.9.2/ztfidr/typing.py` & `ztfidr-0.9.3/ztfidr/typing.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.9.2/ztfidr/utils.py` & `ztfidr-0.9.3/ztfidr/utils.py`

 * *Files identical despite different names*

