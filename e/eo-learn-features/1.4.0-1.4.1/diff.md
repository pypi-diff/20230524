# Comparing `tmp/eo-learn-features-1.4.0.tar.gz` & `tmp/eo-learn-features-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eo-learn-features-1.4.0.tar", last modified: Fri Jan 20 10:59:14 2023, max compression
+gzip compressed data, was "eo-learn-features-1.4.1.tar", last modified: Tue Mar 14 10:33:03 2023, max compression
```

## Comparing `eo-learn-features-1.4.0.tar` & `eo-learn-features-1.4.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-01-20 10:59:14.402053 eo-learn-features-1.4.0/
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1745 2023-01-20 10:59:14.000000 eo-learn-features-1.4.0/LICENSE
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       84 2022-06-13 14:43:39.000000 eo-learn-features-1.4.0/MANIFEST.in
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1724 2023-01-20 10:59:14.398053 eo-learn-features-1.4.0/PKG-INFO
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      246 2021-04-09 13:35:14.000000 eo-learn-features-1.4.0/README.md
-drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-01-20 10:59:14.378053 eo-learn-features-1.4.0/eo_learn_features.egg-info/
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1724 2023-01-20 10:59:14.000000 eo-learn-features-1.4.0/eo_learn_features.egg-info/PKG-INFO
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      770 2023-01-20 10:59:14.000000 eo-learn-features-1.4.0/eo_learn_features.egg-info/SOURCES.txt
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)        1 2023-01-20 10:59:14.000000 eo-learn-features-1.4.0/eo_learn_features.egg-info/dependency_links.txt
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)        1 2021-04-28 12:52:24.000000 eo-learn-features-1.4.0/eo_learn_features.egg-info/not-zip-safe
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      104 2023-01-20 10:59:14.000000 eo-learn-features-1.4.0/eo_learn_features.egg-info/requires.txt
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)        8 2023-01-20 10:59:14.000000 eo-learn-features-1.4.0/eo_learn_features.egg-info/top_level.txt
-drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-01-20 10:59:14.378053 eo-learn-features-1.4.0/eolearn/
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       65 2022-05-03 09:13:51.000000 eo-learn-features-1.4.0/eolearn/__init__.py
-drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-01-20 10:59:14.398053 eo-learn-features-1.4.0/eolearn/features/
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1262 2023-01-20 10:41:16.000000 eo-learn-features-1.4.0/eolearn/features/__init__.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     3707 2023-01-20 10:41:16.000000 eo-learn-features-1.4.0/eolearn/features/bands_extraction.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     6590 2023-01-20 10:41:16.000000 eo-learn-features-1.4.0/eolearn/features/blob.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     6705 2023-01-20 10:41:16.000000 eo-learn-features-1.4.0/eolearn/features/clustering.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     4377 2023-01-20 10:41:16.000000 eo-learn-features-1.4.0/eolearn/features/doubly_logistic_approximation.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)    12809 2023-01-20 10:41:16.000000 eo-learn-features-1.4.0/eolearn/features/feature_manipulation.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     8606 2023-01-20 10:41:16.000000 eo-learn-features-1.4.0/eolearn/features/haralick.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     5260 2023-01-20 10:41:16.000000 eo-learn-features-1.4.0/eolearn/features/hog.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)    30035 2023-01-20 10:41:16.000000 eo-learn-features-1.4.0/eolearn/features/interpolation.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     2529 2023-01-20 10:41:16.000000 eo-learn-features-1.4.0/eolearn/features/local_binary_pattern.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)    17054 2023-01-20 10:41:16.000000 eo-learn-features-1.4.0/eolearn/features/radiometric_normalization.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)    10942 2023-01-20 10:41:16.000000 eo-learn-features-1.4.0/eolearn/features/temporal_features.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     8311 2023-01-20 10:41:16.000000 eo-learn-features-1.4.0/eolearn/features/utils.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      104 2022-06-14 07:56:54.000000 eo-learn-features-1.4.0/requirements.txt
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       38 2023-01-20 10:59:14.402053 eo-learn-features-1.4.0/setup.cfg
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     2541 2022-10-06 11:16:15.000000 eo-learn-features-1.4.0/setup.py
+drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-03-14 10:33:03.083695 eo-learn-features-1.4.1/
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1745 2023-03-14 10:33:02.000000 eo-learn-features-1.4.1/LICENSE
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       84 2022-06-13 14:43:39.000000 eo-learn-features-1.4.1/MANIFEST.in
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1824 2023-03-14 10:33:03.083695 eo-learn-features-1.4.1/PKG-INFO
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      346 2023-03-14 10:22:12.000000 eo-learn-features-1.4.1/README.md
+drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-03-14 10:33:03.063695 eo-learn-features-1.4.1/eo_learn_features.egg-info/
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1824 2023-03-14 10:33:02.000000 eo-learn-features-1.4.1/eo_learn_features.egg-info/PKG-INFO
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      770 2023-03-14 10:33:02.000000 eo-learn-features-1.4.1/eo_learn_features.egg-info/SOURCES.txt
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)        1 2023-03-14 10:33:02.000000 eo-learn-features-1.4.1/eo_learn_features.egg-info/dependency_links.txt
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)        1 2021-04-28 12:52:24.000000 eo-learn-features-1.4.1/eo_learn_features.egg-info/not-zip-safe
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      122 2023-03-14 10:33:02.000000 eo-learn-features-1.4.1/eo_learn_features.egg-info/requires.txt
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)        8 2023-03-14 10:33:02.000000 eo-learn-features-1.4.1/eo_learn_features.egg-info/top_level.txt
+drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-03-14 10:33:03.063695 eo-learn-features-1.4.1/eolearn/
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       65 2022-05-03 09:13:51.000000 eo-learn-features-1.4.1/eolearn/__init__.py
+drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-03-14 10:33:03.083695 eo-learn-features-1.4.1/eolearn/features/
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1262 2023-03-14 10:22:12.000000 eo-learn-features-1.4.1/eolearn/features/__init__.py
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     3613 2023-03-14 10:22:12.000000 eo-learn-features-1.4.1/eolearn/features/bands_extraction.py
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     6353 2023-03-14 10:22:12.000000 eo-learn-features-1.4.1/eolearn/features/blob.py
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     6739 2023-03-14 10:22:12.000000 eo-learn-features-1.4.1/eolearn/features/clustering.py
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     4415 2023-03-14 10:22:12.000000 eo-learn-features-1.4.1/eolearn/features/doubly_logistic_approximation.py
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)    12732 2023-03-14 10:22:12.000000 eo-learn-features-1.4.1/eolearn/features/feature_manipulation.py
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     8619 2023-03-14 10:22:12.000000 eo-learn-features-1.4.1/eolearn/features/haralick.py
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     5255 2023-03-14 10:22:12.000000 eo-learn-features-1.4.1/eolearn/features/hog.py
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)    29787 2023-03-14 10:22:12.000000 eo-learn-features-1.4.1/eolearn/features/interpolation.py
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     2524 2023-03-14 10:22:12.000000 eo-learn-features-1.4.1/eolearn/features/local_binary_pattern.py
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)    17086 2023-03-14 10:22:12.000000 eo-learn-features-1.4.1/eolearn/features/radiometric_normalization.py
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)    10626 2023-03-14 10:22:12.000000 eo-learn-features-1.4.1/eolearn/features/temporal_features.py
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     7379 2023-03-14 10:22:12.000000 eo-learn-features-1.4.1/eolearn/features/utils.py
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      122 2023-03-14 10:22:12.000000 eo-learn-features-1.4.1/requirements.txt
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       38 2023-03-14 10:33:03.083695 eo-learn-features-1.4.1/setup.cfg
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     2541 2022-10-06 11:16:15.000000 eo-learn-features-1.4.1/setup.py
```

### Comparing `eo-learn-features-1.4.0/LICENSE` & `eo-learn-features-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `eo-learn-features-1.4.0/PKG-INFO` & `eo-learn-features-1.4.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: eo-learn-features
-Version: 1.4.0
+Version: 1.4.1
 Summary: A collection of feature manipulation EOTasks and utilities
 Home-page: https://github.com/sentinel-hub/eo-learn
 Author: Sinergise EO research team
 Author-email: eoresearch@sinergise.com
 License: MIT
 Project-URL: Documentation, https://eo-learn.readthedocs.io
 Project-URL: Source Code, https://github.com/sentinel-hub/eo-learn
 Project-URL: Bug Tracker, https://github.com/sentinel-hub/eo-learn/issues
 Project-URL: Forum, https://forum.sentinel-hub.com
 Description: # eolearn.features subpackage
         
         A collection of utilities for extracting data properties and feature manipulation.
         
-        For more information on the package content, visit [readthedocs](https://eo-learn.readthedocs.io/en/latest/eolearn.features.html).
+        For more information about the module visit [readthedocs](https://eo-learn.readthedocs.io/en/latest/reference/eolearn.features.html), or see the [module task index](https://eo-learn.readthedocs.io/en/latest/eotasks.html#features).
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eo-learn-features-1.4.0/eo_learn_features.egg-info/PKG-INFO` & `eo-learn-features-1.4.1/eo_learn_features.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: eo-learn-features
-Version: 1.4.0
+Version: 1.4.1
 Summary: A collection of feature manipulation EOTasks and utilities
 Home-page: https://github.com/sentinel-hub/eo-learn
 Author: Sinergise EO research team
 Author-email: eoresearch@sinergise.com
 License: MIT
 Project-URL: Documentation, https://eo-learn.readthedocs.io
 Project-URL: Source Code, https://github.com/sentinel-hub/eo-learn
 Project-URL: Bug Tracker, https://github.com/sentinel-hub/eo-learn/issues
 Project-URL: Forum, https://forum.sentinel-hub.com
 Description: # eolearn.features subpackage
         
         A collection of utilities for extracting data properties and feature manipulation.
         
-        For more information on the package content, visit [readthedocs](https://eo-learn.readthedocs.io/en/latest/eolearn.features.html).
+        For more information about the module visit [readthedocs](https://eo-learn.readthedocs.io/en/latest/reference/eolearn.features.html), or see the [module task index](https://eo-learn.readthedocs.io/en/latest/eotasks.html#features).
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eo-learn-features-1.4.0/eo_learn_features.egg-info/SOURCES.txt` & `eo-learn-features-1.4.1/eo_learn_features.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eo-learn-features-1.4.0/eolearn/features/__init__.py` & `eo-learn-features-1.4.1/eolearn/features/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,8 +34,8 @@
 )
 from .temporal_features import (
     AddMaxMinNDVISlopeIndicesTask,
     AddMaxMinTemporalIndicesTask,
     AddSpatioTemporalFeaturesTask,
 )
 
-__version__ = "1.4.0"
+__version__ = "1.4.1"
```

