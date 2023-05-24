# Comparing `tmp/Eryn-1.1.1.tar.gz` & `tmp/Eryn-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Eryn-1.1.1.tar", last modified: Fri Mar 31 17:41:07 2023, max compression
+gzip compressed data, was "Eryn-1.1.3.tar", last modified: Wed May 24 18:45:31 2023, max compression
```

## Comparing `Eryn-1.1.1.tar` & `Eryn-1.1.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 mkatz      (501) staff       (20)        0 2023-03-31 17:41:07.983421 Eryn-1.1.1/
-drwxr-xr-x   0 mkatz      (501) staff       (20)        0 2023-03-31 17:41:07.956083 Eryn-1.1.1/Eryn.egg-info/
--rw-r--r--   0 mkatz      (501) staff       (20)     4616 2023-03-31 17:41:07.000000 Eryn-1.1.1/Eryn.egg-info/PKG-INFO
--rw-r--r--   0 mkatz      (501) staff       (20)      857 2023-03-31 17:41:07.000000 Eryn-1.1.1/Eryn.egg-info/SOURCES.txt
--rw-r--r--   0 mkatz      (501) staff       (20)        1 2023-03-31 17:41:07.000000 Eryn-1.1.1/Eryn.egg-info/dependency_links.txt
--rw-r--r--   0 mkatz      (501) staff       (20)        5 2023-03-31 17:41:07.000000 Eryn-1.1.1/Eryn.egg-info/top_level.txt
--rw-r--r--   0 mkatz      (501) staff       (20)     4616 2023-03-31 17:41:07.983046 Eryn-1.1.1/PKG-INFO
--rw-r--r--   0 mkatz      (501) staff       (20)     4301 2023-03-31 17:40:19.000000 Eryn-1.1.1/README.md
-drwxr-xr-x   0 mkatz      (501) staff       (20)        0 2023-03-31 17:41:07.961233 Eryn-1.1.1/eryn/
--rw-r--r--   0 mkatz      (501) staff       (20)       38 2023-03-19 22:11:10.000000 Eryn-1.1.1/eryn/__init__.py
--rw-r--r--   0 mkatz      (501) staff       (20)       21 2023-03-31 17:41:07.000000 Eryn-1.1.1/eryn/_version.py
-drwxr-xr-x   0 mkatz      (501) staff       (20)        0 2023-03-31 17:41:07.964929 Eryn-1.1.1/eryn/backends/
--rw-r--r--   0 mkatz      (501) staff       (20)      380 2023-03-19 22:11:10.000000 Eryn-1.1.1/eryn/backends/__init__.py
--rw-r--r--   0 mkatz      (501) staff       (20)    39175 2023-03-31 17:40:20.000000 Eryn-1.1.1/eryn/backends/backend.py
--rw-r--r--   0 mkatz      (501) staff       (20)    26715 2023-03-31 17:40:20.000000 Eryn-1.1.1/eryn/backends/hdfbackend.py
--rw-r--r--   0 mkatz      (501) staff       (20)    68537 2023-03-31 17:40:20.000000 Eryn-1.1.1/eryn/ensemble.py
--rw-r--r--   0 mkatz      (501) staff       (20)      284 2023-03-19 22:11:10.000000 Eryn-1.1.1/eryn/model.py
-drwxr-xr-x   0 mkatz      (501) staff       (20)        0 2023-03-31 17:41:07.978315 Eryn-1.1.1/eryn/moves/
--rw-r--r--   0 mkatz      (501) staff       (20)     1081 2023-03-19 22:11:10.000000 Eryn-1.1.1/eryn/moves/__init__.py
--rw-r--r--   0 mkatz      (501) staff       (20)     4547 2023-03-19 22:11:10.000000 Eryn-1.1.1/eryn/moves/combine.py
--rw-r--r--   0 mkatz      (501) staff       (20)     7670 2023-03-19 22:11:10.000000 Eryn-1.1.1/eryn/moves/delayedrejection.py
--rw-r--r--   0 mkatz      (501) staff       (20)     3343 2023-03-19 22:11:10.000000 Eryn-1.1.1/eryn/moves/distgen.py
--rw-r--r--   0 mkatz      (501) staff       (20)     9133 2023-03-31 17:40:20.000000 Eryn-1.1.1/eryn/moves/distgenrj.py
--rw-r--r--   0 mkatz      (501) staff       (20)     6728 2023-03-19 22:11:10.000000 Eryn-1.1.1/eryn/moves/gaussian.py
--rw-r--r--   0 mkatz      (501) staff       (20)     8767 2023-03-19 22:11:10.000000 Eryn-1.1.1/eryn/moves/group.py
--rw-r--r--   0 mkatz      (501) staff       (20)     3493 2023-03-19 22:11:10.000000 Eryn-1.1.1/eryn/moves/groupstretch.py
--rw-r--r--   0 mkatz      (501) staff       (20)     6425 2023-03-19 22:11:10.000000 Eryn-1.1.1/eryn/moves/mh.py
--rw-r--r--   0 mkatz      (501) staff       (20)    27584 2023-03-19 22:11:10.000000 Eryn-1.1.1/eryn/moves/move.py
--rw-r--r--   0 mkatz      (501) staff       (20)     5347 2023-03-19 22:11:10.000000 Eryn-1.1.1/eryn/moves/mtdistgen.py
--rw-r--r--   0 mkatz      (501) staff       (20)     8102 2023-03-31 15:07:48.000000 Eryn-1.1.1/eryn/moves/mtdistgenrj.py
--rw-r--r--   0 mkatz      (501) staff       (20)    29678 2023-03-31 17:40:20.000000 Eryn-1.1.1/eryn/moves/multipletry.py
--rw-r--r--   0 mkatz      (501) staff       (20)    12932 2023-03-19 22:11:10.000000 Eryn-1.1.1/eryn/moves/red_blue.py
--rw-r--r--   0 mkatz      (501) staff       (20)    15910 2023-03-31 17:40:20.000000 Eryn-1.1.1/eryn/moves/rj.py
--rw-r--r--   0 mkatz      (501) staff       (20)     8765 2023-03-19 22:11:10.000000 Eryn-1.1.1/eryn/moves/stretch.py
--rw-r--r--   0 mkatz      (501) staff       (20)    23812 2023-03-31 17:40:20.000000 Eryn-1.1.1/eryn/moves/tempering.py
--rw-r--r--   0 mkatz      (501) staff       (20)     1330 2023-03-19 22:11:10.000000 Eryn-1.1.1/eryn/pbar.py
--rw-r--r--   0 mkatz      (501) staff       (20)    11282 2023-03-31 17:40:20.000000 Eryn-1.1.1/eryn/prior.py
--rw-r--r--   0 mkatz      (501) staff       (20)    23945 2023-03-19 22:11:10.000000 Eryn-1.1.1/eryn/state.py
-drwxr-xr-x   0 mkatz      (501) staff       (20)        0 2023-03-31 17:41:07.982220 Eryn-1.1.1/eryn/utils/
--rw-r--r--   0 mkatz      (501) staff       (20)      250 2023-03-19 22:11:10.000000 Eryn-1.1.1/eryn/utils/__init__.py
--rw-r--r--   0 mkatz      (501) staff       (20)     3983 2023-03-19 22:11:10.000000 Eryn-1.1.1/eryn/utils/periodic.py
--rw-r--r--   0 mkatz      (501) staff       (20)     5095 2023-03-19 22:11:10.000000 Eryn-1.1.1/eryn/utils/stopping.py
--rw-r--r--   0 mkatz      (501) staff       (20)     8895 2023-03-19 22:11:10.000000 Eryn-1.1.1/eryn/utils/transform.py
--rw-r--r--   0 mkatz      (501) staff       (20)     2137 2023-03-19 22:11:10.000000 Eryn-1.1.1/eryn/utils/updates.py
--rw-r--r--   0 mkatz      (501) staff       (20)     6692 2023-03-19 22:11:10.000000 Eryn-1.1.1/eryn/utils/utility.py
--rw-r--r--   0 mkatz      (501) staff       (20)       72 2023-03-19 22:11:10.000000 Eryn-1.1.1/pyproject.toml
--rw-r--r--   0 mkatz      (501) staff       (20)       38 2023-03-31 17:41:07.983530 Eryn-1.1.1/setup.cfg
--rw-r--r--   0 mkatz      (501) staff       (20)     1037 2023-03-19 22:11:10.000000 Eryn-1.1.1/setup.py
+drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2023-05-24 18:45:31.339148 Eryn-1.1.3/
+drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2023-05-24 18:45:31.318135 Eryn-1.1.3/Eryn.egg-info/
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     4616 2023-05-24 18:45:31.000000 Eryn-1.1.3/Eryn.egg-info/PKG-INFO
+-rw-r--r--   0 mlkatz1    (502) staff       (20)      857 2023-05-24 18:45:31.000000 Eryn-1.1.3/Eryn.egg-info/SOURCES.txt
+-rw-r--r--   0 mlkatz1    (502) staff       (20)        1 2023-05-24 18:45:31.000000 Eryn-1.1.3/Eryn.egg-info/dependency_links.txt
+-rw-r--r--   0 mlkatz1    (502) staff       (20)        5 2023-05-24 18:45:31.000000 Eryn-1.1.3/Eryn.egg-info/top_level.txt
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     4616 2023-05-24 18:45:31.338844 Eryn-1.1.3/PKG-INFO
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     4301 2023-05-24 18:44:18.000000 Eryn-1.1.3/README.md
+drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2023-05-24 18:45:31.322759 Eryn-1.1.3/eryn/
+-rw-r--r--   0 mlkatz1    (502) staff       (20)       38 2023-05-16 15:38:51.000000 Eryn-1.1.3/eryn/__init__.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)       21 2023-05-24 18:45:31.000000 Eryn-1.1.3/eryn/_version.py
+drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2023-05-24 18:45:31.325210 Eryn-1.1.3/eryn/backends/
+-rw-r--r--   0 mlkatz1    (502) staff       (20)      380 2023-05-16 15:38:51.000000 Eryn-1.1.3/eryn/backends/__init__.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    39175 2023-05-16 15:38:51.000000 Eryn-1.1.3/eryn/backends/backend.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    26715 2023-05-16 15:38:51.000000 Eryn-1.1.3/eryn/backends/hdfbackend.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    68537 2023-05-16 15:38:51.000000 Eryn-1.1.3/eryn/ensemble.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)      284 2023-05-16 15:38:51.000000 Eryn-1.1.3/eryn/model.py
+drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2023-05-24 18:45:31.334623 Eryn-1.1.3/eryn/moves/
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     1081 2023-05-16 15:38:51.000000 Eryn-1.1.3/eryn/moves/__init__.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     4547 2023-05-16 15:38:51.000000 Eryn-1.1.3/eryn/moves/combine.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     7670 2023-05-16 15:38:51.000000 Eryn-1.1.3/eryn/moves/delayedrejection.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     3935 2023-05-16 22:44:45.000000 Eryn-1.1.3/eryn/moves/distgen.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     9133 2023-05-16 15:38:51.000000 Eryn-1.1.3/eryn/moves/distgenrj.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     6728 2023-05-16 15:38:51.000000 Eryn-1.1.3/eryn/moves/gaussian.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     8767 2023-05-16 15:38:51.000000 Eryn-1.1.3/eryn/moves/group.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     3493 2023-05-16 15:38:51.000000 Eryn-1.1.3/eryn/moves/groupstretch.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     6425 2023-05-16 15:38:51.000000 Eryn-1.1.3/eryn/moves/mh.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    28232 2023-05-24 18:44:18.000000 Eryn-1.1.3/eryn/moves/move.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     5347 2023-05-16 15:38:51.000000 Eryn-1.1.3/eryn/moves/mtdistgen.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     8102 2023-05-16 15:38:51.000000 Eryn-1.1.3/eryn/moves/mtdistgenrj.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    29678 2023-05-16 15:38:51.000000 Eryn-1.1.3/eryn/moves/multipletry.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    12932 2023-05-16 15:38:51.000000 Eryn-1.1.3/eryn/moves/red_blue.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    15910 2023-05-16 15:38:51.000000 Eryn-1.1.3/eryn/moves/rj.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     8072 2023-05-24 18:44:18.000000 Eryn-1.1.3/eryn/moves/stretch.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    23812 2023-05-16 15:38:51.000000 Eryn-1.1.3/eryn/moves/tempering.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     1330 2023-05-16 15:38:51.000000 Eryn-1.1.3/eryn/pbar.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    11254 2023-05-16 22:44:45.000000 Eryn-1.1.3/eryn/prior.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    23945 2023-05-16 15:38:51.000000 Eryn-1.1.3/eryn/state.py
+drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2023-05-24 18:45:31.338312 Eryn-1.1.3/eryn/utils/
+-rw-r--r--   0 mlkatz1    (502) staff       (20)      250 2023-05-16 15:38:51.000000 Eryn-1.1.3/eryn/utils/__init__.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     3983 2023-05-16 15:38:51.000000 Eryn-1.1.3/eryn/utils/periodic.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     5095 2023-05-16 15:38:51.000000 Eryn-1.1.3/eryn/utils/stopping.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     8895 2023-05-16 15:38:51.000000 Eryn-1.1.3/eryn/utils/transform.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     2137 2023-05-16 15:38:51.000000 Eryn-1.1.3/eryn/utils/updates.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     6692 2023-05-16 15:38:51.000000 Eryn-1.1.3/eryn/utils/utility.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)       72 2023-05-16 15:38:51.000000 Eryn-1.1.3/pyproject.toml
+-rw-r--r--   0 mlkatz1    (502) staff       (20)       38 2023-05-24 18:45:31.339248 Eryn-1.1.3/setup.cfg
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     1037 2023-05-16 15:38:51.000000 Eryn-1.1.3/setup.py
```

### Comparing `Eryn-1.1.1/Eryn.egg-info/PKG-INFO` & `Eryn-1.1.3/Eryn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Eryn
-Version: 1.1.1
+Version: 1.1.3
 Summary: An all purpose MCMC sampler
 Home-page: https://github.com/mikekatz04/Eryn
 Author: Michael Katz, Nikos Karnesis
 Author-email: mikekatz04@gmail.com
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -55,15 +55,15 @@
 
 Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.
 
 ## Versioning
 
 We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/BlackHolePerturbationToolkit/FastEMRIWaveforms/tags).
 
