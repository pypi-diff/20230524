# Comparing `tmp/bmsdna_lakeapi-0.4.2.tar.gz` & `tmp/bmsdna_lakeapi-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmsdna_lakeapi-0.4.2.tar", max compression
+gzip compressed data, was "bmsdna_lakeapi-0.4.3.tar", max compression
```

## Comparing `bmsdna_lakeapi-0.4.2.tar` & `bmsdna_lakeapi-0.4.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1081 2023-05-24 12:04:18.793997 bmsdna_lakeapi-0.4.2/LICENSE
--rw-r--r--   0        0        0     6853 2023-05-24 12:04:18.793997 bmsdna_lakeapi-0.4.2/README.md
--rw-r--r--   0        0        0      271 2023-05-24 12:04:18.793997 bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/__init__.py
--rw-r--r--   0        0        0        0 2023-05-24 12:04:18.793997 bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/api/__init__.py
--rw-r--r--   0        0        0     1074 2023-05-24 12:04:18.793997 bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/api/api.py
--rw-r--r--   0        0        0      926 2023-05-24 12:04:18.793997 bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/context/__init__.py
--rw-r--r--   0        0        0     5482 2023-05-24 12:04:18.793997 bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/context/df_base.py
--rw-r--r--   0        0        0     4298 2023-05-24 12:04:18.793997 bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/context/df_datafusion.py
--rw-r--r--   0        0        0     9021 2023-05-24 12:04:18.797997 bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/context/df_duckdb.py
--rw-r--r--   0        0        0     6419 2023-05-24 12:04:18.797997 bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/context/df_polars.py
--rw-r--r--   0        0        0        0 2023-05-24 12:04:18.797997 bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/core/__init__.py
--rw-r--r--   0        0        0    12194 2023-05-24 12:04:18.797997 bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/core/config.py
--rw-r--r--   0        0        0    13366 2023-05-24 12:04:18.797997 bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/core/dataframe.py
--rw-r--r--   0        0        0    18523 2023-05-24 12:04:18.797997 bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/core/endpoint.py
--rw-r--r--   0        0        0      187 2023-05-24 12:04:18.797997 bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/core/env.py
--rw-r--r--   0        0        0     1012 2023-05-24 12:04:18.797997 bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/core/log.py
--rw-r--r--   0        0        0     6836 2023-05-24 12:04:18.797997 bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/core/model.py
--rw-r--r--   0        0        0     7822 2023-05-24 12:04:18.797997 bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/core/response.py
--rw-r--r--   0        0        0     4450 2023-05-24 12:04:18.797997 bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/core/route.py
--rw-r--r--   0        0        0     3144 2023-05-24 12:04:18.797997 bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/core/types.py
--rw-r--r--   0        0        0     2367 2023-05-24 12:04:18.797997 bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/core/uservalidation.py
--rw-r--r--   0        0        0      215 2023-05-24 12:04:18.797997 bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/core/yaml.py
--rw-r--r--   0        0        0        0 2023-05-24 12:04:18.797997 bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/polars_extensions/__init__.py
--rw-r--r--   0        0        0     1847 2023-05-24 12:04:18.797997 bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/polars_extensions/delta.py
--rw-r--r--   0        0        0      326 2023-05-24 12:04:18.797997 bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/standalone/__init__.py
--rw-r--r--   0        0        0     1790 2023-05-24 12:04:18.797997 bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/tools/useradd.py
--rw-r--r--   0        0        0     1095 2023-05-24 12:04:18.797997 bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/tools/validateschema.py
--rw-r--r--   0        0        0     3535 2023-05-24 12:04:18.797997 bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/utils/fast_api_utils.py
--rw-r--r--   0        0        0     1842 2023-05-24 12:04:18.797997 bmsdna_lakeapi-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     8147 1970-01-01 00:00:00.000000 bmsdna_lakeapi-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-24 13:50:04.273458 bmsdna_lakeapi-0.4.3/LICENSE
+-rw-r--r--   0        0        0     6939 2023-05-24 13:50:04.273458 bmsdna_lakeapi-0.4.3/README.md
+-rw-r--r--   0        0        0      271 2023-05-24 13:50:04.277458 bmsdna_lakeapi-0.4.3/bmsdna/lakeapi/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 13:50:04.277458 bmsdna_lakeapi-0.4.3/bmsdna/lakeapi/api/__init__.py
+-rw-r--r--   0        0        0     1074 2023-05-24 13:50:04.277458 bmsdna_lakeapi-0.4.3/bmsdna/lakeapi/api/api.py
+-rw-r--r--   0        0        0      926 2023-05-24 13:50:04.277458 bmsdna_lakeapi-0.4.3/bmsdna/lakeapi/context/__init__.py
+-rw-r--r--   0        0        0     5989 2023-05-24 13:50:04.277458 bmsdna_lakeapi-0.4.3/bmsdna/lakeapi/context/df_base.py
+-rw-r--r--   0        0        0     4072 2023-05-24 13:50:04.277458 bmsdna_lakeapi-0.4.3/bmsdna/lakeapi/context/df_datafusion.py
+-rw-r--r--   0        0        0     8573 2023-05-24 13:50:04.277458 bmsdna_lakeapi-0.4.3/bmsdna/lakeapi/context/df_duckdb.py
+-rw-r--r--   0        0        0     6390 2023-05-24 13:50:04.277458 bmsdna_lakeapi-0.4.3/bmsdna/lakeapi/context/df_polars.py
+-rw-r--r--   0        0        0        0 2023-05-24 13:50:04.277458 bmsdna_lakeapi-0.4.3/bmsdna/lakeapi/core/__init__.py
+-rw-r--r--   0        0        0    12194 2023-05-24 13:50:04.277458 bmsdna_lakeapi-0.4.3/bmsdna/lakeapi/core/config.py
+-rw-r--r--   0        0        0    13366 2023-05-24 13:50:04.277458 bmsdna_lakeapi-0.4.3/bmsdna/lakeapi/core/dataframe.py
+-rw-r--r--   0        0        0    19276 2023-05-24 13:50:04.277458 bmsdna_lakeapi-0.4.3/bmsdna/lakeapi/core/endpoint.py
+-rw-r--r--   0        0        0      187 2023-05-24 13:50:04.277458 bmsdna_lakeapi-0.4.3/bmsdna/lakeapi/core/env.py
+-rw-r--r--   0        0        0     1012 2023-05-24 13:50:04.277458 bmsdna_lakeapi-0.4.3/bmsdna/lakeapi/core/log.py
+-rw-r--r--   0        0        0     6836 2023-05-24 13:50:04.277458 bmsdna_lakeapi-0.4.3/bmsdna/lakeapi/core/model.py
+-rw-r--r--   0        0        0     7822 2023-05-24 13:50:04.277458 bmsdna_lakeapi-0.4.3/bmsdna/lakeapi/core/response.py
+-rw-r--r--   0        0        0     4450 2023-05-24 13:50:04.277458 bmsdna_lakeapi-0.4.3/bmsdna/lakeapi/core/route.py
+-rw-r--r--   0        0        0     3141 2023-05-24 13:50:04.277458 bmsdna_lakeapi-0.4.3/bmsdna/lakeapi/core/types.py
+-rw-r--r--   0        0        0     2367 2023-05-24 13:50:04.277458 bmsdna_lakeapi-0.4.3/bmsdna/lakeapi/core/uservalidation.py
+-rw-r--r--   0        0        0      215 2023-05-24 13:50:04.277458 bmsdna_lakeapi-0.4.3/bmsdna/lakeapi/core/yaml.py
+-rw-r--r--   0        0        0        0 2023-05-24 13:50:04.277458 bmsdna_lakeapi-0.4.3/bmsdna/lakeapi/polars_extensions/__init__.py
+-rw-r--r--   0        0        0     1847 2023-05-24 13:50:04.277458 bmsdna_lakeapi-0.4.3/bmsdna/lakeapi/polars_extensions/delta.py
+-rw-r--r--   0        0        0      326 2023-05-24 13:50:04.277458 bmsdna_lakeapi-0.4.3/bmsdna/lakeapi/standalone/__init__.py
+-rw-r--r--   0        0        0     1790 2023-05-24 13:50:04.277458 bmsdna_lakeapi-0.4.3/bmsdna/lakeapi/tools/useradd.py
+-rw-r--r--   0        0        0     1095 2023-05-24 13:50:04.277458 bmsdna_lakeapi-0.4.3/bmsdna/lakeapi/tools/validateschema.py
+-rw-r--r--   0        0        0     3535 2023-05-24 13:50:04.277458 bmsdna_lakeapi-0.4.3/bmsdna/lakeapi/utils/fast_api_utils.py
+-rw-r--r--   0        0        0     1842 2023-05-24 13:50:04.281458 bmsdna_lakeapi-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     8233 1970-01-01 00:00:00.000000 bmsdna_lakeapi-0.4.3/PKG-INFO
```

### Comparing `bmsdna_lakeapi-0.4.2/LICENSE` & `bmsdna_lakeapi-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.2/README.md` & `bmsdna_lakeapi-0.4.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -39,16 +39,16 @@
 
 ## OpenApi
 
 Of course, everything works with Open API and FastAPI. Meaning you can add other FastAPI routes, you can use the /docs and /redoc endpoint.
 
 ## Engine
 
