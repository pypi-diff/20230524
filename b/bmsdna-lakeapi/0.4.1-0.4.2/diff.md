# Comparing `tmp/bmsdna_lakeapi-0.4.1.tar.gz` & `tmp/bmsdna_lakeapi-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmsdna_lakeapi-0.4.1.tar", max compression
+gzip compressed data, was "bmsdna_lakeapi-0.4.2.tar", max compression
```

## Comparing `bmsdna_lakeapi-0.4.1.tar` & `bmsdna_lakeapi-0.4.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1081 2023-05-24 07:16:56.918809 bmsdna_lakeapi-0.4.1/LICENSE
--rw-r--r--   0        0        0     6525 2023-05-24 07:16:56.918809 bmsdna_lakeapi-0.4.1/README.md
--rw-r--r--   0        0        0      166 2023-05-24 07:16:56.922809 bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/__init__.py
--rw-r--r--   0        0        0        0 2023-05-24 07:16:56.922809 bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/api/__init__.py
--rw-r--r--   0        0        0     1074 2023-05-24 07:16:56.922809 bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/api/api.py
--rw-r--r--   0        0        0      926 2023-05-24 07:16:56.922809 bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/context/__init__.py
--rw-r--r--   0        0        0     5461 2023-05-24 07:16:56.922809 bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/context/df_base.py
--rw-r--r--   0        0        0     4277 2023-05-24 07:16:56.922809 bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/context/df_datafusion.py
--rw-r--r--   0        0        0     8833 2023-05-24 07:16:56.922809 bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/context/df_duckdb.py
--rw-r--r--   0        0        0     6398 2023-05-24 07:16:56.922809 bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/context/df_polars.py
--rw-r--r--   0        0        0        0 2023-05-24 07:16:56.922809 bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/core/__init__.py
--rw-r--r--   0        0        0    12689 2023-05-24 07:16:56.922809 bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/core/config.py
--rw-r--r--   0        0        0    13366 2023-05-24 07:16:56.922809 bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/core/dataframe.py
--rw-r--r--   0        0        0    16912 2023-05-24 07:16:56.922809 bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/core/endpoint.py
--rw-r--r--   0        0        0      187 2023-05-24 07:16:56.922809 bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/core/env.py
--rw-r--r--   0        0        0     1012 2023-05-24 07:16:56.922809 bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/core/log.py
--rw-r--r--   0        0        0     6836 2023-05-24 07:16:56.922809 bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/core/model.py
--rw-r--r--   0        0        0     7822 2023-05-24 07:16:56.922809 bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/core/response.py
--rw-r--r--   0        0        0     4450 2023-05-24 07:16:56.922809 bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/core/route.py
--rw-r--r--   0        0        0     1692 2023-05-24 07:16:56.922809 bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/core/types.py
--rw-r--r--   0        0        0     2367 2023-05-24 07:16:56.922809 bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/core/uservalidation.py
--rw-r--r--   0        0        0      215 2023-05-24 07:16:56.922809 bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/core/yaml.py
--rw-r--r--   0        0        0        0 2023-05-24 07:16:56.922809 bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/polars_extensions/__init__.py
--rw-r--r--   0        0        0     1847 2023-05-24 07:16:56.922809 bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/polars_extensions/delta.py
--rw-r--r--   0        0        0      326 2023-05-24 07:16:56.922809 bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/standalone/__init__.py
--rw-r--r--   0        0        0     1790 2023-05-24 07:16:56.922809 bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/tools/useradd.py
--rw-r--r--   0        0        0     1095 2023-05-24 07:16:56.922809 bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/tools/validateschema.py
--rw-r--r--   0        0        0     3535 2023-05-24 07:16:56.922809 bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/utils/fast_api_utils.py
--rw-r--r--   0        0        0     1842 2023-05-24 07:16:56.926809 bmsdna_lakeapi-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     7819 1970-01-01 00:00:00.000000 bmsdna_lakeapi-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-24 12:04:18.793997 bmsdna_lakeapi-0.4.2/LICENSE
+-rw-r--r--   0        0        0     6853 2023-05-24 12:04:18.793997 bmsdna_lakeapi-0.4.2/README.md
+-rw-r--r--   0        0        0      271 2023-05-24 12:04:18.793997 bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:04:18.793997 bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/api/__init__.py
+-rw-r--r--   0        0        0     1074 2023-05-24 12:04:18.793997 bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/api/api.py
+-rw-r--r--   0        0        0      926 2023-05-24 12:04:18.793997 bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/context/__init__.py
+-rw-r--r--   0        0        0     5482 2023-05-24 12:04:18.793997 bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/context/df_base.py
+-rw-r--r--   0        0        0     4298 2023-05-24 12:04:18.793997 bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/context/df_datafusion.py
+-rw-r--r--   0        0        0     9021 2023-05-24 12:04:18.797997 bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/context/df_duckdb.py
+-rw-r--r--   0        0        0     6419 2023-05-24 12:04:18.797997 bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/context/df_polars.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:04:18.797997 bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/core/__init__.py
+-rw-r--r--   0        0        0    12194 2023-05-24 12:04:18.797997 bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/core/config.py
+-rw-r--r--   0        0        0    13366 2023-05-24 12:04:18.797997 bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/core/dataframe.py
+-rw-r--r--   0        0        0    18523 2023-05-24 12:04:18.797997 bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/core/endpoint.py
+-rw-r--r--   0        0        0      187 2023-05-24 12:04:18.797997 bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/core/env.py
+-rw-r--r--   0        0        0     1012 2023-05-24 12:04:18.797997 bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/core/log.py
+-rw-r--r--   0        0        0     6836 2023-05-24 12:04:18.797997 bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/core/model.py
+-rw-r--r--   0        0        0     7822 2023-05-24 12:04:18.797997 bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/core/response.py
+-rw-r--r--   0        0        0     4450 2023-05-24 12:04:18.797997 bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/core/route.py
+-rw-r--r--   0        0        0     3144 2023-05-24 12:04:18.797997 bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/core/types.py
+-rw-r--r--   0        0        0     2367 2023-05-24 12:04:18.797997 bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/core/uservalidation.py
+-rw-r--r--   0        0        0      215 2023-05-24 12:04:18.797997 bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/core/yaml.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:04:18.797997 bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/polars_extensions/__init__.py
+-rw-r--r--   0        0        0     1847 2023-05-24 12:04:18.797997 bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/polars_extensions/delta.py
+-rw-r--r--   0        0        0      326 2023-05-24 12:04:18.797997 bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/standalone/__init__.py
+-rw-r--r--   0        0        0     1790 2023-05-24 12:04:18.797997 bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/tools/useradd.py
+-rw-r--r--   0        0        0     1095 2023-05-24 12:04:18.797997 bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/tools/validateschema.py
+-rw-r--r--   0        0        0     3535 2023-05-24 12:04:18.797997 bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/utils/fast_api_utils.py
+-rw-r--r--   0        0        0     1842 2023-05-24 12:04:18.797997 bmsdna_lakeapi-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     8147 1970-01-01 00:00:00.000000 bmsdna_lakeapi-0.4.2/PKG-INFO
```

### Comparing `bmsdna_lakeapi-0.4.1/LICENSE` & `bmsdna_lakeapi-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.1/README.md` & `bmsdna_lakeapi-0.4.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # The BMS Lake API
 
