# Comparing `tmp/mapel-roommates-2.0.3.dev1.tar.gz` & `tmp/mapel-roommates-2.0.3.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapel-roommates-2.0.3.dev1.tar", last modified: Mon Feb 27 20:15:54 2023, max compression
+gzip compressed data, was "mapel-roommates-2.0.3.dev6.tar", last modified: Wed May 24 14:41:08 2023, max compression
```

## Comparing `mapel-roommates-2.0.3.dev1.tar` & `mapel-roommates-2.0.3.dev6.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:15:54.826114 mapel-roommates-2.0.3.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-02-27 20:15:20.000000 mapel-roommates-2.0.3.dev1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-02-27 20:15:54.826114 mapel-roommates-2.0.3.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-02-27 20:15:20.000000 mapel-roommates-2.0.3.dev1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-02-27 20:15:20.000000 mapel-roommates-2.0.3.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-27 20:15:20.000000 mapel-roommates-2.0.3.dev1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-27 20:15:54.826114 mapel-roommates-2.0.3.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:15:54.818114 mapel-roommates-2.0.3.dev1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:15:54.814114 mapel-roommates-2.0.3.dev1/src/mapel/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:15:54.818114 mapel-roommates-2.0.3.dev1/src/mapel/roommates/
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-02-27 20:15:20.000000 mapel-roommates-2.0.3.dev1/src/mapel/roommates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:15:54.822114 mapel-roommates-2.0.3.dev1/src/mapel/roommates/cultures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 20:15:20.000000 mapel-roommates-2.0.3.dev1/src/mapel/roommates/cultures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-02-27 20:15:20.000000 mapel-roommates-2.0.3.dev1/src/mapel/roommates/cultures/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-02-27 20:15:20.000000 mapel-roommates-2.0.3.dev1/src/mapel/roommates/cultures/euclidean.py
--rw-r--r--   0 runner    (1001) docker     (123)    18773 2023-02-27 20:15:20.000000 mapel-roommates-2.0.3.dev1/src/mapel/roommates/cultures/group_separable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-02-27 20:15:20.000000 mapel-roommates-2.0.3.dev1/src/mapel/roommates/cultures/impartial.py
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-02-27 20:15:20.000000 mapel-roommates-2.0.3.dev1/src/mapel/roommates/cultures/mallows.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-02-27 20:15:20.000000 mapel-roommates-2.0.3.dev1/src/mapel/roommates/cultures/urn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-02-27 20:15:20.000000 mapel-roommates-2.0.3.dev1/src/mapel/roommates/cultures_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:15:54.822114 mapel-roommates-2.0.3.dev1/src/mapel/roommates/features/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 20:15:20.000000 mapel-roommates-2.0.3.dev1/src/mapel/roommates/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10144 2023-02-27 20:15:20.000000 mapel-roommates-2.0.3.dev1/src/mapel/roommates/features/basic_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-02-27 20:15:20.000000 mapel-roommates-2.0.3.dev1/src/mapel/roommates/features/distance_to_stability_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-02-27 20:15:20.000000 mapel-roommates-2.0.3.dev1/src/mapel/roommates/features_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:15:54.822114 mapel-roommates-2.0.3.dev1/src/mapel/roommates/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 20:15:20.000000 mapel-roommates-2.0.3.dev1/src/mapel/roommates/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-02-27 20:15:20.000000 mapel-roommates-2.0.3.dev1/src/mapel/roommates/metrics/main_distances.py
--rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-02-27 20:15:20.000000 mapel-roommates-2.0.3.dev1/src/mapel/roommates/metrics_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:15:54.826114 mapel-roommates-2.0.3.dev1/src/mapel/roommates/objects/
--rw-r--r--   0 runner    (1001) docker     (123)     7741 2023-02-27 20:15:20.000000 mapel-roommates-2.0.3.dev1/src/mapel/roommates/objects/Roommates.py
--rw-r--r--   0 runner    (1001) docker     (123)    19818 2023-02-27 20:15:20.000000 mapel-roommates-2.0.3.dev1/src/mapel/roommates/objects/RoommatesExperiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-02-27 20:15:20.000000 mapel-roommates-2.0.3.dev1/src/mapel/roommates/objects/RoommatesFamily.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 20:15:20.000000 mapel-roommates-2.0.3.dev1/src/mapel/roommates/objects/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:15:54.826114 mapel-roommates-2.0.3.dev1/src/mapel_roommates.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-02-27 20:15:54.000000 mapel-roommates-2.0.3.dev1/src/mapel_roommates.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-02-27 20:15:54.000000 mapel-roommates-2.0.3.dev1/src/mapel_roommates.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 20:15:54.000000 mapel-roommates-2.0.3.dev1/src/mapel_roommates.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-27 20:15:54.000000 mapel-roommates-2.0.3.dev1/src/mapel_roommates.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-27 20:15:54.000000 mapel-roommates-2.0.3.dev1/src/mapel_roommates.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:41:08.035508 mapel-roommates-2.0.3.dev6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-24 14:40:30.000000 mapel-roommates-2.0.3.dev6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-24 14:41:08.035508 mapel-roommates-2.0.3.dev6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-24 14:40:30.000000 mapel-roommates-2.0.3.dev6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-24 14:40:30.000000 mapel-roommates-2.0.3.dev6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-24 14:40:30.000000 mapel-roommates-2.0.3.dev6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 14:41:08.035508 mapel-roommates-2.0.3.dev6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:41:08.027508 mapel-roommates-2.0.3.dev6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:41:08.027508 mapel-roommates-2.0.3.dev6/src/mapel/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:41:08.031508 mapel-roommates-2.0.3.dev6/src/mapel/roommates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-24 14:40:30.000000 mapel-roommates-2.0.3.dev6/src/mapel/roommates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:41:08.031508 mapel-roommates-2.0.3.dev6/src/mapel/roommates/cultures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 14:40:30.000000 mapel-roommates-2.0.3.dev6/src/mapel/roommates/cultures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-24 14:40:30.000000 mapel-roommates-2.0.3.dev6/src/mapel/roommates/cultures/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10165 2023-05-24 14:40:30.000000 mapel-roommates-2.0.3.dev6/src/mapel/roommates/cultures/euclidean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18776 2023-05-24 14:40:30.000000 mapel-roommates-2.0.3.dev6/src/mapel/roommates/cultures/group_separable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-05-24 14:40:30.000000 mapel-roommates-2.0.3.dev6/src/mapel/roommates/cultures/impartial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-05-24 14:40:30.000000 mapel-roommates-2.0.3.dev6/src/mapel/roommates/cultures/mallows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-24 14:40:30.000000 mapel-roommates-2.0.3.dev6/src/mapel/roommates/cultures/urn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-05-24 14:40:30.000000 mapel-roommates-2.0.3.dev6/src/mapel/roommates/cultures_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:41:08.031508 mapel-roommates-2.0.3.dev6/src/mapel/roommates/features/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 14:40:30.000000 mapel-roommates-2.0.3.dev6/src/mapel/roommates/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10144 2023-05-24 14:40:30.000000 mapel-roommates-2.0.3.dev6/src/mapel/roommates/features/basic_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-05-24 14:40:30.000000 mapel-roommates-2.0.3.dev6/src/mapel/roommates/features/distance_to_stability_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-05-24 14:40:30.000000 mapel-roommates-2.0.3.dev6/src/mapel/roommates/features_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:41:08.035508 mapel-roommates-2.0.3.dev6/src/mapel/roommates/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 14:40:30.000000 mapel-roommates-2.0.3.dev6/src/mapel/roommates/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-05-24 14:40:30.000000 mapel-roommates-2.0.3.dev6/src/mapel/roommates/metrics/main_distances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-05-24 14:40:30.000000 mapel-roommates-2.0.3.dev6/src/mapel/roommates/metrics_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:41:08.035508 mapel-roommates-2.0.3.dev6/src/mapel/roommates/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)     7735 2023-05-24 14:40:30.000000 mapel-roommates-2.0.3.dev6/src/mapel/roommates/objects/Roommates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19801 2023-05-24 14:40:30.000000 mapel-roommates-2.0.3.dev6/src/mapel/roommates/objects/RoommatesExperiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-24 14:40:30.000000 mapel-roommates-2.0.3.dev6/src/mapel/roommates/objects/RoommatesFamily.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 14:40:30.000000 mapel-roommates-2.0.3.dev6/src/mapel/roommates/objects/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:41:08.035508 mapel-roommates-2.0.3.dev6/src/mapel_roommates.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-24 14:41:08.000000 mapel-roommates-2.0.3.dev6/src/mapel_roommates.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-24 14:41:08.000000 mapel-roommates-2.0.3.dev6/src/mapel_roommates.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 14:41:08.000000 mapel-roommates-2.0.3.dev6/src/mapel_roommates.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-24 14:41:08.000000 mapel-roommates-2.0.3.dev6/src/mapel_roommates.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-24 14:41:08.000000 mapel-roommates-2.0.3.dev6/src/mapel_roommates.egg-info/top_level.txt
```

### Comparing `mapel-roommates-2.0.3.dev1/LICENSE.txt` & `mapel-roommates-2.0.3.dev6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.3.dev1/PKG-INFO` & `mapel-roommates-2.0.3.dev6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapel-roommates
-Version: 2.0.3.dev1
+Version: 2.0.3.dev6
 Summary: Map of Roommates
 Author-email: Stanislaw Szufa <s.szufa@gmail.com>, Niclas Boehmer <niclas.boehmer@tu-berlin.de>
 License: Copyright (c) 2018-2022 Stanislaw Szufa and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `mapel-roommates-2.0.3.dev1/README.md` & `mapel-roommates-2.0.3.dev6/README.md`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.3.dev1/pyproject.toml` & `mapel-roommates-2.0.3.dev6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65", "wheel", "pybind11>=2.6.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mapel-roommates"