-By default, DuckDB is the query engine. Polars and Datafusion are also supported.
-The query engine can be defined on a route level and on a query level with the hidden parameter $engine="duckdb|datafusion|polars".
+By default, DuckDB is the query engine. Polars and Datafusion are also supported, but lack some features.
+The query engine can be defined on a route level and on a query level with the hidden parameter $engine="duckdb|datafusion|polars". If you want polars or datafusion, also add the extra required
 
 At the moment DuckDB seems to have an edge and performances the best. Also features like full text search are only available with DuckDB.
 
 ## Default Security
 
 By Default, Basic Authentication is enabled. To add a user, simply run `add_lakeapi_user YOURUSERNAME --yaml-file config.yml`. This will add the user to your config yaml (argon2 encrypted).
 The generated Password is printed. If you do not want this logic, you can overwrite the username_retriver of the Default Config
```

### Comparing `bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/api/api.py` & `bmsdna_lakeapi-0.4.3/bmsdna/lakeapi/api/api.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/context/__init__.py` & `bmsdna_lakeapi-0.4.3/bmsdna/lakeapi/context/__init__.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/context/df_base.py` & `bmsdna_lakeapi-0.4.3/bmsdna/lakeapi/context/df_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,28 @@
 from bmsdna.lakeapi.core.config import SearchConfig
 import pypika.terms
 
 if TYPE_CHECKING:
     import pandas as pd
 
 
