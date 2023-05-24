# Comparing `tmp/lineagex-0.0.5a1.tar.gz` & `tmp/lineagex-0.0.5a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lineagex-0.0.5a1.tar", max compression
+gzip compressed data, was "lineagex-0.0.5a2.tar", max compression
```

## Comparing `lineagex-0.0.5a1.tar` & `lineagex-0.0.5a2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0       55 2023-05-12 01:58:21.769698 lineagex-0.0.5a1/lineagex/__init__.py
--rw-r--r--   0        0        0    54175 2023-04-22 19:33:20.371862 lineagex-0.0.5a1/lineagex/app.js
--rw-r--r--   0        0        0    32350 2023-05-20 01:29:26.901284 lineagex-0.0.5a1/lineagex/ColumnLineage.py
--rw-r--r--   0        0        0    24066 2023-05-24 01:05:18.342710 lineagex-0.0.5a1/lineagex/ColumnLineageNoConn.py
--rw-r--r--   0        0        0     1802 2023-05-23 23:33:11.925203 lineagex-0.0.5a1/lineagex/lineagex.py
--rw-r--r--   0        0        0     4691 2023-05-23 23:48:42.350240 lineagex-0.0.5a1/lineagex/LineageXNoConn.py
--rw-r--r--   0        0        0    13522 2023-05-23 21:34:23.590817 lineagex-0.0.5a1/lineagex/LineageXWithConn.py
--rw-r--r--   0        0        0     7176 2023-05-23 22:40:25.559899 lineagex-0.0.5a1/lineagex/SqlToDict.py
--rw-r--r--   0        0        0     1460 2023-05-08 20:36:59.378380 lineagex-0.0.5a1/lineagex/stack.py
--rw-r--r--   0        0        0     7305 2023-05-19 22:10:39.261810 lineagex-0.0.5a1/lineagex/utils.py
--rw-r--r--   0        0        0  3761177 2023-04-22 19:33:20.645016 lineagex-0.0.5a1/lineagex/vendor.js
--rw-r--r--   0        0        0      456 2023-05-24 01:12:49.326096 lineagex-0.0.5a1/pyproject.toml
--rw-r--r--   0        0        0     4158 2023-05-17 20:42:55.789941 lineagex-0.0.5a1/README.md
--rw-r--r--   0        0        0     4865 1970-01-01 00:00:00.000000 lineagex-0.0.5a1/PKG-INFO
+-rw-r--r--   0        0        0       55 2023-05-24 01:42:09.254432 lineagex-0.0.5a2/lineagex/__init__.py
+-rw-r--r--   0        0        0    54175 2023-04-22 19:33:20.371862 lineagex-0.0.5a2/lineagex/app.js
+-rw-r--r--   0        0        0    32350 2023-05-20 01:29:26.901284 lineagex-0.0.5a2/lineagex/ColumnLineage.py
+-rw-r--r--   0        0        0    24066 2023-05-24 01:05:18.342710 lineagex-0.0.5a2/lineagex/ColumnLineageNoConn.py
+-rw-r--r--   0        0        0     1416 2023-05-24 01:29:50.101636 lineagex-0.0.5a2/lineagex/example.py
+-rw-r--r--   0        0        0     1802 2023-05-24 01:42:19.469427 lineagex-0.0.5a2/lineagex/lineagex.py
+-rw-r--r--   0        0        0     4691 2023-05-23 23:48:42.350240 lineagex-0.0.5a2/lineagex/LineageXNoConn.py
+-rw-r--r--   0        0        0    13522 2023-05-23 21:34:23.590817 lineagex-0.0.5a2/lineagex/LineageXWithConn.py
+-rw-r--r--   0        0        0     7176 2023-05-23 22:40:25.559899 lineagex-0.0.5a2/lineagex/SqlToDict.py
+-rw-r--r--   0        0        0     1460 2023-05-08 20:36:59.378380 lineagex-0.0.5a2/lineagex/stack.py
+-rw-r--r--   0        0        0     7305 2023-05-19 22:10:39.261810 lineagex-0.0.5a2/lineagex/utils.py
+-rw-r--r--   0        0        0  3761177 2023-04-22 19:33:20.645016 lineagex-0.0.5a2/lineagex/vendor.js
+-rw-r--r--   0        0        0      456 2023-05-24 01:43:33.472574 lineagex-0.0.5a2/pyproject.toml
+-rw-r--r--   0        0        0     4158 2023-05-17 20:42:55.789941 lineagex-0.0.5a2/README.md
+-rw-r--r--   0        0        0     4865 1970-01-01 00:00:00.000000 lineagex-0.0.5a2/PKG-INFO
```

### Comparing `lineagex-0.0.5a1/lineagex/app.js` & `lineagex-0.0.5a2/lineagex/app.js`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.5a1/lineagex/ColumnLineage.py` & `lineagex-0.0.5a2/lineagex/ColumnLineage.py`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.5a1/lineagex/ColumnLineageNoConn.py` & `lineagex-0.0.5a2/lineagex/ColumnLineageNoConn.py`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.5a1/lineagex/lineagex.py` & `lineagex-0.0.5a2/lineagex/lineagex.py`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.5a1/lineagex/LineageXNoConn.py` & `lineagex-0.0.5a2/lineagex/LineageXNoConn.py`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.5a1/lineagex/LineageXWithConn.py` & `lineagex-0.0.5a2/lineagex/LineageXWithConn.py`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.5a1/lineagex/SqlToDict.py` & `lineagex-0.0.5a2/lineagex/SqlToDict.py`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.5a1/lineagex/stack.py` & `lineagex-0.0.5a2/lineagex/stack.py`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.5a1/lineagex/utils.py` & `lineagex-0.0.5a2/lineagex/utils.py`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.5a1/lineagex/vendor.js` & `lineagex-0.0.5a2/lineagex/vendor.js`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.5a1/README.md` & `lineagex-0.0.5a2/README.md`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.5a1/PKG-INFO` & `lineagex-0.0.5a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lineagex
-Version: 0.0.5a1
+Version: 0.0.5a2
 Summary: A column lineage tool
 License: MIT
 Author: zshandy
 Author-email: zshandy@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

