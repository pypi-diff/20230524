# Comparing `tmp/bmsdna_lakeapi-0.3.0.tar.gz` & `tmp/bmsdna_lakeapi-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmsdna_lakeapi-0.3.0.tar", max compression
+gzip compressed data, was "bmsdna_lakeapi-0.3.1.tar", max compression
```

## Comparing `bmsdna_lakeapi-0.3.0.tar` & `bmsdna_lakeapi-0.3.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1081 2023-05-23 12:38:31.631579 bmsdna_lakeapi-0.3.0/LICENSE
--rw-r--r--   0        0        0     4722 2023-05-23 12:38:31.631579 bmsdna_lakeapi-0.3.0/README.md
--rw-r--r--   0        0        0      166 2023-05-23 12:38:31.631579 bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 12:38:31.631579 bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/api/__init__.py
--rw-r--r--   0        0        0     1135 2023-05-23 12:38:31.631579 bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/api/api.py
--rw-r--r--   0        0        0      926 2023-05-23 12:38:31.631579 bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/context/__init__.py
--rw-r--r--   0        0        0     5349 2023-05-23 12:38:31.631579 bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/context/df_base.py
--rw-r--r--   0        0        0     3699 2023-05-23 12:38:31.631579 bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/context/df_datafusion.py
--rw-r--r--   0        0        0     8721 2023-05-23 12:38:31.631579 bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/context/df_duckdb.py
--rw-r--r--   0        0        0     6281 2023-05-23 12:38:31.631579 bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/context/df_polars.py
--rw-r--r--   0        0        0        0 2023-05-23 12:38:31.631579 bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/core/__init__.py
--rw-r--r--   0        0        0    12689 2023-05-23 12:38:31.631579 bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/core/config.py
--rw-r--r--   0        0        0    13366 2023-05-23 12:38:31.635580 bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/core/dataframe.py
--rw-r--r--   0        0        0    15906 2023-05-23 12:38:31.635580 bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/core/endpoint.py
--rw-r--r--   0        0        0      187 2023-05-23 12:38:31.635580 bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/core/env.py
--rw-r--r--   0        0        0     1012 2023-05-23 12:38:31.635580 bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/core/log.py
--rw-r--r--   0        0        0     6589 2023-05-23 12:38:31.635580 bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/core/model.py
--rw-r--r--   0        0        0     7822 2023-05-23 12:38:31.635580 bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/core/response.py
--rw-r--r--   0        0        0     4450 2023-05-23 12:38:31.635580 bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/core/route.py
--rw-r--r--   0        0        0     1692 2023-05-23 12:38:31.635580 bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/core/types.py
--rw-r--r--   0        0        0     2361 2023-05-23 12:38:31.635580 bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/core/uservalidation.py
--rw-r--r--   0        0        0      215 2023-05-23 12:38:31.635580 bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/core/yaml.py
--rw-r--r--   0        0        0        0 2023-05-23 12:38:31.635580 bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/polars_extensions/__init__.py
--rw-r--r--   0        0        0     1847 2023-05-23 12:38:31.635580 bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/polars_extensions/delta.py
--rw-r--r--   0        0        0      326 2023-05-23 12:38:31.635580 bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/standalone/__init__.py
--rw-r--r--   0        0        0     1784 2023-05-23 12:38:31.635580 bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/tools/useradd.py
--rw-r--r--   0        0        0     1095 2023-05-23 12:38:31.635580 bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/tools/validateschema.py
--rw-r--r--   0        0        0     3535 2023-05-23 12:38:31.635580 bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/utils/fast_api_utils.py
--rw-r--r--   0        0        0     1842 2023-05-23 12:38:31.635580 bmsdna_lakeapi-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     6016 1970-01-01 00:00:00.000000 bmsdna_lakeapi-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-23 13:42:38.102078 bmsdna_lakeapi-0.3.1/LICENSE
+-rw-r--r--   0        0        0     5638 2023-05-23 13:42:38.102078 bmsdna_lakeapi-0.3.1/README.md
+-rw-r--r--   0        0        0      166 2023-05-23 13:42:38.102078 bmsdna_lakeapi-0.3.1/bmsdna/lakeapi/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 13:42:38.102078 bmsdna_lakeapi-0.3.1/bmsdna/lakeapi/api/__init__.py
+-rw-r--r--   0        0        0     1074 2023-05-23 13:42:38.102078 bmsdna_lakeapi-0.3.1/bmsdna/lakeapi/api/api.py
+-rw-r--r--   0        0        0      926 2023-05-23 13:42:38.102078 bmsdna_lakeapi-0.3.1/bmsdna/lakeapi/context/__init__.py
+-rw-r--r--   0        0        0     5349 2023-05-23 13:42:38.102078 bmsdna_lakeapi-0.3.1/bmsdna/lakeapi/context/df_base.py
+-rw-r--r--   0        0        0     3699 2023-05-23 13:42:38.102078 bmsdna_lakeapi-0.3.1/bmsdna/lakeapi/context/df_datafusion.py
+-rw-r--r--   0        0        0     8721 2023-05-23 13:42:38.102078 bmsdna_lakeapi-0.3.1/bmsdna/lakeapi/context/df_duckdb.py
+-rw-r--r--   0        0        0     6281 2023-05-23 13:42:38.102078 bmsdna_lakeapi-0.3.1/bmsdna/lakeapi/context/df_polars.py
+-rw-r--r--   0        0        0        0 2023-05-23 13:42:38.102078 bmsdna_lakeapi-0.3.1/bmsdna/lakeapi/core/__init__.py
+-rw-r--r--   0        0        0    12689 2023-05-23 13:42:38.102078 bmsdna_lakeapi-0.3.1/bmsdna/lakeapi/core/config.py
+-rw-r--r--   0        0        0    13366 2023-05-23 13:42:38.102078 bmsdna_lakeapi-0.3.1/bmsdna/lakeapi/core/dataframe.py
+-rw-r--r--   0        0        0    15906 2023-05-23 13:42:38.102078 bmsdna_lakeapi-0.3.1/bmsdna/lakeapi/core/endpoint.py
+-rw-r--r--   0        0        0      187 2023-05-23 13:42:38.106078 bmsdna_lakeapi-0.3.1/bmsdna/lakeapi/core/env.py
+-rw-r--r--   0        0        0     1012 2023-05-23 13:42:38.106078 bmsdna_lakeapi-0.3.1/bmsdna/lakeapi/core/log.py
+-rw-r--r--   0        0        0     6589 2023-05-23 13:42:38.106078 bmsdna_lakeapi-0.3.1/bmsdna/lakeapi/core/model.py
+-rw-r--r--   0        0        0     7822 2023-05-23 13:42:38.106078 bmsdna_lakeapi-0.3.1/bmsdna/lakeapi/core/response.py
+-rw-r--r--   0        0        0     4450 2023-05-23 13:42:38.106078 bmsdna_lakeapi-0.3.1/bmsdna/lakeapi/core/route.py
+-rw-r--r--   0        0        0     1692 2023-05-23 13:42:38.106078 bmsdna_lakeapi-0.3.1/bmsdna/lakeapi/core/types.py
+-rw-r--r--   0        0        0     2367 2023-05-23 13:42:38.106078 bmsdna_lakeapi-0.3.1/bmsdna/lakeapi/core/uservalidation.py
+-rw-r--r--   0        0        0      215 2023-05-23 13:42:38.106078 bmsdna_lakeapi-0.3.1/bmsdna/lakeapi/core/yaml.py
+-rw-r--r--   0        0        0        0 2023-05-23 13:42:38.106078 bmsdna_lakeapi-0.3.1/bmsdna/lakeapi/polars_extensions/__init__.py
+-rw-r--r--   0        0        0     1847 2023-05-23 13:42:38.106078 bmsdna_lakeapi-0.3.1/bmsdna/lakeapi/polars_extensions/delta.py
+-rw-r--r--   0        0        0      326 2023-05-23 13:42:38.106078 bmsdna_lakeapi-0.3.1/bmsdna/lakeapi/standalone/__init__.py
+-rw-r--r--   0        0        0     1790 2023-05-23 13:42:38.106078 bmsdna_lakeapi-0.3.1/bmsdna/lakeapi/tools/useradd.py
+-rw-r--r--   0        0        0     1095 2023-05-23 13:42:38.106078 bmsdna_lakeapi-0.3.1/bmsdna/lakeapi/tools/validateschema.py
+-rw-r--r--   0        0        0     3535 2023-05-23 13:42:38.106078 bmsdna_lakeapi-0.3.1/bmsdna/lakeapi/utils/fast_api_utils.py
+-rw-r--r--   0        0        0     1842 2023-05-23 13:42:38.106078 bmsdna_lakeapi-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     6932 1970-01-01 00:00:00.000000 bmsdna_lakeapi-0.3.1/PKG-INFO
```

### Comparing `bmsdna_lakeapi-0.3.0/LICENSE` & `bmsdna_lakeapi-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.3.0/README.md` & `bmsdna_lakeapi-0.3.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -20,15 +20,16 @@
 import bmsdna.lakeapi
 
 def_cfg = bmsdna.lakeapi.get_default_config() # Get default startup config
 cfg = dataclasses.replace(def_cfg, enable_sql_endpoint=True, data_path="tests/data") # Use dataclasses.replace to set the properties you want
 sti = bmsdna.lakeapi.init_lakeapi(app, cfg, "config_test.yml") # Enable it. The first parameter is the FastAPI instance, the 2nd one is the basic config and the third one the config of the tables
 ```
 
-## Installation 
+## Installation
+
 [![PyPI version](https://badge.fury.io/py/bmsdna-lakeapi.svg)](https://pypi.org/project/bmsdna-lakeapi/)
 
 Pypi Package `bmsdna-lakeapi` can be installed like any python package : `pip install bmsdna-lakeapi`
 
 ## OpenApi
 
 Of course, everything works with Open API and FastAPI. Meaning you can add other FastAPI routes, you can use the /docs and /redoc endpoint.
@@ -48,17 +49,17 @@
 
 Of course you need to adjust your http options as needed. Also, you need to `pip install` uvicorn/gunicorn
 
 You can still use environment variables for configuration
 
 ## Environment Variables
 
- - CONFIG_PATH: The path of the config file, defaults to `config.yml`. If you want to split the config, you can specify a folder, too
- - DATA_PATH: The path of the data files, defaults to `data`. Paths in `config.yml` are relative to DATA_PATH
- - ENABLE_SQL_ENDPOINT: Set this to 1 to enable the SQL Endpoint
+- CONFIG_PATH: The path of the config file, defaults to `config.yml`. If you want to split the config, you can specify a folder, too
+- DATA_PATH: The path of the data files, defaults to `data`. Paths in `config.yml` are relative to DATA_PATH
+- ENABLE_SQL_ENDPOINT: Set this to 1 to enable the SQL Endpoint
 
 ## Config File
 
 The application by default relies on a Config file beeing present at the root of your project that's call `config.yml`.
 
 The config file looks something like this, see also [our test yaml](config_test.yml):
 
@@ -165,7 +166,19 @@
       - name: cars
         operators:
           - "="
     dataframe:
       uri: csv/fruits.csv
       file_type: csv
 ```
