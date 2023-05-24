# Comparing `tmp/seaduck-0.1.0.tar.gz` & `tmp/seaduck-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seaduck-0.1.0.tar", last modified: Wed May  3 20:06:37 2023, max compression
+gzip compressed data, was "seaduck-0.1.2.tar", last modified: Wed May 24 18:15:12 2023, max compression
```

## Comparing `seaduck-0.1.0.tar` & `seaduck-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,80 @@
-drwxrwxr-x   0 wjiang33  (1001) wjiang33  (1001)        0 2023-05-03 20:06:37.616243 seaduck-0.1.0/
--rw-rw-r--   0 wjiang33  (1001) wjiang33  (1001)     1070 2023-04-20 18:20:06.000000 seaduck-0.1.0/LICENSE
--rw-rw-r--   0 wjiang33  (1001) wjiang33  (1001)       35 2023-04-20 18:20:06.000000 seaduck-0.1.0/MANIFEST.in
--rw-rw-r--   0 wjiang33  (1001) wjiang33  (1001)      295 2023-05-03 20:06:37.612243 seaduck-0.1.0/PKG-INFO
-drwxrwxr-x   0 wjiang33  (1001) wjiang33  (1001)        0 2023-05-03 20:06:37.612243 seaduck-0.1.0/seaduck/
--rw-rw-r--   0 wjiang33  (1001) wjiang33  (1001)    14244 2023-05-02 21:50:14.000000 seaduck-0.1.0/seaduck/OceData.py
--rw-rw-r--   0 wjiang33  (1001) wjiang33  (1001)     4613 2023-05-02 21:50:26.000000 seaduck-0.1.0/seaduck/OceInterp.py
--rw-rw-r--   0 wjiang33  (1001) wjiang33  (1001)      104 2023-04-20 18:20:06.000000 seaduck-0.1.0/seaduck/RuntimeConf.py
--rw-rw-r--   0 wjiang33  (1001) wjiang33  (1001)      269 2023-05-02 21:59:05.000000 seaduck-0.1.0/seaduck/__init__.py
--rw-rw-r--   0 wjiang33  (1001) wjiang33  (1001)    62331 2023-05-02 21:50:28.000000 seaduck-0.1.0/seaduck/eulerian.py
--rw-rw-r--   0 wjiang33  (1001) wjiang33  (1001)     7733 2023-05-02 21:50:29.000000 seaduck-0.1.0/seaduck/get_masks.py
--rw-rw-r--   0 wjiang33  (1001) wjiang33  (1001)    40496 2023-05-02 21:50:33.000000 seaduck-0.1.0/seaduck/kernelNweight.py
--rw-rw-r--   0 wjiang33  (1001) wjiang33  (1001)    49641 2023-05-02 21:50:32.000000 seaduck-0.1.0/seaduck/lagrangian.py
--rw-rw-r--   0 wjiang33  (1001) wjiang33  (1001)     2811 2023-04-27 18:24:17.000000 seaduck-0.1.0/seaduck/smart_read.py
--rw-rw-r--   0 wjiang33  (1001) wjiang33  (1001)    23595 2023-05-02 21:50:30.000000 seaduck-0.1.0/seaduck/topology.py
--rw-rw-r--   0 wjiang33  (1001) wjiang33  (1001)    51737 2023-04-27 19:06:44.000000 seaduck-0.1.0/seaduck/utils.py
-drwxrwxr-x   0 wjiang33  (1001) wjiang33  (1001)        0 2023-05-03 20:06:37.612243 seaduck-0.1.0/seaduck.egg-info/
--rw-rw-r--   0 wjiang33  (1001) wjiang33  (1001)      295 2023-05-03 20:06:37.000000 seaduck-0.1.0/seaduck.egg-info/PKG-INFO
--rw-rw-r--   0 wjiang33  (1001) wjiang33  (1001)      382 2023-05-03 20:06:37.000000 seaduck-0.1.0/seaduck.egg-info/SOURCES.txt
--rw-rw-r--   0 wjiang33  (1001) wjiang33  (1001)        1 2023-05-03 20:06:37.000000 seaduck-0.1.0/seaduck.egg-info/dependency_links.txt
--rw-rw-r--   0 wjiang33  (1001) wjiang33  (1001)        8 2023-05-03 20:06:37.000000 seaduck-0.1.0/seaduck.egg-info/top_level.txt
--rw-rw-r--   0 wjiang33  (1001) wjiang33  (1001)       38 2023-05-03 20:06:37.616243 seaduck-0.1.0/setup.cfg
--rw-rw-r--   0 wjiang33  (1001) wjiang33  (1001)      331 2023-05-03 19:16:51.000000 seaduck-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:15:12.265813 seaduck-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:15:12.257813 seaduck-0.1.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-24 18:14:57.000000 seaduck-0.1.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:15:12.257813 seaduck-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-05-24 18:14:57.000000 seaduck-0.1.2/.github/workflows/on-push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-24 18:14:57.000000 seaduck-0.1.2/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     7160 2023-05-24 18:14:57.000000 seaduck-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-24 18:14:57.000000 seaduck-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-05-24 18:14:57.000000 seaduck-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-24 18:14:57.000000 seaduck-0.1.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    14920 2023-05-24 18:15:12.265813 seaduck-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-24 18:14:57.000000 seaduck-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:15:12.257813 seaduck-0.1.2/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-24 18:14:57.000000 seaduck-0.1.2/ci/environment-ci.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:15:12.257813 seaduck-0.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    10550 2023-05-24 18:14:57.000000 seaduck-0.1.2/docs/AVISO.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11545 2023-05-24 18:14:57.000000 seaduck-0.1.2/docs/Global_ECCO.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-24 18:14:57.000000 seaduck-0.1.2/docs/_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-24 18:14:57.000000 seaduck-0.1.2/docs/_toc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-24 18:14:57.000000 seaduck-0.1.2/docs/all_in_one.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:15:12.257813 seaduck-0.1.2/docs/api_reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-24 18:14:57.000000 seaduck-0.1.2/docs/api_reference/apiref_OceData.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-24 18:14:57.000000 seaduck-0.1.2/docs/api_reference/apiref_OceInterp.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-24 18:14:57.000000 seaduck-0.1.2/docs/api_reference/apiref_eulerian.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-24 18:14:57.000000 seaduck-0.1.2/docs/api_reference/apiref_getmasks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-24 18:14:57.000000 seaduck-0.1.2/docs/api_reference/apiref_kernelNweight.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-24 18:14:57.000000 seaduck-0.1.2/docs/api_reference/apiref_lagrangian.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-24 18:14:57.000000 seaduck-0.1.2/docs/api_reference/apiref_smartread.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-24 18:14:57.000000 seaduck-0.1.2/docs/api_reference/apiref_topology.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-24 18:14:57.000000 seaduck-0.1.2/docs/api_reference/apiref_utils.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:15:12.261813 seaduck-0.1.2/docs/contribute/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-24 18:14:57.000000 seaduck-0.1.2/docs/contribute/contr_cod.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6414 2023-05-24 18:14:57.000000 seaduck-0.1.2/docs/contribute/contr_doc.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-24 18:14:57.000000 seaduck-0.1.2/docs/contribute/prep_env.md
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-24 18:14:57.000000 seaduck-0.1.2/docs/contribute/tidyNpr.md
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-24 18:14:57.000000 seaduck-0.1.2/docs/contribute/use_git.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-24 18:14:57.000000 seaduck-0.1.2/docs/how_to_install.md
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-24 18:14:57.000000 seaduck-0.1.2/docs/intro.md
+-rw-r--r--   0 runner    (1001) docker     (123)   577233 2023-05-24 18:14:57.000000 seaduck-0.1.2/docs/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-24 18:14:57.000000 seaduck-0.1.2/docs/network_of_object.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-05-24 18:14:57.000000 seaduck-0.1.2/docs/notebooks.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-24 18:14:57.000000 seaduck-0.1.2/docs/reference.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5524 2023-05-24 18:14:57.000000 seaduck-0.1.2/docs/references.bib
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-24 18:14:57.000000 seaduck-0.1.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:15:12.261813 seaduck-0.1.2/docs/sciserver_notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-05-24 18:14:57.000000 seaduck-0.1.2/docs/sciserver_notebooks/IGP.md
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-24 18:14:57.000000 seaduck-0.1.2/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-05-24 18:14:57.000000 seaduck-0.1.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:15:12.261813 seaduck-0.1.2/seaduck/
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-24 18:14:57.000000 seaduck-0.1.2/seaduck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48174 2023-05-24 18:14:57.000000 seaduck-0.1.2/seaduck/eulerian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-05-24 18:14:57.000000 seaduck-0.1.2/seaduck/get_masks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28319 2023-05-24 18:14:57.000000 seaduck-0.1.2/seaduck/kernel_weight.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37779 2023-05-24 18:14:57.000000 seaduck-0.1.2/seaduck/lagrangian.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14341 2023-05-24 18:14:57.000000 seaduck-0.1.2/seaduck/ocedata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-05-24 18:14:57.000000 seaduck-0.1.2/seaduck/oceinterp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-24 18:14:57.000000 seaduck-0.1.2/seaduck/runtime_conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-05-24 18:14:57.000000 seaduck-0.1.2/seaduck/smart_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23085 2023-05-24 18:14:57.000000 seaduck-0.1.2/seaduck/topology.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21854 2023-05-24 18:14:57.000000 seaduck-0.1.2/seaduck/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-24 18:15:12.000000 seaduck-0.1.2/seaduck/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:15:12.261813 seaduck-0.1.2/seaduck.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14920 2023-05-24 18:15:12.000000 seaduck-0.1.2/seaduck.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-24 18:15:12.000000 seaduck-0.1.2/seaduck.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 18:15:12.000000 seaduck-0.1.2/seaduck.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-24 18:15:12.000000 seaduck-0.1.2/seaduck.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-24 18:15:12.000000 seaduck-0.1.2/seaduck.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 18:15:12.265813 seaduck-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:15:12.265813 seaduck-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 18:14:57.000000 seaduck-0.1.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-24 18:14:57.000000 seaduck-0.1.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-05-24 18:14:57.000000 seaduck-0.1.2/tests/test_eulerian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-24 18:14:57.000000 seaduck-0.1.2/tests/test_get_masks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-05-24 18:14:57.000000 seaduck-0.1.2/tests/test_lagrangian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-05-24 18:14:57.000000 seaduck-0.1.2/tests/test_ocedata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-05-24 18:14:57.000000 seaduck-0.1.2/tests/test_oceinterp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-24 18:14:57.000000 seaduck-0.1.2/tests/test_smart_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7574 2023-05-24 18:14:57.000000 seaduck-0.1.2/tests/test_topology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-05-24 18:14:57.000000 seaduck-0.1.2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-05-24 18:14:57.000000 seaduck-0.1.2/tests/test_weight.py
```

### Comparing `seaduck-0.1.0/seaduck/OceInterp.py` & `seaduck-0.1.2/seaduck/oceinterp.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,116 +1,137 @@
-from seaduck.lagrangian import particle,uknw,vknw
-from seaduck.eulerian import position
-from seaduck.OceData import OceData
-from seaduck.kernelNweight import KnW
+import warnings
 
 import numpy as np
-import warnings
 
-lagrange_token = '__particle.'
+from seaduck.eulerian import position
+from seaduck.kernel_weight import KnW
+from seaduck.lagrangian import particle, uknw, vknw
+from seaduck.ocedata import OceData
+
+lagrange_token = "__particle."
+
+
+def OceInterp(
+    od,
+    varList,
+    x,
+    y,
+    z,
+    t,
+    kernelList=None,
+    lagrangian=False,
+    lagrange_kwarg={},
+    update_stops="default",
+    return_in_between=True,
+    return_pt_time=True,
+    kernel_kwarg={},
+):
+    """Interp for people who just want to take a quick look.
 
-def OceInterp(od,varList,x,y,z,t,
-              kernelList = None,
-              lagrangian = False,
-              lagrange_kwarg = {},
-              update_stops = 'default',
-              return_in_between  =True,
-              return_pt_time = True,
-              **kernel_kwarg):
-    '''
-    **This is the centerpiece function of the package, through which you can access almost all of its functionality.**
+    **This is the centerpiece function of the package, through which
+    you can access almost all of its functionality.**.
 
     **Parameters:**
 
     + od: OceInterp.OceData object or xarray.Dataset (limited support for netCDF Dataset)
         The dataset to work on.
     + varList: str or list
         A list of variable or pair of variables.
     + kernelList: OceInterp.KnW or list of OceInterp.KnW objects
         Indicates which kernel to use for each interpolation.
     + x, y, z: numpy.ndarray
-        The location of the particles, where x and y are in degrees, and z is in meters (deeper locations are represented by more negative values).
+        The location of the particles, where x and y are in degrees,
+        and z is in meters (deeper locations are represented by more negative values).
     + t: numpy.ndarray
-        In the Eulerian scheme, this represents the time of interpolation. In the Lagrangian scheme, it represents the time needed for output. 
+        In the Eulerian scheme, this represents the time of interpolation.
+        In the Lagrangian scheme, it represents the time needed for output.
     + lagrangian: bool
         Specifies whether the interpolation is done in the Eulerian or Lagrangian scheme.
     + lagrange_kwarg: dict
         Keyword arguments passed into the OceInterp.lagrangian.particle object.
     + update_stops: None, 'default', or iterable of float
         Specifies the time to update the prefetch velocity.
     + return_in_between: bool
-        In Lagrangian mode, this returns the interpolation not only at time t, but also at every point in time when the speed is updated.
+        In Lagrangian mode, this returns the interpolation not only at time t,
+        but also at every point in time when the speed is updated.
     + return_pt_time: bool
         Specifies whether to return the time of all the steps.
-    '''
-    if not isinstance(od,OceData):
+    + kernel_kwarg: dict
+        keyword arguments to pass into seaduck.KnW object.
+    """
+    if not isinstance(od, OceData):
         od = OceData(od)
 
-    if isinstance(varList,dict):
+    if isinstance(varList, dict):
         kernelList = list(varList.values())
-        varList    = list(varList.keys())
+        varList = list(varList.keys())
         print(f"result will be in the order of {varList}")
-    elif isinstance(varList,str):
+    elif isinstance(varList, str):
         varList = [varList]
-    elif isinstance(varList,tuple):
+    elif isinstance(varList, tuple):
         varList = [varList]
-    elif isinstance(varList,list):
+    elif isinstance(varList, list):
         pass
     else:
         raise ValueError("varList type not recognized.")
-
-    if isinstance(kernelList,list):
+    if isinstance(kernelList, list):
         pass
     elif kernelList is None:
         kernelList = []
         the_kernel = KnW(**kernel_kwarg)
         for i in varList:
-            if isinstance(i,str):
+            if isinstance(i, str):
                 kernelList.append(the_kernel)
-            elif isinstance(i,tuple):
+            elif isinstance(i, tuple):
                 if kernel_kwarg != dict():
-                    kernelList.append((the_kernel,the_kernel))
+                    kernelList.append((the_kernel, the_kernel))
                 else:
-                    kernelList.append((uknw,vknw))
+                    kernelList.append((uknw, vknw))
             else:
                 raise ValueError("varList need to be made up of string or tuples")
     if not lagrangian:
         pt = position()
-        pt.from_latlon(x = x,y=y,z=z,t=t,data = od)
-        for i,var in enumerate(varList):
+        pt.from_latlon(x=x, y=y, z=z, t=t, data=od)
+        for i, var in enumerate(varList):
             if lagrange_token in var:
-                raise AttributeError('__particle variables is only available for Lagrangian particles')
-        R = pt.interpolate(varList,kernelList)
+                raise AttributeError(
+                    "__particle variables is only available for Lagrangian particles"
+                )
+        R = pt.interpolate(varList, kernelList)
         return R
-            
+
     else:
         try:
-            assert len(t)>1
+            assert len(t) > 1
         except AssertionError:
-            raise Exception('There needs to be at least two time steps to run the lagrangian particle')
+            raise ValueError(
+                "There needs to be at least two time steps to run the lagrangian particle"
+            )
         t_start = t[0]
         t_nec = t[1:]
-        pt = particle(x = x,y=y,z=z,t=np.ones_like(x)*t_start,data = od,**lagrange_kwarg)
-        stops,raw = pt.to_list_of_time(t_nec,
-                                       update_stops = update_stops,
-                                       return_in_between = return_in_between)
+        pt = particle(
+            x=x, y=y, z=z, t=np.ones_like(x) * t_start, data=od, **lagrange_kwarg
+        )
+        stops, raw = pt.to_list_of_time(
+            t_nec, update_stops=update_stops, return_in_between=return_in_between
+        )
         R = []
-        for i,var in enumerate(varList):
-            if var == lagrange_token+'raw':
+        for i, var in enumerate(varList):
+            if var == lagrange_token + "raw":
                 R.append(raw)
             elif lagrange_token in var:
                 sublist = []
                 for snap in raw:
-                    sublist.append(snap.__dict__[var[len(lagrange_token):]])
+                    sublist.append(snap.__dict__[var[len(lagrange_token) :]])
                 R.append(sublist)
             else:
                 sublist = []
                 for snap in raw:
-                    sublist.append(snap.interpolate(var,kernelList[i]))
+                    sublist.append(snap.interpolate(var, kernelList[i]))
                 R.append(sublist)
-                
+
         if return_pt_time:
-            return stops,R
+            return stops, R
         else:
             if return_in_between:
-                warnings.warn('Some of the returns is not on the times you specified.')
-            return R
+                warnings.warn("Some of the returns is not on the times you specified.")
+            return R
```

### Comparing `seaduck-0.1.0/seaduck/eulerian.py` & `seaduck-0.1.2/seaduck/eulerian.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,1543 +1,1291 @@
-from seaduck.OceData import OceData
-from seaduck.kernelNweight import KnW,_translate_to_tendency,find_pk_4d
+import copy
+
+import numpy as np
+
+from seaduck.get_masks import get_masked
+from seaduck.kernel_weight import KnW, _translate_to_tendency, find_pk_4d
+from seaduck.ocedata import OceData
+
 # from OceInterp.kernel_and_weight import _translate_to_tendency,find_pk_4d
 from seaduck.smart_read import smart_read as sread
-from seaduck.get_masks import get_masked
-from seaduck.utils import local_to_latlon,get_key_by_value,_general_len,local_to_latlon,to_180,get_combination,find_px_py,weight_f_node
+from seaduck.utils import (
+    _general_len,
+    find_px_py,
+    get_key_by_value,
+    local_to_latlon,
+    weight_f_node,
+)
 
-import warnings
-import numpy as np
-import copy
 
