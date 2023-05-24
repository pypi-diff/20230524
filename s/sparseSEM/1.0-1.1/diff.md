# Comparing `tmp/sparseSEM-1.0.tar.gz` & `tmp/sparseSEM-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparseSEM-1.0.tar", last modified: Fri May 12 02:24:06 2023, max compression
+gzip compressed data, was "sparseSEM-1.1.tar", last modified: Wed May 24 20:33:07 2023, max compression
```

## Comparing `sparseSEM-1.0.tar` & `sparseSEM-1.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 anhui      (501) staff       (20)        0 2023-05-12 02:24:06.785153 sparseSEM-1.0/
--rw-r--r--   0 anhui      (501) staff       (20)       52 2023-05-11 03:19:57.000000 sparseSEM-1.0/MANIFEST.in
--rw-r--r--   0 anhui      (501) staff       (20)     2609 2023-05-12 02:24:06.784588 sparseSEM-1.0/PKG-INFO
--rw-r--r--   0 anhui      (501) staff       (20)     1577 2023-04-23 23:00:54.000000 sparseSEM-1.0/README.md
-drwxr-xr-x   0 anhui      (501) staff       (20)        0 2023-05-12 02:24:06.723685 sparseSEM-1.0/data/
--rw-r--r--   0 anhui      (501) staff       (20)     2393 2023-04-25 02:30:52.000000 sparseSEM-1.0/data/B.csv
--rw-r--r--   0 anhui      (501) staff       (20)    13436 2023-04-19 01:21:12.000000 sparseSEM-1.0/data/Missing.csv
--rw-r--r--   0 anhui      (501) staff       (20)    13436 2023-04-19 01:21:08.000000 sparseSEM-1.0/data/X.csv
--rw-r--r--   0 anhui      (501) staff       (20)    62636 2023-04-19 01:21:05.000000 sparseSEM-1.0/data/Y.csv
-drwxr-xr-x   0 anhui      (501) staff       (20)        0 2023-05-12 02:24:06.764012 sparseSEM-1.0/doc/
--rw-r--r--   0 anhui      (501) staff       (20)     6148 2023-04-27 02:57:56.000000 sparseSEM-1.0/doc/.DS_Store
--rw-r--r--   0 anhui      (501) staff       (20)   173524 2023-04-17 18:15:54.000000 sparseSEM-1.0/doc/Fig1_nCPU.png
--rw-r--r--   0 anhui      (501) staff       (20)   369870 2023-04-17 18:15:54.000000 sparseSEM-1.0/doc/Fig2_sigma01.png
--rw-r--r--   0 anhui      (501) staff       (20)   380492 2023-04-17 18:15:54.000000 sparseSEM-1.0/doc/Fig3_sigma05.png
--rwxr-xr-x   0 anhui      (501) staff       (20)  1989713 2023-04-17 18:15:54.000000 sparseSEM-1.0/doc/Fig4_cisTransNetworkYeast_clusters_manualAdjusted_GOterm.jpg
--rwxr-xr-x   0 anhui      (501) staff       (20)   928929 2023-04-17 18:15:54.000000 sparseSEM-1.0/doc/Fig5_yeast_grn_genome_biology.png
--rw-r--r--   0 anhui      (501) staff       (20)    37882 2023-04-18 23:35:33.000000 sparseSEM-1.0/doc/sparseSEM.md
--rw-r--r--   0 anhui      (501) staff       (20)   909391 2023-05-05 02:24:33.000000 sparseSEM-1.0/doc/sparseSEM.pdf
--rw-r--r--   0 anhui      (501) staff       (20)   166880 2023-04-17 19:32:38.000000 sparseSEM-1.0/doc/table1_data.png
--rw-r--r--   0 anhui      (501) staff       (20)   281918 2023-04-17 19:56:05.000000 sparseSEM-1.0/doc/table2_data.png
--rw-r--r--   0 anhui      (501) staff       (20)   144048 2023-04-17 19:57:17.000000 sparseSEM-1.0/doc/table3_data.png
--rw-r--r--   0 anhui      (501) staff       (20)       38 2023-05-12 02:24:06.785349 sparseSEM-1.0/setup.cfg
--rw-r--r--   0 anhui      (501) staff       (20)     2146 2023-05-12 02:24:00.000000 sparseSEM-1.0/setup.py
-drwxr-xr-x   0 anhui      (501) staff       (20)        0 2023-05-12 02:24:06.772742 sparseSEM-1.0/sparseSEM/
--rw-r--r--   0 anhui      (501) staff       (20)      479 2023-05-02 18:28:38.000000 sparseSEM-1.0/sparseSEM/__init__.py
--rw-r--r--   0 anhui      (501) staff       (20)     8065 2023-05-05 02:30:30.000000 sparseSEM-1.0/sparseSEM/elasticNetSML.py
--rw-r--r--   0 anhui      (501) staff       (20)     8684 2023-05-05 02:30:30.000000 sparseSEM-1.0/sparseSEM/elasticNetSMLcv.py
--rw-r--r--   0 anhui      (501) staff       (20)     7919 2023-05-05 02:30:30.000000 sparseSEM-1.0/sparseSEM/elasticNetSMLpoint.py
--rw-r--r--   0 anhui      (501) staff       (20)      911 2023-04-25 02:24:54.000000 sparseSEM-1.0/sparseSEM/loadSEMlib.py
--rwxr-xr-x   0 anhui      (501) staff       (20)   100424 2023-05-03 02:42:08.000000 sparseSEM-1.0/sparseSEM/sparseSEM.cpython-310-darwin.so
-drwxr-xr-x   0 anhui      (501) staff       (20)        0 2023-05-12 02:24:06.782070 sparseSEM-1.0/sparseSEM/src/
--rw-r--r--   0 anhui      (501) staff       (20)    41900 2023-04-23 02:55:12.000000 sparseSEM-1.0/sparseSEM/src/lassoSEM.c
--rw-r--r--   0 anhui      (501) staff       (20)     1550 2023-04-17 14:36:00.000000 sparseSEM-1.0/sparseSEM/src/lassoSEM.h
--rw-r--r--   0 anhui      (501) staff       (20)    90448 2023-05-03 02:40:40.000000 sparseSEM-1.0/sparseSEM/src/lassoSMLv11beta.c
-drwxr-xr-x   0 anhui      (501) staff       (20)        0 2023-05-12 02:24:06.778208 sparseSEM-1.0/sparseSEM.egg-info/
--rw-r--r--   0 anhui      (501) staff       (20)     2609 2023-05-12 02:24:06.000000 sparseSEM-1.0/sparseSEM.egg-info/PKG-INFO
--rw-r--r--   0 anhui      (501) staff       (20)      774 2023-05-12 02:24:06.000000 sparseSEM-1.0/sparseSEM.egg-info/SOURCES.txt
--rw-r--r--   0 anhui      (501) staff       (20)        1 2023-05-12 02:24:06.000000 sparseSEM-1.0/sparseSEM.egg-info/dependency_links.txt
--rw-r--r--   0 anhui      (501) staff       (20)       33 2023-05-12 02:24:06.000000 sparseSEM-1.0/sparseSEM.egg-info/requires.txt
--rw-r--r--   0 anhui      (501) staff       (20)       10 2023-05-12 02:24:06.000000 sparseSEM-1.0/sparseSEM.egg-info/top_level.txt
+drwxr-xr-x   0 anhui      (501) staff       (20)        0 2023-05-24 20:33:07.020300 sparseSEM-1.1/
+-rw-r--r--   0 anhui      (501) staff       (20)       52 2023-05-11 03:19:57.000000 sparseSEM-1.1/MANIFEST.in
+-rw-r--r--   0 anhui      (501) staff       (20)     3243 2023-05-24 20:33:07.019832 sparseSEM-1.1/PKG-INFO
+-rw-r--r--   0 anhui      (501) staff       (20)     2211 2023-05-12 03:20:51.000000 sparseSEM-1.1/README.md
+drwxr-xr-x   0 anhui      (501) staff       (20)        0 2023-05-24 20:33:06.995738 sparseSEM-1.1/data/
+-rw-r--r--   0 anhui      (501) staff       (20)     2393 2023-04-25 02:30:52.000000 sparseSEM-1.1/data/B.csv
+-rw-r--r--   0 anhui      (501) staff       (20)    13436 2023-04-19 01:21:12.000000 sparseSEM-1.1/data/Missing.csv
+-rw-r--r--   0 anhui      (501) staff       (20)    13436 2023-04-19 01:21:08.000000 sparseSEM-1.1/data/X.csv
+-rw-r--r--   0 anhui      (501) staff       (20)    62636 2023-04-19 01:21:05.000000 sparseSEM-1.1/data/Y.csv
+drwxr-xr-x   0 anhui      (501) staff       (20)        0 2023-05-24 20:33:07.009626 sparseSEM-1.1/doc/
+-rw-r--r--   0 anhui      (501) staff       (20)     6148 2023-04-27 02:57:56.000000 sparseSEM-1.1/doc/.DS_Store
+-rw-r--r--   0 anhui      (501) staff       (20)   173524 2023-04-17 18:15:54.000000 sparseSEM-1.1/doc/Fig1_nCPU.png
+-rw-r--r--   0 anhui      (501) staff       (20)   369870 2023-04-17 18:15:54.000000 sparseSEM-1.1/doc/Fig2_sigma01.png
+-rw-r--r--   0 anhui      (501) staff       (20)   380492 2023-04-17 18:15:54.000000 sparseSEM-1.1/doc/Fig3_sigma05.png
+-rwxr-xr-x   0 anhui      (501) staff       (20)  1989713 2023-04-17 18:15:54.000000 sparseSEM-1.1/doc/Fig4_cisTransNetworkYeast_clusters_manualAdjusted_GOterm.jpg
+-rwxr-xr-x   0 anhui      (501) staff       (20)   928929 2023-04-17 18:15:54.000000 sparseSEM-1.1/doc/Fig5_yeast_grn_genome_biology.png
+-rw-r--r--   0 anhui      (501) staff       (20)    37882 2023-04-18 23:35:33.000000 sparseSEM-1.1/doc/sparseSEM.md
+-rw-r--r--   0 anhui      (501) staff       (20)   909391 2023-05-05 02:24:33.000000 sparseSEM-1.1/doc/sparseSEM.pdf
+-rw-r--r--   0 anhui      (501) staff       (20)   166880 2023-04-17 19:32:38.000000 sparseSEM-1.1/doc/table1_data.png
+-rw-r--r--   0 anhui      (501) staff       (20)   281918 2023-04-17 19:56:05.000000 sparseSEM-1.1/doc/table2_data.png
+-rw-r--r--   0 anhui      (501) staff       (20)   144048 2023-04-17 19:57:17.000000 sparseSEM-1.1/doc/table3_data.png
+-rw-r--r--   0 anhui      (501) staff       (20)       38 2023-05-24 20:33:07.020508 sparseSEM-1.1/setup.cfg
+-rw-r--r--   0 anhui      (501) staff       (20)     2279 2023-05-24 20:33:04.000000 sparseSEM-1.1/setup.py
+drwxr-xr-x   0 anhui      (501) staff       (20)        0 2023-05-24 20:33:07.013117 sparseSEM-1.1/sparseSEM/
+-rw-r--r--   0 anhui      (501) staff       (20)      479 2023-05-02 18:28:38.000000 sparseSEM-1.1/sparseSEM/__init__.py
+-rw-r--r--   0 anhui      (501) staff       (20)     8064 2023-05-16 02:29:32.000000 sparseSEM-1.1/sparseSEM/elasticNetSML.py
+-rw-r--r--   0 anhui      (501) staff       (20)     8684 2023-05-05 02:30:30.000000 sparseSEM-1.1/sparseSEM/elasticNetSMLcv.py
+-rw-r--r--   0 anhui      (501) staff       (20)     7919 2023-05-05 02:30:30.000000 sparseSEM-1.1/sparseSEM/elasticNetSMLpoint.py
+-rw-r--r--   0 anhui      (501) staff       (20)      911 2023-04-25 02:24:54.000000 sparseSEM-1.1/sparseSEM/loadSEMlib.py
+-rwxr-xr-x   0 anhui      (501) staff       (20)   100424 2023-05-03 02:42:08.000000 sparseSEM-1.1/sparseSEM/sparseSEM.cpython-310-darwin.so
+drwxr-xr-x   0 anhui      (501) staff       (20)        0 2023-05-24 20:33:07.018810 sparseSEM-1.1/sparseSEM/src/
+-rw-r--r--   0 anhui      (501) staff       (20)    41900 2023-04-23 02:55:12.000000 sparseSEM-1.1/sparseSEM/src/lassoSEM.c
+-rw-r--r--   0 anhui      (501) staff       (20)     1550 2023-04-17 14:36:00.000000 sparseSEM-1.1/sparseSEM/src/lassoSEM.h
+-rw-r--r--   0 anhui      (501) staff       (20)    90448 2023-05-03 02:40:40.000000 sparseSEM-1.1/sparseSEM/src/lassoSMLv11beta.c
+drwxr-xr-x   0 anhui      (501) staff       (20)        0 2023-05-24 20:33:07.016772 sparseSEM-1.1/sparseSEM.egg-info/
+-rw-r--r--   0 anhui      (501) staff       (20)     3243 2023-05-24 20:33:06.000000 sparseSEM-1.1/sparseSEM.egg-info/PKG-INFO
+-rw-r--r--   0 anhui      (501) staff       (20)      774 2023-05-24 20:33:06.000000 sparseSEM-1.1/sparseSEM.egg-info/SOURCES.txt
+-rw-r--r--   0 anhui      (501) staff       (20)        1 2023-05-24 20:33:06.000000 sparseSEM-1.1/sparseSEM.egg-info/dependency_links.txt
+-rw-r--r--   0 anhui      (501) staff       (20)       33 2023-05-24 20:33:06.000000 sparseSEM-1.1/sparseSEM.egg-info/requires.txt
+-rw-r--r--   0 anhui      (501) staff       (20)       10 2023-05-24 20:33:06.000000 sparseSEM-1.1/sparseSEM.egg-info/top_level.txt
```

### Comparing `sparseSEM-1.0/PKG-INFO` & `sparseSEM-1.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparseSEM
-Version: 1.0
+Version: 1.1
 Summary: Python wrapper for sparseSEM
 Home-page: https://scholar.google.com/citations?user=WhDMZEIAAAAJ&hl=en
 Author: Anhui Huang
 Author-email: anhuihuang@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python
