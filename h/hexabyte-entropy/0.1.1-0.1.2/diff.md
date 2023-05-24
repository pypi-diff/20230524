# Comparing `tmp/hexabyte_entropy-0.1.1.tar.gz` & `tmp/hexabyte_entropy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hexabyte_entropy-0.1.1.tar", max compression
+gzip compressed data, was "hexabyte_entropy-0.1.2.tar", max compression
```

## Comparing `hexabyte_entropy-0.1.1.tar` & `hexabyte_entropy-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35149 2023-05-24 01:29:42.379819 hexabyte_entropy-0.1.1/LICENSE
--rw-r--r--   0        0        0      487 2023-05-24 01:29:42.379819 hexabyte_entropy-0.1.1/docs/README.md
--rw-r--r--   0        0        0      166 2023-05-24 01:29:42.379819 hexabyte_entropy-0.1.1/hexabyte_entropy/__init__.py
--rw-r--r--   0        0        0     3001 2023-05-24 01:29:42.379819 hexabyte_entropy-0.1.1/hexabyte_entropy/entropy.py
--rw-r--r--   0        0        0       38 2023-05-24 01:29:42.379819 hexabyte_entropy-0.1.1/hexabyte_entropy/widgets/__init__.py
--rw-r--r--   0        0        0     3270 2023-05-24 01:29:42.379819 hexabyte_entropy-0.1.1/hexabyte_entropy/widgets/entropy_panel.py
--rw-r--r--   0        0        0     8304 2023-05-24 01:29:42.403821 hexabyte_entropy-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1896 1970-01-01 00:00:00.000000 hexabyte_entropy-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-24 01:31:26.272227 hexabyte_entropy-0.1.2/LICENSE
+-rw-r--r--   0        0        0      481 2023-05-24 01:31:26.272227 hexabyte_entropy-0.1.2/docs/README.md
+-rw-r--r--   0        0        0      166 2023-05-24 01:31:26.272227 hexabyte_entropy-0.1.2/hexabyte_entropy/__init__.py
+-rw-r--r--   0        0        0     3001 2023-05-24 01:31:26.272227 hexabyte_entropy-0.1.2/hexabyte_entropy/entropy.py
+-rw-r--r--   0        0        0       38 2023-05-24 01:31:26.272227 hexabyte_entropy-0.1.2/hexabyte_entropy/widgets/__init__.py
+-rw-r--r--   0        0        0     3270 2023-05-24 01:31:26.272227 hexabyte_entropy-0.1.2/hexabyte_entropy/widgets/entropy_panel.py
+-rw-r--r--   0        0        0     8304 2023-05-24 01:31:26.296227 hexabyte_entropy-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1890 1970-01-01 00:00:00.000000 hexabyte_entropy-0.1.2/PKG-INFO
```

### Comparing `hexabyte_entropy-0.1.1/LICENSE` & `hexabyte_entropy-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hexabyte_entropy-0.1.1/hexabyte_entropy/entropy.py` & `hexabyte_entropy-0.1.2/hexabyte_entropy/entropy.py`

 * *Files identical despite different names*

### Comparing `hexabyte_entropy-0.1.1/hexabyte_entropy/widgets/entropy_panel.py` & `hexabyte_entropy-0.1.2/hexabyte_entropy/widgets/entropy_panel.py`

 * *Files identical despite different names*

### Comparing `hexabyte_entropy-0.1.1/pyproject.toml` & `hexabyte_entropy-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hexabyte_entropy"
-version = "0.1.1"
+version = "0.1.2"
 description = "An entropy plugin for the hexabyte hex editor."
 keywords = ["commandline", "hexabyte", "hexeditor", "plugin", "sidebar", "entropy"]
 repository = "https://github.com/thetacom/hexabyte_entropy"
 authors = ["Justin C <justin@thetacom.info>"]
 readme = "docs/README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `hexabyte_entropy-0.1.1/PKG-INFO` & `hexabyte_entropy-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hexabyte-entropy
-Version: 0.1.1
+Version: 0.1.2
 Summary: An entropy plugin for the hexabyte hex editor.
 Home-page: https://github.com/thetacom/hexabyte_entropy
 Keywords: commandline,hexabyte,hexeditor,plugin,sidebar,entropy
 Author: Justin C
 Author-email: justin@thetacom.info
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -26,15 +26,15 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
 Requires-Dist: hexabyte (>=0.6.0rc0,<0.7.0)
 Requires-Dist: hilbertcurve (>=2.0.5,<3.0.0)
 Project-URL: Repository, https://github.com/thetacom/hexabyte_entropy
 Description-Content-Type: text/markdown
 
-# Hexabyte Extended Info Plugin
+# Hexabyte Entropy Plugin
 
 A hexabyte plugin for displaying the entropy of file chunks.
 
 The entropy values are mapped to color codes and then displayed in a scrollable sidebar. Clicking on a chunk will jump the active editor to the location of the selected chunk.
 
 ## Install
```

