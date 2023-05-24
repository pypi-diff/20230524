# Comparing `tmp/light_size_constrained_clustering-0.0.1.tar.gz` & `tmp/light_size_constrained_clustering-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "light_size_constrained_clustering-0.0.1.tar", last modified: Wed May 24 20:47:07 2023, max compression
+gzip compressed data, was "light_size_constrained_clustering-0.0.2.tar", last modified: Wed May 24 20:51:38 2023, max compression
```

## Comparing `light_size_constrained_clustering-0.0.1.tar` & `light_size_constrained_clustering-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 i0365030   (502) staff       (20)        0 2023-05-24 20:47:07.531952 light_size_constrained_clustering-0.0.1/
--rw-r--r--   0 i0365030   (502) staff       (20)     1074 2023-05-24 18:28:58.000000 light_size_constrained_clustering-0.0.1/LICENSE
--rw-r--r--   0 i0365030   (502) staff       (20)     3640 2023-05-24 20:47:07.531793 light_size_constrained_clustering-0.0.1/PKG-INFO
--rw-r--r--   0 i0365030   (502) staff       (20)     3293 2023-05-24 20:44:12.000000 light_size_constrained_clustering-0.0.1/README.md
-drwxr-xr-x   0 i0365030   (502) staff       (20)        0 2023-05-24 20:47:07.527739 light_size_constrained_clustering-0.0.1/light_size_constrained_clustering/
--rw-r--r--   0 i0365030   (502) staff       (20)      106 2023-05-24 20:33:58.000000 light_size_constrained_clustering-0.0.1/light_size_constrained_clustering/__init__.py
--rw-r--r--   0 i0365030   (502) staff       (20)     6178 2023-05-24 20:40:01.000000 light_size_constrained_clustering-0.0.1/light_size_constrained_clustering/base.py
--rw-r--r--   0 i0365030   (502) staff       (20)     6668 2023-05-24 20:18:18.000000 light_size_constrained_clustering-0.0.1/light_size_constrained_clustering/da.py
-drwxr-xr-x   0 i0365030   (502) staff       (20)        0 2023-05-24 20:47:07.530946 light_size_constrained_clustering-0.0.1/light_size_constrained_clustering.egg-info/
--rw-r--r--   0 i0365030   (502) staff       (20)     3640 2023-05-24 20:47:07.000000 light_size_constrained_clustering-0.0.1/light_size_constrained_clustering.egg-info/PKG-INFO
--rw-r--r--   0 i0365030   (502) staff       (20)      455 2023-05-24 20:47:07.000000 light_size_constrained_clustering-0.0.1/light_size_constrained_clustering.egg-info/SOURCES.txt
--rw-r--r--   0 i0365030   (502) staff       (20)        1 2023-05-24 20:47:07.000000 light_size_constrained_clustering-0.0.1/light_size_constrained_clustering.egg-info/dependency_links.txt
--rw-r--r--   0 i0365030   (502) staff       (20)      106 2023-05-24 20:47:07.000000 light_size_constrained_clustering-0.0.1/light_size_constrained_clustering.egg-info/requires.txt
--rw-r--r--   0 i0365030   (502) staff       (20)       34 2023-05-24 20:47:07.000000 light_size_constrained_clustering-0.0.1/light_size_constrained_clustering.egg-info/top_level.txt
--rw-r--r--   0 i0365030   (502) staff       (20)       38 2023-05-24 20:47:07.532003 light_size_constrained_clustering-0.0.1/setup.cfg
--rw-r--r--   0 i0365030   (502) staff       (20)     1312 2023-05-24 20:46:51.000000 light_size_constrained_clustering-0.0.1/setup.py
-drwxr-xr-x   0 i0365030   (502) staff       (20)        0 2023-05-24 20:47:07.531308 light_size_constrained_clustering-0.0.1/tests/
--rw-r--r--   0 i0365030   (502) staff       (20)     1341 2023-05-24 20:41:53.000000 light_size_constrained_clustering-0.0.1/tests/test_da.py
+drwxr-xr-x   0 i0365030   (502) staff       (20)        0 2023-05-24 20:51:38.716120 light_size_constrained_clustering-0.0.2/
+-rw-r--r--   0 i0365030   (502) staff       (20)     1074 2023-05-24 18:28:58.000000 light_size_constrained_clustering-0.0.2/LICENSE
+-rw-r--r--   0 i0365030   (502) staff       (20)     3646 2023-05-24 20:51:38.715961 light_size_constrained_clustering-0.0.2/PKG-INFO
+-rw-r--r--   0 i0365030   (502) staff       (20)     3299 2023-05-24 20:51:17.000000 light_size_constrained_clustering-0.0.2/README.md
+drwxr-xr-x   0 i0365030   (502) staff       (20)        0 2023-05-24 20:51:38.714551 light_size_constrained_clustering-0.0.2/light_size_constrained_clustering/
+-rw-r--r--   0 i0365030   (502) staff       (20)      106 2023-05-24 20:33:58.000000 light_size_constrained_clustering-0.0.2/light_size_constrained_clustering/__init__.py
+-rw-r--r--   0 i0365030   (502) staff       (20)     6178 2023-05-24 20:40:01.000000 light_size_constrained_clustering-0.0.2/light_size_constrained_clustering/base.py
+-rw-r--r--   0 i0365030   (502) staff       (20)     6668 2023-05-24 20:18:18.000000 light_size_constrained_clustering-0.0.2/light_size_constrained_clustering/da.py
+drwxr-xr-x   0 i0365030   (502) staff       (20)        0 2023-05-24 20:51:38.715514 light_size_constrained_clustering-0.0.2/light_size_constrained_clustering.egg-info/
+-rw-r--r--   0 i0365030   (502) staff       (20)     3646 2023-05-24 20:51:38.000000 light_size_constrained_clustering-0.0.2/light_size_constrained_clustering.egg-info/PKG-INFO
+-rw-r--r--   0 i0365030   (502) staff       (20)      455 2023-05-24 20:51:38.000000 light_size_constrained_clustering-0.0.2/light_size_constrained_clustering.egg-info/SOURCES.txt
+-rw-r--r--   0 i0365030   (502) staff       (20)        1 2023-05-24 20:51:38.000000 light_size_constrained_clustering-0.0.2/light_size_constrained_clustering.egg-info/dependency_links.txt
+-rw-r--r--   0 i0365030   (502) staff       (20)      106 2023-05-24 20:51:38.000000 light_size_constrained_clustering-0.0.2/light_size_constrained_clustering.egg-info/requires.txt
+-rw-r--r--   0 i0365030   (502) staff       (20)       34 2023-05-24 20:51:38.000000 light_size_constrained_clustering-0.0.2/light_size_constrained_clustering.egg-info/top_level.txt
+-rw-r--r--   0 i0365030   (502) staff       (20)       38 2023-05-24 20:51:38.716167 light_size_constrained_clustering-0.0.2/setup.cfg
+-rw-r--r--   0 i0365030   (502) staff       (20)     1312 2023-05-24 20:51:23.000000 light_size_constrained_clustering-0.0.2/setup.py
+drwxr-xr-x   0 i0365030   (502) staff       (20)        0 2023-05-24 20:51:38.715634 light_size_constrained_clustering-0.0.2/tests/
+-rw-r--r--   0 i0365030   (502) staff       (20)     1341 2023-05-24 20:41:53.000000 light_size_constrained_clustering-0.0.2/tests/test_da.py
```

### Comparing `light_size_constrained_clustering-0.0.1/LICENSE` & `light_size_constrained_clustering-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `light_size_constrained_clustering-0.0.1/PKG-INFO` & `light_size_constrained_clustering-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: light_size_constrained_clustering
-Version: 0.0.1
+Version: 0.0.2
 Summary: Size Constrained Clustering solver
 Home-page: https://github.com/AlbertPlaPlanas/size_constrained_clustering
 Author: Albert Pla
 Author-email: plaalbert@gmail.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -24,15 +24,15 @@
 
 This is a fork of https://github.com/jingw2/size_constrained_clustering that solves installation issues. And mantains only the Determinstic Annealing clustering.
 
 ### Installation
 Requirement Python >= 3.6, Numpy >= 1.13, Cython >= 0.29
 * install from PyPI
 ```shell
