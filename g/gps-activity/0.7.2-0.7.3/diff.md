# Comparing `tmp/gps_activity-0.7.2.tar.gz` & `tmp/gps_activity-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gps_activity-0.7.2.tar", max compression
+gzip compressed data, was "gps_activity-0.7.3.tar", max compression
```

## Comparing `gps_activity-0.7.2.tar` & `gps_activity-0.7.3.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0     1070 2023-03-05 12:43:52.883092 gps_activity-0.7.2/LICENSE.txt
--rw-r--r--   0        0        0     7442 2023-03-05 12:43:52.883092 gps_activity-0.7.2/README.md
--rw-r--r--   0        0        0      246 2023-03-05 12:43:52.887092 gps_activity-0.7.2/gps_activity/__init__.py
--rw-r--r--   0        0        0     1317 2023-03-05 12:43:52.887092 gps_activity-0.7.2/gps_activity/abstract.py
--rw-r--r--   0        0        0      128 2023-03-05 12:43:52.887092 gps_activity-0.7.2/gps_activity/extraction/__init__.py
--rw-r--r--   0        0        0     3451 2023-03-05 12:43:52.887092 gps_activity-0.7.2/gps_activity/extraction/facade.py
--rw-r--r--   0        0        0      161 2023-03-05 12:43:52.887092 gps_activity-0.7.2/gps_activity/extraction/factory/__init__.py
--rw-r--r--   0        0        0        0 2023-03-05 12:43:52.887092 gps_activity-0.7.2/gps_activity/extraction/factory/classifiers/__init__.py
--rw-r--r--   0        0        0      123 2023-03-05 12:43:52.887092 gps_activity-0.7.2/gps_activity/extraction/factory/clustering/__init__.py
--rw-r--r--   0        0        0     2711 2023-03-05 12:43:52.887092 gps_activity-0.7.2/gps_activity/extraction/factory/clustering/fdbscan.py
--rw-r--r--   0        0        0     1779 2023-03-05 12:43:52.887092 gps_activity-0.7.2/gps_activity/extraction/factory/clustering/stcm.py
--rw-r--r--   0        0        0      103 2023-03-05 12:43:52.887092 gps_activity-0.7.2/gps_activity/extraction/factory/fragmentation/__init__.py
--rw-r--r--   0        0        0      966 2023-03-05 12:43:52.887092 gps_activity-0.7.2/gps_activity/extraction/factory/fragmentation/velocity.py
--rw-r--r--   0        0        0     2950 2023-03-05 12:43:52.887092 gps_activity-0.7.2/gps_activity/extraction/factory/preprocessing.py
--rw-r--r--   0        0        0      179 2023-03-05 12:43:52.887092 gps_activity-0.7.2/gps_activity/extraction/nodes/__init__.py
--rw-r--r--   0        0        0     2736 2023-03-05 12:43:52.887092 gps_activity-0.7.2/gps_activity/extraction/nodes/fdbscan.py
--rw-r--r--   0        0        0     5275 2023-03-05 12:43:52.887092 gps_activity-0.7.2/gps_activity/extraction/nodes/stcm.py
--rw-r--r--   0        0        0      717 2023-03-05 12:43:52.887092 gps_activity-0.7.2/gps_activity/extraction/nodes/velocity_fragmentator.py
--rw-r--r--   0        0        0       89 2023-03-05 12:43:52.887092 gps_activity-0.7.2/gps_activity/linker/__init__.py
--rw-r--r--   0        0        0     4604 2023-03-05 12:43:52.887092 gps_activity-0.7.2/gps_activity/linker/facade.py
--rw-r--r--   0        0        0      428 2023-03-05 12:43:52.887092 gps_activity-0.7.2/gps_activity/linker/factory/__init__.py
--rw-r--r--   0        0        0     2645 2023-03-05 12:43:52.887092 gps_activity-0.7.2/gps_activity/linker/factory/cluster_aggregator.py
--rw-r--r--   0        0        0      797 2023-03-05 12:43:52.887092 gps_activity-0.7.2/gps_activity/linker/factory/coverage_statistics.py
--rw-r--r--   0        0        0     2506 2023-03-05 12:43:52.887092 gps_activity-0.7.2/gps_activity/linker/factory/join_validator.py
--rw-r--r--   0        0        0     3941 2023-03-05 12:43:52.887092 gps_activity-0.7.2/gps_activity/linker/factory/preprocessing.py
--rw-r--r--   0        0        0     1025 2023-03-05 12:43:52.887092 gps_activity-0.7.2/gps_activity/linker/factory/spatial_joiner.py
--rw-r--r--   0        0        0      687 2023-03-05 12:43:52.887092 gps_activity-0.7.2/gps_activity/linker/models.py
--rw-r--r--   0        0        0      317 2023-03-05 12:43:52.887092 gps_activity-0.7.2/gps_activity/linker/nodes/__init__.py
--rw-r--r--   0        0        0     1718 2023-03-05 12:43:52.887092 gps_activity-0.7.2/gps_activity/linker/nodes/cluster_aggregator.py
--rw-r--r--   0        0        0     2637 2023-03-05 12:43:52.887092 gps_activity-0.7.2/gps_activity/linker/nodes/coverage_statistics.py
--rw-r--r--   0        0        0     5207 2023-03-05 12:43:52.887092 gps_activity-0.7.2/gps_activity/linker/nodes/spatial_join_validator.py
--rw-r--r--   0        0        0     1123 2023-03-05 12:43:52.887092 gps_activity-0.7.2/gps_activity/linker/nodes/spatial_joiner.py
--rw-r--r--   0        0        0       89 2023-03-05 12:43:52.887092 gps_activity-0.7.2/gps_activity/metrics/__init__.py
--rw-r--r--   0        0        0     1817 2023-03-05 12:43:52.887092 gps_activity-0.7.2/gps_activity/metrics/facade.py
--rw-r--r--   0        0        0      532 2023-03-05 12:43:52.887092 gps_activity-0.7.2/gps_activity/metrics/models.py
--rw-r--r--   0        0        0      145 2023-03-05 12:43:52.887092 gps_activity-0.7.2/gps_activity/metrics/nodes/__init__.py
--rw-r--r--   0        0        0     1031 2023-03-05 12:43:52.887092 gps_activity-0.7.2/gps_activity/metrics/nodes/fbeta.py
--rw-r--r--   0        0        0      533 2023-03-05 12:43:52.887092 gps_activity-0.7.2/gps_activity/metrics/nodes/precision.py
--rw-r--r--   0        0        0      517 2023-03-05 12:43:52.887092 gps_activity-0.7.2/gps_activity/metrics/nodes/recall.py
--rw-r--r--   0        0        0     7423 2023-03-05 12:43:52.887092 gps_activity-0.7.2/gps_activity/models.py
--rw-r--r--   0        0        0      891 2023-03-05 12:43:52.887092 gps_activity-0.7.2/gps_activity/nodes/__init__.py
--rw-r--r--   0        0        0     2791 2023-03-05 12:43:52.887092 gps_activity-0.7.2/gps_activity/nodes/coordinates_velocity_calculator.py
--rw-r--r--   0        0        0     1300 2023-03-05 12:43:52.887092 gps_activity-0.7.2/gps_activity/nodes/crs_projection.py
--rw-r--r--   0        0        0      716 2023-03-05 12:43:52.887092 gps_activity-0.7.2/gps_activity/nodes/date_extractor.py
--rw-r--r--   0        0        0     1224 2023-03-05 12:43:52.887092 gps_activity-0.7.2/gps_activity/nodes/df_to_gdf.py
--rw-r--r--   0        0        0      407 2023-03-05 12:43:52.887092 gps_activity-0.7.2/gps_activity/nodes/formatting.py
--rw-r--r--   0        0        0      506 2023-03-05 12:43:52.887092 gps_activity-0.7.2/gps_activity/nodes/order_gps.py
--rw-r--r--   0        0        0     1373 2023-03-05 12:43:52.887092 gps_activity-0.7.2/gps_activity/nodes/primary_key_generator.py
--rw-r--r--   0        0        0     1866 2023-03-05 12:43:52.887092 gps_activity-0.7.2/gps_activity/nodes/project_default_fields.py
--rw-r--r--   0        0        0      489 2023-03-05 12:43:52.887092 gps_activity-0.7.2/gps_activity/nodes/schema_validator.py
--rw-r--r--   0        0        0      659 2023-03-05 12:43:52.887092 gps_activity-0.7.2/gps_activity/nodes/timing.py
--rw-r--r--   0        0        0     1202 2023-03-05 12:43:52.887092 gps_activity-0.7.2/gps_activity/nodes/unique_gps_constraint.py
--rw-r--r--   0        0        0     1066 2023-03-05 12:43:52.891092 gps_activity-0.7.2/gps_activity/nodes/unique_vehicle_constrains.py
--rw-r--r--   0        0        0     1639 2023-03-05 12:43:52.891092 gps_activity-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     8757 1970-01-01 00:00:00.000000 gps_activity-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-24 12:29:13.310918 gps_activity-0.7.3/LICENSE.txt
+-rw-r--r--   0        0        0     7442 2023-05-24 12:29:13.310918 gps_activity-0.7.3/README.md
+-rw-r--r--   0        0        0      246 2023-05-24 12:29:13.314920 gps_activity-0.7.3/gps_activity/__init__.py
+-rw-r--r--   0        0        0     1317 2023-05-24 12:29:13.314920 gps_activity-0.7.3/gps_activity/abstract.py
+-rw-r--r--   0        0        0      128 2023-05-24 12:29:13.314920 gps_activity-0.7.3/gps_activity/extraction/__init__.py
+-rw-r--r--   0        0        0     3451 2023-05-24 12:29:13.314920 gps_activity-0.7.3/gps_activity/extraction/facade.py
+-rw-r--r--   0        0        0      161 2023-05-24 12:29:13.314920 gps_activity-0.7.3/gps_activity/extraction/factory/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:29:13.314920 gps_activity-0.7.3/gps_activity/extraction/factory/classifiers/__init__.py
+-rw-r--r--   0        0        0      123 2023-05-24 12:29:13.314920 gps_activity-0.7.3/gps_activity/extraction/factory/clustering/__init__.py
+-rw-r--r--   0        0        0     2711 2023-05-24 12:29:13.314920 gps_activity-0.7.3/gps_activity/extraction/factory/clustering/fdbscan.py
+-rw-r--r--   0        0        0     1779 2023-05-24 12:29:13.314920 gps_activity-0.7.3/gps_activity/extraction/factory/clustering/stcm.py
+-rw-r--r--   0        0        0      103 2023-05-24 12:29:13.314920 gps_activity-0.7.3/gps_activity/extraction/factory/fragmentation/__init__.py
+-rw-r--r--   0        0        0      966 2023-05-24 12:29:13.314920 gps_activity-0.7.3/gps_activity/extraction/factory/fragmentation/velocity.py
+-rw-r--r--   0        0        0     2950 2023-05-24 12:29:13.318921 gps_activity-0.7.3/gps_activity/extraction/factory/preprocessing.py
+-rw-r--r--   0        0        0      179 2023-05-24 12:29:13.318921 gps_activity-0.7.3/gps_activity/extraction/nodes/__init__.py
+-rw-r--r--   0        0        0     2736 2023-05-24 12:29:13.318921 gps_activity-0.7.3/gps_activity/extraction/nodes/fdbscan.py
+-rw-r--r--   0        0        0     5275 2023-05-24 12:29:13.318921 gps_activity-0.7.3/gps_activity/extraction/nodes/stcm.py
+-rw-r--r--   0        0        0      717 2023-05-24 12:29:13.318921 gps_activity-0.7.3/gps_activity/extraction/nodes/velocity_fragmentator.py
+-rw-r--r--   0        0        0       89 2023-05-24 12:29:13.318921 gps_activity-0.7.3/gps_activity/linker/__init__.py
+-rw-r--r--   0        0        0     4604 2023-05-24 12:29:13.318921 gps_activity-0.7.3/gps_activity/linker/facade.py
+-rw-r--r--   0        0        0      428 2023-05-24 12:29:13.318921 gps_activity-0.7.3/gps_activity/linker/factory/__init__.py
+-rw-r--r--   0        0        0     2645 2023-05-24 12:29:13.318921 gps_activity-0.7.3/gps_activity/linker/factory/cluster_aggregator.py
+-rw-r--r--   0        0        0      797 2023-05-24 12:29:13.318921 gps_activity-0.7.3/gps_activity/linker/factory/coverage_statistics.py
+-rw-r--r--   0        0        0     2506 2023-05-24 12:29:13.318921 gps_activity-0.7.3/gps_activity/linker/factory/join_validator.py
+-rw-r--r--   0        0        0     3941 2023-05-24 12:29:13.318921 gps_activity-0.7.3/gps_activity/linker/factory/preprocessing.py
+-rw-r--r--   0        0        0     1025 2023-05-24 12:29:13.318921 gps_activity-0.7.3/gps_activity/linker/factory/spatial_joiner.py
+-rw-r--r--   0        0        0      687 2023-05-24 12:29:13.318921 gps_activity-0.7.3/gps_activity/linker/models.py
+-rw-r--r--   0        0        0      317 2023-05-24 12:29:13.318921 gps_activity-0.7.3/gps_activity/linker/nodes/__init__.py
+-rw-r--r--   0        0        0     1718 2023-05-24 12:29:13.318921 gps_activity-0.7.3/gps_activity/linker/nodes/cluster_aggregator.py
+-rw-r--r--   0        0        0     2637 2023-05-24 12:29:13.318921 gps_activity-0.7.3/gps_activity/linker/nodes/coverage_statistics.py
+-rw-r--r--   0        0        0     5207 2023-05-24 12:29:13.318921 gps_activity-0.7.3/gps_activity/linker/nodes/spatial_join_validator.py
+-rw-r--r--   0        0        0     1123 2023-05-24 12:29:13.318921 gps_activity-0.7.3/gps_activity/linker/nodes/spatial_joiner.py
+-rw-r--r--   0        0        0       89 2023-05-24 12:29:13.318921 gps_activity-0.7.3/gps_activity/metrics/__init__.py
+-rw-r--r--   0        0        0     1817 2023-05-24 12:29:13.318921 gps_activity-0.7.3/gps_activity/metrics/facade.py
+-rw-r--r--   0        0        0      532 2023-05-24 12:29:13.318921 gps_activity-0.7.3/gps_activity/metrics/models.py
+-rw-r--r--   0        0        0      145 2023-05-24 12:29:13.318921 gps_activity-0.7.3/gps_activity/metrics/nodes/__init__.py
+-rw-r--r--   0        0        0     1031 2023-05-24 12:29:13.318921 gps_activity-0.7.3/gps_activity/metrics/nodes/fbeta.py
+-rw-r--r--   0        0        0      533 2023-05-24 12:29:13.318921 gps_activity-0.7.3/gps_activity/metrics/nodes/precision.py
+-rw-r--r--   0        0        0      517 2023-05-24 12:29:13.318921 gps_activity-0.7.3/gps_activity/metrics/nodes/recall.py
+-rw-r--r--   0        0        0     7423 2023-05-24 12:29:13.318921 gps_activity-0.7.3/gps_activity/models.py
+-rw-r--r--   0        0        0      891 2023-05-24 12:29:13.318921 gps_activity-0.7.3/gps_activity/nodes/__init__.py
+-rw-r--r--   0        0        0     2791 2023-05-24 12:29:13.318921 gps_activity-0.7.3/gps_activity/nodes/coordinates_velocity_calculator.py
+-rw-r--r--   0        0        0     1300 2023-05-24 12:29:13.318921 gps_activity-0.7.3/gps_activity/nodes/crs_projection.py
+-rw-r--r--   0        0        0      716 2023-05-24 12:29:13.318921 gps_activity-0.7.3/gps_activity/nodes/date_extractor.py
+-rw-r--r--   0        0        0     1224 2023-05-24 12:29:13.318921 gps_activity-0.7.3/gps_activity/nodes/df_to_gdf.py
+-rw-r--r--   0        0        0      407 2023-05-24 12:29:13.318921 gps_activity-0.7.3/gps_activity/nodes/formatting.py
+-rw-r--r--   0        0        0      506 2023-05-24 12:29:13.318921 gps_activity-0.7.3/gps_activity/nodes/order_gps.py
+-rw-r--r--   0        0        0     1373 2023-05-24 12:29:13.318921 gps_activity-0.7.3/gps_activity/nodes/primary_key_generator.py
+-rw-r--r--   0        0        0     1866 2023-05-24 12:29:13.318921 gps_activity-0.7.3/gps_activity/nodes/project_default_fields.py
+-rw-r--r--   0        0        0      489 2023-05-24 12:29:13.318921 gps_activity-0.7.3/gps_activity/nodes/schema_validator.py
+-rw-r--r--   0        0        0      659 2023-05-24 12:29:13.318921 gps_activity-0.7.3/gps_activity/nodes/timing.py
+-rw-r--r--   0        0        0     1202 2023-05-24 12:29:13.318921 gps_activity-0.7.3/gps_activity/nodes/unique_gps_constraint.py
+-rw-r--r--   0        0        0     1066 2023-05-24 12:29:13.318921 gps_activity-0.7.3/gps_activity/nodes/unique_vehicle_constrains.py
+-rw-r--r--   0        0        0     1589 2023-05-24 12:29:13.318921 gps_activity-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0     8483 1970-01-01 00:00:00.000000 gps_activity-0.7.3/PKG-INFO
```

### Comparing `gps_activity-0.7.2/LICENSE.txt` & `gps_activity-0.7.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gps_activity-0.7.2/README.md` & `gps_activity-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `gps_activity-0.7.2/gps_activity/abstract.py` & `gps_activity-0.7.3/gps_activity/abstract.py`

 * *Files identical despite different names*

