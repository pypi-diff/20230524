# Comparing `tmp/cdk-backup-plan-0.0.4.tar.gz` & `tmp/cdk-backup-plan-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-backup-plan-0.0.4.tar", last modified: Wed Feb 22 15:57:13 2023, max compression
+gzip compressed data, was "cdk-backup-plan-0.0.5.tar", last modified: Wed May 17 16:27:19 2023, max compression
```

## Comparing `cdk-backup-plan-0.0.4.tar` & `cdk-backup-plan-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 15:57:13.449610 cdk-backup-plan-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-02-22 15:56:57.000000 cdk-backup-plan-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-22 15:56:57.000000 cdk-backup-plan-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-02-22 15:57:13.449610 cdk-backup-plan-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-02-22 15:56:57.000000 cdk-backup-plan-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-02-22 15:56:57.000000 cdk-backup-plan-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-22 15:57:13.449610 cdk-backup-plan-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-02-22 15:56:57.000000 cdk-backup-plan-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 15:57:13.449610 cdk-backup-plan-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 15:57:13.449610 cdk-backup-plan-0.0.4/src/cdk_backup_plan/
--rw-r--r--   0 runner    (1001) docker     (123)    14511 2023-02-22 15:56:57.000000 cdk-backup-plan-0.0.4/src/cdk_backup_plan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 15:57:13.449610 cdk-backup-plan-0.0.4/src/cdk_backup_plan/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-02-22 15:56:57.000000 cdk-backup-plan-0.0.4/src/cdk_backup_plan/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17513 2023-02-22 15:56:57.000000 cdk-backup-plan-0.0.4/src/cdk_backup_plan/_jsii/cdk-backup-plan@0.0.4.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 15:56:57.000000 cdk-backup-plan-0.0.4/src/cdk_backup_plan/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 15:57:13.449610 cdk-backup-plan-0.0.4/src/cdk_backup_plan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-02-22 15:57:12.000000 cdk-backup-plan-0.0.4/src/cdk_backup_plan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-02-22 15:57:13.000000 cdk-backup-plan-0.0.4/src/cdk_backup_plan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 15:57:12.000000 cdk-backup-plan-0.0.4/src/cdk_backup_plan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-02-22 15:57:13.000000 cdk-backup-plan-0.0.4/src/cdk_backup_plan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-22 15:57:13.000000 cdk-backup-plan-0.0.4/src/cdk_backup_plan.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:27:19.126893 cdk-backup-plan-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-17 16:27:06.000000 cdk-backup-plan-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-17 16:27:06.000000 cdk-backup-plan-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-05-17 16:27:19.126893 cdk-backup-plan-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-05-17 16:27:06.000000 cdk-backup-plan-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-17 16:27:06.000000 cdk-backup-plan-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 16:27:19.126893 cdk-backup-plan-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-17 16:27:06.000000 cdk-backup-plan-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:27:19.122892 cdk-backup-plan-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:27:19.126893 cdk-backup-plan-0.0.5/src/cdk_backup_plan/
+-rw-r--r--   0 runner    (1001) docker     (123)    14511 2023-05-17 16:27:06.000000 cdk-backup-plan-0.0.5/src/cdk_backup_plan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:27:19.126893 cdk-backup-plan-0.0.5/src/cdk_backup_plan/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-17 16:27:06.000000 cdk-backup-plan-0.0.5/src/cdk_backup_plan/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16920 2023-05-17 16:27:06.000000 cdk-backup-plan-0.0.5/src/cdk_backup_plan/_jsii/cdk-backup-plan@0.0.5.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 16:27:06.000000 cdk-backup-plan-0.0.5/src/cdk_backup_plan/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:27:19.126893 cdk-backup-plan-0.0.5/src/cdk_backup_plan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-05-17 16:27:19.000000 cdk-backup-plan-0.0.5/src/cdk_backup_plan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-17 16:27:19.000000 cdk-backup-plan-0.0.5/src/cdk_backup_plan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 16:27:19.000000 cdk-backup-plan-0.0.5/src/cdk_backup_plan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-17 16:27:19.000000 cdk-backup-plan-0.0.5/src/cdk_backup_plan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-17 16:27:19.000000 cdk-backup-plan-0.0.5/src/cdk_backup_plan.egg-info/top_level.txt
```

### Comparing `cdk-backup-plan-0.0.4/LICENSE` & `cdk-backup-plan-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-backup-plan-0.0.4/PKG-INFO` & `cdk-backup-plan-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cdk-backup-plan
-Version: 0.0.4
+Version: 0.0.5
 Summary: CDK construct to create AWS Backup Plans
 Home-page: https://github.com/aws-samples/cdk-backup-plan.git
 Author: Mauricio Villaescusa<maurovc@amazon.com>
 License: MIT-0
 Project-URL: Source, https://github.com/aws-samples/cdk-backup-plan.git
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -94,9 +94,7 @@
     backup_completion_window=Duration.hours(2),
     resources=[bk.BackupResource.from_rds_database_instance(db)],
 )
 # ...
 ```
 
 > **NOTE:** [Tagging](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_backup.BackupResource.html#static-fromwbrtagkey-value-operation) and/or [ARN](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_backup.BackupResource.html#static-fromwbrarnarn) can be used to reference resources not directly available in the [static methods section](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_backup.BackupResource.html#methods).
-
-
```

### Comparing `cdk-backup-plan-0.0.4/README.md` & `cdk-backup-plan-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `cdk-backup-plan-0.0.4/setup.py` & `cdk-backup-plan-0.0.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-backup-plan",
-    "version": "0.0.4",
+    "version": "0.0.5",
     "description": "CDK construct to create AWS Backup Plans",
     "license": "MIT-0",
     "url": "https://github.com/aws-samples/cdk-backup-plan.git",
     "long_description_content_type": "text/markdown",
     "author": "Mauricio Villaescusa<maurovc@amazon.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,37 +22,38 @@
     },
     "packages": [
         "cdk_backup_plan",
         "cdk_backup_plan._jsii"
     ],
     "package_data": {
         "cdk_backup_plan._jsii": [
-            "cdk-backup-plan@0.0.4.jsii.tgz"
+            "cdk-backup-plan@0.0.5.jsii.tgz"
         ],
         "cdk_backup_plan": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "aws-cdk-lib>=2.49.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.73.0, <2.0.0",
+        "jsii>=1.81.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved"
     ],
     "scripts": []
 }
 """
```

### Comparing `cdk-backup-plan-0.0.4/src/cdk_backup_plan/__init__.py` & `cdk-backup-plan-0.0.5/src/cdk_backup_plan/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-backup-plan-0.0.4/src/cdk_backup_plan.egg-info/PKG-INFO` & `cdk-backup-plan-0.0.5/src/cdk_backup_plan.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cdk-backup-plan
-Version: 0.0.4
+Version: 0.0.5
 Summary: CDK construct to create AWS Backup Plans
 Home-page: https://github.com/aws-samples/cdk-backup-plan.git
 Author: Mauricio Villaescusa<maurovc@amazon.com>
 License: MIT-0
 Project-URL: Source, https://github.com/aws-samples/cdk-backup-plan.git
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -94,9 +94,7 @@
     backup_completion_window=Duration.hours(2),
     resources=[bk.BackupResource.from_rds_database_instance(db)],
 )
 # ...
 ```
 
 > **NOTE:** [Tagging](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_backup.BackupResource.html#static-fromwbrtagkey-value-operation) and/or [ARN](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_backup.BackupResource.html#static-fromwbrarnarn) can be used to reference resources not directly available in the [static methods section](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_backup.BackupResource.html#methods).
-
-
```

