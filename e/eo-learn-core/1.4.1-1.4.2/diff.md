# Comparing `tmp/eo-learn-core-1.4.1.tar.gz` & `tmp/eo-learn-core-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eo-learn-core-1.4.1.tar", last modified: Tue Mar 14 10:32:52 2023, max compression
+gzip compressed data, was "eo-learn-core-1.4.2.tar", last modified: Wed May 24 10:46:31 2023, max compression
```

## Comparing `eo-learn-core-1.4.1.tar` & `eo-learn-core-1.4.2.tar`

### file list

```diff
@@ -1,48 +1,47 @@
-drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-03-14 10:32:52.263625 eo-learn-core-1.4.1/
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1745 2023-03-14 10:32:51.000000 eo-learn-core-1.4.1/LICENSE
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      214 2022-10-06 11:34:49.000000 eo-learn-core-1.4.1/MANIFEST.in
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1858 2023-03-14 10:32:52.263625 eo-learn-core-1.4.1/PKG-INFO
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      378 2023-03-14 10:22:12.000000 eo-learn-core-1.4.1/README.md
-drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-03-14 10:32:52.235625 eo-learn-core-1.4.1/eo_learn_core.egg-info/
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1858 2023-03-14 10:32:52.000000 eo-learn-core-1.4.1/eo_learn_core.egg-info/PKG-INFO
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1054 2023-03-14 10:32:52.000000 eo-learn-core-1.4.1/eo_learn_core.egg-info/SOURCES.txt
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)        1 2023-03-14 10:32:52.000000 eo-learn-core-1.4.1/eo_learn_core.egg-info/dependency_links.txt
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)        1 2021-04-28 12:52:20.000000 eo-learn-core-1.4.1/eo_learn_core.egg-info/not-zip-safe
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      146 2023-03-14 10:32:52.000000 eo-learn-core-1.4.1/eo_learn_core.egg-info/requires.txt
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)        8 2023-03-14 10:32:52.000000 eo-learn-core-1.4.1/eo_learn_core.egg-info/top_level.txt
-drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-03-14 10:32:52.235625 eo-learn-core-1.4.1/eolearn/
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       65 2022-05-03 09:13:51.000000 eo-learn-core-1.4.1/eolearn/__init__.py
-drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-03-14 10:32:52.251625 eo-learn-core-1.4.1/eolearn/core/
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1042 2023-03-14 10:22:12.000000 eo-learn-core-1.4.1/eolearn/core/__init__.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)    12013 2023-03-14 10:22:12.000000 eo-learn-core-1.4.1/eolearn/core/constants.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)    22795 2023-03-14 10:22:12.000000 eo-learn-core-1.4.1/eolearn/core/core_tasks.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)    34480 2023-03-14 10:22:12.000000 eo-learn-core-1.4.1/eolearn/core/eodata.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)    23985 2023-03-14 10:22:12.000000 eo-learn-core-1.4.1/eolearn/core/eodata_io.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)    13702 2023-03-14 10:22:12.000000 eo-learn-core-1.4.1/eolearn/core/eodata_merge.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)    18107 2023-03-14 10:22:12.000000 eo-learn-core-1.4.1/eolearn/core/eoexecution.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     4191 2023-03-14 10:22:12.000000 eo-learn-core-1.4.1/eolearn/core/eonode.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     4960 2023-03-14 10:22:12.000000 eo-learn-core-1.4.1/eolearn/core/eotask.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)    16505 2023-03-14 10:22:12.000000 eo-learn-core-1.4.1/eolearn/core/eoworkflow.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     2202 2023-03-14 10:22:12.000000 eo-learn-core-1.4.1/eolearn/core/eoworkflow_tasks.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      801 2023-03-14 10:22:12.000000 eo-learn-core-1.4.1/eolearn/core/exceptions.py
-drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-03-14 10:32:52.251625 eo-learn-core-1.4.1/eolearn/core/extra/
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       64 2022-05-03 09:13:51.000000 eo-learn-core-1.4.1/eolearn/core/extra/__init__.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     5859 2023-03-14 10:22:12.000000 eo-learn-core-1.4.1/eolearn/core/extra/ray.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     8098 2023-03-14 10:22:12.000000 eo-learn-core-1.4.1/eolearn/core/graph.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)        0 2022-10-06 11:16:15.000000 eo-learn-core-1.4.1/eolearn/core/py.typed
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1880 2023-03-14 10:22:12.000000 eo-learn-core-1.4.1/eolearn/core/types.py
-drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-03-14 10:32:52.263625 eo-learn-core-1.4.1/eolearn/core/utils/
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       41 2022-05-03 09:13:51.000000 eo-learn-core-1.4.1/eolearn/core/utils/__init__.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     4846 2023-03-14 10:22:12.000000 eo-learn-core-1.4.1/eolearn/core/utils/common.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     8310 2023-03-14 10:22:12.000000 eo-learn-core-1.4.1/eolearn/core/utils/fs.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1131 2023-03-14 10:22:12.000000 eo-learn-core-1.4.1/eolearn/core/utils/logging.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     9276 2023-03-14 10:22:12.000000 eo-learn-core-1.4.1/eolearn/core/utils/parallelize.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)    16423 2023-03-14 10:22:12.000000 eo-learn-core-1.4.1/eolearn/core/utils/parsing.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     5303 2023-03-14 10:22:12.000000 eo-learn-core-1.4.1/eolearn/core/utils/raster.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     4034 2023-03-14 10:22:12.000000 eo-learn-core-1.4.1/eolearn/core/utils/testing.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      382 2023-01-20 10:41:16.000000 eo-learn-core-1.4.1/eolearn/core/utils/types.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     2005 2023-03-14 10:22:12.000000 eo-learn-core-1.4.1/eolearn/core/utils/vector_io.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       13 2022-05-03 09:13:51.000000 eo-learn-core-1.4.1/requirements-ray.txt
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      126 2023-03-14 10:22:12.000000 eo-learn-core-1.4.1/requirements.txt
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       38 2023-03-14 10:32:52.263625 eo-learn-core-1.4.1/setup.cfg
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     2666 2022-10-06 11:34:49.000000 eo-learn-core-1.4.1/setup.py
+drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-05-24 10:46:31.371440 eo-learn-core-1.4.2/
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1745 2023-05-24 10:46:31.000000 eo-learn-core-1.4.2/LICENSE
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      214 2023-05-03 06:39:37.000000 eo-learn-core-1.4.2/MANIFEST.in
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1859 2023-05-24 10:46:31.371440 eo-learn-core-1.4.2/PKG-INFO
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      378 2023-05-03 06:39:37.000000 eo-learn-core-1.4.2/README.md
+drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-05-24 10:46:31.339440 eo-learn-core-1.4.2/eo_learn_core.egg-info/
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1859 2023-05-24 10:46:31.000000 eo-learn-core-1.4.2/eo_learn_core.egg-info/PKG-INFO
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1022 2023-05-24 10:46:31.000000 eo-learn-core-1.4.2/eo_learn_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)        1 2023-05-24 10:46:31.000000 eo-learn-core-1.4.2/eo_learn_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)        1 2021-04-28 12:52:20.000000 eo-learn-core-1.4.2/eo_learn_core.egg-info/not-zip-safe
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      133 2023-05-24 10:46:31.000000 eo-learn-core-1.4.2/eo_learn_core.egg-info/requires.txt
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)        8 2023-05-24 10:46:31.000000 eo-learn-core-1.4.2/eo_learn_core.egg-info/top_level.txt
+drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-05-24 10:46:31.339440 eo-learn-core-1.4.2/eolearn/
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       65 2023-05-23 14:00:11.000000 eo-learn-core-1.4.2/eolearn/__init__.py
+drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-05-24 10:46:31.359440 eo-learn-core-1.4.2/eolearn/core/
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1084 2023-05-24 10:35:48.000000 eo-learn-core-1.4.2/eolearn/core/__init__.py
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)    13792 2023-05-24 10:35:48.000000 eo-learn-core-1.4.2/eolearn/core/constants.py
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)    22696 2023-05-24 10:35:48.000000 eo-learn-core-1.4.2/eolearn/core/core_tasks.py
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)    33762 2023-05-24 10:35:48.000000 eo-learn-core-1.4.2/eolearn/core/eodata.py
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)    23822 2023-05-24 10:35:48.000000 eo-learn-core-1.4.2/eolearn/core/eodata_io.py
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)    13360 2023-05-24 10:35:48.000000 eo-learn-core-1.4.2/eolearn/core/eodata_merge.py
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)    18004 2023-05-24 10:35:48.000000 eo-learn-core-1.4.2/eolearn/core/eoexecution.py
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     4191 2023-05-23 14:10:09.000000 eo-learn-core-1.4.2/eolearn/core/eonode.py
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     4894 2023-05-24 10:35:48.000000 eo-learn-core-1.4.2/eolearn/core/eotask.py
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)    16493 2023-05-24 10:35:48.000000 eo-learn-core-1.4.2/eolearn/core/eoworkflow.py
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     2164 2023-05-24 10:35:48.000000 eo-learn-core-1.4.2/eolearn/core/eoworkflow_tasks.py
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      801 2023-05-23 14:10:09.000000 eo-learn-core-1.4.2/eolearn/core/exceptions.py
+drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-05-24 10:46:31.359440 eo-learn-core-1.4.2/eolearn/core/extra/
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       64 2023-05-18 08:30:49.000000 eo-learn-core-1.4.2/eolearn/core/extra/__init__.py
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     5885 2023-05-24 10:35:48.000000 eo-learn-core-1.4.2/eolearn/core/extra/ray.py
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     8103 2023-05-24 10:35:48.000000 eo-learn-core-1.4.2/eolearn/core/graph.py
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)        0 2023-05-03 06:39:37.000000 eo-learn-core-1.4.2/eolearn/core/py.typed
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1858 2023-05-24 10:35:48.000000 eo-learn-core-1.4.2/eolearn/core/types.py
+drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-05-24 10:46:31.371440 eo-learn-core-1.4.2/eolearn/core/utils/
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       41 2023-05-03 06:34:57.000000 eo-learn-core-1.4.2/eolearn/core/utils/__init__.py
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     4866 2023-05-24 10:35:48.000000 eo-learn-core-1.4.2/eolearn/core/utils/common.py
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     8379 2023-05-24 10:35:48.000000 eo-learn-core-1.4.2/eolearn/core/utils/fs.py
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1131 2023-05-23 14:10:09.000000 eo-learn-core-1.4.2/eolearn/core/utils/logging.py
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     9283 2023-05-24 10:35:48.000000 eo-learn-core-1.4.2/eolearn/core/utils/parallelize.py
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)    16343 2023-05-24 10:35:48.000000 eo-learn-core-1.4.2/eolearn/core/utils/parsing.py
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     5288 2023-05-24 10:35:48.000000 eo-learn-core-1.4.2/eolearn/core/utils/raster.py
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     4196 2023-05-24 10:35:48.000000 eo-learn-core-1.4.2/eolearn/core/utils/testing.py
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      387 2023-05-24 10:35:48.000000 eo-learn-core-1.4.2/eolearn/core/utils/types.py
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       13 2023-05-03 06:34:57.000000 eo-learn-core-1.4.2/requirements-ray.txt
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      113 2023-05-24 10:35:48.000000 eo-learn-core-1.4.2/requirements.txt
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       38 2023-05-24 10:46:31.371440 eo-learn-core-1.4.2/setup.cfg
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     2626 2023-05-24 10:35:48.000000 eo-learn-core-1.4.2/setup.py
```

### Comparing `eo-learn-core-1.4.1/LICENSE` & `eo-learn-core-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `eo-learn-core-1.4.1/PKG-INFO` & `eo-learn-core-1.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eo-learn-core
-Version: 1.4.1
+Version: 1.4.2
 Summary: Core Machine Learning Framework at Sinergise
 Home-page: https://github.com/sentinel-hub/eo-learn
 Author: Sinergise EO research team
 Author-email: eoresearch@sinergise.com
 License: MIT
 Project-URL: Documentation, https://eo-learn.readthedocs.io
 Project-URL: Source Code, https://github.com/sentinel-hub/eo-learn
@@ -23,17 +23,17 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Scientific/Engineering :: Image Processing
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: RAY
```

### Comparing `eo-learn-core-1.4.1/eo_learn_core.egg-info/PKG-INFO` & `eo-learn-core-1.4.2/eo_learn_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eo-learn-core
-Version: 1.4.1
+Version: 1.4.2
 Summary: Core Machine Learning Framework at Sinergise
 Home-page: https://github.com/sentinel-hub/eo-learn
 Author: Sinergise EO research team
 Author-email: eoresearch@sinergise.com
 License: MIT
 Project-URL: Documentation, https://eo-learn.readthedocs.io
 Project-URL: Source Code, https://github.com/sentinel-hub/eo-learn
@@ -23,17 +23,17 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Scientific/Engineering :: Image Processing
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: RAY
```

### Comparing `eo-learn-core-1.4.1/eo_learn_core.egg-info/SOURCES.txt` & `eo-learn-core-1.4.2/eo_learn_core.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -32,9 +32,8 @@
 eolearn/core/utils/common.py
 eolearn/core/utils/fs.py
 eolearn/core/utils/logging.py
 eolearn/core/utils/parallelize.py
 eolearn/core/utils/parsing.py
 eolearn/core/utils/raster.py
 eolearn/core/utils/testing.py
-eolearn/core/utils/types.py
-eolearn/core/utils/vector_io.py
+eolearn/core/utils/types.py
```

### Comparing `eo-learn-core-1.4.1/eolearn/core/__init__.py` & `eo-learn-core-1.4.2/eolearn/core/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,18 +18,19 @@
     MoveFeatureTask,
     RemoveFeatureTask,
     RenameFeatureTask,
     SaveTask,
     ZipFeatureTask,
 )
 from .eodata import EOPatch
+from .eodata_merge import merge_eopatches
 from .eoexecution import EOExecutor
 from .eonode import EONode, linearly_connect_tasks
 from .eotask import EOTask
 from .eoworkflow import EOWorkflow, WorkflowResults
 from .eoworkflow_tasks import OutputTask
 from .utils.common import deep_eq
 from .utils.fs import get_filesystem, load_s3_filesystem, pickle_fs, unpickle_fs
 from .utils.parallelize import execute_with_mp_lock, join_futures, join_futures_iter, parallelize
 from .utils.parsing import FeatureParser
 
-__version__ = "1.4.1"
+__version__ = "1.4.2"
```

### Comparing `eo-learn-core-1.4.1/eolearn/core/constants.py` & `eo-learn-core-1.4.2/eolearn/core/constants.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,45 +4,46 @@
 Copyright (c) 2017- Sinergise and contributors
 For the full list of contributors, see the CREDITS file in the root directory of this source tree.
 
 This source code is licensed under the MIT license, see the LICENSE file in the root directory of this source tree.
 """
 import warnings
 from enum import Enum, EnumMeta
-from typing import Any, Optional
+from typing import Any, Optional, TypeVar
 
 from sentinelhub import BBox, MimeType
 from sentinelhub.exceptions import deprecated_function
 
 from .exceptions import EODeprecationWarning
 
 TIMESTAMP_COLUMN = "TIMESTAMP"
+T = TypeVar("T")
 
 
-def _warn_and_adjust(name: str) -> str:
+def _warn_and_adjust(name: T) -> T:
     # since we stick with `UPPER` for attributes and `lower` for values, we include both to reuse function
-    deprecation_msg = None
+    deprecation_msg = None  # placeholder
     if name in ("TIMESTAMP", "timestamp"):
-        name = "TIMESTAMPS" if name == "TIMESTAMP" else "timestamps"
+        name = "TIMESTAMPS" if name == "TIMESTAMP" else "timestamps"  # type: ignore[assignment]
 
     if deprecation_msg:
-        warnings.warn(deprecation_msg, category=EODeprecationWarning, stacklevel=3)  # type: ignore
+        warnings.warn(deprecation_msg, category=EODeprecationWarning, stacklevel=3)  # type: ignore[unreachable]
     return name
 
 
 class EnumWithDeprecations(EnumMeta):
     """A custom EnumMeta class for catching the deprecated Enum members of the FeatureType Enum class."""
 
-    def __getattribute__(cls, name: str) -> Any:
+    def __getattribute__(cls, name: str) -> Any:  # noqa[N805]
         return super().__getattribute__(_warn_and_adjust(name))
 
-    def __getitem__(cls, name: str) -> Any:
+    def __getitem__(cls, name: str) -> Any:  # noqa[N805]
         return super().__getitem__(_warn_and_adjust(name))
 
-    def __call__(cls, value: str, *args: Any, **kwargs: Any) -> Any:
+    def __call__(cls, value: str, *args: Any, **kwargs: Any) -> Any:  # noqa[N805]
         return super().__call__(_warn_and_adjust(value), *args, **kwargs)
 
 
 class FeatureType(Enum, metaclass=EnumWithDeprecations):
     """The Enum class of all possible feature types that can be included in EOPatch.
 
     List of feature types:
@@ -288,21 +289,58 @@
     )
     RASTER_TYPES_4D = frozenset([FeatureType.DATA, FeatureType.MASK])
     RASTER_TYPES_3D = frozenset([FeatureType.DATA_TIMELESS, FeatureType.MASK_TIMELESS])
     RASTER_TYPES_2D = frozenset([FeatureType.SCALAR, FeatureType.LABEL])
     RASTER_TYPES_1D = frozenset([FeatureType.SCALAR_TIMELESS, FeatureType.LABEL_TIMELESS])
 
 
-class OverwritePermission(Enum):
-    """Enum class which specifies which content of saved EOPatch can be overwritten when saving new content.
+def _warn_and_adjust_permissions(name: T) -> T:
+    if isinstance(name, str) and name.upper() == "OVERWRITE_PATCH":
+        warnings.warn(
+            '"OVERWRITE_PATCH" permission is deprecated and will be removed in a future version',
+            category=EODeprecationWarning,
+            stacklevel=3,
+        )
+    return name
+
+
+class PermissionsWithDeprecations(EnumMeta):
+    """A custom EnumMeta class for catching the deprecated Enum members of the OverwritePermission Enum class."""
+
+    def __getattribute__(cls, name: str) -> Any:  # noqa[N805]
+        return super().__getattribute__(_warn_and_adjust_permissions(name))
+
+    def __getitem__(cls, name: str) -> Any:  # noqa[N805]
+        return super().__getitem__(_warn_and_adjust_permissions(name))
+
+    def __call__(cls, value: str, *args: Any, **kwargs: Any) -> Any:  # noqa[N805]
+        return super().__call__(_warn_and_adjust_permissions(value), *args, **kwargs)
+
+
+class OverwritePermission(Enum, metaclass=PermissionsWithDeprecations):
+    """Enum class which specifies which content of the saved EOPatch can be overwritten when saving new content.
 
     Permissions are in the following hierarchy:
 
     - `ADD_ONLY` - Only new features can be added, anything that is already saved cannot be changed.
     - `OVERWRITE_FEATURES` - Overwrite only data for features which have to be saved. The remaining content of saved
       EOPatch will stay unchanged.
-    - `OVERWRITE_PATCH` - Overwrite entire content of saved EOPatch and replace it with the new content.
     """
 
-    ADD_ONLY = 0
-    OVERWRITE_FEATURES = 1
-    OVERWRITE_PATCH = 2
+    ADD_ONLY = "ADD_ONLY"
+    OVERWRITE_FEATURES = "OVERWRITE_FEATURES"
+    OVERWRITE_PATCH = "OVERWRITE_PATCH"
+
+    @classmethod
+    def _missing_(cls, value: object) -> "OverwritePermission":
+        permissions_mapping = {0: "ADD_ONLY", 1: "OVERWRITE_FEATURES", 2: "OVERWRITE_PATCH"}
+        if isinstance(value, int) and value in permissions_mapping:
+            deprecation_msg = (
+                f"Please use strings to instantiate overwrite permissions, e.g., instead of {value} use"
+                f" {permissions_mapping[value]!r}"
+            )
+            warnings.warn(deprecation_msg, category=EODeprecationWarning, stacklevel=3)
+
+            return cls(permissions_mapping[value])
+        if isinstance(value, str) and value.upper() in cls._value2member_map_:
+            return cls(value.upper())
+        return super()._missing_(value)
```

### Comparing `eo-learn-core-1.4.1/eolearn/core/core_tasks.py` & `eo-learn-core-1.4.2/eolearn/core/core_tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,25 @@
 
 This source code is licensed under the MIT license, see the LICENSE file in the root directory of this source tree.
 """
 from __future__ import annotations
 
 import copy
 from abc import ABCMeta
-from typing import Any, Callable, Dict, Iterable, List, Optional, Tuple, Union, cast
+from typing import Any, Callable, Iterable, Tuple, Union, cast
 
 import fs
 import numpy as np
 from fs.base import FS
 
 from sentinelhub import SHConfig
 
 from .constants import FeatureType
 from .eodata import EOPatch
