# Comparing `tmp/fedops-0.2.0.tar.gz` & `tmp/fedops-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedops-0.2.0.tar", last modified: Tue May 23 06:11:38 2023, max compression
+gzip compressed data, was "fedops-0.2.1.tar", last modified: Wed May 24 08:01:18 2023, max compression
```

## Comparing `fedops-0.2.0.tar` & `fedops-0.2.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 06:11:38.043498 fedops-0.2.0/
--rw-r--r--   0 yangsemo   (501) staff       (20)      647 2023-05-23 06:11:38.043364 fedops-0.2.0/PKG-INFO
-drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 06:11:38.039616 fedops-0.2.0/fedops/
--rw-r--r--   0 yangsemo   (501) staff       (20)      872 2023-05-23 04:42:21.000000 fedops-0.2.0/fedops/__init__.py
-drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 06:11:38.042131 fedops-0.2.0/fedops/client/
--rw-r--r--   0 yangsemo   (501) staff       (20)      987 2023-05-23 04:42:21.000000 fedops-0.2.0/fedops/client/__init__.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     6957 2023-05-23 05:45:41.000000 fedops-0.2.0/fedops/client/app.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     5010 2023-05-22 17:11:45.000000 fedops-0.2.0/fedops/client/app_test.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     2817 2023-05-23 04:42:21.000000 fedops-0.2.0/fedops/client/client_api.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     6088 2023-05-23 04:42:21.000000 fedops-0.2.0/fedops/client/client_fl.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     3478 2023-05-23 04:42:21.000000 fedops-0.2.0/fedops/client/client_utils.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     2561 2023-05-23 06:06:12.000000 fedops-0.2.0/fedops/client/client_wandb.py
--rw-r--r--   0 yangsemo   (501) staff       (20)        0 2023-05-22 17:11:45.000000 fedops-0.2.0/fedops/client/test.py
-drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 06:11:38.042847 fedops-0.2.0/fedops/server/
--rw-r--r--   0 yangsemo   (501) staff       (20)      977 2023-05-23 04:42:21.000000 fedops-0.2.0/fedops/server/__init__.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     8963 2023-05-23 05:44:14.000000 fedops-0.2.0/fedops/server/app.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     1283 2023-05-22 17:11:45.000000 fedops-0.2.0/fedops/server/server_api.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     3229 2023-05-23 04:42:21.000000 fedops-0.2.0/fedops/server/server_utils.py
-drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 06:11:38.043063 fedops-0.2.0/fedops/utils/
--rw-r--r--   0 yangsemo   (501) staff       (20)        0 2023-05-22 17:11:45.000000 fedops-0.2.0/fedops/utils/__init__.py
--rw-r--r--   0 yangsemo   (501) staff       (20)      832 2023-05-22 17:11:45.000000 fedops-0.2.0/fedops/utils/version.py
-drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 06:11:38.040551 fedops-0.2.0/fedops.egg-info/
--rw-r--r--   0 yangsemo   (501) staff       (20)      647 2023-05-23 06:11:38.000000 fedops-0.2.0/fedops.egg-info/PKG-INFO
--rw-r--r--   0 yangsemo   (501) staff       (20)      540 2023-05-23 06:11:38.000000 fedops-0.2.0/fedops.egg-info/SOURCES.txt
--rw-r--r--   0 yangsemo   (501) staff       (20)        1 2023-05-23 06:11:38.000000 fedops-0.2.0/fedops.egg-info/dependency_links.txt
--rw-r--r--   0 yangsemo   (501) staff       (20)      187 2023-05-23 06:11:38.000000 fedops-0.2.0/fedops.egg-info/requires.txt
--rw-r--r--   0 yangsemo   (501) staff       (20)        7 2023-05-23 06:11:38.000000 fedops-0.2.0/fedops.egg-info/top_level.txt
--rw-r--r--   0 yangsemo   (501) staff       (20)       38 2023-05-23 06:11:38.043537 fedops-0.2.0/setup.cfg
--rw-r--r--   0 yangsemo   (501) staff       (20)     1130 2023-05-23 06:11:24.000000 fedops-0.2.0/setup.py
+drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-24 08:01:18.552314 fedops-0.2.1/
+-rw-r--r--   0 yangsemo   (501) staff       (20)      647 2023-05-24 08:01:18.552169 fedops-0.2.1/PKG-INFO
+drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-24 08:01:18.548921 fedops-0.2.1/fedops/
+-rw-r--r--   0 yangsemo   (501) staff       (20)      872 2023-05-23 04:42:21.000000 fedops-0.2.1/fedops/__init__.py
+drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-24 08:01:18.551071 fedops-0.2.1/fedops/client/
+-rw-r--r--   0 yangsemo   (501) staff       (20)      987 2023-05-23 04:42:21.000000 fedops-0.2.1/fedops/client/__init__.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     6951 2023-05-24 08:00:46.000000 fedops-0.2.1/fedops/client/app.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     5010 2023-05-22 17:11:45.000000 fedops-0.2.1/fedops/client/app_test.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     2817 2023-05-23 04:42:21.000000 fedops-0.2.1/fedops/client/client_api.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     6088 2023-05-23 04:42:21.000000 fedops-0.2.1/fedops/client/client_fl.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     3478 2023-05-23 04:42:21.000000 fedops-0.2.1/fedops/client/client_utils.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     2561 2023-05-23 06:06:12.000000 fedops-0.2.1/fedops/client/client_wandb.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)        0 2023-05-22 17:11:45.000000 fedops-0.2.1/fedops/client/test.py
+drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-24 08:01:18.551704 fedops-0.2.1/fedops/server/
+-rw-r--r--   0 yangsemo   (501) staff       (20)      977 2023-05-23 04:42:21.000000 fedops-0.2.1/fedops/server/__init__.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     8963 2023-05-23 05:44:14.000000 fedops-0.2.1/fedops/server/app.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     1283 2023-05-22 17:11:45.000000 fedops-0.2.1/fedops/server/server_api.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     3229 2023-05-23 04:42:21.000000 fedops-0.2.1/fedops/server/server_utils.py
+drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-24 08:01:18.551917 fedops-0.2.1/fedops/utils/
+-rw-r--r--   0 yangsemo   (501) staff       (20)        0 2023-05-22 17:11:45.000000 fedops-0.2.1/fedops/utils/__init__.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)      832 2023-05-22 17:11:45.000000 fedops-0.2.1/fedops/utils/version.py
+drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-24 08:01:18.549629 fedops-0.2.1/fedops.egg-info/
+-rw-r--r--   0 yangsemo   (501) staff       (20)      647 2023-05-24 08:01:18.000000 fedops-0.2.1/fedops.egg-info/PKG-INFO
+-rw-r--r--   0 yangsemo   (501) staff       (20)      540 2023-05-24 08:01:18.000000 fedops-0.2.1/fedops.egg-info/SOURCES.txt
+-rw-r--r--   0 yangsemo   (501) staff       (20)        1 2023-05-24 08:01:18.000000 fedops-0.2.1/fedops.egg-info/dependency_links.txt
+-rw-r--r--   0 yangsemo   (501) staff       (20)      187 2023-05-24 08:01:18.000000 fedops-0.2.1/fedops.egg-info/requires.txt
+-rw-r--r--   0 yangsemo   (501) staff       (20)        7 2023-05-24 08:01:18.000000 fedops-0.2.1/fedops.egg-info/top_level.txt
+-rw-r--r--   0 yangsemo   (501) staff       (20)       38 2023-05-24 08:01:18.552355 fedops-0.2.1/setup.cfg
+-rw-r--r--   0 yangsemo   (501) staff       (20)     1130 2023-05-24 08:00:51.000000 fedops-0.2.1/setup.py
```

### Comparing `fedops-0.2.0/PKG-INFO` & `fedops-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedops
-Version: 0.2.0
+Version: 0.2.1
 Summary: FL Lifecycle Operations Management Platform
 Home-page: https://github.com/gachon-CCLab/FedOps.git
 Author: Semo Yang
 Author-email: tpah20@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fedops-0.2.0/fedops/__init__.py` & `fedops-0.2.1/fedops/__init__.py`

 * *Files identical despite different names*

### Comparing `fedops-0.2.0/fedops/client/__init__.py` & `fedops-0.2.1/fedops/client/__init__.py`

 * *Files identical despite different names*

### Comparing `fedops-0.2.0/fedops/client/app.py` & `fedops-0.2.1/fedops/client/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         wandb_name = f"client-v{self.status.FL_next_gl_model}({datetime.now()})"
         # Login and init wandb project
         wandb_run = client_wandb.start_wandb(self.wandb_key, self.task_id, wandb_name)
 
         try:
             # Update wandb config
             wandb_config = {"learning_rate": self.model.optimizer.learning_rate.numpy(),
-                            "optimizer": self.model.optimizer._name,
+                            "optimizer": self.model.optimizer,
                             "dataset": self.dataset, "model_architecture": self.model_name}
             wandb_run.config.update(wandb_config, allow_val_change=True)
 
             # Check data fl client data status in the wandb
             label_values = [[i, self.y_label_counter[i]] for i in range(self.label_count)]
             client_wandb.data_status_wandb(wandb_run, label_values)
