# Comparing `tmp/mapel-marriages-2.0.3.dev1.tar.gz` & `tmp/mapel-marriages-2.0.3.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapel-marriages-2.0.3.dev1.tar", last modified: Mon Feb 27 20:16:02 2023, max compression
+gzip compressed data, was "mapel-marriages-2.0.3.dev6.tar", last modified: Wed May 24 14:41:16 2023, max compression
```

## Comparing `mapel-marriages-2.0.3.dev1.tar` & `mapel-marriages-2.0.3.dev6.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:16:02.654163 mapel-marriages-2.0.3.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-02-27 20:15:20.000000 mapel-marriages-2.0.3.dev1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-02-27 20:16:02.654163 mapel-marriages-2.0.3.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-02-27 20:15:20.000000 mapel-marriages-2.0.3.dev1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-02-27 20:15:20.000000 mapel-marriages-2.0.3.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-27 20:15:20.000000 mapel-marriages-2.0.3.dev1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-27 20:16:02.654163 mapel-marriages-2.0.3.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:16:02.646162 mapel-marriages-2.0.3.dev1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:16:02.646162 mapel-marriages-2.0.3.dev1/src/mapel/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:16:02.650163 mapel-marriages-2.0.3.dev1/src/mapel/marriages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 20:15:20.000000 mapel-marriages-2.0.3.dev1/src/mapel/marriages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:16:02.650163 mapel-marriages-2.0.3.dev1/src/mapel/marriages/cultures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 20:15:20.000000 mapel-marriages-2.0.3.dev1/src/mapel/marriages/cultures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-02-27 20:15:20.000000 mapel-marriages-2.0.3.dev1/src/mapel/marriages/cultures/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16557 2023-02-27 20:15:20.000000 mapel-marriages-2.0.3.dev1/src/mapel/marriages/cultures/euclidean.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-02-27 20:15:20.000000 mapel-marriages-2.0.3.dev1/src/mapel/marriages/cultures/impartial.py
--rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-02-27 20:15:20.000000 mapel-marriages-2.0.3.dev1/src/mapel/marriages/cultures/mallows.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-02-27 20:15:20.000000 mapel-marriages-2.0.3.dev1/src/mapel/marriages/cultures/urn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-02-27 20:15:20.000000 mapel-marriages-2.0.3.dev1/src/mapel/marriages/cultures_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:16:02.650163 mapel-marriages-2.0.3.dev1/src/mapel/marriages/features/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 20:15:20.000000 mapel-marriages-2.0.3.dev1/src/mapel/marriages/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9917 2023-02-27 20:15:20.000000 mapel-marriages-2.0.3.dev1/src/mapel/marriages/features/basic_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-02-27 20:15:20.000000 mapel-marriages-2.0.3.dev1/src/mapel/marriages/features/distance_to_stability_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-02-27 20:15:20.000000 mapel-marriages-2.0.3.dev1/src/mapel/marriages/features/experiments_marriage.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-02-27 20:15:20.000000 mapel-marriages-2.0.3.dev1/src/mapel/marriages/features_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:16:02.650163 mapel-marriages-2.0.3.dev1/src/mapel/marriages/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 20:15:20.000000 mapel-marriages-2.0.3.dev1/src/mapel/marriages/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-02-27 20:15:20.000000 mapel-marriages-2.0.3.dev1/src/mapel/marriages/metrics/main_marriages_distances.py
--rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-02-27 20:15:20.000000 mapel-marriages-2.0.3.dev1/src/mapel/marriages/metrics_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:16:02.650163 mapel-marriages-2.0.3.dev1/src/mapel/marriages/objects/
--rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-02-27 20:15:20.000000 mapel-marriages-2.0.3.dev1/src/mapel/marriages/objects/Marriages.py
--rw-r--r--   0 runner    (1001) docker     (123)    16616 2023-02-27 20:15:20.000000 mapel-marriages-2.0.3.dev1/src/mapel/marriages/objects/MarriagesExperiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-02-27 20:15:20.000000 mapel-marriages-2.0.3.dev1/src/mapel/marriages/objects/MarriagesFamily.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 20:15:20.000000 mapel-marriages-2.0.3.dev1/src/mapel/marriages/objects/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:16:02.654163 mapel-marriages-2.0.3.dev1/src/mapel_marriages.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-02-27 20:16:02.000000 mapel-marriages-2.0.3.dev1/src/mapel_marriages.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-02-27 20:16:02.000000 mapel-marriages-2.0.3.dev1/src/mapel_marriages.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 20:16:02.000000 mapel-marriages-2.0.3.dev1/src/mapel_marriages.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-27 20:16:02.000000 mapel-marriages-2.0.3.dev1/src/mapel_marriages.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-27 20:16:02.000000 mapel-marriages-2.0.3.dev1/src/mapel_marriages.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:41:16.091515 mapel-marriages-2.0.3.dev6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-24 14:40:30.000000 mapel-marriages-2.0.3.dev6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-05-24 14:41:16.091515 mapel-marriages-2.0.3.dev6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-24 14:40:30.000000 mapel-marriages-2.0.3.dev6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-24 14:40:30.000000 mapel-marriages-2.0.3.dev6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-24 14:40:30.000000 mapel-marriages-2.0.3.dev6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 14:41:16.091515 mapel-marriages-2.0.3.dev6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:41:16.075515 mapel-marriages-2.0.3.dev6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:41:16.075515 mapel-marriages-2.0.3.dev6/src/mapel/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:41:16.079516 mapel-marriages-2.0.3.dev6/src/mapel/marriages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 14:40:30.000000 mapel-marriages-2.0.3.dev6/src/mapel/marriages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:41:16.083516 mapel-marriages-2.0.3.dev6/src/mapel/marriages/cultures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 14:40:30.000000 mapel-marriages-2.0.3.dev6/src/mapel/marriages/cultures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-24 14:40:30.000000 mapel-marriages-2.0.3.dev6/src/mapel/marriages/cultures/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16557 2023-05-24 14:40:30.000000 mapel-marriages-2.0.3.dev6/src/mapel/marriages/cultures/euclidean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-05-24 14:40:30.000000 mapel-marriages-2.0.3.dev6/src/mapel/marriages/cultures/impartial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-05-24 14:40:30.000000 mapel-marriages-2.0.3.dev6/src/mapel/marriages/cultures/mallows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-24 14:40:30.000000 mapel-marriages-2.0.3.dev6/src/mapel/marriages/cultures/urn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-05-24 14:40:30.000000 mapel-marriages-2.0.3.dev6/src/mapel/marriages/cultures_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:41:16.083516 mapel-marriages-2.0.3.dev6/src/mapel/marriages/features/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 14:40:30.000000 mapel-marriages-2.0.3.dev6/src/mapel/marriages/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9917 2023-05-24 14:40:30.000000 mapel-marriages-2.0.3.dev6/src/mapel/marriages/features/basic_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-05-24 14:40:30.000000 mapel-marriages-2.0.3.dev6/src/mapel/marriages/features/distance_to_stability_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-05-24 14:40:30.000000 mapel-marriages-2.0.3.dev6/src/mapel/marriages/features/experiments_marriage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-24 14:40:30.000000 mapel-marriages-2.0.3.dev6/src/mapel/marriages/features_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:41:16.087515 mapel-marriages-2.0.3.dev6/src/mapel/marriages/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 14:40:30.000000 mapel-marriages-2.0.3.dev6/src/mapel/marriages/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-05-24 14:40:30.000000 mapel-marriages-2.0.3.dev6/src/mapel/marriages/metrics/main_marriages_distances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-05-24 14:40:30.000000 mapel-marriages-2.0.3.dev6/src/mapel/marriages/metrics_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:41:16.087515 mapel-marriages-2.0.3.dev6/src/mapel/marriages/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)     7927 2023-05-24 14:40:30.000000 mapel-marriages-2.0.3.dev6/src/mapel/marriages/objects/Marriages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16617 2023-05-24 14:40:30.000000 mapel-marriages-2.0.3.dev6/src/mapel/marriages/objects/MarriagesExperiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-05-24 14:40:30.000000 mapel-marriages-2.0.3.dev6/src/mapel/marriages/objects/MarriagesFamily.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 14:40:30.000000 mapel-marriages-2.0.3.dev6/src/mapel/marriages/objects/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:41:16.091515 mapel-marriages-2.0.3.dev6/src/mapel_marriages.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-05-24 14:41:16.000000 mapel-marriages-2.0.3.dev6/src/mapel_marriages.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-24 14:41:16.000000 mapel-marriages-2.0.3.dev6/src/mapel_marriages.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 14:41:16.000000 mapel-marriages-2.0.3.dev6/src/mapel_marriages.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-24 14:41:16.000000 mapel-marriages-2.0.3.dev6/src/mapel_marriages.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-24 14:41:16.000000 mapel-marriages-2.0.3.dev6/src/mapel_marriages.egg-info/top_level.txt
```

### Comparing `mapel-marriages-2.0.3.dev1/LICENSE.txt` & `mapel-marriages-2.0.3.dev6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.0.3.dev1/PKG-INFO` & `mapel-marriages-2.0.3.dev6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapel-marriages
-Version: 2.0.3.dev1
+Version: 2.0.3.dev6
 Summary: Map of Marriages
 Author-email: Stanislaw Szufa <s.szufa@gmail.com>, Niclas Boehmer <niclas.boehmer@tu-berlin.de>
 License: Copyright (c) 2018-2022 Stanislaw Szufa and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `mapel-marriages-2.0.3.dev1/README.md` & `mapel-marriages-2.0.3.dev6/README.md`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.0.3.dev1/pyproject.toml` & `mapel-marriages-2.0.3.dev6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65", "wheel", "pybind11>=2.6.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mapel-marriages"