### Comparing `gps_activity-0.7.2/gps_activity/extraction/facade.py` & `gps_activity-0.7.3/gps_activity/extraction/facade.py`

 * *Files identical despite different names*

### Comparing `gps_activity-0.7.2/gps_activity/extraction/factory/clustering/fdbscan.py` & `gps_activity-0.7.3/gps_activity/extraction/factory/clustering/fdbscan.py`

 * *Files identical despite different names*

### Comparing `gps_activity-0.7.2/gps_activity/extraction/factory/clustering/stcm.py` & `gps_activity-0.7.3/gps_activity/extraction/factory/clustering/stcm.py`

 * *Files identical despite different names*

### Comparing `gps_activity-0.7.2/gps_activity/extraction/factory/fragmentation/velocity.py` & `gps_activity-0.7.3/gps_activity/extraction/factory/fragmentation/velocity.py`

 * *Files identical despite different names*

### Comparing `gps_activity-0.7.2/gps_activity/extraction/factory/preprocessing.py` & `gps_activity-0.7.3/gps_activity/extraction/factory/preprocessing.py`

 * *Files identical despite different names*

### Comparing `gps_activity-0.7.2/gps_activity/extraction/nodes/fdbscan.py` & `gps_activity-0.7.3/gps_activity/extraction/nodes/fdbscan.py`

 * *Files identical despite different names*

