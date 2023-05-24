# Comparing `tmp/cblind-2.2.3.tar.gz` & `tmp/cblind-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cblind-2.2.3.tar", last modified: Tue Nov 30 16:36:13 2021, max compression
+gzip compressed data, was "/home/wafflarg/cblind/dist/.tmp-r19432cn/cblind-2.2.4.tar", last modified: Wed May 24 10:40:27 2023, max compression
```

## Comparing `cblind-2.2.3.tar` & `cblind-2.2.4.tar`

### file list

```diff
@@ -1,19 +1,31 @@
-drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2021-11-30 16:36:13.439910 cblind-2.2.3/
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    35149 2021-02-25 19:20:47.000000 cblind-2.2.3/LICENSE
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     4301 2021-11-30 16:36:13.439910 cblind-2.2.3/PKG-INFO
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     3738 2021-11-30 16:06:46.000000 cblind-2.2.3/README.md
-drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2021-11-30 16:36:13.439910 cblind-2.2.3/cblind/
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)      264 2021-11-24 17:07:18.000000 cblind-2.2.3/cblind/__init__.py
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)       22 2021-11-30 11:15:57.000000 cblind-2.2.3/cblind/__version__.py
--rwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)    26316 2021-11-30 16:15:48.000000 cblind-2.2.3/cblind/cblind.py
-drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2021-11-30 16:36:13.439910 cblind-2.2.3/cblind.egg-info/
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     4301 2021-11-30 16:36:13.000000 cblind-2.2.3/cblind.egg-info/PKG-INFO
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)      295 2021-11-30 16:36:13.000000 cblind-2.2.3/cblind.egg-info/SOURCES.txt
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)        1 2021-11-30 16:36:13.000000 cblind-2.2.3/cblind.egg-info/dependency_links.txt
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)       49 2021-11-30 16:36:13.000000 cblind-2.2.3/cblind.egg-info/entry_points.txt
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)       47 2021-11-30 16:36:13.000000 cblind-2.2.3/cblind.egg-info/requires.txt
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)        7 2021-11-30 16:36:13.000000 cblind-2.2.3/cblind.egg-info/top_level.txt
-drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2021-11-30 16:36:13.439910 cblind-2.2.3/imgs/
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    20566 2021-11-30 15:53:40.000000 cblind-2.2.3/imgs/colormaps.png
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)      768 2021-11-30 16:36:13.439910 cblind-2.2.3/setup.cfg
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)       38 2021-10-04 21:13:09.000000 cblind-2.2.3/setup.py
+drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2023-05-24 10:40:27.870053 cblind-2.2.4/
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    35149 2021-02-25 19:20:47.000000 cblind-2.2.4/LICENSE
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     5145 2023-05-24 10:40:27.870053 cblind-2.2.4/PKG-INFO
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     4590 2023-05-24 10:28:42.000000 cblind-2.2.4/README.md
+drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2023-05-24 10:40:27.866053 cblind-2.2.4/cblind/
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)      264 2023-05-24 10:25:37.000000 cblind-2.2.4/cblind/__init__.py
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)       22 2023-05-24 10:28:36.000000 cblind-2.2.4/cblind/__version__.py
+-rwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)    26291 2023-05-24 10:28:22.000000 cblind-2.2.4/cblind/cblind.py
+drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2023-05-24 10:40:27.866053 cblind-2.2.4/cblind.egg-info/
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     5145 2023-05-24 10:40:27.000000 cblind-2.2.4/cblind.egg-info/PKG-INFO
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)      506 2023-05-24 10:40:27.000000 cblind-2.2.4/cblind.egg-info/SOURCES.txt
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)        1 2023-05-24 10:40:27.000000 cblind-2.2.4/cblind.egg-info/dependency_links.txt
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)       48 2023-05-24 10:40:27.000000 cblind-2.2.4/cblind.egg-info/entry_points.txt
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)       47 2023-05-24 10:40:27.000000 cblind-2.2.4/cblind.egg-info/requires.txt
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)        7 2023-05-24 10:40:27.000000 cblind-2.2.4/cblind.egg-info/top_level.txt
+drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2023-05-24 10:40:27.870053 cblind-2.2.4/imgs/
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    12412 2021-12-01 14:02:06.000000 cblind-2.2.4/imgs/bird.png
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    17820 2021-12-01 14:02:06.000000 cblind-2.2.4/imgs/cblind.png
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    20566 2021-11-30 15:53:40.000000 cblind-2.2.4/imgs/colormaps.png
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)      619 2021-12-01 14:02:06.000000 cblind-2.2.4/imgs/colormaps.py
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     9126 2021-12-01 14:02:06.000000 cblind-2.2.4/imgs/contrast.png
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    26606 2021-12-01 14:02:06.000000 cblind-2.2.4/imgs/extreme_rainbow.png
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    49866 2021-12-01 14:02:06.000000 cblind-2.2.4/imgs/huescale.png
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     1454 2021-12-01 14:02:06.000000 cblind-2.2.4/imgs/huescale.py
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    23133 2021-12-01 14:02:06.000000 cblind-2.2.4/imgs/monocolor.png
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    12215 2021-12-01 14:02:06.000000 cblind-2.2.4/imgs/pregunta.png
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    17609 2021-12-01 14:02:06.000000 cblind-2.2.4/imgs/rainbow.png
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    15675 2021-12-01 14:02:06.000000 cblind-2.2.4/imgs/rbscale.png
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    15832 2021-12-01 14:02:06.000000 cblind-2.2.4/imgs/solstice.png
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     1009 2023-05-24 10:36:38.000000 cblind-2.2.4/pyproject.toml
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)       38 2023-05-24 10:40:27.870053 cblind-2.2.4/setup.cfg
```

### Comparing `cblind-2.2.3/LICENSE` & `cblind-2.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cblind-2.2.3/PKG-INFO` & `cblind-2.2.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: cblind
-Version: 2.2.3
+Version: 2.2.4
 Summary: Color schemes for Python plots, from Paul Tol (2012)
