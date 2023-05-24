# Comparing `tmp/ngspice-tools-0.0.1.tar.gz` & `tmp/ngspice-tools-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngspice-tools-0.0.1.tar", last modified: Wed May  3 13:09:42 2023, max compression
+gzip compressed data, was "ngspice-tools-0.0.2.tar", last modified: Wed May 24 03:03:01 2023, max compression
```

## Comparing `ngspice-tools-0.0.1.tar` & `ngspice-tools-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 nabla     (1000) nabla     (1000)        0 2023-05-03 13:09:42.760951 ngspice-tools-0.0.1/
--rw-r--r--   0 nabla     (1000) nabla     (1000)      597 2023-05-03 13:09:42.760951 ngspice-tools-0.0.1/PKG-INFO
--rw-r--r--   0 nabla     (1000) nabla     (1000)      103 2023-05-03 13:09:26.000000 ngspice-tools-0.0.1/README.rst
-drwxr-xr-x   0 nabla     (1000) nabla     (1000)        0 2023-05-03 13:09:42.760951 ngspice-tools-0.0.1/ngspice_tools/
--rw-rw-r--   0 nabla     (1000) nabla     (1000)       22 2023-05-03 12:39:40.000000 ngspice-tools-0.0.1/ngspice_tools/__init__.py
--rw-rw-r--   0 nabla     (1000) nabla     (1000)     1568 2023-05-03 12:45:33.000000 ngspice-tools-0.0.1/ngspice_tools/ngspice_input.py
--rw-rw-r--   0 nabla     (1000) nabla     (1000)     2186 2023-05-03 12:41:08.000000 ngspice-tools-0.0.1/ngspice_tools/plot_colors.py
--rw-rw-r--   0 nabla     (1000) nabla     (1000)     2072 2023-05-03 12:53:30.000000 ngspice-tools-0.0.1/ngspice_tools/plot_sim.py
-drwxr-xr-x   0 nabla     (1000) nabla     (1000)        0 2023-05-03 13:09:42.760951 ngspice-tools-0.0.1/ngspice_tools.egg-info/
--rw-r--r--   0 nabla     (1000) nabla     (1000)      597 2023-05-03 13:09:42.000000 ngspice-tools-0.0.1/ngspice_tools.egg-info/PKG-INFO
--rw-r--r--   0 nabla     (1000) nabla     (1000)      365 2023-05-03 13:09:42.000000 ngspice-tools-0.0.1/ngspice_tools.egg-info/SOURCES.txt
--rw-r--r--   0 nabla     (1000) nabla     (1000)        1 2023-05-03 13:09:42.000000 ngspice-tools-0.0.1/ngspice_tools.egg-info/dependency_links.txt
--rw-r--r--   0 nabla     (1000) nabla     (1000)       64 2023-05-03 13:09:42.000000 ngspice-tools-0.0.1/ngspice_tools.egg-info/entry_points.txt
--rw-r--r--   0 nabla     (1000) nabla     (1000)       23 2023-05-03 13:09:42.000000 ngspice-tools-0.0.1/ngspice_tools.egg-info/requires.txt
--rw-r--r--   0 nabla     (1000) nabla     (1000)       14 2023-05-03 13:09:42.000000 ngspice-tools-0.0.1/ngspice_tools.egg-info/top_level.txt
--rw-r--r--   0 nabla     (1000) nabla     (1000)     1052 2023-05-03 13:09:42.764284 ngspice-tools-0.0.1/setup.cfg
--rw-r--r--   0 nabla     (1000) nabla     (1000)       38 2023-05-03 12:49:54.000000 ngspice-tools-0.0.1/setup.py
+drwxr-xr-x   0 nabla     (1000) nabla     (1000)        0 2023-05-24 03:03:01.778493 ngspice-tools-0.0.2/
+-rw-r--r--   0 nabla     (1000) nabla     (1000)      597 2023-05-24 03:03:01.778493 ngspice-tools-0.0.2/PKG-INFO
+-rw-r--r--   0 nabla     (1000) nabla     (1000)      103 2023-05-03 13:09:26.000000 ngspice-tools-0.0.2/README.rst
+drwxr-xr-x   0 nabla     (1000) nabla     (1000)        0 2023-05-24 03:03:01.778493 ngspice-tools-0.0.2/ngspice_tools/
+-rw-rw-r--   0 nabla     (1000) nabla     (1000)       22 2023-05-24 03:02:54.000000 ngspice-tools-0.0.2/ngspice_tools/__init__.py
+-rw-rw-r--   0 nabla     (1000) nabla     (1000)     3086 2023-05-19 08:16:56.000000 ngspice-tools-0.0.2/ngspice_tools/ngspice_input.py
+-rw-rw-r--   0 nabla     (1000) nabla     (1000)     2150 2023-05-19 10:18:29.000000 ngspice-tools-0.0.2/ngspice_tools/plot_colors.py
+-rw-rw-r--   0 nabla     (1000) nabla     (1000)     2465 2023-05-19 08:26:14.000000 ngspice-tools-0.0.2/ngspice_tools/plot_sim.py
+drwxr-xr-x   0 nabla     (1000) nabla     (1000)        0 2023-05-24 03:03:01.778493 ngspice-tools-0.0.2/ngspice_tools.egg-info/
+-rw-r--r--   0 nabla     (1000) nabla     (1000)      597 2023-05-24 03:03:01.000000 ngspice-tools-0.0.2/ngspice_tools.egg-info/PKG-INFO
+-rw-r--r--   0 nabla     (1000) nabla     (1000)      365 2023-05-24 03:03:01.000000 ngspice-tools-0.0.2/ngspice_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 nabla     (1000) nabla     (1000)        1 2023-05-24 03:03:01.000000 ngspice-tools-0.0.2/ngspice_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 nabla     (1000) nabla     (1000)       64 2023-05-24 03:03:01.000000 ngspice-tools-0.0.2/ngspice_tools.egg-info/entry_points.txt
+-rw-r--r--   0 nabla     (1000) nabla     (1000)       23 2023-05-24 03:03:01.000000 ngspice-tools-0.0.2/ngspice_tools.egg-info/requires.txt
+-rw-r--r--   0 nabla     (1000) nabla     (1000)       14 2023-05-24 03:03:01.000000 ngspice-tools-0.0.2/ngspice_tools.egg-info/top_level.txt
+-rw-r--r--   0 nabla     (1000) nabla     (1000)     1052 2023-05-24 03:03:01.778493 ngspice-tools-0.0.2/setup.cfg
+-rw-r--r--   0 nabla     (1000) nabla     (1000)       38 2023-05-03 12:49:54.000000 ngspice-tools-0.0.2/setup.py
```

### Comparing `ngspice-tools-0.0.1/PKG-INFO` & `ngspice-tools-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngspice-tools
-Version: 0.0.1
+Version: 0.0.2
 Summary: Command line tool to help plot various ascii ngspice outputs
 Author: Alexander Becker
 Author-email: a.becker@cern.ch
 License: GPL3
 Keywords: signals,science,electronics,visualization
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `ngspice-tools-0.0.1/ngspice_tools/plot_colors.py` & `ngspice-tools-0.0.2/ngspice_tools/plot_colors.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """
 Store constants that define color cycles for the plots
 """
-PALETTS = {'blue-green': ['navy',
-                          'blue',
-                          'royalblue',
+PALETTS = {'blue-green': ['blue',
                           'dodgerblue',
-                          'deepskyblue',
-                          'darkturquoise',
-                          'turquoise',
-                          'aqua',
-                          'aquamarine'],
+                          'lightskyblue',
+                          'cyan',
+                          'lightseagreen',
+                          'mediumspringgreen',
+                          'lawngreen',
+                          'lime'],
            'green-yellow': ['darkgreen',
                             'green',
                             'limegreen',
                             'lime',
                             'lawngreen',
                             'greenyellow',
                             'yellowgreen',
@@ -24,15 +23,15 @@
                           'coral',
                           'orangered',
                           'red',
                           'darkorange',
                           'orange',
                           'gold',
                           'goldenrod'],
-           'green-blue-magenta': ['limegreen',
+           'green-blue-magenta': ['lime',
                                   'springgreen',
                                   'mediumspringgreen',
                                   'aquamarine',
                                   'aqua',
                                   'deepskyblue',
                                   'dodgerblue',
                                   'royalblue',
```