### Comparing `eo-learn-features-1.4.0/eolearn/features/bands_extraction.py` & `eo-learn-features-1.4.1/eolearn/features/bands_extraction.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 """
 A collection of bands extraction EOTasks
 
-Credits:
-Copyright (c) 2017-2022 Matej Aleksandrov, Matej Batič, Grega Milčinski, Domagoj Korais, Matic Lubej (Sinergise)
-Copyright (c) 2017-2022 Žiga Lukšič, Devis Peressutti, Nejc Vesel, Jovan Višnjić, Anže Zupanc (Sinergise)
+Copyright (c) 2017- Sinergise and contributors
+For the full list of contributors, see the CREDITS file in the root directory of this source tree.
 
-This source code is licensed under the MIT license found in the LICENSE
-file in the root directory of this source tree.
+This source code is licensed under the MIT license, see the LICENSE file in the root directory of this source tree.
 """
 from __future__ import annotations
 
 from typing import List, Optional, Tuple
 
 import numpy as np
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `eo-learn-features-1.4.0/eolearn/features/blob.py` & `eo-learn-features-1.4.1/eolearn/features/blob.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 """
 Module for computing blobs in EOPatch
 
-Credits:
-Copyright (c) 2018-2019 Hugo Fournier (Magellium)
-Copyright (c) 2017-2022 Matej Aleksandrov, Devis Peressutti, Žiga Lukšič (Sinergise)
+Copyright (c) 2017- Sinergise and contributors
+For the full list of contributors, see the CREDITS file in the root directory of this source tree.
 
