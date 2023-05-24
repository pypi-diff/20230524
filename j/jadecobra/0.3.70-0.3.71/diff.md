# Comparing `tmp/jadecobra-0.3.70.tar.gz` & `tmp/jadecobra-0.3.71.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jadecobra-0.3.70.tar", last modified: Fri May 19 21:31:47 2023, max compression
+gzip compressed data, was "jadecobra-0.3.71.tar", last modified: Wed May 24 19:22:02 2023, max compression
```

## Comparing `jadecobra-0.3.70.tar` & `jadecobra-0.3.71.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 johnnyblase   (501) staff       (20)        0 2023-05-19 21:31:47.800323 jadecobra-0.3.70/
--rw-r--r--   0 johnnyblase   (501) staff       (20)     1066 2022-08-18 02:10:38.000000 jadecobra-0.3.70/LICENSE
--rw-r--r--   0 johnnyblase   (501) staff       (20)     1878 2023-05-19 21:31:47.800179 jadecobra-0.3.70/PKG-INFO
--rw-r--r--   0 johnnyblase   (501) staff       (20)      150 2022-08-29 03:32:29.000000 jadecobra-0.3.70/README.md
--rw-r--r--   0 johnnyblase   (501) staff       (20)      534 2023-05-19 21:30:26.000000 jadecobra-0.3.70/pyproject.toml
--rw-r--r--   0 johnnyblase   (501) staff       (20)       38 2023-05-19 21:31:47.800364 jadecobra-0.3.70/setup.cfg
-drwxr-xr-x   0 johnnyblase   (501) staff       (20)        0 2023-05-19 21:31:47.791884 jadecobra-0.3.70/src/
-drwxr-xr-x   0 johnnyblase   (501) staff       (20)        0 2023-05-19 21:31:47.792523 jadecobra-0.3.70/src/None/
--rw-r--r--   0 johnnyblase   (501) staff       (20)       22 2023-04-20 16:05:17.000000 jadecobra-0.3.70/src/None/__init__.py
-drwxr-xr-x   0 johnnyblase   (501) staff       (20)        0 2023-05-19 21:31:47.794827 jadecobra-0.3.70/src/jadecobra/
--rw-r--r--   0 johnnyblase   (501) staff       (20)       22 2023-05-19 21:30:26.000000 jadecobra-0.3.70/src/jadecobra/__init__.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)     1422 2022-08-19 16:12:38.000000 jadecobra-0.3.70/src/jadecobra/aws_environment.py
-drwxr-xr-x   0 johnnyblase   (501) staff       (20)        0 2023-05-19 21:31:47.795863 jadecobra-0.3.70/src/jadecobra/aws_lambda/
--rw-r--r--   0 johnnyblase   (501) staff       (20)      170 2023-03-29 21:40:49.000000 jadecobra-0.3.70/src/jadecobra/aws_lambda/__init__.py
-drwxr-xr-x   0 johnnyblase   (501) staff       (20)        0 2023-05-19 21:31:47.797164 jadecobra-0.3.70/src/jadecobra/aws_lambda/deploy/
--rw-r--r--   0 johnnyblase   (501) staff       (20)       27 2022-08-19 16:21:46.000000 jadecobra-0.3.70/src/jadecobra/aws_lambda/deploy/__init__.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)     1349 2023-03-31 22:22:12.000000 jadecobra-0.3.70/src/jadecobra/aws_lambda/deploy/deploy.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)     1187 2023-04-02 23:31:34.000000 jadecobra-0.3.70/src/jadecobra/aws_lambda/deploy/deploy_lambda.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)     1745 2022-08-19 16:21:46.000000 jadecobra-0.3.70/src/jadecobra/aws_lambda/deploy/lambda_function.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)     3888 2023-04-28 20:18:57.000000 jadecobra-0.3.70/src/jadecobra/aws_lambda/deploy/lambda_layer.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)       14 2023-01-30 18:47:15.000000 jadecobra-0.3.70/src/jadecobra/cloudformation_deployer.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)        0 2023-03-31 20:02:12.000000 jadecobra-0.3.70/src/jadecobra/setup_tdd.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)     5269 2023-05-19 21:29:49.000000 jadecobra-0.3.70/src/jadecobra/tester.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)     3265 2023-04-20 18:35:14.000000 jadecobra-0.3.70/src/jadecobra/toolkit.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)     1947 2023-04-20 18:29:33.000000 jadecobra-0.3.70/src/jadecobra/versioning.py
-drwxr-xr-x   0 johnnyblase   (501) staff       (20)        0 2023-05-19 21:31:47.795728 jadecobra-0.3.70/src/jadecobra.egg-info/
--rw-r--r--   0 johnnyblase   (501) staff       (20)     1878 2023-05-19 21:31:47.000000 jadecobra-0.3.70/src/jadecobra.egg-info/PKG-INFO
--rw-r--r--   0 johnnyblase   (501) staff       (20)     1050 2023-05-19 21:31:47.000000 jadecobra-0.3.70/src/jadecobra.egg-info/SOURCES.txt
--rw-r--r--   0 johnnyblase   (501) staff       (20)        1 2023-05-19 21:31:47.000000 jadecobra-0.3.70/src/jadecobra.egg-info/dependency_links.txt
--rw-r--r--   0 johnnyblase   (501) staff       (20)       14 2023-05-19 21:31:47.000000 jadecobra-0.3.70/src/jadecobra.egg-info/requires.txt
--rw-r--r--   0 johnnyblase   (501) staff       (20)       15 2023-05-19 21:31:47.000000 jadecobra-0.3.70/src/jadecobra.egg-info/top_level.txt
-drwxr-xr-x   0 johnnyblase   (501) staff       (20)        0 2023-05-19 21:31:47.799843 jadecobra-0.3.70/tests/
--rw-r--r--   0 johnnyblase   (501) staff       (20)     1393 2023-04-02 23:59:47.000000 jadecobra-0.3.70/tests/test_aws_deploy_lambda.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)     1745 2023-04-03 00:42:01.000000 jadecobra-0.3.70/tests/test_aws_deploy_lambda_function.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)     1869 2023-04-03 00:42:18.000000 jadecobra-0.3.70/tests/test_aws_deploy_lambda_layer.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)      969 2023-04-02 23:59:37.000000 jadecobra-0.3.70/tests/test_aws_lambda.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)     1446 2023-04-02 23:59:37.000000 jadecobra-0.3.70/tests/test_environment.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)      676 2023-04-03 00:32:32.000000 jadecobra-0.3.70/tests/test_jadecobra.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)     5787 2023-05-19 21:31:36.000000 jadecobra-0.3.70/tests/test_jadecobra_tester.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)     1477 2023-04-20 01:08:32.000000 jadecobra-0.3.70/tests/test_jadecobra_toolkit.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)     1949 2023-04-03 02:04:42.000000 jadecobra-0.3.70/tests/test_jadecobra_versioning.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)       72 2023-04-03 02:57:17.000000 jadecobra-0.3.70/tests/test_setup_tdd.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)      977 2023-05-04 15:16:26.000000 jadecobra-0.3.70/tests/test_z_build_publish.py
+drwxr-xr-x   0 johnnyblase   (501) staff       (20)        0 2023-05-24 19:22:02.028380 jadecobra-0.3.71/
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1066 2022-08-18 02:10:38.000000 jadecobra-0.3.71/LICENSE
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1878 2023-05-24 19:22:02.028272 jadecobra-0.3.71/PKG-INFO
+-rw-r--r--   0 johnnyblase   (501) staff       (20)      150 2022-08-29 03:32:29.000000 jadecobra-0.3.71/README.md
+-rw-r--r--   0 johnnyblase   (501) staff       (20)      534 2023-05-24 19:21:51.000000 jadecobra-0.3.71/pyproject.toml
+-rw-r--r--   0 johnnyblase   (501) staff       (20)       38 2023-05-24 19:22:02.028418 jadecobra-0.3.71/setup.cfg
+drwxr-xr-x   0 johnnyblase   (501) staff       (20)        0 2023-05-24 19:22:02.023425 jadecobra-0.3.71/src/
+drwxr-xr-x   0 johnnyblase   (501) staff       (20)        0 2023-05-24 19:22:02.024028 jadecobra-0.3.71/src/None/
+-rw-r--r--   0 johnnyblase   (501) staff       (20)       22 2023-04-20 16:05:17.000000 jadecobra-0.3.71/src/None/__init__.py
+drwxr-xr-x   0 johnnyblase   (501) staff       (20)        0 2023-05-24 19:22:02.024986 jadecobra-0.3.71/src/jadecobra/
+-rw-r--r--   0 johnnyblase   (501) staff       (20)       22 2023-05-24 19:21:51.000000 jadecobra-0.3.71/src/jadecobra/__init__.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1422 2022-08-19 16:12:38.000000 jadecobra-0.3.71/src/jadecobra/aws_environment.py
+drwxr-xr-x   0 johnnyblase   (501) staff       (20)        0 2023-05-24 19:22:02.025801 jadecobra-0.3.71/src/jadecobra/aws_lambda/
+-rw-r--r--   0 johnnyblase   (501) staff       (20)      170 2023-03-29 21:40:49.000000 jadecobra-0.3.71/src/jadecobra/aws_lambda/__init__.py
+drwxr-xr-x   0 johnnyblase   (501) staff       (20)        0 2023-05-24 19:22:02.026449 jadecobra-0.3.71/src/jadecobra/aws_lambda/deploy/
+-rw-r--r--   0 johnnyblase   (501) staff       (20)       27 2022-08-19 16:21:46.000000 jadecobra-0.3.71/src/jadecobra/aws_lambda/deploy/__init__.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1349 2023-03-31 22:22:12.000000 jadecobra-0.3.71/src/jadecobra/aws_lambda/deploy/deploy.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1187 2023-04-02 23:31:34.000000 jadecobra-0.3.71/src/jadecobra/aws_lambda/deploy/deploy_lambda.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1745 2022-08-19 16:21:46.000000 jadecobra-0.3.71/src/jadecobra/aws_lambda/deploy/lambda_function.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     3888 2023-04-28 20:18:57.000000 jadecobra-0.3.71/src/jadecobra/aws_lambda/deploy/lambda_layer.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)       14 2023-01-30 18:47:15.000000 jadecobra-0.3.71/src/jadecobra/cloudformation_deployer.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)        0 2023-03-31 20:02:12.000000 jadecobra-0.3.71/src/jadecobra/setup_tdd.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     5386 2023-05-24 19:20:03.000000 jadecobra-0.3.71/src/jadecobra/tester.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     3265 2023-04-20 18:35:14.000000 jadecobra-0.3.71/src/jadecobra/toolkit.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1947 2023-04-20 18:29:33.000000 jadecobra-0.3.71/src/jadecobra/versioning.py
+drwxr-xr-x   0 johnnyblase   (501) staff       (20)        0 2023-05-24 19:22:02.025662 jadecobra-0.3.71/src/jadecobra.egg-info/
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1878 2023-05-24 19:22:02.000000 jadecobra-0.3.71/src/jadecobra.egg-info/PKG-INFO
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1050 2023-05-24 19:22:02.000000 jadecobra-0.3.71/src/jadecobra.egg-info/SOURCES.txt
+-rw-r--r--   0 johnnyblase   (501) staff       (20)        1 2023-05-24 19:22:02.000000 jadecobra-0.3.71/src/jadecobra.egg-info/dependency_links.txt
+-rw-r--r--   0 johnnyblase   (501) staff       (20)       14 2023-05-24 19:22:02.000000 jadecobra-0.3.71/src/jadecobra.egg-info/requires.txt
+-rw-r--r--   0 johnnyblase   (501) staff       (20)       15 2023-05-24 19:22:02.000000 jadecobra-0.3.71/src/jadecobra.egg-info/top_level.txt
+drwxr-xr-x   0 johnnyblase   (501) staff       (20)        0 2023-05-24 19:22:02.028083 jadecobra-0.3.71/tests/
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1393 2023-04-02 23:59:47.000000 jadecobra-0.3.71/tests/test_aws_deploy_lambda.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1745 2023-04-03 00:42:01.000000 jadecobra-0.3.71/tests/test_aws_deploy_lambda_function.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1869 2023-04-03 00:42:18.000000 jadecobra-0.3.71/tests/test_aws_deploy_lambda_layer.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)      969 2023-04-02 23:59:37.000000 jadecobra-0.3.71/tests/test_aws_lambda.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1446 2023-04-02 23:59:37.000000 jadecobra-0.3.71/tests/test_environment.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)      676 2023-04-03 00:32:32.000000 jadecobra-0.3.71/tests/test_jadecobra.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     5787 2023-05-19 21:31:36.000000 jadecobra-0.3.71/tests/test_jadecobra_tester.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1477 2023-04-20 01:08:32.000000 jadecobra-0.3.71/tests/test_jadecobra_toolkit.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1949 2023-04-03 02:04:42.000000 jadecobra-0.3.71/tests/test_jadecobra_versioning.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)       72 2023-04-03 02:57:17.000000 jadecobra-0.3.71/tests/test_setup_tdd.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)      977 2023-05-04 15:16:26.000000 jadecobra-0.3.71/tests/test_z_build_publish.py
```

### Comparing `jadecobra-0.3.70/LICENSE` & `jadecobra-0.3.71/LICENSE`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.70/PKG-INFO` & `jadecobra-0.3.71/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jadecobra
-Version: 0.3.70
+Version: 0.3.71
 Summary: DRY
 Author-email: johnnyblase <johnnyblasin@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 jadecobra
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `jadecobra-0.3.70/pyproject.toml` & `jadecobra-0.3.71/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "jadecobra"
-version = "0.3.70"
+version = "0.3.71"
 authors = [
   { name="johnnyblase", email="johnnyblasin@gmail.com" },
 ]
 description = "DRY"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.6"