-# def to_180(x):
-#     '''
-#     convert any longitude scale to [-180,180)
-#     '''
-#     x = x%360
-#     return x+(-1)*(x//180)*360
-
-# def local_to_latlon(u,v,cs,sn):
-#     '''convert local vector to north-east '''
-#     uu = u*cs-v*sn
-#     vv = u*sn+v*cs
-#     return uu,vv
-
-# def get_combination(lst,select):
-#     '''
-#     Iteratively find all the combination that
-#     has (select) amount of elements
-#     and every element belongs to lst
-#     This is the same as the one in itertools, 
-#     but I didn't know at the time.
-#     '''
-#     n = len(lst)
-#     if select==1:
-#         return [[num] for num in lst]
-#     else:
-#         the_lst = []
-#         for i,num in enumerate(lst):
-#             sub_lst = get_combination(lst[i+1:],select-1)
-#             for com in sub_lst:
-#                 com.append(num)
-# #             print(sub_lst)
-#             the_lst+=sub_lst
-#         return the_lst
-    
-def _ind_broadcast(x,ind):
-    '''
-    Perform a "cartesian product" on two fattened dimensions 
+def _ind_broadcast(x, ind):
+    """Perform a "cartesian product" on two fattened dimensions.
 
     **Parameters:**
-    
+
     + x: numpy.ndarray
         A new dimension
     + ind: tuple
         Existing indexes
-    '''
+    """
     n = x.shape[0]
-    if len(x.shape) ==1:
-        x = x.reshape((n,1))
+    if len(x.shape) == 1:
+        x = x.reshape((n, 1))
     xsp = x.shape
     ysp = ind[0].shape
-    final_shape = [n]+list(ysp[1:])+list(xsp[1:])
-    
-    R = [np.zeros(final_shape,int) for i in range(len(ind)+1)]
-    
+    final_shape = [n] + list(ysp[1:]) + list(xsp[1:])
+
+    R = [np.zeros(final_shape, int) for i in range(len(ind) + 1)]
+
     dims = len(final_shape)
-    ydim = len(ysp)-1
-    trsp = list(range(1,1+ydim))+[0]+list(range(1+ydim,dims))
-    inv  = np.argsort(trsp)
+    ydim = len(ysp) - 1
+    trsp = list(range(1, 1 + ydim)) + [0] + list(range(1 + ydim, dims))
+    inv = np.argsort(trsp)
     R[0] = R[0].transpose(trsp)
     R[0][:] = x
     R[0] = R[0].transpose(inv)
-    
-    for i in range(1,len(ind)+1):
+
+    for i in range(1, len(ind) + 1):
         R[i] = R[i].T
-        R[i][:] = ind[i-1].T
+        R[i][:] = ind[i - 1].T
         R[i] = R[i].T
     return R
 
+
 def _partial_flatten(ind):
-    '''
-    Converting a high dimensional index set to a 2D one
-    '''
-    if isinstance(ind,tuple):
+    """Convert a high dimensional index set to a 2D one."""
+    if isinstance(ind, tuple):
         shape = ind[0].shape
-        
+
         # num_neighbor = 1
         # for i in range(1,len(shape)):
         #     num_neighbor*=shape[i]
         R = []
         for i in range(len(ind)):
-            R.append(ind[i].reshape(shape[0],-1))
+            R.append(ind[i].reshape(shape[0], -1))
         return tuple(R)
-    elif isinstance(ind,np.ndarray):
+    elif isinstance(ind, np.ndarray):
         shape = ind.shape
-        
         num_neighbor = 1
-        for i in range(1,len(shape)):
-            num_neighbor*=shape[i]
-        return ind.reshape(shape[0],num_neighbor)
-    
-def _in_required(name,required):
-    '''
-    see if a name is in required. 
-    '''
-    if required == 'all':
+        for i in range(1, len(shape)):
+            num_neighbor *= shape[i]
+        return ind.reshape(shape[0], num_neighbor)
+
+
+def _in_required(name, required):
+    """See if a name is in required."""
+    if required == "all":
         return True
     else:
         return name in required
-    
-def _ind_for_mask(ind,dims):
-    '''
+
+
+def _ind_for_mask(ind, dims):
+    """Find the index for masking.
+
     If dims does not include a vertical dimension, assume to be 0.
-    If dims has a temporal dimension, take it away. 
-    Return the index for masking. 
-    '''
-    ind_for_mask = [ind[i] for i in range(len(ind)) if dims[i] not in ['time']]
-    if 'Z' not in dims and 'Zl' not in dims:
-        ind_for_mask.insert(0,np.zeros_like(ind[0]))
+    If dims has a temporal dimension, take it away.
+    Return the index for masking.
+    """
+    ind_for_mask = [ind[i] for i in range(len(ind)) if dims[i] not in ["time"]]
+    if "Z" not in dims and "Zl" not in dims:
+        ind_for_mask.insert(0, np.zeros_like(ind[0]))
     return tuple(ind_for_mask)
 
-def _subtract_i_min(ind,i_min):
-    '''
-    Subtract the index prefix from the actual index. 
+
+def _subtract_i_min(ind, i_min):
+    """Subtract the index prefix from the actual index.
+
     This is used when one is reading from a prefetched subset of the data.
-    '''
+    """
     temp_ind = []
     for i in range(len(i_min)):
-        temp_ind.append(ind[i]-i_min[i])
+        temp_ind.append(ind[i] - i_min[i])
     return tuple(temp_ind)
 
-class position():
-    '''
-    The position object that performs the interpolation.
-    Create a empty one by default. 
-    To actually do interpolation, use from_latlon method to tell the ducks where they are. 
-    '''
-#     self.ind_h_dict = {}
-    def from_latlon(self,x = None,y = None,z = None,t = None,data = None):
-        '''
-        Use the methods from the ocedata to transform 
+
+class position:
+    """The position object that performs the interpolation.
+
+    Create a empty one by default.
+    To actually do interpolation, use from_latlon method to tell the ducks where they are.
+    """
+
+    #     self.ind_h_dict = {}
+    def from_latlon(self, x=None, y=None, z=None, t=None, data=None):
+        """Fill in the coord info using lat-lon-dep-time dims.
+
+        Use the methods from the ocedata to transform
         from lat-lon-dep-time coords to rel-coords
-        store the output in the position object. 
+        store the output in the position object.
 
         **Parameters:**
-        
+
         + x,y,z,t: numpy.ndarray
             1D array of the lat-lon-dep-time coords
         + data: OceData object
-            The field where the positions are defined on. 
-        '''
+            The field where the positions are defined on.
+        """
         if data is None:
             try:
                 self.ocedata
             except AttributeError:
-                raise ValueError('data not provided')
+                raise ValueError("data not provided")
         else:
-            self.ocedata = data
+            if isinstance(data, OceData):
+                self.ocedata = data
+            else:
+                raise ValueError("Input data must be OceData")
         self.tp = self.ocedata.tp
-        length = [_general_len(i) for i in [x,y,z,t]]
+        length = [_general_len(i) for i in [x, y, z, t]]
         self.N = max(length)
-        if any([i!= self.N for i in length if i>1]):
-            raise ValueError('Shapes of input coordinates are not compatible')
-        
-        if isinstance(x,float):
-            x = np.array([1.0])*x
-        if isinstance(y,float):
-            y = np.array([1.0])*y
-        if isinstance(z,float):
-            z = np.array([1.0])*z
-        if isinstance(z,float):
-            t = np.array([1.0])*t
-        
-        for thing in [x,y,z,t]:
-            if len(x.shape)>1:
-                raise ValueError('Input need to be 1D numpy arrays')
+        if any([i != self.N for i in length if i > 1]):
+            raise ValueError("Shapes of input coordinates are not compatible")
+
+        if isinstance(x, float):
+            x = np.array([1.0]) * x
+        if isinstance(y, float):
+            y = np.array([1.0]) * y
+        if isinstance(z, float):
+            z = np.array([1.0]) * z
+        if isinstance(t, float):
+            t = np.array([1.0]) * t
+
+        for thing in [x, y, z, t]:
+            if len(x.shape) > 1:
+                raise ValueError("Input need to be 1D numpy arrays")
         if (x is not None) and (y is not None):
             self.lon = x
             self.lat = y
             (
-                 self.face,
-                 self.iy,
-                 self.ix,
-                 self.rx,
-                 self.ry,
-                 self.cs,
-                 self.sn,
-                 self.dx,
-                 self.dy,
-                 self.bx,
-                 self.by
-            ) = self.ocedata.find_rel_h(x,y)
+                self.face,
+                self.iy,
+                self.ix,
+                self.rx,
+                self.ry,
+                self.cs,
+                self.sn,
+                self.dx,
+                self.dy,
+                self.bx,
+                self.by,
+            ) = self.ocedata.find_rel_h(x, y)
         else:
-            self.lon  = None
-            self.lat  = None
+            self.lon = None
+            self.lat = None
             self.face = None
-            self.iy   = None
-            self.ix   = None
-            self.rx   = None
-            self.ry   = None
-            self.cs   = None
-            self.sn   = None
-            self.dx   = None
-            self.dy   = None
-            self.bx   = None
-            self.by   = None
-        if (z is not None):
+            self.iy = None
+            self.ix = None
+            self.rx = None
+            self.ry = None
+            self.cs = None
+            self.sn = None
+            self.dx = None
+            self.dy = None
+            self.bx = None
+            self.by = None
+        if z is not None:
             self.dep = z
-            if (self.ocedata.readiness['Z']):
-                (
-                    self.iz,
-                    self.rz,
-                    self.dz,
-                    self.bz 
-                ) = self.ocedata.find_rel_v(z)
+            if self.ocedata.readiness["Z"]:
+                (self.iz, self.rz, self.dz, self.bz) = self.ocedata.find_rel_v(z)
             else:
                 (
                     self.iz,
                     self.rz,
                     self.dz,
                     self.bz,
-                ) = [None for i in range(4)]
-            if (self.ocedata.readiness['Zl']):
-                (
-                    self.izl,
-                    self.rzl,
-                    self.dzl,
-                    self.bzl 
-                ) = self.ocedata.find_rel_vl(z)
+                ) = (None for i in range(4))
+            if self.ocedata.readiness["Zl"]:
+                (self.izl, self.rzl, self.dzl, self.bzl) = self.ocedata.find_rel_vl(z)
             else:
                 (
                     self.izl,
                     self.rzl,
                     self.dzl,
                     self.bzl,
-                ) = [None for i in range(4)]
+                ) = (None for i in range(4))
         else:
             (
                 self.iz,
                 self.rz,
                 self.dz,
                 self.bz,
                 self.izl,
                 self.rzl,
                 self.dzl,
                 self.bzl,
-                self.dep
-            ) = [None for i in range(9)]
-            
-        if (t is not None):
+                self.dep,
+            ) = (None for i in range(9))
+
+        if t is not None:
             self.t = t
-            if self.ocedata.readiness['time']:
-                (
-                    self.it,
-                    self.rt,
-                    self.dt,
-                    self.bt 
-                ) = self.ocedata.find_rel_t(t)
+            if self.ocedata.readiness["time"]:
+                (self.it, self.rt, self.dt, self.bt) = self.ocedata.find_rel_t(t)
             else:
                 (
                     self.it,
                     self.rt,
                     self.dt,
                     self.bt,
-                ) = [None for i in range(4)]
+                ) = (None for i in range(4))
         else:
-            (
-                self.it,
-                self.rt,
-                self.dt,
-                self.bt,
-                self.t
-            ) = [None for i in range(5)]
+            (self.it, self.rt, self.dt, self.bt, self.t) = (None for i in range(5))
         return self
-    
-    def subset(self,which):
-        '''
-        Create a subset of the position object
+
+    def subset(self, which):
+        """Create a subset of the position object.
 
         **Parameters:**
-        
+
         + which: numpy.ndarray
             Define which points survive the subset operation.
             It be an array of either boolean or int.
             The selection is similar to that of selecting from a 1D numpy array.
 
         **Returns:**
-        
+
         + the_subset: position object
-            The selected positions. 
-        '''
+            The selected positions.
+        """
         p = position()
         keys = self.__dict__.keys()
         for i in keys:
             item = self.__dict__[i]
-            if isinstance(item,np.ndarray):
-                if len(item.shape) ==1:
+            if isinstance(item, np.ndarray):
+                if len(item.shape) == 1:
                     p.__dict__[i] = item[which]
                     p.N = len(p.__dict__[i])
                 else:
                     p.__dict__[i] = item
             else:
                 p.__dict__[i] = item
         # p.N = max([_general_len(i) for i in p.__dict__.values()])
         return p
-        
-    def fatten_h(self,knw,ind_moves_kwarg = {}):
-        '''
+
+    def fatten_h(self, knw, ind_moves_kwarg={}):
+        """Fatten horizontal indices.
+
         Fatten means to find the neighboring points of the points of interest based on the kernel.
-        faces,iys,ixs are 1d arrays of size n. 
+        faces,iys,ixs are 1d arrays of size n.
         We are applying a kernel of size m.
-        This is going to return a n * m array of indexes. 
-        A very slim vector is now a matrix, and hence the name. 
+        This is going to return a n * m array of indexes.
+        A very slim vector is now a matrix, and hence the name.
         each row represen all the node needed for interpolation of a single point.
-        "h" represent we are only doing it on the horizontal plane
+        "h" represent we are only doing it on the horizontal plane.
 
         **Parameters:**
-        
+
         + knw: KnW object
             The kernel used to find neighboring points.
         + ind_moves_kward: dict
-            Key word argument to put into ind_moves method of the topology object. 
-            Read topology.ind_moves for more detail. 
-        '''
-#         self.ind_h_dict
+            Key word argument to put into ind_moves method of the topology object.
+            Read topology.ind_moves for more detail.
+        """
+        #         self.ind_h_dict
         kernel = knw.kernel
-        kernel_tends =  [_translate_to_tendency(k) for k in kernel]
+        kernel_tends = [_translate_to_tendency(k) for k in kernel]
         m = len(kernel_tends)
         n = len(self.iy)
         tp = self.ocedata.tp
 
-        # the arrays we are going to return 
+        # the arrays we are going to return
         if self.face is not None:
-            n_faces = np.zeros((n,m))
+            n_faces = np.zeros((n, m))
             n_faces.T[:] = self.face
-        n_iys = np.zeros((n,m))
-        n_ixs = np.zeros((n,m))
+        n_iys = np.zeros((n, m))
+        n_ixs = np.zeros((n, m))
 
         # first try to fatten it naively(fast and vectorized)
-        for i,node in enumerate(kernel):
-            x_disp,y_disp = node
-            n_iys[:,i] = self.iy+y_disp
-            n_ixs[:,i] = self.ix+x_disp
+        for i, node in enumerate(kernel):
+            x_disp, y_disp = node
+            n_iys[:, i] = self.iy + y_disp
+            n_ixs[:, i] = self.ix + x_disp
         if self.face is not None:
-            illegal = tp.check_illegal((n_faces,n_iys,n_ixs))
+            illegal = tp.check_illegal((n_faces, n_iys, n_ixs))
         else:
-            illegal = tp.check_illegal((n_iys,n_ixs))
+            illegal = tp.check_illegal((n_iys, n_ixs))
 
         redo = np.array(np.where(illegal)).T
-        for num,loc in enumerate(redo):
-            j,i = loc
+        for num, loc in enumerate(redo):
+            j, i = loc
             if self.face is not None:
-                ind = (self.face[j],self.iy[j],self.ix[j])
+                ind = (self.face[j], self.iy[j], self.ix[j])
             else:
-                ind = (self.iy[j],self.ix[j])
+                ind = (self.iy[j], self.ix[j])
             # everyone start from the [0,0] node
             moves = kernel_tends[i]
             # moves is a list of operations to get to a single point
-            #[2,2] means move to the left and then move to the left again.
-            n_ind = tp.ind_moves(ind,moves,**ind_moves_kwarg)
+            # [2,2] means move to the left and then move to the left again.
+            n_ind = tp.ind_moves(ind, moves, **ind_moves_kwarg)
             if self.face is not None:
-                n_faces[j,i],n_iys[j,i],n_ixs[j,i] = n_ind
+                n_faces[j, i], n_iys[j, i], n_ixs[j, i] = n_ind
             else:
-                n_iys[j,i],n_ixs[j,i] = n_ind
+                n_iys[j, i], n_ixs[j, i] = n_ind
         if self.face is not None:
-            return n_faces.astype('int'),n_iys.astype('int'),n_ixs.astype('int')
+            return n_faces.astype("int"), n_iys.astype("int"), n_ixs.astype("int")
         else:
-            return None,n_iys.astype('int'),n_ixs.astype('int')
-        
-    def fatten_v(self,knw):
-        '''
-        Finding the neighboring center grid points in the vertical direction.
+            return None, n_iys.astype("int"), n_ixs.astype("int")
+
+    def fatten_v(self, knw):
+        """Fatten in vertical center coord.
+
+        Find the neighboring center grid points in the vertical direction.
 
         **Parameters:**
-        
+
         + knw: KnW object
             The kernel used to find neighboring points.
-        '''
+        """
         if self.iz is None:
             return None
-        if knw.vkernel == 'nearest':
+        if knw.vkernel == "nearest":
             return copy.deepcopy(self.iz.astype(int))
-        elif knw.vkernel in ['dz','linear']:
+        elif knw.vkernel in ["dz", "linear"]:
             try:
                 self.iz_lin
             except AttributeError:
                 (
                     self.iz_lin,
                     self.rz_lin,
                     self.dz_bin,
-                    self.bz_lin
+                    self.bz_lin,
                 ) = self.ocedata.find_rel_v_lin(self.dep)
-            return np.vstack([self.iz_lin.astype(int),self.iz_lin.astype(int)-1]).T
+            return np.vstack([self.iz_lin.astype(int), self.iz_lin.astype(int) - 1]).T
         else:
-            raise Exception('vkernel not supported')
-            
-            
-    def fatten_vl(self,knw):
-        '''
+            raise ValueError("vkernel not supported")
+
+    def fatten_vl(self, knw):
+        """Fatten in vertical staggered coord.
+
         Finding the neighboring staggered grid points in the vertical direction.
 
         **Parameters:**
-        
+
         + knw: KnW object
             The kernel used to find neighboring points.
-        '''
+        """
         if self.izl is None:
             return None
-        if knw.vkernel == 'nearest':
+        if knw.vkernel == "nearest":
             return copy.deepcopy(self.izl.astype(int))
-        elif knw.vkernel in ['dz','linear']:
+        elif knw.vkernel in ["dz", "linear"]:
             try:
                 self.izl_lin
             except AttributeError:
                 (
                     self.izl_lin,
                     self.rzl_lin,
                     self.dzl_bin,
-                    self.bzl_lin
+                    self.bzl_lin,
                 ) = self.ocedata.find_rel_vl_lin(self.dep)
-            return np.vstack([self.izl_lin.astype(int),
-                              self.izl_lin.astype(int)-1]).T
+            return np.vstack([self.izl_lin.astype(int), self.izl_lin.astype(int) - 1]).T
         else:
-            raise Exception('vkernel not supported')
-            
-    def fatten_t(self,knw):
-        '''
+            raise ValueError("vkernel not supported")
+
+    def fatten_t(self, knw):
+        """Fatten in the temporal coord.
+
         Finding the neighboring center grid points in the temporal dimension.
 
         **Parameters:**
-        
+
         + knw: KnW object
             The kernel used to find neighboring points.
-        '''
+        """
         if self.it is None:
             return None
-        if knw.tkernel == 'nearest':
+        if knw.tkernel == "nearest":
             return copy.deepcopy(self.it.astype(int))
-        elif knw.tkernel in ['dt','linear']:
+        elif knw.tkernel in ["dt", "linear"]:
             try:
-                self.it_lin
+                self.izl_lin
             except AttributeError:
                 (
                     self.it_lin,
                     self.rt_lin,
                     self.dt_bin,
-                    self.bt_lin
+                    self.bt_lin,
                 ) = self.ocedata.find_rel_t_lin(self.t)
-            return np.vstack([self.it_lin.astype(int),self.it_lin.astype(int)+1]).T
+            return np.vstack([self.it_lin.astype(int), self.it_lin.astype(int) + 1]).T
         else:
-            raise Exception('vkernel not supported')
-    
-    def fatten(self,knw,fourD = False,required = 'all',ind_moves_kwarg = {}):
-        '''
+            raise ValueError("tkernel not supported")
+
+    def fatten(self, knw, fourD=False, required="all", ind_moves_kwarg={}):
+        """Fatten in all the required dimensions.
+
         Finding the neighboring center grid points in all 4 dimensions.
 
         **Parameters:**
-        
+
         + knw: KnW object
             The kernel used to find neighboring points.
         + fourD: Boolean
-            When we are doing nearest neighbor interpolation on some of the dimensions, 
-            with fourD = True, this will create dimensions with length 1, and will squeeze 
+            When we are doing nearest neighbor interpolation on some of the dimensions,
+            with fourD = True, this will create dimensions with length 1, and will squeeze
             the dimension if fourD = False
         + required: str, iterable of str
             Which dims is needed in the process
         + ind_moves_kward: dict
-            Key word argument to put into ind_moves method of the topology object. 
+            Key word argument to put into ind_moves method of the topology object.
             Read topology.ind_moves for more detail.
-        '''
-        if required!='all' and isinstance(required,str):
+        """
+        if required != "all" and isinstance(required, str):
             required = tuple([required])
-        if required =='all' or isinstance(required,tuple):
+        if required == "all" or isinstance(required, tuple):
             pass
         else:
             required = tuple(required)
-        
-        #TODO: register the kernel shape
-        if _in_required('X',required) or _in_required('Y',required) or _in_required('face',required):
-            ffc,fiy,fix = self.fatten_h(knw,ind_moves_kwarg = ind_moves_kwarg)
+
+        # TODO: register the kernel shape
+        if (
+            _in_required("X", required)
+            or _in_required("Y", required)
+            or _in_required("face", required)
+        ):
+            ffc, fiy, fix = self.fatten_h(knw, ind_moves_kwarg=ind_moves_kwarg)
             if ffc is not None:
-                R = (ffc,fiy,fix)
-                keys = ['face','Y','X']
+                R = (ffc, fiy, fix)
+                keys = ["face", "Y", "X"]
             else:
-                R = (fiy,fix)
-                keys = ['Y','X']
+                R = (fiy, fix)
+                keys = ["Y", "X"]
         else:
-            R = (np.zeros(self.N))
-            keys = ['place_holder']
-            
-        if _in_required('Z',required):
+            R = tuple([np.zeros(self.N)])
+            keys = ["place_holder"]
+
+        if _in_required("Z", required):
             fiz = self.fatten_v(knw)
             if fiz is not None:
-                R = _ind_broadcast(fiz,R)
-                keys.insert(0,'Z')
-        elif _in_required('Zl',required):
+                R = _ind_broadcast(fiz, R)
+                keys.insert(0, "Z")
+        elif _in_required("Zl", required):
             fizl = self.fatten_vl(knw)
             if fizl is not None:
-                R = _ind_broadcast(fizl,R)
-                keys.insert(0,'Zl')
+                R = _ind_broadcast(fizl, R)
+                keys.insert(0, "Zl")
         elif fourD:
-            R = [np.expand_dims(R[i],axis = -1) for i in range(len(R))]
-            
-        if _in_required('time',required):
+            R = [np.expand_dims(R[i], axis=-1) for i in range(len(R))]
+
+        if _in_required("time", required):
             fit = self.fatten_t(knw)
             if fit is not None:
-                R = _ind_broadcast(fit,R)
-                keys.insert(0,'time')
+                R = _ind_broadcast(fit, R)
+                keys.insert(0, "time")
         elif fourD:
-            R = [np.expand_dims(R[i],axis = -1) for i in range(len(R))]
-        R = dict(zip(keys,R))
-        if required == 'all':
-            required = [i for i in keys if i!='place_holder']
+            R = [np.expand_dims(R[i], axis=-1) for i in range(len(R))]
+        R = dict(zip(keys, R))
+        if required == "all":
+            required = [i for i in keys if i != "place_holder"]
         return tuple([R[i] for i in required])
-    
+
     def get_px_py(self):
-        '''
-        Get the nearest 4 corner points of the given point. 
+        """Get the nearest 4 corner points of the given point.
+
         Used for oceanparcel style horizontal interpolation.
-        '''
+        """
         if self.face is not None:
-            return find_px_py(self.ocedata.XG,
-                              self.ocedata.YG,
-                              self.ocedata.tp,
-                              self.face,
-                              self.iy,self.ix
-                             )
+            return find_px_py(
+                self.ocedata.XG,
+                self.ocedata.YG,
+                self.ocedata.tp,
+                self.face,
+                self.iy,
+                self.ix,
+            )
         else:
-            return find_px_py(self.ocedata.XG,
-                              self.ocedata.YG,
-                              self.ocedata.tp,
-                              self.iy,self.ix
-                             )
+            return find_px_py(
+                self.ocedata.XG, self.ocedata.YG, self.ocedata.tp, self.iy, self.ix
+            )
+
     def get_f_node_weight(self):
-        '''
-        The weight for the corner points interpolation
-        '''
-        return weight_f_node(self.rx,self.ry)
-    def get_lon_lat(self):
-        '''
-        Return the lat-lon value based on relative coordinate.
-        This method only work if the dataset has readiness['h'] == 'oceanparcel'
-        '''
-        px,py = self.get_px_py()
+        """Find weight for the corner points interpolation."""
+        return weight_f_node(self.rx, self.ry)
+
+    def _get_lon_lat(self):  # pragma: no cover
+        """Return the lat-lon value based on relative coordinate.
+
+        This method only work if the dataset has readiness['h'] == 'oceanparcel'.
+        """
+        px, py = self.get_px_py()
         w = self.get_f_node_weight()
-        lon = np.einsum('nj,nj->n',w,px.T)
-        lat = np.einsum('nj,nj->n',w,py.T)
-        return lon,lat
-            
-    
-    def _get_needed(self,varName,knw,required = None,prefetched = None,**kwarg):
-        '''An internal testing function'''
+        lon = np.einsum("nj,nj->n", w, px.T)
+        lat = np.einsum("nj,nj->n", w, py.T)
+        return lon, lat
+
+    def _get_needed(
+        self, varName, knw, required=None, prefetched=None, **kwarg
+    ):  # pragma: no cover
         if required is None:
             required = self.ocedata._ds[varName].dims
-        ind = self.fatten(knw,required = required,**kwarg)
-        if len(ind)!= len(self.ocedata._ds[varName].dims):
-            raise Exception("""dimension mismatch.
-                            Please check if the position objects have all the dimensions needed""")
+        ind = self.fatten(knw, required=required, **kwarg)
+        if len(ind) != len(self.ocedata._ds[varName].dims):
+            raise Exception(
+                """dimension mismatch.
+                            Please check if the position objects have all the dimensions needed"""
+            )
         if prefetched is None:
-            return sread(self.ocedata[varName],ind)
+            return sread(self.ocedata[varName], ind)
         else:
             return prefetched[ind]
-    
-    def _get_masked(self,knw,gridtype = 'C',**kwarg):
-        '''An internal testing function'''
-        ind = self.fatten(knw,fourD = True,**kwarg)
+
+    def _get_masked(self, knw, gridtype="C", **kwarg):  # pragma: no cover
+        ind = self.fatten(knw, fourD=True, **kwarg)
         if self.it is not None:
             ind = ind[1:]
-        if len(ind)!=len(self.ocedata._ds['maskC'].dims):
-            raise Exception("""dimension mismatch.
-                            Please check if the position objects have all the dimensions needed""")
-        return get_masked(self.ocedata,ind,gridtype = gridtype)
-    
-    def _find_pk4d(self,knw,gridtype = 'C'):
-        '''An internal testing function'''
-        masked = self._get_masked(knw,gridtype = gridtype)
-        pk4d = find_pk_4d(masked,russian_doll = knw.inheritance)
+        if len(ind) != len(self.ocedata._ds["maskC"].dims):
+            raise Exception(
+                """dimension mismatch.
+                            Please check if the position objects have all the dimensions needed"""
+            )
+        return get_masked(self.ocedata, ind, gridtype=gridtype)
+
+    def _find_pk4d(self, knw, gridtype="C"):  # pragma: no cover
+        masked = self._get_masked(knw, gridtype=gridtype)
+        pk4d = find_pk_4d(masked, russian_doll=knw.inheritance)
         return pk4d
-    
-    def _register_interpolation_input(self,varName,knw,
-                    prefetched = None,i_min = None):
-        '''
+
+    def _register_interpolation_input(self, varName, knw, prefetched=None, i_min=None):
+        """Register the input of interpolation function.
+
         Part of the interpolation function.
         Register the input of the interpolation function.
-        For the input format, go to interpolation for more details. 
+        For the input format, go to interpolation for more details.
 
         **Returns:**
-        
+
         + output_format: dict
-            Record information about the original varName input. 
-            Provide the formatting information for output, 
+            Record information about the original varName input.
+            Provide the formatting information for output,
             such that it matches the input in a direct fashion.
         + main_keys: list
-            A list that defines each interpolation to be performed. 
+            A list that defines each interpolation to be performed.
             The combination of variable name and kernel uniquely define such an operation.
         + prefetch_dict: dict
             Lookup the prefetched the data and its index prefix using main_key
         + main_dict: dict
             Lookup the raw information using main_key
         + hash_index: dict
-            Lookup the token that uniquely define its indexing operation using main_key. 
-            Different main_key could share the same token. 
+            Lookup the token that uniquely define its indexing operation using main_key.
+            Different main_key could share the same token.
         + hash_mask: dict
-            Lookup the token that uniquely define its masking operation using main_key. 
-            Different main_key could share the same token. 
+            Lookup the token that uniquely define its masking operation using main_key.
+            Different main_key could share the same token.
         + hash_read: dict
-            Lookup the token that uniquely define its reading of the data using main_key. 
-            Different main_key could share the same token. 
+            Lookup the token that uniquely define its reading of the data using main_key.
+            Different main_key could share the same token.
         + hash_weight: dict
-            Lookup the token that uniquely define its computation of the weight using main_key. 
-            Different main_key could share the same token. 
-        '''
+            Lookup the token that uniquely define its computation of the weight using main_key.
+            Different main_key could share the same token.
+        """
         # prefetch_dict = {var:(prefetched,i_min)}
         # main_dict = {var:(var,kernel)}
         # hash_index = {var:hash(cuvg,kernel_size)}
         # hash_read  = {var:hash(var,kernel_size)}
         # hash_weight= {var:hash(kernel,cuvg)}
         output_format = {}
-        if isinstance(varName,str) or isinstance(varName,tuple):
+        if isinstance(varName, str) or isinstance(varName, tuple):
             varName = [varName]
-            output_format['single'] = True
-        elif isinstance(varName,list):
-            output_format['single'] = False
+            output_format["single"] = True
+        elif isinstance(varName, list):
+            output_format["single"] = False
         else:
-            raise ValueError('varName needs to be string, tuple, or a list of the above.')
+            raise ValueError(
+                "varName needs to be string, tuple, or a list of the above."
+            )
         Nvar = len(varName)
-        
-        if isinstance(knw,KnW):
+
+        if isinstance(knw, KnW):
             knw = [knw for i in range(Nvar)]
-        if isinstance(knw,tuple):
-            if len(knw)!=2:
-                raise ValueError('When knw is a tuple, we assume it to be kernels for a horizontal vector,'
-                                 'thus, it has to have 2 elements')
+        if isinstance(knw, tuple):
+            if len(knw) != 2:
+                raise ValueError(
+                    "When knw is a tuple, we assume it to be kernels for a horizontal vector,"
+                    "thus, it has to have 2 elements"
+                )
             knw = [knw for i in range(Nvar)]
-        elif isinstance(knw,list):
-            if len(knw)!=Nvar:
-                raise ValueError('Mismatch between the number of kernels and variables')
-        elif isinstance(knw,dict):
+        elif isinstance(knw, list):
+            if len(knw) != Nvar:
+                raise ValueError("Mismatch between the number of kernels and variables")
+        elif isinstance(knw, dict):
             temp = []
             for var in varName:
                 a_knw = knw.get(var)
-                if (a_knw is None) or not(isinstance(a_knw,KnW)):
-                    raise ValueError(f'Variable {var} does not have a proper corresponding kernel')
+                if (a_knw is None) or not (isinstance(a_knw, (tuple, KnW))):
+                    raise ValueError(
+                        f"Variable {var} does not have a proper corresponding kernel"
+                    )
                 else:
                     temp.append(a_knw)
             knw = temp
         else:
-            raise ValueError('knw needs to be a KnW object, or list/dictionaries containing that ')
-            
-        if isinstance(prefetched,np.ndarray):
+            raise ValueError(
+                "knw needs to be a KnW object, or list/dictionaries containing that "
+            )
+
+        if isinstance(prefetched, np.ndarray):
             prefetched = [prefetched for i in range(Nvar)]
-        elif isinstance(prefetched,tuple):
+        elif isinstance(prefetched, tuple):
             prefetched = [prefetched for i in range(Nvar)]
         elif prefetched is None:
             prefetched = [prefetched for i in range(Nvar)]
-        elif isinstance(prefetched,list):
-            if len(prefetched)!=Nvar:
-                raise ValueError('Mismatch between the number of prefetched arrays and variables')
-        elif isinstance(prefetched,dict):
+        elif isinstance(prefetched, list):
+            if len(prefetched) != Nvar:
+                raise ValueError(
+                    "Mismatch between the number of prefetched arrays and variables"
+                )
+        elif isinstance(prefetched, dict):
             prefetched = [prefetched.get(var) for var in varName]
         else:
-            raise ValueError('prefetched needs to be a numpy array/tuple pair of numpy array,'
-                             ' or list/dictionaries containing that')
-            
-        if isinstance(i_min,tuple):
+            raise ValueError(
+                "prefetched needs to be a numpy array/tuple pair of numpy array,"
+                " or list/dictionaries containing that"
+            )
+
+        if isinstance(i_min, tuple):
             i_min = [i_min for i in range(Nvar)]
         elif i_min is None:
             i_min = [None for i in range(Nvar)]
-        elif isinstance(i_min,list):
-            if len(i_min)!=Nvar:
-                raise ValueError('Mismatch between the number of prefetched arrays prefix i_min and variables')
-        elif isinstance(i_min,dict):
+        elif isinstance(i_min, list):
+            if len(i_min) != Nvar:
+                raise ValueError(
+                    "Mismatch between the number of prefetched arrays prefix i_min and variables"
+                )
+        elif isinstance(i_min, dict):
             i_min = [i_min.get(var) for var in varName]
         else:
-            raise ValueError('prefetched prefix i_min needs to be a tuple, or list/dictionaries containing that ')
-            
-            
-        output_format['ori_list'] = copy.deepcopy(list(zip(varName,knw)))
+            raise ValueError(
+                "prefetched prefix i_min needs to be a tuple, or list/dictionaries containing that "
+            )
+
+        output_format["ori_list"] = copy.deepcopy(list(zip(varName, knw)))
         new_varName = []
         new_prefetched = []
         new_knw = []
         new_i_min = []
-        for i,var in enumerate(varName):
-            if isinstance(var,str):
+        for i, var in enumerate(varName):
+            if isinstance(var, str):
                 new_varName.append(var)
                 new_prefetched.append(prefetched[i])
                 new_knw.append(knw[i])
                 new_i_min.append(i_min[i])
-            elif isinstance(var,tuple):
+            elif isinstance(var, tuple):
                 if self.face is None:
                     for j in range(len(var)):
                         new_varName.append(var[j])
-                        new_prefetched.append(prefetched[i][j])
+                        if prefetched[i] is not None:
+                            new_prefetched.append(prefetched[i][j])
+                        else:
+                            new_prefetched.append(None)
                         new_knw.append(knw[i][j])
                         new_i_min.append(i_min[i])
                 else:
                     new_varName.append(var)
                     new_prefetched.append(prefetched[i])
                     new_knw.append(knw[i])
                     new_i_min.append(i_min[i])
             elif var is None:
                 pass
             else:
-                raise ValueError('varName needs to be string, tuple, or a list of the above.')
-        
-        
-        # new_prefetched = []
-        # new_knw = []
-        # new_i_min = []
-        # for i in range(len(knw)):
-        #     if output_format['ori_list'][i] is None:
-        #         pass
-        #     elif isinstance(output_format['ori_list'][i],tuple):
-        #         if self.face is None:
-        #             for j in range(len(output_format['ori_list'][i])):
-        #                 new_prefetched.append(prefetched[i][j])
-        #                 new_knw.append(knw[i][j])
-        #                 new_i_min.append(i_min[i])
-        #         else:
-        #             new_prefetched.append(prefetched[i])
-        #             new_knw.append(knw[i])
-        #             new_i_min.append(i_min[i])
-        #     elif isinstance(output_format['ori_list'][i],str):
-        #         new_prefetched.append(prefetched[i])
-        #         new_knw.append(knw[i])
-        #         new_i_min.append(i_min[i])
+                raise ValueError(
+                    "varName needs to be string, tuple, or a list of the above."
+                )
+
         prefetched = new_prefetched
         knw = new_knw
         i_min = new_i_min
         varName = new_varName
-        output_format['final_varName'] = list(zip(varName,knw))
-            
-            
+        output_format["final_varName"] = list(zip(varName, knw))
+
         kernel_size_hash = []
         kernel_hash = []
         mask_ignore = []
         for kkk in knw:
-            if isinstance(kkk,KnW):
+            if isinstance(kkk, KnW):
                 kernel_size_hash.append(kkk.size_hash())
                 kernel_hash.append(hash(kkk))
                 mask_ignore.append(kkk.ignore_mask)
-            elif isinstance(kkk,tuple):
-                if len(kkk)!=2:
-                    raise ValueError('When knw is a tuple, we assume it to be kernels for a horizontal vector,'
-                                     'thus, it has to have 2 elements')
-                uknw,vknw = kkk
+            elif isinstance(kkk, tuple):
+                if len(kkk) != 2:
+                    raise ValueError(
+                        "When knw is a tuple, we assume it to be kernels for a horizontal vector,"
+                        "thus, it has to have 2 elements"
+                    )
+                uknw, vknw = kkk
                 # if not uknw.same_size(vknw):
                 #     raise Exception('u,v kernel needs to have same size'
                 #                     'to navigate the complex grid orientation.'
                 #                     'use a kernel that include both of the uv kernels'
                 #                    )
                 kernel_size_hash.append(uknw.size_hash())
-                kernel_hash.append(hash((uknw,vknw)))
+                kernel_hash.append(hash((uknw, vknw)))
                 mask_ignore.append(uknw.ignore_mask or vknw.ignore_mask)
         dims = []
         for var in varName:
-            if isinstance(var,str):
+            if isinstance(var, str):
                 dims.append(self.ocedata[var].dims)
-            elif isinstance(var,tuple):
+            elif isinstance(var, tuple):
                 temp = []
                 for vvv in var:
                     temp.append(self.ocedata[vvv].dims)
                 dims.append(tuple(temp))
