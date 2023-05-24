# Comparing `tmp/bhousing-model-0.0.2.tar.gz` & `tmp/bhousing-model-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bhousing-model-0.0.2.tar", last modified: Wed May 24 11:04:20 2023, max compression
+gzip compressed data, was "bhousing-model-0.0.3.tar", last modified: Wed May 24 13:14:20 2023, max compression
```

## Comparing `bhousing-model-0.0.2.tar` & `bhousing-model-0.0.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 kompot    (1000) kompot    (1000)        0 2023-05-24 11:04:20.277482 bhousing-model-0.0.2/
--rwxrwxrwx   0 kompot    (1000) kompot    (1000)      409 2023-05-24 10:21:26.000000 bhousing-model-0.0.2/MANIFEST.in
--rw-r--r--   0 kompot    (1000) kompot    (1000)      805 2023-05-24 11:04:20.277482 bhousing-model-0.0.2/PKG-INFO
--rw-r--r--   0 kompot    (1000) kompot    (1000)       19 2023-05-23 17:50:18.000000 bhousing-model-0.0.2/README.md
-drwxr-xr-x   0 kompot    (1000) kompot    (1000)        0 2023-05-24 11:04:20.274148 bhousing-model-0.0.2/bhousing_model/
--rwxrwxrwx   0 kompot    (1000) kompot    (1000)        6 2023-05-24 10:48:29.000000 bhousing-model-0.0.2/bhousing_model/VERSION
--rwxrwxrwx   0 kompot    (1000) kompot    (1000)      856 2023-05-23 10:06:38.000000 bhousing-model-0.0.2/bhousing_model/__init__.py
-drwxr-xr-x   0 kompot    (1000) kompot    (1000)        0 2023-05-24 11:04:20.277482 bhousing-model-0.0.2/bhousing_model/config/
--rwxrwxrwx   0 kompot    (1000) kompot    (1000)        0 2023-03-29 15:52:47.000000 bhousing-model-0.0.2/bhousing_model/config/__init__.py
--rwxrwxrwx   0 kompot    (1000) kompot    (1000)     2062 2023-05-24 10:54:41.000000 bhousing-model-0.0.2/bhousing_model/config/core.py
--rwxrwxrwx   0 kompot    (1000) kompot    (1000)      360 2023-05-23 10:16:04.000000 bhousing-model-0.0.2/bhousing_model/config.yml
-drwxr-xr-x   0 kompot    (1000) kompot    (1000)        0 2023-05-24 11:04:20.277482 bhousing-model-0.0.2/bhousing_model/datasets/
--rw-r--r--   0 kompot    (1000) kompot    (1000)    41088 2023-05-23 07:16:27.000000 bhousing-model-0.0.2/bhousing_model/datasets/bhousing.csv
--rwxrwxrwx   0 kompot    (1000) kompot    (1000)      611 2023-05-23 17:10:44.000000 bhousing-model-0.0.2/bhousing_model/pipeline.py
--rwxrwxrwx   0 kompot    (1000) kompot    (1000)      925 2023-05-24 10:19:11.000000 bhousing-model-0.0.2/bhousing_model/predict.py
-drwxr-xr-x   0 kompot    (1000) kompot    (1000)        0 2023-05-24 11:04:20.277482 bhousing-model-0.0.2/bhousing_model/processing/
--rwxrwxrwx   0 kompot    (1000) kompot    (1000)        0 2023-03-29 15:52:47.000000 bhousing-model-0.0.2/bhousing_model/processing/__init__.py
--rwxrwxrwx   0 kompot    (1000) kompot    (1000)     1661 2023-05-23 08:24:07.000000 bhousing-model-0.0.2/bhousing_model/processing/data_manager.py
--rwxrwxrwx   0 kompot    (1000) kompot    (1000)     2036 2023-05-24 10:54:11.000000 bhousing-model-0.0.2/bhousing_model/processing/validation.py
--rwxrwxrwx   0 kompot    (1000) kompot    (1000)     2416 2023-05-24 10:50:53.000000 bhousing-model-0.0.2/bhousing_model/train_pipeline.py
-drwxr-xr-x   0 kompot    (1000) kompot    (1000)        0 2023-05-24 11:04:20.277482 bhousing-model-0.0.2/bhousing_model/trained_models/
--rw-r--r--   0 kompot    (1000) kompot    (1000)   328211 2023-05-24 11:02:15.000000 bhousing-model-0.0.2/bhousing_model/trained_models/bhousing_model_output_v0.0.2.pkl
-drwxr-xr-x   0 kompot    (1000) kompot    (1000)        0 2023-05-24 11:04:20.277482 bhousing-model-0.0.2/bhousing_model.egg-info/
--rwxrwxrwx   0 kompot    (1000) kompot    (1000)      805 2023-05-24 11:04:20.000000 bhousing-model-0.0.2/bhousing_model.egg-info/PKG-INFO
--rwxrwxrwx   0 kompot    (1000) kompot    (1000)      749 2023-05-24 11:04:20.000000 bhousing-model-0.0.2/bhousing_model.egg-info/SOURCES.txt
--rwxrwxrwx   0 kompot    (1000) kompot    (1000)        1 2023-05-24 11:04:20.000000 bhousing-model-0.0.2/bhousing_model.egg-info/dependency_links.txt
--rwxrwxrwx   0 kompot    (1000) kompot    (1000)      140 2023-05-24 11:04:20.000000 bhousing-model-0.0.2/bhousing_model.egg-info/requires.txt
--rwxrwxrwx   0 kompot    (1000) kompot    (1000)       15 2023-05-24 11:04:20.000000 bhousing-model-0.0.2/bhousing_model.egg-info/top_level.txt
--rwxrwxrwx   0 kompot    (1000) kompot    (1000)     2112 2023-05-23 11:01:34.000000 bhousing-model-0.0.2/pyproject.toml
-drwxr-xr-x   0 kompot    (1000) kompot    (1000)        0 2023-05-24 11:04:20.274148 bhousing-model-0.0.2/requirements/
--rwxrwxrwx   0 kompot    (1000) kompot    (1000)      502 2023-05-23 16:03:47.000000 bhousing-model-0.0.2/requirements/requirements.txt
--rwxrwxrwx   0 kompot    (1000) kompot    (1000)      154 2023-05-23 16:02:07.000000 bhousing-model-0.0.2/requirements/test_requirements.txt
--rw-r--r--   0 kompot    (1000) kompot    (1000)       38 2023-05-24 11:04:20.277482 bhousing-model-0.0.2/setup.cfg
--rwxrwxrwx   0 kompot    (1000) kompot    (1000)     2220 2023-05-23 11:05:28.000000 bhousing-model-0.0.2/setup.py
+drwxr-xr-x   0 kompot    (1000) kompot    (1000)        0 2023-05-24 13:14:20.310581 bhousing-model-0.0.3/
+-rwxrwxrwx   0 kompot    (1000) kompot    (1000)      409 2023-05-24 10:21:26.000000 bhousing-model-0.0.3/MANIFEST.in
+-rw-r--r--   0 kompot    (1000) kompot    (1000)      805 2023-05-24 13:14:20.310581 bhousing-model-0.0.3/PKG-INFO
+-rw-r--r--   0 kompot    (1000) kompot    (1000)     3976 2023-05-24 13:08:39.000000 bhousing-model-0.0.3/README.md
+drwxr-xr-x   0 kompot    (1000) kompot    (1000)        0 2023-05-24 13:14:20.307248 bhousing-model-0.0.3/bhousing_model/
+-rwxrwxrwx   0 kompot    (1000) kompot    (1000)        6 2023-05-24 13:12:10.000000 bhousing-model-0.0.3/bhousing_model/VERSION
+-rwxrwxrwx   0 kompot    (1000) kompot    (1000)      856 2023-05-23 10:06:38.000000 bhousing-model-0.0.3/bhousing_model/__init__.py
+drwxr-xr-x   0 kompot    (1000) kompot    (1000)        0 2023-05-24 13:14:20.307248 bhousing-model-0.0.3/bhousing_model/config/
+-rwxrwxrwx   0 kompot    (1000) kompot    (1000)        0 2023-03-29 15:52:47.000000 bhousing-model-0.0.3/bhousing_model/config/__init__.py
+-rwxrwxrwx   0 kompot    (1000) kompot    (1000)     2062 2023-05-24 10:54:41.000000 bhousing-model-0.0.3/bhousing_model/config/core.py
+-rwxrwxrwx   0 kompot    (1000) kompot    (1000)      360 2023-05-23 10:16:04.000000 bhousing-model-0.0.3/bhousing_model/config.yml
+drwxr-xr-x   0 kompot    (1000) kompot    (1000)        0 2023-05-24 13:14:20.310581 bhousing-model-0.0.3/bhousing_model/datasets/
+-rw-r--r--   0 kompot    (1000) kompot    (1000)    41088 2023-05-23 07:16:27.000000 bhousing-model-0.0.3/bhousing_model/datasets/bhousing.csv
+-rwxrwxrwx   0 kompot    (1000) kompot    (1000)      611 2023-05-23 17:10:44.000000 bhousing-model-0.0.3/bhousing_model/pipeline.py
+-rwxrwxrwx   0 kompot    (1000) kompot    (1000)      925 2023-05-24 10:19:11.000000 bhousing-model-0.0.3/bhousing_model/predict.py
+drwxr-xr-x   0 kompot    (1000) kompot    (1000)        0 2023-05-24 13:14:20.310581 bhousing-model-0.0.3/bhousing_model/processing/
+-rwxrwxrwx   0 kompot    (1000) kompot    (1000)        0 2023-03-29 15:52:47.000000 bhousing-model-0.0.3/bhousing_model/processing/__init__.py
+-rwxrwxrwx   0 kompot    (1000) kompot    (1000)     1661 2023-05-23 08:24:07.000000 bhousing-model-0.0.3/bhousing_model/processing/data_manager.py
+-rwxrwxrwx   0 kompot    (1000) kompot    (1000)     2061 2023-05-24 13:05:20.000000 bhousing-model-0.0.3/bhousing_model/processing/validation.py
+-rwxrwxrwx   0 kompot    (1000) kompot    (1000)     2416 2023-05-24 10:50:53.000000 bhousing-model-0.0.3/bhousing_model/train_pipeline.py
+drwxr-xr-x   0 kompot    (1000) kompot    (1000)        0 2023-05-24 13:14:20.310581 bhousing-model-0.0.3/bhousing_model/trained_models/
+-rw-r--r--   0 kompot    (1000) kompot    (1000)   328211 2023-05-24 11:02:15.000000 bhousing-model-0.0.3/bhousing_model/trained_models/bhousing_model_output_v0.0.2.pkl
+drwxr-xr-x   0 kompot    (1000) kompot    (1000)        0 2023-05-24 13:14:20.307248 bhousing-model-0.0.3/bhousing_model.egg-info/
+-rwxrwxrwx   0 kompot    (1000) kompot    (1000)      805 2023-05-24 13:14:20.000000 bhousing-model-0.0.3/bhousing_model.egg-info/PKG-INFO
+-rwxrwxrwx   0 kompot    (1000) kompot    (1000)      749 2023-05-24 13:14:20.000000 bhousing-model-0.0.3/bhousing_model.egg-info/SOURCES.txt
+-rwxrwxrwx   0 kompot    (1000) kompot    (1000)        1 2023-05-24 13:14:20.000000 bhousing-model-0.0.3/bhousing_model.egg-info/dependency_links.txt
+-rwxrwxrwx   0 kompot    (1000) kompot    (1000)      140 2023-05-24 13:14:20.000000 bhousing-model-0.0.3/bhousing_model.egg-info/requires.txt
+-rwxrwxrwx   0 kompot    (1000) kompot    (1000)       15 2023-05-24 13:14:20.000000 bhousing-model-0.0.3/bhousing_model.egg-info/top_level.txt
+-rwxrwxrwx   0 kompot    (1000) kompot    (1000)     2112 2023-05-23 11:01:34.000000 bhousing-model-0.0.3/pyproject.toml
+drwxr-xr-x   0 kompot    (1000) kompot    (1000)        0 2023-05-24 13:14:20.307248 bhousing-model-0.0.3/requirements/
+-rwxrwxrwx   0 kompot    (1000) kompot    (1000)      502 2023-05-23 16:03:47.000000 bhousing-model-0.0.3/requirements/requirements.txt
+-rwxrwxrwx   0 kompot    (1000) kompot    (1000)      154 2023-05-23 16:02:07.000000 bhousing-model-0.0.3/requirements/test_requirements.txt
+-rw-r--r--   0 kompot    (1000) kompot    (1000)       38 2023-05-24 13:14:20.310581 bhousing-model-0.0.3/setup.cfg
+-rwxrwxrwx   0 kompot    (1000) kompot    (1000)     2220 2023-05-23 11:05:28.000000 bhousing-model-0.0.3/setup.py
```

### Comparing `bhousing-model-0.0.2/PKG-INFO` & `bhousing-model-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bhousing-model
-Version: 0.0.2
+Version: 0.0.3
 Summary: Boston Housing model package.
 Home-page: https://github.com/iCosmos76/bhousing-package
 Author: Belous Vadim
 Author-email: belous.vadim@inbox.ru
 License: BSD-3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `bhousing-model-0.0.2/bhousing_model/__init__.py` & `bhousing-model-0.0.3/bhousing_model/__init__.py`

 * *Files identical despite different names*

