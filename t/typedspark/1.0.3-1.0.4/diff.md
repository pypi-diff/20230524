# Comparing `tmp/typedspark-1.0.3.tar.gz` & `tmp/typedspark-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typedspark-1.0.3.tar", last modified: Sat Apr 29 18:03:11 2023, max compression
+gzip compressed data, was "typedspark-1.0.4.tar", last modified: Wed May 24 19:58:59 2023, max compression
```

## Comparing `typedspark-1.0.3.tar` & `typedspark-1.0.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:03:11.155666 typedspark-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-29 18:02:57.000000 typedspark-1.0.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-29 18:03:11.155666 typedspark-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-29 18:02:57.000000 typedspark-1.0.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-29 18:02:57.000000 typedspark-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 18:03:11.155666 typedspark-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-29 18:02:57.000000 typedspark-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:03:11.155666 typedspark-1.0.3/typedspark/
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-29 18:02:57.000000 typedspark-1.0.3/typedspark/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:03:11.155666 typedspark-1.0.3/typedspark/_core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 18:02:57.000000 typedspark-1.0.3/typedspark/_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-04-29 18:02:57.000000 typedspark-1.0.3/typedspark/_core/column.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-29 18:02:57.000000 typedspark-1.0.3/typedspark/_core/column_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-04-29 18:02:57.000000 typedspark-1.0.3/typedspark/_core/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-04-29 18:02:57.000000 typedspark-1.0.3/typedspark/_core/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-04-29 18:02:57.000000 typedspark-1.0.3/typedspark/_core/validate_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:03:11.155666 typedspark-1.0.3/typedspark/_schema/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 18:02:57.000000 typedspark-1.0.3/typedspark/_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-29 18:02:57.000000 typedspark-1.0.3/typedspark/_schema/dlt_kwargs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-29 18:02:57.000000 typedspark-1.0.3/typedspark/_schema/get_schema_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-04-29 18:02:57.000000 typedspark-1.0.3/typedspark/_schema/get_schema_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-04-29 18:02:57.000000 typedspark-1.0.3/typedspark/_schema/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-04-29 18:02:57.000000 typedspark-1.0.3/typedspark/_schema/structfield.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:03:11.155666 typedspark-1.0.3/typedspark/_transforms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 18:02:57.000000 typedspark-1.0.3/typedspark/_transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-04-29 18:02:57.000000 typedspark-1.0.3/typedspark/_transforms/structtype_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-04-29 18:02:57.000000 typedspark-1.0.3/typedspark/_transforms/transform_to_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-04-29 18:02:57.000000 typedspark-1.0.3/typedspark/_transforms/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:03:11.155666 typedspark-1.0.3/typedspark/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 18:02:57.000000 typedspark-1.0.3/typedspark/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-04-29 18:02:57.000000 typedspark-1.0.3/typedspark/_utils/create_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-04-29 18:02:57.000000 typedspark-1.0.3/typedspark/_utils/load_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-04-29 18:02:57.000000 typedspark-1.0.3/typedspark/_utils/register_schema_to_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 18:02:57.000000 typedspark-1.0.3/typedspark/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:03:11.155666 typedspark-1.0.3/typedspark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-29 18:03:11.000000 typedspark-1.0.3/typedspark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-29 18:03:11.000000 typedspark-1.0.3/typedspark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 18:03:11.000000 typedspark-1.0.3/typedspark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-29 18:03:11.000000 typedspark-1.0.3/typedspark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-29 18:03:11.000000 typedspark-1.0.3/typedspark.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:58:59.619227 typedspark-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-24 19:58:48.000000 typedspark-1.0.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-24 19:58:59.619227 typedspark-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-05-24 19:58:48.000000 typedspark-1.0.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-24 19:58:48.000000 typedspark-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 19:58:59.619227 typedspark-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-24 19:58:48.000000 typedspark-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:58:59.615227 typedspark-1.0.4/typedspark/
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-24 19:58:48.000000 typedspark-1.0.4/typedspark/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:58:59.615227 typedspark-1.0.4/typedspark/_core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 19:58:48.000000 typedspark-1.0.4/typedspark/_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-24 19:58:48.000000 typedspark-1.0.4/typedspark/_core/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-24 19:58:48.000000 typedspark-1.0.4/typedspark/_core/column_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-05-24 19:58:48.000000 typedspark-1.0.4/typedspark/_core/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-05-24 19:58:48.000000 typedspark-1.0.4/typedspark/_core/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-05-24 19:58:48.000000 typedspark-1.0.4/typedspark/_core/validate_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:58:59.619227 typedspark-1.0.4/typedspark/_schema/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 19:58:48.000000 typedspark-1.0.4/typedspark/_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-24 19:58:48.000000 typedspark-1.0.4/typedspark/_schema/dlt_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-24 19:58:48.000000 typedspark-1.0.4/typedspark/_schema/get_schema_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-05-24 19:58:48.000000 typedspark-1.0.4/typedspark/_schema/get_schema_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-05-24 19:58:48.000000 typedspark-1.0.4/typedspark/_schema/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-05-24 19:58:48.000000 typedspark-1.0.4/typedspark/_schema/structfield.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:58:59.619227 typedspark-1.0.4/typedspark/_transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 19:58:48.000000 typedspark-1.0.4/typedspark/_transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-24 19:58:48.000000 typedspark-1.0.4/typedspark/_transforms/structtype_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-24 19:58:48.000000 typedspark-1.0.4/typedspark/_transforms/transform_to_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-24 19:58:48.000000 typedspark-1.0.4/typedspark/_transforms/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:58:59.619227 typedspark-1.0.4/typedspark/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 19:58:48.000000 typedspark-1.0.4/typedspark/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-05-24 19:58:48.000000 typedspark-1.0.4/typedspark/_utils/create_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-05-24 19:58:48.000000 typedspark-1.0.4/typedspark/_utils/load_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-24 19:58:48.000000 typedspark-1.0.4/typedspark/_utils/register_schema_to_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 19:58:48.000000 typedspark-1.0.4/typedspark/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:58:59.615227 typedspark-1.0.4/typedspark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-24 19:58:59.000000 typedspark-1.0.4/typedspark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-24 19:58:59.000000 typedspark-1.0.4/typedspark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 19:58:59.000000 typedspark-1.0.4/typedspark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-24 19:58:59.000000 typedspark-1.0.4/typedspark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-24 19:58:59.000000 typedspark-1.0.4/typedspark.egg-info/top_level.txt
```

### Comparing `typedspark-1.0.3/LICENSE.txt` & `typedspark-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.3/PKG-INFO` & `typedspark-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typedspark
-Version: 1.0.3
+Version: 1.0.4
 Summary: Column-wise type annotations for pyspark DataFrames
 Home-page: https://github.com/kaiko-ai/typedspark
 Author: Nanne Aben
 Author-email: nanne@kaiko.ai
 License: Apache-2.0
 Keywords: pyspark spark typing type checking annotations
 Classifier: Programming Language :: Python
