# Comparing `tmp/databank-0.4.1.tar.gz` & `tmp/databank-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databank-0.4.1.tar", max compression
+gzip compressed data, was "databank-0.5.0.tar", max compression
```

## Comparing `databank-0.4.1.tar` & `databank-0.5.0.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1070 2023-03-24 20:26:16.078915 databank-0.4.1/LICENSE
--rw-r--r--   0        0        0     2706 2023-03-24 20:26:16.078915 databank-0.4.1/README.md
--rw-r--r--   0        0        0       35 2023-03-24 20:26:16.078915 databank-0.4.1/databank/__init__.py
--rw-r--r--   0        0        0     7487 2023-03-24 20:26:16.078915 databank-0.4.1/databank/core.py
--rw-r--r--   0        0        0     2173 2023-03-24 20:26:16.078915 databank-0.4.1/databank/utils.py
--rw-r--r--   0        0        0      513 2023-03-24 20:26:16.078915 databank-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     3187 1970-01-01 00:00:00.000000 databank-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-24 13:17:27.767989 databank-0.5.0/LICENSE
+-rw-r--r--   0        0        0     3490 2023-05-24 13:17:27.767989 databank-0.5.0/README.md
+-rw-r--r--   0        0        0       78 2023-05-24 13:17:27.767989 databank-0.5.0/databank/__init__.py
+-rw-r--r--   0        0        0     7487 2023-05-24 13:17:27.767989 databank-0.5.0/databank/core.py
+-rw-r--r--   0        0        0     3138 2023-05-24 13:17:27.767989 databank-0.5.0/databank/query.py
+-rw-r--r--   0        0        0     2180 2023-05-24 13:17:27.767989 databank-0.5.0/databank/utils.py
+-rw-r--r--   0        0        0      513 2023-05-24 13:17:27.767989 databank-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3971 1970-01-01 00:00:00.000000 databank-0.5.0/PKG-INFO
```

### Comparing `databank-0.4.1/LICENSE` & `databank-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `databank-0.4.1/README.md` & `databank-0.5.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: databank
+Version: 0.5.0
+Summary: Databank is an easy-to-use Python library for making raw SQL queries in a multi-threaded environment.
+Author: snapADDY GmbH
+Author-email: info@snapaddy.com
+Requires-Python: >=3.10,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: sqlalchemy (>=2.0.4,<3.0.0)
+Description-Content-Type: text/markdown
+
 # Databank
 
 [![PyPI](https://img.shields.io/pypi/v/databank.svg)](https://pypi.org/project/databank) ![GitHub Actions](https://github.com/snapADDY/databank/actions/workflows/main.yml/badge.svg)
 
 Databank is an easy-to-use Python library for making raw SQL queries in a multi-threaded environment.
 
 No ORM, no frills. Only raw SQL queries and parameter binding. Thread-safe. Built on top of [SQLAlchemy](https://www.sqlalchemy.org/).
@@ -81,7 +94,36 @@
 If you are using PostgreSQL with `jsonb` columns, you can use a helper function to serialize the parameter values:
 
 ```python
 >>> from databank.utils import serialize_params
 >>> serialize_params({"member": "Ringo", "song": ["Don't Pass Me By", "Octopus's Garden"]})
 {'member': 'Ringo', 'song': '["Don\'t Pass Me By", "Octopus\'s Garden"]'}
 ```
+
+## Query Collection
+
+You can also organize SQL queries in an SQL file and load them into a `QueryCollection`:
+
+```sql
+/* @name insert_data */
+INSERT INTO beatles (id, member) VALUES (:id, :member);
+
+/* @name select_all_data */
+SELECT * FROM beatles;
+```
+
+A query _must_ have a header comment with the name of the query. If a query name is not unique, the last query with the same name will be used. You can parse that file and load the queries into a `QueryCollection`:
+
+```python
+>>> from databank import QueryCollection
+>>> queries = QueryCollection.from_file("queries.sql")
+```
+
+and access the queries like in a dictionary:
+
+```python
+>>> queries["insert_data"]
+'INSERT INTO beatles (id, member) VALUES (:id, :member);'
+>>> queries["select_all_data"]
+'SELECT * FROM beatles;'
+```
+
```

### Comparing `databank-0.4.1/databank/core.py` & `databank-0.5.0/databank/core.py`

 * *Files identical despite different names*

### Comparing `databank-0.4.1/databank/utils.py` & `databank-0.5.0/databank/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import json
-from datetime import datetime, date
+from datetime import date, datetime
 from typing import Any, Mapping, Optional, Union
 
 from sqlalchemy import text
 from sqlalchemy.engine.interfaces import Dialect
 from sqlalchemy.sql.elements import TextClause
 
 # supported types for a row value
-Value = Union[str, int, float, bool, tuple, datetime, date]
+Value = Union[str, int, float, bool, tuple, datetime, date, None]
+
 
 def serialize_params(params: dict[str, Any]) -> dict[str, Value]:
     """Serialize the given parameters to supported data types.
 
     Note
     ----
     Dictionaries and lists are serialized as JSON.
```

### Comparing `databank-0.4.1/pyproject.toml` & `databank-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "databank"
-version = "0.4.1"
+version = "0.5.0"
 description = "Databank is an easy-to-use Python library for making raw SQL queries in a multi-threaded environment."
 readme = "README.md"
 authors = ["snapADDY GmbH <info@snapaddy.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 sqlalchemy = "^2.0.4"
```

### Comparing `databank-0.4.1/PKG-INFO` & `databank-0.5.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: databank
-Version: 0.4.1
-Summary: Databank is an easy-to-use Python library for making raw SQL queries in a multi-threaded environment.
-Author: snapADDY GmbH
-Author-email: info@snapaddy.com
-Requires-Python: >=3.10,<4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: sqlalchemy (>=2.0.4,<3.0.0)
-Description-Content-Type: text/markdown
-
 # Databank
 
 [![PyPI](https://img.shields.io/pypi/v/databank.svg)](https://pypi.org/project/databank) ![GitHub Actions](https://github.com/snapADDY/databank/actions/workflows/main.yml/badge.svg)
 
 Databank is an easy-to-use Python library for making raw SQL queries in a multi-threaded environment.
 
 No ORM, no frills. Only raw SQL queries and parameter binding. Thread-safe. Built on top of [SQLAlchemy](https://www.sqlalchemy.org/).
@@ -95,7 +82,34 @@
 
 ```python
 >>> from databank.utils import serialize_params
 >>> serialize_params({"member": "Ringo", "song": ["Don't Pass Me By", "Octopus's Garden"]})
 {'member': 'Ringo', 'song': '["Don\'t Pass Me By", "Octopus\'s Garden"]'}
 ```
 
+## Query Collection
+
+You can also organize SQL queries in an SQL file and load them into a `QueryCollection`:
+
+```sql
+/* @name insert_data */
+INSERT INTO beatles (id, member) VALUES (:id, :member);
+
+/* @name select_all_data */
+SELECT * FROM beatles;
+```
+
+A query _must_ have a header comment with the name of the query. If a query name is not unique, the last query with the same name will be used. You can parse that file and load the queries into a `QueryCollection`:
+
+```python
+>>> from databank import QueryCollection
+>>> queries = QueryCollection.from_file("queries.sql")
+```
+
+and access the queries like in a dictionary:
+
+```python
+>>> queries["insert_data"]
+'INSERT INTO beatles (id, member) VALUES (:id, :member);'
+>>> queries["select_all_data"]
+'SELECT * FROM beatles;'
+```
```

