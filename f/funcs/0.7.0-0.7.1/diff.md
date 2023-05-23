# Comparing `tmp/funcs-0.7.0.tar.gz` & `tmp/funcs-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcs-0.7.0.tar", max compression
+gzip compressed data, was "funcs-0.7.1.tar", max compression
```

## Comparing `funcs-0.7.0.tar` & `funcs-0.7.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1092 2023-05-22 18:25:43.599021 funcs-0.7.0/LICENSE
--rw-r--r--   0        0        0     2872 2023-05-22 18:25:43.599021 funcs-0.7.0/README.md
--rw-r--r--   0        0        0     1714 2023-05-22 18:25:43.603021 funcs-0.7.0/funcs/__init__.py
--rw-r--r--   0        0        0      883 2023-05-22 18:25:43.603021 funcs-0.7.0/funcs/application.py
--rw-r--r--   0        0        0      857 2023-05-22 18:25:43.603021 funcs-0.7.0/funcs/callers.py
--rw-r--r--   0        0        0     5470 2023-05-22 18:25:43.603021 funcs-0.7.0/funcs/composition.py
--rw-r--r--   0        0        0      832 2023-05-22 18:25:43.603021 funcs-0.7.0/funcs/debug.py
--rw-r--r--   0        0        0      436 2023-05-22 18:25:43.603021 funcs-0.7.0/funcs/decorators.py
--rw-r--r--   0        0        0     6369 2023-05-22 18:25:43.603021 funcs-0.7.0/funcs/flow.py
--rw-r--r--   0        0        0     2260 2023-05-22 18:25:43.603021 funcs-0.7.0/funcs/functions.py
--rw-r--r--   0        0        0      418 2023-05-22 18:25:43.603021 funcs-0.7.0/funcs/getters.py
--rw-r--r--   0        0        0      782 2023-05-22 18:25:43.603021 funcs-0.7.0/funcs/primitives.py
--rw-r--r--   0        0        0        0 2023-05-22 18:25:43.603021 funcs-0.7.0/funcs/py.typed
--rw-r--r--   0        0        0     1113 2023-05-22 18:25:43.603021 funcs-0.7.0/funcs/reduction.py
--rw-r--r--   0        0        0     1031 2023-05-22 18:25:43.603021 funcs-0.7.0/funcs/types.py
--rw-r--r--   0        0        0     2346 2023-05-22 18:25:43.603021 funcs-0.7.0/funcs/unpacking.py
--rw-r--r--   0        0        0     3212 2023-05-22 18:25:43.603021 funcs-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     4102 1970-01-01 00:00:00.000000 funcs-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-05-23 23:04:28.691680 funcs-0.7.1/LICENSE
+-rw-r--r--   0        0        0     2872 2023-05-23 23:04:28.691680 funcs-0.7.1/README.md
+-rw-r--r--   0        0        0     1714 2023-05-23 23:04:28.691680 funcs-0.7.1/funcs/__init__.py
+-rw-r--r--   0        0        0      883 2023-05-23 23:04:28.691680 funcs-0.7.1/funcs/application.py
+-rw-r--r--   0        0        0      857 2023-05-23 23:04:28.691680 funcs-0.7.1/funcs/callers.py
+-rw-r--r--   0        0        0     5470 2023-05-23 23:04:28.691680 funcs-0.7.1/funcs/composition.py
+-rw-r--r--   0        0        0      832 2023-05-23 23:04:28.691680 funcs-0.7.1/funcs/debug.py
+-rw-r--r--   0        0        0      436 2023-05-23 23:04:28.691680 funcs-0.7.1/funcs/decorators.py
+-rw-r--r--   0        0        0     6369 2023-05-23 23:04:28.691680 funcs-0.7.1/funcs/flow.py
+-rw-r--r--   0        0        0     2260 2023-05-23 23:04:28.691680 funcs-0.7.1/funcs/functions.py
+-rw-r--r--   0        0        0      418 2023-05-23 23:04:28.691680 funcs-0.7.1/funcs/getters.py
+-rw-r--r--   0        0        0      782 2023-05-23 23:04:28.691680 funcs-0.7.1/funcs/primitives.py
+-rw-r--r--   0        0        0        0 2023-05-23 23:04:28.691680 funcs-0.7.1/funcs/py.typed
+-rw-r--r--   0        0        0     1113 2023-05-23 23:04:28.691680 funcs-0.7.1/funcs/reduction.py
+-rw-r--r--   0        0        0     1031 2023-05-23 23:04:28.691680 funcs-0.7.1/funcs/types.py
+-rw-r--r--   0        0        0     2346 2023-05-23 23:04:28.691680 funcs-0.7.1/funcs/unpacking.py
+-rw-r--r--   0        0        0     3212 2023-05-23 23:04:28.691680 funcs-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     4102 1970-01-01 00:00:00.000000 funcs-0.7.1/PKG-INFO
```

### Comparing `funcs-0.7.0/LICENSE` & `funcs-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `funcs-0.7.0/README.md` & `funcs-0.7.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 $ poetry add funcs
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-funcs = "^0.7.0"
+funcs = "^0.7.1"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.funcs]
 git = "https://github.com/nekitdev/funcs.git"
```