### Comparing `ngspice-tools-0.0.1/ngspice_tools/plot_sim.py` & `ngspice-tools-0.0.2/ngspice_tools/plot_sim.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,18 +36,27 @@
                  width: float, height: float,
                  dark: bool, colors: str, filetype: str):
     """
     Plot the variables in an ascii formatted ngspice ouptut file
     """
     if dark:
         plt.style.use('dark_background')
-    colors = cycle(PALETTS[colors])
-    title, _, simvars = parse_ngspice_sim_output(infile)
+    clrs = cycle(PALETTS[colors])
+    plot_type, title, _, simvars = parse_ngspice_sim_output(infile)
     fig, axes = plt.subplots(figsize=(width, height))
     axes.set_title(title)
     axes.set_xlabel(simvars[0]['type'] + " " + simvars[0]['unit'])
     axes.set_ylabel(simvars[1]['type'] + " " + simvars[1]['unit'])
-    for v in simvars[1:]:
-        axes.plot(simvars[0]['data'], v['data'],
-                  label=v['name'], color=next(colors))
+    match plot_type:
+        case "tran":
+            for v in simvars[1:]:
+                axes.plot(simvars[0]['data'], v['data'],
+                          label=v['name'], color=next(clrs))
+        case "ac":
+            axes.set_xscale('log')
+            for v in simvars[1:]:
+                xdata = list(map(lambda x: x[0], simvars[0]['data']))
+                ydata = list(map(lambda x: x[0], v['data']))
+                axes.plot(xdata, ydata,
+                          label=v['name'], color=next(clrs))
     fig.legend(bbox_to_anchor=(0.98, 0.8), title="Signals")
     fig.savefig(output + "." + filetype)
```

### Comparing `ngspice-tools-0.0.1/ngspice_tools.egg-info/PKG-INFO` & `ngspice-tools-0.0.2/ngspice_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngspice-tools
-Version: 0.0.1
+Version: 0.0.2
 Summary: Command line tool to help plot various ascii ngspice outputs
 Author: Alexander Becker
 Author-email: a.becker@cern.ch
 License: GPL3
 Keywords: signals,science,electronics,visualization
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `ngspice-tools-0.0.1/setup.cfg` & `ngspice-tools-0.0.2/setup.cfg`

 * *Files identical despite different names*

