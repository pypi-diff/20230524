# Comparing `tmp/objinspect-0.2.1.tar.gz` & `tmp/objinspect-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "objinspect-0.2.1.tar", last modified: Mon May 15 19:56:34 2023, max compression
+gzip compressed data, was "objinspect-0.2.2.tar", last modified: Wed May 24 19:09:01 2023, max compression
```

## Comparing `objinspect-0.2.1.tar` & `objinspect-0.2.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:56:34.199545 objinspect-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-15 19:56:23.000000 objinspect-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-05-15 19:56:34.199545 objinspect-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-05-15 19:56:23.000000 objinspect-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:56:34.199545 objinspect-0.2.1/objinspect/
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-15 19:56:23.000000 objinspect-0.2.1/objinspect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-05-15 19:56:23.000000 objinspect-0.2.1/objinspect/_class.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-15 19:56:23.000000 objinspect-0.2.1/objinspect/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-05-15 19:56:23.000000 objinspect-0.2.1/objinspect/function.py
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-05-15 19:56:23.000000 objinspect-0.2.1/objinspect/method.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-05-15 19:56:23.000000 objinspect-0.2.1/objinspect/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-15 19:56:23.000000 objinspect-0.2.1/objinspect/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:56:34.199545 objinspect-0.2.1/objinspect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-05-15 19:56:34.000000 objinspect-0.2.1/objinspect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-15 19:56:34.000000 objinspect-0.2.1/objinspect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 19:56:34.000000 objinspect-0.2.1/objinspect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-15 19:56:34.000000 objinspect-0.2.1/objinspect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-15 19:56:34.000000 objinspect-0.2.1/objinspect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-05-15 19:56:23.000000 objinspect-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 19:56:34.199545 objinspect-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 19:56:23.000000 objinspect-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:09:01.292092 objinspect-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-24 19:08:47.000000 objinspect-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-05-24 19:09:01.292092 objinspect-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-05-24 19:08:47.000000 objinspect-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:09:01.292092 objinspect-0.2.2/objinspect/
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-24 19:08:47.000000 objinspect-0.2.2/objinspect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-05-24 19:08:47.000000 objinspect-0.2.2/objinspect/_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-24 19:08:47.000000 objinspect-0.2.2/objinspect/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-05-24 19:08:47.000000 objinspect-0.2.2/objinspect/function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-05-24 19:08:47.000000 objinspect-0.2.2/objinspect/method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-05-24 19:08:47.000000 objinspect-0.2.2/objinspect/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-05-24 19:08:47.000000 objinspect-0.2.2/objinspect/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:09:01.292092 objinspect-0.2.2/objinspect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-05-24 19:09:01.000000 objinspect-0.2.2/objinspect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-24 19:09:01.000000 objinspect-0.2.2/objinspect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 19:09:01.000000 objinspect-0.2.2/objinspect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-24 19:09:01.000000 objinspect-0.2.2/objinspect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-24 19:09:01.000000 objinspect-0.2.2/objinspect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-05-24 19:08:47.000000 objinspect-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 19:09:01.292092 objinspect-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 19:08:47.000000 objinspect-0.2.2/setup.py
```

### Comparing `objinspect-0.2.1/LICENSE` & `objinspect-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `objinspect-0.2.1/PKG-INFO` & `objinspect-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: objinspect
-Version: 0.2.1
+Version: 0.2.2
 Summary: View the structure of Python classes and functions
 Author-email: Žiga Ivanšek <ziga.ivansek@gmail.com>
 Project-URL: Repository, https://github.com/zigai/obj-inspect
 Keywords: objinspect,object inspection,code introspection,python inspect
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `objinspect-0.2.1/README.md` & `objinspect-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `objinspect-0.2.1/objinspect/__init__.py` & `objinspect-0.2.2/objinspect/__init__.py`

 * *Files identical despite different names*

### Comparing `objinspect-0.2.1/objinspect/_class.py` & `objinspect-0.2.2/objinspect/_class.py`

 * *Files identical despite different names*

### Comparing `objinspect-0.2.1/objinspect/function.py` & `objinspect-0.2.2/objinspect/function.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import inspect
+from types import NoneType
 from typing import Any, Callable
 
 import docstring_parser
 from docstring_parser import Docstring
 
 from objinspect.parameter import Parameter
 
@@ -47,23 +48,25 @@
         self.skip_self = skip_self
         self.name: str = self.func.__name__
         self.docstring = inspect.getdoc(self.func)
         self.has_docstring = _has_docstr(self.docstring)
         self._parsed_docstr: Docstring | None = (
             docstring_parser.parse(self.docstring) if self.has_docstring else None  # type: ignore
         )
