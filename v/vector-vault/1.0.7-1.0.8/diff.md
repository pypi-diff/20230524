# Comparing `tmp/vector_vault-1.0.7.tar.gz` & `tmp/vector_vault-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-1.0.7.tar", last modified: Wed May 24 20:33:11 2023, max compression
+gzip compressed data, was "vector_vault-1.0.8.tar", last modified: Wed May 24 21:06:30 2023, max compression
```

## Comparing `vector_vault-1.0.7.tar` & `vector_vault-1.0.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-24 20:33:11.830737 vector_vault-1.0.7/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.0.7/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    12182 2023-05-24 20:33:11.830564 vector_vault-1.0.7/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    11457 2023-05-24 20:28:22.000000 vector_vault-1.0.7/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-05-24 20:33:11.830777 vector_vault-1.0.7/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-05-24 19:16:02.000000 vector_vault-1.0.7/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-24 20:33:11.824564 vector_vault-1.0.7/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    12182 2023-05-24 20:33:11.000000 vector_vault-1.0.7/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      406 2023-05-24 20:33:11.000000 vector_vault-1.0.7/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-05-24 20:33:11.000000 vector_vault-1.0.7/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-05-24 20:33:11.000000 vector_vault-1.0.7/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-05-24 20:33:11.000000 vector_vault-1.0.7/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-24 20:33:11.830103 vector_vault-1.0.7/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      702 2023-05-24 19:36:19.000000 vector_vault-1.0.7/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)     6181 2023-05-24 19:11:23.000000 vector_vault-1.0.7/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3525 2023-05-24 19:28:03.000000 vector_vault-1.0.7/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1849 2023-05-24 09:44:23.000000 vector_vault-1.0.7/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.0.7/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1542 2023-05-22 19:15:18.000000 vector_vault-1.0.7/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1079 2023-05-24 19:36:47.000000 vector_vault-1.0.7/vectorvault/signup.py
--rw-r--r--   0 johnrood   (501) staff       (20)    17637 2023-05-24 19:27:56.000000 vector_vault-1.0.7/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.0.7/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-24 21:06:30.496311 vector_vault-1.0.8/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.0.8/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    12741 2023-05-24 21:06:30.496146 vector_vault-1.0.8/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    12016 2023-05-24 21:06:05.000000 vector_vault-1.0.8/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-05-24 21:06:30.496348 vector_vault-1.0.8/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-05-24 21:06:09.000000 vector_vault-1.0.8/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-24 21:06:30.493083 vector_vault-1.0.8/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    12741 2023-05-24 21:06:30.000000 vector_vault-1.0.8/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      406 2023-05-24 21:06:30.000000 vector_vault-1.0.8/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-05-24 21:06:30.000000 vector_vault-1.0.8/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-05-24 21:06:30.000000 vector_vault-1.0.8/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-05-24 21:06:30.000000 vector_vault-1.0.8/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-24 21:06:30.495725 vector_vault-1.0.8/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      702 2023-05-24 19:36:19.000000 vector_vault-1.0.8/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     6181 2023-05-24 19:11:23.000000 vector_vault-1.0.8/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3525 2023-05-24 19:28:03.000000 vector_vault-1.0.8/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1849 2023-05-24 09:44:23.000000 vector_vault-1.0.8/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.0.8/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1542 2023-05-22 19:15:18.000000 vector_vault-1.0.8/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1079 2023-05-24 19:36:47.000000 vector_vault-1.0.8/vectorvault/signup.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    17637 2023-05-24 19:27:56.000000 vector_vault-1.0.8/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.0.8/vectorvault/wrap.py
```

### Comparing `vector_vault-1.0.7/LICENSE` & `vector_vault-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-1.0.7/PKG-INFO` & `vector_vault-1.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 1.0.7
+Version: 1.0.8
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
@@ -13,29 +13,29 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-![alt text](https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/5cdf6b7f-351f-4821-ba6a-beb07aaf1068/Vector+Vault+Header+5033.jpg)
+![alt text](https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/297fde6c-f5b4-4076-83bc-81dcfdbffebe/Vector+Vault+Header+5000.jpg)
 
 Vector Vault is designed to simplify the process of working with vector databases. It allows users to vectorize datasets efficiently, and access them seamlessly from the cloud. It's scalable and suitable for both small and large scale projects. Vector Vault has been designed with a user-friendly interface to make the process of working with vector databases easy and let you focus on what matters. It simplifies complex workflows, ensures secure and isolated data handling, and enables users to create and interact vector databases - aka "vaults" 
 
 Vector Vault was built with the goal of making generative ai work flows simple and easy. By combining vector similarity search with generative ai chat, new possibilities for conversation and communication emerge. For example, product information can be added to a vault, and when a customer asks a product question, the right product information can be instantly retreived and seamlessly used in conversation by chatgpt for an accurate response. This capability allows for informed conversation and the possibilites range from ai automated customer support, to new ways to get news, to ai code reviews that reference source documentation, to ai domain experts for specific knowledges, and much more.
 