```

### Comparing `fedops-0.2.0/fedops/client/app_test.py` & `fedops-0.2.1/fedops/client/app_test.py`

 * *Files identical despite different names*

### Comparing `fedops-0.2.0/fedops/client/client_api.py` & `fedops-0.2.1/fedops/client/client_api.py`

 * *Files identical despite different names*

### Comparing `fedops-0.2.0/fedops/client/client_fl.py` & `fedops-0.2.1/fedops/client/client_fl.py`

 * *Files identical despite different names*

### Comparing `fedops-0.2.0/fedops/client/client_utils.py` & `fedops-0.2.1/fedops/client/client_utils.py`

 * *Files identical despite different names*

### Comparing `fedops-0.2.0/fedops/client/client_wandb.py` & `fedops-0.2.1/fedops/client/client_wandb.py`

 * *Files identical despite different names*

### Comparing `fedops-0.2.0/fedops/server/__init__.py` & `fedops-0.2.1/fedops/server/__init__.py`

 * *Files identical despite different names*

### Comparing `fedops-0.2.0/fedops/server/app.py` & `fedops-0.2.1/fedops/server/app.py`

 * *Files identical despite different names*

### Comparing `fedops-0.2.0/fedops/server/server_api.py` & `fedops-0.2.1/fedops/server/server_api.py`

 * *Files identical despite different names*

### Comparing `fedops-0.2.0/fedops/server/server_utils.py` & `fedops-0.2.1/fedops/server/server_utils.py`

 * *Files identical despite different names*

### Comparing `fedops-0.2.0/fedops/utils/version.py` & `fedops-0.2.1/fedops/utils/version.py`

 * *Files identical despite different names*

### Comparing `fedops-0.2.0/fedops.egg-info/PKG-INFO` & `fedops-0.2.1/fedops.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedops
-Version: 0.2.0
+Version: 0.2.1
 Summary: FL Lifecycle Operations Management Platform
 Home-page: https://github.com/gachon-CCLab/FedOps.git
 Author: Semo Yang
 Author-email: tpah20@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fedops-0.2.0/fedops.egg-info/SOURCES.txt` & `fedops-0.2.1/fedops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fedops-0.2.0/setup.py` & `fedops-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='fedops',
-    version='0.2.0',
+    version='0.2.1',
     author='Semo Yang',
     author_email='tpah20@gmail.com',
     description='FL Lifecycle Operations Management Platform',
     long_description='Long description of your library',
     url='https://github.com/gachon-CCLab/FedOps.git',
     packages=find_packages(),
     install_requires=[
```

