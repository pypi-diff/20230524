# Comparing `tmp/typing_inspect-0.7.1.tar.gz` & `tmp/typing_inspect-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/typing_inspect-0.7.1.tar", last modified: Mon Jun  7 16:11:58 2021, max compression
+gzip compressed data, was "typing_inspect-0.8.0.tar", last modified: Wed Aug 17 13:58:06 2022, max compression
```

## Comparing `typing_inspect-0.7.1.tar` & `typing_inspect-0.8.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ivan      (1000) ivan      (1000)        0 2021-06-07 16:11:58.000000 typing_inspect-0.7.1/
--rw-r--r--   0 ivan      (1000) ivan      (1000)       38 2021-06-07 16:11:58.000000 typing_inspect-0.7.1/setup.cfg
--rw-r--r--   0 ivan      (1000) ivan      (1000)     1345 2021-06-07 16:11:58.000000 typing_inspect-0.7.1/PKG-INFO
--rw-r--r--   0 ivan      (1000) ivan      (1000)     1799 2021-06-07 16:09:07.000000 typing_inspect-0.7.1/setup.py
-drwxr-xr-x   0 ivan      (1000) ivan      (1000)        0 2021-06-07 16:11:58.000000 typing_inspect-0.7.1/typing_inspect.egg-info/
--rw-r--r--   0 ivan      (1000) ivan      (1000)       89 2021-06-07 16:11:57.000000 typing_inspect-0.7.1/typing_inspect.egg-info/requires.txt
--rw-r--r--   0 ivan      (1000) ivan      (1000)     1345 2021-06-07 16:11:57.000000 typing_inspect-0.7.1/typing_inspect.egg-info/PKG-INFO
--rw-r--r--   0 ivan      (1000) ivan      (1000)       15 2021-06-07 16:11:57.000000 typing_inspect-0.7.1/typing_inspect.egg-info/top_level.txt
--rw-r--r--   0 ivan      (1000) ivan      (1000)      268 2021-06-07 16:11:58.000000 typing_inspect-0.7.1/typing_inspect.egg-info/SOURCES.txt
--rw-r--r--   0 ivan      (1000) ivan      (1000)        1 2021-06-07 16:11:57.000000 typing_inspect-0.7.1/typing_inspect.egg-info/dependency_links.txt
--rw-r--r--   0 ivan      (1000) ivan      (1000)    17471 2021-06-07 16:03:10.000000 typing_inspect-0.7.1/test_typing_inspect.py
--rw-r--r--   0 ivan      (1000) ivan      (1000)     3598 2021-06-05 21:25:40.000000 typing_inspect-0.7.1/README.md
--rw-r--r--   0 ivan      (1000) ivan      (1000)     1087 2021-06-05 21:25:40.000000 typing_inspect-0.7.1/LICENSE
--rw-r--r--   0 ivan      (1000) ivan      (1000)      108 2021-06-05 21:25:40.000000 typing_inspect-0.7.1/MANIFEST.in
--rw-r--r--   0 ivan      (1000) ivan      (1000)    26083 2021-06-07 16:03:10.000000 typing_inspect-0.7.1/typing_inspect.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2022-08-17 13:58:06.028567 typing_inspect-0.8.0/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     1087 2022-08-17 13:50:05.000000 typing_inspect-0.8.0/LICENSE
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      108 2022-08-17 13:50:05.000000 typing_inspect-0.8.0/MANIFEST.in
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     1325 2022-08-17 13:58:06.028567 typing_inspect-0.8.0/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     3598 2022-08-17 13:50:05.000000 typing_inspect-0.8.0/README.md
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2022-08-17 13:58:06.028567 typing_inspect-0.8.0/setup.cfg
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     1799 2022-08-17 13:52:41.000000 typing_inspect-0.8.0/setup.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)    18864 2022-08-17 13:50:05.000000 typing_inspect-0.8.0/test_typing_inspect.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2022-08-17 13:58:06.028567 typing_inspect-0.8.0/typing_inspect.egg-info/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     1325 2022-08-17 13:58:06.000000 typing_inspect-0.8.0/typing_inspect.egg-info/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      268 2022-08-17 13:58:06.000000 typing_inspect-0.8.0/typing_inspect.egg-info/SOURCES.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2022-08-17 13:58:06.000000 typing_inspect-0.8.0/typing_inspect.egg-info/dependency_links.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       89 2022-08-17 13:58:06.000000 typing_inspect-0.8.0/typing_inspect.egg-info/requires.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       15 2022-08-17 13:58:06.000000 typing_inspect-0.8.0/typing_inspect.egg-info/top_level.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)    27686 2022-08-17 13:50:05.000000 typing_inspect-0.8.0/typing_inspect.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `typing_inspect-0.7.1/PKG-INFO` & `typing_inspect-0.8.0/typing_inspect.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
-Name: typing_inspect
-Version: 0.7.1
+Name: typing-inspect
+Version: 0.8.0
 Summary: Runtime inspection utilities for typing module.
 Home-page: https://github.com/ilevkivskyi/typing_inspect
 Author: Ivan Levkivskyi
 Author-email: levkivskyi@gmail.com
 License: MIT
 Keywords: typing function annotations type hints hinting checking checker typehints typehinting typechecking inspect reflection introspection
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
@@ -27,9 +26,7 @@
 License-File: LICENSE
 
 Typing Inspect
 ==============
 
 The "typing_inspect" module defines experimental API for runtime
 inspection of types defined in the standard "typing" module.
-
-
```

