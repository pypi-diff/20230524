# Comparing `tmp/bmsdna_lakeapi-0.4.0.tar.gz` & `tmp/bmsdna_lakeapi-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmsdna_lakeapi-0.4.0.tar", max compression
+gzip compressed data, was "bmsdna_lakeapi-0.4.1.tar", max compression
```

## Comparing `bmsdna_lakeapi-0.4.0.tar` & `bmsdna_lakeapi-0.4.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1081 2023-05-24 06:55:50.029073 bmsdna_lakeapi-0.4.0/LICENSE
--rw-r--r--   0        0        0     6414 2023-05-24 06:55:50.029073 bmsdna_lakeapi-0.4.0/README.md
--rw-r--r--   0        0        0      166 2023-05-24 06:55:50.029073 bmsdna_lakeapi-0.4.0/bmsdna/lakeapi/__init__.py
--rw-r--r--   0        0        0        0 2023-05-24 06:55:50.029073 bmsdna_lakeapi-0.4.0/bmsdna/lakeapi/api/__init__.py
--rw-r--r--   0        0        0     1074 2023-05-24 06:55:50.029073 bmsdna_lakeapi-0.4.0/bmsdna/lakeapi/api/api.py
--rw-r--r--   0        0        0      926 2023-05-24 06:55:50.029073 bmsdna_lakeapi-0.4.0/bmsdna/lakeapi/context/__init__.py
--rw-r--r--   0        0        0     5461 2023-05-24 06:55:50.029073 bmsdna_lakeapi-0.4.0/bmsdna/lakeapi/context/df_base.py
--rw-r--r--   0        0        0     4266 2023-05-24 06:55:50.029073 bmsdna_lakeapi-0.4.0/bmsdna/lakeapi/context/df_datafusion.py
--rw-r--r--   0        0        0     8833 2023-05-24 06:55:50.029073 bmsdna_lakeapi-0.4.0/bmsdna/lakeapi/context/df_duckdb.py
--rw-r--r--   0        0        0     6398 2023-05-24 06:55:50.029073 bmsdna_lakeapi-0.4.0/bmsdna/lakeapi/context/df_polars.py
--rw-r--r--   0        0        0        0 2023-05-24 06:55:50.029073 bmsdna_lakeapi-0.4.0/bmsdna/lakeapi/core/__init__.py
--rw-r--r--   0        0        0    12689 2023-05-24 06:55:50.029073 bmsdna_lakeapi-0.4.0/bmsdna/lakeapi/core/config.py
--rw-r--r--   0        0        0    13366 2023-05-24 06:55:50.029073 bmsdna_lakeapi-0.4.0/bmsdna/lakeapi/core/dataframe.py
--rw-r--r--   0        0        0    16791 2023-05-24 06:55:50.029073 bmsdna_lakeapi-0.4.0/bmsdna/lakeapi/core/endpoint.py
--rw-r--r--   0        0        0      187 2023-05-24 06:55:50.029073 bmsdna_lakeapi-0.4.0/bmsdna/lakeapi/core/env.py
--rw-r--r--   0        0        0     1012 2023-05-24 06:55:50.029073 bmsdna_lakeapi-0.4.0/bmsdna/lakeapi/core/log.py
--rw-r--r--   0        0        0     6836 2023-05-24 06:55:50.029073 bmsdna_lakeapi-0.4.0/bmsdna/lakeapi/core/model.py
--rw-r--r--   0        0        0     7822 2023-05-24 06:55:50.029073 bmsdna_lakeapi-0.4.0/bmsdna/lakeapi/core/response.py
--rw-r--r--   0        0        0     4450 2023-05-24 06:55:50.029073 bmsdna_lakeapi-0.4.0/bmsdna/lakeapi/core/route.py
--rw-r--r--   0        0        0     1692 2023-05-24 06:55:50.029073 bmsdna_lakeapi-0.4.0/bmsdna/lakeapi/core/types.py
--rw-r--r--   0        0        0     2367 2023-05-24 06:55:50.029073 bmsdna_lakeapi-0.4.0/bmsdna/lakeapi/core/uservalidation.py
--rw-r--r--   0        0        0      215 2023-05-24 06:55:50.029073 bmsdna_lakeapi-0.4.0/bmsdna/lakeapi/core/yaml.py
--rw-r--r--   0        0        0        0 2023-05-24 06:55:50.029073 bmsdna_lakeapi-0.4.0/bmsdna/lakeapi/polars_extensions/__init__.py
--rw-r--r--   0        0        0     1847 2023-05-24 06:55:50.029073 bmsdna_lakeapi-0.4.0/bmsdna/lakeapi/polars_extensions/delta.py
--rw-r--r--   0        0        0      326 2023-05-24 06:55:50.029073 bmsdna_lakeapi-0.4.0/bmsdna/lakeapi/standalone/__init__.py
--rw-r--r--   0        0        0     1790 2023-05-24 06:55:50.029073 bmsdna_lakeapi-0.4.0/bmsdna/lakeapi/tools/useradd.py
--rw-r--r--   0        0        0     1095 2023-05-24 06:55:50.029073 bmsdna_lakeapi-0.4.0/bmsdna/lakeapi/tools/validateschema.py
--rw-r--r--   0        0        0     3535 2023-05-24 06:55:50.029073 bmsdna_lakeapi-0.4.0/bmsdna/lakeapi/utils/fast_api_utils.py
--rw-r--r--   0        0        0     1842 2023-05-24 06:55:50.033073 bmsdna_lakeapi-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     7708 1970-01-01 00:00:00.000000 bmsdna_lakeapi-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-24 07:16:56.918809 bmsdna_lakeapi-0.4.1/LICENSE
+-rw-r--r--   0        0        0     6525 2023-05-24 07:16:56.918809 bmsdna_lakeapi-0.4.1/README.md
+-rw-r--r--   0        0        0      166 2023-05-24 07:16:56.922809 bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 07:16:56.922809 bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/api/__init__.py
+-rw-r--r--   0        0        0     1074 2023-05-24 07:16:56.922809 bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/api/api.py
+-rw-r--r--   0        0        0      926 2023-05-24 07:16:56.922809 bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/context/__init__.py
+-rw-r--r--   0        0        0     5461 2023-05-24 07:16:56.922809 bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/context/df_base.py
+-rw-r--r--   0        0        0     4277 2023-05-24 07:16:56.922809 bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/context/df_datafusion.py
+-rw-r--r--   0        0        0     8833 2023-05-24 07:16:56.922809 bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/context/df_duckdb.py
+-rw-r--r--   0        0        0     6398 2023-05-24 07:16:56.922809 bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/context/df_polars.py
+-rw-r--r--   0        0        0        0 2023-05-24 07:16:56.922809 bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/core/__init__.py
+-rw-r--r--   0        0        0    12689 2023-05-24 07:16:56.922809 bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/core/config.py
+-rw-r--r--   0        0        0    13366 2023-05-24 07:16:56.922809 bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/core/dataframe.py
+-rw-r--r--   0        0        0    16912 2023-05-24 07:16:56.922809 bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/core/endpoint.py
+-rw-r--r--   0        0        0      187 2023-05-24 07:16:56.922809 bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/core/env.py
+-rw-r--r--   0        0        0     1012 2023-05-24 07:16:56.922809 bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/core/log.py
+-rw-r--r--   0        0        0     6836 2023-05-24 07:16:56.922809 bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/core/model.py
+-rw-r--r--   0        0        0     7822 2023-05-24 07:16:56.922809 bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/core/response.py
+-rw-r--r--   0        0        0     4450 2023-05-24 07:16:56.922809 bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/core/route.py
+-rw-r--r--   0        0        0     1692 2023-05-24 07:16:56.922809 bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/core/types.py
+-rw-r--r--   0        0        0     2367 2023-05-24 07:16:56.922809 bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/core/uservalidation.py
+-rw-r--r--   0        0        0      215 2023-05-24 07:16:56.922809 bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/core/yaml.py
+-rw-r--r--   0        0        0        0 2023-05-24 07:16:56.922809 bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/polars_extensions/__init__.py
+-rw-r--r--   0        0        0     1847 2023-05-24 07:16:56.922809 bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/polars_extensions/delta.py
+-rw-r--r--   0        0        0      326 2023-05-24 07:16:56.922809 bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/standalone/__init__.py
+-rw-r--r--   0        0        0     1790 2023-05-24 07:16:56.922809 bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/tools/useradd.py
+-rw-r--r--   0        0        0     1095 2023-05-24 07:16:56.922809 bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/tools/validateschema.py
+-rw-r--r--   0        0        0     3535 2023-05-24 07:16:56.922809 bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/utils/fast_api_utils.py
+-rw-r--r--   0        0        0     1842 2023-05-24 07:16:56.926809 bmsdna_lakeapi-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     7819 1970-01-01 00:00:00.000000 bmsdna_lakeapi-0.4.1/PKG-INFO
```

### Comparing `bmsdna_lakeapi-0.4.0/LICENSE` & `bmsdna_lakeapi-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.0/README.md` & `bmsdna_lakeapi-0.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # The BMS Lake API
 
 [![tests](https://github.com/bmsuisse/lakeapi/actions/workflows/python-test.yml/badge.svg?branch=main)](https://github.com/bmsuisse/lakeapi/actions/workflows/python-test.yml)
 
+#### Build on giants
+
+<img src="/assets/LakeAPI.drawio.png" alt="LakeAPI" style="height: 100%; width:100%;"/>
+
 A FastAPI Plugin that allows you to expose your Data Lake as an API, allowing multiple output formats, such as Parquet, Csv, Json, Excel, ...
 
 The lake API also contains a minimal security layer for convenience (Basic Auth), but you can also bring your own.
 
 It contrast to [roapi](https://github.com/roapi/roapi), we intentionally do not want to expose most SQL by default, but we limit possible queries using a config. This makes it easy for you to control what happens on your data. If you want the sql endpoint, you can enable this.
 
 To run the app with default config, just do:
```

### Comparing `bmsdna_lakeapi-0.4.0/bmsdna/lakeapi/api/api.py` & `bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/api/api.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.0/bmsdna/lakeapi/context/__init__.py` & `bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/context/__init__.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.0/bmsdna/lakeapi/context/df_base.py` & `bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/context/df_base.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.0/bmsdna/lakeapi/context/df_datafusion.py` & `bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/context/df_datafusion.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,31 +56,30 @@
     def to_arrow_table(self):
         return self.df.to_arrow_table()
 
     def to_arrow_recordbatch(self, chunk_size: int = 10000):
         return self.df.to_arrow_table().to_reader(max_chunksize=chunk_size)
 
 
-from datafusion import udf
-
-
 def to_json_impl(array: pa.Array) -> pa.Array:
     import json
 
     return pa.array([json.dumps(s) for s in array.to_pylist()], type=pa.string)
 
 
 class DatafusionDbExecutionContextBase(ExecutionContext):
     def __init__(self, session: "datafusion.SessionContext"):
         super().__init__()
         self.session = session
         self._registred_udf = False
 
     def json_function(self, term: pypika.terms.Term):
         if not self._registred_udf:  # does not seem to work
+            from datafusion import udf
+
             to_json = udf(to_json_impl, [pa.struct], pyarrow.string(), "stable")
             self.session.register_udf(to_json)
             self._registred_udf = True
         return pypika.terms.Function("to_json", term)
 
     def register_arrow(
         self,
```

### Comparing `bmsdna_lakeapi-0.4.0/bmsdna/lakeapi/context/df_duckdb.py` & `bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/context/df_duckdb.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.0/bmsdna/lakeapi/context/df_polars.py` & `bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/context/df_polars.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.0/bmsdna/lakeapi/core/config.py` & `bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/core/config.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.0/bmsdna/lakeapi/core/dataframe.py` & `bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/core/dataframe.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.0/bmsdna/lakeapi/core/endpoint.py` & `bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/core/endpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -278,14 +278,16 @@
             new_query = new_query.where(expr) if expr is not None else new_query
 
             import pypika
 
             columns = exclude_cols(df.columns())
             if select:
                 columns = [c for c in columns if c in select.split(",")]
+            if has_complex and format in ["csv", "excel", "scsv", "csv4excel"]:
+                jsonify_complex = True
             if jsonify_complex:
                 new_query = new_query.select(
                     *[
                         pypika.Field(c)
                         if not is_complex_type(base_schema, c)
                         else context.json_function(pypika.Field(c)).as_(c)
                         for c in columns
```

### Comparing `bmsdna_lakeapi-0.4.0/bmsdna/lakeapi/core/log.py` & `bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/core/log.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.0/bmsdna/lakeapi/core/model.py` & `bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/core/model.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.0/bmsdna/lakeapi/core/response.py` & `bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/core/response.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.0/bmsdna/lakeapi/core/route.py` & `bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/core/route.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.0/bmsdna/lakeapi/core/types.py` & `bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/core/types.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.0/bmsdna/lakeapi/core/uservalidation.py` & `bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/core/uservalidation.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.0/bmsdna/lakeapi/polars_extensions/delta.py` & `bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/polars_extensions/delta.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.0/bmsdna/lakeapi/tools/useradd.py` & `bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/tools/useradd.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.0/bmsdna/lakeapi/tools/validateschema.py` & `bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/tools/validateschema.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.0/bmsdna/lakeapi/utils/fast_api_utils.py` & `bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/utils/fast_api_utils.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.0/pyproject.toml` & `bmsdna_lakeapi-0.4.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bmsdna-lakeapi"
-version = "0.4.0"
+version = "0.4.1"
 description = ""
 authors = ["DWH Team <you@example.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "bmsdna"}]
 
 [tool.poetry.dependencies]
```

### Comparing `bmsdna_lakeapi-0.4.0/PKG-INFO` & `bmsdna_lakeapi-0.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmsdna-lakeapi
-Version: 0.4.0
+Version: 0.4.1
 Summary: 
 License: MIT
 Author: DWH Team
 Author-email: you@example.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -32,14 +32,18 @@
 Requires-Dist: xlsxwriter (>=3.1.0,<4.0.0)
 Description-Content-Type: text/markdown
 
 # The BMS Lake API
 
 [![tests](https://github.com/bmsuisse/lakeapi/actions/workflows/python-test.yml/badge.svg?branch=main)](https://github.com/bmsuisse/lakeapi/actions/workflows/python-test.yml)
 
+#### Build on giants
+
+<img src="/assets/LakeAPI.drawio.png" alt="LakeAPI" style="height: 100%; width:100%;"/>
+
 A FastAPI Plugin that allows you to expose your Data Lake as an API, allowing multiple output formats, such as Parquet, Csv, Json, Excel, ...
 
 The lake API also contains a minimal security layer for convenience (Basic Auth), but you can also bring your own.
 
 It contrast to [roapi](https://github.com/roapi/roapi), we intentionally do not want to expose most SQL by default, but we limit possible queries using a config. This makes it easy for you to control what happens on your data. If you want the sql endpoint, you can enable this.
 
 To run the app with default config, just do:
```