+
+## Partioning for awesome performance
+
+In order to use partitions, you can either:
+
+- partition by a column you filter on. Obviously
+- partition on a special column called `columnname_md5_prefix_2` which means that you're partitioning by the first two chars of
+  your hex-encoded md5 hash. If you now filter by `columnname` this will greatly reduce files searched for. The number of chars used is up to you, we found two to be meaningful
+- partition on a special column called `columnname_md5_mod_NRPARTIIONS` where your partition value is `str(int(hashlib.md5(COLUMNNAME).hexdigest(), 16) % NRPARTITIONS)`. That might look a bit complicated, but it's not that hard :) your just doing a modulo on your md5 hash which
+  allows you to set the exact number of partitions. Filtering is still happening on `columname` correctly
+
+You must use deltalake to use parttions and you must only have str partition columns for now.
```

### Comparing `bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/api/api.py` & `bmsdna_lakeapi-0.3.1/bmsdna/lakeapi/api/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from dataclasses import dataclass
 from typing import Awaitable, Callable, Final
 from fastapi import FastAPI, Request
 from bmsdna.lakeapi.core.config import BasicConfig, Configs, get_default_config
 from bmsdna.lakeapi.core.route import init_routes
-from bmsdna.lakeapi.core.uservalidation import get_username
 import os
 
 
 @dataclass(frozen=True)
 class LakeApiStartInfo:
     start_config: BasicConfig
     config: Configs
