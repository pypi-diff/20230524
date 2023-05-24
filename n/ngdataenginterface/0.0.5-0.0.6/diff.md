# Comparing `tmp/ngdataenginterface-0.0.5.tar.gz` & `tmp/ngdataenginterface-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngdataenginterface-0.0.5.tar", max compression
+gzip compressed data, was "ngdataenginterface-0.0.6.tar", max compression
```

## Comparing `ngdataenginterface-0.0.5.tar` & `ngdataenginterface-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,10 @@
--rw-r--r--   0        0        0     2934 2023-05-17 17:25:47.717504 ngdataenginterface-0.0.5/README.md
--rw-r--r--   0        0        0      142 2023-05-17 17:25:47.717504 ngdataenginterface-0.0.5/ngdataenginterface/__init__.py
--rw-r--r--   0        0        0       81 2023-05-17 17:25:47.717504 ngdataenginterface-0.0.5/ngdataenginterface/analytical/__init__.py
--rw-r--r--   0        0        0     2429 2023-05-17 17:25:47.717504 ngdataenginterface-0.0.5/ngdataenginterface/analytical/core.py
--rw-r--r--   0        0        0      320 2023-05-17 17:25:47.717504 ngdataenginterface-0.0.5/ngdataenginterface/core/__init__.py
--rw-r--r--   0        0        0     1716 2023-05-17 17:25:47.717504 ngdataenginterface-0.0.5/ngdataenginterface/core/aws_interface.py
--rw-r--r--   0        0        0     1558 2023-05-17 17:25:47.717504 ngdataenginterface-0.0.5/ngdataenginterface/core/partition.py
--rw-r--r--   0        0        0     5627 2023-05-17 17:25:47.717504 ngdataenginterface-0.0.5/ngdataenginterface/core/read.py
--rw-r--r--   0        0        0     2787 2023-05-17 17:25:47.717504 ngdataenginterface-0.0.5/ngdataenginterface/core/schema.py
--rw-r--r--   0        0        0     6726 2023-05-17 17:25:47.717504 ngdataenginterface-0.0.5/ngdataenginterface/core/utils_emr.py
--rw-r--r--   0        0        0     1424 2023-05-17 17:25:47.717504 ngdataenginterface-0.0.5/ngdataenginterface/core/validations.py
--rw-r--r--   0        0        0     4362 2023-05-17 17:25:47.717504 ngdataenginterface-0.0.5/ngdataenginterface/core/write.py
--rw-r--r--   0        0        0      174 2023-05-17 17:25:47.717504 ngdataenginterface-0.0.5/ngdataenginterface/process/__init__.py
--rw-r--r--   0        0        0     4027 2023-05-17 17:25:47.717504 ngdataenginterface-0.0.5/ngdataenginterface/process/cleansing.py
--rw-r--r--   0        0        0      408 2023-05-17 17:25:47.717504 ngdataenginterface-0.0.5/ngdataenginterface/process/export_redshift.py
--rw-r--r--   0        0        0     6859 2023-05-17 17:25:47.717504 ngdataenginterface-0.0.5/ngdataenginterface/process/pismo.py
--rw-r--r--   0        0        0      395 2023-05-17 17:25:47.717504 ngdataenginterface-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3599 1970-01-01 00:00:00.000000 ngdataenginterface-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     2934 2023-05-24 14:11:37.605600 ngdataenginterface-0.0.6/README.md
+-rw-r--r--   0        0        0      348 2023-05-24 14:11:37.605600 ngdataenginterface-0.0.6/ngdataenginterface/__init__.py
+-rw-r--r--   0        0        0     3598 2023-05-24 14:11:37.605600 ngdataenginterface-0.0.6/ngdataenginterface/analytical.py
+-rw-r--r--   0        0        0     3382 2023-05-24 14:11:37.605600 ngdataenginterface-0.0.6/ngdataenginterface/aws_interface.py
+-rw-r--r--   0        0        0     2704 2023-05-24 14:11:37.605600 ngdataenginterface-0.0.6/ngdataenginterface/process.py
+-rw-r--r--   0        0        0     1816 2023-05-24 14:11:37.605600 ngdataenginterface-0.0.6/ngdataenginterface/spark_manager.py
+-rw-r--r--   0        0        0    12412 2023-05-24 14:11:37.606600 ngdataenginterface-0.0.6/ngdataenginterface/table.py
+-rw-r--r--   0        0        0     1425 2023-05-24 14:11:37.606600 ngdataenginterface-0.0.6/ngdataenginterface/utils.py
+-rw-r--r--   0        0        0      395 2023-05-24 14:11:37.606600 ngdataenginterface-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3599 1970-01-01 00:00:00.000000 ngdataenginterface-0.0.6/PKG-INFO
```

### Comparing `ngdataenginterface-0.0.5/README.md` & `ngdataenginterface-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.0.5/PKG-INFO` & `ngdataenginterface-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngdataenginterface
-Version: 0.0.5
+Version: 0.0.6
 Summary: A library for facilitating the development of data engineering pipelines
 Author: NG.CASH
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