+from .eodata_merge import merge_eopatches
 from .eotask import EOTask
 from .types import FeatureSpec, FeaturesSpecification, SingleFeatureSpec
 from .utils.fs import get_filesystem, pickle_fs, unpickle_fs
 
 
 class CopyTask(EOTask):
     """Makes a shallow copy of the given EOPatch.
@@ -44,20 +45,18 @@
 class DeepCopyTask(CopyTask):
     """Makes a deep copy of the given EOPatch."""
 
     def execute(self, eopatch: EOPatch) -> EOPatch:
         return eopatch.copy(features=self.features, deep=True)
 
 
-class IOTask(EOTask, metaclass=ABCMeta):  # noqa B024
+class IOTask(EOTask, metaclass=ABCMeta):
     """An abstract Input/Output task that can handle a path and a filesystem object."""
 
-    def __init__(
-        self, path: str, filesystem: Optional[FS] = None, create: bool = False, config: Optional[SHConfig] = None
-    ):
+    def __init__(self, path: str, filesystem: FS | None = None, create: bool = False, config: SHConfig | None = None):
         """
         :param path: root path where all EOPatches are saved
         :param filesystem: An existing filesystem object. If not given it will be initialized according to the EOPatch
             path.
         :param create: If the filesystem path doesn't exist this flag indicates to either create it or raise an error
         :param config: A configuration object with AWS credentials. By default, is set to None and in this case the
             default configuration will be taken.
@@ -79,15 +78,15 @@
 
         return unpickle_fs(self._pickled_filesystem)
 
 
 class SaveTask(IOTask):
     """Saves the given EOPatch to a filesystem."""
 
-    def __init__(self, path: str, filesystem: Optional[FS] = None, config: Optional[SHConfig] = None, **kwargs: Any):
+    def __init__(self, path: str, filesystem: FS | None = None, config: SHConfig | None = None, **kwargs: Any):
         """
         :param path: root path where all EOPatches are saved
         :param filesystem: An existing filesystem object. If not given it will be initialized according to the EOPatch
             path.
         :param features: A collection of features types specifying features of which type will be saved. By default,
             all features will be saved.
         :param overwrite_permission: A level of permission for overwriting an existing EOPatch
@@ -110,40 +109,38 @@
         eopatch.save(path, filesystem=self.filesystem, **self.kwargs)
         return eopatch
 
 
 class LoadTask(IOTask):
     """Loads an EOPatch from a filesystem."""
 
-    def __init__(self, path: str, filesystem: Optional[FS] = None, config: Optional[SHConfig] = None, **kwargs: Any):
+    def __init__(self, path: str, filesystem: FS | None = None, config: SHConfig | None = None, **kwargs: Any):
         """
         :param path: root directory where all EOPatches are saved
         :param filesystem: An existing filesystem object. If not given it will be initialized according to the EOPatch
             path. If you intend to run this task in multiprocessing mode you shouldn't specify this parameter.
         :param features: A collection of features to be loaded. By default, all features will be loaded.
         :param lazy_loading: If `True` features will be lazy loaded. Default is `False`
         :param config: A configuration object with AWS credentials. By default, is set to None and in this case the
             default configuration will be taken.
         """
         self.kwargs = kwargs
         super().__init__(path, filesystem=filesystem, create=False, config=config)
 
-    def execute(self, eopatch: Optional[EOPatch] = None, *, eopatch_folder: str = "") -> EOPatch:
+    def execute(self, eopatch: EOPatch | None = None, *, eopatch_folder: str = "") -> EOPatch:
         """Loads the EOPatch from disk: `folder/eopatch_folder`.
 
         :param eopatch: Optional input EOPatch. If given the loaded features are merged onto it, otherwise a new EOPatch
             is created.
         :param eopatch_folder: Name of EOPatch folder containing data.
         :return: EOPatch loaded from disk
         """
         path = fs.path.combine(self.filesystem_path, eopatch_folder)
         loaded_patch = EOPatch.load(path, filesystem=self.filesystem, **self.kwargs)
-        if eopatch is None:
-            return loaded_patch
-        return eopatch.merge(loaded_patch)
+        return loaded_patch if eopatch is None else merge_eopatches(eopatch, loaded_patch)
 
 
 class AddFeatureTask(EOTask):
     """Adds a feature to the given EOPatch."""
 
     def __init__(self, feature: FeatureSpec):
         """
@@ -253,29 +250,29 @@
         # Initialize data of the same shape as (FeatureType.DATA, 'data1')
         InitializeFeature((FeatureType.MASK, 'mask1'), shape=(FeatureType.DATA, 'data1'), init_value=1)
     """
 
     def __init__(
         self,
         features: FeaturesSpecification,
-        shape: Union[Tuple[int, ...], FeatureSpec],
+        shape: tuple[int, ...] | FeatureSpec,
         init_value: int = 0,
-        dtype: Union[np.dtype, type] = np.uint8,
+        dtype: np.dtype | type = np.uint8,
     ):
         """
         :param features: A collection of features to initialize.
         :param shape: A shape object (t, n, m, d) or a feature from which to read the shape.
         :param init_value: A value with which to initialize the array of the new feature.
         :param dtype: Type of array values.
         :raises ValueError: Raises an exception when passing the wrong shape argument.
         """
 
         self.features = self.parse_features(features)
-        self.shape_feature: Optional[Tuple[FeatureType, Optional[str]]]
-        self.shape: Union[None, Tuple[int, int, int], Tuple[int, int, int, int]]
+        self.shape_feature: tuple[FeatureType, str | None] | None
+        self.shape: None | tuple[int, int, int] | tuple[int, int, int, int]
 
         try:
             self.shape_feature = self.parse_feature(shape)  # type: ignore[arg-type]
         except ValueError:
             self.shape_feature = None
 
         if self.shape_feature:
@@ -369,15 +366,15 @@
         result = maximum(patch)
     """
 
     def __init__(
         self,
         input_features: FeaturesSpecification,
         output_features: FeaturesSpecification,
-        map_function: Optional[Callable] = None,
+        map_function: Callable | None = None,
         **kwargs: Any,
     ):
         """
         :param input_features: A collection of the input features to be mapped.
         :param output_features: A collection of the output features to which to assign the output data.
         :param map_function: A function or lambda to be applied to the input data.
         :raises ValueError: Raises an exception when passing feature collections with different lengths.
@@ -449,15 +446,15 @@
             result = maximum(patch)
     """
 
     def __init__(
         self,
         input_features: FeaturesSpecification,
         output_feature: SingleFeatureSpec,
-        zip_function: Optional[Callable] = None,
+        zip_function: Callable | None = None,
         **kwargs: Any,
     ):
         """
         :param input_features: A collection of the input features to be mapped.
         :param output_feature: An output feature object to which to assign the data.
         :param zip_function: A function or lambda to be applied to the input data.
         :param kwargs: kwargs to be passed to the zip function.
@@ -486,23 +483,23 @@
         """A function that will be applied to the input features if overridden."""
         raise NotImplementedError("zip_method should be overridden.")
 
 
 class MergeFeatureTask(ZipFeatureTask):
     """Merges multiple features together by concatenating their data along the specified axis."""
 
-    def zip_method(self, *f: np.ndarray, dtype: Union[None, np.dtype, type] = None, axis: int = -1) -> np.ndarray:
+    def zip_method(self, *f: np.ndarray, dtype: None | np.dtype | type = None, axis: int = -1) -> np.ndarray:
         """Concatenates the data of features along the specified axis."""
         return np.concatenate(f, axis=axis, dtype=dtype)  # pylint: disable=unexpected-keyword-arg
 
 
 class ExtractBandsTask(MapFeatureTask):
     """Moves a subset of bands from one feature to a new one."""
 
-    def __init__(self, input_feature: FeaturesSpecification, output_feature: FeaturesSpecification, bands: List[int]):
+    def __init__(self, input_feature: FeaturesSpecification, output_feature: FeaturesSpecification, bands: list[int]):
         """
         :param input_feature: A source feature from which to take the subset of bands.
         :param output_feature: An output feature to which to write the bands.
         :param bands: A list of bands to be moved.
         """
         super().__init__(input_feature, output_feature)
         self.bands = bands
@@ -515,16 +512,16 @@
 
 
 class ExplodeBandsTask(EOTask):
     """Explode a subset of bands from one feature to multiple new features."""
 
     def __init__(
         self,
-        input_feature: Tuple[FeatureType, str],
-        output_mapping: Dict[Tuple[FeatureType, str], Union[int, Iterable[int]]],
+        input_feature: tuple[FeatureType, str],
+        output_mapping: dict[tuple[FeatureType, str], int | Iterable[int]],
     ):
         """
         :param input_feature: A source feature from which to take the subset of bands.
         :param output_mapping: A mapping of output features into the band indices used to explode the input feature.
         """
         self.input_feature = input_feature
         self.output_mapping = output_mapping
@@ -549,25 +546,25 @@
         """
         return EOPatch(**kwargs)
 
 
 class MergeEOPatchesTask(EOTask):
     """Merge content from multiple EOPatches into a single EOPatch.
 
-    Check :func:`EOPatch.merge<eolearn.core.eodata.EOPatch.merge>` for more information about the merging process.
+    Check :func:`merge_eopatches<eolearn.core.eodata_merge.merge_eopatches>` for more information.
     """
 
     def __init__(self, **merge_kwargs: Any):
         """
-        :param merge_kwargs: Keyword arguments defined for `EOPatch.merge` method.
+        :param merge_kwargs: Keyword arguments defined for `merge_eopatches` function.
         """
         self.merge_kwargs = merge_kwargs
 
     def execute(self, *eopatches: EOPatch) -> EOPatch:
         """
         :param eopatches: EOPatches to be merged
         :return: A new EOPatch with merged content
         """
         if not eopatches:
             raise ValueError("At least one EOPatch should be given")
 
-        return eopatches[0].merge(*eopatches[1:], **self.merge_kwargs)
+        return merge_eopatches(*eopatches, **self.merge_kwargs)
```

### Comparing `eo-learn-core-1.4.1/eolearn/core/eodata.py` & `eo-learn-core-1.4.2/eolearn/core/eodata.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,189 +5,171 @@
 For the full list of contributors, see the CREDITS file in the root directory of this source tree.
 
 This source code is licensed under the MIT license, see the LICENSE file in the root directory of this source tree.
 """
 from __future__ import annotations
 
 import concurrent.futures
+import contextlib
 import copy
 import datetime as dt
 import logging
 from abc import ABCMeta, abstractmethod
-from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Set, Tuple, Type, TypeVar, Union, cast, overload
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Iterable,
+    Iterator,
+    Literal,
+    Mapping,
+    MutableMapping,
+    TypeVar,
+    cast,
+    overload,
+)
 from warnings import warn
 
-import attr
-import dateutil.parser
 import geopandas as gpd
 import numpy as np
 from fs.base import FS
-from typing_extensions import Literal
 
-from sentinelhub import CRS, BBox
+from sentinelhub import CRS, BBox, parse_time
 from sentinelhub.exceptions import deprecated_function
 
 from .constants import TIMESTAMP_COLUMN, FeatureType, OverwritePermission
-from .eodata_io import FeatureIO, load_eopatch_content, save_eopatch
-from .eodata_merge import merge_eopatches
+from .eodata_io import FeatureIO, FeatureIOJson, load_eopatch_content, save_eopatch
 from .exceptions import EODeprecationWarning
 from .types import EllipsisType, FeatureSpec, FeaturesSpecification
 from .utils.common import deep_eq, is_discrete_type
 from .utils.fs import get_filesystem
 from .utils.parsing import parse_features
 
 T = TypeVar("T")
-Self = TypeVar("Self")
 
 LOGGER = logging.getLogger(__name__)
 MISSING_BBOX_WARNING = (
     "Initializing an EOPatch without providing a BBox will no longer be possible in the future."
     " EOPatches represent geolocated data and so any EOPatch without a BBox is ill-formed. Consider"
     " using a different data structure for non-geolocated data."
 )
+TIMESTAMP_RENAME_WARNING = "The attribute `timestamp` is deprecated, use `timestamps` instead."
 
 MAX_DATA_REPR_LEN = 100
 
 if TYPE_CHECKING:
-    try:
-        from eolearn.visualization import PlotBackend
-        from eolearn.visualization.eopatch_base import BasePlotConfig
-    except ImportError:
-        pass
+    with contextlib.suppress(ImportError):
+        from eolearn.visualization import PlotBackend, PlotConfig
 
 
-class _FeatureDict(Dict[str, Union[T, FeatureIO[T]]], metaclass=ABCMeta):
+class _FeatureDict(MutableMapping[str, T], metaclass=ABCMeta):
     """A dictionary structure that holds features of certain feature type.
 
     It checks that features have a correct and dimension. It also supports lazy loading by accepting a function as a
     feature value, which is then called when the feature is accessed.
     """
 
     FORBIDDEN_CHARS = {".", "/", "\\", "|", ";", ":", "\n", "\t"}
 
-    def __init__(self, feature_dict: Dict[str, Union[T, FeatureIO[T]]], feature_type: FeatureType):
+    def __init__(self, feature_dict: Mapping[str, T | FeatureIO[T]], feature_type: FeatureType):
         """
         :param feature_dict: A dictionary of feature names and values
         :param feature_type: Type of features
         """
         super().__init__()
 
         self.feature_type = feature_type
+        self._content = dict(feature_dict.items())
 
-        for feature_name, value in feature_dict.items():
-            self[feature_name] = value
-
-    @classmethod
-    def empty_factory(cls: Type[Self], feature_type: FeatureType) -> Callable[[], Self]:
-        """Returns a factory function for creating empty feature dictionaries with an appropriate feature type."""
-
-        def factory() -> Self:
-            return cls(feature_dict={}, feature_type=feature_type)  # type: ignore[call-arg]
-
-        return factory
-
-    def __setitem__(self, feature_name: str, value: Union[T, FeatureIO[T]]) -> None:
+    def __setitem__(self, feature_name: str, value: T | FeatureIO[T]) -> None:
         """Before setting value to the dictionary it checks that value is of correct type and dimension and tries to
         transform value in correct form.
         """
         if not isinstance(value, FeatureIO):
             value = self._parse_feature_value(value, feature_name)
         self._check_feature_name(feature_name)
-        super().__setitem__(feature_name, value)
+        self._content[feature_name] = value
 
     def _check_feature_name(self, feature_name: str) -> None:
         """Ensures that feature names are strings and do not contain forbidden characters."""
         if not isinstance(feature_name, str):
             raise ValueError(f"Feature name must be a string but an object of type {type(feature_name)} was given.")
 
         for char in feature_name:
             if char in self.FORBIDDEN_CHARS:
-                raise ValueError(
-                    f"The name of feature ({self.feature_type}, {feature_name}) contains an illegal character '{char}'."
-                )
+                raise ValueError(f"The feature name of {feature_name} contains an illegal character '{char}'.")
 
         if feature_name == "":
             raise ValueError("Feature name cannot be an empty string.")
 
-    @overload
-    def __getitem__(self, feature_name: str, load: Literal[True] = ...) -> T:
-        ...
-
-    @overload
-    def __getitem__(self, feature_name: str, load: Literal[False] = ...) -> Union[T, FeatureIO[T]]:
-        ...
-
-    def __getitem__(self, feature_name: str, load: bool = True) -> Union[T, FeatureIO[T]]:
+    def __getitem__(self, feature_name: str) -> T:
         """Implements lazy loading."""
-        value = super().__getitem__(feature_name)
+        value = self._content[feature_name]
 
-        if isinstance(value, FeatureIO) and load:
+        if isinstance(value, FeatureIO):
+            value = cast(FeatureIO[T], value)  # not sure why mypy borks this one
             value = value.load()
-            self[feature_name] = value
+            self._content[feature_name] = value
 
         return value
 
+    def _get_unloaded(self, feature_name: str) -> T | FeatureIO[T]:
+        """Returns the value, bypassing lazy-loading mechanisms."""
+        return self._content[feature_name]
+
+    def __delitem__(self, feature_name: str) -> None:
+        del self._content[feature_name]
+
     def __eq__(self, other: object) -> bool:
-        """Compares its content against a content of another feature type dictionary."""
+        # default doesn't know how to compare numpy arrays
         return deep_eq(self, other)
 
-    def __ne__(self, other: object) -> bool:
-        """Compares its content against a content of another feature type dictionary."""
-        return not self.__eq__(other)
-
-    def get_dict(self) -> Dict[str, T]:
-        """Returns a Python dictionary of features and value."""
-        return dict(self)
+    def __len__(self) -> int:
+        return len(self._content)
+
+    def __contains__(self, key: object) -> bool:
+        return key in self._content
+
+    def __iter__(self) -> Iterator[str]:
+        return iter(self._content)
 
     @abstractmethod
     def _parse_feature_value(self, value: object, feature_name: str) -> T:
         """Checks if value fits the feature type. If not it tries to fix it or raise an error.
 
         :raises: ValueError
         """
 
 
 class _FeatureDictNumpy(_FeatureDict[np.ndarray]):
     """_FeatureDict object specialized for Numpy arrays."""
 
-    def __init__(self, feature_dict: Dict[str, Union[np.ndarray, FeatureIO[np.ndarray]]], feature_type: FeatureType):
-        ndim = feature_type.ndim()
-        if ndim is None:
-            raise ValueError(f"Feature type {feature_type} does not represent a Numpy based feature.")
-        self.ndim = ndim
-        super().__init__(feature_dict, feature_type)
-
     def _parse_feature_value(self, value: object, feature_name: str) -> np.ndarray:
         if not isinstance(value, np.ndarray):
             raise ValueError(f"{self.feature_type} feature has to be a numpy array.")
-        if not hasattr(self, "ndim"):  # Because of serialization/deserialization during multiprocessing
-            return value
-        if value.ndim != self.ndim:
+
+        expected_ndim = cast(int, self.feature_type.ndim())  # numpy features have ndim
+        if value.ndim != expected_ndim:
             raise ValueError(
-                f"Numpy array of {self.feature_type} feature has to have {self.ndim} "
-                f"dimension{'s' if self.ndim > 1 else ''} but feature {feature_name} has {value.ndim}."
+                f"Numpy array of {self.feature_type} feature has to have {expected_ndim} "
+                f"dimension{'s' if expected_ndim > 1 else ''} but feature {feature_name} has {value.ndim}."
             )
 
         if self.feature_type.is_discrete() and not is_discrete_type(value.dtype):
             raise ValueError(
                 f"{self.feature_type} is a discrete feature type therefore dtype of data array "
                 f"has to be either integer or boolean type but feature {feature_name} has dtype {value.dtype.type}."
             )
 
         return value
 
 
 class _FeatureDictGeoDf(_FeatureDict[gpd.GeoDataFrame]):
     """_FeatureDict object specialized for GeoDataFrames."""
 
-    def __init__(self, feature_dict: Dict[str, gpd.GeoDataFrame], feature_type: FeatureType):
-        if not feature_type.is_vector():
-            raise ValueError(f"Feature type {feature_type} does not represent a vector feature.")
-        super().__init__(feature_dict, feature_type)
-
     def _parse_feature_value(self, value: object, feature_name: str) -> gpd.GeoDataFrame:
         if isinstance(value, gpd.GeoSeries):
             value = gpd.GeoDataFrame(geometry=value, crs=value.crs)
 
         if isinstance(value, gpd.GeoDataFrame):
             if self.feature_type is FeatureType.VECTOR and TIMESTAMP_COLUMN not in value:
                 raise ValueError(
@@ -206,24 +188,23 @@
 class _FeatureDictJson(_FeatureDict[Any]):
     """_FeatureDict object specialized for meta-info."""
 
     def _parse_feature_value(self, value: object, _: str) -> Any:
         return value
 
 
-def _create_feature_dict(feature_type: FeatureType, value: Dict[str, Any]) -> _FeatureDict:
+def _create_feature_dict(feature_type: FeatureType, value: Mapping[str, Any]) -> _FeatureDict:
     """Creates the correct FeatureDict, corresponding to the FeatureType."""
     if feature_type.is_vector():
         return _FeatureDictGeoDf(value, feature_type)
     if feature_type is FeatureType.META_INFO:
         return _FeatureDictJson(value, feature_type)
     return _FeatureDictNumpy(value, feature_type)
 
 
-@attr.s(repr=False, eq=False, kw_only=True)
 class EOPatch:
     """The basic data object for multi-temporal remotely sensed data, such as satellite imagery and its derivatives.
 
     The EOPatch contains multi-temporal remotely sensed data of a single patch of earth's surface defined by the
     bounding box in specific coordinate reference system. The patch can be a rectangle, polygon, or pixel in space.
     The EOPatch object can also be used to store derived quantities, such as for example means, standard deviations,
     etc., of a patch. In this case the 'space' dimension is equivalent to a pixel.