```

### Comparing `bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/context/__init__.py` & `bmsdna_lakeapi-0.3.1/bmsdna/lakeapi/context/__init__.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/context/df_base.py` & `bmsdna_lakeapi-0.3.1/bmsdna/lakeapi/context/df_base.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/context/df_datafusion.py` & `bmsdna_lakeapi-0.3.1/bmsdna/lakeapi/context/df_datafusion.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/context/df_duckdb.py` & `bmsdna_lakeapi-0.3.1/bmsdna/lakeapi/context/df_duckdb.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/context/df_polars.py` & `bmsdna_lakeapi-0.3.1/bmsdna/lakeapi/context/df_polars.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/core/config.py` & `bmsdna_lakeapi-0.3.1/bmsdna/lakeapi/core/config.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/core/dataframe.py` & `bmsdna_lakeapi-0.3.1/bmsdna/lakeapi/core/dataframe.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/core/endpoint.py` & `bmsdna_lakeapi-0.3.1/bmsdna/lakeapi/core/endpoint.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/core/log.py` & `bmsdna_lakeapi-0.3.1/bmsdna/lakeapi/core/log.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/core/model.py` & `bmsdna_lakeapi-0.3.1/bmsdna/lakeapi/core/model.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/core/response.py` & `bmsdna_lakeapi-0.3.1/bmsdna/lakeapi/core/response.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/core/route.py` & `bmsdna_lakeapi-0.3.1/bmsdna/lakeapi/core/route.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/core/types.py` & `bmsdna_lakeapi-0.3.1/bmsdna/lakeapi/core/types.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/core/uservalidation.py` & `bmsdna_lakeapi-0.3.1/bmsdna/lakeapi/core/uservalidation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from typing import List, Sequence
 from fastapi import Depends, HTTPException, Request, status
 from fastapi.security import HTTPBasic, HTTPBasicCredentials