+def get_sql(sql_or_pypika: str | pypika.queries.QueryBuilder, limit_zero=False) -> str:
+    if limit_zero:
+        sql_or_pypika = (
+            sql_or_pypika.limit(0)
+            if not isinstance(sql_or_pypika, str)
+            else "SELECT * FROM (" + sql_or_pypika + ") s LIMIT 0 "
+        )
+    if isinstance(sql_or_pypika, str):
+        return sql_or_pypika
+    if len(sql_or_pypika._selects) == 0:
+        return sql_or_pypika.select("*").get_sql()
+    return sql_or_pypika.get_sql()
+
+
 class ResultData(ABC):
     @abstractmethod
     def columns(self) -> List[str]:
         ...
 
     @abstractmethod
     def arrow_schema(self) -> pa.Schema:
```

### Comparing `bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/context/df_datafusion.py` & `bmsdna_lakeapi-0.4.3/bmsdna/lakeapi/context/df_datafusion.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from deltalake import DeltaTable
 
 import pyarrow as pa
 from typing import List, Tuple, Any, Union, TYPE_CHECKING
 from bmsdna.lakeapi.core.types import FileTypes
-from bmsdna.lakeapi.context.df_base import ExecutionContext, ResultData
+from bmsdna.lakeapi.context.df_base import ExecutionContext, ResultData, get_sql
 
 if TYPE_CHECKING:
     import datafusion  # lazy import it on runtime
 import pyarrow.dataset
 import pypika.queries
 import pypika.terms
 import pypika