### Comparing `typing_inspect-0.7.1/setup.py` & `typing_inspect-0.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 
 # NOTE: This package must support Python 2.7 in addition to Python 3.x
 
 import sys
 from setuptools import setup
 
-version = '0.7.1'
+version = '0.8.0'
 description = 'Runtime inspection utilities for typing module.'
 long_description = '''
 Typing Inspect
 ==============
 
 The "typing_inspect" module defines experimental API for runtime
 inspection of types defined in the standard "typing" module.
```

### Comparing `typing_inspect-0.7.1/typing_inspect.egg-info/PKG-INFO` & `typing_inspect-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
-Name: typing-inspect
-Version: 0.7.1
+Name: typing_inspect
+Version: 0.8.0
 Summary: Runtime inspection utilities for typing module.
 Home-page: https://github.com/ilevkivskyi/typing_inspect
 Author: Ivan Levkivskyi
 Author-email: levkivskyi@gmail.com
 License: MIT
 Keywords: typing function annotations type hints hinting checking checker typehints typehinting typechecking inspect reflection introspection
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
@@ -27,9 +26,7 @@
 License-File: LICENSE
 
 Typing Inspect
 ==============
 
 The "typing_inspect" module defines experimental API for runtime
 inspection of types defined in the standard "typing" module.
-
-
```

### Comparing `typing_inspect-0.7.1/test_typing_inspect.py` & `typing_inspect-0.8.0/test_typing_inspect.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 import sys
+
+import pytest
+
 from typing_inspect import (
     is_generic_type, is_callable_type, is_new_type, is_tuple_type, is_union_type,
     is_optional_type, is_final_type, is_literal_type, is_typevar, is_classvar,
     is_forward_ref, get_origin, get_parameters, get_last_args, get_args, get_bound,
     get_constraints, get_generic_type, get_generic_bases, get_last_origin,
-    typed_dict_keys, get_forward_arg, WITH_FINAL, WITH_LITERAL, LEGACY_TYPING)
+    typed_dict_keys, get_forward_arg, WITH_FINAL, WITH_LITERAL, LEGACY_TYPING, WITH_NEWTYPE,
+)
 from unittest import TestCase, main, skipIf, skipUnless
 from typing import (
     Union, Callable, Optional, TypeVar, Sequence, AnyStr, Mapping,
     MutableMapping, Iterable, Generic, List, Any, Dict, Tuple, NamedTuple,
 )
 
 from mypy_extensions import TypedDict as METypedDict
 from typing_extensions import TypedDict as TETypedDict
 from typing_extensions import Final
 from typing_extensions import Literal
-
-# Does this raise an exception ?
-#      from typing import NewType
-if sys.version_info < (3, 5, 2):
-    WITH_NEWTYPE = False
-else:
-    from typing import NewType
-    WITH_NEWTYPE = True
-
+from typing_extensions import NewType as NewType_
 
 # Does this raise an exception ?
 #      from typing import ClassVar
 if sys.version_info < (3, 5, 3):
     WITH_CLASSVAR = False
     CLASSVAR_GENERIC = []
     CLASSVAR_TYPEVAR = []
@@ -116,14 +112,26 @@
 
 PY36 = sys.version_info[:3] >= (3, 6, 0)
 PY39 = sys.version_info[:3] >= (3, 9, 0)
 if PY36:
     exec(PY36_TESTS)
 
 
+# It is important for the test that this function is called 'NewType' to simulate the same __qualname__
+# - which is "NewType.<locals>.new_type" - as typing.NewType has, i.e. it should be checked that is_new_type
+# still do not accept a function which has the same __qualname__ and an attribute called __supertype__.
+def NewType(name, tp):
+    def new_type(x):
+        return x
+
+    new_type.__name__ = name
+    new_type.__supertype__ = tp
+    return new_type
+
+
 class IsUtilityTestCase(TestCase):
     def sample_test(self, fun, samples, nonsamples):
         msg = "Error asserting that %s(%s) is %s"
         for s in samples:
             self.assertTrue(fun(s), msg=msg % (fun.__name__, str(s), 'True'))
         for s in nonsamples:
             self.assertFalse(fun(s), msg=msg % (fun.__name__, str(s), 'False'))
@@ -164,14 +172,22 @@
     def test_union(self):
         T = TypeVar('T')
         S = TypeVar('S')
         samples = [Union, Union[T, int], Union[int, Union[T, S]]]
         nonsamples = [int, Union[int, int], [], Iterable[Any]]
         self.sample_test(is_union_type, samples, nonsamples)
 
+    @pytest.mark.skipif(sys.version_info < (3, 10), reason="requires 3.10 or higher")
+    def test_union_pep604(self):
+        T = TypeVar('T')
+        S = TypeVar('S')
+        samples = [T | int, int | (T | S), int | str]
+        nonsamples = [int, int | int, [], Iterable[Any]]
+        self.sample_test(is_union_type, samples, nonsamples)
+
     def test_optional_type(self):
         T = TypeVar('T')
         samples = [type(None),                # none type
                    Optional[int],             # direct union to none type 1
                    Optional[T],               # direct union to none type 2
                    Union[int, type(None)],    # direct union to none type 4
                    ]
@@ -244,30 +260,45 @@
         samples = [ClassVar, ClassVar[int], ClassVar[List[T]]]
         nonsamples = [int, 42, Iterable, List[int], type, T]
         self.sample_test(is_classvar, samples, nonsamples)
 
     @skipIf(not WITH_NEWTYPE, "NewType is not present")
     def test_new_type(self):
         T = TypeVar('T')
+
+        class WithAttrSuperTypeCls:
+            __supertype__ = str
+
+        class WithAttrSuperTypeObj:
+            def __init__(self):
+                self.__supertype__ = str
+
         samples = [
-            NewType('A', int),
-            NewType('B', complex),
-            NewType('C', List[int]),
-            NewType('D', Union['p', 'y', 't', 'h', 'o', 'n']),
-            NewType('E', List[Dict[str, float]]),
-            NewType('F', NewType('F_', int)),
+            NewType_,
+            NewType_('A', int),
+            NewType_('B', complex),
+            NewType_('C', List[int]),
+            NewType_('D', Union['p', 'y', 't', 'h', 'o', 'n']),
+            NewType_('E', List[Dict[str, float]]),
+            NewType_('F', NewType('F_', int)),
         ]
         nonsamples = [
             int,
             42,
             Iterable,
             List[int],
             Union["u", "v"],
             type,
             T,
+            NewType,
+            NewType('N', int),
+            WithAttrSuperTypeCls,
+            WithAttrSuperTypeCls(),
+            WithAttrSuperTypeObj,
+            WithAttrSuperTypeObj(),
         ]
         self.sample_test(is_new_type, samples, nonsamples)
 
     def test_is_forward_ref(self):
         samples = []
         nonsamples = []
         for tp in (
@@ -302,14 +333,16 @@
     def test_origin(self):
         T = TypeVar('T')
         self.assertEqual(get_origin(int), None)
         if WITH_CLASSVAR:
             self.assertEqual(get_origin(ClassVar[int]), None)
         self.assertEqual(get_origin(Generic), Generic)
         self.assertEqual(get_origin(Generic[T]), Generic)
+        # Cannot use assertEqual on Py3.5.2.
+        self.assertIs(get_origin(Literal[42]), Literal)
         if PY39:
             self.assertEqual(get_origin(list[int]), list)
         if GENERIC_TUPLE_PARAMETRIZABLE:
             tp = List[Tuple[T, T]][int]
             self.assertEqual(get_origin(tp), list if NEW_TYPING else List)
 
     def test_parameters(self):
@@ -401,14 +434,18 @@
         if PY39:
             self.assertEqual(get_args(list[int]), (int,))
             self.assertEqual(get_args(tuple[int, str]), (int, str))
             self.assertEqual(get_args(list[list[int]]), (list[int],))
             # This would return (~T,) before Python 3.9.
             self.assertEqual(get_args(List), ())
 
+        if sys.version_info >= (3, 10):
+            self.assertEqual(get_args(int | str), (int, str))
+            self.assertEqual(get_args((int | tuple[T, int])[str]), (int, tuple[str, int]))
+
     def test_bound(self):
         T = TypeVar('T')
         TB = TypeVar('TB', bound=int)
         self.assertEqual(get_bound(T), None)
         self.assertEqual(get_bound(TB), int)
 
     def test_constraints(self):
```

### Comparing `typing_inspect-0.7.1/README.md` & `typing_inspect-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `typing_inspect-0.7.1/LICENSE` & `typing_inspect-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `typing_inspect-0.7.1/typing_inspect.py` & `typing_inspect-0.8.0/typing_inspect.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,43 +12,51 @@
 
 from mypy_extensions import _TypedDictMeta as _TypedDictMeta_Mypy
 
 # See comments in typing_extensions source on why the switch is at 3.9.2
 if (3, 4, 0) <= sys.version_info[:3] < (3, 9, 2):
     from typing_extensions import _TypedDictMeta as _TypedDictMeta_TE
 elif sys.version_info[:3] >= (3, 9, 2):
-    # typing_extensions.TypedDict is a re-export from typing.
-    from typing import _TypedDictMeta as _TypedDictMeta_TE
+    # Situation with typing_extensions.TypedDict is complicated.
+    # Use the one defined in typing_extentions, and if there is none,
+    # fall back to typing.
+    try:
+        from typing_extensions import _TypedDictMeta as _TypedDictMeta_TE
+    except ImportError:
+        from typing import _TypedDictMeta as _TypedDictMeta_TE
 else:
     # typing_extensions.TypedDict is a re-export from typing.
     from typing import TypedDict
     _TypedDictMeta_TE = type(TypedDict)
 
 NEW_TYPING = sys.version_info[:3] >= (3, 7, 0)  # PEP 560
 if NEW_TYPING:
     import collections.abc
 
 WITH_FINAL = True
 WITH_LITERAL = True
 WITH_CLASSVAR = True
+WITH_NEWTYPE = True
 LEGACY_TYPING = False
 
 if NEW_TYPING:
     from typing import (
-        Generic, Callable, Union, TypeVar, ClassVar, Tuple, _GenericAlias, ForwardRef
+        Generic, Callable, Union, TypeVar, ClassVar, Tuple, _GenericAlias,
+        ForwardRef, NewType,
     )
     from typing_extensions import Final, Literal
     if sys.version_info[:3] >= (3, 9, 0):
         from typing import _SpecialGenericAlias
         typingGenericAlias = (_GenericAlias, _SpecialGenericAlias, types.GenericAlias)
     else:
         typingGenericAlias = (_GenericAlias,)
 else:
     from typing import (
-        Callable, CallableMeta, Union, Tuple, TupleMeta, TypeVar, GenericMeta, _ForwardRef
+        Callable, CallableMeta, Union, Tuple, TupleMeta, TypeVar, GenericMeta,
+        _ForwardRef,
     )
     try:
         from typing import _Union, _ClassVar
     except ImportError:
         # support for very old typing module <=3.5.3
         _Union = type(Union)
         WITH_CLASSVAR = False
@@ -59,21 +67,29 @@
     except ImportError:  # python 2.7
         try:
             from typing import _Final
         except ImportError:
             WITH_FINAL = False
 
     try:  # python 3.6
-        from typing_extensions import _Literal
+        from typing_extensions import Literal
     except ImportError:  # python 2.7
         try:
-            from typing import _Literal
+            from typing import Literal
         except ImportError:
             WITH_LITERAL = False
 
+    try:  # python < 3.5.2
+        from typing_extensions import NewType
+    except ImportError:
+        try:
+            from typing import NewType
+        except ImportError:
+            WITH_NEWTYPE = False
+
 
 def _gorg(cls):
     """This function exists for compatibility with old typing versions."""
     assert isinstance(cls, GenericMeta)
     if hasattr(cls, '_gorg'):
         return cls._gorg
     while cls.__origin__ is not None:
@@ -190,33 +206,42 @@
     """
     if NEW_TYPING:
         return (tp is Final or
                 isinstance(tp, typingGenericAlias) and tp.__origin__ is Final)
     return WITH_FINAL and type(tp) is _Final
 
 
+try:
+    MaybeUnionType = types.UnionType
+except AttributeError:
+    MaybeUnionType = None
+
+
 def is_union_type(tp):
     """Test if the type is a union type. Examples::
 
         is_union_type(int) == False
         is_union_type(Union) == True
         is_union_type(Union[int, int]) == False
         is_union_type(Union[T, int]) == True
+        is_union_type(int | int) == False
+        is_union_type(T | int) == True
     """
     if NEW_TYPING:
         return (tp is Union or
-                isinstance(tp, typingGenericAlias) and tp.__origin__ is Union)
+                (isinstance(tp, typingGenericAlias) and tp.__origin__ is Union) or
+                (MaybeUnionType and isinstance(tp, MaybeUnionType)))
     return type(tp) is _Union
 
 
 def is_literal_type(tp):
     if NEW_TYPING:
         return (tp is Literal or
                 isinstance(tp, typingGenericAlias) and tp.__origin__ is Literal)
-    return WITH_LITERAL and type(tp) is _Literal
+    return WITH_LITERAL and type(tp) is type(Literal)
 
 
 def is_typevar(tp):
     """Test if the type represents a type variable. Examples::
 
         is_typevar(int) == False
         is_typevar(T) == True
@@ -243,18 +268,32 @@
         return False
 
 
 def is_new_type(tp):
     """Tests if the type represents a distinct type. Examples::
 
         is_new_type(int) == False
+        is_new_type(NewType) == True
         is_new_type(NewType('Age', int)) == True
         is_new_type(NewType('Scores', List[Dict[str, float]])) == True
     """
-    return getattr(tp, '__supertype__', None) is not None
+    if not WITH_NEWTYPE:
+        return False
+    elif sys.version_info[:3] >= (3, 10, 0) and sys.version_info.releaselevel != 'beta':
+        return tp is NewType or isinstance(tp, NewType)
+    elif sys.version_info[:3] >= (3, 0, 0):
+        return (tp is NewType or
+                (getattr(tp, '__supertype__', None) is not None and
+                 getattr(tp, '__qualname__', '') == 'NewType.<locals>.new_type' and
+                 tp.__module__ in ('typing', 'typing_extensions')))
+    else:  # python 2
+        # __qualname__ is not available in python 2, so we simplify the test here
+        return (tp is NewType or
+                (getattr(tp, '__supertype__', None) is not None and
+                 tp.__module__ in ('typing', 'typing_extensions')))
 
 
 def is_forward_ref(tp):
     """Tests if the type is a :class:`typing.ForwardRef`. Examples::
 
         u = Union["Milk", Way]
         args = get_args(u)
@@ -309,14 +348,16 @@
         return None
     if isinstance(tp, GenericMeta):
         return _gorg(tp)
     if is_union_type(tp):
         return Union
     if is_tuple_type(tp):
         return Tuple
+    if is_literal_type(tp):
+        return Literal
 
     return None
 
 
 def get_parameters(tp):
     """Return type parameters of a parameterizable type as a tuple
     in lexicographic order. Parameterizable types are generic types,
@@ -469,14 +510,16 @@
             raise ValueError('evaluate can only be True in Python >= 3.7')
         # Note special aliases on Python 3.9 don't have __args__.
         if isinstance(tp, typingGenericAlias) and hasattr(tp, '__args__'):
             res = tp.__args__
             if get_origin(tp) is collections.abc.Callable and res[0] is not Ellipsis:
                 res = (list(res[:-1]), res[-1])
             return res
+        if MaybeUnionType and isinstance(tp, MaybeUnionType):
+            return tp.__args__
         return ()
     if is_classvar(tp) or is_final_type(tp):
         return (tp.__type__,) if tp.__type__ is not None else ()
     if is_literal_type(tp):
         return tp.__values__ or ()
     if (
         is_generic_type(tp) or is_union_type(tp) or
```

