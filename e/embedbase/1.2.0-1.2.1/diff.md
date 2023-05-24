# Comparing `tmp/embedbase-1.2.0.tar.gz` & `tmp/embedbase-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedbase-1.2.0.tar", max compression
+gzip compressed data, was "embedbase-1.2.1.tar", max compression
```

## Comparing `embedbase-1.2.0.tar` & `embedbase-1.2.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1069 2023-05-22 12:12:22.291315 embedbase-1.2.0/LICENSE
--rw-r--r--   0        0        0     4905 2023-05-22 12:12:22.291315 embedbase-1.2.0/README.md
--rw-r--r--   0        0        0      121 2023-05-22 12:12:22.423314 embedbase-1.2.0/embedbase/__init__.py
--rw-r--r--   0        0        0     1716 2023-05-22 12:12:22.423314 embedbase-1.2.0/embedbase/__main__.py
--rw-r--r--   0        0        0      976 2023-05-22 12:12:22.423314 embedbase-1.2.0/embedbase/api.py
--rw-r--r--   0        0        0    17884 2023-05-22 12:12:22.423314 embedbase-1.2.0/embedbase/app.py
--rw-r--r--   0        0        0       88 2023-05-22 12:12:22.423314 embedbase-1.2.0/embedbase/database/__init__.py
--rw-r--r--   0        0        0     3406 2023-05-22 12:12:22.423314 embedbase-1.2.0/embedbase/database/base.py
--rw-r--r--   0        0        0     6220 2023-05-22 12:12:22.423314 embedbase-1.2.0/embedbase/database/memory_db.py
--rw-r--r--   0        0        0    10191 2023-05-22 12:12:22.423314 embedbase-1.2.0/embedbase/database/postgres_db.py
--rw-r--r--   0        0        0     7571 2023-05-22 12:12:22.423314 embedbase-1.2.0/embedbase/database/supabase_db.py
--rw-r--r--   0        0        0       77 2023-05-22 12:12:22.423314 embedbase-1.2.0/embedbase/embedding/__init__.py
--rw-r--r--   0        0        0      858 2023-05-22 12:12:22.423314 embedbase-1.2.0/embedbase/embedding/base.py
--rw-r--r--   0        0        0     1237 2023-05-22 12:12:22.423314 embedbase-1.2.0/embedbase/embedding/cohere.py
--rw-r--r--   0        0        0     2059 2023-05-22 12:12:22.423314 embedbase-1.2.0/embedbase/embedding/openai.py
--rw-r--r--   0        0        0     1551 2023-05-22 12:12:22.423314 embedbase-1.2.0/embedbase/firebase_auth.py
--rw-r--r--   0        0        0      690 2023-05-22 12:12:22.423314 embedbase-1.2.0/embedbase/logging_utils.py
--rw-r--r--   0        0        0      955 2023-05-22 12:12:22.423314 embedbase-1.2.0/embedbase/models.py
--rw-r--r--   0        0        0     1285 2023-05-22 12:12:22.423314 embedbase-1.2.0/embedbase/settings.py
--rw-r--r--   0        0        0     3208 2023-05-22 12:12:22.423314 embedbase-1.2.0/embedbase/strings.py
--rw-r--r--   0        0        0      301 2023-05-22 12:12:22.423314 embedbase-1.2.0/embedbase/supabase_auth.py
--rw-r--r--   0        0        0     3867 2023-05-22 12:12:22.423314 embedbase-1.2.0/embedbase/utils.py
--rw-r--r--   0        0        0     3730 2023-05-22 12:12:22.427314 embedbase-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     6337 1970-01-01 00:00:00.000000 embedbase-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-24 18:53:24.608554 embedbase-1.2.1/LICENSE
+-rw-r--r--   0        0        0     4905 2023-05-24 18:53:24.608554 embedbase-1.2.1/README.md
+-rw-r--r--   0        0        0      121 2023-05-24 18:53:24.724556 embedbase-1.2.1/embedbase/__init__.py
+-rw-r--r--   0        0        0     1716 2023-05-24 18:53:24.724556 embedbase-1.2.1/embedbase/__main__.py
+-rw-r--r--   0        0        0      976 2023-05-24 18:53:24.724556 embedbase-1.2.1/embedbase/api.py
+-rw-r--r--   0        0        0    17884 2023-05-24 18:53:24.724556 embedbase-1.2.1/embedbase/app.py
+-rw-r--r--   0        0        0       88 2023-05-24 18:53:24.724556 embedbase-1.2.1/embedbase/database/__init__.py
+-rw-r--r--   0        0        0     3406 2023-05-24 18:53:24.724556 embedbase-1.2.1/embedbase/database/base.py
+-rw-r--r--   0        0        0     6220 2023-05-24 18:53:24.724556 embedbase-1.2.1/embedbase/database/memory_db.py
+-rw-r--r--   0        0        0    10191 2023-05-24 18:53:24.724556 embedbase-1.2.1/embedbase/database/postgres_db.py
+-rw-r--r--   0        0        0     7571 2023-05-24 18:53:24.724556 embedbase-1.2.1/embedbase/database/supabase_db.py
+-rw-r--r--   0        0        0       77 2023-05-24 18:53:24.724556 embedbase-1.2.1/embedbase/embedding/__init__.py
+-rw-r--r--   0        0        0      858 2023-05-24 18:53:24.724556 embedbase-1.2.1/embedbase/embedding/base.py
+-rw-r--r--   0        0        0     1237 2023-05-24 18:53:24.724556 embedbase-1.2.1/embedbase/embedding/cohere.py
+-rw-r--r--   0        0        0     2059 2023-05-24 18:53:24.724556 embedbase-1.2.1/embedbase/embedding/openai.py
+-rw-r--r--   0        0        0     1551 2023-05-24 18:53:24.724556 embedbase-1.2.1/embedbase/firebase_auth.py
+-rw-r--r--   0        0        0      690 2023-05-24 18:53:24.724556 embedbase-1.2.1/embedbase/logging_utils.py
+-rw-r--r--   0        0        0     1095 2023-05-24 18:53:24.724556 embedbase-1.2.1/embedbase/models.py
+-rw-r--r--   0        0        0     1285 2023-05-24 18:53:24.724556 embedbase-1.2.1/embedbase/settings.py
+-rw-r--r--   0        0        0     3208 2023-05-24 18:53:24.724556 embedbase-1.2.1/embedbase/strings.py
+-rw-r--r--   0        0        0      301 2023-05-24 18:53:24.724556 embedbase-1.2.1/embedbase/supabase_auth.py
+-rw-r--r--   0        0        0     3867 2023-05-24 18:53:24.724556 embedbase-1.2.1/embedbase/utils.py
+-rw-r--r--   0        0        0     3730 2023-05-24 18:53:24.728556 embedbase-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     6337 1970-01-01 00:00:00.000000 embedbase-1.2.1/PKG-INFO
```

### Comparing `embedbase-1.2.0/LICENSE` & `embedbase-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.0/README.md` & `embedbase-1.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 - [ ] Github
 
 ### Vector DBs
 - [x] Supabase
 - [x] Postgres
 - [x] Qdrant
 - [ ] Weaviate
