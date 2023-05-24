# Comparing `tmp/serializer_Konchik-0.1.4.tar.gz` & `tmp/serializer_Konchik-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serializer_Konchik-0.1.4.tar", last modified: Mon May 22 17:06:16 2023, max compression
+gzip compressed data, was "serializer_Konchik-0.1.5.tar", last modified: Wed May 24 18:01:30 2023, max compression
```

## Comparing `serializer_Konchik-0.1.4.tar` & `serializer_Konchik-0.1.5.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 17:06:16.016859 serializer_Konchik-0.1.4/
--rw-rw-rw-   0        0        0      262 2023-05-22 17:06:16.016859 serializer_Konchik-0.1.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-22 17:06:15.990535 serializer_Konchik-0.1.4/serializer_Konchik/
--rw-rw-rw-   0        0        0      176 2023-05-22 17:04:23.000000 serializer_Konchik-0.1.4/serializer_Konchik/__init__.py
--rw-rw-rw-   0        0        0     2698 2023-05-20 13:25:33.000000 serializer_Konchik-0.1.4/serializer_Konchik/constants.py
-drwxrwxrwx   0        0        0        0 2023-05-22 17:06:16.009779 serializer_Konchik-0.1.4/serializer_Konchik/packer/
--rw-rw-rw-   0        0        0      110 2023-05-22 17:04:23.000000 serializer_Konchik-0.1.4/serializer_Konchik/packer/__init__.py
--rw-rw-rw-   0        0        0     5256 2023-05-20 20:31:34.000000 serializer_Konchik-0.1.4/serializer_Konchik/packer/packer.py
--rw-rw-rw-   0        0        0     5364 2023-05-20 20:11:55.000000 serializer_Konchik-0.1.4/serializer_Konchik/packer/unpacker.py
-drwxrwxrwx   0        0        0        0 2023-05-22 17:06:16.015863 serializer_Konchik-0.1.4/serializer_Konchik/serializer/
--rw-rw-rw-   0        0        0      226 2023-05-22 17:04:23.000000 serializer_Konchik-0.1.4/serializer_Konchik/serializer/__init__.py
--rw-rw-rw-   0        0        0     1366 2023-05-22 16:01:32.000000 serializer_Konchik-0.1.4/serializer_Konchik/serializer/base_serializer.py
--rw-rw-rw-   0        0        0     3331 2023-05-22 17:04:23.000000 serializer_Konchik-0.1.4/serializer_Konchik/serializer/json_serializer.py
--rw-rw-rw-   0        0        0      732 2023-05-22 17:04:23.000000 serializer_Konchik-0.1.4/serializer_Konchik/serializer/serializer_factory.py
--rw-rw-rw-   0        0        0     3884 2023-05-22 17:04:23.000000 serializer_Konchik-0.1.4/serializer_Konchik/serializer/xml_serializer.py
-drwxrwxrwx   0        0        0        0 2023-05-22 17:06:16.004712 serializer_Konchik-0.1.4/serializer_Konchik.egg-info/
--rw-rw-rw-   0        0        0      262 2023-05-22 17:06:15.000000 serializer_Konchik-0.1.4/serializer_Konchik.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      632 2023-05-22 17:06:15.000000 serializer_Konchik-0.1.4/serializer_Konchik.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 17:06:15.000000 serializer_Konchik-0.1.4/serializer_Konchik.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-22 17:06:15.000000 serializer_Konchik-0.1.4/serializer_Konchik.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-05-22 17:06:15.000000 serializer_Konchik-0.1.4/serializer_Konchik.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 17:06:16.016859 serializer_Konchik-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      595 2023-05-22 17:05:22.000000 serializer_Konchik-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 18:01:30.512196 serializer_Konchik-0.1.5/
+-rw-rw-rw-   0        0        0      262 2023-05-24 18:01:30.512196 serializer_Konchik-0.1.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-24 18:01:30.466194 serializer_Konchik-0.1.5/serializer_Konchik/
+-rw-rw-rw-   0        0        0      176 2023-05-22 17:04:23.000000 serializer_Konchik-0.1.5/serializer_Konchik/__init__.py
+-rw-rw-rw-   0        0        0     2740 2023-05-24 17:05:42.000000 serializer_Konchik-0.1.5/serializer_Konchik/constants.py
+-rw-rw-rw-   0        0        0      116 2023-05-24 17:50:50.000000 serializer_Konchik-0.1.5/serializer_Konchik/is_functions.py
+drwxrwxrwx   0        0        0        0 2023-05-24 18:01:30.488197 serializer_Konchik-0.1.5/serializer_Konchik/packer/
+-rw-rw-rw-   0        0        0      110 2023-05-22 17:04:23.000000 serializer_Konchik-0.1.5/serializer_Konchik/packer/__init__.py
+-rw-rw-rw-   0        0        0     5479 2023-05-24 17:40:53.000000 serializer_Konchik-0.1.5/serializer_Konchik/packer/packer.py
+-rw-rw-rw-   0        0        0     5477 2023-05-24 17:46:20.000000 serializer_Konchik-0.1.5/serializer_Konchik/packer/unpacker.py
+drwxrwxrwx   0        0        0        0 2023-05-24 18:01:30.511210 serializer_Konchik-0.1.5/serializer_Konchik/serializer/
+-rw-rw-rw-   0        0        0      226 2023-05-22 17:04:23.000000 serializer_Konchik-0.1.5/serializer_Konchik/serializer/__init__.py
+-rw-rw-rw-   0        0        0     1366 2023-05-22 16:01:32.000000 serializer_Konchik-0.1.5/serializer_Konchik/serializer/base_serializer.py
+-rw-rw-rw-   0        0        0     3331 2023-05-22 17:04:23.000000 serializer_Konchik-0.1.5/serializer_Konchik/serializer/json_serializer.py
+-rw-rw-rw-   0        0        0      732 2023-05-22 17:04:23.000000 serializer_Konchik-0.1.5/serializer_Konchik/serializer/serializer_factory.py
+-rw-rw-rw-   0        0        0     3884 2023-05-22 17:04:23.000000 serializer_Konchik-0.1.5/serializer_Konchik/serializer/xml_serializer.py
+drwxrwxrwx   0        0        0        0 2023-05-24 18:01:30.482212 serializer_Konchik-0.1.5/serializer_Konchik.egg-info/
+-rw-rw-rw-   0        0        0      262 2023-05-24 18:01:30.000000 serializer_Konchik-0.1.5/serializer_Konchik.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      667 2023-05-24 18:01:30.000000 serializer_Konchik-0.1.5/serializer_Konchik.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 18:01:30.000000 serializer_Konchik-0.1.5/serializer_Konchik.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-24 18:01:30.000000 serializer_Konchik-0.1.5/serializer_Konchik.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-24 18:01:30.000000 serializer_Konchik-0.1.5/serializer_Konchik.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-24 18:01:30.512196 serializer_Konchik-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      595 2023-05-24 17:59:35.000000 serializer_Konchik-0.1.5/setup.py
```

### Comparing `serializer_Konchik-0.1.4/serializer_Konchik/constants.py` & `serializer_Konchik-0.1.5/serializer_Konchik/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,14 +42,16 @@
                               types.MethodDescriptorType,
                               types.BuiltinFunctionType,
                               types.GetSetDescriptorType,
                               types.MappingProxyType)
 
 METHOD_DECORATORS: Final[list] = (classmethod, staticmethod)
 
