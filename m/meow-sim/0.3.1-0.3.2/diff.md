# Comparing `tmp/meow-sim-0.3.1.tar.gz` & `tmp/meow-sim-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meow-sim-0.3.1.tar", last modified: Tue May 23 17:32:38 2023, max compression
+gzip compressed data, was "meow-sim-0.3.2.tar", last modified: Tue May 23 17:35:13 2023, max compression
```

## Comparing `meow-sim-0.3.1.tar` & `meow-sim-0.3.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 17:32:38.393360 meow-sim-0.3.1/
--rw-r--r--   0 root         (0) root         (0)    11347 2023-05-23 17:32:33.000000 meow-sim-0.3.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3178 2023-05-23 17:32:38.393360 meow-sim-0.3.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2060 2023-05-23 17:32:33.000000 meow-sim-0.3.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 17:32:38.389361 meow-sim-0.3.1/meow/
--rw-r--r--   0 root         (0) root         (0)     1414 2023-05-23 17:32:33.000000 meow-sim-0.3.1/meow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 17:32:38.389361 meow-sim-0.3.1/meow/assets/
--rw-r--r--   0 root         (0) root         (0)    10307 2023-05-23 17:32:33.000000 meow-sim-0.3.1/meow/assets/silicon.csv
--rw-r--r--   0 root         (0) root         (0)     8535 2023-05-23 17:32:33.000000 meow-sim-0.3.1/meow/assets/silicon_oxide.csv
--rw-r--r--   0 root         (0) root         (0)     8007 2023-05-23 17:32:33.000000 meow-sim-0.3.1/meow/base_model.py
--rw-r--r--   0 root         (0) root         (0)     1189 2023-05-23 17:32:33.000000 meow-sim-0.3.1/meow/cache.py
--rw-r--r--   0 root         (0) root         (0)     4818 2023-05-23 17:32:33.000000 meow-sim-0.3.1/meow/cell.py
--rw-r--r--   0 root         (0) root         (0)     2783 2023-05-23 17:32:33.000000 meow-sim-0.3.1/meow/cross_section.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 17:32:38.389361 meow-sim-0.3.1/meow/eme/
--rw-r--r--   0 root         (0) root         (0)      623 2023-05-23 17:32:33.000000 meow-sim-0.3.1/meow/eme/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4600 2023-05-23 17:32:33.000000 meow-sim-0.3.1/meow/eme/common.py
--rw-r--r--   0 root         (0) root         (0)     3233 2023-05-23 17:32:33.000000 meow-sim-0.3.1/meow/eme/sax.py
--rw-r--r--   0 root         (0) root         (0)      551 2023-05-23 17:32:33.000000 meow-sim-0.3.1/meow/environment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 17:32:38.389361 meow-sim-0.3.1/meow/fde/
--rw-r--r--   0 root         (0) root         (0)      324 2023-05-23 17:32:33.000000 meow-sim-0.3.1/meow/fde/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3440 2023-05-23 17:32:33.000000 meow-sim-0.3.1/meow/fde/lumerical.py
--rw-r--r--   0 root         (0) root         (0)     2734 2023-05-23 17:32:33.000000 meow-sim-0.3.1/meow/fde/tidy3d.py
--rw-r--r--   0 root         (0) root         (0)     2052 2023-05-23 17:32:33.000000 meow-sim-0.3.1/meow/gds_structures.py
--rw-r--r--   0 root         (0) root         (0)     9211 2023-05-23 17:32:33.000000 meow-sim-0.3.1/meow/geometries.py
--rw-r--r--   0 root         (0) root         (0)      944 2023-05-23 17:32:33.000000 meow-sim-0.3.1/meow/integrate.py
--rw-r--r--   0 root         (0) root         (0)    10785 2023-05-23 17:32:33.000000 meow-sim-0.3.1/meow/materials.py
--rw-r--r--   0 root         (0) root         (0)     3564 2023-05-23 17:32:33.000000 meow-sim-0.3.1/meow/mesh.py
--rw-r--r--   0 root         (0) root         (0)     9814 2023-05-23 17:32:33.000000 meow-sim-0.3.1/meow/mode.py
--rw-r--r--   0 root         (0) root         (0)     1850 2023-05-23 17:32:33.000000 meow-sim-0.3.1/meow/structures.py
--rw-r--r--   0 root         (0) root         (0)     2787 2023-05-23 17:32:33.000000 meow-sim-0.3.1/meow/visualize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 17:32:38.393360 meow-sim-0.3.1/meow_sim.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3178 2023-05-23 17:32:38.000000 meow-sim-0.3.1/meow_sim.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      657 2023-05-23 17:32:38.000000 meow-sim-0.3.1/meow_sim.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 17:32:38.000000 meow-sim-0.3.1/meow_sim.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      385 2023-05-23 17:32:38.000000 meow-sim-0.3.1/meow_sim.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-05-23 17:32:38.000000 meow-sim-0.3.1/meow_sim.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1874 2023-05-23 17:32:33.000000 meow-sim-0.3.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-23 17:32:38.393360 meow-sim-0.3.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 17:32:38.393360 meow-sim-0.3.1/tests/
--rw-r--r--   0 root         (0) root         (0)     4009 2023-05-23 17:32:33.000000 meow-sim-0.3.1/tests/test_deserialization.py
--rw-r--r--   0 root         (0) root         (0)     1322 2023-05-23 17:32:33.000000 meow-sim-0.3.1/tests/test_nbs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 17:35:13.275930 meow-sim-0.3.2/
+-rw-r--r--   0 root         (0) root         (0)    11347 2023-05-23 17:35:07.000000 meow-sim-0.3.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3178 2023-05-23 17:35:13.271930 meow-sim-0.3.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2060 2023-05-23 17:35:07.000000 meow-sim-0.3.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 17:35:13.263930 meow-sim-0.3.2/meow/
+-rw-r--r--   0 root         (0) root         (0)     1414 2023-05-23 17:35:07.000000 meow-sim-0.3.2/meow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 17:35:13.267930 meow-sim-0.3.2/meow/assets/
+-rw-r--r--   0 root         (0) root         (0)    10307 2023-05-23 17:35:07.000000 meow-sim-0.3.2/meow/assets/silicon.csv
+-rw-r--r--   0 root         (0) root         (0)     8535 2023-05-23 17:35:07.000000 meow-sim-0.3.2/meow/assets/silicon_oxide.csv
+-rw-r--r--   0 root         (0) root         (0)     8007 2023-05-23 17:35:07.000000 meow-sim-0.3.2/meow/base_model.py
+-rw-r--r--   0 root         (0) root         (0)     1189 2023-05-23 17:35:07.000000 meow-sim-0.3.2/meow/cache.py
+-rw-r--r--   0 root         (0) root         (0)     4818 2023-05-23 17:35:07.000000 meow-sim-0.3.2/meow/cell.py
+-rw-r--r--   0 root         (0) root         (0)     2783 2023-05-23 17:35:07.000000 meow-sim-0.3.2/meow/cross_section.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 17:35:13.267930 meow-sim-0.3.2/meow/eme/
+-rw-r--r--   0 root         (0) root         (0)      623 2023-05-23 17:35:07.000000 meow-sim-0.3.2/meow/eme/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4600 2023-05-23 17:35:07.000000 meow-sim-0.3.2/meow/eme/common.py
+-rw-r--r--   0 root         (0) root         (0)     3316 2023-05-23 17:35:08.000000 meow-sim-0.3.2/meow/eme/sax.py
+-rw-r--r--   0 root         (0) root         (0)      551 2023-05-23 17:35:08.000000 meow-sim-0.3.2/meow/environment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 17:35:13.267930 meow-sim-0.3.2/meow/fde/
+-rw-r--r--   0 root         (0) root         (0)      324 2023-05-23 17:35:08.000000 meow-sim-0.3.2/meow/fde/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3440 2023-05-23 17:35:08.000000 meow-sim-0.3.2/meow/fde/lumerical.py
+-rw-r--r--   0 root         (0) root         (0)     2734 2023-05-23 17:35:08.000000 meow-sim-0.3.2/meow/fde/tidy3d.py
+-rw-r--r--   0 root         (0) root         (0)     2052 2023-05-23 17:35:08.000000 meow-sim-0.3.2/meow/gds_structures.py
+-rw-r--r--   0 root         (0) root         (0)     9211 2023-05-23 17:35:08.000000 meow-sim-0.3.2/meow/geometries.py
+-rw-r--r--   0 root         (0) root         (0)      944 2023-05-23 17:35:08.000000 meow-sim-0.3.2/meow/integrate.py
+-rw-r--r--   0 root         (0) root         (0)    10785 2023-05-23 17:35:08.000000 meow-sim-0.3.2/meow/materials.py
+-rw-r--r--   0 root         (0) root         (0)     3564 2023-05-23 17:35:08.000000 meow-sim-0.3.2/meow/mesh.py
+-rw-r--r--   0 root         (0) root         (0)     9814 2023-05-23 17:35:08.000000 meow-sim-0.3.2/meow/mode.py
+-rw-r--r--   0 root         (0) root         (0)     1850 2023-05-23 17:35:08.000000 meow-sim-0.3.2/meow/structures.py
+-rw-r--r--   0 root         (0) root         (0)     2787 2023-05-23 17:35:08.000000 meow-sim-0.3.2/meow/visualize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 17:35:13.271930 meow-sim-0.3.2/meow_sim.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3178 2023-05-23 17:35:13.000000 meow-sim-0.3.2/meow_sim.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      657 2023-05-23 17:35:13.000000 meow-sim-0.3.2/meow_sim.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 17:35:13.000000 meow-sim-0.3.2/meow_sim.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      385 2023-05-23 17:35:13.000000 meow-sim-0.3.2/meow_sim.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-05-23 17:35:13.000000 meow-sim-0.3.2/meow_sim.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1874 2023-05-23 17:35:08.000000 meow-sim-0.3.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-23 17:35:13.275930 meow-sim-0.3.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 17:35:13.271930 meow-sim-0.3.2/tests/
+-rw-r--r--   0 root         (0) root         (0)     4009 2023-05-23 17:35:08.000000 meow-sim-0.3.2/tests/test_deserialization.py
+-rw-r--r--   0 root         (0) root         (0)     1322 2023-05-23 17:35:08.000000 meow-sim-0.3.2/tests/test_nbs.py
```

### Comparing `meow-sim-0.3.1/LICENSE` & `meow-sim-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.1/PKG-INFO` & `meow-sim-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow-sim
-Version: 0.3.1
+Version: 0.3.2
 Summary: Modeling of Eigenmodes and Overlaps in Waveguide Structures
 Author: Rockley Photonics
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 License: Apache Software License
 Keywords: eigenmodes,eme,fde,modeling,overlaps,photonics,waveguides
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `meow-sim-0.3.1/README.md` & `meow-sim-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.1/meow/__init__.py` & `meow-sim-0.3.2/meow/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """ MEOW: Modeling of Eigenmodes and Overlaps in Waveguides """
 
 __author__ = "Floris Laporte"
-__version__ = "0.3.1"
+__version__ = "0.3.2"
 
 import warnings
 
 # Silence Excessive Logging...
 
 try:
     from loguru import logger
```