### Comparing `funcs-0.7.0/funcs/__init__.py` & `funcs-0.7.1/funcs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 __description__ = "Functional programming in Python."
 __url__ = "https://github.com/nekitdev/funcs"
 
 __title__ = "funcs"
 __author__ = "nekitdev"
 __license__ = "MIT"
-__version__ = "0.7.0"
+__version__ = "0.7.1"
 
 from funcs.application import apply, partial
 from funcs.callers import caller, method_caller
 from funcs.composition import compose, compose_once, pipe, pipe_once
 from funcs.debug import inspect, tap
 from funcs.decorators import wraps
 from funcs.flow import once, post_processing, reraise, reraise_with, suppress, wrap_with
```

### Comparing `funcs-0.7.0/funcs/application.py` & `funcs-0.7.1/funcs/application.py`

 * *Files identical despite different names*

### Comparing `funcs-0.7.0/funcs/callers.py` & `funcs-0.7.1/funcs/callers.py`

 * *Files identical despite different names*

### Comparing `funcs-0.7.0/funcs/composition.py` & `funcs-0.7.1/funcs/composition.py`

 * *Files identical despite different names*

### Comparing `funcs-0.7.0/funcs/debug.py` & `funcs-0.7.1/funcs/debug.py`

 * *Files identical despite different names*

### Comparing `funcs-0.7.0/funcs/flow.py` & `funcs-0.7.1/funcs/flow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from types import TracebackType as Traceback
-from typing import Callable, Generic, Optional, Type, TypeVar, final, overload
+from typing import Callable, Generic, Optional, Type, TypeVar, overload
 
 from attrs import frozen
 from typing_aliases import (
     AnyContextManager,
     AnyError,
     AnyErrorType,
     AnyErrorTypes,
     SimpleContextManager,
     Unary,
     is_subclass,
 )
-from typing_extensions import Literal, ParamSpec
+from typing_extensions import Literal, ParamSpec, final
 
 from funcs.decorators import wraps
 from funcs.types import MarkerOr, is_not_marker, marker
 
 __all__ = ("once", "reraise", "reraise_with", "suppress", "post_processing", "wrap_with")
 
 P = ParamSpec("P")
```

### Comparing `funcs-0.7.0/funcs/functions.py` & `funcs-0.7.1/funcs/functions.py`

 * *Files identical despite different names*

### Comparing `funcs-0.7.0/funcs/primitives.py` & `funcs-0.7.1/funcs/primitives.py`

 * *Files identical despite different names*

### Comparing `funcs-0.7.0/funcs/reduction.py` & `funcs-0.7.1/funcs/reduction.py`

 * *Files identical despite different names*

### Comparing `funcs-0.7.0/funcs/types.py` & `funcs-0.7.1/funcs/types.py`

 * *Files identical despite different names*

### Comparing `funcs-0.7.0/funcs/unpacking.py` & `funcs-0.7.1/funcs/unpacking.py`

 * *Files identical despite different names*

### Comparing `funcs-0.7.0/pyproject.toml` & `funcs-0.7.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "funcs"
-version = "0.7.0"
+version = "0.7.1"
 description = "Functional programming in Python."
 authors = ["nekitdev"]
 license = "MIT"
 
 readme = "README.md"
 
 homepage = "https://github.com/nekitdev/funcs"
@@ -136,15 +136,15 @@
 warn_unreachable = true
 
 warn_redundant_casts = true
 warn_unused_ignores = false  # compatibility
 
 [tool.changelogging]
 name = "funcs"
-version = "0.7.0"
+version = "0.7.1"
 url = "https://github.com/nekitdev/funcs"
 directory = "changes"
 output = "CHANGELOG.md"
 
 start_string = "<!-- changelogging: start -->"
 
 title_format = "{version} ({date})"
```

### Comparing `funcs-0.7.0/PKG-INFO` & `funcs-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcs
-Version: 0.7.0
+Version: 0.7.1
 Summary: Functional programming in Python.
 Home-page: https://github.com/nekitdev/funcs
 License: MIT
 Keywords: python,function,functional,paradigm
 Author: nekitdev
 Requires-Python: >=3.7
 Classifier: Development Status :: 5 - Production/Stable
@@ -71,15 +71,15 @@
 $ poetry add funcs
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-funcs = "^0.7.0"
+funcs = "^0.7.1"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.funcs]
 git = "https://github.com/nekitdev/funcs.git"
```