-Current Version: 1.1.1
+Current Version: 1.1.3
 
 ## Citation
 
 When using this package, please cite at minimum the following sources:
 
 ```
 @article{Karnesis:2023ras,
```

### Comparing `Eryn-1.1.1/Eryn.egg-info/SOURCES.txt` & `Eryn-1.1.3/Eryn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.1/PKG-INFO` & `Eryn-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Eryn
-Version: 1.1.1
+Version: 1.1.3
 Summary: An all purpose MCMC sampler
 Home-page: https://github.com/mikekatz04/Eryn
 Author: Michael Katz, Nikos Karnesis
 Author-email: mikekatz04@gmail.com
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -55,15 +55,15 @@
 
 Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.
 
 ## Versioning
 
 We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/BlackHolePerturbationToolkit/FastEMRIWaveforms/tags).
 
-Current Version: 1.1.1
+Current Version: 1.1.3
 
 ## Citation
 
 When using this package, please cite at minimum the following sources:
 
 ```
 @article{Karnesis:2023ras,
```

### Comparing `Eryn-1.1.1/README.md` & `Eryn-1.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
 Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.
 
 ## Versioning
 
 We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/BlackHolePerturbationToolkit/FastEMRIWaveforms/tags).
 
-Current Version: 1.1.1
+Current Version: 1.1.3
 
 ## Citation
 
 When using this package, please cite at minimum the following sources:
 
 ```
 @article{Karnesis:2023ras,
```

