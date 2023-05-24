# Comparing `tmp/applovin_report-0.1.8.tar.gz` & `tmp/applovin_report-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "applovin_report-0.1.8.tar", max compression
+gzip compressed data, was "applovin_report-0.1.9.tar", max compression
```

## Comparing `applovin_report-0.1.8.tar` & `applovin_report-0.1.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1062 2023-05-24 11:26:01.036925 applovin_report-0.1.8/LICENSE
--rw-r--r--   0        0        0      782 2023-05-24 11:26:01.036925 applovin_report-0.1.8/README.md
--rw-r--r--   0        0        0      129 2023-05-24 11:26:01.040925 applovin_report-0.1.8/applovin_report/__init__.py
--rw-r--r--   0        0        0       19 2023-05-24 11:26:01.040925 applovin_report-0.1.8/applovin_report/app.py
--rw-r--r--   0        0        0     2502 2023-05-24 11:26:01.040925 applovin_report-0.1.8/pyproject.toml
--rw-r--r--   0        0        0       45 2023-05-24 11:26:01.040925 applovin_report-0.1.8/tests/__init__.py
--rw-r--r--   0        0        0      586 2023-05-24 11:26:01.040925 applovin_report-0.1.8/tests/test_app.py
--rw-r--r--   0        0        0     2700 1970-01-01 00:00:00.000000 applovin_report-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-05-24 11:28:36.620550 applovin_report-0.1.9/LICENSE
+-rw-r--r--   0        0        0      782 2023-05-24 11:28:36.620550 applovin_report-0.1.9/README.md
+-rw-r--r--   0        0        0      129 2023-05-24 11:28:36.620550 applovin_report-0.1.9/applovin_report/__init__.py
+-rw-r--r--   0        0        0       19 2023-05-24 11:28:36.620550 applovin_report-0.1.9/applovin_report/app.py
+-rw-r--r--   0        0        0     2502 2023-05-24 11:28:36.620550 applovin_report-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0       45 2023-05-24 11:28:36.620550 applovin_report-0.1.9/tests/__init__.py
+-rw-r--r--   0        0        0      586 2023-05-24 11:28:36.620550 applovin_report-0.1.9/tests/test_app.py
+-rw-r--r--   0        0        0     2700 1970-01-01 00:00:00.000000 applovin_report-0.1.9/PKG-INFO
```

### Comparing `applovin_report-0.1.8/LICENSE` & `applovin_report-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `applovin_report-0.1.8/README.md` & `applovin_report-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `applovin_report-0.1.8/pyproject.toml` & `applovin_report-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "applovin_report"
-version = "0.1.8"
+version = "0.1.9"
 homepage = "https://github.com/ikamedawn/applovin_report"
 description = "Applovin Report APIs wrapper."
 authors = ["Dawn <minhpc@ikameglobal.com>"]
 readme = "README.md"
 license = "MIT"
 classifiers = [
     'Development Status :: 2 - Pre-Alpha',
```

### Comparing `applovin_report-0.1.8/tests/test_app.py` & `applovin_report-0.1.9/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `applovin_report-0.1.8/PKG-INFO` & `applovin_report-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: applovin-report
-Version: 0.1.8
+Version: 0.1.9
 Summary: Applovin Report APIs wrapper.
 Home-page: https://github.com/ikamedawn/applovin_report
 License: MIT
 Author: Dawn
 Author-email: minhpc@ikameglobal.com
 Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 2 - Pre-Alpha
```