-This source code is licensed under the MIT license found in the LICENSE
-file in the root directory of this source tree.
+This source code is licensed under the MIT license, see the LICENSE file in the root directory of this source tree.
 """
 from __future__ import annotations
 
 from math import sqrt
 from typing import Any, Callable
 
 import numpy as np
@@ -39,35 +37,27 @@
 
     :param feature: A feature that will be used and a new feature name where data will be saved. If new name is not
                     specified it will be saved with name '<feature_name>_BLOB'
 
                     Example: (FeatureType.DATA, 'bands') or (FeatureType.DATA, 'bands', 'blob')
 
     :param blob_object: Name of the blob method to use
-    :type blob_object: skimage.feature.blob_*
     :param blob_parameters: List of parameters to be passed to the blob function. Below is a list of such parameters.
     :param min_sigma: The minimum standard deviation for Gaussian Kernel. Keep this low to detect smaller blobs
-    :type min_sigma: float
     :param max_sigma: The maximum standard deviation for Gaussian Kernel. Keep this high to detect larger blobs
-    :type max_sigma: float
     :param threshold: The absolute lower bound for scale space maxima. Local maxima smaller than thresh are ignored.
                         Reduce this to detect blobs with less intensity
-    :type threshold: float
     :param overlap: A value between 0 and 1. If the area of two blobs overlaps by a fraction greater than threshold,
                     the smaller blob is eliminated
-    :type overlap: float
     :param num_sigma: For ‘Log’ and ‘DoH’: The number of intermediate values of standard deviations to consider between
                         min_sigma and max_sigma
-    :type num_sigma: int
     :param log_scale: For ‘Log’ and ‘DoH’: If set intermediate values of standard deviations are interpolated using a
                         logarithmic scale to the base 10. If not, linear interpolation is used
-    :type log_scale: bool
     :param sigma_ratio: For ‘DoG’: The ratio between the standard deviation of Gaussian Kernels used for computing the
                         Difference of Gaussians
-    :type sigma_ratio: float
     """
 
     def __init__(self, feature: SingleFeatureSpec, blob_object: Callable, **blob_parameters: Any):
         self.feature_parser = self.get_feature_parser(feature)
 
         self.blob_object = blob_object
         self.blob_parameters = blob_parameters
```

### Comparing `eo-learn-features-1.4.0/eolearn/features/clustering.py` & `eo-learn-features-1.4.1/eolearn/features/clustering.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 """
 Module for computing clusters in EOPatch
 
-Credits:
-Copyright (c) 2020 Beno Šircelj (Josef Stefan Institute)
-Copyright (c) 2017-2022 Matej Aleksandrov, Žiga Lukšič (Sinergise)
+Copyright (c) 2017- Sinergise and contributors
+For the full list of contributors, see the CREDITS file in the root directory of this source tree.
 
-This source code is licensed under the MIT license found in the LICENSE
-file in the root directory of this source tree.
+This source code is licensed under the MIT license, see the LICENSE file in the root directory of this source tree.
 """
 from __future__ import annotations
 
 from typing import Callable, List, Optional, Union, cast
 
 import numpy as np
 from sklearn.cluster import AgglomerativeClustering
 from sklearn.feature_extraction.image import grid_to_graph
+from typing_extensions import Literal
 
 from eolearn.core import EOPatch, EOTask, FeatureType
-from eolearn.core.types import FeatureSpec, Literal
+from eolearn.core.types import FeatureSpec
 
 
 class ClusteringTask(EOTask):
     """
     Tasks computes clusters on selected features using `sklearn.cluster.AgglomerativeClustering`.
 
     The algorithm produces a timeless data feature where each cell has a natural number which corresponds to specific
```

### Comparing `eo-learn-features-1.4.0/eolearn/features/doubly_logistic_approximation.py` & `eo-learn-features-1.4.1/eolearn/features/doubly_logistic_approximation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 """
 Module for calculating doubly logistic approximation.
 
-Credits:
-Copyright (c) 2020 Beno Šircelj (Josef Stefan Institute)
-Copyright (c) 2017-2022 Matej Aleksandrov, Žiga Lukšič (Sinergise)
+Copyright (c) 2017- Sinergise and contributors
+For the full list of contributors, see the CREDITS file in the root directory of this source tree.
 