+ITERATOR_TYPE: Final[str] = "iterator"
+
 
 class JsonRegularExpression(enum.Enum):
     INT = r"[+-]?\d+"
     FLOAT = fr"({INT}(?:\.\d+)?(?:e{INT})?)"
     BOOL = r"((True)|(False))\b"
     STR = r"\"((\\\")|[^\"])*\""
     NONE = r"\b(None)\b"
```

### Comparing `serializer_Konchik-0.1.4/serializer_Konchik/packer/packer.py` & `serializer_Konchik-0.1.5/serializer_Konchik/packer/packer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-from typing import Any
-from ..constants import (PRIMITIVES, COLLECTIONS, CODE_ATTRIBUTES,
-                         TYPE, VALUE,
-                         IGNORED_CLASS_ATTRIBUTES, IGNORED_TYPES)
 import inspect
+from typing import Any
 from types import FunctionType, ModuleType, CellType, GeneratorType
+from serializer_Konchik.is_functions import is_iterable
+from serializer_Konchik.constants import (PRIMITIVES, COLLECTIONS, CODE_ATTRIBUTES,
+                                          TYPE, VALUE, ITERATOR_TYPE,
+                                          IGNORED_CLASS_ATTRIBUTES, IGNORED_TYPES)
 
 
 class Packer:
 
     @staticmethod
     def pack(obj: Any) -> dict:
         """
@@ -21,58 +22,61 @@
         dictionary.
         """
 
         if isinstance(obj, PRIMITIVES):
             return {TYPE: type(obj).__name__,
                     VALUE: obj}
 