-        
-        main_keys = list(zip(varName,kernel_hash))
-        prefetch_dict = dict(zip(main_keys,zip(prefetched,i_min)))
-        main_dict     = dict(zip(main_keys,zip(varName,dims,knw)))
-        hash_index    = dict(zip(main_keys,[hash(i) for i in zip(dims,kernel_size_hash)]))
-        hash_mask     = dict(zip(main_keys,[hash(i) for i in zip(dims,mask_ignore,kernel_size_hash)]))
-        hash_read     = dict(zip(main_keys,[hash(i) for i in zip(varName,kernel_size_hash)]))
-        hash_weight   = dict(zip(main_keys,[hash(i) for i in zip(dims,kernel_hash)]))
-        return output_format,main_keys,prefetch_dict,main_dict,hash_index,hash_mask,hash_read,hash_weight
-        
-    
-    def _fatten_required_index_and_register(self,hash_index,main_dict):
-        '''
+
+        main_keys = list(zip(varName, kernel_hash))
+        prefetch_dict = dict(zip(main_keys, zip(prefetched, i_min)))
+        main_dict = dict(zip(main_keys, zip(varName, dims, knw)))
+        hash_index = dict(
+            zip(main_keys, [hash(i) for i in zip(dims, kernel_size_hash)])
+        )
+        hash_mask = dict(
+            zip(main_keys, [hash(i) for i in zip(dims, mask_ignore, kernel_size_hash)])
+        )
+        hash_read = dict(
+            zip(main_keys, [hash(i) for i in zip(varName, kernel_size_hash)])
+        )
+        hash_weight = dict(zip(main_keys, [hash(i) for i in zip(dims, kernel_hash)]))
+        return (
+            output_format,
+            main_keys,
+            prefetch_dict,
+            main_dict,
+            hash_index,
+            hash_mask,
+            hash_read,
+            hash_weight,
+        )
+
+    def _fatten_required_index_and_register(self, hash_index, main_dict):
+        """Fatten for the interpolation process.
+
         Perform the fatten process for each unique token. Register the result as a dict.
 
         **Parameters:**
-        
+
         + hash_index: dict
             See _register_interpolation_input
         + main_dict: dict
             See _register_interpolation_input
 
         **Returns:**
-        
+
         + index_lookup: dict
-            A dictionary to lookup fatten results. 
+            A dictionary to lookup fatten results.
             The keys are the token in hash_index.
-            The values are corresponding results. 
-        '''
+            The values are corresponding results.
+        """
         hsh = np.unique(list(hash_index.values()))
         index_lookup = {}
         for hs in hsh:
-            main_key = get_key_by_value(hash_index,hs)
-            varName,dims,knw = main_dict[main_key]
-            if isinstance(varName,str):
+            main_key = get_key_by_value(hash_index, hs)
+            varName, dims, knw = main_dict[main_key]
+            if isinstance(varName, str):
                 old_dims = dims
-            elif isinstance(varName,tuple):
+            elif isinstance(varName, tuple):
                 old_dims = dims[0]
             dims = []
             for i in old_dims:
-                if i in ['Xp1','Yp1']:
+                if i in ["Xp1", "Yp1"]:
                     dims.append(i[:1])
                 else:
                     dims.append(i)
             dims = tuple(dims)
-            if isinstance(varName,str):
-                ind = self.fatten(knw,required = dims,fourD = True)
+            if isinstance(varName, str):
+                ind = self.fatten(knw, required=dims, fourD=True)
                 index_lookup[hs] = ind
-            elif isinstance(varName,tuple):
-                uknw,vknw = knw
-                uind = self.fatten(uknw,required = dims,fourD = True,ind_moves_kwarg = {'cuvg':'U'})
-                vind = self.fatten(vknw,required = dims,fourD = True,ind_moves_kwarg = {'cuvg':'V'})
-                index_lookup[hs] = (uind,vind)
-            
+            elif isinstance(varName, tuple):
+                uknw, vknw = knw
+                uind = self.fatten(
+                    uknw, required=dims, fourD=True, ind_moves_kwarg={"cuvg": "U"}
+                )
+                vind = self.fatten(
+                    vknw, required=dims, fourD=True, ind_moves_kwarg={"cuvg": "V"}
+                )
+                index_lookup[hs] = (uind, vind)
+
         return index_lookup
-    
-    def _transform_vector_and_register(self,index_lookup,hash_index,main_dict):
-        '''
-        Perform the vector transformation. 
+
+    def _transform_vector_and_register(self, index_lookup, hash_index, main_dict):
+        """Transform vectors for interpolation.
+
+        Perform the vector transformation.
         This is to say that sometimes u velocity becomes v velocity for datasets with face topology.
           Register the result as a dict.
 
         **Parameters:**
-        
+
         + index_lookup: dict
             See _fatten_required_index_and_register
         + hash_index: dict
             See _register_interpolation_input
         + main_dict: dict
             See _register_interpolation_input
 
         **Returns:**
-        
+
         + transform_lookup: dict
-            A dictionary to lookup transformation results. 
+            A dictionary to lookup transformation results.
             The keys are the token in hash_index.
-            The values are corresponding results. 
-        '''
+            The values are corresponding results.
+        """
         hsh = np.unique(list(hash_index.values()))
         transform_lookup = {}
         if self.face is None:
             for hs in hsh:
                 transform_lookup[hs] = None
             return transform_lookup
         for hs in hsh:
-            main_key = get_key_by_value(hash_index,hs)
-            varName,dims,knw = main_dict[main_key]
-            if isinstance(varName,str):
+            main_key = get_key_by_value(hash_index, hs)
+            varName, dims, knw = main_dict[main_key]
+            if isinstance(varName, str):
                 transform_lookup[hs] = None
-            elif isinstance(varName,tuple):
-                uind,vind = index_lookup[hs]
-                uind_dic = dict(zip(dims[0],uind))
-                vind_dic = dict(zip(dims[1],vind))
+            elif isinstance(varName, tuple):
+                uind, vind = index_lookup[hs]
+                uind_dic = dict(zip(dims[0], uind))
+                vind_dic = dict(zip(dims[1], vind))
                 # This only matters when dim == 'face', no need to think about 'Xp1'
-                (UfromUvel,
-                 UfromVvel,
-                 _,
-                 _        ) = self.ocedata.tp.four_matrix_for_uv(uind_dic['face'][:,:,0,0])
-
-                (_,
-                 _,
-                 VfromUvel,
-                 VfromVvel) = self.ocedata.tp.four_matrix_for_uv(vind_dic['face'][:,:,0,0])
-                
+                (UfromUvel, UfromVvel, _, _) = self.ocedata.tp.four_matrix_for_uv(
+                    uind_dic["face"][:, :, 0, 0]
+                )
+
+                (_, _, VfromUvel, VfromVvel) = self.ocedata.tp.four_matrix_for_uv(
+                    vind_dic["face"][:, :, 0, 0]
+                )
+
                 UfromUvel = np.round(UfromUvel)
                 UfromVvel = np.round(UfromVvel)
                 VfromUvel = np.round(VfromUvel)
                 VfromVvel = np.round(VfromVvel)
-                
+
                 bool_ufromu = np.abs(UfromUvel).astype(bool)
                 bool_ufromv = np.abs(UfromVvel).astype(bool)
                 bool_vfromu = np.abs(VfromUvel).astype(bool)
                 bool_vfromv = np.abs(VfromVvel).astype(bool)
-                
+
                 indufromu = tuple([idid[bool_ufromu] for idid in uind])
                 indufromv = tuple([idid[bool_ufromv] for idid in uind])
                 indvfromu = tuple([idid[bool_vfromu] for idid in vind])
                 indvfromv = tuple([idid[bool_vfromv] for idid in vind])
-                
+
                 transform_lookup[hs] = (
-                    (UfromUvel,UfromVvel,VfromUvel,VfromVvel),
-                    (bool_ufromu,bool_ufromv,bool_vfromu,bool_vfromv),
-                    (indufromu,indufromv,indvfromu,indvfromv)
+                    (UfromUvel, UfromVvel, VfromUvel, VfromVvel),
+                    (bool_ufromu, bool_ufromv, bool_vfromu, bool_vfromv),
+                    (indufromu, indufromv, indvfromu, indvfromv),
                 )
             else:
-                raise ValueError(f'unsupported dims: {dims}')
+                raise ValueError(f"unsupported dims: {dims}")
         # modify the index_lookup
         return transform_lookup
-    
-    def _mask_value_and_register(self,index_lookup,transform_lookup,hash_mask,hash_index,main_dict):
-        '''
-        Perform the masking process and register in a dictionary. 
+
+    def _mask_value_and_register(
+        self, index_lookup, transform_lookup, hash_mask, hash_index, main_dict
+    ):
+        """Create masks for interpolation.
+
+        Perform the masking process and register in a dictionary.
 
         **Parameters:**
-        
+
         + index_lookup: dict
             See _fatten_required_index_and_register
         + transform_lookup: dict
-            See _transform_vector_and_lookup 
+            See _transform_vector_and_lookup
         + hash_mask: dict
             See _register_interpolation_input
         + hash_index: dict
             See _register_interpolation_input
         + main_dict: dict
             See _register_interpolation_input
 
         **Returns:**
-        
+
         + mask_lookup: dict
-            A dictionary to lookup masking results. 
+            A dictionary to lookup masking results.
             The keys are the token in hash_mask.
-            The values are corresponding results. 
-        '''
+            The values are corresponding results.
+        """
         hsh = np.unique(list(hash_mask.values()))
         mask_lookup = {}
         for hs in hsh:
-            main_key = get_key_by_value(hash_mask,hs)
-            varName,dims,knw = main_dict[main_key]
+            main_key = get_key_by_value(hash_mask, hs)
+            varName, dims, knw = main_dict[main_key]
             hsind = hash_index[main_key]
-            longDims = ''.join([str(a_thing) for a_thing in dims])
-            if isinstance(knw,KnW):
+            longDims = "".join([str(a_thing) for a_thing in dims])
+            if isinstance(knw, KnW):
                 ignore_mask = knw.ignore_mask
-            elif isinstance(knw,tuple):
+            elif isinstance(knw, tuple):
                 ignore_mask = (knw[0].ignore_mask) or (knw[1].ignore_mask)
-            
-            if ignore_mask or ('X' not in longDims) or ('Y' not in longDims):
+
+            if ignore_mask or ("X" not in longDims) or ("Y" not in longDims):
                 mask_lookup[hs] = None
-            elif isinstance(varName,str):
+            elif isinstance(varName, str):
                 ind = index_lookup[hsind]
-                ind_for_mask = _ind_for_mask(ind,dims)
-                if 'Zl' in dims:
-                    cuvw = 'Wvel'
-                elif 'Z' in dims:
-                    if 'Xp1' in dims and 'Yp1' in dims:
-                        raise NotImplementedError('The masking of corner points are open to '
-                                                  'interpretations thus not implemented, '
-                                                  'let knw.ignore_mask =True to go around')
-                    elif 'Xp1' in dims:
-                        cuvw =  'U'
-                    elif 'Yp1' in dims:
-                        cuvw = 'V'
+                ind_for_mask = _ind_for_mask(ind, dims)
+                if "Zl" in dims:
+                    cuvw = "Wvel"
+                elif "Z" in dims:
+                    if "Xp1" in dims and "Yp1" in dims:
+                        raise NotImplementedError(
+                            "The masking of corner points are open to "
+                            "interpretations thus not implemented, "
+                            "let knw.ignore_mask =True to go around"
+                        )
+                    elif "Xp1" in dims:
+                        cuvw = "U"
+                    elif "Yp1" in dims:
+                        cuvw = "V"
                     else:
-                        cuvw = 'C'
+                        cuvw = "C"
                 else:
-                    cuvw = 'C'
-                masked = get_masked(self.ocedata,ind_for_mask,gridtype = cuvw)
+                    cuvw = "C"
+                masked = get_masked(self.ocedata, ind_for_mask, gridtype=cuvw)
                 mask_lookup[hs] = masked
-            elif isinstance(varName,tuple):
+            elif isinstance(varName, tuple):
                 to_unzip = transform_lookup[hsind]
-                uind,vind = index_lookup[hsind]
+                uind, vind = index_lookup[hsind]
                 if to_unzip is None:
-                    uind_for_mask = _ind_for_mask(uind,dims[0])
-                    vind_for_mask = _ind_for_mask(vind,dims[1])
-                    umask = get_masked(self.ocedata,uind_for_mask,gridtype = 'U')
-                    vmask = get_masked(self.ocedata,vind_for_mask,gridtype = 'V')
+                    uind_for_mask = _ind_for_mask(uind, dims[0])
+                    vind_for_mask = _ind_for_mask(vind, dims[1])
+                    umask = get_masked(self.ocedata, uind_for_mask, gridtype="U")
+                    vmask = get_masked(self.ocedata, vind_for_mask, gridtype="V")
                 else:
                     (
                         _,
-                        (bool_ufromu,bool_ufromv,bool_vfromu,bool_vfromv),
-                        (indufromu,indufromv,indvfromu,indvfromv)
+                        (bool_ufromu, bool_ufromv, bool_vfromu, bool_vfromv),
+                        (indufromu, indufromv, indvfromu, indvfromv),
                     ) = to_unzip
-                    umask = np.full(uind[0].shape,np.nan)
-                    vmask = np.full(vind[0].shape,np.nan)
-                    
-                    umask[bool_ufromu] = get_masked(self.ocedata,_ind_for_mask(indufromu,dims[0]),gridtype = 'U')
-                    umask[bool_ufromv] = get_masked(self.ocedata,_ind_for_mask(indufromv,dims[1]),gridtype = 'V')
-                    vmask[bool_vfromu] = get_masked(self.ocedata,_ind_for_mask(indvfromu,dims[0]),gridtype = 'U')
-                    vmask[bool_vfromv] = get_masked(self.ocedata,_ind_for_mask(indvfromv,dims[1]),gridtype = 'V')
-                mask_lookup[hs] = (umask,vmask)
+                    umask = np.full(uind[0].shape, np.nan)
+                    vmask = np.full(vind[0].shape, np.nan)
+
+                    umask[bool_ufromu] = get_masked(
+                        self.ocedata, _ind_for_mask(indufromu, dims[0]), gridtype="U"
+                    )
+                    umask[bool_ufromv] = get_masked(
+                        self.ocedata, _ind_for_mask(indufromv, dims[1]), gridtype="V"
+                    )
+                    vmask[bool_vfromu] = get_masked(
+                        self.ocedata, _ind_for_mask(indvfromu, dims[0]), gridtype="U"
+                    )
+                    vmask[bool_vfromv] = get_masked(
+                        self.ocedata, _ind_for_mask(indvfromv, dims[1]), gridtype="V"
+                    )
+                mask_lookup[hs] = (umask, vmask)
         return mask_lookup
-    
-    def _read_data_and_register(self,index_lookup,transform_lookup,hash_read,hash_index,main_dict,prefetch_dict):
-        '''
-        Read the data and register them as dict. 
+
+    def _read_data_and_register(
+        self,
+        index_lookup,
+        transform_lookup,
+        hash_read,
+        hash_index,
+        main_dict,
+        prefetch_dict,
+    ):
+        """Read the data and register them as dict.
 
         **Parameters:**
-        
+
         + index_lookup: dict
             See _fatten_required_index_and_register
         + transform_lookup: dict
-            See _transform_vector_and_lookup 
+            See _transform_vector_and_lookup
         + hash_read: dict
             See _register_interpolation_input
         + hash_index: dict
             See _register_interpolation_input
         + main_dict: dict
             See _register_interpolation_input
         + prefetch_dict: dict
             See _register_interpolation_input
 
         **Returns:**
-        
+
         + read_lookup: dict
-            A dictionary to lookup data reading results. 
+            A dictionary to lookup data reading results.
             The keys are the token in hash_read.
-            The values are corresponding results. 
-        '''
+            The values are corresponding results.
+        """
         hsh = np.unique(list(hash_read.values()))
         data_lookup = {}
         for hs in hsh:
-            main_key = get_key_by_value(hash_read,hs)
+            main_key = get_key_by_value(hash_read, hs)
             hsind = hash_index[main_key]
-            varName,dims,knw = main_dict[main_key]
-            prefetched,i_min = prefetch_dict[main_key]
-            if isinstance(varName,str):
+            varName, dims, knw = main_dict[main_key]
+            prefetched, i_min = prefetch_dict[main_key]
+            if isinstance(varName, str):
                 ind = index_lookup[hsind]
                 if prefetched is not None:
                     if i_min is None:
-                        raise ValueError('please pass value of the prefix of prefetched dataset, '
-                                         'even if the prefix is zero')
-                    temp_ind = _subtract_i_min(ind,i_min)
+                        raise ValueError(
+                            "please pass value of the prefix of prefetched dataset, "
+                            "even if the prefix is zero"
+                        )
+                    temp_ind = _subtract_i_min(ind, i_min)
                     needed = np.nan_to_num(prefetched[temp_ind])
                 else:
-                    needed = np.nan_to_num(sread(self.ocedata[varName],ind))
+                    needed = np.nan_to_num(sread(self.ocedata[varName], ind))
                 data_lookup[hs] = needed
-            elif isinstance(varName,tuple):
-                uname,vname = varName
-                uind,vind = index_lookup[hsind]
+            elif isinstance(varName, tuple):
+                uname, vname = varName
+                uind, vind = index_lookup[hsind]
                 (
-                    (UfromUvel,UfromVvel,VfromUvel,VfromVvel),
-                    (bool_ufromu,bool_ufromv,bool_vfromu,bool_vfromv),
-                    (indufromu,indufromv,indvfromu,indvfromv)
+                    (UfromUvel, UfromVvel, VfromUvel, VfromVvel),
+                    (bool_ufromu, bool_ufromv, bool_vfromu, bool_vfromv),
+                    (indufromu, indufromv, indvfromu, indvfromv),
                 ) = transform_lookup[hsind]
-                temp_n_u = np.full(uind[0].shape,np.nan)
-                temp_n_v = np.full(vind[0].shape,np.nan)
+                temp_n_u = np.full(uind[0].shape, np.nan)
+                temp_n_v = np.full(vind[0].shape, np.nan)
                 if prefetched is not None:
-                    upre,vpre = prefetched
-                    ufromu = np.nan_to_num(upre[_subtract_i_min(indufromu,i_min)])
-                    ufromv = np.nan_to_num(vpre[_subtract_i_min(indufromv,i_min)])
-                    vfromu = np.nan_to_num(upre[_subtract_i_min(indvfromu,i_min)])
-                    vfromv = np.nan_to_num(vpre[_subtract_i_min(indvfromv,i_min)])
+                    upre, vpre = prefetched
+                    ufromu = np.nan_to_num(upre[_subtract_i_min(indufromu, i_min)])
+                    ufromv = np.nan_to_num(vpre[_subtract_i_min(indufromv, i_min)])
+                    vfromu = np.nan_to_num(upre[_subtract_i_min(indvfromu, i_min)])
+                    vfromv = np.nan_to_num(vpre[_subtract_i_min(indvfromv, i_min)])
                 else:
-                    ufromu = np.nan_to_num(sread(self.ocedata[uname],indufromu))
-                    ufromv = np.nan_to_num(sread(self.ocedata[vname],indufromv))
-                    vfromu = np.nan_to_num(sread(self.ocedata[uname],indvfromu))
-                    vfromv = np.nan_to_num(sread(self.ocedata[vname],indvfromv))
-                temp_n_u[bool_ufromu] = ufromu#0#
-                temp_n_u[bool_ufromv] = ufromv#1#
-                temp_n_v[bool_vfromu] = vfromu#0#
-                temp_n_v[bool_vfromv] = vfromv#1#
+                    ufromu = np.nan_to_num(sread(self.ocedata[uname], indufromu))
+                    ufromv = np.nan_to_num(sread(self.ocedata[vname], indufromv))
+                    vfromu = np.nan_to_num(sread(self.ocedata[uname], indvfromu))
+                    vfromv = np.nan_to_num(sread(self.ocedata[vname], indvfromv))
+                temp_n_u[bool_ufromu] = ufromu  # 0#
+                temp_n_u[bool_ufromv] = ufromv  # 1#
+                temp_n_v[bool_vfromu] = vfromu  # 0#
+                temp_n_v[bool_vfromv] = vfromv  # 1#
                 # dont_break = np.isclose(temp_n_v,2).any()
                 # if not dont_break:
                 #     print(bool_vfromu)
                 #     raise Exception('what is going on')
                 # else:
                 #     print('somehow it passed')
-                
-                n_u = (np.einsum('nijk,ni->nijk',temp_n_u,UfromUvel)
-                      +np.einsum('nijk,ni->nijk',temp_n_u,UfromVvel))
-                n_v = (np.einsum('nijk,ni->nijk',temp_n_v,VfromUvel)
-                      +np.einsum('nijk,ni->nijk',temp_n_v,VfromVvel))
-                data_lookup[hs] = (n_u,n_v)
-                
+
+                n_u = np.einsum("nijk,ni->nijk", temp_n_u, UfromUvel) + np.einsum(
+                    "nijk,ni->nijk", temp_n_u, UfromVvel
+                )
+                n_v = np.einsum("nijk,ni->nijk", temp_n_v, VfromUvel) + np.einsum(
+                    "nijk,ni->nijk", temp_n_v, VfromVvel
+                )
+                data_lookup[hs] = (n_u, n_v)
+
         return data_lookup
-    
-    def _compute_weight_and_register(self,mask_lookup,hash_weight,hash_mask,main_dict):
-        '''
-        Read the data and register them as dict. 
+
+    def _compute_weight_and_register(
+        self, mask_lookup, hash_weight, hash_mask, main_dict
+    ):
+        """Compute the weights and register them as dict.
 
         **Parameters:**
-        
+
         + mask_lookup: dict
             See _mask_value_and_register
         + hash_weight: dict
             See _register_interpolation_input
         + hash_mask: dict
             See _register_interpolation_input
         + main_dict: dict
             See _register_interpolation_input
 
         **Returns:**
