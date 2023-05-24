# Comparing `tmp/redhat_qe_cloud_tools-1.0.3.tar.gz` & `tmp/redhat_qe_cloud_tools-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redhat_qe_cloud_tools-1.0.3.tar", max compression
+gzip compressed data, was "redhat_qe_cloud_tools-1.0.4.tar", max compression
```

## Comparing `redhat_qe_cloud_tools-1.0.3.tar` & `redhat_qe_cloud_tools-1.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11357 2023-05-17 11:51:42.829928 redhat_qe_cloud_tools-1.0.3/LICENSE
--rw-r--r--   0        0        0      845 2023-05-17 11:51:42.829928 redhat_qe_cloud_tools-1.0.3/README.md
--rw-r--r--   0        0        0        0 2023-05-17 11:51:42.829928 redhat_qe_cloud_tools-1.0.3/clouds/__init__.py
--rw-r--r--   0        0        0      787 2023-05-17 11:51:42.829928 redhat_qe_cloud_tools-1.0.3/clouds/aws/README.md
--rw-r--r--   0        0        0        0 2023-05-17 11:51:42.829928 redhat_qe_cloud_tools-1.0.3/clouds/aws/__init__.py
--rw-r--r--   0        0        0      455 2023-05-17 11:51:42.829928 redhat_qe_cloud_tools-1.0.3/clouds/aws/aws_roles/README.md
--rw-r--r--   0        0        0        0 2023-05-17 11:51:42.829928 redhat_qe_cloud_tools-1.0.3/clouds/aws/aws_roles/__init__.py
--rw-r--r--   0        0        0     1591 2023-05-17 11:51:42.829928 redhat_qe_cloud_tools-1.0.3/clouds/aws/aws_roles/aws_roles.py
--rw-r--r--   0        0        0     1893 2023-05-17 11:51:42.829928 redhat_qe_cloud_tools-1.0.3/clouds/aws/aws_utils.py
--rw-r--r--   0        0        0     6218 2023-05-17 11:51:42.829928 redhat_qe_cloud_tools-1.0.3/clouds/aws/delete_s3_velero_bucket.py
--rw-r--r--   0        0        0      782 2023-05-17 11:51:42.829928 redhat_qe_cloud_tools-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     1561 1970-01-01 00:00:00.000000 redhat_qe_cloud_tools-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-24 07:19:50.881588 redhat_qe_cloud_tools-1.0.4/LICENSE
+-rw-r--r--   0        0        0      845 2023-05-24 07:19:50.881588 redhat_qe_cloud_tools-1.0.4/README.md
+-rw-r--r--   0        0        0        0 2023-05-24 07:19:50.881588 redhat_qe_cloud_tools-1.0.4/clouds/__init__.py
+-rw-r--r--   0        0        0      787 2023-05-24 07:19:50.882588 redhat_qe_cloud_tools-1.0.4/clouds/aws/README.md
+-rw-r--r--   0        0        0        0 2023-05-24 07:19:50.882588 redhat_qe_cloud_tools-1.0.4/clouds/aws/__init__.py
+-rw-r--r--   0        0        0      455 2023-05-24 07:19:50.882588 redhat_qe_cloud_tools-1.0.4/clouds/aws/aws_roles/README.md
+-rw-r--r--   0        0        0        0 2023-05-24 07:19:50.882588 redhat_qe_cloud_tools-1.0.4/clouds/aws/aws_roles/__init__.py
+-rw-r--r--   0        0        0     1193 2023-05-24 07:19:50.882588 redhat_qe_cloud_tools-1.0.4/clouds/aws/aws_roles/aws_roles.py
+-rw-r--r--   0        0        0     1893 2023-05-24 07:19:50.882588 redhat_qe_cloud_tools-1.0.4/clouds/aws/aws_utils.py
+-rw-r--r--   0        0        0     6218 2023-05-24 07:19:50.882588 redhat_qe_cloud_tools-1.0.4/clouds/aws/delete_s3_velero_bucket.py
+-rw-r--r--   0        0        0      782 2023-05-24 07:19:50.882588 redhat_qe_cloud_tools-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1561 1970-01-01 00:00:00.000000 redhat_qe_cloud_tools-1.0.4/PKG-INFO
```

### Comparing `redhat_qe_cloud_tools-1.0.3/LICENSE` & `redhat_qe_cloud_tools-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `redhat_qe_cloud_tools-1.0.3/README.md` & `redhat_qe_cloud_tools-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `redhat_qe_cloud_tools-1.0.3/clouds/aws/README.md` & `redhat_qe_cloud_tools-1.0.4/clouds/aws/README.md`

 * *Files identical despite different names*

### Comparing `redhat_qe_cloud_tools-1.0.3/clouds/aws/aws_roles/aws_roles.py` & `redhat_qe_cloud_tools-1.0.4/clouds/aws/aws_roles/aws_roles.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import os.path
-
 import boto3
 from simple_logger.logger import get_logger
 
 LOGGER = get_logger(name=__name__)
 DEFAULT_AWS_REGION = "us-east-1"
 
 