### Comparing `bhousing-model-0.0.2/bhousing_model/config/core.py` & `bhousing-model-0.0.3/bhousing_model/config/core.py`

 * *Files identical despite different names*

### Comparing `bhousing-model-0.0.2/bhousing_model/datasets/bhousing.csv` & `bhousing-model-0.0.3/bhousing_model/datasets/bhousing.csv`

 * *Files identical despite different names*

### Comparing `bhousing-model-0.0.2/bhousing_model/pipeline.py` & `bhousing-model-0.0.3/bhousing_model/pipeline.py`

 * *Files identical despite different names*

### Comparing `bhousing-model-0.0.2/bhousing_model/predict.py` & `bhousing-model-0.0.3/bhousing_model/predict.py`

 * *Files identical despite different names*

### Comparing `bhousing-model-0.0.2/bhousing_model/processing/data_manager.py` & `bhousing-model-0.0.3/bhousing_model/processing/data_manager.py`

 * *Files identical despite different names*

### Comparing `bhousing-model-0.0.2/bhousing_model/processing/validation.py` & `bhousing-model-0.0.3/bhousing_model/processing/validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,14 +38,15 @@
         errors = error.json()
 
     return relevant_data, errors
 
 
 class BHousingInputSchema(BaseModel):
     ID: Optional[int]
