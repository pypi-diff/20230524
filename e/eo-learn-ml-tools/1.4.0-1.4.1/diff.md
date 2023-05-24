# Comparing `tmp/eo-learn-ml-tools-1.4.0.tar.gz` & `tmp/eo-learn-ml-tools-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eo-learn-ml-tools-1.4.0.tar", last modified: Fri Jan 20 10:59:54 2023, max compression
+gzip compressed data, was "eo-learn-ml-tools-1.4.1.tar", last modified: Tue Mar 14 10:33:40 2023, max compression
```

## Comparing `eo-learn-ml-tools-1.4.0.tar` & `eo-learn-ml-tools-1.4.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-01-20 10:59:54.722319 eo-learn-ml-tools-1.4.0/
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1745 2023-01-20 10:59:54.000000 eo-learn-ml-tools-1.4.0/LICENSE
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       84 2022-06-13 14:43:39.000000 eo-learn-ml-tools-1.4.0/MANIFEST.in
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1739 2023-01-20 10:59:54.722319 eo-learn-ml-tools-1.4.0/PKG-INFO
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      240 2021-04-09 13:35:15.000000 eo-learn-ml-tools-1.4.0/README.md
-drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-01-20 10:59:54.718319 eo-learn-ml-tools-1.4.0/eo_learn_ml_tools.egg-info/
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1739 2023-01-20 10:59:54.000000 eo-learn-ml-tools-1.4.0/eo_learn_ml_tools.egg-info/PKG-INFO
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      536 2023-01-20 10:59:54.000000 eo-learn-ml-tools-1.4.0/eo_learn_ml_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)        1 2023-01-20 10:59:54.000000 eo-learn-ml-tools-1.4.0/eo_learn_ml_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)        1 2021-04-28 12:52:31.000000 eo-learn-ml-tools-1.4.0/eo_learn_ml_tools.egg-info/not-zip-safe
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       51 2023-01-20 10:59:54.000000 eo-learn-ml-tools-1.4.0/eo_learn_ml_tools.egg-info/requires.txt
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)        8 2023-01-20 10:59:54.000000 eo-learn-ml-tools-1.4.0/eo_learn_ml_tools.egg-info/top_level.txt
-drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-01-20 10:59:54.718319 eo-learn-ml-tools-1.4.0/eolearn/
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       65 2022-05-03 09:13:51.000000 eo-learn-ml-tools-1.4.0/eolearn/__init__.py
-drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-01-20 10:59:54.722319 eo-learn-ml-tools-1.4.0/eolearn/ml_tools/
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      231 2023-01-20 10:41:16.000000 eo-learn-ml-tools-1.4.0/eolearn/ml_tools/__init__.py
-drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-01-20 10:59:54.722319 eo-learn-ml-tools-1.4.0/eolearn/ml_tools/extra/
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       64 2022-05-03 09:13:51.000000 eo-learn-ml-tools-1.4.0/eolearn/ml_tools/extra/__init__.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     2132 2023-01-20 10:41:16.000000 eo-learn-ml-tools-1.4.0/eolearn/ml_tools/extra/plotting.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)    18968 2023-01-20 10:41:16.000000 eo-learn-ml-tools-1.4.0/eolearn/ml_tools/sampling.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     5683 2023-01-20 10:41:16.000000 eo-learn-ml-tools-1.4.0/eolearn/ml_tools/train_test_split.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     7332 2023-01-20 10:41:16.000000 eo-learn-ml-tools-1.4.0/eolearn/ml_tools/utils.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       11 2022-05-03 09:13:51.000000 eo-learn-ml-tools-1.4.0/requirements-plotting.txt
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       28 2022-05-03 09:13:51.000000 eo-learn-ml-tools-1.4.0/requirements.txt
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       38 2023-01-20 10:59:54.722319 eo-learn-ml-tools-1.4.0/setup.cfg
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     2619 2022-10-06 11:16:15.000000 eo-learn-ml-tools-1.4.0/setup.py
+drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-03-14 10:33:40.471937 eo-learn-ml-tools-1.4.1/
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1745 2023-03-14 10:33:40.000000 eo-learn-ml-tools-1.4.1/LICENSE
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       84 2022-06-13 14:43:39.000000 eo-learn-ml-tools-1.4.1/MANIFEST.in
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1839 2023-03-14 10:33:40.471937 eo-learn-ml-tools-1.4.1/PKG-INFO
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      340 2023-03-14 10:22:12.000000 eo-learn-ml-tools-1.4.1/README.md
+drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-03-14 10:33:40.463937 eo-learn-ml-tools-1.4.1/eo_learn_ml_tools.egg-info/
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1839 2023-03-14 10:33:40.000000 eo-learn-ml-tools-1.4.1/eo_learn_ml_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      536 2023-03-14 10:33:40.000000 eo-learn-ml-tools-1.4.1/eo_learn_ml_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)        1 2023-03-14 10:33:40.000000 eo-learn-ml-tools-1.4.1/eo_learn_ml_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)        1 2021-04-28 12:52:31.000000 eo-learn-ml-tools-1.4.1/eo_learn_ml_tools.egg-info/not-zip-safe
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       51 2023-03-14 10:33:40.000000 eo-learn-ml-tools-1.4.1/eo_learn_ml_tools.egg-info/requires.txt
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)        8 2023-03-14 10:33:40.000000 eo-learn-ml-tools-1.4.1/eo_learn_ml_tools.egg-info/top_level.txt
+drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-03-14 10:33:40.463937 eo-learn-ml-tools-1.4.1/eolearn/
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       65 2022-05-03 09:13:51.000000 eo-learn-ml-tools-1.4.1/eolearn/__init__.py
+drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-03-14 10:33:40.467937 eo-learn-ml-tools-1.4.1/eolearn/ml_tools/
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      231 2023-03-14 10:22:12.000000 eo-learn-ml-tools-1.4.1/eolearn/ml_tools/__init__.py
+drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-03-14 10:33:40.467937 eo-learn-ml-tools-1.4.1/eolearn/ml_tools/extra/
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       64 2022-05-03 09:13:51.000000 eo-learn-ml-tools-1.4.1/eolearn/ml_tools/extra/__init__.py
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1975 2023-03-14 10:22:12.000000 eo-learn-ml-tools-1.4.1/eolearn/ml_tools/extra/plotting.py
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)    18687 2023-03-14 10:22:12.000000 eo-learn-ml-tools-1.4.1/eolearn/ml_tools/sampling.py
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     5514 2023-03-14 10:22:12.000000 eo-learn-ml-tools-1.4.1/eolearn/ml_tools/train_test_split.py
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     7175 2023-03-14 10:22:12.000000 eo-learn-ml-tools-1.4.1/eolearn/ml_tools/utils.py
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       11 2022-05-03 09:13:51.000000 eo-learn-ml-tools-1.4.1/requirements-plotting.txt
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       28 2022-05-03 09:13:51.000000 eo-learn-ml-tools-1.4.1/requirements.txt
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       38 2023-03-14 10:33:40.471937 eo-learn-ml-tools-1.4.1/setup.cfg
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     2619 2022-10-06 11:16:15.000000 eo-learn-ml-tools-1.4.1/setup.py
```

### Comparing `eo-learn-ml-tools-1.4.0/LICENSE` & `eo-learn-ml-tools-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `eo-learn-ml-tools-1.4.0/PKG-INFO` & `eo-learn-ml-tools-1.4.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: eo-learn-ml-tools
-Version: 1.4.0
+Version: 1.4.1
 Summary: A collection of machine learning EOTasks and utilities
 Home-page: https://github.com/sentinel-hub/eo-learn
 Author: Sinergise EO research team
 Author-email: eoresearch@sinergise.com
 License: MIT
 Project-URL: Documentation, https://eo-learn.readthedocs.io
 Project-URL: Source Code, https://github.com/sentinel-hub/eo-learn
 Project-URL: Bug Tracker, https://github.com/sentinel-hub/eo-learn/issues
 Project-URL: Forum, https://forum.sentinel-hub.com
 Description: # eolearn.ml_tools subpackage
         
         Various tools that can be used before or after the machine learning process.
         
-        For more information on the package content, visit [readthedocs](https://eo-learn.readthedocs.io/en/latest/eolearn.ml_tools.html).
+        For more information about the module visit [readthedocs](https://eo-learn.readthedocs.io/en/latest/reference/eolearn.ml-tools.html), or see the [module task index](https://eo-learn.readthedocs.io/en/latest/eotasks.html#ml-tools).
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eo-learn-ml-tools-1.4.0/eo_learn_ml_tools.egg-info/PKG-INFO` & `eo-learn-ml-tools-1.4.1/eo_learn_ml_tools.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: eo-learn-ml-tools
-Version: 1.4.0
+Version: 1.4.1
 Summary: A collection of machine learning EOTasks and utilities
 Home-page: https://github.com/sentinel-hub/eo-learn
 Author: Sinergise EO research team
 Author-email: eoresearch@sinergise.com
 License: MIT
 Project-URL: Documentation, https://eo-learn.readthedocs.io
 Project-URL: Source Code, https://github.com/sentinel-hub/eo-learn
 Project-URL: Bug Tracker, https://github.com/sentinel-hub/eo-learn/issues
 Project-URL: Forum, https://forum.sentinel-hub.com
 Description: # eolearn.ml_tools subpackage
         
         Various tools that can be used before or after the machine learning process.
         
-        For more information on the package content, visit [readthedocs](https://eo-learn.readthedocs.io/en/latest/eolearn.ml_tools.html).
+        For more information about the module visit [readthedocs](https://eo-learn.readthedocs.io/en/latest/reference/eolearn.ml-tools.html), or see the [module task index](https://eo-learn.readthedocs.io/en/latest/eotasks.html#ml-tools).
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eo-learn-ml-tools-1.4.0/eo_learn_ml_tools.egg-info/SOURCES.txt` & `eo-learn-ml-tools-1.4.1/eo_learn_ml_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eo-learn-ml-tools-1.4.0/eolearn/ml_tools/extra/plotting.py` & `eo-learn-ml-tools-1.4.1/eolearn/ml_tools/extra/plotting.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 """
 The module provides some utility functions for ML specific plotting
 
-Credits:
-Copyright (c) 2017-2022 Matej Aleksandrov, Matej Batič, Grega Milčinski, Domagoj Korais, Matic Lubej (Sinergise)
-Copyright (c) 2017-2022 Žiga Lukšič, Devis Peressutti, Nejc Vesel, Jovan Višnjić, Anže Zupanc (Sinergise)
-Copyright (c) 2017-2019 Blaž Sovdat, Andrej Burja (Sinergise)
+Copyright (c) 2017- Sinergise and contributors
+For the full list of contributors, see the CREDITS file in the root directory of this source tree.
 
-This source code is licensed under the MIT license found in the LICENSE
-file in the root directory of this source tree.
+This source code is licensed under the MIT license, see the LICENSE file in the root directory of this source tree.
 """
 
 import itertools
 from typing import List, Optional, Union
 
 import numpy as np
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `eo-learn-ml-tools-1.4.0/eolearn/ml_tools/sampling.py` & `eo-learn-ml-tools-1.4.1/eolearn/ml_tools/sampling.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 """
 Tasks for spatial sampling of points for building training/validation samples for example.
 
-Credits:
-Copyright (c) 2017-2022 Matej Aleksandrov, Matej Batič, Grega Milčinski, Domagoj Korais, Matic Lubej (Sinergise)
-Copyright (c) 2017-2022 Žiga Lukšič, Devis Peressutti, Nejc Vesel, Jovan Višnjić, Anže Zupanc (Sinergise)
-Copyright (c) 2017-2019 Blaž Sovdat, Andrej Burja (Sinergise)
+Copyright (c) 2017- Sinergise and contributors
+For the full list of contributors, see the CREDITS file in the root directory of this source tree.
 
-This source code is licensed under the MIT license found in the LICENSE
-file in the root directory of this source tree.
+This source code is licensed under the MIT license, see the LICENSE file in the root directory of this source tree.
 """
 from __future__ import annotations
 
 from abc import ABCMeta
 from math import sqrt
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 from shapely.geometry import Point, Polygon
 
