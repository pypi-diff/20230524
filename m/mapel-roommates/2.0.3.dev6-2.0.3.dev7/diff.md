# Comparing `tmp/mapel-roommates-2.0.3.dev6.tar.gz` & `tmp/mapel-roommates-2.0.3.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapel-roommates-2.0.3.dev6.tar", last modified: Wed May 24 14:41:08 2023, max compression
+gzip compressed data, was "mapel-roommates-2.0.3.dev7.tar", last modified: Wed May 24 17:35:00 2023, max compression
```

## Comparing `mapel-roommates-2.0.3.dev6.tar` & `mapel-roommates-2.0.3.dev7.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:41:08.035508 mapel-roommates-2.0.3.dev6/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-24 14:40:30.000000 mapel-roommates-2.0.3.dev6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-24 14:41:08.035508 mapel-roommates-2.0.3.dev6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-24 14:40:30.000000 mapel-roommates-2.0.3.dev6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-24 14:40:30.000000 mapel-roommates-2.0.3.dev6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-24 14:40:30.000000 mapel-roommates-2.0.3.dev6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 14:41:08.035508 mapel-roommates-2.0.3.dev6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:41:08.027508 mapel-roommates-2.0.3.dev6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:41:08.027508 mapel-roommates-2.0.3.dev6/src/mapel/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:41:08.031508 mapel-roommates-2.0.3.dev6/src/mapel/roommates/
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-24 14:40:30.000000 mapel-roommates-2.0.3.dev6/src/mapel/roommates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:41:08.031508 mapel-roommates-2.0.3.dev6/src/mapel/roommates/cultures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 14:40:30.000000 mapel-roommates-2.0.3.dev6/src/mapel/roommates/cultures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-24 14:40:30.000000 mapel-roommates-2.0.3.dev6/src/mapel/roommates/cultures/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10165 2023-05-24 14:40:30.000000 mapel-roommates-2.0.3.dev6/src/mapel/roommates/cultures/euclidean.py
--rw-r--r--   0 runner    (1001) docker     (123)    18776 2023-05-24 14:40:30.000000 mapel-roommates-2.0.3.dev6/src/mapel/roommates/cultures/group_separable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-05-24 14:40:30.000000 mapel-roommates-2.0.3.dev6/src/mapel/roommates/cultures/impartial.py
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-05-24 14:40:30.000000 mapel-roommates-2.0.3.dev6/src/mapel/roommates/cultures/mallows.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-24 14:40:30.000000 mapel-roommates-2.0.3.dev6/src/mapel/roommates/cultures/urn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-05-24 14:40:30.000000 mapel-roommates-2.0.3.dev6/src/mapel/roommates/cultures_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:41:08.031508 mapel-roommates-2.0.3.dev6/src/mapel/roommates/features/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 14:40:30.000000 mapel-roommates-2.0.3.dev6/src/mapel/roommates/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10144 2023-05-24 14:40:30.000000 mapel-roommates-2.0.3.dev6/src/mapel/roommates/features/basic_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-05-24 14:40:30.000000 mapel-roommates-2.0.3.dev6/src/mapel/roommates/features/distance_to_stability_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-05-24 14:40:30.000000 mapel-roommates-2.0.3.dev6/src/mapel/roommates/features_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:41:08.035508 mapel-roommates-2.0.3.dev6/src/mapel/roommates/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 14:40:30.000000 mapel-roommates-2.0.3.dev6/src/mapel/roommates/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-05-24 14:40:30.000000 mapel-roommates-2.0.3.dev6/src/mapel/roommates/metrics/main_distances.py
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-05-24 14:40:30.000000 mapel-roommates-2.0.3.dev6/src/mapel/roommates/metrics_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:41:08.035508 mapel-roommates-2.0.3.dev6/src/mapel/roommates/objects/
--rw-r--r--   0 runner    (1001) docker     (123)     7735 2023-05-24 14:40:30.000000 mapel-roommates-2.0.3.dev6/src/mapel/roommates/objects/Roommates.py
--rw-r--r--   0 runner    (1001) docker     (123)    19801 2023-05-24 14:40:30.000000 mapel-roommates-2.0.3.dev6/src/mapel/roommates/objects/RoommatesExperiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-24 14:40:30.000000 mapel-roommates-2.0.3.dev6/src/mapel/roommates/objects/RoommatesFamily.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 14:40:30.000000 mapel-roommates-2.0.3.dev6/src/mapel/roommates/objects/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:41:08.035508 mapel-roommates-2.0.3.dev6/src/mapel_roommates.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-24 14:41:08.000000 mapel-roommates-2.0.3.dev6/src/mapel_roommates.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-24 14:41:08.000000 mapel-roommates-2.0.3.dev6/src/mapel_roommates.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 14:41:08.000000 mapel-roommates-2.0.3.dev6/src/mapel_roommates.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-24 14:41:08.000000 mapel-roommates-2.0.3.dev6/src/mapel_roommates.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-24 14:41:08.000000 mapel-roommates-2.0.3.dev6/src/mapel_roommates.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:35:00.588660 mapel-roommates-2.0.3.dev7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-24 17:34:29.000000 mapel-roommates-2.0.3.dev7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-24 17:35:00.588660 mapel-roommates-2.0.3.dev7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-24 17:34:29.000000 mapel-roommates-2.0.3.dev7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-24 17:34:29.000000 mapel-roommates-2.0.3.dev7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-24 17:34:29.000000 mapel-roommates-2.0.3.dev7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 17:35:00.588660 mapel-roommates-2.0.3.dev7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:35:00.584660 mapel-roommates-2.0.3.dev7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:35:00.584660 mapel-roommates-2.0.3.dev7/src/mapel/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:35:00.588660 mapel-roommates-2.0.3.dev7/src/mapel/roommates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-24 17:34:29.000000 mapel-roommates-2.0.3.dev7/src/mapel/roommates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:35:00.588660 mapel-roommates-2.0.3.dev7/src/mapel/roommates/cultures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:34:29.000000 mapel-roommates-2.0.3.dev7/src/mapel/roommates/cultures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-24 17:34:29.000000 mapel-roommates-2.0.3.dev7/src/mapel/roommates/cultures/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10165 2023-05-24 17:34:29.000000 mapel-roommates-2.0.3.dev7/src/mapel/roommates/cultures/euclidean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18776 2023-05-24 17:34:29.000000 mapel-roommates-2.0.3.dev7/src/mapel/roommates/cultures/group_separable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-05-24 17:34:29.000000 mapel-roommates-2.0.3.dev7/src/mapel/roommates/cultures/impartial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-05-24 17:34:29.000000 mapel-roommates-2.0.3.dev7/src/mapel/roommates/cultures/mallows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-24 17:34:29.000000 mapel-roommates-2.0.3.dev7/src/mapel/roommates/cultures/urn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-05-24 17:34:29.000000 mapel-roommates-2.0.3.dev7/src/mapel/roommates/cultures_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:35:00.588660 mapel-roommates-2.0.3.dev7/src/mapel/roommates/features/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:34:29.000000 mapel-roommates-2.0.3.dev7/src/mapel/roommates/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10144 2023-05-24 17:34:29.000000 mapel-roommates-2.0.3.dev7/src/mapel/roommates/features/basic_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-05-24 17:34:29.000000 mapel-roommates-2.0.3.dev7/src/mapel/roommates/features/distance_to_stability_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-05-24 17:34:29.000000 mapel-roommates-2.0.3.dev7/src/mapel/roommates/features_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:35:00.588660 mapel-roommates-2.0.3.dev7/src/mapel/roommates/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:34:29.000000 mapel-roommates-2.0.3.dev7/src/mapel/roommates/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-05-24 17:34:29.000000 mapel-roommates-2.0.3.dev7/src/mapel/roommates/metrics/main_distances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-05-24 17:34:29.000000 mapel-roommates-2.0.3.dev7/src/mapel/roommates/metrics_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:35:00.588660 mapel-roommates-2.0.3.dev7/src/mapel/roommates/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)     7735 2023-05-24 17:34:29.000000 mapel-roommates-2.0.3.dev7/src/mapel/roommates/objects/Roommates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19801 2023-05-24 17:34:29.000000 mapel-roommates-2.0.3.dev7/src/mapel/roommates/objects/RoommatesExperiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-24 17:34:29.000000 mapel-roommates-2.0.3.dev7/src/mapel/roommates/objects/RoommatesFamily.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:34:29.000000 mapel-roommates-2.0.3.dev7/src/mapel/roommates/objects/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:35:00.588660 mapel-roommates-2.0.3.dev7/src/mapel_roommates.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-24 17:35:00.000000 mapel-roommates-2.0.3.dev7/src/mapel_roommates.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-24 17:35:00.000000 mapel-roommates-2.0.3.dev7/src/mapel_roommates.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 17:35:00.000000 mapel-roommates-2.0.3.dev7/src/mapel_roommates.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-24 17:35:00.000000 mapel-roommates-2.0.3.dev7/src/mapel_roommates.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-24 17:35:00.000000 mapel-roommates-2.0.3.dev7/src/mapel_roommates.egg-info/top_level.txt
```

### Comparing `mapel-roommates-2.0.3.dev6/LICENSE.txt` & `mapel-roommates-2.0.3.dev7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.3.dev6/PKG-INFO` & `mapel-roommates-2.0.3.dev7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapel-roommates
-Version: 2.0.3.dev6
+Version: 2.0.3.dev7
 Summary: Map of Roommates
 Author-email: Stanislaw Szufa <s.szufa@gmail.com>, Niclas Boehmer <niclas.boehmer@tu-berlin.de>
 License: Copyright (c) 2018-2022 Stanislaw Szufa and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `mapel-roommates-2.0.3.dev6/README.md` & `mapel-roommates-2.0.3.dev7/README.md`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.3.dev6/pyproject.toml` & `mapel-roommates-2.0.3.dev7/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65", "wheel", "pybind11>=2.6.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mapel-roommates"