-        
+
         + weight_lookup: dict
-            A dictionary to lookup the weights computed. 
+            A dictionary to lookup the weights computed.
             The keys are the token in hash_weight.
-            The values are corresponding results. 
-        '''
+            The values are corresponding results.
+        """
         hsh = np.unique(list(hash_weight.values()))
         weight_lookup = {}
         for hs in hsh:
-            main_key = get_key_by_value(hash_weight,hs)
+            main_key = get_key_by_value(hash_weight, hs)
             hsmsk = hash_mask[main_key]
-            varName,dims,knw = main_dict[main_key]
+            varName, dims, knw = main_dict[main_key]
             masked = mask_lookup[hsmsk]
-            if isinstance(varName,tuple):
+            if isinstance(varName, tuple):
                 ori_dims = dims
                 dims = ori_dims[0]
                 ori_knw = knw
                 knw = ori_knw[0]
-                # Assuming the two kernels have the same 
+                # Assuming the two kernels have the same
                 # vertical dimensions, which is reasonable.
-            
+
             # shared part for 'vertical direction'
-            this_bottom_scheme = 'no_flux'
-            if 'Z' in dims:
+            this_bottom_scheme = "no_flux"
+            if "Z" in dims:
                 if self.rz is not None:
-                    if knw.vkernel == 'nearest':
+                    if knw.vkernel == "nearest":
                         rz = self.rz
                     else:
                         rz = self.rz_lin
                 else:
                     rz = 0
-            elif 'Zl' in dims:
+            elif "Zl" in dims:
                 this_bottom_scheme = None
-                if self.rz is not None:
-                    if knw.vkernel == 'nearest':
+                if self.rzl is not None:
+                    if knw.vkernel == "nearest":
                         rz = self.rzl
                     else:
                         rz = self.rzl_lin
                 else:
                     rz = 0
             else:
                 rz = 0
             if self.rt is not None:
-                if knw.tkernel == 'nearest':
+                if knw.tkernel == "nearest":
                     rt = self.rt
                 else:
                     rt = self.rt_lin
             else:
                 rt = 0
-                
-            if isinstance(varName,str):
-                if 'Xp1' in dims:
-                    rx = self.rx+0.5
+
+            if isinstance(varName, str):
+                if "Xp1" in dims:
+                    rx = self.rx + 0.5
                 else:
                     rx = self.rx
-                if 'Yp1' in dims:
-                    ry = self.ry+0.5
+                if "Yp1" in dims:
+                    ry = self.ry + 0.5
                 else:
                     ry = self.ry
                 if masked is None:
                     pk4d = None
                 else:
-                    pk4d = find_pk_4d(masked,russian_doll = knw.inheritance)
-                weight = knw.get_weight(rx = rx,ry = ry,
-                                    rz = rz,rt = rt,
-                                    pk4d = pk4d,
-                                    bottom_scheme = this_bottom_scheme)
+                    pk4d = find_pk_4d(masked, russian_doll=knw.inheritance)
+                weight = knw.get_weight(
+                    rx=rx,
+                    ry=ry,
+                    rz=rz,
+                    rt=rt,
+                    pk4d=pk4d,
+                    bottom_scheme=this_bottom_scheme,
+                )
                 weight_lookup[hs] = weight
-            elif isinstance(varName,tuple):
-                uknw,vknw = ori_knw
+            elif isinstance(varName, tuple):
+                uknw, vknw = ori_knw
                 if masked is None:
                     upk4d = None
                     vpk4d = None
                 else:
-                    umask,vmask = masked
-                    upk4d = find_pk_4d(umask,russian_doll = uknw.inheritance)
-                    vpk4d = find_pk_4d(vmask,russian_doll = vknw.inheritance)
-                uweight = uknw.get_weight(self.rx+1/2,self.ry,rz = rz,rt = rt,pk4d = upk4d)
-                vweight = vknw.get_weight(self.rx,self.ry+1/2,rz = rz,rt = rt,pk4d = vpk4d)
-                weight_lookup[hs] = (uweight,vweight)
+                    umask, vmask = masked
+                    upk4d = find_pk_4d(umask, russian_doll=uknw.inheritance)
+                    vpk4d = find_pk_4d(vmask, russian_doll=vknw.inheritance)
+                uweight = uknw.get_weight(
+                    self.rx + 1 / 2, self.ry, rz=rz, rt=rt, pk4d=upk4d
+                )
+                vweight = vknw.get_weight(
+                    self.rx, self.ry + 1 / 2, rz=rz, rt=rt, pk4d=vpk4d
+                )
+                weight_lookup[hs] = (uweight, vweight)
         return weight_lookup
-    
-    def interpolate(self,varName,knw,
-                    vec_transform = True,
-                    prefetched = None,i_min = None):
-        '''
+
+    def interpolate(
+        self, varName, knw, vec_transform=True, prefetched=None, i_min=None
+    ):
+        """Do interpolation.
+
         This is the method that does the actual interpolation/derivative.
         It is a combination of the following methods:
         _register_interpolation_input,
         _fatten_required_index_and_register,
         _transform_vector_and_register,
         _read_data_and_register,
         _mask_value_and_register,
-        _compute_weight_and_registe,
+        _compute_weight_and_registe,.
 
         **Parameters:**
-        
+
         + varName: list, str, tuple
-            The variables to interpolate. Tuples are used for horizontal vectors. 
-            Put str and list in a list if you have multiple things to interpolate. 
-            This input also defines the format of the output. 
+            The variables to interpolate. Tuples are used for horizontal vectors.
+            Put str and list in a list if you have multiple things to interpolate.
+            This input also defines the format of the output.
         + knw: KnW object, tuple, list, dict
-            The kernel object used for the operation. 
-            Put them in the same order as varName. 
-            Some level of automatic broadcasting is also supported. 
+            The kernel object used for the operation.
+            Put them in the same order as varName.
+            Some level of automatic broadcasting is also supported.
         + vec_transform: Boolean
-            Whether to project the vector field to the local zonal/meridional direction. 
+            Whether to project the vector field to the local zonal/meridional direction.
         + prefetched: numpy.ndarray, tuple, list, dict, None
             The prefetched array for the data, this will effectively overwrite varName.
-            Put them in the same order as varName. 
+            Put them in the same order as varName.
             Some level of automatic broadcasting is also supported.
         + i_min: tuple, list, dict, None
-            The prefix of the prefetched array. 
-            Put them in the same order as varName. 
+            The prefix of the prefetched array.
+            Put them in the same order as varName.
             Some level of automatic broadcasting is also supported.
 
         **Returns:**
-        
+
         + R: list, numpy.array, tuple
-            The interpolation/derivative output in the same format as varName. 
-        '''
+            The interpolation/derivative output in the same format as varName.
+        """
         R = []
         (
             output_format,
             main_keys,
             prefetch_dict,
             main_dict,
             hash_index,
             hash_mask,
             hash_read,
-            hash_weight
-        ) = self._register_interpolation_input(varName,knw,
-                    prefetched = prefetched,i_min = i_min)
-        index_lookup = self._fatten_required_index_and_register(hash_index,
-                                                                main_dict)
-        transform_lookup = self._transform_vector_and_register(index_lookup,
-                                                               hash_index,
-                                                               main_dict)
-        data_lookup = self._read_data_and_register(index_lookup,transform_lookup,
-                                                   hash_read,hash_index,
-                                                   main_dict,prefetch_dict)
-        mask_lookup = self._mask_value_and_register(index_lookup,transform_lookup,
-                                                    hash_mask,hash_index,
-                                                    main_dict)
-        weight_lookup = self._compute_weight_and_register(mask_lookup,
-                                                          hash_weight,hash_mask,
-                                                          main_dict)
+            hash_weight,
+        ) = self._register_interpolation_input(
+            varName, knw, prefetched=prefetched, i_min=i_min
+        )
+        index_lookup = self._fatten_required_index_and_register(hash_index, main_dict)
+        transform_lookup = self._transform_vector_and_register(
+            index_lookup, hash_index, main_dict
+        )
+        data_lookup = self._read_data_and_register(
+            index_lookup,
+            transform_lookup,
+            hash_read,
+            hash_index,
+            main_dict,
+            prefetch_dict,
+        )
+        mask_lookup = self._mask_value_and_register(
+            index_lookup, transform_lookup, hash_mask, hash_index, main_dict
+        )
+        weight_lookup = self._compute_weight_and_register(
+            mask_lookup, hash_weight, hash_mask, main_dict
+        )
         # index_list = []
         for key in main_keys:
-            varName,dims,knw = main_dict[key]
-            if isinstance(varName,str):
+            varName, dims, knw = main_dict[key]
+            if isinstance(varName, str):
                 needed = data_lookup[hash_read[key]]
                 weight = weight_lookup[hash_weight[key]]
                 needed = _partial_flatten(needed)
                 weight = _partial_flatten(weight)
-                R.append(np.einsum('nj,nj->n',needed,weight))
+                R.append(np.einsum("nj,nj->n", needed, weight))
                 # index_list.append((index_lookup[hash_index[key]],
                 #                    transform_lookup[hash_index[key]],
                 #                    data_lookup[hash_read[key]]))
-            elif isinstance(varName,tuple):
-                n_u,n_v = data_lookup[hash_read[key]]
-                uweight,vweight = weight_lookup[hash_weight[key]]
-                u = np.einsum('nijk,nijk->n',n_u,uweight)
-                v = np.einsum('nijk,nijk->n',n_v,vweight)
+            elif isinstance(varName, tuple):
+                n_u, n_v = data_lookup[hash_read[key]]
+                uweight, vweight = weight_lookup[hash_weight[key]]
+                u = np.einsum("nijk,nijk->n", n_u, uweight)
+                v = np.einsum("nijk,nijk->n", n_v, vweight)
                 if vec_transform:
-                    u,v = local_to_latlon(u,v,self.cs,self.sn)
-                R.append((u,v))
+                    u, v = local_to_latlon(u, v, self.cs, self.sn)
+                R.append((u, v))
                 # index_list.append((index_lookup[hash_index[key]],
                 #                    transform_lookup[hash_index[key]],
                 #                    data_lookup[hash_read[key]]))
             else:
-                raise ValueError(f'unexpected varName: {varName}')
-                
-        final_dict = dict(zip(output_format['final_varName'],R))
-        ori_list = output_format['ori_list']
+                raise ValueError(f"unexpected varName: {varName}")
+
+        final_dict = dict(zip(output_format["final_varName"], R))
+        ori_list = output_format["ori_list"]
         output = []
         # print(ori_list,R,final_dict.keys())
         for key in ori_list:
-            var,knw = key
-            
+            var, knw = key
+
             if var is None:
                 output.append(None)
             elif isinstance(var, tuple):
                 if self.face is None:
-                    temp_key = [(var[i],knw[i]) for i in range(len(var))]
+                    temp_key = [(var[i], knw[i]) for i in range(len(var))]
                     values = tuple(final_dict.get(k) for k in temp_key)
                     output.append(values)
                 else:
                     output.append(final_dict.get(key))
             else:
                 output.append(final_dict.get(key))
-        if output_format['single']:
+        if output_format["single"]:
             output = output[0]
         return output
-    
-#     def interpolate(self,varName,knw,
-#                     vec_transform = True,
-#                     prefetched = None,i_min = None):
-#         # implement shortcut u,v,w
-#         # TODO: fix the very subtle bug that cause velocity component parallel to face connection
-#         # TODO: add function to interpolate multiple variable at once. 
-#         if prefetched is not None:
-#             # TODO: I could have a warning about prefetch
-#             # overwriting varName.
-#             # But should I?
-#             pass
-#         if isinstance(varName,str):
-#             old_dims = self.ocedata._ds[varName].dims
-#             dims = []
-#             for i in old_dims:
-#                 if i in ['Xp1','Yp1']:
-#                     dims.append(i[:1])
-#                 else:
-#                     dims.append(i)
-#             dims = tuple(dims)
-#             if 'Xp1' in old_dims:
-#                 rx = self.rx+0.5
-#             else:
-#                 rx = self.rx
-#             if 'Yp1' in old_dims:
-#                 ry = self.ry+0.5
-#             else:
-#                 ry = self.ry
-#             ind = self.fatten(knw,required = dims,fourD = True)
-#             ind_dic = dict(zip(dims,ind))
-#             if prefetched is not None:
-#                 temp_ind = []
-#                 if i_min is None:
-#                     raise ValueError('please pass value for the prefix of prefetched dataset, even if the prefix is zero')
-#                 for i,dim in enumerate(dims):
-#                     a_ind = ind[i]
-#                     a_ind-= i_min[i]
-#                     temp_ind.append(a_ind)
-#                 temp_ind = tuple(temp_ind)
-#                 needed = np.nan_to_num(prefetched[temp_ind])
-#             else:
-#                 needed = np.nan_to_num(sread(self.ocedata[varName],ind))
-            
-#             if 'Z' in dims:
-#                 if self.rz is not None:
-#                     if knw.vkernel == 'nearest':
-#                         rz = self.rz
-#                     else:
-#                         rz = self.rz_lin
-#                 else:
-#                     rz = 0
-#             elif 'Zl' in dims:
-#                 if self.rz is not None:
-#                     if knw.vkernel == 'nearest':
-#                         rz = self.rzl
-#                     else:
-#                         rz = self.rzl_lin
-#                 else:
-#                     rz = 0
-#             else:
-#                 rz = 0
-
-#             if self.rt is not None:
-#                 if knw.tkernel == 'nearest':
-#                     rt = self.rt
-#                 else:
-#                     rt = self.rt_lin
-#             else:
-#                 rt = 0
-            
-#             if not ('X' in dims and 'Y' in dims):
-#                 # if it does not have a horizontal dimension, then we don't have to mask
-#                 masked = np.ones_like(ind[0])
-#             else:
-#                 if 'Zl' in dims:
-#                     # something like wvel
-#                     ind_for_mask = tuple([ind[i] for i in range(len(ind)) if dims[i] not in ['time']])
-#                     masked = get_masked(self.ocedata,ind_for_mask,gridtype = 'Wvel')
-#                     this_bottom_scheme = None
-#                 elif 'Z' in dims:
-#                     # something like salt
-#                     ind_for_mask = tuple([ind[i] for i in range(len(ind)) if dims[i] not in ['time']])
-#                     masked = get_masked(self.ocedata,ind_for_mask,gridtype = 'C')
-#                     this_bottom_scheme = 'no_flux'
-#                 else:
-#                     # something like etan
-#                     ind_for_mask = [ind[i] for i in range(len(ind)) if dims[i] not in ['time']]
-#                     ind_for_mask.insert(0,np.zeros_like(ind[0]))
-#                     ind_for_mask = ind_for_mask
-#                     masked = get_masked(self.ocedata,ind_for_mask,gridtype = 'C')
-#                     this_bottom_scheme = 'no_flux'
-                    
-#             pk4d = find_pk_4d(masked,russian_doll = knw.inheritance)
-
-#             weight = knw.get_weight(rx = rx,ry = ry,
-#                                     rz = rz,rt = rt,
-#                                     pk4d = pk4d,
-#                                     bottom_scheme = this_bottom_scheme)
-
-#             needed = partial_flatten(needed)
-#             weight = partial_flatten(weight)
-
-#             R = np.einsum('nj,nj->n',needed,weight)
-#             return R
-# # vector case is here
-#         elif isinstance(varName,list) or isinstance(varName,tuple):
-#             if len(varName)!=2:
-#                 raise Exception('list varName can only have length 2, representing horizontal vectors')
-#             uname,vname = varName
-#             uknw,vknw = knw
-            
-#             if prefetched is not None:
-#                 upre,vpre = prefetched
-#             else:
-#                 upre = None
-#                 vpre = None
-                
-#             if self.face is None:
-#                 # treat them as scalar then. 
-#                 u = self.interpolate(uname,uknw,
-#                     prefetched = upre,i_min = i_min)
-#                 v = self.interpolate(vname,vknw,
-#                     prefetched = vpre,i_min = i_min)
-#             else:
-#                 if not uknw.same_size(vknw):
-#                     raise Exception('u,v kernel needs to have same size'
-#                                     'to navigate the complex grid orientation.'
-#                                     'use a kernel that include both of the uv kernels'
-#                                    )
-
-#                 old_dims = self.ocedata._ds[uname].dims
-#                 dims = []
-#                 for i in old_dims:
-#                     if i in ['Xp1','Yp1']:
-#                         dims.append(i[:1])
-#                     else:
-#                         dims.append(i)
-#                 dims = tuple(dims)
-#                 uind = self.fatten(uknw,required = dims,fourD = True,ind_moves_kwarg = {'cuvg':'U'})
-#                 vind = self.fatten(uknw,required = dims,fourD = True,ind_moves_kwarg = {'cuvg':'V'})
-#                 uind_dic = dict(zip(dims,uind))
-#                 vind_dic = dict(zip(dims,vind))
-
-#                 if prefetched is not None:
-#                     temp_uind = []
-#                     temp_vind = []
-#                     for i,dim in enumerate(dims):
-#                         a_uind = uind[i]
-#                         a_uind-= i_min[i]
-#                         temp_uind.append(a_uind)
-                        
-#                         a_vind = vind[i]
-#                         a_vind-= i_min[i]
-#                         temp_vind.append(a_vind)
-#                     temp_uind = tuple(temp_uind)
-#                     temp_vind = tuple(temp_vind)
-                    
-#                     n_ufromu = np.nan_to_num(upre[temp_uind])
-#                     n_ufromv = np.nan_to_num(vpre[temp_uind])
-#                     n_vfromu = np.nan_to_num(upre[temp_vind])
-#                     n_vfromv = np.nan_to_num(vpre[temp_vind])
-#                 else:  
-#                     # n_u = np.nan_to_num(sread(self.ocedata[uname],ind))
-#                     # n_v = np.nan_to_num(sread(self.ocedata[vname],ind))
-#                     n_ufromu = np.nan_to_num(sread(self.ocedata[uname],uind))
-#                     n_ufromv = np.nan_to_num(sread(self.ocedata[vname],uind))
-#                     n_vfromu = np.nan_to_num(sread(self.ocedata[uname],vind))
-#                     n_vfromv = np.nan_to_num(sread(self.ocedata[vname],vind))
-#     #             np.nan_to_num(n_u,copy = False)
-#     #             np.nan_to_num(n_v,copy = False)
-
-
-#                 if 'Z' in dims:
-#                     if self.rz is not None:
-#                         if uknw.vkernel == 'nearest':
-#                             rz = self.rz
-#                         else:
-#                             rz = self.rz_lin
-#                     else:
-#                         rz = 0
-#                 elif 'Zl' in dims:
-#                     if self.rz is not None:
-#                         if uknw.vkernel == 'nearest':
-#                             rz = self.rzl
-#                         else:
-#                             rz = self.rzl_lin
-#                     else:
-#                         rz = 0
-#                 else:
-#                     rz = 0
-
-#                 if self.rt is not None:
-#                     if uknw.tkernel == 'nearest':
-#                         rt = self.rt
-#                     else:
-#                         rt = self.rt_lin
-#                 else:
-#                     rt = 0
-
-#                 if not ('X' in dims and 'Y' in dims):
-#                     # if it does not have a horizontal dimension, then we don't have to mask
-#                     umask = np.ones_like(ind[0])
-#                     vmask = np.ones_like(ind[0])
-#                 else:
-#                     # In this part, I am using uind for masking, which is not correct, this is kind of temporary, 
-#                     # because I am ging to overhaul the whole function afterwards
-#                     if 'Zl' in dims:
-#                         warnings.warn('the vertical value of vector is between cells, may result in wrong masking')
-#                         ind_for_mask = tuple([uind[i] for i in range(len(uind)) if dims[i] not in ['time']])
-#                         this_bottom_scheme = None
-#                     elif 'Z' in dims:
-#                         # something like salt
-#                         ind_for_mask = tuple([uind[i] for i in range(len(uind)) if dims[i] not in ['time']])
-#                         this_bottom_scheme = 'no_flux'
-#                     else:
-#                         # something like 
-#                         ind_for_mask = [uind[i] for i in range(len(uind)) if dims[i] not in ['time']]
-#                         ind_for_mask.insert(0,np.zeros_like(ind[0]))
-#                         ind_for_mask = ind_for_mask
-#                         this_bottom_scheme = 'no_flux'
-
-#                     umask = get_masked(self.ocedata,ind_for_mask,gridtype = 'U')
-#                     vmask = get_masked(self.ocedata,ind_for_mask,gridtype = 'V')
-#                 if self.face is not None:
-#     #                 hface = ind4d[2][:,:,0,0]
-#                     (UfromUvel,
-#                      UfromVvel,
-#                      _,
-#                      _        ) = self.ocedata.tp.four_matrix_for_uv(uind_dic['face'][:,:,0,0])
-        
-#                     (_,
-#                      _,
-#                      VfromUvel,
-#                      VfromVvel) = self.ocedata.tp.four_matrix_for_uv(vind_dic['face'][:,:,0,0])
-
-
-#                     temp_n_u = (np.einsum('nijk,ni->nijk',n_ufromu,UfromUvel)
-#                                +np.einsum('nijk,ni->nijk',n_ufromv,UfromVvel))
-#                     temp_n_v = (np.einsum('nijk,ni->nijk',n_vfromu,VfromUvel)
-#                                +np.einsum('nijk,ni->nijk',n_vfromv,VfromVvel))
-
-#                     n_u = temp_n_u
-#                     n_v = temp_n_v
-                    
-#                     # again this part is not accurate
-#                     temp_umask = np.round(np.einsum('nijk,ni->nijk',umask,UfromUvel)+
-#                                      np.einsum('nijk,ni->nijk',vmask,UfromVvel))
-#                     temp_vmask = np.round(np.einsum('nijk,ni->nijk',umask,VfromUvel)+
-#                                      np.einsum('nijk,ni->nijk',vmask,VfromVvel))
-
-#                     umask = temp_umask
-#                     vmask = temp_vmask
-#                 else:
-#                     n_u = n_ufromu
-#                     n_v = n_vfromv
-
-#                 upk4d = find_pk_4d(umask,russian_doll = uknw.inheritance)
-#                 vpk4d = find_pk_4d(vmask,russian_doll = vknw.inheritance)
-#                 uweight = uknw.get_weight(self.rx+1/2,self.ry,rz = rz,rt = rt,pk4d = upk4d)
-#                 vweight = vknw.get_weight(self.rx,self.ry+1/2,rz = rz,rt = rt,pk4d = vpk4d)
-
-#     #             n_u    = partial_flatten(n_u   )
-#     #             uweight = partial_flatten(uweight)
-#     #             n_v    = partial_flatten(n_v   )
-#     #             vweight = partial_flatten(veight)
-#                 u = np.einsum('nijk,nijk->n',n_u,uweight)
-#                 v = np.einsum('nijk,nijk->n',n_v,vweight)
-
-#             if vec_transform:
-#                 u,v = local_to_latlon(u,v,self.cs,self.sn)
-#             return u,v
-#         else:
-#             raise Exception('varList type not supported.')
-
```

### Comparing `seaduck-0.1.0/seaduck/get_masks.py` & `seaduck-0.1.2/seaduck/get_masks.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,214 +1,216 @@
-import numpy as np
-import xarray as xr 
 import copy