```

### Comparing `jadecobra-0.3.70/src/jadecobra/aws_environment.py` & `jadecobra-0.3.71/src/jadecobra/aws_environment.py`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.70/src/jadecobra/aws_lambda/deploy/deploy.py` & `jadecobra-0.3.71/src/jadecobra/aws_lambda/deploy/deploy.py`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.70/src/jadecobra/aws_lambda/deploy/deploy_lambda.py` & `jadecobra-0.3.71/src/jadecobra/aws_lambda/deploy/deploy_lambda.py`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.70/src/jadecobra/aws_lambda/deploy/lambda_function.py` & `jadecobra-0.3.71/src/jadecobra/aws_lambda/deploy/lambda_function.py`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.70/src/jadecobra/aws_lambda/deploy/lambda_layer.py` & `jadecobra-0.3.71/src/jadecobra/aws_lambda/deploy/lambda_layer.py`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.70/src/jadecobra/tester.py` & `jadecobra-0.3.71/src/jadecobra/tester.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,18 +136,22 @@
             if filter in name
         )
 
     @staticmethod
     def remove_date_created(dictionary):
         resources = dictionary['Resources']
         for resource in resources:
-            tags = resources[resource]['Properties']['Tags']
-            for tag in tags:
-                if tag['Key'] == 'DateCreated':
-                    tags.remove(tag)
+            try:
+                tags = resources[resource]['Properties']['Tags']
+            except KeyError:
+                'nothing to do here'
+            else:
+                for tag in tags:
+                    if tag['Key'] == 'DateCreated':
+                        tags.remove(tag)
 
     def remove_layer_assets(self, dictionary):
         for layer in self.filter_keys(
             dictionary=dictionary.get('Resources'),
             filter='LambdaLayer',
         ):
             try:
```