-- [ ] Redix
+- [ ] Redis
 
 ### Embedding Models
 - [x] OpenAI Embeddings
 - [x] sentence-transformers
 - [ ] T5
```

### Comparing `embedbase-1.2.0/embedbase/__main__.py` & `embedbase-1.2.1/embedbase/__main__.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.0/embedbase/api.py` & `embedbase-1.2.1/embedbase/api.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.0/embedbase/app.py` & `embedbase-1.2.1/embedbase/app.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.0/embedbase/database/base.py` & `embedbase-1.2.1/embedbase/database/base.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.0/embedbase/database/memory_db.py` & `embedbase-1.2.1/embedbase/database/memory_db.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.0/embedbase/database/postgres_db.py` & `embedbase-1.2.1/embedbase/database/postgres_db.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.0/embedbase/database/supabase_db.py` & `embedbase-1.2.1/embedbase/database/supabase_db.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.0/embedbase/embedding/base.py` & `embedbase-1.2.1/embedbase/embedding/base.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.0/embedbase/embedding/cohere.py` & `embedbase-1.2.1/embedbase/embedding/cohere.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.0/embedbase/embedding/openai.py` & `embedbase-1.2.1/embedbase/embedding/openai.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.0/embedbase/firebase_auth.py` & `embedbase-1.2.1/embedbase/firebase_auth.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.0/embedbase/logging_utils.py` & `embedbase-1.2.1/embedbase/logging_utils.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.0/embedbase/models.py` & `embedbase-1.2.1/embedbase/models.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List, Optional, Union
 
-from pydantic import BaseModel
+from pydantic import BaseModel, validator
 
 
 class Document(BaseModel):
     id: str
     data: Optional[str]
     hash: str
     embedding: Union[List[float], str]
@@ -16,14 +16,18 @@
     # data can be
     # - a string - for example  "This is a document"
     # TODO: currently only string is supported (later could be images, audio, multi/cross-modal)
     # etc.
     data: str
     metadata: Optional[dict]
 
+    @validator('data')
+    def data_must_not_be_empty(cls, v):
+        assert v != '', 'data must not be empty'
+        return v
 
 class AddRequest(BaseModel):
     documents: List[AddDocument]
     store_data: bool = True
 
 
 class UpdateDocument(BaseModel):
```

### Comparing `embedbase-1.2.0/embedbase/settings.py` & `embedbase-1.2.1/embedbase/settings.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.0/embedbase/strings.py` & `embedbase-1.2.1/embedbase/strings.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.0/embedbase/utils.py` & `embedbase-1.2.1/embedbase/utils.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.0/pyproject.toml` & `embedbase-1.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [virtualenvs]
 create = true
 in-project = true
 
 [tool.poetry]
 name = "embedbase"
-version = "1.2.0"
+version = "1.2.1"
 description = "Open-source API & SDK to integrate your data and easily hook them up to LLMs."
 readme = "README.md"
 authors = ["Different AI <louis@embedbase.xyz>"]
 license = "MIT"
 repository = "https://github.com/different-ai/embedbase"
 homepage = "https://github.com/different-ai/embedbase"
 keywords = ["embeddings", "machine learning", "artificial intelligence", "llm"]
```

### Comparing `embedbase-1.2.0/PKG-INFO` & `embedbase-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embedbase
-Version: 1.2.0
+Version: 1.2.1
 Summary: Open-source API & SDK to integrate your data and easily hook them up to LLMs.
 Home-page: https://github.com/different-ai/embedbase
 License: MIT
 Keywords: embeddings,machine learning,artificial intelligence,llm
 Author: Different AI
 Author-email: louis@embedbase.xyz
 Requires-Python: >=3.8,<4.0
@@ -133,15 +133,15 @@
 - [ ] Github
 
 ### Vector DBs
 - [x] Supabase
 - [x] Postgres
 - [x] Qdrant
 - [ ] Weaviate
-- [ ] Redix
+- [ ] Redis
 
 ### Embedding Models
 - [x] OpenAI Embeddings
 - [x] sentence-transformers
 - [ ] T5
```