@@ -236,157 +217,156 @@
     In addition to that other auxiliary information is also needed and can be stored in additional attributes of the
     EOPatch (thus extending the functionality of numpy ndarray). These attributes are listed in the FeatureType enum.
 
     Currently, the EOPatch object doesn't enforce that the length of timestamps be equal to n_times dimensions of numpy
     arrays in other attributes.
     """
 
-    data: _FeatureDictNumpy = attr.ib(factory=_FeatureDictNumpy.empty_factory(FeatureType.DATA))
-    mask: _FeatureDictNumpy = attr.ib(factory=_FeatureDictNumpy.empty_factory(FeatureType.MASK))
-    scalar: _FeatureDictNumpy = attr.ib(factory=_FeatureDictNumpy.empty_factory(FeatureType.SCALAR))
-    label: _FeatureDictNumpy = attr.ib(factory=_FeatureDictNumpy.empty_factory(FeatureType.LABEL))
-    vector: _FeatureDictGeoDf = attr.ib(factory=_FeatureDictGeoDf.empty_factory(FeatureType.VECTOR))
-    data_timeless: _FeatureDictNumpy = attr.ib(factory=_FeatureDictNumpy.empty_factory(FeatureType.DATA_TIMELESS))
-    mask_timeless: _FeatureDictNumpy = attr.ib(factory=_FeatureDictNumpy.empty_factory(FeatureType.MASK_TIMELESS))
-    scalar_timeless: _FeatureDictNumpy = attr.ib(factory=_FeatureDictNumpy.empty_factory(FeatureType.SCALAR_TIMELESS))
-    label_timeless: _FeatureDictNumpy = attr.ib(factory=_FeatureDictNumpy.empty_factory(FeatureType.LABEL_TIMELESS))
-    vector_timeless: _FeatureDictGeoDf = attr.ib(factory=_FeatureDictGeoDf.empty_factory(FeatureType.VECTOR_TIMELESS))
-    meta_info: _FeatureDictJson = attr.ib(factory=_FeatureDictJson.empty_factory(FeatureType.META_INFO))
-    bbox: Optional[BBox] = attr.ib(default=None)
-    timestamps: List[dt.datetime] = attr.ib(factory=list)
+    # establish types of property value holders
+    _timestamps: list[dt.datetime]
+    _bbox: BBox | None
+    _meta_info: FeatureIOJson | _FeatureDictJson
 
-    def __attrs_post_init__(self) -> None:
-        if self.bbox is None:
-            warn(MISSING_BBOX_WARNING, category=EODeprecationWarning, stacklevel=2)
+    def __init__(
+        self,
+        *,
+        data: Mapping[str, np.ndarray] | None = None,
+        mask: Mapping[str, np.ndarray] | None = None,
+        scalar: Mapping[str, np.ndarray] | None = None,
+        label: Mapping[str, np.ndarray] | None = None,
+        vector: Mapping[str, gpd.GeoDataFrame] | None = None,
+        data_timeless: Mapping[str, np.ndarray] | None = None,
+        mask_timeless: Mapping[str, np.ndarray] | None = None,
+        scalar_timeless: Mapping[str, np.ndarray] | None = None,
+        label_timeless: Mapping[str, np.ndarray] | None = None,
+        vector_timeless: Mapping[str, gpd.GeoDataFrame] | None = None,
+        meta_info: Mapping[str, Any] | None = None,
+        bbox: BBox | None = None,
+        timestamps: list[dt.datetime] | None = None,
+    ):
+        self.data: MutableMapping[str, np.ndarray] = _FeatureDictNumpy(data or {}, FeatureType.DATA)
+        self.mask: MutableMapping[str, np.ndarray] = _FeatureDictNumpy(mask or {}, FeatureType.MASK)
+        self.scalar: MutableMapping[str, np.ndarray] = _FeatureDictNumpy(scalar or {}, FeatureType.SCALAR)
+        self.label: MutableMapping[str, np.ndarray] = _FeatureDictNumpy(label or {}, FeatureType.LABEL)
+        self.vector: MutableMapping[str, gpd.GeoDataFrame] = _FeatureDictGeoDf(vector or {}, FeatureType.VECTOR)
+        self.data_timeless: MutableMapping[str, np.ndarray] = _FeatureDictNumpy(
+            data_timeless or {}, FeatureType.DATA_TIMELESS
+        )
+        self.mask_timeless: MutableMapping[str, np.ndarray] = _FeatureDictNumpy(
+            mask_timeless or {}, FeatureType.MASK_TIMELESS
+        )
+        self.scalar_timeless: MutableMapping[str, np.ndarray] = _FeatureDictNumpy(
+            scalar_timeless or {}, FeatureType.SCALAR_TIMELESS
+        )
+        self.label_timeless: MutableMapping[str, np.ndarray] = _FeatureDictNumpy(
+            label_timeless or {}, FeatureType.LABEL_TIMELESS
+        )
+        self.vector_timeless: MutableMapping[str, gpd.GeoDataFrame] = _FeatureDictGeoDf(
+            vector_timeless or {}, FeatureType.VECTOR_TIMELESS
+        )
+        self.meta_info: MutableMapping[str, Any] = _FeatureDictJson(meta_info or {}, FeatureType.META_INFO)
+        self.bbox = bbox
+        self.timestamps = timestamps or []
 
     @property
-    def timestamp(self) -> List[dt.datetime]:
-        """A property for handling the deprecated timestamp attribute.
-
-        :return: A list of EOPatch timestamps
-        """
-        warn(
-            "The attribute `timestamp` is deprecated, use `timestamps` instead.",
-            category=EODeprecationWarning,
-            stacklevel=2,
-        )
+    def timestamp(self) -> list[dt.datetime]:
+        """A property for handling the deprecated timestamp attribute."""
+        warn(TIMESTAMP_RENAME_WARNING, category=EODeprecationWarning, stacklevel=2)
         return self.timestamps
 
     @timestamp.setter
-    def timestamp(self, value: List[dt.datetime]) -> None:
-        warn(
-            "The attribute `timestamp` is deprecated, use `timestamps` instead.",
-            category=EODeprecationWarning,
-            stacklevel=2,
-        )
+    def timestamp(self, value: list[dt.datetime]) -> None:
+        warn(TIMESTAMP_RENAME_WARNING, category=EODeprecationWarning, stacklevel=2)
         self.timestamps = value
 
-    def __setattr__(self, key: str, value: object, feature_name: Union[str, None, EllipsisType] = None) -> None:
-        """Raises TypeError if feature type attributes are not of correct type.
-
-        In case they are a dictionary they are cast to _FeatureDict class.
-        """
-        if feature_name not in (None, Ellipsis) and FeatureType.has_value(key):
-            self.__getattribute__(key)[feature_name] = value
-            return
-
-        if FeatureType.has_value(key) and not isinstance(value, FeatureIO):
-            feature_type = FeatureType(key)
-            value = self._parse_feature_type_value(feature_type, value)
-
-        super().__setattr__(key, value)
-
-    @staticmethod
-    def _parse_feature_type_value(
-        feature_type: FeatureType, value: object
-    ) -> Union[_FeatureDict, BBox, List[dt.date], None]:
-        """Checks or parses value which will be assigned to a feature type attribute of `EOPatch`. If the value
-        cannot be parsed correctly it raises an error.
-
-        :raises: TypeError, ValueError
-        """
-
-        if feature_type is FeatureType.BBOX and (value is None or isinstance(value, BBox)):
-            if value is None:
-                warn(MISSING_BBOX_WARNING, category=EODeprecationWarning, stacklevel=2)
-            return value
-
-        if feature_type is FeatureType.TIMESTAMPS and isinstance(value, (tuple, list)):
-            return [
-                timestamp if isinstance(timestamp, dt.date) else dateutil.parser.parse(timestamp) for timestamp in value
-            ]
-
-        if isinstance(value, dict):
-            return value if isinstance(value, _FeatureDict) else _create_feature_dict(feature_type, value)
-
-        raise TypeError(f"Cannot parse given value {value} for feature type {feature_type}. Possible type missmatch.")
-
-    def __getattribute__(self, key: str, load: bool = True, feature_name: Union[str, None, EllipsisType] = None) -> Any:
-        """Handles lazy loading and can even provide a single feature from _FeatureDict."""
-        value = super().__getattribute__(key)
+    @property
+    def timestamps(self) -> list[dt.datetime]:
+        """A property for handling the `timestamps` attribute."""
+        return self._timestamps
+
+    @timestamps.setter
+    def timestamps(self, value: Iterable[dt.datetime]) -> None:
+        if isinstance(value, Iterable) and all(isinstance(time, (dt.date, str)) for time in value):
+            self._timestamps = [parse_time(time, force_datetime=True) for time in value]
+        else:
+            raise TypeError(f"Cannot assign {value} as timestamps. Should be a sequence of datetime.datetime objects.")
 
-        if isinstance(value, FeatureIO) and load:
-            value = value.load()
-            setattr(self, key, value)
-            value = getattr(self, key)
+    @property
+    def bbox(self) -> BBox | None:
+        """A property for handling the `bbox` attribute."""
+        return self._bbox
+
+    @bbox.setter
+    def bbox(self, value: BBox | None) -> None:
+        if not (isinstance(value, BBox) or value is None):
+            raise TypeError(f"Cannot assign {value} as bbox. Should be a `BBox` object.")
+        if value is None:
+            warn(MISSING_BBOX_WARNING, category=EODeprecationWarning, stacklevel=2)
+        self._bbox = value
 
-        if feature_name not in (None, Ellipsis) and isinstance(value, _FeatureDict):
-            feature_name = cast(str, feature_name)  # the above check deals with ... and None
-            return value[feature_name]
+    @property
+    def meta_info(self) -> MutableMapping[str, Any]:
+        """A property for handling the `meta_info` attribute."""
+        # once META_INFO becomes regular (in terms of IO) this can be removed
+        if isinstance(self._meta_info, FeatureIOJson):
+            self.meta_info = self._meta_info.load()  # assigned to `meta_info` property to trigger validation
+        return self._meta_info  # type: ignore[return-value] # mypy cannot verify due to mutations
+
+    @meta_info.setter
+    def meta_info(self, value: Mapping[str, Any] | FeatureIOJson) -> None:
+        self._meta_info = value if isinstance(value, FeatureIOJson) else _FeatureDictJson(value, FeatureType.META_INFO)
+
+    def __setattr__(self, key: str, value: object) -> None:
+        """Casts dictionaries to _FeatureDict objects for non-meta features."""
+
+        if FeatureType.has_value(key) and not FeatureType(key).is_meta():
+            if not isinstance(value, (dict, _FeatureDict)):
+                raise TypeError(f"Cannot parse {value} for attribute {key}. Should be a dictionary.")
+            value = _create_feature_dict(FeatureType(key), value)
 
-        return value
+        super().__setattr__(key, value)
 
     @overload
-    def __getitem__(self, key: Union[Literal[FeatureType.BBOX], Tuple[Literal[FeatureType.BBOX], Any]]) -> BBox:
+    def __getitem__(self, key: Literal[FeatureType.BBOX] | tuple[Literal[FeatureType.BBOX], Any]) -> BBox:
         ...
 
     @overload
     def __getitem__(
-        self, key: Union[Literal[FeatureType.TIMESTAMPS], Tuple[Literal[FeatureType.TIMESTAMPS], Any]]
-    ) -> List[dt.datetime]:
+        self, key: Literal[FeatureType.TIMESTAMPS] | tuple[Literal[FeatureType.TIMESTAMPS], Any]
+    ) -> list[dt.datetime]:
         ...
 
     @overload
-    def __getitem__(self, key: Union[FeatureType, Tuple[FeatureType, Union[str, None, EllipsisType]]]) -> Any:
+    def __getitem__(self, key: FeatureType | tuple[FeatureType, str | None | EllipsisType]) -> Any:
         ...
 
-    def __getitem__(self, key: Union[FeatureType, Tuple[FeatureType, Union[str, None, EllipsisType]]]) -> Any:
+    def __getitem__(self, key: FeatureType | tuple[FeatureType, str | None | EllipsisType]) -> Any:
         """Provides features of requested feature type. It can also accept a tuple of (feature_type, feature_name).
 
         :param key: Feature type or a (feature_type, feature_name) pair.
         """
-        if isinstance(key, tuple):
-            feature_type, feature_name = key
-        else:
-            feature_type, feature_name = key, None
-
-        ftype = FeatureType(feature_type).value
-        return self.__getattribute__(ftype, feature_name=feature_name)  # type: ignore[call-arg]
+        feature_type, feature_name = key if isinstance(key, tuple) else (key, None)
+        value = getattr(self, FeatureType(feature_type).value)
+        if feature_name not in (None, Ellipsis) and isinstance(value, _FeatureDict):
+            feature_name = cast(str, feature_name)  # the above check deals with ... and None
+            return value[feature_name]
+        return value
 
-    def __setitem__(
-        self, key: Union[FeatureType, Tuple[FeatureType, Union[str, None, EllipsisType]]], value: Any
-    ) -> None:
-        """Sets a new dictionary / list to the given FeatureType. As a key it can also accept a tuple of
-        (feature_type, feature_name).
+    def __setitem__(self, key: FeatureType | tuple[FeatureType, str | None | EllipsisType], value: Any) -> None:
+        """Sets a new value to the given FeatureType or tuple of (feature_type, feature_name)."""
+        feature_type, feature_name = key if isinstance(key, tuple) else (key, None)
+        ftype_attr = FeatureType(feature_type).value
 
-        :param key: Type of EOPatch feature
-        :param value: New dictionary or list
-        """
-        if isinstance(key, tuple):
-            feature_type, feature_name = key
+        if feature_name not in (None, Ellipsis):
+            getattr(self, ftype_attr)[feature_name] = value
         else:
-            feature_type, feature_name = key, None
-
-        return self.__setattr__(FeatureType(feature_type).value, value, feature_name=feature_name)
-
-    def __delitem__(self, feature: Union[FeatureType, FeatureSpec]) -> None:
-        """Deletes the selected feature type or feature.
+            setattr(self, ftype_attr, value)
 
-        :param feature: EOPatch feature
-        """
+    def __delitem__(self, feature: FeatureType | FeatureSpec) -> None:
+        """Deletes the selected feature type or feature."""
         if isinstance(feature, tuple):
             feature_type, feature_name = feature
             if feature_type in [FeatureType.BBOX, FeatureType.TIMESTAMPS]:
                 feature = feature_type
             else:
                 del self[feature_type][feature_name]
                 return
@@ -417,26 +397,28 @@
                 return bool(self[ftype])
             return fname in self[ftype]
         raise ValueError(
             f"Membership checking is only implemented for elements of type `{FeatureType.__name__}` and for "
             "`(feature_type, feature_name)` pairs."
         )
 
+    @deprecated_function(EODeprecationWarning, "Use the `merge` method instead.")
     def __add__(self, other: EOPatch) -> EOPatch:
         """Merges two EOPatches into a new EOPatch."""
         return self.merge(other)
 
     def __repr__(self) -> str:
         feature_repr_list = []
         for feature_type in FeatureType:
             content = self[feature_type]
             if not content:
                 continue
 
-            if isinstance(content, dict):
+            if isinstance(content, _FeatureDict):
+                content = {k: content._get_unloaded(k) for k in content}  # noqa: SLF001
                 inner_content_repr = "\n    ".join(
                     [f"{label}: {self._repr_value(value)}" for label, value in sorted(content.items())]
                 )
                 content_str = "{\n    " + inner_content_repr + "\n  }"
             else:
                 content_str = self._repr_value(content)
             feature_repr_list.append(f"{feature_type.value}={content_str}")
@@ -463,18 +445,18 @@
         if isinstance(value, (list, tuple, dict)) and value:
             repr_str = str(value)
             if len(repr_str) <= MAX_DATA_REPR_LEN:
                 return repr_str
 
             l_bracket, r_bracket = ("[", "]") if isinstance(value, list) else ("(", ")")
             if isinstance(value, (list, tuple)) and len(value) > 2:
-                repr_str = f"{l_bracket}{repr(value[0])}, ..., {repr(value[-1])}{r_bracket}"
+                repr_str = f"{l_bracket}{value[0]!r}, ..., {value[-1]!r}{r_bracket}"
 
             if len(repr_str) > MAX_DATA_REPR_LEN and isinstance(value, (list, tuple)) and len(value) > 1:
-                repr_str = f"{l_bracket}{repr(value[0])}, ...{r_bracket}"
+                repr_str = f"{l_bracket}{value[0]!r}, ...{r_bracket}"
 
             if len(repr_str) > MAX_DATA_REPR_LEN:
                 repr_str = str(type(value))
 
             return f"{repr_str}, length={len(value)}"
 
         return repr(value)
@@ -494,32 +476,32 @@
             features = ...
 
         new_eopatch = EOPatch(bbox=copy.copy(self.bbox))
         for feature_type, feature_name in parse_features(features, eopatch=self):
             if feature_type in (FeatureType.BBOX, FeatureType.TIMESTAMPS):
                 new_eopatch[feature_type] = copy.copy(self[feature_type])
             else:
-                new_eopatch[feature_type][feature_name] = self[feature_type].__getitem__(feature_name, load=False)
+                new_eopatch[feature_type][feature_name] = self[feature_type]._get_unloaded(feature_name)  # noqa: SLF001
         return new_eopatch
 
-    def __deepcopy__(self, memo: Optional[dict] = None, features: FeaturesSpecification = ...) -> EOPatch:
+    def __deepcopy__(self, memo: dict | None = None, features: FeaturesSpecification = ...) -> EOPatch:
         """Returns a new EOPatch with deep copies of given features.
 
         :param memo: built-in parameter for memoization
         :param features: A collection of features or feature types that will be copied into new EOPatch.
         """
         if not features:  # For some reason deepcopy and copy pass {} by default
             features = ...
 
         new_eopatch = EOPatch(bbox=copy.deepcopy(self.bbox))
         for feature_type, feature_name in parse_features(features, eopatch=self):
             if feature_type in (FeatureType.BBOX, FeatureType.TIMESTAMPS):
                 new_eopatch[feature_type] = copy.deepcopy(self[feature_type], memo=memo)
             else:
-                value = self[feature_type].__getitem__(feature_name, load=False)
+                value = self[feature_type]._get_unloaded(feature_name)  # noqa: SLF001
 
                 if isinstance(value, FeatureIO):
                     # We cannot deepcopy the entire object because of the filesystem attribute
                     value = copy.copy(value)
                     value.loaded_value = copy.deepcopy(value.loaded_value, memo=memo)
                 else:
                     value = copy.deepcopy(value, memo=memo)
@@ -551,33 +533,33 @@
         if feature_type is FeatureType.BBOX:
             raise ValueError("The BBox of an EOPatch should never be undefined.")
         if feature_type is FeatureType.TIMESTAMPS:
             self[feature_type] = []
         else:
             self[feature_type] = {}
 
-    def get_spatial_dimension(self, feature_type: FeatureType, feature_name: str) -> Tuple[int, int]:
+    def get_spatial_dimension(self, feature_type: FeatureType, feature_name: str) -> tuple[int, int]:
         """
         Returns a tuple of spatial dimensions (height, width) of a feature.
 
         :param feature_type: Type of the feature
         :param feature_name: Name of the feature
         """
         if feature_type.is_array() and feature_type.is_spatial():
             shape = self[feature_type][feature_name].shape
             return shape[1:3] if feature_type.is_temporal() else shape[0:2]
 
         raise ValueError(f"Features of type {feature_type} do not have a spatial dimension or are not arrays.")
 
-    def get_features(self) -> List[FeatureSpec]:
+    def get_features(self) -> list[FeatureSpec]:
         """Returns a list of all non-empty features of EOPatch.
 
         :return: List of non-empty features
         """
-        feature_list: List[FeatureSpec] = []
+        feature_list: list[FeatureSpec] = []
         for feature_type in FeatureType:
             if feature_type is FeatureType.BBOX or feature_type is FeatureType.TIMESTAMPS:
                 if feature_type in self:
                     feature_list.append((feature_type, None))
             else:
                 for feature_name in self[feature_type]:
                     feature_list.append((feature_type, feature_name))
@@ -585,15 +567,15 @@
 
     def save(
         self,
         path: str,
         features: FeaturesSpecification = ...,
         overwrite_permission: OverwritePermission = OverwritePermission.ADD_ONLY,
         compress_level: int = 0,
-        filesystem: Optional[FS] = None,
+        filesystem: FS | None = None,
     ) -> None:
         """Method to save an EOPatch from memory to a storage.
 
         :param path: A location where to save EOPatch. It can be either a local path or a remote URL path.
         :param features: A collection of features types specifying features of which type will be saved. By default,
             all features will be saved.
         :param overwrite_permission: A level of permission for overwriting an existing EOPatch
@@ -613,49 +595,50 @@
             features=features,
             compress_level=compress_level,
             overwrite_permission=OverwritePermission(overwrite_permission),
         )
 
     @staticmethod
     def load(
-        path: str, features: FeaturesSpecification = ..., lazy_loading: bool = False, filesystem: Optional[FS] = None
+        path: str, features: FeaturesSpecification = ..., lazy_loading: bool = False, filesystem: FS | None = None
     ) -> EOPatch:
         """Method to load an EOPatch from a storage into memory.
 
         :param path: A location from where to load EOPatch. It can be either a local path or a remote URL path.
         :param features: A collection of features to be loaded. By default, all features will be loaded.
         :param lazy_loading: If `True` features will be lazy loaded.
         :param filesystem: An existing filesystem object. If not given it will be initialized according to the `path`
             parameter.
         :return: Loaded EOPatch
         """
         if filesystem is None:
             filesystem = get_filesystem(path, create=False)
             path = "/"
 
-        bbox, timestamps, meta_info, features_dict = load_eopatch_content(filesystem, path, features=features)
-        eopatch = EOPatch(bbox=bbox)  # type: ignore[arg-type]
+        bbox_io, timestamps_io, meta_info, features_dict = load_eopatch_content(filesystem, path, features=features)
+        eopatch = EOPatch(bbox=None if bbox_io is None else bbox_io.load())
 