### Comparing `gps_activity-0.7.2/gps_activity/extraction/nodes/stcm.py` & `gps_activity-0.7.3/gps_activity/extraction/nodes/stcm.py`

 * *Files identical despite different names*

### Comparing `gps_activity-0.7.2/gps_activity/extraction/nodes/velocity_fragmentator.py` & `gps_activity-0.7.3/gps_activity/extraction/nodes/velocity_fragmentator.py`

 * *Files identical despite different names*

### Comparing `gps_activity-0.7.2/gps_activity/linker/facade.py` & `gps_activity-0.7.3/gps_activity/linker/facade.py`

 * *Files identical despite different names*

### Comparing `gps_activity-0.7.2/gps_activity/linker/factory/cluster_aggregator.py` & `gps_activity-0.7.3/gps_activity/linker/factory/cluster_aggregator.py`

 * *Files identical despite different names*

### Comparing `gps_activity-0.7.2/gps_activity/linker/factory/coverage_statistics.py` & `gps_activity-0.7.3/gps_activity/linker/factory/coverage_statistics.py`

 * *Files identical despite different names*

### Comparing `gps_activity-0.7.2/gps_activity/linker/factory/join_validator.py` & `gps_activity-0.7.3/gps_activity/linker/factory/join_validator.py`

 * *Files identical despite different names*

