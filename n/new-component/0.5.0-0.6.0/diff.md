# Comparing `tmp/new-component-0.5.0.tar.gz` & `tmp/new-component-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "new-component-0.5.0.tar", last modified: Sat May 20 23:19:08 2023, max compression
+gzip compressed data, was "new-component-0.6.0.tar", last modified: Tue May 23 23:13:57 2023, max compression
```

## Comparing `new-component-0.5.0.tar` & `new-component-0.6.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1067 2023-05-20 23:18:31.018940 new-component-0.5.0/LICENSE
--rw-r--r--   0        0        0     4798 2023-05-20 23:18:31.018940 new-component-0.5.0/README.md
--rw-r--r--   0        0        0     2331 2023-05-20 23:18:31.018940 new-component-0.5.0/pyproject.toml
--rw-r--r--   0        0        0       31 2023-05-20 23:18:31.018940 new-component-0.5.0/src/new_component/__init__.py
--rw-r--r--   0        0        0     2751 2023-05-20 23:18:31.018940 new-component-0.5.0/src/new_component/_config.py
--rw-r--r--   0        0        0      708 2023-05-20 23:18:31.018940 new-component-0.5.0/src/new_component/_confirms.py
--rw-r--r--   0        0        0      566 2023-05-20 23:18:31.018940 new-component-0.5.0/src/new_component/_constants.py
--rw-r--r--   0        0        0     2088 2023-05-20 23:18:31.018940 new-component-0.5.0/src/new_component/_echos.py
--rw-r--r--   0        0        0      360 2023-05-20 23:18:31.018940 new-component-0.5.0/src/new_component/_jinja.py
--rw-r--r--   0        0        0      249 2023-05-20 23:18:31.018940 new-component-0.5.0/src/new_component/_utils.py
--rw-r--r--   0        0        0      663 2023-05-20 23:18:31.018940 new-component-0.5.0/src/new_component/_version.py
--rw-r--r--   0        0        0     4357 2023-05-20 23:18:31.018940 new-component-0.5.0/src/new_component/cli.py
--rw-r--r--   0        0        0      142 2023-05-20 23:18:31.018940 new-component-0.5.0/src/new_component/main.py
--rw-r--r--   0        0        0        0 2023-05-20 23:18:31.018940 new-component-0.5.0/src/new_component/py.typed
--rw-r--r--   0        0        0      269 2023-05-20 23:18:31.018940 new-component-0.5.0/src/new_component/templates/component.js.j2
--rw-r--r--   0        0        0       48 2023-05-20 23:18:31.018940 new-component-0.5.0/src/new_component/templates/index.js.j2
--rw-r--r--   0        0        0        0 2023-05-20 23:18:31.018940 new-component-0.5.0/tests/__init__.py
--rw-r--r--   0        0        0     6215 2023-05-20 23:18:31.018940 new-component-0.5.0/tests/test_new_component.py
--rw-r--r--   0        0        0      221 2023-05-20 23:18:31.018940 new-component-0.5.0/tests/test_settings.py
--rw-r--r--   0        0        0      326 2023-05-20 23:18:31.018940 new-component-0.5.0/tests/test_version.py
--rw-r--r--   0        0        0     5401 1970-01-01 00:00:00.000000 new-component-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-23 23:13:33.033156 new-component-0.6.0/LICENSE
+-rw-r--r--   0        0        0     4798 2023-05-23 23:13:33.033156 new-component-0.6.0/README.md
+-rw-r--r--   0        0        0     2331 2023-05-23 23:13:33.033156 new-component-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0       31 2023-05-23 23:13:33.033156 new-component-0.6.0/src/new_component/__init__.py
+-rw-r--r--   0        0        0     2751 2023-05-23 23:13:33.033156 new-component-0.6.0/src/new_component/_config.py
+-rw-r--r--   0        0        0      708 2023-05-23 23:13:33.033156 new-component-0.6.0/src/new_component/_confirms.py
+-rw-r--r--   0        0        0      566 2023-05-23 23:13:33.033156 new-component-0.6.0/src/new_component/_constants.py
+-rw-r--r--   0        0        0     2088 2023-05-23 23:13:33.033156 new-component-0.6.0/src/new_component/_echos.py
+-rw-r--r--   0        0        0      360 2023-05-23 23:13:33.033156 new-component-0.6.0/src/new_component/_jinja.py
+-rw-r--r--   0        0        0      249 2023-05-23 23:13:33.033156 new-component-0.6.0/src/new_component/_utils.py
+-rw-r--r--   0        0        0      663 2023-05-23 23:13:33.033156 new-component-0.6.0/src/new_component/_version.py
+-rw-r--r--   0        0        0     4357 2023-05-23 23:13:33.033156 new-component-0.6.0/src/new_component/cli.py
+-rw-r--r--   0        0        0      142 2023-05-23 23:13:33.033156 new-component-0.6.0/src/new_component/main.py
+-rw-r--r--   0        0        0        0 2023-05-23 23:13:33.033156 new-component-0.6.0/src/new_component/py.typed
+-rw-r--r--   0        0        0      284 2023-05-23 23:13:33.033156 new-component-0.6.0/src/new_component/templates/component.js.j2
+-rw-r--r--   0        0        0       48 2023-05-23 23:13:33.033156 new-component-0.6.0/src/new_component/templates/index.js.j2
+-rw-r--r--   0        0        0        0 2023-05-23 23:13:33.033156 new-component-0.6.0/tests/__init__.py
+-rw-r--r--   0        0        0     6215 2023-05-23 23:13:33.033156 new-component-0.6.0/tests/test_new_component.py
+-rw-r--r--   0        0        0      221 2023-05-23 23:13:33.033156 new-component-0.6.0/tests/test_settings.py
+-rw-r--r--   0        0        0      326 2023-05-23 23:13:33.033156 new-component-0.6.0/tests/test_version.py
+-rw-r--r--   0        0        0     5401 1970-01-01 00:00:00.000000 new-component-0.6.0/PKG-INFO
```

### Comparing `new-component-0.5.0/LICENSE` & `new-component-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `new-component-0.5.0/README.md` & `new-component-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `new-component-0.5.0/pyproject.toml` & `new-component-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     "javascript",
     "styled-components",
 ]
 classifiers = [
     "Topic :: Software Development :: Code Generators",
     "Programming Language :: Python :: 3.11",
 ]
