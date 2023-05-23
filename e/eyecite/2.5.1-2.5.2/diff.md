# Comparing `tmp/eyecite-2.5.1.tar.gz` & `tmp/eyecite-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eyecite-2.5.1.tar", max compression
+gzip compressed data, was "eyecite-2.5.2.tar", max compression
```

## Comparing `eyecite-2.5.1.tar` & `eyecite-2.5.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1326 2023-03-09 23:31:53.401301 eyecite-2.5.1/LICENSE
--rw-r--r--   0        0        0    17650 2023-03-09 23:31:53.401301 eyecite-2.5.1/README.rst
--rw-r--r--   0        0        0      465 2023-03-09 23:31:53.401301 eyecite-2.5.1/eyecite/__init__.py
--rw-r--r--   0        0        0     8563 2023-03-09 23:31:53.401301 eyecite-2.5.1/eyecite/annotate.py
--rw-r--r--   0        0        0     2693 2023-03-09 23:31:53.401301 eyecite-2.5.1/eyecite/clean.py
--rw-r--r--   0        0        0     8212 2023-03-09 23:31:53.401301 eyecite-2.5.1/eyecite/find.py
--rw-r--r--   0        0        0    10229 2023-03-09 23:31:53.401301 eyecite-2.5.1/eyecite/helpers.py
--rw-r--r--   0        0        0    21692 2023-03-09 23:31:53.401301 eyecite-2.5.1/eyecite/models.py
--rw-r--r--   0        0        0        0 2023-03-09 23:31:53.401301 eyecite-2.5.1/eyecite/py.typed
--rw-r--r--   0        0        0     9062 2023-03-09 23:31:53.401301 eyecite-2.5.1/eyecite/regexes.py
--rw-r--r--   0        0        0    11021 2023-03-09 23:31:53.401301 eyecite-2.5.1/eyecite/resolve.py
--rw-r--r--   0        0        0     3602 2023-03-09 23:31:53.401301 eyecite-2.5.1/eyecite/test_factories.py
--rw-r--r--   0        0        0    19456 2023-03-09 23:31:53.401301 eyecite-2.5.1/eyecite/tokenizers.py
--rw-r--r--   0        0        0     3834 2023-03-09 23:31:53.401301 eyecite-2.5.1/eyecite/utils.py
--rw-r--r--   0        0        0     2332 2023-03-09 23:31:53.405301 eyecite-2.5.1/pyproject.toml
--rw-r--r--   0        0        0    19481 1970-01-01 00:00:00.000000 eyecite-2.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1326 2023-05-23 22:32:35.127288 eyecite-2.5.2/LICENSE
+-rw-r--r--   0        0        0    17673 2023-05-23 22:32:35.131288 eyecite-2.5.2/README.rst
+-rw-r--r--   0        0        0      465 2023-05-23 22:32:35.131288 eyecite-2.5.2/eyecite/__init__.py
+-rw-r--r--   0        0        0     8563 2023-05-23 22:32:35.131288 eyecite-2.5.2/eyecite/annotate.py
+-rw-r--r--   0        0        0     2693 2023-05-23 22:32:35.131288 eyecite-2.5.2/eyecite/clean.py
+-rw-r--r--   0        0        0     8212 2023-05-23 22:32:35.131288 eyecite-2.5.2/eyecite/find.py
+-rw-r--r--   0        0        0    10229 2023-05-23 22:32:35.131288 eyecite-2.5.2/eyecite/helpers.py
+-rw-r--r--   0        0        0    21692 2023-05-23 22:32:35.131288 eyecite-2.5.2/eyecite/models.py
+-rw-r--r--   0        0        0        0 2023-05-23 22:32:35.131288 eyecite-2.5.2/eyecite/py.typed
+-rw-r--r--   0        0        0     9062 2023-05-23 22:32:35.131288 eyecite-2.5.2/eyecite/regexes.py
+-rw-r--r--   0        0        0    11021 2023-05-23 22:32:35.131288 eyecite-2.5.2/eyecite/resolve.py
+-rw-r--r--   0        0        0     3602 2023-05-23 22:32:35.131288 eyecite-2.5.2/eyecite/test_factories.py
+-rw-r--r--   0        0        0    19456 2023-05-23 22:32:35.131288 eyecite-2.5.2/eyecite/tokenizers.py
+-rw-r--r--   0        0        0     3834 2023-05-23 22:32:35.131288 eyecite-2.5.2/eyecite/utils.py
+-rw-r--r--   0        0        0     2335 2023-05-23 22:32:35.131288 eyecite-2.5.2/pyproject.toml
+-rw-r--r--   0        0        0    19209 1970-01-01 00:00:00.000000 eyecite-2.5.2/PKG-INFO
```

### Comparing `eyecite-2.5.1/LICENSE` & `eyecite-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `eyecite-2.5.1/README.rst` & `eyecite-2.5.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -410,14 +410,16 @@
     brew install hyperscan
     pip install hyperscan
 
 
 Deployment
 ==========
 
+1. Update CHANGES.md.
+
 1. Update version info in :code:`pyproject.toml` by running :code:`poetry version [major, minor, patch]`.
 
 For an automated deployment, tag the commit with vx.y.z, and push it to main.
 An automated deploy and documentation update will be completed for you.
 
 For a manual deployment, run:
```

