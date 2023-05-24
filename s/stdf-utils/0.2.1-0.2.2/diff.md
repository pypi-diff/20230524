# Comparing `tmp/stdf-utils-0.2.1.tar.gz` & `tmp/stdf-utils-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stdf-utils-0.2.1.tar", last modified: Mon May 22 05:33:13 2023, max compression
+gzip compressed data, was "stdf-utils-0.2.2.tar", last modified: Wed May 24 05:05:09 2023, max compression
```

## Comparing `stdf-utils-0.2.1.tar` & `stdf-utils-0.2.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 05:33:13.653240 stdf-utils-0.2.1/
--rw-rw-rw-   0        0        0     1103 2023-05-16 00:45:08.000000 stdf-utils-0.2.1/LICENSE
--rw-rw-rw-   0        0        0     1340 2023-05-22 05:33:13.652239 stdf-utils-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0       45 2023-05-16 00:45:08.000000 stdf-utils-0.2.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-22 05:33:13.654240 stdf-utils-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1727 2023-05-22 05:32:16.000000 stdf-utils-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-22 05:33:13.573937 stdf-utils-0.2.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-22 05:33:13.613965 stdf-utils-0.2.1/src/stdf_utils/
--rw-rw-rw-   0        0        0      212 2023-05-22 05:24:16.000000 stdf-utils-0.2.1/src/stdf_utils/__init__.py
--rw-rw-rw-   0        0        0      997 2023-05-20 05:29:38.000000 stdf-utils-0.2.1/src/stdf_utils/stdf_patch.py
--rw-rw-rw-   0        0        0     2472 2023-05-22 05:26:05.000000 stdf-utils-0.2.1/src/stdf_utils/stdf_per_part.py
--rw-rw-rw-   0        0        0    27579 2023-05-20 05:25:28.000000 stdf-utils-0.2.1/src/stdf_utils/stdf_record.py
--rw-rw-rw-   0        0        0     2655 2023-05-20 06:45:50.000000 stdf-utils-0.2.1/src/stdf_utils/stdf_to_csv.py
--rw-rw-rw-   0        0        0      503 2023-05-20 04:14:04.000000 stdf-utils-0.2.1/src/stdf_utils/stdf_to_txt.py
--rw-rw-rw-   0        0        0      663 2023-05-20 03:02:13.000000 stdf-utils-0.2.1/src/stdf_utils/util.py
-drwxrwxrwx   0        0        0        0 2023-05-22 05:33:13.627964 stdf-utils-0.2.1/src/stdf_utils.egg-info/
--rw-rw-rw-   0        0        0     1340 2023-05-22 05:33:13.000000 stdf-utils-0.2.1/src/stdf_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      510 2023-05-22 05:33:13.000000 stdf-utils-0.2.1/src/stdf_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 05:33:13.000000 stdf-utils-0.2.1/src/stdf_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-22 05:33:13.000000 stdf-utils-0.2.1/src/stdf_utils.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-22 05:33:13.647965 stdf-utils-0.2.1/tests/
--rw-rw-rw-   0        0        0      728 2023-05-20 06:30:13.000000 stdf-utils-0.2.1/tests/test_stdf_patch.py
--rw-rw-rw-   0        0        0      544 2023-05-22 05:28:49.000000 stdf-utils-0.2.1/tests/test_stdf_per_part.py
--rw-rw-rw-   0        0        0      505 2023-05-20 06:31:39.000000 stdf-utils-0.2.1/tests/test_stdf_record.py
--rw-rw-rw-   0        0        0      677 2023-05-20 07:41:12.000000 stdf-utils-0.2.1/tests/test_stdf_to_csv.py
--rw-rw-rw-   0        0        0      407 2023-05-20 07:24:32.000000 stdf-utils-0.2.1/tests/test_stdf_to_txt.py
+drwxrwxrwx   0        0        0        0 2023-05-24 05:05:09.347051 stdf-utils-0.2.2/
+-rw-rw-rw-   0        0        0     1103 2023-05-16 00:45:08.000000 stdf-utils-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0     1340 2023-05-24 05:05:09.347051 stdf-utils-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0       45 2023-05-16 00:45:08.000000 stdf-utils-0.2.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-24 05:05:09.347051 stdf-utils-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1727 2023-05-24 04:21:18.000000 stdf-utils-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 05:05:09.262487 stdf-utils-0.2.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-24 05:05:09.300182 stdf-utils-0.2.2/src/stdf_utils/
+-rw-rw-rw-   0        0        0      212 2023-05-22 05:24:16.000000 stdf-utils-0.2.2/src/stdf_utils/__init__.py
+-rw-rw-rw-   0        0        0      997 2023-05-20 05:29:38.000000 stdf-utils-0.2.2/src/stdf_utils/stdf_patch.py
+-rw-rw-rw-   0        0        0     2880 2023-05-24 04:59:13.000000 stdf-utils-0.2.2/src/stdf_utils/stdf_per_part.py
+-rw-rw-rw-   0        0        0    27579 2023-05-20 05:25:28.000000 stdf-utils-0.2.2/src/stdf_utils/stdf_record.py
+-rw-rw-rw-   0        0        0     2655 2023-05-20 06:45:50.000000 stdf-utils-0.2.2/src/stdf_utils/stdf_to_csv.py
+-rw-rw-rw-   0        0        0      503 2023-05-20 04:14:04.000000 stdf-utils-0.2.2/src/stdf_utils/stdf_to_txt.py
+-rw-rw-rw-   0        0        0      663 2023-05-20 03:02:13.000000 stdf-utils-0.2.2/src/stdf_utils/util.py
+drwxrwxrwx   0        0        0        0 2023-05-24 05:05:09.315805 stdf-utils-0.2.2/src/stdf_utils.egg-info/
+-rw-rw-rw-   0        0        0     1340 2023-05-24 05:05:09.000000 stdf-utils-0.2.2/src/stdf_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      510 2023-05-24 05:05:09.000000 stdf-utils-0.2.2/src/stdf_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 05:05:09.000000 stdf-utils-0.2.2/src/stdf_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-24 05:05:09.000000 stdf-utils-0.2.2/src/stdf_utils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-24 05:05:09.347051 stdf-utils-0.2.2/tests/
+-rw-rw-rw-   0        0        0      728 2023-05-20 06:30:13.000000 stdf-utils-0.2.2/tests/test_stdf_patch.py
+-rw-rw-rw-   0        0        0      582 2023-05-24 05:03:45.000000 stdf-utils-0.2.2/tests/test_stdf_per_part.py
+-rw-rw-rw-   0        0        0      505 2023-05-20 06:31:39.000000 stdf-utils-0.2.2/tests/test_stdf_record.py
+-rw-rw-rw-   0        0        0      677 2023-05-20 07:41:12.000000 stdf-utils-0.2.2/tests/test_stdf_to_csv.py
+-rw-rw-rw-   0        0        0      407 2023-05-20 07:24:32.000000 stdf-utils-0.2.2/tests/test_stdf_to_txt.py
```

### Comparing `stdf-utils-0.2.1/LICENSE` & `stdf-utils-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `stdf-utils-0.2.1/PKG-INFO` & `stdf-utils-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stdf-utils
-Version: 0.2.1
+Version: 0.2.2
 Summary: stdf file parser and emitter
 Author: Peter JC. Wu
 Author-email: wolf952@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/peterjcwu/stdf-utils
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `stdf-utils-0.2.1/setup.py` & `stdf-utils-0.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 NAME = 'stdf-utils'
-VERSION = '0.2.1'
+VERSION = '0.2.2'
 DESCRIPTION = 'stdf file parser and emitter'
 LONG_DESCRIPTION = """\
 stdf is the standard format of ATE result, and this pacakge supports
 reading and (possibly) editing the stdf file comes form ATE.
 """
 AUTHOR = "Peter JC. Wu"
 AUTHOR_EMAIL = "wolf952@gmail.com"
