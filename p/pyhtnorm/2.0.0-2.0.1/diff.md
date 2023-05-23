# Comparing `tmp/pyhtnorm-2.0.0.tar.gz` & `tmp/pyhtnorm-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhtnorm-2.0.0.tar", last modified: Sun Apr  4 22:57:14 2021, max compression
+gzip compressed data, was "pyhtnorm-2.0.1.tar", last modified: Tue May 23 23:31:54 2023, max compression
```

## Comparing `pyhtnorm-2.0.0.tar` & `pyhtnorm-2.0.1.tar`

### file list

```diff
@@ -1,25 +1,38 @@
--rw-r--r--   0        0        0     1513 2020-12-05 11:30:07.938351 pyhtnorm-2.0.0/LICENSE
--rw-r--r--   0        0        0     8095 2021-04-04 20:47:22.862400 pyhtnorm-2.0.0/README.md
--rw-r--r--   0        0        0     1164 2021-04-04 20:30:47.875703 pyhtnorm-2.0.0/build.py
--rw-r--r--   0        0        0     4663 2021-04-04 19:57:52.978977 pyhtnorm-2.0.0/include/htnorm.h
--rw-r--r--   0        0        0     1815 2021-01-18 17:40:56.921567 pyhtnorm-2.0.0/include/htnorm_rng.h
--rw-r--r--   0        0        0      100 2021-04-04 17:28:56.515377 pyhtnorm-2.0.0/pyhtnorm/__init__.py
--rw-r--r--   0        0        0   935772 2021-04-04 22:41:49.849275 pyhtnorm-2.0.0/pyhtnorm/_htnorm.c
--rw-r--r--   0        0        0     1084 2021-04-04 20:51:02.572406 pyhtnorm-2.0.0/pyproject.toml
--rw-r--r--   0        0        0    10300 2021-04-04 20:21:51.209020 pyhtnorm-2.0.0/src/htnorm.c
--rw-r--r--   0        0        0      724 2021-04-04 20:18:22.895681 pyhtnorm-2.0.0/src/htnorm_always_inline.h
--rw-r--r--   0        0        0     5268 2020-12-24 08:51:59.483338 pyhtnorm-2.0.0/src/htnorm_blas.h
--rw-r--r--   0        0        0     4002 2021-04-04 20:09:31.355665 pyhtnorm-2.0.0/src/htnorm_distributions.c
--rw-r--r--   0        0        0     3193 2021-04-04 20:30:39.915703 pyhtnorm-2.0.0/src/htnorm_distributions.h
--rw-r--r--   0        0        0      857 2021-04-04 20:10:40.195667 pyhtnorm-2.0.0/src/htnorm_pcg32_minimal.h
--rw-r--r--   0        0        0     1117 2021-04-04 20:13:14.009005 pyhtnorm-2.0.0/src/htnorm_pcg64.h
--rw-r--r--   0        0        0     3104 2021-04-04 20:14:38.535674 pyhtnorm-2.0.0/src/htnorm_r_wrapper.c
--rw-r--r--   0        0        0     1424 2021-04-04 20:25:32.429027 pyhtnorm-2.0.0/src/htnorm_rng.c
--rw-r--r--   0        0        0      799 2021-04-04 20:11:42.752335 pyhtnorm-2.0.0/src/htnorm_splitmix64.h
--rw-r--r--   0        0        0     1061 2021-04-04 20:15:31.555676 pyhtnorm-2.0.0/src/htnorm_xoroshiro128p.h
--rw-r--r--   0        0        0    21851 2020-12-20 23:49:30.834462 pyhtnorm-2.0.0/src/htnorm_ziggurat_constants.h
--rw-r--r--   0        0        0     1613 2021-04-04 20:43:39.802393 pyhtnorm-2.0.0/third_party_licenses/LICENSE-OPENBLAS.txt
--rw-r--r--   0        0        0    11522 2021-04-04 19:44:43.525621 pyhtnorm-2.0.0/third_party_licenses/LICENSE-PCG32.txt
--rw-r--r--   0        0        0     2910 2021-04-04 19:42:31.045616 pyhtnorm-2.0.0/third_party_licenses/LICENSE-ZIGGURAT.txt
--rw-r--r--   0        0        0     8948 2021-04-04 22:57:14.981702 pyhtnorm-2.0.0/setup.py
--rw-r--r--   0        0        0     8928 2021-04-04 22:57:14.983227 pyhtnorm-2.0.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 23:31:54.367144 pyhtnorm-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1513 2023-05-23 23:27:24.000000 pyhtnorm-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      159 2023-05-23 23:27:24.000000 pyhtnorm-2.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     9592 2023-05-23 23:31:54.367144 pyhtnorm-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     8511 2023-05-23 23:27:24.000000 pyhtnorm-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 23:31:54.363144 pyhtnorm-2.0.1/include/
+-rw-r--r--   0 runner    (1001) docker     (122)     4663 2023-05-23 23:27:24.000000 pyhtnorm-2.0.1/include/htnorm.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1815 2023-05-23 23:27:24.000000 pyhtnorm-2.0.1/include/htnorm_rng.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 23:31:54.363144 pyhtnorm-2.0.1/pyhtnorm/
+-rw-r--r--   0 runner    (1001) docker     (122)      169 2023-05-23 23:27:24.000000 pyhtnorm-2.0.1/pyhtnorm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11274 2023-05-23 23:27:24.000000 pyhtnorm-2.0.1/pyhtnorm/_htnorm.pyx
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-05-23 23:31:54.000000 pyhtnorm-2.0.1/pyhtnorm/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 23:31:54.363144 pyhtnorm-2.0.1/pyhtnorm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     9592 2023-05-23 23:31:54.000000 pyhtnorm-2.0.1/pyhtnorm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      717 2023-05-23 23:31:54.000000 pyhtnorm-2.0.1/pyhtnorm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-23 23:31:54.000000 pyhtnorm-2.0.1/pyhtnorm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       14 2023-05-23 23:31:54.000000 pyhtnorm-2.0.1/pyhtnorm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-23 23:31:54.000000 pyhtnorm-2.0.1/pyhtnorm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2746 2023-05-23 23:27:24.000000 pyhtnorm-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-23 23:31:54.367144 pyhtnorm-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1519 2023-05-23 23:27:24.000000 pyhtnorm-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 23:31:54.367144 pyhtnorm-2.0.1/src/
+-rw-r--r--   0 runner    (1001) docker     (122)    10300 2023-05-23 23:27:24.000000 pyhtnorm-2.0.1/src/htnorm.c
+-rw-r--r--   0 runner    (1001) docker     (122)      724 2023-05-23 23:27:24.000000 pyhtnorm-2.0.1/src/htnorm_always_inline.h
+-rw-r--r--   0 runner    (1001) docker     (122)     5268 2023-05-23 23:27:24.000000 pyhtnorm-2.0.1/src/htnorm_blas.h
+-rw-r--r--   0 runner    (1001) docker     (122)     4002 2023-05-23 23:27:24.000000 pyhtnorm-2.0.1/src/htnorm_distributions.c
+-rw-r--r--   0 runner    (1001) docker     (122)     3193 2023-05-23 23:27:24.000000 pyhtnorm-2.0.1/src/htnorm_distributions.h
+-rw-r--r--   0 runner    (1001) docker     (122)      857 2023-05-23 23:27:24.000000 pyhtnorm-2.0.1/src/htnorm_pcg32_minimal.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1117 2023-05-23 23:27:24.000000 pyhtnorm-2.0.1/src/htnorm_pcg64.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3104 2023-05-23 23:27:24.000000 pyhtnorm-2.0.1/src/htnorm_r_wrapper.c
+-rw-r--r--   0 runner    (1001) docker     (122)     1424 2023-05-23 23:27:24.000000 pyhtnorm-2.0.1/src/htnorm_rng.c
+-rw-r--r--   0 runner    (1001) docker     (122)      799 2023-05-23 23:27:24.000000 pyhtnorm-2.0.1/src/htnorm_splitmix64.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-05-23 23:27:24.000000 pyhtnorm-2.0.1/src/htnorm_xoroshiro128p.h
+-rw-r--r--   0 runner    (1001) docker     (122)    21851 2023-05-23 23:27:24.000000 pyhtnorm-2.0.1/src/htnorm_ziggurat_constants.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 23:31:54.367144 pyhtnorm-2.0.1/third_party_licenses/
+-rw-r--r--   0 runner    (1001) docker     (122)     1613 2023-05-23 23:27:24.000000 pyhtnorm-2.0.1/third_party_licenses/LICENSE-OPENBLAS.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    11522 2023-05-23 23:27:24.000000 pyhtnorm-2.0.1/third_party_licenses/LICENSE-PCG32.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2910 2023-05-23 23:27:24.000000 pyhtnorm-2.0.1/third_party_licenses/LICENSE-ZIGGURAT.txt
```

### Comparing `pyhtnorm-2.0.0/LICENSE` & `pyhtnorm-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhtnorm-2.0.0/README.md` & `pyhtnorm-2.0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -74,37 +74,39 @@
     return 0;
 }
 ```
 
 ## Python Interface
 [![PyPI - Wheel][10]](https://pypi.org/project/pyhtnorm/#files)
 [![PyPI][11]](https://pypi.org/project/pyhtnorm/)
+[![CI][12]](https://github.com/zoj613/htnorm/actions/workflows/build-and-test.yml)
+[![Codecov][13]](https://codecov.io/gh/zoj613/htnorm/)
+[![PyPI - License][14]](https://github.com/zoj613/htnorm/blob/main/LICENSE)
+
 
 ### Dependencies
-- NumPy >= 1.17
+- NumPy >= 1.19.0
 
-A high level python interface to the library is also provided. Linux users can 
-install it using wheels via pip (thus not needing to worry about availability of C libraries),
+A high level python interface to the library is also provided. Linux and MacOS users can 
+install it using wheels via pip (thus not needing to worry about availability of C libraries).
+Windows OS is currently not supported.
 ```bash
 pip install -U pyhtnorm
 ```
 Wheels are not provided for MacOS. To install via pip, one can run the following commands:
 ```bash
