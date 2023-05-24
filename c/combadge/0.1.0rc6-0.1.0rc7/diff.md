# Comparing `tmp/combadge-0.1.0rc6.tar.gz` & `tmp/combadge-0.1.0rc7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "combadge-0.1.0rc6.tar", max compression
+gzip compressed data, was "combadge-0.1.0rc7.tar", max compression
```

## Comparing `combadge-0.1.0rc6.tar` & `combadge-0.1.0rc7.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0    11350 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/LICENSE
--rw-r--r--   0        0        0     2682 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/README.md
--rw-r--r--   0        0        0        0 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/__init__.py
--rw-r--r--   0        0        0        0 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/core/__init__.py
--rw-r--r--   0        0        0     1259 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/core/backend.py
--rw-r--r--   0        0        0     3377 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/core/binder.py
--rw-r--r--   0        0        0     3016 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/core/interfaces.py
--rw-r--r--   0        0        0        0 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/core/markers/__init__.py
--rw-r--r--   0        0        0     2568 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/core/markers/method.py
--rw-r--r--   0        0        0      902 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/core/markers/parameter.py
--rw-r--r--   0        0        0     1997 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/core/request.py
--rw-r--r--   0        0        0     6303 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/core/response.py
--rw-r--r--   0        0        0     1830 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/core/service.py
--rw-r--r--   0        0        0     2372 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/core/signature.py
--rw-r--r--   0        0        0      343 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/core/typevars.py
--rw-r--r--   0        0        0      203 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/core/warnings.py
--rw-r--r--   0        0        0        0 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/py.typed
--rw-r--r--   0        0        0       50 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/support/__init__.py
--rw-r--r--   0        0        0       40 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/support/http/__init__.py
--rw-r--r--   0        0        0     1470 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/support/http/abc.py
--rw-r--r--   0        0        0      807 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/support/http/aliases.py
--rw-r--r--   0        0        0      264 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/support/http/headers.py
--rw-r--r--   0        0        0     7338 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/support/http/markers.py
--rw-r--r--   0        0        0      398 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/support/http/request.py
--rw-r--r--   0        0        0      124 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/support/httpx/__init__.py
--rw-r--r--   0        0        0        0 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/support/httpx/backends/__init__.py
--rw-r--r--   0        0        0     3374 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/support/httpx/backends/async_.py
--rw-r--r--   0        0        0     1542 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/support/httpx/backends/base.py
--rw-r--r--   0        0        0     3232 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/support/httpx/backends/sync.py
--rw-r--r--   0        0        0        0 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/support/shared/__init__.py
--rw-r--r--   0        0        0      348 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/support/shared/async_.py
--rw-r--r--   0        0        0      308 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/support/shared/contextlib.py
--rw-r--r--   0        0        0      338 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/support/shared/sync.py
--rw-r--r--   0        0        0       39 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/support/soap/__init__.py
--rw-r--r--   0        0        0      256 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/support/soap/abc.py
--rw-r--r--   0        0        0     2198 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/support/soap/markers.py
--rw-r--r--   0        0        0      212 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/support/soap/request.py
--rw-r--r--   0        0        0      870 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/support/soap/response.py
--rw-r--r--   0        0        0      131 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/support/zeep/__init__.py
--rw-r--r--   0        0        0        0 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/support/zeep/backends/__init__.py
--rw-r--r--   0        0        0     3475 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/support/zeep/backends/async_.py
--rw-r--r--   0        0        0     3059 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/support/zeep/backends/base.py
--rw-r--r--   0        0        0     3334 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/support/zeep/backends/sync.py
--rw-r--r--   0        0        0     3397 2023-04-26 16:23:59.259021 combadge-0.1.0rc6/pyproject.toml
--rw-r--r--   0        0        0     4369 1970-01-01 00:00:00.000000 combadge-0.1.0rc6/PKG-INFO
+-rw-r--r--   0        0        0    11350 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/LICENSE
+-rw-r--r--   0        0        0     2682 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/README.md
+-rw-r--r--   0        0        0        0 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/core/__init__.py
+-rw-r--r--   0        0        0     1259 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/core/backend.py
+-rw-r--r--   0        0        0     3358 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/core/binder.py
+-rw-r--r--   0        0        0     2982 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/core/interfaces.py
+-rw-r--r--   0        0        0        0 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/core/markers/__init__.py
+-rw-r--r--   0        0        0     2562 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/core/markers/method.py
+-rw-r--r--   0        0        0      890 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/core/markers/parameter.py
+-rw-r--r--   0        0        0     1997 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/core/request.py
+-rw-r--r--   0        0        0     6312 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/core/response.py
+-rw-r--r--   0        0        0     1830 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/core/service.py
+-rw-r--r--   0        0        0     2354 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/core/signature.py
+-rw-r--r--   0        0        0      343 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/core/typevars.py
+-rw-r--r--   0        0        0      203 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/core/warnings.py
+-rw-r--r--   0        0        0        0 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/py.typed
+-rw-r--r--   0        0        0       50 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/support/__init__.py
+-rw-r--r--   0        0        0       40 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/support/http/__init__.py
+-rw-r--r--   0        0        0     1470 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/support/http/abc.py
+-rw-r--r--   0        0        0      807 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/support/http/aliases.py
+-rw-r--r--   0        0        0      264 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/support/http/headers.py
+-rw-r--r--   0        0        0     7338 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/support/http/markers.py
+-rw-r--r--   0        0        0      398 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/support/http/request.py
+-rw-r--r--   0        0        0      124 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/support/httpx/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/support/httpx/backends/__init__.py
+-rw-r--r--   0        0        0     3349 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/support/httpx/backends/async_.py
+-rw-r--r--   0        0        0     1536 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/support/httpx/backends/base.py
+-rw-r--r--   0        0        0     3207 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/support/httpx/backends/sync.py
+-rw-r--r--   0        0        0        0 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/support/shared/__init__.py
+-rw-r--r--   0        0        0      348 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/support/shared/async_.py
+-rw-r--r--   0        0        0      308 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/support/shared/contextlib.py
+-rw-r--r--   0        0        0      338 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/support/shared/sync.py
+-rw-r--r--   0        0        0       39 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/support/soap/__init__.py
+-rw-r--r--   0        0        0      256 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/support/soap/abc.py
+-rw-r--r--   0        0        0     2198 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/support/soap/markers.py
+-rw-r--r--   0        0        0      212 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/support/soap/request.py
+-rw-r--r--   0        0        0      870 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/support/soap/response.py
+-rw-r--r--   0        0        0      131 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/support/zeep/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/support/zeep/backends/__init__.py
+-rw-r--r--   0        0        0     3450 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/support/zeep/backends/async_.py
+-rw-r--r--   0        0        0     3059 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/support/zeep/backends/base.py
+-rw-r--r--   0        0        0     3296 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/support/zeep/backends/sync.py
+-rw-r--r--   0        0        0     3394 2023-05-24 13:25:27.060479 combadge-0.1.0rc7/pyproject.toml
+-rw-r--r--   0        0        0     4169 1970-01-01 00:00:00.000000 combadge-0.1.0rc7/PKG-INFO
```

### Comparing `combadge-0.1.0rc6/LICENSE` & `combadge-0.1.0rc7/LICENSE`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc6/README.md` & `combadge-0.1.0rc7/README.md`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc6/combadge/core/backend.py` & `combadge-0.1.0rc7/combadge/core/backend.py`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc6/combadge/core/binder.py` & `combadge-0.1.0rc7/combadge/core/binder.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,45 +2,45 @@
 
 from __future__ import annotations
 
 from dataclasses import dataclass
 from functools import update_wrapper
 from inspect import getmembers as get_members
 from inspect import signature as get_signature
-from typing import TYPE_CHECKING, Any, Callable, Generic, Iterable, Optional, Type
+from typing import TYPE_CHECKING, Any, Callable, Generic, Iterable
 
 from combadge.core.markers.method import MethodMarker
 from combadge.core.service import BaseBoundService
 from combadge.core.typevars import BackendT, FunctionT, RequestT, ServiceProtocolT
 
 if TYPE_CHECKING:
     from combadge.core.interfaces import CallServiceMethod, MethodBinder, ProvidesBinder
 
-    def lru_cache(maxsize: Optional[int]) -> Callable[[FunctionT], FunctionT]:
+    def lru_cache(maxsize: int | None) -> Callable[[FunctionT], FunctionT]:
         ...
 
 else:
     from functools import lru_cache
 
 
-def bind(from_protocol: Type[ServiceProtocolT], to_backend: ProvidesBinder) -> ServiceProtocolT:
+def bind(from_protocol: type[ServiceProtocolT], to_backend: ProvidesBinder) -> ServiceProtocolT:
     """
     Create a service instance which implements the specified protocol by calling the specified backend.
 
     Args:
         from_protocol: service protocol description, used to extract request and response types etc.
         to_backend: backend which should perform the service requests
     """
 
     return bind_class(from_protocol, to_backend.binder)(to_backend)
 
 
 @lru_cache(maxsize=100)
 def bind_class(
-    from_protocol: Type[ServiceProtocolT],
+    from_protocol: type[ServiceProtocolT],
     method_binder: MethodBinder[BackendT],
 ) -> Callable[[BackendT], ServiceProtocolT]:
     from combadge.core.signature import Signature
 
     class BoundService(BaseBoundService, from_protocol):  # type: ignore[misc, valid-type]
         """Bound service class that implements the protocol."""
```

