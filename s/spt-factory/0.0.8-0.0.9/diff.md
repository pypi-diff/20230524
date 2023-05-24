# Comparing `tmp/spt_factory-0.0.8.tar.gz` & `tmp/spt_factory-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spt_factory-0.0.8.tar", last modified: Sat Jul 16 11:42:55 2022, max compression
+gzip compressed data, was "spt_factory-0.0.9.tar", last modified: Sat Jul 16 16:30:54 2022, max compression
```

## Comparing `spt_factory-0.0.8.tar` & `spt_factory-0.0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 markporoshin   (501) staff       (20)        0 2022-07-16 11:42:55.772221 spt_factory-0.0.8/
--rw-r--r--   0 markporoshin   (501) staff       (20)      576 2022-07-16 11:42:55.771938 spt_factory-0.0.8/PKG-INFO
--rw-r--r--   0 markporoshin   (501) staff       (20)     2467 2022-07-15 16:39:11.000000 spt_factory-0.0.8/README.md
--rw-r--r--   0 markporoshin   (501) staff       (20)       38 2022-07-16 11:42:55.772320 spt_factory-0.0.8/setup.cfg
--rw-r--r--   0 markporoshin   (501) staff       (20)     1033 2022-07-16 11:42:53.000000 spt_factory-0.0.8/setup.py
-drwxr-xr-x   0 markporoshin   (501) staff       (20)        0 2022-07-16 11:42:55.764412 spt_factory-0.0.8/spt_factory/
--rw-r--r--   0 markporoshin   (501) staff       (20)       33 2022-07-16 11:30:36.000000 spt_factory-0.0.8/spt_factory/__init__.py
--rw-r--r--   0 markporoshin   (501) staff       (20)     2247 2022-07-15 16:35:15.000000 spt_factory-0.0.8/spt_factory/credentials.py
-drwxr-xr-x   0 markporoshin   (501) staff       (20)        0 2022-07-16 11:42:55.769048 spt_factory-0.0.8/spt_factory/datascience/
--rw-r--r--   0 markporoshin   (501) staff       (20)        0 2022-07-16 11:29:26.000000 spt_factory-0.0.8/spt_factory/datascience/__init__.py
--rw-r--r--   0 markporoshin   (501) staff       (20)     2002 2022-07-16 10:07:04.000000 spt_factory-0.0.8/spt_factory/datascience/model_manager.py
--rw-r--r--   0 markporoshin   (501) staff       (20)     1523 2022-07-16 10:07:04.000000 spt_factory-0.0.8/spt_factory/datascience/model_util.py
-drwxr-xr-x   0 markporoshin   (501) staff       (20)        0 2022-07-16 11:42:55.769881 spt_factory-0.0.8/spt_factory/datascience/models/
--rw-r--r--   0 markporoshin   (501) staff       (20)        0 2022-07-16 11:29:38.000000 spt_factory-0.0.8/spt_factory/datascience/models/__init__.py
--rw-r--r--   0 markporoshin   (501) staff       (20)     1598 2022-07-15 14:39:49.000000 spt_factory-0.0.8/spt_factory/datascience/models/base_model.py
--rw-r--r--   0 markporoshin   (501) staff       (20)     1284 2022-07-16 10:07:04.000000 spt_factory-0.0.8/spt_factory/datascience/models_storage.py
--rw-r--r--   0 markporoshin   (501) staff       (20)     2135 2022-07-16 10:07:04.000000 spt_factory-0.0.8/spt_factory/datascience/pipeline_manager.py
-drwxr-xr-x   0 markporoshin   (501) staff       (20)        0 2022-07-16 11:42:55.770729 spt_factory-0.0.8/spt_factory/datascience/pipelines/
--rw-r--r--   0 markporoshin   (501) staff       (20)        0 2022-07-16 11:29:38.000000 spt_factory-0.0.8/spt_factory/datascience/pipelines/__init__.py
--rw-r--r--   0 markporoshin   (501) staff       (20)     1723 2022-07-15 14:39:49.000000 spt_factory-0.0.8/spt_factory/datascience/pipelines/base_pipeline.py
--rw-r--r--   0 markporoshin   (501) staff       (20)      238 2022-07-15 17:01:17.000000 spt_factory-0.0.8/spt_factory/datascience/singleton.py
--rw-r--r--   0 markporoshin   (501) staff       (20)     2272 2022-07-15 20:05:06.000000 spt_factory-0.0.8/spt_factory/factory.py
--rw-r--r--   0 markporoshin   (501) staff       (20)     1961 2022-07-16 10:07:04.000000 spt_factory-0.0.8/spt_factory/resources.py
-drwxr-xr-x   0 markporoshin   (501) staff       (20)        0 2022-07-16 11:42:55.766436 spt_factory-0.0.8/spt_factory.egg-info/
--rw-r--r--   0 markporoshin   (501) staff       (20)      576 2022-07-16 11:42:55.000000 spt_factory-0.0.8/spt_factory.egg-info/PKG-INFO
--rw-r--r--   0 markporoshin   (501) staff       (20)      727 2022-07-16 11:42:55.000000 spt_factory-0.0.8/spt_factory.egg-info/SOURCES.txt
--rw-r--r--   0 markporoshin   (501) staff       (20)        1 2022-07-16 11:42:55.000000 spt_factory-0.0.8/spt_factory.egg-info/dependency_links.txt
--rw-r--r--   0 markporoshin   (501) staff       (20)       38 2022-07-16 11:42:55.000000 spt_factory-0.0.8/spt_factory.egg-info/requires.txt
--rw-r--r--   0 markporoshin   (501) staff       (20)       12 2022-07-16 11:42:55.000000 spt_factory-0.0.8/spt_factory.egg-info/top_level.txt
-drwxr-xr-x   0 markporoshin   (501) staff       (20)        0 2022-07-16 11:42:55.771313 spt_factory-0.0.8/test/
--rw-r--r--   0 markporoshin   (501) staff       (20)      795 2022-07-15 16:39:11.000000 spt_factory-0.0.8/test/test.py
+drwxr-xr-x   0 markporoshin   (501) staff       (20)        0 2022-07-16 16:30:54.654230 spt_factory-0.0.9/
+-rw-r--r--   0 markporoshin   (501) staff       (20)      576 2022-07-16 16:30:54.653706 spt_factory-0.0.9/PKG-INFO
+-rw-r--r--   0 markporoshin   (501) staff       (20)     2467 2022-07-15 16:39:11.000000 spt_factory-0.0.9/README.md
+-rw-r--r--   0 markporoshin   (501) staff       (20)       38 2022-07-16 16:30:54.654373 spt_factory-0.0.9/setup.cfg
+-rw-r--r--   0 markporoshin   (501) staff       (20)     1033 2022-07-16 16:26:35.000000 spt_factory-0.0.9/setup.py
+drwxr-xr-x   0 markporoshin   (501) staff       (20)        0 2022-07-16 16:30:54.647204 spt_factory-0.0.9/spt_factory/
+-rw-r--r--   0 markporoshin   (501) staff       (20)       33 2022-07-16 11:30:36.000000 spt_factory-0.0.9/spt_factory/__init__.py
+-rw-r--r--   0 markporoshin   (501) staff       (20)     2247 2022-07-15 16:35:15.000000 spt_factory-0.0.9/spt_factory/credentials.py
+drwxr-xr-x   0 markporoshin   (501) staff       (20)        0 2022-07-16 16:30:54.650968 spt_factory-0.0.9/spt_factory/datascience/
+-rw-r--r--   0 markporoshin   (501) staff       (20)        0 2022-07-16 11:29:26.000000 spt_factory-0.0.9/spt_factory/datascience/__init__.py
+-rw-r--r--   0 markporoshin   (501) staff       (20)     2606 2022-07-16 11:56:20.000000 spt_factory-0.0.9/spt_factory/datascience/model_manager.py
+-rw-r--r--   0 markporoshin   (501) staff       (20)     1523 2022-07-16 10:07:04.000000 spt_factory-0.0.9/spt_factory/datascience/model_util.py
+drwxr-xr-x   0 markporoshin   (501) staff       (20)        0 2022-07-16 16:30:54.651729 spt_factory-0.0.9/spt_factory/datascience/models/
+-rw-r--r--   0 markporoshin   (501) staff       (20)        0 2022-07-16 11:29:38.000000 spt_factory-0.0.9/spt_factory/datascience/models/__init__.py
+-rw-r--r--   0 markporoshin   (501) staff       (20)     1598 2022-07-15 14:39:49.000000 spt_factory-0.0.9/spt_factory/datascience/models/base_model.py
+-rw-r--r--   0 markporoshin   (501) staff       (20)     1583 2022-07-16 16:21:59.000000 spt_factory-0.0.9/spt_factory/datascience/models_storage.py
+-rw-r--r--   0 markporoshin   (501) staff       (20)     2135 2022-07-16 10:07:04.000000 spt_factory-0.0.9/spt_factory/datascience/pipeline_manager.py
+drwxr-xr-x   0 markporoshin   (501) staff       (20)        0 2022-07-16 16:30:54.652547 spt_factory-0.0.9/spt_factory/datascience/pipelines/
+-rw-r--r--   0 markporoshin   (501) staff       (20)        0 2022-07-16 11:29:38.000000 spt_factory-0.0.9/spt_factory/datascience/pipelines/__init__.py
+-rw-r--r--   0 markporoshin   (501) staff       (20)     1723 2022-07-15 14:39:49.000000 spt_factory-0.0.9/spt_factory/datascience/pipelines/base_pipeline.py
+-rw-r--r--   0 markporoshin   (501) staff       (20)      238 2022-07-15 17:01:17.000000 spt_factory-0.0.9/spt_factory/datascience/singleton.py
+-rw-r--r--   0 markporoshin   (501) staff       (20)     2272 2022-07-15 20:05:06.000000 spt_factory-0.0.9/spt_factory/factory.py
+-rw-r--r--   0 markporoshin   (501) staff       (20)     1961 2022-07-16 10:07:04.000000 spt_factory-0.0.9/spt_factory/resources.py
+drwxr-xr-x   0 markporoshin   (501) staff       (20)        0 2022-07-16 16:30:54.648688 spt_factory-0.0.9/spt_factory.egg-info/
+-rw-r--r--   0 markporoshin   (501) staff       (20)      576 2022-07-16 16:30:54.000000 spt_factory-0.0.9/spt_factory.egg-info/PKG-INFO
+-rw-r--r--   0 markporoshin   (501) staff       (20)      727 2022-07-16 16:30:54.000000 spt_factory-0.0.9/spt_factory.egg-info/SOURCES.txt
+-rw-r--r--   0 markporoshin   (501) staff       (20)        1 2022-07-16 16:30:54.000000 spt_factory-0.0.9/spt_factory.egg-info/dependency_links.txt
+-rw-r--r--   0 markporoshin   (501) staff       (20)       38 2022-07-16 16:30:54.000000 spt_factory-0.0.9/spt_factory.egg-info/requires.txt
+-rw-r--r--   0 markporoshin   (501) staff       (20)       12 2022-07-16 16:30:54.000000 spt_factory-0.0.9/spt_factory.egg-info/top_level.txt
+drwxr-xr-x   0 markporoshin   (501) staff       (20)        0 2022-07-16 16:30:54.653084 spt_factory-0.0.9/test/
+-rw-r--r--   0 markporoshin   (501) staff       (20)      815 2022-07-16 16:29:05.000000 spt_factory-0.0.9/test/test.py
```

### Comparing `spt_factory-0.0.8/PKG-INFO` & `spt_factory-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spt_factory
-Version: 0.0.8
+Version: 0.0.9
 Summary: SPT resource manager
 Home-page: UNKNOWN
 Author: Mark Poroshin
 Author-email: mporoshin@smartpredictiontech.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `spt_factory-0.0.8/README.md` & `spt_factory-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `spt_factory-0.0.8/setup.py` & `spt_factory-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 from setuptools import find_namespace_packages, setup, find_packages
 
 package_name = "spt_factory"