-version = "2.0.3.dev1"
+version = "2.0.3.dev6"
 authors = [
  {name = "Stanislaw Szufa", email = "s.szufa@gmail.com"},
  {name = "Niclas Boehmer", email = "niclas.boehmer@tu-berlin.de"},
 ]
 description = "Map of Roommates"
 classifiers=[
     "Programming Language :: Python :: 3",
```

### Comparing `mapel-roommates-2.0.3.dev1/src/mapel/roommates/__init__.py` & `mapel-roommates-2.0.3.dev6/src/mapel/roommates/__init__.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.3.dev1/src/mapel/roommates/cultures/euclidean.py` & `mapel-roommates-2.0.3.dev6/src/mapel/roommates/cultures/euclidean.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     distances = np.zeros([num_agents, num_agents], dtype=float)
     ones = np.ones([params["dim"]], dtype=float)
 
     for v in range(num_agents):
         for c in range(num_agents):
             votes[v][c] = c
             if params["dim"] == 1:
-                distances[v][c] = (1. - agents_skills[c]) * agents_weights[v]
+                distances[v][c] = abs(1. - agents_skills[c]) * agents_weights[v]
             else:
                 distances[v][c] = weighted_l1(ones, agents_skills[c], agents_weights[v])
         votes[v] = [x for _, x in sorted(zip(distances[v], votes[v]))]
 
     return convert(votes)
```

### Comparing `mapel-roommates-2.0.3.dev1/src/mapel/roommates/cultures/group_separable.py` & `mapel-roommates-2.0.3.dev6/src/mapel/roommates/cultures/group_separable.py`

 * *Files 0% similar despite different names*

```diff
@@ -393,15 +393,15 @@
     patterns = ['M0' for _ in range(num_nodes-num_internal_nodes)] + \
                ['M1' for _ in range(num_internal_nodes)]
     np.random.shuffle(patterns)
     return patterns
 
 
 def _generate_tree(num_nodes, num_internal_nodes, patterns):
-    """ Algorithm from: A linear-time algorithm for the generation of trees """
+    """ Algorithm from: A linear-time embedding_id for the generation of trees """
 
     sequence = []
     sizes = []
     larges = []
     ctr = 0
     inner_ctr = 0
     for i, pattern in enumerate(patterns):
```

### Comparing `mapel-roommates-2.0.3.dev1/src/mapel/roommates/cultures/impartial.py` & `mapel-roommates-2.0.3.dev6/src/mapel/roommates/cultures/impartial.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.3.dev1/src/mapel/roommates/cultures/mallows.py` & `mapel-roommates-2.0.3.dev6/src/mapel/roommates/cultures/mallows.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.3.dev1/src/mapel/roommates/cultures/urn.py` & `mapel-roommates-2.0.3.dev6/src/mapel/roommates/cultures/urn.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.3.dev1/src/mapel/roommates/cultures_.py` & `mapel-roommates-2.0.3.dev6/src/mapel/roommates/cultures_.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.3.dev1/src/mapel/roommates/features/basic_features.py` & `mapel-roommates-2.0.3.dev6/src/mapel/roommates/features/basic_features.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.3.dev1/src/mapel/roommates/features/distance_to_stability_features.py` & `mapel-roommates-2.0.3.dev6/src/mapel/roommates/features/distance_to_stability_features.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.3.dev1/src/mapel/roommates/features_.py` & `mapel-roommates-2.0.3.dev6/src/mapel/roommates/features_.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     one_side_values = np.array([])
     election_id_1 = election.instance_id
 
     for election_id_2 in experiment.instances:
         # if election_id_2 in {'identity_10_100_0', 'uniformity_10_100_0',
         #                      'antagonism_10_100_0', 'stratification_10_100_0'}:
         if election_id_1 != election_id_2:
-            # m = experiment.instances[election_id_1].num_candidates
+            # m = election.instances[election_id_1].num_candidates
             # print(election_id_1, election_id_2)
             true_distance = experiment.distances[election_id_1][election_id_2]
             true_distance /= experiment.distances['MD']['MA']
             embedded_distance = l2(np.array(experiment.coordinates[election_id_1]),
                                    np.array(experiment.coordinates[election_id_2]))
 
             embedded_distance /= \
```

### Comparing `mapel-roommates-2.0.3.dev1/src/mapel/roommates/metrics/main_distances.py` & `mapel-roommates-2.0.3.dev6/src/mapel/roommates/metrics/main_distances.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.3.dev1/src/mapel/roommates/metrics_.py` & `mapel-roommates-2.0.3.dev6/src/mapel/roommates/metrics_.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,18 +71,18 @@
             matchings[election_id_1][election_id_2] = matching
             matchings[election_id_2][election_id_1] = np.argsort(matching)
         distances[election_id_1][election_id_2] = distance
         distances[election_id_2][election_id_1] = distances[election_id_1][election_id_2]
         times[election_id_1][election_id_2] = time() - start_time
         times[election_id_2][election_id_1] = times[election_id_1][election_id_2]
 
-    if experiment.store:
+    if experiment.is_exported:
 
         file_name = f'{experiment.distance_id}_p{t}.csv'
-        path = os.path.join(os.getcwd(), "experiments", experiment.experiment_id, "distances",
+        path = os.path.join(os.getcwd(), "election", experiment.experiment_id, "distances",
                             file_name)
 
         with open(path, 'w', newline='') as csv_file:
             writer = csv.writer(csv_file, delimiter=';')
             writer.writerow(
                 ["instance_id_1", "instance_id_2", "distance", "time"])
```

### Comparing `mapel-roommates-2.0.3.dev1/src/mapel/roommates/objects/Roommates.py` & `mapel-roommates-2.0.3.dev6/src/mapel/roommates/objects/Roommates.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,15 +130,15 @@
 
         if store:
             self.store_instance_in_a_file()
 
     def store_instance_in_a_file(self):
         """ Store votes in a file """
 
-        path_to_folder = os.path.join(os.getcwd(), "experiments", self.experiment_id, "instances")
+        path_to_folder = os.path.join(os.getcwd(), "election", self.experiment_id, "instances")
         make_folder_if_do_not_exist(path_to_folder)
         path_to_file = os.path.join(path_to_folder, f'{self.instance_id}.ri')
 
         with open(path_to_file, 'w') as file_:
 
             if self.culture_id in NICE_NAME:
                 file_.write("# " + NICE_NAME[self.culture_id] + " " + str(self.params) + "\n")
@@ -165,15 +165,15 @@
                         file_.write(", ")
                 file_.write("\n")
 
     def import_real_instance(self, shift=False):
         """ Import real ordinal election form .soc file """
 
         file_name = f'{self.instance_id}.ri'
-        path = os.path.join(os.getcwd(), "experiments", self.experiment_id, "instances", file_name)
+        path = os.path.join(os.getcwd(), "election", self.experiment_id, "instances", file_name)
         print(path)
         with open(path, 'r') as my_file:
             params = 0
             first_line = my_file.readline()
 
             if first_line[0] != '#':
                 culture_id = 'empty'
```

### Comparing `mapel-roommates-2.0.3.dev1/src/mapel/roommates/objects/RoommatesExperiment.py` & `mapel-roommates-2.0.3.dev6/src/mapel/roommates/objects/RoommatesExperiment.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,15 +46,15 @@
             self.import_matchings()
         except:
             pass
 
     def import_matchings(self):
         matchings = {}
 
-        path = os.path.join(os.getcwd(), 'experiments', self.experiment_id, 'features',
+        path = os.path.join(os.getcwd(), 'election', self.experiment_id, 'features',
                             'stable_sr.csv')
         with open(path, 'r', newline='') as csv_file:
             reader = csv.DictReader(csv_file, delimiter=';')
 
             for row in reader:
                 election_id = row['instance_id']
                 value = row['matching']
@@ -170,27 +170,27 @@
             process.join()
 
         distances = {instance_id: {} for instance_id in self.instances}
         times = {instance_id: {} for instance_id in self.instances}
         for t in range(num_threads):
 
             file_name = f'{distance_id}_p{t}.csv'
-            path = os.path.join(os.getcwd(), "experiments", self.experiment_id, "distances",
+            path = os.path.join(os.getcwd(), "election", self.experiment_id, "distances",
                                 file_name)
 
             with open(path, 'r', newline='') as csv_file:
                 reader = csv.DictReader(csv_file, delimiter=';')
 
                 for row in reader:
                     distances[row['instance_id_1']][row['instance_id_2']] = float(row['distance'])
                     times[row['instance_id_1']][row['instance_id_2']] = float(row['time'])
 
-        if self.store:
+        if self.is_exported:
 
-            path_to_folder = os.path.join(os.getcwd(), "experiments", self.experiment_id,
+            path_to_folder = os.path.join(os.getcwd(), "election", self.experiment_id,
                                           "distances")
             make_folder_if_do_not_exist(path_to_folder)
             path_to_file = os.path.join(path_to_folder, f'{distance_id}.csv')
 
             with open(path_to_file, 'w', newline='') as csv_file:
                 writer = csv.writer(csv_file, delimiter=';')
                 writer.writerow(
@@ -213,15 +213,15 @@
 
 
     def import_controllers(self):
         """ Import controllers from a file """
 
         families = {}
 
-        path = os.path.join(os.getcwd(), 'experiments', self.experiment_id, 'map.csv')
+        path = os.path.join(os.getcwd(), 'election', self.experiment_id, 'map.csv')
         file_ = open(path, 'r')
 
         header = [h.strip() for h in file_.readline().split(';')]
         reader = csv.DictReader(file_, fieldnames=header, delimiter=';')
 
         starting_from = 0
         for row in reader:
@@ -293,32 +293,32 @@
 
         if self.instances is None:
             self.instances = {}
 
         for family_id in self.families:
 
             new_instances = self.families[family_id].prepare_family(
-                store=self.store,
+                store=self.is_exported,
                 experiment_id=self.experiment_id)
 
             for instance_id in new_instances:
                 self.instances[instance_id] = new_instances[instance_id]
 
     def compute_stable_sr(self):
         for instance_id in self.instances:
             print(instance_id)
             if instance_id in ['roommates_test']:
                 self.matchings[instance_id] = 'None'
             else:
                 usable_matching = basic.compute_stable_SR(self.instances[instance_id].votes)
                 self.matchings[instance_id] = usable_matching
 
-        if self.store:
+        if self.is_exported:
 
-            path_to_folder = os.path.join(os.getcwd(), "experiments", self.experiment_id,
+            path_to_folder = os.path.join(os.getcwd(), "election", self.experiment_id,
                                           "features")
             make_folder_if_do_not_exist(path_to_folder)
             path_to_file = os.path.join(path_to_folder, f'stable_sr.csv')
 
             with open(path_to_file, 'w', newline='') as csv_file:
                 writer = csv.writer(csv_file, delimiter=';')
                 writer.writerow(
@@ -410,29 +410,29 @@
                     #                     'highest_hb_score']:
                     #     value = feature(election, feature_params)
                     #
                     # elif feature_id in {'avg_distortion_from_guardians',
                     #                     'worst_distortion_from_guardians',
                     #                     'distortion_from_all',
                     #                     'distortion_from_top_100'}:
-                    #     value = feature(self, election_id)
+                    #     value = feature(election, election_id)
                     # else:
                     #     value = feature(election)
 
                     if feature_id in features_with_std:
                         feature_dict['value'][instance_id] = value[0]
                         feature_dict['time'][instance_id] = total_time
                         feature_dict['std'][instance_id] = value[1]
                     else:
                         feature_dict['value'][instance_id] = value
                         feature_dict['time'][instance_id] = total_time
 
-        if self.store:
+        if self.is_exported:
 
-            path_to_folder = os.path.join(os.getcwd(), "experiments", self.experiment_id,
+            path_to_folder = os.path.join(os.getcwd(), "election", self.experiment_id,
                                           "features")
             make_folder_if_do_not_exist(path_to_folder)
             path_to_file = os.path.join(path_to_folder, f'{feature_id}.csv')
 
             with open(path_to_file, 'w', newline='') as csv_file:
                 writer = csv.writer(csv_file, delimiter=';')
 
@@ -449,33 +449,33 @@
                                          round(feature_dict['time'][key],3)])
 
         self.features[feature_id] = feature_dict
         return feature_dict
 
     def create_structure(self) -> None:
 
-        if not os.path.isdir("experiments/"):
-            os.mkdir(os.path.join(os.getcwd(), "experiments"))
+        if not os.path.isdir("election/"):
+            os.mkdir(os.path.join(os.getcwd(), "election"))
 
         if not os.path.isdir("images/"):
             os.mkdir(os.path.join(os.getcwd(), "images"))
 
         if not os.path.isdir("trash/"):
             os.mkdir(os.path.join(os.getcwd(), "trash"))
 
         try:
-            os.mkdir(os.path.join(os.getcwd(), "experiments", self.experiment_id))
-            os.mkdir(os.path.join(os.getcwd(), "experiments", self.experiment_id, "distances"))
-            os.mkdir(os.path.join(os.getcwd(), "experiments", self.experiment_id, "features"))
-            os.mkdir(os.path.join(os.getcwd(), "experiments", self.experiment_id, "coordinates"))
-            os.mkdir(os.path.join(os.getcwd(), "experiments", self.experiment_id, "instances"))
-            os.mkdir(os.path.join(os.getcwd(), "experiments", self.experiment_id, "matrices"))
+            os.mkdir(os.path.join(os.getcwd(), "election", self.experiment_id))
+            os.mkdir(os.path.join(os.getcwd(), "election", self.experiment_id, "distances"))
+            os.mkdir(os.path.join(os.getcwd(), "election", self.experiment_id, "features"))
+            os.mkdir(os.path.join(os.getcwd(), "election", self.experiment_id, "coordinates"))
+            os.mkdir(os.path.join(os.getcwd(), "election", self.experiment_id, "instances"))
+            os.mkdir(os.path.join(os.getcwd(), "election", self.experiment_id, "matrices"))
 
             # PREPARE MAP.CSV FILE
-            path = os.path.join(os.getcwd(), "experiments", self.experiment_id, "map.csv")
+            path = os.path.join(os.getcwd(), "election", self.experiment_id, "map.csv")
 
             with open(path, 'w') as file_csv:
                 file_csv.write(
                     "size;num_agents;culture_id;params;color;alpha;family_id;label;marker;show\n")
                 file_csv.write("10;20;roommates_ic;{};black;1;IC;IC;o;t\n")
         except FileExistsError:
             print("Experiment already exists!")
```

### Comparing `mapel-roommates-2.0.3.dev1/src/mapel/roommates/objects/RoommatesFamily.py` & `mapel-roommates-2.0.3.dev6/src/mapel/roommates/objects/RoommatesFamily.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.3.dev1/src/mapel_roommates.egg-info/PKG-INFO` & `mapel-roommates-2.0.3.dev6/src/mapel_roommates.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapel-roommates
-Version: 2.0.3.dev1
+Version: 2.0.3.dev6
 Summary: Map of Roommates
 Author-email: Stanislaw Szufa <s.szufa@gmail.com>, Niclas Boehmer <niclas.boehmer@tu-berlin.de>
 License: Copyright (c) 2018-2022 Stanislaw Szufa and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `mapel-roommates-2.0.3.dev1/src/mapel_roommates.egg-info/SOURCES.txt` & `mapel-roommates-2.0.3.dev6/src/mapel_roommates.egg-info/SOURCES.txt`

 * *Files identical despite different names*