### Comparing `combadge-0.1.0rc6/combadge/core/interfaces.py` & `combadge-0.1.0rc7/combadge/core/interfaces.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from abc import abstractmethod
 from types import TracebackType
-from typing import Any, Optional, Protocol, Type
+from typing import Any, Protocol
 
 from pydantic import BaseModel
 from typing_extensions import Self
 
 from combadge.core.binder import BaseBoundService, bind
 from combadge.core.signature import Signature
 from combadge.core.typevars import BackendT
@@ -34,25 +34,25 @@
         return self
 
     async def __aenter__(self) -> Self:
         return self
 
     def __exit__(
         self,
-        exc_type: Optional[Type[BaseException]],
-        exc_value: Optional[BaseException],
-        traceback: Optional[TracebackType],
+        exc_type: type[BaseException] | None,
+        exc_value: BaseException | None,
+        traceback: TracebackType | None,
     ) -> Any:
         return None
 
     async def __aexit__(
         self,
-        exc_type: Optional[Type[BaseException]],
-        exc_value: Optional[BaseException],
-        traceback: Optional[TracebackType],
+        exc_type: type[BaseException] | None,
+        exc_value: BaseException | None,
+        traceback: TracebackType | None,
     ) -> Any:
         return None
 
 
 class MethodBinder(Protocol[BackendT]):  # noqa: D101
     @staticmethod
     @abstractmethod