### Comparing `meow-sim-0.3.1/meow/assets/silicon.csv` & `meow-sim-0.3.2/meow/assets/silicon.csv`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.1/meow/assets/silicon_oxide.csv` & `meow-sim-0.3.2/meow/assets/silicon_oxide.csv`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.1/meow/base_model.py` & `meow-sim-0.3.2/meow/base_model.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.1/meow/cache.py` & `meow-sim-0.3.2/meow/cache.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.1/meow/cell.py` & `meow-sim-0.3.2/meow/cell.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.1/meow/cross_section.py` & `meow-sim-0.3.2/meow/cross_section.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.1/meow/eme/__init__.py` & `meow-sim-0.3.2/meow/eme/__init__.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.1/meow/eme/common.py` & `meow-sim-0.3.2/meow/eme/common.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.1/meow/eme/sax.py` & `meow-sim-0.3.2/meow/eme/sax.py`

 * *Files 10% similar despite different names*

```diff
@@ -67,28 +67,29 @@
 ):
     """Calculate the S-matrix for given sets of modes, each set belonging to a `Cell`
 
     Args:
         modes: Each collection of modes for each of the `Cell` objects
         backend: which SAX backend to use to calculate the final S-matrix.
     """
-    sax_backend = _validate_sax_backend(sax_backend)
-    get_interface_s_matrices_ = kwargs.pop(
-        "get_interface_s_matrices", compute_interface_s_matrices
-    )
-    get_interface_s_matrices = partial(get_interface_s_matrices_, **kwargs)
-
     num_modes = len(modes[0])
     mode_names = [f"{i}" for i in range(num_modes)]
-
-    propagations = compute_propagation_s_matrices(modes)
-    interfaces = get_interface_s_matrices(
+    sax_backend = _validate_sax_backend(sax_backend)
+    _compute_propagation_s_matrices = kwargs.pop(
+        "compute_propagation_s_matrices", compute_propagation_s_matrices
+    )
+    _compute_interface_s_matrices = kwargs.pop(
+        "compute_interface_s_matrices", compute_interface_s_matrices
+    )
+    propagations = _compute_propagation_s_matrices(modes)
+    interfaces = _compute_interface_s_matrices(
         modes,
         enforce_reciprocity=enforce_reciprocity,
         enforce_lossy_unitarity=enforce_lossy_unitarity,
+        **kwargs,
     )
 
     # TODO: fix SAX Multimode to reduce this ad-hoc SAX-hacking.
     net = _get_netlist(propagations, interfaces)
     models = net["instances"]
     net["instances"] = {k: k for k in net["instances"]}
     net = Netlist(**net)
```

