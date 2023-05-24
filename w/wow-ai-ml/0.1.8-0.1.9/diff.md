# Comparing `tmp/wow_ai_ml-0.1.8.tar.gz` & `tmp/wow_ai_ml-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wow_ai_ml-0.1.8.tar", max compression
+gzip compressed data, was "wow_ai_ml-0.1.9.tar", max compression
```

## Comparing `wow_ai_ml-0.1.8.tar` & `wow_ai_ml-0.1.9.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0     6415 2023-02-14 16:37:26.303084 wow_ai_ml-0.1.8/README.md
--rw-r--r--   0        0        0      261 2023-05-05 03:06:30.546821 wow_ai_ml-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-01-30 05:04:46.921613 wow_ai_ml-0.1.8/wow_ai_ml/__init__.py
--rw-r--r--   0        0        0     7256 2023-03-30 07:20:26.331095 wow_ai_ml-0.1.8/wow_ai_ml/api.py
--rw-r--r--   0        0        0      267 2023-01-29 17:47:59.351874 wow_ai_ml-0.1.8/wow_ai_ml/default_configs/Dockerfile
--rw-r--r--   0        0        0     2701 2023-01-29 17:47:59.457372 wow_ai_ml-0.1.8/wow_ai_ml/default_configs/README.md
--rw-r--r--   0        0        0     3861 2023-01-29 17:47:57.963857 wow_ai_ml-0.1.8/wow_ai_ml/default_configs/_wsgi.py.tmpl
--rw-r--r--   0        0        0      563 2023-01-29 17:47:59.127706 wow_ai_ml-0.1.8/wow_ai_ml/default_configs/docker-compose.yml
--rw-r--r--   0        0        0       28 2023-01-29 17:47:59.904560 wow_ai_ml-0.1.8/wow_ai_ml/default_configs/requirements.txt
--rw-r--r--   0        0        0     1899 2023-01-29 17:47:56.017679 wow_ai_ml-0.1.8/wow_ai_ml/exceptions.py
--rw-r--r--   0        0        0     2375 2023-01-29 17:48:02.301568 wow_ai_ml-0.1.8/wow_ai_ml/helpers.py
--rw-r--r--   0        0        0    32225 2023-02-14 02:02:44.826340 wow_ai_ml-0.1.8/wow_ai_ml/model.py
--rw-r--r--   0        0        0     7542 2023-01-29 17:48:02.879893 wow_ai_ml-0.1.8/wow_ai_ml/server.py
--rw-r--r--   0        0        0        6 2023-02-01 14:28:47.129345 wow_ai_ml-0.1.8/wow_ai_ml/templates/preview.html
--rw-r--r--   0        0        0     1999 2023-01-29 17:48:03.663323 wow_ai_ml-0.1.8/wow_ai_ml/utils.py
--rw-r--r--   0        0        0     7119 1970-01-01 00:00:00.000000 wow_ai_ml-0.1.8/setup.py
--rw-r--r--   0        0        0     6846 1970-01-01 00:00:00.000000 wow_ai_ml-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     6415 2023-02-14 16:37:26.303084 wow_ai_ml-0.1.9/README.md
+-rw-r--r--   0        0        0      261 2023-05-24 08:27:19.222976 wow_ai_ml-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-01-30 05:04:46.921613 wow_ai_ml-0.1.9/wow_ai_ml/__init__.py
+-rw-r--r--   0        0        0     7256 2023-03-30 07:20:26.331095 wow_ai_ml-0.1.9/wow_ai_ml/api.py
+-rw-r--r--   0        0        0      267 2023-01-29 17:47:59.351874 wow_ai_ml-0.1.9/wow_ai_ml/default_configs/Dockerfile
+-rw-r--r--   0        0        0     2701 2023-01-29 17:47:59.457372 wow_ai_ml-0.1.9/wow_ai_ml/default_configs/README.md
+-rw-r--r--   0        0        0     3861 2023-01-29 17:47:57.963857 wow_ai_ml-0.1.9/wow_ai_ml/default_configs/_wsgi.py.tmpl
+-rw-r--r--   0        0        0      563 2023-01-29 17:47:59.127706 wow_ai_ml-0.1.9/wow_ai_ml/default_configs/docker-compose.yml
+-rw-r--r--   0        0        0       28 2023-01-29 17:47:59.904560 wow_ai_ml-0.1.9/wow_ai_ml/default_configs/requirements.txt
+-rw-r--r--   0        0        0     1899 2023-01-29 17:47:56.017679 wow_ai_ml-0.1.9/wow_ai_ml/exceptions.py
+-rw-r--r--   0        0        0     2375 2023-01-29 17:48:02.301568 wow_ai_ml-0.1.9/wow_ai_ml/helpers.py
+-rw-r--r--   0        0        0    32225 2023-02-14 02:02:44.826340 wow_ai_ml-0.1.9/wow_ai_ml/model.py
+-rw-r--r--   0        0        0     7542 2023-01-29 17:48:02.879893 wow_ai_ml-0.1.9/wow_ai_ml/server.py
+-rw-r--r--   0        0        0        6 2023-02-01 14:28:47.129345 wow_ai_ml-0.1.9/wow_ai_ml/templates/preview.html
+-rw-r--r--   0        0        0     1999 2023-01-29 17:48:03.663323 wow_ai_ml-0.1.9/wow_ai_ml/utils.py
+-rw-r--r--   0        0        0     6846 1970-01-01 00:00:00.000000 wow_ai_ml-0.1.9/PKG-INFO
```

### Comparing `wow_ai_ml-0.1.8/README.md` & `wow_ai_ml-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.1.8/wow_ai_ml/api.py` & `wow_ai_ml-0.1.9/wow_ai_ml/api.py`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.1.8/wow_ai_ml/default_configs/README.md` & `wow_ai_ml-0.1.9/wow_ai_ml/default_configs/README.md`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.1.8/wow_ai_ml/default_configs/_wsgi.py.tmpl` & `wow_ai_ml-0.1.9/wow_ai_ml/default_configs/_wsgi.py.tmpl`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.1.8/wow_ai_ml/default_configs/docker-compose.yml` & `wow_ai_ml-0.1.9/wow_ai_ml/default_configs/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.1.8/wow_ai_ml/exceptions.py` & `wow_ai_ml-0.1.9/wow_ai_ml/exceptions.py`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.1.8/wow_ai_ml/helpers.py` & `wow_ai_ml-0.1.9/wow_ai_ml/helpers.py`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.1.8/wow_ai_ml/model.py` & `wow_ai_ml-0.1.9/wow_ai_ml/model.py`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.1.8/wow_ai_ml/server.py` & `wow_ai_ml-0.1.9/wow_ai_ml/server.py`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.1.8/wow_ai_ml/utils.py` & `wow_ai_ml-0.1.9/wow_ai_ml/utils.py`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.1.8/setup.py` & `wow_ai_ml-0.1.9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,136 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: wow-ai-ml
+Version: 0.1.9
+Summary: 
+Author: TonyShark
+Author-email: quoi@wow-ai.inc
+Requires-Python: >=3.8,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
 
