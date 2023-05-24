# Comparing `tmp/mapel-marriages-2.0.3.dev6.tar.gz` & `tmp/mapel-marriages-2.0.3.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapel-marriages-2.0.3.dev6.tar", last modified: Wed May 24 14:41:16 2023, max compression
+gzip compressed data, was "mapel-marriages-2.0.3.dev7.tar", last modified: Wed May 24 17:35:07 2023, max compression
```

## Comparing `mapel-marriages-2.0.3.dev6.tar` & `mapel-marriages-2.0.3.dev7.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:41:16.091515 mapel-marriages-2.0.3.dev6/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-24 14:40:30.000000 mapel-marriages-2.0.3.dev6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-05-24 14:41:16.091515 mapel-marriages-2.0.3.dev6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-24 14:40:30.000000 mapel-marriages-2.0.3.dev6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-24 14:40:30.000000 mapel-marriages-2.0.3.dev6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-24 14:40:30.000000 mapel-marriages-2.0.3.dev6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 14:41:16.091515 mapel-marriages-2.0.3.dev6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:41:16.075515 mapel-marriages-2.0.3.dev6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:41:16.075515 mapel-marriages-2.0.3.dev6/src/mapel/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:41:16.079516 mapel-marriages-2.0.3.dev6/src/mapel/marriages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 14:40:30.000000 mapel-marriages-2.0.3.dev6/src/mapel/marriages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:41:16.083516 mapel-marriages-2.0.3.dev6/src/mapel/marriages/cultures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 14:40:30.000000 mapel-marriages-2.0.3.dev6/src/mapel/marriages/cultures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-24 14:40:30.000000 mapel-marriages-2.0.3.dev6/src/mapel/marriages/cultures/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16557 2023-05-24 14:40:30.000000 mapel-marriages-2.0.3.dev6/src/mapel/marriages/cultures/euclidean.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-05-24 14:40:30.000000 mapel-marriages-2.0.3.dev6/src/mapel/marriages/cultures/impartial.py
--rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-05-24 14:40:30.000000 mapel-marriages-2.0.3.dev6/src/mapel/marriages/cultures/mallows.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-24 14:40:30.000000 mapel-marriages-2.0.3.dev6/src/mapel/marriages/cultures/urn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-05-24 14:40:30.000000 mapel-marriages-2.0.3.dev6/src/mapel/marriages/cultures_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:41:16.083516 mapel-marriages-2.0.3.dev6/src/mapel/marriages/features/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 14:40:30.000000 mapel-marriages-2.0.3.dev6/src/mapel/marriages/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9917 2023-05-24 14:40:30.000000 mapel-marriages-2.0.3.dev6/src/mapel/marriages/features/basic_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-05-24 14:40:30.000000 mapel-marriages-2.0.3.dev6/src/mapel/marriages/features/distance_to_stability_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-05-24 14:40:30.000000 mapel-marriages-2.0.3.dev6/src/mapel/marriages/features/experiments_marriage.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-24 14:40:30.000000 mapel-marriages-2.0.3.dev6/src/mapel/marriages/features_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:41:16.087515 mapel-marriages-2.0.3.dev6/src/mapel/marriages/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 14:40:30.000000 mapel-marriages-2.0.3.dev6/src/mapel/marriages/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-05-24 14:40:30.000000 mapel-marriages-2.0.3.dev6/src/mapel/marriages/metrics/main_marriages_distances.py
--rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-05-24 14:40:30.000000 mapel-marriages-2.0.3.dev6/src/mapel/marriages/metrics_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:41:16.087515 mapel-marriages-2.0.3.dev6/src/mapel/marriages/objects/
--rw-r--r--   0 runner    (1001) docker     (123)     7927 2023-05-24 14:40:30.000000 mapel-marriages-2.0.3.dev6/src/mapel/marriages/objects/Marriages.py
--rw-r--r--   0 runner    (1001) docker     (123)    16617 2023-05-24 14:40:30.000000 mapel-marriages-2.0.3.dev6/src/mapel/marriages/objects/MarriagesExperiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-05-24 14:40:30.000000 mapel-marriages-2.0.3.dev6/src/mapel/marriages/objects/MarriagesFamily.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 14:40:30.000000 mapel-marriages-2.0.3.dev6/src/mapel/marriages/objects/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:41:16.091515 mapel-marriages-2.0.3.dev6/src/mapel_marriages.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-05-24 14:41:16.000000 mapel-marriages-2.0.3.dev6/src/mapel_marriages.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-24 14:41:16.000000 mapel-marriages-2.0.3.dev6/src/mapel_marriages.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 14:41:16.000000 mapel-marriages-2.0.3.dev6/src/mapel_marriages.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-24 14:41:16.000000 mapel-marriages-2.0.3.dev6/src/mapel_marriages.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-24 14:41:16.000000 mapel-marriages-2.0.3.dev6/src/mapel_marriages.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:35:07.264675 mapel-marriages-2.0.3.dev7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-24 17:34:29.000000 mapel-marriages-2.0.3.dev7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-05-24 17:35:07.264675 mapel-marriages-2.0.3.dev7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-24 17:34:29.000000 mapel-marriages-2.0.3.dev7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-24 17:34:29.000000 mapel-marriages-2.0.3.dev7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-24 17:34:29.000000 mapel-marriages-2.0.3.dev7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 17:35:07.264675 mapel-marriages-2.0.3.dev7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:35:07.260675 mapel-marriages-2.0.3.dev7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:35:07.260675 mapel-marriages-2.0.3.dev7/src/mapel/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:35:07.260675 mapel-marriages-2.0.3.dev7/src/mapel/marriages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:34:29.000000 mapel-marriages-2.0.3.dev7/src/mapel/marriages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:35:07.260675 mapel-marriages-2.0.3.dev7/src/mapel/marriages/cultures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:34:29.000000 mapel-marriages-2.0.3.dev7/src/mapel/marriages/cultures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-24 17:34:29.000000 mapel-marriages-2.0.3.dev7/src/mapel/marriages/cultures/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16557 2023-05-24 17:34:29.000000 mapel-marriages-2.0.3.dev7/src/mapel/marriages/cultures/euclidean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-05-24 17:34:29.000000 mapel-marriages-2.0.3.dev7/src/mapel/marriages/cultures/impartial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-05-24 17:34:29.000000 mapel-marriages-2.0.3.dev7/src/mapel/marriages/cultures/mallows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-24 17:34:29.000000 mapel-marriages-2.0.3.dev7/src/mapel/marriages/cultures/urn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-05-24 17:34:29.000000 mapel-marriages-2.0.3.dev7/src/mapel/marriages/cultures_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:35:07.264675 mapel-marriages-2.0.3.dev7/src/mapel/marriages/features/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:34:29.000000 mapel-marriages-2.0.3.dev7/src/mapel/marriages/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9917 2023-05-24 17:34:29.000000 mapel-marriages-2.0.3.dev7/src/mapel/marriages/features/basic_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-05-24 17:34:29.000000 mapel-marriages-2.0.3.dev7/src/mapel/marriages/features/distance_to_stability_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-05-24 17:34:29.000000 mapel-marriages-2.0.3.dev7/src/mapel/marriages/features/experiments_marriage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-24 17:34:29.000000 mapel-marriages-2.0.3.dev7/src/mapel/marriages/features_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:35:07.264675 mapel-marriages-2.0.3.dev7/src/mapel/marriages/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:34:29.000000 mapel-marriages-2.0.3.dev7/src/mapel/marriages/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-05-24 17:34:29.000000 mapel-marriages-2.0.3.dev7/src/mapel/marriages/metrics/main_marriages_distances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-05-24 17:34:29.000000 mapel-marriages-2.0.3.dev7/src/mapel/marriages/metrics_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:35:07.264675 mapel-marriages-2.0.3.dev7/src/mapel/marriages/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)     7927 2023-05-24 17:34:29.000000 mapel-marriages-2.0.3.dev7/src/mapel/marriages/objects/Marriages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16617 2023-05-24 17:34:29.000000 mapel-marriages-2.0.3.dev7/src/mapel/marriages/objects/MarriagesExperiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-05-24 17:34:29.000000 mapel-marriages-2.0.3.dev7/src/mapel/marriages/objects/MarriagesFamily.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:34:29.000000 mapel-marriages-2.0.3.dev7/src/mapel/marriages/objects/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:35:07.264675 mapel-marriages-2.0.3.dev7/src/mapel_marriages.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-05-24 17:35:07.000000 mapel-marriages-2.0.3.dev7/src/mapel_marriages.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-24 17:35:07.000000 mapel-marriages-2.0.3.dev7/src/mapel_marriages.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 17:35:07.000000 mapel-marriages-2.0.3.dev7/src/mapel_marriages.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-24 17:35:07.000000 mapel-marriages-2.0.3.dev7/src/mapel_marriages.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-24 17:35:07.000000 mapel-marriages-2.0.3.dev7/src/mapel_marriages.egg-info/top_level.txt
```

### Comparing `mapel-marriages-2.0.3.dev6/LICENSE.txt` & `mapel-marriages-2.0.3.dev7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.0.3.dev6/PKG-INFO` & `mapel-marriages-2.0.3.dev7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapel-marriages
-Version: 2.0.3.dev6
+Version: 2.0.3.dev7
 Summary: Map of Marriages
 Author-email: Stanislaw Szufa <s.szufa@gmail.com>, Niclas Boehmer <niclas.boehmer@tu-berlin.de>
 License: Copyright (c) 2018-2022 Stanislaw Szufa and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `mapel-marriages-2.0.3.dev6/README.md` & `mapel-marriages-2.0.3.dev7/README.md`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.0.3.dev6/pyproject.toml` & `mapel-marriages-2.0.3.dev7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65", "wheel", "pybind11>=2.6.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mapel-marriages"