-        if timestamps is not None:
-            eopatch.timestamps = timestamps  # type: ignore[assignment]
+        if timestamps_io is not None:
+            eopatch.timestamps = timestamps_io.load()
         if meta_info is not None:
             eopatch.meta_info = meta_info  # type: ignore[assignment]
         for feature, feature_io in features_dict.items():
             eopatch[feature] = feature_io
 
         if not lazy_loading:
             _trigger_loading_for_eopatch_features(eopatch)
         return eopatch
 
+    @deprecated_function(EODeprecationWarning, "Use the function `eolearn.core.merge_eopatches` instead.")
     def merge(
         self,
         *eopatches: EOPatch,
         features: FeaturesSpecification = ...,
-        time_dependent_op: Union[Literal[None, "concatenate", "min", "max", "mean", "median"], Callable] = None,
-        timeless_op: Union[Literal[None, "concatenate", "min", "max", "mean", "median"], Callable] = None,
+        time_dependent_op: Literal[None, "concatenate", "min", "max", "mean", "median"] | Callable = None,
+        timeless_op: Literal[None, "concatenate", "min", "max", "mean", "median"] | Callable = None,
     ) -> EOPatch:
         """Merge features of given EOPatches into a new EOPatch.
 
         :param eopatches: Any number of EOPatches to be merged together with the current EOPatch
         :param features: A collection of features to be merged together. By default, all features will be merged.
         :param time_dependent_op: An operation to be used to join data for any time-dependent raster feature. Before
             joining time slices of all arrays will be sorted. Supported options are:
@@ -674,25 +657,21 @@
             - 'concatenate': Join arrays over the last (i.e. bands) dimension
             - 'min': Join arrays by taking minimum values. Ignore NaN values.
             - 'max': Join arrays by taking maximum values. Ignore NaN values.
             - 'mean': Join arrays by taking mean values. Ignore NaN values.
             - 'median': Join arrays by taking median values. Ignore NaN values.
         :return: A merged EOPatch
         """
-        eopatch_content = merge_eopatches(
+        from .eodata_merge import merge_eopatches  # pylint: disable=import-outside-toplevel, cyclic-import
+
+        return merge_eopatches(
             self, *eopatches, features=features, time_dependent_op=time_dependent_op, timeless_op=timeless_op
         )
 
-        merged_eopatch = EOPatch(bbox=eopatch_content[(FeatureType.BBOX, None)])
-        for feature, value in eopatch_content.items():
-            merged_eopatch[feature] = value
-
-        return merged_eopatch
-
-    def consolidate_timestamps(self, timestamps: List[dt.datetime]) -> Set[dt.datetime]:
+    def consolidate_timestamps(self, timestamps: list[dt.datetime]) -> set[dt.datetime]:
         """Removes all frames from the EOPatch with a date not found in the provided timestamps list.
 
         :param timestamps: keep frames with date found in this list
         :return: set of removed frames' dates
         """
         remove_from_patch = set(self.timestamps).difference(timestamps)
         remove_from_patch_idxs = [self.timestamps.index(rm_date) for rm_date in remove_from_patch]
@@ -707,20 +686,20 @@
         self.timestamps = good_timestamps
         return remove_from_patch
 
     def plot(
         self,
         feature: FeatureSpec,
         *,
-        times: Union[List[int], slice, None] = None,
-        channels: Union[List[int], slice, None] = None,
-        channel_names: Optional[List[str]] = None,
-        rgb: Optional[Tuple[int, int, int]] = None,
-        backend: Union[str, PlotBackend] = "matplotlib",
-        config: Optional[BasePlotConfig] = None,
+        times: list[int] | slice | None = None,
+        channels: list[int] | slice | None = None,
+        channel_names: list[str] | None = None,
+        rgb: tuple[int, int, int] | None = None,
+        backend: str | PlotBackend = "matplotlib",
+        config: PlotConfig | None = None,
         **kwargs: Any,
     ) -> object:
         """Plots an `EOPatch` feature.
 
         :param feature: A feature in the `EOPatch`.
         :param times: A list or a slice of indices on temporal axis to be used for plotting. If not provided all
             indices will be used.
```

### Comparing `eo-learn-core-1.4.1/eolearn/core/eodata_io.py` & `eo-learn-core-1.4.2/eolearn/core/eodata_io.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,27 @@
 import json
 import platform
 import warnings
 from abc import ABCMeta, abstractmethod
 from collections import defaultdict
 from dataclasses import dataclass, field
 from functools import partial
-from typing import TYPE_CHECKING, Any, BinaryIO, Dict, Generic, Iterator, List, Optional, Tuple, Type, TypeVar, Union
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    BinaryIO,
+    Dict,
+    Generic,
+    Iterator,
+    List,
+    Mapping,
+    Optional,
+    Tuple,
+    TypeVar,
+)
 
 import dateutil.parser
 import fs
 import fs.move
 import geopandas as gpd
 import numpy as np
 import pandas as pd
@@ -35,15 +47,14 @@
 from sentinelhub import CRS, BBox, Geometry, MimeType
 from sentinelhub.exceptions import SHUserWarning, deprecated_function
 
 from .constants import TIMESTAMP_COLUMN, FeatureType, OverwritePermission
 from .exceptions import EODeprecationWarning
 from .types import EllipsisType, FeatureSpec, FeaturesSpecification
 from .utils.parsing import FeatureParser
-from .utils.vector_io import infer_schema
 
 if TYPE_CHECKING:
     from .eodata import EOPatch
 
 T = TypeVar("T")
 Self = TypeVar("Self", bound="FeatureIO")
 PatchContentType: TypeAlias = Tuple[
@@ -58,20 +69,20 @@
 TIMESTAMPS_FILENAME = "timestamps"
 
 
 @dataclass
 class FilesystemDataInfo:
     """Information about data that is present on the filesystem. Fields represent paths to relevant file."""
 
-    timestamps: Optional[str] = None
-    bbox: Optional[str] = None
-    meta_info: Optional[str] = None
-    features: Dict[FeatureType, Dict[str, str]] = field(default_factory=lambda: defaultdict(dict))
+    timestamps: str | None = None
+    bbox: str | None = None
+    meta_info: str | None = None
+    features: dict[FeatureType, dict[str, str]] = field(default_factory=lambda: defaultdict(dict))
 
-    def iterate_features(self) -> Iterator[Tuple[Tuple[FeatureType, str], str]]:
+    def iterate_features(self) -> Iterator[tuple[tuple[FeatureType, str], str]]:
         """Yields `(ftype, fname), path` tuples from `features`."""
         for ftype, ftype_dict in self.features.items():
             for fname, path in ftype_dict.items():
                 yield (ftype, fname), path
 
 
 def save_eopatch(
@@ -89,37 +100,41 @@
     file_information = get_filesystem_data_info(filesystem, patch_location) if patch_exists else FilesystemDataInfo()
 
     _check_collisions(overwrite_permission, eopatch_features, file_information)
 
     # Data must be collected before any tinkering with files due to lazy-loading
     data_for_saving = list(_yield_features_to_save(eopatch, eopatch_features, patch_location))
 
-    if overwrite_permission is OverwritePermission.OVERWRITE_PATCH and patch_exists:
-        _remove_old_eopatch(filesystem, patch_location)
+    with warnings.catch_warnings():
+        warnings.simplefilter("ignore", category=EODeprecationWarning)
+        if overwrite_permission is OverwritePermission.OVERWRITE_PATCH and patch_exists:
+            _remove_old_eopatch(filesystem, patch_location)
 
     ftype_folders = {fs.path.dirname(path) for _, _, path in data_for_saving}
     for folder in ftype_folders:
         filesystem.makedirs(folder, recreate=True)
 
     with concurrent.futures.ThreadPoolExecutor() as executor:
         save_function = partial(_save_single_feature, filesystem=filesystem, compress_level=compress_level)
         list(executor.map(save_function, data_for_saving))  # Wrapped in a list to get better exceptions
 
-    if overwrite_permission is not OverwritePermission.OVERWRITE_PATCH:
-        remove_redundant_files(filesystem, eopatch_features, file_information, compress_level)
+    with warnings.catch_warnings():
+        warnings.simplefilter("ignore", category=EODeprecationWarning)
+        if overwrite_permission is not OverwritePermission.OVERWRITE_PATCH:
+            remove_redundant_files(filesystem, eopatch_features, file_information, compress_level)
 
 
 def _remove_old_eopatch(filesystem: FS, patch_location: str) -> None:
     filesystem.removetree(patch_location)
     filesystem.makedirs(patch_location, recreate=True)
 
 
 def _yield_features_to_save(
-    eopatch: EOPatch, eopatch_features: List[FeatureSpec], patch_location: str
-) -> Iterator[Tuple[Type[FeatureIO], Any, str]]:
+    eopatch: EOPatch, eopatch_features: list[FeatureSpec], patch_location: str
+) -> Iterator[tuple[type[FeatureIO], Any, str]]:
     """Prepares a triple `(featureIO, data, path)` so that the `featureIO` can save `data` to `path`."""
     get_file_path = partial(fs.path.join, patch_location)
     meta_features = {ftype for ftype, _ in eopatch_features if ftype.is_meta()}
 
     if eopatch.bbox is not None:  # remove after BBox is never None
         yield (FeatureIOBBox, eopatch.bbox, get_file_path(BBOX_FILENAME))
 
@@ -130,28 +145,28 @@
         yield (FeatureIOJson, eopatch.meta_info, get_file_path(FeatureType.META_INFO.value))
 
     for ftype, fname in eopatch_features:
         if not ftype.is_meta():
             yield (_get_feature_io_constructor(ftype), eopatch[(ftype, fname)], get_file_path(ftype.value, fname))
 
 
-def _save_single_feature(save_spec: Tuple[Type[FeatureIO[T]], T, str], *, filesystem: FS, compress_level: int) -> None:
+def _save_single_feature(save_spec: tuple[type[FeatureIO[T]], T, str], *, filesystem: FS, compress_level: int) -> None:
     feature_io, data, feature_path = save_spec
     feature_io.save(data, filesystem, feature_path, compress_level)
 
 
 def remove_redundant_files(
     filesystem: FS,
-    eopatch_features: List[FeatureSpec],
+    eopatch_features: list[FeatureSpec],
     preexisting_files: FilesystemDataInfo,
     current_compress_level: int,
 ) -> None:
     """Removes files that should have been overwritten but were not due to different compression levels."""
 
-    def has_different_compression(path: Optional[str]) -> bool:
+    def has_different_compression(path: str | None) -> bool:
         return path is not None and MimeType.GZIP.matches_extension(path) != (current_compress_level > 0)
 
     files_to_remove = []
     saved_meta_types = {ftype for ftype, _ in eopatch_features if ftype.is_meta()}
 
     for ftype, fname in eopatch_features:
         if ftype.is_meta():
@@ -176,15 +191,15 @@
 def load_eopatch_content(
     filesystem: FS, patch_location: str, features: FeaturesSpecification = ...
 ) -> PatchContentType:
     """A utility function used by `EOPatch.load` method."""
     file_information = get_filesystem_data_info(filesystem, patch_location, features)
     bbox, timestamps, meta_info = _load_meta_features(filesystem, file_information, features)
 
-    features_dict: Dict[Tuple[FeatureType, str], FeatureIO] = {}
+    features_dict: dict[tuple[FeatureType, str], FeatureIO] = {}
     for ftype, fname in FeatureParser(features).get_feature_specifications():
         if ftype.is_meta():
             continue
 
         if fname is ...:
             for fname, path in file_information.features.get(ftype, {}).items():
                 features_dict[(ftype, fname)] = _get_feature_io_constructor(ftype)(path, filesystem)
@@ -195,15 +210,15 @@
             features_dict[(ftype, fname)] = _get_feature_io_constructor(ftype)(path, filesystem)
 
     return bbox, timestamps, meta_info, features_dict
 
 
 def _load_meta_features(
     filesystem: FS, file_information: FilesystemDataInfo, features: FeaturesSpecification
-) -> Tuple[Optional[FeatureIOBBox], Optional[FeatureIOTimestamps], Optional[FeatureIOJson]]:
+) -> tuple[FeatureIOBBox | None, FeatureIOTimestamps | None, FeatureIOJson | None]:
     requested = {ftype for ftype, _ in FeatureParser(features).get_feature_specifications() if ftype.is_meta()}
 
     err_msg = "Feature {} is specified to be loaded but does not exist in EOPatch."
 
     bbox = None
     if file_information.bbox is not None:
         bbox = FeatureIOBBox(file_information.bbox, filesystem)
@@ -274,15 +289,15 @@
     # Note: might simplify a few things if we filtered according to features here, especially loading stuff.
     return result
 
 
 @deprecated_function(category=EODeprecationWarning)
 def walk_filesystem(
     filesystem: FS, patch_location: str, features: FeaturesSpecification = ...
-) -> Iterator[Tuple[FeatureType, Union[str, EllipsisType], str]]:
+) -> Iterator[tuple[FeatureType, str | EllipsisType, str]]:
     """Interface to the old walk_filesystem function which yields tuples of (feature_type, feature_name, file_path)."""
     file_information = get_filesystem_data_info(filesystem, patch_location, features)
 
     if file_information.bbox is not None:  # remove after BBox is never None
         yield (FeatureType.BBOX, ..., file_information.bbox)
 
     if file_information.timestamps is not None:
@@ -291,64 +306,64 @@
     if file_information.meta_info is not None:
         yield (FeatureType.META_INFO, ..., file_information.meta_info)
 
     for feature, path in file_information.iterate_features():
         yield (*feature, path)
 
 
-def walk_feature_type_folder(filesystem: FS, folder_path: str) -> Iterator[Tuple[str, str]]:
+def walk_feature_type_folder(filesystem: FS, folder_path: str) -> Iterator[tuple[str, str]]:
     """Walks a feature type subfolder of EOPatch and yields tuples (feature name, path in filesystem).
     Skips folders and files in subfolders.
     """
     for path in filesystem.listdir(folder_path):
         if "/" not in path and "." in path:
             yield _remove_file_extension(path), fs.path.combine(folder_path, path)
 
 
 def _check_collisions(
-    overwrite_permission: OverwritePermission, eopatch_features: List[FeatureSpec], existing_files: FilesystemDataInfo
+    overwrite_permission: OverwritePermission, eopatch_features: list[FeatureSpec], existing_files: FilesystemDataInfo
 ) -> None:
     """Checks for possible name collisions to avoid unintentional overwriting."""
     if overwrite_permission is OverwritePermission.ADD_ONLY:
         _check_letter_case_collisions(eopatch_features, existing_files)
         _check_add_only_permission(eopatch_features, existing_files)
 
     elif platform.system() == "Windows" and overwrite_permission is OverwritePermission.OVERWRITE_FEATURES:
         _check_letter_case_collisions(eopatch_features, existing_files)
 
     else:
         _check_letter_case_collisions(eopatch_features, FilesystemDataInfo())
 
 
-def _check_add_only_permission(eopatch_features: List[FeatureSpec], filesystem_features: FilesystemDataInfo) -> None:
+def _check_add_only_permission(eopatch_features: list[FeatureSpec], filesystem_features: FilesystemDataInfo) -> None:
     """Checks that no existing feature will be overwritten."""
     unique_filesystem_features = {_to_lowercase(*feature) for feature, _ in filesystem_features.iterate_features()}
     unique_eopatch_features = {_to_lowercase(*feature) for feature in eopatch_features}
 
     intersection = unique_filesystem_features.intersection(unique_eopatch_features)
     if intersection:
         raise ValueError(f"Cannot save features {intersection} with overwrite_permission=OverwritePermission.ADD_ONLY")
 
 
-def _check_letter_case_collisions(eopatch_features: List[FeatureSpec], filesystem_features: FilesystemDataInfo) -> None:
+def _check_letter_case_collisions(eopatch_features: list[FeatureSpec], filesystem_features: FilesystemDataInfo) -> None:
     """Check that features have no name clashes (ignoring case) with other EOPatch features and saved features."""
     lowercase_features = {_to_lowercase(*feature) for feature in eopatch_features}
 
     if len(lowercase_features) != len(eopatch_features):
         raise IOError("Some features differ only in casing and cannot be saved in separate files.")
 
     for feature, _ in filesystem_features.iterate_features():
         if feature not in eopatch_features and _to_lowercase(*feature) in lowercase_features:
             raise IOError(
                 f"There already exists a feature {feature} in the filesystem that only differs in "
                 "casing from a feature that should be saved."
             )
 
 
-def _to_lowercase(ftype: FeatureType, fname: Optional[str], *_: Any) -> Tuple[FeatureType, Optional[str]]:
+def _to_lowercase(ftype: FeatureType, fname: str | None, *_: Any) -> tuple[FeatureType, str | None]:
     """Transforms a feature to it's lowercase representation."""
     return ftype, fname if fname is None else fname.lower()
 
 
 def _remove_file_extension(path: str) -> str:
     """This also removes file extensions of form `.geojson.gz` unlike `fs.path.splitext`."""
     return path.split(".")[0]
@@ -368,15 +383,15 @@
         compressed_extension = expected_extension + f".{MimeType.GZIP.extension}"
         if not filename.endswith((expected_extension, compressed_extension)):
             raise ValueError(f"FeatureIO expects a filepath with the {expected_extension} file extension, got {path}")
 
         self.path = path
         self.filesystem = filesystem
 
-        self.loaded_value: Optional[T] = None
+        self.loaded_value: T | None = None
 
     @classmethod
     @abstractmethod
     def get_file_format(cls) -> MimeType:
         """The type of files handled by the FeatureIO."""
 
     def __repr__(self) -> str:
@@ -395,15 +410,15 @@
                     self.loaded_value = self._read_from_file(gzip_fp)
             else:
                 self.loaded_value = self._read_from_file(file_handle)
 
         return self.loaded_value
 
     @abstractmethod
-    def _read_from_file(self, file: Union[BinaryIO, gzip.GzipFile]) -> T:
+    def _read_from_file(self, file: BinaryIO | gzip.GzipFile) -> T:
         """Loads from a file and decodes content."""
 
     @classmethod
     def save(cls, data: T, filesystem: FS, feature_path: str, compress_level: int = 0) -> None:
         """Method for saving a feature. The path is assumed to be filesystem path but without file extensions.
 
         Example of path is `eopatch/data/NDVI`, which is then used to save `eopatch/data/NDVI.npy.gz`.
@@ -432,129 +447,124 @@
                 cls._write_to_file(data, file, path)
             else:
                 with gzip.GzipFile(fileobj=file, compresslevel=compress_level, mode="wb") as gzip_file:
                     cls._write_to_file(data, gzip_file, path)
 
     @classmethod
     @abstractmethod
-    def _write_to_file(cls, data: T, file: Union[BinaryIO, gzip.GzipFile], path: str) -> None:
+    def _write_to_file(cls, data: T, file: BinaryIO | gzip.GzipFile, path: str) -> None:
         """Writes data to a file in the appropriate way."""
 
 
 class FeatureIONumpy(FeatureIO[np.ndarray]):
     """FeatureIO object specialized for Numpy arrays."""
 
     @classmethod
     def get_file_format(cls) -> MimeType:
         return MimeType.NPY
 
-    def _read_from_file(self, file: Union[BinaryIO, gzip.GzipFile]) -> np.ndarray:
+    def _read_from_file(self, file: BinaryIO | gzip.GzipFile) -> np.ndarray:
         return np.load(file, allow_pickle=True)
 
     @classmethod
-    def _write_to_file(cls, data: np.ndarray, file: Union[BinaryIO, gzip.GzipFile], _: str) -> None:
+    def _write_to_file(cls, data: np.ndarray, file: BinaryIO | gzip.GzipFile, _: str) -> None:
         return np.save(file, data)
 
 
 class FeatureIOGeoDf(FeatureIO[gpd.GeoDataFrame]):
     """FeatureIO object specialized for GeoDataFrames."""
 
     @classmethod
     def get_file_format(cls) -> MimeType:
         return MimeType.GPKG
 
-    def _read_from_file(self, file: Union[BinaryIO, gzip.GzipFile]) -> gpd.GeoDataFrame:
+    def _read_from_file(self, file: BinaryIO | gzip.GzipFile) -> gpd.GeoDataFrame:
         dataframe = gpd.read_file(file)
 
         if dataframe.crs is not None:
             # Trying to preserve a standard CRS and passing otherwise
             with contextlib.suppress(ValueError), warnings.catch_warnings():
                 warnings.simplefilter("ignore", category=SHUserWarning)
                 dataframe.crs = CRS(dataframe.crs).pyproj_crs()
 
         if TIMESTAMP_COLUMN in dataframe:
             dataframe[TIMESTAMP_COLUMN] = pd.to_datetime(dataframe[TIMESTAMP_COLUMN])
 
         return dataframe
 
     @classmethod
-    def _write_to_file(cls, data: gpd.GeoDataFrame, file: Union[BinaryIO, gzip.GzipFile], path: str) -> None:
+    def _write_to_file(cls, data: gpd.GeoDataFrame, file: BinaryIO | gzip.GzipFile, path: str) -> None:
         layer = fs.path.basename(path)
-        try:
-            with warnings.catch_warnings():
-                warnings.filterwarnings(
-                    "ignore",
-                    message="You are attempting to write an empty DataFrame to file*",
-                    category=UserWarning,
-                )
-                return data.to_file(file, driver="GPKG", encoding="utf-8", layer=layer, index=False)
-        except ValueError as err:
-            # This workaround is only required for geopandas<0.11.0 and will be removed in the future.
-            if data.empty:
-                schema = infer_schema(data)
-                return data.to_file(file, driver="GPKG", encoding="utf-8", layer=layer, schema=schema)
-            raise err
+        with warnings.catch_warnings():
+            warnings.filterwarnings(
+                "ignore",
+                message="You are attempting to write an empty DataFrame to file*",
+                category=UserWarning,
+            )
+            return data.to_file(file, driver="GPKG", encoding="utf-8", layer=layer, index=False)
 
 
 class FeatureIOJson(FeatureIO[T]):
     """FeatureIO object specialized for JSON-like objects."""
 
     @classmethod
     def get_file_format(cls) -> MimeType:
         return MimeType.JSON
 
-    def _read_from_file(self, file: Union[BinaryIO, gzip.GzipFile]) -> T:
+    def _read_from_file(self, file: BinaryIO | gzip.GzipFile) -> T:
         return json.load(file)
 
     @classmethod
-    def _write_to_file(cls, data: T, file: Union[BinaryIO, gzip.GzipFile], path: str) -> None:
+    def _write_to_file(cls, data: T, file: BinaryIO | gzip.GzipFile, path: str) -> None:
         try:
-            json_data = json.dumps(data, indent=2, default=_jsonify_timestamp)
+            json_data = json.dumps(data, indent=2, default=_better_jsonify)
         except TypeError as exception:
             raise TypeError(
                 f"Failed to serialize when saving JSON file to {path}. Make sure that this feature type "
                 "contains only JSON serializable Python types before attempting to serialize it."
             ) from exception
 
         file.write(json_data.encode())
 
 
 class FeatureIOTimestamps(FeatureIOJson[List[datetime.datetime]]):
     """FeatureIOJson object specialized for List[dt.datetime]."""
 
-    def _read_from_file(self, file: Union[BinaryIO, gzip.GzipFile]) -> List[datetime.datetime]:
+    def _read_from_file(self, file: BinaryIO | gzip.GzipFile) -> list[datetime.datetime]:
         data = json.load(file)
         return [dateutil.parser.parse(timestamp) for timestamp in data]
 
 
 class FeatureIOBBox(FeatureIO[BBox]):
     """FeatureIO object specialized for BBox objects."""
 
     @classmethod
     def get_file_format(cls) -> MimeType:
         return MimeType.GEOJSON
 
-    def _read_from_file(self, file: Union[BinaryIO, gzip.GzipFile]) -> BBox:
+    def _read_from_file(self, file: BinaryIO | gzip.GzipFile) -> BBox:
         json_data = json.load(file)
         return Geometry.from_geojson(json_data).bbox
 
     @classmethod
-    def _write_to_file(cls, data: BBox, file: Union[BinaryIO, gzip.GzipFile], _: str) -> None:
+    def _write_to_file(cls, data: BBox, file: BinaryIO | gzip.GzipFile, _: str) -> None:
         json_data = json.dumps(data.geojson, indent=2)
         file.write(json_data.encode())
 
 
-def _jsonify_timestamp(param: object) -> str:
-    """Adds the option to serialize datetime.date objects via isoformat."""
+def _better_jsonify(param: object) -> Any:
+    """Adds the option to serialize datetime.date and FeatureDict objects via isoformat."""
     if isinstance(param, datetime.date):
         return param.isoformat()
+    if isinstance(param, Mapping):
+        return dict(param.items())
     raise TypeError(f"Object of type {type(param)} is not yet supported in jsonify utility function")
 
 
-def _get_feature_io_constructor(ftype: FeatureType) -> Type[FeatureIO]:
+def _get_feature_io_constructor(ftype: FeatureType) -> type[FeatureIO]:
     """Creates the correct FeatureIO, corresponding to the FeatureType."""
     if ftype is FeatureType.BBOX:
         return FeatureIOBBox
     if ftype is FeatureType.META_INFO:
         return FeatureIOJson
     if ftype is FeatureType.TIMESTAMPS:
         return FeatureIOTimestamps
```

### Comparing `eo-learn-core-1.4.1/eolearn/core/eodata_merge.py` & `eo-learn-core-1.4.2/eolearn/core/eodata_merge.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,109 +8,99 @@
 """
 from __future__ import annotations
 
 import datetime as dt
 import functools
 import itertools as it
 import warnings
-from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Sequence, Tuple, Union, cast
+from typing import Any, Callable, Literal, Sequence, Union, cast
 
 import numpy as np
 import pandas as pd
 from geopandas import GeoDataFrame
-from typing_extensions import Literal
 
 from sentinelhub import BBox
 
 from .constants import FeatureType
+from .eodata import EOPatch
 from .exceptions import EORuntimeWarning
 from .types import FeatureSpec, FeaturesSpecification
 from .utils.parsing import FeatureParser
 
-if TYPE_CHECKING:
-    from .eodata import EOPatch
-
 OperationInputType = Union[Literal[None, "concatenate", "min", "max", "mean", "median"], Callable]
 
 
 def merge_eopatches(
     *eopatches: EOPatch,
     features: FeaturesSpecification = ...,
     time_dependent_op: OperationInputType = None,
     timeless_op: OperationInputType = None,
-) -> Dict[FeatureSpec, Any]:
+) -> EOPatch:
     """Merge features of given EOPatches into a new EOPatch.
 
-    :param eopatches: Any number of EOPatches to be merged together
+    :param eopatches: Any number of EOPatches to be merged together.
     :param features: A collection of features to be merged together. By default, all features will be merged.
-    :param time_dependent_op: An operation to be used to join data for any time-dependent raster feature. Before
-        joining time slices of all arrays will be sorted. Supported options are:
+    :param time_dependent_op: An operation for joining data for time-dependent raster features. Before joining time
+        slices of all arrays will be sorted. Supported options are:
 
-        - None (default): If time slices with matching timestamps have the same values, take one. Raise an error
-          otherwise.
+        - None: If time slices with matching timestamps have the same values, take one. Raise an error otherwise.
         - 'concatenate': Keep all time slices, even the ones with matching timestamps
         - 'min': Join time slices with matching timestamps by taking minimum values. Ignore NaN values.
         - 'max': Join time slices with matching timestamps by taking maximum values. Ignore NaN values.
         - 'mean': Join time slices with matching timestamps by taking mean values. Ignore NaN values.
         - 'median': Join time slices with matching timestamps by taking median values. Ignore NaN values.
+    :param timeless_op: An operation for joining data for timeless raster features. Supported options are:
 
-    :param timeless_op: An operation to be used to join data for any timeless raster feature. Supported options
-        are:
-
-        - None (default): If arrays are the same, take one. Raise an error otherwise.
+        - None: If arrays are the same, take one. Raise an error otherwise.
         - 'concatenate': Join arrays over the last (i.e. bands) dimension
         - 'min': Join arrays by taking minimum values. Ignore NaN values.
         - 'max': Join arrays by taking maximum values. Ignore NaN values.
         - 'mean': Join arrays by taking mean values. Ignore NaN values.
         - 'median': Join arrays by taking median values. Ignore NaN values.
-
-    :return: Contents of a merged EOPatch
+    :return: A merged EOPatch
     """
