# Comparing `tmp/xerparser-0.9.7.tar.gz` & `tmp/xerparser-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xerparser-0.9.7.tar", max compression
+gzip compressed data, was "xerparser-0.9.8.tar", max compression
```

## Comparing `xerparser-0.9.7.tar` & `xerparser-0.9.8.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0    35149 2022-12-03 05:25:25.921903 xerparser-0.9.7/LICENSE
--rw-r--r--   0        0        0     5337 2023-04-19 13:53:53.195483 xerparser-0.9.7/README.md
--rw-r--r--   0        0        0      743 2023-05-24 13:28:30.701948 xerparser-0.9.7/pyproject.toml
--rw-r--r--   0        0        0      962 2023-05-24 13:28:30.701948 xerparser-0.9.7/xerparser/__init__.py
--rw-r--r--   0        0        0      465 2023-03-01 00:04:03.499449 xerparser-0.9.7/xerparser/schemas/__init__.py
--rw-r--r--   0        0        0     2643 2023-03-01 00:04:28.289431 xerparser-0.9.7/xerparser/schemas/account.py
--rw-r--r--   0        0        0     3247 2023-02-06 03:09:28.587242 xerparser-0.9.7/xerparser/schemas/actvcode.py
--rw-r--r--   0        0        0     1547 2023-01-25 01:32:05.201004 xerparser-0.9.7/xerparser/schemas/actvtype.py
--rw-r--r--   0        0        0    11154 2023-03-01 03:39:04.104780 xerparser-0.9.7/xerparser/schemas/calendars.py
--rw-r--r--   0        0        0      957 2023-03-01 00:04:28.289431 xerparser-0.9.7/xerparser/schemas/ermhdr.py
--rw-r--r--   0        0        0     1367 2023-01-25 01:32:05.211004 xerparser-0.9.7/xerparser/schemas/findates.py
--rw-r--r--   0        0        0      749 2023-01-16 21:15:50.835852 xerparser-0.9.7/xerparser/schemas/memotype.py
--rw-r--r--   0        0        0     1094 2023-02-26 04:48:17.672946 xerparser-0.9.7/xerparser/schemas/pcattype.py
--rw-r--r--   0        0        0     3227 2023-02-26 04:48:17.672946 xerparser-0.9.7/xerparser/schemas/pcatval.py
--rw-r--r--   0        0        0     9136 2023-05-14 15:40:28.944059 xerparser-0.9.7/xerparser/schemas/project.py
--rw-r--r--   0        0        0     2897 2023-03-01 00:04:03.499449 xerparser-0.9.7/xerparser/schemas/projwbs.py
--rw-r--r--   0        0        0     1103 2023-03-01 00:04:03.499449 xerparser-0.9.7/xerparser/schemas/rsrc.py
--rw-r--r--   0        0        0     2970 2023-03-01 00:04:28.289431 xerparser-0.9.7/xerparser/schemas/schedoptions.py
--rw-r--r--   0        0        0    16706 2023-05-24 13:28:30.701948 xerparser-0.9.7/xerparser/schemas/task.py
--rw-r--r--   0        0        0     1462 2023-03-06 00:43:40.451659 xerparser-0.9.7/xerparser/schemas/taskfin.py
--rw-r--r--   0        0        0      805 2022-12-26 20:40:30.667590 xerparser-0.9.7/xerparser/schemas/taskmemo.py
--rw-r--r--   0        0        0     2019 2023-01-25 01:32:05.211004 xerparser-0.9.7/xerparser/schemas/taskpred.py
--rw-r--r--   0        0        0     5063 2023-03-17 20:28:16.137376 xerparser-0.9.7/xerparser/schemas/taskrsrc.py
--rw-r--r--   0        0        0     1927 2023-01-25 01:32:05.211004 xerparser-0.9.7/xerparser/schemas/trsrcfin.py
--rw-r--r--   0        0        0     1524 2023-03-01 00:04:03.499449 xerparser-0.9.7/xerparser/schemas/udftype.py
--rw-r--r--   0        0        0        0 2022-12-21 14:16:15.278744 xerparser-0.9.7/xerparser/scripts/__init__.py
--rw-r--r--   0        0        0     1548 2022-12-30 22:42:20.878909 xerparser-0.9.7/xerparser/scripts/dates.py
--rw-r--r--   0        0        0      402 2023-01-25 01:32:05.211004 xerparser-0.9.7/xerparser/scripts/decorators.py
--rw-r--r--   0        0        0        0 2022-12-21 14:16:15.278744 xerparser-0.9.7/xerparser/src/__init__.py
--rw-r--r--   0        0        0     2851 2023-04-08 15:29:35.029582 xerparser-0.9.7/xerparser/src/errors.py
--rw-r--r--   0        0        0     2377 2023-04-08 15:29:35.029582 xerparser-0.9.7/xerparser/src/parser.py
--rw-r--r--   0        0        0      769 2023-04-08 15:29:35.029582 xerparser-0.9.7/xerparser/src/validators.py
--rw-r--r--   0        0        0    10822 2023-05-14 15:40:28.944059 xerparser-0.9.7/xerparser/src/xer.py
--rw-r--r--   0        0        0     6062 1970-01-01 00:00:00.000000 xerparser-0.9.7/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-12-03 05:25:25.921903 xerparser-0.9.8/LICENSE
+-rw-r--r--   0        0        0     5337 2023-04-19 13:53:53.195483 xerparser-0.9.8/README.md
+-rw-r--r--   0        0        0      743 2023-05-24 14:27:09.133625 xerparser-0.9.8/pyproject.toml
+-rw-r--r--   0        0        0      962 2023-05-24 14:29:38.233531 xerparser-0.9.8/xerparser/__init__.py
+-rw-r--r--   0        0        0      465 2023-03-01 00:04:03.499449 xerparser-0.9.8/xerparser/schemas/__init__.py
+-rw-r--r--   0        0        0     2643 2023-03-01 00:04:28.289431 xerparser-0.9.8/xerparser/schemas/account.py
+-rw-r--r--   0        0        0     3247 2023-02-06 03:09:28.587242 xerparser-0.9.8/xerparser/schemas/actvcode.py
+-rw-r--r--   0        0        0     1547 2023-01-25 01:32:05.201004 xerparser-0.9.8/xerparser/schemas/actvtype.py
+-rw-r--r--   0        0        0    11154 2023-03-01 03:39:04.104780 xerparser-0.9.8/xerparser/schemas/calendars.py
+-rw-r--r--   0        0        0      957 2023-03-01 00:04:28.289431 xerparser-0.9.8/xerparser/schemas/ermhdr.py
+-rw-r--r--   0        0        0     1367 2023-01-25 01:32:05.211004 xerparser-0.9.8/xerparser/schemas/findates.py
+-rw-r--r--   0        0        0      749 2023-01-16 21:15:50.835852 xerparser-0.9.8/xerparser/schemas/memotype.py
+-rw-r--r--   0        0        0     1094 2023-02-26 04:48:17.672946 xerparser-0.9.8/xerparser/schemas/pcattype.py
+-rw-r--r--   0        0        0     3227 2023-02-26 04:48:17.672946 xerparser-0.9.8/xerparser/schemas/pcatval.py
+-rw-r--r--   0        0        0     9136 2023-05-14 15:40:28.944059 xerparser-0.9.8/xerparser/schemas/project.py
+-rw-r--r--   0        0        0     2897 2023-03-01 00:04:03.499449 xerparser-0.9.8/xerparser/schemas/projwbs.py
+-rw-r--r--   0        0        0     1103 2023-03-01 00:04:03.499449 xerparser-0.9.8/xerparser/schemas/rsrc.py
+-rw-r--r--   0        0        0     2970 2023-03-01 00:04:28.289431 xerparser-0.9.8/xerparser/schemas/schedoptions.py
+-rw-r--r--   0        0        0    16706 2023-05-24 13:28:30.701948 xerparser-0.9.8/xerparser/schemas/task.py
+-rw-r--r--   0        0        0     1462 2023-03-06 00:43:40.451659 xerparser-0.9.8/xerparser/schemas/taskfin.py
+-rw-r--r--   0        0        0      805 2022-12-26 20:40:30.667590 xerparser-0.9.8/xerparser/schemas/taskmemo.py
+-rw-r--r--   0        0        0     2039 2023-05-24 14:27:09.133625 xerparser-0.9.8/xerparser/schemas/taskpred.py
+-rw-r--r--   0        0        0     5063 2023-03-17 20:28:16.137376 xerparser-0.9.8/xerparser/schemas/taskrsrc.py
+-rw-r--r--   0        0        0     1927 2023-01-25 01:32:05.211004 xerparser-0.9.8/xerparser/schemas/trsrcfin.py
+-rw-r--r--   0        0        0     1524 2023-03-01 00:04:03.499449 xerparser-0.9.8/xerparser/schemas/udftype.py
+-rw-r--r--   0        0        0        0 2022-12-21 14:16:15.278744 xerparser-0.9.8/xerparser/scripts/__init__.py
+-rw-r--r--   0        0        0     1548 2022-12-30 22:42:20.878909 xerparser-0.9.8/xerparser/scripts/dates.py
+-rw-r--r--   0        0        0      402 2023-01-25 01:32:05.211004 xerparser-0.9.8/xerparser/scripts/decorators.py
+-rw-r--r--   0        0        0        0 2022-12-21 14:16:15.278744 xerparser-0.9.8/xerparser/src/__init__.py
+-rw-r--r--   0        0        0     2851 2023-04-08 15:29:35.029582 xerparser-0.9.8/xerparser/src/errors.py
+-rw-r--r--   0        0        0     2377 2023-04-08 15:29:35.029582 xerparser-0.9.8/xerparser/src/parser.py
+-rw-r--r--   0        0        0      883 2023-05-24 14:27:09.133625 xerparser-0.9.8/xerparser/src/validators.py
+-rw-r--r--   0        0        0    10822 2023-05-14 15:40:28.944059 xerparser-0.9.8/xerparser/src/xer.py
+-rw-r--r--   0        0        0     6062 1970-01-01 00:00:00.000000 xerparser-0.9.8/PKG-INFO
```

### Comparing `xerparser-0.9.7/LICENSE` & `xerparser-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.7/README.md` & `xerparser-0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.7/pyproject.toml` & `xerparser-0.9.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xerparser"
-version = "0.9.7"
+version = "0.9.8"
 description = "Parse a P6 .xer file to a Python object."
 authors = ["Jesse <code@seqmanagement.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 keywords = ["primavera", "p6", "xer", "schedule", "scheduling", "planning", "project management", "project controls"]
 repository = "https://github.com/jjCode01/xerparser"
```

### Comparing `xerparser-0.9.7/xerparser/__init__.py` & `xerparser-0.9.8/xerparser/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.9.7"
+__version__ = "0.9.8"
 
 from xerparser.src.errors import find_xer_errors, CorruptXerFile
 from xerparser.src.parser import parser, file_reader
 from xerparser.src.xer import Xer
 from xerparser.schemas.actvcode import ACTVCODE
 from xerparser.schemas.actvtype import ACTVTYPE
 from xerparser.schemas.calendars import CALENDAR
```

### Comparing `xerparser-0.9.7/xerparser/schemas/account.py` & `xerparser-0.9.8/xerparser/schemas/account.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.7/xerparser/schemas/actvcode.py` & `xerparser-0.9.8/xerparser/schemas/actvcode.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.7/xerparser/schemas/actvtype.py` & `xerparser-0.9.8/xerparser/schemas/actvtype.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.7/xerparser/schemas/calendars.py` & `xerparser-0.9.8/xerparser/schemas/calendars.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.7/xerparser/schemas/ermhdr.py` & `xerparser-0.9.8/xerparser/schemas/ermhdr.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.7/xerparser/schemas/findates.py` & `xerparser-0.9.8/xerparser/schemas/findates.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.7/xerparser/schemas/memotype.py` & `xerparser-0.9.8/xerparser/schemas/memotype.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.7/xerparser/schemas/pcattype.py` & `xerparser-0.9.8/xerparser/schemas/pcattype.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.7/xerparser/schemas/pcatval.py` & `xerparser-0.9.8/xerparser/schemas/pcatval.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.7/xerparser/schemas/project.py` & `xerparser-0.9.8/xerparser/schemas/project.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.7/xerparser/schemas/projwbs.py` & `xerparser-0.9.8/xerparser/schemas/projwbs.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.7/xerparser/schemas/rsrc.py` & `xerparser-0.9.8/xerparser/schemas/rsrc.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.7/xerparser/schemas/schedoptions.py` & `xerparser-0.9.8/xerparser/schemas/schedoptions.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.7/xerparser/schemas/task.py` & `xerparser-0.9.8/xerparser/schemas/task.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.7/xerparser/schemas/taskfin.py` & `xerparser-0.9.8/xerparser/schemas/taskfin.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.7/xerparser/schemas/taskmemo.py` & `xerparser-0.9.8/xerparser/schemas/taskmemo.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.7/xerparser/schemas/taskpred.py` & `xerparser-0.9.8/xerparser/schemas/taskpred.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 # xerparser
 # taskpred.py
 
 from datetime import datetime
 from xerparser.schemas.task import TASK
-from xerparser.src.validators import int_or_none, datetime_or_none
+from xerparser.src.validators import int_or_none, datetime_or_none, int_or_zero
 
 
 class TASKPRED:
     """
     A class to represent a relationship between two activities.
 
     """
 
     def __init__(self, predecessor: TASK, successor: TASK, **data) -> None:
-
         self.uid: str = data["task_pred_id"]
         self.task_id: str = data["task_id"]
         self.pred_task_id: str = data["pred_task_id"]
         self.proj_id: str = data["proj_id"]
         self.pred_proj_id: str = data["pred_proj_id"]
         self.pred_type: str = data["pred_type"]
-        self.lag_hr_cnt: int = int(data["lag_hr_cnt"])
+        self.lag_hr_cnt: int = int_or_zero(data["lag_hr_cnt"])
         self.float_path: int | None = int_or_none(data["float_path"])
         self.aref: datetime | None = datetime_or_none(data["aref"])
         self.arls: datetime | None = datetime_or_none(data["arls"])
         self.predecessor: TASK = predecessor
         self.successor: TASK = successor
 
     def __eq__(self, __o: "TASKPRED") -> bool:
```

### Comparing `xerparser-0.9.7/xerparser/schemas/taskrsrc.py` & `xerparser-0.9.8/xerparser/schemas/taskrsrc.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.7/xerparser/schemas/trsrcfin.py` & `xerparser-0.9.8/xerparser/schemas/trsrcfin.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.7/xerparser/schemas/udftype.py` & `xerparser-0.9.8/xerparser/schemas/udftype.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.7/xerparser/scripts/dates.py` & `xerparser-0.9.8/xerparser/scripts/dates.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.7/xerparser/src/errors.py` & `xerparser-0.9.8/xerparser/src/errors.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.7/xerparser/src/parser.py` & `xerparser-0.9.8/xerparser/src/parser.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.7/xerparser/src/validators.py` & `xerparser-0.9.8/xerparser/src/validators.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,9 +27,15 @@
 
 def int_or_none(value: str) -> int | None:
     if value == "" or value is None:
         return None
     return int(value)
 
 
+def int_or_zero(value: str) -> int:
+    if value == "" or value is None:
+        return 0
+    return int(value)
+
+
 def str_or_none(value: str) -> str | None:
     return (value, None)[value == ""]
```

### Comparing `xerparser-0.9.7/xerparser/src/xer.py` & `xerparser-0.9.8/xerparser/src/xer.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.7/PKG-INFO` & `xerparser-0.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xerparser
-Version: 0.9.7
+Version: 0.9.8
 Summary: Parse a P6 .xer file to a Python object.
 Home-page: https://github.com/jjCode01/xerparser
 License: GPL-3.0-only
 Keywords: primavera,p6,xer,schedule,scheduling,planning,project management,project controls
 Author: Jesse
 Author-email: code@seqmanagement.com
 Requires-Python: >=3.10,<4.0
```