### Comparing `jadecobra-0.3.70/src/jadecobra/toolkit.py` & `jadecobra-0.3.71/src/jadecobra/toolkit.py`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.70/src/jadecobra/versioning.py` & `jadecobra-0.3.71/src/jadecobra/versioning.py`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.70/src/jadecobra.egg-info/PKG-INFO` & `jadecobra-0.3.71/src/jadecobra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jadecobra
-Version: 0.3.70
+Version: 0.3.71
 Summary: DRY
 Author-email: johnnyblase <johnnyblasin@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 jadecobra
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `jadecobra-0.3.70/src/jadecobra.egg-info/SOURCES.txt` & `jadecobra-0.3.71/src/jadecobra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.70/tests/test_aws_deploy_lambda.py` & `jadecobra-0.3.71/tests/test_aws_deploy_lambda.py`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.70/tests/test_aws_deploy_lambda_function.py` & `jadecobra-0.3.71/tests/test_aws_deploy_lambda_function.py`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.70/tests/test_aws_deploy_lambda_layer.py` & `jadecobra-0.3.71/tests/test_aws_deploy_lambda_layer.py`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.70/tests/test_aws_lambda.py` & `jadecobra-0.3.71/tests/test_aws_lambda.py`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.70/tests/test_environment.py` & `jadecobra-0.3.71/tests/test_environment.py`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.70/tests/test_jadecobra.py` & `jadecobra-0.3.71/tests/test_jadecobra.py`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.70/tests/test_jadecobra_tester.py` & `jadecobra-0.3.71/tests/test_jadecobra_tester.py`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.70/tests/test_jadecobra_toolkit.py` & `jadecobra-0.3.71/tests/test_jadecobra_toolkit.py`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.70/tests/test_jadecobra_versioning.py` & `jadecobra-0.3.71/tests/test_jadecobra_versioning.py`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.70/tests/test_z_build_publish.py` & `jadecobra-0.3.71/tests/test_z_build_publish.py`

 * *Files identical despite different names*