+import logging
 import warnings
-from seaduck.topology import topology
+
+import numpy as np
+import xarray as xr
+
 from seaduck.smart_read import smart_read
-from seaduck.RuntimeConf import rcParam
 
-def mask_u_node(maskC,tp):
-    '''
+# from seaduck.topology import topology
+
+
+def mask_u_node(maskC, tp):
+    """Mask out U-points.
+
     for MITgcm indexing, U is defined on the left of the cell,
     When the C grid is dry, U are either:
     a. dry;
     b. on the interface, where the cell to the left is wet.
     if b is the case, we need to unmask the udata, because it makes some physical sense.
 
     **Parameters:**
-    
+
     + maskC: numpy.ndarray
-        numpy array with the same shape as the model spacial coordinates. 
+        numpy array with the same shape as the model spacial coordinates.
         1 for wet cells (center points), 0 for dry ones.
     + tp: topology object
-        The topology object for the dataset. 
+        The topology object for the dataset.
 
     **Returns:**
-    
+
     + maskU: numpy.ndarray
-        numpy array with the same shape as the model spacial coordinates. 
+        numpy array with the same shape as the model spacial coordinates.
         1 for wet U-walls (including interface between wet and dry), 0 for dry ones.
-    '''
-        
+    """
     maskU = copy.deepcopy(maskC)
-    indexes = np.array(np.where(maskC==0)).T
-    ### find out which points are masked will make the search faster.
-    nind = tp.ind_tend_vec(indexes.T[1:],np.ones_like(indexes.T[0],int)*2)
-    nind = np.vstack([indexes.T[0],nind])
+    indexes = np.array(np.where(maskC == 0)).T
+    # find out which points are masked will make the search faster.
+    nind = tp.ind_tend_vec(indexes.T[1:], np.ones_like(indexes.T[0], int) * 2)
+    nind = np.vstack([indexes.T[0], nind])
     switch = indexes[np.where(maskC[tuple(nind)])]
     maskU[tuple(switch.T)] = 1
-    
+
     return maskU
 
-def mask_v_node(maskC,tp):
-    '''
+
+def mask_v_node(maskC, tp):
+    """Mask out v-points.
+
     for MITgcm indexing, V is defined on the "south" side of the cell,
     When the C grid is dry, V are either:
     a. dry;
     b. on the interface, where the cell to the downside is wet.
-    if b is the case, we need to unmask the vdata
+    if b is the case, we need to unmask the vdata.
 
     **Parameters:**
-    
+
     + maskC: numpy.ndarray
-        numpy array with the same shape as the model spacial coordinates. 
+        numpy array with the same shape as the model spacial coordinates.
         1 for wet cells (center points), 0 for dry ones.
     + tp: topology object
-        The topology object for the dataset. 
+        The topology object for the dataset.
 
     **Returns:**
-    
+
     + maskV: numpy.ndarray
-        numpy array with the same shape as the model spacial coordinates. 
+        numpy array with the same shape as the model spacial coordinates.
         1 for wet W-walls (including interface between wet and dry), 0 for dry ones.
-    '''
+    """
     maskV = copy.deepcopy(maskC)
-    indexes = np.array(np.where(maskC==0)).T
-    ### find out which points are masked will make the search faster.
-    nind = tp.ind_tend_vec(indexes.T[1:],np.ones_like(indexes.T[0],int)*1)
-    nind = np.vstack([indexes.T[0],nind])
+    indexes = np.array(np.where(maskC == 0)).T
+    # find out which points are masked will make the search faster.
+    nind = tp.ind_tend_vec(indexes.T[1:], np.ones_like(indexes.T[0], int) * 1)
+    nind = np.vstack([indexes.T[0], nind])
     switch = indexes[np.where(maskC[tuple(nind)])]
     maskV[tuple(switch.T)] = 1
     return maskV
 
 
-def mask_w_node(maskC,tp = None):
+def mask_w_node(maskC, tp=None):
     # this one does not need tp object
-    # if you pass something into it by mistake, it will be ignored. 
-    '''
+    # if you pass something into it by mistake, it will be ignored.
+    """Mask out W-points.
+
     for MITgcm indexing, W is defined on the top of the cell,
     When the C grid is dry, W are either:
     a. dry;
     b. on the interface, where the cell above is wet.
-    if b is the case, we need to unmask the wdata
+    if b is the case, we need to unmask the wdata.
 
     **Parameters:**
-    
+
     + maskC: numpy.ndarray
-        numpy array with the same shape as the model spacial coordinates. 
+        numpy array with the same shape as the model spacial coordinates.
         1 for wet cells (center points), 0 for dry ones.
     + tp: topology object
-        The topology object for the dataset. 
+        The topology object for the dataset.
 
     **Returns:**
-    
+
     + maskWvel: numpy.ndarray
-        numpy array with the same shape as the model spacial coordinates. 
+        numpy array with the same shape as the model spacial coordinates.
         1 for wet W-walls (including interface between wet and dry), 0 for dry ones.
-    '''
+    """
     temp = np.zeros_like(maskC)
     temp[1:] = maskC[:-1]
-    maskW = np.logical_or(temp,maskC).astype(int)
+    maskW = np.logical_or(temp, maskC).astype(int)
     return maskW
-    
-def get_masks(od,tp):
-    '''
+
+
+def get_masks(od, tp):
+    """Mask all staggered valocity points.
+
     A wrapper around mask_u_node, mask_v_node, mask_w_node.
-    If there is no maskC in the dataset, just return nothing is masked. 
+    If there is no maskC in the dataset, just return nothing is masked.
 
     **Parameters:**
-    
+
     + od: OceData object
-        The dataset to compute masks on. 
+        The dataset to compute masks on.
     + tp: topology object
         The topology of the datset
 
     **Returns:**
-    
+
     + maskC,maskU,maskV,maskW: numpy.ndarray
-        masks at center points, U-walls, V-walls, W-walls respectively. 
-    '''
+        masks at center points, U-walls, V-walls, W-walls respectively.
+    """
     # tp = topology(od)
     keys = od._ds.keys()
-    if 'maskC' not in keys:
-        warnings.warn('no maskC in the dataset, assuming nothing is masked.')
-        print('no maskC in the dataset, assuming nothing is masked.')
+    if "maskC" not in keys:
+        warnings.warn("no maskC in the dataset, assuming nothing is masked.")
+        logging.warning("no maskC in the dataset, assuming nothing is masked.")
         # od._ds.C_GRID_VARIABLE.to_masked_array().mask
-        maskC = np.ones_like(od._ds.XC+od._ds.Z)
-        # it is inappropriate to fill in the dataset, 
+        maskC = np.ones_like(od._ds.XC + od._ds.Z)
+        # it is inappropriate to fill in the dataset,
         # expecially given that there is no performance boost.
-        return maskC,maskC,maskC,maskC
-    maskC = np.array(od._ds['maskC'])
-    if 'Z' not in od._ds['maskC'].dims:
-        raise NotImplementedError('2D land mask is not yet supported,'
-                                  'you could potentially get around by adding a psuedo dimension'
-                                  'or you could set knw.ignore_mask = True')
-    if 'maskU' not in keys:
-        print('creating maskU,this is going to be very slow!')
-        maskU = mask_u_node(maskC,tp)
-        od._ds['maskU'] = od._ds['Z']+od._ds['XG']
-        od._ds['maskU'].values = maskU
+        return maskC, maskC, maskC, maskC
+    maskC = np.array(od._ds["maskC"])
+    if "Z" not in od._ds["maskC"].dims:
+        raise NotImplementedError(
+            "2D land mask is not yet supported,"
+            "you could potentially get around by adding a psuedo dimension"
+            "or you could set knw.ignore_mask = True"
+        )
+    if "maskU" not in keys:
+        logging.info("creating maskU,this is going to be very slow!")
+        maskU = mask_u_node(maskC, tp)
+        od._ds["maskU"] = od._ds["Z"] + od._ds["XG"]
+        od._ds["maskU"].values = maskU
     else:
-        maskU = np.array(od._ds['maskU'])
-    if 'maskV' not in keys:
-        print('creating maskV,this is going to be very slow!')
-        maskV = mask_v_node(maskC,tp)
-        od._ds['maskV'] = od._ds['Z']+od._ds['YG']
-        od._ds['maskV'].values = maskV
+        maskU = np.array(od._ds["maskU"])
+    if "maskV" not in keys:
+        logging.info("creating maskV,this is going to be very slow!")
+        maskV = mask_v_node(maskC, tp)
+        od._ds["maskV"] = od._ds["Z"] + od._ds["YG"]
+        od._ds["maskV"].values = maskV
     else:
-        maskV = np.array(od._ds['maskV'])
-    if 'maskWvel' not in keys:
+        maskV = np.array(od._ds["maskV"])
+    if "maskWvel" not in keys:
         # there is a maskW with W meaning West in ECCO
-        print('creating maskW,this is going to be somewhat slow')
+        logging.info("creating maskW,this is going to be somewhat slow")
         maskW = mask_w_node(maskC)
-        od._ds['maskWvel'] = od._ds['Z']+od._ds['YC']
-        od._ds['maskWvel'].values = maskW
+        od._ds["maskWvel"] = od._ds["Z"] + od._ds["YC"]
+        od._ds["maskWvel"].values = maskW
     else:
-        maskW = np.array(od._ds['maskWvel'])
-    return maskC,maskU,maskV,maskW
+        maskW = np.array(od._ds["maskWvel"])
+    return maskC, maskU, maskV, maskW
+
+
+def get_masked(od, ind, gridtype="C"):
+    """Return whether points are masked.
 
-def get_masked(od,ind,gridtype = 'C'):
-    '''
     Return whether the indexes of intersts are masked or not.
 
     **Parameters:**
-    
-    + od: OceDataset object
+
+    + od: OceData object
         Dataset to find mask values from.
     + ind: tuple of numpy.ndarray
         Indexes of grid points.
     + gridtype: str
         Whether the indexes is for points at center points or on the walls.
         Options are: ['C','U','V','Wvel'].
-    '''
-    if gridtype not in ['C','U','V','Wvel']:
-        raise NotImplementedError('gridtype for mask not supported')
+    """
+    if gridtype not in ["C", "U", "V", "Wvel"]:
+        raise NotImplementedError("gridtype for mask not supported")
     keys = od._ds.keys()
-    if 'maskC' not in keys:
-        warnings.warn('no maskC in the dataset, assuming nothing is masked.')
-#         print('no maskC in the dataset, assuming nothing is masked.')
-        # od._ds.C_GRID_VARIABLE.to_masked_array().mask
+    if "maskC" not in keys:
+        warnings.warn("no maskC in the dataset, assuming nothing is masked.")
         return np.ones_like(ind[0])
-    elif gridtype == 'C':
-        return smart_read(od._ds.maskC,ind)
-    
-    name = 'mask'+gridtype
+    elif gridtype == "C":
+        return smart_read(od._ds.maskC, ind)
+
+    name = "mask" + gridtype
     tp = od.tp
-    maskC = np.array(od._ds['maskC'])
-    func_dic = {'U':mask_u_node,'V':mask_v_node,'Wvel':mask_w_node}
+    maskC = np.array(od._ds["maskC"])
+    func_dic = {"U": mask_u_node, "V": mask_v_node, "Wvel": mask_w_node}
     rename_dic = {
-        'U':lambda x: x if x!='X' else 'Xp1',
-        'V':lambda x: x if x!='Y' else 'Xp1',
-        'Wvel':lambda x: x if x!='Z' else 'Zl',
+        "U": lambda x: x if x != "X" else "Xp1",
+        "V": lambda x: x if x != "Y" else "Xp1",
+        "Wvel": lambda x: x if x != "Z" else "Zl",
     }
     if name not in keys:
-        if rcParam['debug_level'] in ['high','very_high']:
-            print(f'creating {name}, this is going to be slow!')
-        small_mask = func_dic[gridtype](maskC,tp)
-        dims = tuple(map(
-                                           rename_dic[gridtype],
-                                           od._ds.maskC.dims
-                                       ))
+        small_mask = func_dic[gridtype](maskC, tp)
+        dims = tuple(map(rename_dic[gridtype], od._ds.maskC.dims))
         sizes = tuple([len(od._ds[dim]) for dim in dims])
-#         print(sizes)
         mask = np.zeros(sizes)
-        #indexing sensitive
+        # indexing sensitive
         old_size = small_mask.shape
-        slices = tuple([slice(0,i) for i in old_size])
-#         print(ind_str)
+        slices = tuple([slice(0, i) for i in old_size])
         mask[slices] = small_mask
-        od._ds[name] = xr.DataArray(mask,
-                                    dims = dims
-                                   )
+        od._ds[name] = xr.DataArray(mask, dims=dims)
         return mask[ind]
     else:
-        return smart_read(od._ds[name],ind)
+        return smart_read(od._ds[name], ind)
```

### Comparing `seaduck-0.1.0/seaduck/smart_read.py` & `seaduck-0.1.2/seaduck/smart_read.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,77 +1,79 @@
+from collections import OrderedDict as orderdic
+
 import numpy as np
 import xarray as xr
-from collections import OrderedDict as orderdic
 
-def smart_read(da,ind):
-    '''
-    Read from a xarray.DataArray given tuple indexes, and try to do it fast.
+
+def smart_read(da, ind, memory_chunk=3, xarray_more_efficient=100):
+    """Read from a xarray.DataArray given tuple indexes.
+
+    Try to do it fast and smartly.
 
     **Parameters:**
-    
+
     + da: xarray.DataArray
         DataArray to read from
     + ind: tuple of numpy.ndarray
         The indexes of points of interest, each element does not need to be 1D
 
     **Returns:**
-    
+
     + values: numpy.ndarray
