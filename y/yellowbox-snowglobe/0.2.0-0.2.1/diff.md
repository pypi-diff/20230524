# Comparing `tmp/yellowbox_snowglobe-0.2.0.tar.gz` & `tmp/yellowbox_snowglobe-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yellowbox_snowglobe-0.2.0.tar", max compression
+gzip compressed data, was "yellowbox_snowglobe-0.2.1.tar", max compression
```

## Comparing `yellowbox_snowglobe-0.2.0.tar` & `yellowbox_snowglobe-0.2.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1065 2023-05-08 13:24:31.698884 yellowbox_snowglobe-0.2.0/LICENSE
--rw-r--r--   0        0        0      523 2023-05-08 13:24:31.698884 yellowbox_snowglobe-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      157 2023-05-08 13:24:31.698884 yellowbox_snowglobe-0.2.0/yellowbox_snowglobe/__init__.py
--rw-r--r--   0        0        0       22 2023-05-08 13:24:31.698884 yellowbox_snowglobe-0.2.0/yellowbox_snowglobe/_version.py
--rw-r--r--   0        0        0     7427 2023-05-08 13:24:31.698884 yellowbox_snowglobe-0.2.0/yellowbox_snowglobe/api.py
--rw-r--r--   0        0        0     1426 2023-05-08 13:24:31.698884 yellowbox_snowglobe-0.2.0/yellowbox_snowglobe/case_mode.py
--rw-r--r--   0        0        0      508 2023-05-08 13:24:31.698884 yellowbox_snowglobe-0.2.0/yellowbox_snowglobe/schema_init.py
--rw-r--r--   0        0        0     1834 2023-05-08 13:24:31.698884 yellowbox_snowglobe-0.2.0/yellowbox_snowglobe/service.py
--rw-r--r--   0        0        0     6417 2023-05-08 13:24:31.698884 yellowbox_snowglobe-0.2.0/yellowbox_snowglobe/session.py
--rw-r--r--   0        0        0     6403 2023-05-08 13:24:31.698884 yellowbox_snowglobe-0.2.0/yellowbox_snowglobe/snow_to_post.py
--rw-r--r--   0        0        0      581 1970-01-01 00:00:00.000000 yellowbox_snowglobe-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-17 08:33:48.112085 yellowbox_snowglobe-0.2.1/LICENSE
+-rw-r--r--   0        0        0      523 2023-05-17 08:33:48.112085 yellowbox_snowglobe-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      157 2023-05-17 08:33:48.112085 yellowbox_snowglobe-0.2.1/yellowbox_snowglobe/__init__.py
+-rw-r--r--   0        0        0       22 2023-05-17 08:33:48.112085 yellowbox_snowglobe-0.2.1/yellowbox_snowglobe/_version.py
+-rw-r--r--   0        0        0     7427 2023-05-17 08:33:48.112085 yellowbox_snowglobe-0.2.1/yellowbox_snowglobe/api.py
+-rw-r--r--   0        0        0     1426 2023-05-17 08:33:48.112085 yellowbox_snowglobe-0.2.1/yellowbox_snowglobe/case_mode.py
+-rw-r--r--   0        0        0      508 2023-05-17 08:33:48.112085 yellowbox_snowglobe-0.2.1/yellowbox_snowglobe/schema_init.py
+-rw-r--r--   0        0        0     1834 2023-05-17 08:33:48.112085 yellowbox_snowglobe-0.2.1/yellowbox_snowglobe/service.py
+-rw-r--r--   0        0        0     6423 2023-05-17 08:33:48.112085 yellowbox_snowglobe-0.2.1/yellowbox_snowglobe/session.py
+-rw-r--r--   0        0        0     6403 2023-05-17 08:33:48.112085 yellowbox_snowglobe-0.2.1/yellowbox_snowglobe/snow_to_post.py
+-rw-r--r--   0        0        0      581 1970-01-01 00:00:00.000000 yellowbox_snowglobe-0.2.1/PKG-INFO
```

### Comparing `yellowbox_snowglobe-0.2.0/LICENSE` & `yellowbox_snowglobe-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yellowbox_snowglobe-0.2.0/pyproject.toml` & `yellowbox_snowglobe-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yellowbox-snowglobe"
-version = "0.2.0"
+version = "0.2.1"
 description = ""
 authors = ["Biocatch LTD <serverteam@biocatch.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 yellowbox = { version = ">=0.7.0", extras = ["postgresql", "webserver"] }
```

### Comparing `yellowbox_snowglobe-0.2.0/yellowbox_snowglobe/api.py` & `yellowbox_snowglobe-0.2.1/yellowbox_snowglobe/api.py`

 * *Files identical despite different names*

### Comparing `yellowbox_snowglobe-0.2.0/yellowbox_snowglobe/case_mode.py` & `yellowbox_snowglobe-0.2.1/yellowbox_snowglobe/case_mode.py`

 * *Files identical despite different names*

### Comparing `yellowbox_snowglobe-0.2.0/yellowbox_snowglobe/service.py` & `yellowbox_snowglobe-0.2.1/yellowbox_snowglobe/service.py`

 * *Files identical despite different names*

### Comparing `yellowbox_snowglobe-0.2.0/yellowbox_snowglobe/session.py` & `yellowbox_snowglobe-0.2.1/yellowbox_snowglobe/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     # a session is an individual connection, containing all the data associated with it.
     next_token = 0  # each session is identified by a token the connector must send on every request
 
     def __init__(self, owner: SnowGlobeAPI, db: Optional[str], schema: str):
         self.owner = owner
 
         self.token = str(self.next_token)
-        self.next_token += 1
+        type(self).next_token += 1
         self.schema = schema
         # all these fields are set and replaced together when we switch the DB
         self.db: Optional[str] = None
         self.engine: Optional[Engine] = None
         self._connection: Optional[Connection] = None
         self._transaction: Optional[Transaction] = None
```

### Comparing `yellowbox_snowglobe-0.2.0/yellowbox_snowglobe/snow_to_post.py` & `yellowbox_snowglobe-0.2.1/yellowbox_snowglobe/snow_to_post.py`

 * *Files identical despite different names*

### Comparing `yellowbox_snowglobe-0.2.0/PKG-INFO` & `yellowbox_snowglobe-0.2.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yellowbox-snowglobe
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 License: MIT
 Author: Biocatch LTD
 Author-email: serverteam@biocatch.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