+
     reduce_timestamps = time_dependent_op != "concatenate"
     time_dependent_operation = _parse_operation(time_dependent_op, is_timeless=False)
     timeless_operation = _parse_operation(timeless_op, is_timeless=True)
 
     feature_parser = FeatureParser(features)
     all_features = {feature for eopatch in eopatches for feature in feature_parser.get_features(eopatch)}
-    eopatch_content: Dict[FeatureSpec, object] = {}
 
     timestamps, order_mask_per_eopatch = _merge_timestamps(eopatches, reduce_timestamps)
     optimize_raster_temporal = _check_if_optimize(eopatches, time_dependent_op)
 
+    merged_eopatch = EOPatch(bbox=_get_common_bbox(eopatches), timestamps=timestamps)
+
     for feature in all_features:
         feature_type, feature_name = feature
 
         if feature_type.is_array():
             if feature_type.is_temporal():
-                eopatch_content[feature] = _merge_time_dependent_raster_feature(
+                merged_eopatch[feature] = _merge_time_dependent_raster_feature(
                     eopatches, feature, time_dependent_operation, order_mask_per_eopatch, optimize_raster_temporal
                 )
             else:
-                eopatch_content[feature] = _merge_timeless_raster_feature(eopatches, feature, timeless_operation)
+                merged_eopatch[feature] = _merge_timeless_raster_feature(eopatches, feature, timeless_operation)
 
         if feature_type.is_vector():
-            eopatch_content[feature] = _merge_vector_feature(eopatches, feature)
-
-        if feature_type is FeatureType.TIMESTAMPS:
-            eopatch_content[feature] = timestamps
+            merged_eopatch[feature] = _merge_vector_feature(eopatches, feature)
 
         if feature_type is FeatureType.META_INFO:
             feature_name = cast(str, feature_name)  # parser makes sure of it
-            eopatch_content[feature] = _select_meta_info_feature(eopatches, feature_name)
-
-    eopatch_content[(FeatureType.BBOX, None)] = _get_common_bbox(eopatches)
+            merged_eopatch[feature] = _select_meta_info_feature(eopatches, feature_name)
 
-    return eopatch_content
+    return merged_eopatch
 
 
 def _parse_operation(operation_input: OperationInputType, is_timeless: bool) -> Callable:
     """Transforms operation's instruction (i.e. an input string) into a function that can be applied to a list of
     arrays. If the input already is a function it returns it.
     """
-    defaults: Dict[Optional[str], Callable] = {
+    defaults: dict[str | None, Callable] = {
         None: _return_if_equal_operation,
         "concatenate": functools.partial(np.concatenate, axis=-1 if is_timeless else 0),
         "mean": functools.partial(np.nanmean, axis=0),
         "median": functools.partial(np.nanmedian, axis=0),
         "min": functools.partial(np.nanmin, axis=0),
         "max": functools.partial(np.nanmax, axis=0),
     }
@@ -127,15 +117,15 @@
     if _all_equal(arrays):
         return arrays[0]
     raise ValueError("Cannot merge given arrays because their values are not the same.")
 
 
 def _merge_timestamps(
     eopatches: Sequence[EOPatch], reduce_timestamps: bool
-) -> Tuple[List[dt.datetime], List[np.ndarray]]:
+) -> tuple[list[dt.datetime], list[np.ndarray]]:
     """Merges together timestamps from EOPatches. It also prepares a list of masks, one for each EOPatch, how
     timestamps should be ordered and joined together.
     """
     timestamps_per_eopatch = [eopatch.timestamps for eopatch in eopatches]
     all_timestamps = [timestamp for eopatch_timestamps in timestamps_per_eopatch for timestamp in eopatch_timestamps]
 
     if not all_timestamps:
@@ -211,15 +201,15 @@
 
 
 def _extract_and_join_time_dependent_feature_values(
     eopatches: Sequence[EOPatch],
     feature: FeatureSpec,
     order_mask_per_eopatch: Sequence[np.ndarray],
     optimize: bool,
-) -> Tuple[np.ndarray, np.ndarray]:
+) -> tuple[np.ndarray, np.ndarray]:
     """Collects feature arrays from EOPatches that have them and joins them together. It also joins together
     corresponding order masks.
     """
     arrays = []
     order_masks = []
     feature_type, feature_name = feature
 
@@ -293,33 +283,33 @@
             "used in a merged EOPatch."
         )
         warnings.warn(message, category=EORuntimeWarning)
 
     return values[0]
 
 
-def _get_common_bbox(eopatches: Sequence[EOPatch]) -> Optional[BBox]:
+def _get_common_bbox(eopatches: Sequence[EOPatch]) -> BBox | None:
     """Makes sure that all EOPatches, which define a bounding box and CRS, define the same ones."""
     bboxes = [eopatch.bbox for eopatch in eopatches if eopatch.bbox is not None]
 
     if not bboxes:
         return None
 
     if _all_equal(bboxes):
         return bboxes[0]
     raise ValueError("Cannot merge EOPatches because they are defined for different bounding boxes.")
 
 
-def _extract_feature_values(eopatches: Sequence[EOPatch], feature: FeatureSpec) -> List[Any]:
+def _extract_feature_values(eopatches: Sequence[EOPatch], feature: FeatureSpec) -> list[Any]:
     """A helper function that extracts a feature values from those EOPatches where a feature exists."""
     feature_type, feature_name = feature
     return [eopatch[feature] for eopatch in eopatches if feature_name in eopatch[feature_type]]
 
 
-def _all_equal(values: Union[Sequence[Any], np.ndarray]) -> bool:
+def _all_equal(values: Sequence[Any] | np.ndarray) -> bool:
     """A helper function that checks if all values in a given list are equal to each other."""
     first_value = values[0]
 
     if isinstance(first_value, np.ndarray):
         is_numeric_dtype = np.issubdtype(first_value.dtype, np.number)
         return all(np.array_equal(first_value, array, equal_nan=is_numeric_dtype) for array in values[1:])
```

### Comparing `eo-learn-core-1.4.1/eolearn/core/eoexecution.py` & `eo-learn-core-1.4.2/eolearn/core/eoexecution.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,27 +6,28 @@
 All this is implemented in EOExecutor class.
 
 Copyright (c) 2017- Sinergise and contributors
 For the full list of contributors, see the CREDITS file in the root directory of this source tree.
 
 This source code is licensed under the MIT license, see the LICENSE file in the root directory of this source tree.
 """
+from __future__ import annotations
+
 import concurrent.futures
 import datetime as dt
 import inspect
 import logging
 import threading
 import warnings
 from dataclasses import dataclass
 from logging import FileHandler, Filter, Handler, Logger
-from typing import Any, Callable, Dict, List, Optional, Sequence, Tuple, Union
+from typing import Any, Callable, Protocol, Sequence, Union
 
 import fs
 from fs.base import FS
-from typing_extensions import Protocol
 
 from .eonode import EONode
 from .eoworkflow import EOWorkflow, WorkflowResults
 from .exceptions import EORuntimeWarning
 from .utils.fs import get_base_filesystem_and_path, get_full_path, pickle_fs, unpickle_fs
 from .utils.logging import LogFileFilter
 from .utils.parallelize import _decide_processing_type, _ProcessingType, parallelize
@@ -45,50 +46,50 @@
 
 @dataclass(frozen=True)
 class _ProcessingData:
     """Data to be used in EOExecutor processing. This will be passed to a process pool, so everything has to be
     serializable with pickle."""
 
     workflow: EOWorkflow
-    workflow_kwargs: Dict[EONode, Dict[str, object]]
+    workflow_kwargs: dict[EONode, dict[str, object]]
     pickled_filesystem: bytes
-    log_path: Optional[str]
+    log_path: str | None
     filter_logs_by_thread: bool
-    logs_filter: Optional[Filter]
+    logs_filter: Filter | None
     logs_handler_factory: _HandlerFactoryType
 
 
 @dataclass(frozen=True)
 class _ExecutionRunParams:
     """Parameters that are used during execution run."""
 
-    workers: Optional[int]
+    workers: int | None
     multiprocess: bool
-    tqdm_kwargs: Dict[str, Any]
+    tqdm_kwargs: dict[str, Any]
 
 
 class EOExecutor:
     """Simultaneously executes a workflow with different input arguments. In the process it monitors execution and
     handles errors. It can also save logs and create a html report about each execution.
     """
 
     REPORT_FILENAME = "report.html"
     STATS_START_TIME = "start_time"
     STATS_END_TIME = "end_time"
 
     def __init__(
         self,
         workflow: EOWorkflow,
-        execution_kwargs: Sequence[Dict[EONode, Dict[str, object]]],
+        execution_kwargs: Sequence[dict[EONode, dict[str, object]]],
         *,
-        execution_names: Optional[List[str]] = None,
+        execution_names: list[str] | None = None,
         save_logs: bool = False,
         logs_folder: str = ".",
-        filesystem: Optional[FS] = None,
-        logs_filter: Optional[Filter] = None,
+        filesystem: FS | None = None,
+        logs_filter: Filter | None = None,
         logs_handler_factory: _HandlerFactoryType = FileHandler,
     ):
         """
         :param workflow: A prepared instance of EOWorkflow class
         :param execution_kwargs: A list of dictionaries where each dictionary represents execution inputs for the
             workflow. `EOExecutor` will execute the workflow for each of the given dictionaries in the list. The
             content of such dictionary will be used as `input_kwargs` parameter in `EOWorkflow.execution` method.
@@ -113,52 +114,52 @@
         self.execution_kwargs = self._parse_and_validate_execution_kwargs(execution_kwargs)
         self.execution_names = self._parse_execution_names(execution_names, self.execution_kwargs)
         self.save_logs = save_logs
         self.filesystem, self.logs_folder = self._parse_logs_filesystem(filesystem, logs_folder)
         self.logs_filter = logs_filter
         self.logs_handler_factory = logs_handler_factory
 
-        self.start_time: Optional[dt.datetime] = None
-        self.report_folder: Optional[str] = None
-        self.general_stats: Dict[str, object] = {}
-        self.execution_results: List[WorkflowResults] = []
+        self.start_time: dt.datetime | None = None
+        self.report_folder: str | None = None
+        self.general_stats: dict[str, object] = {}
+        self.execution_results: list[WorkflowResults] = []
 
     @staticmethod
     def _parse_and_validate_execution_kwargs(
-        execution_kwargs: Sequence[Dict[EONode, Dict[str, object]]]
-    ) -> List[Dict[EONode, Dict[str, object]]]:
+        execution_kwargs: Sequence[dict[EONode, dict[str, object]]]
+    ) -> list[dict[EONode, dict[str, object]]]:
         """Parses and validates execution arguments provided by user and raises an error if something is wrong."""
         if not isinstance(execution_kwargs, (list, tuple)):
             raise ValueError("Parameter 'execution_kwargs' should be a list.")
 
         for input_kwargs in execution_kwargs:
             EOWorkflow.validate_input_kwargs(input_kwargs)
 
         return [input_kwargs or {} for input_kwargs in execution_kwargs]
 
     @staticmethod
-    def _parse_execution_names(execution_names: Optional[List[str]], execution_kwargs: Sequence) -> List[str]:
+    def _parse_execution_names(execution_names: list[str] | None, execution_kwargs: Sequence) -> list[str]:
         """Parses a list of execution names."""
         if execution_names is None:
             return [str(num) for num in range(1, len(execution_kwargs) + 1)]
 
         if not isinstance(execution_names, (list, tuple)) or len(execution_names) != len(execution_kwargs):
             raise ValueError(
                 "Parameter 'execution_names' has to be a list of the same size as the list of execution arguments."
             )
         return execution_names
 
     @staticmethod
-    def _parse_logs_filesystem(filesystem: Optional[FS], logs_folder: str) -> Tuple[FS, str]:
+    def _parse_logs_filesystem(filesystem: FS | None, logs_folder: str) -> tuple[FS, str]:
         """Ensures a filesystem and a file path relative to it."""
         if filesystem is None:
             return get_base_filesystem_and_path(logs_folder)
         return filesystem, logs_folder
 