-This source code is licensed under the MIT license found in the LICENSE
-file in the root directory of this source tree.
+This source code is licensed under the MIT license, see the LICENSE file in the root directory of this source tree.
 """
 from __future__ import annotations
 
 import itertools as it
 from typing import List, Optional
 
 import numpy as np
 from scipy.optimize import curve_fit
 
 from eolearn.core import EOPatch, EOTask, FeatureType
 from eolearn.core.types import SingleFeatureSpec
 
 
-def doubly_logistic(middle, initial_value, scale, a1, a2, a3, a4, a5) -> np.ndarray:
+def doubly_logistic(middle, initial_value, scale, a1, a2, a3, a4, a5) -> np.ndarray:  # type: ignore[no-untyped-def]
     # pylint: disable=invalid-name
     """Function passed to `scipy.optimize`"""
     funclist = [lambda y: np.exp(-(((a1 - y) / a4) ** a5)), lambda y: np.exp(-(((y - a1) / a2) ** a3))]
     return initial_value + scale * np.piecewise(middle, [middle < a1, middle >= a1], funclist)
 
 
 class DoublyLogisticApproximationTask(EOTask):
@@ -91,15 +89,15 @@
     def execute(self, eopatch: EOPatch) -> EOPatch:
         """
         :param eopatch: Input eopatch with data on which the doubly logistic approximation is computed
         :return: Output patch with doubly logistic approximation parameters
         """
         data = eopatch[self.feature].squeeze(axis=3)
 
-        times = np.asarray([time.toordinal() for time in eopatch.timestamp])
+        times = np.asarray([time.toordinal() for time in eopatch.timestamps])
         times = (times - times[0]) / (times[-1] - times[0])
 
         time, height, width = data.shape
 
         if self.valid_mask:
             valid_data_mask = eopatch[self.valid_mask]
         else:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `eo-learn-features-1.4.0/eolearn/features/feature_manipulation.py` & `eo-learn-features-1.4.1/eolearn/features/feature_manipulation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 """
 Module for basic feature manipulations, i.e. removing a feature from EOPatch, or removing a slice (time-frame) from
 the time-dependent features.
 
-Credits:
-Copyright (c) 2017-2022 Matej Aleksandrov, Matej Batič, Grega Milčinski, Domagoj Korais, Matic Lubej (Sinergise)
-Copyright (c) 2017-2022 Žiga Lukšič, Devis Peressutti, Nejc Vesel, Jovan Višnjić, Anže Zupanc (Sinergise)
-Copyright (c) 2019-2020 Jernej Puc, Lojze Žust (Sinergise)
-Copyright (c) 2017-2019 Blaž Sovdat, Andrej Burja (Sinergise)
+Copyright (c) 2017- Sinergise and contributors
+For the full list of contributors, see the CREDITS file in the root directory of this source tree.
 
-This source code is licensed under the MIT license found in the LICENSE
-file in the root directory of this source tree.
+This source code is licensed under the MIT license, see the LICENSE file in the root directory of this source tree.
 """
 from __future__ import annotations
 
 import datetime as dt
 import logging
 from functools import partial
 from typing import Any, Callable, Dict, Iterable, List, Optional, Union, cast
 
 import numpy as np
 from geopandas import GeoDataFrame
+from typing_extensions import Literal
 
 from sentinelhub import bbox_to_dimensions
 
-from eolearn.core import EOPatch, EOTask, FeatureType, FeatureTypeSet, MapFeatureTask
-from eolearn.core.types import FeaturesSpecification, Literal, SingleFeatureSpec
+from eolearn.core import EOPatch, EOTask, FeatureType, MapFeatureTask
+from eolearn.core.constants import TIMESTAMP_COLUMN
+from eolearn.core.types import FeaturesSpecification, SingleFeatureSpec
+from eolearn.core.utils.parsing import parse_renamed_features
 
 from .utils import ResizeLib, ResizeMethod, ResizeParam, spatially_resize_image
 
 LOGGER = logging.getLogger(__name__)
 
 
 class SimpleFilterTask(EOTask):
@@ -46,50 +45,51 @@
         filter_features: FeaturesSpecification = ...,
     ):
         """
         :param feature: Feature in the EOPatch , e.g. feature=(FeatureType.DATA, 'bands')
         :param filter_func: A callable that takes a numpy evaluates to bool.
         :param filter_features: A collection of features which will be filtered into a new EOPatch
         """
+
         self.feature = self.parse_feature(
-            feature, allowed_feature_types=FeatureTypeSet.TEMPORAL_TYPES.difference([FeatureType.VECTOR])
+            feature, allowed_feature_types=lambda fty: fty.is_temporal() and not fty.is_vector()
         )
         self.filter_func = filter_func
         self.filter_features_parser = self.get_feature_parser(filter_features)
 
     def _get_filtered_indices(self, feature_data: Iterable) -> List[int]:
         """Get valid time indices from either a numpy array or a list of timestamps."""
         return [idx for idx, img in enumerate(feature_data) if self.filter_func(img)]
 
     @staticmethod
     def _filter_vector_feature(gdf: GeoDataFrame, good_idxs: List[int], timestamps: List[dt.datetime]) -> GeoDataFrame:
         """Filters rows that don't match with the timestamps that will be kept."""
         timestamps_to_keep = {timestamps[idx] for idx in good_idxs}
