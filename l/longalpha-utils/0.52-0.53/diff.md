# Comparing `tmp/longalpha_utils-0.52.tar.gz` & `tmp/longalpha_utils-0.53.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "longalpha_utils-0.52.tar", last modified: Mon May 22 20:01:20 2023, max compression
+gzip compressed data, was "longalpha_utils-0.53.tar", last modified: Wed May 24 14:47:48 2023, max compression
```

## Comparing `longalpha_utils-0.52.tar` & `longalpha_utils-0.53.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:01:20.894785 longalpha_utils-0.52/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-22 20:01:20.894785 longalpha_utils-0.52/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:01:20.890784 longalpha_utils-0.52/longalpha_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-22 20:01:07.000000 longalpha_utils-0.52/longalpha_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-22 20:01:07.000000 longalpha_utils-0.52/longalpha_utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-22 20:01:07.000000 longalpha_utils-0.52/longalpha_utils/messenger.py
--rw-r--r--   0 runner    (1001) docker     (123)    11912 2023-05-22 20:01:07.000000 longalpha_utils-0.52/longalpha_utils/transfers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-05-22 20:01:07.000000 longalpha_utils-0.52/longalpha_utils/us_stock_holidays.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-22 20:01:07.000000 longalpha_utils-0.52/longalpha_utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:01:20.894785 longalpha_utils-0.52/longalpha_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-22 20:01:20.000000 longalpha_utils-0.52/longalpha_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-22 20:01:20.000000 longalpha_utils-0.52/longalpha_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 20:01:20.000000 longalpha_utils-0.52/longalpha_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-22 20:01:20.000000 longalpha_utils-0.52/longalpha_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-22 20:01:20.000000 longalpha_utils-0.52/longalpha_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 20:01:20.894785 longalpha_utils-0.52/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-22 20:01:07.000000 longalpha_utils-0.52/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:47:48.782108 longalpha_utils-0.53/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-24 14:47:48.782108 longalpha_utils-0.53/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:47:48.782108 longalpha_utils-0.53/longalpha_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-24 14:47:37.000000 longalpha_utils-0.53/longalpha_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-24 14:47:37.000000 longalpha_utils-0.53/longalpha_utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-24 14:47:37.000000 longalpha_utils-0.53/longalpha_utils/messenger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11912 2023-05-24 14:47:37.000000 longalpha_utils-0.53/longalpha_utils/transfers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-05-24 14:47:37.000000 longalpha_utils-0.53/longalpha_utils/us_stock_holidays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-24 14:47:37.000000 longalpha_utils-0.53/longalpha_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:47:48.782108 longalpha_utils-0.53/longalpha_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-24 14:47:48.000000 longalpha_utils-0.53/longalpha_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-24 14:47:48.000000 longalpha_utils-0.53/longalpha_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 14:47:48.000000 longalpha_utils-0.53/longalpha_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-24 14:47:48.000000 longalpha_utils-0.53/longalpha_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-24 14:47:48.000000 longalpha_utils-0.53/longalpha_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 14:47:48.782108 longalpha_utils-0.53/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-24 14:47:37.000000 longalpha_utils-0.53/setup.py
```

### Comparing `longalpha_utils-0.52/longalpha_utils/messenger.py` & `longalpha_utils-0.53/longalpha_utils/messenger.py`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.52/longalpha_utils/transfers.py` & `longalpha_utils-0.53/longalpha_utils/transfers.py`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.52/longalpha_utils/us_stock_holidays.py` & `longalpha_utils-0.53/longalpha_utils/us_stock_holidays.py`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.52/longalpha_utils/utils.py` & `longalpha_utils-0.53/longalpha_utils/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import datetime
-from typing import List
-
+from typing import List, Optional
+from datetime import date
+import os
 import pandas as pd
 from pyspark.sql import DataFrame
 
 
 def max_pandas_display(pd: pd, max_row: int = 100) -> None:
     """
     set pandas print format to print all
@@ -38,8 +39,25 @@
 
     """
     if len(dfs) == 0:
         raise ValueError("Dataframes list cannot be empty")
     df = dfs[0]
     for i in dfs[1:]:
         df = df.unionByName(i)
-    return df
+    return df
+
+
+def get_s3_path(bucket: str, prefix: str, day: Optional[date]=None):
+    """
+    Get s3 path for a given day
+    Args:
+        bucket:  s3 bucket
+        prefix:  s3 prefix
+        day:  date
+
+    Returns: s3 path
+
+    """
+    if day:
+        return f"s3a://" + os.path.join(bucket, prefix, day.strftime("%Y"), day.strftime("%m"), day.strftime("%d"))
+    else:
+        return f"s3a://" + os.path.join(bucket, prefix)
```

### Comparing `longalpha_utils-0.52/longalpha_utils.egg-info/requires.txt` & `longalpha_utils-0.53/longalpha_utils.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.52/setup.py` & `longalpha_utils-0.53/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,11 +38,11 @@
     "typing_extensions==4.4.0",
     "urllib3==1.26.14",
     "yagmail==0.15.293",
 ]
 
 setup(
     name="longalpha_utils",
-    version="0.52",
+    version="0.53",
     long_description="Shared utilities for long alpha projects",
     install_requires=REQUIREMENTS,
 )
```