### Comparing `Eryn-1.1.1/eryn/backends/backend.py` & `Eryn-1.1.3/eryn/backends/backend.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.1/eryn/backends/hdfbackend.py` & `Eryn-1.1.3/eryn/backends/hdfbackend.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.1/eryn/ensemble.py` & `Eryn-1.1.3/eryn/ensemble.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.1/eryn/moves/__init__.py` & `Eryn-1.1.3/eryn/moves/__init__.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.1/eryn/moves/combine.py` & `Eryn-1.1.3/eryn/moves/combine.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.1/eryn/moves/delayedrejection.py` & `Eryn-1.1.3/eryn/moves/delayedrejection.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.1/eryn/moves/distgen.py` & `Eryn-1.1.3/eryn/moves/distgen.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,39 +7,46 @@
 __all__ = ["DistributionGenerate"]
 
 
 class DistributionGenerate(MHMove):
     """Generate proposals from a distribution
 
     Args:
-        generate_dist (object): :class:`ProbDistContainer` object that has ``logpdf``
+        generate_dist (dict): Dictionary with keys as branch names and items as
+            :class:`ProbDistContainer` objects that have ``logpdf``
             and ``rvs`` methods.
 
     """
 
     def __init__(self, generate_dist, *args, **kwargs):
+        if not isinstance(generate_dist, dict):
+            raise ValueError(
+                "When entering directly into the DistributionGenerate class, generate_dist must be a dictionary. The keys are branch names and the items are ProbDistContainer objects."
+            )
 
         for key in generate_dist:
             if not isinstance(generate_dist[key], ProbDistContainer):
                 raise ValueError(
                     "Distributions need to be eryn.prior.ProbDistContainer object."
                 )
         self.generate_dist = generate_dist
         super(DistributionGenerate, self).__init__(*args, **kwargs)
 