```

### Comparing `stdf-utils-0.2.1/src/stdf_utils/stdf_patch.py` & `stdf-utils-0.2.2/src/stdf_utils/stdf_patch.py`

 * *Files identical despite different names*

### Comparing `stdf-utils-0.2.1/src/stdf_utils/stdf_per_part.py` & `stdf-utils-0.2.2/src/stdf_utils/stdf_per_part.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import os.path
 from collections import defaultdict
+from datetime import datetime
 from copy import copy
 from .stdf_record import StdfRecord
 from .util import OpenFile
 
 
 class StdfPerPart:
-    def __init__(self,
-                 stdf_path: str,
-                 ptr_filter=None,
-                 ptr_extra_fields=None,
-                 extra_handler=None):
+    def __init__(self, stdf_path: str, ptr_filter=None,
+                 ptr_extra_fields=None, extra_handler=None):
+
         self.stdf_path = stdf_path
         self.ptr_filter = ptr_filter or (lambda d: True)
         self.ptr_extra_fields = ptr_extra_fields or (lambda d: {})
         self.previous_rec: dict = {}
         self.handlers = {
             "Mir": self.mir_handler,
             "Ptr": self.ptr_handler,
             "Prr": self.prr_handler,
+            "Mrr": self.mrr_handler,
             **(extra_handler or {}),
         }
         # cache
         self.mir = {}
         self.prr = {}
         self.ptr = defaultdict(list)
 
