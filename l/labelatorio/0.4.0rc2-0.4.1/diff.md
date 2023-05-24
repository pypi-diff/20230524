# Comparing `tmp/labelatorio-0.4.0rc2.tar.gz` & `tmp/labelatorio-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labelatorio-0.4.0rc2.tar", last modified: Wed Mar  8 22:10:08 2023, max compression
+gzip compressed data, was "labelatorio-0.4.1.tar", last modified: Wed May 24 21:49:57 2023, max compression
```

## Comparing `labelatorio-0.4.0rc2.tar` & `labelatorio-0.4.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-03-08 22:10:08.080115 labelatorio-0.4.0rc2/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1075 2022-08-18 17:22:30.000000 labelatorio-0.4.0rc2/LICENSE
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     2318 2023-03-08 22:10:08.079946 labelatorio-0.4.0rc2/PKG-INFO
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1957 2023-01-26 21:43:46.000000 labelatorio-0.4.0rc2/README.md
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      216 2023-02-19 14:49:50.000000 labelatorio-0.4.0rc2/pyproject.toml
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       38 2023-03-08 22:10:08.080167 labelatorio-0.4.0rc2/setup.cfg
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1272 2023-02-25 18:05:03.000000 labelatorio-0.4.0rc2/setup.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-03-08 22:10:08.075081 labelatorio-0.4.0rc2/src/
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-03-08 22:10:08.078240 labelatorio-0.4.0rc2/src/labelatorio/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      120 2023-03-08 22:09:53.000000 labelatorio-0.4.0rc2/src/labelatorio/__init__.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      284 2022-07-06 06:42:29.000000 labelatorio-0.4.0rc2/src/labelatorio/_helpers.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    34211 2023-03-05 21:31:26.000000 labelatorio-0.4.0rc2/src/labelatorio/client.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    10194 2023-01-18 22:07:41.000000 labelatorio-0.4.0rc2/src/labelatorio/data_model.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1423 2023-01-02 19:19:07.000000 labelatorio-0.4.0rc2/src/labelatorio/enums.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1954 2023-01-02 13:34:08.000000 labelatorio-0.4.0rc2/src/labelatorio/query_model.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     6658 2023-03-07 19:41:38.000000 labelatorio-0.4.0rc2/src/labelatorio/serving.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-03-08 22:10:08.079738 labelatorio-0.4.0rc2/src/labelatorio.egg-info/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     2318 2023-03-08 22:10:07.000000 labelatorio-0.4.0rc2/src/labelatorio.egg-info/PKG-INFO
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      468 2023-03-08 22:10:08.000000 labelatorio-0.4.0rc2/src/labelatorio.egg-info/SOURCES.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-03-08 22:10:07.000000 labelatorio-0.4.0rc2/src/labelatorio.egg-info/dependency_links.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2022-07-06 07:53:36.000000 labelatorio-0.4.0rc2/src/labelatorio.egg-info/not-zip-safe
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       59 2023-03-08 22:10:08.000000 labelatorio-0.4.0rc2/src/labelatorio.egg-info/requires.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       12 2023-03-08 22:10:08.000000 labelatorio-0.4.0rc2/src/labelatorio.egg-info/top_level.txt
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-24 21:49:57.219977 labelatorio-0.4.1/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1075 2022-08-18 17:22:30.000000 labelatorio-0.4.1/LICENSE
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     2315 2023-05-24 21:49:57.219821 labelatorio-0.4.1/PKG-INFO
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1957 2023-01-26 21:43:46.000000 labelatorio-0.4.1/README.md
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      216 2023-02-19 14:49:50.000000 labelatorio-0.4.1/pyproject.toml
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       38 2023-05-24 21:49:57.220024 labelatorio-0.4.1/setup.cfg
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1303 2023-05-24 20:36:11.000000 labelatorio-0.4.1/setup.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-24 21:49:57.214300 labelatorio-0.4.1/src/
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-24 21:49:57.218120 labelatorio-0.4.1/src/labelatorio/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      117 2023-05-24 21:48:40.000000 labelatorio-0.4.1/src/labelatorio/__init__.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      284 2022-07-06 06:42:29.000000 labelatorio-0.4.1/src/labelatorio/_helpers.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    34211 2023-03-05 21:31:26.000000 labelatorio-0.4.1/src/labelatorio/client.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    10194 2023-01-18 22:07:41.000000 labelatorio-0.4.1/src/labelatorio/data_model.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1423 2023-01-02 19:19:07.000000 labelatorio-0.4.1/src/labelatorio/enums.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1954 2023-01-02 13:34:08.000000 labelatorio-0.4.1/src/labelatorio/query_model.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     7879 2023-05-24 21:08:44.000000 labelatorio-0.4.1/src/labelatorio/serving.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-24 21:49:57.219596 labelatorio-0.4.1/src/labelatorio.egg-info/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     2315 2023-05-24 21:49:56.000000 labelatorio-0.4.1/src/labelatorio.egg-info/PKG-INFO
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      468 2023-05-24 21:49:57.000000 labelatorio-0.4.1/src/labelatorio.egg-info/SOURCES.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-05-24 21:49:57.000000 labelatorio-0.4.1/src/labelatorio.egg-info/dependency_links.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2022-07-06 07:53:36.000000 labelatorio-0.4.1/src/labelatorio.egg-info/not-zip-safe
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       67 2023-05-24 21:49:57.000000 labelatorio-0.4.1/src/labelatorio.egg-info/requires.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       12 2023-05-24 21:49:57.000000 labelatorio-0.4.1/src/labelatorio.egg-info/top_level.txt
```

### Comparing `labelatorio-0.4.0rc2/LICENSE` & `labelatorio-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `labelatorio-0.4.0rc2/PKG-INFO` & `labelatorio-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labelatorio
-Version: 0.4.0rc2
+Version: 0.4.1
 Summary: Labelator.io python client
 Home-page: https://github.com/blip-solutions/labelatorio-pyclient
 Author: Juraj Bezdek
 Author-email: juraj.bezdek@blip.solutions
 License: MIT License
 Keywords: client labelator-io
 Requires-Python: >=3.8
```