### Comparing `gps_activity-0.7.2/gps_activity/linker/factory/preprocessing.py` & `gps_activity-0.7.3/gps_activity/linker/factory/preprocessing.py`

 * *Files identical despite different names*

### Comparing `gps_activity-0.7.2/gps_activity/linker/factory/spatial_joiner.py` & `gps_activity-0.7.3/gps_activity/linker/factory/spatial_joiner.py`

 * *Files identical despite different names*

### Comparing `gps_activity-0.7.2/gps_activity/linker/models.py` & `gps_activity-0.7.3/gps_activity/linker/models.py`

 * *Files identical despite different names*

### Comparing `gps_activity-0.7.2/gps_activity/linker/nodes/cluster_aggregator.py` & `gps_activity-0.7.3/gps_activity/linker/nodes/cluster_aggregator.py`

 * *Files identical despite different names*

### Comparing `gps_activity-0.7.2/gps_activity/linker/nodes/coverage_statistics.py` & `gps_activity-0.7.3/gps_activity/linker/nodes/coverage_statistics.py`

 * *Files identical despite different names*

### Comparing `gps_activity-0.7.2/gps_activity/linker/nodes/spatial_join_validator.py` & `gps_activity-0.7.3/gps_activity/linker/nodes/spatial_join_validator.py`

 * *Files identical despite different names*