-        return gdf[gdf.TIMESTAMP.isin(timestamps_to_keep)]
+        return gdf[gdf[TIMESTAMP_COLUMN].isin(timestamps_to_keep)]
 
     def execute(self, eopatch: EOPatch) -> EOPatch:
         """
         :param eopatch: An input EOPatch.
         :return: A new EOPatch with filtered features.
         """
-        filtered_eopatch = EOPatch()
+        filtered_eopatch = EOPatch(bbox=eopatch.bbox)
         good_idxs = self._get_filtered_indices(eopatch[self.feature])
 
         for feature in self.filter_features_parser.get_features(eopatch):
             feature_type, _ = feature
             data = eopatch[feature]
 
-            if feature_type is FeatureType.TIMESTAMP:
+            if feature_type is FeatureType.TIMESTAMPS:
                 data = [data[idx] for idx in good_idxs]
 
             elif feature_type.is_temporal():
-                if feature_type.is_raster():
+                if feature_type.is_array():
                     data = data[good_idxs]
                 else:
-                    data = self._filter_vector_feature(data, good_idxs, eopatch.timestamp)
+                    data = self._filter_vector_feature(data, good_idxs, eopatch.timestamps)
 
             filtered_eopatch[feature] = data
 
         return filtered_eopatch
 
 
 class FilterTimeSeriesTask(SimpleFilterTask):
@@ -108,15 +108,15 @@
         """
         self.start_date = start_date
         self.end_date = end_date
 
         if not isinstance(start_date, dt.datetime) or not isinstance(end_date, dt.datetime):
             raise ValueError("Both start_date and end_date must be datetime.datetime objects.")
 
-        super().__init__((FeatureType.TIMESTAMP, None), self._filter_func, filter_features)
+        super().__init__((FeatureType.TIMESTAMPS, None), self._filter_func, filter_features)
 
 
 class ValueFilloutTask(EOTask):
     """Overwrites occurrences of a desired value with their neighbor values in either forward, backward direction or
     both, along an axis.
 
     Possible fillout operations are 'f' (forward), 'b' (backward) or both, 'fb' or 'bf':
@@ -289,11 +289,11 @@
             if not eopatch.bbox:
                 raise ValueError("Resolution-specified resizing can only be done on EOPatches with a defined BBox.")
             new_width, new_height = bbox_to_dimensions(eopatch.bbox, (self.width_param, self.height_param))
             resize_fun_kwargs = {ResizeParam.NEW_SIZE.value: (new_height, new_width)}
         else:
             resize_fun_kwargs = {self.resize_type.value: (self.height_param, self.width_param)}
 
-        for ftype, fname, new_name in self.parse_renamed_features(self.features, eopatch=eopatch):
-            if ftype.is_spatial() and ftype.is_raster():
+        for ftype, fname, new_name in parse_renamed_features(self.features, eopatch=eopatch):
+            if ftype.is_spatial() and ftype.is_array():
                 eopatch[ftype, new_name] = self.resize_function(eopatch[ftype, fname], **resize_fun_kwargs)
         return eopatch
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `eo-learn-features-1.4.0/eolearn/features/haralick.py` & `eo-learn-features-1.4.1/eolearn/features/haralick.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 """
 Module for computing Haralick textures in EOPatch
 
-Credits:
-Copyright (c) 2018-2019 Hugo Fournier (Magellium)
-Copyright (c) 2017-2022 Matej Aleksandrov, Žiga Lukšič (Sinergise)
+Copyright (c) 2017- Sinergise and contributors
+For the full list of contributors, see the CREDITS file in the root directory of this source tree.
 
-This source code is licensed under the MIT license found in the LICENSE
-file in the root directory of this source tree.
+This source code is licensed under the MIT license, see the LICENSE file in the root directory of this source tree.
 """
 from __future__ import annotations
 
 import itertools as it
 import warnings
 
 import numpy as np
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `eo-learn-features-1.4.0/eolearn/features/hog.py` & `eo-learn-features-1.4.1/eolearn/features/hog.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 """
 Module for computing the Histogram of gradient in EOPatch
 
-Credits:
-Copyright (c) 2018-2019 Hugo Fournier (Magellium)
-Copyright (c) 2017-2022 Matej Aleksandrov, Devis Peressutti, Žiga Lukšič (Sinergise)
+Copyright (c) 2017- Sinergise and contributors
+For the full list of contributors, see the CREDITS file in the root directory of this source tree.
 
-This source code is licensed under the MIT license found in the LICENSE
-file in the root directory of this source tree.
+This source code is licensed under the MIT license, see the LICENSE file in the root directory of this source tree.
 """
 from __future__ import annotations
 
 from typing import Optional, Tuple
 
 import numpy as np
 import skimage.feature
```

### Comparing `eo-learn-features-1.4.0/eolearn/features/interpolation.py` & `eo-learn-features-1.4.1/eolearn/features/interpolation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,32 @@
 """
 Module for interpolating, smoothing and re-sampling features in EOPatch
 
-Credits:
-Copyright (c) 2017-2022 Matej Aleksandrov, Matej Batič, Grega Milčinski, Domagoj Korais, Matic Lubej (Sinergise)
-Copyright (c) 2017-2022 Žiga Lukšič, Devis Peressutti, Nejc Vesel, Jovan Višnjić, Anže Zupanc (Sinergise)
-Copyright (c) 2017-2019 Blaž Sovdat, Andrej Burja (Sinergise)
-Copyright (c) 2018-2019 Filip Koprivec (Jožef Stefan Institute)
-Copyright (c) 2018-2019 William Ouellette
+Copyright (c) 2017- Sinergise and contributors
+For the full list of contributors, see the CREDITS file in the root directory of this source tree.
 
-This source code is licensed under the MIT license found in the LICENSE
-file in the root directory of this source tree.
+This source code is licensed under the MIT license, see the LICENSE file in the root directory of this source tree.
 """
 from __future__ import annotations
 
 import datetime as dt
 import inspect
 import warnings
 from functools import partial
 from typing import Any, Callable, List, Optional, Set, Tuple, Union, cast
 
 import dateutil
 import numpy as np
 import scipy.interpolate
 from sklearn.gaussian_process import GaussianProcessRegressor
 