-        elif isinstance(obj, COLLECTIONS):
+        if isinstance(obj, COLLECTIONS):
             if isinstance(obj, dict):
                 return {TYPE: type(obj).__name__,
                         VALUE: [[Packer.pack(key), Packer.pack(value)]
                                 for key, value in obj.items()]}
             else:
                 return {TYPE: type(obj).__name__,
                         VALUE: [Packer.pack(item) for item in obj]}
 
-        elif inspect.isfunction(obj):
+        if inspect.isfunction(obj):
             return {TYPE: type(obj).__name__,
                     VALUE: Packer._pack_function(obj)}
 
-        elif inspect.iscode(obj):
+        if inspect.iscode(obj):
             return {TYPE: type(obj).__name__,
                     VALUE: {key: Packer.pack(value)
                             for key, value in inspect.getmembers(obj)
                             if key in CODE_ATTRIBUTES}}
 
-        elif isinstance(obj, CellType):
+        if isinstance(obj, CellType):
             return {TYPE: type(obj).__name__,
                     VALUE: Packer.pack(obj.cell_contents)}
 
-        elif inspect.isclass(obj):
+        if inspect.isclass(obj):
             return {TYPE: "class",
                     VALUE: Packer._pack_class(obj)}
 
-        elif isinstance(obj, property):
+        if isinstance(obj, property):
             return {TYPE: type(obj).__name__,
                     VALUE: {"fget": Packer.pack(obj.fget),
                             "fset": Packer.pack(obj.fset),
                             "fdel": Packer.pack(obj.fdel)}}
 
-        elif inspect.isgenerator(obj):
-            raise TypeError("Python does not support creating generators on the fly")
+        if is_iterable(obj):
+            return {TYPE: ITERATOR_TYPE,
+                    VALUE: [Packer.pack(item) for item in obj]}
+
+        # if inspect.isgenerator(obj):
+        #     raise TypeError("Python does not support creating generators on the fly")
 
-        elif inspect.ismethod(obj):
+        if inspect.ismethod(obj):
             return {TYPE: type(obj).__name__,
                     VALUE: Packer._pack_function(obj.__func__)}
 