@@ -18,36 +16,27 @@
 
     """
     LOGGER.info(f"Creating IAM client using region {region}.")
     return boto3.client(service_name="iam", region_name=region)
 
 
 def create_or_update_role_policy(
-    role_name, policy_name, policy_document_path, region=DEFAULT_AWS_REGION
+    role_name, policy_name, policy_document, region=DEFAULT_AWS_REGION
 ):
     """
     Create a new policy role or update an existing one.
 
     Args:
         role_name (str): role policy name
         policy_name (str): policy name
-        policy_document_path (str): path to Json file that holds the policy documents
+        policy_document (str): policy documents as Json file content
         region (str): aws region
-
-    Raises:
-        FileNotFoundError: If policy document not found
     """
     client = iam_client(region=region)
     LOGGER.info(
-        f"Create/Update role {role_name} for policy {policy_name} by documented policy in {policy_document_path}."
+        f"Create/Update role {role_name} for policy {policy_name} by documented policy."
     )
-    if not os.path.isfile(policy_document_path):
-        raise FileNotFoundError(
-            f"File doesn't exists. Please validate file path: '{policy_document_path}'."
-        )
-    with open(policy_document_path, "r") as fd:
-        policy_document = fd.read()
     client.put_role_policy(
         RoleName=role_name,
         PolicyName=policy_name,
         PolicyDocument=policy_document,
     )
```

### Comparing `redhat_qe_cloud_tools-1.0.3/clouds/aws/aws_utils.py` & `redhat_qe_cloud_tools-1.0.4/clouds/aws/aws_utils.py`

 * *Files identical despite different names*

### Comparing `redhat_qe_cloud_tools-1.0.3/clouds/aws/delete_s3_velero_bucket.py` & `redhat_qe_cloud_tools-1.0.4/clouds/aws/delete_s3_velero_bucket.py`

 * *Files identical despite different names*

### Comparing `redhat_qe_cloud_tools-1.0.3/pyproject.toml` & `redhat_qe_cloud_tools-1.0.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 [tool.isort]
 line_length = 88
 profile = "black"
 
 [tool.poetry]
 name = "redhat-qe-cloud-tools"
-version = "1.0.3"
+version = "1.0.4"
 description = "Python utilities to manage cloud services, such as AWS."
 authors = ["Meni Yakove", "Ruth Netser"]
 readme = "README.md"
 repository = "https://github.com/RedHatQE/cloud-tools"
 packages = [{include = "clouds"}]
 
 [tool.poetry.dependencies]
```

### Comparing `redhat_qe_cloud_tools-1.0.3/PKG-INFO` & `redhat_qe_cloud_tools-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redhat-qe-cloud-tools
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python utilities to manage cloud services, such as AWS.
 Home-page: https://github.com/RedHatQE/cloud-tools
 Author: Meni Yakove
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