-    def run(self, workers: Optional[int] = 1, multiprocess: bool = True, **tqdm_kwargs: Any) -> List[WorkflowResults]:
+    def run(self, workers: int | None = 1, multiprocess: bool = True, **tqdm_kwargs: Any) -> list[WorkflowResults]:
         """Runs the executor with n workers.
 
         :param workers: Maximum number of workflows which will be executed in parallel. Default value is `1` which will
             execute workflows consecutively. If set to `None` the number of workers will be the number of processors
             of the system.
         :param multiprocess: If `True` it will use `concurrent.futures.ProcessPoolExecutor` which will distribute
             workflow executions among multiple processors. If `False` it will use
@@ -173,15 +174,15 @@
         self.start_time = dt.datetime.now()
         self.report_folder = fs.path.combine(
             self.logs_folder, f'eoexecution-report-{self.start_time.strftime("%Y_%m_%d-%H_%M_%S")}'
         )
         if self.save_logs:
             self.filesystem.makedirs(self.report_folder, recreate=True)
 
-        log_paths: Sequence[Optional[str]]
+        log_paths: Sequence[str | None]
         if self.save_logs:
             log_paths = self.get_log_paths(full_path=False)
         else:
             log_paths = [None] * len(self.execution_kwargs)
 
         filter_logs_by_thread = not multiprocess and workers is not None and workers > 1
         processing_args = [
@@ -203,58 +204,58 @@
         processing_type = self._get_processing_type(workers=workers, multiprocess=multiprocess)
         self.general_stats = self._prepare_general_stats(workers, processing_type)
 
         return full_execution_results
 
     @classmethod
     def _run_execution(
-        cls, processing_args: List[_ProcessingData], run_params: _ExecutionRunParams
-    ) -> List[WorkflowResults]:
+        cls, processing_args: list[_ProcessingData], run_params: _ExecutionRunParams
+    ) -> list[WorkflowResults]:
         """Parallelizes the execution for each item of processing_args list."""
         return parallelize(
             cls._execute_workflow,
             processing_args,
             workers=run_params.workers,
             multiprocess=run_params.multiprocess,
             **run_params.tqdm_kwargs,
         )
 
     @classmethod
     def _try_add_logging(
         cls,
-        log_path: Optional[str],
+        log_path: str | None,
         pickled_filesystem: bytes,
         filter_logs_by_thread: bool,
-        logs_filter: Optional[Filter],
+        logs_filter: Filter | None,
         logs_handler_factory: _HandlerFactoryType,
-    ) -> Tuple[Optional[Logger], Optional[Handler]]:
+    ) -> tuple[Logger | None, Handler | None]:
         """Adds a handler to a logger and returns them both. In case this fails it shows a warning."""
         if log_path:
             try:
                 logger = logging.getLogger()
                 logger.setLevel(logging.DEBUG)
                 handler = cls._build_log_handler(
                     log_path, pickled_filesystem, filter_logs_by_thread, logs_filter, logs_handler_factory
                 )
                 logger.addHandler(handler)
                 return logger, handler
             except BaseException as exception:
-                warnings.warn(f"Failed to start logging with exception: {repr(exception)}", category=EORuntimeWarning)
+                warnings.warn(f"Failed to start logging with exception: {exception!r}", category=EORuntimeWarning)
 
         return None, None
 
     @classmethod
-    def _try_remove_logging(cls, log_path: Optional[str], logger: Optional[Logger], handler: Optional[Handler]) -> None:
+    def _try_remove_logging(cls, log_path: str | None, logger: Logger | None, handler: Handler | None) -> None:
         """Removes a handler from a logger in case that handler exists."""
         if log_path and logger and handler:
             try:
                 handler.close()
                 logger.removeHandler(handler)
             except BaseException as exception:
-                warnings.warn(f"Failed to end logging with exception: {repr(exception)}", category=EORuntimeWarning)
+                warnings.warn(f"Failed to end logging with exception: {exception!r}", category=EORuntimeWarning)
 
     @classmethod
     def _execute_workflow(cls, data: _ProcessingData) -> WorkflowResults:
         """Handles a single execution of a workflow."""
         logger, handler = cls._try_add_logging(
             data.log_path,
             data.pickled_filesystem,
@@ -269,15 +270,15 @@
         return results
 
     @staticmethod
     def _build_log_handler(
         log_path: str,
         pickled_filesystem: bytes,
         filter_logs_by_thread: bool,
-        logs_filter: Optional[Filter],
+        logs_filter: Filter | None,
         logs_handler_factory: _HandlerFactoryType,
     ) -> Handler:
         """Provides object which handles logs."""
         filesystem = unpickle_fs(pickled_filesystem)
 
         factory_signature = inspect.signature(logs_handler_factory)
         if "filesystem" in factory_signature.parameters:
@@ -295,39 +296,39 @@
 
         if logs_filter:
             handler.addFilter(logs_filter)
 
         return handler
 
     @staticmethod
-    def _get_processing_type(workers: Optional[int], multiprocess: bool) -> _ProcessingType:
+    def _get_processing_type(workers: int | None, multiprocess: bool) -> _ProcessingType:
         """Provides a type of processing according to given parameters."""
         return _decide_processing_type(workers=workers, multiprocess=multiprocess)
 
-    def _prepare_general_stats(self, workers: Optional[int], processing_type: _ProcessingType) -> Dict[str, object]:
+    def _prepare_general_stats(self, workers: int | None, processing_type: _ProcessingType) -> dict[str, object]:
         """Prepares a dictionary with a general statistics about executions."""
         failed_count = sum(results.workflow_failed() for results in self.execution_results)
         return {
             self.STATS_START_TIME: self.start_time,
             self.STATS_END_TIME: dt.datetime.now(),
             "finished": len(self.execution_results) - failed_count,
             "failed": failed_count,
             "processing_type": processing_type.value,
             "workers": workers,
         }
 
-    def get_successful_executions(self) -> List[int]:
+    def get_successful_executions(self) -> list[int]:
         """Returns a list of IDs of successful executions. The IDs are integers from interval
         `[0, len(execution_kwargs) - 1]`, sorted in increasing order.
 
         :return: List of successful execution IDs
         """
         return [idx for idx, results in enumerate(self.execution_results) if not results.workflow_failed()]
 
-    def get_failed_executions(self) -> List[int]:
+    def get_failed_executions(self) -> list[int]:
         """Returns a list of IDs of failed executions. The IDs are integers from interval
         `[0, len(execution_kwargs) - 1]`, sorted in increasing order.
 
         :return: List of failed execution IDs
         """
         return [idx for idx, results in enumerate(self.execution_results) if results.workflow_failed()]
 
@@ -358,38 +359,38 @@
         except ImportError:
             raise RuntimeError(
                 "Subpackage eo-learn-visualization has to be installed in order to create EOExecutor reports."
             )
 
         return EOExecutorVisualization(self).make_report(include_logs=include_logs)
 
-    def get_log_paths(self, full_path: bool = True) -> List[str]:
+    def get_log_paths(self, full_path: bool = True) -> list[str]:
         """Returns a list of file paths containing logs.
 
         :param full_path: A flag to specify if it should return full absolute paths or paths relative to the
             filesystem object.
         :return: A list of paths to log files.
         """
         if self.report_folder is None:
             raise RuntimeError("Executor has to be run before log paths are created.")
         log_paths = [fs.path.combine(self.report_folder, f"eoexecution-{name}.log") for name in self.execution_names]
         if full_path:
             return [get_full_path(self.filesystem, path) for path in log_paths]
         return log_paths
 
-    def read_logs(self) -> List[Optional[str]]:
+    def read_logs(self) -> list[str | None]:
         """Loads the content of log files if logs have been saved."""
         if not self.save_logs:
             return [None] * len(self.execution_kwargs)
 
         log_paths = self.get_log_paths(full_path=False)
         with concurrent.futures.ThreadPoolExecutor() as executor:
             return list(executor.map(self._read_log_file, log_paths))
 
     def _read_log_file(self, log_path: str) -> str:
         """Read a content of a log file."""
         try:
             with self.filesystem.open(log_path, "r") as file_handle:
                 return file_handle.read()
         except BaseException as exception:
-            warnings.warn(f"Failed to load logs with exception: {repr(exception)}", category=EORuntimeWarning)
+            warnings.warn(f"Failed to load logs with exception: {exception!r}", category=EORuntimeWarning)
             return "Failed to load logs"
```

### Comparing `eo-learn-core-1.4.1/eolearn/core/eonode.py` & `eo-learn-core-1.4.2/eolearn/core/eonode.py`

 * *Files identical despite different names*

### Comparing `eo-learn-core-1.4.1/eolearn/core/eotask.py` & `eo-learn-core-1.4.2/eolearn/core/eotask.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 """
 from __future__ import annotations
 
 import inspect
 import logging
 from abc import ABCMeta, abstractmethod
 from dataclasses import dataclass
-from typing import Any, Callable, Dict, Iterable, List, Optional, Tuple, Type, TypeVar, Union
+from typing import Any, Callable, Iterable, TypeVar
 
 from sentinelhub.exceptions import deprecated_function
 
 from .constants import FeatureType
 from .eodata import EOPatch
 from .exceptions import EODeprecationWarning
 from .types import EllipsisType, FeatureSpec, FeaturesSpecification, SingleFeatureSpec
@@ -42,19 +42,19 @@
     parse_renamed_feature = staticmethod(
         deprecated_function(EODeprecationWarning, PARSE_RENAMED_DEPRECATE_MSG)(parse_renamed_feature)
     )
     parse_renamed_features = staticmethod(
         deprecated_function(EODeprecationWarning, PARSE_RENAMED_DEPRECATE_MSG)(parse_renamed_features)
     )
 
-    def __new__(cls: Type[Self], *args: Any, **kwargs: Any) -> Self:
+    def __new__(cls: type[Self], *args: Any, **kwargs: Any) -> Self:
         """Stores initialization parameters and the order to the instance attribute `init_args`."""
         self = super().__new__(cls)  # type: ignore[misc]
 
-        init_args: Dict[str, object] = {}
+        init_args: dict[str, object] = {}
         for arg, value in zip(inspect.getfullargspec(self.__init__).args[1 : len(args) + 1], args):
             init_args[arg] = repr(value)
         for arg in inspect.getfullargspec(self.__init__).args[len(args) + 1 :]:
             if arg in kwargs:
                 init_args[arg] = repr(kwargs[arg])
 
         self._private_task_config = _PrivateTaskConfig(init_args=init_args)
@@ -78,39 +78,39 @@
     @abstractmethod
     def execute(self, *eopatches, **kwargs):  # type: ignore[no-untyped-def] # must be ignored so subclasses can change
         """Override to specify action performed by task."""
 
     @staticmethod
     def parse_feature(
         feature: SingleFeatureSpec,
-        eopatch: Optional[EOPatch] = None,
-        allowed_feature_types: Union[EllipsisType, Iterable[FeatureType], Callable[[FeatureType], bool]] = ...,
-    ) -> Tuple[FeatureType, Optional[str]]:
+        eopatch: EOPatch | None = None,
+        allowed_feature_types: EllipsisType | Iterable[FeatureType] | Callable[[FeatureType], bool] = ...,
+    ) -> tuple[FeatureType, str | None]:
         """See `eolearn.core.utils.parse_feature`."""
         return parse_feature(feature, eopatch, allowed_feature_types)
 
     @staticmethod
     def parse_features(
         features: FeaturesSpecification,
-        eopatch: Optional[EOPatch] = None,
-        allowed_feature_types: Union[EllipsisType, Iterable[FeatureType], Callable[[FeatureType], bool]] = ...,
-    ) -> List[FeatureSpec]:
+        eopatch: EOPatch | None = None,
+        allowed_feature_types: EllipsisType | Iterable[FeatureType] | Callable[[FeatureType], bool] = ...,
+    ) -> list[FeatureSpec]:
         """See `eolearn.core.utils.parse_features`."""
         return parse_features(features, eopatch, allowed_feature_types)
 
     @staticmethod
     def get_feature_parser(
         features: FeaturesSpecification,
-        allowed_feature_types: Union[EllipsisType, Iterable[FeatureType], Callable[[FeatureType], bool]] = ...,
+        allowed_feature_types: EllipsisType | Iterable[FeatureType] | Callable[[FeatureType], bool] = ...,
     ) -> FeatureParser:
         """See :class:`FeatureParser<eolearn.core.utils.FeatureParser>`."""
         return FeatureParser(features, allowed_feature_types=allowed_feature_types)
 
 
 @dataclass(frozen=True)
 class _PrivateTaskConfig:
     """A container for configuration parameters about an EOTask itself.
 
     :param init_args: A dictionary of parameters and values used for EOTask initialization
     """
 
-    init_args: Dict[str, object]
+    init_args: dict[str, object]
```

### Comparing `eo-learn-core-1.4.1/eolearn/core/eoworkflow.py` & `eo-learn-core-1.4.2/eolearn/core/eoworkflow.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,19 +13,21 @@
 The workflow can be exported to a DOT description language and visualized.
 
 Copyright (c) 2017- Sinergise and contributors
 For the full list of contributors, see the CREDITS file in the root directory of this source tree.
 
 This source code is licensed under the MIT license, see the LICENSE file in the root directory of this source tree.
 """
+from __future__ import annotations
+
 import datetime as dt
 import logging
 import traceback
 from dataclasses import dataclass, field, fields
-from typing import Dict, List, Optional, Sequence, Set, Tuple, cast
+from typing import Sequence, Tuple, cast
 
 from .eodata import EOPatch
 from .eonode import EONode, NodeStats
 from .eotask import EOTask
 from .eoworkflow_tasks import OutputTask
 from .graph import DirectedGraph
 
@@ -77,15 +79,15 @@
         for node in nodes:
             if not isinstance(node, EONode):
                 raise ValueError(f"Expected a {EONode.__name__} object but got {type(node)}")
 
         return nodes
 
     @staticmethod
-    def _make_uid_dict(nodes: Sequence[EONode]) -> Dict[str, EONode]:
+    def _make_uid_dict(nodes: Sequence[EONode]) -> dict[str, EONode]:
         """Creates a dictionary mapping node IDs to nodes while checking uniqueness of tasks.
 
         :param nodes: The sequence of workflow nodes defining the computational graph
         :return: A dictionary mapping IDs to nodes
         """
         uid_dict = {}
         for node in nodes:
@@ -112,39 +114,39 @@
                     )
                 dag.add_edge(input_node.uid, node.uid)
             if not node.inputs:
                 dag.add_vertex(node.uid)
         return dag
 
     @classmethod
-    def from_endnodes(cls, *endnodes: EONode) -> "EOWorkflow":
+    def from_endnodes(cls, *endnodes: EONode) -> EOWorkflow:
         """Constructs the EOWorkflow from the end-nodes by recursively extracting nodes in the workflow structure."""
-        all_nodes: Set[EONode] = set()
-        memo: Dict[EONode, Set[EONode]] = {}
+        all_nodes: set[EONode] = set()
+        memo: dict[EONode, set[EONode]] = {}
         for endnode in endnodes:
             all_nodes = all_nodes.union(endnode.get_dependencies(_memo=memo))
         return cls(list(all_nodes))
 
     def execute(
-        self, input_kwargs: Optional[Dict[EONode, Dict[str, object]]] = None, raise_errors: bool = True
-    ) -> "WorkflowResults":
+        self, input_kwargs: dict[EONode, dict[str, object]] | None = None, raise_errors: bool = True
+    ) -> WorkflowResults:
         """Executes the workflow.
 
         :param input_kwargs: External input arguments to the workflow. They have to be in a form of a dictionary where
             each key is an `EONode` used in the workflow and each value is a dictionary or a tuple of arguments.
         :param raise_errors: In case a task in the workflow raises an error this parameter determines how the error
             will be handled. If `True` it will propagate the error and if `False` it will catch the error, write its
             stack trace in logs and in the `WorkflowResults`. In either case workflow execute will stop if an error is
             raised. This rule is not followed only in case of `KeyboardInterrupt` exception where the exception is
             always raised.
         :return: An immutable mapping containing results of terminal tasks
         """
         start_time = dt.datetime.now()
 
-        out_degrees: Dict[str, int] = self.uid_dag.get_outdegrees()
+        out_degrees: dict[str, int] = self.uid_dag.get_outdegrees()
 
         input_kwargs = input_kwargs or {}
         self.validate_input_kwargs(input_kwargs)
         uid_input_kwargs = {node.uid: args for node, args in input_kwargs.items()}
 
         output_results, stats_dict = self._execute_nodes(
             uid_input_kwargs=uid_input_kwargs, out_degrees=out_degrees, raise_errors=raise_errors
@@ -156,15 +158,15 @@
 
         LOGGER.debug("EOWorkflow ended with results %s", repr(results))
         status = "failed" if results.workflow_failed() else "finished"
         LOGGER.debug("EOWorkflow execution %s!", status)
         return results
 
     @staticmethod
-    def validate_input_kwargs(input_kwargs: Dict[EONode, Dict[str, object]]) -> None:
+    def validate_input_kwargs(input_kwargs: dict[EONode, dict[str, object]]) -> None:
         """Validates EOWorkflow input arguments provided by user and raises an error if something is wrong.
 
         :param input_kwargs: A dictionary mapping tasks to task execution arguments
         """
         for node, kwargs in input_kwargs.items():
             if not isinstance(node, EONode):
                 raise ValueError(
@@ -181,24 +183,24 @@
             if not all(isinstance(key, str) for key in kwargs):
                 raise ValueError(
                     "Keys of input argument dictionaries should names of variables, in arguments for node "
                     f"{node.get_name()} one of the keys is not a string."
                 )
 
     def _execute_nodes(
-        self, *, uid_input_kwargs: Dict[str, Dict[str, object]], out_degrees: Dict[str, int], raise_errors: bool
-    ) -> Tuple[dict, dict]:
+        self, *, uid_input_kwargs: dict[str, dict[str, object]], out_degrees: dict[str, int], raise_errors: bool
+    ) -> tuple[dict, dict]:
         """Executes workflow nodes in the predetermined order.
 
         :param uid_input_kwargs: External input arguments to the workflow.
         :param out_degrees: Dictionary mapping node IDs to their out-degrees. (The out-degree equals the number
             of tasks that depend on this task.)
         :return: Results of a workflow
         """
-        intermediate_results: Dict[str, object] = {}
+        intermediate_results: dict[str, object] = {}
         output_results = {}
         stats_dict = {}
 
         for node in self._nodes:
             result, stats = self._execute_node(
                 node=node,
                 node_input_values=[intermediate_results[input_node.uid] for input_node in node.inputs],
@@ -215,16 +217,16 @@
                 output_results[node.task.name] = result
 
             self._relax_dependencies(node=node, out_degrees=out_degrees, intermediate_results=intermediate_results)
 
         return output_results, stats_dict
 
     def _execute_node(
-        self, *, node: EONode, node_input_values: List[object], node_input_kwargs: Dict[str, object], raise_errors: bool
-    ) -> Tuple[object, NodeStats]:
+        self, *, node: EONode, node_input_values: list[object], node_input_kwargs: dict[str, object], raise_errors: bool
+    ) -> tuple[object, NodeStats]:
         """Executes a node in the workflow by running its task and returning the results.
 
         :param node: A node of the workflow.
         :param node_input_values: Values obtained from input nodes in the workflow.
         :param node_input_kwargs: Dictionary containing execution arguments specified by the user.
         :return: The result and statistics of the task in the node.
         """
@@ -253,31 +255,31 @@
             exception=exception,
             exception_traceback=exception_traceback,
         )
         return result, node_stats
 
     @staticmethod
     def _execute_task(
-        task: EOTask, task_args: List[object], task_kwargs: Dict[str, object], raise_errors: bool
-    ) -> Tuple[object, bool]:
+        task: EOTask, task_args: list[object], task_kwargs: dict[str, object], raise_errors: bool
+    ) -> tuple[object, bool]:
         """Executes an EOTask and handles any potential exceptions."""
         if raise_errors:
             return task.execute(*task_args, **task_kwargs), True
 
         try:
             return task.execute(*task_args, **task_kwargs), True
         except KeyboardInterrupt as exception:
             raise KeyboardInterrupt from exception
         except BaseException as exception:
             exception_traceback = traceback.format_exc()
             return (exception, exception_traceback), False
 
     @staticmethod
     def _relax_dependencies(
-        *, node: EONode, out_degrees: Dict[str, int], intermediate_results: Dict[str, object]
+        *, node: EONode, out_degrees: dict[str, int], intermediate_results: dict[str, object]
     ) -> None:
         """Relaxes dependencies incurred by `node` after it has been successfully executed. All the nodes it
         depended on are updated. If `node` was the last remaining node depending on a node `n` then `n`'s result
         are removed from memory.
 
         :param node: A workflow node
         :param out_degrees: Out-degrees of tasks
@@ -291,22 +293,22 @@
             # use sets in order not to attempt to delete the same node twice
             if out_degrees[relevant_node.uid] == 0:
                 LOGGER.debug(
                     "Removing intermediate result of %s (node uid: %s)", relevant_node.get_name(), relevant_node.uid
                 )
                 del intermediate_results[relevant_node.uid]
 
-    def get_nodes(self) -> List[EONode]:
+    def get_nodes(self) -> list[EONode]:
         """Returns an ordered list of all nodes within this workflow, ordered in the execution order.
 
         :return: List of all nodes withing workflow. The order of nodes is the same as the order of execution.
         """
         return self._nodes[:]
 
-    def get_node_with_uid(self, uid: Optional[str], fail_if_missing: bool = False) -> Optional[EONode]:
+    def get_node_with_uid(self, uid: str | None, fail_if_missing: bool = False) -> EONode | None:
         """Returns node with give uid, if it exists in the workflow."""
         if uid in self._uid_dict:
             return self._uid_dict[uid]
         if fail_if_missing:
             raise KeyError(f"No {EONode.__name__} with uid {uid} found in workflow.")
         return None
 
@@ -314,15 +316,15 @@
         """Generates the DOT description of the underlying computational graph.
 
         :return: The DOT representation of the computational graph
         """
         visualization = self._get_visualization()
         return visualization.get_dot()
 
-    def dependency_graph(self, filename: Optional[str] = None):  # type: ignore[no-untyped-def] # same as get_dot
+    def dependency_graph(self, filename: str | None = None):  # type: ignore[no-untyped-def] # same as get_dot
         """Visualize the computational graph.
 
         :param filename: Filename of the output image together with file extension. Supported formats: `png`, `jpg`,
             `pdf`, ... . Check `graphviz` Python package for more options
         :return: The DOT representation of the computational graph, with some more formatting
         """
         visualization = self._get_visualization()
@@ -340,32 +342,32 @@
         return EOWorkflowVisualization(self._nodes)
 
 
 @dataclass(frozen=True)
 class WorkflowResults:
     """An object containing results of an EOWorkflow execution."""
 
-    outputs: Dict[str, object]
+    outputs: dict[str, object]
     start_time: dt.datetime
     end_time: dt.datetime
