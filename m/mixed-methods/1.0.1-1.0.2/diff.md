# Comparing `tmp/mixed_methods-1.0.1.tar.gz` & `tmp/mixed_methods-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mixed_methods-1.0.1.tar", max compression
+gzip compressed data, was "mixed_methods-1.0.2.tar", max compression
```

## Comparing `mixed_methods-1.0.1.tar` & `mixed_methods-1.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1092 2023-05-15 12:40:49.268563 mixed_methods-1.0.1/LICENSE
--rw-r--r--   0        0        0     3459 2023-05-15 12:40:49.268563 mixed_methods-1.0.1/README.md
--rw-r--r--   0        0        0      307 2023-05-15 12:40:49.268563 mixed_methods-1.0.1/mixed_methods/__init__.py
--rw-r--r--   0        0        0     1565 2023-05-15 12:40:49.272563 mixed_methods-1.0.1/mixed_methods/core.py
--rw-r--r--   0        0        0        0 2023-05-15 12:40:49.272563 mixed_methods-1.0.1/mixed_methods/py.typed
--rw-r--r--   0        0        0     3209 2023-05-15 12:40:49.272563 mixed_methods-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     4655 1970-01-01 00:00:00.000000 mixed_methods-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-05-23 23:12:44.640321 mixed_methods-1.0.2/LICENSE
+-rw-r--r--   0        0        0     3459 2023-05-23 23:12:44.640321 mixed_methods-1.0.2/README.md
+-rw-r--r--   0        0        0      307 2023-05-23 23:12:44.640321 mixed_methods-1.0.2/mixed_methods/__init__.py
+-rw-r--r--   0        0        0     1565 2023-05-23 23:12:44.640321 mixed_methods-1.0.2/mixed_methods/core.py
+-rw-r--r--   0        0        0        0 2023-05-23 23:12:44.640321 mixed_methods-1.0.2/mixed_methods/py.typed
+-rw-r--r--   0        0        0     3203 2023-05-23 23:12:44.640321 mixed_methods-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4655 1970-01-01 00:00:00.000000 mixed_methods-1.0.2/PKG-INFO
```

### Comparing `mixed_methods-1.0.1/LICENSE` & `mixed_methods-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mixed_methods-1.0.1/README.md` & `mixed_methods-1.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 $ poetry add mixed-methods
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-mixed-methods = "^1.0.1"
+mixed-methods = "^1.0.2"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.mixed-methods]
 git = "https://github.com/nekitdev/mixed-methods.git"
```

### Comparing `mixed_methods-1.0.1/mixed_methods/core.py` & `mixed_methods-1.0.2/mixed_methods/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from typing import Callable, Generic, Optional, Type, TypeVar, Union, final, overload
+from typing import Callable, Generic, Optional, Type, TypeVar, Union, overload
 
 from attrs import frozen
-from typing_extensions import Concatenate, ParamSpec
+from typing_extensions import Concatenate, ParamSpec, final
 
 __all__ = ("MixedMethod", "mixed_method")
 
 T = TypeVar("T")
 
 # P -> R
```

### Comparing `mixed_methods-1.0.1/pyproject.toml` & `mixed_methods-1.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mixed-methods"
-version = "1.0.1"
+version = "1.0.2"
 description = "Mixed methods."
 authors = ["nekitdev"]
 license = "MIT"
 
 readme = "README.md"
 
 homepage = "https://github.com/nekitdev/mixed-methods"
@@ -63,22 +63,22 @@
 pytest-cov = "4.0.0"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "1.4.3"
-mkdocs-material = "9.1.12"
+mkdocs-material = "9.1.14"
 
 [tool.poetry.group.docs.dependencies.mkdocstrings]
 version = "0.21.2"
 extras = ["python"]
 
 [tool.poetry.group.dev.dependencies]
-changelogging = "1.2.0"
+changelogging = "1.3.0"
 
 [tool.black]
 line_length = 100
 
 [tool.flake8]
 max_line_length = 100
 
@@ -96,15 +96,15 @@
 [tool.coverage.report]
 ignore_errors = true
 exclude_lines = [
     "pragma: never",
     "pragma: no cover",
     "if TYPE_CHECKING",
     "@overload",
-    "@abstractmethod",
+    "@required",
     "raise NotImplementedError",
     "raise AssertionError",
     "def __repr__",
 ]
 
 [tool.coverage.html]
 directory = "coverage"
@@ -132,15 +132,15 @@
 warn_unreachable = true
 
 warn_redundant_casts = true
 warn_unused_ignores = false  # compatibility
 
 [tool.changelogging]
 name = "mixed-methods"
-version = "1.0.1"
+version = "1.0.2"
 url = "https://github.com/nekitdev/mixed-methods"
 directory = "changes"
 output = "CHANGELOG.md"
 
 start_string = "<!-- changelogging: start -->"
 
 title_format = "{version} ({date})"
```

### Comparing `mixed_methods-1.0.1/PKG-INFO` & `mixed_methods-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mixed-methods
-Version: 1.0.1
+Version: 1.0.2
 Summary: Mixed methods.
 Home-page: https://github.com/nekitdev/mixed-methods
 License: MIT
 Keywords: python,mixed,method
 Author: nekitdev
 Requires-Python: >=3.7
 Classifier: Development Status :: 5 - Production/Stable
@@ -70,15 +70,15 @@
 $ poetry add mixed-methods
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-mixed-methods = "^1.0.1"
+mixed-methods = "^1.0.2"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.mixed-methods]
 git = "https://github.com/nekitdev/mixed-methods.git"
```