-Vector Vault uses a proprietary Inception Architecture, allowing you to create any number of vaults, and vaults within a vaults. Each vault is it's own database, and automatically integrates data storage in the cloud. You will need a Vector Vault account in order to get your user id and api key for cloud access. If you don't already have one, you can use the included `register()` function or sign up free at [VectorVault.io](https://vectorvault.io)
+Vector Vault uses a proprietary Inception Architecture, allowing you to create any number of vaults, and vaults within a vaults. Each vault is it's own database, and automatically integrates data storage in the cloud. You will need a Vector Vault account in order to get your user id and api key for cloud access. If you don't already have one, you can use the included `register()` function or sign up at [VectorVault.io](https://vectorvault.io)
 
 This python library allows you to interact with Vector Vault using its Python-based API. It includes operations such as creating a vault, deleting the vault, adding data to the vault, getting vector embeddings for the data, saving data to the vault, interacting with OpenAI's ChatGPT model to get responses, and managing conversation history for more contextualized responses.
 
 <br>
 
 # Interact with your Vault:
 <p align="center">
-  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/000a11f9-c091-4c04-a22d-f262bc5c30dc/Vault+small.png" />
+  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/3a6c60a3-79ac-467c-b640-c434499ca76d/Vector+Vault+Vault+2000.jpg" width="500" height="500" />
 </p>
 
 `add` : Add item to the Vault, with automatic text splitting and processing for long texts. Main way to add to vault
 <br>
 `add_item` : Add item to the Vault
 <br>
 `add_item_with_vector` : Add item to the Vault with vector provided - only accepts vectors of 1536 dimensions
@@ -126,23 +126,28 @@
 ```
 ^ these three lines execute fast and can be called as often as you like. For example: `add`, `get_vectors`, and `save` can be used mid conversation to add every message to the vault one at a time as they comes in.
 
 
 <br>
 <br>
 
-## Use the vault later:
+# Reference Your Vault:
+<p align="center">
+  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/5ae905b0-43d0-4b86-a965-5b447ee8c7de/Vector+Vault+Vault.jpg?content-type=image%2Fjpeg" width="500" height="500" />
+</p>
+
+After you've added some data and want to reference it later, you can call it like this:
 ```
 similar_data = vault.get_similar(text_input) # returns a list with 4 results
-similar_data = vault.get_similar(text_input, n = 10) # returns 10 results
 
 # Print each similar item 
 for result in similar_data:
     print(result['data'])
 ```
+`similar_data = vault.get_similar(text_input, n = 10)` returns 10 results instead of the default of 4.
 
 
 <br>
 
 ## Use the `get_chat()` function to get a response from chatgpt
 The following searches the vault for 4 similar results and then give those to chatgpt as context, asking chatgpt answer the question using the context
 ```
@@ -342,11 +347,14 @@
 
 
 <br>
 <br>
 
 If have any questions, leave a comment. Open the "examples" folder and try out the Google Colab tutorials we have.
 
-Happy coding.
+Happy coding!
+<p align="center">
+  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/8ba5c4eb-e880-426a-94e7-16c750e1bfe7/Looking+out+with+hope+vector+vault+small.png" />
+</p>
```

### Comparing `vector_vault-1.0.7/README.md` & `vector_vault-1.0.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-![alt text](https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/5cdf6b7f-351f-4821-ba6a-beb07aaf1068/Vector+Vault+Header+5033.jpg)
+![alt text](https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/297fde6c-f5b4-4076-83bc-81dcfdbffebe/Vector+Vault+Header+5000.jpg)
 
 Vector Vault is designed to simplify the process of working with vector databases. It allows users to vectorize datasets efficiently, and access them seamlessly from the cloud. It's scalable and suitable for both small and large scale projects. Vector Vault has been designed with a user-friendly interface to make the process of working with vector databases easy and let you focus on what matters. It simplifies complex workflows, ensures secure and isolated data handling, and enables users to create and interact vector databases - aka "vaults" 
 
 Vector Vault was built with the goal of making generative ai work flows simple and easy. By combining vector similarity search with generative ai chat, new possibilities for conversation and communication emerge. For example, product information can be added to a vault, and when a customer asks a product question, the right product information can be instantly retreived and seamlessly used in conversation by chatgpt for an accurate response. This capability allows for informed conversation and the possibilites range from ai automated customer support, to new ways to get news, to ai code reviews that reference source documentation, to ai domain experts for specific knowledges, and much more.
 
-Vector Vault uses a proprietary Inception Architecture, allowing you to create any number of vaults, and vaults within a vaults. Each vault is it's own database, and automatically integrates data storage in the cloud. You will need a Vector Vault account in order to get your user id and api key for cloud access. If you don't already have one, you can use the included `register()` function or sign up free at [VectorVault.io](https://vectorvault.io)
+Vector Vault uses a proprietary Inception Architecture, allowing you to create any number of vaults, and vaults within a vaults. Each vault is it's own database, and automatically integrates data storage in the cloud. You will need a Vector Vault account in order to get your user id and api key for cloud access. If you don't already have one, you can use the included `register()` function or sign up at [VectorVault.io](https://vectorvault.io)
 
 This python library allows you to interact with Vector Vault using its Python-based API. It includes operations such as creating a vault, deleting the vault, adding data to the vault, getting vector embeddings for the data, saving data to the vault, interacting with OpenAI's ChatGPT model to get responses, and managing conversation history for more contextualized responses.
 
 <br>
 
 # Interact with your Vault:
 <p align="center">
-  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/000a11f9-c091-4c04-a22d-f262bc5c30dc/Vault+small.png" />
+  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/3a6c60a3-79ac-467c-b640-c434499ca76d/Vector+Vault+Vault+2000.jpg" width="500" height="500" />
 </p>
 
 `add` : Add item to the Vault, with automatic text splitting and processing for long texts. Main way to add to vault
 <br>
 `add_item` : Add item to the Vault
 <br>
 `add_item_with_vector` : Add item to the Vault with vector provided - only accepts vectors of 1536 dimensions
@@ -107,23 +107,28 @@
 ```
 ^ these three lines execute fast and can be called as often as you like. For example: `add`, `get_vectors`, and `save` can be used mid conversation to add every message to the vault one at a time as they comes in.
 
 
 <br>
 <br>
 
-## Use the vault later:
+# Reference Your Vault:
+<p align="center">
+  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/5ae905b0-43d0-4b86-a965-5b447ee8c7de/Vector+Vault+Vault.jpg?content-type=image%2Fjpeg" width="500" height="500" />
+</p>
+
+After you've added some data and want to reference it later, you can call it like this:
 ```
 similar_data = vault.get_similar(text_input) # returns a list with 4 results
-similar_data = vault.get_similar(text_input, n = 10) # returns 10 results
 
 # Print each similar item 
 for result in similar_data:
     print(result['data'])
 ```
+`similar_data = vault.get_similar(text_input, n = 10)` returns 10 results instead of the default of 4.
 
 
 <br>
 
 ## Use the `get_chat()` function to get a response from chatgpt
 The following searches the vault for 4 similar results and then give those to chatgpt as context, asking chatgpt answer the question using the context
 ```
@@ -323,9 +328,12 @@
 
 
 <br>
 <br>
 
 If have any questions, leave a comment. Open the "examples" folder and try out the Google Colab tutorials we have.
 
-Happy coding.
+Happy coding!
+<p align="center">
+  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/8ba5c4eb-e880-426a-94e7-16c750e1bfe7/Looking+out+with+hope+vector+vault+small.png" />
+</p>
```

### Comparing `vector_vault-1.0.7/setup.py` & `vector_vault-1.0.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="1.0.7",
+    version="1.0.8",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-1.0.7/vector_vault.egg-info/PKG-INFO` & `vector_vault-1.0.8/vector_vault.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 1.0.7
+Version: 1.0.8
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
@@ -13,29 +13,29 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-![alt text](https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/5cdf6b7f-351f-4821-ba6a-beb07aaf1068/Vector+Vault+Header+5033.jpg)
+![alt text](https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/297fde6c-f5b4-4076-83bc-81dcfdbffebe/Vector+Vault+Header+5000.jpg)
 
 Vector Vault is designed to simplify the process of working with vector databases. It allows users to vectorize datasets efficiently, and access them seamlessly from the cloud. It's scalable and suitable for both small and large scale projects. Vector Vault has been designed with a user-friendly interface to make the process of working with vector databases easy and let you focus on what matters. It simplifies complex workflows, ensures secure and isolated data handling, and enables users to create and interact vector databases - aka "vaults" 
 
 Vector Vault was built with the goal of making generative ai work flows simple and easy. By combining vector similarity search with generative ai chat, new possibilities for conversation and communication emerge. For example, product information can be added to a vault, and when a customer asks a product question, the right product information can be instantly retreived and seamlessly used in conversation by chatgpt for an accurate response. This capability allows for informed conversation and the possibilites range from ai automated customer support, to new ways to get news, to ai code reviews that reference source documentation, to ai domain experts for specific knowledges, and much more.
 
-Vector Vault uses a proprietary Inception Architecture, allowing you to create any number of vaults, and vaults within a vaults. Each vault is it's own database, and automatically integrates data storage in the cloud. You will need a Vector Vault account in order to get your user id and api key for cloud access. If you don't already have one, you can use the included `register()` function or sign up free at [VectorVault.io](https://vectorvault.io)
+Vector Vault uses a proprietary Inception Architecture, allowing you to create any number of vaults, and vaults within a vaults. Each vault is it's own database, and automatically integrates data storage in the cloud. You will need a Vector Vault account in order to get your user id and api key for cloud access. If you don't already have one, you can use the included `register()` function or sign up at [VectorVault.io](https://vectorvault.io)
 
 This python library allows you to interact with Vector Vault using its Python-based API. It includes operations such as creating a vault, deleting the vault, adding data to the vault, getting vector embeddings for the data, saving data to the vault, interacting with OpenAI's ChatGPT model to get responses, and managing conversation history for more contextualized responses.
 
 <br>
 
 # Interact with your Vault:
 <p align="center">
-  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/000a11f9-c091-4c04-a22d-f262bc5c30dc/Vault+small.png" />
+  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/3a6c60a3-79ac-467c-b640-c434499ca76d/Vector+Vault+Vault+2000.jpg" width="500" height="500" />
 </p>
 
 `add` : Add item to the Vault, with automatic text splitting and processing for long texts. Main way to add to vault
 <br>
 `add_item` : Add item to the Vault
 <br>
 `add_item_with_vector` : Add item to the Vault with vector provided - only accepts vectors of 1536 dimensions
@@ -126,23 +126,28 @@
 ```
 ^ these three lines execute fast and can be called as often as you like. For example: `add`, `get_vectors`, and `save` can be used mid conversation to add every message to the vault one at a time as they comes in.
 
 
 <br>
 <br>
 
-## Use the vault later:
+# Reference Your Vault:
+<p align="center">
+  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/5ae905b0-43d0-4b86-a965-5b447ee8c7de/Vector+Vault+Vault.jpg?content-type=image%2Fjpeg" width="500" height="500" />
+</p>
+
+After you've added some data and want to reference it later, you can call it like this:
 ```
 similar_data = vault.get_similar(text_input) # returns a list with 4 results
-similar_data = vault.get_similar(text_input, n = 10) # returns 10 results
 
 # Print each similar item 
 for result in similar_data:
     print(result['data'])
 ```
+`similar_data = vault.get_similar(text_input, n = 10)` returns 10 results instead of the default of 4.
 
 
 <br>
 
 ## Use the `get_chat()` function to get a response from chatgpt
 The following searches the vault for 4 similar results and then give those to chatgpt as context, asking chatgpt answer the question using the context
 ```
@@ -342,11 +347,14 @@
 
 
 <br>
 <br>
 
 If have any questions, leave a comment. Open the "examples" folder and try out the Google Colab tutorials we have.
 
-Happy coding.
+Happy coding!
+<p align="center">
+  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/8ba5c4eb-e880-426a-94e7-16c750e1bfe7/Looking+out+with+hope+vector+vault+small.png" />
+</p>
```

### Comparing `vector_vault-1.0.7/vectorvault/__init__.py` & `vector_vault-1.0.8/vectorvault/__init__.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.0.7/vectorvault/ai.py` & `vector_vault-1.0.8/vectorvault/ai.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.0.7/vectorvault/cloudmanager.py` & `vector_vault-1.0.8/vectorvault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.0.7/vectorvault/creds.py` & `vector_vault-1.0.8/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.0.7/vectorvault/download.py` & `vector_vault-1.0.8/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.0.7/vectorvault/itemize.py` & `vector_vault-1.0.8/vectorvault/itemize.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.0.7/vectorvault/signup.py` & `vector_vault-1.0.8/vectorvault/signup.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.0.7/vectorvault/vault.py` & `vector_vault-1.0.8/vectorvault/vault.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.0.7/vectorvault/wrap.py` & `vector_vault-1.0.8/vectorvault/wrap.py`

 * *Files identical despite different names*