-packages = \
-['wow_ai_ml']
+Project description
+What is the WOW AI ML backend?
+The WOW AI ML backend is an SDK that lets you wrap your machine learning code and turn it into a web server. You can then connect that server to a WOW AI instance to perform 2 tasks:
+Dynamically pre-annotate data based on model inference results
+Retrain or fine-tune a model based on recently annotated data
+If you just need to load static pre-annotated data into WOW AI, running an ML backend might be overkill for you. Instead, you can import preannotated data.
+How it works
+Get your model code
+Wrap it with the WOW AI SDK
+Create a running server script
+Launch the script
+Connect WOW AI to ML backend on the UI
+Quickstart
+Follow this example tutorial to run an ML backend with a simple text classifier:
+Clone the repo
+git clone https://github.com/wowai-3/wow-ai-ml-backend  
 
-package_data = \
-{'': ['*'], 'wow_ai_ml': ['default_configs/*', 'templates/*']}
 
-setup_kwargs = {
-    'name': 'wow-ai-ml',
-    'version': '0.1.8',
-    'description': '',
-    'long_description': 'Project description\nWhat is the WOW AI ML backend?\nThe WOW AI ML backend is an SDK that lets you wrap your machine learning code and turn it into a web server. You can then connect that server to a WOW AI instance to perform 2 tasks:\nDynamically pre-annotate data based on model inference results\nRetrain or fine-tune a model based on recently annotated data\nIf you just need to load static pre-annotated data into WOW AI, running an ML backend might be overkill for you. Instead, you can import preannotated data.\nHow it works\nGet your model code\nWrap it with the WOW AI SDK\nCreate a running server script\nLaunch the script\nConnect WOW AI to ML backend on the UI\nQuickstart\nFollow this example tutorial to run an ML backend with a simple text classifier:\nClone the repo\ngit clone https://github.com/wowai-3/wow-ai-ml-backend  \n\n\nSetup environment\nIt is highly recommended to use venv, virtualenv or conda python environments. You can use the same environment as WOW AI does. Read more about creating virtual environments via venv.\ncd wow-ai-ml-backend\n\n# Install wow-ai-ml and its dependencies\npip install -U -e .\n\n# Install example dependencies\npip install -r wow_ai_ml/examples/requirements.txt\n\n\nInitialize an ML backend based on an example script:\nwow-ai-ml init my_ml_backend --script wow_ai_ml/examples/text_classifier/text_classifier.py\n\nThis ML backend is an example provided by WOW AI. See how to create your own ML backend.\nStart ML backend server\nwow-ai-ml start my_ml_backend\n\n\nStart WOW AI and connect it to the running ML backend on the project settings page.\nCreate your own ML backend\nFollow this tutorial to wrap existing machine learning model code with the WOW AI ML SDK to use it as an ML backend with WOW AI.\nBefore you start, determine the following:\nThe expected inputs and outputs for your model. In other words, the type of labeling that your model supports in WOW AI, which informs the WOW AI labeling config. For example, text classification labels of "Dog", "Cat", or "Opossum" could be possible inputs and outputs.\nThe prediction format returned by your ML backend server.\nThis example tutorial outlines how to wrap a simple text classifier based on the scikit-learn framework with the WOW AI ML SDK.\nStart by creating a class declaration. You can create a WOW AI-compatible ML backend server in one command by inheriting it from LabelStudioMLBase.\nfrom wow_ai_ml.model import LabelStudioMLBase\n\nclass MyModel(WOWAIML):\n\n\nThen, define loaders & initializers in the __init__ method.\ndef __init__(self, **kwargs):\n    # don\'t forget to initialize base class...\n    super(MyModel, self).__init__(**kwargs)\n    self.model = self.load_my_model()\n\n\nThere are special variables provided by the inherited class:\nself.parsed_label_config is a Python dict that provides a WOW AI project config structure. See ref for details. Use might want to use this to align your model input/output with WOW AI labeling configuration;\nself.label_config is a raw labeling config string;\nself.train_output is a Python dict with the results of the previous model training runs (the output of the fit() method described bellow) Use this if you want to load the model for the next updates for active learning and model fine-tuning.\nAfter you define the loaders, you can define two methods for your model: an inference call and a training call.\nInference call\nUse an inference call to get pre-annotations from your model on-the-fly. You must update the existing predict method in the example ML backend scripts to make them work for your specific use case. Write your own code to override the predict(tasks, **kwargs) method, which takes JSON-formatted WOW AI tasks and returns predictions in the format accepted by WOW AI.\nExample\ndef predict(self, tasks, **kwargs):\n    predictions = []\n    # Get annotation tag first, and extract from_name/to_name keys from the labeling config to make predictions\n    from_name, schema = list(self.parsed_label_config.items())[0]\n    to_name = schema[\'to_name\'][0]\n    for task in tasks:\n        # for each task, return classification results in the form of "choices" pre-annotations\n        predictions.append({\n            \'result\': [{\n                \'from_name\': from_name,\n                \'to_name\': to_name,\n                \'type\': \'choices\',\n                \'value\': {\'choices\': [\'My Label\']}\n            }],\n            # optionally you can include prediction scores that you can use to sort the tasks and do active learning\n            \'score\': 0.987\n        })\n    return predictions\n\n\nTraining call\nUse the training call to update your model with new annotations. You don\'t need to use this call in your code, for example if you just want to pre-annotate tasks without retraining the model. If you do want to retrain the model based on annotations from WOW AI, use this method.\nWrite your own code to override the fit(annotations, **kwargs) method, which takes JSON-formatted WOW AI annotations and returns an arbitrary dict where some information about the created model can be stored.\nExample\ndef fit(self, completions, workdir=None, **kwargs):\n    # ... do some heavy computations, get your model and store checkpoints and resources\n    return {\'checkpoints\': \'my/model/checkpoints\'}  # <-- you can retrieve this dict as self.train_output in the subsequent calls\n\n\nAfter you wrap your model code with the class, define the loaders, and define the methods, you\'re ready to run your model as an ML backend with WOW AI.\nFor other examples of ML backends, refer to the examples in this repository. These examples aren\'t production-ready, but can help you set up your own code as a WOW AI ML backend.\nDeploy your ML backend to GCP\nBefore you start:\nInstall gcloud\nInit billing for account if it\'s not activated\nInit gcloud, type the following commands and login in browser:\ngcloud auth login\n\n\nActivate your Cloud Build API\nFind your GCP project ID\n(Optional) Add GCP_REGION with your default region to your ENV variables\nTo start deployment:\nCreate your own ML backend\nStart deployment to GCP:\nwow-ai-ml deploy gcp {ml-backend-local-dir} \\\n--from={model-python-script} \\\n--gcp-project-id {gcp-project-id} \\\n--wow-ai-host {https://tool.wowdao.ai} \\\n--wow-ai-api-key {YOUR-wow-ai-API-KEY}\n\n\nAfter WOW AI deploys the model - you will get model endpoint in console.\n\ntwine upload -u \'huonghx\' -p \'y@9^xwWA+!TzmY)\' --repository-url https://upload.pypi.org/legacy/ dist/*\n\n',
-    'author': 'TonyShark',
-    'author_email': 'quoi@wow-ai.inc',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'python_requires': '>=3.8,<4.0',
-}
+Setup environment
+It is highly recommended to use venv, virtualenv or conda python environments. You can use the same environment as WOW AI does. Read more about creating virtual environments via venv.
+cd wow-ai-ml-backend
+
+# Install wow-ai-ml and its dependencies
+pip install -U -e .
+
+# Install example dependencies
+pip install -r wow_ai_ml/examples/requirements.txt
+
+
+Initialize an ML backend based on an example script:
+wow-ai-ml init my_ml_backend --script wow_ai_ml/examples/text_classifier/text_classifier.py
+
+This ML backend is an example provided by WOW AI. See how to create your own ML backend.
+Start ML backend server
+wow-ai-ml start my_ml_backend
+
+
+Start WOW AI and connect it to the running ML backend on the project settings page.
+Create your own ML backend
+Follow this tutorial to wrap existing machine learning model code with the WOW AI ML SDK to use it as an ML backend with WOW AI.
+Before you start, determine the following:
+The expected inputs and outputs for your model. In other words, the type of labeling that your model supports in WOW AI, which informs the WOW AI labeling config. For example, text classification labels of "Dog", "Cat", or "Opossum" could be possible inputs and outputs.
+The prediction format returned by your ML backend server.
+This example tutorial outlines how to wrap a simple text classifier based on the scikit-learn framework with the WOW AI ML SDK.
+Start by creating a class declaration. You can create a WOW AI-compatible ML backend server in one command by inheriting it from LabelStudioMLBase.
+from wow_ai_ml.model import LabelStudioMLBase
+
+class MyModel(WOWAIML):
+
+
+Then, define loaders & initializers in the __init__ method.
+def __init__(self, **kwargs):
+    # don't forget to initialize base class...
+    super(MyModel, self).__init__(**kwargs)
+    self.model = self.load_my_model()
+
+
+There are special variables provided by the inherited class:
+self.parsed_label_config is a Python dict that provides a WOW AI project config structure. See ref for details. Use might want to use this to align your model input/output with WOW AI labeling configuration;
+self.label_config is a raw labeling config string;
+self.train_output is a Python dict with the results of the previous model training runs (the output of the fit() method described bellow) Use this if you want to load the model for the next updates for active learning and model fine-tuning.
+After you define the loaders, you can define two methods for your model: an inference call and a training call.
+Inference call
+Use an inference call to get pre-annotations from your model on-the-fly. You must update the existing predict method in the example ML backend scripts to make them work for your specific use case. Write your own code to override the predict(tasks, **kwargs) method, which takes JSON-formatted WOW AI tasks and returns predictions in the format accepted by WOW AI.
+Example
+def predict(self, tasks, **kwargs):
+    predictions = []
+    # Get annotation tag first, and extract from_name/to_name keys from the labeling config to make predictions
+    from_name, schema = list(self.parsed_label_config.items())[0]
+    to_name = schema['to_name'][0]
+    for task in tasks:
+        # for each task, return classification results in the form of "choices" pre-annotations
+        predictions.append({
+            'result': [{
+                'from_name': from_name,
+                'to_name': to_name,
+                'type': 'choices',
+                'value': {'choices': ['My Label']}
+            }],
+            # optionally you can include prediction scores that you can use to sort the tasks and do active learning
+            'score': 0.987
+        })
+    return predictions
+
+
+Training call
+Use the training call to update your model with new annotations. You don't need to use this call in your code, for example if you just want to pre-annotate tasks without retraining the model. If you do want to retrain the model based on annotations from WOW AI, use this method.
+Write your own code to override the fit(annotations, **kwargs) method, which takes JSON-formatted WOW AI annotations and returns an arbitrary dict where some information about the created model can be stored.
+Example
+def fit(self, completions, workdir=None, **kwargs):
+    # ... do some heavy computations, get your model and store checkpoints and resources
+    return {'checkpoints': 'my/model/checkpoints'}  # <-- you can retrieve this dict as self.train_output in the subsequent calls
+
+
+After you wrap your model code with the class, define the loaders, and define the methods, you're ready to run your model as an ML backend with WOW AI.
+For other examples of ML backends, refer to the examples in this repository. These examples aren't production-ready, but can help you set up your own code as a WOW AI ML backend.
+Deploy your ML backend to GCP
+Before you start:
+Install gcloud
+Init billing for account if it's not activated
+Init gcloud, type the following commands and login in browser:
+gcloud auth login
+
+
+Activate your Cloud Build API
+Find your GCP project ID
+(Optional) Add GCP_REGION with your default region to your ENV variables
+To start deployment:
+Create your own ML backend
+Start deployment to GCP:
+wow-ai-ml deploy gcp {ml-backend-local-dir} \
+--from={model-python-script} \
+--gcp-project-id {gcp-project-id} \
+--wow-ai-host {https://tool.wowdao.ai} \
+--wow-ai-api-key {YOUR-wow-ai-API-KEY}
+
+
+After WOW AI deploys the model - you will get model endpoint in console.
+
+twine upload -u 'huonghx' -p 'y@9^xwWA+!TzmY)' --repository-url https://upload.pypi.org/legacy/ dist/*
 
 
-setup(**setup_kwargs)
```