@@ -30,28 +30,22 @@
 
     def query_builder(self) -> pypika.queries.QueryBuilder:
         return pypika.Query.from_(self.original_sql)
 
     def arrow_schema(self) -> pa.Schema:
         if self._arrow_schema is not None:
             return self._arrow_schema
-        query = (
-            self.original_sql.limit(0).get_sql()
-            if not isinstance(self.original_sql, str)
-            else "SELECT * FROM (" + self.original_sql + ") s LIMIT 0 "
-        )
+        query = get_sql(self.original_sql, limit_zero=True)
         self._arrow_schema = self.session.sql(query).to_arrow_table()
         return self._arrow_schema
 
     @property
     def df(self):
         if self._df is None:
-            self._df = self.session.sql(
-                self.original_sql if isinstance(self.original_sql, str) else self.original_sql.get_sql()
-            )
+            self._df = self.session.sql(get_sql(self.original_sql))
         return self._df
 
     def to_pandas(self):
         return self.df.to_pandas()
 
     def to_arrow_table(self):
         return self.df.to_arrow_table()
```

### Comparing `bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/context/df_duckdb.py` & `bmsdna_lakeapi-0.4.3/bmsdna/lakeapi/context/df_duckdb.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from datetime import datetime
 from deltalake import DeltaTable
 
 import pyarrow as pa
 from typing import List, Optional, Tuple, Any, Union
 from bmsdna.lakeapi.core.types import FileTypes
-from bmsdna.lakeapi.context.df_base import ExecutionContext, ResultData
+from bmsdna.lakeapi.context.df_base import ExecutionContext, ResultData, get_sql
 import duckdb
 import pyarrow.dataset
 import pypika.queries
 import pypika.terms
 import pypika.functions
 import pypika.enums
 import pypika
@@ -36,26 +36,22 @@
 
     def query_builder(self) -> pypika.queries.QueryBuilder:
         return pypika.Query.from_(self.original_sql)
 
     def arrow_schema(self) -> pa.Schema:
         if self._arrow_schema is not None:
             return self._arrow_schema
-        query = (
-            self.original_sql.limit(0).get_sql()
-            if not isinstance(self.original_sql, str)
-            else "SELECT * FROM (" + self.original_sql + ") s LIMIT 0 "
-        )
+        query = get_sql(self.original_sql, limit_zero=True)
         self._arrow_schema = self.con.execute(query).arrow().schema
         return self._arrow_schema
 
     @property
     def df(self):
         if self._df is None:
-            query = self.original_sql if isinstance(self.original_sql, str) else self.original_sql.get_sql()
+            query = get_sql(self.original_sql)
             self._df = self.con.execute(query)
         return self._df
 
     def to_pandas(self):
         return self.df.df()
 
     def to_arrow_table(self):
@@ -63,36 +59,36 @@
 
     def to_arrow_recordbatch(self, chunk_size: int = 10000):
         return self.df.fetch_record_batch(chunk_size)
 
     def write_parquet(self, file_name: str):
         if not ENABLE_COPY_TO:
             return super().write_parquet(file_name)
-        query = self.original_sql if isinstance(self.original_sql, str) else self.original_sql.get_sql()
+        query = get_sql(self.original_sql)
         full_query = f"COPY ({query}) TO '{file_name}' (FORMAT PARQUET,use_tmp_file False, ROW_GROUP_SIZE 10000)"
         self.con.execute(full_query)
 
     def write_nd_json(self, file_name: str):
         if not ENABLE_COPY_TO:
             return super().write_nd_json(file_name)
-        query = self.original_sql if isinstance(self.original_sql, str) else self.original_sql.get_sql()
+        query = get_sql(self.original_sql)
         full_query = f"COPY ({query}) TO '{file_name}' (FORMAT JSON)"
         self.con.execute(full_query)
 
     def write_csv(self, file_name: str, *, separator: str):
         if not ENABLE_COPY_TO:
             return super().write_csv(file_name, separator=separator)