-    def get_proposal(self, all_coords, all_inds, random, **kwargs):
+    def get_proposal(self, branches_coords, random, branches_inds=None, **kwargs):
         """Make a proposal
 
         Args:
-            all_coords (dict): Keys are ``branch_names``. Values are
-                np.ndarray[ntemps, nwalkers, nleaves_max, ndim]. These are the curent
-                coordinates for all the walkers.
-            all_inds (dict): Keys are ``branch_names``. Values are
-                np.ndarray[ntemps, nwalkers, nleaves_max]. These are the boolean
-                arrays marking which leaves are currently used within each walker.
+            branches_coords (dict): Keys are ``branch_names`` and values are
+                np.ndarray[ntemps, nwalkers, nleaves_max, ndim] representing
+                coordinates for walkers.
+            random (object): Current random state object.
+            branches_inds (dict, optional): Keys are ``branch_names`` and values are
+                np.ndarray[ntemps, nwalkers, nleaves_max] representing which
+                leaves are currently being used. (default: ``None``)
+            **kwargs (ignored): This is added for compatibility. It is ignored in this function.
 
         Returns:
             tuple: Tuple containing proposal information.
                 First entry is the new coordinates as a dictionary with keys
                 as ``branch_names`` and values as
                 ``double `` np.ndarray[ntemps, nwalkers, nleaves_max, ndim] containing
                 proposed coordinates. Second entry
@@ -50,23 +57,27 @@
 
         """
 
         # set up all initial holders
         q = {}
         factors = {}
         new_inds = {}