### Comparing `gps_activity-0.7.2/gps_activity/linker/nodes/spatial_joiner.py` & `gps_activity-0.7.3/gps_activity/linker/nodes/spatial_joiner.py`

 * *Files identical despite different names*

### Comparing `gps_activity-0.7.2/gps_activity/metrics/facade.py` & `gps_activity-0.7.3/gps_activity/metrics/facade.py`

 * *Files identical despite different names*

### Comparing `gps_activity-0.7.2/gps_activity/metrics/models.py` & `gps_activity-0.7.3/gps_activity/metrics/models.py`

 * *Files identical despite different names*

### Comparing `gps_activity-0.7.2/gps_activity/metrics/nodes/fbeta.py` & `gps_activity-0.7.3/gps_activity/metrics/nodes/fbeta.py`

 * *Files identical despite different names*

### Comparing `gps_activity-0.7.2/gps_activity/metrics/nodes/precision.py` & `gps_activity-0.7.3/gps_activity/metrics/nodes/precision.py`

 * *Files identical despite different names*

### Comparing `gps_activity-0.7.2/gps_activity/metrics/nodes/recall.py` & `gps_activity-0.7.3/gps_activity/metrics/nodes/recall.py`

 * *Files identical despite different names*

### Comparing `gps_activity-0.7.2/gps_activity/models.py` & `gps_activity-0.7.3/gps_activity/models.py`

 * *Files identical despite different names*