-#set the path to LAPACK shared library
-export LIBS_DIR=<some directory>
 pip install -U pyhtnorm
 ```
-Alternatively, one can install it from source. This requires an installation of [poetry][7] and the following shell commands:
+Alternatively, one can install it from source using the following shell commands:
 
 ```bash
 $ git clone https://github.com/zoj613/htnorm.git
 $ cd htnorm/
-$ poetry install
-# add htnorm to python's path
-$ export PYTHONPATH=$PWD:$PYTHONPATH
+$ export PYHT_LIBS_DIR=<some directory with blas and lapack shared library files> # this is optional
+$ pip install .
 ```
 
 Below is an example of how to use htnorm in python to sample from a multivariate
 gaussian truncated on the hyperplane ![sumzero](https://latex.codecogs.com/svg.latex?%5Cmathbf%7B1%7D%5ET%5Cmathbf%7Bx%7D%20%3D%200) (i.e. making sure the sampled values sum to zero). The python
 interface is such that the code can be easily integrated into other existing libraries.
 Since `v1.0.0`, it supports passing a `numpy.random.Generator` instance as a parameter to aid reproducibility.
 
@@ -197,7 +199,10 @@
 [5]: ./include/htnorm_rng.h
 [6]: ./LICENSE
 [7]: https://python-poetry.org/docs/pyproject/
 [8]: https://www.sciencedirect.com/science/article/abs/pii/S2211675317301574 
 [9]: ./examples/numpy_implementation.py
 [10]: https://img.shields.io/pypi/wheel/pyhtnorm?style=flat-square
 [11]: https://img.shields.io/pypi/v/pyhtnorm?style=flat-square
+[12]: https://img.shields.io/github/workflow/status/zoj613/htnorm/CI/main?style=flat-square
+[13]: https://img.shields.io/codecov/c/github/zoj613/htnorm?style=flat-square
+[14]: https://img.shields.io/pypi/l/pyhtnorm?style=flat-square
```