-        if all_inds is None:
-            all_inds = {
+        if branches_inds is None:
+            branches_inds = {
                 name: np.ones(coords.shape[:-1], dtype=bool)
-                for name, coords in all_coords
+                for name, coords in branches_coords
             }
 
         # iterate through branches and propose new points where inds == True
         for i, (name, coords, inds) in enumerate(
-            zip(all_coords.keys(), all_coords.values(), all_inds.values(),)
+            zip(
+                branches_coords.keys(),
+                branches_coords.values(),
+                branches_inds.values(),
+            )
         ):
             # copy over previous info
             ntemps, nwalkers, _, _ = coords.shape
             q[name] = coords.copy()
             new_inds[name] = inds.copy()
 
             if i == 0:
```

### Comparing `Eryn-1.1.1/eryn/moves/distgenrj.py` & `Eryn-1.1.3/eryn/moves/distgenrj.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.1/eryn/moves/gaussian.py` & `Eryn-1.1.3/eryn/moves/gaussian.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.1/eryn/moves/group.py` & `Eryn-1.1.3/eryn/moves/group.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.1/eryn/moves/groupstretch.py` & `Eryn-1.1.3/eryn/moves/groupstretch.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.1/eryn/moves/mh.py` & `Eryn-1.1.3/eryn/moves/mh.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.1/eryn/moves/move.py` & `Eryn-1.1.3/eryn/moves/move.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,70 +21,90 @@
             This object controls the tempering. It is passed to the parent class
             to moves so that all proposals can share and use temperature settings.
             (default: ``None``)
         periodic (:class:`eryn.utils.PeriodicContainer, optional):
             This object holds periodic information and methods for periodic parameters. It is passed to the parent class
             to moves so that all proposals can share and use periodic information.
             (default: ``None``)
-        gibbs_sampling_setup (str, tuple, dict, or list, optional): This sets the Gibbs Sampling setup if 
+        gibbs_sampling_setup (str, tuple, dict, or list, optional): This sets the Gibbs Sampling setup if
             desired. The Gibbs sampling setup is completely customizable down to the leaf and parameters.
-            All of the separate Gibbs sampling splits will be run within 1 call to this proposal. 
-            If ``None``, run all branches and all parameters. If ``str``, run all parameters within the 
-            branch given as the string. To enter a branch with a specific set of parameters, you can 
+            All of the separate Gibbs sampling splits will be run within 1 call to this proposal.
+            If ``None``, run all branches and all parameters. If ``str``, run all parameters within the
+            branch given as the string. To enter a branch with a specific set of parameters, you can
             provide a 2-tuple with the first entry as the branch name and the second entry as a 2D
             boolean array of shape ``(nleaves_max, ndim)`` that indicates which leaves and/or parameters
-            you want to run. ``None`` can also be entered in the second entry if all parameters are to be run. 
-            A dictionary is also possible with keys as branch names and values as the same 2D boolean array 
+            you want to run. ``None`` can also be entered in the second entry if all parameters are to be run.
+            A dictionary is also possible with keys as branch names and values as the same 2D boolean array
             of shape ``(nleaves_max, ndim)`` that indicates which leaves and/or parameters
             you want to run. ``None`` can also be entered in the value of the dictionary
-            if all parameters are to be run. If multiple keys are provided in the dictionary, those 
-            branches will be run simultaneously in the proposal as one iteration of the proposing loop. 
-            The final option is a list. This is how you make sure to run all the Gibbs splits. Each entry 
-            of the list can be a string, 2-tuple, or dictionary as described above. The list controls 
-            the order in which all of these splits are run. (default: ``None``) 
+            if all parameters are to be run. If multiple keys are provided in the dictionary, those
+            branches will be run simultaneously in the proposal as one iteration of the proposing loop.
+            The final option is a list. This is how you make sure to run all the Gibbs splits. Each entry
+            of the list can be a string, 2-tuple, or dictionary as described above. The list controls
+            the order in which all of these splits are run. (default: ``None``)
         prevent_swaps (bool, optional): If ``True``, do not perform temperature swaps in this move.
-        skip_supp_names_update (list, optional): List of names (`str`), that can be in any 
+        skip_supp_names_update (list, optional): List of names (`str`), that can be in any
             :class:`eryn.state.BranchSupplimental`,
-            to skip when updating states (:func:`Move.update`). This is useful if a 
+            to skip when updating states (:func:`Move.update`). This is useful if a
             large amount of memory is stored in the branch supplimentals.
         is_rj (bool, optional): If using RJ, this should be ``True``. (default: ``False``)
+        use_gpu (bool, optional): If ``True``, use ``CuPy`` for computations.
+            Use ``NumPy`` if ``use_gpu == False``. (default: ``False``)
+        random_seed (int, optional): Set the random seed in ``CuPy/NumPy`` if not ``None``.
+            (default: ``None``)
 
     Raises:
         ValueError: Incorrect inputs.
 
     Attributes:
         Note: All kwargs are stored as attributes.
-        num_proposals (int): the number of times this move has been run. This is needed to 
+        num_proposals (int): the number of times this move has been run. This is needed to
             compute the acceptance fraction.
-        gibbs_sampling_setup (list): All of the Gibbs sampling splits as described above. 
+        gibbs_sampling_setup (list): All of the Gibbs sampling splits as described above.
+        xp (obj): ``NumPy`` or ``CuPy``.
+        use_gpu (bool): Whether ``Cupy`` (``True``) is used or not (``False``).
 
     """
 
     def __init__(
         self,
         temperature_control=None,
         periodic=None,
         gibbs_sampling_setup=None,
         prevent_swaps=False,
         skip_supp_names_update=[],
         is_rj=False,
+        use_gpu=False,
+        random_seed=None,
         **kwargs
     ):
         # store all information
         self.temperature_control = temperature_control
         self.periodic = periodic
         self.skip_supp_names_update = skip_supp_names_update
         self.prevent_swaps = prevent_swaps
 
         self._initialize_branch_setup(gibbs_sampling_setup, is_rj=is_rj)
 
         # keep track of the number of proposals
         self.num_proposals = 0
         self.time = 0
 
+        # change array library based on GPU usage
+        if use_gpu:
+            self.xp = xp
+        else:
+            self.xp = np
+
+        # set the random seet of the library if desired
+        if random_seed is not None:
+            self.xp.random.seed(random_seed)
+
+        self.use_gpu = use_gpu
+
     def _initialize_branch_setup(self, gibbs_sampling_setup, is_rj=False):
         """Initialize the gibbs setup properly."""
         self.gibbs_sampling_setup = gibbs_sampling_setup
 
         message_rj = """inputting gibbs indexing at the leaf/parameter level is not allowed 
                                         with an RJ proposal. Only branch names."""
 
@@ -99,15 +119,14 @@
                 )
 
             if not isinstance(self.gibbs_sampling_setup, list):
                 self.gibbs_sampling_setup = [self.gibbs_sampling_setup]
 
             gibbs_sampling_setup_tmp = []
             for item in self.gibbs_sampling_setup:
-
                 # all the arguments are treated
 
                 # strings indicate single branch all parameters
                 if isinstance(item, str):
                     gibbs_sampling_setup_tmp.append(item)
 
                 # tuple is one branch with a split in the parameters
@@ -190,57 +209,57 @@
         else:
             # no Gibbs sampling
             self.branch_names_run_all = [None]
             self.inds_run_all = [None]
 
     def gibbs_sampling_setup_iterator(self, all_branch_names):
         """Iterate through the gibbs splits as a generator
-        
+
         Args:
             all_branch_names (list): List of all branch names.
 
         Yields:
             2-tuple: Gibbs sampling split.
                         First entry is the branch names to run and the second entry is the index
-                        into the leaves/parameters for this Gibbs split. 
+                        into the leaves/parameters for this Gibbs split.
 
         Raises:
             ValueError: Incorrect inputs.
 
         """
-        for (branch_names_run, inds_run) in zip(
+        for branch_names_run, inds_run in zip(
             self.branch_names_run_all, self.inds_run_all
         ):
             # adjust if branch_names_run is None
             if branch_names_run is None:
                 branch_names_run = all_branch_names
                 inds_run = [None for _ in branch_names_run]
             # yield to the iterator
             yield (branch_names_run, inds_run)
 
     def setup_proposals(
         self, branch_names_run, inds_run, branches_coords, branches_inds
     ):
         """Setup proposals when gibbs sampling.
-        
+
         Get inputs into the proposal including Gibbs split information.
 
         Args:
             branch_names_run (list): List of branch names to run concurrently.
             inds_run (list): List of ``inds`` arrays including Gibbs sampling information.
             branches_coords (dict): Dictionary of coordinate arrays for all branches.
             branches_inds (dict): Dictionary of ``inds`` arrays for all branches.
 
         Returns:
             tuple:  (coords, inds, at_least_one_proposal)
                         * Coords including Gibbs sampling info.
                         * ``inds`` including Gibbs sampling info.
-                        * ``at_least_one_proposal`` is boolean. It is passed out to 
+                        * ``at_least_one_proposal`` is boolean. It is passed out to
                             indicate there is at least one leaf available for the requested branch names.
-        
+
         """
         inds_going_for_proposal = {}
         coords_going_for_proposal = {}
 
         at_least_one_proposal = False
         for bnr, ir in zip(branch_names_run, inds_run):
             if ir is not None:
@@ -274,25 +293,25 @@
         branches_coords,
         new_inds=None,
         branches_inds=None,
         new_branch_supps=None,
         branches_supplimental=None,
     ):
         """Set all not Gibbs-sampled parameters back
-        
+
         Args:
             branch_names_run (list): List of branch names to run concurrently.
             inds_run (list): List of ``inds`` arrays including Gibbs sampling information.
             q (dict): Dictionary of new coordinate arrays for all proposal branches.
             branches_coords (dict): Dictionary of old coordinate arrays for all branches.
             new_inds (dict, optional): Dictionary of new inds arrays for all proposal branches.
             branches_inds (dict, optional): Dictionary of old inds arrays for all branches.
             new_branch_supps (dict, optional): Dictionary of new branches supplimental for all proposal branches.
             branches_supplimental (dict, optional): Dictionary of old branches supplimental for all branches.
-            
+
         """
         # add back any parameters that are fixed for this round
         for bnr, ir in zip(branch_names_run, inds_run):
             if ir is not None:
                 q[bnr][:, :, ~ir] = branches_coords[bnr][:, :, ~ir]
 
         # add other models that were not included
@@ -305,24 +324,24 @@
 
             if new_branch_supps is not None and key not in new_branch_supps:
                 assert branches_supplimental is not None
                 new_branch_supps[key] = branches_supplimental[key].copy()
 
     def ensure_ordering(self, correct_key_order, q, new_inds, new_branch_supps):
         """Ensure proper order of key in dictionaries.
-        
+
         Args:
             correct_key_order (list): Keys in correct order.
             q (dict): Dictionary of new coordinate arrays for all branches.
             new_inds (dict): Dictionary of new inds arrays for all branches.
             new_branch_supps (dict or None): Dictionary of new branches supplimental for all proposal branches.
 
         Returns:
             Tuple: (q, new_inds, new_branch_supps) in correct key order.
-       
+
         """
         if list(q.keys()) != correct_key_order:
             q = {key: q[key] for key in correct_key_order}
 
         if list(new_inds.keys()) != correct_key_order:
             new_inds = {key: new_inds[key] for key in correct_key_order}
 
@@ -332,21 +351,21 @@
         ):
             new_branch_supps = {key: new_branch_supps[key] for key in correct_key_order}
 
         return q, new_inds, new_branch_supps
 
     def fix_logp_gibbs(self, branch_names_run, inds_run, logp, inds):
         """Set any walker with no leaves to have logp = -np.inf
-        
+
         Args:
             branch_names_run (list): List of branch names to run concurrently.
             inds_run (list): List of ``inds`` arrays including Gibbs sampling information.
             logp (np.ndarray): Log of the prior going into final posterior computation.
             inds (dict): Dictionary of ``inds`` arrays for all branches.
-            
+
         """
         total_leaves = np.zeros_like(logp)
         for bnr, ir in zip(branch_names_run, inds_run):
             if ir is not None:
                 tmp = np.zeros_like(inds[bnr], dtype=bool)
 
                 # flatten coordinates to the leaves dimension
@@ -588,15 +607,14 @@
                 )
                 for name in new_inds
                 if temp_change_branch_supplimental[name] is not None
             ]
 
         # sampler level supplimental
         if old_state.supplimental is not None:
-
             old_suppliment = old_state.supplimental.take_along_axis(subset, axis=1)
             new_suppliment = new_state.supplimental[:]
 
             accepted_temp_here = accepted_temp.copy()
 
             temp_change_suppliment = {}
             for name in old_suppliment:
@@ -662,8 +680,7 @@
             )
 
             np.put_along_axis(
                 old_state.blobs, subset[:, :, None], temp_change_blobs, axis=1
             )
 
         return old_state
-
```

### Comparing `Eryn-1.1.1/eryn/moves/mtdistgen.py` & `Eryn-1.1.3/eryn/moves/mtdistgen.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.1/eryn/moves/mtdistgenrj.py` & `Eryn-1.1.3/eryn/moves/mtdistgenrj.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.1/eryn/moves/multipletry.py` & `Eryn-1.1.3/eryn/moves/multipletry.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.1/eryn/moves/red_blue.py` & `Eryn-1.1.3/eryn/moves/red_blue.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.1/eryn/moves/rj.py` & `Eryn-1.1.3/eryn/moves/rj.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.1/eryn/moves/stretch.py` & `Eryn-1.1.3/eryn/moves/stretch.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,117 +19,105 @@
     parallelization as described in `Foreman-Mackey et al. (2013)
     <https://arxiv.org/abs/1202.3665>`_.
 
     This class was originally implemented in ``emcee``.
 
     Args:
         a (double, optional): The stretch scale parameter. (default: ``2.0``)
-        use_gpu (bool, optional): If ``True``, use ``CuPy`` for computations. 
-            Use ``NumPy`` if ``use_gpu == False``. (default: ``False``)
-        return_gpu (bool, optional): If ``use_gpu == True and return_gpu == True``, 
+        return_gpu (bool, optional): If ``use_gpu == True and return_gpu == True``,
             the returned arrays will be returned as ``CuPy`` arrays. (default: ``False``)
-        random_seed (int, optional): Set the random seed in ``CuPy/NumPy`` if not ``None``.
-            (default: ``None``)
         kwargs (dict, optional): Additional keyword arguments passed down through :class:`RedRedBlueMove`_.
 
     Attributes:
         a (double): The stretch scale parameter.
-        xp (obj): ``NumPy`` or ``CuPy``.
-        use_gpu (bool): Whether ``Cupy`` (``True``) is used or not (``False``). 
-        return_gpu (bool): Whether the array being returned is in ``Cupy`` (``True``) 
+        return_gpu (bool): Whether the array being returned is in ``Cupy`` (``True``)
             or ``NumPy`` (``False``).
-        
+
     """
 
     def __init__(
         self, a=2.0, use_gpu=False, return_gpu=False, random_seed=None, **kwargs
     ):
-
         # store scale factor
         self.a = a
 
-        # change array library based on GPU usage
-        if use_gpu:
-            self.xp = xp
-        else:
-            self.xp = np
-
-        # set the random seet of the library if desired
-        if random_seed is not None:
-            self.xp.random.seed(random_seed)
-
-        self.use_gpu = use_gpu
         self.return_gpu = return_gpu
 
         # pass kwargs up
         RedBlueMove.__init__(self, **kwargs)
 
         # how it was formerly
         # super(StretchMove, self).__init__(**kwargs)
 
     def adjust_factors(self, factors, ndims_old, ndims_new):
-        """Adjust the ``factors`` based on changing dimensions. 
+        """Adjust the ``factors`` based on changing dimensions.
 
         ``factors`` is adjusted in place.
 
-        Args: 
+        Args:
             factors (xp.ndarray): Array of ``factors`` values. It is adjusted in place.
             ndims_old (int or xp.ndarray): Old dimension. If given as an ``xp.ndarray``,
                 must be broadcastable with ``factors``.
             ndims_new (int or xp.ndarray): New dimension. If given as an ``xp.ndarray``,
-                must be broadcastable with ``factors``.  
-        
+                must be broadcastable with ``factors``.
+
         """
         # adjusts in place
         logzz = factors / (ndims_old - 1.0)
         factors[:] = logzz * (ndims_new - 1.0)
 
     def choose_c_vals(self, c, Nc, Ns, ntemps, random_number_generator, **kwargs):
         """Get the compliment array
-        
-        The compliment represents the points that are used to move the actual points whose position is 
+
+        The compliment represents the points that are used to move the actual points whose position is
         changing.
 
         Args:
             c (np.ndarray): Possible compliment values with shape ``(ntemps, Nc, nleaves_max, ndim)``.
             Nc (int): Length of the ``...``: the subset of walkers proposed to move now (usually nwalkers/2).
             Ns (int): Number of generation points.
             ntemps (int): Number of temperatures.
             random_number_generator (object): Random state object.
             **kwargs (ignored): Ignored here. For modularity.
 
         Returns:
             np.ndarray: Compliment values to use with shape ``(ntemps, Ns, nleaves_max, ndim)``.
-        
+
         """
-        rint = random_number_generator.randint(Nc, size=(ntemps, Ns,))
+        rint = random_number_generator.randint(
+            Nc,
+            size=(
+                ntemps,
+                Ns,
+            ),
+        )
         c_temp = self.xp.take_along_axis(c, rint[:, :, None, None], axis=1)
         return c_temp
 
     def get_new_points(
         self, name, s, c_temp, Ns, branch_shape, branch_i, random_number_generator
     ):
         """Get mew points in stretch move.
-        
+
         Takes compliment and uses it to get new points for those being proposed.
 
         Args:
             name (str): Branch name.
-            s (np.ndarray): Points to be moved with shape ``(ntemps, Ns, nleaves_max, ndim)``. 
+            s (np.ndarray): Points to be moved with shape ``(ntemps, Ns, nleaves_max, ndim)``.
             c (np.ndarray): Compliment to move points with shape ``(ntemps, Ns, nleaves_max, ndim)``.
-            Ns (int): Number to generate.  
+            Ns (int): Number to generate.
             branch_shape (tuple): Full branch shape.
-            branch_i (int): Which branch in the order is being run now. This ensures that the 
+            branch_i (int): Which branch in the order is being run now. This ensures that the
                 randomly generated quantity per walker remains the same over branches.
             random_number_generator (object): Random state object.
 
         Returns:
             np.ndarray: New proposed points with shape ``(ntemps, Ns, nleaves_max, ndim)``.
-            
-        
+
+
         """
         ntemps, nwalkers, nleaves_max, ndim_here = branch_shape
 
         # only for the first branch do we draw for zz
         if branch_i == 0:
             self.zz = (
                 (self.a - 1.0) * random_number_generator.rand(ntemps, Ns) + 1
@@ -230,8 +218,7 @@
             factors = factors.get()
 
         if gibbs_ndim is not None:
             # adjust factors in place
             self.adjust_factors(factors, ndim, gibbs_ndim)
 
         return newpos, factors
-
```

### Comparing `Eryn-1.1.1/eryn/moves/tempering.py` & `Eryn-1.1.3/eryn/moves/tempering.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.1/eryn/pbar.py` & `Eryn-1.1.3/eryn/pbar.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.1/eryn/prior.py` & `Eryn-1.1.3/eryn/prior.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,20 +15,19 @@
     Args:
         min_val (double): Minimum in the uniform distribution
         max_val (double): Maximum in the uniform distribution
         use_cupy (bool, optional): If ``True``, use CuPy. If ``False`` use Numpy.
             (default: ``False``)
 
     Raises:
-        ValueError: Issue with inputs. 
+        ValueError: Issue with inputs.
 
     """
 
     def __init__(self, min_val, max_val, use_cupy=False):
-
         if min_val > max_val:
             tmp = min_val
             min_val = max_val
             max_val = tmp
         elif min_val == max_val:
             raise ValueError("Min and max values are the same.")
 
@@ -43,15 +42,14 @@
         if use_cupy:
             try:
                 cp.abs(1.0)
             except NameError:
                 raise ValueError("CuPy not found.")
 
     def rvs(self, size=1):
-
         if not isinstance(size, int) and not isinstance(size, tuple):
             raise ValueError("size must be an integer or tuple of ints.")
 
         if isinstance(size, int):
             size = (size,)
 
         xp = np if not self.use_cupy else cp
@@ -59,30 +57,27 @@
         rand_unif = xp.random.rand(*size)
 
         out = rand_unif * self.diff + self.min_val
 
         return out
 
     def pdf(self, x):
-
         out = self.pdf_val * ((x >= self.min_val) & (x <= self.max_val))
 
         return out
 
     def logpdf(self, x):
-
         xp = np if not self.use_cupy else cp
 
         out = xp.zeros_like(x)
         out[(x >= self.min_val) & (x <= self.max_val)] = self.logpdf_val
         out[(x < self.min_val) | (x > self.max_val)] = -np.inf
         return out
 
     def copy(self):
-        breakpoint()
         return deepcopy(self)
 
 
 def uniform_dist(min, max, use_cupy=False):
     """Generate uniform distribution between ``min`` and ``max``
 
     Args:
@@ -211,25 +206,23 @@
 
     Raises:
         ValueError: Missing parameters or incorrect index keys.
 
     """
 
     def __init__(self, priors_in, use_cupy=False):
-
         # copy to have
         self.priors_in = priors_in.copy()
 
         # to separate out in list form
         self.priors = []
 
         # setup lists
         temp_inds = []
         for inds, dist in priors_in.items():
-
             # multiple index
             if isinstance(inds, tuple):
                 inds_in = np.asarray(inds)
                 self.priors.append([inds_in, dist])
 
             # single index
             elif isinstance(inds, int):
```

### Comparing `Eryn-1.1.1/eryn/state.py` & `Eryn-1.1.3/eryn/state.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.1/eryn/utils/periodic.py` & `Eryn-1.1.3/eryn/utils/periodic.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.1/eryn/utils/stopping.py` & `Eryn-1.1.3/eryn/utils/stopping.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.1/eryn/utils/transform.py` & `Eryn-1.1.3/eryn/utils/transform.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.1/eryn/utils/updates.py` & `Eryn-1.1.3/eryn/utils/updates.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.1/eryn/utils/utility.py` & `Eryn-1.1.3/eryn/utils/utility.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.1/setup.py` & `Eryn-1.1.3/setup.py`

 * *Files identical despite different names*