-version = "2.0.3.dev6"
+version = "2.0.3.dev7"
 authors = [
  {name = "Stanislaw Szufa", email = "s.szufa@gmail.com"},
  {name = "Niclas Boehmer", email = "niclas.boehmer@tu-berlin.de"},
 ]
 description = "Map of Roommates"
 classifiers=[
     "Programming Language :: Python :: 3",
```

### Comparing `mapel-roommates-2.0.3.dev6/src/mapel/roommates/__init__.py` & `mapel-roommates-2.0.3.dev7/src/mapel/roommates/__init__.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.3.dev6/src/mapel/roommates/cultures/euclidean.py` & `mapel-roommates-2.0.3.dev7/src/mapel/roommates/cultures/euclidean.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.3.dev6/src/mapel/roommates/cultures/group_separable.py` & `mapel-roommates-2.0.3.dev7/src/mapel/roommates/cultures/group_separable.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.3.dev6/src/mapel/roommates/cultures/impartial.py` & `mapel-roommates-2.0.3.dev7/src/mapel/roommates/cultures/impartial.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.3.dev6/src/mapel/roommates/cultures/mallows.py` & `mapel-roommates-2.0.3.dev7/src/mapel/roommates/cultures/mallows.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.3.dev6/src/mapel/roommates/cultures/urn.py` & `mapel-roommates-2.0.3.dev7/src/mapel/roommates/cultures/urn.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.3.dev6/src/mapel/roommates/cultures_.py` & `mapel-roommates-2.0.3.dev7/src/mapel/roommates/cultures_.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.3.dev6/src/mapel/roommates/features/basic_features.py` & `mapel-roommates-2.0.3.dev7/src/mapel/roommates/features/basic_features.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.3.dev6/src/mapel/roommates/features/distance_to_stability_features.py` & `mapel-roommates-2.0.3.dev7/src/mapel/roommates/features/distance_to_stability_features.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.3.dev6/src/mapel/roommates/features_.py` & `mapel-roommates-2.0.3.dev7/src/mapel/roommates/features_.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.3.dev6/src/mapel/roommates/metrics/main_distances.py` & `mapel-roommates-2.0.3.dev7/src/mapel/roommates/metrics/main_distances.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.3.dev6/src/mapel/roommates/metrics_.py` & `mapel-roommates-2.0.3.dev7/src/mapel/roommates/metrics_.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.3.dev6/src/mapel/roommates/objects/Roommates.py` & `mapel-roommates-2.0.3.dev7/src/mapel/roommates/objects/Roommates.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.3.dev6/src/mapel/roommates/objects/RoommatesExperiment.py` & `mapel-roommates-2.0.3.dev7/src/mapel/roommates/objects/RoommatesExperiment.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.3.dev6/src/mapel/roommates/objects/RoommatesFamily.py` & `mapel-roommates-2.0.3.dev7/src/mapel/roommates/objects/RoommatesFamily.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.3.dev6/src/mapel_roommates.egg-info/PKG-INFO` & `mapel-roommates-2.0.3.dev7/src/mapel_roommates.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapel-roommates
-Version: 2.0.3.dev6
+Version: 2.0.3.dev7
 Summary: Map of Roommates
 Author-email: Stanislaw Szufa <s.szufa@gmail.com>, Niclas Boehmer <niclas.boehmer@tu-berlin.de>
 License: Copyright (c) 2018-2022 Stanislaw Szufa and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `mapel-roommates-2.0.3.dev6/src/mapel_roommates.egg-info/SOURCES.txt` & `mapel-roommates-2.0.3.dev7/src/mapel_roommates.egg-info/SOURCES.txt`

 * *Files identical despite different names*