@@ -26,32 +26,44 @@
 # Elastic Net for Structural Equation Models (SEM)
 
 Anhui Huang | Ph.D. Electrical and Computer Engineering 
 
 <https://scholar.google.com/citations?user=WhDMZEIAAAAJ&hl=en>
 
 
+## PyPI installation 
+`sparseSEM` is available on PyPI:  https://pypi.org/project/sparseSEM/1.0/. Run command `pip install sparseSEM` to install 
+from PyPI.
 
-## Online Documentation
+`test/` folder contains examples using data packed along with this package in `data/` folder. 
+To run `test/` examples, clone this repo, and run from `test/` directory. 
+
+
+## Documentation
 The theory and background for network topology inference using sparse Structural Equation Models (SEM) can be found 
-in my Ph.D dissertation (Huang A. 2014). The experimental study are also available in the documentation in the package.  
+in my Ph.D dissertation (Huang A. 2014). The experimental study are also available in the `doc/` folder in the package.  
 
 
 ## Configuration
 This package was originally developed to leverage high performance computer clusters to enable parallel computation 
 through openMPI.  Users who have access to large scale computational resources can explore the functionality and 
 checkout the openMPI module in this package.
 
 Current package utilizes blas/lapack for high speed computation. To build the C/C++ code, the intel OneMKL library is 
 specified in the package setup. 
 - Install the free OneMKL package (https://www.intel.com/content/www/us/en/docs/oneapi/programming-guide/2023-0/intel-oneapi-math-kernel-library-onemkl.html)
 - Check if your package is the same as in the setup.py file ('/opt/intel/oneapi/mkl/2023.1.0/include'). Update the file 
 accordingly if it was installed in a different path.
 
 
-   
+## R package
+An R package with similiar implementation is also available at CRAN: https://cran.r-project.org/web/packages/sparseSEM/index.html
+
+## OpenMPI
+C/C++ implementation of sparseSEM with openMPI for parallel computation is available in openMPI branch (https://github.com/anhuihng/pySparseSEM/tree/openMPI). 
+
     
 ## Reference
     - Huang A. (2014) Sparse Model Learning for Inferring Genotype and Phenotype Associations. Ph.D Dissertation,
     University of Miami, Coral Gables, FL, USA.
     - Huang A. (2014) sparseSEM: Sparse-Aware Maximum Likelihood for Structural Equation Models. Rpackage
     (https://cran.r-project.org/web/packages/sparseSEM/index.html)
```

### Comparing `sparseSEM-1.0/README.md` & `sparseSEM-1.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,44 @@
 # Elastic Net for Structural Equation Models (SEM)
 
 Anhui Huang | Ph.D. Electrical and Computer Engineering 
 
 <https://scholar.google.com/citations?user=WhDMZEIAAAAJ&hl=en>
 
 
+## PyPI installation 
+`sparseSEM` is available on PyPI:  https://pypi.org/project/sparseSEM/1.0/. Run command `pip install sparseSEM` to install 
+from PyPI.
 
-## Online Documentation
+`test/` folder contains examples using data packed along with this package in `data/` folder. 
+To run `test/` examples, clone this repo, and run from `test/` directory. 
+
+
+## Documentation
 The theory and background for network topology inference using sparse Structural Equation Models (SEM) can be found 
-in my Ph.D dissertation (Huang A. 2014). The experimental study are also available in the documentation in the package.  
+in my Ph.D dissertation (Huang A. 2014). The experimental study are also available in the `doc/` folder in the package.  
 
 
 ## Configuration
 This package was originally developed to leverage high performance computer clusters to enable parallel computation 
 through openMPI.  Users who have access to large scale computational resources can explore the functionality and 
 checkout the openMPI module in this package.
 
 Current package utilizes blas/lapack for high speed computation. To build the C/C++ code, the intel OneMKL library is 
 specified in the package setup. 
 - Install the free OneMKL package (https://www.intel.com/content/www/us/en/docs/oneapi/programming-guide/2023-0/intel-oneapi-math-kernel-library-onemkl.html)
 - Check if your package is the same as in the setup.py file ('/opt/intel/oneapi/mkl/2023.1.0/include'). Update the file 
 accordingly if it was installed in a different path.
 
 
-   
+## R package
+An R package with similiar implementation is also available at CRAN: https://cran.r-project.org/web/packages/sparseSEM/index.html
+
+## OpenMPI
+C/C++ implementation of sparseSEM with openMPI for parallel computation is available in openMPI branch (https://github.com/anhuihng/pySparseSEM/tree/openMPI). 
+
     
 ## Reference
     - Huang A. (2014) Sparse Model Learning for Inferring Genotype and Phenotype Associations. Ph.D Dissertation,
     University of Miami, Coral Gables, FL, USA.
     - Huang A. (2014) sparseSEM: Sparse-Aware Maximum Likelihood for Structural Equation Models. Rpackage
     (https://cran.r-project.org/web/packages/sparseSEM/index.html)
```

### Comparing `sparseSEM-1.0/data/B.csv` & `sparseSEM-1.1/data/B.csv`

 * *Files identical despite different names*

### Comparing `sparseSEM-1.0/data/Missing.csv` & `sparseSEM-1.1/data/Missing.csv`

 * *Files identical despite different names*

### Comparing `sparseSEM-1.0/data/X.csv` & `sparseSEM-1.1/data/X.csv`

 * *Files identical despite different names*

### Comparing `sparseSEM-1.0/data/Y.csv` & `sparseSEM-1.1/data/Y.csv`

 * *Files identical despite different names*

### Comparing `sparseSEM-1.0/doc/.DS_Store` & `sparseSEM-1.1/doc/.DS_Store`

 * *Files identical despite different names*

### Comparing `sparseSEM-1.0/doc/Fig1_nCPU.png` & `sparseSEM-1.1/doc/Fig1_nCPU.png`

 * *Files identical despite different names*

### Comparing `sparseSEM-1.0/doc/Fig2_sigma01.png` & `sparseSEM-1.1/doc/Fig2_sigma01.png`

 * *Files identical despite different names*

### Comparing `sparseSEM-1.0/doc/Fig3_sigma05.png` & `sparseSEM-1.1/doc/Fig3_sigma05.png`

 * *Files identical despite different names*

### Comparing `sparseSEM-1.0/doc/Fig4_cisTransNetworkYeast_clusters_manualAdjusted_GOterm.jpg` & `sparseSEM-1.1/doc/Fig4_cisTransNetworkYeast_clusters_manualAdjusted_GOterm.jpg`

 * *Files identical despite different names*

### Comparing `sparseSEM-1.0/doc/Fig5_yeast_grn_genome_biology.png` & `sparseSEM-1.1/doc/Fig5_yeast_grn_genome_biology.png`

 * *Files identical despite different names*

### Comparing `sparseSEM-1.0/doc/sparseSEM.md` & `sparseSEM-1.1/doc/sparseSEM.md`

 * *Files identical despite different names*

### Comparing `sparseSEM-1.0/doc/sparseSEM.pdf` & `sparseSEM-1.1/doc/sparseSEM.pdf`

 * *Files identical despite different names*

### Comparing `sparseSEM-1.0/doc/table1_data.png` & `sparseSEM-1.1/doc/table1_data.png`

 * *Files identical despite different names*

### Comparing `sparseSEM-1.0/doc/table2_data.png` & `sparseSEM-1.1/doc/table2_data.png`

 * *Files identical despite different names*

### Comparing `sparseSEM-1.0/doc/table3_data.png` & `sparseSEM-1.1/doc/table3_data.png`

 * *Files identical despite different names*

### Comparing `sparseSEM-1.0/setup.py` & `sparseSEM-1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import os
 from setuptools import setup, Extension, find_packages
 
-_VERSION = "1.0"
+_VERSION = "1.1"
 
 sparseSEM_lib = Extension(name='sparseSEM.lassoSML',
-                          sources=[],
+                          sources=['sparseSEM/src/lassoSEM.c',
+                                   'sparseSEM/src/lassoSMLv11beta.c',
+                                   ],
                           include_dirs=['sparseSEM/src',
                                         '/opt/intel/oneapi/mkl/2023.1.0/include'],
                           library_dirs=['/opt/intel/oneapi/mkl/2023.1.0/lib'],
                           libraries=['mkl_rt'],
                           extra_compile_args=['-std=c11', '-O2'])
 
 sparseSEM_lib.name = 'sparseSEM'
```

### Comparing `sparseSEM-1.0/sparseSEM/elasticNetSML.py` & `sparseSEM-1.1/sparseSEM/elasticNetSML.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     Note:
         Regularization path: the lasso-strong rule is applied, thus the path is run through lambda_max to lambda_opt,
         where lambda_max is the lambda that keeps only 1 non-zero edge,and lambda_opt is the optimal lambda from CV.
 
         The program implements the following components:
         Step 1. SEM-ridge regression (L2 penalty) with k-fold CV: this step find the optimal ridge hyperparameter rho
-        Step 2. fit SEM reidge regression model (L2 penalty) with rho from Step 1, obtain the initial status (non-sparse)
+        Step 2. fit SEM ridge regression model (L2 penalty) with rho from Step 1, obtain the initial status (non-sparse)
                 of network structure (B_ridge);
         Step 3.SEM-elastic net regression with k-fold CV: this step finds the optimal hyperparameter (alpha, lambda)
         Step 4. fit SEM-elastic net model with (alpha, lambda) from Step 3.
         Step 5. result calculation for PD, FDR, provide the output
 
 
 FUNCTION INTERFACE:
```

### Comparing `sparseSEM-1.0/sparseSEM/elasticNetSMLcv.py` & `sparseSEM-1.1/sparseSEM/elasticNetSMLcv.py`

 * *Files identical despite different names*

### Comparing `sparseSEM-1.0/sparseSEM/elasticNetSMLpoint.py` & `sparseSEM-1.1/sparseSEM/elasticNetSMLpoint.py`

 * *Files identical despite different names*

### Comparing `sparseSEM-1.0/sparseSEM/loadSEMlib.py` & `sparseSEM-1.1/sparseSEM/loadSEMlib.py`

 * *Files identical despite different names*

### Comparing `sparseSEM-1.0/sparseSEM/sparseSEM.cpython-310-darwin.so` & `sparseSEM-1.1/sparseSEM/sparseSEM.cpython-310-darwin.so`

 * *Files identical despite different names*

### Comparing `sparseSEM-1.0/sparseSEM/src/lassoSEM.c` & `sparseSEM-1.1/sparseSEM/src/lassoSEM.c`

 * *Files identical despite different names*

### Comparing `sparseSEM-1.0/sparseSEM/src/lassoSEM.h` & `sparseSEM-1.1/sparseSEM/src/lassoSEM.h`

 * *Files identical despite different names*

### Comparing `sparseSEM-1.0/sparseSEM/src/lassoSMLv11beta.c` & `sparseSEM-1.1/sparseSEM/src/lassoSMLv11beta.c`

 * *Files identical despite different names*

### Comparing `sparseSEM-1.0/sparseSEM.egg-info/PKG-INFO` & `sparseSEM-1.1/sparseSEM.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparseSEM
-Version: 1.0
+Version: 1.1
 Summary: Python wrapper for sparseSEM
 Home-page: https://scholar.google.com/citations?user=WhDMZEIAAAAJ&hl=en
 Author: Anhui Huang
 Author-email: anhuihuang@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python
@@ -26,32 +26,44 @@
 # Elastic Net for Structural Equation Models (SEM)
 
 Anhui Huang | Ph.D. Electrical and Computer Engineering 
 
 <https://scholar.google.com/citations?user=WhDMZEIAAAAJ&hl=en>
 
 
+## PyPI installation 
+`sparseSEM` is available on PyPI:  https://pypi.org/project/sparseSEM/1.0/. Run command `pip install sparseSEM` to install 
+from PyPI.
 
-## Online Documentation
+`test/` folder contains examples using data packed along with this package in `data/` folder. 
+To run `test/` examples, clone this repo, and run from `test/` directory. 
+
+
+## Documentation
 The theory and background for network topology inference using sparse Structural Equation Models (SEM) can be found 
-in my Ph.D dissertation (Huang A. 2014). The experimental study are also available in the documentation in the package.  
+in my Ph.D dissertation (Huang A. 2014). The experimental study are also available in the `doc/` folder in the package.  
 
 
 ## Configuration
 This package was originally developed to leverage high performance computer clusters to enable parallel computation 
 through openMPI.  Users who have access to large scale computational resources can explore the functionality and 
 checkout the openMPI module in this package.
 
 Current package utilizes blas/lapack for high speed computation. To build the C/C++ code, the intel OneMKL library is 
 specified in the package setup. 
 - Install the free OneMKL package (https://www.intel.com/content/www/us/en/docs/oneapi/programming-guide/2023-0/intel-oneapi-math-kernel-library-onemkl.html)
 - Check if your package is the same as in the setup.py file ('/opt/intel/oneapi/mkl/2023.1.0/include'). Update the file 
 accordingly if it was installed in a different path.
 
 
-   
+## R package
+An R package with similiar implementation is also available at CRAN: https://cran.r-project.org/web/packages/sparseSEM/index.html
+
+## OpenMPI
+C/C++ implementation of sparseSEM with openMPI for parallel computation is available in openMPI branch (https://github.com/anhuihng/pySparseSEM/tree/openMPI). 
+
     
 ## Reference
     - Huang A. (2014) Sparse Model Learning for Inferring Genotype and Phenotype Associations. Ph.D Dissertation,
     University of Miami, Coral Gables, FL, USA.
     - Huang A. (2014) sparseSEM: Sparse-Aware Maximum Likelihood for Structural Equation Models. Rpackage
     (https://cran.r-project.org/web/packages/sparseSEM/index.html)
```

### Comparing `sparseSEM-1.0/sparseSEM.egg-info/SOURCES.txt` & `sparseSEM-1.1/sparseSEM.egg-info/SOURCES.txt`

 * *Files identical despite different names*

