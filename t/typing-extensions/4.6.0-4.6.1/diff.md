# Comparing `tmp/typing_extensions-4.6.0.tar.gz` & `tmp/typing_extensions-4.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typing_extensions-4.6.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "typing_extensions-4.6.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `typing_extensions-4.6.0.tar` & `typing_extensions-4.6.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    10106 2023-05-23 00:07:02.454501 typing_extensions-4.6.0/CHANGELOG.md
--rw-r--r--   0        0        0    12787 2022-12-31 19:31:45.654412 typing_extensions-4.6.0/LICENSE
--rw-r--r--   0        0        0     1290 2023-05-22 00:14:41.277524 typing_extensions-4.6.0/README.md
--rw-r--r--   0        0        0     1916 2023-05-23 00:07:02.456585 typing_extensions-4.6.0/pyproject.toml
--rw-r--r--   0        0        0      426 2022-12-31 19:31:45.655964 typing_extensions-4.6.0/src/_typed_dict_test_helper.py
--rw-r--r--   0        0        0   165606 2023-05-22 14:09:42.548954 typing_extensions-4.6.0/src/test_typing_extensions.py
--rw-r--r--   0        0        0   102170 2023-05-23 00:00:42.513644 typing_extensions-4.6.0/src/typing_extensions.py
--rw-r--r--   0        0        0      135 2023-05-22 00:37:39.060665 typing_extensions-4.6.0/tox.ini
--rw-r--r--   0        0        0     2786 1970-01-01 00:00:00.000000 typing_extensions-4.6.0/PKG-INFO
+-rw-r--r--   0        0        0    10437 2023-05-24 03:05:07.789039 typing_extensions-4.6.1/CHANGELOG.md
+-rw-r--r--   0        0        0    12787 2022-12-31 19:31:45.654412 typing_extensions-4.6.1/LICENSE
+-rw-r--r--   0        0        0     1290 2023-05-22 00:14:41.277524 typing_extensions-4.6.1/README.md
+-rw-r--r--   0        0        0     1916 2023-05-24 03:05:07.789784 typing_extensions-4.6.1/pyproject.toml
+-rw-r--r--   0        0        0      426 2022-12-31 19:31:45.655964 typing_extensions-4.6.1/src/_typed_dict_test_helper.py
+-rw-r--r--   0        0        0   168884 2023-05-24 03:02:38.054358 typing_extensions-4.6.1/src/test_typing_extensions.py
+-rw-r--r--   0        0        0   104451 2023-05-24 03:02:38.059891 typing_extensions-4.6.1/src/typing_extensions.py
+-rw-r--r--   0        0        0      135 2023-05-22 00:37:39.060665 typing_extensions-4.6.1/tox.ini
+-rw-r--r--   0        0        0     2786 1970-01-01 00:00:00.000000 typing_extensions-4.6.1/PKG-INFO
```

### Comparing `typing_extensions-4.6.0/CHANGELOG.md` & `typing_extensions-4.6.1/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+# Release 4.6.1 (May 23, 2023)
+
+- Change deprecated `@runtime` to formal API `@runtime_checkable` in the error
+  message. Patch by Xuehai Pan.
+- Fix regression in 4.6.0 where attempting to define a `Protocol` that was
+  generic over a `ParamSpec` or a `TypeVarTuple` would cause `TypeError` to be
+  raised. Patch by Alex Waygood.
+
 # Release 4.6.0 (May 22, 2023)
 
 - `typing_extensions` is now documented at
   https://typing-extensions.readthedocs.io/en/latest/. Patch by Jelle Zijlstra.
 - Add `typing_extensions.Buffer`, a marker class for buffer types, as proposed
   by PEP 688. Equivalent to `collections.abc.Buffer` in Python 3.12. Patch by
   Jelle Zijlstra.
```

### Comparing `typing_extensions-4.6.0/LICENSE` & `typing_extensions-4.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `typing_extensions-4.6.0/README.md` & `typing_extensions-4.6.1/README.md`

 * *Files identical despite different names*

### Comparing `typing_extensions-4.6.0/pyproject.toml` & `typing_extensions-4.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [build-system]
 requires = ["flit_core >=3.4,<4"]
 build-backend = "flit_core.buildapi"
 
 # Project metadata
 [project]
 name = "typing_extensions"