### Comparing `eyecite-2.5.1/eyecite/annotate.py` & `eyecite-2.5.2/eyecite/annotate.py`

 * *Files identical despite different names*

### Comparing `eyecite-2.5.1/eyecite/clean.py` & `eyecite-2.5.2/eyecite/clean.py`

 * *Files identical despite different names*

### Comparing `eyecite-2.5.1/eyecite/find.py` & `eyecite-2.5.2/eyecite/find.py`

 * *Files identical despite different names*

### Comparing `eyecite-2.5.1/eyecite/helpers.py` & `eyecite-2.5.2/eyecite/helpers.py`

 * *Files identical despite different names*

### Comparing `eyecite-2.5.1/eyecite/models.py` & `eyecite-2.5.2/eyecite/models.py`

 * *Files identical despite different names*

### Comparing `eyecite-2.5.1/eyecite/regexes.py` & `eyecite-2.5.2/eyecite/regexes.py`

 * *Files identical despite different names*

### Comparing `eyecite-2.5.1/eyecite/resolve.py` & `eyecite-2.5.2/eyecite/resolve.py`

 * *Files identical despite different names*

### Comparing `eyecite-2.5.1/eyecite/test_factories.py` & `eyecite-2.5.2/eyecite/test_factories.py`

 * *Files identical despite different names*

### Comparing `eyecite-2.5.1/eyecite/tokenizers.py` & `eyecite-2.5.2/eyecite/tokenizers.py`

 * *Files identical despite different names*

### Comparing `eyecite-2.5.1/eyecite/utils.py` & `eyecite-2.5.2/eyecite/utils.py`

 * *Files identical despite different names*

### Comparing `eyecite-2.5.1/pyproject.toml` & `eyecite-2.5.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
-version = "2.5.1"
+version = "2.5.2"
 authors = ["Free Law Project <info@free.law>"]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Intended Audience :: Developers",
   "Natural Language :: English",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
   "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 description = "Tool for extracting legal citations from text strings."
 keywords = ["legal", "courts", "citations", "extraction", "cites"]
 license = "BSD-2-Clause"
@@ -25,32 +25,32 @@
 repository = "https://github.com/freelawproject/eyecite"
 include = ["eyecite/py.typed"]
 
 [tool.poetry.urls]
 "Organisation Homepage" = "https://free.law/"
 
 [tool.poetry.dependencies]
-python = "^3.7"
-reporters-db = "3.2.32"
+python = "^3.8.1"
+reporters-db = "3.2.36"
 lxml = "^4.6.3"
 pyahocorasick = ">= 1.2"
 fast-diff-match-patch = "^2.0.0"
 regex = ">=2020.1.8"
 courts-db = "^0.10.9"
 
 [tool.poetry.dev-dependencies]
 black = "^23.1.0"
-flake8 = "^3.9.0"
+flake8 = "^6.0.0"
 isort = "^5.8.0"
-mypy = "^0.812"
+mypy = "^1.3.0"
 pylint = "^2.7.2"
-wheel = "^0.38.1"
-pylint-json2html = "^0.3.0"
-exrex = "^0.10.5"
-roman = "^3.3"
+wheel = "^0.40.0"
+pylint-json2html = "^0.4.0"
+exrex = "^0.11.0"
+roman = "^4.0"
 pdoc3 = "^0.10.0"
 hyperscan = ">= 0.1.5"
 
 [tool.poetry.group.benchmark.dependencies]
 matplotlib = "^3.5.3"
 
 [tool.black]
```

### Comparing `eyecite-2.5.1/PKG-INFO` & `eyecite-2.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,45 +1,39 @@
 Metadata-Version: 2.1
 Name: eyecite
-Version: 2.5.1
+Version: 2.5.2
 Summary: Tool for extracting legal citations from text strings.
 Home-page: https://github.com/freelawproject/eyecite
 License: BSD-2-Clause
 Keywords: legal,courts,citations,extraction,cites
 Author: Free Law Project
 Author-email: info@free.law
 Maintainer: Free Law Project
 Maintainer-email: info@free.law
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: courts-db (>=0.10.9,<0.11.0)
 Requires-Dist: fast-diff-match-patch (>=2.0.0,<3.0.0)
 Requires-Dist: lxml (>=4.6.3,<5.0.0)
 Requires-Dist: pyahocorasick (>=1.2)
 Requires-Dist: regex (>=2020.1.8)
-Requires-Dist: reporters-db (==3.2.32)
+Requires-Dist: reporters-db (==3.2.36)
 Project-URL: Organisation Homepage, https://free.law/
 Project-URL: Repository, https://github.com/freelawproject/eyecite
 Description-Content-Type: text/x-rst
 
 eyecite
 ==========
 
@@ -452,14 +446,16 @@
     brew install hyperscan
     pip install hyperscan
 
 
 Deployment
 ==========
 
+1. Update CHANGES.md.
+
 1. Update version info in :code:`pyproject.toml` by running :code:`poetry version [major, minor, patch]`.
 
 For an automated deployment, tag the commit with vx.y.z, and push it to main.
 An automated deploy and documentation update will be completed for you.
 
 For a manual deployment, run:
```

