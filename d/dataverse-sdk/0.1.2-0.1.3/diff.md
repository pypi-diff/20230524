# Comparing `tmp/dataverse-sdk-0.1.2.tar.gz` & `tmp/dataverse-sdk-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataverse-sdk-0.1.2.tar", last modified: Fri May 19 03:20:05 2023, max compression
+gzip compressed data, was "dataverse-sdk-0.1.3.tar", last modified: Wed May 24 06:43:24 2023, max compression
```

## Comparing `dataverse-sdk-0.1.2.tar` & `dataverse-sdk-0.1.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-05-19 03:20:05.431266 dataverse-sdk-0.1.2/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     5378 2023-05-19 03:20:05.431139 dataverse-sdk-0.1.2/PKG-INFO
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     5138 2023-05-17 07:09:24.000000 dataverse-sdk-0.1.2/README.md
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-05-19 03:20:05.428684 dataverse-sdk-0.1.2/dataverse_sdk/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      825 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.2/dataverse_sdk/__init__.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-05-19 03:20:05.429538 dataverse-sdk-0.1.2/dataverse_sdk/apis/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.2/dataverse_sdk/apis/__init__.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     9053 2023-05-19 03:16:44.000000 dataverse-sdk-0.1.2/dataverse_sdk/apis/backend.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)    16063 2023-05-19 03:16:44.000000 dataverse-sdk-0.1.2/dataverse_sdk/client.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     1550 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.2/dataverse_sdk/connections.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      587 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.2/dataverse_sdk/constants.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-05-19 03:20:05.429968 dataverse-sdk-0.1.2/dataverse_sdk/exceptions/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.2/dataverse_sdk/exceptions/__init__.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)       49 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.2/dataverse_sdk/exceptions/client.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-05-19 03:20:05.430665 dataverse-sdk-0.1.2/dataverse_sdk/schemas/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.2/dataverse_sdk/schemas/__init__.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     3036 2023-05-17 07:09:24.000000 dataverse-sdk-0.1.2/dataverse_sdk/schemas/api.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     7709 2023-05-19 03:16:44.000000 dataverse-sdk-0.1.2/dataverse_sdk/schemas/client.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     1164 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.2/dataverse_sdk/schemas/common.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-05-19 03:20:05.430924 dataverse-sdk-0.1.2/dataverse_sdk/utils/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.2/dataverse_sdk/utils/__init__.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      371 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.2/dataverse_sdk/utils/utils.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-05-19 03:20:05.429311 dataverse-sdk-0.1.2/dataverse_sdk.egg-info/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     5378 2023-05-19 03:20:05.000000 dataverse-sdk-0.1.2/dataverse_sdk.egg-info/PKG-INFO
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      629 2023-05-19 03:20:05.000000 dataverse-sdk-0.1.2/dataverse_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 yihsuanchen   (501) staff       (20)        1 2023-05-19 03:20:05.000000 dataverse-sdk-0.1.2/dataverse_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 yihsuanchen   (501) staff       (20)       18 2023-05-19 03:20:05.000000 dataverse-sdk-0.1.2/dataverse_sdk.egg-info/requires.txt
--rw-r--r--   0 yihsuanchen   (501) staff       (20)       14 2023-05-19 03:20:05.000000 dataverse-sdk-0.1.2/dataverse_sdk.egg-info/top_level.txt
--rw-r--r--   0 yihsuanchen   (501) staff       (20)       38 2023-05-19 03:20:05.431304 dataverse-sdk-0.1.2/setup.cfg
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      613 2023-05-17 07:09:24.000000 dataverse-sdk-0.1.2/setup.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-05-24 06:43:24.047591 dataverse-sdk-0.1.3/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     5983 2023-05-24 06:43:24.047472 dataverse-sdk-0.1.3/PKG-INFO
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     5743 2023-05-24 06:41:33.000000 dataverse-sdk-0.1.3/README.md
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-05-24 06:43:24.044969 dataverse-sdk-0.1.3/dataverse_sdk/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      825 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.3/dataverse_sdk/__init__.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-05-24 06:43:24.045980 dataverse-sdk-0.1.3/dataverse_sdk/apis/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.3/dataverse_sdk/apis/__init__.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)    10150 2023-05-24 06:41:33.000000 dataverse-sdk-0.1.3/dataverse_sdk/apis/backend.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)    19626 2023-05-24 06:41:33.000000 dataverse-sdk-0.1.3/dataverse_sdk/client.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     1550 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.3/dataverse_sdk/connections.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      587 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.3/dataverse_sdk/constants.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-05-24 06:43:24.046311 dataverse-sdk-0.1.3/dataverse_sdk/exceptions/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.3/dataverse_sdk/exceptions/__init__.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)       49 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.3/dataverse_sdk/exceptions/client.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-05-24 06:43:24.047047 dataverse-sdk-0.1.3/dataverse_sdk/schemas/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.3/dataverse_sdk/schemas/__init__.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     3036 2023-05-17 07:09:24.000000 dataverse-sdk-0.1.3/dataverse_sdk/schemas/api.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     8689 2023-05-24 06:41:33.000000 dataverse-sdk-0.1.3/dataverse_sdk/schemas/client.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     1164 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.3/dataverse_sdk/schemas/common.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-05-24 06:43:24.047288 dataverse-sdk-0.1.3/dataverse_sdk/utils/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.3/dataverse_sdk/utils/__init__.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      371 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.3/dataverse_sdk/utils/utils.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-05-24 06:43:24.045739 dataverse-sdk-0.1.3/dataverse_sdk.egg-info/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     5983 2023-05-24 06:43:24.000000 dataverse-sdk-0.1.3/dataverse_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      629 2023-05-24 06:43:24.000000 dataverse-sdk-0.1.3/dataverse_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)        1 2023-05-24 06:43:24.000000 dataverse-sdk-0.1.3/dataverse_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)       18 2023-05-24 06:43:24.000000 dataverse-sdk-0.1.3/dataverse_sdk.egg-info/requires.txt
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)       14 2023-05-24 06:43:24.000000 dataverse-sdk-0.1.3/dataverse_sdk.egg-info/top_level.txt
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)       38 2023-05-24 06:43:24.047627 dataverse-sdk-0.1.3/setup.cfg
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      613 2023-05-24 06:41:33.000000 dataverse-sdk-0.1.3/setup.py
```

### Comparing `dataverse-sdk-0.1.2/PKG-INFO` & `dataverse-sdk-0.1.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: dataverse-sdk
-Version: 0.1.2
-Summary: Dataverse SDK For Python
-Home-page: 
-Author: LinkerVision
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9, <4
-Description-Content-Type: text/markdown
-
 # Dataverse SDK For Python
 Dataverse is a MLOPs platform for assisting in data selection, data visualization and model training in comupter vision.
 Use Dataverse-SDK for Python to help you to interact with the Dataverse platform by Python. Currently, the library supports:
   - Create Project with your input ontology and sensors
   - Get Project by project-id
   - Create Dataset from your AWS/Azure storage or local
   - Get Dataset by dataset-id
