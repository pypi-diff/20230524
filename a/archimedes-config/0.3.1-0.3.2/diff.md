# Comparing `tmp/archimedes_config-0.3.1.tar.gz` & `tmp/archimedes_config-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archimedes_config-0.3.1.tar", max compression
+gzip compressed data, was "archimedes_config-0.3.2.tar", max compression
```

## Comparing `archimedes_config-0.3.1.tar` & `archimedes_config-0.3.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      238 2023-05-15 08:32:42.181291 archimedes_config-0.3.1/archimedes_config/__init__.py
--rw-r--r--   0        0        0     8543 2023-05-15 08:32:42.181291 archimedes_config-0.3.1/archimedes_config/arckeyl.py
--rw-r--r--   0        0        0    13575 2023-05-15 08:32:42.181291 archimedes_config-0.3.1/archimedes_config/config_manager.py
--rw-r--r--   0        0        0     2308 2023-05-15 08:32:42.181291 archimedes_config-0.3.1/archimedes_config/keyvault_client.py
--rw-r--r--   0        0        0     1242 2023-05-15 08:32:42.181291 archimedes_config-0.3.1/archimedes_config/keyvault_config_manager.py
--rw-r--r--   0        0        0     1613 2023-05-15 08:32:42.181291 archimedes_config-0.3.1/archimedes_config/utils/path_utils.py
--rw-r--r--   0        0        0     3898 2023-05-15 08:32:42.181291 archimedes_config-0.3.1/archimedes_config/utils/util.py
--rw-r--r--   0        0        0      673 2023-05-15 08:32:42.181291 archimedes_config-0.3.1/archimedes_config/workflows/add_secrets.py
--rw-r--r--   0        0        0      965 2023-05-15 08:32:42.181291 archimedes_config-0.3.1/archimedes_config/workflows/lock_secrets.py
--rw-r--r--   0        0        0     2127 2023-05-15 08:32:42.181291 archimedes_config-0.3.1/archimedes_config/workflows/secret_creation.py
--rw-r--r--   0        0        0      944 2023-05-15 08:32:42.181291 archimedes_config-0.3.1/archimedes_config/workflows/unlock_secrets.py
--rw-r--r--   0        0        0     4126 2023-05-15 08:32:42.181291 archimedes_config-0.3.1/archimedes_config/workflows/workflow_base.py
--rw-r--r--   0        0        0      753 2023-05-15 08:32:42.185291 archimedes_config-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      749 1970-01-01 00:00:00.000000 archimedes_config-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      238 2023-05-24 11:51:36.132879 archimedes_config-0.3.2/archimedes_config/__init__.py
+-rw-r--r--   0        0        0     8543 2023-05-24 11:51:36.132879 archimedes_config-0.3.2/archimedes_config/arckeyl.py
+-rw-r--r--   0        0        0    13575 2023-05-24 11:51:36.132879 archimedes_config-0.3.2/archimedes_config/config_manager.py
+-rw-r--r--   0        0        0     2527 2023-05-24 11:51:36.132879 archimedes_config-0.3.2/archimedes_config/keyvault_client.py
+-rw-r--r--   0        0        0     1242 2023-05-24 11:51:36.132879 archimedes_config-0.3.2/archimedes_config/keyvault_config_manager.py
+-rw-r--r--   0        0        0     1613 2023-05-24 11:51:36.132879 archimedes_config-0.3.2/archimedes_config/utils/path_utils.py
+-rw-r--r--   0        0        0     3898 2023-05-24 11:51:36.132879 archimedes_config-0.3.2/archimedes_config/utils/util.py
+-rw-r--r--   0        0        0      673 2023-05-24 11:51:36.132879 archimedes_config-0.3.2/archimedes_config/workflows/add_secrets.py
+-rw-r--r--   0        0        0      965 2023-05-24 11:51:36.132879 archimedes_config-0.3.2/archimedes_config/workflows/lock_secrets.py
+-rw-r--r--   0        0        0     2127 2023-05-24 11:51:36.132879 archimedes_config-0.3.2/archimedes_config/workflows/secret_creation.py
+-rw-r--r--   0        0        0      944 2023-05-24 11:51:36.132879 archimedes_config-0.3.2/archimedes_config/workflows/unlock_secrets.py
+-rw-r--r--   0        0        0     4126 2023-05-24 11:51:36.132879 archimedes_config-0.3.2/archimedes_config/workflows/workflow_base.py
+-rw-r--r--   0        0        0      753 2023-05-24 11:51:36.132879 archimedes_config-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      749 1970-01-01 00:00:00.000000 archimedes_config-0.3.2/PKG-INFO
```

### Comparing `archimedes_config-0.3.1/archimedes_config/arckeyl.py` & `archimedes_config-0.3.2/archimedes_config/arckeyl.py`

 * *Files identical despite different names*

### Comparing `archimedes_config-0.3.1/archimedes_config/config_manager.py` & `archimedes_config-0.3.2/archimedes_config/config_manager.py`

 * *Files identical despite different names*

### Comparing `archimedes_config-0.3.1/archimedes_config/keyvault_client.py` & `archimedes_config-0.3.2/archimedes_config/keyvault_client.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """
 Client for handling interactions with keyvault
 """
 
