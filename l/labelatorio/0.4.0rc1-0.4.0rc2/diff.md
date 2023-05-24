# Comparing `tmp/labelatorio-0.4.0rc1.tar.gz` & `tmp/labelatorio-0.4.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labelatorio-0.4.0rc1.tar", last modified: Fri Mar  3 22:53:22 2023, max compression
+gzip compressed data, was "labelatorio-0.4.0rc2.tar", last modified: Wed Mar  8 22:10:08 2023, max compression
```

## Comparing `labelatorio-0.4.0rc1.tar` & `labelatorio-0.4.0rc2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-03-03 22:53:22.358992 labelatorio-0.4.0rc1/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1075 2022-08-18 17:22:30.000000 labelatorio-0.4.0rc1/LICENSE
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     2318 2023-03-03 22:53:22.358757 labelatorio-0.4.0rc1/PKG-INFO
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1957 2023-01-26 21:43:46.000000 labelatorio-0.4.0rc1/README.md
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      216 2023-02-19 14:49:50.000000 labelatorio-0.4.0rc1/pyproject.toml
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       38 2023-03-03 22:53:22.359074 labelatorio-0.4.0rc1/setup.cfg
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1272 2023-02-25 18:05:03.000000 labelatorio-0.4.0rc1/setup.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-03-03 22:53:22.353503 labelatorio-0.4.0rc1/src/
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-03-03 22:53:22.357088 labelatorio-0.4.0rc1/src/labelatorio/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      120 2023-03-03 18:48:47.000000 labelatorio-0.4.0rc1/src/labelatorio/__init__.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      284 2022-07-06 06:42:29.000000 labelatorio-0.4.0rc1/src/labelatorio/_helpers.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    34199 2023-02-19 15:11:54.000000 labelatorio-0.4.0rc1/src/labelatorio/client.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    10194 2023-01-18 22:07:41.000000 labelatorio-0.4.0rc1/src/labelatorio/data_model.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1423 2023-01-02 19:19:07.000000 labelatorio-0.4.0rc1/src/labelatorio/enums.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1954 2023-01-02 13:34:08.000000 labelatorio-0.4.0rc1/src/labelatorio/query_model.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     6472 2023-03-03 18:50:48.000000 labelatorio-0.4.0rc1/src/labelatorio/serving.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-03-03 22:53:22.358248 labelatorio-0.4.0rc1/src/labelatorio.egg-info/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     2318 2023-03-03 22:53:22.000000 labelatorio-0.4.0rc1/src/labelatorio.egg-info/PKG-INFO
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      468 2023-03-03 22:53:22.000000 labelatorio-0.4.0rc1/src/labelatorio.egg-info/SOURCES.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-03-03 22:53:22.000000 labelatorio-0.4.0rc1/src/labelatorio.egg-info/dependency_links.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2022-07-06 07:53:36.000000 labelatorio-0.4.0rc1/src/labelatorio.egg-info/not-zip-safe
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       59 2023-03-03 22:53:22.000000 labelatorio-0.4.0rc1/src/labelatorio.egg-info/requires.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       12 2023-03-03 22:53:22.000000 labelatorio-0.4.0rc1/src/labelatorio.egg-info/top_level.txt
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-03-08 22:10:08.080115 labelatorio-0.4.0rc2/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1075 2022-08-18 17:22:30.000000 labelatorio-0.4.0rc2/LICENSE
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     2318 2023-03-08 22:10:08.079946 labelatorio-0.4.0rc2/PKG-INFO
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1957 2023-01-26 21:43:46.000000 labelatorio-0.4.0rc2/README.md
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      216 2023-02-19 14:49:50.000000 labelatorio-0.4.0rc2/pyproject.toml
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       38 2023-03-08 22:10:08.080167 labelatorio-0.4.0rc2/setup.cfg
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1272 2023-02-25 18:05:03.000000 labelatorio-0.4.0rc2/setup.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-03-08 22:10:08.075081 labelatorio-0.4.0rc2/src/
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-03-08 22:10:08.078240 labelatorio-0.4.0rc2/src/labelatorio/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      120 2023-03-08 22:09:53.000000 labelatorio-0.4.0rc2/src/labelatorio/__init__.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      284 2022-07-06 06:42:29.000000 labelatorio-0.4.0rc2/src/labelatorio/_helpers.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    34211 2023-03-05 21:31:26.000000 labelatorio-0.4.0rc2/src/labelatorio/client.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    10194 2023-01-18 22:07:41.000000 labelatorio-0.4.0rc2/src/labelatorio/data_model.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1423 2023-01-02 19:19:07.000000 labelatorio-0.4.0rc2/src/labelatorio/enums.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1954 2023-01-02 13:34:08.000000 labelatorio-0.4.0rc2/src/labelatorio/query_model.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     6658 2023-03-07 19:41:38.000000 labelatorio-0.4.0rc2/src/labelatorio/serving.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-03-08 22:10:08.079738 labelatorio-0.4.0rc2/src/labelatorio.egg-info/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     2318 2023-03-08 22:10:07.000000 labelatorio-0.4.0rc2/src/labelatorio.egg-info/PKG-INFO
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      468 2023-03-08 22:10:08.000000 labelatorio-0.4.0rc2/src/labelatorio.egg-info/SOURCES.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-03-08 22:10:07.000000 labelatorio-0.4.0rc2/src/labelatorio.egg-info/dependency_links.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2022-07-06 07:53:36.000000 labelatorio-0.4.0rc2/src/labelatorio.egg-info/not-zip-safe
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       59 2023-03-08 22:10:08.000000 labelatorio-0.4.0rc2/src/labelatorio.egg-info/requires.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       12 2023-03-08 22:10:08.000000 labelatorio-0.4.0rc2/src/labelatorio.egg-info/top_level.txt
```

### Comparing `labelatorio-0.4.0rc1/LICENSE` & `labelatorio-0.4.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `labelatorio-0.4.0rc1/PKG-INFO` & `labelatorio-0.4.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labelatorio
-Version: 0.4.0rc1
+Version: 0.4.0rc2
 Summary: Labelator.io python client
 Home-page: https://github.com/blip-solutions/labelatorio-pyclient
 Author: Juraj Bezdek
 Author-email: juraj.bezdek@blip.solutions
 License: MIT License
 Keywords: client labelator-io
 Requires-Python: >=3.8
```