-        else:
-            return {TYPE: "object",
-                    VALUE: {"__class__": Packer.pack(obj.__class__),
-                            "__vars__": {key: Packer.pack(value) for key, value in vars(obj)}}}
+        return {TYPE: "object",
+                VALUE: {"__class__": Packer.pack(obj.__class__),
+                        "__vars__": {key: Packer.pack(value) for key, value in vars(obj)}}}
 
     @staticmethod
     def _pack_function(obj: FunctionType, cls=None):
 
         return {"__name__": obj.__name__,
                 "__globals__": Packer._pack_globals(obj, cls),
                 "__closure__": Packer.pack(obj.__closure__),
```

### Comparing `serializer_Konchik-0.1.4/serializer_Konchik/packer/unpacker.py` & `serializer_Konchik-0.1.5/serializer_Konchik/packer/unpacker.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-import types
-
-from ..constants import (PRIMITIVES, COLLECTIONS, CODE_ATTRIBUTES,
-                         TYPE, VALUE, METHOD_DECORATORS)
 from types import NoneType, FunctionType, CodeType, CellType, MethodType
 import inspect
 import builtins
+from serializer_Konchik.constants import (PRIMITIVES, COLLECTIONS, CODE_ATTRIBUTES,
+                                          TYPE, VALUE, METHOD_DECORATORS, ITERATOR_TYPE)
 
 
 class Unpacker:
 
     @staticmethod
     def unpack(obj: dict):
         """
@@ -24,44 +22,46 @@
 
         if obj[TYPE] in tuple(map(lambda p: p.__name__, PRIMITIVES)):
             if obj[TYPE] == str(NoneType.__name__):
                 return None
             else:
                 return getattr(builtins, obj[TYPE])(obj[VALUE])
 
-        elif obj[TYPE] in tuple(map(lambda c: c.__name__, COLLECTIONS)):
+        if obj[TYPE] in tuple(map(lambda c: c.__name__, COLLECTIONS)):
             if obj[TYPE] == dict.__name__:
                 return {Unpacker.unpack(item[0]): Unpacker.unpack(item[1])
                         for item in obj[VALUE]}
             else:
                 return getattr(builtins, obj[TYPE])(Unpacker.unpack(item)
                                                     for item in obj[VALUE])
 
-        elif obj[TYPE] in [FunctionType.__name__, MethodType.__name__]:
+        if obj[TYPE] in [FunctionType.__name__, MethodType.__name__]:
             return Unpacker._unpack_function(obj[VALUE])
 
-        elif obj[TYPE] == CodeType.__name__:
+        if obj[TYPE] == CodeType.__name__:
             return Unpacker._unpack_code(obj[VALUE])
 
-        elif obj[TYPE] == CellType.__name__:
+        if obj[TYPE] == CellType.__name__:
             return CellType(Unpacker.unpack(obj[VALUE]))
 
-        elif obj[TYPE] == "class":
+        if obj[TYPE] == "class":
             return Unpacker._unpack_class(obj[VALUE])
 
-        elif obj[TYPE] in tuple(map(lambda md: md.__name__, METHOD_DECORATORS)):
+        if obj[TYPE] in tuple(map(lambda md: md.__name__, METHOD_DECORATORS)):
             return getattr(builtins, obj[TYPE])(Unpacker.unpack(obj[VALUE]))
 
-        elif obj[TYPE] == property.__name__:
+        if obj[TYPE] == property.__name__:
             return property(fget=Unpacker.unpack(obj[VALUE]["fget"]),
                             fset=Unpacker.unpack(obj[VALUE]["fset"]),
                             fdel=Unpacker.unpack(obj[VALUE]["fdel"]))
 
-        else:
-            return Unpacker._unpack_object(obj[VALUE])
+        if obj[TYPE] == ITERATOR_TYPE:
+            return iter(Unpacker.unpack(item) for item in obj[VALUE])
+
+        return Unpacker._unpack_object(obj[VALUE])
 
     @staticmethod
     def _unpack_function(obj: dict):
         code = Unpacker._unpack_code(obj["__code__"])
 
         globs = Unpacker._unpack_globals(obj["__globals__"], obj)
         globs["builtins"] = __import__("builtins")
```

### Comparing `serializer_Konchik-0.1.4/serializer_Konchik/serializer/base_serializer.py` & `serializer_Konchik-0.1.5/serializer_Konchik/serializer/base_serializer.py`

 * *Files identical despite different names*

### Comparing `serializer_Konchik-0.1.4/serializer_Konchik/serializer/json_serializer.py` & `serializer_Konchik-0.1.5/serializer_Konchik/serializer/json_serializer.py`

 * *Files identical despite different names*

### Comparing `serializer_Konchik-0.1.4/serializer_Konchik/serializer/serializer_factory.py` & `serializer_Konchik-0.1.5/serializer_Konchik/serializer/serializer_factory.py`

 * *Files identical despite different names*

### Comparing `serializer_Konchik-0.1.4/serializer_Konchik/serializer/xml_serializer.py` & `serializer_Konchik-0.1.5/serializer_Konchik/serializer/xml_serializer.py`

 * *Files identical despite different names*

### Comparing `serializer_Konchik-0.1.4/serializer_Konchik.egg-info/SOURCES.txt` & `serializer_Konchik-0.1.5/serializer_Konchik.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 setup.py
 serializer_Konchik/__init__.py
 serializer_Konchik/constants.py
+serializer_Konchik/is_functions.py
 serializer_Konchik.egg-info/PKG-INFO
 serializer_Konchik.egg-info/SOURCES.txt
 serializer_Konchik.egg-info/dependency_links.txt
 serializer_Konchik.egg-info/requires.txt
 serializer_Konchik.egg-info/top_level.txt
 serializer_Konchik/packer/__init__.py
 serializer_Konchik/packer/packer.py
```

### Comparing `serializer_Konchik-0.1.4/setup.py` & `serializer_Konchik-0.1.5/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Always prefer setuptools over distutils
 from setuptools import setup
 
 # This call to setup() does all the work
 setup(
     name="serializer_Konchik",
-    version="0.1.4",
+    version="0.1.5",
     description="JSON / XML serializer",
     author="Denis Konchik",
     author_email="denis.pptx@gmail.com",
     license="MIT",
     classifiers=[
         "Programming Language :: Python",
         "Operating System :: OS Independent"
```

