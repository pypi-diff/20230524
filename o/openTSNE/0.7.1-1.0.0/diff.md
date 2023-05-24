# Comparing `tmp/openTSNE-0.7.1.tar.gz` & `tmp/openTSNE-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openTSNE-0.7.1.tar", last modified: Mon Feb 20 15:29:04 2023, max compression
+gzip compressed data, was "openTSNE-1.0.0.tar", last modified: Wed May 24 14:00:30 2023, max compression
```

## Comparing `openTSNE-0.7.1.tar` & `openTSNE-1.0.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-02-20 15:29:04.613107 openTSNE-0.7.1/
--rw-r--r--   0 vsts      (1001) docker     (123)     1515 2023-02-20 15:28:43.000000 openTSNE-0.7.1/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (123)      139 2023-02-20 15:28:43.000000 openTSNE-0.7.1/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (123)     7693 2023-02-20 15:29:04.609107 openTSNE-0.7.1/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     6462 2023-02-20 15:28:43.000000 openTSNE-0.7.1/README.rst
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-02-20 15:29:04.597106 openTSNE-0.7.1/docs/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-02-20 15:29:04.597106 openTSNE-0.7.1/docs/source/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-02-20 15:29:04.597106 openTSNE-0.7.1/docs/source/images/
--rw-r--r--   0 vsts      (1001) docker     (123)   163220 2023-02-20 15:28:43.000000 openTSNE-0.7.1/docs/source/images/macosko_2015.png
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-02-20 15:29:04.605106 openTSNE-0.7.1/openTSNE/
--rw-r--r--   0 vsts      (1001) docker     (123)      116 2023-02-20 15:28:43.000000 openTSNE-0.7.1/openTSNE/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-02-20 15:29:04.609107 openTSNE-0.7.1/openTSNE/_matrix_mul/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-02-20 15:28:43.000000 openTSNE-0.7.1/openTSNE/_matrix_mul/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      426 2023-02-20 15:28:43.000000 openTSNE-0.7.1/openTSNE/_matrix_mul/matrix_mul.pxd
--rw-r--r--   0 vsts      (1001) docker     (123)     7908 2023-02-20 15:28:43.000000 openTSNE-0.7.1/openTSNE/_matrix_mul/matrix_mul_fftw3.pyx
--rw-r--r--   0 vsts      (1001) docker     (123)   977668 2023-02-20 15:29:01.000000 openTSNE-0.7.1/openTSNE/_matrix_mul/matrix_mul_numpy.cpp
--rw-r--r--   0 vsts      (1001) docker     (123)     5551 2023-02-20 15:28:43.000000 openTSNE-0.7.1/openTSNE/_matrix_mul/matrix_mul_numpy.pyx
--rw-r--r--   0 vsts      (1001) docker     (123)  1725878 2023-02-20 15:29:02.000000 openTSNE-0.7.1/openTSNE/_tsne.cpp
--rw-r--r--   0 vsts      (1001) docker     (123)     2553 2023-02-20 15:28:43.000000 openTSNE-0.7.1/openTSNE/_tsne.pxd
--rw-r--r--   0 vsts      (1001) docker     (123)    48417 2023-02-20 15:28:43.000000 openTSNE-0.7.1/openTSNE/_tsne.pyx
--rw-r--r--   0 vsts      (1001) docker     (123)    46010 2023-02-20 15:28:43.000000 openTSNE-0.7.1/openTSNE/affinity.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3962 2023-02-20 15:28:43.000000 openTSNE-0.7.1/openTSNE/callbacks.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-02-20 15:29:04.609107 openTSNE-0.7.1/openTSNE/dependencies/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-02-20 15:28:43.000000 openTSNE-0.7.1/openTSNE/dependencies/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-02-20 15:29:04.609107 openTSNE-0.7.1/openTSNE/dependencies/annoy/
--rw-r--r--   0 vsts      (1001) docker     (123)       42 2023-02-20 15:28:43.000000 openTSNE-0.7.1/openTSNE/dependencies/annoy/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    45053 2023-02-20 15:28:43.000000 openTSNE-0.7.1/openTSNE/dependencies/annoy/annoylib.h
--rw-r--r--   0 vsts      (1001) docker     (123)    20645 2023-02-20 15:28:43.000000 openTSNE-0.7.1/openTSNE/dependencies/annoy/annoymodule.cc
--rw-r--r--   0 vsts      (1001) docker     (123)     2365 2023-02-20 15:28:43.000000 openTSNE-0.7.1/openTSNE/dependencies/annoy/kissrandom.h
--rw-r--r--   0 vsts      (1001) docker     (123)     5791 2023-02-20 15:28:43.000000 openTSNE-0.7.1/openTSNE/dependencies/annoy/mman.h
--rw-r--r--   0 vsts      (1001) docker     (123)     7606 2023-02-20 15:28:43.000000 openTSNE-0.7.1/openTSNE/initialization.py
--rw-r--r--   0 vsts      (1001) docker     (123)  1017785 2023-02-20 15:29:03.000000 openTSNE-0.7.1/openTSNE/kl_divergence.cpp
--rw-r--r--   0 vsts      (1001) docker     (123)     4079 2023-02-20 15:28:43.000000 openTSNE-0.7.1/openTSNE/kl_divergence.pyx
--rw-r--r--   0 vsts      (1001) docker     (123)      401 2023-02-20 15:28:43.000000 openTSNE-0.7.1/openTSNE/metrics.py
--rw-r--r--   0 vsts      (1001) docker     (123)    22656 2023-02-20 15:28:43.000000 openTSNE-0.7.1/openTSNE/nearest_neighbors.py
--rw-r--r--   0 vsts      (1001) docker     (123)   845094 2023-02-20 15:29:04.000000 openTSNE-0.7.1/openTSNE/quad_tree.cpp
--rw-r--r--   0 vsts      (1001) docker     (123)      537 2023-02-20 15:28:43.000000 openTSNE-0.7.1/openTSNE/quad_tree.pxd
--rw-r--r--   0 vsts      (1001) docker     (123)     5949 2023-02-20 15:28:43.000000 openTSNE-0.7.1/openTSNE/quad_tree.pyx
--rw-r--r--   0 vsts      (1001) docker     (123)     1380 2023-02-20 15:28:43.000000 openTSNE-0.7.1/openTSNE/sklearn.py
--rw-r--r--   0 vsts      (1001) docker     (123)    74784 2023-02-20 15:28:43.000000 openTSNE-0.7.1/openTSNE/tsne.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1531 2023-02-20 15:28:43.000000 openTSNE-0.7.1/openTSNE/utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)       22 2023-02-20 15:28:43.000000 openTSNE-0.7.1/openTSNE/version.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-02-20 15:29:04.609107 openTSNE-0.7.1/openTSNE.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     7693 2023-02-20 15:28:59.000000 openTSNE-0.7.1/openTSNE.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     1255 2023-02-20 15:29:04.000000 openTSNE-0.7.1/openTSNE.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-02-20 15:28:59.000000 openTSNE-0.7.1/openTSNE.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       96 2023-02-20 15:28:59.000000 openTSNE-0.7.1/openTSNE.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        9 2023-02-20 15:28:59.000000 openTSNE-0.7.1/openTSNE.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (123)      126 2023-02-20 15:28:43.000000 openTSNE-0.7.1/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-02-20 15:29:04.613107 openTSNE-0.7.1/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)    10750 2023-02-20 15:28:43.000000 openTSNE-0.7.1/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-02-20 15:29:04.609107 openTSNE-0.7.1/tests/
--rw-r--r--   0 vsts      (1001) docker     (123)    14954 2023-02-20 15:28:43.000000 openTSNE-0.7.1/tests/test_affinities.py
--rw-r--r--   0 vsts      (1001) docker     (123)    14174 2023-02-20 15:28:43.000000 openTSNE-0.7.1/tests/test_correctness.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9729 2023-02-20 15:28:43.000000 openTSNE-0.7.1/tests/test_different_usages.py
--rw-r--r--   0 vsts      (1001) docker     (123)    16289 2023-02-20 15:28:43.000000 openTSNE-0.7.1/tests/test_nearest_neighbors.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1036 2023-02-20 15:28:43.000000 openTSNE-0.7.1/tests/test_sklearn_wrapper.py
--rw-r--r--   0 vsts      (1001) docker     (123)    39230 2023-02-20 15:28:43.000000 openTSNE-0.7.1/tests/test_tsne.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1038 2023-02-20 15:28:43.000000 openTSNE-0.7.1/tests/test_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-24 14:00:30.453655 openTSNE-1.0.0/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1515 2023-05-24 14:00:10.000000 openTSNE-1.0.0/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (123)      139 2023-05-24 14:00:10.000000 openTSNE-1.0.0/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (123)     7693 2023-05-24 14:00:30.453655 openTSNE-1.0.0/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     6462 2023-05-24 14:00:10.000000 openTSNE-1.0.0/README.rst
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-24 14:00:30.441655 openTSNE-1.0.0/docs/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-24 14:00:30.441655 openTSNE-1.0.0/docs/source/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-24 14:00:30.441655 openTSNE-1.0.0/docs/source/images/
+-rw-r--r--   0 vsts      (1001) docker     (123)   163220 2023-05-24 14:00:10.000000 openTSNE-1.0.0/docs/source/images/macosko_2015.png
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-24 14:00:30.449655 openTSNE-1.0.0/openTSNE/
+-rw-r--r--   0 vsts      (1001) docker     (123)      116 2023-05-24 14:00:11.000000 openTSNE-1.0.0/openTSNE/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-24 14:00:30.449655 openTSNE-1.0.0/openTSNE/_matrix_mul/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-24 14:00:11.000000 openTSNE-1.0.0/openTSNE/_matrix_mul/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      426 2023-05-24 14:00:11.000000 openTSNE-1.0.0/openTSNE/_matrix_mul/matrix_mul.pxd
+-rw-r--r--   0 vsts      (1001) docker     (123)     7908 2023-05-24 14:00:11.000000 openTSNE-1.0.0/openTSNE/_matrix_mul/matrix_mul_fftw3.pyx
+-rw-r--r--   0 vsts      (1001) docker     (123)   900688 2023-05-24 14:00:26.000000 openTSNE-1.0.0/openTSNE/_matrix_mul/matrix_mul_numpy.cpp
+-rw-r--r--   0 vsts      (1001) docker     (123)     5551 2023-05-24 14:00:11.000000 openTSNE-1.0.0/openTSNE/_matrix_mul/matrix_mul_numpy.pyx
+-rw-r--r--   0 vsts      (1001) docker     (123)  1650125 2023-05-24 14:00:28.000000 openTSNE-1.0.0/openTSNE/_tsne.cpp
+-rw-r--r--   0 vsts      (1001) docker     (123)     2553 2023-05-24 14:00:11.000000 openTSNE-1.0.0/openTSNE/_tsne.pxd
+-rw-r--r--   0 vsts      (1001) docker     (123)    48417 2023-05-24 14:00:11.000000 openTSNE-1.0.0/openTSNE/_tsne.pyx
+-rw-r--r--   0 vsts      (1001) docker     (123)    47710 2023-05-24 14:00:11.000000 openTSNE-1.0.0/openTSNE/affinity.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3962 2023-05-24 14:00:11.000000 openTSNE-1.0.0/openTSNE/callbacks.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-24 14:00:30.449655 openTSNE-1.0.0/openTSNE/dependencies/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-24 14:00:11.000000 openTSNE-1.0.0/openTSNE/dependencies/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-24 14:00:30.449655 openTSNE-1.0.0/openTSNE/dependencies/annoy/
+-rw-r--r--   0 vsts      (1001) docker     (123)       42 2023-05-24 14:00:11.000000 openTSNE-1.0.0/openTSNE/dependencies/annoy/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    45053 2023-05-24 14:00:11.000000 openTSNE-1.0.0/openTSNE/dependencies/annoy/annoylib.h
+-rw-r--r--   0 vsts      (1001) docker     (123)    20645 2023-05-24 14:00:11.000000 openTSNE-1.0.0/openTSNE/dependencies/annoy/annoymodule.cc
+-rw-r--r--   0 vsts      (1001) docker     (123)     2365 2023-05-24 14:00:11.000000 openTSNE-1.0.0/openTSNE/dependencies/annoy/kissrandom.h
+-rw-r--r--   0 vsts      (1001) docker     (123)     5791 2023-05-24 14:00:11.000000 openTSNE-1.0.0/openTSNE/dependencies/annoy/mman.h
+-rw-r--r--   0 vsts      (1001) docker     (123)     7606 2023-05-24 14:00:11.000000 openTSNE-1.0.0/openTSNE/initialization.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   940883 2023-05-24 14:00:29.000000 openTSNE-1.0.0/openTSNE/kl_divergence.cpp
+-rw-r--r--   0 vsts      (1001) docker     (123)     4079 2023-05-24 14:00:11.000000 openTSNE-1.0.0/openTSNE/kl_divergence.pyx
+-rw-r--r--   0 vsts      (1001) docker     (123)      401 2023-05-24 14:00:11.000000 openTSNE-1.0.0/openTSNE/metrics.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    22824 2023-05-24 14:00:11.000000 openTSNE-1.0.0/openTSNE/nearest_neighbors.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   845157 2023-05-24 14:00:30.000000 openTSNE-1.0.0/openTSNE/quad_tree.cpp
+-rw-r--r--   0 vsts      (1001) docker     (123)      537 2023-05-24 14:00:11.000000 openTSNE-1.0.0/openTSNE/quad_tree.pxd
+-rw-r--r--   0 vsts      (1001) docker     (123)     5949 2023-05-24 14:00:11.000000 openTSNE-1.0.0/openTSNE/quad_tree.pyx
+-rw-r--r--   0 vsts      (1001) docker     (123)     1380 2023-05-24 14:00:11.000000 openTSNE-1.0.0/openTSNE/sklearn.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    74784 2023-05-24 14:00:11.000000 openTSNE-1.0.0/openTSNE/tsne.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1531 2023-05-24 14:00:11.000000 openTSNE-1.0.0/openTSNE/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)       22 2023-05-24 14:00:11.000000 openTSNE-1.0.0/openTSNE/version.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-24 14:00:30.449655 openTSNE-1.0.0/openTSNE.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     7693 2023-05-24 14:00:25.000000 openTSNE-1.0.0/openTSNE.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     1255 2023-05-24 14:00:30.000000 openTSNE-1.0.0/openTSNE.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-24 14:00:25.000000 openTSNE-1.0.0/openTSNE.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       96 2023-05-24 14:00:25.000000 openTSNE-1.0.0/openTSNE.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        9 2023-05-24 14:00:25.000000 openTSNE-1.0.0/openTSNE.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)      126 2023-05-24 14:00:11.000000 openTSNE-1.0.0/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-24 14:00:30.453655 openTSNE-1.0.0/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)    10750 2023-05-24 14:00:11.000000 openTSNE-1.0.0/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-24 14:00:30.453655 openTSNE-1.0.0/tests/
+-rw-r--r--   0 vsts      (1001) docker     (123)    15623 2023-05-24 14:00:11.000000 openTSNE-1.0.0/tests/test_affinities.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    14174 2023-05-24 14:00:11.000000 openTSNE-1.0.0/tests/test_correctness.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9729 2023-05-24 14:00:11.000000 openTSNE-1.0.0/tests/test_different_usages.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    16289 2023-05-24 14:00:11.000000 openTSNE-1.0.0/tests/test_nearest_neighbors.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1036 2023-05-24 14:00:11.000000 openTSNE-1.0.0/tests/test_sklearn_wrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    39230 2023-05-24 14:00:11.000000 openTSNE-1.0.0/tests/test_tsne.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1038 2023-05-24 14:00:11.000000 openTSNE-1.0.0/tests/test_utils.py
```

### Comparing `openTSNE-0.7.1/LICENSE` & `openTSNE-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openTSNE-0.7.1/PKG-INFO` & `openTSNE-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openTSNE
-Version: 0.7.1
+Version: 1.0.0
 Summary: Extensible, parallel implementations of t-SNE
 Home-page: https://github.com/pavlin-policar/openTSNE
 Author: Pavlin Poličar
 Author-email: pavlin.g.p@gmail.com
 License: BSD-3-Clause
 Project-URL: Documentation, https://opentsne.readthedocs.io/
 Project-URL: Source, https://github.com/pavlin-policar/openTSNE
```

### Comparing `openTSNE-0.7.1/README.rst` & `openTSNE-1.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `openTSNE-0.7.1/docs/source/images/macosko_2015.png` & `openTSNE-1.0.0/docs/source/images/macosko_2015.png`

 * *Files identical despite different names*

### Comparing `openTSNE-0.7.1/openTSNE/_matrix_mul/matrix_mul_fftw3.pyx` & `openTSNE-1.0.0/openTSNE/_matrix_mul/matrix_mul_fftw3.pyx`

 * *Files identical despite different names*

### Comparing `openTSNE-0.7.1/openTSNE/_matrix_mul/matrix_mul_numpy.cpp` & `openTSNE-1.0.0/openTSNE/_matrix_mul/matrix_mul_numpy.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "language": "c++",
         "name": "openTSNE._matrix_mul.matrix_mul",
@@ -19,16 +19,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_33"
-#define CYTHON_HEX_VERSION 0x001D21F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -213,15 +213,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -252,15 +252,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -768,15 +768,21 @@
 
 #define __PYX_HAVE__openTSNE___matrix_mul__matrix_mul
 #define __PYX_HAVE_API__openTSNE___matrix_mul__matrix_mul
 /* Early includes */
 #include <string.h>
 #include <stdio.h>
 #include "numpy/arrayobject.h"
+#include "numpy/ndarrayobject.h"
+#include "numpy/ndarraytypes.h"
+#include "numpy/arrayscalars.h"
 #include "numpy/ufuncobject.h"
+
+    /* NumPy API declarations from "numpy/__init__.pxd" */
+    
 #include "pythread.h"
 #include <stdlib.h>
 #include "pystate.h"
 #ifdef _OPENMP
 #include <omp.h>
 #endif /* _OPENMP */
 
@@ -1113,195 +1119,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":775
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":690
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":776
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":691
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":777
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":778
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":693
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":782
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":697
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":783
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":698
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":784
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":785
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":700
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":789
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":704
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":790
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":705
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":799
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":714
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":800
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":715
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":801
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":716
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":803
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":804
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":805
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":720
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":807
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":722
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":808
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":723
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":810
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":811
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":812
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1332,42 +1338,42 @@
 
 /*--- Type declarations ---*/
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":814
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":815
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":730
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":816
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":818
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":733
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -1737,40 +1743,14 @@
 #endif
 
 /* WriteUnraisableException.proto */
 static void __Pyx_WriteUnraisable(const char *name, int clineno,
                                   int lineno, const char *filename,
                                   int full_traceback, int nogil);
 
-/* RaiseException.proto */
-static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
-
-/* DictGetItem.proto */
-#if PY_MAJOR_VERSION >= 3 && !CYTHON_COMPILING_IN_PYPY
-static PyObject *__Pyx_PyDict_GetItem(PyObject *d, PyObject* key);
-#define __Pyx_PyObject_Dict_GetItem(obj, name)\
-    (likely(PyDict_CheckExact(obj)) ?\
-     __Pyx_PyDict_GetItem(obj, name) : PyObject_GetItem(obj, name))
-#else
-#define __Pyx_PyDict_GetItem(d, key) PyObject_GetItem(d, key)
-#define __Pyx_PyObject_Dict_GetItem(obj, name)  PyObject_GetItem(obj, name)
-#endif
-
-/* RaiseTooManyValuesToUnpack.proto */
-static CYTHON_INLINE void __Pyx_RaiseTooManyValuesError(Py_ssize_t expected);
-
-/* RaiseNeedMoreValuesToUnpack.proto */
-static CYTHON_INLINE void __Pyx_RaiseNeedMoreValuesError(Py_ssize_t index);
-
-/* RaiseNoneIterError.proto */
-static CYTHON_INLINE void __Pyx_RaiseNoneNotIterableError(void);
-
-/* ExtTypeTest.proto */
-static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type);
-
 /* GetTopmostException.proto */
 #if CYTHON_USE_EXC_INFO_STACK
 static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
 #endif
 
 /* SaveResetException.proto */
 #if CYTHON_FAST_THREAD_STATE
@@ -1795,14 +1775,17 @@
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_GetException(type, value, tb)  __Pyx__GetException(__pyx_tstate, type, value, tb)
 static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
 #else
 static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb);
 #endif
 
+/* RaiseException.proto */
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
+
 /* RaiseArgTupleInvalid.proto */
 static void __Pyx_RaiseArgtupleInvalid(const char* func_name, int exact,
     Py_ssize_t num_min, Py_ssize_t num_max, Py_ssize_t num_found);
 
 /* RaiseDoubleKeywords.proto */
 static void __Pyx_RaiseDoubleKeywordsError(const char* func_name, PyObject* kw_name);
 
@@ -1890,14 +1873,26 @@
          const char* cstring, Py_ssize_t start, Py_ssize_t stop,
          const char* encoding, const char* errors,
          PyObject* (*decode_func)(const char *s, Py_ssize_t size, const char *errors));
 
 /* GetAttr3.proto */
 static CYTHON_INLINE PyObject *__Pyx_GetAttr3(PyObject *, PyObject *, PyObject *);
 
+/* RaiseTooManyValuesToUnpack.proto */
+static CYTHON_INLINE void __Pyx_RaiseTooManyValuesError(Py_ssize_t expected);
+
+/* RaiseNeedMoreValuesToUnpack.proto */
+static CYTHON_INLINE void __Pyx_RaiseNeedMoreValuesError(Py_ssize_t index);
+
+/* RaiseNoneIterError.proto */
+static CYTHON_INLINE void __Pyx_RaiseNoneNotIterableError(void);
+
+/* ExtTypeTest.proto */
+static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type);
+
 /* SwapException.proto */
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_ExceptionSwap(type, value, tb)  __Pyx__ExceptionSwap(__pyx_tstate, type, value, tb)
 static CYTHON_INLINE void __Pyx__ExceptionSwap(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
 #else
 static CYTHON_INLINE void __Pyx_ExceptionSwap(PyObject **type, PyObject **value, PyObject **tb);
 #endif
@@ -2011,20 +2006,28 @@
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
 #ifndef __PYX_HAVE_RT_ImportType_proto
 #define __PYX_HAVE_RT_ImportType_proto
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#endif
 enum __Pyx_ImportType_CheckSize {
    __Pyx_ImportType_CheckSize_Error = 0,
    __Pyx_ImportType_CheckSize_Warn = 1,
    __Pyx_ImportType_CheckSize_Ignore = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
 #endif
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
 #define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
 #else
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line);
@@ -2225,39 +2228,36 @@
     static CYTHON_INLINE __pyx_t_float_complex __Pyx_c_conj_float(__pyx_t_float_complex);
     #if 1
         static CYTHON_INLINE float __Pyx_c_abs_float(__pyx_t_float_complex);
         static CYTHON_INLINE __pyx_t_float_complex __Pyx_c_pow_float(__pyx_t_float_complex, __pyx_t_float_complex);
     #endif
 #endif
 
-/* GCCDiagnostics.proto */
-#if defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
-#define __Pyx_HAS_GCC_DIAGNOSTIC
-#endif
-
 /* MemviewSliceCopyTemplate.proto */
 static __Pyx_memviewslice
 __pyx_memoryview_copy_new_contig(const __Pyx_memviewslice *from_mvs,
                                  const char *mode, int ndim,
                                  size_t sizeof_dtype, int contig_flag,
                                  int dtype_is_object);
 
-/* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
+/* GCCDiagnostics.proto */
+#if defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
+#define __Pyx_HAS_GCC_DIAGNOSTIC
+#endif
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
 
-/* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_enum__NPY_TYPES(enum NPY_TYPES value);
-
 /* CIntFromPy.proto */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *);
 
 /* CIntToPy.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
+
+/* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE char __Pyx_PyInt_As_char(PyObject *);
 
 /* CheckBinaryVersion.proto */
 static int __Pyx_check_binary_version(void);
@@ -2305,16 +2305,25 @@
 /* Module declarations from 'numpy' */
 
 /* Module declarations from 'numpy' */
 static PyTypeObject *__pyx_ptype_5numpy_dtype = 0;
 static PyTypeObject *__pyx_ptype_5numpy_flatiter = 0;
 static PyTypeObject *__pyx_ptype_5numpy_broadcast = 0;
 static PyTypeObject *__pyx_ptype_5numpy_ndarray = 0;
+static PyTypeObject *__pyx_ptype_5numpy_generic = 0;
+static PyTypeObject *__pyx_ptype_5numpy_number = 0;
+static PyTypeObject *__pyx_ptype_5numpy_integer = 0;
+static PyTypeObject *__pyx_ptype_5numpy_signedinteger = 0;
+static PyTypeObject *__pyx_ptype_5numpy_unsignedinteger = 0;
+static PyTypeObject *__pyx_ptype_5numpy_inexact = 0;
+static PyTypeObject *__pyx_ptype_5numpy_floating = 0;
+static PyTypeObject *__pyx_ptype_5numpy_complexfloating = 0;
+static PyTypeObject *__pyx_ptype_5numpy_flexible = 0;
+static PyTypeObject *__pyx_ptype_5numpy_character = 0;
 static PyTypeObject *__pyx_ptype_5numpy_ufunc = 0;
-static CYTHON_INLINE char *__pyx_f_5numpy__util_dtypestring(PyArray_Descr *, char *, char *, int *); /*proto*/
 
 /* Module declarations from 'openTSNE._matrix_mul.matrix_mul' */
 static PyTypeObject *__pyx_array_type = 0;
 static PyTypeObject *__pyx_MemviewEnum_type = 0;
 static PyTypeObject *__pyx_memoryview_type = 0;
 static PyTypeObject *__pyx_memoryviewslice_type = 0;
 static PyObject *generic = 0;
@@ -2361,17 +2370,16 @@
 static __Pyx_TypeInfo __Pyx_TypeInfo_double = { "double", NULL, sizeof(double), { 0 }, 0, 'R', 0, 0 };
 #define __Pyx_MODULE_NAME "openTSNE._matrix_mul.matrix_mul"
 extern int __pyx_module_is_main_openTSNE___matrix_mul__matrix_mul;
 int __pyx_module_is_main_openTSNE___matrix_mul__matrix_mul = 0;
 
 /* Implementation of 'openTSNE._matrix_mul.matrix_mul' */
 static PyObject *__pyx_builtin_range;
-static PyObject *__pyx_builtin_ValueError;
-static PyObject *__pyx_builtin_RuntimeError;
 static PyObject *__pyx_builtin_ImportError;
+static PyObject *__pyx_builtin_ValueError;
 static PyObject *__pyx_builtin_MemoryError;
 static PyObject *__pyx_builtin_enumerate;
 static PyObject *__pyx_builtin_TypeError;
 static PyObject *__pyx_builtin_Ellipsis;
 static PyObject *__pyx_builtin_id;
 static PyObject *__pyx_builtin_IndexError;
 static const char __pyx_k_O[] = "O";
@@ -2431,15 +2439,14 @@
 static const char __pyx_k_IndexError[] = "IndexError";
 static const char __pyx_k_ValueError[] = "ValueError";
 static const char __pyx_k_pyx_result[] = "__pyx_result";
 static const char __pyx_k_pyx_vtable[] = "__pyx_vtable__";
 static const char __pyx_k_ImportError[] = "ImportError";
 static const char __pyx_k_MemoryError[] = "MemoryError";
 static const char __pyx_k_PickleError[] = "PickleError";
-static const char __pyx_k_RuntimeError[] = "RuntimeError";
 static const char __pyx_k_pyx_checksum[] = "__pyx_checksum";
 static const char __pyx_k_stringsource[] = "stringsource";
 static const char __pyx_k_pyx_getbuffer[] = "__pyx_getbuffer";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
 static const char __pyx_k_View_MemoryView[] = "View.MemoryView";
 static const char __pyx_k_allocate_buffer[] = "allocate_buffer";
 static const char __pyx_k_dtype_is_object[] = "dtype_is_object";
@@ -2452,61 +2459,51 @@
 static const char __pyx_k_contiguous_and_direct[] = "<contiguous and direct>";
 static const char __pyx_k_MemoryView_of_r_object[] = "<MemoryView of %r object>";
 static const char __pyx_k_MemoryView_of_r_at_0x_x[] = "<MemoryView of %r at 0x%x>";
 static const char __pyx_k_contiguous_and_indirect[] = "<contiguous and indirect>";
 static const char __pyx_k_Cannot_index_with_type_s[] = "Cannot index with type '%s'";
 static const char __pyx_k_Invalid_shape_in_axis_d_d[] = "Invalid shape in axis %d: %d.";
 static const char __pyx_k_itemsize_0_for_cython_array[] = "itemsize <= 0 for cython.array";
-static const char __pyx_k_ndarray_is_not_C_contiguous[] = "ndarray is not C contiguous";
 static const char __pyx_k_unable_to_allocate_array_data[] = "unable to allocate array data.";
 static const char __pyx_k_strided_and_direct_or_indirect[] = "<strided and direct or indirect>";
 static const char __pyx_k_numpy_core_multiarray_failed_to[] = "numpy.core.multiarray failed to import";
-static const char __pyx_k_unknown_dtype_code_in_numpy_pxd[] = "unknown dtype code in numpy.pxd (%d)";
 static const char __pyx_k_Buffer_view_does_not_expose_stri[] = "Buffer view does not expose strides";
 static const char __pyx_k_Can_only_create_a_buffer_that_is[] = "Can only create a buffer that is contiguous in memory.";
 static const char __pyx_k_Cannot_assign_to_read_only_memor[] = "Cannot assign to read-only memoryview";
 static const char __pyx_k_Cannot_create_writable_memory_vi[] = "Cannot create writable memory view from read-only memoryview";
 static const char __pyx_k_Empty_shape_tuple_for_cython_arr[] = "Empty shape tuple for cython.array";
-static const char __pyx_k_Format_string_allocated_too_shor[] = "Format string allocated too short, see comment in numpy.pxd";
 static const char __pyx_k_Incompatible_checksums_0x_x_vs_0[] = "Incompatible checksums (0x%x vs (0xb068931, 0x82a3537, 0x6ae9995) = (name))";
 static const char __pyx_k_Indirect_dimensions_not_supporte[] = "Indirect dimensions not supported";
 static const char __pyx_k_Invalid_mode_expected_c_or_fortr[] = "Invalid mode, expected 'c' or 'fortran', got %s";
-static const char __pyx_k_Non_native_byte_order_not_suppor[] = "Non-native byte order not supported";
 static const char __pyx_k_Out_of_bounds_on_buffer_access_a[] = "Out of bounds on buffer access (axis %d)";
 static const char __pyx_k_Unable_to_convert_item_to_object[] = "Unable to convert item to object";
 static const char __pyx_k_got_differing_extents_in_dimensi[] = "got differing extents in dimension %d (got %d and %d)";
-static const char __pyx_k_ndarray_is_not_Fortran_contiguou[] = "ndarray is not Fortran contiguous";
 static const char __pyx_k_no_default___reduce___due_to_non[] = "no default __reduce__ due to non-trivial __cinit__";
 static const char __pyx_k_numpy_core_umath_failed_to_impor[] = "numpy.core.umath failed to import";
 static const char __pyx_k_unable_to_allocate_shape_and_str[] = "unable to allocate shape and strides.";
-static const char __pyx_k_Format_string_allocated_too_shor_2[] = "Format string allocated too short.";
 static PyObject *__pyx_n_s_ASCII;
 static PyObject *__pyx_kp_s_Buffer_view_does_not_expose_stri;
 static PyObject *__pyx_kp_s_Can_only_create_a_buffer_that_is;
 static PyObject *__pyx_kp_s_Cannot_assign_to_read_only_memor;
 static PyObject *__pyx_kp_s_Cannot_create_writable_memory_vi;
 static PyObject *__pyx_kp_s_Cannot_index_with_type_s;
 static PyObject *__pyx_n_s_Ellipsis;
 static PyObject *__pyx_kp_s_Empty_shape_tuple_for_cython_arr;
-static PyObject *__pyx_kp_u_Format_string_allocated_too_shor;
-static PyObject *__pyx_kp_u_Format_string_allocated_too_shor_2;
 static PyObject *__pyx_n_s_ImportError;
 static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0;
 static PyObject *__pyx_n_s_IndexError;
 static PyObject *__pyx_kp_s_Indirect_dimensions_not_supporte;
 static PyObject *__pyx_kp_s_Invalid_mode_expected_c_or_fortr;
 static PyObject *__pyx_kp_s_Invalid_shape_in_axis_d_d;
 static PyObject *__pyx_n_s_MemoryError;
 static PyObject *__pyx_kp_s_MemoryView_of_r_at_0x_x;
 static PyObject *__pyx_kp_s_MemoryView_of_r_object;
-static PyObject *__pyx_kp_u_Non_native_byte_order_not_suppor;
 static PyObject *__pyx_n_b_O;
 static PyObject *__pyx_kp_s_Out_of_bounds_on_buffer_access_a;
 static PyObject *__pyx_n_s_PickleError;
-static PyObject *__pyx_n_s_RuntimeError;
 static PyObject *__pyx_n_s_TypeError;
 static PyObject *__pyx_kp_s_Unable_to_convert_item_to_object;
 static PyObject *__pyx_n_s_ValueError;
 static PyObject *__pyx_n_s_View_MemoryView;
 static PyObject *__pyx_n_s_allocate_buffer;
 static PyObject *__pyx_n_s_base;
 static PyObject *__pyx_n_s_c;
@@ -2537,16 +2534,14 @@
 static PyObject *__pyx_kp_s_itemsize_0_for_cython_array;
 static PyObject *__pyx_n_s_main;
 static PyObject *__pyx_n_s_memview;
 static PyObject *__pyx_n_s_mode;
 static PyObject *__pyx_n_s_multiply;
 static PyObject *__pyx_n_s_name;
 static PyObject *__pyx_n_s_name_2;
-static PyObject *__pyx_kp_u_ndarray_is_not_C_contiguous;
-static PyObject *__pyx_kp_u_ndarray_is_not_Fortran_contiguou;
 static PyObject *__pyx_n_s_ndim;
 static PyObject *__pyx_n_s_new;
 static PyObject *__pyx_kp_s_no_default___reduce___due_to_non;
 static PyObject *__pyx_n_s_np;
 static PyObject *__pyx_n_s_numpy;
 static PyObject *__pyx_kp_u_numpy_core_multiarray_failed_to;
 static PyObject *__pyx_kp_u_numpy_core_umath_failed_to_impor;
@@ -2578,20 +2573,17 @@
 static PyObject *__pyx_kp_s_strided_and_direct_or_indirect;
 static PyObject *__pyx_kp_s_strided_and_indirect;
 static PyObject *__pyx_kp_s_stringsource;
 static PyObject *__pyx_n_s_struct;
 static PyObject *__pyx_n_s_test;
 static PyObject *__pyx_kp_s_unable_to_allocate_array_data;
 static PyObject *__pyx_kp_s_unable_to_allocate_shape_and_str;
-static PyObject *__pyx_kp_u_unknown_dtype_code_in_numpy_pxd;
 static PyObject *__pyx_n_s_unpack;
 static PyObject *__pyx_n_s_update;
 static PyObject *__pyx_n_s_zeros;
-static int __pyx_pf_5numpy_7ndarray___getbuffer__(PyArrayObject *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags); /* proto */
-static void __pyx_pf_5numpy_7ndarray_2__releasebuffer__(PyArrayObject *__pyx_v_self, Py_buffer *__pyx_v_info); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array___cinit__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_shape, Py_ssize_t __pyx_v_itemsize, PyObject *__pyx_v_format, PyObject *__pyx_v_mode, int __pyx_v_allocate_buffer); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array_2__getbuffer__(struct __pyx_array_obj *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags); /* proto */
 static void __pyx_array___pyx_pf_15View_dot_MemoryView_5array_4__dealloc__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_15View_dot_MemoryView_5array_7memview___get__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static Py_ssize_t __pyx_array___pyx_pf_15View_dot_MemoryView_5array_6__len__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_array___pyx_pf_15View_dot_MemoryView_5array_8__getattr__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_attr); /* proto */
 static PyObject *__pyx_array___pyx_pf_15View_dot_MemoryView_5array_10__getitem__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_item); /* proto */
@@ -2645,38 +2637,33 @@
 static PyObject *__pyx_tuple__3;
 static PyObject *__pyx_tuple__4;
 static PyObject *__pyx_tuple__5;
 static PyObject *__pyx_tuple__6;
 static PyObject *__pyx_tuple__7;
 static PyObject *__pyx_tuple__8;
 static PyObject *__pyx_tuple__9;
-static PyObject *__pyx_slice__22;
+static PyObject *__pyx_slice__17;
 static PyObject *__pyx_tuple__10;
 static PyObject *__pyx_tuple__11;
 static PyObject *__pyx_tuple__12;
 static PyObject *__pyx_tuple__13;
 static PyObject *__pyx_tuple__14;
 static PyObject *__pyx_tuple__15;
 static PyObject *__pyx_tuple__16;
-static PyObject *__pyx_tuple__17;
 static PyObject *__pyx_tuple__18;
 static PyObject *__pyx_tuple__19;
 static PyObject *__pyx_tuple__20;
 static PyObject *__pyx_tuple__21;
+static PyObject *__pyx_tuple__22;
 static PyObject *__pyx_tuple__23;
 static PyObject *__pyx_tuple__24;
 static PyObject *__pyx_tuple__25;
 static PyObject *__pyx_tuple__26;
 static PyObject *__pyx_tuple__27;
-static PyObject *__pyx_tuple__28;
-static PyObject *__pyx_tuple__29;
-static PyObject *__pyx_tuple__30;
-static PyObject *__pyx_tuple__31;
-static PyObject *__pyx_tuple__32;
-static PyObject *__pyx_codeobj__33;
+static PyObject *__pyx_codeobj__28;
 /* Late includes */
 
 /* "openTSNE/_matrix_mul/matrix_mul_numpy.pyx":12
  * 
  * 
  * cdef void matrix_multiply_fft_1d(             # <<<<<<<<<<<<<<
  *     double[::1] kernel_tilde,
@@ -3752,874 +3739,15 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_fft_w_coefficients, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_fft_kernel_tilde, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_fft_in_buffer, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_fft_out_buffer, 1);
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":258
- *         # experimental exception made for __getbuffer__ and __releasebuffer__
- *         # -- the details of this may change.
- *         def __getbuffer__(ndarray self, Py_buffer* info, int flags):             # <<<<<<<<<<<<<<
- *             # This implementation of getbuffer is geared towards Cython
- *             # requirements, and does not yet fulfill the PEP.
- */
-
-/* Python wrapper */
-static CYTHON_UNUSED int __pyx_pw_5numpy_7ndarray_1__getbuffer__(PyObject *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags); /*proto*/
-static CYTHON_UNUSED int __pyx_pw_5numpy_7ndarray_1__getbuffer__(PyObject *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__getbuffer__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_5numpy_7ndarray___getbuffer__(((PyArrayObject *)__pyx_v_self), ((Py_buffer *)__pyx_v_info), ((int)__pyx_v_flags));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static int __pyx_pf_5numpy_7ndarray___getbuffer__(PyArrayObject *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags) {
-  int __pyx_v_i;
-  int __pyx_v_ndim;
-  int __pyx_v_endian_detector;
-  int __pyx_v_little_endian;
-  int __pyx_v_t;
-  char *__pyx_v_f;
-  PyArray_Descr *__pyx_v_descr = 0;
-  int __pyx_v_offset;
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  int __pyx_t_2;
-  PyObject *__pyx_t_3 = NULL;
-  int __pyx_t_4;
-  int __pyx_t_5;
-  int __pyx_t_6;
-  PyArray_Descr *__pyx_t_7;
-  PyObject *__pyx_t_8 = NULL;
-  char *__pyx_t_9;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  if (__pyx_v_info == NULL) {
-    PyErr_SetString(PyExc_BufferError, "PyObject_GetBuffer: view==NULL argument is obsolete");
-    return -1;
-  }
-  __Pyx_RefNannySetupContext("__getbuffer__", 0);
-  __pyx_v_info->obj = Py_None; __Pyx_INCREF(Py_None);
-  __Pyx_GIVEREF(__pyx_v_info->obj);
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":265
- * 
- *             cdef int i, ndim
- *             cdef int endian_detector = 1             # <<<<<<<<<<<<<<
- *             cdef bint little_endian = ((<char*>&endian_detector)[0] != 0)
- * 
- */
-  __pyx_v_endian_detector = 1;
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":266
- *             cdef int i, ndim
- *             cdef int endian_detector = 1
- *             cdef bint little_endian = ((<char*>&endian_detector)[0] != 0)             # <<<<<<<<<<<<<<
- * 
- *             ndim = PyArray_NDIM(self)
- */
-  __pyx_v_little_endian = ((((char *)(&__pyx_v_endian_detector))[0]) != 0);
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":268
- *             cdef bint little_endian = ((<char*>&endian_detector)[0] != 0)
- * 
- *             ndim = PyArray_NDIM(self)             # <<<<<<<<<<<<<<
- * 
- *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)
- */
-  __pyx_v_ndim = PyArray_NDIM(__pyx_v_self);
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":270
- *             ndim = PyArray_NDIM(self)
- * 
- *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)             # <<<<<<<<<<<<<<
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_C_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not C contiguous")
- */
-  __pyx_t_2 = (((__pyx_v_flags & PyBUF_C_CONTIGUOUS) == PyBUF_C_CONTIGUOUS) != 0);
-  if (__pyx_t_2) {
-  } else {
-    __pyx_t_1 = __pyx_t_2;
-    goto __pyx_L4_bool_binop_done;
-  }
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":271
- * 
- *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_C_CONTIGUOUS)):             # <<<<<<<<<<<<<<
- *                 raise ValueError(u"ndarray is not C contiguous")
- * 
- */
-  __pyx_t_2 = ((!(PyArray_CHKFLAGS(__pyx_v_self, NPY_ARRAY_C_CONTIGUOUS) != 0)) != 0);
-  __pyx_t_1 = __pyx_t_2;
-  __pyx_L4_bool_binop_done:;
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":270
- *             ndim = PyArray_NDIM(self)
- * 
- *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)             # <<<<<<<<<<<<<<
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_C_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not C contiguous")
- */
-  if (unlikely(__pyx_t_1)) {
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":272
- *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_C_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not C contiguous")             # <<<<<<<<<<<<<<
- * 
- *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)
- */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 272, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(1, 272, __pyx_L1_error)
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":270
- *             ndim = PyArray_NDIM(self)
- * 
- *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)             # <<<<<<<<<<<<<<
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_C_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not C contiguous")
- */
-  }
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":274
- *                 raise ValueError(u"ndarray is not C contiguous")
- * 
- *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)             # <<<<<<<<<<<<<<
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_F_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not Fortran contiguous")
- */
-  __pyx_t_2 = (((__pyx_v_flags & PyBUF_F_CONTIGUOUS) == PyBUF_F_CONTIGUOUS) != 0);
-  if (__pyx_t_2) {
-  } else {
-    __pyx_t_1 = __pyx_t_2;
-    goto __pyx_L7_bool_binop_done;
-  }
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":275
- * 
- *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_F_CONTIGUOUS)):             # <<<<<<<<<<<<<<
- *                 raise ValueError(u"ndarray is not Fortran contiguous")
- * 
- */
-  __pyx_t_2 = ((!(PyArray_CHKFLAGS(__pyx_v_self, NPY_ARRAY_F_CONTIGUOUS) != 0)) != 0);
-  __pyx_t_1 = __pyx_t_2;
-  __pyx_L7_bool_binop_done:;
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":274
- *                 raise ValueError(u"ndarray is not C contiguous")
- * 
- *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)             # <<<<<<<<<<<<<<
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_F_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not Fortran contiguous")
- */
-  if (unlikely(__pyx_t_1)) {
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":276
- *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_F_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not Fortran contiguous")             # <<<<<<<<<<<<<<
- * 
- *             info.buf = PyArray_DATA(self)
- */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 276, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(1, 276, __pyx_L1_error)
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":274
- *                 raise ValueError(u"ndarray is not C contiguous")
- * 
- *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)             # <<<<<<<<<<<<<<
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_F_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not Fortran contiguous")
- */
-  }
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":278
- *                 raise ValueError(u"ndarray is not Fortran contiguous")
- * 
- *             info.buf = PyArray_DATA(self)             # <<<<<<<<<<<<<<
- *             info.ndim = ndim
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
- */
-  __pyx_v_info->buf = PyArray_DATA(__pyx_v_self);
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":279
- * 
- *             info.buf = PyArray_DATA(self)
- *             info.ndim = ndim             # <<<<<<<<<<<<<<
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
- *                 # Allocate new buffer for strides and shape info.
- */
-  __pyx_v_info->ndim = __pyx_v_ndim;
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":280
- *             info.buf = PyArray_DATA(self)
- *             info.ndim = ndim
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):             # <<<<<<<<<<<<<<
- *                 # Allocate new buffer for strides and shape info.
- *                 # This is allocated as one block, strides first.
- */
-  __pyx_t_1 = (((sizeof(npy_intp)) != (sizeof(Py_ssize_t))) != 0);
-  if (__pyx_t_1) {
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":283
- *                 # Allocate new buffer for strides and shape info.
- *                 # This is allocated as one block, strides first.
- *                 info.strides = <Py_ssize_t*>PyObject_Malloc(sizeof(Py_ssize_t) * 2 * <size_t>ndim)             # <<<<<<<<<<<<<<
- *                 info.shape = info.strides + ndim
- *                 for i in range(ndim):
- */
-    __pyx_v_info->strides = ((Py_ssize_t *)PyObject_Malloc((((sizeof(Py_ssize_t)) * 2) * ((size_t)__pyx_v_ndim))));
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":284
- *                 # This is allocated as one block, strides first.
- *                 info.strides = <Py_ssize_t*>PyObject_Malloc(sizeof(Py_ssize_t) * 2 * <size_t>ndim)
- *                 info.shape = info.strides + ndim             # <<<<<<<<<<<<<<
- *                 for i in range(ndim):
- *                     info.strides[i] = PyArray_STRIDES(self)[i]
- */
-    __pyx_v_info->shape = (__pyx_v_info->strides + __pyx_v_ndim);
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":285
- *                 info.strides = <Py_ssize_t*>PyObject_Malloc(sizeof(Py_ssize_t) * 2 * <size_t>ndim)
- *                 info.shape = info.strides + ndim
- *                 for i in range(ndim):             # <<<<<<<<<<<<<<
- *                     info.strides[i] = PyArray_STRIDES(self)[i]
- *                     info.shape[i] = PyArray_DIMS(self)[i]
- */
-    __pyx_t_4 = __pyx_v_ndim;
-    __pyx_t_5 = __pyx_t_4;
-    for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
-      __pyx_v_i = __pyx_t_6;
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":286
- *                 info.shape = info.strides + ndim
- *                 for i in range(ndim):
- *                     info.strides[i] = PyArray_STRIDES(self)[i]             # <<<<<<<<<<<<<<
- *                     info.shape[i] = PyArray_DIMS(self)[i]
- *             else:
- */
-      (__pyx_v_info->strides[__pyx_v_i]) = (PyArray_STRIDES(__pyx_v_self)[__pyx_v_i]);
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":287
- *                 for i in range(ndim):
- *                     info.strides[i] = PyArray_STRIDES(self)[i]
- *                     info.shape[i] = PyArray_DIMS(self)[i]             # <<<<<<<<<<<<<<
- *             else:
- *                 info.strides = <Py_ssize_t*>PyArray_STRIDES(self)
- */
-      (__pyx_v_info->shape[__pyx_v_i]) = (PyArray_DIMS(__pyx_v_self)[__pyx_v_i]);
-    }
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":280
- *             info.buf = PyArray_DATA(self)
- *             info.ndim = ndim
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):             # <<<<<<<<<<<<<<
- *                 # Allocate new buffer for strides and shape info.
- *                 # This is allocated as one block, strides first.
- */
-    goto __pyx_L9;
-  }
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":289
- *                     info.shape[i] = PyArray_DIMS(self)[i]
- *             else:
- *                 info.strides = <Py_ssize_t*>PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
- *                 info.shape = <Py_ssize_t*>PyArray_DIMS(self)
- *             info.suboffsets = NULL
- */
-  /*else*/ {
-    __pyx_v_info->strides = ((Py_ssize_t *)PyArray_STRIDES(__pyx_v_self));
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":290
- *             else:
- *                 info.strides = <Py_ssize_t*>PyArray_STRIDES(self)
- *                 info.shape = <Py_ssize_t*>PyArray_DIMS(self)             # <<<<<<<<<<<<<<
- *             info.suboffsets = NULL
- *             info.itemsize = PyArray_ITEMSIZE(self)
- */
-    __pyx_v_info->shape = ((Py_ssize_t *)PyArray_DIMS(__pyx_v_self));
-  }
-  __pyx_L9:;
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":291
- *                 info.strides = <Py_ssize_t*>PyArray_STRIDES(self)
- *                 info.shape = <Py_ssize_t*>PyArray_DIMS(self)
- *             info.suboffsets = NULL             # <<<<<<<<<<<<<<
- *             info.itemsize = PyArray_ITEMSIZE(self)
- *             info.readonly = not PyArray_ISWRITEABLE(self)
- */
-  __pyx_v_info->suboffsets = NULL;
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":292
- *                 info.shape = <Py_ssize_t*>PyArray_DIMS(self)
- *             info.suboffsets = NULL
- *             info.itemsize = PyArray_ITEMSIZE(self)             # <<<<<<<<<<<<<<
- *             info.readonly = not PyArray_ISWRITEABLE(self)
- * 
- */
-  __pyx_v_info->itemsize = PyArray_ITEMSIZE(__pyx_v_self);
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":293
- *             info.suboffsets = NULL
- *             info.itemsize = PyArray_ITEMSIZE(self)
- *             info.readonly = not PyArray_ISWRITEABLE(self)             # <<<<<<<<<<<<<<
- * 
- *             cdef int t
- */
-  __pyx_v_info->readonly = (!(PyArray_ISWRITEABLE(__pyx_v_self) != 0));
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":296
- * 
- *             cdef int t
- *             cdef char* f = NULL             # <<<<<<<<<<<<<<
- *             cdef dtype descr = <dtype>PyArray_DESCR(self)
- *             cdef int offset
- */
-  __pyx_v_f = NULL;
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":297
- *             cdef int t
- *             cdef char* f = NULL
- *             cdef dtype descr = <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
- *             cdef int offset
- * 
- */
-  __pyx_t_7 = PyArray_DESCR(__pyx_v_self);
-  __pyx_t_3 = ((PyObject *)__pyx_t_7);
-  __Pyx_INCREF(__pyx_t_3);
-  __pyx_v_descr = ((PyArray_Descr *)__pyx_t_3);
-  __pyx_t_3 = 0;
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":300
- *             cdef int offset
- * 
- *             info.obj = self             # <<<<<<<<<<<<<<
- * 
- *             if not PyDataType_HASFIELDS(descr):
- */
-  __Pyx_INCREF(((PyObject *)__pyx_v_self));
-  __Pyx_GIVEREF(((PyObject *)__pyx_v_self));
-  __Pyx_GOTREF(__pyx_v_info->obj);
-  __Pyx_DECREF(__pyx_v_info->obj);
-  __pyx_v_info->obj = ((PyObject *)__pyx_v_self);
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":302
- *             info.obj = self
- * 
- *             if not PyDataType_HASFIELDS(descr):             # <<<<<<<<<<<<<<
- *                 t = descr.type_num
- *                 if ((descr.byteorder == c'>' and little_endian) or
- */
-  __pyx_t_1 = ((!(PyDataType_HASFIELDS(__pyx_v_descr) != 0)) != 0);
-  if (__pyx_t_1) {
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":303
- * 
- *             if not PyDataType_HASFIELDS(descr):
- *                 t = descr.type_num             # <<<<<<<<<<<<<<
- *                 if ((descr.byteorder == c'>' and little_endian) or
- *                     (descr.byteorder == c'<' and not little_endian)):
- */
-    __pyx_t_4 = __pyx_v_descr->type_num;
-    __pyx_v_t = __pyx_t_4;
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":304
- *             if not PyDataType_HASFIELDS(descr):
- *                 t = descr.type_num
- *                 if ((descr.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
- *                     (descr.byteorder == c'<' and not little_endian)):
- *                     raise ValueError(u"Non-native byte order not supported")
- */
-    __pyx_t_2 = ((__pyx_v_descr->byteorder == '>') != 0);
-    if (!__pyx_t_2) {
-      goto __pyx_L15_next_or;
-    } else {
-    }
-    __pyx_t_2 = (__pyx_v_little_endian != 0);
-    if (!__pyx_t_2) {
-    } else {
-      __pyx_t_1 = __pyx_t_2;
-      goto __pyx_L14_bool_binop_done;
-    }
-    __pyx_L15_next_or:;
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":305
- *                 t = descr.type_num
- *                 if ((descr.byteorder == c'>' and little_endian) or
- *                     (descr.byteorder == c'<' and not little_endian)):             # <<<<<<<<<<<<<<
- *                     raise ValueError(u"Non-native byte order not supported")
- *                 if   t == NPY_BYTE:        f = "b"
- */
-    __pyx_t_2 = ((__pyx_v_descr->byteorder == '<') != 0);
-    if (__pyx_t_2) {
-    } else {
-      __pyx_t_1 = __pyx_t_2;
-      goto __pyx_L14_bool_binop_done;
-    }
-    __pyx_t_2 = ((!(__pyx_v_little_endian != 0)) != 0);
-    __pyx_t_1 = __pyx_t_2;
-    __pyx_L14_bool_binop_done:;
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":304
- *             if not PyDataType_HASFIELDS(descr):
- *                 t = descr.type_num
- *                 if ((descr.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
- *                     (descr.byteorder == c'<' and not little_endian)):
- *                     raise ValueError(u"Non-native byte order not supported")
- */
-    if (unlikely(__pyx_t_1)) {
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":306
- *                 if ((descr.byteorder == c'>' and little_endian) or
- *                     (descr.byteorder == c'<' and not little_endian)):
- *                     raise ValueError(u"Non-native byte order not supported")             # <<<<<<<<<<<<<<
- *                 if   t == NPY_BYTE:        f = "b"
- *                 elif t == NPY_UBYTE:       f = "B"
- */
-      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 306, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __PYX_ERR(1, 306, __pyx_L1_error)
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":304
- *             if not PyDataType_HASFIELDS(descr):
- *                 t = descr.type_num
- *                 if ((descr.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
- *                     (descr.byteorder == c'<' and not little_endian)):
- *                     raise ValueError(u"Non-native byte order not supported")
- */
-    }
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":307
- *                     (descr.byteorder == c'<' and not little_endian)):
- *                     raise ValueError(u"Non-native byte order not supported")
- *                 if   t == NPY_BYTE:        f = "b"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_UBYTE:       f = "B"
- *                 elif t == NPY_SHORT:       f = "h"
- */
-    switch (__pyx_v_t) {
-      case NPY_BYTE:
-      __pyx_v_f = ((char *)"b");
-      break;
-      case NPY_UBYTE:
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":308
- *                     raise ValueError(u"Non-native byte order not supported")
- *                 if   t == NPY_BYTE:        f = "b"
- *                 elif t == NPY_UBYTE:       f = "B"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_SHORT:       f = "h"
- *                 elif t == NPY_USHORT:      f = "H"
- */
-      __pyx_v_f = ((char *)"B");
-      break;
-      case NPY_SHORT:
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":309
- *                 if   t == NPY_BYTE:        f = "b"
- *                 elif t == NPY_UBYTE:       f = "B"
- *                 elif t == NPY_SHORT:       f = "h"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_USHORT:      f = "H"
- *                 elif t == NPY_INT:         f = "i"
- */
-      __pyx_v_f = ((char *)"h");
-      break;
-      case NPY_USHORT:
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":310
- *                 elif t == NPY_UBYTE:       f = "B"
- *                 elif t == NPY_SHORT:       f = "h"
- *                 elif t == NPY_USHORT:      f = "H"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_INT:         f = "i"
- *                 elif t == NPY_UINT:        f = "I"
- */
-      __pyx_v_f = ((char *)"H");
-      break;
-      case NPY_INT:
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":311
- *                 elif t == NPY_SHORT:       f = "h"
- *                 elif t == NPY_USHORT:      f = "H"
- *                 elif t == NPY_INT:         f = "i"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_UINT:        f = "I"
- *                 elif t == NPY_LONG:        f = "l"
- */
-      __pyx_v_f = ((char *)"i");
-      break;
-      case NPY_UINT:
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":312
- *                 elif t == NPY_USHORT:      f = "H"
- *                 elif t == NPY_INT:         f = "i"
- *                 elif t == NPY_UINT:        f = "I"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_LONG:        f = "l"
- *                 elif t == NPY_ULONG:       f = "L"
- */
-      __pyx_v_f = ((char *)"I");
-      break;
-      case NPY_LONG:
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":313
- *                 elif t == NPY_INT:         f = "i"
- *                 elif t == NPY_UINT:        f = "I"
- *                 elif t == NPY_LONG:        f = "l"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_ULONG:       f = "L"
- *                 elif t == NPY_LONGLONG:    f = "q"
- */
-      __pyx_v_f = ((char *)"l");
-      break;
-      case NPY_ULONG:
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":314
- *                 elif t == NPY_UINT:        f = "I"
- *                 elif t == NPY_LONG:        f = "l"
- *                 elif t == NPY_ULONG:       f = "L"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_LONGLONG:    f = "q"
- *                 elif t == NPY_ULONGLONG:   f = "Q"
- */
-      __pyx_v_f = ((char *)"L");
-      break;
-      case NPY_LONGLONG:
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":315
- *                 elif t == NPY_LONG:        f = "l"
- *                 elif t == NPY_ULONG:       f = "L"
- *                 elif t == NPY_LONGLONG:    f = "q"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_ULONGLONG:   f = "Q"
- *                 elif t == NPY_FLOAT:       f = "f"
- */
-      __pyx_v_f = ((char *)"q");
-      break;
-      case NPY_ULONGLONG:
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":316
- *                 elif t == NPY_ULONG:       f = "L"
- *                 elif t == NPY_LONGLONG:    f = "q"
- *                 elif t == NPY_ULONGLONG:   f = "Q"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_FLOAT:       f = "f"
- *                 elif t == NPY_DOUBLE:      f = "d"
- */
-      __pyx_v_f = ((char *)"Q");
-      break;
-      case NPY_FLOAT:
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":317
- *                 elif t == NPY_LONGLONG:    f = "q"
- *                 elif t == NPY_ULONGLONG:   f = "Q"
- *                 elif t == NPY_FLOAT:       f = "f"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_DOUBLE:      f = "d"
- *                 elif t == NPY_LONGDOUBLE:  f = "g"
- */
-      __pyx_v_f = ((char *)"f");
-      break;
-      case NPY_DOUBLE:
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":318
- *                 elif t == NPY_ULONGLONG:   f = "Q"
- *                 elif t == NPY_FLOAT:       f = "f"
- *                 elif t == NPY_DOUBLE:      f = "d"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_LONGDOUBLE:  f = "g"
- *                 elif t == NPY_CFLOAT:      f = "Zf"
- */
-      __pyx_v_f = ((char *)"d");
-      break;
-      case NPY_LONGDOUBLE:
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":319
- *                 elif t == NPY_FLOAT:       f = "f"
- *                 elif t == NPY_DOUBLE:      f = "d"
- *                 elif t == NPY_LONGDOUBLE:  f = "g"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_CFLOAT:      f = "Zf"
- *                 elif t == NPY_CDOUBLE:     f = "Zd"
- */
-      __pyx_v_f = ((char *)"g");
-      break;
-      case NPY_CFLOAT:
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":320
- *                 elif t == NPY_DOUBLE:      f = "d"
- *                 elif t == NPY_LONGDOUBLE:  f = "g"
- *                 elif t == NPY_CFLOAT:      f = "Zf"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_CDOUBLE:     f = "Zd"
- *                 elif t == NPY_CLONGDOUBLE: f = "Zg"
- */
-      __pyx_v_f = ((char *)"Zf");
-      break;
-      case NPY_CDOUBLE:
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":321
- *                 elif t == NPY_LONGDOUBLE:  f = "g"
- *                 elif t == NPY_CFLOAT:      f = "Zf"
- *                 elif t == NPY_CDOUBLE:     f = "Zd"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_CLONGDOUBLE: f = "Zg"
- *                 elif t == NPY_OBJECT:      f = "O"
- */
-      __pyx_v_f = ((char *)"Zd");
-      break;
-      case NPY_CLONGDOUBLE:
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":322
- *                 elif t == NPY_CFLOAT:      f = "Zf"
- *                 elif t == NPY_CDOUBLE:     f = "Zd"
- *                 elif t == NPY_CLONGDOUBLE: f = "Zg"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_OBJECT:      f = "O"
- *                 else:
- */
-      __pyx_v_f = ((char *)"Zg");
-      break;
-      case NPY_OBJECT:
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":323
- *                 elif t == NPY_CDOUBLE:     f = "Zd"
- *                 elif t == NPY_CLONGDOUBLE: f = "Zg"
- *                 elif t == NPY_OBJECT:      f = "O"             # <<<<<<<<<<<<<<
- *                 else:
- *                     raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)
- */
-      __pyx_v_f = ((char *)"O");
-      break;
-      default:
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":325
- *                 elif t == NPY_OBJECT:      f = "O"
- *                 else:
- *                     raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)             # <<<<<<<<<<<<<<
- *                 info.format = f
- *                 return
- */
-      __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_t); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 325, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_8 = PyUnicode_Format(__pyx_kp_u_unknown_dtype_code_in_numpy_pxd, __pyx_t_3); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 325, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 325, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __PYX_ERR(1, 325, __pyx_L1_error)
-      break;
-    }
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":326
- *                 else:
- *                     raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)
- *                 info.format = f             # <<<<<<<<<<<<<<
- *                 return
- *             else:
- */
-    __pyx_v_info->format = __pyx_v_f;
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":327
- *                     raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)
- *                 info.format = f
- *                 return             # <<<<<<<<<<<<<<
- *             else:
- *                 info.format = <char*>PyObject_Malloc(_buffer_format_string_len)
- */
-    __pyx_r = 0;
-    goto __pyx_L0;
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":302
- *             info.obj = self
- * 
- *             if not PyDataType_HASFIELDS(descr):             # <<<<<<<<<<<<<<
- *                 t = descr.type_num
- *                 if ((descr.byteorder == c'>' and little_endian) or
- */
-  }
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":329
- *                 return
- *             else:
- *                 info.format = <char*>PyObject_Malloc(_buffer_format_string_len)             # <<<<<<<<<<<<<<
- *                 info.format[0] = c'^' # Native data types, manual alignment
- *                 offset = 0
- */
-  /*else*/ {
-    __pyx_v_info->format = ((char *)PyObject_Malloc(0xFF));
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":330
- *             else:
- *                 info.format = <char*>PyObject_Malloc(_buffer_format_string_len)
- *                 info.format[0] = c'^' # Native data types, manual alignment             # <<<<<<<<<<<<<<
- *                 offset = 0
- *                 f = _util_dtypestring(descr, info.format + 1,
- */
-    (__pyx_v_info->format[0]) = '^';
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":331
- *                 info.format = <char*>PyObject_Malloc(_buffer_format_string_len)
- *                 info.format[0] = c'^' # Native data types, manual alignment
- *                 offset = 0             # <<<<<<<<<<<<<<
- *                 f = _util_dtypestring(descr, info.format + 1,
- *                                       info.format + _buffer_format_string_len,
- */
-    __pyx_v_offset = 0;
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":332
- *                 info.format[0] = c'^' # Native data types, manual alignment
- *                 offset = 0
- *                 f = _util_dtypestring(descr, info.format + 1,             # <<<<<<<<<<<<<<
- *                                       info.format + _buffer_format_string_len,
- *                                       &offset)
- */
-    __pyx_t_9 = __pyx_f_5numpy__util_dtypestring(__pyx_v_descr, (__pyx_v_info->format + 1), (__pyx_v_info->format + 0xFF), (&__pyx_v_offset)); if (unlikely(__pyx_t_9 == ((char *)NULL))) __PYX_ERR(1, 332, __pyx_L1_error)
-    __pyx_v_f = __pyx_t_9;
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":335
- *                                       info.format + _buffer_format_string_len,
- *                                       &offset)
- *                 f[0] = c'\0' # Terminate format string             # <<<<<<<<<<<<<<
- * 
- *         def __releasebuffer__(ndarray self, Py_buffer* info):
- */
-    (__pyx_v_f[0]) = '\x00';
-  }
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":258
- *         # experimental exception made for __getbuffer__ and __releasebuffer__
- *         # -- the details of this may change.
- *         def __getbuffer__(ndarray self, Py_buffer* info, int flags):             # <<<<<<<<<<<<<<
- *             # This implementation of getbuffer is geared towards Cython
- *             # requirements, and does not yet fulfill the PEP.
- */
-
-  /* function exit code */
-  __pyx_r = 0;
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_8);
-  __Pyx_AddTraceback("numpy.ndarray.__getbuffer__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = -1;
-  if (__pyx_v_info->obj != NULL) {
-    __Pyx_GOTREF(__pyx_v_info->obj);
-    __Pyx_DECREF(__pyx_v_info->obj); __pyx_v_info->obj = 0;
-  }
-  goto __pyx_L2;
-  __pyx_L0:;
-  if (__pyx_v_info->obj == Py_None) {
-    __Pyx_GOTREF(__pyx_v_info->obj);
-    __Pyx_DECREF(__pyx_v_info->obj); __pyx_v_info->obj = 0;
-  }
-  __pyx_L2:;
-  __Pyx_XDECREF((PyObject *)__pyx_v_descr);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":337
- *                 f[0] = c'\0' # Terminate format string
- * 
- *         def __releasebuffer__(ndarray self, Py_buffer* info):             # <<<<<<<<<<<<<<
- *             if PyArray_HASFIELDS(self):
- *                 PyObject_Free(info.format)
- */
-
-/* Python wrapper */
-static CYTHON_UNUSED void __pyx_pw_5numpy_7ndarray_3__releasebuffer__(PyObject *__pyx_v_self, Py_buffer *__pyx_v_info); /*proto*/
-static CYTHON_UNUSED void __pyx_pw_5numpy_7ndarray_3__releasebuffer__(PyObject *__pyx_v_self, Py_buffer *__pyx_v_info) {
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__releasebuffer__ (wrapper)", 0);
-  __pyx_pf_5numpy_7ndarray_2__releasebuffer__(((PyArrayObject *)__pyx_v_self), ((Py_buffer *)__pyx_v_info));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-}
-
-static void __pyx_pf_5numpy_7ndarray_2__releasebuffer__(PyArrayObject *__pyx_v_self, Py_buffer *__pyx_v_info) {
-  __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  __Pyx_RefNannySetupContext("__releasebuffer__", 0);
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":338
- * 
- *         def __releasebuffer__(ndarray self, Py_buffer* info):
- *             if PyArray_HASFIELDS(self):             # <<<<<<<<<<<<<<
- *                 PyObject_Free(info.format)
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
- */
-  __pyx_t_1 = (PyArray_HASFIELDS(__pyx_v_self) != 0);
-  if (__pyx_t_1) {
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":339
- *         def __releasebuffer__(ndarray self, Py_buffer* info):
- *             if PyArray_HASFIELDS(self):
- *                 PyObject_Free(info.format)             # <<<<<<<<<<<<<<
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
- *                 PyObject_Free(info.strides)
- */
-    PyObject_Free(__pyx_v_info->format);
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":338
- * 
- *         def __releasebuffer__(ndarray self, Py_buffer* info):
- *             if PyArray_HASFIELDS(self):             # <<<<<<<<<<<<<<
- *                 PyObject_Free(info.format)
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
- */
-  }
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":340
- *             if PyArray_HASFIELDS(self):
- *                 PyObject_Free(info.format)
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):             # <<<<<<<<<<<<<<
- *                 PyObject_Free(info.strides)
- *                 # info.shape was stored after info.strides in the same block
- */
-  __pyx_t_1 = (((sizeof(npy_intp)) != (sizeof(Py_ssize_t))) != 0);
-  if (__pyx_t_1) {
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":341
- *                 PyObject_Free(info.format)
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
- *                 PyObject_Free(info.strides)             # <<<<<<<<<<<<<<
- *                 # info.shape was stored after info.strides in the same block
- * 
- */
-    PyObject_Free(__pyx_v_info->strides);
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":340
- *             if PyArray_HASFIELDS(self):
- *                 PyObject_Free(info.format)
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):             # <<<<<<<<<<<<<<
- *                 PyObject_Free(info.strides)
- *                 # info.shape was stored after info.strides in the same block
- */
-  }
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":337
- *                 f[0] = c'\0' # Terminate format string
- * 
- *         def __releasebuffer__(ndarray self, Py_buffer* info):             # <<<<<<<<<<<<<<
- *             if PyArray_HASFIELDS(self):
- *                 PyObject_Free(info.format)
- */
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-}
-
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":820
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -4628,29 +3756,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":821
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":736
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 821, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 736, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":820
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -4661,15 +3789,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":823
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -4678,29 +3806,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":824
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":739
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 824, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 739, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":823
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -4711,15 +3839,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":826
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -4728,29 +3856,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":827
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":742
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 827, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 742, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":826
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -4761,15 +3889,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":829
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -4778,29 +3906,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":830
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":745
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 830, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 745, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":829
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -4811,15 +3939,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":832
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -4828,29 +3956,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":833
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":748
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 833, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 748, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":832
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -4861,966 +3989,217 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":835
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":836
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":837
+    /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":752
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":836
+    /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":839
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":754
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
- * cdef inline char* _util_dtypestring(dtype descr, char* f, char* end, int* offset) except NULL:
+ * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":835
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":841
- *         return ()
- * 
- * cdef inline char* _util_dtypestring(dtype descr, char* f, char* end, int* offset) except NULL:             # <<<<<<<<<<<<<<
- *     # Recursive utility function used in __getbuffer__ to get format
- *     # string. The new location in the format string is returned.
- */
-
-static CYTHON_INLINE char *__pyx_f_5numpy__util_dtypestring(PyArray_Descr *__pyx_v_descr, char *__pyx_v_f, char *__pyx_v_end, int *__pyx_v_offset) {
-  PyArray_Descr *__pyx_v_child = 0;
-  int __pyx_v_endian_detector;
-  int __pyx_v_little_endian;
-  PyObject *__pyx_v_fields = 0;
-  PyObject *__pyx_v_childname = NULL;
-  PyObject *__pyx_v_new_offset = NULL;
-  PyObject *__pyx_v_t = NULL;
-  char *__pyx_r;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  Py_ssize_t __pyx_t_2;
-  PyObject *__pyx_t_3 = NULL;
-  PyObject *__pyx_t_4 = NULL;
-  int __pyx_t_5;
-  int __pyx_t_6;
-  int __pyx_t_7;
-  long __pyx_t_8;
-  char *__pyx_t_9;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("_util_dtypestring", 0);
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":846
- * 
- *     cdef dtype child
- *     cdef int endian_detector = 1             # <<<<<<<<<<<<<<
- *     cdef bint little_endian = ((<char*>&endian_detector)[0] != 0)
- *     cdef tuple fields
- */
-  __pyx_v_endian_detector = 1;
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":847
- *     cdef dtype child
- *     cdef int endian_detector = 1
- *     cdef bint little_endian = ((<char*>&endian_detector)[0] != 0)             # <<<<<<<<<<<<<<
- *     cdef tuple fields
- * 
- */
-  __pyx_v_little_endian = ((((char *)(&__pyx_v_endian_detector))[0]) != 0);
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":850
- *     cdef tuple fields
- * 
- *     for childname in descr.names:             # <<<<<<<<<<<<<<
- *         fields = descr.fields[childname]
- *         child, new_offset = fields
- */
-  if (unlikely(__pyx_v_descr->names == Py_None)) {
-    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-    __PYX_ERR(1, 850, __pyx_L1_error)
-  }
-  __pyx_t_1 = __pyx_v_descr->names; __Pyx_INCREF(__pyx_t_1); __pyx_t_2 = 0;
-  for (;;) {
-    if (__pyx_t_2 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
-    #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_3); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(1, 850, __pyx_L1_error)
-    #else
-    __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 850, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    #endif
-    __Pyx_XDECREF_SET(__pyx_v_childname, __pyx_t_3);
-    __pyx_t_3 = 0;
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":851
- * 
- *     for childname in descr.names:
- *         fields = descr.fields[childname]             # <<<<<<<<<<<<<<
- *         child, new_offset = fields
- * 
- */
-    if (unlikely(__pyx_v_descr->fields == Py_None)) {
-      PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(1, 851, __pyx_L1_error)
-    }
-    __pyx_t_3 = __Pyx_PyDict_GetItem(__pyx_v_descr->fields, __pyx_v_childname); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 851, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    if (!(likely(PyTuple_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_t_3)->tp_name), 0))) __PYX_ERR(1, 851, __pyx_L1_error)
-    __Pyx_XDECREF_SET(__pyx_v_fields, ((PyObject*)__pyx_t_3));
-    __pyx_t_3 = 0;
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":852
- *     for childname in descr.names:
- *         fields = descr.fields[childname]
- *         child, new_offset = fields             # <<<<<<<<<<<<<<
- * 
- *         if (end - f) - <int>(new_offset - offset[0]) < 15:
- */
-    if (likely(__pyx_v_fields != Py_None)) {
-      PyObject* sequence = __pyx_v_fields;
-      Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
-      if (unlikely(size != 2)) {
-        if (size > 2) __Pyx_RaiseTooManyValuesError(2);
-        else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-        __PYX_ERR(1, 852, __pyx_L1_error)
-      }
-      #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-      __pyx_t_3 = PyTuple_GET_ITEM(sequence, 0); 
-      __pyx_t_4 = PyTuple_GET_ITEM(sequence, 1); 
-      __Pyx_INCREF(__pyx_t_3);
-      __Pyx_INCREF(__pyx_t_4);
-      #else
-      __pyx_t_3 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 852, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 852, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      #endif
-    } else {
-      __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(1, 852, __pyx_L1_error)
-    }
-    if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_dtype))))) __PYX_ERR(1, 852, __pyx_L1_error)
-    __Pyx_XDECREF_SET(__pyx_v_child, ((PyArray_Descr *)__pyx_t_3));
-    __pyx_t_3 = 0;
-    __Pyx_XDECREF_SET(__pyx_v_new_offset, __pyx_t_4);
-    __pyx_t_4 = 0;
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":854
- *         child, new_offset = fields
- * 
- *         if (end - f) - <int>(new_offset - offset[0]) < 15:             # <<<<<<<<<<<<<<
- *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")
- * 
- */
-    __pyx_t_4 = __Pyx_PyInt_From_int((__pyx_v_offset[0])); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 854, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_3 = PyNumber_Subtract(__pyx_v_new_offset, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 854, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 854, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_6 = ((((__pyx_v_end - __pyx_v_f) - ((int)__pyx_t_5)) < 15) != 0);
-    if (unlikely(__pyx_t_6)) {
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":855
- * 
- *         if (end - f) - <int>(new_offset - offset[0]) < 15:
- *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")             # <<<<<<<<<<<<<<
- * 
- *         if ((child.byteorder == c'>' and little_endian) or
- */
-      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 855, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __PYX_ERR(1, 855, __pyx_L1_error)
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":854
- *         child, new_offset = fields
- * 
- *         if (end - f) - <int>(new_offset - offset[0]) < 15:             # <<<<<<<<<<<<<<
- *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")
- * 
- */
-    }
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":857
- *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")
- * 
- *         if ((child.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
- *             (child.byteorder == c'<' and not little_endian)):
- *             raise ValueError(u"Non-native byte order not supported")
- */
-    __pyx_t_7 = ((__pyx_v_child->byteorder == '>') != 0);
-    if (!__pyx_t_7) {
-      goto __pyx_L8_next_or;
-    } else {
-    }
-    __pyx_t_7 = (__pyx_v_little_endian != 0);
-    if (!__pyx_t_7) {
-    } else {
-      __pyx_t_6 = __pyx_t_7;
-      goto __pyx_L7_bool_binop_done;
-    }
-    __pyx_L8_next_or:;
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":858
- * 
- *         if ((child.byteorder == c'>' and little_endian) or
- *             (child.byteorder == c'<' and not little_endian)):             # <<<<<<<<<<<<<<
- *             raise ValueError(u"Non-native byte order not supported")
- *             # One could encode it in the format string and have Cython
- */
-    __pyx_t_7 = ((__pyx_v_child->byteorder == '<') != 0);
-    if (__pyx_t_7) {
-    } else {
-      __pyx_t_6 = __pyx_t_7;
-      goto __pyx_L7_bool_binop_done;
-    }
-    __pyx_t_7 = ((!(__pyx_v_little_endian != 0)) != 0);
-    __pyx_t_6 = __pyx_t_7;
-    __pyx_L7_bool_binop_done:;
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":857
- *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")
- * 
- *         if ((child.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
- *             (child.byteorder == c'<' and not little_endian)):
- *             raise ValueError(u"Non-native byte order not supported")
- */
-    if (unlikely(__pyx_t_6)) {
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":859
- *         if ((child.byteorder == c'>' and little_endian) or
- *             (child.byteorder == c'<' and not little_endian)):
- *             raise ValueError(u"Non-native byte order not supported")             # <<<<<<<<<<<<<<
- *             # One could encode it in the format string and have Cython
- *             # complain instead, BUT: < and > in format strings also imply
- */
-      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 859, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __PYX_ERR(1, 859, __pyx_L1_error)
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":857
- *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")
- * 
- *         if ((child.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
- *             (child.byteorder == c'<' and not little_endian)):
- *             raise ValueError(u"Non-native byte order not supported")
- */
-    }
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":869
- * 
- *         # Output padding bytes
- *         while offset[0] < new_offset:             # <<<<<<<<<<<<<<
- *             f[0] = 120 # "x"; pad byte
- *             f += 1
- */
-    while (1) {
-      __pyx_t_3 = __Pyx_PyInt_From_int((__pyx_v_offset[0])); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 869, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_t_3, __pyx_v_new_offset, Py_LT); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 869, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 869, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (!__pyx_t_6) break;
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":870
- *         # Output padding bytes
- *         while offset[0] < new_offset:
- *             f[0] = 120 # "x"; pad byte             # <<<<<<<<<<<<<<
- *             f += 1
- *             offset[0] += 1
- */
-      (__pyx_v_f[0]) = 0x78;
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":871
- *         while offset[0] < new_offset:
- *             f[0] = 120 # "x"; pad byte
- *             f += 1             # <<<<<<<<<<<<<<
- *             offset[0] += 1
- * 
- */
-      __pyx_v_f = (__pyx_v_f + 1);
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":872
- *             f[0] = 120 # "x"; pad byte
- *             f += 1
- *             offset[0] += 1             # <<<<<<<<<<<<<<
- * 
- *         offset[0] += child.itemsize
- */
-      __pyx_t_8 = 0;
-      (__pyx_v_offset[__pyx_t_8]) = ((__pyx_v_offset[__pyx_t_8]) + 1);
-    }
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":874
- *             offset[0] += 1
- * 
- *         offset[0] += child.itemsize             # <<<<<<<<<<<<<<
- * 
- *         if not PyDataType_HASFIELDS(child):
- */
-    __pyx_t_8 = 0;
-    (__pyx_v_offset[__pyx_t_8]) = ((__pyx_v_offset[__pyx_t_8]) + __pyx_v_child->elsize);
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":876
- *         offset[0] += child.itemsize
- * 
- *         if not PyDataType_HASFIELDS(child):             # <<<<<<<<<<<<<<
- *             t = child.type_num
- *             if end - f < 5:
- */
-    __pyx_t_6 = ((!(PyDataType_HASFIELDS(__pyx_v_child) != 0)) != 0);
-    if (__pyx_t_6) {
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":877
- * 
- *         if not PyDataType_HASFIELDS(child):
- *             t = child.type_num             # <<<<<<<<<<<<<<
- *             if end - f < 5:
- *                 raise RuntimeError(u"Format string allocated too short.")
- */
-      __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_child->type_num); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 877, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __Pyx_XDECREF_SET(__pyx_v_t, __pyx_t_4);
-      __pyx_t_4 = 0;
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":878
- *         if not PyDataType_HASFIELDS(child):
- *             t = child.type_num
- *             if end - f < 5:             # <<<<<<<<<<<<<<
- *                 raise RuntimeError(u"Format string allocated too short.")
- * 
- */
-      __pyx_t_6 = (((__pyx_v_end - __pyx_v_f) < 5) != 0);
-      if (unlikely(__pyx_t_6)) {
-
-        /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":879
- *             t = child.type_num
- *             if end - f < 5:
- *                 raise RuntimeError(u"Format string allocated too short.")             # <<<<<<<<<<<<<<
- * 
- *             # Until ticket #99 is fixed, use integers to avoid warnings
- */
-        __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 879, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_4);
-        __Pyx_Raise(__pyx_t_4, 0, 0, 0);
-        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        __PYX_ERR(1, 879, __pyx_L1_error)
-
-        /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":878
- *         if not PyDataType_HASFIELDS(child):
- *             t = child.type_num
- *             if end - f < 5:             # <<<<<<<<<<<<<<
- *                 raise RuntimeError(u"Format string allocated too short.")
- * 
- */
-      }
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":882
- * 
- *             # Until ticket #99 is fixed, use integers to avoid warnings
- *             if   t == NPY_BYTE:        f[0] =  98 #"b"             # <<<<<<<<<<<<<<
- *             elif t == NPY_UBYTE:       f[0] =  66 #"B"
- *             elif t == NPY_SHORT:       f[0] = 104 #"h"
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_BYTE); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 882, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 882, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 882, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 98;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":883
- *             # Until ticket #99 is fixed, use integers to avoid warnings
- *             if   t == NPY_BYTE:        f[0] =  98 #"b"
- *             elif t == NPY_UBYTE:       f[0] =  66 #"B"             # <<<<<<<<<<<<<<
- *             elif t == NPY_SHORT:       f[0] = 104 #"h"
- *             elif t == NPY_USHORT:      f[0] =  72 #"H"
- */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_UBYTE); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 883, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 883, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 883, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 66;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":884
- *             if   t == NPY_BYTE:        f[0] =  98 #"b"
- *             elif t == NPY_UBYTE:       f[0] =  66 #"B"
- *             elif t == NPY_SHORT:       f[0] = 104 #"h"             # <<<<<<<<<<<<<<
- *             elif t == NPY_USHORT:      f[0] =  72 #"H"
- *             elif t == NPY_INT:         f[0] = 105 #"i"
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_SHORT); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 884, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 884, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 884, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 0x68;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":885
- *             elif t == NPY_UBYTE:       f[0] =  66 #"B"
- *             elif t == NPY_SHORT:       f[0] = 104 #"h"
- *             elif t == NPY_USHORT:      f[0] =  72 #"H"             # <<<<<<<<<<<<<<
- *             elif t == NPY_INT:         f[0] = 105 #"i"
- *             elif t == NPY_UINT:        f[0] =  73 #"I"
- */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_USHORT); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 885, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 885, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 885, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 72;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":886
- *             elif t == NPY_SHORT:       f[0] = 104 #"h"
- *             elif t == NPY_USHORT:      f[0] =  72 #"H"
- *             elif t == NPY_INT:         f[0] = 105 #"i"             # <<<<<<<<<<<<<<
- *             elif t == NPY_UINT:        f[0] =  73 #"I"
- *             elif t == NPY_LONG:        f[0] = 108 #"l"
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_INT); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 886, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 886, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 886, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 0x69;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":887
- *             elif t == NPY_USHORT:      f[0] =  72 #"H"
- *             elif t == NPY_INT:         f[0] = 105 #"i"
- *             elif t == NPY_UINT:        f[0] =  73 #"I"             # <<<<<<<<<<<<<<
- *             elif t == NPY_LONG:        f[0] = 108 #"l"
- *             elif t == NPY_ULONG:       f[0] = 76  #"L"
- */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_UINT); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 887, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 887, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 887, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 73;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":888
- *             elif t == NPY_INT:         f[0] = 105 #"i"
- *             elif t == NPY_UINT:        f[0] =  73 #"I"
- *             elif t == NPY_LONG:        f[0] = 108 #"l"             # <<<<<<<<<<<<<<
- *             elif t == NPY_ULONG:       f[0] = 76  #"L"
- *             elif t == NPY_LONGLONG:    f[0] = 113 #"q"
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_LONG); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 888, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 888, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 888, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 0x6C;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":889
- *             elif t == NPY_UINT:        f[0] =  73 #"I"
- *             elif t == NPY_LONG:        f[0] = 108 #"l"
- *             elif t == NPY_ULONG:       f[0] = 76  #"L"             # <<<<<<<<<<<<<<
- *             elif t == NPY_LONGLONG:    f[0] = 113 #"q"
- *             elif t == NPY_ULONGLONG:   f[0] = 81  #"Q"
- */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_ULONG); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 889, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 889, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 889, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 76;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":890
- *             elif t == NPY_LONG:        f[0] = 108 #"l"
- *             elif t == NPY_ULONG:       f[0] = 76  #"L"
- *             elif t == NPY_LONGLONG:    f[0] = 113 #"q"             # <<<<<<<<<<<<<<
- *             elif t == NPY_ULONGLONG:   f[0] = 81  #"Q"
- *             elif t == NPY_FLOAT:       f[0] = 102 #"f"
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_LONGLONG); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 890, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 890, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 890, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 0x71;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":891
- *             elif t == NPY_ULONG:       f[0] = 76  #"L"
- *             elif t == NPY_LONGLONG:    f[0] = 113 #"q"
- *             elif t == NPY_ULONGLONG:   f[0] = 81  #"Q"             # <<<<<<<<<<<<<<
- *             elif t == NPY_FLOAT:       f[0] = 102 #"f"
- *             elif t == NPY_DOUBLE:      f[0] = 100 #"d"
- */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_ULONGLONG); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 891, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 891, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 891, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 81;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":892
- *             elif t == NPY_LONGLONG:    f[0] = 113 #"q"
- *             elif t == NPY_ULONGLONG:   f[0] = 81  #"Q"
- *             elif t == NPY_FLOAT:       f[0] = 102 #"f"             # <<<<<<<<<<<<<<
- *             elif t == NPY_DOUBLE:      f[0] = 100 #"d"
- *             elif t == NPY_LONGDOUBLE:  f[0] = 103 #"g"
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_FLOAT); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 892, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 892, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 892, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 0x66;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":893
- *             elif t == NPY_ULONGLONG:   f[0] = 81  #"Q"
- *             elif t == NPY_FLOAT:       f[0] = 102 #"f"
- *             elif t == NPY_DOUBLE:      f[0] = 100 #"d"             # <<<<<<<<<<<<<<
- *             elif t == NPY_LONGDOUBLE:  f[0] = 103 #"g"
- *             elif t == NPY_CFLOAT:      f[0] = 90; f[1] = 102; f += 1 # Zf
- */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_DOUBLE); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 893, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 893, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 893, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 0x64;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":894
- *             elif t == NPY_FLOAT:       f[0] = 102 #"f"
- *             elif t == NPY_DOUBLE:      f[0] = 100 #"d"
- *             elif t == NPY_LONGDOUBLE:  f[0] = 103 #"g"             # <<<<<<<<<<<<<<
- *             elif t == NPY_CFLOAT:      f[0] = 90; f[1] = 102; f += 1 # Zf
- *             elif t == NPY_CDOUBLE:     f[0] = 90; f[1] = 100; f += 1 # Zd
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_LONGDOUBLE); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 894, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 894, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 894, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 0x67;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":895
- *             elif t == NPY_DOUBLE:      f[0] = 100 #"d"
- *             elif t == NPY_LONGDOUBLE:  f[0] = 103 #"g"
- *             elif t == NPY_CFLOAT:      f[0] = 90; f[1] = 102; f += 1 # Zf             # <<<<<<<<<<<<<<
- *             elif t == NPY_CDOUBLE:     f[0] = 90; f[1] = 100; f += 1 # Zd
- *             elif t == NPY_CLONGDOUBLE: f[0] = 90; f[1] = 103; f += 1 # Zg
- */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_CFLOAT); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 895, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 895, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 895, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 90;
-        (__pyx_v_f[1]) = 0x66;
-        __pyx_v_f = (__pyx_v_f + 1);
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":896
- *             elif t == NPY_LONGDOUBLE:  f[0] = 103 #"g"
- *             elif t == NPY_CFLOAT:      f[0] = 90; f[1] = 102; f += 1 # Zf
- *             elif t == NPY_CDOUBLE:     f[0] = 90; f[1] = 100; f += 1 # Zd             # <<<<<<<<<<<<<<
- *             elif t == NPY_CLONGDOUBLE: f[0] = 90; f[1] = 103; f += 1 # Zg
- *             elif t == NPY_OBJECT:      f[0] = 79 #"O"
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_CDOUBLE); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 896, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 896, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 896, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 90;
-        (__pyx_v_f[1]) = 0x64;
-        __pyx_v_f = (__pyx_v_f + 1);
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":897
- *             elif t == NPY_CFLOAT:      f[0] = 90; f[1] = 102; f += 1 # Zf
- *             elif t == NPY_CDOUBLE:     f[0] = 90; f[1] = 100; f += 1 # Zd
- *             elif t == NPY_CLONGDOUBLE: f[0] = 90; f[1] = 103; f += 1 # Zg             # <<<<<<<<<<<<<<
- *             elif t == NPY_OBJECT:      f[0] = 79 #"O"
- *             else:
- */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_CLONGDOUBLE); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 897, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 897, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 897, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 90;
-        (__pyx_v_f[1]) = 0x67;
-        __pyx_v_f = (__pyx_v_f + 1);
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":898
- *             elif t == NPY_CDOUBLE:     f[0] = 90; f[1] = 100; f += 1 # Zd
- *             elif t == NPY_CLONGDOUBLE: f[0] = 90; f[1] = 103; f += 1 # Zg
- *             elif t == NPY_OBJECT:      f[0] = 79 #"O"             # <<<<<<<<<<<<<<
- *             else:
- *                 raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_OBJECT); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 898, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 898, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 898, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (likely(__pyx_t_6)) {
-        (__pyx_v_f[0]) = 79;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":900
- *             elif t == NPY_OBJECT:      f[0] = 79 #"O"
- *             else:
- *                 raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)             # <<<<<<<<<<<<<<
- *             f += 1
- *         else:
- */
-      /*else*/ {
-        __pyx_t_3 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_unknown_dtype_code_in_numpy_pxd, __pyx_v_t); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 900, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 900, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_4);
-        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        __Pyx_Raise(__pyx_t_4, 0, 0, 0);
-        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        __PYX_ERR(1, 900, __pyx_L1_error)
-      }
-      __pyx_L15:;
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":901
- *             else:
- *                 raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)
- *             f += 1             # <<<<<<<<<<<<<<
- *         else:
- *             # Cython ignores struct boundary information ("T{...}"),
- */
-      __pyx_v_f = (__pyx_v_f + 1);
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":876
- *         offset[0] += child.itemsize
- * 
- *         if not PyDataType_HASFIELDS(child):             # <<<<<<<<<<<<<<
- *             t = child.type_num
- *             if end - f < 5:
- */
-      goto __pyx_L13;
-    }
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":905
- *             # Cython ignores struct boundary information ("T{...}"),
- *             # so don't output it
- *             f = _util_dtypestring(child, f, end, offset)             # <<<<<<<<<<<<<<
- *     return f
- * 
- */
-    /*else*/ {
-      __pyx_t_9 = __pyx_f_5numpy__util_dtypestring(__pyx_v_child, __pyx_v_f, __pyx_v_end, __pyx_v_offset); if (unlikely(__pyx_t_9 == ((char *)NULL))) __PYX_ERR(1, 905, __pyx_L1_error)
-      __pyx_v_f = __pyx_t_9;
-    }
-    __pyx_L13:;
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":850
- *     cdef tuple fields
- * 
- *     for childname in descr.names:             # <<<<<<<<<<<<<<
- *         fields = descr.fields[childname]
- *         child, new_offset = fields
- */
-  }
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":906
- *             # so don't output it
- *             f = _util_dtypestring(child, f, end, offset)
- *     return f             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = __pyx_v_f;
-  goto __pyx_L0;
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":841
- *         return ()
- * 
- * cdef inline char* _util_dtypestring(dtype descr, char* f, char* end, int* offset) except NULL:             # <<<<<<<<<<<<<<
- *     # Recursive utility function used in __getbuffer__ to get format
- *     # string. The new location in the format string is returned.
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_AddTraceback("numpy._util_dtypestring", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XDECREF((PyObject *)__pyx_v_child);
-  __Pyx_XDECREF(__pyx_v_fields);
-  __Pyx_XDECREF(__pyx_v_childname);
-  __Pyx_XDECREF(__pyx_v_new_offset);
-  __Pyx_XDECREF(__pyx_v_t);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1021
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1022
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":930
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1023
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":931
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1021
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1025
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1026
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":934
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1027
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1028
+    /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":936
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1027
+    /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1029
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":937
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1025
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1033
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
- *         _import_array()
+ *         __pyx_import_array()
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_import_array(void) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
@@ -5831,105 +4210,105 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1034
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
- *         _import_array()
+ *         __pyx_import_array()
  *     except Exception:
  */
   {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1035
+      /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":943
  * cdef inline int import_array() except -1:
  *     try:
- *         _import_array()             # <<<<<<<<<<<<<<
+ *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 1035, __pyx_L3_error)
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 943, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1034
+      /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
- *         _import_array()
+ *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1036
+    /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *     try:
- *         _import_array()
+ *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 1036, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 944, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1037
- *         _import_array()
+      /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":945
+ *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 1037, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 945, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 1037, __pyx_L5_except_error)
+      __PYX_ERR(1, 945, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1034
+    /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
- *         _import_array()
+ *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1033
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
- *         _import_array()
+ *         __pyx_import_array()
  */
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_5);
@@ -5939,15 +4318,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1039
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5963,15 +4342,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1040
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -5979,84 +4358,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1041
+      /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":949
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 1041, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 949, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1040
+      /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1042
+    /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 1042, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 950, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1043
+      /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 1043, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 951, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 1043, __pyx_L5_except_error)
+      __PYX_ERR(1, 951, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1040
+    /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1039
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6071,15 +4450,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1045
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6095,15 +4474,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1046
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -6111,81 +4490,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1047
+      /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":955
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 1047, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 955, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1046
+      /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1048
+    /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":956
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
+ * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 1048, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 956, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1049
+      /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":957
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
+ * 
+ * cdef extern from *:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 1049, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 957, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 1049, __pyx_L5_except_error)
+      __PYX_ERR(1, 957, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1046
+    /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1045
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6200,14 +4582,188 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":967
+ * 
+ * 
+ * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.timedelta64)`
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
+
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":979
+ *     bool
+ *     """
+ *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":967
+ * 
+ * 
+ * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.timedelta64)`
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":982
+ * 
+ * 
+ * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.datetime64)`
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("is_datetime64_object", 0);
+
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":994
+ *     bool
+ *     """
+ *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":982
+ * 
+ * 
+ * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.datetime64)`
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":997
+ * 
+ * 
+ * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy datetime64 object
+ */
+
+static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
+  npy_datetime __pyx_r;
+
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":1004
+ *     also needed.  That can be found using `get_datetime64_unit`.
+ *     """
+ *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":997
+ * 
+ * 
+ * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy datetime64 object
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":1007
+ * 
+ * 
+ * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy timedelta64 object
+ */
+
+static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
+  npy_timedelta __pyx_r;
+
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":1011
+ *     returns the int64 value underlying scalar numpy timedelta64 object
+ *     """
+ *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":1007
+ * 
+ * 
+ * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy timedelta64 object
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":1014
+ * 
+ * 
+ * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the unit part of the dtype for a numpy datetime64 object.
+ */
+
+static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
+  NPY_DATETIMEUNIT __pyx_r;
+
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":1018
+ *     returns the unit part of the dtype for a numpy datetime64 object.
+ *     """
+ *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
+ */
+  __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":1014
+ * 
+ * 
+ * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the unit part of the dtype for a numpy datetime64 object.
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
 /* "View.MemoryView":123
  *         cdef bint dtype_is_object
  * 
  *     def __cinit__(array self, tuple shape, Py_ssize_t itemsize, format not None,             # <<<<<<<<<<<<<<
  *                   mode="c", bint allocate_buffer=True):
  * 
  */
@@ -6403,15 +4959,15 @@
     /* "View.MemoryView":134
  * 
  *         if not self.ndim:
  *             raise ValueError("Empty shape tuple for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if itemsize <= 0:
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 134, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 134, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(2, 134, __pyx_L1_error)
 
     /* "View.MemoryView":133
  *         self.itemsize = itemsize
@@ -6435,15 +4991,15 @@
     /* "View.MemoryView":137
  * 
  *         if itemsize <= 0:
  *             raise ValueError("itemsize <= 0 for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if not isinstance(format, bytes):
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 137, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 137, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(2, 137, __pyx_L1_error)
 
     /* "View.MemoryView":136
  *             raise ValueError("Empty shape tuple for cython.array")
@@ -6562,15 +5118,15 @@
     /* "View.MemoryView":149
  * 
  *         if not self._shape:
  *             raise MemoryError("unable to allocate shape and strides.")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 149, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 149, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(2, 149, __pyx_L1_error)
 
     /* "View.MemoryView":148
  *         self._strides = self._shape + self.ndim
@@ -6836,15 +5392,15 @@
       /* "View.MemoryView":177
  *             self.data = <char *>malloc(self.len)
  *             if not self.data:
  *                 raise MemoryError("unable to allocate array data.")             # <<<<<<<<<<<<<<
  * 
  *             if self.dtype_is_object:
  */
-      __pyx_t_10 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(2, 177, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(2, 177, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_Raise(__pyx_t_10, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       __PYX_ERR(2, 177, __pyx_L1_error)
 
       /* "View.MemoryView":176
  * 
@@ -7080,15 +5636,15 @@
     /* "View.MemoryView":193
  *             bufmode = PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         if not (flags & bufmode):
  *             raise ValueError("Can only create a buffer that is contiguous in memory.")             # <<<<<<<<<<<<<<
  *         info.buf = self.data
  *         info.len = self.len
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 193, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 193, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(2, 193, __pyx_L1_error)
 
     /* "View.MemoryView":192
  *         elif self.mode == u"fortran":
@@ -7814,15 +6370,15 @@
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(2, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
@@ -7870,15 +6426,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__14, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(2, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
@@ -9599,15 +8155,15 @@
     /* "View.MemoryView":420
  *     def __setitem__(memoryview self, object index, object value):
  *         if self.view.readonly:
  *             raise TypeError("Cannot assign to read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         have_slices, index = _unellipsify(index, self.view.ndim)
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__15, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 420, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 420, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __PYX_ERR(2, 420, __pyx_L1_error)
 
     /* "View.MemoryView":419
  * 
@@ -10647,15 +9203,15 @@
       /* "View.MemoryView":497
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:
  *             raise ValueError("Unable to convert item to object")             # <<<<<<<<<<<<<<
  *         else:
  *             if len(self.view.format) == 1:
  */
-      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__16, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 497, __pyx_L5_except_error)
+      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 497, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_Raise(__pyx_t_6, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __PYX_ERR(2, 497, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
@@ -11009,15 +9565,15 @@
     /* "View.MemoryView":522
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         if flags & PyBUF_WRITABLE and self.view.readonly:
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_ND:
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__17, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 522, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 522, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(2, 522, __pyx_L1_error)
 
     /* "View.MemoryView":521
  *     @cname('getbuffer')
@@ -11558,15 +10114,15 @@
     /* "View.MemoryView":572
  *         if self.view.strides == NULL:
  * 
  *             raise ValueError("Buffer view does not expose strides")             # <<<<<<<<<<<<<<
  * 
  *         return tuple([stride for stride in self.view.strides[:self.view.ndim]])
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__18, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 572, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 572, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __PYX_ERR(2, 572, __pyx_L1_error)
 
     /* "View.MemoryView":570
  *     @property
@@ -11675,15 +10231,15 @@
  *             return (-1,) * self.view.ndim             # <<<<<<<<<<<<<<
  * 
  *         return tuple([suboffset for suboffset in self.view.suboffsets[:self.view.ndim]])
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_self->view.ndim); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 579, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = PyNumber_Multiply(__pyx_tuple__19, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 579, __pyx_L1_error)
+    __pyx_t_3 = PyNumber_Multiply(__pyx_tuple__14, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 579, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
     /* "View.MemoryView":578
@@ -12713,15 +11269,15 @@
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__20, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__15, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(2, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
@@ -12769,15 +11325,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__21, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__16, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(2, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
@@ -13126,17 +11682,17 @@
  *             else:
  */
         __pyx_t_8 = PyObject_Length(__pyx_v_tup); if (unlikely(__pyx_t_8 == ((Py_ssize_t)-1))) __PYX_ERR(2, 684, __pyx_L1_error)
         __pyx_t_7 = PyList_New(1 * ((((__pyx_v_ndim - __pyx_t_8) + 1)<0) ? 0:((__pyx_v_ndim - __pyx_t_8) + 1))); if (unlikely(!__pyx_t_7)) __PYX_ERR(2, 684, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
         { Py_ssize_t __pyx_temp;
           for (__pyx_temp=0; __pyx_temp < ((__pyx_v_ndim - __pyx_t_8) + 1); __pyx_temp++) {
-            __Pyx_INCREF(__pyx_slice__22);
-            __Pyx_GIVEREF(__pyx_slice__22);
-            PyList_SET_ITEM(__pyx_t_7, __pyx_temp, __pyx_slice__22);
+            __Pyx_INCREF(__pyx_slice__17);
+            __Pyx_GIVEREF(__pyx_slice__17);
+            PyList_SET_ITEM(__pyx_t_7, __pyx_temp, __pyx_slice__17);
           }
         }
         __pyx_t_9 = __Pyx_PyList_Extend(__pyx_v_result, __pyx_t_7); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(2, 684, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
         /* "View.MemoryView":685
  *             if not seen_ellipsis:
@@ -13161,15 +11717,15 @@
  *                 seen_ellipsis = True
  *             else:
  *                 result.append(slice(None))             # <<<<<<<<<<<<<<
  *             have_slices = True
  *         else:
  */
       /*else*/ {
-        __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_result, __pyx_slice__22); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(2, 687, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_result, __pyx_slice__17); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(2, 687, __pyx_L1_error)
       }
       __pyx_L7:;
 
       /* "View.MemoryView":688
  *             else:
  *                 result.append(slice(None))
  *             have_slices = True             # <<<<<<<<<<<<<<
@@ -13301,17 +11857,17 @@
  * 
  *     return have_slices or nslices, tuple(result)
  */
     __pyx_t_3 = PyList_New(1 * ((__pyx_v_nslices<0) ? 0:__pyx_v_nslices)); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 698, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     { Py_ssize_t __pyx_temp;
       for (__pyx_temp=0; __pyx_temp < __pyx_v_nslices; __pyx_temp++) {
-        __Pyx_INCREF(__pyx_slice__22);
-        __Pyx_GIVEREF(__pyx_slice__22);
-        PyList_SET_ITEM(__pyx_t_3, __pyx_temp, __pyx_slice__22);
+        __Pyx_INCREF(__pyx_slice__17);
+        __Pyx_GIVEREF(__pyx_slice__17);
+        PyList_SET_ITEM(__pyx_t_3, __pyx_temp, __pyx_slice__17);
       }
     }
     __pyx_t_9 = __Pyx_PyList_Extend(__pyx_v_result, __pyx_t_3); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(2, 698, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
     /* "View.MemoryView":697
  * 
@@ -13430,15 +11986,15 @@
       /* "View.MemoryView":705
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:
  *             raise ValueError("Indirect dimensions not supported")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-      __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__23, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 705, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__18, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 705, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_Raise(__pyx_t_5, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __PYX_ERR(2, 705, __pyx_L1_error)
 
       /* "View.MemoryView":704
  * cdef assert_direct_dimensions(Py_ssize_t *suboffsets, int ndim):
@@ -15614,15 +14170,15 @@
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__24, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__19, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(2, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
@@ -15670,15 +14226,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__25, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__20, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(2, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
@@ -18947,15 +17503,15 @@
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xb068931, 0x82a3537, 0x6ae9995):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb068931, 0x82a3537, 0x6ae9995) = (name))" % __pyx_checksum)
  */
   __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__26, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__21, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(2, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xb068931, 0x82a3537, 0x6ae9995):
@@ -20022,30 +18578,26 @@
   {&__pyx_kp_s_Buffer_view_does_not_expose_stri, __pyx_k_Buffer_view_does_not_expose_stri, sizeof(__pyx_k_Buffer_view_does_not_expose_stri), 0, 0, 1, 0},
   {&__pyx_kp_s_Can_only_create_a_buffer_that_is, __pyx_k_Can_only_create_a_buffer_that_is, sizeof(__pyx_k_Can_only_create_a_buffer_that_is), 0, 0, 1, 0},
   {&__pyx_kp_s_Cannot_assign_to_read_only_memor, __pyx_k_Cannot_assign_to_read_only_memor, sizeof(__pyx_k_Cannot_assign_to_read_only_memor), 0, 0, 1, 0},
   {&__pyx_kp_s_Cannot_create_writable_memory_vi, __pyx_k_Cannot_create_writable_memory_vi, sizeof(__pyx_k_Cannot_create_writable_memory_vi), 0, 0, 1, 0},
   {&__pyx_kp_s_Cannot_index_with_type_s, __pyx_k_Cannot_index_with_type_s, sizeof(__pyx_k_Cannot_index_with_type_s), 0, 0, 1, 0},
   {&__pyx_n_s_Ellipsis, __pyx_k_Ellipsis, sizeof(__pyx_k_Ellipsis), 0, 0, 1, 1},
   {&__pyx_kp_s_Empty_shape_tuple_for_cython_arr, __pyx_k_Empty_shape_tuple_for_cython_arr, sizeof(__pyx_k_Empty_shape_tuple_for_cython_arr), 0, 0, 1, 0},
-  {&__pyx_kp_u_Format_string_allocated_too_shor, __pyx_k_Format_string_allocated_too_shor, sizeof(__pyx_k_Format_string_allocated_too_shor), 0, 1, 0, 0},
-  {&__pyx_kp_u_Format_string_allocated_too_shor_2, __pyx_k_Format_string_allocated_too_shor_2, sizeof(__pyx_k_Format_string_allocated_too_shor_2), 0, 1, 0, 0},
   {&__pyx_n_s_ImportError, __pyx_k_ImportError, sizeof(__pyx_k_ImportError), 0, 0, 1, 1},
   {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_k_Incompatible_checksums_0x_x_vs_0, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0), 0, 0, 1, 0},
   {&__pyx_n_s_IndexError, __pyx_k_IndexError, sizeof(__pyx_k_IndexError), 0, 0, 1, 1},
   {&__pyx_kp_s_Indirect_dimensions_not_supporte, __pyx_k_Indirect_dimensions_not_supporte, sizeof(__pyx_k_Indirect_dimensions_not_supporte), 0, 0, 1, 0},
   {&__pyx_kp_s_Invalid_mode_expected_c_or_fortr, __pyx_k_Invalid_mode_expected_c_or_fortr, sizeof(__pyx_k_Invalid_mode_expected_c_or_fortr), 0, 0, 1, 0},
   {&__pyx_kp_s_Invalid_shape_in_axis_d_d, __pyx_k_Invalid_shape_in_axis_d_d, sizeof(__pyx_k_Invalid_shape_in_axis_d_d), 0, 0, 1, 0},
   {&__pyx_n_s_MemoryError, __pyx_k_MemoryError, sizeof(__pyx_k_MemoryError), 0, 0, 1, 1},
   {&__pyx_kp_s_MemoryView_of_r_at_0x_x, __pyx_k_MemoryView_of_r_at_0x_x, sizeof(__pyx_k_MemoryView_of_r_at_0x_x), 0, 0, 1, 0},
   {&__pyx_kp_s_MemoryView_of_r_object, __pyx_k_MemoryView_of_r_object, sizeof(__pyx_k_MemoryView_of_r_object), 0, 0, 1, 0},
-  {&__pyx_kp_u_Non_native_byte_order_not_suppor, __pyx_k_Non_native_byte_order_not_suppor, sizeof(__pyx_k_Non_native_byte_order_not_suppor), 0, 1, 0, 0},
   {&__pyx_n_b_O, __pyx_k_O, sizeof(__pyx_k_O), 0, 0, 0, 1},
   {&__pyx_kp_s_Out_of_bounds_on_buffer_access_a, __pyx_k_Out_of_bounds_on_buffer_access_a, sizeof(__pyx_k_Out_of_bounds_on_buffer_access_a), 0, 0, 1, 0},
   {&__pyx_n_s_PickleError, __pyx_k_PickleError, sizeof(__pyx_k_PickleError), 0, 0, 1, 1},
-  {&__pyx_n_s_RuntimeError, __pyx_k_RuntimeError, sizeof(__pyx_k_RuntimeError), 0, 0, 1, 1},
   {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
   {&__pyx_kp_s_Unable_to_convert_item_to_object, __pyx_k_Unable_to_convert_item_to_object, sizeof(__pyx_k_Unable_to_convert_item_to_object), 0, 0, 1, 0},
   {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
   {&__pyx_n_s_View_MemoryView, __pyx_k_View_MemoryView, sizeof(__pyx_k_View_MemoryView), 0, 0, 1, 1},
   {&__pyx_n_s_allocate_buffer, __pyx_k_allocate_buffer, sizeof(__pyx_k_allocate_buffer), 0, 0, 1, 1},
   {&__pyx_n_s_base, __pyx_k_base, sizeof(__pyx_k_base), 0, 0, 1, 1},
   {&__pyx_n_s_c, __pyx_k_c, sizeof(__pyx_k_c), 0, 0, 1, 1},
@@ -20076,16 +18628,14 @@
   {&__pyx_kp_s_itemsize_0_for_cython_array, __pyx_k_itemsize_0_for_cython_array, sizeof(__pyx_k_itemsize_0_for_cython_array), 0, 0, 1, 0},
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
   {&__pyx_n_s_memview, __pyx_k_memview, sizeof(__pyx_k_memview), 0, 0, 1, 1},
   {&__pyx_n_s_mode, __pyx_k_mode, sizeof(__pyx_k_mode), 0, 0, 1, 1},
   {&__pyx_n_s_multiply, __pyx_k_multiply, sizeof(__pyx_k_multiply), 0, 0, 1, 1},
   {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
   {&__pyx_n_s_name_2, __pyx_k_name_2, sizeof(__pyx_k_name_2), 0, 0, 1, 1},
-  {&__pyx_kp_u_ndarray_is_not_C_contiguous, __pyx_k_ndarray_is_not_C_contiguous, sizeof(__pyx_k_ndarray_is_not_C_contiguous), 0, 1, 0, 0},
-  {&__pyx_kp_u_ndarray_is_not_Fortran_contiguou, __pyx_k_ndarray_is_not_Fortran_contiguou, sizeof(__pyx_k_ndarray_is_not_Fortran_contiguou), 0, 1, 0, 0},
   {&__pyx_n_s_ndim, __pyx_k_ndim, sizeof(__pyx_k_ndim), 0, 0, 1, 1},
   {&__pyx_n_s_new, __pyx_k_new, sizeof(__pyx_k_new), 0, 0, 1, 1},
   {&__pyx_kp_s_no_default___reduce___due_to_non, __pyx_k_no_default___reduce___due_to_non, sizeof(__pyx_k_no_default___reduce___due_to_non), 0, 0, 1, 0},
   {&__pyx_n_s_np, __pyx_k_np, sizeof(__pyx_k_np), 0, 0, 1, 1},
   {&__pyx_n_s_numpy, __pyx_k_numpy, sizeof(__pyx_k_numpy), 0, 0, 1, 1},
   {&__pyx_kp_u_numpy_core_multiarray_failed_to, __pyx_k_numpy_core_multiarray_failed_to, sizeof(__pyx_k_numpy_core_multiarray_failed_to), 0, 1, 0, 0},
   {&__pyx_kp_u_numpy_core_umath_failed_to_impor, __pyx_k_numpy_core_umath_failed_to_impor, sizeof(__pyx_k_numpy_core_umath_failed_to_impor), 0, 1, 0, 0},
@@ -20117,25 +18667,23 @@
   {&__pyx_kp_s_strided_and_direct_or_indirect, __pyx_k_strided_and_direct_or_indirect, sizeof(__pyx_k_strided_and_direct_or_indirect), 0, 0, 1, 0},
   {&__pyx_kp_s_strided_and_indirect, __pyx_k_strided_and_indirect, sizeof(__pyx_k_strided_and_indirect), 0, 0, 1, 0},
   {&__pyx_kp_s_stringsource, __pyx_k_stringsource, sizeof(__pyx_k_stringsource), 0, 0, 1, 0},
   {&__pyx_n_s_struct, __pyx_k_struct, sizeof(__pyx_k_struct), 0, 0, 1, 1},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_kp_s_unable_to_allocate_array_data, __pyx_k_unable_to_allocate_array_data, sizeof(__pyx_k_unable_to_allocate_array_data), 0, 0, 1, 0},
   {&__pyx_kp_s_unable_to_allocate_shape_and_str, __pyx_k_unable_to_allocate_shape_and_str, sizeof(__pyx_k_unable_to_allocate_shape_and_str), 0, 0, 1, 0},
-  {&__pyx_kp_u_unknown_dtype_code_in_numpy_pxd, __pyx_k_unknown_dtype_code_in_numpy_pxd, sizeof(__pyx_k_unknown_dtype_code_in_numpy_pxd), 0, 1, 0, 0},
   {&__pyx_n_s_unpack, __pyx_k_unpack, sizeof(__pyx_k_unpack), 0, 0, 1, 1},
   {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
   {&__pyx_n_s_zeros, __pyx_k_zeros, sizeof(__pyx_k_zeros), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 55, __pyx_L1_error)
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(1, 272, __pyx_L1_error)
-  __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(1, 855, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 1037, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 945, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(2, 134, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(2, 149, __pyx_L1_error)
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(2, 152, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(2, 2, __pyx_L1_error)
   __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(2, 406, __pyx_L1_error)
   __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(2, 615, __pyx_L1_error)
   __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(2, 834, __pyx_L1_error)
   return 0;
@@ -20143,350 +18691,295 @@
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":272
- *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_C_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not C contiguous")             # <<<<<<<<<<<<<<
- * 
- *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)
- */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_ndarray_is_not_C_contiguous); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 272, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple_);
-  __Pyx_GIVEREF(__pyx_tuple_);
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":276
- *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_F_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not Fortran contiguous")             # <<<<<<<<<<<<<<
- * 
- *             info.buf = PyArray_DATA(self)
- */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_ndarray_is_not_Fortran_contiguou); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 276, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__2);
-  __Pyx_GIVEREF(__pyx_tuple__2);
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":306
- *                 if ((descr.byteorder == c'>' and little_endian) or
- *                     (descr.byteorder == c'<' and not little_endian)):
- *                     raise ValueError(u"Non-native byte order not supported")             # <<<<<<<<<<<<<<
- *                 if   t == NPY_BYTE:        f = "b"
- *                 elif t == NPY_UBYTE:       f = "B"
- */
-  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_Non_native_byte_order_not_suppor); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 306, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__3);
-  __Pyx_GIVEREF(__pyx_tuple__3);
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":855
- * 
- *         if (end - f) - <int>(new_offset - offset[0]) < 15:
- *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")             # <<<<<<<<<<<<<<
- * 
- *         if ((child.byteorder == c'>' and little_endian) or
- */
-  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_u_Format_string_allocated_too_shor); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 855, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__4);
-  __Pyx_GIVEREF(__pyx_tuple__4);
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":879
- *             t = child.type_num
- *             if end - f < 5:
- *                 raise RuntimeError(u"Format string allocated too short.")             # <<<<<<<<<<<<<<
- * 
- *             # Until ticket #99 is fixed, use integers to avoid warnings
- */
-  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_u_Format_string_allocated_too_shor_2); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(1, 879, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__5);
-  __Pyx_GIVEREF(__pyx_tuple__5);
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1037
- *         _import_array()
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":945
+ *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(1, 1037, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__6);
-  __Pyx_GIVEREF(__pyx_tuple__6);
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 945, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple_);
+  __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1043
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(1, 1043, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__7);
-  __Pyx_GIVEREF(__pyx_tuple__7);
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 951, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__2);
+  __Pyx_GIVEREF(__pyx_tuple__2);
 
   /* "View.MemoryView":134
  * 
  *         if not self.ndim:
  *             raise ValueError("Empty shape tuple for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if itemsize <= 0:
  */
-  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_s_Empty_shape_tuple_for_cython_arr); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(2, 134, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__8);
-  __Pyx_GIVEREF(__pyx_tuple__8);
+  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_s_Empty_shape_tuple_for_cython_arr); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(2, 134, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__3);
+  __Pyx_GIVEREF(__pyx_tuple__3);
 
   /* "View.MemoryView":137
  * 
  *         if itemsize <= 0:
  *             raise ValueError("itemsize <= 0 for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if not isinstance(format, bytes):
  */
-  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_s_itemsize_0_for_cython_array); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 137, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__9);
-  __Pyx_GIVEREF(__pyx_tuple__9);
+  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_s_itemsize_0_for_cython_array); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(2, 137, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__4);
+  __Pyx_GIVEREF(__pyx_tuple__4);
 
   /* "View.MemoryView":149
  * 
  *         if not self._shape:
  *             raise MemoryError("unable to allocate shape and strides.")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_shape_and_str); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 149, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__10);
-  __Pyx_GIVEREF(__pyx_tuple__10);
+  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_shape_and_str); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(2, 149, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__5);
+  __Pyx_GIVEREF(__pyx_tuple__5);
 
   /* "View.MemoryView":177
  *             self.data = <char *>malloc(self.len)
  *             if not self.data:
  *                 raise MemoryError("unable to allocate array data.")             # <<<<<<<<<<<<<<
  * 
  *             if self.dtype_is_object:
  */
-  __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_array_data); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(2, 177, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__11);
-  __Pyx_GIVEREF(__pyx_tuple__11);
+  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_array_data); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(2, 177, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__6);
+  __Pyx_GIVEREF(__pyx_tuple__6);
 
   /* "View.MemoryView":193
  *             bufmode = PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         if not (flags & bufmode):
  *             raise ValueError("Can only create a buffer that is contiguous in memory.")             # <<<<<<<<<<<<<<
  *         info.buf = self.data
  *         info.len = self.len
  */
-  __pyx_tuple__12 = PyTuple_Pack(1, __pyx_kp_s_Can_only_create_a_buffer_that_is); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(2, 193, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__12);
-  __Pyx_GIVEREF(__pyx_tuple__12);
+  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_s_Can_only_create_a_buffer_that_is); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(2, 193, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__7);
+  __Pyx_GIVEREF(__pyx_tuple__7);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_tuple__13 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(2, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__13);
-  __Pyx_GIVEREF(__pyx_tuple__13);
+  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(2, 2, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__8);
+  __Pyx_GIVEREF(__pyx_tuple__8);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__14 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(2, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__14);
-  __Pyx_GIVEREF(__pyx_tuple__14);
+  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__9);
+  __Pyx_GIVEREF(__pyx_tuple__9);
 
   /* "View.MemoryView":420
  *     def __setitem__(memoryview self, object index, object value):
  *         if self.view.readonly:
  *             raise TypeError("Cannot assign to read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         have_slices, index = _unellipsify(index, self.view.ndim)
  */
-  __pyx_tuple__15 = PyTuple_Pack(1, __pyx_kp_s_Cannot_assign_to_read_only_memor); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(2, 420, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__15);
-  __Pyx_GIVEREF(__pyx_tuple__15);
+  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_s_Cannot_assign_to_read_only_memor); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 420, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__10);
+  __Pyx_GIVEREF(__pyx_tuple__10);
 
   /* "View.MemoryView":497
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:
  *             raise ValueError("Unable to convert item to object")             # <<<<<<<<<<<<<<
  *         else:
  *             if len(self.view.format) == 1:
  */
-  __pyx_tuple__16 = PyTuple_Pack(1, __pyx_kp_s_Unable_to_convert_item_to_object); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(2, 497, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__16);
-  __Pyx_GIVEREF(__pyx_tuple__16);
+  __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_s_Unable_to_convert_item_to_object); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(2, 497, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__11);
+  __Pyx_GIVEREF(__pyx_tuple__11);
 
   /* "View.MemoryView":522
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         if flags & PyBUF_WRITABLE and self.view.readonly:
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_ND:
  */
-  __pyx_tuple__17 = PyTuple_Pack(1, __pyx_kp_s_Cannot_create_writable_memory_vi); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(2, 522, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__17);
-  __Pyx_GIVEREF(__pyx_tuple__17);
+  __pyx_tuple__12 = PyTuple_Pack(1, __pyx_kp_s_Cannot_create_writable_memory_vi); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(2, 522, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__12);
+  __Pyx_GIVEREF(__pyx_tuple__12);
 
   /* "View.MemoryView":572
  *         if self.view.strides == NULL:
  * 
  *             raise ValueError("Buffer view does not expose strides")             # <<<<<<<<<<<<<<
  * 
  *         return tuple([stride for stride in self.view.strides[:self.view.ndim]])
  */
-  __pyx_tuple__18 = PyTuple_Pack(1, __pyx_kp_s_Buffer_view_does_not_expose_stri); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(2, 572, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__18);
-  __Pyx_GIVEREF(__pyx_tuple__18);
+  __pyx_tuple__13 = PyTuple_Pack(1, __pyx_kp_s_Buffer_view_does_not_expose_stri); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(2, 572, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__13);
+  __Pyx_GIVEREF(__pyx_tuple__13);
 
   /* "View.MemoryView":579
  *     def suboffsets(self):
  *         if self.view.suboffsets == NULL:
  *             return (-1,) * self.view.ndim             # <<<<<<<<<<<<<<
  * 
  *         return tuple([suboffset for suboffset in self.view.suboffsets[:self.view.ndim]])
  */
-  __pyx_tuple__19 = PyTuple_New(1); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(2, 579, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__19);
+  __pyx_tuple__14 = PyTuple_New(1); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(2, 579, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__14);
   __Pyx_INCREF(__pyx_int_neg_1);
   __Pyx_GIVEREF(__pyx_int_neg_1);
-  PyTuple_SET_ITEM(__pyx_tuple__19, 0, __pyx_int_neg_1);
-  __Pyx_GIVEREF(__pyx_tuple__19);
+  PyTuple_SET_ITEM(__pyx_tuple__14, 0, __pyx_int_neg_1);
+  __Pyx_GIVEREF(__pyx_tuple__14);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_tuple__20 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(2, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__20);
-  __Pyx_GIVEREF(__pyx_tuple__20);
+  __pyx_tuple__15 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(2, 2, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__15);
+  __Pyx_GIVEREF(__pyx_tuple__15);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__21 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(2, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__21);
-  __Pyx_GIVEREF(__pyx_tuple__21);
+  __pyx_tuple__16 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__16);
+  __Pyx_GIVEREF(__pyx_tuple__16);
 
   /* "View.MemoryView":684
  *         if item is Ellipsis:
  *             if not seen_ellipsis:
  *                 result.extend([slice(None)] * (ndim - len(tup) + 1))             # <<<<<<<<<<<<<<
  *                 seen_ellipsis = True
  *             else:
  */
-  __pyx_slice__22 = PySlice_New(Py_None, Py_None, Py_None); if (unlikely(!__pyx_slice__22)) __PYX_ERR(2, 684, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_slice__22);
-  __Pyx_GIVEREF(__pyx_slice__22);
+  __pyx_slice__17 = PySlice_New(Py_None, Py_None, Py_None); if (unlikely(!__pyx_slice__17)) __PYX_ERR(2, 684, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_slice__17);
+  __Pyx_GIVEREF(__pyx_slice__17);
 
   /* "View.MemoryView":705
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:
  *             raise ValueError("Indirect dimensions not supported")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__23 = PyTuple_Pack(1, __pyx_kp_s_Indirect_dimensions_not_supporte); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(2, 705, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__23);
-  __Pyx_GIVEREF(__pyx_tuple__23);
+  __pyx_tuple__18 = PyTuple_Pack(1, __pyx_kp_s_Indirect_dimensions_not_supporte); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(2, 705, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__18);
+  __Pyx_GIVEREF(__pyx_tuple__18);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_tuple__24 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(2, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__24);
-  __Pyx_GIVEREF(__pyx_tuple__24);
+  __pyx_tuple__19 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(2, 2, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__19);
+  __Pyx_GIVEREF(__pyx_tuple__19);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__25 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(2, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__25);
-  __Pyx_GIVEREF(__pyx_tuple__25);
-  __pyx_tuple__26 = PyTuple_Pack(3, __pyx_int_184977713, __pyx_int_136983863, __pyx_int_112105877); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(2, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__26);
-  __Pyx_GIVEREF(__pyx_tuple__26);
+  __pyx_tuple__20 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__20);
+  __Pyx_GIVEREF(__pyx_tuple__20);
+  __pyx_tuple__21 = PyTuple_Pack(3, __pyx_int_184977713, __pyx_int_136983863, __pyx_int_112105877); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__21);
+  __Pyx_GIVEREF(__pyx_tuple__21);
 
   /* "View.MemoryView":287
  *         return self.name
  * 
  * cdef generic = Enum("<strided and direct or indirect>")             # <<<<<<<<<<<<<<
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")
  */
-  __pyx_tuple__27 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct_or_indirect); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(2, 287, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__27);
-  __Pyx_GIVEREF(__pyx_tuple__27);
+  __pyx_tuple__22 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct_or_indirect); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(2, 287, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__22);
+  __Pyx_GIVEREF(__pyx_tuple__22);
 
   /* "View.MemoryView":288
  * 
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default             # <<<<<<<<<<<<<<
  * cdef indirect = Enum("<strided and indirect>")
  * 
  */
-  __pyx_tuple__28 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(2, 288, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__28);
-  __Pyx_GIVEREF(__pyx_tuple__28);
+  __pyx_tuple__23 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(2, 288, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__23);
+  __Pyx_GIVEREF(__pyx_tuple__23);
 
   /* "View.MemoryView":289
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__29 = PyTuple_Pack(1, __pyx_kp_s_strided_and_indirect); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(2, 289, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__29);
-  __Pyx_GIVEREF(__pyx_tuple__29);
+  __pyx_tuple__24 = PyTuple_Pack(1, __pyx_kp_s_strided_and_indirect); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(2, 289, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__24);
+  __Pyx_GIVEREF(__pyx_tuple__24);
 
   /* "View.MemoryView":292
  * 
  * 
  * cdef contiguous = Enum("<contiguous and direct>")             # <<<<<<<<<<<<<<
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")
  * 
  */
-  __pyx_tuple__30 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_direct); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(2, 292, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__30);
-  __Pyx_GIVEREF(__pyx_tuple__30);
+  __pyx_tuple__25 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_direct); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(2, 292, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__25);
+  __Pyx_GIVEREF(__pyx_tuple__25);
 
   /* "View.MemoryView":293
  * 
  * cdef contiguous = Enum("<contiguous and direct>")
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__31 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_indirect); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(2, 293, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__31);
-  __Pyx_GIVEREF(__pyx_tuple__31);
+  __pyx_tuple__26 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_indirect); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(2, 293, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__26);
+  __Pyx_GIVEREF(__pyx_tuple__26);
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_Enum(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_tuple__32 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__32)) __PYX_ERR(2, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__32);
-  __Pyx_GIVEREF(__pyx_tuple__32);
-  __pyx_codeobj__33 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__32, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Enum, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__33)) __PYX_ERR(2, 1, __pyx_L1_error)
+  __pyx_tuple__27 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(2, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__27);
+  __Pyx_GIVEREF(__pyx_tuple__27);
+  __pyx_codeobj__28 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__27, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Enum, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__28)) __PYX_ERR(2, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -20621,33 +19114,68 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 206, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 200, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 206, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 229, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 233, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 242, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 917, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT(PyArray_Descr),
+  __Pyx_ImportType_CheckSize_Ignore);
+   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 200, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
+   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 223, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayMultiIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
+   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 227, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayObject),
+  __Pyx_ImportType_CheckSize_Ignore);
+   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 239, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 771, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 773, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 775, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 777, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 779, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 781, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 783, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 785, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 787, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 789, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT(PyUFuncObject),
+  __Pyx_ImportType_CheckSize_Ignore);
+   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 827, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -20908,71 +19436,71 @@
   /* "View.MemoryView":287
  *         return self.name
  * 
  * cdef generic = Enum("<strided and direct or indirect>")             # <<<<<<<<<<<<<<
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__27, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 287, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__22, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 287, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(generic);
   __Pyx_DECREF_SET(generic, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "View.MemoryView":288
  * 
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default             # <<<<<<<<<<<<<<
  * cdef indirect = Enum("<strided and indirect>")
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__28, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 288, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__23, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 288, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(strided);
   __Pyx_DECREF_SET(strided, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "View.MemoryView":289
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__29, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 289, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__24, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 289, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(indirect);
   __Pyx_DECREF_SET(indirect, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "View.MemoryView":292
  * 
  * 
  * cdef contiguous = Enum("<contiguous and direct>")             # <<<<<<<<<<<<<<
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__30, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 292, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__25, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 292, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(contiguous);
   __Pyx_DECREF_SET(contiguous, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "View.MemoryView":293
  * 
  * cdef contiguous = Enum("<contiguous and direct>")
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__31, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 293, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__26, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 293, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(indirect_contiguous);
   __Pyx_DECREF_SET(indirect_contiguous, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "View.MemoryView":317
@@ -21619,228 +20147,14 @@
     }
 #ifdef WITH_THREAD
     if (nogil)
         PyGILState_Release(state);
 #endif
 }
 
-/* RaiseException */
-#if PY_MAJOR_VERSION < 3
-static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb,
-                        CYTHON_UNUSED PyObject *cause) {
-    __Pyx_PyThreadState_declare
-    Py_XINCREF(type);
-    if (!value || value == Py_None)
-        value = NULL;
-    else
-        Py_INCREF(value);
-    if (!tb || tb == Py_None)
-        tb = NULL;
-    else {
-        Py_INCREF(tb);
-        if (!PyTraceBack_Check(tb)) {
-            PyErr_SetString(PyExc_TypeError,
-                "raise: arg 3 must be a traceback or None");
-            goto raise_error;
-        }
-    }
-    if (PyType_Check(type)) {
-#if CYTHON_COMPILING_IN_PYPY
-        if (!value) {
-            Py_INCREF(Py_None);
-            value = Py_None;
-        }
-#endif
-        PyErr_NormalizeException(&type, &value, &tb);
-    } else {
-        if (value) {
-            PyErr_SetString(PyExc_TypeError,
-                "instance exception may not have a separate value");
-            goto raise_error;
-        }
-        value = type;
-        type = (PyObject*) Py_TYPE(type);
-        Py_INCREF(type);
-        if (!PyType_IsSubtype((PyTypeObject *)type, (PyTypeObject *)PyExc_BaseException)) {
-            PyErr_SetString(PyExc_TypeError,
-                "raise: exception class must be a subclass of BaseException");
-            goto raise_error;
-        }
-    }
-    __Pyx_PyThreadState_assign
-    __Pyx_ErrRestore(type, value, tb);
-    return;
-raise_error:
-    Py_XDECREF(value);
-    Py_XDECREF(type);
-    Py_XDECREF(tb);
-    return;
-}
-#else
-static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause) {
-    PyObject* owned_instance = NULL;
-    if (tb == Py_None) {
-        tb = 0;
-    } else if (tb && !PyTraceBack_Check(tb)) {
-        PyErr_SetString(PyExc_TypeError,
-            "raise: arg 3 must be a traceback or None");
-        goto bad;
-    }
-    if (value == Py_None)
-        value = 0;
-    if (PyExceptionInstance_Check(type)) {
-        if (value) {
-            PyErr_SetString(PyExc_TypeError,
-                "instance exception may not have a separate value");
-            goto bad;
-        }
-        value = type;
-        type = (PyObject*) Py_TYPE(value);
-    } else if (PyExceptionClass_Check(type)) {
-        PyObject *instance_class = NULL;
-        if (value && PyExceptionInstance_Check(value)) {
-            instance_class = (PyObject*) Py_TYPE(value);
-            if (instance_class != type) {
-                int is_subclass = PyObject_IsSubclass(instance_class, type);
-                if (!is_subclass) {
-                    instance_class = NULL;
-                } else if (unlikely(is_subclass == -1)) {
-                    goto bad;
-                } else {
-                    type = instance_class;
-                }
-            }
-        }
-        if (!instance_class) {
-            PyObject *args;
-            if (!value)
-                args = PyTuple_New(0);
-            else if (PyTuple_Check(value)) {
-                Py_INCREF(value);
-                args = value;
-            } else
-                args = PyTuple_Pack(1, value);
-            if (!args)
-                goto bad;
-            owned_instance = PyObject_Call(type, args, NULL);
-            Py_DECREF(args);
-            if (!owned_instance)
-                goto bad;
-            value = owned_instance;
-            if (!PyExceptionInstance_Check(value)) {
-                PyErr_Format(PyExc_TypeError,
-                             "calling %R should have returned an instance of "
-                             "BaseException, not %R",
-                             type, Py_TYPE(value));
-                goto bad;
-            }
-        }
-    } else {
-        PyErr_SetString(PyExc_TypeError,
-            "raise: exception class must be a subclass of BaseException");
-        goto bad;
-    }
-    if (cause) {
-        PyObject *fixed_cause;
-        if (cause == Py_None) {
-            fixed_cause = NULL;
-        } else if (PyExceptionClass_Check(cause)) {
-            fixed_cause = PyObject_CallObject(cause, NULL);
-            if (fixed_cause == NULL)
-                goto bad;
-        } else if (PyExceptionInstance_Check(cause)) {
-            fixed_cause = cause;
-            Py_INCREF(fixed_cause);
-        } else {
-            PyErr_SetString(PyExc_TypeError,
-                            "exception causes must derive from "
-                            "BaseException");
-            goto bad;
-        }
-        PyException_SetCause(value, fixed_cause);
-    }
-    PyErr_SetObject(type, value);
-    if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
-        PyThreadState *tstate = __Pyx_PyThreadState_Current;
-        PyObject* tmp_tb = tstate->curexc_traceback;
-        if (tb != tmp_tb) {
-            Py_INCREF(tb);
-            tstate->curexc_traceback = tb;
-            Py_XDECREF(tmp_tb);
-        }
-#endif
-    }
-bad:
-    Py_XDECREF(owned_instance);
-    return;
-}
-#endif
-
-/* DictGetItem */
-#if PY_MAJOR_VERSION >= 3 && !CYTHON_COMPILING_IN_PYPY
-static PyObject *__Pyx_PyDict_GetItem(PyObject *d, PyObject* key) {
-    PyObject *value;
-    value = PyDict_GetItemWithError(d, key);
-    if (unlikely(!value)) {
-        if (!PyErr_Occurred()) {
-            if (unlikely(PyTuple_Check(key))) {
-                PyObject* args = PyTuple_Pack(1, key);
-                if (likely(args)) {
-                    PyErr_SetObject(PyExc_KeyError, args);
-                    Py_DECREF(args);
-                }
-            } else {
-                PyErr_SetObject(PyExc_KeyError, key);
-            }
-        }
-        return NULL;
-    }
-    Py_INCREF(value);
-    return value;
-}
-#endif
-
-/* RaiseTooManyValuesToUnpack */
-static CYTHON_INLINE void __Pyx_RaiseTooManyValuesError(Py_ssize_t expected) {
-    PyErr_Format(PyExc_ValueError,
-                 "too many values to unpack (expected %" CYTHON_FORMAT_SSIZE_T "d)", expected);
-}
-
-/* RaiseNeedMoreValuesToUnpack */
-static CYTHON_INLINE void __Pyx_RaiseNeedMoreValuesError(Py_ssize_t index) {
-    PyErr_Format(PyExc_ValueError,
-                 "need more than %" CYTHON_FORMAT_SSIZE_T "d value%.1s to unpack",
-                 index, (index == 1) ? "" : "s");
-}
-
-/* RaiseNoneIterError */
-static CYTHON_INLINE void __Pyx_RaiseNoneNotIterableError(void) {
-    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-}
-
-/* ExtTypeTest */
-static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type) {
-    if (unlikely(!type)) {
-        PyErr_SetString(PyExc_SystemError, "Missing type object");
-        return 0;
-    }
-    if (likely(__Pyx_TypeCheck(obj, type)))
-        return 1;
-    PyErr_Format(PyExc_TypeError, "Cannot convert %.200s to %.200s",
-                 Py_TYPE(obj)->tp_name, type->tp_name);
-    return 0;
-}
-
 /* GetTopmostException */
 #if CYTHON_USE_EXC_INFO_STACK
 static _PyErr_StackItem *
 __Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
 {
     _PyErr_StackItem *exc_info = tstate->exc_info;
     while ((exc_info->exc_type == NULL || exc_info->exc_type == Py_None) &&
@@ -21988,14 +20302,173 @@
     *tb = 0;
     Py_XDECREF(local_type);
     Py_XDECREF(local_value);
     Py_XDECREF(local_tb);
     return -1;
 }
 
+/* RaiseException */
+#if PY_MAJOR_VERSION < 3
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb,
+                        CYTHON_UNUSED PyObject *cause) {
+    __Pyx_PyThreadState_declare
+    Py_XINCREF(type);
+    if (!value || value == Py_None)
+        value = NULL;
+    else
+        Py_INCREF(value);
+    if (!tb || tb == Py_None)
+        tb = NULL;
+    else {
+        Py_INCREF(tb);
+        if (!PyTraceBack_Check(tb)) {
+            PyErr_SetString(PyExc_TypeError,
+                "raise: arg 3 must be a traceback or None");
+            goto raise_error;
+        }
+    }
+    if (PyType_Check(type)) {
+#if CYTHON_COMPILING_IN_PYPY
+        if (!value) {
+            Py_INCREF(Py_None);
+            value = Py_None;
+        }
+#endif
+        PyErr_NormalizeException(&type, &value, &tb);
+    } else {
+        if (value) {
+            PyErr_SetString(PyExc_TypeError,
+                "instance exception may not have a separate value");
+            goto raise_error;
+        }
+        value = type;
+        type = (PyObject*) Py_TYPE(type);
+        Py_INCREF(type);
+        if (!PyType_IsSubtype((PyTypeObject *)type, (PyTypeObject *)PyExc_BaseException)) {
+            PyErr_SetString(PyExc_TypeError,
+                "raise: exception class must be a subclass of BaseException");
+            goto raise_error;
+        }
+    }
+    __Pyx_PyThreadState_assign
+    __Pyx_ErrRestore(type, value, tb);
+    return;
+raise_error:
+    Py_XDECREF(value);
+    Py_XDECREF(type);
+    Py_XDECREF(tb);
+    return;
+}
+#else
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause) {
+    PyObject* owned_instance = NULL;
+    if (tb == Py_None) {
+        tb = 0;
+    } else if (tb && !PyTraceBack_Check(tb)) {
+        PyErr_SetString(PyExc_TypeError,
+            "raise: arg 3 must be a traceback or None");
+        goto bad;
+    }
+    if (value == Py_None)
+        value = 0;
+    if (PyExceptionInstance_Check(type)) {
+        if (value) {
+            PyErr_SetString(PyExc_TypeError,
+                "instance exception may not have a separate value");
+            goto bad;
+        }
+        value = type;
+        type = (PyObject*) Py_TYPE(value);
+    } else if (PyExceptionClass_Check(type)) {
+        PyObject *instance_class = NULL;
+        if (value && PyExceptionInstance_Check(value)) {
+            instance_class = (PyObject*) Py_TYPE(value);
+            if (instance_class != type) {
+                int is_subclass = PyObject_IsSubclass(instance_class, type);
+                if (!is_subclass) {
+                    instance_class = NULL;
+                } else if (unlikely(is_subclass == -1)) {
+                    goto bad;
+                } else {
+                    type = instance_class;
+                }
+            }
+        }
+        if (!instance_class) {
+            PyObject *args;
+            if (!value)
+                args = PyTuple_New(0);
+            else if (PyTuple_Check(value)) {
+                Py_INCREF(value);
+                args = value;
+            } else
+                args = PyTuple_Pack(1, value);
+            if (!args)
+                goto bad;
+            owned_instance = PyObject_Call(type, args, NULL);
+            Py_DECREF(args);
+            if (!owned_instance)
+                goto bad;
+            value = owned_instance;
+            if (!PyExceptionInstance_Check(value)) {
+                PyErr_Format(PyExc_TypeError,
+                             "calling %R should have returned an instance of "
+                             "BaseException, not %R",
+                             type, Py_TYPE(value));
+                goto bad;
+            }
+        }
+    } else {
+        PyErr_SetString(PyExc_TypeError,
+            "raise: exception class must be a subclass of BaseException");
+        goto bad;
+    }
+    if (cause) {
+        PyObject *fixed_cause;
+        if (cause == Py_None) {
+            fixed_cause = NULL;
+        } else if (PyExceptionClass_Check(cause)) {
+            fixed_cause = PyObject_CallObject(cause, NULL);
+            if (fixed_cause == NULL)
+                goto bad;
+        } else if (PyExceptionInstance_Check(cause)) {
+            fixed_cause = cause;
+            Py_INCREF(fixed_cause);
+        } else {
+            PyErr_SetString(PyExc_TypeError,
+                            "exception causes must derive from "
+                            "BaseException");
+            goto bad;
+        }
+        PyException_SetCause(value, fixed_cause);
+    }
+    PyErr_SetObject(type, value);
+    if (tb) {
+#if CYTHON_FAST_THREAD_STATE
+        PyThreadState *tstate = __Pyx_PyThreadState_Current;
+        PyObject* tmp_tb = tstate->curexc_traceback;
+        if (tb != tmp_tb) {
+            Py_INCREF(tb);
+            tstate->curexc_traceback = tb;
+            Py_XDECREF(tmp_tb);
+        }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
+#endif
+    }
+bad:
+    Py_XDECREF(owned_instance);
+    return;
+}
+#endif
+
 /* RaiseArgTupleInvalid */
 static void __Pyx_RaiseArgtupleInvalid(
     const char* func_name,
     int exact,
     Py_ssize_t num_min,
     Py_ssize_t num_max,
     Py_ssize_t num_found)
@@ -22477,14 +20950,45 @@
     return d;
 }
 static CYTHON_INLINE PyObject *__Pyx_GetAttr3(PyObject *o, PyObject *n, PyObject *d) {
     PyObject *r = __Pyx_GetAttr(o, n);
     return (likely(r)) ? r : __Pyx_GetAttr3Default(d);
 }
 
+/* RaiseTooManyValuesToUnpack */
+static CYTHON_INLINE void __Pyx_RaiseTooManyValuesError(Py_ssize_t expected) {
+    PyErr_Format(PyExc_ValueError,
+                 "too many values to unpack (expected %" CYTHON_FORMAT_SSIZE_T "d)", expected);
+}
+
+/* RaiseNeedMoreValuesToUnpack */
+static CYTHON_INLINE void __Pyx_RaiseNeedMoreValuesError(Py_ssize_t index) {
+    PyErr_Format(PyExc_ValueError,
+                 "need more than %" CYTHON_FORMAT_SSIZE_T "d value%.1s to unpack",
+                 index, (index == 1) ? "" : "s");
+}
+
+/* RaiseNoneIterError */
+static CYTHON_INLINE void __Pyx_RaiseNoneNotIterableError(void) {
+    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
+}
+
+/* ExtTypeTest */
+static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type) {
+    if (unlikely(!type)) {
+        PyErr_SetString(PyExc_SystemError, "Missing type object");
+        return 0;
+    }
+    if (likely(__Pyx_TypeCheck(obj, type)))
+        return 1;
+    PyErr_Format(PyExc_TypeError, "Cannot convert %.200s to %.200s",
+                 Py_TYPE(obj)->tp_name, type->tp_name);
+    return 0;
+}
+
 /* SwapException */
 #if CYTHON_FAST_THREAD_STATE
 static CYTHON_INLINE void __Pyx__ExceptionSwap(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
     PyObject *tmp_type, *tmp_value, *tmp_tb;
     #if CYTHON_USE_EXC_INFO_STACK
     _PyErr_StackItem *exc_info = tstate->exc_info;
     tmp_type = exc_info->exc_type;
@@ -23036,44 +21540,62 @@
     return ret;
 }
 
 /* TypeImport */
 #ifndef __PYX_HAVE_RT_ImportType
 #define __PYX_HAVE_RT_ImportType
 static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
     if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
@@ -23325,29 +21847,27 @@
     Py_XDECREF(py_code);
     Py_XDECREF(py_frame);
 }
 
 #if PY_MAJOR_VERSION < 3
 static int __Pyx_GetBuffer(PyObject *obj, Py_buffer *view, int flags) {
     if (PyObject_CheckBuffer(obj)) return PyObject_GetBuffer(obj, view, flags);
-        if (__Pyx_TypeCheck(obj, __pyx_ptype_5numpy_ndarray)) return __pyx_pw_5numpy_7ndarray_1__getbuffer__(obj, view, flags);
         if (__Pyx_TypeCheck(obj, __pyx_array_type)) return __pyx_array_getbuffer(obj, view, flags);
         if (__Pyx_TypeCheck(obj, __pyx_memoryview_type)) return __pyx_memoryview_getbuffer(obj, view, flags);
     PyErr_Format(PyExc_TypeError, "'%.200s' does not have the buffer interface", Py_TYPE(obj)->tp_name);
     return -1;
 }
 static void __Pyx_ReleaseBuffer(Py_buffer *view) {
     PyObject *obj = view->obj;
     if (!obj) return;
     if (PyObject_CheckBuffer(obj)) {
         PyBuffer_Release(view);
         return;
     }
     if ((0)) {}
-        else if (__Pyx_TypeCheck(obj, __pyx_ptype_5numpy_ndarray)) __pyx_pw_5numpy_7ndarray_3__releasebuffer__(obj, view);
     view->obj = NULL;
     Py_DECREF(obj);
 }
 #endif
 
 
 /* MemviewSliceIsContig */
@@ -24567,36 +23087,14 @@
             z.real = z_r * cosf(z_theta);
             z.imag = z_r * sinf(z_theta);
             return z;
         }
     #endif
 #endif
 
-/* CIntFromPyVerify */
-  #define __PYX_VERIFY_RETURN_INT(target_type, func_type, func_value)\
-    __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 0)
-#define __PYX_VERIFY_RETURN_INT_EXC(target_type, func_type, func_value)\
-    __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 1)
-#define __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, exc)\
-    {\
-        func_type value = func_value;\
-        if (sizeof(target_type) < sizeof(func_type)) {\
-            if (unlikely(value != (func_type) (target_type) value)) {\
-                func_type zero = 0;\
-                if (exc && unlikely(value == (func_type)-1 && PyErr_Occurred()))\
-                    return (target_type) -1;\
-                if (is_unsigned && unlikely(value < zero))\
-                    goto raise_neg_overflow;\
-                else\
-                    goto raise_overflow;\
-            }\
-        }\
-        return (target_type) value;\
-    }
-
 /* MemviewSliceCopyTemplate */
   static __Pyx_memviewslice
 __pyx_memoryview_copy_new_contig(const __Pyx_memviewslice *from_mvs,
                                  const char *mode, int ndim,
                                  size_t sizeof_dtype, int contig_flag,
                                  int dtype_is_object)
 {
@@ -24656,51 +23154,35 @@
     __Pyx_XDECREF(shape_tuple);
     __Pyx_XDECREF(temp_int);
     __Pyx_XDECREF(array_obj);
     __Pyx_RefNannyFinishContext();
     return new_mvs;
 }
 
-/* CIntToPy */
-  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const int neg_one = (int) -1, const_zero = (int) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
-    const int is_unsigned = neg_one > const_zero;
-    if (is_unsigned) {
-        if (sizeof(int) < sizeof(long)) {
-            return PyInt_FromLong((long) value);
-        } else if (sizeof(int) <= sizeof(unsigned long)) {
-            return PyLong_FromUnsignedLong((unsigned long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
-            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
-#endif
-        }
-    } else {
-        if (sizeof(int) <= sizeof(long)) {
-            return PyInt_FromLong((long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
-            return PyLong_FromLongLong((PY_LONG_LONG) value);
-#endif
-        }
-    }
-    {
-        int one = 1; int little = (int)*(unsigned char *)&one;
-        unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(int),
-                                     little, !is_unsigned);
+/* CIntFromPyVerify */
+  #define __PYX_VERIFY_RETURN_INT(target_type, func_type, func_value)\
+    __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 0)
+#define __PYX_VERIFY_RETURN_INT_EXC(target_type, func_type, func_value)\
+    __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 1)
+#define __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, exc)\
+    {\
+        func_type value = func_value;\
+        if (sizeof(target_type) < sizeof(func_type)) {\
+            if (unlikely(value != (func_type) (target_type) value)) {\
+                func_type zero = 0;\
+                if (exc && unlikely(value == (func_type)-1 && PyErr_Occurred()))\
+                    return (target_type) -1;\
+                if (is_unsigned && unlikely(value < zero))\
+                    goto raise_neg_overflow;\
+                else\
+                    goto raise_overflow;\
+            }\
+        }\
+        return (target_type) value;\
     }
-}
 
 /* CIntFromPy */
   static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
@@ -24890,52 +23372,14 @@
     return (int) -1;
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to int");
     return (int) -1;
 }
 
-/* CIntToPy */
-  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_enum__NPY_TYPES(enum NPY_TYPES value) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const enum NPY_TYPES neg_one = (enum NPY_TYPES) -1, const_zero = (enum NPY_TYPES) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
-    const int is_unsigned = neg_one > const_zero;
-    if (is_unsigned) {
-        if (sizeof(enum NPY_TYPES) < sizeof(long)) {
-            return PyInt_FromLong((long) value);
-        } else if (sizeof(enum NPY_TYPES) <= sizeof(unsigned long)) {
-            return PyLong_FromUnsignedLong((unsigned long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(enum NPY_TYPES) <= sizeof(unsigned PY_LONG_LONG)) {
-            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
-#endif
-        }
-    } else {
-        if (sizeof(enum NPY_TYPES) <= sizeof(long)) {
-            return PyInt_FromLong((long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(enum NPY_TYPES) <= sizeof(PY_LONG_LONG)) {
-            return PyLong_FromLongLong((PY_LONG_LONG) value);
-#endif
-        }
-    }
-    {
-        int one = 1; int little = (int)*(unsigned char *)&one;
-        unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(enum NPY_TYPES),
-                                     little, !is_unsigned);
-    }
-}
-
 /* CIntFromPy */
   static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const long neg_one = (long) -1, const_zero = (long) 0;
@@ -25125,14 +23569,52 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to long");
     return (long) -1;
 }
 
 /* CIntToPy */
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const int neg_one = (int) -1, const_zero = (int) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
+    const int is_unsigned = neg_one > const_zero;
+    if (is_unsigned) {
+        if (sizeof(int) < sizeof(long)) {
+            return PyInt_FromLong((long) value);
+        } else if (sizeof(int) <= sizeof(unsigned long)) {
+            return PyLong_FromUnsignedLong((unsigned long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
+            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
+#endif
+        }
+    } else {
+        if (sizeof(int) <= sizeof(long)) {
+            return PyInt_FromLong((long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
+            return PyLong_FromLongLong((PY_LONG_LONG) value);
+#endif
+        }
+    }
+    {
+        int one = 1; int little = (int)*(unsigned char *)&one;
+        unsigned char *bytes = (unsigned char *)&value;
+        return _PyLong_FromByteArray(bytes, sizeof(int),
+                                     little, !is_unsigned);
+    }
+}
+
+/* CIntToPy */
   static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const long neg_one = (long) -1, const_zero = (long) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
```

### Comparing `openTSNE-0.7.1/openTSNE/_matrix_mul/matrix_mul_numpy.pyx` & `openTSNE-1.0.0/openTSNE/_matrix_mul/matrix_mul_numpy.pyx`

 * *Files identical despite different names*

### Comparing `openTSNE-0.7.1/openTSNE/_tsne.cpp` & `openTSNE-1.0.0/openTSNE/_tsne.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "language": "c++",
         "name": "openTSNE._tsne",
@@ -19,16 +19,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_33"
-#define CYTHON_HEX_VERSION 0x001D21F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -213,15 +213,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -252,15 +252,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -768,15 +768,21 @@
 
 #define __PYX_HAVE__openTSNE___tsne
 #define __PYX_HAVE_API__openTSNE___tsne
 /* Early includes */
 #include <string.h>
 #include <stdio.h>
 #include "numpy/arrayobject.h"
+#include "numpy/ndarrayobject.h"
+#include "numpy/ndarraytypes.h"
+#include "numpy/arrayscalars.h"
 #include "numpy/ufuncobject.h"
+
+    /* NumPy API declarations from "numpy/__init__.pxd" */
+    
 #include <stdlib.h>
 #include "math.h"
 #include "pythread.h"
 #include "pystate.h"
 #ifdef _OPENMP
 #include <omp.h>
 #endif /* _OPENMP */
@@ -1115,195 +1121,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":775
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":690
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":776
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":691
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":777
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":778
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":693
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":782
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":697
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":783
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":698
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":784
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":785
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":700
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":789
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":704
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":790
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":705
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":799
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":714
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":800
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":715
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":801
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":716
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":803
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":804
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":805
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":720
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":807
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":722
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":808
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":723
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":810
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":811
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":812
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1335,42 +1341,42 @@
 /*--- Type declarations ---*/
 struct __pyx_obj_8openTSNE_9quad_tree_QuadTree;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":814
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":815
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":730
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":816
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":818
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":733
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -2055,17 +2061,14 @@
 
 /* ArgTypeTest.proto */
 #define __Pyx_ArgTypeTest(obj, type, none_allowed, name, exact)\
     ((likely((Py_TYPE(obj) == type) | (none_allowed && (obj == Py_None)))) ? 1 :\
         __Pyx__ArgTypeTest(obj, type, name, exact))
 static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact);
 
-/* ExtTypeTest.proto */
-static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type);
-
 /* GetTopmostException.proto */
 #if CYTHON_USE_EXC_INFO_STACK
 static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
 #endif
 
 /* SaveResetException.proto */
 #if CYTHON_FAST_THREAD_STATE
@@ -2145,14 +2148,17 @@
          const char* cstring, Py_ssize_t start, Py_ssize_t stop,
          const char* encoding, const char* errors,
          PyObject* (*decode_func)(const char *s, Py_ssize_t size, const char *errors));
 
 /* GetAttr3.proto */
 static CYTHON_INLINE PyObject *__Pyx_GetAttr3(PyObject *, PyObject *, PyObject *);
 
+/* ExtTypeTest.proto */
+static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type);
+
 /* SwapException.proto */
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_ExceptionSwap(type, value, tb)  __Pyx__ExceptionSwap(__pyx_tstate, type, value, tb)
 static CYTHON_INLINE void __Pyx__ExceptionSwap(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
 #else
 static CYTHON_INLINE void __Pyx_ExceptionSwap(PyObject **type, PyObject **value, PyObject **tb);
 #endif
@@ -2249,20 +2255,28 @@
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
 #ifndef __PYX_HAVE_RT_ImportType_proto
 #define __PYX_HAVE_RT_ImportType_proto
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#endif
 enum __Pyx_ImportType_CheckSize {
    __Pyx_ImportType_CheckSize_Error = 0,
    __Pyx_ImportType_CheckSize_Warn = 1,
    __Pyx_ImportType_CheckSize_Ignore = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
 #endif
 
 /* GetVTable.proto */
 static void* __Pyx_GetVtable(PyObject *dict);
 
 /* FetchCommonType.proto */
 static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type);
@@ -2574,17 +2588,14 @@
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
 
 /* BytesContains.proto */
 static CYTHON_INLINE int __Pyx_BytesContains(PyObject* bytes, char character);
 
-/* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_enum__NPY_TYPES(enum NPY_TYPES value);
-
 /* ImportNumPyArray.proto */
 static PyObject *__pyx_numpy_ndarray = NULL;
 static PyObject* __Pyx_ImportNumPyArrayTypeIfAvailable(void);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *);
 
@@ -2636,16 +2647,25 @@
 /* Module declarations from 'numpy' */
 
 /* Module declarations from 'numpy' */
 static PyTypeObject *__pyx_ptype_5numpy_dtype = 0;
 static PyTypeObject *__pyx_ptype_5numpy_flatiter = 0;
 static PyTypeObject *__pyx_ptype_5numpy_broadcast = 0;
 static PyTypeObject *__pyx_ptype_5numpy_ndarray = 0;
+static PyTypeObject *__pyx_ptype_5numpy_generic = 0;
+static PyTypeObject *__pyx_ptype_5numpy_number = 0;
+static PyTypeObject *__pyx_ptype_5numpy_integer = 0;
+static PyTypeObject *__pyx_ptype_5numpy_signedinteger = 0;
+static PyTypeObject *__pyx_ptype_5numpy_unsignedinteger = 0;
+static PyTypeObject *__pyx_ptype_5numpy_inexact = 0;
+static PyTypeObject *__pyx_ptype_5numpy_floating = 0;
+static PyTypeObject *__pyx_ptype_5numpy_complexfloating = 0;
+static PyTypeObject *__pyx_ptype_5numpy_flexible = 0;
+static PyTypeObject *__pyx_ptype_5numpy_character = 0;
 static PyTypeObject *__pyx_ptype_5numpy_ufunc = 0;
-static CYTHON_INLINE char *__pyx_f_5numpy__util_dtypestring(PyArray_Descr *, char *, char *, int *); /*proto*/
 
 /* Module declarations from 'openTSNE.quad_tree' */
 static PyTypeObject *__pyx_ptype_8openTSNE_9quad_tree_QuadTree = 0;
 static int (*__pyx_f_8openTSNE_9quad_tree_is_close)(__pyx_t_8openTSNE_9quad_tree_Node *, double *, double); /*proto*/
 
 /* Module declarations from 'libc.stdlib' */
 
@@ -2724,17 +2744,16 @@
 extern int __pyx_module_is_main_openTSNE___tsne;
 int __pyx_module_is_main_openTSNE___tsne = 0;
 
 /* Implementation of 'openTSNE._tsne' */
 static PyObject *__pyx_builtin_range;
 static PyObject *__pyx_builtin_TypeError;
 static PyObject *__pyx_builtin_MemoryError;
-static PyObject *__pyx_builtin_ValueError;
-static PyObject *__pyx_builtin_RuntimeError;
 static PyObject *__pyx_builtin_ImportError;
+static PyObject *__pyx_builtin_ValueError;
 static PyObject *__pyx_builtin_enumerate;
 static PyObject *__pyx_builtin_Ellipsis;
 static PyObject *__pyx_builtin_id;
 static PyObject *__pyx_builtin_IndexError;
 static const char __pyx_k_[] = "()";
 static const char __pyx_k_C[] = "C";
 static const char __pyx_k_O[] = "O";
@@ -2819,15 +2838,14 @@
 static const char __pyx_k_pyx_vtable[] = "__pyx_vtable__";
 static const char __pyx_k_signatures[] = "signatures";
 static const char __pyx_k_zeros_like[] = "zeros_like";
 static const char __pyx_k_ImportError[] = "ImportError";
 static const char __pyx_k_MemoryError[] = "MemoryError";
 static const char __pyx_k_PickleError[] = "PickleError";
 static const char __pyx_k_num_threads[] = "num_threads";
-static const char __pyx_k_RuntimeError[] = "RuntimeError";
 static const char __pyx_k_pyx_checksum[] = "__pyx_checksum";
 static const char __pyx_k_stringsource[] = "stringsource";
 static const char __pyx_k_pyx_getbuffer[] = "__pyx_getbuffer";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
 static const char __pyx_k_openTSNE__tsne[] = "openTSNE._tsne";
 static const char __pyx_k_perplexity_tol[] = "perplexity_tol";
 static const char __pyx_k_y_tilde_values[] = "y_tilde_values";
@@ -2855,72 +2873,62 @@
 static const char __pyx_k_pairwise_normalization[] = "pairwise_normalization";
 static const char __pyx_k_MemoryView_of_r_at_0x_x[] = "<MemoryView of %r at 0x%x>";
 static const char __pyx_k_contiguous_and_indirect[] = "<contiguous and indirect>";
 static const char __pyx_k_Cannot_index_with_type_s[] = "Cannot index with type '%s'";
 static const char __pyx_k_Invalid_shape_in_axis_d_d[] = "Invalid shape in axis %d: %d.";
 static const char __pyx_k_No_matching_signature_found[] = "No matching signature found";
 static const char __pyx_k_itemsize_0_for_cython_array[] = "itemsize <= 0 for cython.array";
-static const char __pyx_k_ndarray_is_not_C_contiguous[] = "ndarray is not C contiguous";
 static const char __pyx_k_estimate_positive_gradient_nn[] = "estimate_positive_gradient_nn";
 static const char __pyx_k_unable_to_allocate_array_data[] = "unable to allocate array data.";
 static const char __pyx_k_pyx_fuse_0estimate_positive_gr[] = "__pyx_fuse_0estimate_positive_gradient_nn";
 static const char __pyx_k_pyx_fuse_1estimate_positive_gr[] = "__pyx_fuse_1estimate_positive_gradient_nn";
 static const char __pyx_k_strided_and_direct_or_indirect[] = "<strided and direct or indirect>";
 static const char __pyx_k_numpy_core_multiarray_failed_to[] = "numpy.core.multiarray failed to import";
-static const char __pyx_k_unknown_dtype_code_in_numpy_pxd[] = "unknown dtype code in numpy.pxd (%d)";
 static const char __pyx_k_Buffer_view_does_not_expose_stri[] = "Buffer view does not expose strides";
 static const char __pyx_k_Can_only_create_a_buffer_that_is[] = "Can only create a buffer that is contiguous in memory.";
 static const char __pyx_k_Cannot_assign_to_read_only_memor[] = "Cannot assign to read-only memoryview";
 static const char __pyx_k_Cannot_create_writable_memory_vi[] = "Cannot create writable memory view from read-only memoryview";
 static const char __pyx_k_Empty_shape_tuple_for_cython_arr[] = "Empty shape tuple for cython.array";
 static const char __pyx_k_Expected_at_least_d_argument_s_g[] = "Expected at least %d argument%s, got %d";
-static const char __pyx_k_Format_string_allocated_too_shor[] = "Format string allocated too short, see comment in numpy.pxd";
 static const char __pyx_k_Function_call_with_ambiguous_arg[] = "Function call with ambiguous argument types";
 static const char __pyx_k_Incompatible_checksums_0x_x_vs_0[] = "Incompatible checksums (0x%x vs (0xb068931, 0x82a3537, 0x6ae9995) = (name))";
 static const char __pyx_k_Indirect_dimensions_not_supporte[] = "Indirect dimensions not supported";
 static const char __pyx_k_Invalid_mode_expected_c_or_fortr[] = "Invalid mode, expected 'c' or 'fortran', got %s";
-static const char __pyx_k_Non_native_byte_order_not_suppor[] = "Non-native byte order not supported";
 static const char __pyx_k_Out_of_bounds_on_buffer_access_a[] = "Out of bounds on buffer access (axis %d)";
 static const char __pyx_k_Unable_to_convert_item_to_object[] = "Unable to convert item to object";
 static const char __pyx_k_got_differing_extents_in_dimensi[] = "got differing extents in dimension %d (got %d and %d)";
-static const char __pyx_k_ndarray_is_not_Fortran_contiguou[] = "ndarray is not Fortran contiguous";
 static const char __pyx_k_no_default___reduce___due_to_non[] = "no default __reduce__ due to non-trivial __cinit__";
 static const char __pyx_k_numpy_core_umath_failed_to_impor[] = "numpy.core.umath failed to import";
 static const char __pyx_k_unable_to_allocate_shape_and_str[] = "unable to allocate shape and strides.";
-static const char __pyx_k_Format_string_allocated_too_shor_2[] = "Format string allocated too short.";
 static PyObject *__pyx_kp_s_;
 static PyObject *__pyx_n_s_ASCII;
 static PyObject *__pyx_kp_s_Buffer_view_does_not_expose_stri;
 static PyObject *__pyx_n_u_C;
 static PyObject *__pyx_kp_s_Can_only_create_a_buffer_that_is;
 static PyObject *__pyx_kp_s_Cannot_assign_to_read_only_memor;
 static PyObject *__pyx_kp_s_Cannot_create_writable_memory_vi;
 static PyObject *__pyx_kp_s_Cannot_index_with_type_s;
 static PyObject *__pyx_n_s_Ellipsis;
 static PyObject *__pyx_kp_s_Empty_shape_tuple_for_cython_arr;
 static PyObject *__pyx_kp_s_Expected_at_least_d_argument_s_g;
-static PyObject *__pyx_kp_u_Format_string_allocated_too_shor;
-static PyObject *__pyx_kp_u_Format_string_allocated_too_shor_2;
 static PyObject *__pyx_kp_s_Function_call_with_ambiguous_arg;
 static PyObject *__pyx_n_s_ImportError;
 static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0;
 static PyObject *__pyx_n_s_IndexError;
 static PyObject *__pyx_kp_s_Indirect_dimensions_not_supporte;
 static PyObject *__pyx_kp_s_Invalid_mode_expected_c_or_fortr;
 static PyObject *__pyx_kp_s_Invalid_shape_in_axis_d_d;
 static PyObject *__pyx_n_s_MemoryError;
 static PyObject *__pyx_kp_s_MemoryView_of_r_at_0x_x;
 static PyObject *__pyx_kp_s_MemoryView_of_r_object;
 static PyObject *__pyx_kp_s_No_matching_signature_found;
-static PyObject *__pyx_kp_u_Non_native_byte_order_not_suppor;
 static PyObject *__pyx_n_b_O;
 static PyObject *__pyx_kp_s_Out_of_bounds_on_buffer_access_a;
 static PyObject *__pyx_n_s_P_data;
 static PyObject *__pyx_n_s_PickleError;
-static PyObject *__pyx_n_s_RuntimeError;
 static PyObject *__pyx_n_s_TypeError;
 static PyObject *__pyx_kp_s_Unable_to_convert_item_to_object;
 static PyObject *__pyx_n_s_ValueError;
 static PyObject *__pyx_n_s_View_MemoryView;
 static PyObject *__pyx_kp_s__2;
 static PyObject *__pyx_n_s_allocate_buffer;
 static PyObject *__pyx_n_s_args;
@@ -2974,16 +2982,14 @@
 static PyObject *__pyx_n_s_max_iter;
 static PyObject *__pyx_n_s_memview;
 static PyObject *__pyx_n_s_min_num_intervals;
 static PyObject *__pyx_n_s_mode;
 static PyObject *__pyx_n_s_n_interpolation_points;
 static PyObject *__pyx_n_s_name;
 static PyObject *__pyx_n_s_name_2;
-static PyObject *__pyx_kp_u_ndarray_is_not_C_contiguous;
-static PyObject *__pyx_kp_u_ndarray_is_not_Fortran_contiguou;
 static PyObject *__pyx_n_s_ndim;
 static PyObject *__pyx_n_s_new;
 static PyObject *__pyx_kp_s_no_default___reduce___due_to_non;
 static PyObject *__pyx_n_s_np;
 static PyObject *__pyx_n_s_num_threads;
 static PyObject *__pyx_n_s_numpy;
 static PyObject *__pyx_kp_u_numpy_core_multiarray_failed_to;
@@ -3031,15 +3037,14 @@
 static PyObject *__pyx_n_s_strip;
 static PyObject *__pyx_n_s_struct;
 static PyObject *__pyx_n_s_test;
 static PyObject *__pyx_n_s_theta;
 static PyObject *__pyx_n_s_tree;
 static PyObject *__pyx_kp_s_unable_to_allocate_array_data;
 static PyObject *__pyx_kp_s_unable_to_allocate_shape_and_str;
-static PyObject *__pyx_kp_u_unknown_dtype_code_in_numpy_pxd;
 static PyObject *__pyx_n_s_unpack;
 static PyObject *__pyx_n_s_update;
 static PyObject *__pyx_n_s_y_tilde_values;
 static PyObject *__pyx_n_s_zeros;
 static PyObject *__pyx_n_s_zeros_like;
 static PyObject *__pyx_pf_8openTSNE_5_tsne_compute_gaussian_perplexity(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_distances, __Pyx_memviewslice __pyx_v_desired_perplexities, double __pyx_v_perplexity_tol, Py_ssize_t __pyx_v_max_iter, Py_ssize_t __pyx_v_num_threads); /* proto */
 static PyObject *__pyx_pf_8openTSNE_5_tsne_2estimate_positive_gradient_nn(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_signatures, PyObject *__pyx_v_args, PyObject *__pyx_v_kwargs, CYTHON_UNUSED PyObject *__pyx_v_defaults); /* proto */
@@ -3048,16 +3053,14 @@
 static PyObject *__pyx_pf_8openTSNE_5_tsne_4estimate_negative_gradient_bh(CYTHON_UNUSED PyObject *__pyx_self, struct __pyx_obj_8openTSNE_9quad_tree_QuadTree *__pyx_v_tree, __Pyx_memviewslice __pyx_v_embedding, __Pyx_memviewslice __pyx_v_gradient, double __pyx_v_theta, double __pyx_v_dof, Py_ssize_t __pyx_v_num_threads, int __pyx_v_pairwise_normalization); /* proto */
 static PyObject *__pyx_pf_8openTSNE_5_tsne_6estimate_negative_gradient_fft_1d(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_embedding, __Pyx_memviewslice __pyx_v_gradient, Py_ssize_t __pyx_v_n_interpolation_points, Py_ssize_t __pyx_v_min_num_intervals, double __pyx_v_ints_in_interval, double __pyx_v_dof); /* proto */
 static PyObject *__pyx_pf_8openTSNE_5_tsne_8prepare_negative_gradient_fft_interpolation_grid_1d(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_reference_embedding, Py_ssize_t __pyx_v_n_interpolation_points, Py_ssize_t __pyx_v_min_num_intervals, double __pyx_v_ints_in_interval, double __pyx_v_dof, double __pyx_v_padding); /* proto */
 static PyObject *__pyx_pf_8openTSNE_5_tsne_10estimate_negative_gradient_fft_1d_with_grid(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_embedding, __Pyx_memviewslice __pyx_v_gradient, __Pyx_memviewslice __pyx_v_y_tilde_values, __Pyx_memviewslice __pyx_v_box_lower_bounds, Py_ssize_t __pyx_v_n_interpolation_points, double __pyx_v_dof); /* proto */
 static PyObject *__pyx_pf_8openTSNE_5_tsne_12estimate_negative_gradient_fft_2d(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_embedding, __Pyx_memviewslice __pyx_v_gradient, Py_ssize_t __pyx_v_n_interpolation_points, Py_ssize_t __pyx_v_min_num_intervals, double __pyx_v_ints_in_interval, double __pyx_v_dof); /* proto */
 static PyObject *__pyx_pf_8openTSNE_5_tsne_14prepare_negative_gradient_fft_interpolation_grid_2d(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_reference_embedding, Py_ssize_t __pyx_v_n_interpolation_points, Py_ssize_t __pyx_v_min_num_intervals, double __pyx_v_ints_in_interval, double __pyx_v_dof, double __pyx_v_padding); /* proto */
 static PyObject *__pyx_pf_8openTSNE_5_tsne_16estimate_negative_gradient_fft_2d_with_grid(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_embedding, __Pyx_memviewslice __pyx_v_gradient, __Pyx_memviewslice __pyx_v_y_tilde_values, __Pyx_memviewslice __pyx_v_box_x_lower_bounds, __Pyx_memviewslice __pyx_v_box_y_lower_bounds, Py_ssize_t __pyx_v_n_interpolation_points, double __pyx_v_dof); /* proto */
-static int __pyx_pf_5numpy_7ndarray___getbuffer__(PyArrayObject *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags); /* proto */
-static void __pyx_pf_5numpy_7ndarray_2__releasebuffer__(PyArrayObject *__pyx_v_self, Py_buffer *__pyx_v_info); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array___cinit__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_shape, Py_ssize_t __pyx_v_itemsize, PyObject *__pyx_v_format, PyObject *__pyx_v_mode, int __pyx_v_allocate_buffer); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array_2__getbuffer__(struct __pyx_array_obj *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags); /* proto */
 static void __pyx_array___pyx_pf_15View_dot_MemoryView_5array_4__dealloc__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_15View_dot_MemoryView_5array_7memview___get__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static Py_ssize_t __pyx_array___pyx_pf_15View_dot_MemoryView_5array_6__len__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_array___pyx_pf_15View_dot_MemoryView_5array_8__getattr__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_attr); /* proto */
 static PyObject *__pyx_array___pyx_pf_15View_dot_MemoryView_5array_10__getitem__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_item); /* proto */
@@ -3317,15 +3320,15 @@
 static Py_ssize_t __pyx_k__6;
 static int __pyx_k__7;
 static double __pyx_k__8;
 static Py_ssize_t __pyx_k__9;
 static int __pyx_k__10;
 static PyObject *__pyx_tuple__3;
 static PyObject *__pyx_tuple__4;
-static PyObject *__pyx_slice__32;
+static PyObject *__pyx_slice__27;
 static PyObject *__pyx_tuple__11;
 static PyObject *__pyx_tuple__12;
 static PyObject *__pyx_tuple__13;
 static PyObject *__pyx_tuple__14;
 static PyObject *__pyx_tuple__15;
 static PyObject *__pyx_tuple__16;
 static PyObject *__pyx_tuple__17;
@@ -3334,32 +3337,27 @@
 static PyObject *__pyx_tuple__20;
 static PyObject *__pyx_tuple__21;
 static PyObject *__pyx_tuple__22;
 static PyObject *__pyx_tuple__23;
 static PyObject *__pyx_tuple__24;
 static PyObject *__pyx_tuple__25;
 static PyObject *__pyx_tuple__26;
-static PyObject *__pyx_tuple__27;
 static PyObject *__pyx_tuple__28;
 static PyObject *__pyx_tuple__29;
 static PyObject *__pyx_tuple__30;
 static PyObject *__pyx_tuple__31;
-static PyObject *__pyx_tuple__33;
+static PyObject *__pyx_tuple__32;
 static PyObject *__pyx_tuple__34;
 static PyObject *__pyx_tuple__35;
 static PyObject *__pyx_tuple__36;
 static PyObject *__pyx_tuple__37;
+static PyObject *__pyx_tuple__38;
 static PyObject *__pyx_tuple__39;
-static PyObject *__pyx_tuple__40;
-static PyObject *__pyx_tuple__41;
-static PyObject *__pyx_tuple__42;
-static PyObject *__pyx_tuple__43;
-static PyObject *__pyx_tuple__44;
-static PyObject *__pyx_codeobj__38;
-static PyObject *__pyx_codeobj__45;
+static PyObject *__pyx_codeobj__33;
+static PyObject *__pyx_codeobj__40;
 /* Late includes */
 
 /* "openTSNE/_tsne.pyx":30
  * 
  * 
  * cpdef double[:, ::1] compute_gaussian_perplexity(             # <<<<<<<<<<<<<<
  *     double[:, :] distances,
@@ -18769,874 +18767,15 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_box_x_lower_bounds, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_box_y_lower_bounds, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":258
- *         # experimental exception made for __getbuffer__ and __releasebuffer__
- *         # -- the details of this may change.
- *         def __getbuffer__(ndarray self, Py_buffer* info, int flags):             # <<<<<<<<<<<<<<
- *             # This implementation of getbuffer is geared towards Cython
- *             # requirements, and does not yet fulfill the PEP.
- */
-
-/* Python wrapper */
-static CYTHON_UNUSED int __pyx_pw_5numpy_7ndarray_1__getbuffer__(PyObject *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags); /*proto*/
-static CYTHON_UNUSED int __pyx_pw_5numpy_7ndarray_1__getbuffer__(PyObject *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__getbuffer__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_5numpy_7ndarray___getbuffer__(((PyArrayObject *)__pyx_v_self), ((Py_buffer *)__pyx_v_info), ((int)__pyx_v_flags));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static int __pyx_pf_5numpy_7ndarray___getbuffer__(PyArrayObject *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags) {
-  int __pyx_v_i;
-  int __pyx_v_ndim;
-  int __pyx_v_endian_detector;
-  int __pyx_v_little_endian;
-  int __pyx_v_t;
-  char *__pyx_v_f;
-  PyArray_Descr *__pyx_v_descr = 0;
-  int __pyx_v_offset;
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  int __pyx_t_2;
-  PyObject *__pyx_t_3 = NULL;
-  int __pyx_t_4;
-  int __pyx_t_5;
-  int __pyx_t_6;
-  PyArray_Descr *__pyx_t_7;
-  PyObject *__pyx_t_8 = NULL;
-  char *__pyx_t_9;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  if (__pyx_v_info == NULL) {
-    PyErr_SetString(PyExc_BufferError, "PyObject_GetBuffer: view==NULL argument is obsolete");
-    return -1;
-  }
-  __Pyx_RefNannySetupContext("__getbuffer__", 0);
-  __pyx_v_info->obj = Py_None; __Pyx_INCREF(Py_None);
-  __Pyx_GIVEREF(__pyx_v_info->obj);
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":265
- * 
- *             cdef int i, ndim
- *             cdef int endian_detector = 1             # <<<<<<<<<<<<<<
- *             cdef bint little_endian = ((<char*>&endian_detector)[0] != 0)
- * 
- */
-  __pyx_v_endian_detector = 1;
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":266
- *             cdef int i, ndim
- *             cdef int endian_detector = 1
- *             cdef bint little_endian = ((<char*>&endian_detector)[0] != 0)             # <<<<<<<<<<<<<<
- * 
- *             ndim = PyArray_NDIM(self)
- */
-  __pyx_v_little_endian = ((((char *)(&__pyx_v_endian_detector))[0]) != 0);
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":268
- *             cdef bint little_endian = ((<char*>&endian_detector)[0] != 0)
- * 
- *             ndim = PyArray_NDIM(self)             # <<<<<<<<<<<<<<
- * 
- *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)
- */
-  __pyx_v_ndim = PyArray_NDIM(__pyx_v_self);
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":270
- *             ndim = PyArray_NDIM(self)
- * 
- *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)             # <<<<<<<<<<<<<<
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_C_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not C contiguous")
- */
-  __pyx_t_2 = (((__pyx_v_flags & PyBUF_C_CONTIGUOUS) == PyBUF_C_CONTIGUOUS) != 0);
-  if (__pyx_t_2) {
-  } else {
-    __pyx_t_1 = __pyx_t_2;
-    goto __pyx_L4_bool_binop_done;
-  }
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":271
- * 
- *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_C_CONTIGUOUS)):             # <<<<<<<<<<<<<<
- *                 raise ValueError(u"ndarray is not C contiguous")
- * 
- */
-  __pyx_t_2 = ((!(PyArray_CHKFLAGS(__pyx_v_self, NPY_ARRAY_C_CONTIGUOUS) != 0)) != 0);
-  __pyx_t_1 = __pyx_t_2;
-  __pyx_L4_bool_binop_done:;
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":270
- *             ndim = PyArray_NDIM(self)
- * 
- *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)             # <<<<<<<<<<<<<<
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_C_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not C contiguous")
- */
-  if (unlikely(__pyx_t_1)) {
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":272
- *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_C_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not C contiguous")             # <<<<<<<<<<<<<<
- * 
- *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)
- */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 272, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(1, 272, __pyx_L1_error)
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":270
- *             ndim = PyArray_NDIM(self)
- * 
- *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)             # <<<<<<<<<<<<<<
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_C_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not C contiguous")
- */
-  }
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":274
- *                 raise ValueError(u"ndarray is not C contiguous")
- * 
- *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)             # <<<<<<<<<<<<<<
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_F_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not Fortran contiguous")
- */
-  __pyx_t_2 = (((__pyx_v_flags & PyBUF_F_CONTIGUOUS) == PyBUF_F_CONTIGUOUS) != 0);
-  if (__pyx_t_2) {
-  } else {
-    __pyx_t_1 = __pyx_t_2;
-    goto __pyx_L7_bool_binop_done;
-  }
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":275
- * 
- *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_F_CONTIGUOUS)):             # <<<<<<<<<<<<<<
- *                 raise ValueError(u"ndarray is not Fortran contiguous")
- * 
- */
-  __pyx_t_2 = ((!(PyArray_CHKFLAGS(__pyx_v_self, NPY_ARRAY_F_CONTIGUOUS) != 0)) != 0);
-  __pyx_t_1 = __pyx_t_2;
-  __pyx_L7_bool_binop_done:;
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":274
- *                 raise ValueError(u"ndarray is not C contiguous")
- * 
- *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)             # <<<<<<<<<<<<<<
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_F_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not Fortran contiguous")
- */
-  if (unlikely(__pyx_t_1)) {
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":276
- *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_F_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not Fortran contiguous")             # <<<<<<<<<<<<<<
- * 
- *             info.buf = PyArray_DATA(self)
- */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 276, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(1, 276, __pyx_L1_error)
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":274
- *                 raise ValueError(u"ndarray is not C contiguous")
- * 
- *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)             # <<<<<<<<<<<<<<
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_F_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not Fortran contiguous")
- */
-  }
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":278
- *                 raise ValueError(u"ndarray is not Fortran contiguous")
- * 
- *             info.buf = PyArray_DATA(self)             # <<<<<<<<<<<<<<
- *             info.ndim = ndim
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
- */
-  __pyx_v_info->buf = PyArray_DATA(__pyx_v_self);
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":279
- * 
- *             info.buf = PyArray_DATA(self)
- *             info.ndim = ndim             # <<<<<<<<<<<<<<
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
- *                 # Allocate new buffer for strides and shape info.
- */
-  __pyx_v_info->ndim = __pyx_v_ndim;
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":280
- *             info.buf = PyArray_DATA(self)
- *             info.ndim = ndim
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):             # <<<<<<<<<<<<<<
- *                 # Allocate new buffer for strides and shape info.
- *                 # This is allocated as one block, strides first.
- */
-  __pyx_t_1 = (((sizeof(npy_intp)) != (sizeof(Py_ssize_t))) != 0);
-  if (__pyx_t_1) {
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":283
- *                 # Allocate new buffer for strides and shape info.
- *                 # This is allocated as one block, strides first.
- *                 info.strides = <Py_ssize_t*>PyObject_Malloc(sizeof(Py_ssize_t) * 2 * <size_t>ndim)             # <<<<<<<<<<<<<<
- *                 info.shape = info.strides + ndim
- *                 for i in range(ndim):
- */
-    __pyx_v_info->strides = ((Py_ssize_t *)PyObject_Malloc((((sizeof(Py_ssize_t)) * 2) * ((size_t)__pyx_v_ndim))));
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":284
- *                 # This is allocated as one block, strides first.
- *                 info.strides = <Py_ssize_t*>PyObject_Malloc(sizeof(Py_ssize_t) * 2 * <size_t>ndim)
- *                 info.shape = info.strides + ndim             # <<<<<<<<<<<<<<
- *                 for i in range(ndim):
- *                     info.strides[i] = PyArray_STRIDES(self)[i]
- */
-    __pyx_v_info->shape = (__pyx_v_info->strides + __pyx_v_ndim);
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":285
- *                 info.strides = <Py_ssize_t*>PyObject_Malloc(sizeof(Py_ssize_t) * 2 * <size_t>ndim)
- *                 info.shape = info.strides + ndim
- *                 for i in range(ndim):             # <<<<<<<<<<<<<<
- *                     info.strides[i] = PyArray_STRIDES(self)[i]
- *                     info.shape[i] = PyArray_DIMS(self)[i]
- */
-    __pyx_t_4 = __pyx_v_ndim;
-    __pyx_t_5 = __pyx_t_4;
-    for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
-      __pyx_v_i = __pyx_t_6;
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":286
- *                 info.shape = info.strides + ndim
- *                 for i in range(ndim):
- *                     info.strides[i] = PyArray_STRIDES(self)[i]             # <<<<<<<<<<<<<<
- *                     info.shape[i] = PyArray_DIMS(self)[i]
- *             else:
- */
-      (__pyx_v_info->strides[__pyx_v_i]) = (PyArray_STRIDES(__pyx_v_self)[__pyx_v_i]);
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":287
- *                 for i in range(ndim):
- *                     info.strides[i] = PyArray_STRIDES(self)[i]
- *                     info.shape[i] = PyArray_DIMS(self)[i]             # <<<<<<<<<<<<<<
- *             else:
- *                 info.strides = <Py_ssize_t*>PyArray_STRIDES(self)
- */
-      (__pyx_v_info->shape[__pyx_v_i]) = (PyArray_DIMS(__pyx_v_self)[__pyx_v_i]);
-    }
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":280
- *             info.buf = PyArray_DATA(self)
- *             info.ndim = ndim
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):             # <<<<<<<<<<<<<<
- *                 # Allocate new buffer for strides and shape info.
- *                 # This is allocated as one block, strides first.
- */
-    goto __pyx_L9;
-  }
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":289
- *                     info.shape[i] = PyArray_DIMS(self)[i]
- *             else:
- *                 info.strides = <Py_ssize_t*>PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
- *                 info.shape = <Py_ssize_t*>PyArray_DIMS(self)
- *             info.suboffsets = NULL
- */
-  /*else*/ {
-    __pyx_v_info->strides = ((Py_ssize_t *)PyArray_STRIDES(__pyx_v_self));
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":290
- *             else:
- *                 info.strides = <Py_ssize_t*>PyArray_STRIDES(self)
- *                 info.shape = <Py_ssize_t*>PyArray_DIMS(self)             # <<<<<<<<<<<<<<
- *             info.suboffsets = NULL
- *             info.itemsize = PyArray_ITEMSIZE(self)
- */
-    __pyx_v_info->shape = ((Py_ssize_t *)PyArray_DIMS(__pyx_v_self));
-  }
-  __pyx_L9:;
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":291
- *                 info.strides = <Py_ssize_t*>PyArray_STRIDES(self)
- *                 info.shape = <Py_ssize_t*>PyArray_DIMS(self)
- *             info.suboffsets = NULL             # <<<<<<<<<<<<<<
- *             info.itemsize = PyArray_ITEMSIZE(self)
- *             info.readonly = not PyArray_ISWRITEABLE(self)
- */
-  __pyx_v_info->suboffsets = NULL;
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":292
- *                 info.shape = <Py_ssize_t*>PyArray_DIMS(self)
- *             info.suboffsets = NULL
- *             info.itemsize = PyArray_ITEMSIZE(self)             # <<<<<<<<<<<<<<
- *             info.readonly = not PyArray_ISWRITEABLE(self)
- * 
- */
-  __pyx_v_info->itemsize = PyArray_ITEMSIZE(__pyx_v_self);
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":293
- *             info.suboffsets = NULL
- *             info.itemsize = PyArray_ITEMSIZE(self)
- *             info.readonly = not PyArray_ISWRITEABLE(self)             # <<<<<<<<<<<<<<
- * 
- *             cdef int t
- */
-  __pyx_v_info->readonly = (!(PyArray_ISWRITEABLE(__pyx_v_self) != 0));
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":296
- * 
- *             cdef int t
- *             cdef char* f = NULL             # <<<<<<<<<<<<<<
- *             cdef dtype descr = <dtype>PyArray_DESCR(self)
- *             cdef int offset
- */
-  __pyx_v_f = NULL;
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":297
- *             cdef int t
- *             cdef char* f = NULL
- *             cdef dtype descr = <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
- *             cdef int offset
- * 
- */
-  __pyx_t_7 = PyArray_DESCR(__pyx_v_self);
-  __pyx_t_3 = ((PyObject *)__pyx_t_7);
-  __Pyx_INCREF(__pyx_t_3);
-  __pyx_v_descr = ((PyArray_Descr *)__pyx_t_3);
-  __pyx_t_3 = 0;
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":300
- *             cdef int offset
- * 
- *             info.obj = self             # <<<<<<<<<<<<<<
- * 
- *             if not PyDataType_HASFIELDS(descr):
- */
-  __Pyx_INCREF(((PyObject *)__pyx_v_self));
-  __Pyx_GIVEREF(((PyObject *)__pyx_v_self));
-  __Pyx_GOTREF(__pyx_v_info->obj);
-  __Pyx_DECREF(__pyx_v_info->obj);
-  __pyx_v_info->obj = ((PyObject *)__pyx_v_self);
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":302
- *             info.obj = self
- * 
- *             if not PyDataType_HASFIELDS(descr):             # <<<<<<<<<<<<<<
- *                 t = descr.type_num
- *                 if ((descr.byteorder == c'>' and little_endian) or
- */
-  __pyx_t_1 = ((!(PyDataType_HASFIELDS(__pyx_v_descr) != 0)) != 0);
-  if (__pyx_t_1) {
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":303
- * 
- *             if not PyDataType_HASFIELDS(descr):
- *                 t = descr.type_num             # <<<<<<<<<<<<<<
- *                 if ((descr.byteorder == c'>' and little_endian) or
- *                     (descr.byteorder == c'<' and not little_endian)):
- */
-    __pyx_t_4 = __pyx_v_descr->type_num;
-    __pyx_v_t = __pyx_t_4;
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":304
- *             if not PyDataType_HASFIELDS(descr):
- *                 t = descr.type_num
- *                 if ((descr.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
- *                     (descr.byteorder == c'<' and not little_endian)):
- *                     raise ValueError(u"Non-native byte order not supported")
- */
-    __pyx_t_2 = ((__pyx_v_descr->byteorder == '>') != 0);
-    if (!__pyx_t_2) {
-      goto __pyx_L15_next_or;
-    } else {
-    }
-    __pyx_t_2 = (__pyx_v_little_endian != 0);
-    if (!__pyx_t_2) {
-    } else {
-      __pyx_t_1 = __pyx_t_2;
-      goto __pyx_L14_bool_binop_done;
-    }
-    __pyx_L15_next_or:;
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":305
- *                 t = descr.type_num
- *                 if ((descr.byteorder == c'>' and little_endian) or
- *                     (descr.byteorder == c'<' and not little_endian)):             # <<<<<<<<<<<<<<
- *                     raise ValueError(u"Non-native byte order not supported")
- *                 if   t == NPY_BYTE:        f = "b"
- */
-    __pyx_t_2 = ((__pyx_v_descr->byteorder == '<') != 0);
-    if (__pyx_t_2) {
-    } else {
-      __pyx_t_1 = __pyx_t_2;
-      goto __pyx_L14_bool_binop_done;
-    }
-    __pyx_t_2 = ((!(__pyx_v_little_endian != 0)) != 0);
-    __pyx_t_1 = __pyx_t_2;
-    __pyx_L14_bool_binop_done:;
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":304
- *             if not PyDataType_HASFIELDS(descr):
- *                 t = descr.type_num
- *                 if ((descr.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
- *                     (descr.byteorder == c'<' and not little_endian)):
- *                     raise ValueError(u"Non-native byte order not supported")
- */
-    if (unlikely(__pyx_t_1)) {
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":306
- *                 if ((descr.byteorder == c'>' and little_endian) or
- *                     (descr.byteorder == c'<' and not little_endian)):
- *                     raise ValueError(u"Non-native byte order not supported")             # <<<<<<<<<<<<<<
- *                 if   t == NPY_BYTE:        f = "b"
- *                 elif t == NPY_UBYTE:       f = "B"
- */
-      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 306, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __PYX_ERR(1, 306, __pyx_L1_error)
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":304
- *             if not PyDataType_HASFIELDS(descr):
- *                 t = descr.type_num
- *                 if ((descr.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
- *                     (descr.byteorder == c'<' and not little_endian)):
- *                     raise ValueError(u"Non-native byte order not supported")
- */
-    }
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":307
- *                     (descr.byteorder == c'<' and not little_endian)):
- *                     raise ValueError(u"Non-native byte order not supported")
- *                 if   t == NPY_BYTE:        f = "b"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_UBYTE:       f = "B"
- *                 elif t == NPY_SHORT:       f = "h"
- */
-    switch (__pyx_v_t) {
-      case NPY_BYTE:
-      __pyx_v_f = ((char *)"b");
-      break;
-      case NPY_UBYTE:
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":308
- *                     raise ValueError(u"Non-native byte order not supported")
- *                 if   t == NPY_BYTE:        f = "b"
- *                 elif t == NPY_UBYTE:       f = "B"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_SHORT:       f = "h"
- *                 elif t == NPY_USHORT:      f = "H"
- */
-      __pyx_v_f = ((char *)"B");
-      break;
-      case NPY_SHORT:
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":309
- *                 if   t == NPY_BYTE:        f = "b"
- *                 elif t == NPY_UBYTE:       f = "B"
- *                 elif t == NPY_SHORT:       f = "h"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_USHORT:      f = "H"
- *                 elif t == NPY_INT:         f = "i"
- */
-      __pyx_v_f = ((char *)"h");
-      break;
-      case NPY_USHORT:
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":310
- *                 elif t == NPY_UBYTE:       f = "B"
- *                 elif t == NPY_SHORT:       f = "h"
- *                 elif t == NPY_USHORT:      f = "H"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_INT:         f = "i"
- *                 elif t == NPY_UINT:        f = "I"
- */
-      __pyx_v_f = ((char *)"H");
-      break;
-      case NPY_INT:
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":311
- *                 elif t == NPY_SHORT:       f = "h"
- *                 elif t == NPY_USHORT:      f = "H"
- *                 elif t == NPY_INT:         f = "i"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_UINT:        f = "I"
- *                 elif t == NPY_LONG:        f = "l"
- */
-      __pyx_v_f = ((char *)"i");
-      break;
-      case NPY_UINT:
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":312
- *                 elif t == NPY_USHORT:      f = "H"
- *                 elif t == NPY_INT:         f = "i"
- *                 elif t == NPY_UINT:        f = "I"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_LONG:        f = "l"
- *                 elif t == NPY_ULONG:       f = "L"
- */
-      __pyx_v_f = ((char *)"I");
-      break;
-      case NPY_LONG:
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":313
- *                 elif t == NPY_INT:         f = "i"
- *                 elif t == NPY_UINT:        f = "I"
- *                 elif t == NPY_LONG:        f = "l"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_ULONG:       f = "L"
- *                 elif t == NPY_LONGLONG:    f = "q"
- */
-      __pyx_v_f = ((char *)"l");
-      break;
-      case NPY_ULONG:
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":314
- *                 elif t == NPY_UINT:        f = "I"
- *                 elif t == NPY_LONG:        f = "l"
- *                 elif t == NPY_ULONG:       f = "L"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_LONGLONG:    f = "q"
- *                 elif t == NPY_ULONGLONG:   f = "Q"
- */
-      __pyx_v_f = ((char *)"L");
-      break;
-      case NPY_LONGLONG:
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":315
- *                 elif t == NPY_LONG:        f = "l"
- *                 elif t == NPY_ULONG:       f = "L"
- *                 elif t == NPY_LONGLONG:    f = "q"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_ULONGLONG:   f = "Q"
- *                 elif t == NPY_FLOAT:       f = "f"
- */
-      __pyx_v_f = ((char *)"q");
-      break;
-      case NPY_ULONGLONG:
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":316
- *                 elif t == NPY_ULONG:       f = "L"
- *                 elif t == NPY_LONGLONG:    f = "q"
- *                 elif t == NPY_ULONGLONG:   f = "Q"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_FLOAT:       f = "f"
- *                 elif t == NPY_DOUBLE:      f = "d"
- */
-      __pyx_v_f = ((char *)"Q");
-      break;
-      case NPY_FLOAT:
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":317
- *                 elif t == NPY_LONGLONG:    f = "q"
- *                 elif t == NPY_ULONGLONG:   f = "Q"
- *                 elif t == NPY_FLOAT:       f = "f"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_DOUBLE:      f = "d"
- *                 elif t == NPY_LONGDOUBLE:  f = "g"
- */
-      __pyx_v_f = ((char *)"f");
-      break;
-      case NPY_DOUBLE:
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":318
- *                 elif t == NPY_ULONGLONG:   f = "Q"
- *                 elif t == NPY_FLOAT:       f = "f"
- *                 elif t == NPY_DOUBLE:      f = "d"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_LONGDOUBLE:  f = "g"
- *                 elif t == NPY_CFLOAT:      f = "Zf"
- */
-      __pyx_v_f = ((char *)"d");
-      break;
-      case NPY_LONGDOUBLE:
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":319
- *                 elif t == NPY_FLOAT:       f = "f"
- *                 elif t == NPY_DOUBLE:      f = "d"
- *                 elif t == NPY_LONGDOUBLE:  f = "g"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_CFLOAT:      f = "Zf"
- *                 elif t == NPY_CDOUBLE:     f = "Zd"
- */
-      __pyx_v_f = ((char *)"g");
-      break;
-      case NPY_CFLOAT:
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":320
- *                 elif t == NPY_DOUBLE:      f = "d"
- *                 elif t == NPY_LONGDOUBLE:  f = "g"
- *                 elif t == NPY_CFLOAT:      f = "Zf"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_CDOUBLE:     f = "Zd"
- *                 elif t == NPY_CLONGDOUBLE: f = "Zg"
- */
-      __pyx_v_f = ((char *)"Zf");
-      break;
-      case NPY_CDOUBLE:
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":321
- *                 elif t == NPY_LONGDOUBLE:  f = "g"
- *                 elif t == NPY_CFLOAT:      f = "Zf"
- *                 elif t == NPY_CDOUBLE:     f = "Zd"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_CLONGDOUBLE: f = "Zg"
- *                 elif t == NPY_OBJECT:      f = "O"
- */
-      __pyx_v_f = ((char *)"Zd");
-      break;
-      case NPY_CLONGDOUBLE:
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":322
- *                 elif t == NPY_CFLOAT:      f = "Zf"
- *                 elif t == NPY_CDOUBLE:     f = "Zd"
- *                 elif t == NPY_CLONGDOUBLE: f = "Zg"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_OBJECT:      f = "O"
- *                 else:
- */
-      __pyx_v_f = ((char *)"Zg");
-      break;
-      case NPY_OBJECT:
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":323
- *                 elif t == NPY_CDOUBLE:     f = "Zd"
- *                 elif t == NPY_CLONGDOUBLE: f = "Zg"
- *                 elif t == NPY_OBJECT:      f = "O"             # <<<<<<<<<<<<<<
- *                 else:
- *                     raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)
- */
-      __pyx_v_f = ((char *)"O");
-      break;
-      default:
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":325
- *                 elif t == NPY_OBJECT:      f = "O"
- *                 else:
- *                     raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)             # <<<<<<<<<<<<<<
- *                 info.format = f
- *                 return
- */
-      __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_t); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 325, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_8 = PyUnicode_Format(__pyx_kp_u_unknown_dtype_code_in_numpy_pxd, __pyx_t_3); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 325, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 325, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __PYX_ERR(1, 325, __pyx_L1_error)
-      break;
-    }
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":326
- *                 else:
- *                     raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)
- *                 info.format = f             # <<<<<<<<<<<<<<
- *                 return
- *             else:
- */
-    __pyx_v_info->format = __pyx_v_f;
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":327
- *                     raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)
- *                 info.format = f
- *                 return             # <<<<<<<<<<<<<<
- *             else:
- *                 info.format = <char*>PyObject_Malloc(_buffer_format_string_len)
- */
-    __pyx_r = 0;
-    goto __pyx_L0;
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":302
- *             info.obj = self
- * 
- *             if not PyDataType_HASFIELDS(descr):             # <<<<<<<<<<<<<<
- *                 t = descr.type_num
- *                 if ((descr.byteorder == c'>' and little_endian) or
- */
-  }
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":329
- *                 return
- *             else:
- *                 info.format = <char*>PyObject_Malloc(_buffer_format_string_len)             # <<<<<<<<<<<<<<
- *                 info.format[0] = c'^' # Native data types, manual alignment
- *                 offset = 0
- */
-  /*else*/ {
-    __pyx_v_info->format = ((char *)PyObject_Malloc(0xFF));
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":330
- *             else:
- *                 info.format = <char*>PyObject_Malloc(_buffer_format_string_len)
- *                 info.format[0] = c'^' # Native data types, manual alignment             # <<<<<<<<<<<<<<
- *                 offset = 0
- *                 f = _util_dtypestring(descr, info.format + 1,
- */
-    (__pyx_v_info->format[0]) = '^';
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":331
- *                 info.format = <char*>PyObject_Malloc(_buffer_format_string_len)
- *                 info.format[0] = c'^' # Native data types, manual alignment
- *                 offset = 0             # <<<<<<<<<<<<<<
- *                 f = _util_dtypestring(descr, info.format + 1,
- *                                       info.format + _buffer_format_string_len,
- */
-    __pyx_v_offset = 0;
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":332
- *                 info.format[0] = c'^' # Native data types, manual alignment
- *                 offset = 0
- *                 f = _util_dtypestring(descr, info.format + 1,             # <<<<<<<<<<<<<<
- *                                       info.format + _buffer_format_string_len,
- *                                       &offset)
- */
-    __pyx_t_9 = __pyx_f_5numpy__util_dtypestring(__pyx_v_descr, (__pyx_v_info->format + 1), (__pyx_v_info->format + 0xFF), (&__pyx_v_offset)); if (unlikely(__pyx_t_9 == ((char *)NULL))) __PYX_ERR(1, 332, __pyx_L1_error)
-    __pyx_v_f = __pyx_t_9;
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":335
- *                                       info.format + _buffer_format_string_len,
- *                                       &offset)
- *                 f[0] = c'\0' # Terminate format string             # <<<<<<<<<<<<<<
- * 
- *         def __releasebuffer__(ndarray self, Py_buffer* info):
- */
-    (__pyx_v_f[0]) = '\x00';
-  }
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":258
- *         # experimental exception made for __getbuffer__ and __releasebuffer__
- *         # -- the details of this may change.
- *         def __getbuffer__(ndarray self, Py_buffer* info, int flags):             # <<<<<<<<<<<<<<
- *             # This implementation of getbuffer is geared towards Cython
- *             # requirements, and does not yet fulfill the PEP.
- */
-
-  /* function exit code */
-  __pyx_r = 0;
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_8);
-  __Pyx_AddTraceback("numpy.ndarray.__getbuffer__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = -1;
-  if (__pyx_v_info->obj != NULL) {
-    __Pyx_GOTREF(__pyx_v_info->obj);
-    __Pyx_DECREF(__pyx_v_info->obj); __pyx_v_info->obj = 0;
-  }
-  goto __pyx_L2;
-  __pyx_L0:;
-  if (__pyx_v_info->obj == Py_None) {
-    __Pyx_GOTREF(__pyx_v_info->obj);
-    __Pyx_DECREF(__pyx_v_info->obj); __pyx_v_info->obj = 0;
-  }
-  __pyx_L2:;
-  __Pyx_XDECREF((PyObject *)__pyx_v_descr);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":337
- *                 f[0] = c'\0' # Terminate format string
- * 
- *         def __releasebuffer__(ndarray self, Py_buffer* info):             # <<<<<<<<<<<<<<
- *             if PyArray_HASFIELDS(self):
- *                 PyObject_Free(info.format)
- */
-
-/* Python wrapper */
-static CYTHON_UNUSED void __pyx_pw_5numpy_7ndarray_3__releasebuffer__(PyObject *__pyx_v_self, Py_buffer *__pyx_v_info); /*proto*/
-static CYTHON_UNUSED void __pyx_pw_5numpy_7ndarray_3__releasebuffer__(PyObject *__pyx_v_self, Py_buffer *__pyx_v_info) {
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__releasebuffer__ (wrapper)", 0);
-  __pyx_pf_5numpy_7ndarray_2__releasebuffer__(((PyArrayObject *)__pyx_v_self), ((Py_buffer *)__pyx_v_info));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-}
-
-static void __pyx_pf_5numpy_7ndarray_2__releasebuffer__(PyArrayObject *__pyx_v_self, Py_buffer *__pyx_v_info) {
-  __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  __Pyx_RefNannySetupContext("__releasebuffer__", 0);
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":338
- * 
- *         def __releasebuffer__(ndarray self, Py_buffer* info):
- *             if PyArray_HASFIELDS(self):             # <<<<<<<<<<<<<<
- *                 PyObject_Free(info.format)
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
- */
-  __pyx_t_1 = (PyArray_HASFIELDS(__pyx_v_self) != 0);
-  if (__pyx_t_1) {
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":339
- *         def __releasebuffer__(ndarray self, Py_buffer* info):
- *             if PyArray_HASFIELDS(self):
- *                 PyObject_Free(info.format)             # <<<<<<<<<<<<<<
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
- *                 PyObject_Free(info.strides)
- */
-    PyObject_Free(__pyx_v_info->format);
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":338
- * 
- *         def __releasebuffer__(ndarray self, Py_buffer* info):
- *             if PyArray_HASFIELDS(self):             # <<<<<<<<<<<<<<
- *                 PyObject_Free(info.format)
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
- */
-  }
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":340
- *             if PyArray_HASFIELDS(self):
- *                 PyObject_Free(info.format)
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):             # <<<<<<<<<<<<<<
- *                 PyObject_Free(info.strides)
- *                 # info.shape was stored after info.strides in the same block
- */
-  __pyx_t_1 = (((sizeof(npy_intp)) != (sizeof(Py_ssize_t))) != 0);
-  if (__pyx_t_1) {
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":341
- *                 PyObject_Free(info.format)
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
- *                 PyObject_Free(info.strides)             # <<<<<<<<<<<<<<
- *                 # info.shape was stored after info.strides in the same block
- * 
- */
-    PyObject_Free(__pyx_v_info->strides);
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":340
- *             if PyArray_HASFIELDS(self):
- *                 PyObject_Free(info.format)
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):             # <<<<<<<<<<<<<<
- *                 PyObject_Free(info.strides)
- *                 # info.shape was stored after info.strides in the same block
- */
-  }
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":337
- *                 f[0] = c'\0' # Terminate format string
- * 
- *         def __releasebuffer__(ndarray self, Py_buffer* info):             # <<<<<<<<<<<<<<
- *             if PyArray_HASFIELDS(self):
- *                 PyObject_Free(info.format)
- */
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-}
-
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":820
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -19645,29 +18784,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":821
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":736
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 821, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 736, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":820
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -19678,15 +18817,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":823
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -19695,29 +18834,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":824
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":739
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 824, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 739, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":823
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -19728,15 +18867,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":826
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -19745,29 +18884,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":827
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":742
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 827, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 742, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":826
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -19778,15 +18917,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":829
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -19795,29 +18934,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":830
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":745
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 830, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 745, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":829
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -19828,15 +18967,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":832
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -19845,29 +18984,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":833
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":748
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 833, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 748, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":832
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -19878,966 +19017,217 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":835
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":836
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":837
+    /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":752
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":836
+    /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":839
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":754
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
- * cdef inline char* _util_dtypestring(dtype descr, char* f, char* end, int* offset) except NULL:
+ * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":835
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":841
- *         return ()
- * 
- * cdef inline char* _util_dtypestring(dtype descr, char* f, char* end, int* offset) except NULL:             # <<<<<<<<<<<<<<
- *     # Recursive utility function used in __getbuffer__ to get format
- *     # string. The new location in the format string is returned.
- */
-
-static CYTHON_INLINE char *__pyx_f_5numpy__util_dtypestring(PyArray_Descr *__pyx_v_descr, char *__pyx_v_f, char *__pyx_v_end, int *__pyx_v_offset) {
-  PyArray_Descr *__pyx_v_child = 0;
-  int __pyx_v_endian_detector;
-  int __pyx_v_little_endian;
-  PyObject *__pyx_v_fields = 0;
-  PyObject *__pyx_v_childname = NULL;
-  PyObject *__pyx_v_new_offset = NULL;
-  PyObject *__pyx_v_t = NULL;
-  char *__pyx_r;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  Py_ssize_t __pyx_t_2;
-  PyObject *__pyx_t_3 = NULL;
-  PyObject *__pyx_t_4 = NULL;
-  int __pyx_t_5;
-  int __pyx_t_6;
-  int __pyx_t_7;
-  long __pyx_t_8;
-  char *__pyx_t_9;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("_util_dtypestring", 0);
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":846
- * 
- *     cdef dtype child
- *     cdef int endian_detector = 1             # <<<<<<<<<<<<<<
- *     cdef bint little_endian = ((<char*>&endian_detector)[0] != 0)
- *     cdef tuple fields
- */
-  __pyx_v_endian_detector = 1;
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":847
- *     cdef dtype child
- *     cdef int endian_detector = 1
- *     cdef bint little_endian = ((<char*>&endian_detector)[0] != 0)             # <<<<<<<<<<<<<<
- *     cdef tuple fields
- * 
- */
-  __pyx_v_little_endian = ((((char *)(&__pyx_v_endian_detector))[0]) != 0);
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":850
- *     cdef tuple fields
- * 
- *     for childname in descr.names:             # <<<<<<<<<<<<<<
- *         fields = descr.fields[childname]
- *         child, new_offset = fields
- */
-  if (unlikely(__pyx_v_descr->names == Py_None)) {
-    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-    __PYX_ERR(1, 850, __pyx_L1_error)
-  }
-  __pyx_t_1 = __pyx_v_descr->names; __Pyx_INCREF(__pyx_t_1); __pyx_t_2 = 0;
-  for (;;) {
-    if (__pyx_t_2 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
-    #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_3); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(1, 850, __pyx_L1_error)
-    #else
-    __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 850, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    #endif
-    __Pyx_XDECREF_SET(__pyx_v_childname, __pyx_t_3);
-    __pyx_t_3 = 0;
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":851
- * 
- *     for childname in descr.names:
- *         fields = descr.fields[childname]             # <<<<<<<<<<<<<<
- *         child, new_offset = fields
- * 
- */
-    if (unlikely(__pyx_v_descr->fields == Py_None)) {
-      PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(1, 851, __pyx_L1_error)
-    }
-    __pyx_t_3 = __Pyx_PyDict_GetItem(__pyx_v_descr->fields, __pyx_v_childname); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 851, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    if (!(likely(PyTuple_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_t_3)->tp_name), 0))) __PYX_ERR(1, 851, __pyx_L1_error)
-    __Pyx_XDECREF_SET(__pyx_v_fields, ((PyObject*)__pyx_t_3));
-    __pyx_t_3 = 0;
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":852
- *     for childname in descr.names:
- *         fields = descr.fields[childname]
- *         child, new_offset = fields             # <<<<<<<<<<<<<<
- * 
- *         if (end - f) - <int>(new_offset - offset[0]) < 15:
- */
-    if (likely(__pyx_v_fields != Py_None)) {
-      PyObject* sequence = __pyx_v_fields;
-      Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
-      if (unlikely(size != 2)) {
-        if (size > 2) __Pyx_RaiseTooManyValuesError(2);
-        else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-        __PYX_ERR(1, 852, __pyx_L1_error)
-      }
-      #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-      __pyx_t_3 = PyTuple_GET_ITEM(sequence, 0); 
-      __pyx_t_4 = PyTuple_GET_ITEM(sequence, 1); 
-      __Pyx_INCREF(__pyx_t_3);
-      __Pyx_INCREF(__pyx_t_4);
-      #else
-      __pyx_t_3 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 852, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 852, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      #endif
-    } else {
-      __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(1, 852, __pyx_L1_error)
-    }
-    if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_dtype))))) __PYX_ERR(1, 852, __pyx_L1_error)
-    __Pyx_XDECREF_SET(__pyx_v_child, ((PyArray_Descr *)__pyx_t_3));
-    __pyx_t_3 = 0;
-    __Pyx_XDECREF_SET(__pyx_v_new_offset, __pyx_t_4);
-    __pyx_t_4 = 0;
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":854
- *         child, new_offset = fields
- * 
- *         if (end - f) - <int>(new_offset - offset[0]) < 15:             # <<<<<<<<<<<<<<
- *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")
- * 
- */
-    __pyx_t_4 = __Pyx_PyInt_From_int((__pyx_v_offset[0])); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 854, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_3 = PyNumber_Subtract(__pyx_v_new_offset, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 854, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 854, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_6 = ((((__pyx_v_end - __pyx_v_f) - ((int)__pyx_t_5)) < 15) != 0);
-    if (unlikely(__pyx_t_6)) {
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":855
- * 
- *         if (end - f) - <int>(new_offset - offset[0]) < 15:
- *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")             # <<<<<<<<<<<<<<
- * 
- *         if ((child.byteorder == c'>' and little_endian) or
- */
-      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple__14, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 855, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __PYX_ERR(1, 855, __pyx_L1_error)
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":854
- *         child, new_offset = fields
- * 
- *         if (end - f) - <int>(new_offset - offset[0]) < 15:             # <<<<<<<<<<<<<<
- *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")
- * 
- */
-    }
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":857
- *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")
- * 
- *         if ((child.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
- *             (child.byteorder == c'<' and not little_endian)):
- *             raise ValueError(u"Non-native byte order not supported")
- */
-    __pyx_t_7 = ((__pyx_v_child->byteorder == '>') != 0);
-    if (!__pyx_t_7) {
-      goto __pyx_L8_next_or;
-    } else {
-    }
-    __pyx_t_7 = (__pyx_v_little_endian != 0);
-    if (!__pyx_t_7) {
-    } else {
-      __pyx_t_6 = __pyx_t_7;
-      goto __pyx_L7_bool_binop_done;
-    }
-    __pyx_L8_next_or:;
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":858
- * 
- *         if ((child.byteorder == c'>' and little_endian) or
- *             (child.byteorder == c'<' and not little_endian)):             # <<<<<<<<<<<<<<
- *             raise ValueError(u"Non-native byte order not supported")
- *             # One could encode it in the format string and have Cython
- */
-    __pyx_t_7 = ((__pyx_v_child->byteorder == '<') != 0);
-    if (__pyx_t_7) {
-    } else {
-      __pyx_t_6 = __pyx_t_7;
-      goto __pyx_L7_bool_binop_done;
-    }
-    __pyx_t_7 = ((!(__pyx_v_little_endian != 0)) != 0);
-    __pyx_t_6 = __pyx_t_7;
-    __pyx_L7_bool_binop_done:;
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":857
- *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")
- * 
- *         if ((child.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
- *             (child.byteorder == c'<' and not little_endian)):
- *             raise ValueError(u"Non-native byte order not supported")
- */
-    if (unlikely(__pyx_t_6)) {
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":859
- *         if ((child.byteorder == c'>' and little_endian) or
- *             (child.byteorder == c'<' and not little_endian)):
- *             raise ValueError(u"Non-native byte order not supported")             # <<<<<<<<<<<<<<
- *             # One could encode it in the format string and have Cython
- *             # complain instead, BUT: < and > in format strings also imply
- */
-      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 859, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __PYX_ERR(1, 859, __pyx_L1_error)
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":857
- *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")
- * 
- *         if ((child.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
- *             (child.byteorder == c'<' and not little_endian)):
- *             raise ValueError(u"Non-native byte order not supported")
- */
-    }
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":869
- * 
- *         # Output padding bytes
- *         while offset[0] < new_offset:             # <<<<<<<<<<<<<<
- *             f[0] = 120 # "x"; pad byte
- *             f += 1
- */
-    while (1) {
-      __pyx_t_3 = __Pyx_PyInt_From_int((__pyx_v_offset[0])); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 869, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_t_3, __pyx_v_new_offset, Py_LT); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 869, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 869, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (!__pyx_t_6) break;
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":870
- *         # Output padding bytes
- *         while offset[0] < new_offset:
- *             f[0] = 120 # "x"; pad byte             # <<<<<<<<<<<<<<
- *             f += 1
- *             offset[0] += 1
- */
-      (__pyx_v_f[0]) = 0x78;
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":871
- *         while offset[0] < new_offset:
- *             f[0] = 120 # "x"; pad byte
- *             f += 1             # <<<<<<<<<<<<<<
- *             offset[0] += 1
- * 
- */
-      __pyx_v_f = (__pyx_v_f + 1);
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":872
- *             f[0] = 120 # "x"; pad byte
- *             f += 1
- *             offset[0] += 1             # <<<<<<<<<<<<<<
- * 
- *         offset[0] += child.itemsize
- */
-      __pyx_t_8 = 0;
-      (__pyx_v_offset[__pyx_t_8]) = ((__pyx_v_offset[__pyx_t_8]) + 1);
-    }
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":874
- *             offset[0] += 1
- * 
- *         offset[0] += child.itemsize             # <<<<<<<<<<<<<<
- * 
- *         if not PyDataType_HASFIELDS(child):
- */
-    __pyx_t_8 = 0;
-    (__pyx_v_offset[__pyx_t_8]) = ((__pyx_v_offset[__pyx_t_8]) + __pyx_v_child->elsize);
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":876
- *         offset[0] += child.itemsize
- * 
- *         if not PyDataType_HASFIELDS(child):             # <<<<<<<<<<<<<<
- *             t = child.type_num
- *             if end - f < 5:
- */
-    __pyx_t_6 = ((!(PyDataType_HASFIELDS(__pyx_v_child) != 0)) != 0);
-    if (__pyx_t_6) {
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":877
- * 
- *         if not PyDataType_HASFIELDS(child):
- *             t = child.type_num             # <<<<<<<<<<<<<<
- *             if end - f < 5:
- *                 raise RuntimeError(u"Format string allocated too short.")
- */
-      __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_child->type_num); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 877, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __Pyx_XDECREF_SET(__pyx_v_t, __pyx_t_4);
-      __pyx_t_4 = 0;
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":878
- *         if not PyDataType_HASFIELDS(child):
- *             t = child.type_num
- *             if end - f < 5:             # <<<<<<<<<<<<<<
- *                 raise RuntimeError(u"Format string allocated too short.")
- * 
- */
-      __pyx_t_6 = (((__pyx_v_end - __pyx_v_f) < 5) != 0);
-      if (unlikely(__pyx_t_6)) {
-
-        /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":879
- *             t = child.type_num
- *             if end - f < 5:
- *                 raise RuntimeError(u"Format string allocated too short.")             # <<<<<<<<<<<<<<
- * 
- *             # Until ticket #99 is fixed, use integers to avoid warnings
- */
-        __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple__15, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 879, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_4);
-        __Pyx_Raise(__pyx_t_4, 0, 0, 0);
-        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        __PYX_ERR(1, 879, __pyx_L1_error)
-
-        /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":878
- *         if not PyDataType_HASFIELDS(child):
- *             t = child.type_num
- *             if end - f < 5:             # <<<<<<<<<<<<<<
- *                 raise RuntimeError(u"Format string allocated too short.")
- * 
- */
-      }
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":882
- * 
- *             # Until ticket #99 is fixed, use integers to avoid warnings
- *             if   t == NPY_BYTE:        f[0] =  98 #"b"             # <<<<<<<<<<<<<<
- *             elif t == NPY_UBYTE:       f[0] =  66 #"B"
- *             elif t == NPY_SHORT:       f[0] = 104 #"h"
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_BYTE); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 882, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 882, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 882, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 98;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":883
- *             # Until ticket #99 is fixed, use integers to avoid warnings
- *             if   t == NPY_BYTE:        f[0] =  98 #"b"
- *             elif t == NPY_UBYTE:       f[0] =  66 #"B"             # <<<<<<<<<<<<<<
- *             elif t == NPY_SHORT:       f[0] = 104 #"h"
- *             elif t == NPY_USHORT:      f[0] =  72 #"H"
- */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_UBYTE); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 883, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 883, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 883, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 66;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":884
- *             if   t == NPY_BYTE:        f[0] =  98 #"b"
- *             elif t == NPY_UBYTE:       f[0] =  66 #"B"
- *             elif t == NPY_SHORT:       f[0] = 104 #"h"             # <<<<<<<<<<<<<<
- *             elif t == NPY_USHORT:      f[0] =  72 #"H"
- *             elif t == NPY_INT:         f[0] = 105 #"i"
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_SHORT); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 884, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 884, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 884, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 0x68;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":885
- *             elif t == NPY_UBYTE:       f[0] =  66 #"B"
- *             elif t == NPY_SHORT:       f[0] = 104 #"h"
- *             elif t == NPY_USHORT:      f[0] =  72 #"H"             # <<<<<<<<<<<<<<
- *             elif t == NPY_INT:         f[0] = 105 #"i"
- *             elif t == NPY_UINT:        f[0] =  73 #"I"
- */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_USHORT); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 885, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 885, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 885, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 72;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":886
- *             elif t == NPY_SHORT:       f[0] = 104 #"h"
- *             elif t == NPY_USHORT:      f[0] =  72 #"H"
- *             elif t == NPY_INT:         f[0] = 105 #"i"             # <<<<<<<<<<<<<<
- *             elif t == NPY_UINT:        f[0] =  73 #"I"
- *             elif t == NPY_LONG:        f[0] = 108 #"l"
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_INT); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 886, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 886, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 886, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 0x69;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":887
- *             elif t == NPY_USHORT:      f[0] =  72 #"H"
- *             elif t == NPY_INT:         f[0] = 105 #"i"
- *             elif t == NPY_UINT:        f[0] =  73 #"I"             # <<<<<<<<<<<<<<
- *             elif t == NPY_LONG:        f[0] = 108 #"l"
- *             elif t == NPY_ULONG:       f[0] = 76  #"L"
- */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_UINT); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 887, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 887, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 887, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 73;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":888
- *             elif t == NPY_INT:         f[0] = 105 #"i"
- *             elif t == NPY_UINT:        f[0] =  73 #"I"
- *             elif t == NPY_LONG:        f[0] = 108 #"l"             # <<<<<<<<<<<<<<
- *             elif t == NPY_ULONG:       f[0] = 76  #"L"
- *             elif t == NPY_LONGLONG:    f[0] = 113 #"q"
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_LONG); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 888, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 888, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 888, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 0x6C;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":889
- *             elif t == NPY_UINT:        f[0] =  73 #"I"
- *             elif t == NPY_LONG:        f[0] = 108 #"l"
- *             elif t == NPY_ULONG:       f[0] = 76  #"L"             # <<<<<<<<<<<<<<
- *             elif t == NPY_LONGLONG:    f[0] = 113 #"q"
- *             elif t == NPY_ULONGLONG:   f[0] = 81  #"Q"
- */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_ULONG); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 889, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 889, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 889, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 76;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":890
- *             elif t == NPY_LONG:        f[0] = 108 #"l"
- *             elif t == NPY_ULONG:       f[0] = 76  #"L"
- *             elif t == NPY_LONGLONG:    f[0] = 113 #"q"             # <<<<<<<<<<<<<<
- *             elif t == NPY_ULONGLONG:   f[0] = 81  #"Q"
- *             elif t == NPY_FLOAT:       f[0] = 102 #"f"
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_LONGLONG); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 890, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 890, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 890, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 0x71;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":891
- *             elif t == NPY_ULONG:       f[0] = 76  #"L"
- *             elif t == NPY_LONGLONG:    f[0] = 113 #"q"
- *             elif t == NPY_ULONGLONG:   f[0] = 81  #"Q"             # <<<<<<<<<<<<<<
- *             elif t == NPY_FLOAT:       f[0] = 102 #"f"
- *             elif t == NPY_DOUBLE:      f[0] = 100 #"d"
- */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_ULONGLONG); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 891, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 891, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 891, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 81;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":892
- *             elif t == NPY_LONGLONG:    f[0] = 113 #"q"
- *             elif t == NPY_ULONGLONG:   f[0] = 81  #"Q"
- *             elif t == NPY_FLOAT:       f[0] = 102 #"f"             # <<<<<<<<<<<<<<
- *             elif t == NPY_DOUBLE:      f[0] = 100 #"d"
- *             elif t == NPY_LONGDOUBLE:  f[0] = 103 #"g"
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_FLOAT); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 892, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 892, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 892, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 0x66;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":893
- *             elif t == NPY_ULONGLONG:   f[0] = 81  #"Q"
- *             elif t == NPY_FLOAT:       f[0] = 102 #"f"
- *             elif t == NPY_DOUBLE:      f[0] = 100 #"d"             # <<<<<<<<<<<<<<
- *             elif t == NPY_LONGDOUBLE:  f[0] = 103 #"g"
- *             elif t == NPY_CFLOAT:      f[0] = 90; f[1] = 102; f += 1 # Zf
- */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_DOUBLE); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 893, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 893, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 893, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 0x64;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":894
- *             elif t == NPY_FLOAT:       f[0] = 102 #"f"
- *             elif t == NPY_DOUBLE:      f[0] = 100 #"d"
- *             elif t == NPY_LONGDOUBLE:  f[0] = 103 #"g"             # <<<<<<<<<<<<<<
- *             elif t == NPY_CFLOAT:      f[0] = 90; f[1] = 102; f += 1 # Zf
- *             elif t == NPY_CDOUBLE:     f[0] = 90; f[1] = 100; f += 1 # Zd
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_LONGDOUBLE); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 894, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 894, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 894, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 0x67;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":895
- *             elif t == NPY_DOUBLE:      f[0] = 100 #"d"
- *             elif t == NPY_LONGDOUBLE:  f[0] = 103 #"g"
- *             elif t == NPY_CFLOAT:      f[0] = 90; f[1] = 102; f += 1 # Zf             # <<<<<<<<<<<<<<
- *             elif t == NPY_CDOUBLE:     f[0] = 90; f[1] = 100; f += 1 # Zd
- *             elif t == NPY_CLONGDOUBLE: f[0] = 90; f[1] = 103; f += 1 # Zg
- */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_CFLOAT); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 895, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 895, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 895, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 90;
-        (__pyx_v_f[1]) = 0x66;
-        __pyx_v_f = (__pyx_v_f + 1);
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":896
- *             elif t == NPY_LONGDOUBLE:  f[0] = 103 #"g"
- *             elif t == NPY_CFLOAT:      f[0] = 90; f[1] = 102; f += 1 # Zf
- *             elif t == NPY_CDOUBLE:     f[0] = 90; f[1] = 100; f += 1 # Zd             # <<<<<<<<<<<<<<
- *             elif t == NPY_CLONGDOUBLE: f[0] = 90; f[1] = 103; f += 1 # Zg
- *             elif t == NPY_OBJECT:      f[0] = 79 #"O"
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_CDOUBLE); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 896, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 896, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 896, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 90;
-        (__pyx_v_f[1]) = 0x64;
-        __pyx_v_f = (__pyx_v_f + 1);
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":897
- *             elif t == NPY_CFLOAT:      f[0] = 90; f[1] = 102; f += 1 # Zf
- *             elif t == NPY_CDOUBLE:     f[0] = 90; f[1] = 100; f += 1 # Zd
- *             elif t == NPY_CLONGDOUBLE: f[0] = 90; f[1] = 103; f += 1 # Zg             # <<<<<<<<<<<<<<
- *             elif t == NPY_OBJECT:      f[0] = 79 #"O"
- *             else:
- */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_CLONGDOUBLE); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 897, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 897, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 897, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 90;
-        (__pyx_v_f[1]) = 0x67;
-        __pyx_v_f = (__pyx_v_f + 1);
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":898
- *             elif t == NPY_CDOUBLE:     f[0] = 90; f[1] = 100; f += 1 # Zd
- *             elif t == NPY_CLONGDOUBLE: f[0] = 90; f[1] = 103; f += 1 # Zg
- *             elif t == NPY_OBJECT:      f[0] = 79 #"O"             # <<<<<<<<<<<<<<
- *             else:
- *                 raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_OBJECT); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 898, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 898, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 898, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (likely(__pyx_t_6)) {
-        (__pyx_v_f[0]) = 79;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":900
- *             elif t == NPY_OBJECT:      f[0] = 79 #"O"
- *             else:
- *                 raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)             # <<<<<<<<<<<<<<
- *             f += 1
- *         else:
- */
-      /*else*/ {
-        __pyx_t_3 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_unknown_dtype_code_in_numpy_pxd, __pyx_v_t); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 900, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 900, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_4);
-        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        __Pyx_Raise(__pyx_t_4, 0, 0, 0);
-        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        __PYX_ERR(1, 900, __pyx_L1_error)
-      }
-      __pyx_L15:;
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":901
- *             else:
- *                 raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)
- *             f += 1             # <<<<<<<<<<<<<<
- *         else:
- *             # Cython ignores struct boundary information ("T{...}"),
- */
-      __pyx_v_f = (__pyx_v_f + 1);
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":876
- *         offset[0] += child.itemsize
- * 
- *         if not PyDataType_HASFIELDS(child):             # <<<<<<<<<<<<<<
- *             t = child.type_num
- *             if end - f < 5:
- */
-      goto __pyx_L13;
-    }
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":905
- *             # Cython ignores struct boundary information ("T{...}"),
- *             # so don't output it
- *             f = _util_dtypestring(child, f, end, offset)             # <<<<<<<<<<<<<<
- *     return f
- * 
- */
-    /*else*/ {
-      __pyx_t_9 = __pyx_f_5numpy__util_dtypestring(__pyx_v_child, __pyx_v_f, __pyx_v_end, __pyx_v_offset); if (unlikely(__pyx_t_9 == ((char *)NULL))) __PYX_ERR(1, 905, __pyx_L1_error)
-      __pyx_v_f = __pyx_t_9;
-    }
-    __pyx_L13:;
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":850
- *     cdef tuple fields
- * 
- *     for childname in descr.names:             # <<<<<<<<<<<<<<
- *         fields = descr.fields[childname]
- *         child, new_offset = fields
- */
-  }
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":906
- *             # so don't output it
- *             f = _util_dtypestring(child, f, end, offset)
- *     return f             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = __pyx_v_f;
-  goto __pyx_L0;
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":841
- *         return ()
- * 
- * cdef inline char* _util_dtypestring(dtype descr, char* f, char* end, int* offset) except NULL:             # <<<<<<<<<<<<<<
- *     # Recursive utility function used in __getbuffer__ to get format
- *     # string. The new location in the format string is returned.
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_AddTraceback("numpy._util_dtypestring", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XDECREF((PyObject *)__pyx_v_child);
-  __Pyx_XDECREF(__pyx_v_fields);
-  __Pyx_XDECREF(__pyx_v_childname);
-  __Pyx_XDECREF(__pyx_v_new_offset);
-  __Pyx_XDECREF(__pyx_v_t);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1021
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1022
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":930
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1023
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":931
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1021
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1025
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1026
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":934
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1027
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1028
+    /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":936
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1027
+    /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1029
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":937
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1025
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1033
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
- *         _import_array()
+ *         __pyx_import_array()
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_import_array(void) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
@@ -20848,105 +19238,105 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1034
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
- *         _import_array()
+ *         __pyx_import_array()
  *     except Exception:
  */
   {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1035
+      /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":943
  * cdef inline int import_array() except -1:
  *     try:
- *         _import_array()             # <<<<<<<<<<<<<<
+ *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 1035, __pyx_L3_error)
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 943, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1034
+      /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
- *         _import_array()
+ *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1036
+    /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *     try:
- *         _import_array()
+ *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 1036, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 944, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1037
- *         _import_array()
+      /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":945
+ *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__16, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 1037, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 945, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 1037, __pyx_L5_except_error)
+      __PYX_ERR(1, 945, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1034
+    /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
- *         _import_array()
+ *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1033
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
- *         _import_array()
+ *         __pyx_import_array()
  */
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_5);
@@ -20956,15 +19346,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1039
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -20980,15 +19370,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1040
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -20996,84 +19386,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1041
+      /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":949
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 1041, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 949, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1040
+      /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1042
+    /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 1042, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 950, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1043
+      /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__17, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 1043, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 951, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 1043, __pyx_L5_except_error)
+      __PYX_ERR(1, 951, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1040
+    /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1039
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -21088,15 +19478,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1045
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -21112,15 +19502,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1046
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -21128,81 +19518,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1047
+      /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":955
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 1047, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 955, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1046
+      /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1048
+    /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":956
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
+ * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 1048, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 956, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1049
+      /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":957
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
+ * 
+ * cdef extern from *:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__17, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 1049, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 957, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 1049, __pyx_L5_except_error)
+      __PYX_ERR(1, 957, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1046
+    /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1045
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -21217,14 +19610,188 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":967
+ * 
+ * 
+ * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.timedelta64)`
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
+
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":979
+ *     bool
+ *     """
+ *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":967
+ * 
+ * 
+ * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.timedelta64)`
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":982
+ * 
+ * 
+ * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.datetime64)`
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("is_datetime64_object", 0);
+
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":994
+ *     bool
+ *     """
+ *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":982
+ * 
+ * 
+ * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.datetime64)`
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":997
+ * 
+ * 
+ * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy datetime64 object
+ */
+
+static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
+  npy_datetime __pyx_r;
+
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":1004
+ *     also needed.  That can be found using `get_datetime64_unit`.
+ *     """
+ *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":997
+ * 
+ * 
+ * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy datetime64 object
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":1007
+ * 
+ * 
+ * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy timedelta64 object
+ */
+
+static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
+  npy_timedelta __pyx_r;
+
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":1011
+ *     returns the int64 value underlying scalar numpy timedelta64 object
+ *     """
+ *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":1007
+ * 
+ * 
+ * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy timedelta64 object
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":1014
+ * 
+ * 
+ * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the unit part of the dtype for a numpy datetime64 object.
+ */
+
+static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
+  NPY_DATETIMEUNIT __pyx_r;
+
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":1018
+ *     returns the unit part of the dtype for a numpy datetime64 object.
+ *     """
+ *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
+ */
+  __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":1014
+ * 
+ * 
+ * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the unit part of the dtype for a numpy datetime64 object.
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
 /* "View.MemoryView":123
  *         cdef bint dtype_is_object
  * 
  *     def __cinit__(array self, tuple shape, Py_ssize_t itemsize, format not None,             # <<<<<<<<<<<<<<
  *                   mode="c", bint allocate_buffer=True):
  * 
  */
@@ -21420,15 +19987,15 @@
     /* "View.MemoryView":134
  * 
  *         if not self.ndim:
  *             raise ValueError("Empty shape tuple for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if itemsize <= 0:
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__18, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 134, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 134, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(2, 134, __pyx_L1_error)
 
     /* "View.MemoryView":133
  *         self.itemsize = itemsize
@@ -21452,15 +20019,15 @@
     /* "View.MemoryView":137
  * 
  *         if itemsize <= 0:
  *             raise ValueError("itemsize <= 0 for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if not isinstance(format, bytes):
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__19, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 137, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__14, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 137, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(2, 137, __pyx_L1_error)
 
     /* "View.MemoryView":136
  *             raise ValueError("Empty shape tuple for cython.array")
@@ -21579,15 +20146,15 @@
     /* "View.MemoryView":149
  * 
  *         if not self._shape:
  *             raise MemoryError("unable to allocate shape and strides.")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__20, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 149, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__15, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 149, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(2, 149, __pyx_L1_error)
 
     /* "View.MemoryView":148
  *         self._strides = self._shape + self.ndim
@@ -21853,15 +20420,15 @@
       /* "View.MemoryView":177
  *             self.data = <char *>malloc(self.len)
  *             if not self.data:
  *                 raise MemoryError("unable to allocate array data.")             # <<<<<<<<<<<<<<
  * 
  *             if self.dtype_is_object:
  */
-      __pyx_t_10 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__21, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(2, 177, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__16, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(2, 177, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_Raise(__pyx_t_10, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       __PYX_ERR(2, 177, __pyx_L1_error)
 
       /* "View.MemoryView":176
  * 
@@ -22097,15 +20664,15 @@
     /* "View.MemoryView":193
  *             bufmode = PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         if not (flags & bufmode):
  *             raise ValueError("Can only create a buffer that is contiguous in memory.")             # <<<<<<<<<<<<<<
  *         info.buf = self.data
  *         info.len = self.len
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__22, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 193, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__17, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 193, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(2, 193, __pyx_L1_error)
 
     /* "View.MemoryView":192
  *         elif self.mode == u"fortran":
@@ -22831,15 +21398,15 @@
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__23, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__18, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(2, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
@@ -22887,15 +21454,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__24, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__19, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(2, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
@@ -24616,15 +23183,15 @@
     /* "View.MemoryView":420
  *     def __setitem__(memoryview self, object index, object value):
  *         if self.view.readonly:
  *             raise TypeError("Cannot assign to read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         have_slices, index = _unellipsify(index, self.view.ndim)
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__25, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 420, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__20, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 420, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __PYX_ERR(2, 420, __pyx_L1_error)
 
     /* "View.MemoryView":419
  * 
@@ -25664,15 +24231,15 @@
       /* "View.MemoryView":497
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:
  *             raise ValueError("Unable to convert item to object")             # <<<<<<<<<<<<<<
  *         else:
  *             if len(self.view.format) == 1:
  */
-      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__26, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 497, __pyx_L5_except_error)
+      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__21, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 497, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_Raise(__pyx_t_6, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __PYX_ERR(2, 497, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
@@ -26026,15 +24593,15 @@
     /* "View.MemoryView":522
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         if flags & PyBUF_WRITABLE and self.view.readonly:
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_ND:
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__27, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 522, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__22, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 522, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(2, 522, __pyx_L1_error)
 
     /* "View.MemoryView":521
  *     @cname('getbuffer')
@@ -26575,15 +25142,15 @@
     /* "View.MemoryView":572
  *         if self.view.strides == NULL:
  * 
  *             raise ValueError("Buffer view does not expose strides")             # <<<<<<<<<<<<<<
  * 
  *         return tuple([stride for stride in self.view.strides[:self.view.ndim]])
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__28, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 572, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__23, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 572, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __PYX_ERR(2, 572, __pyx_L1_error)
 
     /* "View.MemoryView":570
  *     @property
@@ -26692,15 +25259,15 @@
  *             return (-1,) * self.view.ndim             # <<<<<<<<<<<<<<
  * 
  *         return tuple([suboffset for suboffset in self.view.suboffsets[:self.view.ndim]])
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_self->view.ndim); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 579, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = PyNumber_Multiply(__pyx_tuple__29, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 579, __pyx_L1_error)
+    __pyx_t_3 = PyNumber_Multiply(__pyx_tuple__24, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 579, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
     /* "View.MemoryView":578
@@ -27730,15 +26297,15 @@
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__30, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__25, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(2, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
@@ -27786,15 +26353,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__31, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__26, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(2, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
@@ -28143,17 +26710,17 @@
  *             else:
  */
         __pyx_t_8 = PyObject_Length(__pyx_v_tup); if (unlikely(__pyx_t_8 == ((Py_ssize_t)-1))) __PYX_ERR(2, 684, __pyx_L1_error)
         __pyx_t_7 = PyList_New(1 * ((((__pyx_v_ndim - __pyx_t_8) + 1)<0) ? 0:((__pyx_v_ndim - __pyx_t_8) + 1))); if (unlikely(!__pyx_t_7)) __PYX_ERR(2, 684, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
         { Py_ssize_t __pyx_temp;
           for (__pyx_temp=0; __pyx_temp < ((__pyx_v_ndim - __pyx_t_8) + 1); __pyx_temp++) {
-            __Pyx_INCREF(__pyx_slice__32);
-            __Pyx_GIVEREF(__pyx_slice__32);
-            PyList_SET_ITEM(__pyx_t_7, __pyx_temp, __pyx_slice__32);
+            __Pyx_INCREF(__pyx_slice__27);
+            __Pyx_GIVEREF(__pyx_slice__27);
+            PyList_SET_ITEM(__pyx_t_7, __pyx_temp, __pyx_slice__27);
           }
         }
         __pyx_t_9 = __Pyx_PyList_Extend(__pyx_v_result, __pyx_t_7); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(2, 684, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
         /* "View.MemoryView":685
  *             if not seen_ellipsis:
@@ -28178,15 +26745,15 @@
  *                 seen_ellipsis = True
  *             else:
  *                 result.append(slice(None))             # <<<<<<<<<<<<<<
  *             have_slices = True
  *         else:
  */
       /*else*/ {
-        __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_result, __pyx_slice__32); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(2, 687, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_result, __pyx_slice__27); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(2, 687, __pyx_L1_error)
       }
       __pyx_L7:;
 
       /* "View.MemoryView":688
  *             else:
  *                 result.append(slice(None))
  *             have_slices = True             # <<<<<<<<<<<<<<
@@ -28318,17 +26885,17 @@
  * 
  *     return have_slices or nslices, tuple(result)
  */
     __pyx_t_3 = PyList_New(1 * ((__pyx_v_nslices<0) ? 0:__pyx_v_nslices)); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 698, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     { Py_ssize_t __pyx_temp;
       for (__pyx_temp=0; __pyx_temp < __pyx_v_nslices; __pyx_temp++) {
-        __Pyx_INCREF(__pyx_slice__32);
-        __Pyx_GIVEREF(__pyx_slice__32);
-        PyList_SET_ITEM(__pyx_t_3, __pyx_temp, __pyx_slice__32);
+        __Pyx_INCREF(__pyx_slice__27);
+        __Pyx_GIVEREF(__pyx_slice__27);
+        PyList_SET_ITEM(__pyx_t_3, __pyx_temp, __pyx_slice__27);
       }
     }
     __pyx_t_9 = __Pyx_PyList_Extend(__pyx_v_result, __pyx_t_3); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(2, 698, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
     /* "View.MemoryView":697
  * 
@@ -28447,15 +27014,15 @@
       /* "View.MemoryView":705
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:
  *             raise ValueError("Indirect dimensions not supported")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-      __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__33, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 705, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__28, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 705, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_Raise(__pyx_t_5, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __PYX_ERR(2, 705, __pyx_L1_error)
 
       /* "View.MemoryView":704
  * cdef assert_direct_dimensions(Py_ssize_t *suboffsets, int ndim):
@@ -30631,15 +29198,15 @@
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__34, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__29, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(2, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
@@ -30687,15 +29254,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__35, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__30, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(2, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
@@ -33964,15 +32531,15 @@
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xb068931, 0x82a3537, 0x6ae9995):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb068931, 0x82a3537, 0x6ae9995) = (name))" % __pyx_checksum)
  */
   __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__36, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__31, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(2, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xb068931, 0x82a3537, 0x6ae9995):
@@ -35050,33 +33617,29 @@
   {&__pyx_kp_s_Can_only_create_a_buffer_that_is, __pyx_k_Can_only_create_a_buffer_that_is, sizeof(__pyx_k_Can_only_create_a_buffer_that_is), 0, 0, 1, 0},
   {&__pyx_kp_s_Cannot_assign_to_read_only_memor, __pyx_k_Cannot_assign_to_read_only_memor, sizeof(__pyx_k_Cannot_assign_to_read_only_memor), 0, 0, 1, 0},
   {&__pyx_kp_s_Cannot_create_writable_memory_vi, __pyx_k_Cannot_create_writable_memory_vi, sizeof(__pyx_k_Cannot_create_writable_memory_vi), 0, 0, 1, 0},
   {&__pyx_kp_s_Cannot_index_with_type_s, __pyx_k_Cannot_index_with_type_s, sizeof(__pyx_k_Cannot_index_with_type_s), 0, 0, 1, 0},
   {&__pyx_n_s_Ellipsis, __pyx_k_Ellipsis, sizeof(__pyx_k_Ellipsis), 0, 0, 1, 1},
   {&__pyx_kp_s_Empty_shape_tuple_for_cython_arr, __pyx_k_Empty_shape_tuple_for_cython_arr, sizeof(__pyx_k_Empty_shape_tuple_for_cython_arr), 0, 0, 1, 0},
   {&__pyx_kp_s_Expected_at_least_d_argument_s_g, __pyx_k_Expected_at_least_d_argument_s_g, sizeof(__pyx_k_Expected_at_least_d_argument_s_g), 0, 0, 1, 0},
-  {&__pyx_kp_u_Format_string_allocated_too_shor, __pyx_k_Format_string_allocated_too_shor, sizeof(__pyx_k_Format_string_allocated_too_shor), 0, 1, 0, 0},
-  {&__pyx_kp_u_Format_string_allocated_too_shor_2, __pyx_k_Format_string_allocated_too_shor_2, sizeof(__pyx_k_Format_string_allocated_too_shor_2), 0, 1, 0, 0},
   {&__pyx_kp_s_Function_call_with_ambiguous_arg, __pyx_k_Function_call_with_ambiguous_arg, sizeof(__pyx_k_Function_call_with_ambiguous_arg), 0, 0, 1, 0},
   {&__pyx_n_s_ImportError, __pyx_k_ImportError, sizeof(__pyx_k_ImportError), 0, 0, 1, 1},
   {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_k_Incompatible_checksums_0x_x_vs_0, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0), 0, 0, 1, 0},
   {&__pyx_n_s_IndexError, __pyx_k_IndexError, sizeof(__pyx_k_IndexError), 0, 0, 1, 1},
   {&__pyx_kp_s_Indirect_dimensions_not_supporte, __pyx_k_Indirect_dimensions_not_supporte, sizeof(__pyx_k_Indirect_dimensions_not_supporte), 0, 0, 1, 0},
   {&__pyx_kp_s_Invalid_mode_expected_c_or_fortr, __pyx_k_Invalid_mode_expected_c_or_fortr, sizeof(__pyx_k_Invalid_mode_expected_c_or_fortr), 0, 0, 1, 0},
   {&__pyx_kp_s_Invalid_shape_in_axis_d_d, __pyx_k_Invalid_shape_in_axis_d_d, sizeof(__pyx_k_Invalid_shape_in_axis_d_d), 0, 0, 1, 0},
   {&__pyx_n_s_MemoryError, __pyx_k_MemoryError, sizeof(__pyx_k_MemoryError), 0, 0, 1, 1},
   {&__pyx_kp_s_MemoryView_of_r_at_0x_x, __pyx_k_MemoryView_of_r_at_0x_x, sizeof(__pyx_k_MemoryView_of_r_at_0x_x), 0, 0, 1, 0},
   {&__pyx_kp_s_MemoryView_of_r_object, __pyx_k_MemoryView_of_r_object, sizeof(__pyx_k_MemoryView_of_r_object), 0, 0, 1, 0},
   {&__pyx_kp_s_No_matching_signature_found, __pyx_k_No_matching_signature_found, sizeof(__pyx_k_No_matching_signature_found), 0, 0, 1, 0},
-  {&__pyx_kp_u_Non_native_byte_order_not_suppor, __pyx_k_Non_native_byte_order_not_suppor, sizeof(__pyx_k_Non_native_byte_order_not_suppor), 0, 1, 0, 0},
   {&__pyx_n_b_O, __pyx_k_O, sizeof(__pyx_k_O), 0, 0, 0, 1},
   {&__pyx_kp_s_Out_of_bounds_on_buffer_access_a, __pyx_k_Out_of_bounds_on_buffer_access_a, sizeof(__pyx_k_Out_of_bounds_on_buffer_access_a), 0, 0, 1, 0},
   {&__pyx_n_s_P_data, __pyx_k_P_data, sizeof(__pyx_k_P_data), 0, 0, 1, 1},
   {&__pyx_n_s_PickleError, __pyx_k_PickleError, sizeof(__pyx_k_PickleError), 0, 0, 1, 1},
-  {&__pyx_n_s_RuntimeError, __pyx_k_RuntimeError, sizeof(__pyx_k_RuntimeError), 0, 0, 1, 1},
   {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
   {&__pyx_kp_s_Unable_to_convert_item_to_object, __pyx_k_Unable_to_convert_item_to_object, sizeof(__pyx_k_Unable_to_convert_item_to_object), 0, 0, 1, 0},
   {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
   {&__pyx_n_s_View_MemoryView, __pyx_k_View_MemoryView, sizeof(__pyx_k_View_MemoryView), 0, 0, 1, 1},
   {&__pyx_kp_s__2, __pyx_k__2, sizeof(__pyx_k__2), 0, 0, 1, 0},
   {&__pyx_n_s_allocate_buffer, __pyx_k_allocate_buffer, sizeof(__pyx_k_allocate_buffer), 0, 0, 1, 1},
   {&__pyx_n_s_args, __pyx_k_args, sizeof(__pyx_k_args), 0, 0, 1, 1},
@@ -35130,16 +33693,14 @@
   {&__pyx_n_s_max_iter, __pyx_k_max_iter, sizeof(__pyx_k_max_iter), 0, 0, 1, 1},
   {&__pyx_n_s_memview, __pyx_k_memview, sizeof(__pyx_k_memview), 0, 0, 1, 1},
   {&__pyx_n_s_min_num_intervals, __pyx_k_min_num_intervals, sizeof(__pyx_k_min_num_intervals), 0, 0, 1, 1},
   {&__pyx_n_s_mode, __pyx_k_mode, sizeof(__pyx_k_mode), 0, 0, 1, 1},
   {&__pyx_n_s_n_interpolation_points, __pyx_k_n_interpolation_points, sizeof(__pyx_k_n_interpolation_points), 0, 0, 1, 1},
   {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
   {&__pyx_n_s_name_2, __pyx_k_name_2, sizeof(__pyx_k_name_2), 0, 0, 1, 1},
-  {&__pyx_kp_u_ndarray_is_not_C_contiguous, __pyx_k_ndarray_is_not_C_contiguous, sizeof(__pyx_k_ndarray_is_not_C_contiguous), 0, 1, 0, 0},
-  {&__pyx_kp_u_ndarray_is_not_Fortran_contiguou, __pyx_k_ndarray_is_not_Fortran_contiguou, sizeof(__pyx_k_ndarray_is_not_Fortran_contiguou), 0, 1, 0, 0},
   {&__pyx_n_s_ndim, __pyx_k_ndim, sizeof(__pyx_k_ndim), 0, 0, 1, 1},
   {&__pyx_n_s_new, __pyx_k_new, sizeof(__pyx_k_new), 0, 0, 1, 1},
   {&__pyx_kp_s_no_default___reduce___due_to_non, __pyx_k_no_default___reduce___due_to_non, sizeof(__pyx_k_no_default___reduce___due_to_non), 0, 0, 1, 0},
   {&__pyx_n_s_np, __pyx_k_np, sizeof(__pyx_k_np), 0, 0, 1, 1},
   {&__pyx_n_s_num_threads, __pyx_k_num_threads, sizeof(__pyx_k_num_threads), 0, 0, 1, 1},
   {&__pyx_n_s_numpy, __pyx_k_numpy, sizeof(__pyx_k_numpy), 0, 0, 1, 1},
   {&__pyx_kp_u_numpy_core_multiarray_failed_to, __pyx_k_numpy_core_multiarray_failed_to, sizeof(__pyx_k_numpy_core_multiarray_failed_to), 0, 1, 0, 0},
@@ -35187,29 +33748,27 @@
   {&__pyx_n_s_strip, __pyx_k_strip, sizeof(__pyx_k_strip), 0, 0, 1, 1},
   {&__pyx_n_s_struct, __pyx_k_struct, sizeof(__pyx_k_struct), 0, 0, 1, 1},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_n_s_theta, __pyx_k_theta, sizeof(__pyx_k_theta), 0, 0, 1, 1},
   {&__pyx_n_s_tree, __pyx_k_tree, sizeof(__pyx_k_tree), 0, 0, 1, 1},
   {&__pyx_kp_s_unable_to_allocate_array_data, __pyx_k_unable_to_allocate_array_data, sizeof(__pyx_k_unable_to_allocate_array_data), 0, 0, 1, 0},
   {&__pyx_kp_s_unable_to_allocate_shape_and_str, __pyx_k_unable_to_allocate_shape_and_str, sizeof(__pyx_k_unable_to_allocate_shape_and_str), 0, 0, 1, 0},
-  {&__pyx_kp_u_unknown_dtype_code_in_numpy_pxd, __pyx_k_unknown_dtype_code_in_numpy_pxd, sizeof(__pyx_k_unknown_dtype_code_in_numpy_pxd), 0, 1, 0, 0},
   {&__pyx_n_s_unpack, __pyx_k_unpack, sizeof(__pyx_k_unpack), 0, 0, 1, 1},
   {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
   {&__pyx_n_s_y_tilde_values, __pyx_k_y_tilde_values, sizeof(__pyx_k_y_tilde_values), 0, 0, 1, 1},
   {&__pyx_n_s_zeros, __pyx_k_zeros, sizeof(__pyx_k_zeros), 0, 0, 1, 1},
   {&__pyx_n_s_zeros_like, __pyx_k_zeros_like, sizeof(__pyx_k_zeros_like), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 57, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(0, 103, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(0, 135, __pyx_L1_error)
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(1, 272, __pyx_L1_error)
-  __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(1, 855, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 1037, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 945, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(2, 134, __pyx_L1_error)
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(2, 152, __pyx_L1_error)
   __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(2, 406, __pyx_L1_error)
   __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(2, 615, __pyx_L1_error)
   __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(2, 834, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
@@ -35229,362 +33788,307 @@
   __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_s_No_matching_signature_found); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 103, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
   __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_s_Function_call_with_ambiguous_arg); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 103, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":272
- *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_C_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not C contiguous")             # <<<<<<<<<<<<<<
- * 
- *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)
- */
-  __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_u_ndarray_is_not_C_contiguous); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(1, 272, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__11);
-  __Pyx_GIVEREF(__pyx_tuple__11);
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":276
- *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_F_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not Fortran contiguous")             # <<<<<<<<<<<<<<
- * 
- *             info.buf = PyArray_DATA(self)
- */
-  __pyx_tuple__12 = PyTuple_Pack(1, __pyx_kp_u_ndarray_is_not_Fortran_contiguou); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(1, 276, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__12);
-  __Pyx_GIVEREF(__pyx_tuple__12);
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":306
- *                 if ((descr.byteorder == c'>' and little_endian) or
- *                     (descr.byteorder == c'<' and not little_endian)):
- *                     raise ValueError(u"Non-native byte order not supported")             # <<<<<<<<<<<<<<
- *                 if   t == NPY_BYTE:        f = "b"
- *                 elif t == NPY_UBYTE:       f = "B"
- */
-  __pyx_tuple__13 = PyTuple_Pack(1, __pyx_kp_u_Non_native_byte_order_not_suppor); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(1, 306, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__13);
-  __Pyx_GIVEREF(__pyx_tuple__13);
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":855
- * 
- *         if (end - f) - <int>(new_offset - offset[0]) < 15:
- *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")             # <<<<<<<<<<<<<<
- * 
- *         if ((child.byteorder == c'>' and little_endian) or
- */
-  __pyx_tuple__14 = PyTuple_Pack(1, __pyx_kp_u_Format_string_allocated_too_shor); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(1, 855, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__14);
-  __Pyx_GIVEREF(__pyx_tuple__14);
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":879
- *             t = child.type_num
- *             if end - f < 5:
- *                 raise RuntimeError(u"Format string allocated too short.")             # <<<<<<<<<<<<<<
- * 
- *             # Until ticket #99 is fixed, use integers to avoid warnings
- */
-  __pyx_tuple__15 = PyTuple_Pack(1, __pyx_kp_u_Format_string_allocated_too_shor_2); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(1, 879, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__15);
-  __Pyx_GIVEREF(__pyx_tuple__15);
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1037
- *         _import_array()
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":945
+ *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple__16 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(1, 1037, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__16);
-  __Pyx_GIVEREF(__pyx_tuple__16);
+  __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(1, 945, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__11);
+  __Pyx_GIVEREF(__pyx_tuple__11);
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1043
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__17 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(1, 1043, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__17);
-  __Pyx_GIVEREF(__pyx_tuple__17);
+  __pyx_tuple__12 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(1, 951, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__12);
+  __Pyx_GIVEREF(__pyx_tuple__12);
 
   /* "View.MemoryView":134
  * 
  *         if not self.ndim:
  *             raise ValueError("Empty shape tuple for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if itemsize <= 0:
  */
-  __pyx_tuple__18 = PyTuple_Pack(1, __pyx_kp_s_Empty_shape_tuple_for_cython_arr); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(2, 134, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__18);
-  __Pyx_GIVEREF(__pyx_tuple__18);
+  __pyx_tuple__13 = PyTuple_Pack(1, __pyx_kp_s_Empty_shape_tuple_for_cython_arr); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(2, 134, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__13);
+  __Pyx_GIVEREF(__pyx_tuple__13);
 
   /* "View.MemoryView":137
  * 
  *         if itemsize <= 0:
  *             raise ValueError("itemsize <= 0 for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if not isinstance(format, bytes):
  */
-  __pyx_tuple__19 = PyTuple_Pack(1, __pyx_kp_s_itemsize_0_for_cython_array); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(2, 137, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__19);
-  __Pyx_GIVEREF(__pyx_tuple__19);
+  __pyx_tuple__14 = PyTuple_Pack(1, __pyx_kp_s_itemsize_0_for_cython_array); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(2, 137, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__14);
+  __Pyx_GIVEREF(__pyx_tuple__14);
 
   /* "View.MemoryView":149
  * 
  *         if not self._shape:
  *             raise MemoryError("unable to allocate shape and strides.")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__20 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_shape_and_str); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(2, 149, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__20);
-  __Pyx_GIVEREF(__pyx_tuple__20);
+  __pyx_tuple__15 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_shape_and_str); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(2, 149, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__15);
+  __Pyx_GIVEREF(__pyx_tuple__15);
 
   /* "View.MemoryView":177
  *             self.data = <char *>malloc(self.len)
  *             if not self.data:
  *                 raise MemoryError("unable to allocate array data.")             # <<<<<<<<<<<<<<
  * 
  *             if self.dtype_is_object:
  */
-  __pyx_tuple__21 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_array_data); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(2, 177, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__21);
-  __Pyx_GIVEREF(__pyx_tuple__21);
+  __pyx_tuple__16 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_array_data); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(2, 177, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__16);
+  __Pyx_GIVEREF(__pyx_tuple__16);
 
   /* "View.MemoryView":193
  *             bufmode = PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         if not (flags & bufmode):
  *             raise ValueError("Can only create a buffer that is contiguous in memory.")             # <<<<<<<<<<<<<<
  *         info.buf = self.data
  *         info.len = self.len
  */
-  __pyx_tuple__22 = PyTuple_Pack(1, __pyx_kp_s_Can_only_create_a_buffer_that_is); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(2, 193, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__22);
-  __Pyx_GIVEREF(__pyx_tuple__22);
+  __pyx_tuple__17 = PyTuple_Pack(1, __pyx_kp_s_Can_only_create_a_buffer_that_is); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(2, 193, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__17);
+  __Pyx_GIVEREF(__pyx_tuple__17);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_tuple__23 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(2, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__23);
-  __Pyx_GIVEREF(__pyx_tuple__23);
+  __pyx_tuple__18 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(2, 2, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__18);
+  __Pyx_GIVEREF(__pyx_tuple__18);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__24 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(2, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__24);
-  __Pyx_GIVEREF(__pyx_tuple__24);
+  __pyx_tuple__19 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__19);
+  __Pyx_GIVEREF(__pyx_tuple__19);
 
   /* "View.MemoryView":420
  *     def __setitem__(memoryview self, object index, object value):
  *         if self.view.readonly:
  *             raise TypeError("Cannot assign to read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         have_slices, index = _unellipsify(index, self.view.ndim)
  */
-  __pyx_tuple__25 = PyTuple_Pack(1, __pyx_kp_s_Cannot_assign_to_read_only_memor); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(2, 420, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__25);
-  __Pyx_GIVEREF(__pyx_tuple__25);
+  __pyx_tuple__20 = PyTuple_Pack(1, __pyx_kp_s_Cannot_assign_to_read_only_memor); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(2, 420, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__20);
+  __Pyx_GIVEREF(__pyx_tuple__20);
 
   /* "View.MemoryView":497
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:
  *             raise ValueError("Unable to convert item to object")             # <<<<<<<<<<<<<<
  *         else:
  *             if len(self.view.format) == 1:
  */
-  __pyx_tuple__26 = PyTuple_Pack(1, __pyx_kp_s_Unable_to_convert_item_to_object); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(2, 497, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__26);
-  __Pyx_GIVEREF(__pyx_tuple__26);
+  __pyx_tuple__21 = PyTuple_Pack(1, __pyx_kp_s_Unable_to_convert_item_to_object); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(2, 497, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__21);
+  __Pyx_GIVEREF(__pyx_tuple__21);
 
   /* "View.MemoryView":522
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         if flags & PyBUF_WRITABLE and self.view.readonly:
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_ND:
  */
-  __pyx_tuple__27 = PyTuple_Pack(1, __pyx_kp_s_Cannot_create_writable_memory_vi); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(2, 522, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__27);
-  __Pyx_GIVEREF(__pyx_tuple__27);
+  __pyx_tuple__22 = PyTuple_Pack(1, __pyx_kp_s_Cannot_create_writable_memory_vi); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(2, 522, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__22);
+  __Pyx_GIVEREF(__pyx_tuple__22);
 
   /* "View.MemoryView":572
  *         if self.view.strides == NULL:
  * 
  *             raise ValueError("Buffer view does not expose strides")             # <<<<<<<<<<<<<<
  * 
  *         return tuple([stride for stride in self.view.strides[:self.view.ndim]])
  */
-  __pyx_tuple__28 = PyTuple_Pack(1, __pyx_kp_s_Buffer_view_does_not_expose_stri); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(2, 572, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__28);
-  __Pyx_GIVEREF(__pyx_tuple__28);
+  __pyx_tuple__23 = PyTuple_Pack(1, __pyx_kp_s_Buffer_view_does_not_expose_stri); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(2, 572, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__23);
+  __Pyx_GIVEREF(__pyx_tuple__23);
 
   /* "View.MemoryView":579
  *     def suboffsets(self):
  *         if self.view.suboffsets == NULL:
  *             return (-1,) * self.view.ndim             # <<<<<<<<<<<<<<
  * 
  *         return tuple([suboffset for suboffset in self.view.suboffsets[:self.view.ndim]])
  */
-  __pyx_tuple__29 = PyTuple_New(1); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(2, 579, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__29);
+  __pyx_tuple__24 = PyTuple_New(1); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(2, 579, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__24);
   __Pyx_INCREF(__pyx_int_neg_1);
   __Pyx_GIVEREF(__pyx_int_neg_1);
-  PyTuple_SET_ITEM(__pyx_tuple__29, 0, __pyx_int_neg_1);
-  __Pyx_GIVEREF(__pyx_tuple__29);
+  PyTuple_SET_ITEM(__pyx_tuple__24, 0, __pyx_int_neg_1);
+  __Pyx_GIVEREF(__pyx_tuple__24);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_tuple__30 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(2, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__30);
-  __Pyx_GIVEREF(__pyx_tuple__30);
+  __pyx_tuple__25 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(2, 2, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__25);
+  __Pyx_GIVEREF(__pyx_tuple__25);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__31 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(2, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__31);
-  __Pyx_GIVEREF(__pyx_tuple__31);
+  __pyx_tuple__26 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__26);
+  __Pyx_GIVEREF(__pyx_tuple__26);
 
   /* "View.MemoryView":684
  *         if item is Ellipsis:
  *             if not seen_ellipsis:
  *                 result.extend([slice(None)] * (ndim - len(tup) + 1))             # <<<<<<<<<<<<<<
  *                 seen_ellipsis = True
  *             else:
  */
-  __pyx_slice__32 = PySlice_New(Py_None, Py_None, Py_None); if (unlikely(!__pyx_slice__32)) __PYX_ERR(2, 684, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_slice__32);
-  __Pyx_GIVEREF(__pyx_slice__32);
+  __pyx_slice__27 = PySlice_New(Py_None, Py_None, Py_None); if (unlikely(!__pyx_slice__27)) __PYX_ERR(2, 684, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_slice__27);
+  __Pyx_GIVEREF(__pyx_slice__27);
 
   /* "View.MemoryView":705
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:
  *             raise ValueError("Indirect dimensions not supported")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__33 = PyTuple_Pack(1, __pyx_kp_s_Indirect_dimensions_not_supporte); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(2, 705, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__33);
-  __Pyx_GIVEREF(__pyx_tuple__33);
+  __pyx_tuple__28 = PyTuple_Pack(1, __pyx_kp_s_Indirect_dimensions_not_supporte); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(2, 705, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__28);
+  __Pyx_GIVEREF(__pyx_tuple__28);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_tuple__34 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__34)) __PYX_ERR(2, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__34);
-  __Pyx_GIVEREF(__pyx_tuple__34);
+  __pyx_tuple__29 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(2, 2, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__29);
+  __Pyx_GIVEREF(__pyx_tuple__29);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__35 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__35)) __PYX_ERR(2, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__35);
-  __Pyx_GIVEREF(__pyx_tuple__35);
-  __pyx_tuple__36 = PyTuple_Pack(3, __pyx_int_184977713, __pyx_int_136983863, __pyx_int_112105877); if (unlikely(!__pyx_tuple__36)) __PYX_ERR(2, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__36);
-  __Pyx_GIVEREF(__pyx_tuple__36);
+  __pyx_tuple__30 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__30);
+  __Pyx_GIVEREF(__pyx_tuple__30);
+  __pyx_tuple__31 = PyTuple_Pack(3, __pyx_int_184977713, __pyx_int_136983863, __pyx_int_112105877); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__31);
+  __Pyx_GIVEREF(__pyx_tuple__31);
 
   /* "openTSNE/_tsne.pyx":103
  * 
  * 
  * cpdef tuple estimate_positive_gradient_nn(             # <<<<<<<<<<<<<<
  *     sparse_index_type[:] indices,
  *     sparse_index_type[:] indptr,
  */
-  __pyx_tuple__37 = PyTuple_Pack(9, __pyx_n_s_indices, __pyx_n_s_indptr, __pyx_n_s_P_data, __pyx_n_s_embedding, __pyx_n_s_reference_embedding, __pyx_n_s_gradient, __pyx_n_s_dof, __pyx_n_s_num_threads, __pyx_n_s_should_eval_error); if (unlikely(!__pyx_tuple__37)) __PYX_ERR(0, 103, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__37);
-  __Pyx_GIVEREF(__pyx_tuple__37);
-  __pyx_codeobj__38 = (PyObject*)__Pyx_PyCode_New(9, 0, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__37, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_openTSNE__tsne_pyx, __pyx_n_s_pyx_fuse_0estimate_positive_gr, 103, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__38)) __PYX_ERR(0, 103, __pyx_L1_error)
+  __pyx_tuple__32 = PyTuple_Pack(9, __pyx_n_s_indices, __pyx_n_s_indptr, __pyx_n_s_P_data, __pyx_n_s_embedding, __pyx_n_s_reference_embedding, __pyx_n_s_gradient, __pyx_n_s_dof, __pyx_n_s_num_threads, __pyx_n_s_should_eval_error); if (unlikely(!__pyx_tuple__32)) __PYX_ERR(0, 103, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__32);
+  __Pyx_GIVEREF(__pyx_tuple__32);
+  __pyx_codeobj__33 = (PyObject*)__Pyx_PyCode_New(9, 0, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__32, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_openTSNE__tsne_pyx, __pyx_n_s_pyx_fuse_0estimate_positive_gr, 103, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__33)) __PYX_ERR(0, 103, __pyx_L1_error)
 
   /* "View.MemoryView":287
  *         return self.name
  * 
  * cdef generic = Enum("<strided and direct or indirect>")             # <<<<<<<<<<<<<<
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")
  */
-  __pyx_tuple__39 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct_or_indirect); if (unlikely(!__pyx_tuple__39)) __PYX_ERR(2, 287, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__39);
-  __Pyx_GIVEREF(__pyx_tuple__39);
+  __pyx_tuple__34 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct_or_indirect); if (unlikely(!__pyx_tuple__34)) __PYX_ERR(2, 287, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__34);
+  __Pyx_GIVEREF(__pyx_tuple__34);
 
   /* "View.MemoryView":288
  * 
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default             # <<<<<<<<<<<<<<
  * cdef indirect = Enum("<strided and indirect>")
  * 
  */
-  __pyx_tuple__40 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct); if (unlikely(!__pyx_tuple__40)) __PYX_ERR(2, 288, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__40);
-  __Pyx_GIVEREF(__pyx_tuple__40);
+  __pyx_tuple__35 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct); if (unlikely(!__pyx_tuple__35)) __PYX_ERR(2, 288, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__35);
+  __Pyx_GIVEREF(__pyx_tuple__35);
 
   /* "View.MemoryView":289
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__41 = PyTuple_Pack(1, __pyx_kp_s_strided_and_indirect); if (unlikely(!__pyx_tuple__41)) __PYX_ERR(2, 289, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__41);
-  __Pyx_GIVEREF(__pyx_tuple__41);
+  __pyx_tuple__36 = PyTuple_Pack(1, __pyx_kp_s_strided_and_indirect); if (unlikely(!__pyx_tuple__36)) __PYX_ERR(2, 289, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__36);
+  __Pyx_GIVEREF(__pyx_tuple__36);
 
   /* "View.MemoryView":292
  * 
  * 
  * cdef contiguous = Enum("<contiguous and direct>")             # <<<<<<<<<<<<<<
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")
  * 
  */
-  __pyx_tuple__42 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_direct); if (unlikely(!__pyx_tuple__42)) __PYX_ERR(2, 292, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__42);
-  __Pyx_GIVEREF(__pyx_tuple__42);
+  __pyx_tuple__37 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_direct); if (unlikely(!__pyx_tuple__37)) __PYX_ERR(2, 292, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__37);
+  __Pyx_GIVEREF(__pyx_tuple__37);
 
   /* "View.MemoryView":293
  * 
  * cdef contiguous = Enum("<contiguous and direct>")
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__43 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_indirect); if (unlikely(!__pyx_tuple__43)) __PYX_ERR(2, 293, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__43);
-  __Pyx_GIVEREF(__pyx_tuple__43);
+  __pyx_tuple__38 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_indirect); if (unlikely(!__pyx_tuple__38)) __PYX_ERR(2, 293, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__38);
+  __Pyx_GIVEREF(__pyx_tuple__38);
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_Enum(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_tuple__44 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__44)) __PYX_ERR(2, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__44);
-  __Pyx_GIVEREF(__pyx_tuple__44);
-  __pyx_codeobj__45 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__44, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Enum, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__45)) __PYX_ERR(2, 1, __pyx_L1_error)
+  __pyx_tuple__39 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__39)) __PYX_ERR(2, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__39);
+  __Pyx_GIVEREF(__pyx_tuple__39);
+  __pyx_codeobj__40 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__39, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Enum, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__40)) __PYX_ERR(2, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -35941,37 +34445,73 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 206, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 200, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 206, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 229, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 233, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 242, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 917, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT(PyArray_Descr),
+  __Pyx_ImportType_CheckSize_Ignore);
+   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 200, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
+   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 223, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayMultiIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
+   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 227, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayObject),
+  __Pyx_ImportType_CheckSize_Ignore);
+   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 239, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 771, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 773, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 775, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 777, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 779, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 781, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 783, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 785, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 787, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 789, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT(PyUFuncObject),
+  __Pyx_ImportType_CheckSize_Ignore);
+   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 827, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("openTSNE.quad_tree"); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 23, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_8openTSNE_9quad_tree_QuadTree = __Pyx_ImportType(__pyx_t_1, "openTSNE.quad_tree", "QuadTree", sizeof(struct __pyx_obj_8openTSNE_9quad_tree_QuadTree), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_8openTSNE_9quad_tree_QuadTree = __Pyx_ImportType(__pyx_t_1, "openTSNE.quad_tree", "QuadTree", sizeof(struct __pyx_obj_8openTSNE_9quad_tree_QuadTree), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_8openTSNE_9quad_tree_QuadTree),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_8openTSNE_9quad_tree_QuadTree) __PYX_ERR(4, 23, __pyx_L1_error)
   __pyx_vtabptr_8openTSNE_9quad_tree_QuadTree = (struct __pyx_vtabstruct_8openTSNE_9quad_tree_QuadTree*)__Pyx_GetVtable(__pyx_ptype_8openTSNE_9quad_tree_QuadTree->tp_dict); if (unlikely(!__pyx_vtabptr_8openTSNE_9quad_tree_QuadTree)) __PYX_ERR(4, 23, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
@@ -36315,25 +34855,25 @@
   __pyx_k__9 = 1;
   __pyx_k__10 = 0;
   __pyx_k__8 = 1;
   __pyx_k__9 = 1;
   __pyx_k__10 = 0;
   __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 103, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_0__pyx_mdef_8openTSNE_5_tsne_19__pyx_fuse_0estimate_positive_gradient_nn, 0, __pyx_n_s_pyx_fuse_0estimate_positive_gr, NULL, __pyx_n_s_openTSNE__tsne, __pyx_d, ((PyObject *)__pyx_codeobj__38)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 103, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_0__pyx_mdef_8openTSNE_5_tsne_19__pyx_fuse_0estimate_positive_gradient_nn, 0, __pyx_n_s_pyx_fuse_0estimate_positive_gr, NULL, __pyx_n_s_openTSNE__tsne, __pyx_d, ((PyObject *)__pyx_codeobj__33)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 103, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_t_5);
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_int32_t, __pyx_t_1) < 0) __PYX_ERR(0, 103, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_1__pyx_mdef_8openTSNE_5_tsne_21__pyx_fuse_1estimate_positive_gradient_nn, 0, __pyx_n_s_pyx_fuse_1estimate_positive_gr, NULL, __pyx_n_s_openTSNE__tsne, __pyx_d, ((PyObject *)__pyx_codeobj__38)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 103, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_1__pyx_mdef_8openTSNE_5_tsne_21__pyx_fuse_1estimate_positive_gradient_nn, 0, __pyx_n_s_pyx_fuse_1estimate_positive_gr, NULL, __pyx_n_s_openTSNE__tsne, __pyx_d, ((PyObject *)__pyx_codeobj__33)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 103, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_t_5);
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_int64_t, __pyx_t_1) < 0) __PYX_ERR(0, 103, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_mdef_8openTSNE_5_tsne_3estimate_positive_gradient_nn, 0, __pyx_n_s_estimate_positive_gradient_nn, NULL, __pyx_n_s_openTSNE__tsne, __pyx_d, ((PyObject *)__pyx_codeobj__38)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 103, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_mdef_8openTSNE_5_tsne_3estimate_positive_gradient_nn, 0, __pyx_n_s_estimate_positive_gradient_nn, NULL, __pyx_n_s_openTSNE__tsne, __pyx_d, ((PyObject *)__pyx_codeobj__33)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 103, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_t_5);
   ((__pyx_FusedFunctionObject *) __pyx_t_1)->__signatures__ = __pyx_t_2;
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_t_2 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_estimate_positive_gradient_nn, __pyx_t_1) < 0) __PYX_ERR(0, 103, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
@@ -36365,71 +34905,71 @@
   /* "View.MemoryView":287
  *         return self.name
  * 
  * cdef generic = Enum("<strided and direct or indirect>")             # <<<<<<<<<<<<<<
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")
  */
-  __pyx_t_5 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__39, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 287, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__34, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 287, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_XGOTREF(generic);
   __Pyx_DECREF_SET(generic, __pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_5);
   __pyx_t_5 = 0;
 
   /* "View.MemoryView":288
  * 
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default             # <<<<<<<<<<<<<<
  * cdef indirect = Enum("<strided and indirect>")
  * 
  */
-  __pyx_t_5 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__40, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 288, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__35, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 288, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_XGOTREF(strided);
   __Pyx_DECREF_SET(strided, __pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_5);
   __pyx_t_5 = 0;
 
   /* "View.MemoryView":289
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_5 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__41, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 289, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__36, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 289, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_XGOTREF(indirect);
   __Pyx_DECREF_SET(indirect, __pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_5);
   __pyx_t_5 = 0;
 
   /* "View.MemoryView":292
  * 
  * 
  * cdef contiguous = Enum("<contiguous and direct>")             # <<<<<<<<<<<<<<
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")
  * 
  */
-  __pyx_t_5 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__42, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 292, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__37, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 292, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_XGOTREF(contiguous);
   __Pyx_DECREF_SET(contiguous, __pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_5);
   __pyx_t_5 = 0;
 
   /* "View.MemoryView":293
  * 
  * cdef contiguous = Enum("<contiguous and direct>")
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_5 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__43, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 293, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__38, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 293, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_XGOTREF(indirect_contiguous);
   __Pyx_DECREF_SET(indirect_contiguous, __pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_5);
   __pyx_t_5 = 0;
 
   /* "View.MemoryView":317
@@ -37342,28 +35882,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -37994,27 +36534,14 @@
     }
     PyErr_Format(PyExc_TypeError,
         "Argument '%.200s' has incorrect type (expected %.200s, got %.200s)",
         name, type->tp_name, Py_TYPE(obj)->tp_name);
     return 0;
 }
 
-/* ExtTypeTest */
-static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type) {
-    if (unlikely(!type)) {
-        PyErr_SetString(PyExc_SystemError, "Missing type object");
-        return 0;
-    }
-    if (likely(__Pyx_TypeCheck(obj, type)))
-        return 1;
-    PyErr_Format(PyExc_TypeError, "Cannot convert %.200s to %.200s",
-                 Py_TYPE(obj)->tp_name, type->tp_name);
-    return 0;
-}
-
 /* GetTopmostException */
 #if CYTHON_USE_EXC_INFO_STACK
 static _PyErr_StackItem *
 __Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
 {
     _PyErr_StackItem *exc_info = tstate->exc_info;
     while ((exc_info->exc_type == NULL || exc_info->exc_type == Py_None) &&
@@ -38401,14 +36928,27 @@
     return d;
 }
 static CYTHON_INLINE PyObject *__Pyx_GetAttr3(PyObject *o, PyObject *n, PyObject *d) {
     PyObject *r = __Pyx_GetAttr(o, n);
     return (likely(r)) ? r : __Pyx_GetAttr3Default(d);
 }
 
+/* ExtTypeTest */
+static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type) {
+    if (unlikely(!type)) {
+        PyErr_SetString(PyExc_SystemError, "Missing type object");
+        return 0;
+    }
+    if (likely(__Pyx_TypeCheck(obj, type)))
+        return 1;
+    PyErr_Format(PyExc_TypeError, "Cannot convert %.200s to %.200s",
+                 Py_TYPE(obj)->tp_name, type->tp_name);
+    return 0;
+}
+
 /* SwapException */
 #if CYTHON_FAST_THREAD_STATE
 static CYTHON_INLINE void __Pyx__ExceptionSwap(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
     PyObject *tmp_type, *tmp_value, *tmp_tb;
     #if CYTHON_USE_EXC_INFO_STACK
     _PyErr_StackItem *exc_info = tstate->exc_info;
     tmp_type = exc_info->exc_type;
@@ -38960,44 +37500,62 @@
     return ret;
 }
 
 /* TypeImport */
 #ifndef __PYX_HAVE_RT_ImportType
 #define __PYX_HAVE_RT_ImportType
 static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
     if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
@@ -40283,29 +38841,27 @@
     Py_XDECREF(py_code);
     Py_XDECREF(py_frame);
 }
 
 #if PY_MAJOR_VERSION < 3
 static int __Pyx_GetBuffer(PyObject *obj, Py_buffer *view, int flags) {
     if (PyObject_CheckBuffer(obj)) return PyObject_GetBuffer(obj, view, flags);
-        if (__Pyx_TypeCheck(obj, __pyx_ptype_5numpy_ndarray)) return __pyx_pw_5numpy_7ndarray_1__getbuffer__(obj, view, flags);
         if (__Pyx_TypeCheck(obj, __pyx_array_type)) return __pyx_array_getbuffer(obj, view, flags);
         if (__Pyx_TypeCheck(obj, __pyx_memoryview_type)) return __pyx_memoryview_getbuffer(obj, view, flags);
     PyErr_Format(PyExc_TypeError, "'%.200s' does not have the buffer interface", Py_TYPE(obj)->tp_name);
     return -1;
 }
 static void __Pyx_ReleaseBuffer(Py_buffer *view) {
     PyObject *obj = view->obj;
     if (!obj) return;
     if (PyObject_CheckBuffer(obj)) {
         PyBuffer_Release(view);
         return;
     }
     if ((0)) {}
-        else if (__Pyx_TypeCheck(obj, __pyx_ptype_5numpy_ndarray)) __pyx_pw_5numpy_7ndarray_3__releasebuffer__(obj, view);
     view->obj = NULL;
     Py_DECREF(obj);
 }
 #endif
 
 
 /* MemviewSliceIsContig */
@@ -42089,52 +40645,14 @@
 /* BytesContains */
   static CYTHON_INLINE int __Pyx_BytesContains(PyObject* bytes, char character) {
     const Py_ssize_t length = PyBytes_GET_SIZE(bytes);
     char* char_start = PyBytes_AS_STRING(bytes);
     return memchr(char_start, (unsigned char)character, (size_t)length) != NULL;
 }
 
-/* CIntToPy */
-  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_enum__NPY_TYPES(enum NPY_TYPES value) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const enum NPY_TYPES neg_one = (enum NPY_TYPES) -1, const_zero = (enum NPY_TYPES) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
-    const int is_unsigned = neg_one > const_zero;
-    if (is_unsigned) {
-        if (sizeof(enum NPY_TYPES) < sizeof(long)) {
-            return PyInt_FromLong((long) value);
-        } else if (sizeof(enum NPY_TYPES) <= sizeof(unsigned long)) {
-            return PyLong_FromUnsignedLong((unsigned long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(enum NPY_TYPES) <= sizeof(unsigned PY_LONG_LONG)) {
-            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
-#endif
-        }
-    } else {
-        if (sizeof(enum NPY_TYPES) <= sizeof(long)) {
-            return PyInt_FromLong((long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(enum NPY_TYPES) <= sizeof(PY_LONG_LONG)) {
-            return PyLong_FromLongLong((PY_LONG_LONG) value);
-#endif
-        }
-    }
-    {
-        int one = 1; int little = (int)*(unsigned char *)&one;
-        unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(enum NPY_TYPES),
-                                     little, !is_unsigned);
-    }
-}
-
 /* ImportNumPyArray */
   static PyObject* __Pyx__ImportNumPyArray(void) {
     PyObject *numpy_module, *ndarray_object = NULL;
     numpy_module = __Pyx_Import(__pyx_n_s_numpy, NULL, 0);
     if (likely(numpy_module)) {
         ndarray_object = PyObject_GetAttrString(numpy_module, "ndarray");
         Py_DECREF(numpy_module);
```

### Comparing `openTSNE-0.7.1/openTSNE/_tsne.pxd` & `openTSNE-1.0.0/openTSNE/_tsne.pxd`

 * *Files identical despite different names*

### Comparing `openTSNE-0.7.1/openTSNE/_tsne.pyx` & `openTSNE-1.0.0/openTSNE/_tsne.pyx`

 * *Files identical despite different names*

### Comparing `openTSNE-0.7.1/openTSNE/affinity.py` & `openTSNE-1.0.0/openTSNE/affinity.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 import scipy.sparse as sp
 
 from openTSNE import _tsne
 from openTSNE import nearest_neighbors
 from openTSNE import utils
 from openTSNE.utils import is_package_installed
 
+import warnings
+
 log = logging.getLogger(__name__)
 
 
 class Affinities:
     """Compute the affinities between samples.
 
     t-SNE takes as input an affinity matrix :math:`P`, and does not really care
@@ -75,44 +77,46 @@
     def n_samples(self):
         if self.knn_index is None:
             raise RuntimeError("`knn_index` is not set!")
         return self.knn_index.n_samples
 
 
 class PerplexityBasedNN(Affinities):
-    """Compute affinities using nearest neighbors.
+    """Compute standard, Gaussian affinities using nearest neighbors.
 
     Please see the :ref:`parameter-guide` for more information.
 
     Parameters
     ----------
     data: np.ndarray
         The data matrix.
 
     perplexity: float
         Perplexity can be thought of as the continuous :math:`k` number of
         nearest neighbors, for which t-SNE will attempt to preserve distances.
 
     method: str
         Specifies the nearest neighbor method to use. Can be ``exact``, ``annoy``,
-        ``pynndescent``, ``hnsw``, ``approx``, or ``auto`` (default). ``approx`` uses Annoy
-        if the input data matrix is not a sparse object and if Annoy supports
-        the given metric. Otherwise it uses Pynndescent. ``auto`` uses exact
-        nearest neighbors for N<1000 and the same heuristic as ``approx`` for N>=1000.
+        ``pynndescent``, ``hnsw``, ``approx``, or ``auto`` (default). ``approx``
+        uses Annoy if the input data matrix is not a sparse object and if Annoy
+        supports the given metric. Otherwise, it uses Pynndescent. ``auto`` uses
+        exact nearest neighbors for N<1000 and the same heuristic as ``approx``
+        for N>=1000.
 
     metric: Union[str, Callable]
         The metric to be used to compute affinities between points in the
         original space.
 
     metric_params: dict
         Additional keyword arguments for the metric function.
 
     symmetrize: bool
-        Symmetrize affinity matrix. Standard t-SNE symmetrizes the interactions
-        but when embedding new data, symmetrization is not performed.
+        Symmetrize the affinity matrix. During standard t-SNE optimization, the
+        affinities are symmetrized. However, when embedding new data points into
+        existing embeddings, symmetrization is not performed.
 
     n_jobs: int
         The number of threads to use while running t-SNE. This follows the
         scikit-learn convention, ``-1`` meaning all processors, ``-2`` meaning
         all but one, etc.
 
     random_state: Union[int, RandomState]
@@ -346,15 +350,15 @@
 
         return perplexity
 
 
 def get_knn_index(
     data, method, k, metric, metric_params=None, n_jobs=1, random_state=None, verbose=False
 ):
-    # If we're dealing with a precomputed distance matrix, our job is very easy
+    # If we're dealing with a precomputed distance matrix, our job is very easy,
     # so we can skip all the remaining checks
     if metric == "precomputed":
         return nearest_neighbors.PrecomputedDistanceMatrix(data, k=k)
 
     preferred_approx_method = nearest_neighbors.Annoy
     if is_package_installed("pynndescent") and (sp.issparse(data) or metric not in [
         "cosine",
@@ -416,15 +420,15 @@
 
     This method computes an approximation to P using the nearest neighbors.
 
     Parameters
     ----------
     neighbors: np.ndarray
         A `n_samples * k_neighbors` matrix containing the indices to each
-        points" nearest neighbors in descending order.
+        points' nearest neighbors in descending order.
     distances: np.ndarray
         A `n_samples * k_neighbors` matrix containing the distances to the
         neighbors at indices defined in the neighbors parameter.
     perplexities: double
         The desired perplexity of the probability distribution.
     symmetrize: bool
         Whether to symmetrize the probability matrix or not. Symmetrizing is
@@ -487,15 +491,15 @@
     elif normalization == "point-wise":
         P = sp.diags(np.asarray(1 / P.sum(axis=1)).ravel()) @ P
 
     return P
 
 
 class FixedSigmaNN(Affinities):
-    """Compute affinities using using nearest neighbors and a fixed bandwidth
+    """Compute affinities using nearest neighbors and a fixed bandwidth
     for the Gaussians in the ambient space.
 
     Using a fixed Gaussian bandwidth can enable us to find smaller clusters of
     data points than we might be able to using the automatically determined
     bandwidths using perplexity. Note however that this requires mostly trial
     and error.
 
@@ -508,30 +512,31 @@
         The bandwidth to use for the Gaussian kernels in the ambient space.
 
     k: int
         The number of nearest neighbors to consider for each kernel.
 
     method: str
         Specifies the nearest neighbor method to use. Can be ``exact``, ``annoy``,
-        ``pynndescent``, ``hnsw``, ``approx``, or ``auto`` (default). ``approx`` uses Annoy
-        if the input data matrix is not a sparse object and if Annoy supports
-        the given metric. Otherwise it uses Pynndescent. ``auto`` uses exact
-        nearest neighbors for N<1000 and the same heuristic as ``approx`` for N>=1000.
-
+        ``pynndescent``, ``hnsw``, ``approx``, or ``auto`` (default). ``approx``
+        uses Annoy if the input data matrix is not a sparse object and if Annoy
+        supports the given metric. Otherwise, it uses Pynndescent. ``auto`` uses
+        exact nearest neighbors for N<1000 and the same heuristic as ``approx``
+        for N>=1000.
 
     metric: Union[str, Callable]
         The metric to be used to compute affinities between points in the
         original space.
 
     metric_params: dict
         Additional keyword arguments for the metric function.
 
     symmetrize: bool
-        Symmetrize affinity matrix. Standard t-SNE symmetrizes the interactions
-        but when embedding new data, symmetrization is not performed.
+        Symmetrize the affinity matrix. During standard t-SNE optimization, the
+        affinities are symmetrized. However, when embedding new data points into
+        existing embeddings, symmetrization is not performed.
 
     n_jobs: int
         The number of threads to use while running t-SNE. This follows the
         scikit-learn convention, ``-1`` meaning all processors, ``-2`` meaning
         all but one, etc.
 
     random_state: Union[int, RandomState]
@@ -719,29 +724,31 @@
         A list of perplexity values, which will be used in the multiscale
         Gaussian kernel. Perplexity can be thought of as the continuous
         :math:`k` number of nearest neighbors, for which t-SNE will attempt to
         preserve distances.
 
     method: str
         Specifies the nearest neighbor method to use. Can be ``exact``, ``annoy``,
-        ``pynndescent``, ``hnsw``, ``approx``, or ``auto`` (default). ``approx`` uses Annoy
-        if the input data matrix is not a sparse object and if Annoy supports
-        the given metric. Otherwise it uses Pynndescent. ``auto`` uses exact
-        nearest neighbors for N<1000 and the same heuristic as ``approx`` for N>=1000.
+        ``pynndescent``, ``hnsw``, ``approx``, or ``auto`` (default). ``approx``
+        uses Annoy if the input data matrix is not a sparse object and if Annoy
+        supports the given metric. Otherwise, it uses Pynndescent. ``auto`` uses
+        exact nearest neighbors for N<1000 and the same heuristic as ``approx``
+        for N>=1000.
 
     metric: Union[str, Callable]
         The metric to be used to compute affinities between points in the
         original space.
 
     metric_params: dict
         Additional keyword arguments for the metric function.
 
     symmetrize: bool
-        Symmetrize affinity matrix. Standard t-SNE symmetrizes the interactions
-        but when embedding new data, symmetrization is not performed.
+        Symmetrize the affinity matrix. During standard t-SNE optimization, the
+        affinities are symmetrized. However, when embedding new data points into
+        existing embeddings, symmetrization is not performed.
 
     n_jobs: int
         The number of threads to use while running t-SNE. This follows the
         scikit-learn convention, ``-1`` meaning all processors, ``-2`` meaning
         all but one, etc.
 
     random_state: Union[int, RandomState]
@@ -1010,29 +1017,31 @@
         A list of perplexity values, which will be used in the multiscale
         Gaussian kernel. Perplexity can be thought of as the continuous
         :math:`k` number of nearest neighbors, for which t-SNE will attempt to
         preserve distances.
 
     method: str
         Specifies the nearest neighbor method to use. Can be ``exact``, ``annoy``,
-        ``pynndescent``, ``hnsw``, ``approx``, or ``auto`` (default). ``approx`` uses Annoy
-        if the input data matrix is not a sparse object and if Annoy supports
-        the given metric. Otherwise it uses Pynndescent. ``auto`` uses exact
-        nearest neighbors for N<1000 and the same heuristic as ``approx`` for N>=1000.
+        ``pynndescent``, ``hnsw``, ``approx``, or ``auto`` (default). ``approx``
+        uses Annoy if the input data matrix is not a sparse object and if Annoy
+        supports the given metric. Otherwise, it uses Pynndescent. ``auto`` uses
+        exact nearest neighbors for N<1000 and the same heuristic as ``approx``
+        for N>=1000.
 
     metric: Union[str, Callable]
         The metric to be used to compute affinities between points in the
         original space.
 
     metric_params: dict
         Additional keyword arguments for the metric function.
 
     symmetrize: bool
-        Symmetrize affinity matrix. Standard t-SNE symmetrizes the interactions
-        but when embedding new data, symmetrization is not performed.
+        Symmetrize the affinity matrix. During standard t-SNE optimization, the
+        affinities are symmetrized. However, when embedding new data points into
+        existing embeddings, symmetrization is not performed.
 
     n_jobs: int
         The number of threads to use while running t-SNE. This follows the
         scikit-learn convention, ``-1`` meaning all processors, ``-2`` meaning
         all but one, etc.
 
     random_state: Union[int, RandomState]
@@ -1082,42 +1091,52 @@
         elif normalization == "point-wise":
             P = sp.diags(np.asarray(1 / P.sum(axis=1)).ravel()) @ P
 
         return P
 
 
 class Uniform(Affinities):
-    """Compute affinities using using nearest neighbors and uniform kernel in
+    """Compute affinities using nearest neighbors and uniform kernel in
     the ambient space.
 
     Parameters
     ----------
     data: np.ndarray
         The data matrix.
 
     k_neighbors: int
 
     method: str
         Specifies the nearest neighbor method to use. Can be ``exact``, ``annoy``,
-        ``pynndescent``, ``hnsw``, ``approx``, or ``auto`` (default). ``approx`` uses Annoy
-        if the input data matrix is not a sparse object and if Annoy supports
-        the given metric. Otherwise it uses Pynndescent. ``auto`` uses exact
-        nearest neighbors for N<1000 and the same heuristic as ``approx`` for N>=1000.
-
+        ``pynndescent``, ``hnsw``, ``approx``, or ``auto`` (default). ``approx``
+        uses Annoy if the input data matrix is not a sparse object and if Annoy
+        supports the given metric. Otherwise, it uses Pynndescent. ``auto`` uses
+        exact nearest neighbors for N<1000 and the same heuristic as ``approx``
+        for N>=1000.
 
     metric: Union[str, Callable]
         The metric to be used to compute affinities between points in the
         original space.
 
     metric_params: dict
         Additional keyword arguments for the metric function.
 
-    symmetrize: bool
-        Symmetrize affinity matrix. Standard t-SNE symmetrizes the interactions
-        but when embedding new data, symmetrization is not performed.
+    symmetrize: Union[str, bool]
+        Symmetrize the affinity matrix. During standard t-SNE optimization, the
+        affinities are symmetrized. However, when embedding new data points into
+        existing embeddings, symmetrization is not performed.
+        The uniform affinity supports ``max`` and ``mean`` symmetrization, as
+        well as no symmetrization via ``none``.
+        The ``max`` symmetrization yields a binary affinity matrix with all
+        non-zero elements (corresponding to edges of the kNN graph) being the
+        same. The ``mean`` symmetrization performs symmetrization via
+        (A + A.T) / 2, resulting in the affinity matrix with two possible
+        non-zero values. Applying no symmetrization results in a non-symmetric
+        affinity matrix. We default to ``mean`` symmetrization, but the default
+        will change to ``max`` in future versions.
 
     n_jobs: int
         The number of threads to use while running t-SNE. This follows the
         scikit-learn convention, ``-1`` meaning all processors, ``-2`` meaning
         all but one, etc.
 
     random_state: Union[int, RandomState]
@@ -1184,16 +1203,32 @@
                 neighbors.ravel(),
                 range(0, n_samples * k_neighbors + 1, k_neighbors),
             ),
             shape=(n_samples, n_samples),
         )
 
         # Symmetrize the probability matrix
-        if symmetrize:
+        if symmetrize == "max":
+            P = (P + P.T > 0).astype(float)
+        elif symmetrize == "mean":
+            P = (P + P.T) / 2
+        elif symmetrize == "none" or symmetrize is False:
+            pass
+        elif symmetrize is True:
+            # Backward compatibility
             P = (P + P.T) / 2
+            warnings.warn(
+                f"Using `mean` symmetrization, but the default behaviour is going to "
+                f"change to `max` in future versions.",
+                category=FutureWarning,
+            )
+        else:
+            raise ValueError(
+                f"Symmetrization method `{symmetrize}` is not recognized."
+            )
 
         # Convert weights to probabilities
         P /= np.sum(P)
 
         self.P = P
         self.verbose = verbose
         self.n_jobs = n_jobs
@@ -1268,15 +1303,15 @@
 
 class PrecomputedAffinities(Affinities):
     """Use a precomputed affinity matrix.
 
     Parameters
     ----------
     affinities: scipy.sparse.csr_matrix, np.ndarray
-        A N x N matrix containing the affinities.
+        An N x N matrix containing the affinities.
     normalize: bool
         Normalize the affinity matrix to sum to 1. Default is True.
 
     """
 
     def __init__(self, affinities, normalize=True):
         if not isinstance(affinities, sp.csr_matrix):
```

### Comparing `openTSNE-0.7.1/openTSNE/callbacks.py` & `openTSNE-1.0.0/openTSNE/callbacks.py`

 * *Files identical despite different names*

### Comparing `openTSNE-0.7.1/openTSNE/dependencies/annoy/annoylib.h` & `openTSNE-1.0.0/openTSNE/dependencies/annoy/annoylib.h`

 * *Files identical despite different names*

### Comparing `openTSNE-0.7.1/openTSNE/dependencies/annoy/annoymodule.cc` & `openTSNE-1.0.0/openTSNE/dependencies/annoy/annoymodule.cc`

 * *Files identical despite different names*

### Comparing `openTSNE-0.7.1/openTSNE/dependencies/annoy/kissrandom.h` & `openTSNE-1.0.0/openTSNE/dependencies/annoy/kissrandom.h`

 * *Files identical despite different names*

### Comparing `openTSNE-0.7.1/openTSNE/dependencies/annoy/mman.h` & `openTSNE-1.0.0/openTSNE/dependencies/annoy/mman.h`

 * *Files identical despite different names*

### Comparing `openTSNE-0.7.1/openTSNE/initialization.py` & `openTSNE-1.0.0/openTSNE/initialization.py`

 * *Files identical despite different names*

### Comparing `openTSNE-0.7.1/openTSNE/kl_divergence.cpp` & `openTSNE-1.0.0/openTSNE/kl_divergence.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "language": "c++",
         "name": "openTSNE.kl_divergence",
@@ -19,16 +19,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_33"
-#define CYTHON_HEX_VERSION 0x001D21F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -213,15 +213,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -252,15 +252,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -768,15 +768,21 @@
 
 #define __PYX_HAVE__openTSNE__kl_divergence
 #define __PYX_HAVE_API__openTSNE__kl_divergence
 /* Early includes */
 #include <string.h>
 #include <stdio.h>
 #include "numpy/arrayobject.h"
+#include "numpy/ndarrayobject.h"
+#include "numpy/ndarraytypes.h"
+#include "numpy/arrayscalars.h"
 #include "numpy/ufuncobject.h"
+
+    /* NumPy API declarations from "numpy/__init__.pxd" */
+    
 #include "math.h"
 #include "pythread.h"
 #include <stdlib.h>
 #include "pystate.h"
 #ifdef _OPENMP
 #include <omp.h>
 #endif /* _OPENMP */
@@ -1115,195 +1121,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":775
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":690
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":776
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":691
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":777
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":778
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":693
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":782
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":697
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":783
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":698
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":784
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":785
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":700
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":789
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":704
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":790
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":705
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":799
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":714
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":800
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":715
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":801
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":716
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":803
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":804
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":805
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":720
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":807
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":722
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":808
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":723
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":810
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":811
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":812
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1335,42 +1341,42 @@
 /*--- Type declarations ---*/
 struct __pyx_obj_8openTSNE_9quad_tree_QuadTree;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":814
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":815
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":730
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":816
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":818
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":733
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -1973,34 +1979,14 @@
 /* PyObjectCallNoArg.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func);
 #else
 #define __Pyx_PyObject_CallNoArg(func) __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL)
 #endif
 
-/* RaiseException.proto */
-static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
-
-/* DictGetItem.proto */
-#if PY_MAJOR_VERSION >= 3 && !CYTHON_COMPILING_IN_PYPY
-static PyObject *__Pyx_PyDict_GetItem(PyObject *d, PyObject* key);
-#define __Pyx_PyObject_Dict_GetItem(obj, name)\
-    (likely(PyDict_CheckExact(obj)) ?\
-     __Pyx_PyDict_GetItem(obj, name) : PyObject_GetItem(obj, name))
-#else
-#define __Pyx_PyDict_GetItem(d, key) PyObject_GetItem(d, key)
-#define __Pyx_PyObject_Dict_GetItem(obj, name)  PyObject_GetItem(obj, name)
-#endif
-
-/* RaiseNoneIterError.proto */
-static CYTHON_INLINE void __Pyx_RaiseNoneNotIterableError(void);
-
-/* ExtTypeTest.proto */
-static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type);
-
 /* GetTopmostException.proto */
 #if CYTHON_USE_EXC_INFO_STACK
 static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
 #endif
 
 /* SaveResetException.proto */
 #if CYTHON_FAST_THREAD_STATE
@@ -2025,14 +2011,17 @@
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_GetException(type, value, tb)  __Pyx__GetException(__pyx_tstate, type, value, tb)
 static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
 #else
 static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb);
 #endif
 
+/* RaiseException.proto */
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
+
 /* ArgTypeTest.proto */
 #define __Pyx_ArgTypeTest(obj, type, none_allowed, name, exact)\
     ((likely((Py_TYPE(obj) == type) | (none_allowed && (obj == Py_None)))) ? 1 :\
         __Pyx__ArgTypeTest(obj, type, name, exact))
 static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact);
 
 /* PyObjectCall2Args.proto */
@@ -2111,14 +2100,20 @@
          const char* cstring, Py_ssize_t start, Py_ssize_t stop,
          const char* encoding, const char* errors,
          PyObject* (*decode_func)(const char *s, Py_ssize_t size, const char *errors));
 
 /* GetAttr3.proto */
 static CYTHON_INLINE PyObject *__Pyx_GetAttr3(PyObject *, PyObject *, PyObject *);
 
+/* RaiseNoneIterError.proto */
+static CYTHON_INLINE void __Pyx_RaiseNoneNotIterableError(void);
+
+/* ExtTypeTest.proto */
+static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type);
+
 /* SwapException.proto */
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_ExceptionSwap(type, value, tb)  __Pyx__ExceptionSwap(__pyx_tstate, type, value, tb)
 static CYTHON_INLINE void __Pyx__ExceptionSwap(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
 #else
 static CYTHON_INLINE void __Pyx_ExceptionSwap(PyObject **type, PyObject **value, PyObject **tb);
 #endif
@@ -2232,20 +2227,28 @@
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
 #ifndef __PYX_HAVE_RT_ImportType_proto
 #define __PYX_HAVE_RT_ImportType_proto
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#endif
 enum __Pyx_ImportType_CheckSize {
    __Pyx_ImportType_CheckSize_Error = 0,
    __Pyx_ImportType_CheckSize_Warn = 1,
    __Pyx_ImportType_CheckSize_Ignore = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
 #endif
 
 /* GetVTable.proto */
 static void* __Pyx_GetVtable(PyObject *dict);
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
@@ -2462,17 +2465,14 @@
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
 
-/* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_enum__NPY_TYPES(enum NPY_TYPES value);
-
 /* CIntFromPy.proto */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *);
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
 
 /* CIntFromPy.proto */
@@ -2520,16 +2520,25 @@
 /* Module declarations from 'numpy' */
 
 /* Module declarations from 'numpy' */
 static PyTypeObject *__pyx_ptype_5numpy_dtype = 0;
 static PyTypeObject *__pyx_ptype_5numpy_flatiter = 0;
 static PyTypeObject *__pyx_ptype_5numpy_broadcast = 0;
 static PyTypeObject *__pyx_ptype_5numpy_ndarray = 0;
+static PyTypeObject *__pyx_ptype_5numpy_generic = 0;
+static PyTypeObject *__pyx_ptype_5numpy_number = 0;
+static PyTypeObject *__pyx_ptype_5numpy_integer = 0;
+static PyTypeObject *__pyx_ptype_5numpy_signedinteger = 0;
+static PyTypeObject *__pyx_ptype_5numpy_unsignedinteger = 0;
+static PyTypeObject *__pyx_ptype_5numpy_inexact = 0;
+static PyTypeObject *__pyx_ptype_5numpy_floating = 0;
+static PyTypeObject *__pyx_ptype_5numpy_complexfloating = 0;
+static PyTypeObject *__pyx_ptype_5numpy_flexible = 0;
+static PyTypeObject *__pyx_ptype_5numpy_character = 0;
 static PyTypeObject *__pyx_ptype_5numpy_ufunc = 0;
-static CYTHON_INLINE char *__pyx_f_5numpy__util_dtypestring(PyArray_Descr *, char *, char *, int *); /*proto*/
 
 /* Module declarations from 'openTSNE.quad_tree' */
 static PyTypeObject *__pyx_ptype_8openTSNE_9quad_tree_QuadTree = 0;
 
 /* Module declarations from 'openTSNE._tsne' */
 static double (*__pyx_f_8openTSNE_5_tsne_estimate_negative_gradient_bh)(struct __pyx_obj_8openTSNE_9quad_tree_QuadTree *, __Pyx_memviewslice, __Pyx_memviewslice, int __pyx_skip_dispatch, struct __pyx_opt_args_8openTSNE_5_tsne_estimate_negative_gradient_bh *__pyx_optional_args); /*proto*/
 static double (*__pyx_f_8openTSNE_5_tsne_estimate_negative_gradient_fft_1d)(__Pyx_memviewslice, __Pyx_memviewslice, int __pyx_skip_dispatch, struct __pyx_opt_args_8openTSNE_5_tsne_estimate_negative_gradient_fft_1d *__pyx_optional_args); /*proto*/
@@ -2589,17 +2598,16 @@
 static __Pyx_TypeInfo __Pyx_TypeInfo_int = { "int", NULL, sizeof(int), { 0 }, 0, IS_UNSIGNED(int) ? 'U' : 'I', IS_UNSIGNED(int), 0 };
 #define __Pyx_MODULE_NAME "openTSNE.kl_divergence"
 extern int __pyx_module_is_main_openTSNE__kl_divergence;
 int __pyx_module_is_main_openTSNE__kl_divergence = 0;
 
 /* Implementation of 'openTSNE.kl_divergence' */
 static PyObject *__pyx_builtin_range;
-static PyObject *__pyx_builtin_ValueError;
-static PyObject *__pyx_builtin_RuntimeError;
 static PyObject *__pyx_builtin_ImportError;
+static PyObject *__pyx_builtin_ValueError;
 static PyObject *__pyx_builtin_MemoryError;
 static PyObject *__pyx_builtin_enumerate;
 static PyObject *__pyx_builtin_TypeError;
 static PyObject *__pyx_builtin_Ellipsis;
 static PyObject *__pyx_builtin_id;
 static PyObject *__pyx_builtin_IndexError;
 static const char __pyx_k_O[] = "O";
@@ -2664,15 +2672,14 @@
 static const char __pyx_k_ValueError[] = "ValueError";
 static const char __pyx_k_empty_like[] = "empty_like";
 static const char __pyx_k_pyx_result[] = "__pyx_result";
 static const char __pyx_k_pyx_vtable[] = "__pyx_vtable__";
 static const char __pyx_k_ImportError[] = "ImportError";
 static const char __pyx_k_MemoryError[] = "MemoryError";
 static const char __pyx_k_PickleError[] = "PickleError";
-static const char __pyx_k_RuntimeError[] = "RuntimeError";
 static const char __pyx_k_pyx_checksum[] = "__pyx_checksum";
 static const char __pyx_k_stringsource[] = "stringsource";
 static const char __pyx_k_pyx_getbuffer[] = "__pyx_getbuffer";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
 static const char __pyx_k_View_MemoryView[] = "View.MemoryView";
 static const char __pyx_k_allocate_buffer[] = "allocate_buffer";
 static const char __pyx_k_dtype_is_object[] = "dtype_is_object";
@@ -2689,64 +2696,54 @@
 static const char __pyx_k_MemoryView_of_r_object[] = "<MemoryView of %r object>";
 static const char __pyx_k_n_interpolation_points[] = "n_interpolation_points";
 static const char __pyx_k_MemoryView_of_r_at_0x_x[] = "<MemoryView of %r at 0x%x>";
 static const char __pyx_k_contiguous_and_indirect[] = "<contiguous and indirect>";
 static const char __pyx_k_Cannot_index_with_type_s[] = "Cannot index with type '%s'";
 static const char __pyx_k_Invalid_shape_in_axis_d_d[] = "Invalid shape in axis %d: %d.";
 static const char __pyx_k_itemsize_0_for_cython_array[] = "itemsize <= 0 for cython.array";
-static const char __pyx_k_ndarray_is_not_C_contiguous[] = "ndarray is not C contiguous";
 static const char __pyx_k_estimate_positive_gradient_nn[] = "estimate_positive_gradient_nn";
 static const char __pyx_k_unable_to_allocate_array_data[] = "unable to allocate array data.";
 static const char __pyx_k_strided_and_direct_or_indirect[] = "<strided and direct or indirect>";
 static const char __pyx_k_numpy_core_multiarray_failed_to[] = "numpy.core.multiarray failed to import";
-static const char __pyx_k_unknown_dtype_code_in_numpy_pxd[] = "unknown dtype code in numpy.pxd (%d)";
 static const char __pyx_k_Buffer_view_does_not_expose_stri[] = "Buffer view does not expose strides";
 static const char __pyx_k_Can_only_create_a_buffer_that_is[] = "Can only create a buffer that is contiguous in memory.";
 static const char __pyx_k_Cannot_assign_to_read_only_memor[] = "Cannot assign to read-only memoryview";
 static const char __pyx_k_Cannot_create_writable_memory_vi[] = "Cannot create writable memory view from read-only memoryview";
 static const char __pyx_k_Empty_shape_tuple_for_cython_arr[] = "Empty shape tuple for cython.array";
-static const char __pyx_k_Format_string_allocated_too_shor[] = "Format string allocated too short, see comment in numpy.pxd";
 static const char __pyx_k_Incompatible_checksums_0x_x_vs_0[] = "Incompatible checksums (0x%x vs (0xb068931, 0x82a3537, 0x6ae9995) = (name))";
 static const char __pyx_k_Indirect_dimensions_not_supporte[] = "Indirect dimensions not supported";
 static const char __pyx_k_Invalid_mode_expected_c_or_fortr[] = "Invalid mode, expected 'c' or 'fortran', got %s";
-static const char __pyx_k_Non_native_byte_order_not_suppor[] = "Non-native byte order not supported";
 static const char __pyx_k_Out_of_bounds_on_buffer_access_a[] = "Out of bounds on buffer access (axis %d)";
 static const char __pyx_k_Unable_to_convert_item_to_object[] = "Unable to convert item to object";
 static const char __pyx_k_got_differing_extents_in_dimensi[] = "got differing extents in dimension %d (got %d and %d)";
-static const char __pyx_k_ndarray_is_not_Fortran_contiguou[] = "ndarray is not Fortran contiguous";
 static const char __pyx_k_no_default___reduce___due_to_non[] = "no default __reduce__ due to non-trivial __cinit__";
 static const char __pyx_k_numpy_core_umath_failed_to_impor[] = "numpy.core.umath failed to import";
 static const char __pyx_k_unable_to_allocate_shape_and_str[] = "unable to allocate shape and strides.";
-static const char __pyx_k_Format_string_allocated_too_shor_2[] = "Format string allocated too short.";
 static PyObject *__pyx_n_s_ASCII;
 static PyObject *__pyx_kp_s_Buffer_view_does_not_expose_stri;
 static PyObject *__pyx_kp_s_Can_only_create_a_buffer_that_is;
 static PyObject *__pyx_kp_s_Cannot_assign_to_read_only_memor;
 static PyObject *__pyx_kp_s_Cannot_create_writable_memory_vi;
 static PyObject *__pyx_kp_s_Cannot_index_with_type_s;
 static PyObject *__pyx_n_s_Ellipsis;
 static PyObject *__pyx_kp_s_Empty_shape_tuple_for_cython_arr;
-static PyObject *__pyx_kp_u_Format_string_allocated_too_shor;
-static PyObject *__pyx_kp_u_Format_string_allocated_too_shor_2;
 static PyObject *__pyx_n_s_ImportError;
 static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0;
 static PyObject *__pyx_n_s_IndexError;
 static PyObject *__pyx_kp_s_Indirect_dimensions_not_supporte;
 static PyObject *__pyx_kp_s_Invalid_mode_expected_c_or_fortr;
 static PyObject *__pyx_kp_s_Invalid_shape_in_axis_d_d;
 static PyObject *__pyx_n_s_MemoryError;
 static PyObject *__pyx_kp_s_MemoryView_of_r_at_0x_x;
 static PyObject *__pyx_kp_s_MemoryView_of_r_object;
-static PyObject *__pyx_kp_u_Non_native_byte_order_not_suppor;
 static PyObject *__pyx_n_b_O;
 static PyObject *__pyx_kp_s_Out_of_bounds_on_buffer_access_a;
 static PyObject *__pyx_n_s_P;
 static PyObject *__pyx_n_s_P_data;
 static PyObject *__pyx_n_s_PickleError;
-static PyObject *__pyx_n_s_RuntimeError;
 static PyObject *__pyx_n_s_TypeError;
 static PyObject *__pyx_kp_s_Unable_to_convert_item_to_object;
 static PyObject *__pyx_n_s_ValueError;
 static PyObject *__pyx_n_s_View_MemoryView;
 static PyObject *__pyx_n_s_allocate_buffer;
 static PyObject *__pyx_n_s_base;
 static PyObject *__pyx_n_s_c;
@@ -2784,16 +2781,14 @@
 static PyObject *__pyx_n_s_main;
 static PyObject *__pyx_n_s_memview;
 static PyObject *__pyx_n_s_min_num_intervals;
 static PyObject *__pyx_n_s_mode;
 static PyObject *__pyx_n_s_n_interpolation_points;
 static PyObject *__pyx_n_s_name;
 static PyObject *__pyx_n_s_name_2;
-static PyObject *__pyx_kp_u_ndarray_is_not_C_contiguous;
-static PyObject *__pyx_kp_u_ndarray_is_not_Fortran_contiguou;
 static PyObject *__pyx_n_s_ndim;
 static PyObject *__pyx_n_s_new;
 static PyObject *__pyx_kp_s_no_default___reduce___due_to_non;
 static PyObject *__pyx_n_s_np;
 static PyObject *__pyx_n_s_numpy;
 static PyObject *__pyx_kp_u_numpy_core_multiarray_failed_to;
 static PyObject *__pyx_kp_u_numpy_core_umath_failed_to_impor;
@@ -2827,22 +2822,19 @@
 static PyObject *__pyx_kp_s_stringsource;
 static PyObject *__pyx_n_s_struct;
 static PyObject *__pyx_n_s_test;
 static PyObject *__pyx_n_s_theta;
 static PyObject *__pyx_n_s_tsne;
 static PyObject *__pyx_kp_s_unable_to_allocate_array_data;
 static PyObject *__pyx_kp_s_unable_to_allocate_shape_and_str;
-static PyObject *__pyx_kp_u_unknown_dtype_code_in_numpy_pxd;
 static PyObject *__pyx_n_s_unpack;
 static PyObject *__pyx_n_s_update;
 static PyObject *__pyx_pf_8openTSNE_13kl_divergence_kl_divergence_exact(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_P, __Pyx_memviewslice __pyx_v_embedding); /* proto */
 static PyObject *__pyx_pf_8openTSNE_13kl_divergence_2kl_divergence_approx_bh(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_indices, __Pyx_memviewslice __pyx_v_indptr, __Pyx_memviewslice __pyx_v_P_data, __Pyx_memviewslice __pyx_v_embedding, double __pyx_v_theta, double __pyx_v_dof); /* proto */
 static PyObject *__pyx_pf_8openTSNE_13kl_divergence_4kl_divergence_approx_fft(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_indices, __Pyx_memviewslice __pyx_v_indptr, __Pyx_memviewslice __pyx_v_P_data, __Pyx_memviewslice __pyx_v_embedding, double __pyx_v_dof, Py_ssize_t __pyx_v_n_interpolation_points, Py_ssize_t __pyx_v_min_num_intervals, double __pyx_v_ints_in_interval); /* proto */
-static int __pyx_pf_5numpy_7ndarray___getbuffer__(PyArrayObject *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags); /* proto */
-static void __pyx_pf_5numpy_7ndarray_2__releasebuffer__(PyArrayObject *__pyx_v_self, Py_buffer *__pyx_v_info); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array___cinit__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_shape, Py_ssize_t __pyx_v_itemsize, PyObject *__pyx_v_format, PyObject *__pyx_v_mode, int __pyx_v_allocate_buffer); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array_2__getbuffer__(struct __pyx_array_obj *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags); /* proto */
 static void __pyx_array___pyx_pf_15View_dot_MemoryView_5array_4__dealloc__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_15View_dot_MemoryView_5array_7memview___get__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static Py_ssize_t __pyx_array___pyx_pf_15View_dot_MemoryView_5array_6__len__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_array___pyx_pf_15View_dot_MemoryView_5array_8__getattr__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_attr); /* proto */
 static PyObject *__pyx_array___pyx_pf_15View_dot_MemoryView_5array_10__getitem__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_item); /* proto */
@@ -2896,38 +2888,33 @@
 static PyObject *__pyx_tuple__3;
 static PyObject *__pyx_tuple__4;
 static PyObject *__pyx_tuple__5;
 static PyObject *__pyx_tuple__6;
 static PyObject *__pyx_tuple__7;
 static PyObject *__pyx_tuple__8;
 static PyObject *__pyx_tuple__9;
-static PyObject *__pyx_slice__22;
+static PyObject *__pyx_slice__17;
 static PyObject *__pyx_tuple__10;
 static PyObject *__pyx_tuple__11;
 static PyObject *__pyx_tuple__12;
 static PyObject *__pyx_tuple__13;
 static PyObject *__pyx_tuple__14;
 static PyObject *__pyx_tuple__15;
 static PyObject *__pyx_tuple__16;
-static PyObject *__pyx_tuple__17;
 static PyObject *__pyx_tuple__18;
 static PyObject *__pyx_tuple__19;
 static PyObject *__pyx_tuple__20;
 static PyObject *__pyx_tuple__21;
+static PyObject *__pyx_tuple__22;
 static PyObject *__pyx_tuple__23;
 static PyObject *__pyx_tuple__24;
 static PyObject *__pyx_tuple__25;
 static PyObject *__pyx_tuple__26;
 static PyObject *__pyx_tuple__27;
-static PyObject *__pyx_tuple__28;
-static PyObject *__pyx_tuple__29;
-static PyObject *__pyx_tuple__30;
-static PyObject *__pyx_tuple__31;
-static PyObject *__pyx_tuple__32;
-static PyObject *__pyx_codeobj__33;
+static PyObject *__pyx_codeobj__28;
 /* Late includes */
 
 /* "openTSNE/kl_divergence.pyx":25
  * 
  * 
  * cdef sqeuclidean(double[:] x, double[:] y):             # <<<<<<<<<<<<<<
  *     cdef:
@@ -4588,874 +4575,15 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_P_data, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_embedding, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":258
- *         # experimental exception made for __getbuffer__ and __releasebuffer__
- *         # -- the details of this may change.
- *         def __getbuffer__(ndarray self, Py_buffer* info, int flags):             # <<<<<<<<<<<<<<
- *             # This implementation of getbuffer is geared towards Cython
- *             # requirements, and does not yet fulfill the PEP.
- */
-
-/* Python wrapper */
-static CYTHON_UNUSED int __pyx_pw_5numpy_7ndarray_1__getbuffer__(PyObject *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags); /*proto*/
-static CYTHON_UNUSED int __pyx_pw_5numpy_7ndarray_1__getbuffer__(PyObject *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__getbuffer__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_5numpy_7ndarray___getbuffer__(((PyArrayObject *)__pyx_v_self), ((Py_buffer *)__pyx_v_info), ((int)__pyx_v_flags));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static int __pyx_pf_5numpy_7ndarray___getbuffer__(PyArrayObject *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags) {
-  int __pyx_v_i;
-  int __pyx_v_ndim;
-  int __pyx_v_endian_detector;
-  int __pyx_v_little_endian;
-  int __pyx_v_t;
-  char *__pyx_v_f;
-  PyArray_Descr *__pyx_v_descr = 0;
-  int __pyx_v_offset;
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  int __pyx_t_2;
-  PyObject *__pyx_t_3 = NULL;
-  int __pyx_t_4;
-  int __pyx_t_5;
-  int __pyx_t_6;
-  PyArray_Descr *__pyx_t_7;
-  PyObject *__pyx_t_8 = NULL;
-  char *__pyx_t_9;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  if (__pyx_v_info == NULL) {
-    PyErr_SetString(PyExc_BufferError, "PyObject_GetBuffer: view==NULL argument is obsolete");
-    return -1;
-  }
-  __Pyx_RefNannySetupContext("__getbuffer__", 0);
-  __pyx_v_info->obj = Py_None; __Pyx_INCREF(Py_None);
-  __Pyx_GIVEREF(__pyx_v_info->obj);
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":265
- * 
- *             cdef int i, ndim
- *             cdef int endian_detector = 1             # <<<<<<<<<<<<<<
- *             cdef bint little_endian = ((<char*>&endian_detector)[0] != 0)
- * 
- */
-  __pyx_v_endian_detector = 1;
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":266
- *             cdef int i, ndim
- *             cdef int endian_detector = 1
- *             cdef bint little_endian = ((<char*>&endian_detector)[0] != 0)             # <<<<<<<<<<<<<<
- * 
- *             ndim = PyArray_NDIM(self)
- */
-  __pyx_v_little_endian = ((((char *)(&__pyx_v_endian_detector))[0]) != 0);
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":268
- *             cdef bint little_endian = ((<char*>&endian_detector)[0] != 0)
- * 
- *             ndim = PyArray_NDIM(self)             # <<<<<<<<<<<<<<
- * 
- *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)
- */
-  __pyx_v_ndim = PyArray_NDIM(__pyx_v_self);
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":270
- *             ndim = PyArray_NDIM(self)
- * 
- *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)             # <<<<<<<<<<<<<<
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_C_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not C contiguous")
- */
-  __pyx_t_2 = (((__pyx_v_flags & PyBUF_C_CONTIGUOUS) == PyBUF_C_CONTIGUOUS) != 0);
-  if (__pyx_t_2) {
-  } else {
-    __pyx_t_1 = __pyx_t_2;
-    goto __pyx_L4_bool_binop_done;
-  }
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":271
- * 
- *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_C_CONTIGUOUS)):             # <<<<<<<<<<<<<<
- *                 raise ValueError(u"ndarray is not C contiguous")
- * 
- */
-  __pyx_t_2 = ((!(PyArray_CHKFLAGS(__pyx_v_self, NPY_ARRAY_C_CONTIGUOUS) != 0)) != 0);
-  __pyx_t_1 = __pyx_t_2;
-  __pyx_L4_bool_binop_done:;
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":270
- *             ndim = PyArray_NDIM(self)
- * 
- *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)             # <<<<<<<<<<<<<<
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_C_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not C contiguous")
- */
-  if (unlikely(__pyx_t_1)) {
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":272
- *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_C_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not C contiguous")             # <<<<<<<<<<<<<<
- * 
- *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)
- */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 272, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(1, 272, __pyx_L1_error)
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":270
- *             ndim = PyArray_NDIM(self)
- * 
- *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)             # <<<<<<<<<<<<<<
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_C_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not C contiguous")
- */
-  }
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":274
- *                 raise ValueError(u"ndarray is not C contiguous")
- * 
- *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)             # <<<<<<<<<<<<<<
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_F_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not Fortran contiguous")
- */
-  __pyx_t_2 = (((__pyx_v_flags & PyBUF_F_CONTIGUOUS) == PyBUF_F_CONTIGUOUS) != 0);
-  if (__pyx_t_2) {
-  } else {
-    __pyx_t_1 = __pyx_t_2;
-    goto __pyx_L7_bool_binop_done;
-  }
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":275
- * 
- *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_F_CONTIGUOUS)):             # <<<<<<<<<<<<<<
- *                 raise ValueError(u"ndarray is not Fortran contiguous")
- * 
- */
-  __pyx_t_2 = ((!(PyArray_CHKFLAGS(__pyx_v_self, NPY_ARRAY_F_CONTIGUOUS) != 0)) != 0);
-  __pyx_t_1 = __pyx_t_2;
-  __pyx_L7_bool_binop_done:;
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":274
- *                 raise ValueError(u"ndarray is not C contiguous")
- * 
- *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)             # <<<<<<<<<<<<<<
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_F_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not Fortran contiguous")
- */
-  if (unlikely(__pyx_t_1)) {
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":276
- *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_F_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not Fortran contiguous")             # <<<<<<<<<<<<<<
- * 
- *             info.buf = PyArray_DATA(self)
- */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 276, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(1, 276, __pyx_L1_error)
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":274
- *                 raise ValueError(u"ndarray is not C contiguous")
- * 
- *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)             # <<<<<<<<<<<<<<
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_F_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not Fortran contiguous")
- */
-  }
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":278
- *                 raise ValueError(u"ndarray is not Fortran contiguous")
- * 
- *             info.buf = PyArray_DATA(self)             # <<<<<<<<<<<<<<
- *             info.ndim = ndim
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
- */
-  __pyx_v_info->buf = PyArray_DATA(__pyx_v_self);
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":279
- * 
- *             info.buf = PyArray_DATA(self)
- *             info.ndim = ndim             # <<<<<<<<<<<<<<
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
- *                 # Allocate new buffer for strides and shape info.
- */
-  __pyx_v_info->ndim = __pyx_v_ndim;
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":280
- *             info.buf = PyArray_DATA(self)
- *             info.ndim = ndim
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):             # <<<<<<<<<<<<<<
- *                 # Allocate new buffer for strides and shape info.
- *                 # This is allocated as one block, strides first.
- */
-  __pyx_t_1 = (((sizeof(npy_intp)) != (sizeof(Py_ssize_t))) != 0);
-  if (__pyx_t_1) {
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":283
- *                 # Allocate new buffer for strides and shape info.
- *                 # This is allocated as one block, strides first.
- *                 info.strides = <Py_ssize_t*>PyObject_Malloc(sizeof(Py_ssize_t) * 2 * <size_t>ndim)             # <<<<<<<<<<<<<<
- *                 info.shape = info.strides + ndim
- *                 for i in range(ndim):
- */
-    __pyx_v_info->strides = ((Py_ssize_t *)PyObject_Malloc((((sizeof(Py_ssize_t)) * 2) * ((size_t)__pyx_v_ndim))));
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":284
- *                 # This is allocated as one block, strides first.
- *                 info.strides = <Py_ssize_t*>PyObject_Malloc(sizeof(Py_ssize_t) * 2 * <size_t>ndim)
- *                 info.shape = info.strides + ndim             # <<<<<<<<<<<<<<
- *                 for i in range(ndim):
- *                     info.strides[i] = PyArray_STRIDES(self)[i]
- */
-    __pyx_v_info->shape = (__pyx_v_info->strides + __pyx_v_ndim);
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":285
- *                 info.strides = <Py_ssize_t*>PyObject_Malloc(sizeof(Py_ssize_t) * 2 * <size_t>ndim)
- *                 info.shape = info.strides + ndim
- *                 for i in range(ndim):             # <<<<<<<<<<<<<<
- *                     info.strides[i] = PyArray_STRIDES(self)[i]
- *                     info.shape[i] = PyArray_DIMS(self)[i]
- */
-    __pyx_t_4 = __pyx_v_ndim;
-    __pyx_t_5 = __pyx_t_4;
-    for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
-      __pyx_v_i = __pyx_t_6;
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":286
- *                 info.shape = info.strides + ndim
- *                 for i in range(ndim):
- *                     info.strides[i] = PyArray_STRIDES(self)[i]             # <<<<<<<<<<<<<<
- *                     info.shape[i] = PyArray_DIMS(self)[i]
- *             else:
- */
-      (__pyx_v_info->strides[__pyx_v_i]) = (PyArray_STRIDES(__pyx_v_self)[__pyx_v_i]);
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":287
- *                 for i in range(ndim):
- *                     info.strides[i] = PyArray_STRIDES(self)[i]
- *                     info.shape[i] = PyArray_DIMS(self)[i]             # <<<<<<<<<<<<<<
- *             else:
- *                 info.strides = <Py_ssize_t*>PyArray_STRIDES(self)
- */
-      (__pyx_v_info->shape[__pyx_v_i]) = (PyArray_DIMS(__pyx_v_self)[__pyx_v_i]);
-    }
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":280
- *             info.buf = PyArray_DATA(self)
- *             info.ndim = ndim
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):             # <<<<<<<<<<<<<<
- *                 # Allocate new buffer for strides and shape info.
- *                 # This is allocated as one block, strides first.
- */
-    goto __pyx_L9;
-  }
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":289
- *                     info.shape[i] = PyArray_DIMS(self)[i]
- *             else:
- *                 info.strides = <Py_ssize_t*>PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
- *                 info.shape = <Py_ssize_t*>PyArray_DIMS(self)
- *             info.suboffsets = NULL
- */
-  /*else*/ {
-    __pyx_v_info->strides = ((Py_ssize_t *)PyArray_STRIDES(__pyx_v_self));
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":290
- *             else:
- *                 info.strides = <Py_ssize_t*>PyArray_STRIDES(self)
- *                 info.shape = <Py_ssize_t*>PyArray_DIMS(self)             # <<<<<<<<<<<<<<
- *             info.suboffsets = NULL
- *             info.itemsize = PyArray_ITEMSIZE(self)
- */
-    __pyx_v_info->shape = ((Py_ssize_t *)PyArray_DIMS(__pyx_v_self));
-  }
-  __pyx_L9:;
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":291
- *                 info.strides = <Py_ssize_t*>PyArray_STRIDES(self)
- *                 info.shape = <Py_ssize_t*>PyArray_DIMS(self)
- *             info.suboffsets = NULL             # <<<<<<<<<<<<<<
- *             info.itemsize = PyArray_ITEMSIZE(self)
- *             info.readonly = not PyArray_ISWRITEABLE(self)
- */
-  __pyx_v_info->suboffsets = NULL;
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":292
- *                 info.shape = <Py_ssize_t*>PyArray_DIMS(self)
- *             info.suboffsets = NULL
- *             info.itemsize = PyArray_ITEMSIZE(self)             # <<<<<<<<<<<<<<
- *             info.readonly = not PyArray_ISWRITEABLE(self)
- * 
- */
-  __pyx_v_info->itemsize = PyArray_ITEMSIZE(__pyx_v_self);
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":293
- *             info.suboffsets = NULL
- *             info.itemsize = PyArray_ITEMSIZE(self)
- *             info.readonly = not PyArray_ISWRITEABLE(self)             # <<<<<<<<<<<<<<
- * 
- *             cdef int t
- */
-  __pyx_v_info->readonly = (!(PyArray_ISWRITEABLE(__pyx_v_self) != 0));
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":296
- * 
- *             cdef int t
- *             cdef char* f = NULL             # <<<<<<<<<<<<<<
- *             cdef dtype descr = <dtype>PyArray_DESCR(self)
- *             cdef int offset
- */
-  __pyx_v_f = NULL;
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":297
- *             cdef int t
- *             cdef char* f = NULL
- *             cdef dtype descr = <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
- *             cdef int offset
- * 
- */
-  __pyx_t_7 = PyArray_DESCR(__pyx_v_self);
-  __pyx_t_3 = ((PyObject *)__pyx_t_7);
-  __Pyx_INCREF(__pyx_t_3);
-  __pyx_v_descr = ((PyArray_Descr *)__pyx_t_3);
-  __pyx_t_3 = 0;
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":300
- *             cdef int offset
- * 
- *             info.obj = self             # <<<<<<<<<<<<<<
- * 
- *             if not PyDataType_HASFIELDS(descr):
- */
-  __Pyx_INCREF(((PyObject *)__pyx_v_self));
-  __Pyx_GIVEREF(((PyObject *)__pyx_v_self));
-  __Pyx_GOTREF(__pyx_v_info->obj);
-  __Pyx_DECREF(__pyx_v_info->obj);
-  __pyx_v_info->obj = ((PyObject *)__pyx_v_self);
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":302
- *             info.obj = self
- * 
- *             if not PyDataType_HASFIELDS(descr):             # <<<<<<<<<<<<<<
- *                 t = descr.type_num
- *                 if ((descr.byteorder == c'>' and little_endian) or
- */
-  __pyx_t_1 = ((!(PyDataType_HASFIELDS(__pyx_v_descr) != 0)) != 0);
-  if (__pyx_t_1) {
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":303
- * 
- *             if not PyDataType_HASFIELDS(descr):
- *                 t = descr.type_num             # <<<<<<<<<<<<<<
- *                 if ((descr.byteorder == c'>' and little_endian) or
- *                     (descr.byteorder == c'<' and not little_endian)):
- */
-    __pyx_t_4 = __pyx_v_descr->type_num;
-    __pyx_v_t = __pyx_t_4;
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":304
- *             if not PyDataType_HASFIELDS(descr):
- *                 t = descr.type_num
- *                 if ((descr.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
- *                     (descr.byteorder == c'<' and not little_endian)):
- *                     raise ValueError(u"Non-native byte order not supported")
- */
-    __pyx_t_2 = ((__pyx_v_descr->byteorder == '>') != 0);
-    if (!__pyx_t_2) {
-      goto __pyx_L15_next_or;
-    } else {
-    }
-    __pyx_t_2 = (__pyx_v_little_endian != 0);
-    if (!__pyx_t_2) {
-    } else {
-      __pyx_t_1 = __pyx_t_2;
-      goto __pyx_L14_bool_binop_done;
-    }
-    __pyx_L15_next_or:;
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":305
- *                 t = descr.type_num
- *                 if ((descr.byteorder == c'>' and little_endian) or
- *                     (descr.byteorder == c'<' and not little_endian)):             # <<<<<<<<<<<<<<
- *                     raise ValueError(u"Non-native byte order not supported")
- *                 if   t == NPY_BYTE:        f = "b"
- */
-    __pyx_t_2 = ((__pyx_v_descr->byteorder == '<') != 0);
-    if (__pyx_t_2) {
-    } else {
-      __pyx_t_1 = __pyx_t_2;
-      goto __pyx_L14_bool_binop_done;
-    }
-    __pyx_t_2 = ((!(__pyx_v_little_endian != 0)) != 0);
-    __pyx_t_1 = __pyx_t_2;
-    __pyx_L14_bool_binop_done:;
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":304
- *             if not PyDataType_HASFIELDS(descr):
- *                 t = descr.type_num
- *                 if ((descr.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
- *                     (descr.byteorder == c'<' and not little_endian)):
- *                     raise ValueError(u"Non-native byte order not supported")
- */
-    if (unlikely(__pyx_t_1)) {
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":306
- *                 if ((descr.byteorder == c'>' and little_endian) or
- *                     (descr.byteorder == c'<' and not little_endian)):
- *                     raise ValueError(u"Non-native byte order not supported")             # <<<<<<<<<<<<<<
- *                 if   t == NPY_BYTE:        f = "b"
- *                 elif t == NPY_UBYTE:       f = "B"
- */
-      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 306, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __PYX_ERR(1, 306, __pyx_L1_error)
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":304
- *             if not PyDataType_HASFIELDS(descr):
- *                 t = descr.type_num
- *                 if ((descr.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
- *                     (descr.byteorder == c'<' and not little_endian)):
- *                     raise ValueError(u"Non-native byte order not supported")
- */
-    }
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":307
- *                     (descr.byteorder == c'<' and not little_endian)):
- *                     raise ValueError(u"Non-native byte order not supported")
- *                 if   t == NPY_BYTE:        f = "b"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_UBYTE:       f = "B"
- *                 elif t == NPY_SHORT:       f = "h"
- */
-    switch (__pyx_v_t) {
-      case NPY_BYTE:
-      __pyx_v_f = ((char *)"b");
-      break;
-      case NPY_UBYTE:
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":308
- *                     raise ValueError(u"Non-native byte order not supported")
- *                 if   t == NPY_BYTE:        f = "b"
- *                 elif t == NPY_UBYTE:       f = "B"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_SHORT:       f = "h"
- *                 elif t == NPY_USHORT:      f = "H"
- */
-      __pyx_v_f = ((char *)"B");
-      break;
-      case NPY_SHORT:
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":309
- *                 if   t == NPY_BYTE:        f = "b"
- *                 elif t == NPY_UBYTE:       f = "B"
- *                 elif t == NPY_SHORT:       f = "h"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_USHORT:      f = "H"
- *                 elif t == NPY_INT:         f = "i"
- */
-      __pyx_v_f = ((char *)"h");
-      break;
-      case NPY_USHORT:
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":310
- *                 elif t == NPY_UBYTE:       f = "B"
- *                 elif t == NPY_SHORT:       f = "h"
- *                 elif t == NPY_USHORT:      f = "H"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_INT:         f = "i"
- *                 elif t == NPY_UINT:        f = "I"
- */
-      __pyx_v_f = ((char *)"H");
-      break;
-      case NPY_INT:
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":311
- *                 elif t == NPY_SHORT:       f = "h"
- *                 elif t == NPY_USHORT:      f = "H"
- *                 elif t == NPY_INT:         f = "i"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_UINT:        f = "I"
- *                 elif t == NPY_LONG:        f = "l"
- */
-      __pyx_v_f = ((char *)"i");
-      break;
-      case NPY_UINT:
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":312
- *                 elif t == NPY_USHORT:      f = "H"
- *                 elif t == NPY_INT:         f = "i"
- *                 elif t == NPY_UINT:        f = "I"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_LONG:        f = "l"
- *                 elif t == NPY_ULONG:       f = "L"
- */
-      __pyx_v_f = ((char *)"I");
-      break;
-      case NPY_LONG:
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":313
- *                 elif t == NPY_INT:         f = "i"
- *                 elif t == NPY_UINT:        f = "I"
- *                 elif t == NPY_LONG:        f = "l"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_ULONG:       f = "L"
- *                 elif t == NPY_LONGLONG:    f = "q"
- */
-      __pyx_v_f = ((char *)"l");
-      break;
-      case NPY_ULONG:
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":314
- *                 elif t == NPY_UINT:        f = "I"
- *                 elif t == NPY_LONG:        f = "l"
- *                 elif t == NPY_ULONG:       f = "L"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_LONGLONG:    f = "q"
- *                 elif t == NPY_ULONGLONG:   f = "Q"
- */
-      __pyx_v_f = ((char *)"L");
-      break;
-      case NPY_LONGLONG:
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":315
- *                 elif t == NPY_LONG:        f = "l"
- *                 elif t == NPY_ULONG:       f = "L"
- *                 elif t == NPY_LONGLONG:    f = "q"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_ULONGLONG:   f = "Q"
- *                 elif t == NPY_FLOAT:       f = "f"
- */
-      __pyx_v_f = ((char *)"q");
-      break;
-      case NPY_ULONGLONG:
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":316
- *                 elif t == NPY_ULONG:       f = "L"
- *                 elif t == NPY_LONGLONG:    f = "q"
- *                 elif t == NPY_ULONGLONG:   f = "Q"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_FLOAT:       f = "f"
- *                 elif t == NPY_DOUBLE:      f = "d"
- */
-      __pyx_v_f = ((char *)"Q");
-      break;
-      case NPY_FLOAT:
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":317
- *                 elif t == NPY_LONGLONG:    f = "q"
- *                 elif t == NPY_ULONGLONG:   f = "Q"
- *                 elif t == NPY_FLOAT:       f = "f"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_DOUBLE:      f = "d"
- *                 elif t == NPY_LONGDOUBLE:  f = "g"
- */
-      __pyx_v_f = ((char *)"f");
-      break;
-      case NPY_DOUBLE:
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":318
- *                 elif t == NPY_ULONGLONG:   f = "Q"
- *                 elif t == NPY_FLOAT:       f = "f"
- *                 elif t == NPY_DOUBLE:      f = "d"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_LONGDOUBLE:  f = "g"
- *                 elif t == NPY_CFLOAT:      f = "Zf"
- */
-      __pyx_v_f = ((char *)"d");
-      break;
-      case NPY_LONGDOUBLE:
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":319
- *                 elif t == NPY_FLOAT:       f = "f"
- *                 elif t == NPY_DOUBLE:      f = "d"
- *                 elif t == NPY_LONGDOUBLE:  f = "g"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_CFLOAT:      f = "Zf"
- *                 elif t == NPY_CDOUBLE:     f = "Zd"
- */
-      __pyx_v_f = ((char *)"g");
-      break;
-      case NPY_CFLOAT:
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":320
- *                 elif t == NPY_DOUBLE:      f = "d"
- *                 elif t == NPY_LONGDOUBLE:  f = "g"
- *                 elif t == NPY_CFLOAT:      f = "Zf"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_CDOUBLE:     f = "Zd"
- *                 elif t == NPY_CLONGDOUBLE: f = "Zg"
- */
-      __pyx_v_f = ((char *)"Zf");
-      break;
-      case NPY_CDOUBLE:
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":321
- *                 elif t == NPY_LONGDOUBLE:  f = "g"
- *                 elif t == NPY_CFLOAT:      f = "Zf"
- *                 elif t == NPY_CDOUBLE:     f = "Zd"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_CLONGDOUBLE: f = "Zg"
- *                 elif t == NPY_OBJECT:      f = "O"
- */
-      __pyx_v_f = ((char *)"Zd");
-      break;
-      case NPY_CLONGDOUBLE:
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":322
- *                 elif t == NPY_CFLOAT:      f = "Zf"
- *                 elif t == NPY_CDOUBLE:     f = "Zd"
- *                 elif t == NPY_CLONGDOUBLE: f = "Zg"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_OBJECT:      f = "O"
- *                 else:
- */
-      __pyx_v_f = ((char *)"Zg");
-      break;
-      case NPY_OBJECT:
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":323
- *                 elif t == NPY_CDOUBLE:     f = "Zd"
- *                 elif t == NPY_CLONGDOUBLE: f = "Zg"
- *                 elif t == NPY_OBJECT:      f = "O"             # <<<<<<<<<<<<<<
- *                 else:
- *                     raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)
- */
-      __pyx_v_f = ((char *)"O");
-      break;
-      default:
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":325
- *                 elif t == NPY_OBJECT:      f = "O"
- *                 else:
- *                     raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)             # <<<<<<<<<<<<<<
- *                 info.format = f
- *                 return
- */
-      __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_t); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 325, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_8 = PyUnicode_Format(__pyx_kp_u_unknown_dtype_code_in_numpy_pxd, __pyx_t_3); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 325, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 325, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __PYX_ERR(1, 325, __pyx_L1_error)
-      break;
-    }
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":326
- *                 else:
- *                     raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)
- *                 info.format = f             # <<<<<<<<<<<<<<
- *                 return
- *             else:
- */
-    __pyx_v_info->format = __pyx_v_f;
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":327
- *                     raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)
- *                 info.format = f
- *                 return             # <<<<<<<<<<<<<<
- *             else:
- *                 info.format = <char*>PyObject_Malloc(_buffer_format_string_len)
- */
-    __pyx_r = 0;
-    goto __pyx_L0;
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":302
- *             info.obj = self
- * 
- *             if not PyDataType_HASFIELDS(descr):             # <<<<<<<<<<<<<<
- *                 t = descr.type_num
- *                 if ((descr.byteorder == c'>' and little_endian) or
- */
-  }
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":329
- *                 return
- *             else:
- *                 info.format = <char*>PyObject_Malloc(_buffer_format_string_len)             # <<<<<<<<<<<<<<
- *                 info.format[0] = c'^' # Native data types, manual alignment
- *                 offset = 0
- */
-  /*else*/ {
-    __pyx_v_info->format = ((char *)PyObject_Malloc(0xFF));
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":330
- *             else:
- *                 info.format = <char*>PyObject_Malloc(_buffer_format_string_len)
- *                 info.format[0] = c'^' # Native data types, manual alignment             # <<<<<<<<<<<<<<
- *                 offset = 0
- *                 f = _util_dtypestring(descr, info.format + 1,
- */
-    (__pyx_v_info->format[0]) = '^';
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":331
- *                 info.format = <char*>PyObject_Malloc(_buffer_format_string_len)
- *                 info.format[0] = c'^' # Native data types, manual alignment
- *                 offset = 0             # <<<<<<<<<<<<<<
- *                 f = _util_dtypestring(descr, info.format + 1,
- *                                       info.format + _buffer_format_string_len,
- */
-    __pyx_v_offset = 0;
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":332
- *                 info.format[0] = c'^' # Native data types, manual alignment
- *                 offset = 0
- *                 f = _util_dtypestring(descr, info.format + 1,             # <<<<<<<<<<<<<<
- *                                       info.format + _buffer_format_string_len,
- *                                       &offset)
- */
-    __pyx_t_9 = __pyx_f_5numpy__util_dtypestring(__pyx_v_descr, (__pyx_v_info->format + 1), (__pyx_v_info->format + 0xFF), (&__pyx_v_offset)); if (unlikely(__pyx_t_9 == ((char *)NULL))) __PYX_ERR(1, 332, __pyx_L1_error)
-    __pyx_v_f = __pyx_t_9;
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":335
- *                                       info.format + _buffer_format_string_len,
- *                                       &offset)
- *                 f[0] = c'\0' # Terminate format string             # <<<<<<<<<<<<<<
- * 
- *         def __releasebuffer__(ndarray self, Py_buffer* info):
- */
-    (__pyx_v_f[0]) = '\x00';
-  }
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":258
- *         # experimental exception made for __getbuffer__ and __releasebuffer__
- *         # -- the details of this may change.
- *         def __getbuffer__(ndarray self, Py_buffer* info, int flags):             # <<<<<<<<<<<<<<
- *             # This implementation of getbuffer is geared towards Cython
- *             # requirements, and does not yet fulfill the PEP.
- */
-
-  /* function exit code */
-  __pyx_r = 0;
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_8);
-  __Pyx_AddTraceback("numpy.ndarray.__getbuffer__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = -1;
-  if (__pyx_v_info->obj != NULL) {
-    __Pyx_GOTREF(__pyx_v_info->obj);
-    __Pyx_DECREF(__pyx_v_info->obj); __pyx_v_info->obj = 0;
-  }
-  goto __pyx_L2;
-  __pyx_L0:;
-  if (__pyx_v_info->obj == Py_None) {
-    __Pyx_GOTREF(__pyx_v_info->obj);
-    __Pyx_DECREF(__pyx_v_info->obj); __pyx_v_info->obj = 0;
-  }
-  __pyx_L2:;
-  __Pyx_XDECREF((PyObject *)__pyx_v_descr);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":337
- *                 f[0] = c'\0' # Terminate format string
- * 
- *         def __releasebuffer__(ndarray self, Py_buffer* info):             # <<<<<<<<<<<<<<
- *             if PyArray_HASFIELDS(self):
- *                 PyObject_Free(info.format)
- */
-
-/* Python wrapper */
-static CYTHON_UNUSED void __pyx_pw_5numpy_7ndarray_3__releasebuffer__(PyObject *__pyx_v_self, Py_buffer *__pyx_v_info); /*proto*/
-static CYTHON_UNUSED void __pyx_pw_5numpy_7ndarray_3__releasebuffer__(PyObject *__pyx_v_self, Py_buffer *__pyx_v_info) {
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__releasebuffer__ (wrapper)", 0);
-  __pyx_pf_5numpy_7ndarray_2__releasebuffer__(((PyArrayObject *)__pyx_v_self), ((Py_buffer *)__pyx_v_info));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-}
-
-static void __pyx_pf_5numpy_7ndarray_2__releasebuffer__(PyArrayObject *__pyx_v_self, Py_buffer *__pyx_v_info) {
-  __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  __Pyx_RefNannySetupContext("__releasebuffer__", 0);
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":338
- * 
- *         def __releasebuffer__(ndarray self, Py_buffer* info):
- *             if PyArray_HASFIELDS(self):             # <<<<<<<<<<<<<<
- *                 PyObject_Free(info.format)
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
- */
-  __pyx_t_1 = (PyArray_HASFIELDS(__pyx_v_self) != 0);
-  if (__pyx_t_1) {
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":339
- *         def __releasebuffer__(ndarray self, Py_buffer* info):
- *             if PyArray_HASFIELDS(self):
- *                 PyObject_Free(info.format)             # <<<<<<<<<<<<<<
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
- *                 PyObject_Free(info.strides)
- */
-    PyObject_Free(__pyx_v_info->format);
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":338
- * 
- *         def __releasebuffer__(ndarray self, Py_buffer* info):
- *             if PyArray_HASFIELDS(self):             # <<<<<<<<<<<<<<
- *                 PyObject_Free(info.format)
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
- */
-  }
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":340
- *             if PyArray_HASFIELDS(self):
- *                 PyObject_Free(info.format)
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):             # <<<<<<<<<<<<<<
- *                 PyObject_Free(info.strides)
- *                 # info.shape was stored after info.strides in the same block
- */
-  __pyx_t_1 = (((sizeof(npy_intp)) != (sizeof(Py_ssize_t))) != 0);
-  if (__pyx_t_1) {
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":341
- *                 PyObject_Free(info.format)
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
- *                 PyObject_Free(info.strides)             # <<<<<<<<<<<<<<
- *                 # info.shape was stored after info.strides in the same block
- * 
- */
-    PyObject_Free(__pyx_v_info->strides);
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":340
- *             if PyArray_HASFIELDS(self):
- *                 PyObject_Free(info.format)
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):             # <<<<<<<<<<<<<<
- *                 PyObject_Free(info.strides)
- *                 # info.shape was stored after info.strides in the same block
- */
-  }
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":337
- *                 f[0] = c'\0' # Terminate format string
- * 
- *         def __releasebuffer__(ndarray self, Py_buffer* info):             # <<<<<<<<<<<<<<
- *             if PyArray_HASFIELDS(self):
- *                 PyObject_Free(info.format)
- */
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-}
-
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":820
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -5464,29 +4592,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":821
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":736
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 821, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 736, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":820
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -5497,15 +4625,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":823
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -5514,29 +4642,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":824
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":739
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 824, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 739, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":823
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -5547,15 +4675,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":826
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -5564,29 +4692,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":827
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":742
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 827, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 742, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":826
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -5597,15 +4725,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":829
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -5614,29 +4742,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":830
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":745
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 830, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 745, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":829
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -5647,15 +4775,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":832
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -5664,29 +4792,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":833
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":748
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 833, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 748, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":832
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -5697,966 +4825,217 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":835
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":836
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":837
+    /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":752
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":836
+    /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":839
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":754
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
- * cdef inline char* _util_dtypestring(dtype descr, char* f, char* end, int* offset) except NULL:
+ * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":835
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":841
- *         return ()
- * 
- * cdef inline char* _util_dtypestring(dtype descr, char* f, char* end, int* offset) except NULL:             # <<<<<<<<<<<<<<
- *     # Recursive utility function used in __getbuffer__ to get format
- *     # string. The new location in the format string is returned.
- */
-
-static CYTHON_INLINE char *__pyx_f_5numpy__util_dtypestring(PyArray_Descr *__pyx_v_descr, char *__pyx_v_f, char *__pyx_v_end, int *__pyx_v_offset) {
-  PyArray_Descr *__pyx_v_child = 0;
-  int __pyx_v_endian_detector;
-  int __pyx_v_little_endian;
-  PyObject *__pyx_v_fields = 0;
-  PyObject *__pyx_v_childname = NULL;
-  PyObject *__pyx_v_new_offset = NULL;
-  PyObject *__pyx_v_t = NULL;
-  char *__pyx_r;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  Py_ssize_t __pyx_t_2;
-  PyObject *__pyx_t_3 = NULL;
-  PyObject *__pyx_t_4 = NULL;
-  int __pyx_t_5;
-  int __pyx_t_6;
-  int __pyx_t_7;
-  long __pyx_t_8;
-  char *__pyx_t_9;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("_util_dtypestring", 0);
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":846
- * 
- *     cdef dtype child
- *     cdef int endian_detector = 1             # <<<<<<<<<<<<<<
- *     cdef bint little_endian = ((<char*>&endian_detector)[0] != 0)
- *     cdef tuple fields
- */
-  __pyx_v_endian_detector = 1;
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":847
- *     cdef dtype child
- *     cdef int endian_detector = 1
- *     cdef bint little_endian = ((<char*>&endian_detector)[0] != 0)             # <<<<<<<<<<<<<<
- *     cdef tuple fields
- * 
- */
-  __pyx_v_little_endian = ((((char *)(&__pyx_v_endian_detector))[0]) != 0);
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":850
- *     cdef tuple fields
- * 
- *     for childname in descr.names:             # <<<<<<<<<<<<<<
- *         fields = descr.fields[childname]
- *         child, new_offset = fields
- */
-  if (unlikely(__pyx_v_descr->names == Py_None)) {
-    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-    __PYX_ERR(1, 850, __pyx_L1_error)
-  }
-  __pyx_t_1 = __pyx_v_descr->names; __Pyx_INCREF(__pyx_t_1); __pyx_t_2 = 0;
-  for (;;) {
-    if (__pyx_t_2 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
-    #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_3); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(1, 850, __pyx_L1_error)
-    #else
-    __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 850, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    #endif
-    __Pyx_XDECREF_SET(__pyx_v_childname, __pyx_t_3);
-    __pyx_t_3 = 0;
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":851
- * 
- *     for childname in descr.names:
- *         fields = descr.fields[childname]             # <<<<<<<<<<<<<<
- *         child, new_offset = fields
- * 
- */
-    if (unlikely(__pyx_v_descr->fields == Py_None)) {
-      PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(1, 851, __pyx_L1_error)
-    }
-    __pyx_t_3 = __Pyx_PyDict_GetItem(__pyx_v_descr->fields, __pyx_v_childname); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 851, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    if (!(likely(PyTuple_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_t_3)->tp_name), 0))) __PYX_ERR(1, 851, __pyx_L1_error)
-    __Pyx_XDECREF_SET(__pyx_v_fields, ((PyObject*)__pyx_t_3));
-    __pyx_t_3 = 0;
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":852
- *     for childname in descr.names:
- *         fields = descr.fields[childname]
- *         child, new_offset = fields             # <<<<<<<<<<<<<<
- * 
- *         if (end - f) - <int>(new_offset - offset[0]) < 15:
- */
-    if (likely(__pyx_v_fields != Py_None)) {
-      PyObject* sequence = __pyx_v_fields;
-      Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
-      if (unlikely(size != 2)) {
-        if (size > 2) __Pyx_RaiseTooManyValuesError(2);
-        else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-        __PYX_ERR(1, 852, __pyx_L1_error)
-      }
-      #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-      __pyx_t_3 = PyTuple_GET_ITEM(sequence, 0); 
-      __pyx_t_4 = PyTuple_GET_ITEM(sequence, 1); 
-      __Pyx_INCREF(__pyx_t_3);
-      __Pyx_INCREF(__pyx_t_4);
-      #else
-      __pyx_t_3 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 852, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 852, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      #endif
-    } else {
-      __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(1, 852, __pyx_L1_error)
-    }
-    if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_dtype))))) __PYX_ERR(1, 852, __pyx_L1_error)
-    __Pyx_XDECREF_SET(__pyx_v_child, ((PyArray_Descr *)__pyx_t_3));
-    __pyx_t_3 = 0;
-    __Pyx_XDECREF_SET(__pyx_v_new_offset, __pyx_t_4);
-    __pyx_t_4 = 0;
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":854
- *         child, new_offset = fields
- * 
- *         if (end - f) - <int>(new_offset - offset[0]) < 15:             # <<<<<<<<<<<<<<
- *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")
- * 
- */
-    __pyx_t_4 = __Pyx_PyInt_From_int((__pyx_v_offset[0])); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 854, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_3 = PyNumber_Subtract(__pyx_v_new_offset, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 854, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 854, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_6 = ((((__pyx_v_end - __pyx_v_f) - ((int)__pyx_t_5)) < 15) != 0);
-    if (unlikely(__pyx_t_6)) {
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":855
- * 
- *         if (end - f) - <int>(new_offset - offset[0]) < 15:
- *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")             # <<<<<<<<<<<<<<
- * 
- *         if ((child.byteorder == c'>' and little_endian) or
- */
-      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 855, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __PYX_ERR(1, 855, __pyx_L1_error)
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":854
- *         child, new_offset = fields
- * 
- *         if (end - f) - <int>(new_offset - offset[0]) < 15:             # <<<<<<<<<<<<<<
- *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")
- * 
- */
-    }
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":857
- *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")
- * 
- *         if ((child.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
- *             (child.byteorder == c'<' and not little_endian)):
- *             raise ValueError(u"Non-native byte order not supported")
- */
-    __pyx_t_7 = ((__pyx_v_child->byteorder == '>') != 0);
-    if (!__pyx_t_7) {
-      goto __pyx_L8_next_or;
-    } else {
-    }
-    __pyx_t_7 = (__pyx_v_little_endian != 0);
-    if (!__pyx_t_7) {
-    } else {
-      __pyx_t_6 = __pyx_t_7;
-      goto __pyx_L7_bool_binop_done;
-    }
-    __pyx_L8_next_or:;
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":858
- * 
- *         if ((child.byteorder == c'>' and little_endian) or
- *             (child.byteorder == c'<' and not little_endian)):             # <<<<<<<<<<<<<<
- *             raise ValueError(u"Non-native byte order not supported")
- *             # One could encode it in the format string and have Cython
- */
-    __pyx_t_7 = ((__pyx_v_child->byteorder == '<') != 0);
-    if (__pyx_t_7) {
-    } else {
-      __pyx_t_6 = __pyx_t_7;
-      goto __pyx_L7_bool_binop_done;
-    }
-    __pyx_t_7 = ((!(__pyx_v_little_endian != 0)) != 0);
-    __pyx_t_6 = __pyx_t_7;
-    __pyx_L7_bool_binop_done:;
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":857
- *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")
- * 
- *         if ((child.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
- *             (child.byteorder == c'<' and not little_endian)):
- *             raise ValueError(u"Non-native byte order not supported")
- */
-    if (unlikely(__pyx_t_6)) {
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":859
- *         if ((child.byteorder == c'>' and little_endian) or
- *             (child.byteorder == c'<' and not little_endian)):
- *             raise ValueError(u"Non-native byte order not supported")             # <<<<<<<<<<<<<<
- *             # One could encode it in the format string and have Cython
- *             # complain instead, BUT: < and > in format strings also imply
- */
-      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 859, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __PYX_ERR(1, 859, __pyx_L1_error)
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":857
- *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")
- * 
- *         if ((child.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
- *             (child.byteorder == c'<' and not little_endian)):
- *             raise ValueError(u"Non-native byte order not supported")
- */
-    }
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":869
- * 
- *         # Output padding bytes
- *         while offset[0] < new_offset:             # <<<<<<<<<<<<<<
- *             f[0] = 120 # "x"; pad byte
- *             f += 1
- */
-    while (1) {
-      __pyx_t_3 = __Pyx_PyInt_From_int((__pyx_v_offset[0])); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 869, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_t_3, __pyx_v_new_offset, Py_LT); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 869, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 869, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (!__pyx_t_6) break;
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":870
- *         # Output padding bytes
- *         while offset[0] < new_offset:
- *             f[0] = 120 # "x"; pad byte             # <<<<<<<<<<<<<<
- *             f += 1
- *             offset[0] += 1
- */
-      (__pyx_v_f[0]) = 0x78;
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":871
- *         while offset[0] < new_offset:
- *             f[0] = 120 # "x"; pad byte
- *             f += 1             # <<<<<<<<<<<<<<
- *             offset[0] += 1
- * 
- */
-      __pyx_v_f = (__pyx_v_f + 1);
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":872
- *             f[0] = 120 # "x"; pad byte
- *             f += 1
- *             offset[0] += 1             # <<<<<<<<<<<<<<
- * 
- *         offset[0] += child.itemsize
- */
-      __pyx_t_8 = 0;
-      (__pyx_v_offset[__pyx_t_8]) = ((__pyx_v_offset[__pyx_t_8]) + 1);
-    }
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":874
- *             offset[0] += 1
- * 
- *         offset[0] += child.itemsize             # <<<<<<<<<<<<<<
- * 
- *         if not PyDataType_HASFIELDS(child):
- */
-    __pyx_t_8 = 0;
-    (__pyx_v_offset[__pyx_t_8]) = ((__pyx_v_offset[__pyx_t_8]) + __pyx_v_child->elsize);
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":876
- *         offset[0] += child.itemsize
- * 
- *         if not PyDataType_HASFIELDS(child):             # <<<<<<<<<<<<<<
- *             t = child.type_num
- *             if end - f < 5:
- */
-    __pyx_t_6 = ((!(PyDataType_HASFIELDS(__pyx_v_child) != 0)) != 0);
-    if (__pyx_t_6) {
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":877
- * 
- *         if not PyDataType_HASFIELDS(child):
- *             t = child.type_num             # <<<<<<<<<<<<<<
- *             if end - f < 5:
- *                 raise RuntimeError(u"Format string allocated too short.")
- */
-      __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_child->type_num); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 877, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __Pyx_XDECREF_SET(__pyx_v_t, __pyx_t_4);
-      __pyx_t_4 = 0;
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":878
- *         if not PyDataType_HASFIELDS(child):
- *             t = child.type_num
- *             if end - f < 5:             # <<<<<<<<<<<<<<
- *                 raise RuntimeError(u"Format string allocated too short.")
- * 
- */
-      __pyx_t_6 = (((__pyx_v_end - __pyx_v_f) < 5) != 0);
-      if (unlikely(__pyx_t_6)) {
-
-        /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":879
- *             t = child.type_num
- *             if end - f < 5:
- *                 raise RuntimeError(u"Format string allocated too short.")             # <<<<<<<<<<<<<<
- * 
- *             # Until ticket #99 is fixed, use integers to avoid warnings
- */
-        __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 879, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_4);
-        __Pyx_Raise(__pyx_t_4, 0, 0, 0);
-        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        __PYX_ERR(1, 879, __pyx_L1_error)
-
-        /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":878
- *         if not PyDataType_HASFIELDS(child):
- *             t = child.type_num
- *             if end - f < 5:             # <<<<<<<<<<<<<<
- *                 raise RuntimeError(u"Format string allocated too short.")
- * 
- */
-      }
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":882
- * 
- *             # Until ticket #99 is fixed, use integers to avoid warnings
- *             if   t == NPY_BYTE:        f[0] =  98 #"b"             # <<<<<<<<<<<<<<
- *             elif t == NPY_UBYTE:       f[0] =  66 #"B"
- *             elif t == NPY_SHORT:       f[0] = 104 #"h"
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_BYTE); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 882, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 882, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 882, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 98;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":883
- *             # Until ticket #99 is fixed, use integers to avoid warnings
- *             if   t == NPY_BYTE:        f[0] =  98 #"b"
- *             elif t == NPY_UBYTE:       f[0] =  66 #"B"             # <<<<<<<<<<<<<<
- *             elif t == NPY_SHORT:       f[0] = 104 #"h"
- *             elif t == NPY_USHORT:      f[0] =  72 #"H"
- */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_UBYTE); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 883, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 883, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 883, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 66;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":884
- *             if   t == NPY_BYTE:        f[0] =  98 #"b"
- *             elif t == NPY_UBYTE:       f[0] =  66 #"B"
- *             elif t == NPY_SHORT:       f[0] = 104 #"h"             # <<<<<<<<<<<<<<
- *             elif t == NPY_USHORT:      f[0] =  72 #"H"
- *             elif t == NPY_INT:         f[0] = 105 #"i"
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_SHORT); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 884, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 884, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 884, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 0x68;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":885
- *             elif t == NPY_UBYTE:       f[0] =  66 #"B"
- *             elif t == NPY_SHORT:       f[0] = 104 #"h"
- *             elif t == NPY_USHORT:      f[0] =  72 #"H"             # <<<<<<<<<<<<<<
- *             elif t == NPY_INT:         f[0] = 105 #"i"
- *             elif t == NPY_UINT:        f[0] =  73 #"I"
- */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_USHORT); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 885, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 885, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 885, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 72;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":886
- *             elif t == NPY_SHORT:       f[0] = 104 #"h"
- *             elif t == NPY_USHORT:      f[0] =  72 #"H"
- *             elif t == NPY_INT:         f[0] = 105 #"i"             # <<<<<<<<<<<<<<
- *             elif t == NPY_UINT:        f[0] =  73 #"I"
- *             elif t == NPY_LONG:        f[0] = 108 #"l"
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_INT); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 886, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 886, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 886, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 0x69;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":887
- *             elif t == NPY_USHORT:      f[0] =  72 #"H"
- *             elif t == NPY_INT:         f[0] = 105 #"i"
- *             elif t == NPY_UINT:        f[0] =  73 #"I"             # <<<<<<<<<<<<<<
- *             elif t == NPY_LONG:        f[0] = 108 #"l"
- *             elif t == NPY_ULONG:       f[0] = 76  #"L"
- */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_UINT); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 887, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 887, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 887, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 73;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":888
- *             elif t == NPY_INT:         f[0] = 105 #"i"
- *             elif t == NPY_UINT:        f[0] =  73 #"I"
- *             elif t == NPY_LONG:        f[0] = 108 #"l"             # <<<<<<<<<<<<<<
- *             elif t == NPY_ULONG:       f[0] = 76  #"L"
- *             elif t == NPY_LONGLONG:    f[0] = 113 #"q"
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_LONG); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 888, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 888, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 888, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 0x6C;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":889
- *             elif t == NPY_UINT:        f[0] =  73 #"I"
- *             elif t == NPY_LONG:        f[0] = 108 #"l"
- *             elif t == NPY_ULONG:       f[0] = 76  #"L"             # <<<<<<<<<<<<<<
- *             elif t == NPY_LONGLONG:    f[0] = 113 #"q"
- *             elif t == NPY_ULONGLONG:   f[0] = 81  #"Q"
- */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_ULONG); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 889, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 889, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 889, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 76;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":890
- *             elif t == NPY_LONG:        f[0] = 108 #"l"
- *             elif t == NPY_ULONG:       f[0] = 76  #"L"
- *             elif t == NPY_LONGLONG:    f[0] = 113 #"q"             # <<<<<<<<<<<<<<
- *             elif t == NPY_ULONGLONG:   f[0] = 81  #"Q"
- *             elif t == NPY_FLOAT:       f[0] = 102 #"f"
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_LONGLONG); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 890, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 890, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 890, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 0x71;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":891
- *             elif t == NPY_ULONG:       f[0] = 76  #"L"
- *             elif t == NPY_LONGLONG:    f[0] = 113 #"q"
- *             elif t == NPY_ULONGLONG:   f[0] = 81  #"Q"             # <<<<<<<<<<<<<<
- *             elif t == NPY_FLOAT:       f[0] = 102 #"f"
- *             elif t == NPY_DOUBLE:      f[0] = 100 #"d"
- */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_ULONGLONG); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 891, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 891, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 891, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 81;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":892
- *             elif t == NPY_LONGLONG:    f[0] = 113 #"q"
- *             elif t == NPY_ULONGLONG:   f[0] = 81  #"Q"
- *             elif t == NPY_FLOAT:       f[0] = 102 #"f"             # <<<<<<<<<<<<<<
- *             elif t == NPY_DOUBLE:      f[0] = 100 #"d"
- *             elif t == NPY_LONGDOUBLE:  f[0] = 103 #"g"
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_FLOAT); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 892, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 892, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 892, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 0x66;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":893
- *             elif t == NPY_ULONGLONG:   f[0] = 81  #"Q"
- *             elif t == NPY_FLOAT:       f[0] = 102 #"f"
- *             elif t == NPY_DOUBLE:      f[0] = 100 #"d"             # <<<<<<<<<<<<<<
- *             elif t == NPY_LONGDOUBLE:  f[0] = 103 #"g"
- *             elif t == NPY_CFLOAT:      f[0] = 90; f[1] = 102; f += 1 # Zf
- */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_DOUBLE); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 893, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 893, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 893, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 0x64;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":894
- *             elif t == NPY_FLOAT:       f[0] = 102 #"f"
- *             elif t == NPY_DOUBLE:      f[0] = 100 #"d"
- *             elif t == NPY_LONGDOUBLE:  f[0] = 103 #"g"             # <<<<<<<<<<<<<<
- *             elif t == NPY_CFLOAT:      f[0] = 90; f[1] = 102; f += 1 # Zf
- *             elif t == NPY_CDOUBLE:     f[0] = 90; f[1] = 100; f += 1 # Zd
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_LONGDOUBLE); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 894, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 894, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 894, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 0x67;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":895
- *             elif t == NPY_DOUBLE:      f[0] = 100 #"d"
- *             elif t == NPY_LONGDOUBLE:  f[0] = 103 #"g"
- *             elif t == NPY_CFLOAT:      f[0] = 90; f[1] = 102; f += 1 # Zf             # <<<<<<<<<<<<<<
- *             elif t == NPY_CDOUBLE:     f[0] = 90; f[1] = 100; f += 1 # Zd
- *             elif t == NPY_CLONGDOUBLE: f[0] = 90; f[1] = 103; f += 1 # Zg
- */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_CFLOAT); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 895, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 895, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 895, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 90;
-        (__pyx_v_f[1]) = 0x66;
-        __pyx_v_f = (__pyx_v_f + 1);
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":896
- *             elif t == NPY_LONGDOUBLE:  f[0] = 103 #"g"
- *             elif t == NPY_CFLOAT:      f[0] = 90; f[1] = 102; f += 1 # Zf
- *             elif t == NPY_CDOUBLE:     f[0] = 90; f[1] = 100; f += 1 # Zd             # <<<<<<<<<<<<<<
- *             elif t == NPY_CLONGDOUBLE: f[0] = 90; f[1] = 103; f += 1 # Zg
- *             elif t == NPY_OBJECT:      f[0] = 79 #"O"
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_CDOUBLE); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 896, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 896, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 896, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 90;
-        (__pyx_v_f[1]) = 0x64;
-        __pyx_v_f = (__pyx_v_f + 1);
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":897
- *             elif t == NPY_CFLOAT:      f[0] = 90; f[1] = 102; f += 1 # Zf
- *             elif t == NPY_CDOUBLE:     f[0] = 90; f[1] = 100; f += 1 # Zd
- *             elif t == NPY_CLONGDOUBLE: f[0] = 90; f[1] = 103; f += 1 # Zg             # <<<<<<<<<<<<<<
- *             elif t == NPY_OBJECT:      f[0] = 79 #"O"
- *             else:
- */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_CLONGDOUBLE); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 897, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 897, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 897, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 90;
-        (__pyx_v_f[1]) = 0x67;
-        __pyx_v_f = (__pyx_v_f + 1);
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":898
- *             elif t == NPY_CDOUBLE:     f[0] = 90; f[1] = 100; f += 1 # Zd
- *             elif t == NPY_CLONGDOUBLE: f[0] = 90; f[1] = 103; f += 1 # Zg
- *             elif t == NPY_OBJECT:      f[0] = 79 #"O"             # <<<<<<<<<<<<<<
- *             else:
- *                 raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_OBJECT); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 898, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 898, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 898, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (likely(__pyx_t_6)) {
-        (__pyx_v_f[0]) = 79;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":900
- *             elif t == NPY_OBJECT:      f[0] = 79 #"O"
- *             else:
- *                 raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)             # <<<<<<<<<<<<<<
- *             f += 1
- *         else:
- */
-      /*else*/ {
-        __pyx_t_3 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_unknown_dtype_code_in_numpy_pxd, __pyx_v_t); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 900, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 900, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_4);
-        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        __Pyx_Raise(__pyx_t_4, 0, 0, 0);
-        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        __PYX_ERR(1, 900, __pyx_L1_error)
-      }
-      __pyx_L15:;
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":901
- *             else:
- *                 raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)
- *             f += 1             # <<<<<<<<<<<<<<
- *         else:
- *             # Cython ignores struct boundary information ("T{...}"),
- */
-      __pyx_v_f = (__pyx_v_f + 1);
-
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":876
- *         offset[0] += child.itemsize
- * 
- *         if not PyDataType_HASFIELDS(child):             # <<<<<<<<<<<<<<
- *             t = child.type_num
- *             if end - f < 5:
- */
-      goto __pyx_L13;
-    }
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":905
- *             # Cython ignores struct boundary information ("T{...}"),
- *             # so don't output it
- *             f = _util_dtypestring(child, f, end, offset)             # <<<<<<<<<<<<<<
- *     return f
- * 
- */
-    /*else*/ {
-      __pyx_t_9 = __pyx_f_5numpy__util_dtypestring(__pyx_v_child, __pyx_v_f, __pyx_v_end, __pyx_v_offset); if (unlikely(__pyx_t_9 == ((char *)NULL))) __PYX_ERR(1, 905, __pyx_L1_error)
-      __pyx_v_f = __pyx_t_9;
-    }
-    __pyx_L13:;
-
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":850
- *     cdef tuple fields
- * 
- *     for childname in descr.names:             # <<<<<<<<<<<<<<
- *         fields = descr.fields[childname]
- *         child, new_offset = fields
- */
-  }
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":906
- *             # so don't output it
- *             f = _util_dtypestring(child, f, end, offset)
- *     return f             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = __pyx_v_f;
-  goto __pyx_L0;
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":841
- *         return ()
- * 
- * cdef inline char* _util_dtypestring(dtype descr, char* f, char* end, int* offset) except NULL:             # <<<<<<<<<<<<<<
- *     # Recursive utility function used in __getbuffer__ to get format
- *     # string. The new location in the format string is returned.
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_AddTraceback("numpy._util_dtypestring", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XDECREF((PyObject *)__pyx_v_child);
-  __Pyx_XDECREF(__pyx_v_fields);
-  __Pyx_XDECREF(__pyx_v_childname);
-  __Pyx_XDECREF(__pyx_v_new_offset);
-  __Pyx_XDECREF(__pyx_v_t);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1021
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1022
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":930
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1023
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":931
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1021
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1025
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1026
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":934
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1027
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1028
+    /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":936
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1027
+    /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1029
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":937
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1025
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1033
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
- *         _import_array()
+ *         __pyx_import_array()
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_import_array(void) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
@@ -6667,105 +5046,105 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1034
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
- *         _import_array()
+ *         __pyx_import_array()
  *     except Exception:
  */
   {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1035
+      /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":943
  * cdef inline int import_array() except -1:
  *     try:
- *         _import_array()             # <<<<<<<<<<<<<<
+ *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 1035, __pyx_L3_error)
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 943, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1034
+      /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
- *         _import_array()
+ *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1036
+    /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *     try:
- *         _import_array()
+ *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 1036, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 944, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1037
- *         _import_array()
+      /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":945
+ *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 1037, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 945, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 1037, __pyx_L5_except_error)
+      __PYX_ERR(1, 945, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1034
+    /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
- *         _import_array()
+ *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1033
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
- *         _import_array()
+ *         __pyx_import_array()
  */
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_5);
@@ -6775,15 +5154,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1039
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6799,15 +5178,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1040
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -6815,84 +5194,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1041
+      /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":949
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 1041, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 949, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1040
+      /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1042
+    /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 1042, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 950, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1043
+      /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 1043, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 951, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 1043, __pyx_L5_except_error)
+      __PYX_ERR(1, 951, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1040
+    /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1039
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6907,15 +5286,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1045
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6931,15 +5310,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1046
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -6947,81 +5326,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1047
+      /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":955
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 1047, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 955, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1046
+      /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1048
+    /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":956
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
+ * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 1048, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 956, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1049
+      /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":957
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
+ * 
+ * cdef extern from *:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 1049, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 957, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 1049, __pyx_L5_except_error)
+      __PYX_ERR(1, 957, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1046
+    /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1045
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -7036,14 +5418,188 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":967
+ * 
+ * 
+ * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.timedelta64)`
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
+
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":979
+ *     bool
+ *     """
+ *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":967
+ * 
+ * 
+ * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.timedelta64)`
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":982
+ * 
+ * 
+ * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.datetime64)`
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("is_datetime64_object", 0);
+
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":994
+ *     bool
+ *     """
+ *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":982
+ * 
+ * 
+ * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.datetime64)`
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":997
+ * 
+ * 
+ * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy datetime64 object
+ */
+
+static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
+  npy_datetime __pyx_r;
+
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":1004
+ *     also needed.  That can be found using `get_datetime64_unit`.
+ *     """
+ *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":997
+ * 
+ * 
+ * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy datetime64 object
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":1007
+ * 
+ * 
+ * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy timedelta64 object
+ */
+
+static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
+  npy_timedelta __pyx_r;
+
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":1011
+ *     returns the int64 value underlying scalar numpy timedelta64 object
+ *     """
+ *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":1007
+ * 
+ * 
+ * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy timedelta64 object
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":1014
+ * 
+ * 
+ * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the unit part of the dtype for a numpy datetime64 object.
+ */
+
+static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
+  NPY_DATETIMEUNIT __pyx_r;
+
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":1018
+ *     returns the unit part of the dtype for a numpy datetime64 object.
+ *     """
+ *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
+ */
+  __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":1014
+ * 
+ * 
+ * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the unit part of the dtype for a numpy datetime64 object.
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
 /* "View.MemoryView":123
  *         cdef bint dtype_is_object
  * 
  *     def __cinit__(array self, tuple shape, Py_ssize_t itemsize, format not None,             # <<<<<<<<<<<<<<
  *                   mode="c", bint allocate_buffer=True):
  * 
  */
@@ -7239,15 +5795,15 @@
     /* "View.MemoryView":134
  * 
  *         if not self.ndim:
  *             raise ValueError("Empty shape tuple for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if itemsize <= 0:
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 134, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 134, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(2, 134, __pyx_L1_error)
 
     /* "View.MemoryView":133
  *         self.itemsize = itemsize
@@ -7271,15 +5827,15 @@
     /* "View.MemoryView":137
  * 
  *         if itemsize <= 0:
  *             raise ValueError("itemsize <= 0 for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if not isinstance(format, bytes):
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 137, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 137, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(2, 137, __pyx_L1_error)
 
     /* "View.MemoryView":136
  *             raise ValueError("Empty shape tuple for cython.array")
@@ -7398,15 +5954,15 @@
     /* "View.MemoryView":149
  * 
  *         if not self._shape:
  *             raise MemoryError("unable to allocate shape and strides.")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 149, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 149, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(2, 149, __pyx_L1_error)
 
     /* "View.MemoryView":148
  *         self._strides = self._shape + self.ndim
@@ -7672,15 +6228,15 @@
       /* "View.MemoryView":177
  *             self.data = <char *>malloc(self.len)
  *             if not self.data:
  *                 raise MemoryError("unable to allocate array data.")             # <<<<<<<<<<<<<<
  * 
  *             if self.dtype_is_object:
  */
-      __pyx_t_10 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(2, 177, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(2, 177, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_Raise(__pyx_t_10, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       __PYX_ERR(2, 177, __pyx_L1_error)
 
       /* "View.MemoryView":176
  * 
@@ -7916,15 +6472,15 @@
     /* "View.MemoryView":193
  *             bufmode = PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         if not (flags & bufmode):
  *             raise ValueError("Can only create a buffer that is contiguous in memory.")             # <<<<<<<<<<<<<<
  *         info.buf = self.data
  *         info.len = self.len
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 193, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 193, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(2, 193, __pyx_L1_error)
 
     /* "View.MemoryView":192
  *         elif self.mode == u"fortran":
@@ -8650,15 +7206,15 @@
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(2, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
@@ -8706,15 +7262,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__14, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(2, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
@@ -10435,15 +8991,15 @@
     /* "View.MemoryView":420
  *     def __setitem__(memoryview self, object index, object value):
  *         if self.view.readonly:
  *             raise TypeError("Cannot assign to read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         have_slices, index = _unellipsify(index, self.view.ndim)
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__15, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 420, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 420, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __PYX_ERR(2, 420, __pyx_L1_error)
 
     /* "View.MemoryView":419
  * 
@@ -11483,15 +10039,15 @@
       /* "View.MemoryView":497
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:
  *             raise ValueError("Unable to convert item to object")             # <<<<<<<<<<<<<<
  *         else:
  *             if len(self.view.format) == 1:
  */
-      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__16, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 497, __pyx_L5_except_error)
+      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 497, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_Raise(__pyx_t_6, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __PYX_ERR(2, 497, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
@@ -11845,15 +10401,15 @@
     /* "View.MemoryView":522
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         if flags & PyBUF_WRITABLE and self.view.readonly:
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_ND:
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__17, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 522, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 522, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(2, 522, __pyx_L1_error)
 
     /* "View.MemoryView":521
  *     @cname('getbuffer')
@@ -12394,15 +10950,15 @@
     /* "View.MemoryView":572
  *         if self.view.strides == NULL:
  * 
  *             raise ValueError("Buffer view does not expose strides")             # <<<<<<<<<<<<<<
  * 
  *         return tuple([stride for stride in self.view.strides[:self.view.ndim]])
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__18, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 572, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 572, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __PYX_ERR(2, 572, __pyx_L1_error)
 
     /* "View.MemoryView":570
  *     @property
@@ -12511,15 +11067,15 @@
  *             return (-1,) * self.view.ndim             # <<<<<<<<<<<<<<
  * 
  *         return tuple([suboffset for suboffset in self.view.suboffsets[:self.view.ndim]])
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_self->view.ndim); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 579, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = PyNumber_Multiply(__pyx_tuple__19, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 579, __pyx_L1_error)
+    __pyx_t_3 = PyNumber_Multiply(__pyx_tuple__14, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 579, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
     /* "View.MemoryView":578
@@ -13549,15 +12105,15 @@
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__20, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__15, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(2, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
@@ -13605,15 +12161,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__21, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__16, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(2, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
@@ -13962,17 +12518,17 @@
  *             else:
  */
         __pyx_t_8 = PyObject_Length(__pyx_v_tup); if (unlikely(__pyx_t_8 == ((Py_ssize_t)-1))) __PYX_ERR(2, 684, __pyx_L1_error)
         __pyx_t_7 = PyList_New(1 * ((((__pyx_v_ndim - __pyx_t_8) + 1)<0) ? 0:((__pyx_v_ndim - __pyx_t_8) + 1))); if (unlikely(!__pyx_t_7)) __PYX_ERR(2, 684, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
         { Py_ssize_t __pyx_temp;
           for (__pyx_temp=0; __pyx_temp < ((__pyx_v_ndim - __pyx_t_8) + 1); __pyx_temp++) {
-            __Pyx_INCREF(__pyx_slice__22);
-            __Pyx_GIVEREF(__pyx_slice__22);
-            PyList_SET_ITEM(__pyx_t_7, __pyx_temp, __pyx_slice__22);
+            __Pyx_INCREF(__pyx_slice__17);
+            __Pyx_GIVEREF(__pyx_slice__17);
+            PyList_SET_ITEM(__pyx_t_7, __pyx_temp, __pyx_slice__17);
           }
         }
         __pyx_t_9 = __Pyx_PyList_Extend(__pyx_v_result, __pyx_t_7); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(2, 684, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
         /* "View.MemoryView":685
  *             if not seen_ellipsis:
@@ -13997,15 +12553,15 @@
  *                 seen_ellipsis = True
  *             else:
  *                 result.append(slice(None))             # <<<<<<<<<<<<<<
  *             have_slices = True
  *         else:
  */
       /*else*/ {
-        __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_result, __pyx_slice__22); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(2, 687, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_result, __pyx_slice__17); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(2, 687, __pyx_L1_error)
       }
       __pyx_L7:;
 
       /* "View.MemoryView":688
  *             else:
  *                 result.append(slice(None))
  *             have_slices = True             # <<<<<<<<<<<<<<
@@ -14137,17 +12693,17 @@
  * 
  *     return have_slices or nslices, tuple(result)
  */
     __pyx_t_3 = PyList_New(1 * ((__pyx_v_nslices<0) ? 0:__pyx_v_nslices)); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 698, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     { Py_ssize_t __pyx_temp;
       for (__pyx_temp=0; __pyx_temp < __pyx_v_nslices; __pyx_temp++) {
-        __Pyx_INCREF(__pyx_slice__22);
-        __Pyx_GIVEREF(__pyx_slice__22);
-        PyList_SET_ITEM(__pyx_t_3, __pyx_temp, __pyx_slice__22);
+        __Pyx_INCREF(__pyx_slice__17);
+        __Pyx_GIVEREF(__pyx_slice__17);
+        PyList_SET_ITEM(__pyx_t_3, __pyx_temp, __pyx_slice__17);
       }
     }
     __pyx_t_9 = __Pyx_PyList_Extend(__pyx_v_result, __pyx_t_3); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(2, 698, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
     /* "View.MemoryView":697
  * 
@@ -14266,15 +12822,15 @@
       /* "View.MemoryView":705
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:
  *             raise ValueError("Indirect dimensions not supported")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-      __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__23, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 705, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__18, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 705, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_Raise(__pyx_t_5, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __PYX_ERR(2, 705, __pyx_L1_error)
 
       /* "View.MemoryView":704
  * cdef assert_direct_dimensions(Py_ssize_t *suboffsets, int ndim):
@@ -16450,15 +15006,15 @@
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__24, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__19, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(2, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
@@ -16506,15 +15062,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__25, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__20, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(2, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
@@ -19783,15 +18339,15 @@
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xb068931, 0x82a3537, 0x6ae9995):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb068931, 0x82a3537, 0x6ae9995) = (name))" % __pyx_checksum)
  */
   __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__26, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__21, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(2, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xb068931, 0x82a3537, 0x6ae9995):
@@ -20861,32 +19417,28 @@
   {&__pyx_kp_s_Buffer_view_does_not_expose_stri, __pyx_k_Buffer_view_does_not_expose_stri, sizeof(__pyx_k_Buffer_view_does_not_expose_stri), 0, 0, 1, 0},
   {&__pyx_kp_s_Can_only_create_a_buffer_that_is, __pyx_k_Can_only_create_a_buffer_that_is, sizeof(__pyx_k_Can_only_create_a_buffer_that_is), 0, 0, 1, 0},
   {&__pyx_kp_s_Cannot_assign_to_read_only_memor, __pyx_k_Cannot_assign_to_read_only_memor, sizeof(__pyx_k_Cannot_assign_to_read_only_memor), 0, 0, 1, 0},
   {&__pyx_kp_s_Cannot_create_writable_memory_vi, __pyx_k_Cannot_create_writable_memory_vi, sizeof(__pyx_k_Cannot_create_writable_memory_vi), 0, 0, 1, 0},
   {&__pyx_kp_s_Cannot_index_with_type_s, __pyx_k_Cannot_index_with_type_s, sizeof(__pyx_k_Cannot_index_with_type_s), 0, 0, 1, 0},
   {&__pyx_n_s_Ellipsis, __pyx_k_Ellipsis, sizeof(__pyx_k_Ellipsis), 0, 0, 1, 1},
   {&__pyx_kp_s_Empty_shape_tuple_for_cython_arr, __pyx_k_Empty_shape_tuple_for_cython_arr, sizeof(__pyx_k_Empty_shape_tuple_for_cython_arr), 0, 0, 1, 0},
-  {&__pyx_kp_u_Format_string_allocated_too_shor, __pyx_k_Format_string_allocated_too_shor, sizeof(__pyx_k_Format_string_allocated_too_shor), 0, 1, 0, 0},
-  {&__pyx_kp_u_Format_string_allocated_too_shor_2, __pyx_k_Format_string_allocated_too_shor_2, sizeof(__pyx_k_Format_string_allocated_too_shor_2), 0, 1, 0, 0},
   {&__pyx_n_s_ImportError, __pyx_k_ImportError, sizeof(__pyx_k_ImportError), 0, 0, 1, 1},
   {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_k_Incompatible_checksums_0x_x_vs_0, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0), 0, 0, 1, 0},
   {&__pyx_n_s_IndexError, __pyx_k_IndexError, sizeof(__pyx_k_IndexError), 0, 0, 1, 1},
   {&__pyx_kp_s_Indirect_dimensions_not_supporte, __pyx_k_Indirect_dimensions_not_supporte, sizeof(__pyx_k_Indirect_dimensions_not_supporte), 0, 0, 1, 0},
   {&__pyx_kp_s_Invalid_mode_expected_c_or_fortr, __pyx_k_Invalid_mode_expected_c_or_fortr, sizeof(__pyx_k_Invalid_mode_expected_c_or_fortr), 0, 0, 1, 0},
   {&__pyx_kp_s_Invalid_shape_in_axis_d_d, __pyx_k_Invalid_shape_in_axis_d_d, sizeof(__pyx_k_Invalid_shape_in_axis_d_d), 0, 0, 1, 0},
   {&__pyx_n_s_MemoryError, __pyx_k_MemoryError, sizeof(__pyx_k_MemoryError), 0, 0, 1, 1},
   {&__pyx_kp_s_MemoryView_of_r_at_0x_x, __pyx_k_MemoryView_of_r_at_0x_x, sizeof(__pyx_k_MemoryView_of_r_at_0x_x), 0, 0, 1, 0},
   {&__pyx_kp_s_MemoryView_of_r_object, __pyx_k_MemoryView_of_r_object, sizeof(__pyx_k_MemoryView_of_r_object), 0, 0, 1, 0},
-  {&__pyx_kp_u_Non_native_byte_order_not_suppor, __pyx_k_Non_native_byte_order_not_suppor, sizeof(__pyx_k_Non_native_byte_order_not_suppor), 0, 1, 0, 0},
   {&__pyx_n_b_O, __pyx_k_O, sizeof(__pyx_k_O), 0, 0, 0, 1},
   {&__pyx_kp_s_Out_of_bounds_on_buffer_access_a, __pyx_k_Out_of_bounds_on_buffer_access_a, sizeof(__pyx_k_Out_of_bounds_on_buffer_access_a), 0, 0, 1, 0},
   {&__pyx_n_s_P, __pyx_k_P, sizeof(__pyx_k_P), 0, 0, 1, 1},
   {&__pyx_n_s_P_data, __pyx_k_P_data, sizeof(__pyx_k_P_data), 0, 0, 1, 1},
   {&__pyx_n_s_PickleError, __pyx_k_PickleError, sizeof(__pyx_k_PickleError), 0, 0, 1, 1},
-  {&__pyx_n_s_RuntimeError, __pyx_k_RuntimeError, sizeof(__pyx_k_RuntimeError), 0, 0, 1, 1},
   {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
   {&__pyx_kp_s_Unable_to_convert_item_to_object, __pyx_k_Unable_to_convert_item_to_object, sizeof(__pyx_k_Unable_to_convert_item_to_object), 0, 0, 1, 0},
   {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
   {&__pyx_n_s_View_MemoryView, __pyx_k_View_MemoryView, sizeof(__pyx_k_View_MemoryView), 0, 0, 1, 1},
   {&__pyx_n_s_allocate_buffer, __pyx_k_allocate_buffer, sizeof(__pyx_k_allocate_buffer), 0, 0, 1, 1},
   {&__pyx_n_s_base, __pyx_k_base, sizeof(__pyx_k_base), 0, 0, 1, 1},
   {&__pyx_n_s_c, __pyx_k_c, sizeof(__pyx_k_c), 0, 0, 1, 1},
@@ -20924,16 +19476,14 @@
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
   {&__pyx_n_s_memview, __pyx_k_memview, sizeof(__pyx_k_memview), 0, 0, 1, 1},
   {&__pyx_n_s_min_num_intervals, __pyx_k_min_num_intervals, sizeof(__pyx_k_min_num_intervals), 0, 0, 1, 1},
   {&__pyx_n_s_mode, __pyx_k_mode, sizeof(__pyx_k_mode), 0, 0, 1, 1},
   {&__pyx_n_s_n_interpolation_points, __pyx_k_n_interpolation_points, sizeof(__pyx_k_n_interpolation_points), 0, 0, 1, 1},
   {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
   {&__pyx_n_s_name_2, __pyx_k_name_2, sizeof(__pyx_k_name_2), 0, 0, 1, 1},
-  {&__pyx_kp_u_ndarray_is_not_C_contiguous, __pyx_k_ndarray_is_not_C_contiguous, sizeof(__pyx_k_ndarray_is_not_C_contiguous), 0, 1, 0, 0},
-  {&__pyx_kp_u_ndarray_is_not_Fortran_contiguou, __pyx_k_ndarray_is_not_Fortran_contiguou, sizeof(__pyx_k_ndarray_is_not_Fortran_contiguou), 0, 1, 0, 0},
   {&__pyx_n_s_ndim, __pyx_k_ndim, sizeof(__pyx_k_ndim), 0, 0, 1, 1},
   {&__pyx_n_s_new, __pyx_k_new, sizeof(__pyx_k_new), 0, 0, 1, 1},
   {&__pyx_kp_s_no_default___reduce___due_to_non, __pyx_k_no_default___reduce___due_to_non, sizeof(__pyx_k_no_default___reduce___due_to_non), 0, 0, 1, 0},
   {&__pyx_n_s_np, __pyx_k_np, sizeof(__pyx_k_np), 0, 0, 1, 1},
   {&__pyx_n_s_numpy, __pyx_k_numpy, sizeof(__pyx_k_numpy), 0, 0, 1, 1},
   {&__pyx_kp_u_numpy_core_multiarray_failed_to, __pyx_k_numpy_core_multiarray_failed_to, sizeof(__pyx_k_numpy_core_multiarray_failed_to), 0, 1, 0, 0},
   {&__pyx_kp_u_numpy_core_umath_failed_to_impor, __pyx_k_numpy_core_umath_failed_to_impor, sizeof(__pyx_k_numpy_core_umath_failed_to_impor), 0, 1, 0, 0},
@@ -20967,24 +19517,22 @@
   {&__pyx_kp_s_stringsource, __pyx_k_stringsource, sizeof(__pyx_k_stringsource), 0, 0, 1, 0},
   {&__pyx_n_s_struct, __pyx_k_struct, sizeof(__pyx_k_struct), 0, 0, 1, 1},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_n_s_theta, __pyx_k_theta, sizeof(__pyx_k_theta), 0, 0, 1, 1},
   {&__pyx_n_s_tsne, __pyx_k_tsne, sizeof(__pyx_k_tsne), 0, 0, 1, 1},
   {&__pyx_kp_s_unable_to_allocate_array_data, __pyx_k_unable_to_allocate_array_data, sizeof(__pyx_k_unable_to_allocate_array_data), 0, 0, 1, 0},
   {&__pyx_kp_s_unable_to_allocate_shape_and_str, __pyx_k_unable_to_allocate_shape_and_str, sizeof(__pyx_k_unable_to_allocate_shape_and_str), 0, 0, 1, 0},
-  {&__pyx_kp_u_unknown_dtype_code_in_numpy_pxd, __pyx_k_unknown_dtype_code_in_numpy_pxd, sizeof(__pyx_k_unknown_dtype_code_in_numpy_pxd), 0, 1, 0, 0},
   {&__pyx_n_s_unpack, __pyx_k_unpack, sizeof(__pyx_k_unpack), 0, 0, 1, 1},
   {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 31, __pyx_L1_error)
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(1, 272, __pyx_L1_error)
-  __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(1, 855, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 1037, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 945, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(2, 134, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(2, 149, __pyx_L1_error)
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(2, 152, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(2, 2, __pyx_L1_error)
   __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(2, 406, __pyx_L1_error)
   __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(2, 615, __pyx_L1_error)
   __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(2, 834, __pyx_L1_error)
   return 0;
@@ -20992,350 +19540,295 @@
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":272
- *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_C_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not C contiguous")             # <<<<<<<<<<<<<<
- * 
- *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)
- */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_ndarray_is_not_C_contiguous); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 272, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple_);
-  __Pyx_GIVEREF(__pyx_tuple_);
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":276
- *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_F_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not Fortran contiguous")             # <<<<<<<<<<<<<<
- * 
- *             info.buf = PyArray_DATA(self)
- */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_ndarray_is_not_Fortran_contiguou); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 276, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__2);
-  __Pyx_GIVEREF(__pyx_tuple__2);
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":306
- *                 if ((descr.byteorder == c'>' and little_endian) or
- *                     (descr.byteorder == c'<' and not little_endian)):
- *                     raise ValueError(u"Non-native byte order not supported")             # <<<<<<<<<<<<<<
- *                 if   t == NPY_BYTE:        f = "b"
- *                 elif t == NPY_UBYTE:       f = "B"
- */
-  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_Non_native_byte_order_not_suppor); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 306, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__3);
-  __Pyx_GIVEREF(__pyx_tuple__3);
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":855
- * 
- *         if (end - f) - <int>(new_offset - offset[0]) < 15:
- *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")             # <<<<<<<<<<<<<<
- * 
- *         if ((child.byteorder == c'>' and little_endian) or
- */
-  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_u_Format_string_allocated_too_shor); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 855, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__4);
-  __Pyx_GIVEREF(__pyx_tuple__4);
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":879
- *             t = child.type_num
- *             if end - f < 5:
- *                 raise RuntimeError(u"Format string allocated too short.")             # <<<<<<<<<<<<<<
- * 
- *             # Until ticket #99 is fixed, use integers to avoid warnings
- */
-  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_u_Format_string_allocated_too_shor_2); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(1, 879, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__5);
-  __Pyx_GIVEREF(__pyx_tuple__5);
-
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1037
- *         _import_array()
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":945
+ *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(1, 1037, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__6);
-  __Pyx_GIVEREF(__pyx_tuple__6);
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 945, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple_);
+  __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../../../../tmp/build-env-0449cl2j/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1043
+  /* "../../../../../tmp/build-env-g728jl9l/lib/python3.10/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(1, 1043, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__7);
-  __Pyx_GIVEREF(__pyx_tuple__7);
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 951, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__2);
+  __Pyx_GIVEREF(__pyx_tuple__2);
 
   /* "View.MemoryView":134
  * 
  *         if not self.ndim:
  *             raise ValueError("Empty shape tuple for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if itemsize <= 0:
  */
-  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_s_Empty_shape_tuple_for_cython_arr); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(2, 134, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__8);
-  __Pyx_GIVEREF(__pyx_tuple__8);
+  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_s_Empty_shape_tuple_for_cython_arr); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(2, 134, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__3);
+  __Pyx_GIVEREF(__pyx_tuple__3);
 
   /* "View.MemoryView":137
  * 
  *         if itemsize <= 0:
  *             raise ValueError("itemsize <= 0 for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if not isinstance(format, bytes):
  */
-  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_s_itemsize_0_for_cython_array); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 137, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__9);
-  __Pyx_GIVEREF(__pyx_tuple__9);
+  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_s_itemsize_0_for_cython_array); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(2, 137, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__4);
+  __Pyx_GIVEREF(__pyx_tuple__4);
 
   /* "View.MemoryView":149
  * 
  *         if not self._shape:
  *             raise MemoryError("unable to allocate shape and strides.")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_shape_and_str); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 149, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__10);
-  __Pyx_GIVEREF(__pyx_tuple__10);
+  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_shape_and_str); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(2, 149, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__5);
+  __Pyx_GIVEREF(__pyx_tuple__5);
 
   /* "View.MemoryView":177
  *             self.data = <char *>malloc(self.len)
  *             if not self.data:
  *                 raise MemoryError("unable to allocate array data.")             # <<<<<<<<<<<<<<
  * 
  *             if self.dtype_is_object:
  */
-  __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_array_data); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(2, 177, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__11);
-  __Pyx_GIVEREF(__pyx_tuple__11);
+  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_array_data); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(2, 177, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__6);
+  __Pyx_GIVEREF(__pyx_tuple__6);
 
   /* "View.MemoryView":193
  *             bufmode = PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         if not (flags & bufmode):
  *             raise ValueError("Can only create a buffer that is contiguous in memory.")             # <<<<<<<<<<<<<<
  *         info.buf = self.data
  *         info.len = self.len
  */
-  __pyx_tuple__12 = PyTuple_Pack(1, __pyx_kp_s_Can_only_create_a_buffer_that_is); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(2, 193, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__12);
-  __Pyx_GIVEREF(__pyx_tuple__12);
+  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_s_Can_only_create_a_buffer_that_is); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(2, 193, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__7);
+  __Pyx_GIVEREF(__pyx_tuple__7);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_tuple__13 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(2, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__13);
-  __Pyx_GIVEREF(__pyx_tuple__13);
+  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(2, 2, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__8);
+  __Pyx_GIVEREF(__pyx_tuple__8);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__14 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(2, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__14);
-  __Pyx_GIVEREF(__pyx_tuple__14);
+  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__9);
+  __Pyx_GIVEREF(__pyx_tuple__9);
 
   /* "View.MemoryView":420
  *     def __setitem__(memoryview self, object index, object value):
  *         if self.view.readonly:
  *             raise TypeError("Cannot assign to read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         have_slices, index = _unellipsify(index, self.view.ndim)
  */
-  __pyx_tuple__15 = PyTuple_Pack(1, __pyx_kp_s_Cannot_assign_to_read_only_memor); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(2, 420, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__15);
-  __Pyx_GIVEREF(__pyx_tuple__15);
+  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_s_Cannot_assign_to_read_only_memor); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 420, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__10);
+  __Pyx_GIVEREF(__pyx_tuple__10);
 
   /* "View.MemoryView":497
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:
  *             raise ValueError("Unable to convert item to object")             # <<<<<<<<<<<<<<
  *         else:
  *             if len(self.view.format) == 1:
  */
-  __pyx_tuple__16 = PyTuple_Pack(1, __pyx_kp_s_Unable_to_convert_item_to_object); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(2, 497, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__16);
-  __Pyx_GIVEREF(__pyx_tuple__16);
+  __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_s_Unable_to_convert_item_to_object); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(2, 497, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__11);
+  __Pyx_GIVEREF(__pyx_tuple__11);
 
   /* "View.MemoryView":522
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         if flags & PyBUF_WRITABLE and self.view.readonly:
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_ND:
  */
-  __pyx_tuple__17 = PyTuple_Pack(1, __pyx_kp_s_Cannot_create_writable_memory_vi); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(2, 522, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__17);
-  __Pyx_GIVEREF(__pyx_tuple__17);
+  __pyx_tuple__12 = PyTuple_Pack(1, __pyx_kp_s_Cannot_create_writable_memory_vi); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(2, 522, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__12);
+  __Pyx_GIVEREF(__pyx_tuple__12);
 
   /* "View.MemoryView":572
  *         if self.view.strides == NULL:
  * 
  *             raise ValueError("Buffer view does not expose strides")             # <<<<<<<<<<<<<<
  * 
  *         return tuple([stride for stride in self.view.strides[:self.view.ndim]])
  */
-  __pyx_tuple__18 = PyTuple_Pack(1, __pyx_kp_s_Buffer_view_does_not_expose_stri); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(2, 572, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__18);
-  __Pyx_GIVEREF(__pyx_tuple__18);
+  __pyx_tuple__13 = PyTuple_Pack(1, __pyx_kp_s_Buffer_view_does_not_expose_stri); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(2, 572, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__13);
+  __Pyx_GIVEREF(__pyx_tuple__13);
 
   /* "View.MemoryView":579
  *     def suboffsets(self):
  *         if self.view.suboffsets == NULL:
  *             return (-1,) * self.view.ndim             # <<<<<<<<<<<<<<
  * 
  *         return tuple([suboffset for suboffset in self.view.suboffsets[:self.view.ndim]])
  */
-  __pyx_tuple__19 = PyTuple_New(1); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(2, 579, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__19);
+  __pyx_tuple__14 = PyTuple_New(1); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(2, 579, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__14);
   __Pyx_INCREF(__pyx_int_neg_1);
   __Pyx_GIVEREF(__pyx_int_neg_1);
-  PyTuple_SET_ITEM(__pyx_tuple__19, 0, __pyx_int_neg_1);
-  __Pyx_GIVEREF(__pyx_tuple__19);
+  PyTuple_SET_ITEM(__pyx_tuple__14, 0, __pyx_int_neg_1);
+  __Pyx_GIVEREF(__pyx_tuple__14);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_tuple__20 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(2, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__20);
-  __Pyx_GIVEREF(__pyx_tuple__20);
+  __pyx_tuple__15 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(2, 2, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__15);
+  __Pyx_GIVEREF(__pyx_tuple__15);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__21 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(2, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__21);
-  __Pyx_GIVEREF(__pyx_tuple__21);
+  __pyx_tuple__16 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__16);
+  __Pyx_GIVEREF(__pyx_tuple__16);
 
   /* "View.MemoryView":684
  *         if item is Ellipsis:
  *             if not seen_ellipsis:
  *                 result.extend([slice(None)] * (ndim - len(tup) + 1))             # <<<<<<<<<<<<<<
  *                 seen_ellipsis = True
  *             else:
  */
-  __pyx_slice__22 = PySlice_New(Py_None, Py_None, Py_None); if (unlikely(!__pyx_slice__22)) __PYX_ERR(2, 684, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_slice__22);
-  __Pyx_GIVEREF(__pyx_slice__22);
+  __pyx_slice__17 = PySlice_New(Py_None, Py_None, Py_None); if (unlikely(!__pyx_slice__17)) __PYX_ERR(2, 684, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_slice__17);
+  __Pyx_GIVEREF(__pyx_slice__17);
 
   /* "View.MemoryView":705
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:
  *             raise ValueError("Indirect dimensions not supported")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__23 = PyTuple_Pack(1, __pyx_kp_s_Indirect_dimensions_not_supporte); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(2, 705, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__23);
-  __Pyx_GIVEREF(__pyx_tuple__23);
+  __pyx_tuple__18 = PyTuple_Pack(1, __pyx_kp_s_Indirect_dimensions_not_supporte); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(2, 705, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__18);
+  __Pyx_GIVEREF(__pyx_tuple__18);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_tuple__24 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(2, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__24);
-  __Pyx_GIVEREF(__pyx_tuple__24);
+  __pyx_tuple__19 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(2, 2, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__19);
+  __Pyx_GIVEREF(__pyx_tuple__19);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__25 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(2, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__25);
-  __Pyx_GIVEREF(__pyx_tuple__25);
-  __pyx_tuple__26 = PyTuple_Pack(3, __pyx_int_184977713, __pyx_int_136983863, __pyx_int_112105877); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(2, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__26);
-  __Pyx_GIVEREF(__pyx_tuple__26);
+  __pyx_tuple__20 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__20);
+  __Pyx_GIVEREF(__pyx_tuple__20);
+  __pyx_tuple__21 = PyTuple_Pack(3, __pyx_int_184977713, __pyx_int_136983863, __pyx_int_112105877); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__21);
+  __Pyx_GIVEREF(__pyx_tuple__21);
 
   /* "View.MemoryView":287
  *         return self.name
  * 
  * cdef generic = Enum("<strided and direct or indirect>")             # <<<<<<<<<<<<<<
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")
  */
-  __pyx_tuple__27 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct_or_indirect); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(2, 287, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__27);
-  __Pyx_GIVEREF(__pyx_tuple__27);
+  __pyx_tuple__22 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct_or_indirect); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(2, 287, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__22);
+  __Pyx_GIVEREF(__pyx_tuple__22);
 
   /* "View.MemoryView":288
  * 
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default             # <<<<<<<<<<<<<<
  * cdef indirect = Enum("<strided and indirect>")
  * 
  */
-  __pyx_tuple__28 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(2, 288, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__28);
-  __Pyx_GIVEREF(__pyx_tuple__28);
+  __pyx_tuple__23 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(2, 288, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__23);
+  __Pyx_GIVEREF(__pyx_tuple__23);
 
   /* "View.MemoryView":289
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__29 = PyTuple_Pack(1, __pyx_kp_s_strided_and_indirect); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(2, 289, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__29);
-  __Pyx_GIVEREF(__pyx_tuple__29);
+  __pyx_tuple__24 = PyTuple_Pack(1, __pyx_kp_s_strided_and_indirect); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(2, 289, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__24);
+  __Pyx_GIVEREF(__pyx_tuple__24);
 
   /* "View.MemoryView":292
  * 
  * 
  * cdef contiguous = Enum("<contiguous and direct>")             # <<<<<<<<<<<<<<
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")
  * 
  */
-  __pyx_tuple__30 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_direct); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(2, 292, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__30);
-  __Pyx_GIVEREF(__pyx_tuple__30);
+  __pyx_tuple__25 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_direct); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(2, 292, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__25);
+  __Pyx_GIVEREF(__pyx_tuple__25);
 
   /* "View.MemoryView":293
  * 
  * cdef contiguous = Enum("<contiguous and direct>")
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__31 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_indirect); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(2, 293, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__31);
-  __Pyx_GIVEREF(__pyx_tuple__31);
+  __pyx_tuple__26 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_indirect); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(2, 293, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__26);
+  __Pyx_GIVEREF(__pyx_tuple__26);
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_Enum(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_tuple__32 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__32)) __PYX_ERR(2, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__32);
-  __Pyx_GIVEREF(__pyx_tuple__32);
-  __pyx_codeobj__33 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__32, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Enum, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__33)) __PYX_ERR(2, 1, __pyx_L1_error)
+  __pyx_tuple__27 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(2, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__27);
+  __Pyx_GIVEREF(__pyx_tuple__27);
+  __pyx_codeobj__28 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__27, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Enum, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__28)) __PYX_ERR(2, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -21462,37 +19955,73 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 206, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 200, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 206, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 229, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 233, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 242, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 917, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT(PyArray_Descr),
+  __Pyx_ImportType_CheckSize_Ignore);
+   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 200, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
+   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 223, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayMultiIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
+   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 227, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayObject),
+  __Pyx_ImportType_CheckSize_Ignore);
+   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 239, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 771, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 773, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 775, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 777, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 779, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 781, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 783, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 785, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 787, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 789, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT(PyUFuncObject),
+  __Pyx_ImportType_CheckSize_Ignore);
+   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 827, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("openTSNE.quad_tree"); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 23, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_8openTSNE_9quad_tree_QuadTree = __Pyx_ImportType(__pyx_t_1, "openTSNE.quad_tree", "QuadTree", sizeof(struct __pyx_obj_8openTSNE_9quad_tree_QuadTree), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_8openTSNE_9quad_tree_QuadTree = __Pyx_ImportType(__pyx_t_1, "openTSNE.quad_tree", "QuadTree", sizeof(struct __pyx_obj_8openTSNE_9quad_tree_QuadTree), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_8openTSNE_9quad_tree_QuadTree),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_8openTSNE_9quad_tree_QuadTree) __PYX_ERR(4, 23, __pyx_L1_error)
   __pyx_vtabptr_8openTSNE_9quad_tree_QuadTree = (struct __pyx_vtabstruct_8openTSNE_9quad_tree_QuadTree*)__Pyx_GetVtable(__pyx_ptype_8openTSNE_9quad_tree_QuadTree->tp_dict); if (unlikely(!__pyx_vtabptr_8openTSNE_9quad_tree_QuadTree)) __PYX_ERR(4, 23, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
@@ -21821,71 +20350,71 @@
   /* "View.MemoryView":287
  *         return self.name
  * 
  * cdef generic = Enum("<strided and direct or indirect>")             # <<<<<<<<<<<<<<
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")
  */
-  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__27, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 287, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__22, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 287, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_XGOTREF(generic);
   __Pyx_DECREF_SET(generic, __pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_3);
   __pyx_t_3 = 0;
 
   /* "View.MemoryView":288
  * 
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default             # <<<<<<<<<<<<<<
  * cdef indirect = Enum("<strided and indirect>")
  * 
  */
-  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__28, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 288, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__23, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 288, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_XGOTREF(strided);
   __Pyx_DECREF_SET(strided, __pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_3);
   __pyx_t_3 = 0;
 
   /* "View.MemoryView":289
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__29, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 289, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__24, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 289, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_XGOTREF(indirect);
   __Pyx_DECREF_SET(indirect, __pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_3);
   __pyx_t_3 = 0;
 
   /* "View.MemoryView":292
  * 
  * 
  * cdef contiguous = Enum("<contiguous and direct>")             # <<<<<<<<<<<<<<
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")
  * 
  */
-  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__30, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 292, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__25, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 292, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_XGOTREF(contiguous);
   __Pyx_DECREF_SET(contiguous, __pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_3);
   __pyx_t_3 = 0;
 
   /* "View.MemoryView":293
  * 
  * cdef contiguous = Enum("<contiguous and direct>")
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__31, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 293, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__26, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 293, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_XGOTREF(indirect_contiguous);
   __Pyx_DECREF_SET(indirect_contiguous, __pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_3);
   __pyx_t_3 = 0;
 
   /* "View.MemoryView":317
@@ -22851,215 +21380,14 @@
             return __Pyx_PyObject_CallMethO(func, NULL);
         }
     }
     return __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL);
 }
 #endif
 
-/* RaiseException */
-#if PY_MAJOR_VERSION < 3
-static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb,
-                        CYTHON_UNUSED PyObject *cause) {
-    __Pyx_PyThreadState_declare
-    Py_XINCREF(type);
-    if (!value || value == Py_None)
-        value = NULL;
-    else
-        Py_INCREF(value);
-    if (!tb || tb == Py_None)
-        tb = NULL;
-    else {
-        Py_INCREF(tb);
-        if (!PyTraceBack_Check(tb)) {
-            PyErr_SetString(PyExc_TypeError,
-                "raise: arg 3 must be a traceback or None");
-            goto raise_error;
-        }
-    }
-    if (PyType_Check(type)) {
-#if CYTHON_COMPILING_IN_PYPY
-        if (!value) {
-            Py_INCREF(Py_None);
-            value = Py_None;
-        }
-#endif
-        PyErr_NormalizeException(&type, &value, &tb);
-    } else {
-        if (value) {
-            PyErr_SetString(PyExc_TypeError,
-                "instance exception may not have a separate value");
-            goto raise_error;
-        }
-        value = type;
-        type = (PyObject*) Py_TYPE(type);
-        Py_INCREF(type);
-        if (!PyType_IsSubtype((PyTypeObject *)type, (PyTypeObject *)PyExc_BaseException)) {
-            PyErr_SetString(PyExc_TypeError,
-                "raise: exception class must be a subclass of BaseException");
-            goto raise_error;
-        }
-    }
-    __Pyx_PyThreadState_assign
-    __Pyx_ErrRestore(type, value, tb);
-    return;
-raise_error:
-    Py_XDECREF(value);
-    Py_XDECREF(type);
-    Py_XDECREF(tb);
-    return;
-}
-#else
-static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause) {
-    PyObject* owned_instance = NULL;
-    if (tb == Py_None) {
-        tb = 0;
-    } else if (tb && !PyTraceBack_Check(tb)) {
-        PyErr_SetString(PyExc_TypeError,
-            "raise: arg 3 must be a traceback or None");
-        goto bad;
-    }
-    if (value == Py_None)
-        value = 0;
-    if (PyExceptionInstance_Check(type)) {
-        if (value) {
-            PyErr_SetString(PyExc_TypeError,
-                "instance exception may not have a separate value");
-            goto bad;
-        }
-        value = type;
-        type = (PyObject*) Py_TYPE(value);
-    } else if (PyExceptionClass_Check(type)) {
-        PyObject *instance_class = NULL;
-        if (value && PyExceptionInstance_Check(value)) {
-            instance_class = (PyObject*) Py_TYPE(value);
-            if (instance_class != type) {
-                int is_subclass = PyObject_IsSubclass(instance_class, type);
-                if (!is_subclass) {
-                    instance_class = NULL;
-                } else if (unlikely(is_subclass == -1)) {
-                    goto bad;
-                } else {
-                    type = instance_class;
-                }
-            }
-        }
-        if (!instance_class) {
-            PyObject *args;
-            if (!value)
-                args = PyTuple_New(0);
-            else if (PyTuple_Check(value)) {
-                Py_INCREF(value);
-                args = value;
-            } else
-                args = PyTuple_Pack(1, value);
-            if (!args)
-                goto bad;
-            owned_instance = PyObject_Call(type, args, NULL);
-            Py_DECREF(args);
-            if (!owned_instance)
-                goto bad;
-            value = owned_instance;
-            if (!PyExceptionInstance_Check(value)) {
-                PyErr_Format(PyExc_TypeError,
-                             "calling %R should have returned an instance of "
-                             "BaseException, not %R",
-                             type, Py_TYPE(value));
-                goto bad;
-            }
-        }
-    } else {
-        PyErr_SetString(PyExc_TypeError,
-            "raise: exception class must be a subclass of BaseException");
-        goto bad;
-    }
-    if (cause) {
-        PyObject *fixed_cause;
-        if (cause == Py_None) {
-            fixed_cause = NULL;
-        } else if (PyExceptionClass_Check(cause)) {
-            fixed_cause = PyObject_CallObject(cause, NULL);
-            if (fixed_cause == NULL)
-                goto bad;
-        } else if (PyExceptionInstance_Check(cause)) {
-            fixed_cause = cause;
-            Py_INCREF(fixed_cause);
-        } else {
-            PyErr_SetString(PyExc_TypeError,
-                            "exception causes must derive from "
-                            "BaseException");
-            goto bad;
-        }
-        PyException_SetCause(value, fixed_cause);
-    }
-    PyErr_SetObject(type, value);
-    if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
-        PyThreadState *tstate = __Pyx_PyThreadState_Current;
-        PyObject* tmp_tb = tstate->curexc_traceback;
-        if (tb != tmp_tb) {
-            Py_INCREF(tb);
-            tstate->curexc_traceback = tb;
-            Py_XDECREF(tmp_tb);
-        }
-#endif
-    }
-bad:
-    Py_XDECREF(owned_instance);
-    return;
-}
-#endif
-
-/* DictGetItem */
-#if PY_MAJOR_VERSION >= 3 && !CYTHON_COMPILING_IN_PYPY
-static PyObject *__Pyx_PyDict_GetItem(PyObject *d, PyObject* key) {
-    PyObject *value;
-    value = PyDict_GetItemWithError(d, key);
-    if (unlikely(!value)) {
-        if (!PyErr_Occurred()) {
-            if (unlikely(PyTuple_Check(key))) {
-                PyObject* args = PyTuple_Pack(1, key);
-                if (likely(args)) {
-                    PyErr_SetObject(PyExc_KeyError, args);
-                    Py_DECREF(args);
-                }
-            } else {
-                PyErr_SetObject(PyExc_KeyError, key);
-            }
-        }
-        return NULL;
-    }
-    Py_INCREF(value);
-    return value;
-}
-#endif
-
-/* RaiseNoneIterError */
-static CYTHON_INLINE void __Pyx_RaiseNoneNotIterableError(void) {
-    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-}
-
-/* ExtTypeTest */
-static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type) {
-    if (unlikely(!type)) {
-        PyErr_SetString(PyExc_SystemError, "Missing type object");
-        return 0;
-    }
-    if (likely(__Pyx_TypeCheck(obj, type)))
-        return 1;
-    PyErr_Format(PyExc_TypeError, "Cannot convert %.200s to %.200s",
-                 Py_TYPE(obj)->tp_name, type->tp_name);
-    return 0;
-}
-
 /* GetTopmostException */
 #if CYTHON_USE_EXC_INFO_STACK
 static _PyErr_StackItem *
 __Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
 {
     _PyErr_StackItem *exc_info = tstate->exc_info;
     while ((exc_info->exc_type == NULL || exc_info->exc_type == Py_None) &&
@@ -23207,14 +21535,173 @@
     *tb = 0;
     Py_XDECREF(local_type);
     Py_XDECREF(local_value);
     Py_XDECREF(local_tb);
     return -1;
 }
 
+/* RaiseException */
+#if PY_MAJOR_VERSION < 3
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb,
+                        CYTHON_UNUSED PyObject *cause) {
+    __Pyx_PyThreadState_declare
+    Py_XINCREF(type);
+    if (!value || value == Py_None)
+        value = NULL;
+    else
+        Py_INCREF(value);
+    if (!tb || tb == Py_None)
+        tb = NULL;
+    else {
+        Py_INCREF(tb);
+        if (!PyTraceBack_Check(tb)) {
+            PyErr_SetString(PyExc_TypeError,
+                "raise: arg 3 must be a traceback or None");
+            goto raise_error;
+        }
+    }
+    if (PyType_Check(type)) {
+#if CYTHON_COMPILING_IN_PYPY
+        if (!value) {
+            Py_INCREF(Py_None);
+            value = Py_None;
+        }
+#endif
+        PyErr_NormalizeException(&type, &value, &tb);
+    } else {
+        if (value) {
+            PyErr_SetString(PyExc_TypeError,
+                "instance exception may not have a separate value");
+            goto raise_error;
+        }
+        value = type;
+        type = (PyObject*) Py_TYPE(type);
+        Py_INCREF(type);
+        if (!PyType_IsSubtype((PyTypeObject *)type, (PyTypeObject *)PyExc_BaseException)) {
+            PyErr_SetString(PyExc_TypeError,
+                "raise: exception class must be a subclass of BaseException");
+            goto raise_error;
+        }
+    }
+    __Pyx_PyThreadState_assign
+    __Pyx_ErrRestore(type, value, tb);
+    return;
+raise_error:
+    Py_XDECREF(value);
+    Py_XDECREF(type);
+    Py_XDECREF(tb);
+    return;
+}
+#else
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause) {
+    PyObject* owned_instance = NULL;
+    if (tb == Py_None) {
+        tb = 0;
+    } else if (tb && !PyTraceBack_Check(tb)) {
+        PyErr_SetString(PyExc_TypeError,
+            "raise: arg 3 must be a traceback or None");
+        goto bad;
+    }
+    if (value == Py_None)
+        value = 0;
+    if (PyExceptionInstance_Check(type)) {
+        if (value) {
+            PyErr_SetString(PyExc_TypeError,
+                "instance exception may not have a separate value");
+            goto bad;
+        }
+        value = type;
+        type = (PyObject*) Py_TYPE(value);
+    } else if (PyExceptionClass_Check(type)) {
+        PyObject *instance_class = NULL;
+        if (value && PyExceptionInstance_Check(value)) {
+            instance_class = (PyObject*) Py_TYPE(value);
+            if (instance_class != type) {
+                int is_subclass = PyObject_IsSubclass(instance_class, type);
+                if (!is_subclass) {
+                    instance_class = NULL;
+                } else if (unlikely(is_subclass == -1)) {
+                    goto bad;
+                } else {
+                    type = instance_class;
+                }
+            }
+        }
+        if (!instance_class) {
+            PyObject *args;
+            if (!value)
+                args = PyTuple_New(0);
+            else if (PyTuple_Check(value)) {
+                Py_INCREF(value);
+                args = value;
+            } else
+                args = PyTuple_Pack(1, value);
+            if (!args)
+                goto bad;
+            owned_instance = PyObject_Call(type, args, NULL);
+            Py_DECREF(args);
+            if (!owned_instance)
+                goto bad;
+            value = owned_instance;
+            if (!PyExceptionInstance_Check(value)) {
+                PyErr_Format(PyExc_TypeError,
+                             "calling %R should have returned an instance of "
+                             "BaseException, not %R",
+                             type, Py_TYPE(value));
+                goto bad;
+            }
+        }
+    } else {
+        PyErr_SetString(PyExc_TypeError,
+            "raise: exception class must be a subclass of BaseException");
+        goto bad;
+    }
+    if (cause) {
+        PyObject *fixed_cause;
+        if (cause == Py_None) {
+            fixed_cause = NULL;
+        } else if (PyExceptionClass_Check(cause)) {
+            fixed_cause = PyObject_CallObject(cause, NULL);
+            if (fixed_cause == NULL)
+                goto bad;
+        } else if (PyExceptionInstance_Check(cause)) {
+            fixed_cause = cause;
+            Py_INCREF(fixed_cause);
+        } else {
+            PyErr_SetString(PyExc_TypeError,
+                            "exception causes must derive from "
+                            "BaseException");
+            goto bad;
+        }
+        PyException_SetCause(value, fixed_cause);
+    }
+    PyErr_SetObject(type, value);
+    if (tb) {
+#if CYTHON_FAST_THREAD_STATE
+        PyThreadState *tstate = __Pyx_PyThreadState_Current;
+        PyObject* tmp_tb = tstate->curexc_traceback;
+        if (tb != tmp_tb) {
+            Py_INCREF(tb);
+            tstate->curexc_traceback = tb;
+            Py_XDECREF(tmp_tb);
+        }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
+#endif
+    }
+bad:
+    Py_XDECREF(owned_instance);
+    return;
+}
+#endif
+
 /* ArgTypeTest */
 static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact)
 {
     if (unlikely(!type)) {
         PyErr_SetString(PyExc_SystemError, "Missing type object");
         return 0;
     }
@@ -23583,14 +22070,32 @@
     return d;
 }
 static CYTHON_INLINE PyObject *__Pyx_GetAttr3(PyObject *o, PyObject *n, PyObject *d) {
     PyObject *r = __Pyx_GetAttr(o, n);
     return (likely(r)) ? r : __Pyx_GetAttr3Default(d);
 }
 
+/* RaiseNoneIterError */
+static CYTHON_INLINE void __Pyx_RaiseNoneNotIterableError(void) {
+    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
+}
+
+/* ExtTypeTest */
+static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type) {
+    if (unlikely(!type)) {
+        PyErr_SetString(PyExc_SystemError, "Missing type object");
+        return 0;
+    }
+    if (likely(__Pyx_TypeCheck(obj, type)))
+        return 1;
+    PyErr_Format(PyExc_TypeError, "Cannot convert %.200s to %.200s",
+                 Py_TYPE(obj)->tp_name, type->tp_name);
+    return 0;
+}
+
 /* SwapException */
 #if CYTHON_FAST_THREAD_STATE
 static CYTHON_INLINE void __Pyx__ExceptionSwap(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
     PyObject *tmp_type, *tmp_value, *tmp_tb;
     #if CYTHON_USE_EXC_INFO_STACK
     _PyErr_StackItem *exc_info = tstate->exc_info;
     tmp_type = exc_info->exc_type;
@@ -24142,44 +22647,62 @@
     return ret;
 }
 
 /* TypeImport */
 #ifndef __PYX_HAVE_RT_ImportType
 #define __PYX_HAVE_RT_ImportType
 static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
     if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
@@ -24451,29 +22974,27 @@
     Py_XDECREF(py_code);
     Py_XDECREF(py_frame);
 }
 
 #if PY_MAJOR_VERSION < 3
 static int __Pyx_GetBuffer(PyObject *obj, Py_buffer *view, int flags) {
     if (PyObject_CheckBuffer(obj)) return PyObject_GetBuffer(obj, view, flags);
-        if (__Pyx_TypeCheck(obj, __pyx_ptype_5numpy_ndarray)) return __pyx_pw_5numpy_7ndarray_1__getbuffer__(obj, view, flags);
         if (__Pyx_TypeCheck(obj, __pyx_array_type)) return __pyx_array_getbuffer(obj, view, flags);
         if (__Pyx_TypeCheck(obj, __pyx_memoryview_type)) return __pyx_memoryview_getbuffer(obj, view, flags);
     PyErr_Format(PyExc_TypeError, "'%.200s' does not have the buffer interface", Py_TYPE(obj)->tp_name);
     return -1;
 }
 static void __Pyx_ReleaseBuffer(Py_buffer *view) {
     PyObject *obj = view->obj;
     if (!obj) return;
     if (PyObject_CheckBuffer(obj)) {
         PyBuffer_Release(view);
         return;
     }
     if ((0)) {}
-        else if (__Pyx_TypeCheck(obj, __pyx_ptype_5numpy_ndarray)) __pyx_pw_5numpy_7ndarray_3__releasebuffer__(obj, view);
     view->obj = NULL;
     Py_DECREF(obj);
 }
 #endif
 
 
 /* MemviewSliceIsContig */
@@ -26025,52 +24546,14 @@
     return (int) -1;
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to int");
     return (int) -1;
 }
 
-/* CIntToPy */
-  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_enum__NPY_TYPES(enum NPY_TYPES value) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const enum NPY_TYPES neg_one = (enum NPY_TYPES) -1, const_zero = (enum NPY_TYPES) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
-    const int is_unsigned = neg_one > const_zero;
-    if (is_unsigned) {
-        if (sizeof(enum NPY_TYPES) < sizeof(long)) {
-            return PyInt_FromLong((long) value);
-        } else if (sizeof(enum NPY_TYPES) <= sizeof(unsigned long)) {
-            return PyLong_FromUnsignedLong((unsigned long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(enum NPY_TYPES) <= sizeof(unsigned PY_LONG_LONG)) {
-            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
-#endif
-        }
-    } else {
-        if (sizeof(enum NPY_TYPES) <= sizeof(long)) {
-            return PyInt_FromLong((long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(enum NPY_TYPES) <= sizeof(PY_LONG_LONG)) {
-            return PyLong_FromLongLong((PY_LONG_LONG) value);
-#endif
-        }
-    }
-    {
-        int one = 1; int little = (int)*(unsigned char *)&one;
-        unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(enum NPY_TYPES),
-                                     little, !is_unsigned);
-    }
-}
-
 /* CIntFromPy */
   static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const long neg_one = (long) -1, const_zero = (long) 0;
```

### Comparing `openTSNE-0.7.1/openTSNE/kl_divergence.pyx` & `openTSNE-1.0.0/openTSNE/kl_divergence.pyx`

 * *Files identical despite different names*

### Comparing `openTSNE-0.7.1/openTSNE/nearest_neighbors.py` & `openTSNE-1.0.0/openTSNE/nearest_neighbors.py`

 * *Files 2% similar despite different names*

```diff
@@ -389,14 +389,20 @@
         "braycurtis",
         "spearmanr",
         "tsss",
         "true_angular",
         "hellinger",
         "kantorovich",
         "wasserstein",
+        "wasserstein_1d",
+        "wasserstein-1d",
+        "kantorovich-1d",
+        "kantorovich_1d",
+        "circular_kantorovich",
+        "circular_wasserstein",
         "sinkhorn",
         "jensen-shannon",
         "jensen_shannon",
         "symmetric-kl",
         "symmetric_kl",
         "symmetric_kullback_liebler",
         "hamming",
```

### Comparing `openTSNE-0.7.1/openTSNE/quad_tree.cpp` & `openTSNE-1.0.0/openTSNE/quad_tree.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "language": "c++",
         "name": "openTSNE.quad_tree",
@@ -19,16 +19,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_33"
-#define CYTHON_HEX_VERSION 0x001D21F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -213,15 +213,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -252,15 +252,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -19650,28 +19650,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
```

### Comparing `openTSNE-0.7.1/openTSNE/quad_tree.pxd` & `openTSNE-1.0.0/openTSNE/quad_tree.pxd`

 * *Files identical despite different names*

### Comparing `openTSNE-0.7.1/openTSNE/quad_tree.pyx` & `openTSNE-1.0.0/openTSNE/quad_tree.pyx`

 * *Files identical despite different names*

### Comparing `openTSNE-0.7.1/openTSNE/sklearn.py` & `openTSNE-1.0.0/openTSNE/sklearn.py`

 * *Files identical despite different names*

### Comparing `openTSNE-0.7.1/openTSNE/tsne.py` & `openTSNE-1.0.0/openTSNE/tsne.py`

 * *Files identical despite different names*

### Comparing `openTSNE-0.7.1/openTSNE/utils.py` & `openTSNE-1.0.0/openTSNE/utils.py`

 * *Files identical despite different names*

### Comparing `openTSNE-0.7.1/openTSNE.egg-info/PKG-INFO` & `openTSNE-1.0.0/openTSNE.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openTSNE
-Version: 0.7.1
+Version: 1.0.0
 Summary: Extensible, parallel implementations of t-SNE
 Home-page: https://github.com/pavlin-policar/openTSNE
 Author: Pavlin Poličar
 Author-email: pavlin.g.p@gmail.com
 License: BSD-3-Clause
 Project-URL: Documentation, https://opentsne.readthedocs.io/
 Project-URL: Source, https://github.com/pavlin-policar/openTSNE
```

### Comparing `openTSNE-0.7.1/openTSNE.egg-info/SOURCES.txt` & `openTSNE-1.0.0/openTSNE.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openTSNE-0.7.1/setup.py` & `openTSNE-1.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `openTSNE-0.7.1/tests/test_affinities.py` & `openTSNE-1.0.0/tests/test_affinities.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,16 @@
 Uniform = partial(affinity.Uniform, method="exact")
 
 AFFINITY_CLASSES = [
     ("PerplexityBasedNN", PerplexityBasedNN),
     ("FixedSigmaNN", partial(FixedSigmaNN, sigma=1)),
     ("MultiscaleMixture", partial(MultiscaleMixture, perplexities=[10, 20])),
     ("Multiscale", partial(Multiscale, perplexities=[10, 20])),
-    ("Uniform", partial(Uniform, k_neighbors=5)),
+    ("UniformMean", partial(Uniform, k_neighbors=5, symmetrize="mean")),
+    ("UniformMax", partial(Uniform, k_neighbors=5, symmetrize="max")),
 ]
 
 
 class TestPerplexityBased(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
         cls.x = np.random.normal(100, 50, (91, 4))
@@ -62,15 +63,15 @@
         reduced_P = aff.P.copy()
         self.assertTrue(reduced_P.nnz >= n_samples * k_neighbors)
         self.assertTrue(reduced_P.nnz < original_P.nnz,
                         "Lower perplexities should consider less neighbors, "
                         "resulting in a sparser affinity matrix")
                         
         # Check that increasing the perplexity works (with a warning)
-        # Larger then the original perplexity, but still less than the number of
+        # Larger than the original perplexity, but still less than the number of
         # nearest neighbors
         perplexity = 40
         with self.assertLogs(affinity.log, level="WARNING"):
             aff.set_perplexity(perplexity)
             self.assertEqual(aff.perplexity, perplexity)
             self.assertEqual(aff.effective_perplexity_, perplexity)
 
@@ -249,14 +250,28 @@
 
         values = new_p.data
         np.testing.assert_allclose(values, values[0])
 
         new_p = new_p.toarray()
         np.testing.assert_allclose(new_p.sum(axis=1), np.ones(self.y.shape[0]))
 
+    def test_symmetrize_mean_has_two_distinct_values(self):
+        aff = Uniform(self.x, k_neighbors=10, symmetrize="mean")
+        values = aff.P.data
+        self.assertEqual(len(np.unique(values)), 2)
+
+    def test_symmetrize_max_has_one_distinct_value(self):
+        aff = Uniform(self.x, k_neighbors=10, symmetrize="max")
+        values = aff.P.data
+        self.assertEqual(len(np.unique(values)), 1)
+
+    def test_symmetrize_with_invalid_parameter(self):
+        with self.assertRaises(ValueError):
+            Uniform(self.x, k_neighbors=10, symmetrize="invalid")
+
 
 class TestAffinityMatrixCorrectness(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
         cls.iris = datasets.load_iris().data
 
     def test_that_regular_matrix_sums_to_one(self):
@@ -337,14 +352,15 @@
 
     def test_to_new(self):
         knn_index = nearest_neighbors.Sklearn(self.iris, k=30)
         for method_name, cls in AFFINITY_CLASSES:
             aff = cls(knn_index=knn_index)
             aff.to_new(self.iris)
 
+
 class TestPrecomputedAffinity(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
         cls.iris = datasets.load_iris().data
 
     def test_precomputed_affinity_matches(self):
         aff1 = PerplexityBasedNN(self.iris)
```

### Comparing `openTSNE-0.7.1/tests/test_correctness.py` & `openTSNE-1.0.0/tests/test_correctness.py`

 * *Files identical despite different names*

### Comparing `openTSNE-0.7.1/tests/test_different_usages.py` & `openTSNE-1.0.0/tests/test_different_usages.py`

 * *Files identical despite different names*

### Comparing `openTSNE-0.7.1/tests/test_nearest_neighbors.py` & `openTSNE-1.0.0/tests/test_nearest_neighbors.py`

 * *Files identical despite different names*

### Comparing `openTSNE-0.7.1/tests/test_sklearn_wrapper.py` & `openTSNE-1.0.0/tests/test_sklearn_wrapper.py`

 * *Files identical despite different names*

### Comparing `openTSNE-0.7.1/tests/test_tsne.py` & `openTSNE-1.0.0/tests/test_tsne.py`

 * *Files identical despite different names*

### Comparing `openTSNE-0.7.1/tests/test_utils.py` & `openTSNE-1.0.0/tests/test_utils.py`

 * *Files identical despite different names*