### Comparing `labelatorio-0.4.0rc2/README.md` & `labelatorio-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `labelatorio-0.4.0rc2/setup.py` & `labelatorio-0.4.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,10 +24,11 @@
                 python_requires='>=3.8',
                 install_requires=[
                     "pandas",
                     "requests",
                     "dataclasses-json",
                     "marshmallow",
                     "tqdm",
-                    "pydantic"
+                    "pydantic",
+                    "aiohttp"
                 ]
                 )
```

### Comparing `labelatorio-0.4.0rc2/src/labelatorio/client.py` & `labelatorio-0.4.1/src/labelatorio/client.py`

 * *Files identical despite different names*

### Comparing `labelatorio-0.4.0rc2/src/labelatorio/data_model.py` & `labelatorio-0.4.1/src/labelatorio/data_model.py`

 * *Files identical despite different names*

### Comparing `labelatorio-0.4.0rc2/src/labelatorio/enums.py` & `labelatorio-0.4.1/src/labelatorio/enums.py`

 * *Files identical despite different names*

### Comparing `labelatorio-0.4.0rc2/src/labelatorio/query_model.py` & `labelatorio-0.4.1/src/labelatorio/query_model.py`

 * *Files identical despite different names*

### Comparing `labelatorio-0.4.0rc2/src/labelatorio/serving.py` & `labelatorio-0.4.1/src/labelatorio/serving.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 
 from typing import Dict, List, Union, Optional
 from pydantic import BaseModel, root_validator
 import requests
 import logging
+import aiohttp
+import json
 
 class PredictionRequestRecord(BaseModel):
     text:str
     key:Optional[str]
     contextData:Optional[Dict[str,str]]
     reviewProjectId:Optional[str] #where to send data for review... if not set, will be determined by model project
 
@@ -85,15 +87,15 @@
         if not url:
             if not node_name or not tennant_id :
                 raise Exception("if url is not set, then tenant_id + node_name parameter must be set")
             else:
                 url = f"https://api.labelator.io/nodes/{tennant_id}/{node_name}"
         
 
-        if not requests.get(url).status_code==200:
+        if not requests.get(url, timeout=timeout).status_code==200:
             raise Exception(f"Unable to contact node at {url}")
         self.url=url.rstrip("/")
         self.headers={"access_token": access_token}
         self.timeout=timeout
     
     def predict(
             self,
@@ -115,14 +117,41 @@
             )
 
         if response.status_code==200:
             return PredictResponse(**response.json())
         else:
             raise Exception(f"Unexpected response: {response.status_code}: {response.reason}")
     
+    
+
+
+    async def apredict(
+            self,
+            query: Union[str, PredictionRequestRecord, List[str], List[PredictionRequestRecord]],
+            model=None,
+            explain=False,
+            test=False
+    ) -> PredictResponse:
+        if isinstance(query, str) or isinstance(query, PredictionRequestRecord):
+            query = [query]
+
+        query_url = f"{self.url}/predict"
+        params = {k: v for k, v in {"explain": explain, "text": test, "model_name": model}.items() if v}
+        json_payload = {"texts": [req.dict() if isinstance(req, PredictionRequestRecord) else req for req in query]}
+
+        async with aiohttp.ClientSession() as session:
+            async with session.post(query_url, json=json_payload, headers=self.headers, params=params,
+                                    timeout=self.timeout) as response:
+                if response.status == 200:
+                    response_text = await response.text()
+                    data = json.loads(response_text)
+                    return PredictResponse(**data)
+                else:
+                    raise Exception(f"Unexpected response: {response.status}: {response.reason}")
+
     def get_answers(
             self,
             query:Union[str, AskQuestionRecord, List[str], List[AskQuestionRecord]] , 
             top_k:int=None,
             model=None,
             explain=False,
             test=False,
```

### Comparing `labelatorio-0.4.0rc2/src/labelatorio.egg-info/PKG-INFO` & `labelatorio-0.4.1/src/labelatorio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labelatorio
-Version: 0.4.0rc2
+Version: 0.4.1
 Summary: Labelator.io python client
 Home-page: https://github.com/blip-solutions/labelatorio-pyclient
 Author: Juraj Bezdek
 Author-email: juraj.bezdek@blip.solutions
 License: MIT License
 Keywords: client labelator-io
 Requires-Python: >=3.8
```

