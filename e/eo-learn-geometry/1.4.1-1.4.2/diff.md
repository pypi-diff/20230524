# Comparing `tmp/eo-learn-geometry-1.4.1.tar.gz` & `tmp/eo-learn-geometry-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eo-learn-geometry-1.4.1.tar", last modified: Tue Mar 14 10:33:08 2023, max compression
+gzip compressed data, was "eo-learn-geometry-1.4.2.tar", last modified: Wed May 24 10:46:49 2023, max compression
```

## Comparing `eo-learn-geometry-1.4.1.tar` & `eo-learn-geometry-1.4.2.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-03-14 10:33:08.191728 eo-learn-geometry-1.4.1/
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1745 2023-03-14 10:33:07.000000 eo-learn-geometry-1.4.1/LICENSE
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       84 2022-06-13 14:43:39.000000 eo-learn-geometry-1.4.1/MANIFEST.in
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1830 2023-03-14 10:33:08.191728 eo-learn-geometry-1.4.1/PKG-INFO
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      364 2023-03-14 10:22:12.000000 eo-learn-geometry-1.4.1/README.md
-drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-03-14 10:33:08.183728 eo-learn-geometry-1.4.1/eo_learn_geometry.egg-info/
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1830 2023-03-14 10:33:08.000000 eo-learn-geometry-1.4.1/eo_learn_geometry.egg-info/PKG-INFO
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      446 2023-03-14 10:33:08.000000 eo-learn-geometry-1.4.1/eo_learn_geometry.egg-info/SOURCES.txt
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)        1 2023-03-14 10:33:08.000000 eo-learn-geometry-1.4.1/eo_learn_geometry.egg-info/dependency_links.txt
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)        1 2021-04-28 12:52:26.000000 eo-learn-geometry-1.4.1/eo_learn_geometry.egg-info/not-zip-safe
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       76 2023-03-14 10:33:08.000000 eo-learn-geometry-1.4.1/eo_learn_geometry.egg-info/requires.txt
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)        8 2023-03-14 10:33:08.000000 eo-learn-geometry-1.4.1/eo_learn_geometry.egg-info/top_level.txt
-drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-03-14 10:33:08.183728 eo-learn-geometry-1.4.1/eolearn/
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       65 2022-05-03 09:13:51.000000 eo-learn-geometry-1.4.1/eolearn/__init__.py
-drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-03-14 10:33:08.187728 eo-learn-geometry-1.4.1/eolearn/geometry/
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      432 2023-03-14 10:22:12.000000 eo-learn-geometry-1.4.1/eolearn/geometry/__init__.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     6800 2023-03-14 10:22:12.000000 eo-learn-geometry-1.4.1/eolearn/geometry/morphology.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     6064 2023-03-14 10:22:12.000000 eo-learn-geometry-1.4.1/eolearn/geometry/superpixel.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)    23522 2023-03-14 10:22:12.000000 eo-learn-geometry-1.4.1/eolearn/geometry/transformations.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       76 2022-05-03 09:14:16.000000 eo-learn-geometry-1.4.1/requirements.txt
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       38 2023-03-14 10:33:08.191728 eo-learn-geometry-1.4.1/setup.cfg
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     2529 2022-10-06 11:16:15.000000 eo-learn-geometry-1.4.1/setup.py
+drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-05-24 10:46:49.114965 eo-learn-geometry-1.4.2/
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1745 2023-05-24 10:46:48.000000 eo-learn-geometry-1.4.2/LICENSE
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      118 2023-05-24 10:35:48.000000 eo-learn-geometry-1.4.2/MANIFEST.in
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1831 2023-05-24 10:46:49.114965 eo-learn-geometry-1.4.2/PKG-INFO
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      364 2023-05-03 06:39:37.000000 eo-learn-geometry-1.4.2/README.md
+drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-05-24 10:46:49.106966 eo-learn-geometry-1.4.2/eo_learn_geometry.egg-info/
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1831 2023-05-24 10:46:49.000000 eo-learn-geometry-1.4.2/eo_learn_geometry.egg-info/PKG-INFO
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      472 2023-05-24 10:46:49.000000 eo-learn-geometry-1.4.2/eo_learn_geometry.egg-info/SOURCES.txt
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)        1 2023-05-24 10:46:49.000000 eo-learn-geometry-1.4.2/eo_learn_geometry.egg-info/dependency_links.txt
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)        1 2021-04-28 12:52:26.000000 eo-learn-geometry-1.4.2/eo_learn_geometry.egg-info/not-zip-safe
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       76 2023-05-24 10:46:49.000000 eo-learn-geometry-1.4.2/eo_learn_geometry.egg-info/requires.txt
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)        8 2023-05-24 10:46:49.000000 eo-learn-geometry-1.4.2/eo_learn_geometry.egg-info/top_level.txt
+drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-05-24 10:46:49.106966 eo-learn-geometry-1.4.2/eolearn/
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       65 2023-05-23 14:00:11.000000 eo-learn-geometry-1.4.2/eolearn/__init__.py
+drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-05-24 10:46:49.114965 eo-learn-geometry-1.4.2/eolearn/geometry/
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      432 2023-05-24 10:35:48.000000 eo-learn-geometry-1.4.2/eolearn/geometry/__init__.py
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     6762 2023-05-24 10:35:48.000000 eo-learn-geometry-1.4.2/eolearn/geometry/morphology.py
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)        0 2023-05-03 06:39:37.000000 eo-learn-geometry-1.4.2/eolearn/geometry/py.typed
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     6064 2023-05-19 10:26:16.000000 eo-learn-geometry-1.4.2/eolearn/geometry/superpixel.py
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)    22267 2023-05-24 10:35:48.000000 eo-learn-geometry-1.4.2/eolearn/geometry/transformations.py
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       76 2023-05-03 06:34:57.000000 eo-learn-geometry-1.4.2/requirements.txt
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       38 2023-05-24 10:46:49.114965 eo-learn-geometry-1.4.2/setup.cfg
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     2489 2023-05-24 10:35:48.000000 eo-learn-geometry-1.4.2/setup.py
```

### Comparing `eo-learn-geometry-1.4.1/LICENSE` & `eo-learn-geometry-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `eo-learn-geometry-1.4.1/PKG-INFO` & `eo-learn-geometry-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eo-learn-geometry
-Version: 1.4.1
+Version: 1.4.2
 Summary: A collection of geometry EOTasks and utilities
 Home-page: https://github.com/sentinel-hub/eo-learn
 Author: Sinergise EO research team
 Author-email: eoresearch@sinergise.com
 License: MIT
 Project-URL: Documentation, https://eo-learn.readthedocs.io
 Project-URL: Source Code, https://github.com/sentinel-hub/eo-learn
@@ -23,16 +23,16 @@
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
```