-from eolearn.core import EOPatch, EOTask, FeatureType, FeatureTypeSet
+from eolearn.core import EOPatch, EOTask, FeatureType
 from eolearn.core.types import FeaturesSpecification, SingleFeatureSpec
 
 _FractionType = Union[float, Dict[int, float]]
 
 
 def random_point_in_triangle(triangle: Polygon, rng: Optional[np.random.Generator] = None) -> Point:
     """Selects a random point from an interior of a triangle.
@@ -140,22 +137,21 @@
         mask_of_samples: Optional[Tuple[FeatureType, str]] = None,
     ):
         """
         :param features_to_sample: Features that will be spatially sampled according to given sampling parameters.
         :param mask_of_samples: An output mask timeless feature of counts how many times each pixel has been sampled.
         """
         self.features_parser = self.get_feature_parser(
-            features_to_sample,
-            allowed_feature_types=FeatureTypeSet.SPATIAL_TYPES & FeatureTypeSet.RASTER_TYPES,
+            features_to_sample, allowed_feature_types=lambda fty: fty.is_image()
         )
 
         self.mask_of_samples = mask_of_samples
         if mask_of_samples is not None:
             self.mask_of_samples = self.parse_feature(  # type: ignore[assignment]
-                self.mask_of_samples, allowed_feature_types={FeatureType.MASK_TIMELESS}
+                mask_of_samples, allowed_feature_types={FeatureType.MASK_TIMELESS}
             )
 
     def _apply_sampling(self, eopatch: EOPatch, row_grid: np.ndarray, column_grid: np.ndarray) -> EOPatch:
         """Applies masks of sampled indices to EOPatch features to create sampled features and a mask of samples"""
         image_shape = None
         for feature_type, feature_name, new_feature_name in self.features_parser.get_renamed_features(eopatch):
             if feature_name is not None:
@@ -324,16 +320,16 @@
         :return: An EOPatch with additional spatially sampled features
         """
         rng = np.random.default_rng(seed)
 
         sampling_image = self._generate_dummy_mask(eopatch)
 
         amount = self.amount if amount is None else amount
