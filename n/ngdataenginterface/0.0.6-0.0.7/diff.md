# Comparing `tmp/ngdataenginterface-0.0.6.tar.gz` & `tmp/ngdataenginterface-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngdataenginterface-0.0.6.tar", max compression
+gzip compressed data, was "ngdataenginterface-0.0.7.tar", max compression
```

## Comparing `ngdataenginterface-0.0.6.tar` & `ngdataenginterface-0.0.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     2934 2023-05-24 14:11:37.605600 ngdataenginterface-0.0.6/README.md
--rw-r--r--   0        0        0      348 2023-05-24 14:11:37.605600 ngdataenginterface-0.0.6/ngdataenginterface/__init__.py
--rw-r--r--   0        0        0     3598 2023-05-24 14:11:37.605600 ngdataenginterface-0.0.6/ngdataenginterface/analytical.py
--rw-r--r--   0        0        0     3382 2023-05-24 14:11:37.605600 ngdataenginterface-0.0.6/ngdataenginterface/aws_interface.py
--rw-r--r--   0        0        0     2704 2023-05-24 14:11:37.605600 ngdataenginterface-0.0.6/ngdataenginterface/process.py
--rw-r--r--   0        0        0     1816 2023-05-24 14:11:37.605600 ngdataenginterface-0.0.6/ngdataenginterface/spark_manager.py
--rw-r--r--   0        0        0    12412 2023-05-24 14:11:37.606600 ngdataenginterface-0.0.6/ngdataenginterface/table.py
--rw-r--r--   0        0        0     1425 2023-05-24 14:11:37.606600 ngdataenginterface-0.0.6/ngdataenginterface/utils.py
--rw-r--r--   0        0        0      395 2023-05-24 14:11:37.606600 ngdataenginterface-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     3599 1970-01-01 00:00:00.000000 ngdataenginterface-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     2934 2023-05-24 21:21:18.472560 ngdataenginterface-0.0.7/README.md
+-rw-r--r--   0        0        0      348 2023-05-24 21:21:18.472560 ngdataenginterface-0.0.7/ngdataenginterface/__init__.py
+-rw-r--r--   0        0        0     3598 2023-05-24 21:21:18.472560 ngdataenginterface-0.0.7/ngdataenginterface/analytical.py
+-rw-r--r--   0        0        0     3382 2023-05-24 21:21:18.472560 ngdataenginterface-0.0.7/ngdataenginterface/aws_interface.py
+-rw-r--r--   0        0        0     2704 2023-05-24 21:21:18.472560 ngdataenginterface-0.0.7/ngdataenginterface/process.py
+-rw-r--r--   0        0        0     1816 2023-05-24 21:21:18.472560 ngdataenginterface-0.0.7/ngdataenginterface/spark_manager.py
+-rw-r--r--   0        0        0    12412 2023-05-24 21:21:18.472560 ngdataenginterface-0.0.7/ngdataenginterface/table.py
+-rw-r--r--   0        0        0     2046 2023-05-24 21:21:18.472560 ngdataenginterface-0.0.7/ngdataenginterface/utils.py
+-rw-r--r--   0        0        0      395 2023-05-24 21:21:18.472560 ngdataenginterface-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     3599 1970-01-01 00:00:00.000000 ngdataenginterface-0.0.7/PKG-INFO
```

### Comparing `ngdataenginterface-0.0.6/README.md` & `ngdataenginterface-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.0.6/ngdataenginterface/analytical.py` & `ngdataenginterface-0.0.7/ngdataenginterface/analytical.py`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.0.6/ngdataenginterface/aws_interface.py` & `ngdataenginterface-0.0.7/ngdataenginterface/aws_interface.py`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.0.6/ngdataenginterface/process.py` & `ngdataenginterface-0.0.7/ngdataenginterface/process.py`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.0.6/ngdataenginterface/spark_manager.py` & `ngdataenginterface-0.0.7/ngdataenginterface/spark_manager.py`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.0.6/ngdataenginterface/table.py` & `ngdataenginterface-0.0.7/ngdataenginterface/table.py`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.0.6/ngdataenginterface/utils.py` & `ngdataenginterface-0.0.7/ngdataenginterface/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 from pyspark.sql.types import *
+import string
+import re
+from datetime import datetime
 
 
 def handle_pyspark_timestamp_in_schema(pyspark_schema: StructType) -> StructType:
     """Recursive function that modifies StructType pyspark schema field to handle timestamp inconsistency when
     parsing JSON-Schema types.
 
     Parameters
@@ -33,7 +36,24 @@
         # if 'format' is in field metadata key and the value is 'date-time' or 'date'
         # convert field type to TimestampType
         elif "format" in field_metadata.keys():
             field_format = field_metadata["format"]
             if field_format in ("date-time", "date"):
                 field.dataType = TimestampType()
     return pyspark_schema
+
+
+def import_from_custom_package(package_name, variable):
+    # importing variable from custom package
+    return getattr(__import__(package_name), variable)
+
+
+def import_table_current_step_params(params, table, current_step):
+    # importing table current step params from database params
+    return params[table][current_step]
+
+
+def handle_execution_date_args(dt: str):
+    match = re.search(r"(?<=\.).+?(?=\:)", dt)
+    if match:
+        dt = dt.replace(f".{match.group()[:-3]}", "")
+    return datetime.strptime("".join(dt.rsplit(":", 1)), "%Y-%m-%dT%H:%M:%S%z")
```

### Comparing `ngdataenginterface-0.0.6/PKG-INFO` & `ngdataenginterface-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngdataenginterface
-Version: 0.0.6
+Version: 0.0.7
 Summary: A library for facilitating the development of data engineering pipelines
 Author: NG.CASH
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