-import argon2
 from bmsdna.lakeapi.core.config import BasicConfig, Configs, UserConfig
 from bmsdna.lakeapi.core.yaml import get_yaml
 import inspect
 from aiocache import cached, Cache
 from aiocache.serializers import PickleSerializer
 from bmsdna.lakeapi.core.env import CACHE_EXPIRATION_TIME_SECONDS
 
@@ -19,14 +18,16 @@
 
 
 userhashmap: dict[str, str] | None = None
 
 
 @cache
 async def is_correct(hash: str, pwd_str: str):
+    import argon2
+
     ph = argon2.PasswordHasher()
     return ph.verify(hash.encode("utf-8"), pwd_str.encode("utf-8"))
 
 
 async def get_username(req: Request, basic_config: BasicConfig, users: Sequence[UserConfig]):
     if req.query_params.get("token") and basic_config.token_jwt_secret is not None:
         import jwt
```

### Comparing `bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/polars_extensions/delta.py` & `bmsdna_lakeapi-0.3.1/bmsdna/lakeapi/polars_extensions/delta.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/tools/useradd.py` & `bmsdna_lakeapi-0.3.1/bmsdna/lakeapi/tools/useradd.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import argon2
-import ruamel.yaml as yml  # need to use ruaml.yaml to write yaml because it preserves comments
 from typing import cast, List, Optional
 import secrets
 import string
 
 
 def generate_strong_password():
     # define the alphabet
@@ -34,14 +33,16 @@
 
 def useradd(name: str, pwd: Optional[str], yaml_file: str):
     hasher = argon2.PasswordHasher()
     if not pwd:
         pwd = generate_strong_password()
     print(name + ": " + pwd)
     hash = hasher.hash(pwd)
+    import ruamel.yaml as yml  # need to use ruaml.yaml to write yaml because it preserves comments
+
     yaml = yml.YAML()
     yaml.indent = 2
     with open(yaml_file, "r", encoding="utf-8") as r:
         data = yaml.load(r)
         cast(list, data["users"]).append({"name": name, "passwordhash": hash})
     with open(yaml_file, "w", encoding="utf-8") as f:
         yaml.dump(data, f)
