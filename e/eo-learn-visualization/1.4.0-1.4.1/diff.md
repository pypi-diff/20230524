# Comparing `tmp/eo-learn-visualization-1.4.0.tar.gz` & `tmp/eo-learn-visualization-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eo-learn-visualization-1.4.0.tar", last modified: Fri Jan 20 10:59:59 2023, max compression
+gzip compressed data, was "eo-learn-visualization-1.4.1.tar", last modified: Tue Mar 14 10:33:45 2023, max compression
```

## Comparing `eo-learn-visualization-1.4.0.tar` & `eo-learn-visualization-1.4.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-01-20 10:59:59.530350 eo-learn-visualization-1.4.0/
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1745 2023-01-20 10:59:59.000000 eo-learn-visualization-1.4.0/LICENSE
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      143 2022-06-13 14:43:39.000000 eo-learn-visualization-1.4.0/MANIFEST.in
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1744 2023-01-20 10:59:59.530350 eo-learn-visualization-1.4.0/PKG-INFO
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      219 2021-07-28 10:08:22.000000 eo-learn-visualization-1.4.0/README.md
-drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-01-20 10:59:59.518350 eo-learn-visualization-1.4.0/eo_learn_visualization.egg-info/
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1744 2023-01-20 10:59:59.000000 eo-learn-visualization-1.4.0/eo_learn_visualization.egg-info/PKG-INFO
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      577 2023-01-20 10:59:59.000000 eo-learn-visualization-1.4.0/eo_learn_visualization.egg-info/SOURCES.txt
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)        1 2023-01-20 10:59:59.000000 eo-learn-visualization-1.4.0/eo_learn_visualization.egg-info/dependency_links.txt
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)        1 2021-04-28 12:52:33.000000 eo-learn-visualization-1.4.0/eo_learn_visualization.egg-info/not-zip-safe
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       64 2023-01-20 10:59:59.000000 eo-learn-visualization-1.4.0/eo_learn_visualization.egg-info/requires.txt
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)        8 2023-01-20 10:59:59.000000 eo-learn-visualization-1.4.0/eo_learn_visualization.egg-info/top_level.txt
-drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-01-20 10:59:59.518350 eo-learn-visualization-1.4.0/eolearn/
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       65 2022-05-03 09:13:51.000000 eo-learn-visualization-1.4.0/eolearn/__init__.py
-drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-01-20 10:59:59.526350 eo-learn-visualization-1.4.0/eolearn/visualization/
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      117 2023-01-20 10:41:16.000000 eo-learn-visualization-1.4.0/eolearn/visualization/__init__.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     9579 2023-01-20 10:41:16.000000 eo-learn-visualization-1.4.0/eolearn/visualization/eoexecutor.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)    10108 2023-01-20 10:41:16.000000 eo-learn-visualization-1.4.0/eolearn/visualization/eopatch.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     6010 2023-01-20 10:41:16.000000 eo-learn-visualization-1.4.0/eolearn/visualization/eopatch_base.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     3037 2022-06-13 14:10:04.000000 eo-learn-visualization-1.4.0/eolearn/visualization/eoworkflow.py
-drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-01-20 10:59:59.526350 eo-learn-visualization-1.4.0/eolearn/visualization/report_templates/
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     6786 2022-05-03 09:13:51.000000 eo-learn-visualization-1.4.0/eolearn/visualization/report_templates/report.html
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       64 2022-05-03 09:13:51.000000 eo-learn-visualization-1.4.0/requirements.txt
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       38 2023-01-20 10:59:59.530350 eo-learn-visualization-1.4.0/setup.cfg
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     2670 2023-01-20 10:41:16.000000 eo-learn-visualization-1.4.0/setup.py
+drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-03-14 10:33:45.403969 eo-learn-visualization-1.4.1/
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1745 2023-03-14 10:33:45.000000 eo-learn-visualization-1.4.1/LICENSE
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      143 2022-06-13 14:43:39.000000 eo-learn-visualization-1.4.1/MANIFEST.in
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1747 2023-03-14 10:33:45.403969 eo-learn-visualization-1.4.1/PKG-INFO
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      222 2023-03-14 10:22:12.000000 eo-learn-visualization-1.4.1/README.md
+drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-03-14 10:33:45.395969 eo-learn-visualization-1.4.1/eo_learn_visualization.egg-info/
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1747 2023-03-14 10:33:45.000000 eo-learn-visualization-1.4.1/eo_learn_visualization.egg-info/PKG-INFO
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      577 2023-03-14 10:33:45.000000 eo-learn-visualization-1.4.1/eo_learn_visualization.egg-info/SOURCES.txt
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)        1 2023-03-14 10:33:45.000000 eo-learn-visualization-1.4.1/eo_learn_visualization.egg-info/dependency_links.txt
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)        1 2021-04-28 12:52:33.000000 eo-learn-visualization-1.4.1/eo_learn_visualization.egg-info/not-zip-safe
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       58 2023-03-14 10:33:45.000000 eo-learn-visualization-1.4.1/eo_learn_visualization.egg-info/requires.txt
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)        8 2023-03-14 10:33:45.000000 eo-learn-visualization-1.4.1/eo_learn_visualization.egg-info/top_level.txt
+drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-03-14 10:33:45.399969 eo-learn-visualization-1.4.1/eolearn/
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       65 2022-05-03 09:13:51.000000 eo-learn-visualization-1.4.1/eolearn/__init__.py
+drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-03-14 10:33:45.403969 eo-learn-visualization-1.4.1/eolearn/visualization/
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      117 2023-03-14 10:22:12.000000 eo-learn-visualization-1.4.1/eolearn/visualization/__init__.py
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     9374 2023-03-14 10:22:12.000000 eo-learn-visualization-1.4.1/eolearn/visualization/eoexecutor.py
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)    10013 2023-03-14 10:22:12.000000 eo-learn-visualization-1.4.1/eolearn/visualization/eopatch.py
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     5972 2023-03-14 10:22:12.000000 eo-learn-visualization-1.4.1/eolearn/visualization/eopatch_base.py
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     2821 2023-03-14 10:22:12.000000 eo-learn-visualization-1.4.1/eolearn/visualization/eoworkflow.py
+drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-03-14 10:33:45.403969 eo-learn-visualization-1.4.1/eolearn/visualization/report_templates/
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     6786 2022-05-03 09:13:51.000000 eo-learn-visualization-1.4.1/eolearn/visualization/report_templates/report.html
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       58 2023-03-14 10:22:12.000000 eo-learn-visualization-1.4.1/requirements.txt
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       38 2023-03-14 10:33:45.403969 eo-learn-visualization-1.4.1/setup.cfg
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     2670 2023-01-20 10:41:16.000000 eo-learn-visualization-1.4.1/setup.py
```

### Comparing `eo-learn-visualization-1.4.0/LICENSE` & `eo-learn-visualization-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `eo-learn-visualization-1.4.0/PKG-INFO` & `eo-learn-visualization-1.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: eo-learn-visualization
-Version: 1.4.0
+Version: 1.4.1
 Summary: A collection of visualization utilities
 Home-page: https://github.com/sentinel-hub/eo-learn
 Author: Sinergise EO research team
 Author-email: eoresearch@sinergise.com
 License: MIT
 Project-URL: Documentation, https://eo-learn.readthedocs.io
 Project-URL: Source Code, https://github.com/sentinel-hub/eo-learn
 Project-URL: Bug Tracker, https://github.com/sentinel-hub/eo-learn/issues
 Project-URL: Forum, https://forum.sentinel-hub.com
 Description: # eolearn.visualization subpackage
         
         A collection of data visualization utilities.
         
-        For more information on the package content, visit [readthedocs](https://eo-learn.readthedocs.io/en/latest/eolearn.visualization.html).
+        For more information about the module visit [readthedocs](https://eo-learn.readthedocs.io/en/latest/reference/eolearn.visualization.html).
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eo-learn-visualization-1.4.0/eo_learn_visualization.egg-info/PKG-INFO` & `eo-learn-visualization-1.4.1/eo_learn_visualization.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: eo-learn-visualization
-Version: 1.4.0
+Version: 1.4.1
 Summary: A collection of visualization utilities
 Home-page: https://github.com/sentinel-hub/eo-learn
 Author: Sinergise EO research team
 Author-email: eoresearch@sinergise.com
 License: MIT
 Project-URL: Documentation, https://eo-learn.readthedocs.io
 Project-URL: Source Code, https://github.com/sentinel-hub/eo-learn
 Project-URL: Bug Tracker, https://github.com/sentinel-hub/eo-learn/issues
 Project-URL: Forum, https://forum.sentinel-hub.com
 Description: # eolearn.visualization subpackage
         
         A collection of data visualization utilities.
         
-        For more information on the package content, visit [readthedocs](https://eo-learn.readthedocs.io/en/latest/eolearn.visualization.html).
+        For more information about the module visit [readthedocs](https://eo-learn.readthedocs.io/en/latest/reference/eolearn.visualization.html).
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eo-learn-visualization-1.4.0/eo_learn_visualization.egg-info/SOURCES.txt` & `eo-learn-visualization-1.4.1/eo_learn_visualization.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eo-learn-visualization-1.4.0/eolearn/visualization/eoexecutor.py` & `eo-learn-visualization-1.4.1/eolearn/visualization/eoexecutor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 """
 Module with utilities for visualizing EOExecutor
 
-Credits:
-Copyright (c) 2017-2022 Matej Aleksandrov, Matej Batič, Grega Milčinski, Domagoj Korais, Matic Lubej (Sinergise)
-Copyright (c) 2017-2022 Žiga Lukšič, Devis Peressutti, Tomislav Slijepčević, Nejc Vesel, Jovan Višnjić (Sinergise)
-Copyright (c) 2017-2022 Anže Zupanc (Sinergise)
-Copyright (c) 2017-2019 Blaž Sovdat, Andrej Burja (Sinergise)
+Copyright (c) 2017- Sinergise and contributors
+For the full list of contributors, see the CREDITS file in the root directory of this source tree.
 
-This source code is licensed under the MIT license found in the LICENSE
-file in the root directory of this source tree.
+This source code is licensed under the MIT license, see the LICENSE file in the root directory of this source tree.
 """
 import base64
 import datetime as dt
 import importlib
 import inspect
 import os
 import warnings
@@ -178,15 +174,15 @@
                 subpackage = importlib.import_module(subpackage_name)
                 subpackage_version = subpackage.__version__ if hasattr(subpackage, "__version__") else "unknown"
                 source = subpackage_name, subpackage_version
             else:
                 try:
                     source = inspect.getsource(task.__class__)
                     source = pygments.highlight(source, lexer, formatter)
-                except TypeError:
+                except (TypeError, OSError):
                     # Jupyter notebook does not have __file__ method to collect source code
                     # StackOverflow provides no solutions
                     # Could be investigated further by looking into Jupyter Notebook source code
                     source = None
 
             sources[key] = source
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `eo-learn-visualization-1.4.0/eolearn/visualization/eopatch.py` & `eo-learn-visualization-1.4.1/eolearn/visualization/eopatch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 """
 This module implements visualizations for `EOPatch`
 
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
 
 import datetime as dt
 import itertools as it
 from dataclasses import dataclass, field
 from enum import Enum
@@ -112,15 +110,15 @@
         if feature_type.is_vector():
             return self._plot_vector_feature(
                 data,
                 timestamp_column=self.config.timestamp_column if feature_type.is_temporal() else None,
                 title=feature_name,
             )
 
-        if not feature_type.is_raster():
+        if not feature_type.is_array():
             raise ValueError(f"Plotting of {feature_type} is not supported")
 
         if feature_type.is_spatial():
             if feature_type.is_timeless():
                 return self._plot_raster_grid(data[np.newaxis, ...], title=feature_name)
             return self._plot_raster_grid(data, timestamps=timestamps, title=feature_name)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `eo-learn-visualization-1.4.0/eolearn/visualization/eopatch_base.py` & `eo-learn-visualization-1.4.1/eolearn/visualization/eopatch_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 """
 This module implements base objects for `EOPatch` visualizations.
 
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
 
 import abc
 import datetime as dt
 from dataclasses import dataclass
 from typing import Any, List, Optional, Tuple, Union
 
 import numpy as np
 from geopandas import GeoDataFrame
 
 from eolearn.core import EOPatch