### Comparing `gps_activity-0.7.2/gps_activity/nodes/__init__.py` & `gps_activity-0.7.3/gps_activity/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `gps_activity-0.7.2/gps_activity/nodes/coordinates_velocity_calculator.py` & `gps_activity-0.7.3/gps_activity/nodes/coordinates_velocity_calculator.py`

 * *Files identical despite different names*

### Comparing `gps_activity-0.7.2/gps_activity/nodes/crs_projection.py` & `gps_activity-0.7.3/gps_activity/nodes/crs_projection.py`

 * *Files identical despite different names*

### Comparing `gps_activity-0.7.2/gps_activity/nodes/date_extractor.py` & `gps_activity-0.7.3/gps_activity/nodes/date_extractor.py`

 * *Files identical despite different names*

### Comparing `gps_activity-0.7.2/gps_activity/nodes/df_to_gdf.py` & `gps_activity-0.7.3/gps_activity/nodes/df_to_gdf.py`

 * *Files identical despite different names*

### Comparing `gps_activity-0.7.2/gps_activity/nodes/primary_key_generator.py` & `gps_activity-0.7.3/gps_activity/nodes/primary_key_generator.py`

 * *Files identical despite different names*

### Comparing `gps_activity-0.7.2/gps_activity/nodes/project_default_fields.py` & `gps_activity-0.7.3/gps_activity/nodes/project_default_fields.py`

 * *Files identical despite different names*

### Comparing `gps_activity-0.7.2/gps_activity/nodes/timing.py` & `gps_activity-0.7.3/gps_activity/nodes/timing.py`

 * *Files identical despite different names*

### Comparing `gps_activity-0.7.2/gps_activity/nodes/unique_gps_constraint.py` & `gps_activity-0.7.3/gps_activity/nodes/unique_gps_constraint.py`

 * *Files identical despite different names*

### Comparing `gps_activity-0.7.2/gps_activity/nodes/unique_vehicle_constrains.py` & `gps_activity-0.7.3/gps_activity/nodes/unique_vehicle_constrains.py`

 * *Files identical despite different names*

### Comparing `gps_activity-0.7.2/pyproject.toml` & `gps_activity-0.7.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gps_activity"
-version = "0.7.2"
+version = "0.7.3"
 packages = [ { include = "gps_activity"}]
 description = "A light-weight mobile module for analysis of GPS activity"
 authors = [
     "Adil Rashitov <adil@wastelab.com>",
     "Elias Willemse <elias@wastelabs.co>"
 ]
 license = "LICENSE.txt"
