# Comparing `tmp/EBglmnet-1.0.tar.gz` & `tmp/EBglmnet-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EBglmnet-1.0.tar", last modified: Wed May 24 19:05:29 2023, max compression
+gzip compressed data, was "EBglmnet-1.1.tar", last modified: Wed May 24 20:18:40 2023, max compression
```

## Comparing `EBglmnet-1.0.tar` & `EBglmnet-1.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 anhui      (501) staff       (20)        0 2023-05-24 19:05:29.884527 EBglmnet-1.0/
-drwxr-xr-x   0 anhui      (501) staff       (20)        0 2023-05-24 19:05:29.855529 EBglmnet-1.0/EBglmnet/
--rw-r--r--   0 anhui      (501) staff       (20)     3958 2023-05-24 16:26:11.000000 EBglmnet-1.0/EBglmnet/CVonePair.py
--rw-r--r--   0 anhui      (501) staff       (20)     6781 2023-05-24 16:26:11.000000 EBglmnet-1.0/EBglmnet/EBelasticNet.py
--rwxr-xr-x   0 anhui      (501) staff       (20)   101056 2023-05-24 15:47:04.000000 EBglmnet-1.0/EBglmnet/EBglmnet.cpython-310-darwin.so
--rw-r--r--   0 anhui      (501) staff       (20)     6512 2023-05-24 16:26:11.000000 EBglmnet-1.0/EBglmnet/EBlassoNEG.py
--rw-r--r--   0 anhui      (501) staff       (20)    10641 2023-05-22 18:09:49.000000 EBglmnet-1.0/EBglmnet/EmpBayesGlmnet.py
--rw-r--r--   0 anhui      (501) staff       (20)     1222 2023-05-23 20:34:59.000000 EBglmnet-1.0/EBglmnet/__init__.py
--rw-r--r--   0 anhui      (501) staff       (20)     7355 2023-05-24 16:26:11.000000 EBglmnet-1.0/EBglmnet/cvEBelasticNet.py
--rw-r--r--   0 anhui      (501) staff       (20)    10103 2023-05-24 18:40:50.000000 EBglmnet-1.0/EBglmnet/cvEBglmnet.py
--rw-r--r--   0 anhui      (501) staff       (20)     7295 2023-05-24 16:26:11.000000 EBglmnet-1.0/EBglmnet/cvEBlassoNE.py
--rw-r--r--   0 anhui      (501) staff       (20)    11585 2023-05-24 16:26:11.000000 EBglmnet-1.0/EBglmnet/cvEBlassoNEG.py
--rw-r--r--   0 anhui      (501) staff       (20)      913 2023-05-23 02:41:10.000000 EBglmnet-1.0/EBglmnet/lambdaMax.py
--rw-r--r--   0 anhui      (501) staff       (20)      949 2023-05-24 15:48:27.000000 EBglmnet-1.0/EBglmnet/loadEBglmnetLib.py
-drwxr-xr-x   0 anhui      (501) staff       (20)        0 2023-05-24 19:05:29.874494 EBglmnet-1.0/EBglmnet/src/
--rw-r--r--   0 anhui      (501) staff       (20)    11627 2023-05-14 04:36:30.000000 EBglmnet-1.0/EBglmnet/src/Binary.c
--rw-r--r--   0 anhui      (501) staff       (20)     1313 2022-12-20 16:42:16.000000 EBglmnet-1.0/EBglmnet/src/Binary.h
--rw-r--r--   0 anhui      (501) staff       (20)     7134 2023-05-22 14:59:44.000000 EBglmnet-1.0/EBglmnet/src/CVonePara.c
--rw-r--r--   0 anhui      (501) staff       (20)    20218 2023-05-14 04:36:30.000000 EBglmnet-1.0/EBglmnet/src/Linear.c
--rw-r--r--   0 anhui      (501) staff       (20)     3439 2022-12-19 01:39:30.000000 EBglmnet-1.0/EBglmnet/src/Linear.h
--rw-r--r--   0 anhui      (501) staff       (20)     6060 2023-05-14 04:28:16.000000 EBglmnet-1.0/EBglmnet/src/NEG.c
--rw-r--r--   0 anhui      (501) staff       (20)     1396 2023-05-22 14:59:44.000000 EBglmnet-1.0/EBglmnet/src/NEG.h
--rw-r--r--   0 anhui      (501) staff       (20)     3887 2023-05-14 04:28:16.000000 EBglmnet-1.0/EBglmnet/src/elasticNet.c
--rw-r--r--   0 anhui      (501) staff       (20)     1317 2023-05-22 14:59:44.000000 EBglmnet-1.0/EBglmnet/src/elasticNet.h
--rw-r--r--   0 anhui      (501) staff       (20)    13529 2023-05-22 14:59:44.000000 EBglmnet-1.0/EBglmnet/src/elasticNetBinary.c
--rw-r--r--   0 anhui      (501) staff       (20)    14857 2023-05-24 16:05:35.000000 EBglmnet-1.0/EBglmnet/src/elasticNetLinear.c
--rw-r--r--   0 anhui      (501) staff       (20)    11395 2023-05-22 14:59:44.000000 EBglmnet-1.0/EBglmnet/src/fEBBinaryNEG.c
--rw-r--r--   0 anhui      (501) staff       (20)    14939 2023-05-22 14:59:44.000000 EBglmnet-1.0/EBglmnet/src/fEBLinearNEG.c
--rwxr-xr-x   0 anhui      (501) staff       (20)   101056 2023-05-24 15:47:04.000000 EBglmnet-1.0/EBglmnet.cpython-310-darwin.so
-drwxr-xr-x   0 anhui      (501) staff       (20)        0 2023-05-24 19:05:29.859356 EBglmnet-1.0/EBglmnet.egg-info/
--rw-r--r--   0 anhui      (501) staff       (20)     4452 2023-05-24 19:05:29.000000 EBglmnet-1.0/EBglmnet.egg-info/PKG-INFO
--rw-r--r--   0 anhui      (501) staff       (20)      942 2023-05-24 19:05:29.000000 EBglmnet-1.0/EBglmnet.egg-info/SOURCES.txt
--rw-r--r--   0 anhui      (501) staff       (20)        1 2023-05-24 19:05:29.000000 EBglmnet-1.0/EBglmnet.egg-info/dependency_links.txt
--rw-r--r--   0 anhui      (501) staff       (20)       31 2023-05-24 19:05:29.000000 EBglmnet-1.0/EBglmnet.egg-info/requires.txt
--rw-r--r--   0 anhui      (501) staff       (20)        9 2023-05-24 19:05:29.000000 EBglmnet-1.0/EBglmnet.egg-info/top_level.txt
--rw-r--r--   0 anhui      (501) staff       (20)       64 2023-05-24 03:17:47.000000 EBglmnet-1.0/MANIFEST.in
--rw-r--r--   0 anhui      (501) staff       (20)     4452 2023-05-24 19:05:29.884018 EBglmnet-1.0/PKG-INFO
--rw-r--r--   0 anhui      (501) staff       (20)     3421 2023-05-24 19:05:03.000000 EBglmnet-1.0/README.md
-drwxr-xr-x   0 anhui      (501) staff       (20)        0 2023-05-24 19:05:29.880273 EBglmnet-1.0/data/
--rw-r--r--   0 anhui      (501) staff       (20)   328703 2023-05-14 03:43:00.000000 EBglmnet-1.0/data/simulation.csv
--rw-r--r--   0 anhui      (501) staff       (20)      513 2023-05-14 03:43:52.000000 EBglmnet-1.0/data/simulation_parameters.csv
--rw-r--r--   0 anhui      (501) staff       (20)     1996 2023-05-14 03:38:17.000000 EBglmnet-1.0/data/statex77.csv
-drwxr-xr-x   0 anhui      (501) staff       (20)        0 2023-05-24 19:05:29.881208 EBglmnet-1.0/doc/
--rw-r--r--   0 anhui      (501) staff       (20)   187251 2023-05-13 02:55:34.000000 EBglmnet-1.0/doc/EBglmnet_intro.pdf
--rw-r--r--   0 anhui      (501) staff       (20)       38 2023-05-24 19:05:29.884699 EBglmnet-1.0/setup.cfg
--rw-r--r--   0 anhui      (501) staff       (20)     3081 2023-05-24 16:00:34.000000 EBglmnet-1.0/setup.py
+drwxr-xr-x   0 anhui      (501) staff       (20)        0 2023-05-24 20:18:40.919570 EBglmnet-1.1/
+drwxr-xr-x   0 anhui      (501) staff       (20)        0 2023-05-24 20:18:40.892997 EBglmnet-1.1/EBglmnet/
+-rw-r--r--   0 anhui      (501) staff       (20)     3958 2023-05-24 16:26:11.000000 EBglmnet-1.1/EBglmnet/CVonePair.py
+-rw-r--r--   0 anhui      (501) staff       (20)     6781 2023-05-24 16:26:11.000000 EBglmnet-1.1/EBglmnet/EBelasticNet.py
+-rwxr-xr-x   0 anhui      (501) staff       (20)   101056 2023-05-24 15:47:04.000000 EBglmnet-1.1/EBglmnet/EBglmnet.cpython-310-darwin.so
+-rw-r--r--   0 anhui      (501) staff       (20)     6512 2023-05-24 16:26:11.000000 EBglmnet-1.1/EBglmnet/EBlassoNEG.py
+-rw-r--r--   0 anhui      (501) staff       (20)    10641 2023-05-22 18:09:49.000000 EBglmnet-1.1/EBglmnet/EmpBayesGlmnet.py
+-rw-r--r--   0 anhui      (501) staff       (20)     1222 2023-05-23 20:34:59.000000 EBglmnet-1.1/EBglmnet/__init__.py
+-rw-r--r--   0 anhui      (501) staff       (20)     7355 2023-05-24 16:26:11.000000 EBglmnet-1.1/EBglmnet/cvEBelasticNet.py
+-rw-r--r--   0 anhui      (501) staff       (20)    10103 2023-05-24 18:40:50.000000 EBglmnet-1.1/EBglmnet/cvEBglmnet.py
+-rw-r--r--   0 anhui      (501) staff       (20)     7295 2023-05-24 16:26:11.000000 EBglmnet-1.1/EBglmnet/cvEBlassoNE.py
+-rw-r--r--   0 anhui      (501) staff       (20)    11585 2023-05-24 16:26:11.000000 EBglmnet-1.1/EBglmnet/cvEBlassoNEG.py
+-rw-r--r--   0 anhui      (501) staff       (20)      913 2023-05-23 02:41:10.000000 EBglmnet-1.1/EBglmnet/lambdaMax.py
+-rw-r--r--   0 anhui      (501) staff       (20)      949 2023-05-24 15:48:27.000000 EBglmnet-1.1/EBglmnet/loadEBglmnetLib.py
+drwxr-xr-x   0 anhui      (501) staff       (20)        0 2023-05-24 20:18:40.909829 EBglmnet-1.1/EBglmnet/src/
+-rw-r--r--   0 anhui      (501) staff       (20)    11627 2023-05-14 04:36:30.000000 EBglmnet-1.1/EBglmnet/src/Binary.c
+-rw-r--r--   0 anhui      (501) staff       (20)     1313 2022-12-20 16:42:16.000000 EBglmnet-1.1/EBglmnet/src/Binary.h
+-rw-r--r--   0 anhui      (501) staff       (20)     7134 2023-05-22 14:59:44.000000 EBglmnet-1.1/EBglmnet/src/CVonePara.c
+-rw-r--r--   0 anhui      (501) staff       (20)    20218 2023-05-14 04:36:30.000000 EBglmnet-1.1/EBglmnet/src/Linear.c
+-rw-r--r--   0 anhui      (501) staff       (20)     3439 2022-12-19 01:39:30.000000 EBglmnet-1.1/EBglmnet/src/Linear.h
+-rw-r--r--   0 anhui      (501) staff       (20)     6060 2023-05-14 04:28:16.000000 EBglmnet-1.1/EBglmnet/src/NEG.c
+-rw-r--r--   0 anhui      (501) staff       (20)     1396 2023-05-22 14:59:44.000000 EBglmnet-1.1/EBglmnet/src/NEG.h
+-rw-r--r--   0 anhui      (501) staff       (20)     3887 2023-05-14 04:28:16.000000 EBglmnet-1.1/EBglmnet/src/elasticNet.c
+-rw-r--r--   0 anhui      (501) staff       (20)     1317 2023-05-22 14:59:44.000000 EBglmnet-1.1/EBglmnet/src/elasticNet.h
+-rw-r--r--   0 anhui      (501) staff       (20)    13529 2023-05-22 14:59:44.000000 EBglmnet-1.1/EBglmnet/src/elasticNetBinary.c
+-rw-r--r--   0 anhui      (501) staff       (20)    14857 2023-05-24 16:05:35.000000 EBglmnet-1.1/EBglmnet/src/elasticNetLinear.c
+-rw-r--r--   0 anhui      (501) staff       (20)    11395 2023-05-22 14:59:44.000000 EBglmnet-1.1/EBglmnet/src/fEBBinaryNEG.c
+-rw-r--r--   0 anhui      (501) staff       (20)    14939 2023-05-22 14:59:44.000000 EBglmnet-1.1/EBglmnet/src/fEBLinearNEG.c
+-rwxr-xr-x   0 anhui      (501) staff       (20)   101056 2023-05-24 15:47:04.000000 EBglmnet-1.1/EBglmnet.cpython-310-darwin.so
+drwxr-xr-x   0 anhui      (501) staff       (20)        0 2023-05-24 20:18:40.896221 EBglmnet-1.1/EBglmnet.egg-info/
+-rw-r--r--   0 anhui      (501) staff       (20)     4451 2023-05-24 20:18:40.000000 EBglmnet-1.1/EBglmnet.egg-info/PKG-INFO
+-rw-r--r--   0 anhui      (501) staff       (20)      942 2023-05-24 20:18:40.000000 EBglmnet-1.1/EBglmnet.egg-info/SOURCES.txt
+-rw-r--r--   0 anhui      (501) staff       (20)        1 2023-05-24 20:18:40.000000 EBglmnet-1.1/EBglmnet.egg-info/dependency_links.txt
+-rw-r--r--   0 anhui      (501) staff       (20)       31 2023-05-24 20:18:40.000000 EBglmnet-1.1/EBglmnet.egg-info/requires.txt
+-rw-r--r--   0 anhui      (501) staff       (20)        9 2023-05-24 20:18:40.000000 EBglmnet-1.1/EBglmnet.egg-info/top_level.txt
+-rw-r--r--   0 anhui      (501) staff       (20)       64 2023-05-24 03:17:47.000000 EBglmnet-1.1/MANIFEST.in
+-rw-r--r--   0 anhui      (501) staff       (20)     4451 2023-05-24 20:18:40.919007 EBglmnet-1.1/PKG-INFO
+-rw-r--r--   0 anhui      (501) staff       (20)     3421 2023-05-24 19:05:03.000000 EBglmnet-1.1/README.md
+drwxr-xr-x   0 anhui      (501) staff       (20)        0 2023-05-24 20:18:40.915291 EBglmnet-1.1/data/
+-rw-r--r--   0 anhui      (501) staff       (20)   328703 2023-05-14 03:43:00.000000 EBglmnet-1.1/data/simulation.csv
+-rw-r--r--   0 anhui      (501) staff       (20)      513 2023-05-14 03:43:52.000000 EBglmnet-1.1/data/simulation_parameters.csv
+-rw-r--r--   0 anhui      (501) staff       (20)     1996 2023-05-14 03:38:17.000000 EBglmnet-1.1/data/statex77.csv
+drwxr-xr-x   0 anhui      (501) staff       (20)        0 2023-05-24 20:18:40.916352 EBglmnet-1.1/doc/
+-rw-r--r--   0 anhui      (501) staff       (20)   187251 2023-05-13 02:55:34.000000 EBglmnet-1.1/doc/EBglmnet_intro.pdf
+-rw-r--r--   0 anhui      (501) staff       (20)       38 2023-05-24 20:18:40.919751 EBglmnet-1.1/setup.cfg
+-rw-r--r--   0 anhui      (501) staff       (20)     3080 2023-05-24 20:18:35.000000 EBglmnet-1.1/setup.py
```

### Comparing `EBglmnet-1.0/EBglmnet/CVonePair.py` & `EBglmnet-1.1/EBglmnet/CVonePair.py`

 * *Files identical despite different names*

### Comparing `EBglmnet-1.0/EBglmnet/EBelasticNet.py` & `EBglmnet-1.1/EBglmnet/EBelasticNet.py`

 * *Files identical despite different names*

### Comparing `EBglmnet-1.0/EBglmnet/EBglmnet.cpython-310-darwin.so` & `EBglmnet-1.1/EBglmnet/EBglmnet.cpython-310-darwin.so`

 * *Files identical despite different names*

### Comparing `EBglmnet-1.0/EBglmnet/EBlassoNEG.py` & `EBglmnet-1.1/EBglmnet/EBlassoNEG.py`

 * *Files identical despite different names*

### Comparing `EBglmnet-1.0/EBglmnet/EmpBayesGlmnet.py` & `EBglmnet-1.1/EBglmnet/EmpBayesGlmnet.py`

 * *Files identical despite different names*

### Comparing `EBglmnet-1.0/EBglmnet/__init__.py` & `EBglmnet-1.1/EBglmnet/__init__.py`

 * *Files identical despite different names*

### Comparing `EBglmnet-1.0/EBglmnet/cvEBelasticNet.py` & `EBglmnet-1.1/EBglmnet/cvEBelasticNet.py`

 * *Files identical despite different names*

### Comparing `EBglmnet-1.0/EBglmnet/cvEBglmnet.py` & `EBglmnet-1.1/EBglmnet/cvEBglmnet.py`

 * *Files identical despite different names*

### Comparing `EBglmnet-1.0/EBglmnet/cvEBlassoNE.py` & `EBglmnet-1.1/EBglmnet/cvEBlassoNE.py`

 * *Files identical despite different names*

### Comparing `EBglmnet-1.0/EBglmnet/cvEBlassoNEG.py` & `EBglmnet-1.1/EBglmnet/cvEBlassoNEG.py`

 * *Files identical despite different names*

### Comparing `EBglmnet-1.0/EBglmnet/lambdaMax.py` & `EBglmnet-1.1/EBglmnet/lambdaMax.py`

 * *Files identical despite different names*

### Comparing `EBglmnet-1.0/EBglmnet/loadEBglmnetLib.py` & `EBglmnet-1.1/EBglmnet/loadEBglmnetLib.py`

 * *Files identical despite different names*

### Comparing `EBglmnet-1.0/EBglmnet/src/Binary.c` & `EBglmnet-1.1/EBglmnet/src/Binary.c`

 * *Files identical despite different names*

### Comparing `EBglmnet-1.0/EBglmnet/src/Binary.h` & `EBglmnet-1.1/EBglmnet/src/Binary.h`

 * *Files identical despite different names*

### Comparing `EBglmnet-1.0/EBglmnet/src/CVonePara.c` & `EBglmnet-1.1/EBglmnet/src/CVonePara.c`

 * *Files identical despite different names*

### Comparing `EBglmnet-1.0/EBglmnet/src/Linear.c` & `EBglmnet-1.1/EBglmnet/src/Linear.c`

 * *Files identical despite different names*

### Comparing `EBglmnet-1.0/EBglmnet/src/Linear.h` & `EBglmnet-1.1/EBglmnet/src/Linear.h`

 * *Files identical despite different names*

### Comparing `EBglmnet-1.0/EBglmnet/src/NEG.c` & `EBglmnet-1.1/EBglmnet/src/NEG.c`

 * *Files identical despite different names*

### Comparing `EBglmnet-1.0/EBglmnet/src/NEG.h` & `EBglmnet-1.1/EBglmnet/src/NEG.h`

 * *Files identical despite different names*

### Comparing `EBglmnet-1.0/EBglmnet/src/elasticNet.c` & `EBglmnet-1.1/EBglmnet/src/elasticNet.c`

 * *Files identical despite different names*

### Comparing `EBglmnet-1.0/EBglmnet/src/elasticNet.h` & `EBglmnet-1.1/EBglmnet/src/elasticNet.h`

 * *Files identical despite different names*

### Comparing `EBglmnet-1.0/EBglmnet/src/elasticNetBinary.c` & `EBglmnet-1.1/EBglmnet/src/elasticNetBinary.c`

 * *Files identical despite different names*

### Comparing `EBglmnet-1.0/EBglmnet/src/elasticNetLinear.c` & `EBglmnet-1.1/EBglmnet/src/elasticNetLinear.c`

 * *Files identical despite different names*

### Comparing `EBglmnet-1.0/EBglmnet/src/fEBBinaryNEG.c` & `EBglmnet-1.1/EBglmnet/src/fEBBinaryNEG.c`

 * *Files identical despite different names*

### Comparing `EBglmnet-1.0/EBglmnet/src/fEBLinearNEG.c` & `EBglmnet-1.1/EBglmnet/src/fEBLinearNEG.c`

 * *Files identical despite different names*

### Comparing `EBglmnet-1.0/EBglmnet.cpython-310-darwin.so` & `EBglmnet-1.1/EBglmnet.cpython-310-darwin.so`

 * *Files identical despite different names*

### Comparing `EBglmnet-1.0/EBglmnet.egg-info/PKG-INFO` & `EBglmnet-1.1/EBglmnet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: EBglmnet
-Version: 1.0
-Summary: Python wrapper for sparseSEM
+Version: 1.1
+Summary: Python wrapper for EBglmnet
 Home-page: https://scholar.google.com/citations?user=WhDMZEIAAAAJ&hl=en
 Author: Anhui Huang
 Author-email: anhuihuang@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `EBglmnet-1.0/EBglmnet.egg-info/SOURCES.txt` & `EBglmnet-1.1/EBglmnet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `EBglmnet-1.0/PKG-INFO` & `EBglmnet-1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: EBglmnet
