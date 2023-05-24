# Comparing `tmp/prfiesta-0.8.0b124.tar.gz` & `tmp/prfiesta-0.8.1b125.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prfiesta-0.8.0b124.tar", max compression
+gzip compressed data, was "prfiesta-0.8.1b125.tar", max compression
```

## Comparing `prfiesta-0.8.0b124.tar` & `prfiesta-0.8.1b125.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1078 2023-05-24 05:22:40.958774 prfiesta-0.8.0b124/LICENSE
--rw-r--r--   0        0        0     6603 2023-05-24 05:22:40.958774 prfiesta-0.8.0b124/README.md
--rw-r--r--   0        0        0      487 2023-05-24 05:22:40.966774 prfiesta-0.8.0b124/prfiesta/__init__.py
--rw-r--r--   0        0        0     2763 2023-05-24 05:22:40.966774 prfiesta-0.8.0b124/prfiesta/__main__.py
--rw-r--r--   0        0        0        0 2023-05-24 05:22:40.966774 prfiesta-0.8.0b124/prfiesta/analysis/__init__.py
--rw-r--r--   0        0        0     4729 2023-05-24 05:22:40.966774 prfiesta-0.8.0b124/prfiesta/analysis/plot.py
--rw-r--r--   0        0        0     1007 2023-05-24 05:22:40.966774 prfiesta-0.8.0b124/prfiesta/analysis/view.py
--rw-r--r--   0        0        0        0 2023-05-24 05:22:40.966774 prfiesta-0.8.0b124/prfiesta/collectors/__init__.py
--rw-r--r--   0        0        0     4981 2023-05-24 05:22:40.966774 prfiesta-0.8.0b124/prfiesta/collectors/github.py
--rw-r--r--   0        0        0      571 2023-05-24 05:22:40.966774 prfiesta-0.8.0b124/prfiesta/environment.py
--rw-r--r--   0        0        0      975 2023-05-24 05:22:40.966774 prfiesta-0.8.0b124/prfiesta/output.py
--rw-r--r--   0        0        0      275 2023-05-24 05:22:40.966774 prfiesta-0.8.0b124/prfiesta/spinner.py
--rw-r--r--   0        0        0     3187 2023-05-24 05:22:48.510861 prfiesta-0.8.0b124/pyproject.toml
--rw-r--r--   0        0        0     7952 1970-01-01 00:00:00.000000 prfiesta-0.8.0b124/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-05-24 05:35:54.493772 prfiesta-0.8.1b125/LICENSE
+-rw-r--r--   0        0        0     6603 2023-05-24 05:35:54.493772 prfiesta-0.8.1b125/README.md
+-rw-r--r--   0        0        0      487 2023-05-24 05:35:54.501772 prfiesta-0.8.1b125/prfiesta/__init__.py
+-rw-r--r--   0        0        0     2763 2023-05-24 05:35:54.501772 prfiesta-0.8.1b125/prfiesta/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-24 05:35:54.501772 prfiesta-0.8.1b125/prfiesta/analysis/__init__.py
+-rw-r--r--   0        0        0     4729 2023-05-24 05:35:54.501772 prfiesta-0.8.1b125/prfiesta/analysis/plot.py
+-rw-r--r--   0        0        0     1007 2023-05-24 05:35:54.501772 prfiesta-0.8.1b125/prfiesta/analysis/view.py
+-rw-r--r--   0        0        0        0 2023-05-24 05:35:54.501772 prfiesta-0.8.1b125/prfiesta/collectors/__init__.py
+-rw-r--r--   0        0        0     4981 2023-05-24 05:35:54.501772 prfiesta-0.8.1b125/prfiesta/collectors/github.py
+-rw-r--r--   0        0        0      571 2023-05-24 05:35:54.501772 prfiesta-0.8.1b125/prfiesta/environment.py
+-rw-r--r--   0        0        0      975 2023-05-24 05:35:54.501772 prfiesta-0.8.1b125/prfiesta/output.py
+-rw-r--r--   0        0        0      275 2023-05-24 05:35:54.501772 prfiesta-0.8.1b125/prfiesta/spinner.py
+-rw-r--r--   0        0        0     3187 2023-05-24 05:36:03.749879 prfiesta-0.8.1b125/pyproject.toml
+-rw-r--r--   0        0        0     7952 1970-01-01 00:00:00.000000 prfiesta-0.8.1b125/PKG-INFO
```

### Comparing `prfiesta-0.8.0b124/LICENSE` & `prfiesta-0.8.1b125/LICENSE`

 * *Files identical despite different names*

### Comparing `prfiesta-0.8.0b124/README.md` & `prfiesta-0.8.1b125/README.md`

 * *Files identical despite different names*

### Comparing `prfiesta-0.8.0b124/prfiesta/__main__.py` & `prfiesta-0.8.1b125/prfiesta/__main__.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.8.0b124/prfiesta/analysis/plot.py` & `prfiesta-0.8.1b125/prfiesta/analysis/plot.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.8.0b124/prfiesta/analysis/view.py` & `prfiesta-0.8.1b125/prfiesta/analysis/view.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.8.0b124/prfiesta/collectors/github.py` & `prfiesta-0.8.1b125/prfiesta/collectors/github.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.8.0b124/prfiesta/environment.py` & `prfiesta-0.8.1b125/prfiesta/environment.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.8.0b124/prfiesta/output.py` & `prfiesta-0.8.1b125/prfiesta/output.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.8.0b124/pyproject.toml` & `prfiesta-0.8.1b125/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prfiesta"
-version = "0.8.0b124"
+version = "0.8.1b125"
 description = "Analyze Individual Contributor Pull Requests"
 authors = ["kiran94"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/kiran94/prfiesta"
 repository = "https://github.com/kiran94/prfiesta"
 documentation = "https://github.com/kiran94/prfiesta/blob/main/README.md"
```

### Comparing `prfiesta-0.8.0b124/PKG-INFO` & `prfiesta-0.8.1b125/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prfiesta
-Version: 0.8.0b124
+Version: 0.8.1b125
 Summary: Analyze Individual Contributor Pull Requests
 Home-page: https://github.com/kiran94/prfiesta
 License: MIT
 Keywords: pull-request,pull-request-review,performance-review
 Author: kiran94
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
```