```

### Comparing `bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/tools/validateschema.py` & `bmsdna_lakeapi-0.3.1/bmsdna/lakeapi/tools/validateschema.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/utils/fast_api_utils.py` & `bmsdna_lakeapi-0.3.1/bmsdna/lakeapi/utils/fast_api_utils.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.3.0/pyproject.toml` & `bmsdna_lakeapi-0.3.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bmsdna-lakeapi"
-version = "0.3.0"
+version = "0.3.1"
 description = ""
 authors = ["DWH Team <you@example.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "bmsdna"}]
 
 [tool.poetry.dependencies]
```

### Comparing `bmsdna_lakeapi-0.3.0/PKG-INFO` & `bmsdna_lakeapi-0.3.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmsdna-lakeapi
-Version: 0.3.0
+Version: 0.3.1
 Summary: 
 License: MIT
 Author: DWH Team
 Author-email: you@example.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -54,15 +54,16 @@
 import bmsdna.lakeapi
 
 def_cfg = bmsdna.lakeapi.get_default_config() # Get default startup config
 cfg = dataclasses.replace(def_cfg, enable_sql_endpoint=True, data_path="tests/data") # Use dataclasses.replace to set the properties you want
 sti = bmsdna.lakeapi.init_lakeapi(app, cfg, "config_test.yml") # Enable it. The first parameter is the FastAPI instance, the 2nd one is the basic config and the third one the config of the tables
 ```
 
-## Installation 
+## Installation
+
 [![PyPI version](https://badge.fury.io/py/bmsdna-lakeapi.svg)](https://pypi.org/project/bmsdna-lakeapi/)
 
 Pypi Package `bmsdna-lakeapi` can be installed like any python package : `pip install bmsdna-lakeapi`
 
 ## OpenApi
 
 Of course, everything works with Open API and FastAPI. Meaning you can add other FastAPI routes, you can use the /docs and /redoc endpoint.
@@ -82,17 +83,17 @@
 
 Of course you need to adjust your http options as needed. Also, you need to `pip install` uvicorn/gunicorn
 
 You can still use environment variables for configuration
 
 ## Environment Variables
 
- - CONFIG_PATH: The path of the config file, defaults to `config.yml`. If you want to split the config, you can specify a folder, too
- - DATA_PATH: The path of the data files, defaults to `data`. Paths in `config.yml` are relative to DATA_PATH
- - ENABLE_SQL_ENDPOINT: Set this to 1 to enable the SQL Endpoint
+- CONFIG_PATH: The path of the config file, defaults to `config.yml`. If you want to split the config, you can specify a folder, too
+- DATA_PATH: The path of the data files, defaults to `data`. Paths in `config.yml` are relative to DATA_PATH
+- ENABLE_SQL_ENDPOINT: Set this to 1 to enable the SQL Endpoint
 
 ## Config File
 
 The application by default relies on a Config file beeing present at the root of your project that's call `config.yml`.
 
 The config file looks something like this, see also [our test yaml](config_test.yml):
 
@@ -200,7 +201,19 @@
         operators:
           - "="
     dataframe:
       uri: csv/fruits.csv
       file_type: csv
 ```
 
+## Partioning for awesome performance
+
+In order to use partitions, you can either:
+
+- partition by a column you filter on. Obviously
+- partition on a special column called `columnname_md5_prefix_2` which means that you're partitioning by the first two chars of
+  your hex-encoded md5 hash. If you now filter by `columnname` this will greatly reduce files searched for. The number of chars used is up to you, we found two to be meaningful
+- partition on a special column called `columnname_md5_mod_NRPARTIIONS` where your partition value is `str(int(hashlib.md5(COLUMNNAME).hexdigest(), 16) % NRPARTITIONS)`. That might look a bit complicated, but it's not that hard :) your just doing a modulo on your md5 hash which
+  allows you to set the exact number of partitions. Filtering is still happening on `columname` correctly
+
+You must use deltalake to use parttions and you must only have str partition columns for now.
+
```