```

### Comparing `typedspark-1.0.3/README.rst` & `typedspark-1.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.3/pyproject.toml` & `typedspark-1.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.3/setup.py` & `typedspark-1.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.3/typedspark/__init__.py` & `typedspark-1.0.4/typedspark/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""typedspark: column-wise type annotations for pyspark DataFrames"""
+"""Typedspark: column-wise type annotations for pyspark DataFrames."""
 
 from typedspark._core.column import Column
 from typedspark._core.column_meta import ColumnMeta
 from typedspark._core.dataset import DataSet
 from typedspark._core.datatypes import ArrayType, DecimalType, MapType, StructType
 from typedspark._schema.schema import MetaSchema, Schema
 from typedspark._transforms.structtype_column import structtype_column
```

### Comparing `typedspark-1.0.3/typedspark/_core/column.py` & `typedspark-1.0.4/typedspark/_core/column.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 from pyspark.sql.functions import col
 from pyspark.sql.types import DataType
 
 T = TypeVar("T", bound=DataType)
 
 
 class EmptyColumn(SparkColumn):
-    """Column object to be instantiated when there is no active Spark
-    session."""
+    """Column object to be instantiated when there is no active Spark session."""
 
     def __init__(self, *args, **kwargs) -> None:  # pragma: no cover
         pass
 
 
 class Column(SparkColumn, Generic[T]):
     """Represents a ``Column`` in a ``Schema``. Can be used as:
```

### Comparing `typedspark-1.0.3/typedspark/_core/column_meta.py` & `typedspark-1.0.4/typedspark/_core/column_meta.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.3/typedspark/_core/dataset.py` & `typedspark-1.0.4/typedspark/_core/dataset.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.3/typedspark/_core/datatypes.py` & `typedspark-1.0.4/typedspark/_core/datatypes.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.3/typedspark/_core/validate_schema.py` & `typedspark-1.0.4/typedspark/_core/validate_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""Module containing functions that are related to validating schema's at
-runtime."""
+"""Module containing functions that are related to validating schema's at runtime."""
 from typing import Dict, Set
 
 from pyspark.sql.types import ArrayType, DataType, MapType, StructField, StructType
 
 
 def validate_schema(
     structtype_expected: StructType, structtype_observed: StructType, schema_name: str
@@ -13,16 +12,15 @@
     observed = unpack_schema(structtype_observed)
 
     check_names(set(expected.keys()), set(observed.keys()), schema_name)
     check_dtypes(expected, observed, schema_name)
 
 
 def unpack_schema(schema: StructType) -> Dict[str, StructField]:
-    """Converts the observed schema to a dictionary mapping column name to
-    StructField.
+    """Converts the observed schema to a dictionary mapping column name to StructField.
 
     We ignore columns that start with ``__``.
     """
     res = {}
     for field in schema.fields:
         if field.name.startswith("__"):
             continue
@@ -52,16 +50,15 @@
 
 
 def check_dtypes(
     schema_expected: Dict[str, StructField],
     schema_observed: Dict[str, StructField],
     schema_name: str,
 ) -> None:
-    """Checks for each column whether the observed and expected data type
-    match.
+    """Checks for each column whether the observed and expected data type match.
 
     Is order insensitive.
     """
     for name, structfield_expected in schema_expected.items():
         structfield_observed = schema_observed[name]
         check_dtype(
             name,
```

### Comparing `typedspark-1.0.3/typedspark/_schema/get_schema_definition.py` & `typedspark-1.0.4/typedspark/_schema/get_schema_definition.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.3/typedspark/_schema/get_schema_imports.py` & `typedspark-1.0.4/typedspark/_schema/get_schema_imports.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.3/typedspark/_schema/schema.py` & `typedspark-1.0.4/typedspark/_schema/schema.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.3/typedspark/_schema/structfield.py` & `typedspark-1.0.4/typedspark/_schema/structfield.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.3/typedspark/_transforms/structtype_column.py` & `typedspark-1.0.4/typedspark/_transforms/structtype_column.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,15 +43,14 @@
 
     return struct([v.alias(k) for k, v in _transformations.items()])
 
 
 def _order_columns(
     transformations: Dict[str, SparkColumn], schema: Type[Schema]
 ) -> Dict[str, SparkColumn]:
-    """chispa's DataFrame comparer doesn't deal nicely with StructTypes whose
-    columns are ordered differently, hence we order them the same as in the
-    schema here."""
+    """Chispa's DataFrame comparer doesn't deal nicely with StructTypes whose columns
+    are ordered differently, hence we order them the same as in the schema here."""
     transformations_ordered = {}
     for field in schema.get_structtype().fields:
         transformations_ordered[field.name] = transformations[field.name]
 
     return transformations_ordered
```

### Comparing `typedspark-1.0.3/typedspark/_transforms/transform_to_schema.py` & `typedspark-1.0.4/typedspark/_transforms/transform_to_schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""Module containing functions that are related to transformations to
-DataSets."""
+"""Module containing functions that are related to transformations to DataSets."""
 from functools import reduce
 from typing import Dict, Optional, Type, TypeVar
 
 from pyspark.sql import Column as SparkColumn
 from pyspark.sql import DataFrame
 
 from typedspark._core.column import Column
```

### Comparing `typedspark-1.0.3/typedspark/_transforms/utils.py` & `typedspark-1.0.4/typedspark/_transforms/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,32 +9,31 @@
 
 
 def add_nulls_for_unspecified_columns(
     transformations: Dict[str, SparkColumn],
     schema: Type[Schema],
     previously_existing_columns: Optional[List[str]] = None,
 ) -> Dict[str, SparkColumn]:
-    """Takes the columns from the schema that are not present in the
-    transformation dictionary and sets their values to Null (casted to the
-    corresponding type defined in the schema)."""
+    """Takes the columns from the schema that are not present in the transformation
+    dictionary and sets their values to Null (casted to the corresponding type defined
+    in the schema)."""
     _previously_existing_columns = (
         [] if previously_existing_columns is None else previously_existing_columns
     )
     for field in schema.get_structtype().fields:
         if field.name not in transformations and field.name not in _previously_existing_columns:
             transformations[field.name] = lit(None).cast(field.dataType)
 
     return transformations
 
 
 def convert_keys_to_strings(
     transformations: Optional[Dict[Column, SparkColumn]]
 ) -> Dict[str, SparkColumn]:
-    """Takes the Column keys in transformations and converts them to
-    strings."""
+    """Takes the Column keys in transformations and converts them to strings."""
     if transformations is None:
         return {}
 
     _transformations = {k.str: v for k, v in transformations.items()}
 
     if len(transformations) != len(_transformations):
         raise ValueError(
```

### Comparing `typedspark-1.0.3/typedspark/_utils/create_dataset.py` & `typedspark-1.0.4/typedspark/_utils/create_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,16 +94,16 @@
     }
     return Row(**data_converted)
 
 
 def _create_column_wise_data_from_dict(
     schema: Type[T], data: Dict[Column, List[Any]]
 ) -> List[List[Any]]:
-    """Converts a dict of column to data to a list of lists, where each inner
-    list contains the data for a column."""
+    """Converts a dict of column to data to a list of lists, where each inner list
+    contains the data for a column."""
     data_converted = {k.str: v for k, v in data.items()}
     n_rows_unique = {len(v) for _, v in data.items()}
     if len(n_rows_unique) > 1:
         raise ValueError("The number of rows in the provided data differs per column.")
 
     n_rows = list(n_rows_unique)[0]
     col_data = []
@@ -115,16 +115,16 @@
 
     return col_data
 
 
 def _create_column_wise_data_from_list(
     schema: Type[T], data: List[Dict[Column, Any]]
 ) -> List[List[Any]]:
-    """Converts a list of dicts of column to data to a list of lists, where
-    each inner list contains the data for a column."""
+    """Converts a list of dicts of column to data to a list of lists, where each inner
+    list contains the data for a column."""
     data_converted = [{k.str: v for k, v in row.items()} for row in data]
 
     col_data = []
     for col in get_type_hints(schema).keys():
         col_data += [[row[col] if col in row else None for row in data_converted]]
 
     return col_data
```

### Comparing `typedspark-1.0.3/typedspark/_utils/load_table.py` & `typedspark-1.0.4/typedspark/_utils/load_table.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.3/typedspark/_utils/register_schema_to_dataset.py` & `typedspark-1.0.4/typedspark/_utils/register_schema_to_dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""Module containing functions that are related to registering schema's to
-DataSets."""
+"""Module containing functions that are related to registering schema's to DataSets."""
 import itertools
 from typing import Type, TypeVar
 
 from typedspark._core.dataset import DataSet
 from typedspark._schema.schema import Schema
 
 T = TypeVar("T", bound=Schema)
@@ -62,8 +61,8 @@
         Contains the DataFrame that this Schema is linked to.
         """
 
         _linked_dataframe = dataframe
         _current_id = _counter()
         _original_name = schema.get_schema_name()
 
-    return LinkedSchema
+    return LinkedSchema  # type: ignore
```

### Comparing `typedspark-1.0.3/typedspark.egg-info/PKG-INFO` & `typedspark-1.0.4/typedspark.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typedspark
-Version: 1.0.3
+Version: 1.0.4
 Summary: Column-wise type annotations for pyspark DataFrames
 Home-page: https://github.com/kaiko-ai/typedspark
 Author: Nanne Aben
 Author-email: nanne@kaiko.ai
 License: Apache-2.0
 Keywords: pyspark spark typing type checking annotations
 Classifier: Programming Language :: Python
```

### Comparing `typedspark-1.0.3/typedspark.egg-info/SOURCES.txt` & `typedspark-1.0.4/typedspark.egg-info/SOURCES.txt`

 * *Files identical despite different names*