+from eolearn.core.constants import TIMESTAMP_COLUMN
 from eolearn.core.types import SingleFeatureSpec
 from eolearn.core.utils.common import is_discrete_type
 from eolearn.core.utils.parsing import parse_feature
 
 
 @dataclass
 class BasePlotConfig:
@@ -31,15 +30,15 @@
     :param rgb_factor: A factor by which to scale RGB images to make them look better.
     :param timestamp_column: A name of a column containing timestamps in a `GeoDataFrame` feature. If set to `None` it
         will plot temporal vector features as if they were timeless.
     :param geometry_column: A name of a column containing geometries in a `GeoDataFrame` feature.
     """
 
     rgb_factor: Optional[float] = 3.5
-    timestamp_column: Optional[str] = "TIMESTAMP"
+    timestamp_column: Optional[str] = TIMESTAMP_COLUMN
     geometry_column: str = "geometry"
 
 
 class BaseEOPatchVisualization(metaclass=abc.ABCMeta):
     """A base class for EOPatch visualization"""
 
     def __init__(
@@ -75,32 +74,32 @@
         self.times = times
 
         self.channels = channels
         self.channel_names = None if channel_names is None else [str(name) for name in channel_names]
 
         if rgb and len(rgb) != 3:
             raise ValueError(f"Parameter rgb should be a list of 3 indices but got {rgb}")
-        if rgb and not (feature_type.is_spatial() and feature_type.is_raster()):
+        if rgb and not (feature_type.is_spatial() and feature_type.is_array()):
             raise ValueError("Parameter rgb can only be provided for plotting spatial raster features.")
         self.rgb = rgb
 
         if self.channels and self.rgb:
             raise ValueError("Only one of parameters channels and rgb can be provided.")
 
     @abc.abstractmethod
     def plot(self) -> object:
         """Plots the given feature"""
 
     def collect_and_prepare_feature(self) -> Tuple[Any, List[dt.datetime]]:
         """Collects a feature from EOPatch and modifies it according to plotting parameters"""
         feature_type, _ = self.feature
         data = self.eopatch[self.feature]
-        timestamps = self.eopatch.timestamp
+        timestamps = self.eopatch.timestamps
 
-        if feature_type.is_raster():
+        if feature_type.is_array():
             if self.times is not None:
                 data = data[self.times, ...]
                 if timestamps:
                     timestamps = list(np.array(timestamps)[self.times])
 
             if self.channels is not None:
                 data = data[..., self.channels]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `eo-learn-visualization-1.4.0/eolearn/visualization/eoworkflow.py` & `eo-learn-visualization-1.4.1/eolearn/visualization/eoworkflow.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 """
 Visualization of EOWorkflow
 
