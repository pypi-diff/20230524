# Comparing `tmp/vector_vault-1.0.5.tar.gz` & `tmp/vector_vault-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-1.0.5.tar", last modified: Wed May 24 18:42:04 2023, max compression
+gzip compressed data, was "vector_vault-1.0.6.tar", last modified: Wed May 24 18:50:08 2023, max compression
```

## Comparing `vector_vault-1.0.5.tar` & `vector_vault-1.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-24 18:42:04.004975 vector_vault-1.0.5/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.0.5/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    11781 2023-05-24 18:42:04.004830 vector_vault-1.0.5/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    11056 2023-05-22 19:56:00.000000 vector_vault-1.0.5/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-05-24 18:42:04.005012 vector_vault-1.0.5/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-05-24 18:41:59.000000 vector_vault-1.0.5/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-24 18:42:04.002341 vector_vault-1.0.5/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    11781 2023-05-24 18:42:03.000000 vector_vault-1.0.5/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      406 2023-05-24 18:42:04.000000 vector_vault-1.0.5/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-05-24 18:42:03.000000 vector_vault-1.0.5/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-05-24 18:42:03.000000 vector_vault-1.0.5/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-05-24 18:42:03.000000 vector_vault-1.0.5/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-24 18:42:04.004444 vector_vault-1.0.5/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      674 2023-05-24 05:16:14.000000 vector_vault-1.0.5/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)     6430 2023-05-24 18:41:32.000000 vector_vault-1.0.5/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3525 2023-05-24 09:57:37.000000 vector_vault-1.0.5/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1849 2023-05-24 09:44:23.000000 vector_vault-1.0.5/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.0.5/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1542 2023-05-22 19:15:18.000000 vector_vault-1.0.5/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1160 2023-05-24 08:46:13.000000 vector_vault-1.0.5/vectorvault/signup.py
--rw-r--r--   0 johnrood   (501) staff       (20)    17191 2023-05-24 09:54:51.000000 vector_vault-1.0.5/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.0.5/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-24 18:50:08.902947 vector_vault-1.0.6/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.0.6/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    11781 2023-05-24 18:50:08.902799 vector_vault-1.0.6/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    11056 2023-05-22 19:56:00.000000 vector_vault-1.0.6/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-05-24 18:50:08.902990 vector_vault-1.0.6/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-05-24 18:49:50.000000 vector_vault-1.0.6/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-24 18:50:08.900085 vector_vault-1.0.6/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    11781 2023-05-24 18:50:08.000000 vector_vault-1.0.6/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      406 2023-05-24 18:50:08.000000 vector_vault-1.0.6/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-05-24 18:50:08.000000 vector_vault-1.0.6/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-05-24 18:50:08.000000 vector_vault-1.0.6/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-05-24 18:50:08.000000 vector_vault-1.0.6/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-24 18:50:08.902330 vector_vault-1.0.6/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      674 2023-05-24 05:16:14.000000 vector_vault-1.0.6/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     6429 2023-05-24 18:48:55.000000 vector_vault-1.0.6/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3525 2023-05-24 09:57:37.000000 vector_vault-1.0.6/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1849 2023-05-24 09:44:23.000000 vector_vault-1.0.6/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.0.6/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1542 2023-05-22 19:15:18.000000 vector_vault-1.0.6/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1160 2023-05-24 08:46:13.000000 vector_vault-1.0.6/vectorvault/signup.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    17191 2023-05-24 09:54:51.000000 vector_vault-1.0.6/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.0.6/vectorvault/wrap.py
```

### Comparing `vector_vault-1.0.5/LICENSE` & `vector_vault-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-1.0.5/PKG-INFO` & `vector_vault-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 1.0.5
+Version: 1.0.6
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
```

### Comparing `vector_vault-1.0.5/README.md` & `vector_vault-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `vector_vault-1.0.5/setup.py` & `vector_vault-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="1.0.5",
+    version="1.0.6",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-1.0.5/vector_vault.egg-info/PKG-INFO` & `vector_vault-1.0.6/vector_vault.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 1.0.5
+Version: 1.0.6
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
```

### Comparing `vector_vault-1.0.5/vectorvault/__init__.py` & `vector_vault-1.0.6/vectorvault/__init__.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.0.5/vectorvault/ai.py` & `vector_vault-1.0.6/vectorvault/ai.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,35 +60,34 @@
         Answer:"""
 
         intokes = self.get_tokens(user_input)
         contokes = self.get_tokens(context)
         histokes = self.get_tokens(history) if history else 0
         if intokes + contokes + histokes > 4000:
             tokes_left = 4000 - intokes
-            if history > 0:
+            if history:
                 tokes_left = 2000 - intokes # remove more history than context
                 char_left = tokes_left * 4
                 history = history[-char_left:]
                 tokes_left_after_hist = 4000 - self.get_tokens(user_input + history)
                 char_left_after_hist = tokes_left_after_hist * 4
                 context = context[-char_left_after_hist:]
-                double_check = self.get_tokens(user_input+history+context)
+                double_check = self.get_tokens(user_input + history + context)
                 if double_check > 4096: # max input
                     remainder = double_check - 4096
                     char_to_take_away = remainder * 5
                     context = context[-char_to_take_away:] # go back x characters and then take the allowed context forward
             else:
                 char_left = tokes_left * 4 # multiply characters by tokens 
                 context = context[-char_left:] # take away excess characters 
-                double_check = self.get_tokens(user_input+context) # doulble check tokens input
+                double_check = self.get_tokens(user_input + context) # double check tokens input
                 if double_check > 4096: # max input
                     remainder = double_check - 4096 # figure out how
                     char_to_take_away = remainder * 5 # calc character excess if double_check failed
-                    context -= context[:char_to_take_away] # minus excess characters from beginning of string
-
+                    context = context[char_to_take_away:] # minus excess characters from beginning of string
 
         # Format the prompt
         user_input = history + user_input
         prompt = prompt_template.format(context=context, question=user_input)
 
         response = openai.ChatCompletion.create(
             model=model,
```

### Comparing `vector_vault-1.0.5/vectorvault/cloudmanager.py` & `vector_vault-1.0.6/vectorvault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.0.5/vectorvault/creds.py` & `vector_vault-1.0.6/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.0.5/vectorvault/download.py` & `vector_vault-1.0.6/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.0.5/vectorvault/itemize.py` & `vector_vault-1.0.6/vectorvault/itemize.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.0.5/vectorvault/signup.py` & `vector_vault-1.0.6/vectorvault/signup.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.0.5/vectorvault/vault.py` & `vector_vault-1.0.6/vectorvault/vault.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.0.5/vectorvault/wrap.py` & `vector_vault-1.0.6/vectorvault/wrap.py`

 * *Files identical despite different names*

