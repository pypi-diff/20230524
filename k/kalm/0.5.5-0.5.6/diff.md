# Comparing `tmp/kalm-0.5.5.tar.gz` & `tmp/kalm-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kalm-0.5.5.tar", max compression
+gzip compressed data, was "kalm-0.5.6.tar", max compression
```

## Comparing `kalm-0.5.5.tar` & `kalm-0.5.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1081 2023-05-09 13:16:08.584607 kalm-0.5.5/LICENSE.txt
--rw-r--r--   0        0        0     1890 2023-05-09 13:17:44.333161 kalm-0.5.5/pyproject.toml
--rw-r--r--   0        0        0    10421 2023-05-09 13:16:08.588607 kalm-0.5.5/src/kalm/__init__.py
--rw-r--r--   0        0        0       34 2023-05-09 13:16:08.588607 kalm-0.5.5/src/kalm/jenkins.py
--rw-r--r--   0        0        0    32279 2023-05-09 13:16:08.588607 kalm-0.5.5/src/kalm/kalm.py
--rw-r--r--   0        0        0     1296 2023-05-09 13:16:08.588607 kalm-0.5.5/src/kalm/netbox.py
--rw-r--r--   0        0        0        9 2023-05-09 13:16:08.588607 kalm-0.5.5/src/kalm/package_data.dat
--rw-r--r--   0        0        0      312 2023-05-09 13:16:08.588607 kalm-0.5.5/src/kalm/toolbox.py
--rw-r--r--   0        0        0      960 1970-01-01 00:00:00.000000 kalm-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-09 12:32:33.321460 kalm-0.5.6/LICENSE.txt
+-rw-r--r--   0        0        0     1890 2023-05-09 13:19:17.365700 kalm-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0    10421 2023-05-09 12:32:33.321460 kalm-0.5.6/src/kalm/__init__.py
+-rw-r--r--   0        0        0       33 2023-05-09 13:19:17.365700 kalm-0.5.6/src/kalm/jenkins.py
+-rw-r--r--   0        0        0    32279 2023-05-09 12:32:33.321460 kalm-0.5.6/src/kalm/kalm.py
+-rw-r--r--   0        0        0     1296 2023-05-09 12:32:33.321460 kalm-0.5.6/src/kalm/netbox.py
+-rw-r--r--   0        0        0        9 2023-05-09 12:32:33.321460 kalm-0.5.6/src/kalm/package_data.dat
+-rw-r--r--   0        0        0      312 2023-05-09 12:32:33.321460 kalm-0.5.6/src/kalm/toolbox.py
+-rw-r--r--   0        0        0      960 1970-01-01 00:00:00.000000 kalm-0.5.6/PKG-INFO
```

### Comparing `kalm-0.5.5/LICENSE.txt` & `kalm-0.5.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kalm-0.5.5/pyproject.toml` & `kalm-0.5.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kalm"
-version = "0.5.5"
+version = "0.5.6"
 description = "Knowit Automation lifecycle management"
 authors = ["Jakob Holst <jakob.holst@knowit.dk>"]
 license = "MIT"
 homepage = "https://kalm.openknowit.com"
 repository = "https://github.com/miracle-as/openknowit_kalm.git"
 
 [tool.poetry.scripts]
```

### Comparing `kalm-0.5.5/src/kalm/__init__.py` & `kalm-0.5.6/src/kalm/__init__.py`

 * *Files identical despite different names*

### Comparing `kalm-0.5.5/src/kalm/kalm.py` & `kalm-0.5.6/src/kalm/kalm.py`

 * *Files identical despite different names*

### Comparing `kalm-0.5.5/src/kalm/netbox.py` & `kalm-0.5.6/src/kalm/netbox.py`

 * *Files identical despite different names*

### Comparing `kalm-0.5.5/PKG-INFO` & `kalm-0.5.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kalm
-Version: 0.5.5
+Version: 0.5.6
 Summary: Knowit Automation lifecycle management
 Home-page: https://kalm.openknowit.com
 License: MIT
 Author: Jakob Holst
 Author-email: jakob.holst@knowit.dk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