-Version: 1.0
-Summary: Python wrapper for sparseSEM
+Version: 1.1
+Summary: Python wrapper for EBglmnet
 Home-page: https://scholar.google.com/citations?user=WhDMZEIAAAAJ&hl=en
 Author: Anhui Huang
 Author-email: anhuihuang@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `EBglmnet-1.0/README.md` & `EBglmnet-1.1/README.md`

 * *Files identical despite different names*

### Comparing `EBglmnet-1.0/data/simulation.csv` & `EBglmnet-1.1/data/simulation.csv`

 * *Files identical despite different names*

### Comparing `EBglmnet-1.0/data/simulation_parameters.csv` & `EBglmnet-1.1/data/simulation_parameters.csv`

 * *Files identical despite different names*

### Comparing `EBglmnet-1.0/data/statex77.csv` & `EBglmnet-1.1/data/statex77.csv`

 * *Files identical despite different names*

### Comparing `EBglmnet-1.0/doc/EBglmnet_intro.pdf` & `EBglmnet-1.1/doc/EBglmnet_intro.pdf`

 * *Files identical despite different names*

### Comparing `EBglmnet-1.0/setup.py` & `EBglmnet-1.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from setuptools import setup, Extension, find_packages
 import subprocess
-_VERSION = "1.0"
+_VERSION = "1.1"
 
 EBglmnet_lib = Extension(name='EBglmnet.EBglmnet',
                           sources=['EBglmnet/src/Binary.c',
                                     'EBglmnet/src/CVonePara.c',
                                     'EBglmnet/src/elasticNet.c',
                                     'EBglmnet/src/elasticNetBinary.c',
                                     'EBglmnet/src/elasticNetLinear.c',
@@ -22,15 +22,15 @@
 
 EBglmnet_lib.name = 'EBglmnet'
 
 if __name__ == "__main__":
     setup(
         name="EBglmnet",
         version=_VERSION,
-        description="Python wrapper for sparseSEM",
+        description="Python wrapper for EBglmnet",
         long_description_content_type="text/markdown",
         long_description=open('README.md').read(),
         author="Anhui Huang",
         author_email="anhuihuang@gmail.com",
         url="https://scholar.google.com/citations?user=WhDMZEIAAAAJ&hl=en",
         install_requires=[
             "numpy>=1.9.2",
```