-[![tests](https://github.com/bmsuisse/lakeapi/actions/workflows/python-test.yml/badge.svg?branch=main)](https://github.com/bmsuisse/lakeapi/actions/workflows/python-test.yml)
-
-#### Build on giants
+<h1 align="center">
+  <img src="assets\LakeAPI.drawio.png">
+  <br>
+</h1>
 
-<img src="/assets/LakeAPI.drawio.png" alt="LakeAPI" style="height: 100%; width:100%;"/>
+[![tests](https://github.com/bmsuisse/lakeapi/actions/workflows/python-test.yml/badge.svg?branch=main)](https://github.com/bmsuisse/lakeapi/actions/workflows/python-test.yml)
 
 A FastAPI Plugin that allows you to expose your Data Lake as an API, allowing multiple output formats, such as Parquet, Csv, Json, Excel, ...
 
 The lake API also contains a minimal security layer for convenience (Basic Auth), but you can also bring your own.
 
 It contrast to [roapi](https://github.com/roapi/roapi), we intentionally do not want to expose most SQL by default, but we limit possible queries using a config. This makes it easy for you to control what happens on your data. If you want the sql endpoint, you can enable this.
 
@@ -36,14 +37,21 @@
 
 Pypi Package `bmsdna-lakeapi` can be installed like any python package : `pip install bmsdna-lakeapi`
 
 ## OpenApi
 
 Of course, everything works with Open API and FastAPI. Meaning you can add other FastAPI routes, you can use the /docs and /redoc endpoint.
 
+## Engine
+
+By default, DuckDB is the query engine. Polars and Datafusion are also supported.
+The query engine can be defined on a route level and on a query level with the hidden parameter $engine="duckdb|datafusion|polars".
+
+At the moment DuckDB seems to have an edge and performances the best. Also features like full text search are only available with DuckDB.
+
 ## Default Security
 
 By Default, Basic Authentication is enabled. To add a user, simply run `add_lakeapi_user YOURUSERNAME --yaml-file config.yml`. This will add the user to your config yaml (argon2 encrypted).
 The generated Password is printed. If you do not want this logic, you can overwrite the username_retriver of the Default Config
 
 ## Standalone Mode
```

### Comparing `bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/api/api.py` & `bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/api/api.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/context/__init__.py` & `bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/context/__init__.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/context/df_base.py` & `bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/context/df_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,15 +122,15 @@
         self,
         source_view: str,
         search_configs: list[SearchConfig],
     ):
         pass
 
     @abstractmethod
-    def json_function(self, term: pypika.terms.Term) -> pypika.terms.Term:
+    def json_function(self, term: pypika.terms.Term, assure_string=False) -> pypika.terms.Term:
         ...
 
     def search_score_function(
         self,
         source_view: str,
         search_text: str,
         search_config: SearchConfig,
```

### Comparing `bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/context/df_datafusion.py` & `bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/context/df_datafusion.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 
 class DatafusionDbExecutionContextBase(ExecutionContext):
     def __init__(self, session: "datafusion.SessionContext"):
         super().__init__()
         self.session = session
         self._registred_udf = False
 
-    def json_function(self, term: pypika.terms.Term):
+    def json_function(self, term: pypika.terms.Term, assure_string=False):
         if not self._registred_udf:  # does not seem to work
             from datafusion import udf
 
             to_json = udf(to_json_impl, [pa.struct], pyarrow.string(), "stable")
             self.session.register_udf(to_json)
             self._registred_udf = True
         return pypika.terms.Function("to_json", term)
```

### Comparing `bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/context/df_duckdb.py` & `bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/context/df_duckdb.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 from typing import List, Optional, Tuple, Any, Union
 from bmsdna.lakeapi.core.types import FileTypes
 from bmsdna.lakeapi.context.df_base import ExecutionContext, ResultData
 import duckdb
 import pyarrow.dataset
 import pypika.queries
 import pypika.terms
+import pypika.functions
+import pypika.enums
 import pypika
 import os
 from datetime import datetime, timezone
 from bmsdna.lakeapi.core.config import SearchConfig
 
 ENABLE_COPY_TO = os.getenv("ENABLE_COPY_TO", "0") == "1"
 
@@ -152,16 +154,19 @@
         search_text: str,
         search_config: SearchConfig,
         alias: Optional[str],
     ):
         fields = ",".join(search_config.columns)
         return Match25Term(source_view, pypika.queries.Field("__search_id"), search_text, fields)
 
-    def json_function(self, term: pypika.terms.Term):
-        return pypika.terms.Function("to_json", term)
+    def json_function(self, term: pypika.terms.Term, assure_string=False):
+        fn = pypika.terms.Function("to_json", term)
+        if assure_string:
+            return pypika.functions.Cast(fn, pypika.enums.SqlTypes.VARCHAR)
+        return fn
 
     def init_search(
         self,
         source_view: str,
         search_configs: list[SearchConfig],
     ):
         modified_date = self.modified_dates[source_view]
```

### Comparing `bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/context/df_polars.py` & `bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/context/df_polars.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,15 +121,15 @@
 
         ds = pl.scan_ds(ds)
         self.sql_context.register(name, ds)
 
     def close(self):
         pass
 
-    def json_function(self, term: pypika.terms.Term):
+    def json_function(self, term: pypika.terms.Term, assure_string=False):
         raise NotImplementedError()
 
     def register_dataframe(
         self,
         name: str,
         uri: str,
         file_type: FileTypes,
```

### Comparing `bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/core/config.py` & `bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/core/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from fastapi import APIRouter, Request
 
 import yaml
 from polars.type_aliases import JoinStrategy
 from bmsdna.lakeapi.core.env import CACHE_EXPIRATION_TIME_SECONDS
 
 from bmsdna.lakeapi.core.log import get_logger
-from bmsdna.lakeapi.core.types import FileTypes, OperatorType, PolaryTypeFunction, Engines
+from bmsdna.lakeapi.core.types import FileTypes, OperatorType, Param, PolaryTypeFunction, Engines, SearchConfig
 
 logger = get_logger(__name__)
 
 
 @dataclass(frozen=True)
 class BasicConfig:
     username_retriever: Callable[[Request, "BasicConfig", "Sequence[UserConfig]"], str | Awaitable[str]]
@@ -51,29 +51,14 @@
         data_path=os.environ.get("DATA_PATH", "data"),
         token_jwt_secret=os.getenv("JWT_SECRET", None),
         min_search_length=3,
     )
 
 
 @dataclass
-class Param:
-    name: str
-    combi: Optional[Optional[List[str]]] = None
-    default: Optional[str] = None
-    required: Optional[bool] = False
-    operators: Optional[list[OperatorType]] = None
-    colname: Optional[str] = None
-
-    @property
-    def real_default(self) -> str:
-        self._real_default = ast.literal_eval(self.default) if self.default else None
-        return cast(str, self._real_default)
-
-
-@dataclass
 class Filter:
     key: str
     operator: Literal[
         "=",
         ">",
         "<",
         ">=",
@@ -142,20 +127,14 @@
     sortby: Optional[List[SortBy]] = None
     joins: Optional[List[Join]] = None
     filters: Optional[List[Filter]] = None
     cache_expiration_time_seconds: Optional[int] = CACHE_EXPIRATION_TIME_SECONDS
 
 
 @dataclass
-class SearchConfig:
-    name: str
-    columns: List[str]
-
-
-@dataclass
 class Option:
     ...
 
 
 @dataclass
 class Config:
     name: str
```

### Comparing `bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/core/dataframe.py` & `bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/core/dataframe.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/core/endpoint.py` & `bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/core/endpoint.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import inspect
 from pathlib import Path
-from typing import List, Literal, Optional, Type, Union, cast
-
+from typing import Any, List, Literal, Optional, Type, Union, cast
+from typing_extensions import TypedDict, NotRequired, Required
 import duckdb
 import polars as pl
 import pyarrow as pa
 import pypika
 import pypika.queries as fn
 from aiocache import Cache, cached
 from aiocache.serializers import PickleSerializer
@@ -20,28 +20,34 @@
     Request,
 )
 from pydantic import BaseModel
 from pypika.queries import QueryBuilder
 
 from bmsdna.lakeapi.context import get_context_by_engine
 from bmsdna.lakeapi.context.df_base import ResultData
-from bmsdna.lakeapi.core.config import BasicConfig, Config, Configs
+from bmsdna.lakeapi.core.config import BasicConfig, Config, Configs, Param, SearchConfig
 from bmsdna.lakeapi.core.dataframe import (
     Dataframe,
     filter_df_based_on_params,
     filter_partitions_based_on_params,
 )
 from bmsdna.lakeapi.core.log import get_logger
 from bmsdna.lakeapi.core.model import (
     create_parameter_model,
     create_response_model,
     should_hide_colname,
 )
 from bmsdna.lakeapi.core.response import create_response
-from bmsdna.lakeapi.core.types import OutputFileType, Engines
+from bmsdna.lakeapi.core.types import (
+    MetadataDetailResult,
+    MetadataSchemaField,
+    MetadataSchemaFieldType,
+    OutputFileType,
+    Engines,
+)
 from bmsdna.lakeapi.core.env import CACHE_EXPIRATION_TIME_SECONDS
 
 cache = cached(ttl=CACHE_EXPIRATION_TIME_SECONDS, cache=Cache.MEMORY, serializer=PickleSerializer())
 
 logger = get_logger(__name__)
 
 
@@ -110,87 +116,114 @@
     }
 
 
 def create_detailed_meta_endpoint(
     metamodel: Optional[ResultData], config: Config, router: APIRouter, basic_config: BasicConfig
 ):
     route = config.route + "/metadata_detail"
+    has_complex = True
+    if metamodel is not None:
+        has_complex = any((pa.types.is_struct(t) or pa.types.is_list(t) for t in metamodel.arrow_schema().types))
 
     @router.get(
         route,
         tags=["metadata", "metadata:" + config.tag],
         operation_id=config.tag + "_" + config.name,
         name=config.name + "_metadata",
     )
-    def get_detailed_metadata(req: Request):
+    def get_detailed_metadata(
+        req: Request, jsonify_complex=Query(title="jsonify_complex", include_in_schema=has_complex, default=False)
+    ) -> MetadataDetailResult:
         import json
 
         req.state.lake_api_basic_config = basic_config
         from bmsdna.lakeapi.context.df_duckdb import DuckDbExecutionContext
 
         with DuckDbExecutionContext() as context:
             realdataframe = Dataframe(
                 config.version_str, config.tag, config.name, config.datasource, context, basic_config=basic_config
             )
+
             partition_columns = []
             partition_values = None
             delta_tbl = None
             df = realdataframe.get_df(None)
             if config.datasource.file_type == "delta":
                 delta_tbl = DeltaTable(realdataframe.uri)
                 partition_columns = delta_tbl.metadata().partition_columns
                 if len(partition_columns) > 0:
                     qb: QueryBuilder = (
                         df.query_builder().select(*[pypika.Field(c) for c in partition_columns]).distinct()
                     )
                     partition_values = context.execute_sql(qb).to_arrow_table().to_pylist()
             schema = df.arrow_schema()
             str_cols = [name for name in schema.names if pa.types.is_string(schema.field(name).type)]
-
+            complex_str_cols = (
+                [
+                    name
+                    for name in schema.names
+                    if pa.types.is_struct(schema.field(name).type) or pa.types.is_list(schema.field(name).type)
+                ]
+                if jsonify_complex
+                else []
+            )
             str_lengths_df = (
                 (
                     context.execute_sql(
                         df.query_builder().select(
-                            *[fn.Function("MAX", fn.Function("LEN", fn.Field(sc))).as_(sc) for sc in str_cols]
+                            *(
+                                [fn.Function("MAX", fn.Function("LEN", fn.Field(sc))).as_(sc) for sc in str_cols]
+                                + [
+                                    fn.Function(
+                                        "MAX",
+                                        fn.Function("LEN", context.json_function(fn.Field(sc), assure_string=True)),
+                                    ).as_(sc)
+                                    for sc in complex_str_cols
+                                ]
+                            )
                         )
                     )
                     .to_arrow_table()
                     .to_pylist()
                 )
-                if len(str_cols) > 0
+                if len(str_cols) > 0 or len(complex_str_cols) > 0
                 else [{}]
             )
             str_lengths = str_lengths_df[0]
 
-            def _recursive_get_type(t: Optional[pa.DataType]):
-                if t is None:
-                    return None
-                return {
-                    "type_str": str(t),
-                    "base_type": str(t),  # legacy
-                    "fields": [
-                        {"name": f.name, "type": _recursive_get_type(f.type)}
+            def _recursive_get_type(t: pa.DataType) -> MetadataSchemaFieldType:
+                is_complex = pa.types.is_struct(t) or pa.types.is_list(t)
+
+                return MetadataSchemaFieldType(
+                    type_str=str(pa.string()) if is_complex and jsonify_complex else str(t),
+                    orig_type_str=str(t),
+                    fields=[
+                        MetadataSchemaField(name=f.name, type=_recursive_get_type(f.type))
                         for f in [t.field(find) for find in range(0, cast(pa.StructType, t).num_fields)]
                     ]
-                    if pa.types.is_struct(t)
+                    if pa.types.is_struct(t) and not jsonify_complex
+                    else None,
+                    inner=_recursive_get_type(t.value_type)
+                    if pa.types.is_list(t) and t.value_type is not None and not jsonify_complex
                     else None,
-                    "inner": _recursive_get_type(t.value_type) if pa.types.is_list(t) else None,
-                }
+                )
 
             schema = df.arrow_schema()
-            return {
-                "partition_values": partition_values,
-                "partition_columns": partition_columns,
-                "max_string_lengths": str_lengths,
-                "schema": [{"name": n, "type": _recursive_get_type(schema.field(n).type)} for n in schema.names],
-                "delta_meta": _to_dict(delta_tbl.metadata() if delta_tbl else None),
-                "delta_schema": json.loads(delta_tbl.schema().to_json()) if delta_tbl else None,
-                "parameters": config.params,
-                "search": config.search,
-            }
+            return MetadataDetailResult(
+                partition_values=partition_values,
+                partition_columns=partition_columns,
+                max_string_lengths=str_lengths,
+                data_schema=[
+                    MetadataSchemaField(name=n, type=_recursive_get_type(schema.field(n).type)) for n in schema.names
+                ],
+                delta_meta=_to_dict(delta_tbl.metadata() if delta_tbl else None),
+                delta_schema=json.loads(delta_tbl.schema().to_json()) if delta_tbl else None,
+                parameters=config.params,  # type: ignore
+                search=config.search,
+            )
 
 
 def exclude_cols(columns: List[str]) -> List[str]:
     columns = [c for c in columns if not should_hide_colname(c)]
     return columns
```

### Comparing `bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/core/log.py` & `bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/core/log.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/core/model.py` & `bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/core/model.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/core/response.py` & `bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/core/response.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/core/route.py` & `bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/core/route.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/core/uservalidation.py` & `bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/core/uservalidation.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/polars_extensions/delta.py` & `bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/polars_extensions/delta.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/tools/useradd.py` & `bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/tools/useradd.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/tools/validateschema.py` & `bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/tools/validateschema.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.1/bmsdna/lakeapi/utils/fast_api_utils.py` & `bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/utils/fast_api_utils.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.1/pyproject.toml` & `bmsdna_lakeapi-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bmsdna-lakeapi"
-version = "0.4.1"
+version = "0.4.2"
 description = ""
 authors = ["DWH Team <you@example.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "bmsdna"}]
 
 [tool.poetry.dependencies]
```

### Comparing `bmsdna_lakeapi-0.4.1/PKG-INFO` & `bmsdna_lakeapi-0.4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmsdna-lakeapi
-Version: 0.4.1
+Version: 0.4.2
 Summary: 
 License: MIT
 Author: DWH Team
 Author-email: you@example.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -30,19 +30,20 @@
 Requires-Dist: ruamel.yaml (>=0.17.26,<0.18.0) ; extra == "useradd"
 Requires-Dist: xlsx2csv (>=0.8.1,<0.9.0) ; extra == "polars"
 Requires-Dist: xlsxwriter (>=3.1.0,<4.0.0)
 Description-Content-Type: text/markdown
 
 # The BMS Lake API
 
-[![tests](https://github.com/bmsuisse/lakeapi/actions/workflows/python-test.yml/badge.svg?branch=main)](https://github.com/bmsuisse/lakeapi/actions/workflows/python-test.yml)
-
-#### Build on giants
+<h1 align="center">
+  <img src="assets\LakeAPI.drawio.png">
+  <br>
+</h1>
 
-<img src="/assets/LakeAPI.drawio.png" alt="LakeAPI" style="height: 100%; width:100%;"/>
+[![tests](https://github.com/bmsuisse/lakeapi/actions/workflows/python-test.yml/badge.svg?branch=main)](https://github.com/bmsuisse/lakeapi/actions/workflows/python-test.yml)
 
 A FastAPI Plugin that allows you to expose your Data Lake as an API, allowing multiple output formats, such as Parquet, Csv, Json, Excel, ...
 
 The lake API also contains a minimal security layer for convenience (Basic Auth), but you can also bring your own.
 
 It contrast to [roapi](https://github.com/roapi/roapi), we intentionally do not want to expose most SQL by default, but we limit possible queries using a config. This makes it easy for you to control what happens on your data. If you want the sql endpoint, you can enable this.
 
@@ -70,14 +71,21 @@
 
 Pypi Package `bmsdna-lakeapi` can be installed like any python package : `pip install bmsdna-lakeapi`
 
 ## OpenApi
 
 Of course, everything works with Open API and FastAPI. Meaning you can add other FastAPI routes, you can use the /docs and /redoc endpoint.
 
+## Engine
+
+By default, DuckDB is the query engine. Polars and Datafusion are also supported.
+The query engine can be defined on a route level and on a query level with the hidden parameter $engine="duckdb|datafusion|polars".
+
+At the moment DuckDB seems to have an edge and performances the best. Also features like full text search are only available with DuckDB.
+
 ## Default Security
 
 By Default, Basic Authentication is enabled. To add a user, simply run `add_lakeapi_user YOURUSERNAME --yaml-file config.yml`. This will add the user to your config yaml (argon2 encrypted).
 The generated Password is printed. If you do not want this logic, you can overwrite the username_retriver of the Default Config
 
 ## Standalone Mode
```