```

### Comparing `combadge-0.1.0rc6/combadge/core/markers/method.py` & `combadge-0.1.0rc7/combadge/core/markers/method.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from abc import ABC
 from inspect import BoundArguments
-from typing import Any, Callable, Generic, List
+from typing import Any, Callable, Generic
 
 from combadge.core.typevars import FunctionT, RequestT
 
 
 class MethodMarker(ABC, Generic[RequestT, FunctionT]):
     """Method-specific marker that modifies an entire request based on all the call arguments."""
 
@@ -30,15 +30,15 @@
 
         Args:
             request: request that is being constructed, please refer to the ABCs for relevant keys
             arguments: bound service call arguments
         """
 
     @staticmethod
-    def ensure_markers(in_: Any) -> List[MethodMarker]:
+    def ensure_markers(in_: Any) -> list[MethodMarker]:
         """Ensure that the argument contains the mark list attribute, and return the list."""
         try:
             marks = in_.__combadge_marks__
         except AttributeError:
             marks = in_.__combadge_marks__ = []
         return marks
```

### Comparing `combadge-0.1.0rc6/combadge/core/markers/parameter.py` & `combadge-0.1.0rc7/combadge/core/markers/parameter.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
-from typing import Any, Generic, List, Type
+from typing import Any, Generic
 
 from typing_extensions import Annotated, get_origin
 from typing_extensions import get_args as get_type_args
 
 from combadge.core.typevars import RequestT
 
 
 class ParameterMarker(Generic[RequestT], ABC):
     """Parameter-specific marker that modifies a request with a call-time argument."""
 
     __slots__ = ()
 
     @staticmethod
-    def extract(type_: Type[Any]) -> List[ParameterMarker]:
+    def extract(type_: type[Any]) -> list[ParameterMarker]:
         """Extract all parameter markers from the type annotation."""
         if get_origin(type_) is Annotated:
             return [arg for arg in get_type_args(type_) if isinstance(arg, ParameterMarker)]
         return []
 
     @abstractmethod
     def prepare_request(self, request: RequestT, value: Any) -> None:
```

### Comparing `combadge-0.1.0rc6/combadge/core/request.py` & `combadge-0.1.0rc7/combadge/core/request.py`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc6/combadge/core/response.py` & `combadge-0.1.0rc7/combadge/core/response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Generic response models."""
 
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
-from typing import Any, Generic, Iterable, NoReturn, Optional, Type, Union
+from typing import Any, Generic, Iterable, NoReturn
 
 from pydantic import BaseModel
 from typing_extensions import Self, TypeAlias
 
 from combadge.core.typevars import ResponseT
 
 