@@ -16,44 +16,40 @@
                  'Topic :: Scientific/Engineering',
                  "Operating System :: OS Independent",
                  'Programming Language :: Python :: 3.8',
                  'Programming Language :: Python :: 3.9',
                  'Programming Language :: Python :: 3.10',
                  ]
 
+
 [tool.poetry.dependencies]
-python = ">=3.8, <3.12"
-pandas = "^1.4.3"
-geopandas = "^0.11.1"
-scikit-learn = "^1.1.1"
-pandera = "^0.11.0"
-numpy = "^1.23.1"
-Rtree = "^1.0.0"
-scipy = "^1.9.0"
-pygeos = "^0.12.0"
+# By 2023.05.24 pandera@0.15.1 is limited to >=3.8.1,<3.12
+python = ">=3.8.1,<3.12"
+pandas = "^2.0.1"
+geopandas = "0.12.2"
+scikit-learn = "^1.2.2"
+pandera = "^0.15.1"
+numpy = "^1.24.3"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.1.2"
-pytest-cov = "^3.0.0"
-pytest-parallel = "^0.1.1"
-pre-commit = "^2.20.0"
-cognitive-complexity = "^1.2.0"
-coverage = "^6.4.2"
-flake8 = "^5.0.3"
-flake8-bugbear = "^22.7.1"
-flake8-builtins = "^1.5.3"
+flake8 = "^6.0.0"
+flake8-bugbear = "^23.5.9"
+flake8-builtins = "^2.1.0"
 flake8-cognitive-complexity = "^0.1.0"
 flake8-commas = "^2.1.0"
-flake8-functions = "^0.0.7"
-flake8-import-order = "^0.18.1"
+flake8-functions = "^0.0.8"
+flake8-import-order = "^0.18.2"
 flake8-polyfill = "^1.0.2"
-twine = "^4.0.1"
-build = "^0.8.0"
-commitizen = "^2.29.2"
-
-
-[tool.poetry.group.dev.dependencies]
-pylint = "^2.15.10"
+pytest = "^7.3.1"
+pytest-cov = "^4.0.0"
+pytest-parallel = "^0.1.1"
+pre-commit = "^3.3.2"
+cognitive-complexity = "^1.3.0"
+coverage = "^7.2.6"
+twine = "^4.0.2"
+build = "^0.10.0"
+commitizen = "^3.2.2"
+pylint = "^2.17.4"
 
 [build-system]
-requires = ["poetry-core>=1.0.0", "wheel"]
+requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `gps_activity-0.7.2/PKG-INFO` & `gps_activity-0.7.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,32 @@
 Metadata-Version: 2.1
 Name: gps-activity
-Version: 0.7.2
+Version: 0.7.3
 Summary: A light-weight mobile module for analysis of GPS activity
 License: LICENSE.txt
 Author: Adil Rashitov
 Author-email: adil@wastelab.com
-Requires-Python: >=3.8,<3.12
+Requires-Python: >=3.8.1,<3.12
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
-Requires-Dist: Rtree (>=1.0.0,<2.0.0)
-Requires-Dist: geopandas (>=0.11.1,<0.12.0)
-Requires-Dist: numpy (>=1.23.1,<2.0.0)
-Requires-Dist: pandas (>=1.4.3,<2.0.0)
-Requires-Dist: pandera (>=0.11.0,<0.12.0)
-Requires-Dist: pygeos (>=0.12.0,<0.13.0)
-Requires-Dist: scikit-learn (>=1.1.1,<2.0.0)
-Requires-Dist: scipy (>=1.9.0,<2.0.0)
+Requires-Dist: geopandas (==0.12.2)
+Requires-Dist: numpy (>=1.24.3,<2.0.0)
+Requires-Dist: pandas (>=2.0.1,<3.0.0)
+Requires-Dist: pandera (>=0.15.1,<0.16.0)
+Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
 Description-Content-Type: text/markdown
 
 # **GPS activity** 🚛
 
 ![Python versions](https://img.shields.io/pypi/pyversions/gps_activity)
 ![Latest release](https://img.shields.io/github/v/release/WasteLabs/gps_activity)
 ![Latest release date](https://img.shields.io/github/release-date/WasteLabs/gps_activity)
```