-        self._parameters = self._find_parameters()
+        self.return_type = NoneType
+        self._parameters = self._get_parameters()
         self.description = _get_docstr_desc(self._parsed_docstr)
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(name='{self.name}', parameters={len(self._parameters)}, description='{self.description}')"
 
-    def _find_parameters(self) -> dict[str, Parameter]:
-        args = inspect.signature(self.func)
-        params = [Parameter.from_inspect_param(i) for i in args.parameters.values()]
+    def _get_parameters(self) -> dict[str, Parameter]:
+        signature = inspect.signature(self.func)
+        params = [Parameter.from_inspect_param(i) for i in signature.parameters.values()]
+        self.return_type = signature.return_annotation
 
         # Try finding descriptions for parameters
         if self._parsed_docstr is not None:
             params_mapping = {par.arg_name: par for par in self._parsed_docstr.params}
             for param in params:
                 if parameter := params_mapping.get(param.name, False):
                     if parameter.description:  # type: ignore
```

### Comparing `objinspect-0.2.1/objinspect/method.py` & `objinspect-0.2.2/objinspect/method.py`

 * *Files identical despite different names*

### Comparing `objinspect-0.2.1/objinspect/parameter.py` & `objinspect-0.2.2/objinspect/parameter.py`

 * *Files identical despite different names*

### Comparing `objinspect-0.2.1/objinspect/util.py` & `objinspect-0.2.2/objinspect/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,24 +63,24 @@
     >>> import math
     >>> call_method(math, "pow", args=(2, 2))
     4.0
     """
     return getattr(obj, name)(*args, **kwargs)
 
 
-def get_uninherited_method_names(cls) -> list[str]:
+def get_uninherited_methods(cls) -> list[str]:
     """
     Get the methods of a class that are not inherited from its parent classes.
     """
     return [
         name
         for name, method in cls.__dict__.items()
         if isinstance(method, (FunctionType, classmethod, staticmethod))
     ]
 
 
 __all__ = [
     "type_to_str",
     "get_enum_choices",
     "call_method",
-    "get_uninherited_method_names",
+    "get_uninherited_methods",
 ]
```

### Comparing `objinspect-0.2.1/objinspect.egg-info/PKG-INFO` & `objinspect-0.2.2/objinspect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: objinspect
-Version: 0.2.1
+Version: 0.2.2
 Summary: View the structure of Python classes and functions
 Author-email: Žiga Ivanšek <ziga.ivansek@gmail.com>
 Project-URL: Repository, https://github.com/zigai/obj-inspect
 Keywords: objinspect,object inspection,code introspection,python inspect
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `objinspect-0.2.1/pyproject.toml` & `objinspect-0.2.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "objinspect"
-version = "0.2.1"
+version = "0.2.2"
 description = "View the structure of Python classes and functions"
 authors = [{ name = "Žiga Ivanšek", email = "ziga.ivansek@gmail.com" }]
 license = { file = "LICENSE.txt" }
 readme = "README.md"
 requires-python = ">=3.10"
 
 classifiers = [
-    "Intended Audience :: Developers",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3.10",
-     "Programming Language :: Python :: 3.11",
-    "Programming Language :: Python :: 3 :: Only",
-    "Topic :: Software Development :: Libraries :: Python Modules",
+  "Intended Audience :: Developers",
+  "License :: OSI Approved :: MIT License",
+  "Operating System :: OS Independent",
+  "Programming Language :: Python",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3 :: Only",
+  "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 keywords = [
   "objinspect",
   "object inspection",
   "code introspection",
   "python inspect",
@@ -42,32 +42,32 @@
 line-length = 100
 target_version = ['py310']
 
 [tool.ruff]
 line-length = 100
 extend-ignore = ["E731", "E741", "N802", "N803", "N806", "E501"]
 exclude = [
-    ".bzr",
-    ".direnv",
-    ".eggs",
-    ".git",
-    ".hg",
-    ".mypy_cache",
-    ".nox",
-    ".pants.d",
-    ".pytype",
-    ".ruff_cache",
-    ".svn",
-    ".tox",
-    ".venv",
-    "__pypackages__",
-    "_build",
-    "buck-out",
-    "build",
-    "dist",
-    "node_modules",
-    "venv",
-    "tests",
+  ".bzr",
+  ".direnv",
+  ".eggs",
+  ".git",
+  ".hg",
+  ".mypy_cache",
+  ".nox",
+  ".pants.d",
+  ".pytype",
+  ".ruff_cache",
+  ".svn",
+  ".tox",
+  ".venv",
+  "__pypackages__",
+  "_build",
+  "buck-out",
+  "build",
+  "dist",
+  "node_modules",
+  "venv",
+  "tests",
 ]
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["F401", "E402"]
```

