# Comparing `tmp/hierarch-1.1.3.tar.gz` & `tmp/hierarch-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hierarch-1.1.3.tar", last modified: Fri Jul  9 05:19:45 2021, max compression
+gzip compressed data, was "hierarch-1.1.5.tar", max compression
```

## Comparing `hierarch-1.1.3.tar` & `hierarch-1.1.5.tar`

### file list

```diff
@@ -1,19 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-09 05:19:45.984609 hierarch-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1093 2021-07-09 05:19:39.000000 hierarch-1.1.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3393 2021-07-09 05:19:45.984609 hierarch-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2497 2021-07-09 05:19:39.000000 hierarch-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-09 05:19:45.984609 hierarch-1.1.3/hierarch/
--rw-r--r--   0 runner    (1001) docker     (121)      374 2021-07-09 05:19:39.000000 hierarch-1.1.3/hierarch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12096 2021-07-09 05:19:39.000000 hierarch-1.1.3/hierarch/internal_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     3776 2021-07-09 05:19:39.000000 hierarch-1.1.3/hierarch/numba_overloads.py
--rw-r--r--   0 runner    (1001) docker     (121)     7103 2021-07-09 05:19:39.000000 hierarch-1.1.3/hierarch/power.py
--rw-r--r--   0 runner    (1001) docker     (121)    23375 2021-07-09 05:19:39.000000 hierarch-1.1.3/hierarch/resampling.py
--rw-r--r--   0 runner    (1001) docker     (121)    42812 2021-07-09 05:19:39.000000 hierarch-1.1.3/hierarch/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-09 05:19:45.984609 hierarch-1.1.3/hierarch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3393 2021-07-09 05:19:45.000000 hierarch-1.1.3/hierarch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      328 2021-07-09 05:19:45.000000 hierarch-1.1.3/hierarch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-09 05:19:45.000000 hierarch-1.1.3/hierarch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       55 2021-07-09 05:19:45.000000 hierarch-1.1.3/hierarch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2021-07-09 05:19:45.000000 hierarch-1.1.3/hierarch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-07-09 05:19:45.984609 hierarch-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      855 2021-07-09 05:19:39.000000 hierarch-1.1.3/setup.py
+-rw-r--r--   0        0        0     1093 2023-05-24 20:22:48.609884 hierarch-1.1.5/LICENSE.txt
+-rw-r--r--   0        0        0     2478 2023-05-24 20:22:48.609884 hierarch-1.1.5/README.md
+-rw-r--r--   0        0        0      374 2023-05-24 20:22:48.613884 hierarch-1.1.5/hierarch/__init__.py
+-rw-r--r--   0        0        0    12082 2023-05-24 20:22:48.613884 hierarch-1.1.5/hierarch/internal_functions.py
+-rw-r--r--   0        0        0     3776 2023-05-24 20:22:48.613884 hierarch-1.1.5/hierarch/numba_overloads.py
+-rw-r--r--   0        0        0     7505 2023-05-24 20:22:48.613884 hierarch-1.1.5/hierarch/power.py
+-rw-r--r--   0        0        0    21647 2023-05-24 20:22:48.613884 hierarch-1.1.5/hierarch/resampling.py
+-rw-r--r--   0        0        0    42838 2023-05-24 20:22:48.613884 hierarch-1.1.5/hierarch/stats.py
+-rw-r--r--   0        0        0      768 2023-05-24 20:22:48.613884 hierarch-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3187 1970-01-01 00:00:00.000000 hierarch-1.1.5/PKG-INFO
```

### Comparing `hierarch-1.1.3/LICENSE.txt` & `hierarch-1.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hierarch-1.1.3/PKG-INFO` & `hierarch-1.1.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,76 +1,83 @@
 Metadata-Version: 2.1
 Name: hierarch
-Version: 1.1.3
+Version: 1.1.5
 Summary: Hierarchical hypothesis testing library
 Home-page: https://github.com/rishi-kulkarni/hierarch
+License: LICENSE.txt
 Author: Rishi Kulkarni