@@ -37,20 +37,27 @@
                 if rec_type == "Prr":
                     site = self.prr["site"]
                     yield {
                         "mir": copy(self.mir),
                         "prr": copy(self.prr),
                         "ptr": self.ptr.pop(site) if site in self.ptr else [],
                     }
+                elif rec_type == "Mrr":
+                    yield {
+                        "mir": copy(self.mir),
+                        "prr": {},
+                        "ptr": [],
+                    }
 
     def mir_handler(self, d: dict) -> None:
         self.mir = {
             "node": d["NODE_NAM"].decode(),
             "job": d["JOB_NAM"].decode().split("/")[-1].replace(".prog", ""),
             "name": os.path.basename(self.stdf_path).split(".")[0],
+            "start_t": datetime.fromtimestamp(d["START_T"])
         }
 
     def ptr_handler(self, d: dict) -> None:
         site: int = d["SITE_NUM"]
         if self.ptr_filter(d):
             self.ptr[site].append({
                 "t_num": d["TEST_NUM"],
@@ -67,7 +74,10 @@
             "part_id": d["PART_ID"].decode(),
             "site": d["SITE_NUM"],
             "x": d["X_COORD"],
             "y": d["Y_COORD"],
             "sb": d["SOFT_BIN"],
             "hb": d["HARD_BIN"],
         }
+
+    def mrr_handler(self, d: dict) -> None:
+        self.mir["finish_t"] = datetime.fromtimestamp(d["FINISH_T"])
```

### Comparing `stdf-utils-0.2.1/src/stdf_utils/stdf_record.py` & `stdf-utils-0.2.2/src/stdf_utils/stdf_record.py`

 * *Files identical despite different names*

### Comparing `stdf-utils-0.2.1/src/stdf_utils/stdf_to_csv.py` & `stdf-utils-0.2.2/src/stdf_utils/stdf_to_csv.py`

 * *Files identical despite different names*

### Comparing `stdf-utils-0.2.1/src/stdf_utils/util.py` & `stdf-utils-0.2.2/src/stdf_utils/util.py`

 * *Files identical despite different names*

### Comparing `stdf-utils-0.2.1/src/stdf_utils.egg-info/PKG-INFO` & `stdf-utils-0.2.2/src/stdf_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stdf-utils
-Version: 0.2.1
+Version: 0.2.2
 Summary: stdf file parser and emitter
 Author: Peter JC. Wu
 Author-email: wolf952@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/peterjcwu/stdf-utils
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `stdf-utils-0.2.1/tests/test_stdf_patch.py` & `stdf-utils-0.2.2/tests/test_stdf_patch.py`

 * *Files identical despite different names*

### Comparing `stdf-utils-0.2.1/tests/test_stdf_per_part.py` & `stdf-utils-0.2.2/tests/test_stdf_per_part.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 class TestStdfPerTd(TestCase):
     def setUp(self) -> None:
         self.f = os.path.abspath(os.path.join(__file__, os.pardir, "data", "lot2.stdf.gz"))
 
     def test_stdf_per_td(self):
-        for td in StdfPerPart(self.f, extra_handler={"Mrr": self.mrr_handler}):
-            assert "mir" in td.keys()
-            assert "prr" in td.keys()
-            assert "ptr" in td.keys()
-
-    @staticmethod
-    def mrr_handler(d):
-        print(d)
+        last_td = {}
+        for td in StdfPerPart(self.f):
+            last_td = td
+            self.assertIn("mir", td.keys())
+            self.assertIn("prr", td.keys())
+            self.assertIn("ptr", td.keys())
+        else:
+            self.assertIn("finish_t", last_td["mir"].keys())
```

### Comparing `stdf-utils-0.2.1/tests/test_stdf_to_csv.py` & `stdf-utils-0.2.2/tests/test_stdf_to_csv.py`

 * *Files identical despite different names*