-from eolearn.core import EOPatch, EOTask, FeatureType, FeatureTypeSet
+from eolearn.core import EOPatch, EOTask, FeatureType
 from eolearn.core.exceptions import EOUserWarning
 from eolearn.core.types import FeaturesSpecification, SingleFeatureSpec
+from eolearn.core.utils.parsing import parse_renamed_feature
 
 try:
     import numba
 except ImportError as exception:
     warnings.warn(
         f"Failed to import numba with exception: '{exception}'. Some interpolation tasks won't work", EOUserWarning
     )
@@ -129,15 +125,17 @@
         copy_features: Optional[FeaturesSpecification] = None,
         unknown_value: float = np.nan,
         filling_factor: int = 10,
         scale_time: int = 3600,
         interpolate_pixel_wise: bool = False,
         **interpolation_parameters: Any,
     ):
-        self.renamed_feature = self.parse_renamed_feature(feature, allowed_feature_types=FeatureTypeSet.RASTER_TYPES_4D)
+        self.renamed_feature = parse_renamed_feature(
+            feature, allowed_feature_types=[FeatureType.MASK, FeatureType.DATA]
+        )
 
         self.interpolation_object = interpolation_object
         self.resample_range = resample_range
         self.result_interval = result_interval
 
         self.mask_feature_parser = (
             None
@@ -315,17 +313,19 @@
 
         # initialise array of interpolated values
         new_data = np.full((len(resampled_times), nobs), np.nan, dtype=data.dtype)
 
         # array defining index correspondence between reference times and resampled times
         ori2res = np.array(
             [
-                np.abs(resampled_times - o).argmin()
-                if np.min(resampled_times) <= o <= np.max(resampled_times)
-                else None
+                (
+                    np.abs(resampled_times - o).argmin()
+                    if np.min(resampled_times) <= o <= np.max(resampled_times)
+                    else None
+                )
                 for o in times
             ]
         )
 
         # find NaNs that start or end a time-series
         row_nans, col_nans = np.where(self._get_start_end_nans(data))
         nan_row_res_indices = np.array([index for index in ori2res[row_nans] if index is not None], dtype=np.int32)
@@ -359,23 +359,23 @@
         :param series: One dimensional array of time series
         :return: Initialized interpolation model class
         """
         if str(inspect.getmodule(self.interpolation_object))[9:14] == "numpy":
             return partial(self.interpolation_object, xp=times, fp=series, left=np.nan, right=np.nan)
         return self.interpolation_object(times, series, **self.interpolation_parameters)
 
-    def get_resampled_timestamp(self, timestamp: List[dt.datetime]) -> List[dt.datetime]:
+    def get_resampled_timestamp(self, timestamps: List[dt.datetime]) -> List[dt.datetime]:
         """Takes a list of timestamps and generates new list of timestamps according to ``resample_range``
 
         :param timestamp: list of timestamps
         :return: new list of timestamps
         """
         days: List[dt.datetime]
         if self.resample_range is None:
-            return timestamp
+            return timestamps
 
         if not isinstance(self.resample_range, (tuple, list)):
             raise ValueError(f"Invalid resample_range {self.resample_range}, expected tuple")
 
         if tuple(map(type, self.resample_range)) == (str, str, int):
             resample_range = cast(Tuple[str, str, int], self.resample_range)
             start_date = dateutil.parser.parse(resample_range[0])
@@ -397,29 +397,29 @@
     @staticmethod
     def _get_eopatch_time_series(
         eopatch: EOPatch, ref_date: Optional[dt.datetime] = None, scale_time: int = 1
     ) -> np.ndarray:
         """Returns a numpy array with seconds passed between the reference date and the timestamp of each image.
 
         An array is constructed as time_series[i] = (timestamp[i] - ref_date).total_seconds().
-        If reference date is None the first date in the EOPatch's timestamp is taken.
-        If EOPatch timestamp attribute is empty the method returns None.
+        If reference date is None the first date in the EOPatch's timestamp array is taken.
+        If EOPatch `timestamps` attribute is empty the method returns None.
 
         :param eopatch: the EOPatch whose timestamps are used to construct the time series
         :param ref_date: reference date relative to which the time is measured
         :param scale_time: scale seconds by factor. If `60`, time will be in minutes, if `3600` hours
         """
-        if not eopatch.timestamp:
+        if not eopatch.timestamps:
             return np.zeros(0, dtype=np.int64)
 
         if ref_date is None:
-            ref_date = eopatch.timestamp[0]
+            ref_date = eopatch.timestamps[0]
 
         return np.asarray(
-            [round((timestamp - ref_date).total_seconds() / scale_time) for timestamp in eopatch.timestamp],
+            [round((timestamp - ref_date).total_seconds() / scale_time) for timestamp in eopatch.timestamps],
             dtype=np.int64,
         )
 
     def execute(self, eopatch: EOPatch) -> EOPatch:
         """Execute method that processes EOPatch and returns EOPatch"""
         # pylint: disable=too-many-locals
         feature_type, feature_name, new_feature_name = self.renamed_feature
@@ -439,28 +439,24 @@
                 negated_mask = ~eopatch[mask_type][mask_name].astype(bool)
                 feature_data = self._mask_feature_data(feature_data, negated_mask, mask_type)
 
         # Flatten array
         feature_data = np.reshape(feature_data, (time_num, height * width * band_num))
 
         # If resampling create new EOPatch
-        new_eopatch = EOPatch() if self.resample_range else eopatch
+        new_eopatch = EOPatch(bbox=eopatch.bbox) if self.resample_range else eopatch
 
         # Resample times
         times = self._get_eopatch_time_series(eopatch, scale_time=self.scale_time)
-        new_eopatch.timestamp = self.get_resampled_timestamp(eopatch.timestamp)
-        total_diff = int((new_eopatch.timestamp[0].date() - eopatch.timestamp[0].date()).total_seconds())
+        new_eopatch.timestamps = self.get_resampled_timestamp(eopatch.timestamps)
+        total_diff = int((new_eopatch.timestamps[0].date() - eopatch.timestamps[0].date()).total_seconds())
         resampled_times = (
             self._get_eopatch_time_series(new_eopatch, scale_time=self.scale_time) + total_diff // self.scale_time
         )
 
-        # Add BBox to eopatch if it was created anew
-        if new_eopatch.bbox is None:
-            new_eopatch.bbox = eopatch.bbox
-
         # Replace duplicate acquisitions which have same values on the chosen timescale with their average
         feature_data, times = self._get_unique_times(feature_data, times)
 
         # Interpolate
         feature_data = self.interpolate_data(feature_data, times, resampled_times)
 
         # Normalize
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `eo-learn-features-1.4.0/eolearn/features/local_binary_pattern.py` & `eo-learn-features-1.4.1/eolearn/features/local_binary_pattern.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 """
 Module for computing the Local Binary Pattern in EOPatch
 
-Credits:
-Copyright (c) 2018-2019 Hugo Fournier (Magellium)
-Copyright (c) 2017-2022 Matej Aleksandrov, Devis Peressutti, Žiga Lukšič (Sinergise)
+Copyright (c) 2017- Sinergise and contributors
+For the full list of contributors, see the CREDITS file in the root directory of this source tree.
 
-This source code is licensed under the MIT license found in the LICENSE
-file in the root directory of this source tree.
+This source code is licensed under the MIT license, see the LICENSE file in the root directory of this source tree.
 """
 from __future__ import annotations
 
 import numpy as np
 import skimage.feature
 
 from eolearn.core import EOPatch, EOTask
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `eo-learn-features-1.4.0/eolearn/features/radiometric_normalization.py` & `eo-learn-features-1.4.1/eolearn/features/radiometric_normalization.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 """
 Module for radiometric normalization
 
-Credits:
-Copyright (c) 2018-2019 Johannes Schmid (GeoVille)
-Copyright (c) 2017-2022 Matej Aleksandrov, Matic Lubej, Devis Peressutti, Žiga Lukšič (Sinergise)
+Copyright (c) 2017- Sinergise and contributors
+For the full list of contributors, see the CREDITS file in the root directory of this source tree.
 
-This source code is licensed under the MIT license found in the LICENSE
-file in the root directory of this source tree.
+This source code is licensed under the MIT license, see the LICENSE file in the root directory of this source tree.
 """
 from __future__ import annotations
 
 from abc import ABCMeta, abstractmethod
 from typing import Optional
 
 import numpy as np
 
 from eolearn.core import EOPatch, EOTask
 from eolearn.core.types import SingleFeatureSpec
+from eolearn.core.utils.parsing import parse_renamed_feature
 
 
 class ReferenceScenesTask(EOTask):
     """Creates a layer of reference scenes which have the highest fraction of valid pixels.
 
     The number of reference scenes is limited to a definable number.
 
@@ -36,15 +35,15 @@
 
     def __init__(
         self,
         feature: SingleFeatureSpec,
         valid_fraction_feature: SingleFeatureSpec,
         max_scene_number: Optional[int] = None,
     ):
-        self.renamed_feature = self.parse_renamed_feature(feature)
+        self.renamed_feature = parse_renamed_feature(feature)
         self.valid_fraction_feature = self.parse_feature(valid_fraction_feature)
         self.number = max_scene_number
 
     def execute(self, eopatch: EOPatch) -> EOPatch:
         feature_type, feature_name, new_feature_name = self.renamed_feature
         valid_fraction_feature_type, valid_fraction_feature_name = self.valid_fraction_feature
 
@@ -371,15 +370,15 @@
     :param feature: Name of the eopatch data layer that will undergo a histogram match.
         Should be of the FeatureType "DATA".
     :param reference: Name of the eopatch data layer that represents the reference for the histogram match.
         Should be of the FeatureType "DATA_TIMELESS".
     """
 
     def __init__(self, feature: SingleFeatureSpec, reference: SingleFeatureSpec):
-        self.renamed_feature = self.parse_renamed_feature(feature)
+        self.renamed_feature = parse_renamed_feature(feature)
         self.reference = self.parse_feature(reference)
 
     def execute(self, eopatch: EOPatch) -> EOPatch:
         """Perform histogram matching of the time-series with respect to a reference scene
 
         :param eopatch: eopatch holding the time-series and reference data
         :return: The same eopatch instance with the normalised time-series
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `eo-learn-features-1.4.0/eolearn/features/temporal_features.py` & `eo-learn-features-1.4.1/eolearn/features/temporal_features.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 """
 Module handling processing of temporal features
 
-Credits:
-Copyright (c) 2017-2022 Matej Aleksandrov, Matej Batič, Grega Milčinski, Domagoj Korais, Matic Lubej (Sinergise)
-Copyright (c) 2017-2022 Žiga Lukšič, Devis Peressutti, Nejc Vesel, Jovan Višnjić, Anže Zupanc (Sinergise)
-Copyright (c) 2019-2020 Jernej Puc, Lojze Žust (Sinergise)
-Copyright (c) 2017-2019 Blaž Sovdat, Andrej Burja (Sinergise)
+Copyright (c) 2017- Sinergise and contributors
+For the full list of contributors, see the CREDITS file in the root directory of this source tree.
 
-This source code is licensed under the MIT license found in the LICENSE
-file in the root directory of this source tree.
+This source code is licensed under the MIT license, see the LICENSE file in the root directory of this source tree.
 """
 
 import itertools as it
 from typing import List, Optional
 
 import numpy as np
 
@@ -184,19 +180,16 @@
         argmax_feature: str = "ARGMAX_NDVI_SLOPE",
         argmin_feature: str = "ARGMIN_NDVI_SLOPE",
         mask_data: bool = True,
     ):
         """Task constructor
 
         :param data_feature: Name of data feature with NDVI values. Default is `'NDVI'`
-        :type data_feature: str
         :param argmax_feature: Name of feature with computed argmax values of the NDVI slope
-        :type argmax_feature: str
         :param argmin_feature: Name of feature with computed argmin values of the NDVI slope
-        :type argmin_feature: str
         :param mask_data: Flag for masking NDVI data. Default is `True`
         """
         self.data_feature = data_feature
         self.argmax_feature = argmax_feature
         self.argmin_feature = argmin_feature
         self.mask_data = mask_data
 
@@ -215,15 +208,15 @@
         if self.mask_data:
             valid_data_mask = eopatch.mask["VALID_DATA"]
         else:
             valid_data_mask = eopatch.mask["IS_DATA"]
 
         ndvi = np.ma.array(eopatch.data[self.data_feature], dtype=np.float32, mask=~valid_data_mask.astype(bool))
 
-        all_dates = np.asarray([x.toordinal() for x in eopatch.timestamp])
+        all_dates = np.asarray([x.toordinal() for x in eopatch.timestamps])
 
         if ndvi.ndim == 4:
             h, w = ndvi.shape[1:3]
         else:
             raise ValueError(f"{self.data_feature} feature has incorrect number of dimensions")
 
         argmax_ndvi_slope, argmin_ndvi_slope = np.zeros((h, w, 1), dtype=np.uint8), np.zeros((h, w, 1), dtype=np.uint8)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `eo-learn-features-1.4.0/eolearn/features/utils.py` & `eo-learn-features-1.4.1/eolearn/features/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """
 Utilities for EOPatch feature modification
 
-Credits:
-Copyright (c) 2017-2022 Matej Aleksandrov, Žiga Lukšič (Sinergise)
+Copyright (c) 2017- Sinergise and contributors
+For the full list of contributors, see the CREDITS file in the root directory of this source tree.
 
-This source code is licensed under the MIT license found in the LICENSE
-file in the root directory of this source tree.
+This source code is licensed under the MIT license, see the LICENSE file in the root directory of this source tree.
 """
 import warnings
 from enum import Enum
 from functools import partial
-from typing import Callable, Dict, Optional, Tuple, Union
+from typing import Dict, Optional, Tuple, Union
 
 import numpy as np
 from PIL import Image
 
 from eolearn.core.exceptions import EORuntimeWarning
+from eolearn.core.utils.common import _apply_to_spatial_axes
 
 _CV2_IMPORT_MESSAGE = "The CV2 backend is not installed by default. We suggest you install the `opencv-python` package."
 
 
 class ResizeParam(Enum):
     """Descriptors of spatial-resizing parameter options."""
 
@@ -167,31 +167,7 @@
         # remove negatives so that there are no underflows when casting back
         resized_data = resized_data.clip(min=0)
     return resized_data.astype(old_dtype)
 
 
 def _pil_resize_ndarray(image: np.ndarray, size: Tuple[int, int], method: Image.Resampling) -> np.ndarray:
     return np.array(Image.fromarray(image).resize(size, method))
-
-
-def _apply_to_spatial_axes(
-    resize_function: Callable[[np.ndarray], np.ndarray], data: np.ndarray, spatial_axes: Tuple[int, int]
-) -> np.ndarray:
-    """Helper function for applying resizing to spatial axes
-
-    Recursively slices data into smaller-dimensional ones, until only the spatial axes remain. The indices of spatial
-    axes have to be adjusted if the recursion-axis is smaller than either one, e.g. spatial axes (1, 2) become (0, 1)
-    after splitting the 3D data along axis 0 into 2D arrays.
-
-    After achieving 2D data slices the resizing function is applied. The data is then reconstructed into original form.
-    """
-
-    if data.ndim <= 2:
-        return resize_function(data)
-
-    axis = next(i for i in range(data.ndim) if i not in spatial_axes)
-    data = np.moveaxis(data, axis, 0)
-
-    ax1, ax2 = (ax if axis > ax else ax - 1 for ax in spatial_axes)
-
-    mapped_slices = [_apply_to_spatial_axes(resize_function, data_slice, (ax1, ax2)) for data_slice in data]
-    return np.moveaxis(np.stack(mapped_slices), 0, axis)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `eo-learn-features-1.4.0/setup.py` & `eo-learn-features-1.4.1/setup.py`

 * *Files identical despite different names*