-version = "2.0.3.dev6"
+version = "2.0.3.dev7"
 authors = [
  {name = "Stanislaw Szufa", email = "s.szufa@gmail.com"},
  {name = "Niclas Boehmer", email = "niclas.boehmer@tu-berlin.de"},
 ]
 description = "Map of Marriages"
 classifiers=[
     "Programming Language :: Python :: 3",
```

### Comparing `mapel-marriages-2.0.3.dev6/src/mapel/marriages/cultures/euclidean.py` & `mapel-marriages-2.0.3.dev7/src/mapel/marriages/cultures/euclidean.py`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.0.3.dev6/src/mapel/marriages/cultures/impartial.py` & `mapel-marriages-2.0.3.dev7/src/mapel/marriages/cultures/impartial.py`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.0.3.dev6/src/mapel/marriages/cultures/mallows.py` & `mapel-marriages-2.0.3.dev7/src/mapel/marriages/cultures/mallows.py`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.0.3.dev6/src/mapel/marriages/cultures/urn.py` & `mapel-marriages-2.0.3.dev7/src/mapel/marriages/cultures/urn.py`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.0.3.dev6/src/mapel/marriages/cultures_.py` & `mapel-marriages-2.0.3.dev7/src/mapel/marriages/cultures_.py`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.0.3.dev6/src/mapel/marriages/features/basic_features.py` & `mapel-marriages-2.0.3.dev7/src/mapel/marriages/features/basic_features.py`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.0.3.dev6/src/mapel/marriages/features/distance_to_stability_features.py` & `mapel-marriages-2.0.3.dev7/src/mapel/marriages/features/distance_to_stability_features.py`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.0.3.dev6/src/mapel/marriages/features/experiments_marriage.py` & `mapel-marriages-2.0.3.dev7/src/mapel/marriages/features/experiments_marriage.py`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.0.3.dev6/src/mapel/marriages/features_.py` & `mapel-marriages-2.0.3.dev7/src/mapel/marriages/features_.py`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.0.3.dev6/src/mapel/marriages/metrics/main_marriages_distances.py` & `mapel-marriages-2.0.3.dev7/src/mapel/marriages/metrics/main_marriages_distances.py`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.0.3.dev6/src/mapel/marriages/metrics_.py` & `mapel-marriages-2.0.3.dev7/src/mapel/marriages/metrics_.py`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.0.3.dev6/src/mapel/marriages/objects/Marriages.py` & `mapel-marriages-2.0.3.dev7/src/mapel/marriages/objects/Marriages.py`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.0.3.dev6/src/mapel/marriages/objects/MarriagesExperiment.py` & `mapel-marriages-2.0.3.dev7/src/mapel/marriages/objects/MarriagesExperiment.py`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.0.3.dev6/src/mapel/marriages/objects/MarriagesFamily.py` & `mapel-marriages-2.0.3.dev7/src/mapel/marriages/objects/MarriagesFamily.py`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.0.3.dev6/src/mapel_marriages.egg-info/PKG-INFO` & `mapel-marriages-2.0.3.dev7/src/mapel_marriages.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapel-marriages
-Version: 2.0.3.dev6
+Version: 2.0.3.dev7
 Summary: Map of Marriages
 Author-email: Stanislaw Szufa <s.szufa@gmail.com>, Niclas Boehmer <niclas.boehmer@tu-berlin.de>
 License: Copyright (c) 2018-2022 Stanislaw Szufa and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `mapel-marriages-2.0.3.dev6/src/mapel_marriages.egg-info/SOURCES.txt` & `mapel-marriages-2.0.3.dev7/src/mapel_marriages.egg-info/SOURCES.txt`

 * *Files identical despite different names*