-Author-email: rkulk@stanford.edu
-License: UNKNOWN
-Description: # hierarch
-        
-        ## A Hierarchical Resampling Package for Python
-        
-        Version 1.1.3
-        
-        hierarch is a package for hierarchical resampling (bootstrapping, permutation) of datasets in Python. Because for loops are ultimately intrinsic to cluster-aware resampling, hierarch uses Numba to accelerate many of its key functions.
-        
-        hierarch has several functions to assist in performing resampling-based (and therefore distribution-free) hypothesis tests, confidence interval calculations, and power analyses on hierarchical data.
-        
-        ## Table of Contents
-        
-        1. [Introduction](#introduction)
-        2. [Setup](#setup)
-        3. [Documentation](#documentation)
-        4. [Citation](#citation)
-        
-        
-        <a name="introduction"></a>
-        ## Introduction 
-        
-        Design-based randomization tests represents the platinum standard for significance analyses [[1, 2, 3]](#1) - that is, they produce probability statements that depend only on the experimental design, not at all on less-than-verifiable assumptions about the probability distributions of the data-generating process. Researchers can use hierarch to quickly perform automated design-based randomization tests for experiments with arbitrary levels of hierarchy.
-        
-        
-        <a id="1">[1]</a> Tukey, J.W. (1993). Tightening the Clinical Trial. Controlled Clinical Trials, 14(4), 266-285.
-        
-        <a id="1">[2]</a> Millard, S.P., Krause, A. (2001). Applied Statistics in the Pharmaceutical Industry. Springer.
-        
-        <a id="1">[3]</a> Berger, V.W. (2000). Pros and cons of permutation tests in clinical trials. Statistics in Medicine, 19(10), 1319-1328.
-        
-        
-        <a name="setup"></a>
-        ## Setup 
-        
-        ### Dependencies
-        * numpy
-        * pandas (for importing data)
-        * numba
-        * scipy (for power analysis)
-        
-        ### Installation
-        
-        The easiest way to install hierarch is via PyPi. 
-        
-        ```pip install hierarch```
-        
-        Alternatively, you can install from Anaconda.
-        
-        ```conda install -c rkulk111 hierarch```
-        
-        
-        <a name="documentation"></a>
-        ## Documentation
-        Check out our user guide at [readthedocs](https://hierarch.readthedocs.io/).
-        
-        <a name="citation"></a>
-        ## Citation
-        If hierarch helps you analyze your data, please consider citing it. The manuscript also
-        contains a set of simulations validating hierarchical randomization tests in a variety of
-        conditions.
-        
-        Analyzing Nested Experimental Designs – A User-Friendly Resampling Method to Determine Experimental Significance. Rishikesh U. Kulkarni, Catherine L. Wang, Carolyn R. Bertozzi. bioRxiv 2021.06.29.450439; doi: https://doi.org/10.1101/2021.06.29.450439
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
+Author-email: rishi@kulkarni.science
+Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: numba (>=0.57,<0.58)
+Requires-Dist: pandas (>=1.5.3,<3.0.0)
+Requires-Dist: scipy (>=1.10.0,<2.0.0)
 Description-Content-Type: text/markdown
+
+# hierarch
+
+## A Hierarchical Resampling Package for Python
+
+Version 1.1.3
+
+hierarch is a package for hierarchical resampling (bootstrapping, permutation) of datasets in Python. Because for loops are ultimately intrinsic to cluster-aware resampling, hierarch uses Numba to accelerate many of its key functions.
+
+hierarch has several functions to assist in performing resampling-based (and therefore distribution-free) hypothesis tests, confidence interval calculations, and power analyses on hierarchical data.
+
+## Table of Contents
+
+1. [Introduction](#introduction)
+2. [Setup](#setup)
+3. [Documentation](#documentation)
+4. [Citation](#citation)
+
+
+<a name="introduction"></a>
+## Introduction 
+
+Design-based randomization tests represents the platinum standard for significance analyses [[1, 2, 3]](#1) - that is, they produce probability statements that depend only on the experimental design, not at all on less-than-verifiable assumptions about the probability distributions of the data-generating process. Researchers can use hierarch to quickly perform automated design-based randomization tests for experiments with arbitrary levels of hierarchy.
+
+
+<a id="1">[1]</a> Tukey, J.W. (1993). Tightening the Clinical Trial. Controlled Clinical Trials, 14(4), 266-285.
+
+<a id="1">[2]</a> Millard, S.P., Krause, A. (2001). Applied Statistics in the Pharmaceutical Industry. Springer.
+
+<a id="1">[3]</a> Berger, V.W. (2000). Pros and cons of permutation tests in clinical trials. Statistics in Medicine, 19(10), 1319-1328.
+
+
+<a name="setup"></a>
+## Setup 
+
+### Dependencies
+* numpy
+* pandas (for importing data)
+* numba
+* scipy (for power analysis)
+
+### Installation
+
+The easiest way to install hierarch is via PyPi. 
+
+```pip install hierarch```
+
+Alternatively, you can install from Anaconda.
+
+```conda install -c rkulk111 hierarch```
+
+
+<a name="documentation"></a>
+## Documentation
+Check out our user guide at [readthedocs](https://hierarch.readthedocs.io/).
+
+<a name="citation"></a>
+## Citation
+If hierarch helps you analyze your data, please consider citing it. The manuscript also
+contains a set of simulations validating hierarchical randomization tests in a variety of
+conditions.
+
+Kulkarni RU, Wang CL, Bertozzi CR (2022) Analyzing nested experimental designs—A user-friendly resampling method to determine experimental significance. PLoS Comput Biol 18(5): e1010061. https://doi.org/10.1371/journal.pcbi.1010061
```

### Comparing `hierarch-1.1.3/README.md` & `hierarch-1.1.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -55,8 +55,8 @@
 
 <a name="citation"></a>
 ## Citation
 If hierarch helps you analyze your data, please consider citing it. The manuscript also
 contains a set of simulations validating hierarchical randomization tests in a variety of
 conditions.
 
-Analyzing Nested Experimental Designs – A User-Friendly Resampling Method to Determine Experimental Significance. Rishikesh U. Kulkarni, Catherine L. Wang, Carolyn R. Bertozzi. bioRxiv 2021.06.29.450439; doi: https://doi.org/10.1101/2021.06.29.450439
+Kulkarni RU, Wang CL, Bertozzi CR (2022) Analyzing nested experimental designs—A user-friendly resampling method to determine experimental significance. PLoS Comput Biol 18(5): e1010061. https://doi.org/10.1371/journal.pcbi.1010061
```

### Comparing `hierarch-1.1.3/hierarch/internal_functions.py` & `hierarch-1.1.5/hierarch/internal_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import numpy as np
 from hierarch import numba_overloads
 import numba as nb
-import pandas as pd
 
 assert numba_overloads
 
 
 @nb.jit(nopython=True, cache=True)
 def set_numba_random_state(seed: int):
     """Helper function to set numba's RNG seed.
@@ -37,15 +36,14 @@
     list of 1D arrays
         Values from col: -1 corresponding to the treatment_labels in target column.
     """
 
     ret_list = []
 
     for key in treatment_labels:
-
         # grab values from the data column for each label
         ret_list.append(data[:, -1][np.equal(data[:, col], key)])
 
     return ret_list
 
 
 @nb.jit(nopython=True, cache=True)
@@ -170,34 +168,33 @@
     ub : int
         The upper bound plus one.
 
     Returns
     -------
     int
     """
-    x = np.random.randint(low=2 ** 32)
+    x = np.random.randint(low=0, high=2**32)
     m = ub * x
-    l = np.uint32(m)
-    if l < ub:
+    lower = np.uint32(m)
+    if lower < ub:
         t = -np.uint32(ub)
         if t >= ub:
             t -= ub
             if t >= ub:
                 t %= ub
-        while l < t:
-            x = np.random.randint(low=2 ** 32)
+        while lower < t:
+            x = np.random.randint(low=0, high=2**32)
             m = ub * x
-            l = np.uint32(m)
+            lower = np.uint32(m)
     return m >> 32
 
 
 @nb.jit(nopython=True, cache=True)
 def nb_fast_shuffle(arr):
-    """Reimplementation of Fisher-Yates shuffle using bounded_uint to generate random numbers.
-    """
+    """Reimplementation of Fisher-Yates shuffle using bounded_uint to generate random numbers."""
     i = arr.shape[0] - 1
     while i > 0:
         j = bounded_uint(i + 1)
         arr[i], arr[j] = arr[j], arr[i]
         i -= 1
 
 
@@ -335,15 +332,14 @@
 class GroupbyMean:
     """Class for performing groupby reductions on numpy arrays.
 
     Currently only supports mean reduction.
     """
 
     def __init__(self):
-
         self.cache_dict = {}
 
     def fit(self, reference_data):
         """Fits the class to reference data.
 
         Parameters
         ----------
@@ -352,15 +348,14 @@
 
         """
         self.reference_dict = {}
 
         reference = reference_data[:, :-1]
 
         for i in reversed(range(1, reference.shape[1])):
-
             reference, counts = nb_unique(reference[:, :-1])[0::2]
 
             self.reference_dict[i] = (reference, counts.astype(np.int64))
 
     def transform(self, target, iterations=1):
         """Performs iterative groupby reductions.
 
@@ -374,23 +369,20 @@
         Returns
         -------
         2D numeric array
             Array with the same number of rows as target data, but one fewer column
             for each iteration. Final column values are combined by taking the mean.
         """
         for i in range(iterations):
-
             key = hash((target[:, :-2]).tobytes())
 
             try:
-
                 reduce_at_list, reduce_at_counts = self.cache_dict[key]
 
             except KeyError:
-
                 column = target.shape[1] - 2
 
                 reference, counts = self.reference_dict[column]
 
                 reduce_at_list = class_make_ufunc_list(
                     target[:, :-2], reference, counts
                 )
@@ -398,28 +390,26 @@
                 reduce_at_counts = (
                     np.append(reduce_at_list[1:], target[:, -2].size) - reduce_at_list
                 )
 
                 self.cache_dict[key] = reduce_at_list, reduce_at_counts
 
                 if len(self.cache_dict.keys()) > 50:
-
                     self.cache_dict.pop(list(self.cache_dict)[0])
 
             agg_col = np.add.reduceat(target[:, -1], reduce_at_list) / reduce_at_counts
 
             target = target[reduce_at_list][:, :-1]
 
             target[:, -1] = agg_col
 
         return target
 
     def fit_transform(self, target, reference_data=None, iterations=1):
-        """Combines fit() and transform() for convenience. See those methods for details.
-        """
+        """Combines fit() and transform() for convenience. See those methods for details."""
         if reference_data is None:
             reference_data = target
         self.fit(reference_data)
         return self.transform(target, iterations=iterations)
 
 
 @nb.jit(nopython=True, cache=True)
@@ -455,8 +445,7 @@
 
     else:
         for idx, _ in enumerate(ufunc_list):
             ufunc_list[idx] = i
             i += counts[(reference == target[i]).flatten()].item()
 
     return ufunc_list
-
```

### Comparing `hierarch-1.1.3/hierarch/numba_overloads.py` & `hierarch-1.1.5/hierarch/numba_overloads.py`

 * *Files identical despite different names*

### Comparing `hierarch-1.1.3/hierarch/power.py` & `hierarch-1.1.5/hierarch/power.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import numpy as np
-import scipy.stats as stats
 
 
 class DataSimulator:
     """Class for simulating data for a power analysis.
 
     Parameters
     ----------
@@ -21,19 +20,18 @@
 
     >>> paramlist = [[0, 0], [[stats.norm]]*6, [stats.norm, 0, 1]]
     >>> paramlist = [[0]*2, [stats.norm], [stats.norm]]
 
     """
 
     def __init__(self, paramlist, random_state=None):
-
         self.parameters = paramlist
         self.random_generator = np.random.default_rng(random_state)
 
-    def fit(self, hierarchy=[]):
+    def fit(self, hierarchy):
         """Fit the DataSimulator to a hierarchy.
 
         Parameters
         ----------
         hierarchy : list of ints, optional
             number of clusters in each column, by default []
 
@@ -62,18 +60,25 @@
                [2., 1., 3., 0.],
                [2., 2., 1., 0.],
                [2., 2., 2., 0.],
                [2., 2., 3., 0.],
                [2., 3., 1., 0.],
                [2., 3., 2., 0.],
                [2., 3., 3., 0.]])
-        
+
 
         """
-        self.container = _make_ref_container(hierarchy.copy())
+
+        if len(hierarchy) != len(self.parameters):
+            raise ValueError("hierarchy and parameters should be the same length.")
+
+        try:
+            self.container = _make_ref_container(hierarchy.copy())
+        except TypeError:
+            raise TypeError("hierarchy must be a list of integers.")
 
     def generate(self):
         """Generate a simulated dataset based on specified parameters and hierarchy.
 
         Returns
         -------
         2D numeric
@@ -102,17 +107,22 @@
                [ 2.        ,  2.        ,  2.        ,  0.64816363],
                [ 2.        ,  2.        ,  3.        ,  0.91349805],
                [ 2.        ,  3.        ,  1.        ,  0.17077167],
                [ 2.        ,  3.        ,  2.        ,  1.74043839],
                [ 2.        ,  3.        ,  3.        ,  1.45309889]])
         """
         output = self.container.copy()
-        output[:, -1] = _gen_fake_data(
-            self.container, self.parameters, random_state=self.random_generator
-        )
+        try:
+            output[:, -1] = _gen_fake_data(
+                self.container, self.parameters, random_state=self.random_generator
+            )
+        except AttributeError:
+            raise AttributeError(
+                "parameters must be a list of list of integers or scipy.stats distributions."
+            )
         return output
 
 
 def _gen_fake_data(reference, params, random_state=None):
     """Generates y-values for a design matrix.
 
     Parameters
@@ -131,17 +141,15 @@
         Simulated y-values.
     """
     rng = np.random.default_rng(random_state)
 
     fakedata = np.copy(reference)
     fakedata = fakedata.astype("float64")
     for i in range(reference.shape[1] - 1):
-
         if type(params[i][0]) is not int:
-
             idx, replicates = np.unique(
                 reference[:, : i + 1], return_counts=True, axis=0
             )
             ranlist = []
             if not isinstance(params[i][0], list):
                 for j in range(len(idx)):
                     ranlist.append(params[i][0].rvs(*params[i][1:], random_state=rng))
@@ -164,15 +172,15 @@
 
         if i > 0:
             fakedata[:, i] = fakedata[:, i] + fakedata[:, i - 1]
     else:
         return fakedata[:, -2]
 
 
-def _make_ref_container(samples_per_level=[]):
+def _make_ref_container(samples_per_level):
     """Converts a hierarchy list into a design matrix.
 
     Parameters
     ----------
     samples_per_level : list, optional
         List of ints specifying hierarchy, by default []
```

### Comparing `hierarch-1.1.3/hierarch/resampling.py` & `hierarch-1.1.5/hierarch/resampling.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,22 @@
-import numpy as np
+from functools import lru_cache
 from itertools import cycle
+from typing import Callable, Dict, Generator, Iterable, Union
+
+import numpy as np
 from numba import jit
-from functools import lru_cache
+
 from hierarch.internal_functions import (
-    nb_unique,
+    _repeat,
     id_cluster_counts,
     msp,
-    set_numba_random_state,
-    _repeat,
     nb_fast_shuffle,
     nb_strat_shuffle,
+    nb_unique,
+    set_numba_random_state,
     weights_to_index,
 )
 
 
 class Bootstrapper:
     """Bootstrapper(random_state=None, kind="weights")
 
@@ -206,27 +209,31 @@
 
     """
 
     #: ("weights", "indexes", "bayesian) The three possible arguments that
     # can be provided to the "kind" keyword argument.
     _BOOTSTRAP_ALGORITHMS = tuple(["weights", "indexes", "bayesian"])
 
-    def __init__(self, random_state=None, kind="weights"):
+    def __init__(
+        self,
+        random_state: Union[np.random.Generator, int, None] = None,
+        kind: str = "weights",
+    ) -> None:
 
         self.random_generator = np.random.default_rng(random_state)
         # this is a bit hacky, but we use the numpy generator to seed Numba
         # this makes it both reproducible and thread-safe enough
-        nb_seed = self.random_generator.integers(low=2 ** 32 - 1)
+        nb_seed = self.random_generator.integers(low=2**32 - 1)
         set_numba_random_state(nb_seed)
         if kind in self._BOOTSTRAP_ALGORITHMS:
             self.kind = kind
         else:
             raise KeyError("Invalid 'kind' argument.")
 
-    def fit(self, data, skip=None, y=-1):
+    def fit(self, data: np.ndarray, skip=None, y=-1) -> None:
         """Fit the bootstrapper to the target data.
 
         Parameters
         ----------
         data : 2D array
             Target data. Must be lexicographically sorted.
         sort : bool
@@ -247,18 +254,17 @@
         """
         try:
             if not np.issubdtype(data.dtype, np.number):
                 raise ValueError(
                     "Bootstrapper can only handle numeric datatypes. Please pre-process your data."
                 )
         except AttributeError:
-            print(
+            raise AttributeError(
                 "Bootstrapper can only handle numpy arrays. Please pre-process your data."
             )
-            raise
 
         if skip is not None:
             skip = list(skip)
             for v in iter(skip):
                 if not isinstance(v, int):
                     raise IndexError(
                         "skip values must be integers corresponding to column indices."
@@ -280,15 +286,15 @@
 
         kind = str(self.kind)
 
         self.transform = _bootstrapper_factory(
             tuple(columns_to_resample), cluster_dict, shape, kind
         )
 
-    def transform(self, data, start: int):
+    def transform(self, data: np.ndarray, start: int) -> np.ndarray:
         """Generate a bootstrapped sample from target data.
 
         Parameters
         ----------
         data : 2D array
             Target data. Must be sorted by row.
         start : int
@@ -299,140 +305,95 @@
         2D array
             Array matching target data, but resampled with replacement
             according to "kind" argument.
 
         """
         raise Exception("Use fit() before using transform().")
 
+
 @lru_cache()
-def _bootstrapper_factory(columns_to_resample, clusternum_dict, shape, kind):
-    """Factory function that returns the appropriate transform().
-    """
-    clusternum_dict = tuple(map(np.array, clusternum_dict))
+def _bootstrapper_factory(
+    columns_to_resample: int, clusternum_dict: Dict, shape: int, kind: str
+) -> Callable:
+    """Factory function that returns the appropriate transform()."""
+
+    # these helper functions wrap the distributions so that they take the same arguments
+    @jit(nopython=True)
+    def _multinomial_distribution(weights, idx, v):
+        return np.random.multinomial(v * weights[idx], [1 / v] * v)
+
+    @jit(nopython=True)
+    def _dirichlet_distribution(weights, idx, v):
+        return (
+            np.random.dirichlet([1 for a in range(v.item())], size=None)
+            * weights[idx]
+            * v.item()
+        )
+
+    @jit(nopython=True)
+    def _bootstrap_algorithm(data, start):
+        # at the start, everything is weighted equally
+        weights = np.array([1 for i in clusternum_dict[start]], dtype=_weight_dtype)
+
+        for key in range(start, shape):
+            # fetch design matrix info for current column
+            to_do = clusternum_dict[key]
+            # preallocate the full array for new_weight
+            new_weight = np.empty(to_do.sum(), _weight_dtype)
+            place = 0
+
+            # if not resampling this column, new_weight is the prior column's weights
+            if not columns_to_resample[key]:
+                for idx, v in enumerate(to_do):
+                    new_weight[place : place + v] = np.array(
+                        [weights[idx] for m in range(v.item())]
+                    )
+                    place += v
+
+            # else do a multinomial experiment to generate new_weight
+            else:
+                for idx, v in enumerate(to_do):
+                    # v*weights[idx] carries over weights from previous columns
+                    new_weight[place : place + v] = _dist(weights, idx, v)
+                    place += v
+
+            weights = new_weight
+
+        return weights
+
+    clusternum_dict = tuple(np.array(cluster) for cluster in clusternum_dict)
     columns_to_resample = np.array(columns_to_resample)
 
-    if kind == "weights":
+    if kind in ("weights", "indexes"):
+        _weight_dtype = np.int64
+        _dist = _multinomial_distribution
+
+    elif kind in ("bayesian"):
+        # bayesian bootstrap produces non-integer weights
+        _weight_dtype = np.float64
+        _dist = _dirichlet_distribution
+
+    if kind in ("weights", "bayesian"):
 
         @jit(nopython=True)
         def _bootstrapper_impl(data, start):
             out = data.astype(np.float64)
-            # at the start, everything is weighted equally
-            weights = np.array([1 for i in clusternum_dict[start]])
-
-            for key in range(start, shape):
-                # fetch design matrix info for current column
-                to_do = clusternum_dict[key]
-                # preallocate the full array for new_weight
-                new_weight = np.empty(to_do.sum(), np.int64)
-                place = 0
-
-                # if not resampling this column, new_weight is the prior column's weights
-                if not columns_to_resample[key]:
-                    for idx, v in enumerate(to_do):
-                        new_weight[place : place + v] = np.array(
-                            [weights[idx] for m in range(v.item())]
-                        )
-                        place += v
-
-                # else do a multinomial experiment to generate new_weight
-                else:
-                    for idx, v in enumerate(to_do):
-                        # v*weights[idx] carries over weights from previous columns
-                        new_weight[place : place + v] = np.random.multinomial(
-                            v * weights[idx], [1 / v] * v
-                        )
-                        place += v
-
-                weights = new_weight
-
+            weights = _bootstrap_algorithm(out, start)
             out[:, -1] = out[:, -1] * weights
             return out
 
     elif kind == "indexes":
 
         @jit(nopython=True)
         def _bootstrapper_impl(data, start):
             out = data.astype(np.float64)
-            # at the start, everything is weighted equally
-            weights = np.array([1 for i in clusternum_dict[start]])
-
-            for key in range(start, shape):
-                # fetch design matrix info for current column
-                to_do = clusternum_dict[key]
-                # preallocate the full array for new_weight
-                new_weight = np.empty(to_do.sum(), np.int64)
-                place = 0
-
-                # if not resampling this column, new_weight is the prior column's weights
-                if not columns_to_resample[key]:
-                    for idx, v in enumerate(to_do):
-                        new_weight[place : place + v] = np.array(
-                            [weights[idx] for m in range(v.item())]
-                        )
-                        place += v
-
-                # else do a multinomial experiment to generate new_weight
-                else:
-                    for idx, v in enumerate(to_do):
-                        # v*weights[idx] carries over weights from previous columns
-                        new_weight[place : place + v] = np.random.multinomial(
-                            v * weights[idx], [1 / v] * v
-                        )
-                        place += v
-
-                weights = new_weight
-
+            weights = _bootstrap_algorithm(out, start)
             indexes = weights_to_index(weights)
             return out[indexes]
 
-    elif kind == "bayesian":
-
-        @jit(nopython=True)
-        def _bootstrapper_impl(data, start):
-            out = data.astype(np.float64)
-            # at the start, everything is weighted equally
-            # dype is float64 because weights can be any real number
-            weights = np.array(
-                [1 for i in clusternum_dict[start]], dtype=np.float64
-            )
-
-            for key in range(start, shape):
-                # fetch design matrix info for current column
-                to_do = clusternum_dict[key]
-                # preallocate the full array for new_weight
-                new_weight = np.empty(to_do.sum(), np.float64)
-                place = 0
-
-                # if not resampling this column, new_weight is all 1
-                if not columns_to_resample[key]:
-                    for idx, v in enumerate(to_do):
-                        new_weight[place : place + v] = np.array(
-                            [weights[idx] for m in range(v.item())],
-                            dtype=np.float64,
-                        )
-                        place += v
-
-                # else do a dirichlet experiment to generate new_weight
-                else:
-                    for idx, v in enumerate(to_do):
-                        # multiplying by weights[idx] carries over prior columns
-                        new_weight[place : place + v] = (
-                            np.random.dirichlet(
-                                [1 for a in range(v.item())], size=None
-                            )
-                            * weights[idx]
-                            * v.item()
-                        )
-                        place += v
-
-                weights = new_weight
-
-            out[:, -1] = out[:, -1] * weights
-            return out
-
     else:
         raise KeyError(
             "No such bootstrapping algorithm. kind must be 'weights' or 'indexes' or 'bayesian'"
         )
 
     return _bootstrapper_impl
 
@@ -441,15 +402,15 @@
 
     """Class for performing cluster-aware permutation on a target column.
 
     Parameters
     ----------
     random_state : int or numpy.random.Generator instance, optional
         Seedable for reproducibility, by default None
-        
+
     Examples
     --------
     When the column to resample is the first column, Permuter performs an
     ordinary shuffle.
 
     >>> from hierarch.power import DataSimulator
     >>> from hierarch.internal_functions import GroupbyMean
@@ -510,29 +471,31 @@
            [1., 3., 1.],
            [2., 2., 1.],
            [2., 1., 1.],
            [2., 3., 1.]])
 
     Exact within-cluster permutations are not implemented, but there are typically
     too many to be worth attempting.
-    
+
     >>> permute = Permuter(random_state=2)
     >>> permute.fit(test, col_to_permute=1, exact=True)
     Traceback (most recent call last):
         ...
     NotImplementedError: Exact permutation only available for col_to_permute = 0.
     """
 
-    def __init__(self, random_state=None):
+    def __init__(
+        self, random_state: Union[np.random.Generator, int, None] = None
+    ) -> None:
         self.random_generator = np.random.default_rng(random_state)
         if random_state is not None:
-            nb_seed = self.random_generator.integers(low=2 ** 32)
+            nb_seed = self.random_generator.integers(low=2**32)
             set_numba_random_state(nb_seed)
 
-    def fit(self, data, col_to_permute: int, exact=False):
+    def fit(self, data: np.ndarray, col_to_permute: int, exact: bool = False) -> None:
         """Fit the permuter to the target data.
 
         Parameters
         ----------
         data : 2D numeric ndarray
             Target data.
         col_to_permute : int
@@ -581,15 +544,15 @@
                 col_values = data[:, col_to_permute][indexes]
                 col_values = tuple(col_values.tolist())
                 counts = tuple(counts.tolist())
                 self.transform = _random_repeat_return(
                     col_to_permute, col_values, keys, counts
                 )
 
-    def transform(self, data):
+    def transform(self, data: np.ndarray) -> np.ndarray:
         """Permute target column in-place.
 
         Parameters
         ----------
         data : 2D numeric ndarray
             Target data.
 
@@ -597,41 +560,46 @@
         -------
         data : 2D numeric ndarray
             Original data with target column shuffled, in a stratified fashion if necessary.
         """
 
         # this method is defined on the fly in fit() based one of the
         # four static methods defined below
-        raise Exception("Use fit() before calling transform.")
+        raise Exception("Use fit() before using transform().")
 
-def _exact_return(col_to_permute, generator):
-    """Transformer when exact is True and permutations are unrestricted.
-    """
+
+def _exact_return(
+    col_to_permute: int, generator: Generator[Iterable, None, None]
+) -> Callable:
+    """Transformer when exact is True and permutations are unrestricted."""
 
     def _exact_return_impl(data):
         data[:, col_to_permute] = next(generator)
         return data
 
     return _exact_return_impl
 
-def _exact_repeat_return(col_to_permute, generator, counts):
+
+def _exact_repeat_return(
+    col_to_permute: int, generator: Generator[Iterable, None, None], counts: Iterable
+) -> Callable:
     """Transformer when exact is True and permutations are restricted by
     repetition of treated entities.
     """
 
     def _rep_iter_return_impl(data):
         data[:, col_to_permute] = _repeat(tuple(next(generator)), counts)
         return data
 
     return _rep_iter_return_impl
 
+
 @lru_cache()
-def _random_return(col_to_permute, keys):
-    """Transformer when exact is False and repetition is not required.
-    """
+def _random_return(col_to_permute: int, keys: Iterable) -> Callable:
+    """Transformer when exact is False and repetition is not required."""
 
     if col_to_permute == 0:
 
         @jit(nopython=True)
         def _random_return_impl(data):
             nb_fast_shuffle(data[:, col_to_permute])
             return data
@@ -641,18 +609,20 @@
         @jit(nopython=True)
         def _random_return_impl(data):
             nb_strat_shuffle(data[:, col_to_permute], keys)
             return data
 
     return _random_return_impl
 
+
 @lru_cache()
-def _random_repeat_return(col_to_permute, col_values, keys, counts):
-    """Transformer when exact is False and repetition is required.
-    """
+def _random_repeat_return(
+    col_to_permute: int, col_values: Iterable, keys: Iterable, counts: Iterable
+) -> Callable:
+    """Transformer when exact is False and repetition is required."""
     col_values = np.array(col_values)
     counts = np.array(counts)
     if col_to_permute == 0:
 
         @jit(nopython=True)
         def _random_repeat_return_impl(data):
             shuffled_col_values = col_values.copy()
@@ -666,8 +636,7 @@
         def _random_repeat_return_impl(data):
             shuffled_col_values = col_values.copy()
             nb_strat_shuffle(shuffled_col_values, keys)
             data[:, col_to_permute] = np.repeat(shuffled_col_values, counts)
             return data
 
     return _random_repeat_return_impl
-
```

### Comparing `hierarch-1.1.3/hierarch/stats.py` & `hierarch-1.1.5/hierarch/stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,20 +24,18 @@
     -------
     2D array of float64s
         An array identical to data, but all elements that cannot be cast
         to np.float64s replaced with integer values.
     """
     # don't want to overwrite data
     if isinstance(data, np.ndarray):
-
         encoded = data.copy()
 
     # coerce dataframe to numpy array
     elif isinstance(data, pd.DataFrame):
-
         encoded = data.to_numpy()
 
     for idx, v in enumerate(encoded.T):
         # attempt to cast array as floats
         try:
             encoded = encoded.astype(np.float64)
             # if we can cast the array as floats, encoding is complete
@@ -48,38 +46,39 @@
             try:
                 encoded[:, idx] = encoded[:, idx].astype(np.float64)
             # if we still can't, encode that column
             except ValueError:
                 encoded[:, idx] = np.unique(v, return_inverse=True)[1]
     # stable sort sort the output by row
     encoded = np.unique(encoded, axis=0)
+    encoded = encoded.astype(np.float64)
 
     return encoded
 
 
 @jit(nopython=True, cache=True)
 def studentized_covariance(x, y):
     """Studentized sample covariance between two variables.
 
     Sample covariance between two variables divided by standard error of
-    sample covariance. Uses a bias-corrected approximation of standard error. 
+    sample covariance. Uses a bias-corrected approximation of standard error.
     This computes an approximately pivotal test statistic.
 
     Parameters
     ----------
     x, y: numeric array-likes
 
     Returns
     -------
     float64
         Studentized covariance.
 
     Examples
     --------
-    >>> x = np.array([[0, 0, 0, 0, 0, 1, 1, 1, 1, 1], 
+    >>> x = np.array([[0, 0, 0, 0, 0, 1, 1, 1, 1, 1],
     ...               [1, 2, 3, 4, 5, 2, 3, 4, 5, 6]])
     >>> x.T
     array([[0, 1],
            [0, 2],
            [0, 3],
            [0, 4],
            [0, 5],
@@ -89,15 +88,15 @@
            [1, 5],
            [1, 6]])
     >>> studentized_covariance(x.T[:,0], x.T[:,1])
     1.0039690353154482
 
     This is approximately equal to the t-statistic.
 
-    >>> import scipy.stats as stats    
+    >>> import scipy.stats as stats
     >>> a = np.array([2, 3, 4, 5, 6])
     >>> b = np.array([1, 2, 3, 4, 5])
     >>> stats.ttest_ind(a, b, equal_var=False)[0]
     1.0
 
     """
     n = len(x)
@@ -106,15 +105,15 @@
     numerator = bivar_central_moment(x, y, pow=1, ddof=1)
 
     # the denominator is the sample standard deviation of the sample covariance, aka
     # the standard error of sample covariance. the denominator has three terms.
 
     # first term is the second symmetric bivariate central moment. an approximate
     # bias correction of n - root(2) is applied
-    denom_1 = bivar_central_moment(x, y, pow=2, ddof=2 ** 0.5)
+    denom_1 = bivar_central_moment(x, y, pow=2, ddof=2**0.5)
 
     # second term is the product of the standard deviations of x and y over n - 1.
     # this term rapidly goes to 0 as n goes to infinity
     denom_2 = (
         bivar_central_moment(x, x, pow=1, ddof=1)
         * bivar_central_moment(y, y, pow=1, ddof=1)
     ) / (n - 1)
@@ -161,16 +160,16 @@
     This uses the same calculation as scipy's ttest function.
 
     >>> import scipy.stats as stats
     >>> a = np.array([1, 2, 3, 4, 5])
     >>> b = np.array([10, 11, 12, 13, 14])
     >>> stats.ttest_ind(a, b, equal_var=False)[0]
     -9.0
-    
-    
+
+
     Notes
     ----------
     Details on the validity of this test statistic can be found in
     "Studentized permutation tests for non-i.i.d. hypotheses and the
     generalized Behrens-Fisher problem" by Arnold Janssen.
     https://doi.org/10.1016/S0167-7152(97)00043-6.
 
@@ -197,15 +196,15 @@
 
     Parameters
     ----------
     treatment_col : 1D tuple
         Treatment column in the design matrix. Needs to be a tuple
         so lru_cache can work.
     compare : {'means', 'corr'}
-        Specifies test statistic to return. 
+        Specifies test statistic to return.
 
     Returns
     -------
     function
         Functions that come out of _test_stat_factory take the treatment
         column of a design matrix and the dependent variable column to compute
         a test statistic.
@@ -288,15 +287,15 @@
 
     Returns
     -------
     float64
         p-value for the hypothesis test
 
     list
-        Empirical null distribution used to calculate the p-value        
+        Empirical null distribution used to calculate the p-value
 
     Raises
     ------
     TypeError
         Raised if input data is not ndarray or DataFrame.
     KeyError
         If comparison is a string, it must be in the TEST_STATISTICS dictionary.
@@ -319,35 +318,35 @@
 
     >>> hypothesis_test(data, treatment_col=0,
     ...                 bootstraps=1000, permutations='all',
     ...                 random_state=1)
     0.013714285714285714
 
     By setting compare to "means", this function will perform a permutation t-test.
-    "corr", which is based on a studentized covariance test statistic, should give the 
-    same or a very similar p-value to the permutation t-test for datasets with two 
+    "corr", which is based on a studentized covariance test statistic, should give the
+    same or a very similar p-value to the permutation t-test for datasets with two
     treatment groups.
 
     >>> hypothesis_test(data, treatment_col=0, compare='means',
     ...                 bootstraps=1000, permutations='all',
     ...                 random_state=1)
     0.013714285714285714
 
-    This test can handle data with multiple treatment groups that have a 
+    This test can handle data with multiple treatment groups that have a
     hypothesized linear relationship.
-    
+
     >>> paramlist = [[0, 2/3, 4/3, 2], [stats.norm], [stats.norm]]
     >>> hierarchy = [4, 2, 3]
     >>> datagen = DataSimulator(paramlist, random_state=2)
     >>> datagen.fit(hierarchy)
     >>> data = datagen.generate()
     >>> print(data.shape)
     (24, 4)
 
-    There are 2,520 possible permutations, so choose a subset. 
+    There are 2,520 possible permutations, so choose a subset.
 
     >>> hypothesis_test(data, treatment_col=0,
     ...                 bootstraps=100, permutations=1000,
     ...                 random_state=1)
     0.0067
 
 
@@ -383,15 +382,16 @@
     elif not isinstance(permutations, int) or permutations < 1:
         raise TypeError("permutations must be 'all' or an integer greater than 0")
 
     # initialize and fit the bootstrapper to the data
     bootstrapper = Bootstrapper(random_state=rng, kind=kind)
     bootstrapper.fit(data, skip=skip)
 
-    # fetch test statistic from dictionary or, if given a custom test statistic, make sure it is callable
+    # fetch test statistic from dictionary or, if given a custom test
+    # statistic, make sure it is callable
     if isinstance(compare, str):
         teststat = _test_stat_factory(tuple(data[:, treatment_col].tolist()), compare)
     elif callable(compare):
         teststat = compare
     else:
         raise AttributeError("Custom test statistics must be callable.")
 
@@ -539,16 +539,17 @@
         Bootstrapper algorithm. See Bootstrapper class, by default "weights"
     seed : int or numpy.random.Generator instance, optional
         Seedable for reproducibility, by default None
 
     Returns
     -------
     ndarray
-        numpy ndarray with col 0, 1 corresponding to treatment labels, col 2 corresponding to an uncorrected p-value,
-        and col 3 corresponding to a corrected p-value if a correction was specified.
+        numpy ndarray with col 0, 1 corresponding to treatment labels, col 2 corresponding
+        to an uncorrected p-value, and col 3 corresponding to a corrected p-value if a
+        correction was specified.
 
     Raises
     ------
     KeyError
         Raised if passed correction is not valid.
     TypeError
         Raised if input data is not ndarray or DataFrame.
@@ -608,16 +609,16 @@
            [ 4.        ,  2.        ,  1.        , -0.04362144],
            [ 4.        ,  2.        ,  2.        , -0.91632938],
            [ 4.        ,  2.        ,  3.        , -0.06984773],
            [ 4.        ,  3.        ,  1.        ,  0.64219601],
            [ 4.        ,  3.        ,  2.        ,  0.58229922],
            [ 4.        ,  3.        ,  3.        ,  0.04042133]])
 
-    There are six total comparisons that can be made. Condition 1 and 2 are in the first two columns and the p-values are in the
-    final column.
+    There are six total comparisons that can be made. Condition 1 and 2 are in the first
+    two columns and the p-values are in the final column.
 
     >>> multi_sample_test(data, treatment_col=0, hypotheses="all",
     ...                   correction=None, bootstraps=1000,
     ...                   permutations="all", random_state=111)
       Condition 1 Condition 2 p-value
     0         2.0         3.0  0.0355
     1         1.0         3.0  0.0394
@@ -636,15 +637,15 @@
       Condition 1 Condition 2 p-value Corrected p-value
     0         2.0         3.0  0.0355            0.0814
     1         1.0         3.0  0.0394            0.0814
     2         3.0         4.0  0.0407            0.0814
     3         2.0         4.0  0.1477           0.22155
     4         1.0         2.0  0.4022            0.4559
     5         1.0         4.0  0.4559            0.4559
-    
+
     Perhaps the experimenter is not interested in every pairwise comparison - perhaps
     condition 2 is a control that all other conditions are meant to be compared to.
     The comparisons of interest can be specified using a list.
 
     >>> tests = [[2.0, 1.0], [2.0, 3.0], [2.0, 4.0]]
     >>> multi_sample_test(data, treatment_col=0, hypotheses=tests,
     ...                   correction='fdr', bootstraps=1000,
@@ -660,16 +661,17 @@
     MULTIPLE_COMPARISONS_CORRECTIONS = {
         "fdr": _false_discovery_adjust,
     }
     if correction is not None:
         try:
             multiple_correction = MULTIPLE_COMPARISONS_CORRECTIONS[correction]
         except KeyError:
-            print(correction + " is not a valid multiple comparisons correction.")
-            raise
+            raise KeyError(
+                correction + " is not a valid multiple comparisons correction."
+            )
 
     random_state = np.random.default_rng(random_state)
 
     # coerce data into an object array
     if isinstance(data_array, pd.DataFrame):
         if isinstance(treatment_col, str):
             treatment_col = data_array.columns.get_loc(treatment_col)
@@ -859,15 +861,14 @@
     compare="corr",
     skip=None,
     bootstraps=50,
     permutations=100,
     kind="bayesian",
     random_state=None,
 ):
-
     """Compute a confidence inverval via test inversion.
 
     Confidence interval can be calculated by inverting the acceptance region of a hypothesis test.
     Using a test statistic that is approximately normally distributed under the null makes this
     much easier.
 
     Parameters
@@ -883,15 +884,15 @@
     interval : float, optional
         Percentage value indicating the confidence interval's coverage, by default 95
     iterations : int, optional
         Maximum number of times the interval will be refined, by default 7
     tolerance : float, optional
         If the delta between the current bounds and the target interval is less than
         this value, refinement will stop. Setting this number too close to the Monte Carlo
-        error of the underlying hypothesis test will have a negative effect on coverage. 
+        error of the underlying hypothesis test will have a negative effect on coverage.
     compare : str, optional
         The test statistic to use to perform the hypothesis test, by default "corr"
         which automatically calls the studentized covariance test statistic.
     skip : list of ints, optional
         Columns to skip in the bootstrap. Skip columns that were sampled
         without replacement from the prior column, by default None
     bootstraps : int, optional
@@ -912,15 +913,15 @@
 
     Notes
     -----
     While the Efron bootstrap is the default in most of hierarch's statistical functions,
     using the Bayesian bootstrap here helps get tighter confidence intervals with the
     correct coverage without having to massively increase the number of resamples.
 
-    The inversion procedure performed by this function is described in detail in 
+    The inversion procedure performed by this function is described in detail in
     "Randomization, Bootstrap and Monte Carlo Methods in Biology" by Bryan FJ Manly.
     https://doi.org/10.1201/9781315273075.
 
     Examples
     --------
     Specify the parameters of a dataset with a difference of means of 2.
 
@@ -930,15 +931,15 @@
     >>> hierarchy = [2, 4, 3]
     >>> datagen = DataSimulator(paramlist, random_state=2)
     >>> datagen.fit(hierarchy)
     >>> data = datagen.generate()
     >>> print(data.shape)
     (24, 4)
 
-    >>> confidence_interval(data, treatment_col=0, interval=95, 
+    >>> confidence_interval(data, treatment_col=0, interval=95,
     ...    bootstraps=1000, permutations='all', random_state=1)
     (1.314807450602109, 6.124658302189696)
 
     The true difference is 2, which falls within the interval. We can examine
     the p-value for the corresponding dataset:
 
     >>> from hierarch.stats import hypothesis_test
@@ -946,29 +947,29 @@
     ...                 bootstraps=1000, permutations='all',
     ...                 random_state=1)
     0.013714285714285714
 
     This suggests that while the 95% confidence interval does not contain 0, the 99.5%
     confidence interval should.
 
-    >>> confidence_interval(data, treatment_col=0, interval=99.5, 
+    >>> confidence_interval(data, treatment_col=0, interval=99.5,
     ...    bootstraps=1000, permutations='all', random_state=1)
     (-0.12320618535452432, 7.56267193814634)
 
     A permutation t-test can be used to generate the null distribution by
     specifying compare = "means". This should return the same or a very
     similar interval.
 
-    >>> confidence_interval(data, treatment_col=0, interval=95, 
-    ...    compare='means', bootstraps=1000, 
+    >>> confidence_interval(data, treatment_col=0, interval=95,
+    ...    compare='means', bootstraps=1000,
     ...    permutations='all', random_state=1)
     (1.314807450602109, 6.124658302189696)
 
     Setting compare = "corr" will generate a confidence interval for the slope
-    in a regression equation.     
+    in a regression equation.
 
     >>> paramlist = [[0, 1, 2, 3], [stats.norm], [stats.norm]]
     >>> hierarchy = [4, 4, 3]
     >>> datagen = DataSimulator(paramlist, random_state=2)
     >>> datagen.fit(hierarchy)
     >>> data = datagen.generate()
 
@@ -1004,15 +1005,16 @@
         test[:, treatment_col], test[:, -1]
     ) / bivar_central_moment(test[:, treatment_col], test[:, treatment_col])
 
     # subtract the observed covariance out
     correction = start_slope * null_imposed_data[:, treatment_col]
     null_imposed_data[:, -1] -= correction
 
-    # compute the null distribution for the null hypothesis that the true effect size is equal to the MLE
+    # compute the null distribution for the null hypothesis that the true effect
+    # size is equal to the MLE
     _, null = hypothesis_test(
         null_imposed_data,
         treatment_col,
         skip=skip,
         bootstraps=bootstraps,
         permutations=permutations,
         kind=kind,
@@ -1036,15 +1038,14 @@
 
     if compare == "means":
         alternative_lower, alternative_upper = "greater", "less"
     else:
         alternative_lower, alternative_upper = "less", "greater"
 
     for i in range(iterations):
-
         bound_imposed_data = null_imposed_data.copy()
         bound_imposed_data[:, -1] += (current_lower) * bound_imposed_data[
             :, treatment_col
         ]
         current_p, null = hypothesis_test(
             bound_imposed_data,
             treatment_col,
@@ -1071,15 +1072,14 @@
         warn(
             " ".join(["lower tail:", str(current_p), "failed to converge"]),
             ConvergenceWarning,
             stacklevel=2,
         )
 
     for i in range(iterations):
-
         bound_imposed_data = null_imposed_data.copy()
         bound_imposed_data[:, -1] += (current_upper) * bound_imposed_data[
             :, treatment_col
         ]
         current_p, null = hypothesis_test(
             bound_imposed_data,
             treatment_col,
@@ -1150,15 +1150,15 @@
     >>> datagen = DataSimulator(paramlist, random_state=2)
     >>> datagen.fit(hierarchy)
     >>> data = datagen.generate()
     >>> null = np.array(hypothesis_test(data, 0, return_null=True, random_state=5)[1])
     >>> _compute_interval(null, data, 0, 0.025)
     -1.6381035977603908
 
-    The test statistic distribution is essentially symmetric about 0. 
+    The test statistic distribution is essentially symmetric about 0.
 
     >>> _compute_interval(null, data, 0, 0.975)
     1.6560744165754229
 
     """
     x = null_data[:, treatment_col]
     y = null_data[:, -1]
@@ -1201,15 +1201,15 @@
     >>> _cov_std_error(x, y)
     0.32587563558526406
 
     """
     n = len(x)
     # first term is the second symmetric bivariate central moment. an approximate
     # bias correction of n - root(2) is applied
-    denom_1 = bivar_central_moment(x, y, pow=2, ddof=2 ** 0.5)
+    denom_1 = bivar_central_moment(x, y, pow=2, ddof=2**0.5)
 
     # second term is the product of the standard deviations of x and y over n - 1.
     # this term rapidly goes to 0 as n goes to infinity
     denom_2 = (
         bivar_central_moment(x, x, pow=1, ddof=1)
         * bivar_central_moment(y, y, pow=1, ddof=1)
     ) / (n - 1)
```