-        The values of the points of interest. Has the same shape as the elements in ind. 
-    '''
-#     print('read called')
+        The values of the points of interest. Has the same shape as the elements in ind.
+    """
     the_shape = ind[0].shape
     ind = tuple([i.ravel() for i in ind])
-    memory_chunk = 3
-    xarray_more_efficient = 100
-    if da.chunks is None:
+    if len(da.dims) != len(ind):
+        raise ValueError("index does not match the number of dimensions")
+    if da.chunks is None or da.chunks == {}:
         npck = np.array(da)
         return npck[ind].reshape(the_shape)
-    if np.prod([len(i) for i in da.chunks])<=memory_chunk:# if the number of chunks is small don't bother 
+    if (
+        np.prod([len(i) for i in da.chunks]) <= memory_chunk
+    ):  # if the number of chunks is small don't bother
         npck = np.array(da)
         return npck[ind].reshape(the_shape)
-    cksz = orderdic(da.chunksizes)
+    cksz = orderdic(zip(da.dims, da.chunks))
     keys = list(cksz.keys())
     n = len(ind[0])
     result = np.zeros(n)
-    
-    if len(keys)!=len(ind):
-        raise Exception('index does not match the number of dimensions')
+
     new_dic = dict()
     # typically what happens is that the first a few indexes are chunked
     # here we figure out what is the last dimension chunked.
-    for i in range(len(cksz)-1,-1,-1):
-        if len(cksz[keys[i]])>1:
+    for i in range(len(cksz) - 1, -1, -1):
+        if len(cksz[keys[i]]) > 1:
             last = i
             break
-    
-    ckbl = np.zeros((n,i+1)).astype(int)
+
+    ckbl = np.zeros((n, i + 1)).astype(int)
     # register each each dimension and the chunk they are in
-    for i,k in enumerate(keys[:i+1]):
+    for i, k in enumerate(keys[: i + 1]):
         ix = ind[i]
         suffix = np.cumsum(cksz[k])
         new_dic[i] = suffix
-        ckbl[:,i] = np.searchsorted(suffix,ix,side = 'right')
+        ckbl[:, i] = np.searchsorted(suffix, ix, side="right")
     # this is the time limiting step for localized long query.
-    ckus,inverse = np.unique(ckbl,axis = 0,return_inverse = True)
+    ckus, inverse = np.unique(ckbl, axis=0, return_inverse=True)
     # ckus is the individual chunks used
-    if len(ckus) <=xarray_more_efficient:
-#         print('use smart')
-        for i,k in enumerate(ckus):
+    if len(ckus) <= xarray_more_efficient:
+        # logging.debug('use smart')
+        for i, k in enumerate(ckus):
             ind_str = []
             pre = []
-            which = (inverse == i)
-            for j,p in enumerate(k):
-                sf = new_dic[j][p]# the upperbound of index
-                pr = sf-cksz[keys[j]][p]# the lower bound of index
-                ind_str.append(f'{pr}:{sf}')
+            which = inverse == i
+            for j, p in enumerate(k):
+                sf = new_dic[j][p]  # the upperbound of index
+                pr = sf - cksz[keys[j]][p]  # the lower bound of index
+                ind_str.append(f"{pr}:{sf}")
                 pre.append(pr)
             prs = np.zeros(len(keys)).astype(int)
-            prs[:last+1] = pre
+            prs[: last + 1] = pre
             npck = eval(f'np.array(da[{",".join(ind_str)}])')
-            subind = tuple([ind[dim][which]-prs[dim] for dim in range(len(ind))])
+            subind = tuple([ind[dim][which] - prs[dim] for dim in range(len(ind))])
             result[which] = npck[subind]
         return result.reshape(the_shape)
     else:
-#         print('use xarray')
+        # logging.debug('use xarray')
         xrind = tuple([xr.DataArray(dim, dims=["x"]) for dim in ind])
-        return np.array(da[xrind]).reshape(the_shape)
+        return np.array(da[xrind]).reshape(the_shape)
```

### Comparing `seaduck-0.1.0/seaduck/topology.py` & `seaduck-0.1.2/seaduck/topology.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,615 +1,648 @@
-# import pandas as pd
-import numpy as np
-from numba import njit
 import copy
-from seaduck.RuntimeConf import rcParam
+import logging
+
+import numpy as np
+
+from seaduck.runtime_conf import compileable
 
 # If you have encountered a NotImplementedError and come to this file,
 # I suggest you read the ***class topology*** near the bottom of this file.
 
-# llc_face_connect = pd.read_csv('llc_face_connect.csv')
-# llc_face_connect = llc_face_connect.drop(columns = 'Unnamed: 0',axis = 1).fillna(42).astype(int)
-tends = [0,1,2,3]#up,down,left,right #list(llc_face_connect.columns)
-
-# llc_face_connect = np.array(llc_face_connect)
-llc_face_connect = np.array([[ 1, 42, 12,  3],
-                             [ 2,  0, 11,  4],
-                             [ 6,  1, 10,  5],
-                             [ 4, 42,  0,  9],
-                             [ 5,  3,  1,  8],
-                             [ 6,  4,  2,  7],
-                             [10,  5,  2,  7],
-                             [10,  5,  6,  8],
-                             [11,  4,  7,  9],
-                             [12,  3,  8, 42],
-                             [ 2,  7,  6, 11],
-                             [ 1,  8, 10, 12],
-                             [ 0,  9, 11, 42]])
-
-directions = np.array([np.pi/2,-np.pi/2,np.pi,0])
-
-@njit
-def llc_mutual_direction(face,nface,transitive = False):
-    '''
-    The compileable version of mutual direction for llc grid. 
-    See topology.mutual direction for more detail. 
-    '''
+tends = [0, 1, 2, 3]  # up,down,left,right #list(llc_face_connect.columns)
+
+llc_face_connect = np.array(
+    [
+        [1, 42, 12, 3],
+        [2, 0, 11, 4],
+        [6, 1, 10, 5],
+        [4, 42, 0, 9],
+        [5, 3, 1, 8],
+        [6, 4, 2, 7],
+        [10, 5, 2, 7],
+        [10, 5, 6, 8],
+        [11, 4, 7, 9],
+        [12, 3, 8, 42],
+        [2, 7, 6, 11],
+        [1, 8, 10, 12],
+        [0, 9, 11, 42],
+    ]
+)
+
+directions = np.array([np.pi / 2, -np.pi / 2, np.pi, 0])
+
+
+@compileable
+def llc_mutual_direction(face, nface, transitive=False):
+    """Find the relative orientation of two faces.
+
+    The compileable version of mutual direction for llc grid.
+    See topology.mutual direction for more detail.
+    """
     edge_n = np.where(llc_face_connect[face] == nface)
     nedge_n = np.where(llc_face_connect[nface] == face)
-    if edge_n[0][0] in [0,1,2,3] and nedge_n[0][0] in [0,1,2,3]:
-        return edge_n[0][0],nedge_n[0][0]
+    try:
+        found = edge_n[0][0] in [0, 1, 2, 3] and nedge_n[0][0] in [0, 1, 2, 3]
+    except Exception:  # It has to be a index error, but numba does not support that
+        found = False
+    if found:
+        return edge_n[0][0], nedge_n[0][0]
     elif transitive:
         common = -1
         for i in llc_face_connect[face]:
             if i in llc_face_connect[nface]:
                 common = i
                 break
-        if common<0:
-            raise ValueError('The two faces does not share common face, transitive did not help')
+        if common < 0:
+            raise ValueError(
+                "The two faces does not share common face, transitive did not help"
+            )
         else:
             edge_1 = np.where(llc_face_connect[face] == common)[0][0]
             nedge_1 = np.where(llc_face_connect[common] == face)[0][0]
             edge_2 = np.where(llc_face_connect[common] == nface)[0][0]
             nedge_2 = np.where(llc_face_connect[nface] == common)[0][0]
-            if (edge_1 in [0,1] and nedge_1 in [0,1]) or (edge_1 in [2,3] and nedge_1 in [2,3]):
-                return edge_2,nedge_2
-            elif (edge_2 in [0,1] and nedge_2 in [0,1]) or (edge_2 in [2,3] and nedge_2 in [2,3]):
-                return edge_1,nedge_1
+            if (edge_1 in [0, 1] and nedge_1 in [0, 1]) or (
+                edge_1 in [2, 3] and nedge_1 in [2, 3]
+            ):
+                return edge_2, nedge_2
+            elif (edge_2 in [0, 1] and nedge_2 in [0, 1]) or (
+                edge_2 in [2, 3] and nedge_2 in [2, 3]
+            ):
+                return edge_1, nedge_1
             else:
-                raise NotImplementedError('the common face is not parallel to either of the face')
+                raise NotImplementedError(
+                    "the common face is not parallel to either of the face"
+                )
     else:
-        raise ValueError('The two faces are not connected (transitive = False)')
-            
-        
-
-@njit
-def llc_get_the_other_edge(face,edge):
-    '''
-    The compileable version of get_the_other_edge for llc grid. 
-    See topology.get_the_other_edge for more detail. 
-    '''
+        raise ValueError("The two faces are not connected (transitive = False)")
+
+
+@compileable
+def llc_get_the_other_edge(face, edge):
+    """See what is adjacent to the face by this edge.
+
+    The compileable version of get_the_other_edge for llc grid.
+    See topology.get_the_other_edge for more detail.
+    """
     face_connect = llc_face_connect
-    nface = face_connect[face,edge]
-    if nface ==42:
-        raise IndexError('Reaching the edge where the face is not connected to any other face')
+    nface = face_connect[face, edge]
+    if nface == 42:
+        raise IndexError(
+            "Reaching the edge where the face is not connected to any other face"
+        )
     nedge_n = np.where(face_connect[nface] == face)
-    return nface,nedge_n[0][0]
+    return nface, nedge_n[0][0]
+
 
-@njit
-def box_ind_tend(ind,tend,iymax,ixmax):
-    '''
-    The compileable version of ind_tend for regional (box) grid. 
-    See topology.ind_tend for more detail. 
-    '''
-    iy,ix = ind
+@compileable
+def box_ind_tend(ind, tend, iymax, ixmax):
+    """Move an index in a direction.
+
+    The compileable version of ind_tend for regional (box) grid.
+    See topology.ind_tend for more detail.
+    """
+    iy, ix = ind
     if tend == 0:
-        iy+=1
+        iy += 1
     elif tend == 1:
-        iy -=1
+        iy -= 1
     elif tend == 2:
-        ix-=1
+        ix -= 1
     elif tend == 3:
-        ix +=1
+        ix += 1
     # it would be better to raise an error here.
-    if (iy>iymax) or (iy<0):
-        return (-1,-1)
-    if (iy>iymax) or (iy<0):
-        return (-1,-1)
-    return (iy,ix)
-@njit
-def x_per_ind_tend(ind,tend,iymax,ixmax):
-    '''
-    The compileable version of ind_tend for zonally periodic (x-per) grid. 
-    See topology.ind_tend for more detail. 
-    '''
-    iy,ix = ind
+    if (iy > iymax) or (iy < 0):
+        return (-1, -1)
+    if (ix > ixmax) or (ix < 0):
+        return (-1, -1)
+    return (iy, ix)
+
+
+@compileable
+def x_per_ind_tend(ind, tend, iymax, ixmax):
+    """Move an index in a direction.
+
+    The compileable version of ind_tend for zonally periodic (x-per) grid.
+    See topology.ind_tend for more detail.
+    """
+    iy, ix = ind
     if tend == 0:
-        iy+=1
+        iy += 1
     elif tend == 1:
-        iy -=1
+        iy -= 1
     elif tend == 2:
-        ix-=1
+        ix -= 1
     elif tend == 3:
-        ix +=1
-    if (iy>iymax) or (iy<0):
-        return (-1,-1)
-    if ix>ixmax:
-        return (iy,ix-ixmax)
-    if ix<0:
-        return (iy,ixmax+ix+1)
-    return (iy,ix)
-
-@njit
-def llc_ind_tend(ind,tendency,iymax,ixmax,gridoffset = 0):
-    '''
-    The compileable version of ind_tend for llc grid. 
-    See topology.ind_tend for more detail. 
-    '''
-#     iymax = 89
-#     ixmax = 89
-    face,iy,ix = ind
+        ix += 1
+    if (iy > iymax) or (iy < 0):
+        return (-1, -1)
+    if ix > ixmax:
+        return (iy, ix - ixmax)
+    if ix < 0:
+        return (iy, ixmax + ix + 1)
+    return (iy, ix)
+
+
+@compileable
+def llc_ind_tend(ind, tendency, iymax, ixmax):
+    """Move an index in a direction.
+
+    The compileable version of ind_tend for llc grid.
+    See topology.ind_tend for more detail.
+    """
+    #     iymax = 89
+    #     ixmax = 89
+    face, iy, ix = ind
     if tendency == 3:
-        if ix!=ixmax:
-            ix+=1
+        if ix != ixmax:
+            ix += 1
         else:
-            nface,nedge = llc_get_the_other_edge(face,3) 
+            nface, nedge = llc_get_the_other_edge(face, 3)
             if nedge == 1:
-                face,iy,ix = [nface,0,ixmax-iy]
-                if gridoffset ==0:
-                    pass
-                elif gridoffset==-1:
-                    face,iy,ix = llc_ind_tend((face,iy,ix),3,iymax,ixmax)
-                elif gridoffset == 1:
-                    face,iy,ix = llc_ind_tend((face,iy,ix),2,iymax,ixmax)
-                else:
-                    raise ValueError('gridoffset must be -1 or 1')
+                face, iy, ix = [nface, 0, ixmax - iy]
             elif nedge == 0:
-                face,iy,ix = [nface,iymax,iy]
+                face, iy, ix = [nface, iymax, iy]
             elif nedge == 2:
-                face,iy,ix = [nface,iy,0]
+                face, iy, ix = [nface, iy, 0]
             elif nedge == 3:
-                face,iy,ix = [nface,iymax-iy,ixmax]
+                face, iy, ix = [nface, iymax - iy, ixmax]
     if tendency == 2:
-        if ix!=0:
-            ix-=1
+        if ix != 0:
+            ix -= 1
         else:
-            nface,nedge = llc_get_the_other_edge(face,2) 
+            nface, nedge = llc_get_the_other_edge(face, 2)
             if nedge == 1:
-                face,iy,ix = [nface,0,iy]
+                face, iy, ix = [nface, 0, iy]
             elif nedge == 0:
-                face,iy,ix = [nface,iymax,ixmax-iy]
-                if gridoffset ==0:
-                    pass
-                elif gridoffset==-1:
-                    face,iy,ix = llc_ind_tend((face,iy,ix),3,iymax,ixmax)
-                elif gridoffset == 1:
-                    face,iy,ix = llc_ind_tend((face,iy,ix),2,iymax,ixmax)
-                else:
-                    raise ValueError('gridoffset must be -1 or 1')
+                face, iy, ix = [nface, iymax, ixmax - iy]
             elif nedge == 2:
-                face,iy,ix = [nface,iymax-iy,0]
+                face, iy, ix = [nface, iymax - iy, 0]
             elif nedge == 3:
-                face,iy,ix = [nface,iy,ixmax]
+                face, iy, ix = [nface, iy, ixmax]
     if tendency == 0:
-        if iy!=iymax:
-            iy+=1
+        if iy != iymax:
+            iy += 1
         else:
-            nface,nedge = llc_get_the_other_edge(face,0) 
+            nface, nedge = llc_get_the_other_edge(face, 0)
             if nedge == 1:
-                face,iy,ix = [nface,0,ix]
+                face, iy, ix = [nface, 0, ix]
             elif nedge == 0:
-                face,iy,ix = [nface,iymax,ixmax-ix]
+                face, iy, ix = [nface, iymax, ixmax - ix]
             elif nedge == 2:
-                face,iy,ix = [nface,iymax-ix,0]
-                if gridoffset ==0:
-                    pass
-                elif gridoffset==-1:
-                    face,iy,ix = llc_ind_tend((face,iy,ix),0,iymax,ixmax)
-                elif gridoffset == 1:
-                    face,iy,ix = llc_ind_tend((face,iy,ix),1,iymax,ixmax)
-                else:
-                    raise ValueError('gridoffset must be -1,1 or 1')
+                face, iy, ix = [nface, iymax - ix, 0]
             elif nedge == 3:
-                face,iy,ix = [nface,ix,ixmax]
+                face, iy, ix = [nface, ix, ixmax]
     if tendency == 1:
-        if iy!=0:
-            iy-=1
+        if iy != 0:
+            iy -= 1
         else:
-            nface,nedge = llc_get_the_other_edge(face,1) 
+            nface, nedge = llc_get_the_other_edge(face, 1)
             if nedge == 1:
-                face,iy,ix = [nface,0,ixmax - ix]
+                face, iy, ix = [nface, 0, ixmax - ix]
             elif nedge == 0:
-                face,iy,ix = [nface,iymax,ix]
+                face, iy, ix = [nface, iymax, ix]
             elif nedge == 2:
-                face,iy,ix = [nface,ix,0]
+                face, iy, ix = [nface, ix, 0]
             elif nedge == 3:
-                face,iy,ix = [nface,iymax-ix,ixmax]
-                if gridoffset ==0:
-                    pass
-                elif gridoffset==-1:
-                    face,iy,ix = llc_ind_tend((face,iy,ix),0,iymax,ixmax)
-                elif gridoffset == 1:
-                    face,iy,ix = llc_ind_tend((face,iy,ix),1,iymax,ixmax)
-                else:
-                    raise ValueError('gridoffset must be -1,1 or 1')
-    return(face,iy,ix)
+                face, iy, ix = [nface, iymax - ix, ixmax]
+    return (face, iy, ix)
 
-@njit
+
+@compileable
 def llc_get_uv_mask_from_face(faces):
-    '''
-    The compileable version of get_uv_mask_from_face for llc grid. 
-    See topology.get_uv_mask_from_face for more detail. 
-    '''
+    """Get the masking of UV points.
+
+    The compileable version of get_uv_mask_from_face for llc grid.
+    See topology.get_uv_mask_from_face for more detail.
+    """
     # we are considering a row from the fatten_face
-    # faces is essentially which face each node of the kernel is on. 
-    n = len(faces)# it should have been m to be more consistent with other code
+    # faces is essentially which face each node of the kernel is on.
+    n = len(faces)  # it should have been m to be more consistent with other code
     UfromUvel = np.ones(n)
     UfromVvel = np.zeros(n)
     VfromUvel = np.zeros(n)
     VfromVvel = np.ones(n)
     # if all of the node are on the same face, we don't have to convert anything
-    if np.abs(np.ones(n)*faces[0]-faces).max()<1e-5:
-        return UfromUvel,UfromVvel,VfromUvel, VfromVvel
+    if np.abs(np.ones(n) * faces[0] - faces).max() < 1e-5:
+        return UfromUvel, UfromVvel, VfromUvel, VfromVvel
     else:
-        for i in range(1,n):
-            if faces[i]==faces[0]:
+        for i in range(1, n):
+            if faces[i] == faces[0]:
                 continue
             # if the face is not the same, we need to do something
             else:
                 # get how much the new face is rotated from the old face
-                edge,nedge = llc_mutual_direction(faces[0],faces[i],transitive = True)
-                rot = np.pi-directions[edge]+directions[nedge]
+                edge, nedge = llc_mutual_direction(faces[0], faces[i], transitive=True)
+                rot = np.pi - directions[edge] + directions[nedge]
                 # you can think of this as a rotation matrix
                 UfromUvel[i] = np.cos(rot)
                 UfromVvel[i] = np.sin(rot)
                 VfromUvel[i] = -np.sin(rot)
                 VfromVvel[i] = np.cos(rot)
-        return UfromUvel,UfromVvel,VfromUvel, VfromVvel
+        return UfromUvel, UfromVvel, VfromUvel, VfromVvel
 
-class topology():
-    '''
-    This is a light weight object that remembers the structure of the grid, 
-    what is connected, what is not. The core method is simply move the index to a direction. 
-    In the movie kill Bill, the bride sat in a car and said "wiggle your big toe". 
-    After the toe moved, "the hard part is over". You get the idea. 
+
+class topology:
+    """Topology object.
+
+    A light weight object that remembers the structure of the grid,
+    what is connected, what is not. The core method is simply move the index to a direction.
+    In the movie kill Bill, the bride sat in a car and said "wiggle your big toe".
+    After the toe moved, "the hard part is over". You get the idea.
 
     **Parameters:**
-    
+
     + od: xarray.Dataset, OceData object
-        The dataset to record topological info from. 
+        The dataset to record topological info from.
     + typ: None, or str
-        Type of the grid. 
-        Currently we support 
-        'box' for regional dataset, 
+        Type of the grid.
+        Currently we support
+        'box' for regional dataset,
         'x-periodic' for zonally periodic ones,
         'llc' for lat-lon-cap dataset.
         We recommend that users put None here,
-        so that the type is figured out automatically. 
-    '''
-    def __init__(self,od,typ = None):
+        so that the type is figured out automatically.
+    """
+
+    def __init__(self, od, typ=None):
         try:
-            h_shape = od['XC'].shape
+            h_shape = od["XC"].shape
         except KeyError:
             try:
-                h_shape = (int(od['lat'].shape[0]),int(od['lon'].shape[0]))
+                h_shape = (int(od["lat"].shape[0]), int(od["lon"].shape[0]))
             except KeyError:
-                raise KeyError("Either XC or lat/lon is needed to create the topology object")
+                raise KeyError(
+                    "Either XC or lat/lon is needed to create the topology object"
+                )
         self.h_shape = h_shape
         try:
-            self.itmax = len(od['time'])-1
+            self.itmax = len(od["time"]) - 1
         except (KeyError, TypeError):
             self.itmax = 0
         try:
-            self.izmax = len(od['Z'])-1
+            self.izmax = len(od["Z"]) - 1
         except (KeyError, TypeError):
             self.izmax = 0
-            
+
         if typ:
             self.typ = typ
         elif typ is None:
             if len(h_shape) == 3:
-                self.num_face,self.iymax,self.ixmax = h_shape
-                self.iymax -=1
-                self.ixmax -=1
-                if self.num_face ==13:
-                    self.typ = 'LLC'
+                self.num_face, self.iymax, self.ixmax = h_shape
+                self.iymax -= 1
+                self.ixmax -= 1
+                if self.num_face == 13:
+                    self.typ = "LLC"
                     # we can potentially generate the face connection in runtime
                     # say, put the csv file on cloud
-                elif self.num_face ==6:
-                    self.typ = 'cubed_sphere'
+                else:
+                    raise NotImplementedError(
+                        "Other complex topology is not implemented yet."
+                        "If you want to work with such data, please contact the authors."
+                    )
             elif len(h_shape) == 2:
-                self.iymax,self.ixmax = h_shape
-                self.iymax -=1
-                self.ixmax -=1
+                self.iymax, self.ixmax = h_shape
+                self.iymax -= 1
+                self.ixmax -= 1
                 try:
-                    lon_right = float(od['XC'][0,self.ixmax])
-                    lon_left  = float(od['XC'][0,  0  ])
+                    lon_right = float(od["XC"][0, self.ixmax])
+                    lon_left = float(od["XC"][0, 0])
                 except KeyError:
-                    lon_right = float(od['lon'][self.ixmax])
-                    lon_left  = float(od['lon'][0])
-                left_to_right = (lon_right - lon_left)%360
-                right_to_left = (lon_left - lon_right)%360
-                if left_to_right >50*right_to_left:
-                    self.typ = 'x_periodic'
+                    lon_right = float(od["lon"][self.ixmax])
+                    lon_left = float(od["lon"][0])
+                left_to_right = (lon_right - lon_left) % 360
+                right_to_left = (lon_left - lon_right) % 360
+                if left_to_right > 50 * right_to_left:
+                    self.typ = "x_periodic"
                 else:
-                    self.typ = 'box'
-                    
-    def get_the_other_edge(self,face,edge):
-        '''
+                    self.typ = "box"
+
+    def get_the_other_edge(self, face, edge):
+        """See what is adjacent to the face by this edge.
+
         The (edge) side of the (face) is connected to
         the (nedge) side of the (nface).
-        0,1,2,3 stands for up, down, left, right
+        0,1,2,3 stands for up, down, left, right.
 
         **Parameters:**
-        
+
         + face: int
             The face of interst
         + edge: 0,1,2,3
             which direction of the face we are looking for
-        
+
         **Returns:**
 
         + nface: int
             The face adjacent to face in the edge direction.
         + nedge: 0,1,2,3
-            The face is connected to nface in which direction. 
-        '''
-        if self.typ =='LLC':
-            return llc_get_the_other_edge(face,edge)
-        elif self.typ in ['x_periodic','box']:
-            raise Exception('It makes no sense to tinker with face_connection when there is only one face')
+            The face is connected to nface in which direction.
+        """
+        if self.typ == "LLC":
+            return llc_get_the_other_edge(face, edge)
+        elif self.typ in ["x_periodic", "box"]:
+            raise Exception(
+                "It makes no sense to tinker with face_connection when there is only one face"
+            )
         else:
             raise NotImplementedError
-    def mutual_direction(self,face,nface,**kwarg):
-        '''
+
+    def mutual_direction(self, face, nface, **kwarg):
+        """Find the relative orientation of two faces.
+
         0,1,2,3 stands for up, down, left, right
-        given 2 faces, the returns are 
+        given 2 faces, the returns are
         1. the 2nd face is to which direction of the 1st face
-        2. the 1st face is to which direction of the 2nd face
-        '''
-        if self.typ =='LLC':
-            return llc_mutual_direction(face,nface,**kwarg)
-        elif self.typ in ['x_periodic','box']:
-            raise Exception('It makes no sense to tinker with face_connection when there is only one face')
+        2. the 1st face is to which direction of the 2nd face.
+        """
+        if self.typ == "LLC":
+            return llc_mutual_direction(face, nface, **kwarg)
+        elif self.typ in ["x_periodic", "box"]:
+            raise Exception(
+                "It makes no sense to tinker with face_connection when there is only one face"
+            )
         else:
             raise NotImplementedError
-            
-    def ind_tend(self,ind,tend,cuvg = 'C',**kwarg):
-        '''
+
+    def ind_tend(self, ind, tend, cuvg="C", **kwarg):
+        """Move an index in a direction.
+
         ind is a tuple that is face,iy,ix,
         tendency again is up, down, left, right represented by 0,1,2,3
         return the next cell.
 
         **Parameters:**
-        
+
         + ind: tuple
             The index to find the neighbor of
         + tend: int
-            Which direction to move from the original index. 
+            Which direction to move from the original index.
         + cuvg:
-            Whether we are moving from C grid, U grid, V grid, or G grid. 
+            Whether we are moving from C grid, U grid, V grid, or G grid.
         + kwarg:dict
-            Keyword argument that currently only apply for the llc case. 
-            Use gridoffset keyword when you are dealing with different grid-indexing, 
+            Keyword argument that currently only apply for the llc case.
+            Use gridoffset keyword when you are dealing with different grid-indexing,
             -1 for MITgcm (default), 1 for NEMO.
-        '''
-        if -1 in ind:# meaning invalid point
+        """
+        if -1 in ind:
+            # meaning invalid point
             return tuple([-1 for i in ind])
-#         if tend not in [0,1,2,3]:
-#             raise Exception('Illegal move. Must be 0,1,2,3')
-        if self.typ == 'LLC':
-            if cuvg == 'C':
-                return llc_ind_tend(ind,tend,self.iymax,self.ixmax,**kwarg)
-            elif cuvg == 'U':
-                UorV,R = self._ind_tend_U(ind,tend)
+        #         if tend not in [0,1,2,3]:
+        #             raise Exception('Illegal move. Must be 0,1,2,3')
+        if self.typ == "LLC":
+            if cuvg == "C":
+                return llc_ind_tend(ind, tend, self.iymax, self.ixmax, **kwarg)
+            elif cuvg == "U":
+                UorV, R = self._ind_tend_U(ind, tend)
                 return R
-            elif cuvg == 'V':
-                UorV,R = self._ind_tend_V(ind,tend)
+            elif cuvg == "V":
+                UorV, R = self._ind_tend_V(ind, tend)
                 return R
-            elif cuvg == 'G':
-                raise NotImplementedError('G grid is not yet supported')
+            elif cuvg == "G":
+                raise NotImplementedError("G grid is not yet supported")
             else:
-                raise ValueError('The type of grid point should be among C,U,V,G')
-        elif self.typ == 'x_periodic':
-            return x_per_ind_tend(ind,tend,self.iymax,self.ixmax,**kwarg)
-        elif self.typ == 'box':
-            return box_ind_tend(ind,tend,self.iymax,self.ixmax,**kwarg)
+                raise ValueError("The type of grid point should be among C,U,V,G")
+        elif self.typ == "x_periodic":
+            return x_per_ind_tend(ind, tend, self.iymax, self.ixmax, **kwarg)
+        elif self.typ == "box":
+            return box_ind_tend(ind, tend, self.iymax, self.ixmax, **kwarg)
         else:
             raise NotImplementedError
-    def ind_moves(self,ind,moves,**kwarg):
-        '''
+
+    def ind_moves(self, ind, moves, **kwarg):
+        """Move an index in a serie of directions.
+
         moves being a list of directions (0,1,2,3),
         ind being the starting index,
-        return the index after moving in the directions in the list
+        return the index after moving in the directions in the list.
 
         **Parameters:**
-        
+
         + ind: tuple
             Index of the starting position
         + moves: iterable
-            A sequence of steps to "walk" from the original position. 
+            A sequence of steps to "walk" from the original position.
         + kwarg: dict
-            Keyword arguments that pass into ind_tend. 
-        '''
+            Keyword arguments that pass into ind_tend.
+        """
         if self.check_illegal(ind):
-            return tuple([-1 for i in ind])# the origin is invalid
-        if not set(moves).issubset({0,1,2,3}):
-            raise Exception('Illegal move. Must be 0,1,2,3')
-        if self.typ in ['LLC','cubed_sphere']:
-            face,iy,ix = ind
+            return tuple([-1 for i in ind])  # the origin is invalid
+        if not set(moves).issubset({0, 1, 2, 3}):
+            raise ValueError("Illegal move. Must be 0,1,2,3")
+        if self.typ in ["LLC", "cubed_sphere"]:
+            face, iy, ix = ind
             for k in range(len(moves)):
                 move = moves[k]
-                ind =  self.ind_tend(ind,move,**kwarg)
-                if ind[0]!=face:# if the face has changed
-                    '''
+                ind = self.ind_tend(ind, move, **kwarg)
+                if ind[0] != face:  # if the face has changed
+                    """
                     there are times where the the kernel lies between
-                    2 faces that define 'left' differently. That's why 
+                    2 faces that define 'left' differently. That's why
                     when that happens we need to correct the direction
                     you want to move the indexes.
-                    '''
-                    edge,nedge = self.mutual_direction(face,ind[0],transitive = True)
-                    rot = (np.pi-directions[edge]+directions[nedge])%(np.pi*2)
-                    if np.isclose(rot,0):
+                    """
+                    edge, nedge = self.mutual_direction(face, ind[0], transitive=True)
+                    rot = (np.pi - directions[edge] + directions[nedge]) % (np.pi * 2)
+                    if np.isclose(rot, 0):
                         pass
-                    elif np.isclose(rot,np.pi/2):
-                        moves[k+1:] = [[2,3,1,0][move] for move in moves[k+1:]]
-                    elif np.isclose(rot,3*np.pi/2):
-                        moves[k+1:] = [[3,2,0,1][move] for move in moves[k+1:]]
+                    elif np.isclose(rot, np.pi / 2):
+                        moves[k + 1 :] = [[2, 3, 1, 0][move] for move in moves[k + 1 :]]
+                    elif np.isclose(rot, 3 * np.pi / 2):
+                        moves[k + 1 :] = [[3, 2, 0, 1][move] for move in moves[k + 1 :]]
                     face = ind[0]
-                    # if the old face is on the left of the new face, 
+                    # if the old face is on the left of the new face,
                     # the particle should be heading right
-        elif self.typ in ['x_periodic','box']:
+        elif self.typ in ["x_periodic", "box"]:
             for move in moves:
-                ind = self.ind_tend(ind,move)
+                ind = self.ind_tend(ind, move)
         return ind
-    def check_illegal(self,ind):
-        '''
+
+    def check_illegal(self, ind):
+        """Check if the index is legal.
+
         A vectorized check to see whether the index is legal,
         index can be a tuple of numpy ndarrays.
-        no negative index is permitted for sanity reason. 
+        no negative index is permitted for sanity reason.
 
         **Parameters:**
-        
+
         + ind: tuple
-            Each element of the tuple is iterable of one dimension of the indexes. 
-        '''
-        if isinstance(ind[0],int):# for single item
+            Each element of the tuple is iterable of one dimension of the indexes.
+        """
+        if isinstance(ind[0], int):  # for single item
             result = False
-            for i,z in enumerate(ind):
+            for i, z in enumerate(ind):
                 max_pos = self.h_shape[i]
-                if not (0<=z<=max_pos-1):
+                if not (0 <= z <= max_pos - 1):
                     result = True
             return result
-        else:# for numpy ndarray
+        else:  # for numpy ndarray
             result = np.zeros_like(ind[0])
-            result = False # make it cleaner
-            for i,z in enumerate(ind):
+            result = False  # make it cleaner
+            for i, z in enumerate(ind):
                 max_pos = self.h_shape[i]
-                result = np.logical_or(np.logical_or((0>z),(z>max_pos-1)),result)
+                result = np.logical_or(
+                    np.logical_or((0 > z), (z > max_pos - 1)), result
+                )
             return result
-    def ind_tend_vec(self,inds,tend,**kwarg):
-        '''
-        Vectorized version for ind_tend method. 
+
+    def ind_tend_vec(self, inds, tend, **kwarg):
+        """Move many indices in a list of directions.
+
+        Vectorized version for ind_tend method.
 
         **Parameters:**
-        
+
         + inds: tuple or numpy.array
-            Each element of the tuple is iterable of one dimension of the indexes. 
+            Each element of the tuple is iterable of one dimension of the indexes.
         + tend: iterable
-            Which direction should each index take. 
+            Which direction should each index take.
         + kwarg: dict
-            Keyword argument that feeds into ind_tend. 
-        '''
+            Keyword argument that feeds into ind_tend.
+        """
         inds = np.array(inds)
         old_inds = copy.deepcopy(inds)
         move_dic = {
-            0:np.array([1,0]),# delta_y,delta_x
-            1:np.array([-1,0]),
-            2:np.array([0,-1]),
-            3:np.array([0,1])
+            0: np.array([1, 0]),  # delta_y,delta_x
+            1: np.array([-1, 0]),
+            2: np.array([0, -1]),
+            3: np.array([0, 1]),
         }
         naive_move = np.array([move_dic[i] for i in tend]).T.astype(int)
-        inds[-2:]+=naive_move
+        inds[-2:] += naive_move
         illegal = self.check_illegal(inds)
         redo = np.array(np.where(illegal)).T
         particle_on_edge = False
-        for num,loc in enumerate(redo):
+        for num, loc in enumerate(redo):
             j = loc[0]
-            ind = tuple(old_inds[:,j])
+            ind = tuple(old_inds[:, j])
             try:
-                n_ind = self.ind_tend(ind,int(tend[j]),**kwarg)
+                n_ind = self.ind_tend(ind, int(tend[j]), **kwarg)
             except IndexError:
                 particle_on_edge = True
                 n_ind = ind
-            inds[:,j] = np.array(n_ind).ravel()
-        if particle_on_edge and rcParam['debug_level'] == 'very_high':
-            print('Warning:Some points are on the edge')
+            inds[:, j] = np.array(n_ind).ravel()
+        if particle_on_edge:
+            logging.warning("Some points are on the edge")
         for i in range(len(inds)):
             inds[i] = inds[i].astype(int)
         return inds
-    def _find_wall_between(self,ind1,ind2):
-        '''
-        return the wall between two adjacent cells,
+
+    def _find_wall_between(self, ind1, ind2):
+        """Return the wall between two adjacent cells.
+
         if the input is not adjacent, error may not be raised
         This scheme is only valid if there is face in the dimensions.
-        '''
-        (fc1,iy1,ix1) = ind1
-        (fc2,iy2,ix2) = ind2
-        Non_normal_connection = ValueError(f'The two face connecting the indexes {ind1},{ind2}'
-                                           ' are not connected in a normal way')
+        """
+        (fc1, iy1, ix1) = ind1
+        (fc2, iy2, ix2) = ind2
+        Non_normal_connection = ValueError(
+            f"The two face connecting the indexes {ind1},{ind2}"
+            " are not connected in a normal way"
+        )
         if fc1 == fc2:
-            R = tuple(np.ceil((np.array(ind1)+np.array(ind2))/2).astype(int))
-            other = ind1 if ind2==R else ind2
-            (fcr,iyr,ixr) = R
-            (fco,iyo,ixo) = other
-            if ixr>ixo:
-                return 'U',R
-            elif iyr>iyo:
-                return 'V',R
+            R = tuple(np.ceil((np.array(ind1) + np.array(ind2)) / 2).astype(int))
+            other = ind1 if ind2 == R else ind2
+            (fcr, iyr, ixr) = R
+            (fco, iyo, ixo) = other
+            if ixr > ixo:
+                return "U", R
+            elif iyr > iyo:
+                return "V", R
             else:
-                raise IndexError('there is no wall between a cell and itself')
+                raise IndexError("there is no wall between a cell and itself")
                 # This error can be raised when there is three instead of four points in a corner
         else:
-            d1to2,d2to1 = self.mutual_direction(fc1,fc2)
-            if d1to2 in [0,3]:
+            d1to2, d2to1 = self.mutual_direction(fc1, fc2)
+            if d1to2 in [0, 3]:
                 R = ind2
                 if d2to1 == 1:
-                    return 'V',R
+                    return "V", R
                 elif d2to1 == 2:
-                    return 'U',R
+                    return "U", R
                 else:
                     raise Non_normal_connection
-            elif d2to1 in [0,3]:
+            elif d2to1 in [0, 3]:
                 R = ind1
                 if d1to2 == 1:
-                    return 'V',R
+                    return "V", R
                 elif d1to2 == 2:
-                    return 'U',R
+                    return "U", R
                 else:
                     raise Non_normal_connection
             else:
                 raise Non_normal_connection
-            
-    def _ind_tend_U(self,ind,tend):
-        '''
-        A subset of ind_tend that deal with special issues 
-        that comes from staggered grid. Read ind_tend for more info 
-        '''
+
+    def _ind_tend_U(self, ind, tend):
+        """Move an U-index in a direction.
+
+        A subset of ind_tend that deal with special issues
+        that comes from staggered grid. Read ind_tend for more info.
+        """
         # TODO: implement different grid offset case
-        if tend in [2,3]:
-            return 'U',self.ind_tend(ind,tend)
+        if tend in [2, 3]:
+            return "U", self.ind_tend(ind, tend)
         else:
-            first = self.ind_tend(ind,tend)
+            first = self.ind_tend(ind, tend)
             if first[0] == ind[0]:
-                return 'U',first
+                return "U", first
             else:
-                alter = self.ind_moves(ind,[2,tend])
+                alter = self.ind_moves(ind, [2, tend])
                 # TODO: Add the case of alter == first for three-way join of faces.Low priority
-                return self._find_wall_between(first,alter)
-            
-    def _ind_tend_V(self,ind,tend):
-        '''
-        A subset of ind_tend that deal with special issues 
-        that comes from staggered grid. Read ind_tend for more info 
-        '''
+                return self._find_wall_between(first, alter)
+
+    def _ind_tend_V(self, ind, tend):
+        """Move an V-index in a direction.
+
+        A subset of ind_tend that deal with special issues
+        that comes from staggered grid. Read ind_tend for more info.
+        """
         # TODO: implement different grid offset case
-        if tend in [0,1]:
-            return 'V',self.ind_tend(ind,tend)
+        if tend in [0, 1]:
+            return "V", self.ind_tend(ind, tend)
         else:
-            first = self.ind_tend(ind,tend)
+            first = self.ind_tend(ind, tend)
             if first[0] == ind[0]:
-                return 'V',first
+                return "V", first
             else:
-                alter = self.ind_moves(ind,[1,tend])
-                return self._find_wall_between(first,alter)
-        
-    def get_uv_mask_from_face(self,faces):
-        '''
+                alter = self.ind_moves(ind, [1, tend])
+                return self._find_wall_between(first, alter)
+
+    def get_uv_mask_from_face(self, faces):
+        """Get the masking of UV points.
+
         The background is as following:
-        For a dataset with face connection, 
-        when one is finding the neighboring cells for vector interpolation, 
-        the fact that faces can be rotated against each other can create 
+        For a dataset with face connection,
+        when one is finding the neighboring cells for vector interpolation,
+        the fact that faces can be rotated against each other can create
         local inconsistency in vector definition near face connections.
-        This method corrects that. 
+        This method corrects that.
 
         **Parameters:**
-        
+
         + faces: iterable
-            1D iterable of faces, the first one is assumed to be the reference. 
-        '''
-        if self.typ =='LLC':
+            1D iterable of faces, the first one is assumed to be the reference.
+        """
+        if self.typ == "LLC":
             return llc_get_uv_mask_from_face(faces)
-        elif self.typ in ['x_periodic','box']:
-            raise Exception('It makes no sense to tinker with face_connection when there is only one face')
+        elif self.typ in ["x_periodic", "box"]:
+            raise Exception(
+                "It makes no sense to tinker with face_connection when there is only one face"
+            )
         else:
             raise NotImplementedError
-            
-    def four_matrix_for_uv(self,fface):
-        '''
-        Expand get_uv_mask_from_face to 2D array of faces. 
-        '''
+
+    def four_matrix_for_uv(self, fface):
+        """Expand get_uv_mask_from_face to 2D array of faces."""
         # apply get_uv_mask for the n*m matrix
-        UfromUvel,UfromVvel,VfromUvel, VfromVvel = [np.zeros(fface.shape) for i in range(4)]
+        UfromUvel, UfromVvel, VfromUvel, VfromVvel = (
+            np.zeros(fface.shape) for i in range(4)
+        )
         for i in range(fface.shape[0]):
-            UfromUvel[i],UfromVvel[i],VfromUvel[i], VfromVvel[i] = self.get_uv_mask_from_face(fface[i])
-        return UfromUvel,UfromVvel,VfromUvel, VfromVvel
+            (
+                UfromUvel[i],
+                UfromVvel[i],
+                VfromUvel[i],
+                VfromVvel[i],
+            ) = self.get_uv_mask_from_face(fface[i])
+        return UfromUvel, UfromVvel, VfromUvel, VfromVvel
```