-Home-page: https://github.com/volodia99/cblind
 Author: G. Wafflard-Fernandez
 License: GPL-3.0
-Platform: UNKNOWN
+Project-URL: Homepage, https://github.com/volodia99/cblind
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-# colorblind
+# cblind
+[![PyPI](https://img.shields.io/pypi/v/cblind)](https://pypi.org/project/cblind/)
 
-A colorblind-friendly python module that allows optimal color choice for plotting multiple curves  
+A colorblind-friendly python module that allows color choice for plotting multiple curves  
 Works only with python 3  
-3 optimal colormaps are now available to map 2D fields  
-Version: 2.2.2
+8 colormaps are now available to map 2D fields  
+Version: 2.2.4
 Author: Gaylor Wafflard-Fernandez  
 Author-email: gaylor.wafflard@univ-grenoble-alpes.fr
 
 ## Installation
 
 Install with `pip`
 
@@ -50,134 +50,154 @@
 
 from 1 to 12 plots [DISTINCT COLORS]. For more than 12 plots, the linestyle is changed.  
 
 ```python
 cb.test_cblind(nb_of_plots)
 ```
 
+![cblind](https://github.com/Volodia99/cblind/raw/master/imgs/cblind.png)
+
 ### contrast
 
 ```python
 color, linestyle = cb.Coloplots().contrast(nb_of_plots)
 ```
 
 for less than 4 contrast plots [DISTINCT COLORS]. For more than 12 plots, the linestyle is changed.  
 
 ```python
 cb.test_contrast(nb_of_plots)
 ```
 
+![contrast](https://github.com/Volodia99/cblind/raw/master/imgs/contrast.png)
+
 ### huescale
 
 ```python
 color, linestyle = cb.Coloplots().huescale(nb_of_plots, *option)
 ```
 
 from 1 to 9 plots [SEQUENTIAL DATA]. With option "blue","bluegreen","green", "gold","brown","rose","purple" for less than 3 plots, otherwise ocherscale.  
 
 ```python
 cb.test_huescale(nb_of_plots, *option)
 ```
 
+![huescale](https://github.com/Volodia99/cblind/raw/master/imgs/huescale.png)
+
 ### rbscale
 
 ```python
 color, linestyle = cb.Coloplots().rbscale(nb_of_plots)
 ```
 
 from 3 to 11 plots [DIVERGING DATA].  
 
 ```python
 cb.test_rbscale(nb_of_plots)
 ```
 
+![rbscale](https://github.com/Volodia99/cblind/raw/master/imgs/rbscale.png)
+
 ### rainbow
 
 ```python
 color, linestyle = cb.Coloplots().rainbow(nb_of_plots)
 ```
 
 from 4 to 12 plots [RAINBOW SCHEME].  
 
 ```python
 cb.test_rainbow(nb_of_plots)
 ```
 
+![rainbow](https://github.com/Volodia99/cblind/raw/master/imgs/rainbow.png)
+
 ### extreme_rainbow
 
 ```python
 color, linestyle = cb.Coloplots().extreme_rainbow(nb_of_plots)
 ```
 
 from 1 to 34 plots [RAINBOW SCHEME].  
 
 ```python
 cb.test_extreme_rainbow(nb_of_plots)
 ```
 
+![extreme_rainbow](https://github.com/Volodia99/cblind/raw/master/imgs/extreme_rainbow.png)
+
 ### solstice
 
 ```python
 color, linestyle = cb.Coloplots().solstice(nb_of_plots)
 ```
 
 for less than 11 plots [DIVERGING DATA]  
 
 ```python
 cb.test_solstice(nb_of_plots)
 ```
 
+![solstice](https://github.com/Volodia99/cblind/raw/master/imgs/solstice.png)
+
 ### bird
 
 ```python
 color, linestyle = cb.Coloplots().bird(nb_of_plots)
 ```
 
 for less than 9 plots [DIVERGING DATA]  
 
 ```python
 cb.test_bird(nb_of_plots)
 ```
 
+![bird](https://github.com/Volodia99/cblind/raw/master/imgs/bird.png)
+
 ### pregunta
 
 ```python
 color, linestyle = cb.Coloplots().pregunta(nb_of_plots)
 ```
 
 for less than 9 plots [DIVERGING DATA]  
 
 ```python
 cb.test_pregunta(nb_of_plots)
 ```
 
+![pregunta](https://github.com/Volodia99/cblind/raw/master/imgs/pregunta.png)
+
 ### monocolor
 
 ```python
 color, linestyle = cb.Coloplots().monocolor(nb_of_plots, *option)
 ```
 
 from 1 to 13 monochromatic plots [MONOCOLOR/PRINTING] with different linestyles. With option "b&w", "blue", "red", "yellow", "green", "purple".
 
 ```python
 cb.test_monocolor(nb_of_plots, *option)
 ```
 
+![monocolor](https://github.com/Volodia99/cblind/raw/master/imgs/monocolor.png)
+
 ## Usage for colormaps
 
 8 cblind palettes are available for now : "cb.rbscale", "cb.rainbow", "cb.extreme_rainbow", "cb.huescale", 
 "cb.solstice", "cb.bird", "cb.pregunta", "cb.iris", but also all colormaps from matplotlib + "\_r" variants for reverse colormaps.  
 
 ```python
 cmap = cb.cbmap(palette, nbin)
 ```
 
 The `nbin` argument is used to discretize the colormaps.  
 
-![Colormaps](https://github.com/Volodia99/cblind/raw/master/imgs/colormaps.png)
+![colormaps](https://github.com/Volodia99/cblind/raw/master/imgs/colormaps.png)
 
 To test the colormaps, you can try:
 
 ```python
 cb.test_mapping(palette, nbin)
 ```
 
@@ -199,9 +219,7 @@
 ```python
 cb.mapping(fig,ax,data2d,extent,palette=palette,nbin=nbin)
 ```
 
 **REFERENCE**  
 Paul Tol. 2012. "Colour Schemes." SRON Technical Note, SRON/EPS/TN/09-002.  
 https://personal.sron.nl/~pault/data/colourschemes.pdf
-
-
```

### Comparing `cblind-2.2.3/README.md` & `cblind-2.2.4/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-# colorblind
+# cblind
+[![PyPI](https://img.shields.io/pypi/v/cblind)](https://pypi.org/project/cblind/)
 
-A colorblind-friendly python module that allows optimal color choice for plotting multiple curves  
+A colorblind-friendly python module that allows color choice for plotting multiple curves  
 Works only with python 3  
-3 optimal colormaps are now available to map 2D fields  
-Version: 2.2.2
+8 colormaps are now available to map 2D fields  
+Version: 2.2.4
 Author: Gaylor Wafflard-Fernandez  
 Author-email: gaylor.wafflard@univ-grenoble-alpes.fr
 
 ## Installation
 
 Install with `pip`
 
@@ -33,134 +34,154 @@
 
 from 1 to 12 plots [DISTINCT COLORS]. For more than 12 plots, the linestyle is changed.  
 
 ```python
 cb.test_cblind(nb_of_plots)
 ```
 
+![cblind](https://github.com/Volodia99/cblind/raw/master/imgs/cblind.png)
+
 ### contrast
 
 ```python
 color, linestyle = cb.Coloplots().contrast(nb_of_plots)
 ```
 
 for less than 4 contrast plots [DISTINCT COLORS]. For more than 12 plots, the linestyle is changed.  
 
 ```python
 cb.test_contrast(nb_of_plots)
 ```
 
+![contrast](https://github.com/Volodia99/cblind/raw/master/imgs/contrast.png)
+
 ### huescale
 
 ```python
 color, linestyle = cb.Coloplots().huescale(nb_of_plots, *option)
 ```
 
 from 1 to 9 plots [SEQUENTIAL DATA]. With option "blue","bluegreen","green", "gold","brown","rose","purple" for less than 3 plots, otherwise ocherscale.  
 
 ```python
 cb.test_huescale(nb_of_plots, *option)
 ```
 
+![huescale](https://github.com/Volodia99/cblind/raw/master/imgs/huescale.png)
+
 ### rbscale
 
 ```python
 color, linestyle = cb.Coloplots().rbscale(nb_of_plots)
 ```
 
 from 3 to 11 plots [DIVERGING DATA].  
 
 ```python
 cb.test_rbscale(nb_of_plots)
 ```
 
+![rbscale](https://github.com/Volodia99/cblind/raw/master/imgs/rbscale.png)
+
 ### rainbow
 
 ```python
 color, linestyle = cb.Coloplots().rainbow(nb_of_plots)
 ```
 
 from 4 to 12 plots [RAINBOW SCHEME].  
 
 ```python
 cb.test_rainbow(nb_of_plots)
 ```
 
+![rainbow](https://github.com/Volodia99/cblind/raw/master/imgs/rainbow.png)
+
 ### extreme_rainbow
 
 ```python
 color, linestyle = cb.Coloplots().extreme_rainbow(nb_of_plots)
 ```
 
 from 1 to 34 plots [RAINBOW SCHEME].  
 
 ```python
 cb.test_extreme_rainbow(nb_of_plots)
 ```
 
+![extreme_rainbow](https://github.com/Volodia99/cblind/raw/master/imgs/extreme_rainbow.png)
+
 ### solstice
 
 ```python
 color, linestyle = cb.Coloplots().solstice(nb_of_plots)
 ```
 
 for less than 11 plots [DIVERGING DATA]  
 
 ```python
 cb.test_solstice(nb_of_plots)
 ```
 
+![solstice](https://github.com/Volodia99/cblind/raw/master/imgs/solstice.png)
+
 ### bird
 
 ```python
 color, linestyle = cb.Coloplots().bird(nb_of_plots)
 ```
 
 for less than 9 plots [DIVERGING DATA]  
 
 ```python
 cb.test_bird(nb_of_plots)
 ```
 
+![bird](https://github.com/Volodia99/cblind/raw/master/imgs/bird.png)
+
 ### pregunta
 
 ```python
 color, linestyle = cb.Coloplots().pregunta(nb_of_plots)
 ```
 
 for less than 9 plots [DIVERGING DATA]  
 
 ```python
 cb.test_pregunta(nb_of_plots)
 ```
 
+![pregunta](https://github.com/Volodia99/cblind/raw/master/imgs/pregunta.png)
+
 ### monocolor
 
 ```python
 color, linestyle = cb.Coloplots().monocolor(nb_of_plots, *option)
 ```
 
 from 1 to 13 monochromatic plots [MONOCOLOR/PRINTING] with different linestyles. With option "b&w", "blue", "red", "yellow", "green", "purple".
 
 ```python
 cb.test_monocolor(nb_of_plots, *option)
 ```
 
+![monocolor](https://github.com/Volodia99/cblind/raw/master/imgs/monocolor.png)
+
 ## Usage for colormaps
 
 8 cblind palettes are available for now : "cb.rbscale", "cb.rainbow", "cb.extreme_rainbow", "cb.huescale", 
 "cb.solstice", "cb.bird", "cb.pregunta", "cb.iris", but also all colormaps from matplotlib + "\_r" variants for reverse colormaps.  
 
 ```python
 cmap = cb.cbmap(palette, nbin)
 ```
 
 The `nbin` argument is used to discretize the colormaps.  
 
-![Colormaps](https://github.com/Volodia99/cblind/raw/master/imgs/colormaps.png)
+![colormaps](https://github.com/Volodia99/cblind/raw/master/imgs/colormaps.png)
 
 To test the colormaps, you can try:
 
 ```python
 cb.test_mapping(palette, nbin)
 ```
```

### Comparing `cblind-2.2.3/cblind/cblind.py` & `cblind-2.2.4/cblind/cblind.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import sys
 from cycler import cycler
 
 import numpy as np
 import scipy.special as ss
 import matplotlib.pyplot as plt
 from matplotlib import colors as mcolors
-from matplotlib import cm
 
 from rich import print as rprint
 
 PALETTES = ("cb.rbscale", "cb.rainbow", "cb.huescale", "cb.solstice", "cb.bird", "cb.pregunta", "cb.iris", "cb.extreme_rainbow")
 PALETTES_FULL = (*PALETTES,*tuple([i+"_r" for i in PALETTES]))
 
 STYLES = {
@@ -493,15 +492,15 @@
         cbcmap = mcolors.LinearSegmentedColormap.from_list(f"{palette_tmp}", cmap_iris, N=nbin)
     if palette[-2:]=="_r":
         cbcmap = reversed_cmap(cbcmap, name=f"{palette}_r", nbin=nbin)
     return(cbcmap)
 
 def cbmap(palette=None, nbin=None):
     if palette not in PALETTES_FULL:
-        palette = cm.get_cmap(palette, nbin)
+        palette = plt.get_cmap(palette, nbin)
     else:
         palette = _get_cbmap(palette, nbin)
     return palette
 
 def mapping(fig, ax, data2d, palette=None, nbin=None):
     im=ax.imshow(data2d, cmap=cbmap(palette=palette, nbin=nbin), aspect='auto')
     fig.colorbar(im)
```

### Comparing `cblind-2.2.3/cblind.egg-info/PKG-INFO` & `cblind-2.2.4/cblind.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: cblind
-Version: 2.2.3
+Version: 2.2.4
 Summary: Color schemes for Python plots, from Paul Tol (2012)
-Home-page: https://github.com/volodia99/cblind
 Author: G. Wafflard-Fernandez
 License: GPL-3.0
-Platform: UNKNOWN
+Project-URL: Homepage, https://github.com/volodia99/cblind
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-# colorblind
+# cblind
+[![PyPI](https://img.shields.io/pypi/v/cblind)](https://pypi.org/project/cblind/)
 
-A colorblind-friendly python module that allows optimal color choice for plotting multiple curves  
+A colorblind-friendly python module that allows color choice for plotting multiple curves  
 Works only with python 3  
-3 optimal colormaps are now available to map 2D fields  
-Version: 2.2.2
+8 colormaps are now available to map 2D fields  
+Version: 2.2.4
 Author: Gaylor Wafflard-Fernandez  
 Author-email: gaylor.wafflard@univ-grenoble-alpes.fr
 
 ## Installation
 
 Install with `pip`
 
@@ -50,134 +50,154 @@
 
 from 1 to 12 plots [DISTINCT COLORS]. For more than 12 plots, the linestyle is changed.  
 
 ```python
 cb.test_cblind(nb_of_plots)
 ```
 
+![cblind](https://github.com/Volodia99/cblind/raw/master/imgs/cblind.png)
+
 ### contrast
 
 ```python
 color, linestyle = cb.Coloplots().contrast(nb_of_plots)
 ```
 
 for less than 4 contrast plots [DISTINCT COLORS]. For more than 12 plots, the linestyle is changed.  
 
 ```python
 cb.test_contrast(nb_of_plots)
 ```
 
+![contrast](https://github.com/Volodia99/cblind/raw/master/imgs/contrast.png)
+
 ### huescale
 
 ```python
 color, linestyle = cb.Coloplots().huescale(nb_of_plots, *option)
 ```
 
 from 1 to 9 plots [SEQUENTIAL DATA]. With option "blue","bluegreen","green", "gold","brown","rose","purple" for less than 3 plots, otherwise ocherscale.  
 
 ```python
 cb.test_huescale(nb_of_plots, *option)
 ```
 
+![huescale](https://github.com/Volodia99/cblind/raw/master/imgs/huescale.png)
+
 ### rbscale
 
 ```python
 color, linestyle = cb.Coloplots().rbscale(nb_of_plots)
 ```
 
 from 3 to 11 plots [DIVERGING DATA].  
 
 ```python
 cb.test_rbscale(nb_of_plots)
 ```
 
+![rbscale](https://github.com/Volodia99/cblind/raw/master/imgs/rbscale.png)
+
 ### rainbow
 
 ```python
 color, linestyle = cb.Coloplots().rainbow(nb_of_plots)
 ```
 
 from 4 to 12 plots [RAINBOW SCHEME].  
 
 ```python
 cb.test_rainbow(nb_of_plots)
 ```
 
+![rainbow](https://github.com/Volodia99/cblind/raw/master/imgs/rainbow.png)
+
 ### extreme_rainbow
 
 ```python
 color, linestyle = cb.Coloplots().extreme_rainbow(nb_of_plots)
 ```
 
 from 1 to 34 plots [RAINBOW SCHEME].  
 
 ```python
 cb.test_extreme_rainbow(nb_of_plots)
 ```
 
+![extreme_rainbow](https://github.com/Volodia99/cblind/raw/master/imgs/extreme_rainbow.png)
+
 ### solstice
 
 ```python
 color, linestyle = cb.Coloplots().solstice(nb_of_plots)
 ```
 
 for less than 11 plots [DIVERGING DATA]  
 
 ```python
 cb.test_solstice(nb_of_plots)
 ```
 
+![solstice](https://github.com/Volodia99/cblind/raw/master/imgs/solstice.png)
+
 ### bird
 
 ```python
 color, linestyle = cb.Coloplots().bird(nb_of_plots)
 ```
 
 for less than 9 plots [DIVERGING DATA]  
 
 ```python
 cb.test_bird(nb_of_plots)
 ```
 
+![bird](https://github.com/Volodia99/cblind/raw/master/imgs/bird.png)
+
 ### pregunta
 
 ```python
 color, linestyle = cb.Coloplots().pregunta(nb_of_plots)
 ```
 
 for less than 9 plots [DIVERGING DATA]  
 
 ```python
 cb.test_pregunta(nb_of_plots)
 ```
 
+![pregunta](https://github.com/Volodia99/cblind/raw/master/imgs/pregunta.png)
+
 ### monocolor
 
 ```python
 color, linestyle = cb.Coloplots().monocolor(nb_of_plots, *option)
 ```
 
 from 1 to 13 monochromatic plots [MONOCOLOR/PRINTING] with different linestyles. With option "b&w", "blue", "red", "yellow", "green", "purple".
 
 ```python
 cb.test_monocolor(nb_of_plots, *option)
 ```
 
+![monocolor](https://github.com/Volodia99/cblind/raw/master/imgs/monocolor.png)
+
 ## Usage for colormaps
 
 8 cblind palettes are available for now : "cb.rbscale", "cb.rainbow", "cb.extreme_rainbow", "cb.huescale", 
 "cb.solstice", "cb.bird", "cb.pregunta", "cb.iris", but also all colormaps from matplotlib + "\_r" variants for reverse colormaps.  
 
 ```python
 cmap = cb.cbmap(palette, nbin)
 ```
 
 The `nbin` argument is used to discretize the colormaps.  
 
-![Colormaps](https://github.com/Volodia99/cblind/raw/master/imgs/colormaps.png)
+![colormaps](https://github.com/Volodia99/cblind/raw/master/imgs/colormaps.png)
 
 To test the colormaps, you can try:
 
 ```python
 cb.test_mapping(palette, nbin)
 ```
 
@@ -199,9 +219,7 @@
 ```python
 cb.mapping(fig,ax,data2d,extent,palette=palette,nbin=nbin)
 ```
 
 **REFERENCE**  
 Paul Tol. 2012. "Colour Schemes." SRON Technical Note, SRON/EPS/TN/09-002.  
 https://personal.sron.nl/~pault/data/colourschemes.pdf
-
-
```

### Comparing `cblind-2.2.3/imgs/colormaps.png` & `cblind-2.2.4/imgs/colormaps.png`

 * *Files identical despite different names*