### Comparing `pyhtnorm-2.0.0/build.py` & `pyhtnorm-2.0.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,59 @@
-from distutils.core import Extension
+import platform
 import os
+from os.path import join
+from setuptools import Extension, setup
 
 import numpy as np
+from numpy.distutils.misc_util import get_info
 
 
 source_files = [
-    "pyhtnorm/_htnorm.c",
+    "pyhtnorm/_htnorm.pyx",
     "src/htnorm_rng.c",
     "src/htnorm_distributions.c",
     "src/htnorm.c"
 ]
 
-# get environmental variables to determine the flow of the build process
-BUILD_WHEELS = os.getenv("BUILD_WHEELS", None)
-LIBS_DIR = os.getenv("LIBS_DIR", '/usr/lib')
-
-libraries = ['m']
-
-# when building manylinux2014 wheels for pypi use different directories as
-# required by CentOS, else allow the user to specify them when building from
-# source distribution
-if BUILD_WHEELS:
-    library_dirs = ['/usr/lib64']
-    libraries.append('openblas')
+macros = [('NPY_NO_DEPRECATED_API', 0)]
+if os.getenv("BUILD_WITH_COVERAGE", None):
+    macros.append(('CYTHON_TRACE_NOGIL', 1))
+
+if platform.system() == 'Windows':
+    compile_args = ['/O2']
 else:
-    library_dirs = [LIBS_DIR]
-    libraries.extend(['blas', 'lapack'])
+    compile_args = ['-O2', '-std=c99']
+
+# https://numpy.org/devdocs/reference/random/examples/cython/setup.py.html
+include_path = np.get_include()
+lib_dirs = [
+    join(include_path, '..', '..', 'random', 'lib'), *get_info('npymath')['library_dirs'],
+]
+
+platform_lib_dirs = {
+    "Linux": ["/usr/lib"],
+    "Darwin": ["/usr/local/opt/lapack/lib", "/usr/local/opt/openblas/lib"],
+    "Windows": [],
+}
+lib_dirs.extend(platform_lib_dirs[platform.system()])
+
+if conda_prefix := os.getenv("MAMBA_ROOT_PREFIX", None):
+    lib_dirs.append(f"{conda_prefix}/envs/pyhtnorm-dev/lib")
+
+
+if user_defined_libs_dir := os.getenv("PYHT_LIBS_DIR", None):
+    lib_dirs.append(user_defined_libs_dir)
 
 
 extensions = [
     Extension(
-        "_htnorm",
-        source_files,
-        include_dirs=[np.get_include(), './include', 'src'],
-        library_dirs=library_dirs,
-        libraries=libraries,
-        define_macros=[('NPY_NO_DEPRECATED_API', 0)],
-        extra_compile_args=['-std=c99']
-    )
+        "pyhtnorm._htnorm",
+        sources=source_files,
+        include_dirs=[include_path, "./include", "./src"],
+        library_dirs=lib_dirs,
+        libraries=['npyrandom', 'npymath', 'openblas', 'lapack'],
+        define_macros=macros,
+        extra_compile_args=compile_args,
+    ),
 ]
 
-
-def build(setup_kwargs):
-    """Build extension modules."""
-    kwargs = dict(ext_modules=extensions, zip_safe=False)
-    setup_kwargs.update(kwargs)
+setup(ext_modules=extensions)
```

### Comparing `pyhtnorm-2.0.0/include/htnorm.h` & `pyhtnorm-2.0.1/include/htnorm.h`

 * *Files identical despite different names*

### Comparing `pyhtnorm-2.0.0/include/htnorm_rng.h` & `pyhtnorm-2.0.1/include/htnorm_rng.h`

 * *Files identical despite different names*

### Comparing `pyhtnorm-2.0.0/src/htnorm.c` & `pyhtnorm-2.0.1/src/htnorm.c`

 * *Files identical despite different names*

### Comparing `pyhtnorm-2.0.0/src/htnorm_always_inline.h` & `pyhtnorm-2.0.1/src/htnorm_always_inline.h`

 * *Files identical despite different names*

### Comparing `pyhtnorm-2.0.0/src/htnorm_blas.h` & `pyhtnorm-2.0.1/src/htnorm_blas.h`

 * *Files identical despite different names*

### Comparing `pyhtnorm-2.0.0/src/htnorm_distributions.c` & `pyhtnorm-2.0.1/src/htnorm_distributions.c`

 * *Files identical despite different names*

### Comparing `pyhtnorm-2.0.0/src/htnorm_distributions.h` & `pyhtnorm-2.0.1/src/htnorm_distributions.h`

 * *Files identical despite different names*

### Comparing `pyhtnorm-2.0.0/src/htnorm_pcg32_minimal.h` & `pyhtnorm-2.0.1/src/htnorm_pcg32_minimal.h`

 * *Files identical despite different names*

### Comparing `pyhtnorm-2.0.0/src/htnorm_pcg64.h` & `pyhtnorm-2.0.1/src/htnorm_pcg64.h`

 * *Files identical despite different names*

### Comparing `pyhtnorm-2.0.0/src/htnorm_r_wrapper.c` & `pyhtnorm-2.0.1/src/htnorm_r_wrapper.c`

 * *Files identical despite different names*

### Comparing `pyhtnorm-2.0.0/src/htnorm_rng.c` & `pyhtnorm-2.0.1/src/htnorm_rng.c`

 * *Files identical despite different names*

### Comparing `pyhtnorm-2.0.0/src/htnorm_splitmix64.h` & `pyhtnorm-2.0.1/src/htnorm_splitmix64.h`

 * *Files identical despite different names*

### Comparing `pyhtnorm-2.0.0/src/htnorm_xoroshiro128p.h` & `pyhtnorm-2.0.1/src/htnorm_xoroshiro128p.h`

 * *Files identical despite different names*

### Comparing `pyhtnorm-2.0.0/src/htnorm_ziggurat_constants.h` & `pyhtnorm-2.0.1/src/htnorm_ziggurat_constants.h`

 * *Files identical despite different names*

### Comparing `pyhtnorm-2.0.0/third_party_licenses/LICENSE-OPENBLAS.txt` & `pyhtnorm-2.0.1/third_party_licenses/LICENSE-OPENBLAS.txt`

 * *Files identical despite different names*

### Comparing `pyhtnorm-2.0.0/third_party_licenses/LICENSE-PCG32.txt` & `pyhtnorm-2.0.1/third_party_licenses/LICENSE-PCG32.txt`

 * *Files identical despite different names*

### Comparing `pyhtnorm-2.0.0/third_party_licenses/LICENSE-ZIGGURAT.txt` & `pyhtnorm-2.0.1/third_party_licenses/LICENSE-ZIGGURAT.txt`

 * *Files identical despite different names*

### Comparing `pyhtnorm-2.0.0/setup.py` & `pyhtnorm-2.0.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,231 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pyhtnorm
+Version: 2.0.1
+Summary: Fast Simulation of Hyperplane-Truncated Multivatiate Normal Distributions
+Author-email: Zolisa Bleki <zolisa.bleki@gmail.com>
+License: BSD 3-Clause License
+Project-URL: source, https://github.com/zoj613/htnorm
+Project-URL: tracker, https://github.com/zoj613/htnorm/issues
+Keywords: statistical sampling,multivariate gaussian distribution,hyperplane truncated multivariate normal,structured precision multivariate normal,sampling distribution,posterior sampling
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: C
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Microsoft :: Windows :: Windows 10
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Typing :: Typed
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
 