@@ -51,15 +41,15 @@
 The following sections provide examples for the most common DataVerse tasksm including:
 
 * [List Projects](#list-projects)
 * [Create Project](#create-project)
 * [Get Project](#get-project)
 * [Create Dataset](#create-dataset)
 * [Get Dataset](#get-dataset)
-
+* [List Models](#list-models)
 
 ### List Projects
 The `list_projects` method will list all projects of the given sites.
 
 
 ```Python
 projects = client.list_projects(current_user = True,
@@ -162,14 +152,38 @@
 
 The `get_dataset` method retrieves the dataset info from the connected site. The `id` parameter is the unique interger ID of the dataset, not its "name" property.
 
 ```Python
 dataset = client.get_dataset(id)
 ```
 
+### List Models
+The `list_models` method will list all the models in the given project
+
+```Python
+#1
+models = client.list_models(project_id = 1)
+#2
+project = client.get_project(project_id=1)
+models = project.list_models()
+```
+### Get Model
+The `get_model` method will get the model detail info by the given model-id
+
+```Python
+model = client.get_model(model_id=30)
+model = project.get_model(model_id=30)
+```
+From the given model, we could get the label file and the triton model file by the commands below.
+```Python
+model.get_label_file()
+model.get_triton_model_file()
+
+```
+
 
 ## Troubleshooting
 
 
 ## Next steps
```

### Comparing `dataverse-sdk-0.1.2/README.md` & `dataverse-sdk-0.1.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: dataverse-sdk
+Version: 0.1.3
+Summary: Dataverse SDK For Python
+Home-page: 
+Author: LinkerVision
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.9, <4
+Description-Content-Type: text/markdown
+
 # Dataverse SDK For Python
 Dataverse is a MLOPs platform for assisting in data selection, data visualization and model training in comupter vision.
 Use Dataverse-SDK for Python to help you to interact with the Dataverse platform by Python. Currently, the library supports:
   - Create Project with your input ontology and sensors
   - Get Project by project-id
   - Create Dataset from your AWS/Azure storage or local
   - Get Dataset by dataset-id
@@ -41,15 +51,15 @@
 The following sections provide examples for the most common DataVerse tasksm including:
 
 * [List Projects](#list-projects)
 * [Create Project](#create-project)
 * [Get Project](#get-project)
 * [Create Dataset](#create-dataset)
 * [Get Dataset](#get-dataset)
-
+* [List Models](#list-models)
 
 ### List Projects
 The `list_projects` method will list all projects of the given sites.
 
 
 ```Python
 projects = client.list_projects(current_user = True,
@@ -152,14 +162,38 @@
 
 The `get_dataset` method retrieves the dataset info from the connected site. The `id` parameter is the unique interger ID of the dataset, not its "name" property.
 
 ```Python
 dataset = client.get_dataset(id)
 ```
 
+### List Models
+The `list_models` method will list all the models in the given project
+
+```Python
+#1
+models = client.list_models(project_id = 1)
+#2
+project = client.get_project(project_id=1)
+models = project.list_models()
+```
+### Get Model
+The `get_model` method will get the model detail info by the given model-id
+
+```Python
+model = client.get_model(model_id=30)
+model = project.get_model(model_id=30)
+```
+From the given model, we could get the label file and the triton model file by the commands below.
+```Python
+model.get_label_file()
+model.get_triton_model_file()
+
+```
+
 
 ## Troubleshooting
 
 
 ## Next steps
```

### Comparing `dataverse-sdk-0.1.2/dataverse_sdk/__init__.py` & `dataverse-sdk-0.1.3/dataverse_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `dataverse-sdk-0.1.2/dataverse_sdk/apis/backend.py` & `dataverse-sdk-0.1.3/dataverse_sdk/apis/backend.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import inspect
 import json
 import logging
+from io import BytesIO
 from typing import Optional, Union
 from urllib.parse import urlencode
 
 import requests
 from requests import sessions
 from requests.adapters import HTTPAdapter, Retry
 
@@ -183,14 +184,47 @@
         resp = self.send_request(
             url=f"{self.host}/api/projects/basic/?{urlencode(kwargs)}",
             method="get",
             headers=self.headers,
         )
         return resp.json()["results"]
 
+    def list_ml_models(self, project_id: int, **kwargs) -> list:
+        kwargs["project"] = project_id
+        resp = self.send_request(
+            url=f"{self.host}/api/ml_models/?{urlencode(kwargs)}",
+            method="get",
+            headers=self.headers,
+        )
+        return resp.json()["results"]
+
+    def get_ml_model(self, model_id: int) -> dict:
+        resp = self.send_request(
+            url=f"{self.host}/api/ml_models/{model_id}/",
+            method="get",
+            headers=self.headers,
+        )
+        return resp.json()
+
+    def get_ml_model_labels(self, model_id: int) -> Optional[BytesIO]:
+        resp = self.send_request(
+            url=f"{self.host}/api/ml_models/{model_id}/labels/",
+            method="get",
+            headers=self.headers,
+        )
+        return resp
+
+    def get_ml_model_file(self, model_id: int) -> Optional[BytesIO]:
+        resp = self.send_request(
+            url=f"{self.host}/api/ml_models/{model_id}/model/",
+            method="get",
+            headers=self.headers,
+        )
+        return resp
+
     def create_dataset(
         self,
         name: str,
         data_source: str,
         project_id: int,
         sensor_ids: list[int],
         type: str,
```

### Comparing `dataverse-sdk-0.1.2/dataverse_sdk/client.py` & `dataverse-sdk-0.1.3/dataverse_sdk/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from io import BytesIO
 from os.path import isfile
 from typing import Optional
 
 from pydantic import ValidationError
 
 from .apis.backend import BackendAPI
 from .connections import add_connection, get_connection
@@ -10,15 +11,23 @@
 from .schemas.api import (
     AttributeAPISchema,
     DatasetAPISchema,
     OntologyAPISchema,
     ProjectAPISchema,
     ProjectTagAPISchema,
 )
-from .schemas.client import Dataset, DataSource, Ontology, Project, ProjectTag, Sensor
+from .schemas.client import (
+    Dataset,
+    DataSource,
+    MLModel,
+    Ontology,
+    Project,
+    ProjectTag,
+    Sensor,
+)
 from .schemas.common import AnnotationFormat, DatasetType, OntologyImageType, SensorType
 from .utils.utils import get_filepaths
 
 
 class DataverseClient:
     def __init__(
         self,
@@ -233,14 +242,122 @@
 
         try:
             project_data: dict = self._api_client.get_project(project_id=project_id)
         except Exception as e:
             raise ClientConnectionError(f"Failed to get the project: {e}")
         return Project.create(project_data)
 
+    @staticmethod
+    def list_models(
+        project_id: int,
+        client: Optional["DataverseClient"] = None,
+    ) -> list:
+        """Get the model list by project id
+
+        Parameters
+        ----------
+        project_id : int
+        client : Optional["DataverseClient"], optional
+            clientclass, by default None
+
+        Returns
+        -------
+        list
+            model list from api response
+
+        Raises
+        ------
+        ClientConnectionError
+            raise exception if there is any error occurs when calling backend APIs.
+        """
+        if client is None:
+            client = DataverseClient.get_client()
+        api = client._api_client
+        try:
+            model_list: list = api.list_ml_models(project_id=project_id)
+        except Exception as e:
+            raise ClientConnectionError(f"Failed to get the models: {e}")
+        return model_list
+
+    @staticmethod
+    def get_model(
+        model_id: int,
+        client: Optional["DataverseClient"] = None,
+        project: Optional["Project"] = None,
+    ) -> MLModel:
+        """get the model detail by model id
+
+        Parameters
+        ----------
+        model_id : int
+        client : Optional["DataverseClient&quot"], optional
+            client class, by default None
+        project : Optional["Project"], optional
+            the project class, by default None
+
+        Returns
+        -------
+        MLModel
+            BaseModel for ml_model that store model information
+
+        Raises
+        ------
+        ClientConnectionError
+            raise exception if there is any error occurs when calling backend APIs.
+        """
+        if client is None:
+            client = DataverseClient.get_client()
+        api = client._api_client
+        try:
+            model_data: dict = api.get_ml_model(model_id=model_id)
+        except Exception as e:
+            raise ClientConnectionError(f"Failed to get the dataset: {e}")
+
+        target_class_id = {
+            ontology_class["id"] for ontology_class in model_data["classes"]
+        }
+        if project is None:
+            project = client.get_project(project_id=model_data["project"]["id"])
+        # get classes used in the model
+        classes = [
+            ontology_class
+            for ontology_class in project.ontology.classes
+            if ontology_class.id in target_class_id
+        ]
+        model_data.update({"id": model_id, "project": project, "classes": classes})
+        return MLModel(**model_data)
+
+    @staticmethod
+    def get_label_file(
+        model_id: int, client: Optional["DataverseClient"] = None
+    ) -> Optional[BytesIO]:
+        if client is None:
+            client = DataverseClient.get_client()
+        api = client._api_client
+        try:
+            labels: BytesIO = api.get_ml_model_labels(model_id=model_id)
+        except Exception as e:
+            raise ClientConnectionError(f"Failed to get model labels: {e}")
+        if labels:
+            return labels
+
+    @staticmethod
+    def get_triton_model_file(
+        model_id: int, client: Optional["DataverseClient"] = None
+    ) -> Optional[BytesIO]:
+        if client is None:
+            client = DataverseClient.get_client()
+        api = client._api_client
+        try:
+            model_file: BytesIO = api.get_ml_model_file(model_id=model_id)
+        except Exception as e:
+            raise ClientConnectionError(f"Failed to get triton model file: {e}")
+        if model_file:
+            return model_file
+
     def get_dataset(self, dataset_id: int):
         """Get dataset detail and status by id
 
         Parameters
         ----------
         dataset_id : int
             dataset-id in db
```

### Comparing `dataverse-sdk-0.1.2/dataverse_sdk/connections.py` & `dataverse-sdk-0.1.3/dataverse_sdk/connections.py`

 * *Files identical despite different names*

### Comparing `dataverse-sdk-0.1.2/dataverse_sdk/constants.py` & `dataverse-sdk-0.1.3/dataverse_sdk/constants.py`

 * *Files identical despite different names*

### Comparing `dataverse-sdk-0.1.2/dataverse_sdk/schemas/api.py` & `dataverse-sdk-0.1.3/dataverse_sdk/schemas/api.py`

 * *Files identical despite different names*

### Comparing `dataverse-sdk-0.1.2/dataverse_sdk/schemas/client.py` & `dataverse-sdk-0.1.3/dataverse_sdk/schemas/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -151,14 +151,26 @@
             description=project_data["description"],
             ego_car=project_data["ego_car"],
             ontology=ontology,
             sensors=sensors,
             project_tag=project_tag,
         )
 
+    def list_models(self) -> list:
+        from ..client import DataverseClient
+
+        model_list: list = DataverseClient.list_models(project_id=self.id)
+        return model_list
+
+    def get_model(self, model_id: int):
+        from ..client import DataverseClient
+
+        model_data = DataverseClient.get_model(model_id=model_id, project=self)
+        return model_data
+
     def create_dataset(
         self,
         name: str,
         data_source: DataSource,
         sensors: list[Sensor],
         type: DatasetType,
         annotation_format: AnnotationFormat,
@@ -265,7 +277,32 @@
     pcd_count: Optional[int] = None
     created_by: Optional[int] = None
     container_name: Optional[str] = None
     storage_url: Optional[str] = None
 
     class Config:
         extra = "allow"
+
+
+class MLModel(BaseModel):
+    id: Optional[int] = None
+    name: str
+    updated_at: str
+    project: Project
+    classes: list
+    triton_model_name: str
+    description: Optional[str] = None
+
+    class Config:
+        extra = "allow"
+
+    def get_label_file(self) -> dict:
+        from ..client import DataverseClient
+
+        labels: dict = DataverseClient.get_label_file(model_id=self.id)
+        return labels
+
+    def get_triton_model_file(self):
+        from ..client import DataverseClient
+
+        model_file = DataverseClient.get_triton_model_file(model_id=self.id)
+        return model_file
```

### Comparing `dataverse-sdk-0.1.2/dataverse_sdk/schemas/common.py` & `dataverse-sdk-0.1.3/dataverse_sdk/schemas/common.py`

 * *Files identical despite different names*

### Comparing `dataverse-sdk-0.1.2/dataverse_sdk.egg-info/PKG-INFO` & `dataverse-sdk-0.1.3/dataverse_sdk.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataverse-sdk
-Version: 0.1.2
+Version: 0.1.3
 Summary: Dataverse SDK For Python
 Home-page: 
 Author: LinkerVision
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
 
@@ -51,15 +51,15 @@
 The following sections provide examples for the most common DataVerse tasksm including:
 
 * [List Projects](#list-projects)
 * [Create Project](#create-project)
 * [Get Project](#get-project)
 * [Create Dataset](#create-dataset)
 * [Get Dataset](#get-dataset)
-
+* [List Models](#list-models)
 
 ### List Projects
 The `list_projects` method will list all projects of the given sites.
 
 
 ```Python
 projects = client.list_projects(current_user = True,
@@ -162,14 +162,38 @@
 
 The `get_dataset` method retrieves the dataset info from the connected site. The `id` parameter is the unique interger ID of the dataset, not its "name" property.
 
 ```Python
 dataset = client.get_dataset(id)
 ```
 
+### List Models
+The `list_models` method will list all the models in the given project
+
+```Python
+#1
+models = client.list_models(project_id = 1)
+#2
+project = client.get_project(project_id=1)
+models = project.list_models()
+```
+### Get Model
+The `get_model` method will get the model detail info by the given model-id
+
+```Python
+model = client.get_model(model_id=30)
+model = project.get_model(model_id=30)
+```
+From the given model, we could get the label file and the triton model file by the commands below.
+```Python
+model.get_label_file()
+model.get_triton_model_file()
+
+```
+
 
 ## Troubleshooting
 
 
 ## Next steps
```

### Comparing `dataverse-sdk-0.1.2/dataverse_sdk.egg-info/SOURCES.txt` & `dataverse-sdk-0.1.3/dataverse_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dataverse-sdk-0.1.2/setup.py` & `dataverse-sdk-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 AUTHOR = "LinkerVision"
 PACKAGE_NAME = "dataverse-sdk"
-PACKAGE_VERSION = "0.1.2"
+PACKAGE_VERSION = "0.1.3"
 DESC = "Dataverse SDK For Python"
 with open("README.md", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name=PACKAGE_NAME,
     version=PACKAGE_VERSION,
```