-import os
 from typing import Union
 
 from azure.core.exceptions import ResourceNotFoundError  # pylint:disable=import-error
 from azure.identity import (  # pylint:disable=import-error
-    DefaultAzureCredential,
+    AzureCliCredential,
+    ChainedTokenCredential,
     EnvironmentCredential,
+    ManagedIdentityCredential,
+    SharedTokenCacheCredential,
 )
 from azure.keyvault.secrets import SecretClient  # pylint:disable=import-error
 
 
 class AzureKeyVaultClient:
     """
     Python client to handle communications with Azure keyvault
@@ -28,36 +30,32 @@
         self.client = SecretClient(vault_url=self.vault_url, credential=self.credential)
 
     @staticmethod
     def get_credential():
         """
         Generates az credentials for authentication
 
-        This method expects
-            AZURE_TENANT_ID
-            AZURE_CLIENT_ID
-            AZURE_CLIENT_SECRET
-        set as environments.
-
-        If these are unavailable, az cli login will be used.
-
-        :return:
+        The following order of credential methods will be
+        1. EnvironmentCredential:
+            Secrets set in environment variables.
+            Refer to azure identity docs for the correct combination of Environment variables.
+        2. ManagedIdentityCredential:
+            Identity provided to resources hosted on Azure.
+        3. AzureCliCredential:
+            Credentials set using `az login`.
+        4. SharedTokenCacheCredential:
+            For windows, using the login provided for the user.
         """
-        if (
-            "AZURE_TENANT_ID" in os.environ
-            and "AZURE_CLIENT_ID" in os.environ
-            and "AZURE_CLIENT_SECRET" in os.environ
-        ):
-            print("Using environment variables")
-            credential = EnvironmentCredential()
-        else:
-            print("Using default creds")
-            credential = DefaultAzureCredential()
-
-        return credential
+        credential_chain = (
+            EnvironmentCredential(),
+            ManagedIdentityCredential(),
+            AzureCliCredential(),
+            SharedTokenCacheCredential(),
+        )
+        return ChainedTokenCredential(*credential_chain)
 
     def get_secret(
         self, name: str, return_none_if_not_found: bool = True
     ) -> Union[str, None]:
         """
         Retrieves secret for provided name from key vaults
```

### Comparing `archimedes_config-0.3.1/archimedes_config/keyvault_config_manager.py` & `archimedes_config-0.3.2/archimedes_config/keyvault_config_manager.py`

 * *Files identical despite different names*

### Comparing `archimedes_config-0.3.1/archimedes_config/utils/path_utils.py` & `archimedes_config-0.3.2/archimedes_config/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `archimedes_config-0.3.1/archimedes_config/utils/util.py` & `archimedes_config-0.3.2/archimedes_config/utils/util.py`

 * *Files identical despite different names*

### Comparing `archimedes_config-0.3.1/archimedes_config/workflows/add_secrets.py` & `archimedes_config-0.3.2/archimedes_config/workflows/add_secrets.py`

 * *Files identical despite different names*

### Comparing `archimedes_config-0.3.1/archimedes_config/workflows/lock_secrets.py` & `archimedes_config-0.3.2/archimedes_config/workflows/lock_secrets.py`

 * *Files identical despite different names*

### Comparing `archimedes_config-0.3.1/archimedes_config/workflows/secret_creation.py` & `archimedes_config-0.3.2/archimedes_config/workflows/secret_creation.py`

 * *Files identical despite different names*

### Comparing `archimedes_config-0.3.1/archimedes_config/workflows/unlock_secrets.py` & `archimedes_config-0.3.2/archimedes_config/workflows/unlock_secrets.py`

 * *Files identical despite different names*

### Comparing `archimedes_config-0.3.1/archimedes_config/workflows/workflow_base.py` & `archimedes_config-0.3.2/archimedes_config/workflows/workflow_base.py`

 * *Files identical despite different names*

### Comparing `archimedes_config-0.3.1/pyproject.toml` & `archimedes_config-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "archimedes-config"
-version = "0.3.1"
+version = "0.3.2"
 description = ""
 authors = ["BigyaPradhan <bigya.pradhan@optimeering.com>"]
 packages = [{include = "archimedes_config"}]
 
 [tool.poetry.dependencies]
 python = ">=3.7.0,<3.12"
 cryptography = "^39.0.1"
```

### Comparing `archimedes_config-0.3.1/PKG-INFO` & `archimedes_config-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: archimedes-config
-Version: 0.3.1
+Version: 0.3.2
 Summary: 
 Author: BigyaPradhan
 Author-email: bigya.pradhan@optimeering.com
 Requires-Python: >=3.7.0,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