### Comparing `eo-learn-geometry-1.4.1/eo_learn_geometry.egg-info/PKG-INFO` & `eo-learn-geometry-1.4.2/eo_learn_geometry.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eo-learn-geometry
-Version: 1.4.1
+Version: 1.4.2
 Summary: A collection of geometry EOTasks and utilities
 Home-page: https://github.com/sentinel-hub/eo-learn
 Author: Sinergise EO research team
 Author-email: eoresearch@sinergise.com
 License: MIT
 Project-URL: Documentation, https://eo-learn.readthedocs.io
 Project-URL: Source Code, https://github.com/sentinel-hub/eo-learn
@@ -23,16 +23,16 @@
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
```

### Comparing `eo-learn-geometry-1.4.1/eolearn/geometry/morphology.py` & `eo-learn-geometry-1.4.2/eolearn/geometry/morphology.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 This source code is licensed under the MIT license, see the LICENSE file in the root directory of this source tree.
 """
 from __future__ import annotations
 
 import itertools as it
 from enum import Enum
-from typing import Callable, List, Optional, Tuple, Union, cast
+from typing import Callable, Tuple, cast
 
 import numpy as np
 import skimage.filters.rank
 import skimage.morphology
 
 from eolearn.core import EOPatch, EOTask, FeatureType, MapFeatureTask
 from eolearn.core.types import FeaturesSpecification, SingleFeatureSpec
@@ -31,15 +31,15 @@
     :param no_data_label: Value used to replace eroded pixels. Default is set to `0`
     """
 
     def __init__(
         self,
         mask_feature: SingleFeatureSpec,
         disk_radius: int = 1,
-        erode_labels: Optional[List[int]] = None,
+        erode_labels: list[int] | None = None,
         no_data_label: int = 0,
     ):
         if not isinstance(disk_radius, int) or disk_radius is None or disk_radius < 1:
             raise ValueError("Disk radius should be an integer larger than 0!")
 
         parsed_mask_feature = cast(
             Tuple[FeatureType, str, str],
@@ -135,18 +135,18 @@
 
 class MorphologicalFilterTask(MapFeatureTask):
     """Performs morphological operations on masks."""
 
     def __init__(
         self,
         input_features: FeaturesSpecification,
-        output_features: Optional[FeaturesSpecification] = None,
+        output_features: FeaturesSpecification | None = None,
         *,
-        morph_operation: Union[MorphologicalOperations, Callable],
-        struct_elem: Optional[np.ndarray] = None,
+        morph_operation: MorphologicalOperations | Callable,
+        struct_elem: np.ndarray | None = None,
     ):
         """
         :param input_features: Input features to be processed.
         :param output_features: Outputs of input features. If not provided the `input_features` are overwritten.
         :param morph_operation: A morphological operation.
         :param struct_elem: A structuring element to be used with the morphological operation. Usually it is generated
             with a factory method from MorphologicalStructElements
```

### Comparing `eo-learn-geometry-1.4.1/eolearn/geometry/superpixel.py` & `eo-learn-geometry-1.4.2/eolearn/geometry/superpixel.py`

 * *Files identical despite different names*

### Comparing `eo-learn-geometry-1.4.1/eolearn/geometry/transformations.py` & `eo-learn-geometry-1.4.2/eolearn/geometry/transformations.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 For the full list of contributors, see the CREDITS file in the root directory of this source tree.
 
 This source code is licensed under the MIT license, see the LICENSE file in the root directory of this source tree.
 """
 from __future__ import annotations
 
 import datetime as dt
-import functools
+import itertools as it
 import logging
 import warnings
-from typing import Any, Callable, Iterator, List, Optional, Tuple, Union, cast
+from functools import partial
+from typing import Any, Callable, Iterator, Tuple, cast
 
 import numpy as np
 import pandas as pd
-import pyproj
 import rasterio.features
 import rasterio.transform
 import shapely.geometry
 import shapely.ops
 import shapely.wkt
 from affine import Affine
 from geopandas import GeoDataFrame, GeoSeries
@@ -45,38 +45,36 @@
 
     In the background it uses `rasterio.features.rasterize`, documented in `rasterio documentation
     <https://rasterio.readthedocs.io/en/stable/api/rasterio.features.html#rasterio.features.rasterize>`__.
     """
 
     # A mapping between types that are not supported by rasterio into types that are. After rasterization the task
     # will cast results back into the original dtype.
-    _RASTERIO_BASIC_DTYPES_MAP = {
+    _RASTERIO_DTYPES_MAP = {
         bool: np.uint8,
+        np.dtype(bool): np.uint8,
         np.int8: np.int16,
+        np.dtype(np.int8): np.int16,
         float: np.float64,
-    }
-    _RASTERIO_DTYPES_MAP = {
-        dtype: rasterio_type
-        for basic_type, rasterio_type in _RASTERIO_BASIC_DTYPES_MAP.items()
-        for dtype in [basic_type, np.dtype(basic_type)]
+        np.dtype(float): np.float64,
     }
 
     def __init__(
         self,
-        vector_input: Union[GeoDataFrame, SingleFeatureSpec],
+        vector_input: GeoDataFrame | SingleFeatureSpec,
         raster_feature: SingleFeatureSpec,
         *,
-        values: Union[None, float, List[float]] = None,
-        values_column: Optional[str] = None,
-        raster_shape: Union[None, Tuple[int, int], SingleFeatureSpec] = None,
-        raster_resolution: Union[None, float, Tuple[float, float]] = None,
-        raster_dtype: Union[np.dtype, type] = np.uint8,
+        values: None | float | list[float] = None,
+        values_column: str | None = None,
+        raster_shape: None | tuple[int, int] | SingleFeatureSpec = None,
+        raster_resolution: None | float | tuple[float, float] = None,
+        raster_dtype: np.dtype | type = np.uint8,
         no_data_value: float = 0,
         write_to_existing: bool = False,
-        overlap_value: Optional[float] = None,
+        overlap_value: float | None = None,
         buffer: float = 0,
         **rasterio_params: Any,
     ):
         """
         :param vector_input: Vector data to be used for rasterization. It can be given as a feature in `EOPatch` or
             as a geopandas `GeoDataFrame`.
         :param raster_feature: New or existing raster feature into which data will be written. If existing raster
@@ -99,17 +97,18 @@
         :param overlap_value: A value to override parts of raster where polygons of different classes overlap. If None,
             rasterization overlays polygon as it is the default behavior of `rasterio.features.rasterize`.
         :param buffer: Buffer value passed to vector_data.buffer() before rasterization. If 0, no buffering is done.
         :param: rasterio_params: Additional parameters to be passed to `rasterio.features.rasterize`. Currently,
             available parameters are `all_touched` and `merge_alg`
         """
         self.vector_input, self.raster_feature = self._parse_main_params(vector_input, raster_feature)
+        self._rasterize_per_timestamp = self.raster_feature[0].is_temporal()
 
         if _vector_is_timeless(self.vector_input) and not self.raster_feature[0].is_timeless():
-            raise ValueError("Vector input has no time-dependence but a time-dependent raster feature was selected")
+            raise ValueError("Vector input has no time-dependence but a time-dependent output feature was selected")
 
         self.values = values
         self.values_column = values_column
         if values_column is None and (values is None or not isinstance(values, (int, float))):
             raise ValueError("One of parameters 'values' and 'values_column' is missing")
 
         self.raster_shape = raster_shape
@@ -120,182 +119,151 @@
         self.raster_dtype = raster_dtype
         self.no_data_value = no_data_value
         self.write_to_existing = write_to_existing
         self.rasterio_params = rasterio_params
         self.overlap_value = overlap_value
         self.buffer = buffer
 
-        self._rasterize_per_timestamp = self.raster_feature[0].is_temporal()
-
     def _parse_main_params(
-        self, vector_input: Union[GeoDataFrame, SingleFeatureSpec], raster_feature: SingleFeatureSpec
-    ) -> Tuple[Union[GeoDataFrame, Tuple[FeatureType, str]], Tuple[FeatureType, str]]:
+        self, vector_input: GeoDataFrame | SingleFeatureSpec, raster_feature: SingleFeatureSpec
+    ) -> tuple[GeoDataFrame | tuple[FeatureType, str], tuple[FeatureType, str]]:
         """Parsing first 2 parameters - what vector data will be used and in which raster feature it will be saved"""
         if not _is_geopandas_object(vector_input):
             vector_input = self.parse_feature(vector_input, allowed_feature_types=lambda fty: fty.is_vector())
 
         parsed_raster_feature = self.parse_feature(raster_feature, allowed_feature_types=lambda fty: fty.is_image())
         return vector_input, parsed_raster_feature  # type: ignore[return-value]
 
     def _get_vector_data_iterator(
         self, eopatch: EOPatch, join_per_value: bool
-    ) -> Iterator[Tuple[Optional[dt.datetime], Optional[ShapeIterator]]]:
+    ) -> Iterator[tuple[dt.datetime | None, ShapeIterator]]:
         """Collects and prepares vector shapes for rasterization. It works as an iterator that returns pairs of
         `(timestamp or None, <iterator over shapes and values>)`
 
         :param eopatch: An EOPatch from where geometries will be obtained
         :param join_per_value: If `True` it will join geometries with the same value using a cascaded union
         """
-        vector_data = self._get_vector_data_from_eopatch(eopatch)
+        vector_data = self.vector_input if _is_geopandas_object(self.vector_input) else eopatch[self.vector_input]
         # EOPatch has a bbox, verified in execute
         vector_data = self._preprocess_vector_data(vector_data, cast(BBox, eopatch.bbox), eopatch.timestamps)
 
         if self._rasterize_per_timestamp:
-            for timestamp, vector_data_per_timestamp in vector_data.groupby(TIMESTAMP_COLUMN):
-                yield timestamp.to_pydatetime(), self._vector_data_to_shape_iterator(
-                    vector_data_per_timestamp, join_per_value
-                )
-        else:
+            for timestamp, data_for_time in vector_data.groupby(TIMESTAMP_COLUMN):
+                if not data_for_time.empty:
+                    yield timestamp.to_pydatetime(), self._vector_data_to_shape_iterator(data_for_time, join_per_value)
+        elif not vector_data.empty:
             yield None, self._vector_data_to_shape_iterator(vector_data, join_per_value)
 
-    def _get_vector_data_from_eopatch(self, eopatch: EOPatch) -> GeoDataFrame:
-        """Provides a vector dataframe either from the attribute or from given EOPatch feature"""
-        if _is_geopandas_object(self.vector_input):
-            return self.vector_input
-
-        return eopatch[self.vector_input]
-
     def _preprocess_vector_data(
-        self, vector_data: GeoDataFrame, bbox: BBox, timestamps: List[dt.datetime]
+        self, vector_data: GeoDataFrame, bbox: BBox, timestamps: list[dt.datetime]
     ) -> GeoDataFrame:
         """Applies preprocessing steps on a dataframe with geometries and potential values and timestamps"""
-        columns_to_keep = ["geometry"]
-        if self._rasterize_per_timestamp:
-            columns_to_keep.append(TIMESTAMP_COLUMN)
-        if self.values_column is not None:
-            columns_to_keep.append(self.values_column)
-        vector_data = vector_data[columns_to_keep]
-
-        if self._rasterize_per_timestamp:
-            vector_data[TIMESTAMP_COLUMN] = vector_data[TIMESTAMP_COLUMN].apply(parse_time)
-            vector_data = vector_data[vector_data[TIMESTAMP_COLUMN].isin(timestamps)]
-
-        if self.values_column is not None and self.values is not None:
-            values = [self.values] if isinstance(self.values, (int, float)) else self.values
-            vector_data = vector_data[vector_data[self.values_column].isin(values)]
+        vector_data = self._reduce_vector_data(vector_data, timestamps)
 
-        gpd_crs = vector_data.crs
-        # This special case has to be handled because of WGS84 and lat-lon order:
-        if isinstance(gpd_crs, pyproj.CRS):
-            gpd_crs = gpd_crs.to_epsg()
-        vector_data_crs = CRS(gpd_crs)
-
-        if bbox.crs is not vector_data_crs:
+        if bbox.crs is not CRS(vector_data.crs.to_epsg()):
             warnings.warn(
-                (
-                    "Vector data is not in the same CRS as EOPatch, this task will re-project vector data for "
-                    "each execution"
-                ),
+                "Vector data is not in the same CRS as EOPatch, the task will re-project vectors for each execution",
                 EORuntimeWarning,
             )
             vector_data = vector_data.to_crs(bbox.crs.pyproj_crs())
 
         bbox_poly = bbox.geometry
         vector_data = vector_data[vector_data.geometry.intersects(bbox_poly)].copy(deep=True)
 
         if self.buffer:
             vector_data.geometry = vector_data.geometry.buffer(self.buffer)
             vector_data = vector_data[~vector_data.is_empty]
 
         if not vector_data.geometry.is_valid.all():
-            warnings.warn("Given vector polygons contain some invalid geometries, they will be fixed", EORuntimeWarning)
+            warnings.warn("Given vector polygons contain some invalid geometries, attempting to fix", EORuntimeWarning)
             vector_data.geometry = vector_data.geometry.buffer(0)
 
         if vector_data.geometry.has_z.any():
-            warnings.warn(
-                "Given vector polygons contain some 3D geometries, they will be projected to 2D", EORuntimeWarning
-            )
-            vector_data.geometry = vector_data.geometry.map(
-                functools.partial(shapely.ops.transform, lambda *args: args[:2])
-            )
+            warnings.warn("Polygons contain 3D geometries, they will be projected to 2D", EORuntimeWarning)
+            vector_data.geometry = vector_data.geometry.map(partial(shapely.ops.transform, lambda *args: args[:2]))
 
         return vector_data
 
-    def _vector_data_to_shape_iterator(
-        self, vector_data: GeoDataFrame, join_per_value: bool
-    ) -> Optional[ShapeIterator]:
-        """Returns an iterator of pairs `(shape, value)` or `None` if given dataframe is empty"""
-        if vector_data.empty:
-            return None
+    def _reduce_vector_data(self, vector_data: GeoDataFrame, timestamps: list[dt.datetime]) -> GeoDataFrame:
+        """Removes all redundant columns and rows."""
+        columns_to_keep = ["geometry"]
+        if self._rasterize_per_timestamp:
+            columns_to_keep.append(TIMESTAMP_COLUMN)
+        if self.values_column is not None:
+            columns_to_keep.append(self.values_column)
+        vector_data = vector_data[columns_to_keep]
 
+        if self._rasterize_per_timestamp:
+            vector_data[TIMESTAMP_COLUMN] = vector_data[TIMESTAMP_COLUMN].apply(parse_time)
+            vector_data = vector_data[vector_data[TIMESTAMP_COLUMN].isin(timestamps)]
+
+        if self.values_column is not None and self.values is not None:
+            values = [self.values] if isinstance(self.values, (int, float)) else self.values
+            vector_data = vector_data[vector_data[self.values_column].isin(values)]
+        return vector_data
+
+    def _vector_data_to_shape_iterator(self, vector_data: GeoDataFrame, join_per_value: bool) -> ShapeIterator:
         if self.values_column is None:
             value = cast(float, self.values)  # cast is checked at init
-            return zip(vector_data.geometry, [value] * len(vector_data.index))
+            return zip(vector_data.geometry, it.repeat(value))
 
+        values = vector_data[self.values_column]
         if join_per_value:
-            classes = np.unique(vector_data[self.values_column])
-            grouped = (vector_data.geometry[vector_data[self.values_column] == cl] for cl in classes)
+            groups = {val: vector_data.geometry[values == val] for val in np.unique(values)}
             join_function = shapely.ops.unary_union if shapely.__version__ >= "1.8.0" else shapely.ops.cascaded_union
-            grouped = (join_function(group) for group in grouped)
-            return zip(grouped, classes)
+            return ((join_function(group), val) for val, group in groups.items())
 
-        return zip(vector_data.geometry, vector_data[self.values_column])
+        return zip(vector_data.geometry, values)
 
-    def _get_raster_shape(self, eopatch: EOPatch) -> Tuple[int, int]:
+    def _get_raster_shape(self, eopatch: EOPatch) -> tuple[int, int]:
         """Determines the shape of new raster feature, returns a pair (height, width)"""
         if isinstance(self.raster_shape, (tuple, list)) and len(self.raster_shape) == 2:
             if isinstance(self.raster_shape[0], int) and isinstance(self.raster_shape[1], int):
                 return self.raster_shape
 
-            feature_type, feature_name = self.parse_feature(
-                self.raster_shape, allowed_feature_types=lambda fty: fty.is_array()
-            )
-            return eopatch.get_spatial_dimension(feature_type, cast(str, feature_name))  # cast verified in parser
+            ftype, fname = self.parse_feature(self.raster_shape, allowed_feature_types=lambda fty: fty.is_array())
+            return eopatch.get_spatial_dimension(ftype, cast(str, fname))  # cast verified in parser
 
         if self.raster_resolution:
             # parsing from strings is not denoted in types, so an explicit upcast is required
-            raw_resolution: Union[str, float, Tuple[float, float]] = self.raster_resolution
+            raw_resolution: str | float | tuple[float, float] = self.raster_resolution
             resolution = float(raw_resolution.strip("m")) if isinstance(raw_resolution, str) else raw_resolution
 
             width, height = bbox_to_dimensions(cast(BBox, eopatch.bbox), resolution)  # cast verified in execute
             return height, width
 
         raise ValueError("Could not determine shape of the raster image")
 
     def _get_raster(self, eopatch: EOPatch, height: int, width: int) -> np.ndarray:
         """Provides raster into which data will be written"""
-        feature_type, feature_name = self.raster_feature
         raster_shape = (len(eopatch.timestamps), height, width) if self._rasterize_per_timestamp else (height, width)
 
-        if self.write_to_existing and feature_name in eopatch[feature_type]:
+        if self.write_to_existing and self.raster_feature in eopatch:
             raster = eopatch[self.raster_feature]
 
-            expected_full_shape = raster_shape + (1,)
+            expected_full_shape = (*raster_shape, 1)
             if raster.shape != expected_full_shape:
-                warnings.warn(
-                    (
-                        f"The existing raster feature {self.raster_feature} has a shape {raster.shape} but "
-                        f"the expected shape is {expected_full_shape}. This might cause errors or unexpected "
-                        "results."
-                    ),
-                    EORuntimeWarning,
+                msg = (
+                    f"The existing raster feature {self.raster_feature} has a shape {raster.shape} but the expected"
+                    f" shape is {expected_full_shape}. This might cause errors or unexpected results."
                 )
+                warnings.warn(msg, EORuntimeWarning)
 
             return raster.squeeze(axis=-1)
 
         return np.full(raster_shape, self.no_data_value, dtype=self.raster_dtype)
 
     def _get_rasterization_function(self, bbox: BBox, height: int, width: int) -> Callable:
         """Provides a function that rasterizes shapes into output raster and already contains all optional parameters"""
         affine_transform = rasterio.transform.from_bounds(*bbox, width=width, height=height)
         rasterize_params = dict(self.rasterio_params, transform=affine_transform)
 
         base_rasterize_func = rasterio.features.rasterize if self.overlap_value is None else self.rasterize_overlapped
 
-        return functools.partial(base_rasterize_func, **rasterize_params)
+        return partial(base_rasterize_func, **rasterize_params)
 
     def rasterize_overlapped(self, shapes: ShapeIterator, out: np.ndarray, **rasterize_args: Any) -> None:
         """Rasterize overlapped classes.
 
         :param shapes: Shapes to be rasterized.
         :param out: A numpy array to which to rasterize polygon classes.
         :param rasterize_args: Keyword arguments to be passed to `rasterio.features.rasterize`.
@@ -331,17 +299,14 @@
         if original_dtype in self._RASTERIO_DTYPES_MAP:
             rasterio_dtype = self._RASTERIO_DTYPES_MAP[original_dtype]
             raster = raster.astype(rasterio_dtype)
 
         timestamp_to_index = {timestamp: index for index, timestamp in enumerate(eopatch.timestamps)}
 
         for timestamp, shape_iterator in vector_data_iterator:
-            if shape_iterator is None:
-                continue
-
             if timestamp is None:
                 rasterize_func(shape_iterator, out=raster)
             else:
                 time_index = timestamp_to_index[timestamp]
                 rasterize_func(shape_iterator, out=raster[time_index, ...])
 
         if original_dtype is not raster.dtype:
@@ -364,17 +329,17 @@
     same vector feature
     """
 
     def __init__(
         self,
         features: FeaturesSpecification,
         *,
-        values: Optional[List[int]] = None,
+        values: list[int] | None = None,
         values_column: str = "VALUE",
-        raster_dtype: Union[None, np.dtype, type] = None,
+        raster_dtype: None | np.dtype | type = None,
         **rasterio_params: Any,
     ):
         """
         :param features: One or more raster mask features which will be vectorized together with an optional new name
             of vector feature. If no new name is given the same name will be used.
 
             Examples:
@@ -394,38 +359,32 @@
         self.feature_parser = self.get_feature_parser(features, allowed_feature_types=lambda fty: fty.is_discrete())
         self.values = values
         self.values_column = values_column
         self.raster_dtype = raster_dtype
         self.rasterio_params = rasterio_params
 
     def _vectorize_single_raster(
-        self, raster: np.ndarray, affine_transform: Affine, crs: CRS, timestamps: Optional[dt.datetime] = None
+        self, raster: np.ndarray, affine_transform: Affine, crs: CRS, timestamps: dt.datetime | None = None
     ) -> GeoDataFrame:
         """Vectorizes a data slice of a single time component
 
         :param raster: Numpy array or shape (height, width, channels)
         :param affine_transform: Object holding a transform vector (i.e. geographical location vector) of the raster
         :param crs: Coordinate reference system
         :param timestamp: Time of the data slice
         :return: Vectorized data
         """
-        mask = None
-        if self.values:
-            mask = np.zeros(raster.shape, dtype=bool)
-            for value in self.values:
-                mask[raster == value] = True
+        mask = np.isin(raster, self.values) if self.values is not None else None
 
         geo_list = []
         value_list = []
         for idx in range(raster.shape[-1]):
+            idx_mask = None if mask is None else mask[..., idx]
             for geojson, value in rasterio.features.shapes(
-                raster[..., idx],
-                mask=None if mask is None else mask[..., idx],
-                transform=affine_transform,
-                **self.rasterio_params,
+                raster[..., idx], mask=idx_mask, transform=affine_transform, **self.rasterio_params
             ):
                 geo_list.append(shapely.geometry.shape(geojson))
                 value_list.append(value)
 
         series_dict = {self.values_column: pd.Series(value_list, dtype=self.raster_dtype)}
         if timestamps is not None:
             series_dict[TIMESTAMP_COLUMN] = pd.to_datetime([timestamps] * len(geo_list))
@@ -441,50 +400,46 @@
         """Execute function which adds new vector layer to the EOPatch
 
         :param eopatch: input EOPatch
         :return: New EOPatch with added vector layer
         """
         if eopatch.bbox is None:
             raise ValueError("EOPatch has to have a bounding box")
+        crs = eopatch.bbox.crs
 
-        for raster_ft, raster_fn, vector_fn in self.feature_parser.get_renamed_features(eopatch):
-            vector_ft = FeatureType.VECTOR_TIMELESS if raster_ft.is_timeless() else FeatureType.VECTOR
-
-            raster = eopatch[raster_ft][raster_fn]
-            height, width = raster.shape[:2] if raster_ft.is_timeless() else raster.shape[1:3]
+        for raster_type, raster_name, vector_name in self.feature_parser.get_renamed_features(eopatch):
+            vector_type = FeatureType.VECTOR_TIMELESS if raster_type.is_timeless() else FeatureType.VECTOR
+            raster = eopatch[raster_type, raster_name]
+            height, width = raster.shape[:2] if raster_type.is_timeless() else raster.shape[1:3]
 
             if self.raster_dtype:
                 raster = raster.astype(self.raster_dtype)
 
             affine_transform = rasterio.transform.from_bounds(*eopatch.bbox, width=width, height=height)
 
-            crs = eopatch.bbox.crs
-
-            if raster_ft.is_timeless():
-                eopatch[vector_ft][vector_fn] = self._vectorize_single_raster(raster, affine_transform, crs)
+            if raster_type.is_timeless():
+                eopatch[vector_type, vector_name] = self._vectorize_single_raster(raster, affine_transform, crs)
             else:
                 gpd_list = [
-                    self._vectorize_single_raster(
-                        raster[time_idx, ...], affine_transform, crs, timestamps=eopatch.timestamps[time_idx]
-                    )
-                    for time_idx in range(raster.shape[0])
+                    self._vectorize_single_raster(raster[idx, ...], affine_transform, crs, eopatch.timestamps[idx])
+                    for idx in range(raster.shape[0])
                 ]
 
-                eopatch[vector_ft][vector_fn] = GeoDataFrame(
+                eopatch[vector_type, vector_name] = GeoDataFrame(
                     pd.concat(gpd_list, ignore_index=True), crs=gpd_list[0].crs
                 )
 
         return eopatch
 
 
 def _is_geopandas_object(data: object) -> bool:
     """A frequently used check if object is geopandas `GeoDataFrame` or `GeoSeries`"""
     return isinstance(data, (GeoDataFrame, GeoSeries))
 
 
-def _vector_is_timeless(vector_input: Union[GeoDataFrame, Tuple[FeatureType, Any]]) -> bool:
+def _vector_is_timeless(vector_input: GeoDataFrame | tuple[FeatureType, Any]) -> bool:
     """Used to check if the vector input (either geopandas object EOPatch Feature) is time independent"""
     if _is_geopandas_object(vector_input):
         return TIMESTAMP_COLUMN not in vector_input
 
     vector_type, _ = vector_input
     return vector_type.is_timeless()
```

### Comparing `eo-learn-geometry-1.4.1/setup.py` & `eo-learn-geometry-1.4.2/setup.py`

 * *Files 7% similar despite different names*

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
     name="eo-learn-geometry",
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     version=get_version(),
     description="A collection of geometry EOTasks and utilities",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     url="https://github.com/sentinel-hub/eo-learn",
     project_urls={
         "Documentation": "https://eo-learn.readthedocs.io",
@@ -55,16 +53,16 @@
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