@@ -19,15 +19,15 @@
 
     Notes:
         - `#!python BaseResponse` is the lower-level API,
           users should consider inheriting from `#!python SuccessfulResponse` and `#!python ErrorResponse`.
     """
 
     @abstractmethod
-    def raise_for_result(self, exception: Optional[BaseException] = None) -> Union[None, NoReturn]:
+    def raise_for_result(self, exception: BaseException | None = None) -> None | NoReturn:
         """
         Raise an exception if the service call has failed.
 
         Raises:
             ErrorResponse.Error: an error derived from `ErrorResponse`
 
         Returns:
@@ -41,15 +41,15 @@
 
             The advice is to use [`unwrap()`][combadge.core.response.BaseResponse.unwrap]
             for the time being.
         """
         raise NotImplementedError
 
     @abstractmethod
-    def unwrap(self) -> Union[Self, NoReturn]:
+    def unwrap(self) -> Self | NoReturn:
         """
         Return itself if the call was successful, raises an exception otherwise.
 
         This method allows «unpacking» a response with proper type hinting.
         The trick here is that all error responses' `unwrap()` are annotated with `NoReturn`,
         which suggests a type linter, that `unwrap()` may never return an error.
 
@@ -78,15 +78,15 @@
 class SuccessfulResponse(BaseResponse):
     """
     Parent model for successful responses.
 
     Users should not use it directly, but inherit their response models from it.
     """
 
-    def raise_for_result(self, exception: Optional[BaseException] = None) -> None:
+    def raise_for_result(self, exception: BaseException | None = None) -> None:
         """
         Do nothing.
 
         This call is a no-op since the response is successful.
         """
 
     def unwrap(self) -> Self:
@@ -133,15 +133,15 @@
             super().__init__(response)
 
         @property
         def response(self) -> ResponseT:
             """Get the response that caused the exception."""
             return self.args[0]
 
-    def __init_subclass__(cls, exception_bases: Iterable[Type[BaseException]] = (), **kwargs: Any) -> None:
+    def __init_subclass__(cls, exception_bases: Iterable[type[BaseException]] = (), **kwargs: Any) -> None:
         """
         Build the derived exception class.
 
         Args:
             exception_bases: additional bases for the derived exception class
             kwargs: forwarded to the superclass
         """
@@ -159,20 +159,21 @@
             """
             Derived exception class.
 
             Notes:
                 - This docstring is overridden by the corresponding model docstring.
             """
 
+        DerivedException.__module__ = cls.__module__
         DerivedException.__name__ = f"{cls.__name__}.Error"
         DerivedException.__qualname__ = f"{cls.__qualname__}.Error"
         DerivedException.__doc__ = cls.__doc__ or DerivedException.__doc__
         cls.Error = DerivedException  # type: ignore
 
-    def raise_for_result(self, exception: Optional[BaseException] = None) -> NoReturn:
+    def raise_for_result(self, exception: BaseException | None = None) -> NoReturn:
         """
         Raise the derived exception.
 
         Args:
             exception: if set, raise the specified exception instead of the derived one.
         """
         if not exception:
```

### Comparing `combadge-0.1.0rc6/combadge/core/service.py` & `combadge-0.1.0rc7/combadge/core/service.py`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc6/combadge/core/signature.py` & `combadge-0.1.0rc7/combadge/core/signature.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from functools import cached_property
 from inspect import BoundArguments
 from inspect import signature as get_signature
-from typing import Any, Callable, Dict, List, Type
+from typing import Any, Callable
 
 from pydantic import BaseModel, create_model
 
 from combadge.core.binder import ParameterDescriptor
 from combadge.core.markers.method import MethodMarker
 from combadge.core.markers.parameter import ParameterMarker
 from combadge.core.response import SuccessfulResponse
@@ -24,40 +24,40 @@
     """
     Contains extracted information about a service method.
 
     Why? Because passing all these parameters into `bind_method` would be messy.
     """
 
     bind_arguments: Callable[..., BoundArguments]
-    method_markers: List[MethodMarker]
-    annotations: Dict[str, Any]
+    method_markers: list[MethodMarker]
+    annotations: dict[str, Any]
 
     __slots__ = ("bind_arguments", "method_markers", "annotations", "__dict__")
 
     @classmethod
     def from_method(cls, method: Any) -> Signature:
         """Create a signature from the specified method."""
         return Signature(
             bind_arguments=get_signature(method).bind,
             method_markers=MethodMarker.ensure_markers(method),
             annotations=get_annotations(method, eval_str=True),
         )
 
     @cached_property
-    def parameter_descriptors(self) -> List[ParameterDescriptor]:
+    def parameter_descriptors(self) -> list[ParameterDescriptor]:
         """Get the parameter descriptors: separate list item for each parameter ⨯ marker combination."""
         return [
             ParameterDescriptor(name=name, prepare_request=marker.prepare_request)
             for name, annotation in self.annotations.items()
             for marker in ParameterMarker.extract(annotation)
         ]
 
     @cached_property
-    def return_type(self) -> Type[BaseModel]:
+    def return_type(self) -> type[BaseModel]:
         """Get the method's return type."""
         return self.annotations.get("return", SuccessfulResponse)
 
     @cached_property
-    def parameters_model(self) -> Type[BaseModel]:
+    def parameters_model(self) -> type[BaseModel]:
         """Get dynamically constructed model for this method."""
-        field_definitions: Dict[str, Any] = {name: (type_, ...) for name, type_ in self.annotations.items()}
+        field_definitions: dict[str, Any] = {name: (type_, ...) for name, type_ in self.annotations.items()}
         return create_model("DynamicModel", **field_definitions)  # TODO: better model name.
```

### Comparing `combadge-0.1.0rc6/combadge/support/http/abc.py` & `combadge-0.1.0rc7/combadge/support/http/abc.py`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc6/combadge/support/http/aliases.py` & `combadge-0.1.0rc7/combadge/support/http/aliases.py`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc6/combadge/support/http/markers.py` & `combadge-0.1.0rc7/combadge/support/http/markers.py`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc6/combadge/support/httpx/backends/async_.py` & `combadge-0.1.0rc7/combadge/support/httpx/backends/async_.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from contextlib import AbstractAsyncContextManager
 from types import TracebackType
-from typing import Any, Callable, Optional, Type
+from typing import Any, Callable
 
 from httpx import AsyncClient, Response
 from pydantic import BaseModel
 from typing_extensions import Self
 
 from combadge.core.backend import ServiceContainer
 from combadge.core.binder import BaseBoundService