-        query = self.original_sql if isinstance(self.original_sql, str) else self.original_sql.get_sql()
+        query = get_sql(self.original_sql)
         full_query = f"COPY ({query}) TO '{file_name}' (FORMAT CSV, delim '{separator}', header True)"
         self.con.execute(full_query)
 
     def write_json(self, file_name: str):
         if not ENABLE_COPY_TO:
             return super().write_json(file_name)
-        query = self.original_sql if isinstance(self.original_sql, str) else self.original_sql.get_sql()
+        query = get_sql(self.original_sql)
         full_query = f"COPY ({query}) TO '{file_name}' (FORMAT JSON, Array True)"
         self.con.execute(full_query)
 
 
 class Match25Term(pypika.terms.Term):
     def __init__(
         self,
```

### Comparing `bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/context/df_polars.py` & `bmsdna_lakeapi-0.4.3/bmsdna/lakeapi/context/df_polars.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import datetime
-from bmsdna.lakeapi.context.df_base import ExecutionContext, ResultData
+from bmsdna.lakeapi.context.df_base import ExecutionContext, ResultData, get_sql
 
 
 import pyarrow as pa
 from typing import List, Optional, Tuple, Union, cast, TYPE_CHECKING, Any
 import threading
 from bmsdna.lakeapi.core.types import FileTypes
 import pyarrow.dataset
@@ -169,15 +169,15 @@
         sql: Union[
             pypika.queries.QueryBuilder,
             str,
         ],
     ) -> PolarsResultData:
         import polars as pl
 
-        df = self.sql_context.execute(sql.get_sql() if not isinstance(sql, str) else sql)
+        df = self.sql_context.execute(get_sql(sql))
         if isinstance(df, pl.LazyFrame):
             df = df.collect()
         return PolarsResultData(df, self.sql_context)
 
     def __enter__(self):
         return self
```

### Comparing `bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/core/config.py` & `bmsdna_lakeapi-0.4.3/bmsdna/lakeapi/core/config.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/core/dataframe.py` & `bmsdna_lakeapi-0.4.3/bmsdna/lakeapi/core/dataframe.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/core/endpoint.py` & `bmsdna_lakeapi-0.4.3/bmsdna/lakeapi/core/endpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     Query,
     Request,
 )
 from pydantic import BaseModel
 from pypika.queries import QueryBuilder
 
 from bmsdna.lakeapi.context import get_context_by_engine
-from bmsdna.lakeapi.context.df_base import ResultData
+from bmsdna.lakeapi.context.df_base import ResultData, get_sql
 from bmsdna.lakeapi.core.config import BasicConfig, Config, Configs, Param, SearchConfig
 from bmsdna.lakeapi.core.dataframe import (
     Dataframe,
     filter_df_based_on_params,
     filter_partitions_based_on_params,
 )
 from bmsdna.lakeapi.core.log import get_logger
@@ -139,21 +139,26 @@
         from bmsdna.lakeapi.context.df_duckdb import DuckDbExecutionContext
 
         with DuckDbExecutionContext() as context:
             realdataframe = Dataframe(
                 config.version_str, config.tag, config.name, config.datasource, context, basic_config=basic_config
             )
 
+            if not realdataframe.file_exists():
+                raise HTTPException(404)
             partition_columns = []
             partition_values = None
             delta_tbl = None
             df = realdataframe.get_df(None)
             if config.datasource.file_type == "delta":
                 delta_tbl = DeltaTable(realdataframe.uri)
                 partition_columns = delta_tbl.metadata().partition_columns
+                partition_columns = [
+                    c for c in partition_columns if not should_hide_colname(c)
+                ]  # also hide those from metadata detail
                 if len(partition_columns) > 0:
                     qb: QueryBuilder = (
                         df.query_builder().select(*[pypika.Field(c) for c in partition_columns]).distinct()
                     )
                     partition_values = context.execute_sql(qb).to_arrow_table().to_pylist()
             schema = df.arrow_schema()
             str_cols = [name for name in schema.names if pa.types.is_string(schema.field(name).type)]
