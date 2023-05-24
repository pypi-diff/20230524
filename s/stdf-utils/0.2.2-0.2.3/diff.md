# Comparing `tmp/stdf-utils-0.2.2.tar.gz` & `tmp/stdf-utils-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stdf-utils-0.2.2.tar", last modified: Wed May 24 05:05:09 2023, max compression
+gzip compressed data, was "stdf-utils-0.2.3.tar", last modified: Wed May 24 07:18:17 2023, max compression
```

## Comparing `stdf-utils-0.2.2.tar` & `stdf-utils-0.2.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 05:05:09.347051 stdf-utils-0.2.2/
--rw-rw-rw-   0        0        0     1103 2023-05-16 00:45:08.000000 stdf-utils-0.2.2/LICENSE
--rw-rw-rw-   0        0        0     1340 2023-05-24 05:05:09.347051 stdf-utils-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0       45 2023-05-16 00:45:08.000000 stdf-utils-0.2.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-24 05:05:09.347051 stdf-utils-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1727 2023-05-24 04:21:18.000000 stdf-utils-0.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-24 05:05:09.262487 stdf-utils-0.2.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-24 05:05:09.300182 stdf-utils-0.2.2/src/stdf_utils/
--rw-rw-rw-   0        0        0      212 2023-05-22 05:24:16.000000 stdf-utils-0.2.2/src/stdf_utils/__init__.py
--rw-rw-rw-   0        0        0      997 2023-05-20 05:29:38.000000 stdf-utils-0.2.2/src/stdf_utils/stdf_patch.py
--rw-rw-rw-   0        0        0     2880 2023-05-24 04:59:13.000000 stdf-utils-0.2.2/src/stdf_utils/stdf_per_part.py
--rw-rw-rw-   0        0        0    27579 2023-05-20 05:25:28.000000 stdf-utils-0.2.2/src/stdf_utils/stdf_record.py
--rw-rw-rw-   0        0        0     2655 2023-05-20 06:45:50.000000 stdf-utils-0.2.2/src/stdf_utils/stdf_to_csv.py
--rw-rw-rw-   0        0        0      503 2023-05-20 04:14:04.000000 stdf-utils-0.2.2/src/stdf_utils/stdf_to_txt.py
--rw-rw-rw-   0        0        0      663 2023-05-20 03:02:13.000000 stdf-utils-0.2.2/src/stdf_utils/util.py
-drwxrwxrwx   0        0        0        0 2023-05-24 05:05:09.315805 stdf-utils-0.2.2/src/stdf_utils.egg-info/
--rw-rw-rw-   0        0        0     1340 2023-05-24 05:05:09.000000 stdf-utils-0.2.2/src/stdf_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      510 2023-05-24 05:05:09.000000 stdf-utils-0.2.2/src/stdf_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 05:05:09.000000 stdf-utils-0.2.2/src/stdf_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-24 05:05:09.000000 stdf-utils-0.2.2/src/stdf_utils.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-24 05:05:09.347051 stdf-utils-0.2.2/tests/
--rw-rw-rw-   0        0        0      728 2023-05-20 06:30:13.000000 stdf-utils-0.2.2/tests/test_stdf_patch.py
--rw-rw-rw-   0        0        0      582 2023-05-24 05:03:45.000000 stdf-utils-0.2.2/tests/test_stdf_per_part.py
--rw-rw-rw-   0        0        0      505 2023-05-20 06:31:39.000000 stdf-utils-0.2.2/tests/test_stdf_record.py
--rw-rw-rw-   0        0        0      677 2023-05-20 07:41:12.000000 stdf-utils-0.2.2/tests/test_stdf_to_csv.py
--rw-rw-rw-   0        0        0      407 2023-05-20 07:24:32.000000 stdf-utils-0.2.2/tests/test_stdf_to_txt.py
+drwxrwxrwx   0        0        0        0 2023-05-24 07:18:17.862238 stdf-utils-0.2.3/
+-rw-rw-rw-   0        0        0     1103 2023-05-16 00:45:08.000000 stdf-utils-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0     1340 2023-05-24 07:18:17.860195 stdf-utils-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0       45 2023-05-16 00:45:08.000000 stdf-utils-0.2.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-24 07:18:17.862238 stdf-utils-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1727 2023-05-24 07:16:43.000000 stdf-utils-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 07:18:17.773191 stdf-utils-0.2.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-24 07:18:17.813191 stdf-utils-0.2.3/src/stdf_utils/
+-rw-rw-rw-   0        0        0      212 2023-05-22 05:24:16.000000 stdf-utils-0.2.3/src/stdf_utils/__init__.py
+-rw-rw-rw-   0        0        0      997 2023-05-20 05:29:38.000000 stdf-utils-0.2.3/src/stdf_utils/stdf_patch.py
+-rw-rw-rw-   0        0        0     2885 2023-05-24 07:16:14.000000 stdf-utils-0.2.3/src/stdf_utils/stdf_per_part.py
+-rw-rw-rw-   0        0        0    27579 2023-05-20 05:25:28.000000 stdf-utils-0.2.3/src/stdf_utils/stdf_record.py
+-rw-rw-rw-   0        0        0     2655 2023-05-20 06:45:50.000000 stdf-utils-0.2.3/src/stdf_utils/stdf_to_csv.py
+-rw-rw-rw-   0        0        0      503 2023-05-20 04:14:04.000000 stdf-utils-0.2.3/src/stdf_utils/stdf_to_txt.py
+-rw-rw-rw-   0        0        0      663 2023-05-20 03:02:13.000000 stdf-utils-0.2.3/src/stdf_utils/util.py
+drwxrwxrwx   0        0        0        0 2023-05-24 07:18:17.831191 stdf-utils-0.2.3/src/stdf_utils.egg-info/
+-rw-rw-rw-   0        0        0     1340 2023-05-24 07:18:17.000000 stdf-utils-0.2.3/src/stdf_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      510 2023-05-24 07:18:17.000000 stdf-utils-0.2.3/src/stdf_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 07:18:17.000000 stdf-utils-0.2.3/src/stdf_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-24 07:18:17.000000 stdf-utils-0.2.3/src/stdf_utils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-24 07:18:17.855232 stdf-utils-0.2.3/tests/
+-rw-rw-rw-   0        0        0      728 2023-05-20 06:30:13.000000 stdf-utils-0.2.3/tests/test_stdf_patch.py
+-rw-rw-rw-   0        0        0      572 2023-05-24 07:15:50.000000 stdf-utils-0.2.3/tests/test_stdf_per_part.py
+-rw-rw-rw-   0        0        0      505 2023-05-20 06:31:39.000000 stdf-utils-0.2.3/tests/test_stdf_record.py
+-rw-rw-rw-   0        0        0      677 2023-05-20 07:41:12.000000 stdf-utils-0.2.3/tests/test_stdf_to_csv.py
+-rw-rw-rw-   0        0        0      407 2023-05-20 07:24:32.000000 stdf-utils-0.2.3/tests/test_stdf_to_txt.py
```

### Comparing `stdf-utils-0.2.2/LICENSE` & `stdf-utils-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `stdf-utils-0.2.2/PKG-INFO` & `stdf-utils-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stdf-utils
-Version: 0.2.2
+Version: 0.2.3
 Summary: stdf file parser and emitter
 Author: Peter JC. Wu
 Author-email: wolf952@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/peterjcwu/stdf-utils
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `stdf-utils-0.2.2/setup.py` & `stdf-utils-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 NAME = 'stdf-utils'
-VERSION = '0.2.2'
+VERSION = '0.2.3'
 DESCRIPTION = 'stdf file parser and emitter'
 LONG_DESCRIPTION = """\
 stdf is the standard format of ATE result, and this pacakge supports
 reading and (possibly) editing the stdf file comes form ATE.
 """
 AUTHOR = "Peter JC. Wu"
 AUTHOR_EMAIL = "wolf952@gmail.com"
