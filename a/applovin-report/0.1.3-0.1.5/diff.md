# Comparing `tmp/applovin_report-0.1.3.tar.gz` & `tmp/applovin_report-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "applovin_report-0.1.3.tar", max compression
+gzip compressed data, was "applovin_report-0.1.5.tar", max compression
```

## Comparing `applovin_report-0.1.3.tar` & `applovin_report-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1062 2023-05-24 07:10:10.662819 applovin_report-0.1.3/LICENSE
--rw-r--r--   0        0        0      782 2023-05-24 07:10:10.662819 applovin_report-0.1.3/README.md
--rw-r--r--   0        0        0      129 2023-05-24 07:10:10.662819 applovin_report-0.1.3/applovin_report/__init__.py
--rw-r--r--   0        0        0       19 2023-05-24 07:10:10.662819 applovin_report-0.1.3/applovin_report/app.py
--rw-r--r--   0        0        0     2502 2023-05-24 07:10:10.666819 applovin_report-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       45 2023-05-24 07:10:10.666819 applovin_report-0.1.3/tests/__init__.py
--rw-r--r--   0        0        0      586 2023-05-24 07:10:10.666819 applovin_report-0.1.3/tests/test_app.py
--rw-r--r--   0        0        0     2700 1970-01-01 00:00:00.000000 applovin_report-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-05-24 09:04:42.041811 applovin_report-0.1.5/LICENSE
+-rw-r--r--   0        0        0      782 2023-05-24 09:04:42.041811 applovin_report-0.1.5/README.md
+-rw-r--r--   0        0        0      129 2023-05-24 09:04:42.041811 applovin_report-0.1.5/applovin_report/__init__.py
+-rw-r--r--   0        0        0       19 2023-05-24 09:04:42.045811 applovin_report-0.1.5/applovin_report/app.py
+-rw-r--r--   0        0        0     2502 2023-05-24 09:04:42.045811 applovin_report-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0       45 2023-05-24 09:04:42.045811 applovin_report-0.1.5/tests/__init__.py
+-rw-r--r--   0        0        0      586 2023-05-24 09:04:42.045811 applovin_report-0.1.5/tests/test_app.py
+-rw-r--r--   0        0        0     2700 1970-01-01 00:00:00.000000 applovin_report-0.1.5/PKG-INFO
```

### Comparing `applovin_report-0.1.3/LICENSE` & `applovin_report-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `applovin_report-0.1.3/README.md` & `applovin_report-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `applovin_report-0.1.3/pyproject.toml` & `applovin_report-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "applovin_report"
-version = "0.1.3"
+version = "0.1.5"
 homepage = "https://github.com/ikamedawn/applovin_report"
 description = "Applovin Report APIs wrapper."
 authors = ["Dawn <minhpc@ikameglobal.com>"]
 readme = "README.md"
 license = "MIT"
 classifiers = [
     'Development Status :: 2 - Pre-Alpha',
```

### Comparing `applovin_report-0.1.3/tests/test_app.py` & `applovin_report-0.1.5/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `applovin_report-0.1.3/PKG-INFO` & `applovin_report-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: applovin-report
-Version: 0.1.3
+Version: 0.1.5
 Summary: Applovin Report APIs wrapper.
 Home-page: https://github.com/ikamedawn/applovin_report
 License: MIT
 Author: Dawn
 Author-email: minhpc@ikameglobal.com
 Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 2 - Pre-Alpha
```