-version = "0.5.0"
+version = "0.6.0"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://new-component.iancleary.me"
 Repository = "https://github.com/iancleary/new-component"
```

### Comparing `new-component-0.5.0/src/new_component/_config.py` & `new-component-0.6.0/src/new_component/_config.py`

 * *Files identical despite different names*

### Comparing `new-component-0.5.0/src/new_component/_confirms.py` & `new-component-0.6.0/src/new_component/_confirms.py`

 * *Files identical despite different names*

### Comparing `new-component-0.5.0/src/new_component/_constants.py` & `new-component-0.6.0/src/new_component/_constants.py`

 * *Files identical despite different names*

### Comparing `new-component-0.5.0/src/new_component/_echos.py` & `new-component-0.6.0/src/new_component/_echos.py`

 * *Files identical despite different names*

### Comparing `new-component-0.5.0/src/new_component/_version.py` & `new-component-0.6.0/src/new_component/_version.py`

 * *Files identical despite different names*

### Comparing `new-component-0.5.0/src/new_component/cli.py` & `new-component-0.6.0/src/new_component/cli.py`

 * *Files identical despite different names*

### Comparing `new-component-0.5.0/tests/test_new_component.py` & `new-component-0.6.0/tests/test_new_component.py`

 * *Files identical despite different names*

### Comparing `new-component-0.5.0/PKG-INFO` & `new-component-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: new_component
-Version: 0.5.0
+Version: 0.6.0
 Summary: Quickly create opinionated Styled Components for React Projects
 License: MIT
 Keywords: script,javascript,styled-components
 Author-email: Ian Cleary <github@iancleary.me>
 Requires-Python: >=3.11
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Code Generators
```