@@ -40,15 +40,15 @@
             request_with: an optional context manager getter to wrap each request into
             raise_for_status: automatically call `raise_for_status()`
         """
         BaseHttpxBackend.__init__(self, client, raise_for_status=raise_for_status)
         SupportsRequestWith.__init__(self, request_with)
         ServiceContainer.__init__(self)
 
-    async def __call__(self, request: Request, response_type: Type[ResponseT]) -> ResponseT:
+    async def __call__(self, request: Request, response_type: type[ResponseT]) -> ResponseT:
         """
         Call the backend and parse a response.
 
         !!! info ""
             One does not normally need to call this directly, unless writing a custom binder.
         """
         response: Response = await self._client.request(
@@ -76,12 +76,12 @@
 
     async def __aenter__(self) -> Self:
         self._client = await self._client.__aenter__()
         return self
 
     async def __aexit__(
         self,
-        exc_type: Optional[Type[BaseException]],
-        exc_value: Optional[BaseException],
-        traceback: Optional[TracebackType],
+        exc_type: type[BaseException] | None,
+        exc_value: BaseException | None,
+        traceback: TracebackType | None,
     ) -> Any:
         return await self._client.__aexit__(exc_type, exc_value, traceback)
```

### Comparing `combadge-0.1.0rc6/combadge/support/httpx/backends/base.py` & `combadge-0.1.0rc7/combadge/support/httpx/backends/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import Generic, Type, TypeVar
+from typing import Generic, TypeVar
 
 from httpx import AsyncClient, Client, Response
 from pydantic import parse_obj_as
 
 from combadge.core.interfaces import ProvidesBinder
 from combadge.core.typevars import ResponseT
 from combadge.support.http.aliases import CONTENT_ALIAS, REASON_ALIAS, STATUS_CODE_ALIAS
@@ -26,15 +26,15 @@
     _client: _ClientT
 
     def __init__(self, client: _ClientT, *, raise_for_status: bool = True) -> None:  # noqa: D107
         self._client = client
         self._raise_for_status = raise_for_status
 
     @classmethod
-    def _parse_response(cls, from_response: Response, to_type: Type[ResponseT]) -> ResponseT:
+    def _parse_response(cls, from_response: Response, to_type: type[ResponseT]) -> ResponseT:
         try:
             json_fields = from_response.json()
         except ValueError:
             json_fields = {}
         return parse_obj_as(
             to_type,
             {
```

### Comparing `combadge-0.1.0rc6/combadge/support/httpx/backends/sync.py` & `combadge-0.1.0rc7/combadge/support/httpx/backends/sync.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from contextlib import AbstractContextManager, nullcontext
 from types import TracebackType
-from typing import Any, Callable, Optional, Type
+from typing import Any, Callable
 
 from httpx import Client, Response
 from pydantic import BaseModel
 from typing_extensions import Self
 
 from combadge.core.backend import ServiceContainer
 from combadge.core.binder import BaseBoundService
@@ -39,15 +39,15 @@
             request_with: an optional context manager getter to wrap each request into
             raise_for_status: automatically call `raise_for_status()`
         """
         BaseHttpxBackend.__init__(self, client, raise_for_status=raise_for_status)
         SupportsRequestWith.__init__(self, request_with)
         ServiceContainer.__init__(self)
 