-Credits:
-Copyright (c) 2017-2022 Matej Aleksandrov, Matej Batič, Grega Milčinski, Domagoj Korais, Matic Lubej (Sinergise)
-Copyright (c) 2017-2022 Žiga Lukšič, Devis Peressutti, Tomislav Slijepčević, Nejc Vesel, Jovan Višnjić (Sinergise)
-Copyright (c) 2017-2022 Anže Zupanc (Sinergise)
-Copyright (c) 2017-2019 Blaž Sovdat, Andrej Burja (Sinergise)
+Copyright (c) 2017- Sinergise and contributors
+For the full list of contributors, see the CREDITS file in the root directory of this source tree.
 
-This source code is licensed under the MIT license found in the LICENSE
-file in the root directory of this source tree.
+This source code is licensed under the MIT license, see the LICENSE file in the root directory of this source tree.
 """
 from typing import Dict, List, Optional, Sequence
 
 from graphviz import Digraph
 
 from eolearn.core import EONode
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `eo-learn-visualization-1.4.0/eolearn/visualization/report_templates/report.html` & `eo-learn-visualization-1.4.1/eolearn/visualization/report_templates/report.html`

 * *Files identical despite different names*

### Comparing `eo-learn-visualization-1.4.0/setup.py` & `eo-learn-visualization-1.4.1/setup.py`

 * *Files identical despite different names*