-pip install size-constrained-clustering
+pip install light-size-constrained-clustering
 ```
 
 ### Methods
 * Deterministic Annealling Algorithm: Input target cluster distribution, return correspondent clusters
 
 ### Usage:
```

### Comparing `light_size_constrained_clustering-0.0.1/README.md` & `light_size_constrained_clustering-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 This is a fork of https://github.com/jingw2/size_constrained_clustering that solves installation issues. And mantains only the Determinstic Annealing clustering.
 
 ### Installation
 Requirement Python >= 3.6, Numpy >= 1.13, Cython >= 0.29
 * install from PyPI
 ```shell
-pip install size-constrained-clustering
+pip install light-size-constrained-clustering
 ```
 
 ### Methods
 * Deterministic Annealling Algorithm: Input target cluster distribution, return correspondent clusters
 
 ### Usage:
```

### Comparing `light_size_constrained_clustering-0.0.1/light_size_constrained_clustering/base.py` & `light_size_constrained_clustering-0.0.2/light_size_constrained_clustering/base.py`

 * *Files identical despite different names*

### Comparing `light_size_constrained_clustering-0.0.1/light_size_constrained_clustering/da.py` & `light_size_constrained_clustering-0.0.2/light_size_constrained_clustering/da.py`

 * *Files identical despite different names*

### Comparing `light_size_constrained_clustering-0.0.1/light_size_constrained_clustering.egg-info/PKG-INFO` & `light_size_constrained_clustering-0.0.2/light_size_constrained_clustering.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: light-size-constrained-clustering
-Version: 0.0.1
+Version: 0.0.2
 Summary: Size Constrained Clustering solver
 Home-page: https://github.com/AlbertPlaPlanas/size_constrained_clustering
 Author: Albert Pla
 Author-email: plaalbert@gmail.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -24,15 +24,15 @@
 
 This is a fork of https://github.com/jingw2/size_constrained_clustering that solves installation issues. And mantains only the Determinstic Annealing clustering.
 
 ### Installation
 Requirement Python >= 3.6, Numpy >= 1.13, Cython >= 0.29
 * install from PyPI
 ```shell
-pip install size-constrained-clustering
+pip install light-size-constrained-clustering
 ```
 
 ### Methods
 * Deterministic Annealling Algorithm: Input target cluster distribution, return correspondent clusters
 
 ### Usage:
```

### Comparing `light_size_constrained_clustering-0.0.1/setup.py` & `light_size_constrained_clustering-0.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 path = os.path.dirname(os.path.abspath(__file__))
 
 with open(os.path.join(path, "requirements.txt")) as fp:
     install_requires = fp.read().strip().split("\n")
 
 
-VERSION = "0.0.1"
+VERSION = "0.0.2"
 LICENSE = "MIT"
 setup(
     #ext_modules=extensions,
     version=VERSION,
     setup_requires=["numpy"],
     install_requires=install_requires,
     name="light_size_constrained_clustering",
```

### Comparing `light_size_constrained_clustering-0.0.1/tests/test_da.py` & `light_size_constrained_clustering-0.0.2/tests/test_da.py`

 * *Files identical despite different names*

