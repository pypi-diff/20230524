# Comparing `tmp/vector_vault-1.0.3.tar.gz` & `tmp/vector_vault-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-1.0.3.tar", last modified: Wed May 24 09:55:51 2023, max compression
+gzip compressed data, was "vector_vault-1.0.4.tar", last modified: Wed May 24 09:58:03 2023, max compression
```

## Comparing `vector_vault-1.0.3.tar` & `vector_vault-1.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-24 09:55:51.035622 vector_vault-1.0.3/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.0.3/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    11781 2023-05-24 09:55:51.035483 vector_vault-1.0.3/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    11056 2023-05-22 19:56:00.000000 vector_vault-1.0.3/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-05-24 09:55:51.035655 vector_vault-1.0.3/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-05-24 09:55:46.000000 vector_vault-1.0.3/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-24 09:55:51.033116 vector_vault-1.0.3/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    11781 2023-05-24 09:55:51.000000 vector_vault-1.0.3/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      406 2023-05-24 09:55:51.000000 vector_vault-1.0.3/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-05-24 09:55:51.000000 vector_vault-1.0.3/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-05-24 09:55:51.000000 vector_vault-1.0.3/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-05-24 09:55:51.000000 vector_vault-1.0.3/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-24 09:55:51.035330 vector_vault-1.0.3/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      674 2023-05-24 05:16:14.000000 vector_vault-1.0.3/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)     5163 2023-05-22 21:46:43.000000 vector_vault-1.0.3/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3524 2023-05-24 09:54:58.000000 vector_vault-1.0.3/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1849 2023-05-24 09:44:23.000000 vector_vault-1.0.3/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.0.3/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1542 2023-05-22 19:15:18.000000 vector_vault-1.0.3/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1160 2023-05-24 08:46:13.000000 vector_vault-1.0.3/vectorvault/signup.py
--rw-r--r--   0 johnrood   (501) staff       (20)    17191 2023-05-24 09:54:51.000000 vector_vault-1.0.3/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.0.3/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-24 09:58:03.900353 vector_vault-1.0.4/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.0.4/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    11781 2023-05-24 09:58:03.900206 vector_vault-1.0.4/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    11056 2023-05-22 19:56:00.000000 vector_vault-1.0.4/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-05-24 09:58:03.900389 vector_vault-1.0.4/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-05-24 09:57:59.000000 vector_vault-1.0.4/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-24 09:58:03.897747 vector_vault-1.0.4/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    11781 2023-05-24 09:58:03.000000 vector_vault-1.0.4/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      406 2023-05-24 09:58:03.000000 vector_vault-1.0.4/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-05-24 09:58:03.000000 vector_vault-1.0.4/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-05-24 09:58:03.000000 vector_vault-1.0.4/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-05-24 09:58:03.000000 vector_vault-1.0.4/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-24 09:58:03.900016 vector_vault-1.0.4/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      674 2023-05-24 05:16:14.000000 vector_vault-1.0.4/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     5163 2023-05-22 21:46:43.000000 vector_vault-1.0.4/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3525 2023-05-24 09:57:37.000000 vector_vault-1.0.4/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1849 2023-05-24 09:44:23.000000 vector_vault-1.0.4/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.0.4/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1542 2023-05-22 19:15:18.000000 vector_vault-1.0.4/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1160 2023-05-24 08:46:13.000000 vector_vault-1.0.4/vectorvault/signup.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    17191 2023-05-24 09:54:51.000000 vector_vault-1.0.4/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.0.4/vectorvault/wrap.py
```

### Comparing `vector_vault-1.0.3/LICENSE` & `vector_vault-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-1.0.3/PKG-INFO` & `vector_vault-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 1.0.3
+Version: 1.0.4
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
```

### Comparing `vector_vault-1.0.3/README.md` & `vector_vault-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `vector_vault-1.0.3/setup.py` & `vector_vault-1.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="1.0.3",
+    version="1.0.4",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-1.0.3/vector_vault.egg-info/PKG-INFO` & `vector_vault-1.0.4/vector_vault.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 1.0.3
+Version: 1.0.4
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
```

### Comparing `vector_vault-1.0.3/vectorvault/__init__.py` & `vector_vault-1.0.4/vectorvault/__init__.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.0.3/vectorvault/ai.py` & `vector_vault-1.0.4/vectorvault/ai.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.0.3/vectorvault/cloudmanager.py` & `vector_vault-1.0.4/vectorvault/cloudmanager.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # is strictly forbidden unless prior written permission is obtained
 # from Vector Vault.
 
 import tempfile
 import os
 import json
 from .creds import CustomCredentials
-from itemize import name
+from .itemize import name
 from google.cloud import storage
 from concurrent.futures import ThreadPoolExecutor, as_completed
 
 
 class CloudManager:
     def __init__(self, user: str, api_key: str, vault: str):
         self.user = self.get_user_id(user)
```

### Comparing `vector_vault-1.0.3/vectorvault/creds.py` & `vector_vault-1.0.4/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.0.3/vectorvault/download.py` & `vector_vault-1.0.4/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.0.3/vectorvault/itemize.py` & `vector_vault-1.0.4/vectorvault/itemize.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.0.3/vectorvault/signup.py` & `vector_vault-1.0.4/vectorvault/signup.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.0.3/vectorvault/vault.py` & `vector_vault-1.0.4/vectorvault/vault.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.0.3/vectorvault/wrap.py` & `vector_vault-1.0.4/vectorvault/wrap.py`

 * *Files identical despite different names*