```

### Comparing `stdf-utils-0.2.2/src/stdf_utils/stdf_patch.py` & `stdf-utils-0.2.3/src/stdf_utils/stdf_patch.py`

 * *Files identical despite different names*

### Comparing `stdf-utils-0.2.2/src/stdf_utils/stdf_per_part.py` & `stdf-utils-0.2.3/src/stdf_utils/stdf_per_part.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
                         "ptr": [],
                     }
 
     def mir_handler(self, d: dict) -> None:
         self.mir = {
             "node": d["NODE_NAM"].decode(),
             "job": d["JOB_NAM"].decode().split("/")[-1].replace(".prog", ""),
-            "name": os.path.basename(self.stdf_path).split(".")[0],
+            "stdf_name": os.path.basename(self.stdf_path).split(".")[0],
             "start_t": datetime.fromtimestamp(d["START_T"])
         }
 
     def ptr_handler(self, d: dict) -> None:
         site: int = d["SITE_NUM"]
         if self.ptr_filter(d):
             self.ptr[site].append({
```

### Comparing `stdf-utils-0.2.2/src/stdf_utils/stdf_record.py` & `stdf-utils-0.2.3/src/stdf_utils/stdf_record.py`

 * *Files identical despite different names*

### Comparing `stdf-utils-0.2.2/src/stdf_utils/stdf_to_csv.py` & `stdf-utils-0.2.3/src/stdf_utils/stdf_to_csv.py`

 * *Files identical despite different names*

### Comparing `stdf-utils-0.2.2/src/stdf_utils/util.py` & `stdf-utils-0.2.3/src/stdf_utils/util.py`

 * *Files identical despite different names*

### Comparing `stdf-utils-0.2.2/src/stdf_utils.egg-info/PKG-INFO` & `stdf-utils-0.2.3/src/stdf_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stdf-utils
-Version: 0.2.2
+Version: 0.2.3
 Summary: stdf file parser and emitter
 Author: Peter JC. Wu
 Author-email: wolf952@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/peterjcwu/stdf-utils
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `stdf-utils-0.2.2/tests/test_stdf_patch.py` & `stdf-utils-0.2.3/tests/test_stdf_patch.py`

 * *Files identical despite different names*

### Comparing `stdf-utils-0.2.2/tests/test_stdf_to_csv.py` & `stdf-utils-0.2.3/tests/test_stdf_to_csv.py`

 * *Files identical despite different names*