-    def __call__(self, request: Request, response_type: Type[ResponseT]) -> ResponseT:
+    def __call__(self, request: Request, response_type: type[ResponseT]) -> ResponseT:
         """
         Call the backend and parse a response.
 
         !!! info ""
             One does not normally need to call this directly, unless writing a custom binder.
         """
         response: Response = self._client.request(
@@ -75,12 +75,12 @@
 
     def __enter__(self) -> Self:
         self._client = self._client.__enter__()
         return self
 
     def __exit__(
         self,
-        exc_type: Optional[Type[BaseException]],
-        exc_value: Optional[BaseException],
-        traceback: Optional[TracebackType],
+        exc_type: type[BaseException] | None,
+        exc_value: BaseException | None,
+        traceback: TracebackType | None,
     ) -> Any:
         return self._client.__exit__(exc_type, exc_value, traceback)
```

### Comparing `combadge-0.1.0rc6/combadge/support/soap/markers.py` & `combadge-0.1.0rc7/combadge/support/soap/markers.py`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc6/combadge/support/soap/response.py` & `combadge-0.1.0rc7/combadge/support/soap/response.py`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc6/combadge/support/zeep/backends/async_.py` & `combadge-0.1.0rc7/combadge/support/zeep/backends/async_.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from contextlib import AbstractAsyncContextManager
 from types import TracebackType
-from typing import Any, Callable, Optional, Type
+from typing import Any, Callable
 
 from pydantic import BaseModel
 from typing_extensions import Self
 from zeep.exceptions import Fault
 from zeep.proxy import AsyncOperationProxy, AsyncServiceProxy
 
 from combadge.core.backend import ServiceContainer
@@ -47,16 +47,16 @@
         BaseZeepBackend.__init__(self, service)
         SupportsRequestWith.__init__(self, request_with)
         ServiceContainer.__init__(self)
 
     async def __call__(
         self,
         request: Request,
-        response_type: Type[ResponseT],
-        fault_type: Type[SoapFaultT],
+        response_type: type[ResponseT],
+        fault_type: type[SoapFaultT],
     ) -> BaseModel:
         """
         Call the specified service method.
 
         Args:
             request: prepared request
             response_type: non-fault response model type
@@ -84,12 +84,12 @@
 
     async def __aenter__(self) -> Self:
         self._service = await self._service.__aenter__()
         return self
 
     async def __aexit__(
         self,
-        exc_type: Optional[Type[BaseException]],
-        exc_value: Optional[BaseException],
-        traceback: Optional[TracebackType],
+        exc_type: type[BaseException] | None,
+        exc_value: BaseException | None,
+        traceback: TracebackType | None,
     ) -> Any:
         return await self._service.__aexit__(exc_type, exc_value, traceback)
```

### Comparing `combadge-0.1.0rc6/combadge/support/zeep/backends/base.py` & `combadge-0.1.0rc7/combadge/support/zeep/backends/base.py`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc6/combadge/support/zeep/backends/sync.py` & `combadge-0.1.0rc7/combadge/support/zeep/backends/sync.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from contextlib import AbstractContextManager, nullcontext
 from types import TracebackType
-from typing import Any, Callable, Optional, Type, Union
+from typing import Any, Callable
 
 from pydantic import BaseModel
 from typing_extensions import Self
 from zeep.exceptions import Fault
 from zeep.proxy import OperationProxy, ServiceProxy
 
 from combadge.core.backend import ServiceContainer
@@ -42,17 +42,17 @@
         BaseZeepBackend.__init__(self, service)
         SupportsRequestWith.__init__(self, request_with)
         ServiceContainer.__init__(self)
 
     def __call__(
         self,
         request: Request,
-        response_type: Type[ResponseT],
-        fault_type: Type[SoapFaultT],
-    ) -> Union[ResponseT, SoapFaultT]:
+        response_type: type[ResponseT],
+        fault_type: type[SoapFaultT],
+    ) -> ResponseT | SoapFaultT:
         """
         Call the specified service method.
 
         Args:
             request: prepared request
             response_type: non-fault response model type
             fault_type: SOAP fault model type
@@ -79,12 +79,12 @@
 
     def __enter__(self) -> Self:
         self._service = self._service.__enter__()
         return self
 
     def __exit__(
         self,
-        exc_type: Optional[Type[BaseException]],
-        exc_value: Optional[BaseException],
-        traceback: Optional[TracebackType],
+        exc_type: type[BaseException] | None,
+        exc_value: BaseException | None,
+        traceback: TracebackType | None,
     ) -> Any:
         return self._service.__exit__(exc_type, exc_value, traceback)
```

### Comparing `combadge-0.1.0rc6/pyproject.toml` & `combadge-0.1.0rc7/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,21 @@
+[project]
+requires-python = ">=3.8"
+
 [tool.poetry]
 authors = [
     "Pavel Perestoronin <pavel.perestoronin@kpn.com>",
 ]
 description = "Generic API client based on Pydantic"
 keywords = ["api", "api-client", "pydantic"]
 license = "Apache-2.0"
 name = "combadge"
 readme = "README.md"
 repository = "https://github.com/kpn/combadge"
-version = "0.1.0rc6"
+version = "0.1.0rc7"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
@@ -78,17 +81,14 @@
     "D406",
     "D407",
     "PT001",
     "PT011",
     "PT013",
     "RET505",
     "TRY003",
-    "UP006",  # 3.9
-    "UP007",  # 3.10
-    "UP033",  # 3.9
 ]
 unfixable = ["B"]
 
 [tool.ruff.per-file-ignores]
 "tests/*" = ["D101", "D102", "D106"]
 
 [tool.ruff.flake8-quotes]
@@ -135,14 +135,15 @@
 mypy = "^1.0.0"
 pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
 types-requests = "^2.28.11.8"
 ruff = "^0.0.263"
 pytest-recording = "^0.12.1"
 pytest-asyncio = "^0.20.3"
+urllib3 = "^1.26.16"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 mkdocs-material = "^9.0.12"
 pillow = "^9.4.0"
```

### Comparing `combadge-0.1.0rc6/PKG-INFO` & `combadge-0.1.0rc7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: combadge
-Version: 0.1.0rc6
+Version: 0.1.0rc7
 Summary: Generic API client based on Pydantic
 Home-page: https://github.com/kpn/combadge
 License: Apache-2.0
 Keywords: api,api-client,pydantic
 Author: Pavel Perestoronin
 Author-email: pavel.perestoronin@kpn.com
 Requires-Python: >=3.8.1,<4.0.0
@@ -12,20 +12,16 @@
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System
 Classifier: Topic :: System :: Networking
 Classifier: Typing :: Typed
```

