# Comparing `tmp/eo-learn-io-1.4.1.tar.gz` & `tmp/eo-learn-io-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eo-learn-io-1.4.1.tar", last modified: Tue Mar 14 10:33:13 2023, max compression
+gzip compressed data, was "eo-learn-io-1.4.2.tar", last modified: Wed May 24 10:46:54 2023, max compression
```

## Comparing `eo-learn-io-1.4.1.tar` & `eo-learn-io-1.4.2.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-03-14 10:33:13.035759 eo-learn-io-1.4.1/
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1745 2023-03-14 10:33:12.000000 eo-learn-io-1.4.1/LICENSE
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      154 2022-06-13 16:47:13.000000 eo-learn-io-1.4.1/MANIFEST.in
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1853 2023-03-14 10:33:13.035759 eo-learn-io-1.4.1/PKG-INFO
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      363 2023-03-14 10:22:12.000000 eo-learn-io-1.4.1/README.md
-drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-03-14 10:33:13.023759 eo-learn-io-1.4.1/eo_learn_io.egg-info/
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1853 2023-03-14 10:33:12.000000 eo-learn-io-1.4.1/eo_learn_io.egg-info/PKG-INFO
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      548 2023-03-14 10:33:12.000000 eo-learn-io-1.4.1/eo_learn_io.egg-info/SOURCES.txt
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)        1 2023-03-14 10:33:12.000000 eo-learn-io-1.4.1/eo_learn_io.egg-info/dependency_links.txt
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)        1 2021-04-28 12:52:28.000000 eo-learn-io-1.4.1/eo_learn_io.egg-info/not-zip-safe
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      158 2023-03-14 10:33:12.000000 eo-learn-io-1.4.1/eo_learn_io.egg-info/requires.txt
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)        8 2023-03-14 10:33:12.000000 eo-learn-io-1.4.1/eo_learn_io.egg-info/top_level.txt
-drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-03-14 10:33:13.023759 eo-learn-io-1.4.1/eolearn/
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       65 2022-05-03 09:13:51.000000 eo-learn-io-1.4.1/eolearn/__init__.py
-drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-03-14 10:33:13.027759 eo-learn-io-1.4.1/eolearn/io/
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      422 2023-03-14 10:22:12.000000 eo-learn-io-1.4.1/eolearn/io/__init__.py
-drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-03-14 10:33:13.031759 eo-learn-io-1.4.1/eolearn/io/extra/
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       64 2022-05-03 09:13:51.000000 eo-learn-io-1.4.1/eolearn/io/extra/__init__.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     3004 2023-03-14 10:22:12.000000 eo-learn-io-1.4.1/eolearn/io/extra/geodb.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)    12914 2023-03-14 10:22:12.000000 eo-learn-io-1.4.1/eolearn/io/extra/meteoblue.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     9882 2023-03-14 10:22:12.000000 eo-learn-io-1.4.1/eolearn/io/geometry_io.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     7051 2023-03-14 10:22:12.000000 eo-learn-io-1.4.1/eolearn/io/geopedia.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)    27040 2023-03-14 10:22:12.000000 eo-learn-io-1.4.1/eolearn/io/raster_io.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)    35930 2023-03-14 10:22:12.000000 eo-learn-io-1.4.1/eolearn/io/sentinelhub_process.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       73 2022-05-03 09:13:51.000000 eo-learn-io-1.4.1/requirements-geodb.txt
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       28 2021-10-27 12:20:57.000000 eo-learn-io-1.4.1/requirements-meteoblue.txt
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      188 2023-03-14 10:22:12.000000 eo-learn-io-1.4.1/requirements.txt
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       38 2023-03-14 10:33:13.035759 eo-learn-io-1.4.1/setup.cfg
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     2605 2022-10-06 11:16:15.000000 eo-learn-io-1.4.1/setup.py
+drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-05-24 10:46:54.006838 eo-learn-io-1.4.2/
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1745 2023-05-24 10:46:53.000000 eo-learn-io-1.4.2/LICENSE
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      182 2023-05-24 10:35:48.000000 eo-learn-io-1.4.2/MANIFEST.in
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1854 2023-05-24 10:46:54.006838 eo-learn-io-1.4.2/PKG-INFO
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      363 2023-05-03 06:39:37.000000 eo-learn-io-1.4.2/README.md
+drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-05-24 10:46:53.990839 eo-learn-io-1.4.2/eo_learn_io.egg-info/
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1854 2023-05-24 10:46:53.000000 eo-learn-io-1.4.2/eo_learn_io.egg-info/PKG-INFO
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      568 2023-05-24 10:46:53.000000 eo-learn-io-1.4.2/eo_learn_io.egg-info/SOURCES.txt
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)        1 2023-05-24 10:46:53.000000 eo-learn-io-1.4.2/eo_learn_io.egg-info/dependency_links.txt
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)        1 2021-04-28 12:52:28.000000 eo-learn-io-1.4.2/eo_learn_io.egg-info/not-zip-safe
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      152 2023-05-24 10:46:53.000000 eo-learn-io-1.4.2/eo_learn_io.egg-info/requires.txt
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)        8 2023-05-24 10:46:53.000000 eo-learn-io-1.4.2/eo_learn_io.egg-info/top_level.txt
+drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-05-24 10:46:53.994839 eo-learn-io-1.4.2/eolearn/
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       65 2023-05-23 14:00:11.000000 eo-learn-io-1.4.2/eolearn/__init__.py
+drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-05-24 10:46:53.998839 eo-learn-io-1.4.2/eolearn/io/
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      422 2023-05-24 10:35:48.000000 eo-learn-io-1.4.2/eolearn/io/__init__.py
+drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-05-24 10:46:54.002838 eo-learn-io-1.4.2/eolearn/io/extra/
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       64 2023-05-03 06:34:57.000000 eo-learn-io-1.4.2/eolearn/io/extra/__init__.py
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     3023 2023-05-24 10:35:48.000000 eo-learn-io-1.4.2/eolearn/io/extra/geodb.py
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)    12905 2023-05-24 10:35:48.000000 eo-learn-io-1.4.2/eolearn/io/extra/meteoblue.py
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     9682 2023-05-24 10:35:48.000000 eo-learn-io-1.4.2/eolearn/io/geometry_io.py
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     7051 2023-05-23 14:10:09.000000 eo-learn-io-1.4.2/eolearn/io/geopedia.py
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)        0 2023-05-24 10:35:48.000000 eo-learn-io-1.4.2/eolearn/io/py.typed
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)    26742 2023-05-24 10:35:48.000000 eo-learn-io-1.4.2/eolearn/io/raster_io.py
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)    30196 2023-05-24 10:35:48.000000 eo-learn-io-1.4.2/eolearn/io/sentinelhub_process.py
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       73 2023-05-03 06:34:57.000000 eo-learn-io-1.4.2/requirements-geodb.txt
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       28 2021-10-27 12:20:57.000000 eo-learn-io-1.4.2/requirements-meteoblue.txt
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      111 2023-05-24 10:35:48.000000 eo-learn-io-1.4.2/requirements.txt
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       38 2023-05-24 10:46:54.006838 eo-learn-io-1.4.2/setup.cfg
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     2565 2023-05-24 10:35:48.000000 eo-learn-io-1.4.2/setup.py
```

### Comparing `eo-learn-io-1.4.1/LICENSE` & `eo-learn-io-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `eo-learn-io-1.4.1/PKG-INFO` & `eo-learn-io-1.4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eo-learn-io
-Version: 1.4.1
+Version: 1.4.2
 Summary: A collection of input/output EOTasks and utilities
 Home-page: https://github.com/sentinel-hub/eo-learn
 Author: Sinergise EO research team
 Author-email: eoresearch@sinergise.com
 License: MIT
 Project-URL: Documentation, https://eo-learn.readthedocs.io
 Project-URL: Source Code, https://github.com/sentinel-hub/eo-learn
@@ -23,17 +23,17 @@
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
 Provides-Extra: METEOBLUE
```

### Comparing `eo-learn-io-1.4.1/eo_learn_io.egg-info/PKG-INFO` & `eo-learn-io-1.4.2/eo_learn_io.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eo-learn-io
-Version: 1.4.1
+Version: 1.4.2
 Summary: A collection of input/output EOTasks and utilities
 Home-page: https://github.com/sentinel-hub/eo-learn
 Author: Sinergise EO research team
 Author-email: eoresearch@sinergise.com
 License: MIT
 Project-URL: Documentation, https://eo-learn.readthedocs.io
 Project-URL: Source Code, https://github.com/sentinel-hub/eo-learn
@@ -23,17 +23,17 @@
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
 Provides-Extra: METEOBLUE
```

### Comparing `eo-learn-io-1.4.1/eo_learn_io.egg-info/SOURCES.txt` & `eo-learn-io-1.4.2/eo_learn_io.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -11,12 +11,13 @@
 eo_learn_io.egg-info/not-zip-safe
 eo_learn_io.egg-info/requires.txt
 eo_learn_io.egg-info/top_level.txt
 eolearn/__init__.py
 eolearn/io/__init__.py
 eolearn/io/geometry_io.py
 eolearn/io/geopedia.py
+eolearn/io/py.typed
 eolearn/io/raster_io.py
 eolearn/io/sentinelhub_process.py
 eolearn/io/extra/__init__.py
 eolearn/io/extra/geodb.py
 eolearn/io/extra/meteoblue.py
```

### Comparing `eo-learn-io-1.4.1/eolearn/io/extra/geodb.py` & `eo-learn-io-1.4.2/eolearn/io/extra/geodb.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 To use tasks from this module you have to install dependencies defined in `requirements-geodb.txt`.
 
 Copyright (c) 2017- Sinergise and contributors
 For the full list of contributors, see the CREDITS file in the root directory of this source tree.
 
 This source code is licensed under the MIT license, see the LICENSE file in the root directory of this source tree.
 """
+from __future__ import annotations
 
-from typing import Any, Optional
+from typing import Any
 
 from sentinelhub import CRS, BBox
 
 from eolearn.core.types import FeatureSpec
 
 from ..geometry_io import _BaseVectorImportTask
 
@@ -43,15 +44,15 @@
         :param kwargs: Additional args that will be passed to `geodb_client.get_collection_by_bbox` call
             (e.g. where="id>-1", operator="and")
         """
         self.geodb_client = geodb_client
         self.geodb_db = geodb_db
         self.geodb_collection = geodb_collection
         self.geodb_kwargs = kwargs