+    CRIM Optional[float]
     ZN: Optional[float]
     INDUS: Optional[float]
     CHAS: Optional[float]
     NOX: Optional[float]
     RM: Optional[float]
     AGE: Optional[float]
     DIS: Optional[float]
```

### Comparing `bhousing-model-0.0.2/bhousing_model/train_pipeline.py` & `bhousing-model-0.0.3/bhousing_model/train_pipeline.py`

 * *Files identical despite different names*

### Comparing `bhousing-model-0.0.2/bhousing_model/trained_models/bhousing_model_output_v0.0.2.pkl` & `bhousing-model-0.0.3/bhousing_model/trained_models/bhousing_model_output_v0.0.2.pkl`

 * *Files identical despite different names*

### Comparing `bhousing-model-0.0.2/bhousing_model.egg-info/PKG-INFO` & `bhousing-model-0.0.3/bhousing_model.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bhousing-model
-Version: 0.0.2
+Version: 0.0.3
 Summary: Boston Housing model package.
 Home-page: https://github.com/iCosmos76/bhousing-package
 Author: Belous Vadim
 Author-email: belous.vadim@inbox.ru
 License: BSD-3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `bhousing-model-0.0.2/bhousing_model.egg-info/SOURCES.txt` & `bhousing-model-0.0.3/bhousing_model.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bhousing-model-0.0.2/pyproject.toml` & `bhousing-model-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bhousing-model-0.0.2/setup.py` & `bhousing-model-0.0.3/setup.py`

 * *Files identical despite different names*