### Comparing `labelatorio-0.4.0rc1/README.md` & `labelatorio-0.4.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `labelatorio-0.4.0rc1/setup.py` & `labelatorio-0.4.0rc2/setup.py`

 * *Files identical despite different names*

### Comparing `labelatorio-0.4.0rc1/src/labelatorio/client.py` & `labelatorio-0.4.0rc2/src/labelatorio/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 import os
 from zipfile import ZipFile
 import labelatorio.enums as enums
 from labelatorio.query_model import DocumentQueryFilter, Or
 import time
 
 
-
 class Client:
     """
     A python native Labelator.io Client class that encapsulates access to your Labelator.io data.
    
     """
 
     def __init__(self, 
@@ -462,15 +461,15 @@
             query (Union[DocumentQueryFilter,Or]): query filter to match the documents to be deleted
             wait_for_completion (bool, optional): Triggers synchronous exectuion. Limits the number of records to be deleted to 10 000 (but can be run in loop until no data remains). Defaults to False.
 
         Returns:
             None
         """
 
-        self._call_endpoint("DELETE", f"/projects/{project_id}/doc/", body=query, query_params={"wait_for_completion":wait_for_completion}, entityClass=None)
+        self._call_endpoint("POST", f"/projects/{project_id}/doc/delete-by-query", body=query, query_params={"wait_for_completion":wait_for_completion}, entityClass=None)
 
 
     def delete_all(self, project_id:str)-> None:
         """Bulk delete of all documents in project!
 
         Args:
             project_id (str): Uuid of project
```

### Comparing `labelatorio-0.4.0rc1/src/labelatorio/data_model.py` & `labelatorio-0.4.0rc2/src/labelatorio/data_model.py`

 * *Files identical despite different names*

### Comparing `labelatorio-0.4.0rc1/src/labelatorio/enums.py` & `labelatorio-0.4.0rc2/src/labelatorio/enums.py`

 * *Files identical despite different names*

### Comparing `labelatorio-0.4.0rc1/src/labelatorio/query_model.py` & `labelatorio-0.4.0rc2/src/labelatorio/query_model.py`

 * *Files identical despite different names*

### Comparing `labelatorio-0.4.0rc1/src/labelatorio/serving.py` & `labelatorio-0.4.0rc2/src/labelatorio/serving.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 class Prediction(BaseModel):
     label:str
     score:float
 
 class Answer(BaseModel):
     answer:str
-    score:float
+    score:Optional[float]
 
 class PredictedItem(BaseModel):
     predicted:Union[List[Prediction],List[Answer], None]
     handling:str
     key:Optional[str]=None
     explanations:Optional[List[Dict]]=None
 
@@ -121,30 +121,33 @@
     
     def get_answers(
             self,
             query:Union[str, AskQuestionRecord, List[str], List[AskQuestionRecord]] , 
             top_k:int=None,
             model=None,
             explain=False,
-            test=False
+            test=False,
+            additional_instructions:Optional[str]=None
         )->Union[List[Answer],Answer]:
 
         return_first=False
         if not isinstance(query,list):
             query=[query]
             return_first=True
         if isinstance(query[0],PredictionRequestRecord):
             logging.warn("Using PredictionRequestRecord as a query for get_answer is obsolete. Please use AskQuestionRecord")
         
-            
+        payload = {"texts":[req.dict() if isinstance(req,BaseModel) else req  for req in query]}
+        if additional_instructions:
+            payload["additional_instructions"]=additional_instructions
         
         query_url =  f"{self.url }/get-answer"
         response = requests.post(
                 query_url,
-                json={"texts":[req.dict() if isinstance(req,BaseModel) else req  for req in query]}, 
+                json=payload, 
                 headers=self.headers,
                 params={k:v for k,v in {"explain":explain, "test":test,"top_k":top_k,  "model_name":model}.items() if v},
                 timeout= self.timeout,
             )
 
         if response.status_code==200:
             predictions = response.json().get("predictions")
```

### Comparing `labelatorio-0.4.0rc1/src/labelatorio.egg-info/PKG-INFO` & `labelatorio-0.4.0rc2/src/labelatorio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labelatorio
-Version: 0.4.0rc1
+Version: 0.4.0rc2
 Summary: Labelator.io python client
 Home-page: https://github.com/blip-solutions/labelatorio-pyclient
 Author: Juraj Bezdek
 Author-email: juraj.bezdek@blip.solutions
 License: MIT License
 Keywords: client labelator-io
 Requires-Python: >=3.8
```