-modules = \
-['__init__']
-install_requires = \
-['numpy>=1.18.1,<2.0.0']
-
-setup_kwargs = {
-    'name': 'pyhtnorm',
-    'version': '2.0.0',
-    'description': 'Fast Simulation of Hyperplane-Truncated Multivatiate Normal Distributions',
-    'long_description': '# htnorm\n\nThis repo provides a C implementation of a fast and exact sampling algorithm for a \nmultivariate normal distribution (MVN) truncated on a hyperplane as described [here][1]\n\nThis repo implements the following from the paper:\n\n- Efficient sampling from a MVN truncated on a hyperplane: \n\n    ![hptrunc](https://latex.codecogs.com/svg.latex?%5Cmathbf%7Bx%7D%20%5Csim%20%5Cmathcal%7BN%7D_%7B%5Cmathcal%7BS%7D%7D%28%5Cmathbf%7B%5Cmu%7D%2C%20%5Cmathbf%7B%5CSigma%7D%29%3B%20%5Chspace%7B2mm%7D%20%5Cmathcal%7BS%7D%20%3D%20%5C%7B%5Cmathbf%7Bx%7D%20%3A%20%5Cmathbf%7BG%7D%5Cmathbf%7Bx%7D%20%3D%20%5Cmathbf%7Br%7D%5C%7D%2C%20%5Cmathbf%7BG%7D%20%5Cin%20%5Cmathcal%7BR%7D%5E%7Bk_2%20%5Ctimes%20k%7D%2C%20rank%28%5Cmathbf%7BG%7D%29%20%3D%20k_2%20%3C%20k)\n\n- Efficient sampling from a MVN with a stuctured precision matrix that is a sum of an invertible matrix and a low rank matrix: \n\n    ![struc](https://latex.codecogs.com/svg.latex?%5Cmathbf%7Bx%7D%20%5Csim%20%5Cmathcal%7BN%7D%5C%5B%5Cmathbf%7B%5Cmu%7D%2C%20%28%5Cmathbf%7BA%7D%20&plus;%20%5Cmathbf%7B%5CPhi%7D%5ET%5Cmathbf%7B%5COmega%7D%5Cmathbf%7B%5CPhi%7D%29%5E%7B-1%7D%5C%5D%3B%20%5Chspace%7B2mm%7D%20%5Cmathbf%7B%5CPhi%7D%20%5Cin%20%5Cmathcal%7BR%7D%5E%7Bn%20%5Ctimes%20p%7D%2C%20%5Cmathbf%7B%5COmega%7D%20%5Cin%20%5Cmathcal%7BR%7D%5E%7Bn%20%5Ctimes%20n%7D%2C%20%5Cmathbf%7BA%7D%20%5Cin%20%5Cmathcal%7BR%7D%5E%7Bp%20%5Ctimes%20p%7D)\n\n- Efficient sampling from a MVN with a structured precision and mean:\n\n    ![strucmean](https://latex.codecogs.com/svg.latex?%5Cmathbf%7Bx%7D%20%5Csim%20%5Cmathcal%7BN%7D%5CBig%5C%5B%28%5Cmathbf%7BA%7D%20&plus;%20%5Cmathbf%7B%5CPhi%7D%5ET%5Cmathbf%7B%5COmega%7D%5Cmathbf%7B%5CPhi%7D%29%5E%7B-1%7D%5Cmathbf%7B%5CPhi%7D%5ET%5Cmathbf%7B%5COmega%7D%5Cmathbf%7Bt%7D%2C%20%28%5Cmathbf%7BA%7D%20&plus;%20%5Cmathbf%7B%5CPhi%7D%5ET%5Cmathbf%7B%5COmega%7D%5Cmathbf%7B%5CPhi%7D%29%5E%7B-1%7D%5CBig%5C%5D%3B%20%5Chspace%7B2mm%7D%20%5Cmathbf%7B%5COmega%7D%20%5Cin%20%5Cmathcal%7BR%7D%5E%7Bn%20%5Ctimes%20n%7D%2C%20%5Cmathbf%7BA%7D%20%5Cin%20%5Cmathcal%7BR%7D%5E%7Bp%20%5Ctimes%20p%7D)\n\nThe algorithms implemented have the following practical applications:\n- Topic models when unknown parameters can be interpreted as fractions.\n- Admixture models\n- discrete graphical models\n- Sampling from the posterior distribution of an Intrinsic Conditional Autoregressive prior [icar][8]\n- Sampling from the posterior conditional distributions of various bayesian regression problems.\n\n\n## Dependencies\n\n- A C compiler that implements the C99 standard or later\n- An installation of `LAPACK`.\n\n## Usage\n\nBuilding a shared library of `htnorm` can be done with the following:\n```bash\n# optionally set path to LAPACK shared library\n$ export LIBS_DIR="some/path/to/lib/"\n$ make lib\n```\nAfterwards the shared library will be found in a `lib/` directory of the project root,\nand the library can be linked dynamically via `-lhtnorm`.\n\nThe puplic interface exposes the samplers through the function declarations\n```C\n int htn_hyperplane_truncated_mvn(rng_t* rng, const ht_config_t* conf, double* out);\n int htn_structured_precision_mvn(rng_t* rng, const sp_config_t* conf, double* out);\n```\n\nThe details of the parameters are documented in ther header files ["htnorm.h"][4].\n\nRandom number generation is done using [PCG64][2] or [Xoroshiro128plus][3] bitgenerators. \nThe interface allows using a custom bitgenerator, and the details are documented in the header file \n["rng.h"][5].\n\n## Example\n```C\n#include "htnorm.h"\n\nint main (void)\n{\n    ...\n    // instantiate a random number generator\n    rng_t* rng = rng_new_pcg64_seeded(12345);\n    ht_config_t config;\n    init_ht_config(&config, ...);\n    double* out = ...; // array to store the samples\n    int res = htn_hyperplane_truncated_mvn(rng, &config, out);\n    // res contains a number that indicates whether sampling failed or not.\n    ...\n    // finally free the RNG pointer at some point\n    rng_free(rng);\n    ...\n    return 0;\n}\n```\n\n## Python Interface\n[![PyPI - Wheel][10]](https://pypi.org/project/pyhtnorm/#files)\n[![PyPI][11]](https://pypi.org/project/pyhtnorm/)\n\n### Dependencies\n- NumPy >= 1.17\n\nA high level python interface to the library is also provided. Linux users can \ninstall it using wheels via pip (thus not needing to worry about availability of C libraries),\n```bash\npip install -U pyhtnorm\n```\nWheels are not provided for MacOS. To install via pip, one can run the following commands:\n```bash\n#set the path to LAPACK shared library\nexport LIBS_DIR=<some directory>\npip install -U pyhtnorm\n```\nAlternatively, one can install it from source. This requires an installation of [poetry][7] and the following shell commands:\n\n```bash\n$ git clone https://github.com/zoj613/htnorm.git\n$ cd htnorm/\n$ poetry install\n# add htnorm to python\'s path\n$ export PYTHONPATH=$PWD:$PYTHONPATH\n```\n\nBelow is an example of how to use htnorm in python to sample from a multivariate\ngaussian truncated on the hyperplane ![sumzero](https://latex.codecogs.com/svg.latex?%5Cmathbf%7B1%7D%5ET%5Cmathbf%7Bx%7D%20%3D%200) (i.e. making sure the sampled values sum to zero). The python\ninterface is such that the code can be easily integrated into other existing libraries.\nSince `v1.0.0`, it supports passing a `numpy.random.Generator` instance as a parameter to aid reproducibility.\n\n```python\nfrom pyhtnorm import hyperplane_truncated_mvnorm, structured_precision_mvnorm\nimport numpy as np\n\nrng = np.random.default_rng()\n\n# generate example input\nk1, k2 = 1000, 1\ntemp = rng.random((k1, k1))\ncov = temp @ temp.T\nG = np.ones((k2, k1))\nr = np.zeros(k2)\nmean = rng.random(k1)\n\n# passing `random_state` is optional. If the argument is not used, a fresh\n# random generator state is instantiated internally using system entropy.\no = hyperplane_truncated_mvnorm(mean, cov, G, r, random_state=rng)\nprint(o.sum())  # verify if sampled values sum to zero\n# alternatively one can pass an array to store the results in\nhyperplane_truncated_mvnorm(mean, cov, G, r, out=o)\n```\n\nFor more information about the function\'s arguments, refer to its docstring.\n\nA pure numpy implementation is demonstrated in this [example script][9].\n\n\n## R Interface\n\nOne can also use the package in R. To install, use one the following commands:\n```R\ndevtools::install_github("zoj613/htnorm")\npak::pkg_install("zoj613/htnorm")\n```\n\nBelow is an R translation of the above python example:\n\n```R\nlibrary(htnorm)\n\n# make dummy data\nmean <- rnorm(1000)\ncov <- matrix(rnorm(1000 * 1000), ncol=1000)\ncov <- cov %*% t(cov)\nG <- matrix(rep(1, 1000), ncol=1000)\nr <- c(0)\n\n# initialize the Generator instance\nrng <- HTNGenerator(seed=12345, gen="pcg64")\n\nsamples <- rng$hyperplane_truncated_mvnorm(mean, cov, G, r)\n#verify if sampled values sum to zero\nsum(samples)\n\n# optionally pass a vector to store the results in\nout <- rep(0, 1000)\nrng$hyperplane_truncated_mvnorm(mean, cov, G, r, out = out)\nsum(out)  #verify\n\nout <- rep(0, 1000)\neig <- eigen(cov)\nphi <- eig$vectors\nomega <- diag(eig$values)\na <- diag(runif(length(mean)))\nrng$structured_precision_mvnorm(mean, a, phi, omega, a_type = "diagonal", out = out)\n```\n\n## Licensing\n\n`htnorm` is free software made available under the BSD-3 License. For details\nsee the [LICENSE][6] file.\n\n\n## References\n- Cong, Yulai; Chen, Bo; Zhou, Mingyuan. Fast Simulation of Hyperplane-Truncated \n   Multivariate Normal Distributions. Bayesian Anal. 12 (2017), no. 4, 1017--1037. \n   doi:10.1214/17-BA1052.\n- Bhattacharya, A., Chakraborty, A., and Mallick, B. K. (2016). \n  “Fast sampling with Gaussian scale mixture priors in high-dimensional regression.” \n  Biometrika, 103(4):985. \n\n\n[1]: https://projecteuclid.org/euclid.ba/1488337478\n[2]: https://www.pcg-random.org/\n[3]: https://en.wikipedia.org/wiki/Xoroshiro128%2B\n[4]: ./include/htnorm.h \n[5]: ./include/htnorm_rng.h\n[6]: ./LICENSE\n[7]: https://python-poetry.org/docs/pyproject/\n[8]: https://www.sciencedirect.com/science/article/abs/pii/S2211675317301574 \n[9]: ./examples/numpy_implementation.py\n[10]: https://img.shields.io/pypi/wheel/pyhtnorm?style=flat-square\n[11]: https://img.shields.io/pypi/v/pyhtnorm?style=flat-square\n',
-    'author': 'Zolisa Bleki',
-    'author_email': None,
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/zoj613/htnorm/',
-    'py_modules': modules,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7.0,<4.0.0',
+# htnorm
+
+This repo provides a C implementation of a fast and exact sampling algorithm for a 
+multivariate normal distribution (MVN) truncated on a hyperplane as described [here][1]
+
+This repo implements the following from the paper:
+
+- Efficient sampling from a MVN truncated on a hyperplane: 
+
+    ![hptrunc](https://latex.codecogs.com/svg.latex?%5Cmathbf%7Bx%7D%20%5Csim%20%5Cmathcal%7BN%7D_%7B%5Cmathcal%7BS%7D%7D%28%5Cmathbf%7B%5Cmu%7D%2C%20%5Cmathbf%7B%5CSigma%7D%29%3B%20%5Chspace%7B2mm%7D%20%5Cmathcal%7BS%7D%20%3D%20%5C%7B%5Cmathbf%7Bx%7D%20%3A%20%5Cmathbf%7BG%7D%5Cmathbf%7Bx%7D%20%3D%20%5Cmathbf%7Br%7D%5C%7D%2C%20%5Cmathbf%7BG%7D%20%5Cin%20%5Cmathcal%7BR%7D%5E%7Bk_2%20%5Ctimes%20k%7D%2C%20rank%28%5Cmathbf%7BG%7D%29%20%3D%20k_2%20%3C%20k)
+
+- Efficient sampling from a MVN with a stuctured precision matrix that is a sum of an invertible matrix and a low rank matrix: 
+
+    ![struc](https://latex.codecogs.com/svg.latex?%5Cmathbf%7Bx%7D%20%5Csim%20%5Cmathcal%7BN%7D%5C%5B%5Cmathbf%7B%5Cmu%7D%2C%20%28%5Cmathbf%7BA%7D%20&plus;%20%5Cmathbf%7B%5CPhi%7D%5ET%5Cmathbf%7B%5COmega%7D%5Cmathbf%7B%5CPhi%7D%29%5E%7B-1%7D%5C%5D%3B%20%5Chspace%7B2mm%7D%20%5Cmathbf%7B%5CPhi%7D%20%5Cin%20%5Cmathcal%7BR%7D%5E%7Bn%20%5Ctimes%20p%7D%2C%20%5Cmathbf%7B%5COmega%7D%20%5Cin%20%5Cmathcal%7BR%7D%5E%7Bn%20%5Ctimes%20n%7D%2C%20%5Cmathbf%7BA%7D%20%5Cin%20%5Cmathcal%7BR%7D%5E%7Bp%20%5Ctimes%20p%7D)
+
+- Efficient sampling from a MVN with a structured precision and mean:
+
+    ![strucmean](https://latex.codecogs.com/svg.latex?%5Cmathbf%7Bx%7D%20%5Csim%20%5Cmathcal%7BN%7D%5CBig%5C%5B%28%5Cmathbf%7BA%7D%20&plus;%20%5Cmathbf%7B%5CPhi%7D%5ET%5Cmathbf%7B%5COmega%7D%5Cmathbf%7B%5CPhi%7D%29%5E%7B-1%7D%5Cmathbf%7B%5CPhi%7D%5ET%5Cmathbf%7B%5COmega%7D%5Cmathbf%7Bt%7D%2C%20%28%5Cmathbf%7BA%7D%20&plus;%20%5Cmathbf%7B%5CPhi%7D%5ET%5Cmathbf%7B%5COmega%7D%5Cmathbf%7B%5CPhi%7D%29%5E%7B-1%7D%5CBig%5C%5D%3B%20%5Chspace%7B2mm%7D%20%5Cmathbf%7B%5COmega%7D%20%5Cin%20%5Cmathcal%7BR%7D%5E%7Bn%20%5Ctimes%20n%7D%2C%20%5Cmathbf%7BA%7D%20%5Cin%20%5Cmathcal%7BR%7D%5E%7Bp%20%5Ctimes%20p%7D)
+
+The algorithms implemented have the following practical applications:
+- Topic models when unknown parameters can be interpreted as fractions.
+- Admixture models
+- discrete graphical models
+- Sampling from the posterior distribution of an Intrinsic Conditional Autoregressive prior [icar][8]
+- Sampling from the posterior conditional distributions of various bayesian regression problems.
+
+
+## Dependencies
+
+- A C compiler that implements the C99 standard or later
+- An installation of `LAPACK`.
+
+## Usage
+
+Building a shared library of `htnorm` can be done with the following:
+```bash
+# optionally set path to LAPACK shared library
+$ export LIBS_DIR="some/path/to/lib/"
+$ make lib
+```
+Afterwards the shared library will be found in a `lib/` directory of the project root,
+and the library can be linked dynamically via `-lhtnorm`.
+
+The puplic interface exposes the samplers through the function declarations
+```C
+ int htn_hyperplane_truncated_mvn(rng_t* rng, const ht_config_t* conf, double* out);
+ int htn_structured_precision_mvn(rng_t* rng, const sp_config_t* conf, double* out);
+```
+
+The details of the parameters are documented in ther header files ["htnorm.h"][4].
+
+Random number generation is done using [PCG64][2] or [Xoroshiro128plus][3] bitgenerators. 
+The interface allows using a custom bitgenerator, and the details are documented in the header file 
+["rng.h"][5].
+
+## Example
+```C
+#include "htnorm.h"
+
+int main (void)
+{
+    ...
+    // instantiate a random number generator
+    rng_t* rng = rng_new_pcg64_seeded(12345);
+    ht_config_t config;
+    init_ht_config(&config, ...);
+    double* out = ...; // array to store the samples
+    int res = htn_hyperplane_truncated_mvn(rng, &config, out);
+    // res contains a number that indicates whether sampling failed or not.
+    ...
+    // finally free the RNG pointer at some point
+    rng_free(rng);
+    ...
+    return 0;
 }
-from build import *
-build(setup_kwargs)
+```
+
+## Python Interface
+[![PyPI - Wheel][10]](https://pypi.org/project/pyhtnorm/#files)
+[![PyPI][11]](https://pypi.org/project/pyhtnorm/)
+[![CI][12]](https://github.com/zoj613/htnorm/actions/workflows/build-and-test.yml)
+[![Codecov][13]](https://codecov.io/gh/zoj613/htnorm/)
+[![PyPI - License][14]](https://github.com/zoj613/htnorm/blob/main/LICENSE)
+
+
+### Dependencies
+- NumPy >= 1.19.0
+
+A high level python interface to the library is also provided. Linux and MacOS users can 
+install it using wheels via pip (thus not needing to worry about availability of C libraries).
+Windows OS is currently not supported.
+```bash
+pip install -U pyhtnorm
+```
+Wheels are not provided for MacOS. To install via pip, one can run the following commands:
+```bash
+pip install -U pyhtnorm
+```
+Alternatively, one can install it from source using the following shell commands:
+
+```bash
+$ git clone https://github.com/zoj613/htnorm.git
+$ cd htnorm/
+$ export PYHT_LIBS_DIR=<some directory with blas and lapack shared library files> # this is optional
+$ pip install .
+```
+
+Below is an example of how to use htnorm in python to sample from a multivariate
+gaussian truncated on the hyperplane ![sumzero](https://latex.codecogs.com/svg.latex?%5Cmathbf%7B1%7D%5ET%5Cmathbf%7Bx%7D%20%3D%200) (i.e. making sure the sampled values sum to zero). The python
+interface is such that the code can be easily integrated into other existing libraries.
+Since `v1.0.0`, it supports passing a `numpy.random.Generator` instance as a parameter to aid reproducibility.
+
+```python
+from pyhtnorm import hyperplane_truncated_mvnorm, structured_precision_mvnorm
+import numpy as np
+
+rng = np.random.default_rng()
+
+# generate example input
+k1, k2 = 1000, 1
+temp = rng.random((k1, k1))
+cov = temp @ temp.T
+G = np.ones((k2, k1))
+r = np.zeros(k2)
+mean = rng.random(k1)
+
+# passing `random_state` is optional. If the argument is not used, a fresh
+# random generator state is instantiated internally using system entropy.
+o = hyperplane_truncated_mvnorm(mean, cov, G, r, random_state=rng)
+print(o.sum())  # verify if sampled values sum to zero
+# alternatively one can pass an array to store the results in
+hyperplane_truncated_mvnorm(mean, cov, G, r, out=o)
+```
+
+For more information about the function's arguments, refer to its docstring.
+
+A pure numpy implementation is demonstrated in this [example script][9].
+
+
+## R Interface
+
+One can also use the package in R. To install, use one the following commands:
+```R
+devtools::install_github("zoj613/htnorm")
+pak::pkg_install("zoj613/htnorm")
+```
+
+Below is an R translation of the above python example:
+
+```R
+library(htnorm)
+
+# make dummy data
+mean <- rnorm(1000)
+cov <- matrix(rnorm(1000 * 1000), ncol=1000)
+cov <- cov %*% t(cov)
+G <- matrix(rep(1, 1000), ncol=1000)
+r <- c(0)
+
+# initialize the Generator instance
+rng <- HTNGenerator(seed=12345, gen="pcg64")
+
+samples <- rng$hyperplane_truncated_mvnorm(mean, cov, G, r)
+#verify if sampled values sum to zero
+sum(samples)
+
+# optionally pass a vector to store the results in
+out <- rep(0, 1000)
+rng$hyperplane_truncated_mvnorm(mean, cov, G, r, out = out)
+sum(out)  #verify
+
+out <- rep(0, 1000)
+eig <- eigen(cov)
+phi <- eig$vectors
+omega <- diag(eig$values)
+a <- diag(runif(length(mean)))
+rng$structured_precision_mvnorm(mean, a, phi, omega, a_type = "diagonal", out = out)
+```
+
+## Licensing
+
+`htnorm` is free software made available under the BSD-3 License. For details
+see the [LICENSE][6] file.
+
+
+## References
+- Cong, Yulai; Chen, Bo; Zhou, Mingyuan. Fast Simulation of Hyperplane-Truncated 
+   Multivariate Normal Distributions. Bayesian Anal. 12 (2017), no. 4, 1017--1037. 
+   doi:10.1214/17-BA1052.
+- Bhattacharya, A., Chakraborty, A., and Mallick, B. K. (2016). 
+  “Fast sampling with Gaussian scale mixture priors in high-dimensional regression.” 
+  Biometrika, 103(4):985. 
+
 
-setup(**setup_kwargs)
+[1]: https://projecteuclid.org/euclid.ba/1488337478
+[2]: https://www.pcg-random.org/
+[3]: https://en.wikipedia.org/wiki/Xoroshiro128%2B
+[4]: ./include/htnorm.h 
+[5]: ./include/htnorm_rng.h
+[6]: ./LICENSE
+[7]: https://python-poetry.org/docs/pyproject/
+[8]: https://www.sciencedirect.com/science/article/abs/pii/S2211675317301574 
+[9]: ./examples/numpy_implementation.py
+[10]: https://img.shields.io/pypi/wheel/pyhtnorm?style=flat-square
+[11]: https://img.shields.io/pypi/v/pyhtnorm?style=flat-square
+[12]: https://img.shields.io/github/workflow/status/zoj613/htnorm/CI/main?style=flat-square
+[13]: https://img.shields.io/codecov/c/github/zoj613/htnorm?style=flat-square
+[14]: https://img.shields.io/pypi/l/pyhtnorm?style=flat-square
```

### Comparing `pyhtnorm-2.0.0/PKG-INFO` & `pyhtnorm-2.0.1/pyhtnorm.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 Metadata-Version: 2.1
 Name: pyhtnorm
-Version: 2.0.0
+Version: 2.0.1
 Summary: Fast Simulation of Hyperplane-Truncated Multivatiate Normal Distributions
-Home-page: https://github.com/zoj613/htnorm/
-License: BSD-3-Clause
+Author-email: Zolisa Bleki <zolisa.bleki@gmail.com>
+License: BSD 3-Clause License
+Project-URL: source, https://github.com/zoj613/htnorm
+Project-URL: tracker, https://github.com/zoj613/htnorm/issues
 Keywords: statistical sampling,multivariate gaussian distribution,hyperplane truncated multivariate normal,structured precision multivariate normal,sampling distribution,posterior sampling
-Author: Zolisa Bleki
-Requires-Python: >=3.7.0,<4.0.0
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: numpy (>=1.18.1,<2.0.0)
-Project-URL: Repository, https://github.com/zoj613/htnorm/
+Classifier: Programming Language :: C
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Microsoft :: Windows :: Windows 10
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Typing :: Typed
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # htnorm
 
 This repo provides a C implementation of a fast and exact sampling algorithm for a 
 multivariate normal distribution (MVN) truncated on a hyperplane as described [here][1]
 
 This repo implements the following from the paper:
@@ -92,37 +97,39 @@
     return 0;
 }
 ```
 
 ## Python Interface
 [![PyPI - Wheel][10]](https://pypi.org/project/pyhtnorm/#files)
 [![PyPI][11]](https://pypi.org/project/pyhtnorm/)
+[![CI][12]](https://github.com/zoj613/htnorm/actions/workflows/build-and-test.yml)
+[![Codecov][13]](https://codecov.io/gh/zoj613/htnorm/)
+[![PyPI - License][14]](https://github.com/zoj613/htnorm/blob/main/LICENSE)
+
 
 ### Dependencies
-- NumPy >= 1.17
+- NumPy >= 1.19.0
 
-A high level python interface to the library is also provided. Linux users can 
-install it using wheels via pip (thus not needing to worry about availability of C libraries),
+A high level python interface to the library is also provided. Linux and MacOS users can 
+install it using wheels via pip (thus not needing to worry about availability of C libraries).
+Windows OS is currently not supported.
 ```bash
 pip install -U pyhtnorm
 ```
 Wheels are not provided for MacOS. To install via pip, one can run the following commands:
 ```bash
-#set the path to LAPACK shared library
-export LIBS_DIR=<some directory>
 pip install -U pyhtnorm
 ```
-Alternatively, one can install it from source. This requires an installation of [poetry][7] and the following shell commands:
+Alternatively, one can install it from source using the following shell commands:
 
 ```bash
 $ git clone https://github.com/zoj613/htnorm.git
 $ cd htnorm/
-$ poetry install
-# add htnorm to python's path
-$ export PYTHONPATH=$PWD:$PYTHONPATH
+$ export PYHT_LIBS_DIR=<some directory with blas and lapack shared library files> # this is optional
+$ pip install .
 ```
 
 Below is an example of how to use htnorm in python to sample from a multivariate
 gaussian truncated on the hyperplane ![sumzero](https://latex.codecogs.com/svg.latex?%5Cmathbf%7B1%7D%5ET%5Cmathbf%7Bx%7D%20%3D%200) (i.e. making sure the sampled values sum to zero). The python
 interface is such that the code can be easily integrated into other existing libraries.
 Since `v1.0.0`, it supports passing a `numpy.random.Generator` instance as a parameter to aid reproducibility.
 
@@ -215,8 +222,10 @@
 [5]: ./include/htnorm_rng.h
 [6]: ./LICENSE
 [7]: https://python-poetry.org/docs/pyproject/
 [8]: https://www.sciencedirect.com/science/article/abs/pii/S2211675317301574 
 [9]: ./examples/numpy_implementation.py
 [10]: https://img.shields.io/pypi/wheel/pyhtnorm?style=flat-square
 [11]: https://img.shields.io/pypi/v/pyhtnorm?style=flat-square
-
+[12]: https://img.shields.io/github/workflow/status/zoj613/htnorm/CI/main?style=flat-square
+[13]: https://img.shields.io/codecov/c/github/zoj613/htnorm?style=flat-square
+[14]: https://img.shields.io/pypi/l/pyhtnorm?style=flat-square
```