### Comparing `meow-sim-0.3.1/meow/environment.py` & `meow-sim-0.3.2/meow/environment.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.1/meow/fde/lumerical.py` & `meow-sim-0.3.2/meow/fde/lumerical.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.1/meow/fde/tidy3d.py` & `meow-sim-0.3.2/meow/fde/tidy3d.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.1/meow/gds_structures.py` & `meow-sim-0.3.2/meow/gds_structures.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.1/meow/geometries.py` & `meow-sim-0.3.2/meow/geometries.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.1/meow/integrate.py` & `meow-sim-0.3.2/meow/integrate.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.1/meow/materials.py` & `meow-sim-0.3.2/meow/materials.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.1/meow/mesh.py` & `meow-sim-0.3.2/meow/mesh.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.1/meow/mode.py` & `meow-sim-0.3.2/meow/mode.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.1/meow/structures.py` & `meow-sim-0.3.2/meow/structures.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.1/meow/visualize.py` & `meow-sim-0.3.2/meow/visualize.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.1/meow_sim.egg-info/PKG-INFO` & `meow-sim-0.3.2/meow_sim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow-sim
-Version: 0.3.1
+Version: 0.3.2
 Summary: Modeling of Eigenmodes and Overlaps in Waveguide Structures
 Author: Rockley Photonics
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 License: Apache Software License
 Keywords: eigenmodes,eme,fde,modeling,overlaps,photonics,waveguides
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `meow-sim-0.3.1/meow_sim.egg-info/SOURCES.txt` & `meow-sim-0.3.2/meow_sim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.1/pyproject.toml` & `meow-sim-0.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["build", "pip", "setuptools", "wheel", "pybind11"]
 
 [project]
 name = "meow-sim"
-version = "0.3.1"
+version = "0.3.2"
 authors = [
 { name = "Rockley Photonics" },
 { name = "Floris Laporte", email = "floris.laporte@rockleyphotonics.com" },
 ]
 description = "Modeling of Eigenmodes and Overlaps in Waveguide Structures"
 requires-python = ">=3.8"
 keywords = [
```

### Comparing `meow-sim-0.3.1/tests/test_deserialization.py` & `meow-sim-0.3.2/tests/test_deserialization.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.1/tests/test_nbs.py` & `meow-sim-0.3.2/tests/test_nbs.py`

 * *Files identical despite different names*