@@ -297,28 +302,44 @@
 
         ExecutionContext = get_context_by_engine(engine)
 
         with ExecutionContext() as context:
             realdataframe = Dataframe(
                 config.version_str, config.tag, config.name, config.datasource, context, basic_config=basic_config
             )
-
             parts = await get_partitions(realdataframe, params, config)
             df = realdataframe.get_df(parts or None)
 
             expr = await get_params_filter_expr(df.columns(), config, params)
             base_schema = df.arrow_schema()
             new_query = df.query_builder()
             new_query = new_query.where(expr) if expr is not None else new_query
 
+            searches = {}
+            if config.search is not None and params is not None:
+                search_dict = {c.name.lower(): c for c in config.search}
+                searches = {
+                    k: (v, search_dict[k.lower()])
+                    for k, v in params.dict(exclude_unset=True).items()
+                    if k.lower() in search_dict and v is not None and len(v) >= basic_config.min_search_length
+                }
+
             import pypika
 
             columns = exclude_cols(df.columns())
             if select:
                 columns = [c for c in columns if c in select.split(",")]
+            if config.datasource.exclude and len(config.datasource.exclude) > 0:
+                columns = [c for c in columns if c not in config.datasource.exclude]
+            if config.datasource.sortby and len(searches) == 0:
+                for s in config.datasource.sortby:
+                    new_query = new_query.orderby(
+                        s.by,
+                        ord=pypika.Order.desc if s.direction and s.direction.lower() == "desc" else pypika.Order.asc,
+                    )
             if has_complex and format in ["csv", "excel", "scsv", "csv4excel"]:
                 jsonify_complex = True
             if jsonify_complex:
                 new_query = new_query.select(
                     *[
                         pypika.Field(c)
                         if not is_complex_type(base_schema, c)
@@ -333,41 +354,34 @@
                 assert len(columns) <= 3  # reduce complexity here
                 new_query = new_query.distinct()
 
             if not (limit == -1 and config.allow_get_all_pages):
                 limit = 1000 if limit == -1 else limit
                 new_query = new_query.offset(offset or 0).limit(limit)
 
-            if config.search is not None and params is not None:
-                search_dict = {c.name.lower(): c for c in config.search}
-                searches = {
-                    k: (v, search_dict[k.lower()])
-                    for k, v in params.dict(exclude_unset=True).items()
-                    if k.lower() in search_dict and v is not None and len(v) >= basic_config.min_search_length
-                }
-                if len(searches) > 0:
-                    import pypika.queries
-                    import pypika.terms
-
-                    source_view = realdataframe.tablename
-                    context.init_search(source_view, config.search)
-                    score_sum = None
-                    for search_key, (search_val, search_cfg) in searches.items():
-                        score_sum = (
-                            context.search_score_function(source_view, search_val, search_cfg, alias=None)
-                            if score_sum is None
-                            else score_sum
-                            + context.search_score_function(source_view, search_val, search_cfg, alias=None)
-                        )
-                    assert score_sum is not None
-                    new_query = new_query.select(score_sum.as_("search_score"))
-                    new_query = new_query.where(pypika.terms.NotNullCriterion(pypika.queries.Field("search_score")))
-                    new_query = new_query.orderby(pypika.queries.Field("search_score"), order=pypika.Order.desc)
+            if len(searches) > 0 and config.search is not None:
+                import pypika.queries
+                import pypika.terms
+
+                source_view = realdataframe.tablename
+                context.init_search(source_view, config.search)
+                score_sum = None
+                for search_key, (search_val, search_cfg) in searches.items():
+                    score_sum = (
+                        context.search_score_function(source_view, search_val, search_cfg, alias=None)
+                        if score_sum is None
+                        else score_sum + context.search_score_function(source_view, search_val, search_cfg, alias=None)
+                    )
+                assert score_sum is not None
+                new_query = new_query.select(score_sum.as_("search_score"))
+                new_query = new_query.where(pypika.terms.NotNullCriterion(pypika.queries.Field("search_score")))
+
+                new_query = new_query.orderby(pypika.queries.Field("search_score"), order=pypika.Order.desc)
 
-            logger.info(f"Query: {new_query.get_sql()}")
+            logger.info(f"Query: {get_sql(new_query)}")
 
             df2 = context.execute_sql(new_query)
 
             try:
                 return await create_response(
                     username, request.url, format or request.headers["Accept"], df2, context, basic_config=basic_config
                 )
```

### Comparing `bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/core/log.py` & `bmsdna_lakeapi-0.4.3/bmsdna/lakeapi/core/log.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/core/model.py` & `bmsdna_lakeapi-0.4.3/bmsdna/lakeapi/core/model.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/core/response.py` & `bmsdna_lakeapi-0.4.3/bmsdna/lakeapi/core/response.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/core/route.py` & `bmsdna_lakeapi-0.4.3/bmsdna/lakeapi/core/route.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/core/types.py` & `bmsdna_lakeapi-0.4.3/bmsdna/lakeapi/core/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,20 +132,20 @@
         import ast
 
         self._real_default = ast.literal_eval(self.default) if self.default else None
         return cast(str, self._real_default)
 
 
 class MetadataDetailResult(BaseModel):
-    partition_values: Optional[dict[str, Any]]
+    partition_values: Optional[list[dict[str, Any]]]
     partition_columns: List[str]
     max_string_lengths: dict[str, int]
     data_schema: list[MetadataSchemaField]
     delta_meta: Optional[dict]
     delta_schema: Any
     parameters: Optional[List[Any]]
-    search: Optional[List[SearchConfig]]
+    search: Optional[List[Any]]
 
 
 MetadataSchemaFieldType.update_forward_refs()
 MetadataSchemaField.update_forward_refs()
 MetadataDetailResult.update_forward_refs()
```

### Comparing `bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/core/uservalidation.py` & `bmsdna_lakeapi-0.4.3/bmsdna/lakeapi/core/uservalidation.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/polars_extensions/delta.py` & `bmsdna_lakeapi-0.4.3/bmsdna/lakeapi/polars_extensions/delta.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/tools/useradd.py` & `bmsdna_lakeapi-0.4.3/bmsdna/lakeapi/tools/useradd.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/tools/validateschema.py` & `bmsdna_lakeapi-0.4.3/bmsdna/lakeapi/tools/validateschema.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.2/bmsdna/lakeapi/utils/fast_api_utils.py` & `bmsdna_lakeapi-0.4.3/bmsdna/lakeapi/utils/fast_api_utils.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.2/pyproject.toml` & `bmsdna_lakeapi-0.4.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bmsdna-lakeapi"
-version = "0.4.2"
+version = "0.4.3"
 description = ""
 authors = ["DWH Team <you@example.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "bmsdna"}]
 
 [tool.poetry.dependencies]
```

### Comparing `bmsdna_lakeapi-0.4.2/PKG-INFO` & `bmsdna_lakeapi-0.4.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmsdna-lakeapi
-Version: 0.4.2
+Version: 0.4.3
 Summary: 
 License: MIT
 Author: DWH Team
 Author-email: you@example.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -73,16 +73,16 @@
 
 ## OpenApi
 
 Of course, everything works with Open API and FastAPI. Meaning you can add other FastAPI routes, you can use the /docs and /redoc endpoint.
 
 ## Engine
 
-By default, DuckDB is the query engine. Polars and Datafusion are also supported.
-The query engine can be defined on a route level and on a query level with the hidden parameter $engine="duckdb|datafusion|polars".
+By default, DuckDB is the query engine. Polars and Datafusion are also supported, but lack some features.
+The query engine can be defined on a route level and on a query level with the hidden parameter $engine="duckdb|datafusion|polars". If you want polars or datafusion, also add the extra required
 
 At the moment DuckDB seems to have an edge and performances the best. Also features like full text search are only available with DuckDB.
 
 ## Default Security
 
 By Default, Basic Authentication is enabled. To add a user, simply run `add_lakeapi_user YOURUSERNAME --yaml-file config.yml`. This will add the user to your config yaml (argon2 encrypted).
 The generated Password is printed. If you do not want this logic, you can overwrite the username_retriver of the Default Config
```