-    stats: Dict[str, NodeStats]
-    error_node_uid: Optional[str] = field(init=False, default=None)
+    stats: dict[str, NodeStats]
+    error_node_uid: str | None = field(init=False, default=None)
 
     def __post_init__(self) -> None:
         """Checks if there is any node that failed during the workflow execution."""
         for node_uid, node_stats in self.stats.items():
             if node_stats.exception is not None:
                 super().__setattr__("error_node_uid", node_uid)
                 break
 
     def workflow_failed(self) -> bool:
         """Informs if the EOWorkflow execution failed."""
         return self.error_node_uid is not None
 
-    def drop_outputs(self) -> "WorkflowResults":
+    def drop_outputs(self) -> WorkflowResults:
         """Creates a new WorkflowResults object without outputs which can take a lot of memory."""
         new_params = {
             param.name: {} if param.name == "outputs" else getattr(self, param.name)
             for param in fields(self)
             if param.init
         }
         return WorkflowResults(**new_params)
```

### Comparing `eo-learn-core-1.4.1/eolearn/core/eoworkflow_tasks.py` & `eo-learn-core-1.4.2/eolearn/core/eoworkflow_tasks.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,43 +4,41 @@
 Copyright (c) 2017- Sinergise and contributors
 For the full list of contributors, see the CREDITS file in the root directory of this source tree.
 
 This source code is licensed under the MIT license, see the LICENSE file in the root directory of this source tree.
 """
 from __future__ import annotations
 
-from typing import Optional
-
 from .eodata import EOPatch
 from .eotask import EOTask
 from .types import FeaturesSpecification
 from .utils.common import generate_uid
 
 
 class InputTask(EOTask):
     """Introduces data into an EOWorkflow, where the data can be specified at initialization or at execution."""
 
-    def __init__(self, value: Optional[object] = None):
+    def __init__(self, value: object | None = None):
         """
         :param value: Default value that the task should provide as a result. Can be overridden in execution arguments
         """
         self.value = value
 
-    def execute(self, *, value: Optional[object] = None) -> object:
+    def execute(self, *, value: object | None = None) -> object:
         """
         :param value: A value that the task should provide as its result. If not set uses the value from initialization
         :return: Directly returns `value`
         """
         return value or self.value
 
 
 class OutputTask(EOTask):
     """Stores data as an output of `EOWorkflow` results."""
 
-    def __init__(self, name: Optional[str] = None, features: FeaturesSpecification = ...):
+    def __init__(self, name: str | None = None, features: FeaturesSpecification = ...):
         """
         :param name: A name under which the data will be saved in `WorkflowResults`, auto-generated if `None`
         :param features: A collection of features to be kept if the data is an `EOPatch`
         """
         self._name = name or generate_uid("output")
         self.features = features
```

### Comparing `eo-learn-core-1.4.1/eolearn/core/exceptions.py` & `eo-learn-core-1.4.2/eolearn/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `eo-learn-core-1.4.1/eolearn/core/extra/ray.py` & `eo-learn-core-1.4.2/eolearn/core/extra/ray.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 In order to use this module you have to install `ray` Python package.
 
 Copyright (c) 2017- Sinergise and contributors
 For the full list of contributors, see the CREDITS file in the root directory of this source tree.
 
 This source code is licensed under the MIT license, see the LICENSE file in the root directory of this source tree.
 """
-from typing import Any, Callable, Collection, Generator, Iterable, List, Optional, Tuple, TypeVar, cast
+from __future__ import annotations
+
+from typing import Any, Callable, Collection, Generator, Iterable, List, TypeVar, cast
 
 try:
     import ray
 except ImportError as exception:
     raise ImportError("This module requires an installation of Ray Python package") from exception
 
 from ..eoexecution import EOExecutor, _ExecutionRunParams, _ProcessingData
@@ -23,15 +25,15 @@
 _InputType = TypeVar("_InputType")
 _OutputType = TypeVar("_OutputType")
 
 
 class RayExecutor(EOExecutor):
     """A special type of `EOExecutor` that works with Ray framework"""
 
-    def run(self, **tqdm_kwargs: Any) -> List[WorkflowResults]:  # type: ignore
+    def run(self, **tqdm_kwargs: Any) -> list[WorkflowResults]:  # type: ignore[override]
         """Runs the executor using a Ray cluster
 
         Before calling this method make sure to initialize a Ray cluster using `ray.init`.
 
         :param tqdm_kwargs: Keyword arguments that will be propagated to `tqdm` progress bar.
         :return: A list of EOWorkflow results
         """
@@ -39,16 +41,16 @@
             raise RuntimeError("Please initialize a Ray cluster before calling this method")
 
         workers = ray.available_resources().get("CPU")
         return super().run(workers=workers, multiprocess=True, **tqdm_kwargs)
 
     @classmethod
     def _run_execution(
-        cls, processing_args: List[_ProcessingData], run_params: _ExecutionRunParams
-    ) -> List[WorkflowResults]:
+        cls, processing_args: list[_ProcessingData], run_params: _ExecutionRunParams
+    ) -> list[WorkflowResults]:
         """Runs ray execution"""
         futures = [_ray_workflow_executor.remote(workflow_args) for workflow_args in processing_args]
         return join_ray_futures(futures, **run_params.tqdm_kwargs)
 
     @staticmethod
     def _get_processing_type(*_: Any, **__: Any) -> _ProcessingType:
         """Provides a type of processing for later references."""
@@ -60,15 +62,15 @@
     """Called to execute a workflow on a ray worker"""
     # pylint: disable=protected-access
     return RayExecutor._execute_workflow(workflow_args)
 
 
 def parallelize_with_ray(
     function: Callable[[_InputType], _OutputType], *params: Iterable[_InputType], **tqdm_kwargs: Any
-) -> List[_OutputType]:
+) -> list[_OutputType]:
     """Parallelizes function execution with Ray.
 
     Note that this function will automatically connect to a Ray cluster, if a connection wouldn't exist yet. But it
     won't automatically shut down the connection.
 
     :param function: A normal function that is not yet decorated by `ray.remote`.
     :param params: Iterables of parameters that will be used with given function.
@@ -79,45 +81,45 @@
         raise RuntimeError("Please initialize a Ray cluster before calling this method")
 
     ray_function = ray.remote(function)
     futures = [ray_function.remote(*function_params) for function_params in zip(*params)]
     return join_ray_futures(futures, **tqdm_kwargs)
 
 
-def join_ray_futures(futures: List[ray.ObjectRef], **tqdm_kwargs: Any) -> List[Any]:
+def join_ray_futures(futures: list[ray.ObjectRef], **tqdm_kwargs: Any) -> list[Any]:
     """Resolves futures, monitors progress, and returns a list of results.
 
     :param futures: A list of futures to be joined. Note that this list will be reduced into an empty list as a side
         effect of this function. This way Ray future objects will get cleared from memory already during the execution
         and this will free memory from Ray Plasma store. But this can be achieved only if future objects aren't kept in
         memory outside `futures` list.
     :param tqdm_kwargs: Keyword arguments that will be propagated to `tqdm` progress bar.
     :return: A list of results in the order that corresponds with the order of the given input `futures`.
     """
-    results: List[Optional[Any]] = [None] * len(futures)
+    results: list[Any | None] = [None] * len(futures)
     for position, result in join_ray_futures_iter(futures, **tqdm_kwargs):
         results[position] = result
 
     return cast(List[Any], results)
 
 
 def join_ray_futures_iter(
-    futures: List[ray.ObjectRef], update_interval: float = 0.5, **tqdm_kwargs: Any
-) -> Generator[Tuple[int, Any], None, None]:
+    futures: list[ray.ObjectRef], update_interval: float = 0.5, **tqdm_kwargs: Any
+) -> Generator[tuple[int, Any], None, None]:
     """Resolves futures, monitors progress, and serves as an iterator over results.
 
     :param futures: A list of futures to be joined. Note that this list will be reduced into an empty list as a side
         effect of this function. This way Ray future objects will get cleared from memory already during the execution
         and this will free memory from Ray Plasma store. But this can be achieved only if future objects aren't kept in
         memory outside `futures` list.
     :param update_interval: A number of seconds to wait between consecutive updates of a progress bar.
     :param tqdm_kwargs: Keyword arguments that will be propagated to `tqdm` progress bar.
     :return: A generator that will be returning pairs `(index, result)` where `index` will define the position of future
         in the original list to which `result` belongs to.
     """
 
     def _ray_wait_function(
         remaining_futures: Collection[ray.ObjectRef],
-    ) -> Tuple[Collection[ray.ObjectRef], Collection[ray.ObjectRef]]:
+    ) -> tuple[Collection[ray.ObjectRef], Collection[ray.ObjectRef]]:
         return ray.wait(remaining_futures, num_returns=len(remaining_futures), timeout=float(update_interval))
 
     return _base_join_futures_iter(_ray_wait_function, ray.get, futures, **tqdm_kwargs)
```

### Comparing `eo-learn-core-1.4.1/eolearn/core/graph.py` & `eo-learn-core-1.4.2/eolearn/core/graph.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 eoworkflow module.
 
 Copyright (c) 2017- Sinergise and contributors
 For the full list of contributors, see the CREDITS file in the root directory of this source tree.
 
 This source code is licensed under the MIT license, see the LICENSE file in the root directory of this source tree.
 """
+from __future__ import annotations
 
 import collections
 import copy
-from typing import DefaultDict, Dict, Generic, Iterator, List, Optional, Sequence, Set, Tuple, TypeVar
+from typing import Generic, Iterator, Sequence, TypeVar
 
 _T = TypeVar("_T")
 
 
 class CyclicDependencyError(ValueError):
     """This error is raised when trying to get a topological ordering of a `DirectedGraph`."""
 
@@ -23,15 +24,15 @@
     """A directed graph using adjacency-list representation. The graph is multi-edge.
 
     Constructs a new graph from an adjacency list. If adjacency_dict is None, an empty graph is constructed.
 
     :param adjacency_dict: A dictionary mapping vertices to lists of neighbors
     """
 
-    def __init__(self, adjacency_dict: Optional[Dict[_T, List[_T]]] = None):
+    def __init__(self, adjacency_dict: dict[_T, list[_T]] | None = None):
         self._adj_dict = (
             collections.defaultdict(list, adjacency_dict) if adjacency_dict else collections.defaultdict(list)
         )
         self._indegrees = self._make_indegrees_dict()
         self._vertices = set(self._adj_dict.keys()) | {v for neighs in self._adj_dict.values() for v in neighs}
 
     def __len__(self) -> int:
@@ -45,58 +46,58 @@
         """
         return vertex in self._vertices
 
     def __iter__(self) -> Iterator[_T]:
         """Returns iterator over the vertices of the graph."""
         return iter(self._vertices)
 
-    def _make_indegrees_dict(self) -> DefaultDict[_T, int]:
-        indegrees: DefaultDict[_T, int] = collections.defaultdict(int)
+    def _make_indegrees_dict(self) -> collections.defaultdict[_T, int]:
+        indegrees: collections.defaultdict[_T, int] = collections.defaultdict(int)
 
         for u_vertex in self._adj_dict:
             for v_vertex in self._adj_dict[u_vertex]:
                 indegrees[v_vertex] += 1
 
         return indegrees
 
-    def get_indegrees(self) -> Dict[_T, int]:
+    def get_indegrees(self) -> dict[_T, int]:
         """Returns a dictionary containing in-degrees of vertices of the graph."""
         return dict(self._indegrees)
 
     def get_indegree(self, vertex: _T) -> int:
         """Returns the in-degree of the vertex.
 
         The in-degree is the number of vertices `vertex'` such that `vertex' -> vertex` is an edge of the graph.
 
         :param vertex: Vertex
         """
         return self._indegrees[vertex]
 
-    def get_outdegrees(self) -> Dict[_T, int]:
+    def get_outdegrees(self) -> dict[_T, int]:
         """
         :return: dictionary of out-degrees, see get_outdegree
         """
         return {vertex: len(self._adj_dict[vertex]) for vertex in self._adj_dict}
 
     def get_outdegree(self, vertex: _T) -> int:
         """Returns the out-degree of the vertex.
 
         The out-degree is the number of vertices `vertex'` such that `vertex -> vertex'` is an edge of the graph.
 
         :param vertex: Vertex
         """
         return len(self._adj_dict[vertex])
 
-    def get_adj_dict(self) -> Dict[_T, list]:
+    def get_adj_dict(self) -> dict[_T, list]:
         """
         :return: adj_dict
         """
         return {vertex: copy.copy(neighbours) for vertex, neighbours in self._adj_dict.items()}
 
-    def get_vertices(self) -> Set[_T]:
+    def get_vertices(self) -> set[_T]:
         """Returns the set of vertices of the graph."""
         return set(self._vertices)
 
     def add_edge(self, u_vertex: _T, v_vertex: _T) -> None:
         """Adds the edge `u_vertex -> v_vertex` to the graph if the edge is not already present.
 
         :param u_vertex: Vertex
@@ -156,30 +157,30 @@
         self._vertices.remove(vertex)
         return True
 
     def is_edge(self, u_vertex: _T, v_vertex: _T) -> bool:
         """True if `u_vertex -> v_vertex` is an edge of the graph. False otherwise."""
         return v_vertex in self._adj_dict[u_vertex]
 
-    def get_neighbors(self, vertex: _T) -> List[_T]:
+    def get_neighbors(self, vertex: _T) -> list[_T]:
         """Returns the set of successor vertices of `vertex`."""
         return copy.copy(self._adj_dict[vertex])
 
     @staticmethod
-    def from_edges(edges: Sequence[Tuple[_T, _T]]) -> "DirectedGraph[_T]":
+    def from_edges(edges: Sequence[tuple[_T, _T]]) -> DirectedGraph[_T]:
         """Return DirectedGraph created from edges.
         :param edges: Pairs of objects that describe all the edges of the graph
         """
         dag: DirectedGraph = DirectedGraph[_T]()
         for _u, _v in edges:
             dag.add_edge(_u, _v)
         return dag
 
     @staticmethod
-    def _is_cyclic(graph: "DirectedGraph") -> bool:
+    def _is_cyclic(graph: DirectedGraph) -> bool:
         """True if the directed graph contains a cycle. False otherwise.
 
         The algorithm is naive, running in O(V^2) time, and not intended for serious use! For production purposes on
         larger graphs consider implementing Tarjan's O(V+E)-time algorithm instead.
         """
         # pylint: disable=invalid-name
         vertices = graph.get_vertices()
@@ -192,15 +193,15 @@
                 for v in graph.get_neighbors(u):
                     if v == w:
                         return True
                     if v not in seen:
                         stack.append(v)
         return False
 
-    def topologically_ordered_vertices(self) -> List[_T]:
+    def topologically_ordered_vertices(self) -> list[_T]:
         """Computes an ordering `<` of vertices so that for any two vertices `v` and `v'` we have that if `v˙ depends
         on `v'` then `v' < v`. In words, all dependencies of a vertex precede the vertex in this ordering.
 
         :return: A list of topologically ordered dependencies
         """
         in_degrees = self.get_indegrees()
```

### Comparing `eo-learn-core-1.4.1/eolearn/core/types.py` & `eo-learn-core-1.4.2/eolearn/core/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,25 +5,23 @@
 For the full list of contributors, see the CREDITS file in the root directory of this source tree.
 
 This source code is licensed under the MIT license, see the LICENSE file in the root directory of this source tree.
 """
 import sys
 
 # pylint: disable=unused-import
-from typing import Dict, Iterable, Optional, Sequence, Tuple, Union
-
-from typing_extensions import Literal
+from typing import Dict, Iterable, Literal, Optional, Sequence, Tuple, Union
 
 from .constants import FeatureType
 
 if sys.version_info >= (3, 10):
     from types import EllipsisType  # pylint: disable=ungrouped-imports
     from typing import TypeAlias
 else:
-    import builtins  # noqa: F401
+    import builtins  # noqa: F401, RUF100
 
     from typing_extensions import TypeAlias
 
     EllipsisType: TypeAlias = "builtins.ellipsis"
 
 
 # DEVELOPER NOTE: the #: comments are applied as docstrings
```

### Comparing `eo-learn-core-1.4.1/eolearn/core/utils/common.py` & `eo-learn-core-1.4.2/eolearn/core/utils/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 Copyright (c) 2017- Sinergise and contributors
 For the full list of contributors, see the CREDITS file in the root directory of this source tree.
 
 This source code is licensed under the MIT license, see the LICENSE file in the root directory of this source tree.
 """
 import uuid
-from typing import Callable, Sequence, Tuple, Union, cast
+from typing import Callable, Mapping, Sequence, Tuple, Union, cast
 
 import geopandas as gpd
 import numpy as np
 from geopandas.testing import assert_geodataframe_equal
 
 
 def deep_eq(fst_obj: object, snd_obj: object) -> bool:
@@ -54,15 +54,15 @@
             return False
 
     if isinstance(fst_obj, (tuple, list)):
         snd_obj = cast(Sequence, snd_obj)
 
         return len(fst_obj) == len(snd_obj) and all(map(deep_eq, fst_obj, snd_obj))
 
-    if isinstance(fst_obj, dict):
+    if isinstance(fst_obj, (dict, Mapping)):
         snd_obj = cast(dict, snd_obj)
 
         if fst_obj.keys() != snd_obj.keys():
             return False
 
         return all(deep_eq(fst_obj[key], snd_obj[key]) for key in fst_obj)
```

### Comparing `eo-learn-core-1.4.1/eolearn/core/utils/fs.py` & `eo-learn-core-1.4.2/eolearn/core/utils/fs.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,17 @@
 from fs.base import FS
 from fs.memoryfs import MemoryFS
 from fs.tempfs import TempFS
 from fs_s3fs import S3FS
 
 from sentinelhub import SHConfig
 
+# because we access internals when pickling FS
+# ruff: noqa: SLF001
+
 
 def get_filesystem(
     path: Union[str, Path], create: bool = False, config: Optional[SHConfig] = None, **kwargs: Any
 ) -> FS:
     """A utility function for initializing any type of filesystem object with PyFilesystem2 package.
 
     :param path: A filesystem path
```

### Comparing `eo-learn-core-1.4.1/eolearn/core/utils/logging.py` & `eo-learn-core-1.4.2/eolearn/core/utils/logging.py`

 * *Files identical despite different names*

### Comparing `eo-learn-core-1.4.1/eolearn/core/utils/parallelize.py` & `eo-learn-core-1.4.2/eolearn/core/utils/parallelize.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,26 +3,28 @@
 library.
 
 Copyright (c) 2017- Sinergise and contributors
 For the full list of contributors, see the CREDITS file in the root directory of this source tree.
 
 This source code is licensed under the MIT license, see the LICENSE file in the root directory of this source tree.
 """
+from __future__ import annotations
+
 import concurrent.futures
 import multiprocessing
 from concurrent.futures import FIRST_COMPLETED, Executor, Future, ProcessPoolExecutor, ThreadPoolExecutor
 from enum import Enum
-from typing import TYPE_CHECKING, Any, Callable, Collection, Generator, Iterable, List, Optional, Tuple, TypeVar, cast
+from typing import TYPE_CHECKING, Any, Callable, Collection, Generator, Iterable, List, TypeVar, cast
 
 from tqdm.auto import tqdm
 
 if TYPE_CHECKING:
     from threading import Lock
 
-    MULTIPROCESSING_LOCK: Optional[Lock] = None
+    MULTIPROCESSING_LOCK: Lock | None = None
 else:
     MULTIPROCESSING_LOCK = None
 
 # pylint: disable=invalid-name
 _T = TypeVar("_T")
 _FutureType = TypeVar("_FutureType")
 _OutputType = TypeVar("_OutputType")
@@ -33,15 +35,15 @@
 
     SINGLE_PROCESS = "single process"
     MULTIPROCESSING = "multiprocessing"
     MULTITHREADING = "multithreading"
     RAY = "ray"
 
 
-def _decide_processing_type(workers: Optional[int], multiprocess: bool) -> _ProcessingType:
+def _decide_processing_type(workers: int | None, multiprocess: bool) -> _ProcessingType:
     """Decides processing type according to given parameters.
 
     :param workers: A number of workers to be used (either threads or processes). If a single worker is given it will
         always use the current thread and process.
     :param multiprocess: A flag to decide between multiple processes and multiple threads in a single process.
     :return: An enum defining a type of processing.
     """