-        self._dataset_crs: Optional[CRS] = None
+        self._dataset_crs: CRS | None = None
 
         super().__init__(feature=feature, reproject=reproject, clip=clip)
 
     @property
     def dataset_crs(self) -> CRS:
         """Provides a "crs" of dataset, loads it lazily (i.e. the first time it is needed)
 
@@ -59,15 +60,15 @@
         """
         if self._dataset_crs is None:
             srid = self.geodb_client.get_collection_srid(collection=self.geodb_collection, database=self.geodb_db)
             self._dataset_crs = CRS(f"epsg:{srid}")
 
         return self._dataset_crs
 
-    def _load_vector_data(self, bbox: Optional[BBox]) -> Any:
+    def _load_vector_data(self, bbox: BBox | None) -> Any:
         """Loads vector data from geoDB table"""
         prepared_bbox = bbox.transform_bounds(self.dataset_crs).geometry.bounds if bbox else None
 
         if "comparison_mode" not in self.geodb_kwargs:
             self.geodb_kwargs["comparison_mode"] = "intersects"
 
         return self.geodb_client.get_collection_by_bbox(
```

### Comparing `eo-learn-io-1.4.1/eolearn/io/extra/meteoblue.py` & `eo-learn-io-1.4.2/eolearn/io/extra/meteoblue.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,17 +8,19 @@
     pip install eo-learn-io[METEOBLUE]
 
 Copyright (c) 2017- Sinergise and contributors
 For the full list of contributors, see the CREDITS file in the root directory of this source tree.
 
 This source code is licensed under the MIT license, see the LICENSE file in the root directory of this source tree.
 """
+from __future__ import annotations
+
 import datetime as dt
 from abc import ABCMeta, abstractmethod
-from typing import Any, List, Optional, Tuple
+from typing import Any
 
 import dateutil.parser
 import geopandas as gpd
 import numpy as np
 import pandas as pd
 import shapely.geometry
 
@@ -37,20 +39,20 @@
 
 
 class BaseMeteoblueTask(EOTask, metaclass=ABCMeta):
     """A base task implementing the logic that is common for all meteoblue tasks"""
 
     def __init__(
         self,
-        feature: Tuple[FeatureType, str],
+        feature: tuple[FeatureType, str],
         apikey: str,
-        query: Optional[dict] = None,
-        units: Optional[dict] = None,
-        time_difference: dt.timedelta = dt.timedelta(minutes=30),  # noqa: B008
-        cache_folder: Optional[str] = None,
+        query: dict | None = None,
+        units: dict | None = None,
+        time_difference: dt.timedelta = dt.timedelta(minutes=30),  # noqa: B008, RUF100
+        cache_folder: str | None = None,
         cache_max_age: int = 604800,
     ):
         """
         :param feature: A feature in which meteoblue data will be stored
         :param apikey: meteoblue API key
         :param query: meteoblue dataset API query definition. If set to None (default) the query has to be set
             in the execute method instead.
@@ -68,62 +70,62 @@
 
         self.client = meteoblue_dataset_sdk.Client(apikey=apikey, cache=cache)
         self.query = query
         self.units = units
         self.time_difference = time_difference
 
     @staticmethod
-    def _get_modified_eopatch(eopatch: Optional[EOPatch], bbox: Optional[BBox]) -> Tuple[EOPatch, BBox]:
+    def _get_modified_eopatch(eopatch: EOPatch | None, bbox: BBox | None) -> tuple[EOPatch, BBox]:
         if bbox is not None:
             if eopatch is None:
                 eopatch = EOPatch(bbox=bbox)
             elif eopatch.bbox is None:
                 eopatch.bbox = bbox
             elif eopatch.bbox != bbox:
                 raise ValueError("Provided eopatch.bbox and bbox are not the same")
             return eopatch, bbox
 
         if eopatch is None or eopatch.bbox is None:
             raise ValueError("Bounding box is not provided")
         return eopatch, eopatch.bbox
 
-    def _prepare_time_intervals(self, eopatch: EOPatch, time_interval: Optional[RawTimeIntervalType]) -> List[str]:
+    def _prepare_time_intervals(self, eopatch: EOPatch, time_interval: RawTimeIntervalType | None) -> list[str]:
         """Prepare a list of time intervals for which data will be collected from meteoblue services"""
         if not eopatch.timestamps and not time_interval:
             raise ValueError(
                 "Time interval should either be defined with `eopatch.timestamps` or `time_interval` parameter"
             )
 
         if time_interval:
             serialized_start_time, serialized_end_time = serialize_time(parse_time_interval(time_interval))
             return [f"{serialized_start_time}/{serialized_end_time}"]
 
         timestamps = eopatch.timestamps
-        time_intervals: List[str] = []
+        time_intervals: list[str] = []
         for timestamp in timestamps:
             start_time = timestamp - self.time_difference
             end_time = timestamp + self.time_difference
 
             serizalized_start_time, serizalized_end_time = serialize_time((start_time, end_time))
 
             time_intervals.append(f"{serizalized_start_time}/{serizalized_end_time}")
 
         return time_intervals
 
     @abstractmethod
-    def _get_data(self, query: dict) -> Tuple[Any, List[dt.datetime]]:
+    def _get_data(self, query: dict) -> tuple[Any, list[dt.datetime]]:
         """It should return an output feature object and a list of timestamps"""
 
     def execute(
         self,
-        eopatch: Optional[EOPatch] = None,
+        eopatch: EOPatch | None = None,
         *,
-        query: Optional[dict] = None,
-        bbox: Optional[BBox] = None,
-        time_interval: Optional[RawTimeIntervalType] = None,
+        query: dict | None = None,
+        bbox: BBox | None = None,
+        time_interval: RawTimeIntervalType | None = None,
     ) -> EOPatch:
         """Execute method that adds new meteoblue data into an EOPatch
 
         :param eopatch: An EOPatch in which data will be added. If not provided a new EOPatch will be created.
         :param bbox: A bounding box of a request. Should be provided if eopatch parameter is not provided.
         :param query: meteoblue dataset API query definition. This query takes precedence over one defined in __init__.
         :param time_interval: An interval for which data should be downloaded. If not provided then timestamps from
@@ -163,15 +165,15 @@
     The data is obtained as a VECTOR feature in a ``geopandas.GeoDataFrame`` where columns include latitude, longitude,
     timestamp and a column for each weather variable. All data is downloaded from the
     meteoblue dataset API (<https://docs.meteoblue.com/en/weather-apis/dataset-api/dataset-api>).
 
     A meteoblue API key is required to retrieve data.
     """
 
-    def _get_data(self, query: dict) -> Tuple[gpd.GeoDataFrame, List[dt.datetime]]:
+    def _get_data(self, query: dict) -> tuple[gpd.GeoDataFrame, list[dt.datetime]]:
         """Provides a GeoDataFrame with information about weather control points and an empty list of timestamps"""
         result = self.client.querySync(query)
         dataframe = meteoblue_to_dataframe(result)
         geometry = gpd.points_from_xy(dataframe.Longitude, dataframe.Latitude)
         crs = CRS.WGS84.pyproj_crs()
         gdf = gpd.GeoDataFrame(dataframe, geometry=geometry, crs=crs)
         return gdf, []
@@ -183,15 +185,15 @@
     It returns a 4D numpy array with dimensions (time, height, width, weather variables) which should be stored as a
     DATA feature. Data is resampled to WGS84 plate carrée to a specified resolution using the
     meteoblue dataset API (<https://docs.meteoblue.com/en/weather-apis/dataset-api/dataset-api>).
 
     A meteoblue API key is required to retrieve data.
     """
 
-    def _get_data(self, query: dict) -> Tuple[np.ndarray, List[dt.datetime]]:
+    def _get_data(self, query: dict) -> tuple[np.ndarray, list[dt.datetime]]:
         """Return a 4-dimensional numpy array of shape (time, height, width, weather variables) and a list of
         timestamps
         """
         result = self.client.querySync(query)
 
         data = meteoblue_to_numpy(result)
         timestamps = _meteoblue_timestamps_from_geometry(result.geometries[0])
@@ -204,15 +206,15 @@
     :param result: A response of meteoblue API of type `Dataset_pb2.DatasetApiProtobuf`
     :returns: A dataframe with columns TIMESTAMP, Longitude, Latitude and aggregation columns
     """
     geometry = result.geometries[0]
     code_names = [f"{code.code}_{code.level}_{code.aggregation}" for code in geometry.codes]
 
     if not geometry.timeIntervals:
-        return pd.DataFrame(columns=[TIMESTAMP_COLUMN, "Longitude", "Latitude"] + code_names)
+        return pd.DataFrame(columns=[TIMESTAMP_COLUMN, "Longitude", "Latitude", *code_names])
 
     dataframes = []
     for index, time_interval in enumerate(geometry.timeIntervals):
         timestamps = _meteoblue_timestamps_from_time_interval(time_interval)
 
         n_locations = len(geometry.lats)
         n_timesteps = len(timestamps)
@@ -267,20 +269,20 @@
 
     n_timesteps = data.size // n_locations // n_codes
     data = data.reshape((n_codes, n_timesteps, geo_ny, geo_nx))
 
     return data.transpose((1, 2, 3, 0))
 
 
-def _meteoblue_timestamps_from_geometry(geometry_pb: Any) -> List[dt.datetime]:
+def _meteoblue_timestamps_from_geometry(geometry_pb: Any) -> list[dt.datetime]:
     """Transforms a protobuf geometry object into a list of datetime objects"""
     return list(pd.core.common.flatten(map(_meteoblue_timestamps_from_time_interval, geometry_pb.timeIntervals)))
 
 
-def _meteoblue_timestamps_from_time_interval(timestamp_pb: Any) -> List[dt.datetime]:
+def _meteoblue_timestamps_from_time_interval(timestamp_pb: Any) -> list[dt.datetime]:
     """Transforms a protobuf timestamp object into a list of datetime objects"""
     if timestamp_pb.timestrings:
         # Time intervals like weekly data, return an `array of strings` as timestamps
         # For time indications like `20200801T0000-20200802T235959` we only return the first date as datetime
         return list(map(_parse_timestring, timestamp_pb.timestrings))
 
     # Regular time intervals return `start, end and stride` as a time axis
```

### Comparing `eo-learn-io-1.4.1/eolearn/io/geometry_io.py` & `eo-learn-io-1.4.2/eolearn/io/geometry_io.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,17 +3,20 @@
 
 Copyright (c) 2017- Sinergise and contributors
 For the full list of contributors, see the CREDITS file in the root directory of this source tree.
 
 This source code is licensed under the MIT license, see the LICENSE file in the root directory of this source tree.
 """
 
+from __future__ import annotations
+
 import abc
 import logging
-from typing import Any, Optional, Union
+from contextlib import nullcontext
+from typing import Any
 
 import boto3
 import fiona
 import geopandas as gpd
 from fiona.session import AWSSession
 from fs.base import FS
 from fs_s3fs import S3FS
@@ -27,32 +30,32 @@
 LOGGER = logging.getLogger(__name__)
 
 
 class _BaseVectorImportTask(EOTask, metaclass=abc.ABCMeta):
     """Base Vector Import Task, implementing common methods"""
 
     def __init__(
-        self, feature: FeatureSpec, reproject: bool = True, clip: bool = False, config: Optional[SHConfig] = None
+        self, feature: FeatureSpec, reproject: bool = True, clip: bool = False, config: SHConfig | None = None
     ):
         """
         :param feature: A vector feature into which to import data
         :param reproject: Should the geometries be transformed to coordinate reference system of the requested bbox?
         :param clip: Should the geometries be clipped to the requested bbox, or should be geometries kept as they are?
         :param config: A configuration object with credentials
         """
         self.feature = self.parse_feature(feature, allowed_feature_types=lambda fty: fty.is_vector())
         self.config = config or SHConfig()
         self.reproject = reproject
         self.clip = clip
 
     @abc.abstractmethod
-    def _load_vector_data(self, bbox: Optional[BBox]) -> gpd.GeoDataFrame:
+    def _load_vector_data(self, bbox: BBox | None) -> gpd.GeoDataFrame:
         """Loads vector data given a bounding box"""
 
-    def _reproject_and_clip(self, vectors: gpd.GeoDataFrame, bbox: Optional[BBox]) -> gpd.GeoDataFrame:
+    def _reproject_and_clip(self, vectors: gpd.GeoDataFrame, bbox: BBox | None) -> gpd.GeoDataFrame:
         """Method to reproject and clip vectors to the EOPatch crs and bbox"""
 
         if self.reproject:
             if not bbox:
                 raise ValueError("To reproject vector data, eopatch.bbox has to be defined!")
 
             vectors = vectors.to_crs(bbox.crs.pyproj_crs())
@@ -66,15 +69,15 @@
                 raise ValueError("To clip, vectors should be in same CRS as EOPatch bbox!")
 
             extent = gpd.GeoSeries([bbox.geometry], crs=bbox_crs)
             vectors = gpd.clip(vectors, extent, keep_geom_type=True)
 
         return vectors
 
-    def execute(self, eopatch: Optional[EOPatch] = None, *, bbox: Optional[BBox] = None) -> EOPatch:
+    def execute(self, eopatch: EOPatch | None = None, *, bbox: BBox | None = None) -> EOPatch:
         """
         :param eopatch: An existing EOPatch. If none is provided it will create a new one.
         :param bbox: A bounding box for which to load data. By default, if none is provided, it will take a bounding box
             of given EOPatch. If given EOPatch is not provided it will load the entire dataset.
         :return: An EOPatch with an additional vector feature
         """
         if bbox is None and eopatch is not None:
@@ -98,16 +101,16 @@
 
     def __init__(
         self,
         feature: FeatureSpec,
         path: str,
         reproject: bool = True,
         clip: bool = False,
-        filesystem: Optional[FS] = None,
-        config: Optional[SHConfig] = None,
+        filesystem: FS | None = None,
+        config: SHConfig | None = None,
         **kwargs: Any,
     ):
         """
         :param feature: A vector feature into which to import data
         :param path: A path to a dataset containing vector data. It can be either a local path or a path to s3 bucket.
             If `filesystem` parameter is given the path should be relative to the filesystem, otherwise it should
             be an absolute path.
@@ -121,15 +124,15 @@
             filesystem, path = get_base_filesystem_and_path(path, config=config)
         self.path = path
         self.full_path = get_full_path(filesystem, path)
         self._pickled_filesystem = pickle_fs(filesystem)
 
         self.fiona_kwargs = kwargs
         self._aws_session = None
-        self._dataset_crs: Optional[CRS] = None
+        self._dataset_crs: CRS | None = None
 
         super().__init__(feature=feature, reproject=reproject, clip=clip, config=config)
 
     @property
     def aws_session(self) -> AWSSession:
         """Because the session object cannot be pickled this provides the session lazily (i.e. the first time it is
         needed)
@@ -148,74 +151,65 @@
                 region_name=filesystem.region,
             )
             self._aws_session = AWSSession(boto_session)
 
         return self._aws_session
 
     @property
-    def dataset_crs(self) -> Optional[CRS]:
-        """Provides a CRS of dataset, it loads it lazily (i.e. the first time it is needed)
-
-        :return: Dataset's CRS
-        """
+    def dataset_crs(self) -> CRS:
+        """Provides a CRS of dataset, it loads it lazily (i.e. the first time it is needed)"""
         if self._dataset_crs is None:
-            if self.full_path.startswith("s3://"):
-                with fiona.Env(session=self.aws_session):
-                    self._read_crs()
-            else:
-                self._read_crs()
+            is_on_s3 = self.full_path.startswith("s3://")
+            with fiona.Env(session=self.aws_session) if is_on_s3 else nullcontext():
+                with fiona.open(self.full_path, **self.fiona_kwargs) as features:
+                    self._dataset_crs = CRS(features.crs)
 
         return self._dataset_crs
 
-    def _read_crs(self) -> None:
-        """Reads information about CRS from a dataset"""
-        with fiona.open(self.full_path, **self.fiona_kwargs) as features:
-            self._dataset_crs = CRS(features.crs)
-
-    def _load_vector_data(self, bbox: Optional[BBox]) -> gpd.GeoDataFrame:
+    def _load_vector_data(self, bbox: BBox | None) -> gpd.GeoDataFrame:
         """Loads vector data either from S3 or local path"""
-        bbox_bounds = bbox.transform_bounds(self.dataset_crs).geometry.bounds if bbox and self.dataset_crs else None
+        bbox_bounds = bbox.transform_bounds(self.dataset_crs).geometry.bounds if bbox else None
 
         if self.full_path.startswith("s3://"):
             with fiona.Env(session=self.aws_session), fiona.open(self.full_path, **self.fiona_kwargs) as features:
                 feature_iter = features if bbox_bounds is None else features.filter(bbox=bbox_bounds)
 
                 return gpd.GeoDataFrame.from_features(
                     feature_iter,
-                    columns=list(features.schema["properties"]) + ["geometry"],
-                    crs=self.dataset_crs.pyproj_crs() if self.dataset_crs else None,
+                    columns=list(features.schema["properties"]) + ["geometry"],  # noqa: RUF005
+                    crs=self.dataset_crs.pyproj_crs(),
                 )
 
         return gpd.read_file(self.full_path, bbox=bbox_bounds, **self.fiona_kwargs)
 
 
 class GeopediaVectorImportTask(_BaseVectorImportTask):
     """A task for importing `Geopedia <https://geopedia.world>`__ features into EOPatch vector features"""
 
     def __init__(
         self,
         feature: FeatureSpec,
-        geopedia_table: Union[str, int],
+        geopedia_table: str | int,
         reproject: bool = True,
         clip: bool = False,
         **kwargs: Any,
     ):
         """
         :param feature: A vector feature into which to import data
         :param geopedia_table: A Geopedia table from which to retrieve features
         :param reproject: Should the geometries be transformed to coordinate reference system of the requested bbox?
         :param clip: Should the geometries be clipped to the requested bbox, or should be geometries kept as they are?
         :param kwargs: Additional args that will be passed to `GeopediaFeatureIterator`
         """
         self.geopedia_table = geopedia_table
         self.geopedia_kwargs = kwargs
-        self.dataset_crs: Optional[CRS] = None
+        self.dataset_crs: CRS | None = None
         super().__init__(feature=feature, reproject=reproject, clip=clip)
 
-    def _load_vector_data(self, bbox: Optional[BBox]) -> gpd.GeoDataFrame:
+    def _load_vector_data(self, bbox: BBox | None) -> gpd.GeoDataFrame:
         """Loads vector data from geopedia table"""
         prepared_bbox = bbox.transform_bounds(CRS.POP_WEB) if bbox else None
 
         geopedia_iterator = GeopediaFeatureIterator(
             layer=self.geopedia_table,
             bbox=prepared_bbox,
             offset=0,
```

### Comparing `eo-learn-io-1.4.1/eolearn/io/geopedia.py` & `eo-learn-io-1.4.2/eolearn/io/geopedia.py`

 * *Files identical despite different names*

### Comparing `eo-learn-io-1.4.1/eolearn/io/raster_io.py` & `eo-learn-io-1.4.2/eolearn/io/raster_io.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,20 +2,22 @@
 Module containing tasks used for reading and writing to disk
 
 Copyright (c) 2017- Sinergise and contributors
 For the full list of contributors, see the CREDITS file in the root directory of this source tree.
 
 This source code is licensed under the MIT license, see the LICENSE file in the root directory of this source tree.
 """
+from __future__ import annotations
+
 import datetime as dt
 import functools
 import logging
 import warnings
 from abc import ABCMeta
-from typing import Any, BinaryIO, List, Optional, Tuple, Union
+from typing import Any, BinaryIO
 
 import fs
 import numpy as np
 import rasterio
 import rasterio.warp
 from affine import Affine
 from fs.base import FS
@@ -33,35 +35,34 @@
 from eolearn.core.exceptions import EORuntimeWarning
 from eolearn.core.types import SingleFeatureSpec
 from eolearn.core.utils.fs import get_base_filesystem_and_path, get_full_path
 
 LOGGER = logging.getLogger(__name__)
 
 
-class BaseRasterIoTask(IOTask, metaclass=ABCMeta):  # noqa: B024
+class BaseRasterIoTask(IOTask, metaclass=ABCMeta):
     """Base abstract class for raster IO tasks"""
 
     def __init__(
         self,
         feature: SingleFeatureSpec,
         folder: str,
         *,
-        filesystem: Optional[FS] = None,
-        image_dtype: Optional[Union[np.dtype, type]] = None,
-        no_data_value: Optional[float] = None,
+        filesystem: FS | None = None,
+        image_dtype: np.dtype | type | None = None,
+        no_data_value: float | None = None,
         create: bool = False,
-        config: Optional[SHConfig] = None,
+        config: SHConfig | None = None,
     ):
         """
         :param feature: Feature which will be exported or imported
         :param folder: A path to a main folder containing all image, potentially in its subfolders. If `filesystem`
             parameter is defined, then `folder` should be a path relative to filesystem object. Otherwise, it should be
             an absolute path.
-        :param filesystem: An existing filesystem object. If not given it will be initialized according to `folder`
-            parameter.
+        :param filesystem: A filesystem object. If not given it will be initialized according to `folder` parameter.
         :param image_dtype: A data type of data in exported images or data imported from images.
         :param no_data_value: When exporting this is the NoData value of pixels in exported images.
             When importing this value is assigned to the pixels with NoData.
         :param create: If the filesystem path doesn't exist this flag indicates to either create it or raise an error.
         :param config: A configuration object with AWS credentials. By default, is set to None and in this case the
             default configuration will be taken.
         """
@@ -71,71 +72,67 @@
         self.feature = ftype, fname
         self.image_dtype = image_dtype
         self.no_data_value = no_data_value
 
         if filesystem is None:
             filesystem, folder = get_base_filesystem_and_path(folder, create=create, config=config)
 
+        # the super-class takes care of filesystem pickling
         super().__init__(folder, filesystem=filesystem, create=create, config=config)
 
-    def _get_filename_paths(self, filename_template: Union[str, List[str]], timestamps: List[dt.datetime]) -> List[str]:
+    def _get_filename_paths(self, filename_template: str | list[str], timestamps: list[dt.datetime]) -> list[str]:
         """From a filename "template" and base path on the filesystem it generates full paths to tiff files. The paths
         are still relative to the filesystem object.
+
+        If the file extension is not provided, it will default to `.tif`. If a "*" wildcard or a datetime format
+        substring (e.g. "%Y%m%dT%H%M%S") is provided in the template, it returns multiple GeoTIFF paths where each one
+        will correspond to a single timestamp. Alternatively, a list of paths can be provided, one for each timestamp.
         """
         if isinstance(filename_template, str):
             filename_path = fs.path.join(self.filesystem_path, filename_template)
             filename_paths = self._generate_paths(filename_path, timestamps)
 
         elif isinstance(filename_template, list):
-            filename_paths = []
-            for timestamp_index, path in enumerate(filename_template):
-                filename_path = fs.path.join(self.filesystem_path, path)
-                if len(filename_template) == len(timestamps):
-                    filename_paths.extend(self._generate_paths(filename_path, [timestamps[timestamp_index]]))
-                elif not timestamps:
-                    filename_paths.extend(self._generate_paths(filename_path, timestamps))
-                else:
-                    raise ValueError(
-                        "The number of provided timestamps does not match the number of provided filenames."
-                    )
+            if timestamps and len(filename_template) != len(timestamps):
+                raise ValueError("The number of provided timestamps does not match the number of provided filenames.")
+
+            filenames = []
+            for idx, path in enumerate(filename_template):
+                timestamps = [] if not timestamps else [timestamps[idx]]
+                filenames.extend(self._generate_paths(path, timestamps))
+
+            filename_paths = [fs.path.join(self.filesystem_path, path) for path in filenames]
+
         else:
-            raise TypeError(
-                f"The 'filename' parameter must either be a list or a string, but {filename_template} found"
-            )
+            raise TypeError(f"The `filename` parameter must be a list or a string, but {filename_template} found")
 
         if self._create_path:
-            paths_to_create = {fs.path.dirname(filename_path) for filename_path in filename_paths}
-            for filename_path in paths_to_create:
-                self.filesystem.makedirs(filename_path, recreate=True)
+            unique_folder_paths = {fs.path.dirname(filename_path) for filename_path in filename_paths}
+            for folder_path in unique_folder_paths:
+                self.filesystem.makedirs(folder_path, recreate=True)
 
         return filename_paths
 
     @classmethod
-    def _generate_paths(cls, path_template: str, timestamps: List[dt.datetime]) -> List[str]:
+    def _generate_paths(cls, path_template: str, timestamps: list[dt.datetime]) -> list[str]:
         """Uses a filename path template to create a list of actual filename paths."""
-        if not cls._has_tiff_file_extension(path_template):
+        has_tiff_file_extensions = path_template.lower().endswith(".tif") or path_template.lower().endswith(".tiff")
+        if not has_tiff_file_extensions:
             path_template = f"{path_template}.tif"
 
         if not timestamps:
             return [path_template]
 
-        if "*" in path_template:
-            path_template = path_template.replace("*", "%Y%m%dT%H%M%S")
+        path_template = path_template.replace("*", "%Y%m%dT%H%M%S")
 
-        if timestamps[0].strftime(path_template) == path_template:
+        if timestamps[0].strftime(path_template) == path_template:  # unaffected by timestamps
             return [path_template]
 
         return [timestamp.strftime(path_template) for timestamp in timestamps]
 
-    @staticmethod
-    def _has_tiff_file_extension(path: str) -> bool:
-        """Checks if path ends with a tiff file extension."""
-        path = path.lower()
-        return path.endswith(".tif") or path.endswith(".tiff")
-
 
 class ExportToTiffTask(BaseRasterIoTask):
     """Task exports specified feature to GeoTIFF.
 
     The task can export also features with sizes of both time and band dimension greater than `1`. When exporting
     only multiple times or only multiple bands, the GeoTIFF channels are in the expected order. However, when
     exporting multiple times and bands, the order obeys the following pattern:
@@ -147,19 +144,19 @@
     """
 
     def __init__(
         self,
         feature: SingleFeatureSpec,
         folder: str,
         *,
-        date_indices: Union[List[int], Tuple[int, int], Tuple[dt.datetime, dt.datetime], Tuple[str, str], None] = None,
-        band_indices: Union[List[int], Tuple[int, int], None] = None,
-        crs: Union[CRS, int, str, None] = None,
+        date_indices: list[int] | tuple[int, int] | tuple[dt.datetime, dt.datetime] | tuple[str, str] | None = None,
+        band_indices: list[int] | tuple[int, int] | None = None,
+        crs: CRS | int | str | None = None,
         fail_on_missing: bool = True,
-        compress: Optional[str] = None,
+        compress: str | None = None,
         **kwargs: Any,
     ):
         """
         :param feature: A feature to be exported.
         :param folder: A path to a main folder containing all image, potentially in its subfolders. If `filesystem`
             parameter is defined, then `folder` should be a path relative to filesystem object. Otherwise, it should be
             an absolute path.
@@ -181,26 +178,25 @@
         self.date_indices = date_indices
         self.band_indices = band_indices
         self.crs = None if crs is None else CRS(crs)
         self.fail_on_missing = fail_on_missing
         self.compress = compress
 
     def _prepare_image_array(
-        self, data_array: np.ndarray, timestamps: List[dt.datetime], feature: Tuple[FeatureType, str]
+        self, data_array: np.ndarray, timestamps: list[dt.datetime], feature: tuple[FeatureType, str]
     ) -> np.ndarray:
         """Collects a feature from EOPatch and prepares the array of an image which will be rasterized. The resulting
         array has shape (channels, height, width) and is of correct dtype.
         """
         data_array = self._reduce_by_bands(data_array)
 
         feature_type, _ = feature
         if feature_type.is_temporal():
             data_array = self._reduce_by_time(data_array, timestamps)
         else:
-            # add temporal dimension
             data_array = np.expand_dims(data_array, axis=0)
 
         if not feature_type.is_spatial():
             # add height and width dimensions
             data_array = np.expand_dims(np.expand_dims(data_array, axis=1), axis=1)
 
         data_array = self._set_export_dtype(data_array, feature)
@@ -224,95 +220,85 @@
         if isinstance(self.band_indices, tuple):
             if tuple(map(type, self.band_indices)) != (int, int):
                 raise ValueError(f"Invalid format in {self.band_indices} tuple, expected integers")
             return array[..., self.band_indices[0] : self.band_indices[1] + 1]
 
         raise ValueError(f"Invalid format in {self.band_indices}, expected tuple or list")
 
-    def _reduce_by_time(self, array: np.ndarray, timestamps: List[dt.datetime]) -> np.ndarray:
+    def _reduce_by_time(self, data_array: np.ndarray, timestamps: list[dt.datetime]) -> np.ndarray:
         """Reduce array by selecting a subset of times."""
         if self.date_indices is None:
-            return array
+            return data_array
 
         if isinstance(self.date_indices, list):
             if [date for date in self.date_indices if not isinstance(date, int)]:
                 raise ValueError(f"Invalid format in {self.date_indices} list, expected integers")
-            return array[np.array(self.date_indices), ...]
+            return data_array[np.array(self.date_indices), ...]
 
         if isinstance(self.date_indices, tuple):
             dates = np.array(timestamps)
             start_idx, end_idx = self.date_indices
             if isinstance(start_idx, int) and isinstance(end_idx, int):
                 start_date, end_date = dates[start_idx], dates[end_idx]
             elif isinstance(start_idx, str) and isinstance(end_idx, str):
                 start_date, end_date = parse_time_interval((start_idx, end_idx))
             elif isinstance(start_idx, dt.datetime) and isinstance(end_idx, dt.datetime):
                 start_date, end_date = start_idx, end_idx
             else:
                 raise ValueError(f"Invalid format in {self.date_indices} tuple, expected ints, strings, or datetimes")
-            return array[np.nonzero(np.where((dates >= start_date) & (dates <= end_date), dates, 0))[0]]
+            return data_array[np.nonzero(np.where((dates >= start_date) & (dates <= end_date), dates, 0))[0]]
 
         raise ValueError(f"Invalid format in {self.date_indices}, expected tuple or list")
 
-    def _set_export_dtype(self, data_array: np.ndarray, feature: Tuple[FeatureType, str]) -> np.ndarray:
+    def _set_export_dtype(self, data_array: np.ndarray, feature: tuple[FeatureType, str]) -> np.ndarray:
         """To a given array it sets a dtype in which data will be exported"""
         image_dtype = data_array.dtype if self.image_dtype is None else self.image_dtype
 
         if image_dtype == np.int64:
             image_dtype = np.int32
             warnings.warn(
-                (
-                    f"Data from feature {feature} cannot be exported to tiff with dtype numpy.int64. Will export "
-                    "as numpy.int32 instead"
-                ),
-                EORuntimeWarning,
+                f"Cannot export {feature} with dtype numpy.int64. Will export as numpy.int32 instead", EORuntimeWarning
             )
 
-        if image_dtype == data_array.dtype:
-            return data_array
-        return data_array.astype(image_dtype)
+        return data_array.astype(image_dtype) if image_dtype != data_array.dtype else data_array
 
     def _get_source_and_destination_params(
         self, data_array: np.ndarray, bbox: BBox
-    ) -> Tuple[Tuple[str, Affine], Tuple[str, Affine], Tuple[int, int]]:
-        """
-        Calculates source and destination CRS and transforms. Additionally, it returns destination height and width
-        """
+    ) -> tuple[tuple[str, Affine], tuple[str, Affine], tuple[int, int]]:
+        """Calculates source and destination CRS and transforms. Also returns destination height and width."""
         _, height, width = data_array.shape
 
         src_crs = bbox.crs.ogc_string()
         src_transform = rasterio.transform.from_bounds(*bbox, width=width, height=height)
 
-        if self.crs:
-            dst_crs = self.crs.ogc_string()
-            dst_transform, dst_width, dst_height = rasterio.warp.calculate_default_transform(
-                src_crs, dst_crs, width, height, *bbox
-            )
-        else:
-            dst_crs = src_crs
-            dst_transform = src_transform
-            dst_width, dst_height = width, height
+        if self.crs is None:
+            return (src_crs, src_transform), (src_crs, src_transform), (height, width)
 
+        dst_crs = self.crs.ogc_string()
+        dst_transform, dst_width, dst_height = rasterio.warp.calculate_default_transform(
+            src_crs, dst_crs, width, height, *bbox
+        )
         return (src_crs, src_transform), (dst_crs, dst_transform), (dst_height, dst_width)
 
     def _export_tiff(
         self,
         image_array: np.ndarray,
         filesystem: FS,
         path: str,
         channel_count: int,
+        *,
         dst_crs: str,
         dst_transform: Affine,
         dst_height: int,
         dst_width: int,
         src_crs: str,
         src_transform: Affine,
     ) -> None:
         """Export an EOPatch feature to tiff based on input channel range."""
-        with rasterio.Env(), filesystem.openbin(path, "w") as file_handle:  # noqa: SIM117
+        with rasterio.Env(), filesystem.openbin(path, "w") as file_handle:
             with rasterio.open(
                 file_handle,
                 "w",
                 driver="GTiff",
                 width=dst_width,
                 height=dst_height,
                 count=channel_count,
@@ -332,15 +318,15 @@
                             src_transform=src_transform,
                             src_crs=src_crs,
                             dst_transform=dst_transform,
                             dst_crs=dst_crs,
                             resampling=rasterio.warp.Resampling.nearest,
                         )
 
-    def execute(self, eopatch: EOPatch, *, filename: Union[str, List[str], None] = "") -> EOPatch:
+    def execute(self, eopatch: EOPatch, *, filename: str | list[str] | None = "") -> EOPatch:
         """Execute method
 
         :param eopatch: An input EOPatch
         :param filename: A filename with a path to a tiff file. The path has to be a relative to the filesystem object
             and path from `folder` initialization parameter. If the file extension of the image file is not provided,
             it will default to `.tif`. If a "*" wildcard or a datetime.strftime substring (e.g. "%Y%m%dT%H%M%S") is
             provided in the path, an EOPatch feature will be split over multiple GeoTIFFs where each one will correspond
@@ -348,35 +334,31 @@
             parameter to `None` to disable exporting.
         :return: Unchanged input EOPatch
         """
         if filename is None:
             return eopatch
 
         if self.feature not in eopatch:
-            error_msg = f"Feature {self.feature[1]} of type {self.feature[0]} was not found in EOPatch"
+            error_msg = f"Feature {self.feature} was not found in EOPatch"
             LOGGER.warning(error_msg)
             if self.fail_on_missing:
                 raise ValueError(error_msg)
             return eopatch
         if eopatch.bbox is None:
-            raise ValueError(
-                "Given EOPatch is missing a bounding box and therefore no feature can be exported to GeoTIFF"
-            )
+            raise ValueError("EOPatch without a bounding box encountered, cannot export to GeoTIFF")
 
         image_array = self._prepare_image_array(eopatch[self.feature], eopatch.timestamps, self.feature)
 
-        (
-            (src_crs, src_transform),
-            (dst_crs, dst_transform),
-            (dst_height, dst_width),
-        ) = self._get_source_and_destination_params(image_array, eopatch.bbox)
+        src_info, dst_info, (dst_height, dst_width) = self._get_source_and_destination_params(image_array, eopatch.bbox)
+        src_crs, src_transform = src_info
+        dst_crs, dst_transform = dst_info
 
         filename_paths = self._get_filename_paths(filename, eopatch.timestamps)
 
-        with self.filesystem as filesystem:
+        with self.filesystem as filesystem:  # no worries about `close`, filesystem is freshly unpickled by the property
             export_function = functools.partial(
                 self._export_tiff,
                 filesystem=filesystem,
                 dst_crs=dst_crs,
                 dst_transform=dst_transform,
                 dst_height=dst_height,
                 dst_width=dst_width,
@@ -411,15 +393,15 @@
 
     def __init__(
         self,
         feature: SingleFeatureSpec,
         folder: str,
         *,
         use_vsi: bool = False,
-        timestamp_size: Optional[int] = None,
+        timestamp_size: int | None = None,
         **kwargs: Any,
     ):
         """
         :param feature: EOPatch feature into which data will be imported
         :param folder: A directory containing image files or a path of an image file
         :param use_vsi: A flag to define if reading should be done with GDAL/rasterio virtual system (VSI)
             functionality. The flag only has an effect when the task is used to read an image from a remote storage
@@ -448,15 +430,15 @@
             aws_access_key_id=filesystem.aws_access_key_id,
             aws_secret_access_key=filesystem.aws_secret_access_key,
             aws_session_token=filesystem.aws_session_token,
             region_name=filesystem.region,
             endpoint_url=filesystem.endpoint_url,
         )
 
-    def _load_from_image(self, path: str, filesystem: FS, bbox: Optional[BBox]) -> Tuple[np.ndarray, Optional[BBox]]:
+    def _load_from_image(self, path: str, filesystem: FS, bbox: BBox | None) -> tuple[np.ndarray, BBox | None]:
         """The method decides in what way data will be loaded from the image.
 
         The method always uses `rasterio.Env` to suppress any low-level warnings. In case of a local filesystem
         benchmarks show that without `filesystem.openbin` in some cases `rasterio` can read much faster. Otherwise,
         reading depends on `use_vsi` flag. In some cases where a sub-image window is read and the image is in certain
         format (e.g. COG), benchmarks show that reading with virtual system (VSI) is much faster. In other cases,
         reading with `filesystem.openbin` is faster.
@@ -471,26 +453,24 @@
             with rasterio.Env(session=session):
                 full_path = get_full_path(filesystem, path)
                 return self._read_image(full_path, bbox)
 
         with rasterio.Env(), filesystem.openbin(path, "r") as file_handle:
             return self._read_image(file_handle, bbox)
 
-    def _read_image(self, file_object: Union[str, BinaryIO], bbox: Optional[BBox]) -> Tuple[np.ndarray, Optional[BBox]]:
+    def _read_image(self, file_object: str | BinaryIO, bbox: BBox | None) -> tuple[np.ndarray, BBox | None]:
         """Reads data from the image."""
         src: DatasetReader
         with rasterio.open(file_object) as src:
             read_window, read_bbox = self._get_reading_window_and_bbox(src, bbox)
             boundless_reading = read_window is not None
             return src.read(window=read_window, boundless=boundless_reading, fill_value=self.no_data_value), read_bbox
 
     @staticmethod
-    def _get_reading_window_and_bbox(
-        reader: DatasetReader, bbox: Optional[BBox]
-    ) -> Tuple[Optional[Window], Optional[BBox]]:
+    def _get_reading_window_and_bbox(reader: DatasetReader, bbox: BBox | None) -> tuple[Window | None, BBox | None]:
         """Provides a reading window for which data will be read from image. If it returns `None` this means that the
         whole image should be read. Those cases are when bbox is not defined, image is not geo-referenced, or
         bbox coordinates exactly match image coordinates. Additionally, it provides a bounding box of reading window
         if an image is geo-referenced."""
         image_crs = reader.crs
         image_transform = reader.transform
         image_bounds = reader.bounds
@@ -507,18 +487,18 @@
             bbox = bbox.transform(image_crs.to_epsg())
 
         if bbox == image_bbox:
             return None, original_bbox
 
         return from_bounds(*iter(bbox), transform=image_transform), original_bbox
 
-    def _load_data(self, filename_paths: List[str], initial_bbox: Optional[BBox]) -> Tuple[np.ndarray, Optional[BBox]]:
+    def _load_data(self, filename_paths: list[str], initial_bbox: BBox | None) -> tuple[np.ndarray, BBox | None]:
         """Load data from images, join them, and provide their bounding box."""
-        data_per_path: List[np.ndarray] = []
-        final_bbox: Optional[BBox] = None
+        data_per_path = []
+        final_bbox: BBox | None = None
 
         with self.filesystem as filesystem:
             for path in filename_paths:
                 data, bbox = self._load_from_image(path, filesystem, initial_bbox)
                 data_per_path.append(data)
 
                 if bbox is None:
@@ -528,15 +508,15 @@
                         "Given images have different geo-references. They can't be imported into an EOPatch that"
                         " doesn't have a bounding box."
                     )
                 final_bbox = bbox
 
         return np.concatenate(data_per_path, axis=0), final_bbox
 
-    def execute(self, eopatch: Optional[EOPatch] = None, *, filename: Optional[str] = "") -> EOPatch:
+    def execute(self, eopatch: EOPatch | None = None, *, filename: str | None = "") -> EOPatch:
         """Execute method which adds a new feature to the EOPatch.
 
         :param eopatch: input EOPatch or None if a new EOPatch should be created
         :param filename: filename of tiff file or None if entire path has already been specified in `folder` parameter
             of task initialization.
         """
         if filename is None:
```

### Comparing `eo-learn-io-1.4.1/eolearn/io/sentinelhub_process.py` & `eo-learn-io-1.4.2/eolearn/io/sentinelhub_process.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,59 +7,58 @@
 This source code is licensed under the MIT license, see the LICENSE file in the root directory of this source tree.
 """
 from __future__ import annotations
 
 import datetime as dt
 import logging
 from abc import ABCMeta, abstractmethod
-from typing import Any, Callable, Dict, Iterable, List, Optional, Tuple, Union, cast
+from typing import Any, Callable, Iterable, List, Literal, Tuple, cast
 
 import numpy as np
-from typing_extensions import Literal
 
 from sentinelhub import (
     BBox,
     DataCollection,
     Geometry,
     MimeType,
     MosaickingOrder,
     ResamplingType,
-    SentinelHubCatalog,
     SentinelHubDownloadClient,
     SentinelHubRequest,
     SentinelHubSession,
     SHConfig,
     bbox_to_dimensions,
     filter_times,
     parse_time_interval,
 )
-from sentinelhub.data_collections_bands import Band
+from sentinelhub.api.catalog import get_available_timestamps
+from sentinelhub.evalscript import generate_evalscript, parse_data_collection_bands
 from sentinelhub.types import JsonDict, RawTimeIntervalType
 
 from eolearn.core import EOPatch, EOTask, FeatureType
 from eolearn.core.types import FeatureRenameSpec, FeatureSpec, FeaturesSpecification
-from eolearn.core.utils.parsing import parse_renamed_features
+from eolearn.core.utils.parsing import parse_renamed_feature, parse_renamed_features
 
 LOGGER = logging.getLogger(__name__)
 
 
 class SentinelHubInputBaseTask(EOTask, metaclass=ABCMeta):
     """Base class for Processing API input tasks"""
 
     def __init__(
         self,
         data_collection: DataCollection,
-        size: Optional[Tuple[int, int]] = None,
-        resolution: Optional[Union[float, Tuple[float, float]]] = None,
-        cache_folder: Optional[str] = None,
-        config: Optional[SHConfig] = None,
-        max_threads: Optional[int] = None,
-        upsampling: Optional[ResamplingType] = None,
-        downsampling: Optional[ResamplingType] = None,
-        session_loader: Optional[Callable[[], SentinelHubSession]] = None,
+        size: tuple[int, int] | None = None,
+        resolution: float | tuple[float, float] | None = None,
+        cache_folder: str | None = None,
+        config: SHConfig | None = None,
+        max_threads: int | None = None,
+        upsampling: ResamplingType | None = None,
+        downsampling: ResamplingType | None = None,
+        session_loader: Callable[[], SentinelHubSession] | None = None,
     ):
         """
         :param data_collection: A collection of requested satellite data.
         :param size: Number of pixels in x and y dimension.
         :param resolution: Resolution in meters, passed as a single number or a tuple of two numbers -
             resolution in horizontal and resolution in vertical direction.
         :param cache_folder: Path to cache_folder. If set to None (default) requests will not be cached.
@@ -81,18 +80,18 @@
         self.cache_folder = cache_folder
         self.session_loader = session_loader
         self.upsampling = upsampling
         self.downsampling = downsampling
 
     def execute(
         self,
-        eopatch: Optional[EOPatch] = None,
-        bbox: Optional[BBox] = None,
-        time_interval: Optional[RawTimeIntervalType] = None,  # should be kept at this to prevent code-breaks
-        geometry: Optional[Geometry] = None,
+        eopatch: EOPatch | None = None,
+        bbox: BBox | None = None,
+        time_interval: RawTimeIntervalType | None = None,  # should be kept at this to prevent code-breaks
+        geometry: Geometry | None = None,
     ) -> EOPatch:
         """Main execute method for the Process API tasks.
         The `geometry` is used only in conjunction with the `bbox` and does not act as a replacement."""
 
         eopatch_bbox = eopatch.bbox if eopatch is not None else None
         area_bbox = self._consolidate_bbox(bbox, eopatch_bbox)
 
@@ -126,78 +125,78 @@
 
         temporal_dim = 1 if timestamps is None else len(timestamps)
         shape = temporal_dim, size_y, size_x
         self._extract_data(eopatch, responses, shape)
 
         return eopatch
 
-    def _get_size(self, bbox: BBox) -> Tuple[int, int]:
+    def _get_size(self, bbox: BBox) -> tuple[int, int]:
         """Get the size (width, height) for the request either from inputs, or from the (existing) eopatch"""
         if self.size is not None:
             return self.size
 
         if self.resolution is not None:
             return bbox_to_dimensions(bbox, self.resolution)
 
         raise ValueError("Size or resolution for the requests should be provided!")
 
     @staticmethod
-    def _consolidate_bbox(bbox: Optional[BBox], eopatch_bbox: Optional[BBox]) -> BBox:
+    def _consolidate_bbox(bbox: BBox | None, eopatch_bbox: BBox | None) -> BBox:
         if eopatch_bbox is None:
             if bbox is None:
                 raise ValueError("Either the eopatch or the task must provide valid bbox.")
             return bbox
 
         if bbox is None or eopatch_bbox == bbox:
             return eopatch_bbox
         raise ValueError("Either the eopatch or the task must provide bbox, or they must be the same.")
 
     @abstractmethod
-    def _extract_data(self, eopatch: EOPatch, responses: List[Any], shape: Tuple[int, ...]) -> EOPatch:
+    def _extract_data(self, eopatch: EOPatch, responses: list[Any], shape: tuple[int, ...]) -> EOPatch:
         """Extract data from the received images and assign them to eopatch features"""
 
     @abstractmethod
     def _build_requests(
         self,
-        bbox: Optional[BBox],
+        bbox: BBox | None,
         size_x: int,
         size_y: int,
-        timestamps: Optional[List[dt.datetime]],
-        time_interval: Optional[RawTimeIntervalType],
-        geometry: Optional[Geometry],
-    ) -> List[SentinelHubRequest]:
+        timestamps: list[dt.datetime] | None,
+        time_interval: RawTimeIntervalType | None,
+        geometry: Geometry | None,
+    ) -> list[SentinelHubRequest]:
         """Build requests"""
 
     @abstractmethod
-    def _get_timestamps(self, time_interval: Optional[RawTimeIntervalType], bbox: BBox) -> List[dt.datetime]:
+    def _get_timestamps(self, time_interval: RawTimeIntervalType | None, bbox: BBox) -> list[dt.datetime]:
         """Get the timestamp array needed as a parameter for downloading the images"""
 
 
 class SentinelHubEvalscriptTask(SentinelHubInputBaseTask):
     """Process API task to download data using evalscript"""
 
     # pylint: disable=too-many-arguments
     def __init__(
         self,
         features: FeaturesSpecification,
         evalscript: str,
         data_collection: DataCollection,
-        size: Optional[Tuple[int, int]] = None,
-        resolution: Optional[Union[float, Tuple[float, float]]] = None,
-        maxcc: Optional[float] = None,
-        time_difference: Optional[dt.timedelta] = None,
-        mosaicking_order: Optional[Union[str, MosaickingOrder]] = None,
-        cache_folder: Optional[str] = None,
-        config: Optional[SHConfig] = None,
-        max_threads: Optional[int] = None,
-        upsampling: Optional[ResamplingType] = None,
-        downsampling: Optional[ResamplingType] = None,
-        aux_request_args: Optional[dict] = None,
-        session_loader: Optional[Callable[[], SentinelHubSession]] = None,
-        timestamp_filter: Callable[[List[dt.datetime], dt.timedelta], List[dt.datetime]] = filter_times,
+        size: tuple[int, int] | None = None,
+        resolution: float | tuple[float, float] | None = None,
+        maxcc: float | None = None,
+        time_difference: dt.timedelta | None = None,
+        mosaicking_order: str | MosaickingOrder | None = None,
+        cache_folder: str | None = None,
+        config: SHConfig | None = None,
+        max_threads: int | None = None,
+        upsampling: ResamplingType | None = None,
+        downsampling: ResamplingType | None = None,
+        aux_request_args: dict | None = None,
+        session_loader: Callable[[], SentinelHubSession] | None = None,
+        timestamp_filter: Callable[[list[dt.datetime], dt.timedelta], list[dt.datetime]] = filter_times,
     ):
         """
         :param features: Features to construct from the evalscript.
         :param evalscript: Evalscript for the request. Beware that all outputs from SentinelHub services should be named
             and should have the same name as corresponding feature
         :param data_collection: Source of requested satellite data.
         :param size: Number of pixels in x and y dimension.
@@ -239,83 +238,83 @@
 
         self.maxcc = maxcc
         self.time_difference = time_difference or dt.timedelta(seconds=1)
         self.timestamp_filter = timestamp_filter
         self.mosaicking_order = None if mosaicking_order is None else MosaickingOrder(mosaicking_order)
         self.aux_request_args = aux_request_args
 
-    def _parse_and_validate_features(self, features: FeaturesSpecification) -> List[FeatureRenameSpec]:
+    def _parse_and_validate_features(self, features: FeaturesSpecification) -> list[FeatureRenameSpec]:
         _features = parse_renamed_features(
             features, allowed_feature_types=lambda fty: fty.is_array() or fty == FeatureType.META_INFO
         )
 
         ftr_data_types = {ft for ft, _, _ in _features if not ft.is_meta()}
         if all(ft.is_timeless() for ft in ftr_data_types) or all(ft.is_temporal() for ft in ftr_data_types):
             return _features
 
         raise ValueError("Cannot mix time dependent and timeless requests!")
 
-    def _create_response_objects(self) -> List[JsonDict]:
+    def _create_response_objects(self) -> list[JsonDict]:
         """Construct SentinelHubRequest output_responses from features"""
         responses = []
         for feat_type, feat_name, _ in self.features:
             if feat_type.is_array():
                 feat_name = cast(str, feat_name)  # can only be string since it's an array type
                 responses.append(SentinelHubRequest.output_response(feat_name, MimeType.TIFF))
             elif feat_type.is_meta():
                 responses.append(SentinelHubRequest.output_response("userdata", MimeType.JSON))
             else:
                 # should not happen as features have already been validated
                 raise ValueError(f"{feat_type} not supported!")
 
         return responses
 
-    def _get_timestamps(self, time_interval: Optional[RawTimeIntervalType], bbox: BBox) -> List[dt.datetime]:
+    def _get_timestamps(self, time_interval: RawTimeIntervalType | None, bbox: BBox) -> list[dt.datetime]:
         """Get the timestamp array needed as a parameter for downloading the images"""
         if any(feat_type.is_timeless() for feat_type, _, _ in self.features if feat_type.is_array()):
             return []
 
-        return get_available_timestamps(
+        timestamps = get_available_timestamps(
             bbox=bbox,
             time_interval=time_interval,
-            timestamp_filter=self.timestamp_filter,
             data_collection=self.data_collection,
             maxcc=self.maxcc,
-            time_difference=self.time_difference,
             config=self.config,
         )
 
+        return self.timestamp_filter(timestamps, self.time_difference)
+
     def _build_requests(
         self,
-        bbox: Optional[BBox],
+        bbox: BBox | None,
         size_x: int,
         size_y: int,
-        timestamps: Optional[List[dt.datetime]],
-        time_interval: Optional[RawTimeIntervalType],
-        geometry: Optional[Geometry],
-    ) -> List[SentinelHubRequest]:
+        timestamps: list[dt.datetime] | None,
+        time_interval: RawTimeIntervalType | None,
+        geometry: Geometry | None,
+    ) -> list[SentinelHubRequest]:
         """Defines request timestamps and builds requests. In case `timestamps` is either `None` or an empty list it
         still has to create at least one request in order to obtain back number of bands of responses."""
-        dates: List[Optional[Tuple[Optional[dt.datetime], Optional[dt.datetime]]]]
+        dates: list[tuple[dt.datetime | None, dt.datetime | None] | None]
         if timestamps:
             dates = [(date - self.time_difference, date + self.time_difference) for date in timestamps]
         elif timestamps is None:
             dates = [None]
         else:
             dates = [parse_time_interval(time_interval, allow_undefined=True)]
 
         return [self._create_sh_request(date, bbox, size_x, size_y, geometry) for date in dates]
 
     def _create_sh_request(
         self,
-        time_interval: Optional[RawTimeIntervalType],
-        bbox: Optional[BBox],
+        time_interval: RawTimeIntervalType | None,
+        bbox: BBox | None,
         size_x: int,
         size_y: int,
-        geometry: Optional[Geometry],
+        geometry: Geometry | None,
     ) -> SentinelHubRequest:
         """Create an instance of SentinelHubRequest"""
         return SentinelHubRequest(
             evalscript=self.evalscript,
             input_data=[
                 SentinelHubRequest.input_data(
                     data_collection=self.data_collection,
@@ -331,15 +330,15 @@
             bbox=bbox,
             geometry=geometry,
             size=(size_x, size_y),
             data_folder=self.cache_folder,
             config=self.config,
         )
 
-    def _extract_data(self, eopatch: EOPatch, responses: List[Any], shape: Tuple[int, ...]) -> EOPatch:
+    def _extract_data(self, eopatch: EOPatch, responses: list[Any], shape: tuple[int, ...]) -> EOPatch:
         """Extract data from the received images and assign them to eopatch features"""
         # pylint: disable=arguments-renamed
         if len(self.features) == 1:
             ftype, fname, _ = self.features[0]
             extension = "json" if ftype.is_meta() else "tif"
             responses = [{f"{fname}.{extension}": data} for data in responses]
 
@@ -359,44 +358,37 @@
         return eopatch
 
 
 class SentinelHubInputTask(SentinelHubInputBaseTask):
     """Process API input task that loads 16bit integer data and converts it to a 32bit float feature."""
 
     # pylint: disable=too-many-arguments
-    DTYPE_TO_SAMPLE_TYPE: Dict[type, str] = {
-        bool: "SampleType.UINT8",
-        np.uint8: "SampleType.UINT8",
-        np.uint16: "SampleType.UINT16",
-        np.float32: "SampleType.FLOAT32",
-    }
-
     # pylint: disable=too-many-locals
     def __init__(
         self,
         data_collection: DataCollection,
-        size: Optional[Tuple[int, int]] = None,
-        resolution: Optional[Union[float, Tuple[float, float]]] = None,
-        bands_feature: Optional[Tuple[FeatureType, str]] = None,
-        bands: Optional[List[str]] = None,
-        additional_data: Optional[List[Tuple[FeatureType, str]]] = None,
-        evalscript: Optional[str] = None,
-        maxcc: Optional[float] = None,
-        time_difference: Optional[dt.timedelta] = None,
-        cache_folder: Optional[str] = None,
-        config: Optional[SHConfig] = None,
-        max_threads: Optional[int] = None,
-        bands_dtype: Union[None, np.dtype, type] = None,
+        size: tuple[int, int] | None = None,
+        resolution: float | tuple[float, float] | None = None,
+        bands_feature: tuple[FeatureType, str] | None = None,
+        bands: list[str] | None = None,
+        additional_data: list[tuple[FeatureType, str]] | None = None,
+        evalscript: str | None = None,
+        maxcc: float | None = None,
+        time_difference: dt.timedelta | None = None,
+        cache_folder: str | None = None,
+        config: SHConfig | None = None,
+        max_threads: int | None = None,
+        bands_dtype: None | np.dtype | type = None,
         single_scene: bool = False,
-        mosaicking_order: Optional[Union[str, MosaickingOrder]] = None,
-        upsampling: Optional[ResamplingType] = None,
-        downsampling: Optional[ResamplingType] = None,
-        aux_request_args: Optional[dict] = None,
-        session_loader: Optional[Callable[[], SentinelHubSession]] = None,
-        timestamp_filter: Callable[[List[dt.datetime], dt.timedelta], List[dt.datetime]] = filter_times,
+        mosaicking_order: str | MosaickingOrder | None = None,
+        upsampling: ResamplingType | None = None,
+        downsampling: ResamplingType | None = None,
+        aux_request_args: dict | None = None,
+        session_loader: Callable[[], SentinelHubSession] | None = None,
+        timestamp_filter: Callable[[list[dt.datetime], dt.timedelta], list[dt.datetime]] = filter_times,
     ):
         """
         :param data_collection: Source of requested satellite data.
         :param size: Number of pixels in x and y dimension.
         :param resolution: Resolution in meters, passed as a single number or a tuple of two numbers -
             resolution in horizontal and resolution in vertical direction.
         :param bands_feature: A target feature into which to save the downloaded images.
@@ -442,139 +434,80 @@
         self.mosaicking_order = None if mosaicking_order is None else MosaickingOrder(mosaicking_order)
         self.aux_request_args = aux_request_args
 
         self.bands_feature = None
         self.requested_bands = []
         if bands_feature:
             self.bands_feature = self.parse_feature(bands_feature, allowed_feature_types=[FeatureType.DATA])
-            if bands is not None:
-                self.requested_bands = self._parse_requested_bands(bands, self.data_collection.bands)
-            else:
-                self.requested_bands = list(self.data_collection.bands)
+            bands = bands if bands is not None else [band.name for band in data_collection.bands]
+            self.requested_bands = parse_data_collection_bands(data_collection, bands)
 
         self.requested_additional_bands = []
-        self.additional_data: Optional[List[FeatureRenameSpec]] = None
+        self.additional_data: list[FeatureRenameSpec] | None = None
         if additional_data is not None:
-            parsed_additional_data = parse_renamed_features(additional_data)  # parser gives too general type
-            additional_bands = cast(List[str], [band for _, band, _ in parsed_additional_data])
-            parsed_bands = self._parse_requested_bands(additional_bands, self.data_collection.metabands)
-            self.requested_additional_bands = parsed_bands
-            self.additional_data = parsed_additional_data
-
-    def _parse_requested_bands(self, bands: List[str], available_bands: Tuple[Band, ...]) -> List[Band]:
-        """Checks that all requested bands are available and returns the band information for further processing"""
-        requested_bands = []
-        band_info_dict = {band_info.name: band_info for band_info in available_bands}
-        for band_name in bands:
-            if band_name in band_info_dict:
-                requested_bands.append(band_info_dict[band_name])
-            else:
-                raise ValueError(
-                    f"Data collection {self.data_collection} does not have specifications for {band_name}."
-                    f"Available bands are {[band.name for band in self.data_collection.bands]} and meta-bands"
-                    f"{[band.name for band in self.data_collection.metabands]}"
-                )
-        return requested_bands
-
-    def generate_evalscript(self) -> str:
-        """Generate the evalscript to be passed with the request, based on chosen bands"""
-        evalscript = """
-            //VERSION=3
-
-            function setup() {{
-                return {{
-                    input: [{{
-                        bands: [{bands}],
-                        units: [{units}]
-                    }}],
-                    output: [
-                        {outputs}
-                    ]
-                }}
-            }}
-
-            function evaluatePixel(sample) {{
-                return {{ {samples} }}
-            }}
-        """
-
-        bands, units, outputs, samples = [], [], [], []
-        for band in self.requested_bands + self.requested_additional_bands:
-            unit_choice = 0  # use default units
-            if band in self.requested_bands and self.bands_dtype is not None:
-                if self.bands_dtype not in band.output_types:
-                    raise ValueError(
-                        f"Band {band.name} only supports output types {band.output_types} but `bands_dtype` is set to "
-                        f"{self.bands_dtype}. To use default types set `bands_dtype` to None."
-                    )
-                unit_choice = band.output_types.index(self.bands_dtype)
-
-            sample_type = SentinelHubInputTask.DTYPE_TO_SAMPLE_TYPE[band.output_types[unit_choice]]
-
-            bands.append(f'"{band.name}"')
-            units.append(f'"{band.units[unit_choice].value}"')
-            samples.append(f"{band.name}: [sample.{band.name}]")
-            outputs.append(f'{{ id: "{band.name}", bands: 1, sampleType: {sample_type} }}')
-
-        evalscript = evalscript.format(
-            bands=", ".join(bands), units=", ".join(units), outputs=", ".join(outputs), samples=", ".join(samples)
-        )
-
-        return evalscript
+            self.additional_data = parse_renamed_features(additional_data)  # parser gives too general type
+            additional_bands = cast(List[str], [band for _, band, _ in self.additional_data])
+            self.requested_additional_bands = parse_data_collection_bands(data_collection, additional_bands)
 
-    def _get_timestamps(self, time_interval: Optional[RawTimeIntervalType], bbox: BBox) -> List[dt.datetime]:
+    def _get_timestamps(self, time_interval: RawTimeIntervalType | None, bbox: BBox) -> list[dt.datetime]:
         """Get the timestamp array needed as a parameter for downloading the images"""
         if self.single_scene:
             return [time_interval[0]]  # type: ignore[index, list-item]
 
-        return get_available_timestamps(
+        timestamps = get_available_timestamps(
             bbox=bbox,
             time_interval=time_interval,
-            timestamp_filter=self.timestamp_filter,
             data_collection=self.data_collection,
             maxcc=self.maxcc,
-            time_difference=self.time_difference,
             config=self.config,
         )
 
+        return self.timestamp_filter(timestamps, self.time_difference)
+
     def _build_requests(
         self,
-        bbox: Optional[BBox],
+        bbox: BBox | None,
         size_x: int,
         size_y: int,
-        timestamps: Optional[List[dt.datetime]],
-        time_interval: Optional[RawTimeIntervalType],
-        geometry: Optional[Geometry],
-    ) -> List[SentinelHubRequest]:
+        timestamps: list[dt.datetime] | None,
+        time_interval: RawTimeIntervalType | None,
+        geometry: Geometry | None,
+    ) -> list[SentinelHubRequest]:
         """Build requests"""
         if timestamps is None:
-            intervals: List[Optional[RawTimeIntervalType]] = [None]
+            intervals: list[RawTimeIntervalType | None] = [None]
         elif self.single_scene:
             intervals = [parse_time_interval(time_interval)]
         else:
             intervals = [(date - self.time_difference, date + self.time_difference) for date in timestamps]
 
         return [self._create_sh_request(time_interval, bbox, size_x, size_y, geometry) for time_interval in intervals]
 
     def _create_sh_request(
         self,
-        time_interval: Optional[RawTimeIntervalType],
-        bbox: Optional[BBox],
+        time_interval: RawTimeIntervalType | None,
+        bbox: BBox | None,
         size_x: int,
         size_y: int,
-        geometry: Optional[Geometry],
+        geometry: Geometry | None,
     ) -> SentinelHubRequest:
         """Create an instance of SentinelHubRequest"""
         responses = [
             SentinelHubRequest.output_response(band.name, MimeType.TIFF)
             for band in self.requested_bands + self.requested_additional_bands
         ]
+        evalscript = generate_evalscript(
+            data_collection=self.data_collection,
+            bands=[band.name for band in self.requested_bands],
+            meta_bands=[band.name for band in self.requested_additional_bands],
+            prioritize_dn=not np.issubdtype(self.bands_dtype, np.floating),
+        )
 
         return SentinelHubRequest(
-            evalscript=self.evalscript or self.generate_evalscript(),
+            evalscript=self.evalscript or evalscript,
             input_data=[
                 SentinelHubRequest.input_data(
                     data_collection=self.data_collection,
                     time_interval=time_interval,
                     mosaicking_order=self.mosaicking_order,
                     maxcc=self.maxcc,
                     upsampling=self.upsampling,
@@ -586,15 +519,15 @@
             bbox=bbox,
             geometry=geometry,
             size=(size_x, size_y),
             data_folder=self.cache_folder,
             config=self.config,
         )
 
-    def _extract_data(self, eopatch: EOPatch, responses: List[Any], shape: Tuple[int, ...]) -> EOPatch:
+    def _extract_data(self, eopatch: EOPatch, responses: list[Any], shape: tuple[int, ...]) -> EOPatch:
         """Extract data from the received images and assign them to eopatch features"""
         if len(self.requested_bands) + len(self.requested_additional_bands) == 1:
             # if only one band is requested the response is not a tar so we reshape it
             only_band = (self.requested_bands + self.requested_additional_bands)[0]
             responses = [{only_band.name + ".tif": image} for image in responses]
 
         if self.additional_data:
@@ -602,88 +535,65 @@
 
         if self.bands_feature:
             self._extract_bands_feature(eopatch, responses, shape)
 
         return eopatch
 
     def _extract_additional_features(
-        self, eopatch: EOPatch, images: Iterable[np.ndarray], shape: Tuple[int, ...]
+        self, eopatch: EOPatch, images: Iterable[np.ndarray], shape: tuple[int, ...]
     ) -> None:
         """Extracts additional features from response into an EOPatch"""
         additional_data = cast(List[FeatureRenameSpec], self.additional_data)  # verified by `if` in _extract_data
         for (ftype, _, new_name), band_info in zip(additional_data, self.requested_additional_bands):
             tiffs = [tar[band_info.name + ".tif"] for tar in images]
             eopatch[ftype, new_name] = self._extract_array(tiffs, 0, shape, band_info.output_types[0])
 
-    def _extract_bands_feature(self, eopatch: EOPatch, images: Iterable[np.ndarray], shape: Tuple[int, ...]) -> None:
+    def _extract_bands_feature(self, eopatch: EOPatch, images: Iterable[np.ndarray], shape: tuple[int, ...]) -> None:
         """Extract the bands feature arrays and concatenate them along the last axis"""
         processed_bands = []
         for band_info in self.requested_bands:
             tiffs = [tar[band_info.name + ".tif"] for tar in images]
             dtype = self.bands_dtype or band_info.output_types[0]
             processed_bands.append(self._extract_array(tiffs, 0, shape, dtype))
 
         bands_feature = cast(Tuple[FeatureType, str], self.bands_feature)  # verified by `if` in _extract_data
         eopatch[bands_feature] = np.concatenate(processed_bands, axis=-1)
 
     @staticmethod
-    def _extract_array(
-        tiffs: List[np.ndarray], idx: int, shape: Tuple[int, ...], dtype: Union[type, np.dtype]
-    ) -> np.ndarray:
+    def _extract_array(tiffs: list[np.ndarray], idx: int, shape: tuple[int, ...], dtype: type | np.dtype) -> np.ndarray:
         """Extract a numpy array from the received tiffs"""
         feature_arrays = (np.atleast_3d(img)[..., idx] for img in tiffs)
         return np.asarray(list(feature_arrays), dtype=dtype).reshape(*shape, 1)
 
 
 class SentinelHubDemTask(SentinelHubEvalscriptTask):
     """
     Adds DEM data (one of the `collections <https://docs.sentinel-hub.com/api/latest/data/dem/#deminstance>`__) to
         DATA_TIMELESS EOPatch feature.
     """
 
     def __init__(
         self,
-        feature: Union[None, str, FeatureSpec] = None,
+        feature: None | str | FeatureSpec = None,
         data_collection: DataCollection = DataCollection.DEM,
         **kwargs: Any,
     ):
+        dem_band = data_collection.bands[0].name
+        renamed_feature: tuple[FeatureType, str, str]
+
         if feature is None:
-            feature = (FeatureType.DATA_TIMELESS, "dem")
+            renamed_feature = (FeatureType.DATA_TIMELESS, dem_band, dem_band)
         elif isinstance(feature, str):
-            feature = (FeatureType.DATA_TIMELESS, feature)
-
-        feature_type, feature_name = feature
-        if feature_type.is_temporal():
-            raise ValueError("DEM feature should be timeless!")
-
-        band = data_collection.bands[0]
-
-        evalscript = f"""
-            //VERSION=3
-
-            function setup() {{
-                return {{
-                    input: [{{
-                        bands: ["{band.name}"],
-                        units: ["{band.units[0].value}"]
-                    }}],
-                    output: {{
-                        id: "{feature_name}",
-                        bands: 1,
-                        sampleType: SampleType.UINT16
-                    }}
-                }}
-            }}
-
-            function evaluatePixel(sample) {{
-                return {{ {feature_name}: [sample.{band.name}] }}
-            }}
-        """
+            renamed_feature = (FeatureType.DATA_TIMELESS, dem_band, feature)
+        else:
+            ftype, _, fname = parse_renamed_feature(feature, allowed_feature_types=lambda ftype: ftype.is_timeless())
+            renamed_feature = (ftype, dem_band, fname or dem_band)
 
-        super().__init__(evalscript=evalscript, features=[feature], data_collection=data_collection, **kwargs)
+        evalscript = generate_evalscript(data_collection=data_collection, bands=[dem_band])
+        super().__init__(evalscript=evalscript, features=[renamed_feature], data_collection=data_collection, **kwargs)
 
 
 class SentinelHubSen2corTask(SentinelHubInputTask):
     """
     Adds SCL (scene classification), CLD (cloud probability) or SNW (snow probability) (or their combination)
     Sen2Cor classification results to EOPatch's MASK or DATA feature. The feature is added to MASK (SCL) or
     DATA (CLD, SNW) feature types of EOPatch. The feature names are set to be SCL, CLD or SNW.
@@ -700,15 +610,15 @@
        * 9 - CLOUD_HIGH_PROBABILITY
        * 10 - THIN_CIRRUS
        * 11 - SNOW
     """
 
     def __init__(
         self,
-        sen2cor_classification: Union[Literal["SCL", "CLD", "SNW"], List[Literal["SCL", "CLD", "SNW"]]],
+        sen2cor_classification: Literal["SCL", "CLD", "SNW"] | list[Literal["SCL", "CLD", "SNW"]],
         data_collection: DataCollection = DataCollection.SENTINEL2_L2A,
         **kwargs: Any,
     ):
         """
         :param sen2cor_classification: "SCL" (scene classification), "CLD" (cloud probability) or "SNW"
             (snow probability) masks to be retrieved. Also, a list of their combination (e.g. ["SCL","CLD"])
         :param kwargs: Additional arguments that will be passed to the `SentinelHubInputTask`
@@ -724,54 +634,9 @@
                 raise ValueError(
                     f"Unsupported Sen2Cor classification type: {s2c}. Possible types are: {classification_types}!"
                 )
 
         if data_collection != DataCollection.SENTINEL2_L2A:
             raise ValueError("Sen2Cor classification layers are only available on Sentinel-2 L2A data.")
 
-        features: List[Tuple[FeatureType, str]] = [(classification_types[s2c], s2c) for s2c in sen2cor_classification]
+        features: list[tuple[FeatureType, str]] = [(classification_types[s2c], s2c) for s2c in sen2cor_classification]
         super().__init__(additional_data=features, data_collection=data_collection, **kwargs)
-
-
-def get_available_timestamps(
-    bbox: BBox,
-    data_collection: DataCollection,
-    *,
-    time_interval: Optional[RawTimeIntervalType] = None,
-    time_difference: dt.timedelta = dt.timedelta(seconds=-1),  # noqa: B008
-    timestamp_filter: Callable[[List[dt.datetime], dt.timedelta], List[dt.datetime]] = filter_times,
-    maxcc: Optional[float] = None,
-    config: Optional[SHConfig] = None,
-) -> List[dt.datetime]:
-    """Helper function to search for all available timestamps, based on query parameters.
-
-    :param bbox: A bounding box of the search area.
-    :param data_collection: A data collection for which to find available timestamps.
-    :param time_interval: A time interval from which to provide the timestamps.
-    :param time_difference: Minimum allowed time difference, used when filtering dates.
-    :param timestamp_filter: A function that performs the final filtering of timestamps, usually to remove multiple
-        occurrences within the time_difference window. The filtration is performed after all suitable timestamps for
-        the given region are obtained (with maxcc filtering already done by SH). By default only keeps the oldest
-        timestamp when multiple occur within `time_difference`.
-    :param maxcc: Maximum cloud coverage filter from interval [0, 1], default is None.
-    :param config: A configuration object.
-    :return: A list of timestamps of available observations.
-    """
-    query_filter = None
-    if maxcc is not None and data_collection.has_cloud_coverage:
-        if isinstance(maxcc, (int, float)) and (maxcc < 0 or maxcc > 1):
-            raise ValueError('Maximum cloud coverage "maxcc" parameter should be a float on an interval [0, 1]')
-        query_filter = f"eo:cloud_cover < {int(maxcc * 100)}"
-
-    fields = {"include": ["properties.datetime"], "exclude": []}
-
-    if data_collection.service_url:
-        config = config.copy() if config else SHConfig()
-        config.sh_base_url = data_collection.service_url
-
-    catalog = SentinelHubCatalog(config=config)
-    search_iterator = catalog.search(
-        collection=data_collection, bbox=bbox, time=time_interval, filter=query_filter, fields=fields
-    )
-
-    all_timestamps = search_iterator.get_timestamps()
-    return timestamp_filter(all_timestamps, time_difference)
```

### Comparing `eo-learn-io-1.4.1/setup.py` & `eo-learn-io-1.4.2/setup.py`

 * *Files 3% similar despite different names*

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
     name="eo-learn-io",
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     version=get_version(),
     description="A collection of input/output EOTasks and utilities",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     url="https://github.com/sentinel-hub/eo-learn",
     project_urls={
         "Documentation": "https://eo-learn.readthedocs.io",
@@ -56,16 +54,16 @@
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