-version = "2.0.3.dev1"
+version = "2.0.3.dev6"
 authors = [
  {name = "Stanislaw Szufa", email = "s.szufa@gmail.com"},
  {name = "Niclas Boehmer", email = "niclas.boehmer@tu-berlin.de"},
 ]
 description = "Map of Marriages"
 classifiers=[
     "Programming Language :: Python :: 3",
```

### Comparing `mapel-marriages-2.0.3.dev1/src/mapel/marriages/cultures/euclidean.py` & `mapel-marriages-2.0.3.dev6/src/mapel/marriages/cultures/euclidean.py`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.0.3.dev1/src/mapel/marriages/cultures/impartial.py` & `mapel-marriages-2.0.3.dev6/src/mapel/marriages/cultures/impartial.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 #
 #     return [votes_1, votes_2]
 #
 #
 # def generate_asymmetric__id_votes(num_agents: int = None, params=None):
 #     votes = [list(range(num_agents)) for _ in range(num_agents)]
 #
-#     votes_1 = [rotate(vote, shift) for shift, vote in enumerate(votes)]
+#     votes_1 = [rotate(vote, is_shifted) for is_shifted, vote in enumerate(votes)]
 #     votes_2 = [list(range(num_agents)) for _ in range(num_agents)]
 #
 #     return [votes_1, votes_2]
 
 
 def generate_symmetric_votes(num_agents: int = None, params=None):
```

### Comparing `mapel-marriages-2.0.3.dev1/src/mapel/marriages/cultures/mallows.py` & `mapel-marriages-2.0.3.dev6/src/mapel/marriages/cultures/mallows.py`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.0.3.dev1/src/mapel/marriages/cultures/urn.py` & `mapel-marriages-2.0.3.dev6/src/mapel/marriages/cultures/urn.py`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.0.3.dev1/src/mapel/marriages/cultures_.py` & `mapel-marriages-2.0.3.dev6/src/mapel/marriages/cultures_.py`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.0.3.dev1/src/mapel/marriages/features/basic_features.py` & `mapel-marriages-2.0.3.dev6/src/mapel/marriages/features/basic_features.py`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.0.3.dev1/src/mapel/marriages/features/distance_to_stability_features.py` & `mapel-marriages-2.0.3.dev6/src/mapel/marriages/features/distance_to_stability_features.py`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.0.3.dev1/src/mapel/marriages/features/experiments_marriage.py` & `mapel-marriages-2.0.3.dev6/src/mapel/marriages/features/experiments_marriage.py`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.0.3.dev1/src/mapel/marriages/features_.py` & `mapel-marriages-2.0.3.dev6/src/mapel/marriages/features_.py`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.0.3.dev1/src/mapel/marriages/metrics/main_marriages_distances.py` & `mapel-marriages-2.0.3.dev6/src/mapel/marriages/metrics/main_marriages_distances.py`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.0.3.dev1/src/mapel/marriages/metrics_.py` & `mapel-marriages-2.0.3.dev6/src/mapel/marriages/metrics_.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,22 +92,22 @@
             matchings[instance_id_1][instance_id_2] = matching
             matchings[instance_id_2][instance_id_1] = np.argsort(matching)
         distances[instance_id_1][instance_id_2] = distance
         distances[instance_id_2][instance_id_1] = distances[instance_id_1][instance_id_2]
         times[instance_id_1][instance_id_2] = time() - start_time
         times[instance_id_2][instance_id_1] = times[instance_id_1][instance_id_2]
 
-    if exp.store:
+    if exp.is_exported:
         _store_distances(exp, instances_ids, distances, times, t)
 
 
 def _store_distances(exp, instances_ids, distances, times, t):
     """ Store distances to file """
     file_name = f'{exp.distance_id}_p{t}.csv'
-    path = os.path.join(os.getcwd(), "experiments", exp.experiment_id, "distances", file_name)
+    path = os.path.join(os.getcwd(), "election", exp.experiment_id, "distances", file_name)
     with open(path, 'w', newline='') as csv_file:
         writer = csv.writer(csv_file, delimiter=';')
         writer.writerow(["instance_id_1", "instance_id_2", "distance", "time"])
         for election_id_1, election_id_2 in instances_ids:
             distance = float(distances[election_id_1][election_id_2])
             time_ = float(times[election_id_1][election_id_2])
             writer.writerow([election_id_1, election_id_2, distance, time_])
```

### Comparing `mapel-marriages-2.0.3.dev1/src/mapel/marriages/objects/Marriages.py` & `mapel-marriages-2.0.3.dev6/src/mapel/marriages/objects/Marriages.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,17 +92,17 @@
         return matrix
 
     # PREPARE INSTANCE
     def prepare_instance(self, store=None, params: dict = None):
         if params is None:
             params = {}
 
-        # if self.culture_id == 'norm-mallows' and 'norm-phi' not in params:
+        # if election.culture_id == 'norm-mallows' and 'norm-phi' not in params:
         #     params['norm-phi'] = np.random.rand()
-        # elif self.culture_id == 'urn' and 'alpha' not in params:
+        # elif election.culture_id == 'urn' and 'alpha' not in params:
         #     params['alpha'] = np.random.rand()
         if 'norm-phi' in params:
             params['alpha'] = params['norm-phi']
         else:
             params['alpha'] = 1
 
         self.params = params
@@ -111,15 +111,15 @@
 
         if store:
             self.store_instance_in_a_file()
 
     def store_instance_in_a_file(self):
         """ Store votes in a file """
 
-        path_to_folder = os.path.join(os.getcwd(), "experiments", self.experiment_id, "instances")
+        path_to_folder = os.path.join(os.getcwd(), "election", self.experiment_id, "instances")
         make_folder_if_do_not_exist(path_to_folder)
         path_to_file = os.path.join(path_to_folder, f'{self.instance_id}.mi')
 
         with open(path_to_file, 'w') as file_:
 
             if self.model_id in NICE_NAME:
                 file_.write("# " + NICE_NAME[self.model_id] + " " + str(self.params) + "\n")
@@ -132,15 +132,15 @@
 
                 for i in range(self.num_agents):
                     if s == 0:
                         file_.write(str(i) + ', a' + str(i) + "\n")
                     else:
                         file_.write(str(i) + ', b' + str(i) + "\n")
 
-                # c = Counter(map(tuple, self.votes[s]))
+                # c = Counter(map(tuple, election.votes[s]))
                 # counted_votes = [[count, list(row)] for row, count in c.items()]
                 # counted_votes = sorted(counted_votes, reverse=True)
 
                 votes = self.votes[s]
                 # print(votes)
 
                 file_.write(str(self.num_agents) + ', ' + str(self.num_agents) + ', ' +
@@ -167,15 +167,15 @@
 
     def import_real_instance(self, shift=False):
         """ Import real ordinal election form .soc file """
 
         votes = [0, 0]
 
         file_name = f'{self.instance_id}.mi'
-        path = os.path.join(os.getcwd(), "experiments", self.experiment_id, "instances", file_name)
+        path = os.path.join(os.getcwd(), "election", self.experiment_id, "instances", file_name)
         with open(path, 'r') as my_file:
 
             params = 0
             first_line = my_file.readline()
 
             if first_line[0] != '#':
                 model_id = 'empty'
```

### Comparing `mapel-marriages-2.0.3.dev1/src/mapel/marriages/objects/MarriagesExperiment.py` & `mapel-marriages-2.0.3.dev6/src/mapel/marriages/objects/MarriagesExperiment.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,20 +37,20 @@
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
         self.default_num_agents = 10
 
         self.matchings = {}
 
-        # self.import_matchings()
+        # election.import_matchings()
 
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
@@ -133,34 +133,34 @@
                 process.join()
 
             distances = {instance_id: {} for instance_id in self.instances}
             times = {instance_id: {} for instance_id in self.instances}
             for t in range(num_processes):
 
                 file_name = f'{distance_id}_p{t}.csv'
-                path = os.path.join(os.getcwd(), "experiments", self.experiment_id, "distances",
+                path = os.path.join(os.getcwd(), "election", self.experiment_id, "distances",
                                     file_name)
 
                 with open(path, 'r', newline='') as csv_file:
                     reader = csv.DictReader(csv_file, delimiter=';')
 
                     for row in reader:
                         distances[row['instance_id_1']][row['instance_id_2']] = float(
                             row['distance'])
                         times[row['instance_id_1']][row['instance_id_2']] = float(row['time'])
 
-        if self.store:
+        if self.is_exported:
             self._store_distances_to_file(distance_id, distances, times)
 
         self.distances = distances
         self.times = times
         self.matchings = matchings
 
     def _store_distances_to_file(self, distance_id, distances, times):
-        path_to_folder = os.path.join(os.getcwd(), "experiments", self.experiment_id, "distances")
+        path_to_folder = os.path.join(os.getcwd(), "election", self.experiment_id, "distances")
         make_folder_if_do_not_exist(path_to_folder)
         path_to_file = os.path.join(path_to_folder, f'{distance_id}.csv')
 
         with open(path_to_file, 'w', newline='') as csv_file:
             writer = csv.writer(csv_file, delimiter=';')
             writer.writerow(["instance_id_1", "instance_id_2", "distance", "time"])
 
@@ -170,15 +170,15 @@
                 writer.writerow([election_1, election_2, distance, time_])
 
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
@@ -251,32 +251,32 @@
 
         if self.instances is None:
             self.instances = {}
 
         for family_id in self.families:
 
             new_instances = self.families[family_id].prepare_family(
-                store=self.store,
+                is_exported=self.is_exported,
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
@@ -293,15 +293,15 @@
 
         feature_dict = {'value': {}, 'time': {}, 'std': {}}
 
         features_with_time = {}
         features_with_std = {'avg_num_of_bps_for_rand_matching',
                              'avg_number_of_bps_for_random_matching'}
 
-        # print(self.matchings)
+        # print(election.matchings)
 
         if feature_id == 'summed_rank_difference':
             minimal = get_values_from_csv_file(self, feature_id='summed_rank_minimal_matching')
             maximal = get_values_from_csv_file(self, feature_id='summed_rank_maximal_matching')
 
             for instance_id in self.instances:
                 if minimal[instance_id] is None:
@@ -314,15 +314,15 @@
         else:
 
             for instance_id in self.instances:
                 print(instance_id)
                 feature = features.get_feature(feature_id)
                 instance = self.instances[instance_id]
                 # if feature_id in ['summed_rank_minimal_matching'] \
-                #         and self.matchings[instance_id] is None:
+                #         and election.matchings[instance_id] is None:
                 #     value = 'None'
                 # else:
                 value = feature(instance.votes)
                 print(value)
                 #
                 # elif feature_id in ['largest_cohesive_group', 'number_of_cohesive_groups',
                 #                     'number_of_cohesive_groups_brute',
@@ -336,30 +336,30 @@
                 #                     'highest_hb_score']:
                 #     value = feature(election, feature_params)
                 #
                 # elif feature_id in {'avg_distortion_from_guardians',
                 #                     'worst_distortion_from_guardians',
                 #                     'distortion_from_all',
                 #                     'distortion_from_top_100'}:
-                #     value = feature(self, election_id)
+                #     value = feature(election, election_id)
                 # else:
                 #     value = feature(election)
 
                 if feature_id in features_with_time:
                     feature_dict['value'][instance_id] = value[0]
                     feature_dict['time'][instance_id] = value[1]
                 elif feature_id in features_with_std:
                     feature_dict['value'][instance_id] = value[0]
                     feature_dict['std'][instance_id] = value[1]
                 else:
                     feature_dict['value'][instance_id] = value
 
-        if self.store:
+        if self.is_exported:
 
-            path_to_folder = os.path.join(os.getcwd(), "experiments", self.experiment_id,
+            path_to_folder = os.path.join(os.getcwd(), "election", self.experiment_id,
                                           "features")
             make_folder_if_do_not_exist(path_to_folder)
             path_to_file = os.path.join(path_to_folder, f'{feature_id}.csv')
 
             with open(path_to_file, 'w', newline='') as csv_file:
                 writer = csv.writer(csv_file, delimiter=';')
 
@@ -377,33 +377,33 @@
                         writer.writerow([key, feature_dict['value'][key]])
 
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
                 file_csv.write("10;16;ic;{};black;1;IC;IC;o;t\n")
         except FileExistsError:
             print("Experiment already exists!")
```

### Comparing `mapel-marriages-2.0.3.dev1/src/mapel/marriages/objects/MarriagesFamily.py` & `mapel-marriages-2.0.3.dev6/src/mapel/marriages/objects/MarriagesFamily.py`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.0.3.dev1/src/mapel_marriages.egg-info/PKG-INFO` & `mapel-marriages-2.0.3.dev6/src/mapel_marriages.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapel-marriages
-Version: 2.0.3.dev1
+Version: 2.0.3.dev6
 Summary: Map of Marriages
 Author-email: Stanislaw Szufa <s.szufa@gmail.com>, Niclas Boehmer <niclas.boehmer@tu-berlin.de>
 License: Copyright (c) 2018-2022 Stanislaw Szufa and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `mapel-marriages-2.0.3.dev1/src/mapel_marriages.egg-info/SOURCES.txt` & `mapel-marriages-2.0.3.dev6/src/mapel_marriages.egg-info/SOURCES.txt`

 * *Files identical despite different names*