-        if isinstance(amount, (int, np.integer)):  # type: ignore[unreachable]
-            n_samples_per_value = {1: amount}  # type: ignore[unreachable]
+        if isinstance(amount, (int, np.integer)):
+            n_samples_per_value = {1: amount}
         else:
             n_samples_per_value = {1: round(sampling_image.size * amount)}
 
         rows, columns = sample_by_values(sampling_image, n_samples_per_value, rng=rng, replace=self.replace)
         size_x, size_y = self.sample_size  # this way it also works for lists
         row_grid, column_grid = expand_to_grids(rows, columns, sample_size=(size_x, size_y))
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `eo-learn-ml-tools-1.4.0/eolearn/ml_tools/train_test_split.py` & `eo-learn-ml-tools-1.4.1/eolearn/ml_tools/train_test_split.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 """
 Tasks used for train set preparation
 
-Credits:
-Copyright (c) 2017-2022 Matej Aleksandrov, Matej Batič, Grega Milčinski, Domagoj Korais, Matic Lubej (Sinergise)
-Copyright (c) 2017-2022 Žiga Lukšič, Devis Peressutti, Nejc Vesel, Jovan Višnjić, Anže Zupanc (Sinergise)
-Copyright (c) 2017-2019 Blaž Sovdat, Andrej Burja (Sinergise)
+Copyright (c) 2017- Sinergise and contributors
+For the full list of contributors, see the CREDITS file in the root directory of this source tree.
 
-This source code is licensed under the MIT license found in the LICENSE
-file in the root directory of this source tree.
+This source code is licensed under the MIT license, see the LICENSE file in the root directory of this source tree.
 """
 from __future__ import annotations
 
 from enum import Enum
 from typing import Any, List, Optional, Union
 
 import numpy as np
 
 from eolearn.core import EOPatch, EOTask, FeatureType
-from eolearn.core.types import FeaturesSpecification
+from eolearn.core.types import SingleFeatureSpec
 
 
 class TrainTestSplitType(Enum):
     """An enum defining TrainTestSplitTask's methods of splitting the data into subsets"""
 
     PER_PIXEL = "per_pixel"
     PER_CLASS = "per_class"
@@ -62,16 +59,16 @@
 
     After execution each pixel will have a value representing the train, test and/or validation set stored in the
     output feature.
     """
 
     def __init__(
         self,
-        input_feature: FeaturesSpecification,
-        output_feature: FeaturesSpecification,
+        input_feature: SingleFeatureSpec,
+        output_feature: SingleFeatureSpec,
         bins: Union[float, List[Any]],
         split_type: TrainTestSplitType = TrainTestSplitType.PER_PIXEL,
         ignore_values: Optional[List[int]] = None,
     ):
         """
         :param input_feature: The input feature to guide the split.
         :param input_feature: The output feature where to save the mask.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `eo-learn-ml-tools-1.4.0/eolearn/ml_tools/utils.py` & `eo-learn-ml-tools-1.4.1/eolearn/ml_tools/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 """
 The utilities module is a collection of methods used across the eolearn package, such as checking whether two objects
 are deeply equal, padding of an image, etc.
 
-Credits:
-Copyright (c) 2017-2022 Matej Aleksandrov, Matej Batič, Grega Milčinski, Domagoj Korais, Matic Lubej (Sinergise)
-Copyright (c) 2017-2022 Žiga Lukšič, Devis Peressutti, Nejc Vesel, Jovan Višnjić, Anže Zupanc (Sinergise)
-Copyright (c) 2017-2019 Blaž Sovdat, Andrej Burja (Sinergise)
+Copyright (c) 2017- Sinergise and contributors
+For the full list of contributors, see the CREDITS file in the root directory of this source tree.
 
-This source code is licensed under the MIT license found in the LICENSE
-file in the root directory of this source tree.
+This source code is licensed under the MIT license, see the LICENSE file in the root directory of this source tree.
 """
 
 from typing import Any, Optional
 
 import numpy as np
 
 from sentinelhub.exceptions import deprecated_function
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `eo-learn-ml-tools-1.4.0/setup.py` & `eo-learn-ml-tools-1.4.1/setup.py`

 * *Files identical despite different names*

