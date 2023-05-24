# Comparing `tmp/vector_vault-1.0.0.tar.gz` & `tmp/vector_vault-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-1.0.0.tar", last modified: Tue May 23 07:07:35 2023, max compression
+gzip compressed data, was "vector_vault-1.0.1.tar", last modified: Wed May 24 09:10:38 2023, max compression
```

## Comparing `vector_vault-1.0.0.tar` & `vector_vault-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-23 07:07:35.789477 vector_vault-1.0.0/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.0.0/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    11781 2023-05-23 07:07:35.789327 vector_vault-1.0.0/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    11056 2023-05-22 19:56:00.000000 vector_vault-1.0.0/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-05-23 07:07:35.789524 vector_vault-1.0.0/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-05-23 07:07:12.000000 vector_vault-1.0.0/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-23 07:07:35.787204 vector_vault-1.0.0/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    11781 2023-05-23 07:07:35.000000 vector_vault-1.0.0/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      384 2023-05-23 07:07:35.000000 vector_vault-1.0.0/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-05-23 07:07:35.000000 vector_vault-1.0.0/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-05-23 07:07:35.000000 vector_vault-1.0.0/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-05-23 07:07:35.000000 vector_vault-1.0.0/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-23 07:07:35.789138 vector_vault-1.0.0/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      675 2023-05-21 06:23:38.000000 vector_vault-1.0.0/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)     5163 2023-05-22 21:46:43.000000 vector_vault-1.0.0/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3380 2023-05-22 19:00:54.000000 vector_vault-1.0.0/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1824 2023-05-22 19:13:17.000000 vector_vault-1.0.0/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.0.0/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1542 2023-05-22 19:15:18.000000 vector_vault-1.0.0/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)    17191 2023-05-22 19:49:38.000000 vector_vault-1.0.0/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.0.0/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-24 09:10:38.183840 vector_vault-1.0.1/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.0.1/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    11781 2023-05-24 09:10:38.183695 vector_vault-1.0.1/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    11056 2023-05-22 19:56:00.000000 vector_vault-1.0.1/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-05-24 09:10:38.183877 vector_vault-1.0.1/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-05-24 09:10:17.000000 vector_vault-1.0.1/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-24 09:10:38.181298 vector_vault-1.0.1/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    11781 2023-05-24 09:10:38.000000 vector_vault-1.0.1/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      406 2023-05-24 09:10:38.000000 vector_vault-1.0.1/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-05-24 09:10:38.000000 vector_vault-1.0.1/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-05-24 09:10:38.000000 vector_vault-1.0.1/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-05-24 09:10:38.000000 vector_vault-1.0.1/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-24 09:10:38.183412 vector_vault-1.0.1/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      674 2023-05-24 05:16:14.000000 vector_vault-1.0.1/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     5163 2023-05-22 21:46:43.000000 vector_vault-1.0.1/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3380 2023-05-24 09:09:28.000000 vector_vault-1.0.1/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1806 2023-05-24 09:08:54.000000 vector_vault-1.0.1/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.0.1/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1542 2023-05-22 19:15:18.000000 vector_vault-1.0.1/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1160 2023-05-24 08:46:13.000000 vector_vault-1.0.1/vectorvault/signup.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    17191 2023-05-24 09:09:19.000000 vector_vault-1.0.1/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.0.1/vectorvault/wrap.py
```

### Comparing `vector_vault-1.0.0/LICENSE` & `vector_vault-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-1.0.0/PKG-INFO` & `vector_vault-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 1.0.0
+Version: 1.0.1
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
```

### Comparing `vector_vault-1.0.0/README.md` & `vector_vault-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `vector_vault-1.0.0/setup.py` & `vector_vault-1.0.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="1.0.0",
+    version="1.0.1",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-1.0.0/vector_vault.egg-info/PKG-INFO` & `vector_vault-1.0.1/vector_vault.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 1.0.0
+Version: 1.0.1
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
```

### Comparing `vector_vault-1.0.0/vectorvault/__init__.py` & `vector_vault-1.0.1/vectorvault/__init__.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # patents in process, and are protected by trade secret or copyright law.
 # Dissemination of this information or reproduction of this material
 # is strictly forbidden unless prior written permission is obtained
 # from Vector Vault.
 
 from .vault import Vault
 from .download import download_url
-from .wrap import wrap
+from .wrap import wrap
```

### Comparing `vector_vault-1.0.0/vectorvault/ai.py` & `vector_vault-1.0.1/vectorvault/ai.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.0.0/vectorvault/cloudmanager.py` & `vector_vault-1.0.1/vectorvault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.0.0/vectorvault/creds.py` & `vector_vault-1.0.1/vectorvault/creds.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 class CustomCredentials(Credentials):
     def __init__(self, user, api):
         self.user = user
         self.api = api
         self.token = None
         self.expiry = None
-        self.refresh(requests.Request())
+        self.refresh()
 
     def apply(self, headers, token=None):
         headers["Authorization"] = f"Bearer {self.token}"
 
     @property
     def valid(self):
         if self.expiry is None:
```

### Comparing `vector_vault-1.0.0/vectorvault/download.py` & `vector_vault-1.0.1/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.0.0/vectorvault/itemize.py` & `vector_vault-1.0.1/vectorvault/itemize.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.0.0/vectorvault/vault.py` & `vector_vault-1.0.1/vectorvault/vault.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.0.0/vectorvault/wrap.py` & `vector_vault-1.0.1/vectorvault/wrap.py`

 * *Files identical despite different names*