-package_version = "0.0.8"
+package_version = "0.0.9"
 description = """SPT resource manager"""
 
 setup(
     name=package_name,
     version=package_version,
     description=description,
     long_description=description,
```

### Comparing `spt_factory-0.0.8/spt_factory/credentials.py` & `spt_factory-0.0.9/spt_factory/credentials.py`

 * *Files identical despite different names*

### Comparing `spt_factory-0.0.8/spt_factory/datascience/model_manager.py` & `spt_factory-0.0.9/spt_factory/datascience/model_manager.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from abc import ABC, abstractmethod
 from hashlib import sha256
 
 from spt_factory.datascience.model_util import ModelUtil
-from spt_factory.datascience.models.base_model import BaseModel
+from spt_factory.datascience.models.base_model import BaseModel, ModelConfig
 from functools import lru_cache
 from spt_factory.datascience.singleton import Singleton
 from spt_factory.datascience.models_storage import MongoModelStorage
 
 
 class ModelManager(metaclass=Singleton):
     __slots__ = 'model_util', 'model_storage'
@@ -21,22 +21,39 @@
         Return model object by id
         :param model_id: id of the model
         :return:
         """
         pass
 
     @abstractmethod
-    def save_model(self, path,  model_config) -> str:
+    def save_model(self, path,  model) -> str:
         """
         Save model and return model id
         :param model: model inherit from BaseModel
         :return: model id
         """
         pass
 
+    @abstractmethod
+    def get_model_config(self, model_id) -> ModelConfig:
+        """
+        Return model object by id
+        :param model_id: id of the model
+        :return:
+        """
+        pass
+
+    @abstractmethod
+    def save_model_config(self, model_config):
+        """
+        Save model config
+        :param model: model inherit from BaseModel
+        """
+        pass
+
 
 class SPTModelManager(ModelManager):
 
     def __init__(self, model_util: ModelUtil, model_storage: MongoModelStorage):
         super().__init__(model_util, model_storage)
 
     @lru_cache(maxsize=512)
@@ -55,8 +72,14 @@
         self.model_util.save_model_config(model_config)
         return model_id
 
     def produce_model_id(self, model_name, model_version):
         return sha256(f"{model_name}-{model_version}".encode("utf-8")).hexdigest()
 
     def increment_model_version(self, version):
-        return version + 1
+        return version + 1
+
+    def get_model_config(self, model_id):
+        return self.model_storage.load_model_config(model_id)
+
+    def save_model_config(self, model_config):
+        self.model_util.save_model_config(model_config)
```

### Comparing `spt_factory-0.0.8/spt_factory/datascience/model_util.py` & `spt_factory-0.0.9/spt_factory/datascience/model_util.py`

 * *Files identical despite different names*

### Comparing `spt_factory-0.0.8/spt_factory/datascience/models/base_model.py` & `spt_factory-0.0.9/spt_factory/datascience/models/base_model.py`

 * *Files identical despite different names*

### Comparing `spt_factory-0.0.8/spt_factory/datascience/models_storage.py` & `spt_factory-0.0.9/spt_factory/datascience/models_storage.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,29 +11,38 @@
     def save_model(self, path, model, model_id, version: int):
         pass
 
     @abstractmethod
     def load_model(self, model_id):
         pass
 
+    @abstractmethod
+    def load_model_config(self, model_id):
+        pass
+
 
 class MongoModelStorage(ModelStorage, metaclass=Singleton):
 
     def __init__(self, spt):
         self.mongo_client = spt.get_mongo()
 
     def save_model(self, path, model, model_id, version: int):
         model_config = model.save_model(path, model_id, version)
         return model_config
 
-    def load_model_object(self, model_package, model_class, model_config):
+    def _load_model_object(self, model_package, model_class, model_config):
         module = import_module(model_package)
         return getattr(
             module, model_class
         ).load_model(model_config)
 
     def load_model(self, model_id):
         model_config_dict = self.mongo_client.spt.models.find_one({'id': model_id})
         model_config = ModelConfig.from_dict(model_config_dict)
         model_package = model_config.model_package
         model_class = model_config.model_class
-        return self.load_model_object(model_package, model_class, model_config)
+        return self._load_model_object(model_package, model_class, model_config)
+
+    def load_model_config(self, model_id):
+        model_config_dict = self.mongo_client.spt.models.find_one({'id': model_id})
+        model_config = ModelConfig.from_dict(model_config_dict)
+        return model_config
```

### Comparing `spt_factory-0.0.8/spt_factory/datascience/pipeline_manager.py` & `spt_factory-0.0.9/spt_factory/datascience/pipeline_manager.py`

 * *Files identical despite different names*

### Comparing `spt_factory-0.0.8/spt_factory/datascience/pipelines/base_pipeline.py` & `spt_factory-0.0.9/spt_factory/datascience/pipelines/base_pipeline.py`

 * *Files identical despite different names*

### Comparing `spt_factory-0.0.8/spt_factory/factory.py` & `spt_factory-0.0.9/spt_factory/factory.py`

 * *Files identical despite different names*

### Comparing `spt_factory-0.0.8/spt_factory/resources.py` & `spt_factory-0.0.9/spt_factory/resources.py`

 * *Files identical despite different names*

### Comparing `spt_factory-0.0.8/spt_factory.egg-info/PKG-INFO` & `spt_factory-0.0.9/spt_factory.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spt-factory
-Version: 0.0.8
+Version: 0.0.9
 Summary: SPT resource manager
 Home-page: UNKNOWN
 Author: Mark Poroshin
 Author-email: mporoshin@smartpredictiontech.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `spt_factory-0.0.8/spt_factory.egg-info/SOURCES.txt` & `spt_factory-0.0.9/spt_factory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