@@ -51,18 +53,18 @@
         return _ProcessingType.MULTIPROCESSING
     return _ProcessingType.MULTITHREADING
 
 
 def parallelize(
     function: Callable[..., _OutputType],
     *params: Iterable[Any],
-    workers: Optional[int],
+    workers: int | None,
     multiprocess: bool = True,
     **tqdm_kwargs: Any,
-) -> List[_OutputType]:
+) -> list[_OutputType]:
     """Parallelizes the function on given parameters using the specified number of workers.
 
     :param function: A function to be parallelized.
     :param params: Sequences of parameters to be given to the function. It uses the same logic as Python `map` function.
     :param workers: Maximum number of time the function will be executed in parallel.
     :param multiprocess: If `True` it will use `concurrent.futures.ProcessPoolExecutor` which will distribute
         workflow executions among multiple processors. If `False` it will use
@@ -114,76 +116,76 @@
 
 
 def submit_and_monitor_execution(
     executor: Executor,
     function: Callable[..., _OutputType],
     *params: Iterable[Any],
     **tqdm_kwargs: Any,
-) -> List[_OutputType]:
+) -> list[_OutputType]:
     """Performs the execution parallelization and monitors the process using a progress bar.
 
     :param executor: An object that performs parallelization.
     :param function: A function to be parallelized.
     :param params: Each element in a sequence are parameters for a single call of `function`.
     :return: A list of results in the same order as input parameters given by `executor_params`.
     """
     futures = [executor.submit(function, *function_params) for function_params in zip(*params)]
     return join_futures(futures, **tqdm_kwargs)
 
 
-def join_futures(futures: List[Future], **tqdm_kwargs: Any) -> List[Any]:
+def join_futures(futures: list[Future], **tqdm_kwargs: Any) -> list[Any]:
     """Resolves futures, monitors progress, and returns a list of results.
 
     :param futures: A list of futures to be joined. Note that this list will be reduced into an empty list as a side
         effect of this function. This way future objects will get cleared from memory already during the execution
         which will free some extra memory. But this can be achieved only if future objects aren't kept in memory
         outside `futures` list.
     :param tqdm_kwargs: Keyword arguments that will be propagated to `tqdm` progress bar.
     :return: A list of results in the order that corresponds with the order of the given input `futures`.
     """
-    results: List[Optional[Any]] = [None] * len(futures)
+    results: list[Any | None] = [None] * len(futures)
     for position, result in join_futures_iter(futures, **tqdm_kwargs):
         results[position] = result
 
     return cast(List[Any], results)
 
 
 def join_futures_iter(
-    futures: List[Future], update_interval: float = 0.5, **tqdm_kwargs: Any
-) -> Generator[Tuple[int, Any], None, None]:
+    futures: list[Future], update_interval: float = 0.5, **tqdm_kwargs: Any
+) -> Generator[tuple[int, Any], None, None]:
     """Resolves futures, monitors progress, and serves as an iterator over results.
 
     :param futures: A list of futures to be joined. Note that this list will be reduced into an empty list as a side
         effect of this function. This way future objects will get cleared from memory already during the execution
         which will free some extra memory. But this can be achieved only if future objects aren't kept in memory
         outside `futures` list.
     :param update_interval: A number of seconds to wait between consecutive updates of a progress bar.
     :param tqdm_kwargs: Keyword arguments that will be propagated to `tqdm` progress bar.
     :return: A generator that will be returning pairs `(index, result)` where `index` will define the position of future
         in the original list to which `result` belongs to.
     """
 
-    def _wait_function(remaining_futures: Collection[Future]) -> Tuple[Collection[Future], Collection[Future]]:
+    def _wait_function(remaining_futures: Collection[Future]) -> tuple[Collection[Future], Collection[Future]]:
         done, not_done = concurrent.futures.wait(
             remaining_futures, timeout=float(update_interval), return_when=FIRST_COMPLETED
         )
         return done, not_done
 
     def _get_result(future: Future) -> Any:
         return future.result()
 
     return _base_join_futures_iter(_wait_function, _get_result, futures, **tqdm_kwargs)
 
 
 def _base_join_futures_iter(
-    wait_function: Callable[[Collection[_FutureType]], Tuple[Collection[_FutureType], Collection[_FutureType]]],
+    wait_function: Callable[[Collection[_FutureType]], tuple[Collection[_FutureType], Collection[_FutureType]]],
     get_result_function: Callable[[_FutureType], _OutputType],
-    futures: List[_FutureType],
+    futures: list[_FutureType],
     **tqdm_kwargs: Any,
-) -> Generator[Tuple[int, _OutputType], None, None]:
+) -> Generator[tuple[int, _OutputType], None, None]:
     """A generalized utility function that resolves futures, monitors progress, and serves as an iterator over
     results."""
     if not isinstance(futures, list):
         raise ValueError(f"Parameters 'futures' should be a list but {type(futures)} was given")
     remaining_futures: Collection[_FutureType] = _make_copy_and_empty_given(futures)
 
     id_to_position_map = {id(future): index for index, future in enumerate(remaining_futures)}
@@ -194,13 +196,13 @@
             for future in done:
                 result = get_result_function(future)
                 result_position = id_to_position_map[id(future)]
                 pbar.update(1)
                 yield result_position, result
 
 
-def _make_copy_and_empty_given(items: List[_T]) -> List[_T]:
+def _make_copy_and_empty_given(items: list[_T]) -> list[_T]:
     """Removes items from the given list and returns its copy. The side effect of removing items is intentional."""
     items_copy = items[:]
     while items:
         items.pop()
     return items_copy
```

### Comparing `eo-learn-core-1.4.1/eolearn/core/utils/parsing.py` & `eo-learn-core-1.4.2/eolearn/core/utils/parsing.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 For the full list of contributors, see the CREDITS file in the root directory of this source tree.
 
 This source code is licensed under the MIT license, see the LICENSE file in the root directory of this source tree.
 """
 from __future__ import annotations
 
 import contextlib
-from typing import TYPE_CHECKING, Callable, Iterable, List, Optional, Sequence, Tuple, Union, cast
+from typing import TYPE_CHECKING, Callable, Iterable, Sequence, Tuple, Union, cast
 
 from ..constants import FeatureType
 from ..types import (
     DictFeatureSpec,
     EllipsisType,
     FeatureRenameSpec,
     FeatureSpec,
@@ -86,15 +86,15 @@
     - For `get_features` a list of pairs `(feature_type, feature_name)`.
     - For `get_renamed_features` a list of triples `(feature_type, old_name, new_name)`.
     """
 
     def __init__(
         self,
         features: FeaturesSpecification,
-        allowed_feature_types: Union[Iterable[FeatureType], Callable[[FeatureType], bool], EllipsisType] = ...,
+        allowed_feature_types: Iterable[FeatureType] | Callable[[FeatureType], bool] | EllipsisType = ...,
     ):
         """
         :param features: A collection of features in one of the supported formats
         :param allowed_feature_types: Makes sure that only features of these feature types will be returned, otherwise
             an error is raised
         :raises: ValueError
         """
@@ -102,15 +102,15 @@
             self.allowed_feature_types = set(filter(allowed_feature_types, FeatureType))
         else:
             self.allowed_feature_types = (
                 set(allowed_feature_types) if isinstance(allowed_feature_types, Iterable) else set(FeatureType)
             )
         self._feature_specs = self._parse_features(features)
 
-    def _parse_features(self, features: FeaturesSpecification) -> List[_ParserFeaturesSpec]:
+    def _parse_features(self, features: FeaturesSpecification) -> list[_ParserFeaturesSpec]:
         """This method parses and validates input, returning a list of `(ftype, old_name, new_name)` triples.
 
         Due to typing issues the all-features requests are transformed from `(ftype, ...)` to `(ftype, None, None)`.
         This is a correct schema for BBOX and TIMESTAMPS while for other features this is corrected when outputting,
         either by processing the request or by substituting ellipses back (case of `get_feature_specifications`).
         """
 
@@ -131,18 +131,18 @@
         raise ValueError(
             f"Unable to parse features {features}. Please see specifications of FeatureParser on viable inputs."
         )
 
     def _parse_dict(
         self,
         features: DictFeatureSpec,
-    ) -> List[_ParserFeaturesSpec]:
+    ) -> list[_ParserFeaturesSpec]:
         """Implements parsing and validation in case the input is a dictionary."""
 
-        feature_specs: List[_ParserFeaturesSpec] = []
+        feature_specs: list[_ParserFeaturesSpec] = []
 
         for feature_type, feature_names in features.items():
             feature_type = self._parse_feature_type(feature_type, message_about_position="keys of the dictionary")
 
             if feature_names in (..., None):
                 feature_specs.append((feature_type, None, None))
                 continue
@@ -155,19 +155,19 @@
             parsed_names = [(feature_type, *self._parse_feature_name(feature_type, name)) for name in feature_names]
             feature_specs.extend(parsed_names)
 
         return feature_specs
 
     def _parse_sequence(
         self,
-        features: Union[SingleFeatureSpec, SequenceFeatureSpec],
-    ) -> List[_ParserFeaturesSpec]:
+        features: SingleFeatureSpec | SequenceFeatureSpec,
+    ) -> list[_ParserFeaturesSpec]:
         """Implements parsing and validation in case the input is a tuple describing a single feature or a sequence."""
 
-        feature_specs: List[_ParserFeaturesSpec] = []
+        feature_specs: list[_ParserFeaturesSpec] = []
 
         # Check for possible singleton
         if 2 <= len(features) <= 3:
             with contextlib.suppress(ValueError):
                 return [(self._parse_singleton(features))]
 
         for feature in features:
@@ -196,15 +196,15 @@
 
         self._fail_for_noname_features(feature_type, feature_name)
 
         feature_name = feature_name[0] if len(feature_name) == 1 else feature_name
         parsed_name = self._parse_feature_name(feature_type, feature_name)
         return (feature_type, *parsed_name)
 
-    def _parse_feature_type(self, feature_type: Union[str, FeatureType], *, message_about_position: str) -> FeatureType:
+    def _parse_feature_type(self, feature_type: str | FeatureType, *, message_about_position: str) -> FeatureType:
         """Tries to extract a feature type if possible, fails otherwise.
 
         The parameter `message_about_position` is used for more informative error messages.
         """
         try:
             feature_type = FeatureType(feature_type)
         except ValueError as exception:
@@ -215,15 +215,15 @@
         if feature_type not in self.allowed_feature_types:
             raise ValueError(
                 f"Allowed feature types were set to be {self.allowed_feature_types} but found {feature_type}"
             )
         return feature_type
 
     @staticmethod
-    def _parse_feature_name(feature_type: FeatureType, name: object) -> Tuple[str, str]:
+    def _parse_feature_name(feature_type: FeatureType, name: object) -> tuple[str, str]:
         """Parses input in places where a feature name is expected, handling the cases of a name and renaming pair."""
         if isinstance(name, str):
             return name, name
         if isinstance(name, (tuple, list)):
             if len(name) != 2 or not all(isinstance(n, str) for n in name):
                 raise ValueError(
                     "When specifying a re-name for a feature it must be a pair of strings `(old_name, new_name)`, "
@@ -243,46 +243,46 @@
         """
         if feature_type in (FeatureType.BBOX, FeatureType.TIMESTAMPS):
             raise ValueError(
                 f"For features of type {feature_type} the only acceptable specification is `...` or `None`, got"
                 f" {specification} instead."
             )
 
-    def get_feature_specifications(self) -> List[Tuple[FeatureType, Union[str, EllipsisType]]]:
+    def get_feature_specifications(self) -> list[tuple[FeatureType, str | EllipsisType]]:
         """Returns the feature specifications in a more streamlined fashion.
 
         Requests for all features, e.g. `(FeatureType.DATA, ...)`, are returned directly.
         """
         return [(ftype, ... if fname is None else fname) for ftype, fname, _ in self._feature_specs]
 
-    def get_features(self, eopatch: Optional[EOPatch] = None) -> List[FeatureSpec]:
+    def get_features(self, eopatch: EOPatch | None = None) -> list[FeatureSpec]:
         """Returns a list of `(feature_type, feature_name)` pairs.
 
         For features that specify renaming, the new name of the feature is ignored.
 
         If `eopatch` is provided, the method checks that the EOPatch contains all the specified data and processes
         requests for all features, e.g. `(FeatureType.DATA, ...)`, by listing all available features of given type.
 
         If `eopatch` is not provided the method fails if an all-feature request is in the specification.
         """
         renamed_features = self.get_renamed_features(eopatch)
         return [feature[:2] for feature in renamed_features]  # pattern unpacking messes with typechecking
 
-    def get_renamed_features(self, eopatch: Optional[EOPatch] = None) -> List[FeatureRenameSpec]:
+    def get_renamed_features(self, eopatch: EOPatch | None = None) -> list[FeatureRenameSpec]:
         """Returns a list of `(feature_type, old_name, new_name)` triples.
 
         For features without a specified renaming the new name is equal to the old one.
 
         If `eopatch` is provided, the method checks that the EOPatch contains all the specified data and processes
         requests for all features, e.g. `(FeatureType.DATA, ...)`, by listing all available features of given type.
         In these cases the returned `old_name` and `new_name` are equal.
 
         If `eopatch` is not provided the method fails if an all-feature request is in the specification.
         """
-        parsed_features: List[FeatureRenameSpec] = []
+        parsed_features: list[FeatureRenameSpec] = []
         for feature_spec in self._feature_specs:
             ftype, old_name, new_name = feature_spec
 
             if ftype is FeatureType.BBOX or ftype is FeatureType.TIMESTAMPS:
                 parsed_features.append((ftype, None, None))
 
             elif old_name is not None and new_name is not None:
@@ -299,59 +299,59 @@
                     " but the `eopatch` parameter was not provided."
                 )
         return parsed_features
 
 
 def parse_feature(
     feature: SingleFeatureSpec,
-    eopatch: Optional[EOPatch] = None,
-    allowed_feature_types: Union[EllipsisType, Iterable[FeatureType], Callable[[FeatureType], bool]] = ...,
-) -> Tuple[FeatureType, Optional[str]]:
+    eopatch: EOPatch | None = None,
+    allowed_feature_types: EllipsisType | Iterable[FeatureType] | Callable[[FeatureType], bool] = ...,
+) -> tuple[FeatureType, str | None]:
     """Parses input describing a single feature into a `(feature_type, feature_name)` pair.
 
     See :class:`FeatureParser<eolearn.core.utilities.FeatureParser>` for viable inputs.
     """
 
     features = FeatureParser([feature], allowed_feature_types=allowed_feature_types).get_features(eopatch)
     if len(features) != 1:
         raise ValueError(f"Specification {feature} resulted in {len(features)} features, expected 1.")
     return features[0]
 
 
 def parse_renamed_feature(
     feature: SingleFeatureSpec,
-    eopatch: Optional[EOPatch] = None,
-    allowed_feature_types: Union[EllipsisType, Iterable[FeatureType], Callable[[FeatureType], bool]] = ...,
+    eopatch: EOPatch | None = None,
+    allowed_feature_types: EllipsisType | Iterable[FeatureType] | Callable[[FeatureType], bool] = ...,
 ) -> FeatureRenameSpec:
     """Parses input describing a single feature into a `(feature_type, old_name, new_name)` triple.
 
     See :class:`FeatureParser<eolearn.core.utilities.FeatureParser>` for viable inputs.
     """
 
     features = FeatureParser([feature], allowed_feature_types=allowed_feature_types).get_renamed_features(eopatch)
     if len(features) != 1:
         raise ValueError(f"Specification {feature} resulted in {len(features)} features, expected 1.")
     return features[0]
 
 
 def parse_features(
     features: FeaturesSpecification,
-    eopatch: Optional[EOPatch] = None,
-    allowed_feature_types: Union[EllipsisType, Iterable[FeatureType], Callable[[FeatureType], bool]] = ...,
-) -> List[FeatureSpec]:
+    eopatch: EOPatch | None = None,
+    allowed_feature_types: EllipsisType | Iterable[FeatureType] | Callable[[FeatureType], bool] = ...,
+) -> list[FeatureSpec]:
     """Parses input describing features into a list of `(feature_type, feature_name)` pairs.
 
     See :class:`FeatureParser<eolearn.core.utilities.FeatureParser>` for viable inputs.
     """
     return FeatureParser(features, allowed_feature_types=allowed_feature_types).get_features(eopatch)
 
 
 def parse_renamed_features(
     features: FeaturesSpecification,
-    eopatch: Optional[EOPatch] = None,
-    allowed_feature_types: Union[EllipsisType, Iterable[FeatureType], Callable[[FeatureType], bool]] = ...,
-) -> List[FeatureRenameSpec]:
+    eopatch: EOPatch | None = None,
+    allowed_feature_types: EllipsisType | Iterable[FeatureType] | Callable[[FeatureType], bool] = ...,
+) -> list[FeatureRenameSpec]:
     """Parses input describing features into a list of `(feature_type, old_name, new_name)` triples.
 
     See :class:`FeatureParser<eolearn.core.utilities.FeatureParser>` for viable inputs.
     """
     return FeatureParser(features, allowed_feature_types=allowed_feature_types).get_renamed_features(eopatch)
```

### Comparing `eo-learn-core-1.4.1/eolearn/core/utils/raster.py` & `eo-learn-core-1.4.2/eolearn/core/utils/raster.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 Useful utilities for working with raster data, typically `numpy` arrays.
 
 Copyright (c) 2017- Sinergise and contributors
 For the full list of contributors, see the CREDITS file in the root directory of this source tree.
 
 This source code is licensed under the MIT license, see the LICENSE file in the root directory of this source tree.
 """
-from typing import Tuple
+from typing import Literal, Tuple
 
 import numpy as np
-from typing_extensions import Literal
 
 
 def fast_nanpercentile(data: np.ndarray, percentile: float, *, method: str = "linear") -> np.ndarray:
     """This is an alternative implementation of `numpy.nanpercentile`. For cases where the size of the first dimension
     is relatively small compared to the size of the entire array it works much faster than the original.
 
     The algorithm divides pixel data over the first axis into groups by how many NaN values they have. In each group
@@ -53,15 +52,15 @@
             result = np.percentile(chunk, q=percentile, axis=0, **method_kwargs)  # type: ignore[call-overload]
 
         combined_data[mask] = result
 
     return combined_data
 
 
-def constant_pad(
+def constant_pad(  # noqa: C901
     array: np.ndarray,
     multiple_of: Tuple[int, int],
     up_down_rule: Literal["even", "up", "down"] = "even",
     left_right_rule: Literal["even", "left", "right"] = "even",
     pad_value: float = 0,
 ) -> np.ndarray:
     """Function pads an image of shape (rows, columns, channels) with zeros.
```

### Comparing `eo-learn-core-1.4.1/eolearn/core/utils/testing.py` & `eo-learn-core-1.4.2/eolearn/core/utils/testing.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 Copyright (c) 2017- Sinergise and contributors
 For the full list of contributors, see the CREDITS file in the root directory of this source tree.
 
 This source code is licensed under the MIT license, see the LICENSE file in the root directory of this source tree.
 """
 import datetime as dt
+import string
 from dataclasses import dataclass, field
 from typing import Any, List, Optional, Tuple
 
 import geopandas as gpd
 import numpy as np
 import pandas as pd
 from geopandas.testing import assert_geodataframe_equal
@@ -46,26 +47,32 @@
     bbox: BBox = DEFAULT_BBOX,
     timestamps: Optional[List[dt.datetime]] = None,
     seed: int = 42,
     config: Optional[PatchGeneratorConfig] = None,
 ) -> EOPatch:
     """A class for generating EOPatches with dummy data."""
     config = config if config is not None else PatchGeneratorConfig()
-    supported_feature_types = [ftype for ftype in FeatureType if ftype.is_array()]
-    parsed_features = FeatureParser(features or [], supported_feature_types).get_features()
-    rng = np.random.default_rng(seed)
 
+    parsed_features = FeatureParser(
+        features or [], lambda feature_type: feature_type.is_array() or feature_type == FeatureType.META_INFO
+    ).get_features()
+
+    rng = np.random.default_rng(seed)
     timestamps = timestamps if timestamps is not None else config.timestamps
     patch = EOPatch(bbox=bbox, timestamps=timestamps)
 
     # fill eopatch with random data
     # note: the patch generation functionality could be extended by generating extra random features
     for ftype, fname in parsed_features:
-        shape = _get_feature_shape(rng, ftype, timestamps, config)
-        patch[(ftype, fname)] = _generate_feature_data(rng, ftype, shape, config)
+        if ftype == FeatureType.META_INFO:
+            patch[(ftype, fname)] = "".join(rng.choice(list(string.ascii_letters), 20))
+        else:
+            shape = _get_feature_shape(rng, ftype, timestamps, config)
+            patch[(ftype, fname)] = _generate_feature_data(rng, ftype, shape, config)
+
     return patch
 
 
 def _generate_feature_data(
     rng: np.random.Generator, ftype: FeatureType, shape: Tuple[int, ...], config: PatchGeneratorConfig
 ) -> np.ndarray:
     if ftype.is_discrete():
```

### Comparing `eo-learn-core-1.4.1/setup.py` & `eo-learn-core-1.4.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,17 +3,15 @@
 from setuptools import find_packages, setup
 
 
 def get_long_description():
     this_directory = os.path.abspath(os.path.dirname(__file__))
 
     with open(os.path.join(this_directory, "README.md"), encoding="utf-8") as f:
-        long_description = f.read()
-
-    return long_description
+        return f.read()
 
 
 def parse_requirements(file):
     with open(os.path.join(os.path.dirname(__file__), file)) as requirements_file:
         return sorted({line.partition("#")[0].strip() for line in requirements_file} - set(""))
 
 
@@ -25,15 +23,15 @@
                 version = line.split("=")[1].strip()
                 version = version.strip('"').strip("'")
     return version
 
 
 setup(
     name="eo-learn-core",
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     version=get_version(),
     description="Core Machine Learning Framework at Sinergise",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     url="https://github.com/sentinel-hub/eo-learn",
     project_urls={
         "Documentation": "https://eo-learn.readthedocs.io",
@@ -57,16 +55,16 @@
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
         "Operating System :: MacOS",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: Unix",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Scientific/Engineering",
         "Topic :: Scientific/Engineering :: GIS",
         "Topic :: Scientific/Engineering :: Image Processing",
     ],
 )
```