-version = "4.6.0"
+version = "4.6.1"
 description = "Backported and Experimental Type Hints for Python 3.7+"
 readme = "README.md"
 requires-python = ">=3.7"
 license = { file = "LICENSE" }
 keywords = [
     "annotations",
     "backport",
```

### Comparing `typing_extensions-4.6.0/src/test_typing_extensions.py` & `typing_extensions-4.6.1/src/test_typing_extensions.py`

 * *Files 1% similar despite different names*

```diff
@@ -2609,14 +2609,70 @@
             pass
 
         class CustomProtocolWithoutInitB(Protocol):
             pass
 
         self.assertEqual(CustomProtocolWithoutInitA.__init__, CustomProtocolWithoutInitB.__init__)
 
+    def test_protocol_generic_over_paramspec(self):
+        P = ParamSpec("P")
+        T = TypeVar("T")
+        T2 = TypeVar("T2")
+
+        class MemoizedFunc(Protocol[P, T, T2]):
+            cache: typing.Dict[T2, T]
+            def __call__(self, *args: P.args, **kwargs: P.kwargs) -> T: ...
+
+        self.assertEqual(MemoizedFunc.__parameters__, (P, T, T2))
+        self.assertTrue(MemoizedFunc._is_protocol)
+
+        with self.assertRaises(TypeError):
+            MemoizedFunc[[int, str, str]]
+
+        if sys.version_info >= (3, 10):
+            # These unfortunately don't pass on <=3.9,
+            # due to typing._type_check on older Python versions
+            X = MemoizedFunc[[int, str, str], T, T2]
+            self.assertEqual(X.__parameters__, (T, T2))
+            self.assertEqual(X.__args__, ((int, str, str), T, T2))
+
+            Y = X[bytes, memoryview]
+            self.assertEqual(Y.__parameters__, ())
+            self.assertEqual(Y.__args__, ((int, str, str), bytes, memoryview))
+
+    def test_protocol_generic_over_typevartuple(self):
+        Ts = TypeVarTuple("Ts")
+        T = TypeVar("T")
+        T2 = TypeVar("T2")
+
+        class MemoizedFunc(Protocol[Unpack[Ts], T, T2]):
+            cache: typing.Dict[T2, T]
+            def __call__(self, *args: Unpack[Ts]) -> T: ...
+
+        self.assertEqual(MemoizedFunc.__parameters__, (Ts, T, T2))
+        self.assertTrue(MemoizedFunc._is_protocol)
+
+        things = "arguments" if sys.version_info >= (3, 11) else "parameters"
+
+        # A bug was fixed in 3.11.1
+        # (https://github.com/python/cpython/commit/74920aa27d0c57443dd7f704d6272cca9c507ab3)
+        # That means this assertion doesn't pass on 3.11.0,
+        # but it passes on all other Python versions
+        if sys.version_info[:3] != (3, 11, 0):
+            with self.assertRaisesRegex(TypeError, f"Too few {things}"):
+                MemoizedFunc[int]
+
+        X = MemoizedFunc[int, T, T2]
+        self.assertEqual(X.__parameters__, (T, T2))
+        self.assertEqual(X.__args__, (int, T, T2))
+
+        Y = X[bytes, memoryview]
+        self.assertEqual(Y.__parameters__, ())
+        self.assertEqual(Y.__args__, (int, bytes, memoryview))
+
 
 class Point2DGeneric(Generic[T], TypedDict):
     a: T
     b: T
 
 
 class Bar(Foo):
@@ -3398,33 +3454,41 @@
         T = TypeVar("T")
         P = ParamSpec("P")
         P_2 = ParamSpec("P_2")
 
         class X(Generic[T, P]):
             pass
 
-        G1 = X[int, P_2]
-        self.assertEqual(G1.__args__, (int, P_2))
-        self.assertEqual(G1.__parameters__, (P_2,))
-
-        G2 = X[int, Concatenate[int, P_2]]
-        self.assertEqual(G2.__args__, (int, Concatenate[int, P_2]))
-        self.assertEqual(G2.__parameters__, (P_2,))
+        class Y(Protocol[T, P]):
+            pass
+
+        for klass in X, Y:
+            with self.subTest(klass=klass.__name__):
+                G1 = klass[int, P_2]
+                self.assertEqual(G1.__args__, (int, P_2))
+                self.assertEqual(G1.__parameters__, (P_2,))
+
+                G2 = klass[int, Concatenate[int, P_2]]
+                self.assertEqual(G2.__args__, (int, Concatenate[int, P_2]))
+                self.assertEqual(G2.__parameters__, (P_2,))
 
         # The following are some valid uses cases in PEP 612 that don't work:
         # These do not work in 3.9, _type_check blocks the list and ellipsis.
         # G3 = X[int, [int, bool]]
         # G4 = X[int, ...]
         # G5 = Z[[int, str, bool]]
         # Not working because this is special-cased in 3.10.
         # G6 = Z[int, str, bool]
 
         class Z(Generic[P]):
             pass
 
+        class ProtoZ(Protocol[P]):
+            pass
+
     def test_pickle(self):
         global P, P_co, P_contra, P_default
         P = ParamSpec('P')
         P_co = ParamSpec('P_co', covariant=True)
         P_contra = ParamSpec('P_contra', contravariant=True)
         P_default = ParamSpec('P_default', default=int)
         for proto in range(pickle.HIGHEST_PROTOCOL):
@@ -3723,39 +3787,57 @@
     def test_concatenation(self):
         Xs = TypeVarTuple('Xs')
         self.assertEqual(Tuple[int, Unpack[Xs]].__args__, (int, Unpack[Xs]))
         self.assertEqual(Tuple[Unpack[Xs], int].__args__, (Unpack[Xs], int))
         self.assertEqual(Tuple[int, Unpack[Xs], str].__args__,
                          (int, Unpack[Xs], str))
         class C(Generic[Unpack[Xs]]): pass
-        self.assertEqual(C[int, Unpack[Xs]].__args__, (int, Unpack[Xs]))
-        self.assertEqual(C[Unpack[Xs], int].__args__, (Unpack[Xs], int))
-        self.assertEqual(C[int, Unpack[Xs], str].__args__,
-                         (int, Unpack[Xs], str))
+        class D(Protocol[Unpack[Xs]]): pass
+        for klass in C, D:
+            with self.subTest(klass=klass.__name__):
+                self.assertEqual(klass[int, Unpack[Xs]].__args__, (int, Unpack[Xs]))
+                self.assertEqual(klass[Unpack[Xs], int].__args__, (Unpack[Xs], int))
+                self.assertEqual(klass[int, Unpack[Xs], str].__args__,
+                                 (int, Unpack[Xs], str))
 
     def test_class(self):
         Ts = TypeVarTuple('Ts')
 
         class C(Generic[Unpack[Ts]]): pass
-        self.assertEqual(C[int].__args__, (int,))
-        self.assertEqual(C[int, str].__args__, (int, str))
+        class D(Protocol[Unpack[Ts]]): pass
+
+        for klass in C, D:
+            with self.subTest(klass=klass.__name__):
+                self.assertEqual(klass[int].__args__, (int,))
+                self.assertEqual(klass[int, str].__args__, (int, str))
 
         with self.assertRaises(TypeError):
             class C(Generic[Unpack[Ts], int]): pass
 
+        with self.assertRaises(TypeError):
+            class D(Protocol[Unpack[Ts], int]): pass
+
         T1 = TypeVar('T')
         T2 = TypeVar('T')
         class C(Generic[T1, T2, Unpack[Ts]]): pass
-        self.assertEqual(C[int, str].__args__, (int, str))
-        self.assertEqual(C[int, str, float].__args__, (int, str, float))
-        self.assertEqual(C[int, str, float, bool].__args__, (int, str, float, bool))
-        # TODO This should probably also fail on 3.11, pending changes to CPython.
-        if not TYPING_3_11_0:
-            with self.assertRaises(TypeError):
-                C[int]
+        class D(Protocol[T1, T2, Unpack[Ts]]): pass
+        for klass in C, D:
+            with self.subTest(klass=klass.__name__):
+                self.assertEqual(klass[int, str].__args__, (int, str))
+                self.assertEqual(klass[int, str, float].__args__, (int, str, float))
+                self.assertEqual(
+                    klass[int, str, float, bool].__args__, (int, str, float, bool)
+                )
+                # A bug was fixed in 3.11.1
+                # (https://github.com/python/cpython/commit/74920aa27d0c57443dd7f704d6272cca9c507ab3)
+                # That means this assertion doesn't pass on 3.11.0,
+                # but it passes on all other Python versions
+                if sys.version_info[:3] != (3, 11, 0):
+                    with self.assertRaises(TypeError):
+                        klass[int]
 
 
 class TypeVarTupleTests(BaseTestCase):
 
     def test_basic_plain(self):
         Ts = TypeVarTuple('Ts')
         self.assertEqual(Ts, Ts)
```

### Comparing `typing_extensions-4.6.0/src/typing_extensions.py` & `typing_extensions-4.6.1/src/typing_extensions.py`

 * *Files 2% similar despite different names*

```diff
@@ -608,139 +608,199 @@
                 if val is None and callable(getattr(cls, attr, None)):
                     break
             else:
                 return True
 
             return False
 
-    class Protocol(metaclass=_ProtocolMeta):
-        # There is quite a lot of overlapping code with typing.Generic.
-        # Unfortunately it is hard to avoid this while these live in two different
-        # modules. The duplicated code will be removed when Protocol is moved to typing.
-        """Base class for protocol classes. Protocol classes are defined as::
-
-            class Proto(Protocol):
-                def meth(self) -> int:
-                    ...
-
-        Such classes are primarily used with static type checkers that recognize
-        structural subtyping (static duck-typing), for example::
-
-            class C:
-                def meth(self) -> int:
-                    return 0
-
-            def func(x: Proto) -> int:
-                return x.meth()
-
-            func(C())  # Passes static type check
-
-        See PEP 544 for details. Protocol classes decorated with
-        @typing_extensions.runtime act as simple-minded runtime protocol that checks
-        only the presence of given attributes, ignoring their type signatures.
-
-        Protocol classes can be generic, they are defined as::
-
-            class GenProto(Protocol[T]):
-                def meth(self) -> T:
-                    ...
-        """
-        __slots__ = ()
-        _is_protocol = True
-        _is_runtime_protocol = False
-
-        def __new__(cls, *args, **kwds):
-            if cls is Protocol:
-                raise TypeError("Type Protocol cannot be instantiated; "
-                                "it can only be used as a base class")
-            return super().__new__(cls)
-
-        @typing._tp_cache
-        def __class_getitem__(cls, params):
-            if not isinstance(params, tuple):
-                params = (params,)
-            if not params and cls is not typing.Tuple:
-                raise TypeError(
-                    f"Parameter list to {cls.__qualname__}[...] cannot be empty")
-            msg = "Parameters to generic types must be types."
-            params = tuple(typing._type_check(p, msg) for p in params)
-            if cls is Protocol:
-                # Generic can only be subscripted with unique type variables.
-                if not all(isinstance(p, typing.TypeVar) for p in params):
-                    i = 0
-                    while isinstance(params[i], typing.TypeVar):
-                        i += 1
-                    raise TypeError(
-                        "Parameters to Protocol[...] must all be type variables."
-                        f" Parameter {i + 1} is {params[i]}")
-                if len(set(params)) != len(params):
-                    raise TypeError(
-                        "Parameters to Protocol[...] must all be unique")
-            else:
-                # Subscripting a regular Generic subclass.
-                _check_generic(cls, params, len(cls.__parameters__))
-            return typing._GenericAlias(cls, params)
-
-        def __init_subclass__(cls, *args, **kwargs):
-            if '__orig_bases__' in cls.__dict__:
-                error = typing.Generic in cls.__orig_bases__
+        def __eq__(cls, other):
+            # Hack so that typing.Generic.__class_getitem__
+            # treats typing_extensions.Protocol
+            # as equivalent to typing.Protocol on Python 3.8+
+            if super().__eq__(other) is True:
+                return True
+            return (
+                cls is Protocol and other is getattr(typing, "Protocol", object())
+            )
+
+        # This has to be defined, or the abc-module cache
+        # complains about classes with this metaclass being unhashable,
+        # if we define only __eq__!
+        def __hash__(cls) -> int:
+            return type.__hash__(cls)
+
+    @classmethod
+    def _proto_hook(cls, other):
+        if not cls.__dict__.get('_is_protocol', False):
+            return NotImplemented
+
+        # First, perform various sanity checks.
+        if not getattr(cls, '_is_runtime_protocol', False):
+            if _allow_reckless_class_checks():
+                return NotImplemented
+            raise TypeError("Instance and class checks can only be used with"
+                            " @runtime_checkable protocols")
+
+        if not isinstance(other, type):
+            # Same error message as for issubclass(1, int).
+            raise TypeError('issubclass() arg 1 must be a class')
+
+        # Second, perform the actual structural compatibility check.
+        for attr in cls.__protocol_attrs__:
+            for base in other.__mro__:
+                # Check if the members appears in the class dictionary...
+                if attr in base.__dict__:
+                    if base.__dict__[attr] is None:
+                        return NotImplemented
+                    break
+
+                # ...or in annotations, if it is a sub-protocol.
+                annotations = getattr(base, '__annotations__', {})
+                if (
+                    isinstance(annotations, collections.abc.Mapping)
+                    and attr in annotations
+                    and issubclass(other, (typing.Generic, _ProtocolMeta))
+                    and other._is_protocol
+                ):
+                    break
             else:
-                error = typing.Generic in cls.__bases__
-            if error:
-                raise TypeError("Cannot inherit from plain Generic")
-            _maybe_adjust_parameters(cls)
-
-            # Determine if this is a protocol or a concrete subclass.
-            if not cls.__dict__.get('_is_protocol', None):
-                cls._is_protocol = any(b is Protocol for b in cls.__bases__)
+                return NotImplemented
+        return True
+
+    def _check_proto_bases(cls):
+        for base in cls.__bases__:
+            if not (base in (object, typing.Generic) or
+                    base.__module__ in _PROTO_ALLOWLIST and
+                    base.__name__ in _PROTO_ALLOWLIST[base.__module__] or
+                    isinstance(base, _ProtocolMeta) and base._is_protocol):
+                raise TypeError('Protocols can only inherit from other'
+                                f' protocols, got {repr(base)}')
+
+    if sys.version_info >= (3, 8):
+        class Protocol(typing.Generic, metaclass=_ProtocolMeta):
+            __doc__ = typing.Protocol.__doc__
+            __slots__ = ()
+            _is_protocol = True
+            _is_runtime_protocol = False
+
+            def __init_subclass__(cls, *args, **kwargs):
+                super().__init_subclass__(*args, **kwargs)
+
+                # Determine if this is a protocol or a concrete subclass.
+                if not cls.__dict__.get('_is_protocol', False):
+                    cls._is_protocol = any(b is Protocol for b in cls.__bases__)
+
+                # Set (or override) the protocol subclass hook.
+                if '__subclasshook__' not in cls.__dict__:
+                    cls.__subclasshook__ = _proto_hook
+
+                # We have nothing more to do for non-protocols...
+                if not cls._is_protocol:
+                    return
+
+                # ... otherwise check consistency of bases, and prohibit instantiation.
+                _check_proto_bases(cls)
+                if cls.__init__ is Protocol.__init__:
+                    cls.__init__ = _no_init
+
+    else:
+        class Protocol(metaclass=_ProtocolMeta):
+            # There is quite a lot of overlapping code with typing.Generic.
+            # Unfortunately it is hard to avoid this on Python <3.8,
+            # as the typing module on Python 3.7 doesn't let us subclass typing.Generic!
+            """Base class for protocol classes. Protocol classes are defined as::
+
+                class Proto(Protocol):
+                    def meth(self) -> int:
+                        ...
+
+            Such classes are primarily used with static type checkers that recognize
+            structural subtyping (static duck-typing), for example::
+
+                class C:
+                    def meth(self) -> int:
+                        return 0
+
+                def func(x: Proto) -> int:
+                    return x.meth()
+
+                func(C())  # Passes static type check
+
+            See PEP 544 for details. Protocol classes decorated with
+            @typing_extensions.runtime_checkable act
+            as simple-minded runtime-checkable protocols that check
+            only the presence of given attributes, ignoring their type signatures.
+
+            Protocol classes can be generic, they are defined as::
+
+                class GenProto(Protocol[T]):
+                    def meth(self) -> T:
+                        ...
+            """
+            __slots__ = ()
+            _is_protocol = True
+            _is_runtime_protocol = False
+
+            def __new__(cls, *args, **kwds):
+                if cls is Protocol:
+                    raise TypeError("Type Protocol cannot be instantiated; "
+                                    "it can only be used as a base class")
+                return super().__new__(cls)
+
+            @typing._tp_cache
+            def __class_getitem__(cls, params):
+                if not isinstance(params, tuple):
+                    params = (params,)
+                if not params and cls is not typing.Tuple:
+                    raise TypeError(
+                        f"Parameter list to {cls.__qualname__}[...] cannot be empty")
+                msg = "Parameters to generic types must be types."
+                params = tuple(typing._type_check(p, msg) for p in params)
+                if cls is Protocol:
+                    # Generic can only be subscripted with unique type variables.
+                    if not all(isinstance(p, typing.TypeVar) for p in params):
+                        i = 0
+                        while isinstance(params[i], typing.TypeVar):
+                            i += 1
+                        raise TypeError(
+                            "Parameters to Protocol[...] must all be type variables."
+                            f" Parameter {i + 1} is {params[i]}")
+                    if len(set(params)) != len(params):
+                        raise TypeError(
+                            "Parameters to Protocol[...] must all be unique")
+                else:
+                    # Subscripting a regular Generic subclass.
+                    _check_generic(cls, params, len(cls.__parameters__))
+                return typing._GenericAlias(cls, params)
+
+            def __init_subclass__(cls, *args, **kwargs):
+                if '__orig_bases__' in cls.__dict__:
+                    error = typing.Generic in cls.__orig_bases__
+                else:
+                    error = typing.Generic in cls.__bases__
+                if error:
+                    raise TypeError("Cannot inherit from plain Generic")
+                _maybe_adjust_parameters(cls)
 
-            # Set (or override) the protocol subclass hook.
-            def _proto_hook(other):
+                # Determine if this is a protocol or a concrete subclass.
                 if not cls.__dict__.get('_is_protocol', None):
-                    return NotImplemented
-                if not getattr(cls, '_is_runtime_protocol', False):
-                    if _allow_reckless_class_checks():
-                        return NotImplemented
-                    raise TypeError("Instance and class checks can only be used with"
-                                    " @runtime protocols")
-                if not isinstance(other, type):
-                    # Same error as for issubclass(1, int)
-                    raise TypeError('issubclass() arg 1 must be a class')
-                for attr in cls.__protocol_attrs__:
-                    for base in other.__mro__:
-                        if attr in base.__dict__:
-                            if base.__dict__[attr] is None:
-                                return NotImplemented
-                            break
-                        annotations = getattr(base, '__annotations__', {})
-                        if (isinstance(annotations, typing.Mapping) and
-                                attr in annotations and
-                                isinstance(other, _ProtocolMeta) and
-                                other._is_protocol):
-                            break
-                    else:
-                        return NotImplemented
-                return True
-            if '__subclasshook__' not in cls.__dict__:
-                cls.__subclasshook__ = _proto_hook
+                    cls._is_protocol = any(b is Protocol for b in cls.__bases__)
 
-            # We have nothing more to do for non-protocols.
-            if not cls._is_protocol:
-                return
-
-            # Check consistency of bases.
-            for base in cls.__bases__:
-                if not (base in (object, typing.Generic) or
-                        base.__module__ in _PROTO_ALLOWLIST and
-                        base.__name__ in _PROTO_ALLOWLIST[base.__module__] or
-                        isinstance(base, _ProtocolMeta) and base._is_protocol):
-                    raise TypeError('Protocols can only inherit from other'
-                                    f' protocols, got {repr(base)}')
-            if cls.__init__ is Protocol.__init__:
-                cls.__init__ = _no_init
+                # Set (or override) the protocol subclass hook.
+                if '__subclasshook__' not in cls.__dict__:
+                    cls.__subclasshook__ = _proto_hook
+
+                # We have nothing more to do for non-protocols.
+                if not cls._is_protocol:
+                    return
+
+                # Check consistency of bases.
+                _check_proto_bases(cls)
+                if cls.__init__ is Protocol.__init__:
+                    cls.__init__ = _no_init
 
     def runtime_checkable(cls):
         """Mark a protocol class as a runtime protocol, so that it
         can be used with isinstance() and issubclass(). Raise TypeError
         if applied to a non-protocol class.
 
         This allows a simple-minded structural check very similar to the
```

### Comparing `typing_extensions-4.6.0/PKG-INFO` & `typing_extensions-4.6.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typing_extensions
-Version: 4.6.0
+Version: 4.6.1
 Summary: Backported and Experimental Type Hints for Python 3.7+
 Keywords: annotations,backport,checker,checking,function,hinting,hints,type,typechecking,typehinting,typehints,typing
 Author-email: "Guido van Rossum, Jukka Lehtosalo, Łukasz Langa, Michael Lee" <levkivskyi@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

