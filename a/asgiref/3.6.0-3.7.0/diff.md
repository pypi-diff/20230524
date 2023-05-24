# Comparing `tmp/asgiref-3.6.0.tar.gz` & `tmp/asgiref-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asgiref-3.6.0.tar", last modified: Tue Dec 20 09:06:25 2022, max compression
+gzip compressed data, was "asgiref-3.7.0.tar", last modified: Tue May 23 16:55:41 2023, max compression
```

## Comparing `asgiref-3.6.0.tar` & `asgiref-3.7.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2022-12-20 09:06:25.459062 asgiref-3.6.0/
--rw-r--r--   0 carlton    (501) staff       (20)     1552 2022-04-19 07:47:42.000000 asgiref-3.6.0/LICENSE
--rw-r--r--   0 carlton    (501) staff       (20)       70 2022-04-19 07:47:42.000000 asgiref-3.6.0/MANIFEST.in
--rw-r--r--   0 carlton    (501) staff       (20)     9006 2022-12-20 09:06:25.459167 asgiref-3.6.0/PKG-INFO
--rw-r--r--   0 carlton    (501) staff       (20)     7756 2022-07-06 14:22:11.000000 asgiref-3.6.0/README.rst
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2022-12-20 09:06:25.456699 asgiref-3.6.0/asgiref/
--rw-r--r--   0 carlton    (501) staff       (20)       22 2022-12-20 08:57:26.000000 asgiref-3.6.0/asgiref/__init__.py
--rw-r--r--   0 carlton    (501) staff       (20)     1606 2022-12-15 09:04:51.000000 asgiref-3.6.0/asgiref/compatibility.py
--rw-r--r--   0 carlton    (501) staff       (20)     2801 2022-04-19 07:47:42.000000 asgiref-3.6.0/asgiref/current_thread_executor.py
--rw-r--r--   0 carlton    (501) staff       (20)     4854 2022-04-19 07:47:42.000000 asgiref-3.6.0/asgiref/local.py
--rw-r--r--   0 carlton    (501) staff       (20)        0 2022-04-19 07:47:42.000000 asgiref-3.6.0/asgiref/py.typed
--rw-r--r--   0 carlton    (501) staff       (20)     6005 2022-08-08 06:48:57.000000 asgiref-3.6.0/asgiref/server.py
--rw-r--r--   0 carlton    (501) staff       (20)    20664 2022-12-15 09:04:51.000000 asgiref-3.6.0/asgiref/sync.py
--rw-r--r--   0 carlton    (501) staff       (20)     3119 2022-04-19 07:47:42.000000 asgiref-3.6.0/asgiref/testing.py
--rw-r--r--   0 carlton    (501) staff       (20)     3627 2022-12-15 18:33:28.000000 asgiref-3.6.0/asgiref/timeout.py
--rw-r--r--   0 carlton    (501) staff       (20)     5843 2022-12-15 09:04:51.000000 asgiref-3.6.0/asgiref/typing.py
--rw-r--r--   0 carlton    (501) staff       (20)     6575 2022-04-19 07:47:42.000000 asgiref-3.6.0/asgiref/wsgi.py
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2022-12-20 09:06:25.457631 asgiref-3.6.0/asgiref.egg-info/
--rw-r--r--   0 carlton    (501) staff       (20)     9006 2022-12-20 09:06:25.000000 asgiref-3.6.0/asgiref.egg-info/PKG-INFO
--rw-r--r--   0 carlton    (501) staff       (20)      613 2022-12-20 09:06:25.000000 asgiref-3.6.0/asgiref.egg-info/SOURCES.txt
--rw-r--r--   0 carlton    (501) staff       (20)        1 2022-12-20 09:06:25.000000 asgiref-3.6.0/asgiref.egg-info/dependency_links.txt
--rw-r--r--   0 carlton    (501) staff       (20)        1 2022-07-06 08:14:22.000000 asgiref-3.6.0/asgiref.egg-info/not-zip-safe
--rw-r--r--   0 carlton    (501) staff       (20)       88 2022-12-20 09:06:25.000000 asgiref-3.6.0/asgiref.egg-info/requires.txt
--rw-r--r--   0 carlton    (501) staff       (20)        8 2022-12-20 09:06:25.000000 asgiref-3.6.0/asgiref.egg-info/top_level.txt
--rw-r--r--   0 carlton    (501) staff       (20)     2737 2022-12-20 09:06:25.459771 asgiref-3.6.0/setup.cfg
--rw-r--r--   0 carlton    (501) staff       (20)       62 2022-04-19 07:47:42.000000 asgiref-3.6.0/setup.py
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2022-12-20 09:06:25.458884 asgiref-3.6.0/tests/
--rw-r--r--   0 carlton    (501) staff       (20)     2329 2022-04-19 07:47:42.000000 asgiref-3.6.0/tests/test_compatibility.py
--rw-r--r--   0 carlton    (501) staff       (20)     8031 2022-04-19 07:47:42.000000 asgiref-3.6.0/tests/test_local.py
--rw-r--r--   0 carlton    (501) staff       (20)     4837 2022-12-15 09:04:51.000000 asgiref-3.6.0/tests/test_server.py
--rw-r--r--   0 carlton    (501) staff       (20)    20811 2022-12-15 09:04:51.000000 asgiref-3.6.0/tests/test_sync.py
--rw-r--r--   0 carlton    (501) staff       (20)     2121 2022-07-06 14:22:11.000000 asgiref-3.6.0/tests/test_sync_contextvars.py
--rw-r--r--   0 carlton    (501) staff       (20)     1396 2022-04-19 07:47:42.000000 asgiref-3.6.0/tests/test_testing.py
--rw-r--r--   0 carlton    (501) staff       (20)     8718 2022-04-19 07:47:42.000000 asgiref-3.6.0/tests/test_wsgi.py
+drwxr-xr-x   0 andrew    (1000) andrew    (1000)        0 2023-05-23 16:55:41.218827 asgiref-3.7.0/
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     1552 2023-05-23 16:35:51.000000 asgiref-3.7.0/LICENSE
+-rw-r--r--   0 andrew    (1000) andrew    (1000)       70 2023-05-23 16:35:51.000000 asgiref-3.7.0/MANIFEST.in
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     9006 2023-05-23 16:55:41.218827 asgiref-3.7.0/PKG-INFO
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     7756 2023-05-23 16:35:51.000000 asgiref-3.7.0/README.rst
+drwxr-xr-x   0 andrew    (1000) andrew    (1000)        0 2023-05-23 16:55:41.218827 asgiref-3.7.0/asgiref/
+-rw-r--r--   0 andrew    (1000) andrew    (1000)       22 2023-05-23 16:48:39.000000 asgiref-3.7.0/asgiref/__init__.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     1606 2023-05-23 16:35:51.000000 asgiref-3.7.0/asgiref/compatibility.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     3985 2023-05-23 16:35:51.000000 asgiref-3.7.0/asgiref/current_thread_executor.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     4854 2023-05-23 16:35:51.000000 asgiref-3.7.0/asgiref/local.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)        0 2023-05-23 16:35:51.000000 asgiref-3.7.0/asgiref/py.typed
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     6005 2023-05-23 16:35:51.000000 asgiref-3.7.0/asgiref/server.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)    21906 2023-05-23 16:35:51.000000 asgiref-3.7.0/asgiref/sync.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     3119 2023-05-23 16:35:51.000000 asgiref-3.7.0/asgiref/testing.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     3627 2023-05-23 16:35:51.000000 asgiref-3.7.0/asgiref/timeout.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     6238 2023-05-23 16:35:51.000000 asgiref-3.7.0/asgiref/typing.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     6575 2023-05-23 16:35:51.000000 asgiref-3.7.0/asgiref/wsgi.py
+drwxr-xr-x   0 andrew    (1000) andrew    (1000)        0 2023-05-23 16:55:41.218827 asgiref-3.7.0/asgiref.egg-info/
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     9006 2023-05-23 16:55:41.000000 asgiref-3.7.0/asgiref.egg-info/PKG-INFO
+-rw-r--r--   0 andrew    (1000) andrew    (1000)      613 2023-05-23 16:55:41.000000 asgiref-3.7.0/asgiref.egg-info/SOURCES.txt
+-rw-r--r--   0 andrew    (1000) andrew    (1000)        1 2023-05-23 16:55:41.000000 asgiref-3.7.0/asgiref.egg-info/dependency_links.txt
+-rw-r--r--   0 andrew    (1000) andrew    (1000)        1 2023-05-23 16:55:41.000000 asgiref-3.7.0/asgiref.egg-info/not-zip-safe
+-rw-r--r--   0 andrew    (1000) andrew    (1000)       89 2023-05-23 16:55:41.000000 asgiref-3.7.0/asgiref.egg-info/requires.txt
+-rw-r--r--   0 andrew    (1000) andrew    (1000)        8 2023-05-23 16:55:41.000000 asgiref-3.7.0/asgiref.egg-info/top_level.txt
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     2738 2023-05-23 16:55:41.218827 asgiref-3.7.0/setup.cfg
+-rw-r--r--   0 andrew    (1000) andrew    (1000)       62 2023-05-23 16:35:51.000000 asgiref-3.7.0/setup.py
+drwxr-xr-x   0 andrew    (1000) andrew    (1000)        0 2023-05-23 16:55:41.218827 asgiref-3.7.0/tests/
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     2329 2023-05-23 16:35:51.000000 asgiref-3.7.0/tests/test_compatibility.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     8031 2023-05-23 16:35:51.000000 asgiref-3.7.0/tests/test_local.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     4837 2023-05-23 16:35:51.000000 asgiref-3.7.0/tests/test_server.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)    20811 2023-05-23 16:35:51.000000 asgiref-3.7.0/tests/test_sync.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     2121 2023-05-23 16:35:51.000000 asgiref-3.7.0/tests/test_sync_contextvars.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     1396 2023-05-23 16:35:51.000000 asgiref-3.7.0/tests/test_testing.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     8718 2023-05-23 16:35:51.000000 asgiref-3.7.0/tests/test_wsgi.py
```

### Comparing `asgiref-3.6.0/LICENSE` & `asgiref-3.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asgiref-3.6.0/PKG-INFO` & `asgiref-3.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asgiref
-Version: 3.6.0
+Version: 3.7.0
 Summary: ASGI specs, helper code, and adapters
 Home-page: https://github.com/django/asgiref/
 Author: Django Software Foundation
 Author-email: foundation@djangoproject.com
 License: BSD-3-Clause
 Project-URL: Documentation, https://asgi.readthedocs.io/
 Project-URL: Further Documentation, https://docs.djangoproject.com/en/stable/topics/async/#async-adapter-functions
```

### Comparing `asgiref-3.6.0/README.rst` & `asgiref-3.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `asgiref-3.6.0/asgiref/compatibility.py` & `asgiref-3.7.0/asgiref/compatibility.py`

 * *Files identical despite different names*

### Comparing `asgiref-3.6.0/asgiref/local.py` & `asgiref-3.7.0/asgiref/local.py`

 * *Files identical despite different names*

### Comparing `asgiref-3.6.0/asgiref/server.py` & `asgiref-3.7.0/asgiref/server.py`

 * *Files identical despite different names*

### Comparing `asgiref-3.6.0/asgiref/sync.py` & `asgiref-3.7.0/asgiref/sync.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,60 +5,83 @@
 import inspect
 import os
 import sys
 import threading
 import warnings
 import weakref
 from concurrent.futures import Future, ThreadPoolExecutor
-from typing import Any, Callable, Dict, Optional, overload
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Awaitable,
+    Callable,
+    Coroutine,
+    Dict,
+    Generic,
+    List,
+    Optional,
+    TypeVar,
+    Union,
+    overload,
+)
 
 from .current_thread_executor import CurrentThreadExecutor
 from .local import Local
 
+if sys.version_info >= (3, 10):
+    from typing import ParamSpec
+else:
+    from typing_extensions import ParamSpec
 
-def _restore_context(context):
+if TYPE_CHECKING:
+    # This is not available to import at runtime
+    from _typeshed import OptExcInfo
+
+_F = TypeVar("_F", bound=Callable[..., Any])
+_P = ParamSpec("_P")
+_R = TypeVar("_R")
+
+
+def _restore_context(context: contextvars.Context) -> None:
     # Check for changes in contextvars, and set them to the current
     # context for downstream consumers
     for cvar in context:
+        cvalue = context.get(cvar)
         try:
-            if cvar.get() != context.get(cvar):
-                cvar.set(context.get(cvar))
+            if cvar.get() != cvalue:
+                cvar.set(cvalue)
         except LookupError:
-            cvar.set(context.get(cvar))
+            cvar.set(cvalue)
 
 
 # Python 3.12 deprecates asyncio.iscoroutinefunction() as an alias for
 # inspect.iscoroutinefunction(), whilst also removing the _is_coroutine marker.
 # The latter is replaced with the inspect.markcoroutinefunction decorator.
 # Until 3.12 is the minimum supported Python version, provide a shim.
 # Django 4.0 only supports 3.8+, so don't concern with the _or_partial backport.
 
-# Type hint: should be generic: whatever T it takes it returns. (Same id)
-def markcoroutinefunction(func: Any) -> Any:
-    if hasattr(inspect, "markcoroutinefunction"):
-        return inspect.markcoroutinefunction(func)
-    else:
+if hasattr(inspect, "markcoroutinefunction"):
+    iscoroutinefunction = inspect.iscoroutinefunction
+    markcoroutinefunction: Callable[[_F], _F] = inspect.markcoroutinefunction
+else:
+    iscoroutinefunction = asyncio.iscoroutinefunction  # type: ignore[assignment]
+
+    def markcoroutinefunction(func: _F) -> _F:
         func._is_coroutine = asyncio.coroutines._is_coroutine  # type: ignore
         return func
 
 
-def iscoroutinefunction(func: Any) -> bool:
-    if hasattr(inspect, "markcoroutinefunction"):
-        return inspect.iscoroutinefunction(func)
-    else:
-        return asyncio.iscoroutinefunction(func)
-
-
-def _iscoroutinefunction_or_partial(func: Any) -> bool:
-    # Python < 3.8 does not correctly determine partially wrapped
-    # coroutine functions are coroutine functions, hence the need for
-    # this to exist. Code taken from CPython.
-    if sys.version_info >= (3, 8):
-        return iscoroutinefunction(func)
-    else:
+if sys.version_info >= (3, 8):
+    _iscoroutinefunction_or_partial = iscoroutinefunction
+else:
+
+    def _iscoroutinefunction_or_partial(func: Any) -> bool:
+        # Python < 3.8 does not correctly determine partially wrapped
+        # coroutine functions are coroutine functions, hence the need for
+        # this to exist. Code taken from CPython.
         while inspect.ismethod(func):
             func = func.__func__
         while isinstance(func, functools.partial):
             func = func.func
 
         return iscoroutinefunction(func)
 
@@ -100,15 +123,15 @@
 
         executor = SyncToAsync.context_to_thread_executor.pop(self, None)
         if executor:
             executor.shutdown()
         SyncToAsync.thread_sensitive_context.reset(self.token)
 
 
-class AsyncToSync:
+class AsyncToSync(Generic[_P, _R]):
     """
     Utility class which turns an awaitable that only works on the thread with
     the event loop into a synchronous callable that works in a subthread.
 
     If the call stack contains an async loop, the code runs there.
     Otherwise, the code runs in a new loop in a new thread.
 
@@ -124,29 +147,36 @@
     # Local, not a threadlocal, so that tasks can work out what their parent used.
     executors = Local()
 
     # When we can't find a CurrentThreadExecutor from the context, such as
     # inside create_task, we'll look it up here from the running event loop.
     loop_thread_executors: "Dict[asyncio.AbstractEventLoop, CurrentThreadExecutor]" = {}
 
-    def __init__(self, awaitable, force_new_loop=False):
+    def __init__(
+        self,
+        awaitable: Union[
+            Callable[_P, Coroutine[Any, Any, _R]],
+            Callable[_P, Awaitable[_R]],
+        ],
+        force_new_loop: bool = False,
+    ):
         if not callable(awaitable) or (
             not _iscoroutinefunction_or_partial(awaitable)
             and not _iscoroutinefunction_or_partial(
                 getattr(awaitable, "__call__", awaitable)
             )
         ):
             # Python does not have very reliable detection of async functions
             # (lots of false negatives) so this is just a warning.
             warnings.warn(
                 "async_to_sync was passed a non-async-marked callable", stacklevel=2
             )
         self.awaitable = awaitable
         try:
-            self.__self__ = self.awaitable.__self__
+            self.__self__ = self.awaitable.__self__  # type: ignore[union-attr]
         except AttributeError:
             pass
         if force_new_loop:
             # They have asked that we always run in a new sub-loop.
             self.main_event_loop = None
         else:
             try:
@@ -162,15 +192,17 @@
                 if main_event_loop_pid and main_event_loop_pid == os.getpid():
                     self.main_event_loop = getattr(
                         SyncToAsync.threadlocal, "main_event_loop", None
                     )
                 else:
                     self.main_event_loop = None
 
-    def __call__(self, *args, **kwargs):
+    def __call__(self, *args: _P.args, **kwargs: _P.kwargs) -> _R:
+        __traceback_hide__ = True  # noqa: F841
+
         # You can't call AsyncToSync from a thread with a running event loop
         try:
             event_loop = asyncio.get_running_loop()
         except RuntimeError:
             pass
         else:
             if event_loop.is_running():
@@ -180,15 +212,15 @@
                 )
 
         # Wrapping context in list so it can be reassigned from within
         # `main_wrap`.
         context = [contextvars.copy_context()]
 
         # Make a future for the return information
-        call_result = Future()
+        call_result: "Future[_R]" = Future()
         # Get the source thread
         source_thread = threading.current_thread()
         # Make a CurrentThreadExecutor we'll use to idle in this thread - we
         # need one for every sync frame, even if there's one above us in the
         # same thread.
         if hasattr(self.executors, "current"):
             old_current_executor = self.executors.current
@@ -198,15 +230,20 @@
         self.executors.current = current_executor
         loop = None
         # Use call_soon_threadsafe to schedule a synchronous callback on the
         # main event loop's thread if it's there, otherwise make a new loop
         # in this thread.
         try:
             awaitable = self.main_wrap(
-                args, kwargs, call_result, source_thread, sys.exc_info(), context
+                call_result,
+                source_thread,
+                sys.exc_info(),
+                context,
+                *args,
+                **kwargs,
             )
 
             if not (self.main_event_loop and self.main_event_loop.is_running()):
                 # Make our own event loop - in a new thread - and run inside that.
                 loop = asyncio.new_event_loop()
                 self.loop_thread_executors[loop] = current_executor
                 loop_executor = ThreadPoolExecutor(max_workers=1)
@@ -271,32 +308,42 @@
                         )
                 if hasattr(loop, "shutdown_asyncgens"):
                     loop.run_until_complete(loop.shutdown_asyncgens())
             finally:
                 loop.close()
                 asyncio.set_event_loop(self.main_event_loop)
 
-    def __get__(self, parent, objtype):
+    def __get__(self, parent: Any, objtype: Any) -> Callable[_P, _R]:
         """
         Include self for methods
         """
         func = functools.partial(self.__call__, parent)
         return functools.update_wrapper(func, self.awaitable)
 
     async def main_wrap(
-        self, args, kwargs, call_result, source_thread, exc_info, context
-    ):
+        self,
+        call_result: "Future[_R]",
+        source_thread: threading.Thread,
+        exc_info: "OptExcInfo",
+        context: List[contextvars.Context],
+        *args: _P.args,
+        **kwargs: _P.kwargs,
+    ) -> None:
         """
         Wraps the awaitable with something that puts the result into the
         result/exception future.
         """
+
+        __traceback_hide__ = True  # noqa: F841
+
         if context is not None:
             _restore_context(context[0])
 
         current_task = SyncToAsync.get_current_task()
+        assert current_task is not None
         self.launch_map[current_task] = source_thread
         try:
             # If we have an exception, run the function inside the except block
             # after raising it so exc_info is correctly populated.
             if exc_info[1]:
                 try:
                     raise exc_info[1]
@@ -310,15 +357,15 @@
             call_result.set_result(result)
         finally:
             del self.launch_map[current_task]
 
             context[0] = contextvars.copy_context()
 
 
-class SyncToAsync:
+class SyncToAsync(Generic[_P, _R]):
     """
     Utility class which turns a synchronous callable into an awaitable that
     runs in a threadpool. It also sets a threadlocal inside the thread so
     calls to AsyncToSync can escape it.
 
     If thread_sensitive is passed, the code will run in the same thread as any
     outer code. This is needed for underlying Python code that is not
@@ -343,33 +390,33 @@
     threadlocal = threading.local()
 
     # Single-thread executor for thread-sensitive code
     single_thread_executor = ThreadPoolExecutor(max_workers=1)
 
     # Maintain a contextvar for the current execution context. Optionally used
     # for thread sensitive mode.
-    thread_sensitive_context: "contextvars.ContextVar[str]" = contextvars.ContextVar(
-        "thread_sensitive_context"
+    thread_sensitive_context: "contextvars.ContextVar[ThreadSensitiveContext]" = (
+        contextvars.ContextVar("thread_sensitive_context")
     )
 
     # Contextvar that is used to detect if the single thread executor
     # would be awaited on while already being used in the same context
     deadlock_context: "contextvars.ContextVar[bool]" = contextvars.ContextVar(
         "deadlock_context"
     )
 
     # Maintaining a weak reference to the context ensures that thread pools are
     # erased once the context goes out of scope. This terminates the thread pool.
-    context_to_thread_executor: "weakref.WeakKeyDictionary[object, ThreadPoolExecutor]" = (
+    context_to_thread_executor: "weakref.WeakKeyDictionary[ThreadSensitiveContext, ThreadPoolExecutor]" = (
         weakref.WeakKeyDictionary()
     )
 
     def __init__(
         self,
-        func: Callable[..., Any],
+        func: Callable[_P, _R],
         thread_sensitive: bool = True,
         executor: Optional["ThreadPoolExecutor"] = None,
     ) -> None:
         if (
             not callable(func)
             or _iscoroutinefunction_or_partial(func)
             or _iscoroutinefunction_or_partial(getattr(func, "__call__", func))
@@ -383,104 +430,105 @@
             raise TypeError("executor must not be set when thread_sensitive is True")
         self._executor = executor
         try:
             self.__self__ = func.__self__  # type: ignore
         except AttributeError:
             pass
 
-    async def __call__(self, *args, **kwargs):
+    async def __call__(self, *args: _P.args, **kwargs: _P.kwargs) -> _R:
+        __traceback_hide__ = True  # noqa: F841
         loop = asyncio.get_running_loop()
 
         # Work out what thread to run the code in
         if self._thread_sensitive:
             if hasattr(AsyncToSync.executors, "current"):
                 # If we have a parent sync thread above somewhere, use that
                 executor = AsyncToSync.executors.current
-            elif self.thread_sensitive_context and self.thread_sensitive_context.get(
-                None
-            ):
+            elif self.thread_sensitive_context.get(None):
                 # If we have a way of retrieving the current context, attempt
                 # to use a per-context thread pool executor
                 thread_sensitive_context = self.thread_sensitive_context.get()
 
                 if thread_sensitive_context in self.context_to_thread_executor:
                     # Re-use thread executor in current context
                     executor = self.context_to_thread_executor[thread_sensitive_context]
                 else:
                     # Create new thread executor in current context
                     executor = ThreadPoolExecutor(max_workers=1)
                     self.context_to_thread_executor[thread_sensitive_context] = executor
             elif loop in AsyncToSync.loop_thread_executors:
                 # Re-use thread executor for running loop
                 executor = AsyncToSync.loop_thread_executors[loop]
-            elif self.deadlock_context and self.deadlock_context.get(False):
+            elif self.deadlock_context.get(False):
                 raise RuntimeError(
                     "Single thread executor already being used, would deadlock"
                 )
             else:
                 # Otherwise, we run it in a fixed single thread
                 executor = self.single_thread_executor
-                if self.deadlock_context:
-                    self.deadlock_context.set(True)
+                self.deadlock_context.set(True)
         else:
             # Use the passed in executor, or the loop's default if it is None
             executor = self._executor
 
         context = contextvars.copy_context()
         child = functools.partial(self.func, *args, **kwargs)
         func = context.run
-        args = (child,)
-        kwargs = {}
 
         try:
             # Run the code in the right thread
-            future = loop.run_in_executor(
+            ret: _R = await loop.run_in_executor(
                 executor,
                 functools.partial(
                     self.thread_handler,
                     loop,
                     self.get_current_task(),
                     sys.exc_info(),
                     func,
-                    *args,
-                    **kwargs,
+                    child,
                 ),
             )
-            ret = await asyncio.wait_for(future, timeout=None)
 
         finally:
             _restore_context(context)
-            if self.deadlock_context:
-                self.deadlock_context.set(False)
+            self.deadlock_context.set(False)
 
         return ret
 
-    def __get__(self, parent, objtype):
+    def __get__(
+        self, parent: Any, objtype: Any
+    ) -> Callable[_P, Coroutine[Any, Any, _R]]:
         """
         Include self for methods
         """
         func = functools.partial(self.__call__, parent)
         return functools.update_wrapper(func, self.func)
 
     def thread_handler(self, loop, source_task, exc_info, func, *args, **kwargs):
         """
         Wraps the sync application with exception handling.
         """
+
+        __traceback_hide__ = True  # noqa: F841
+
         # Set the threadlocal for AsyncToSync
         self.threadlocal.main_event_loop = loop
         self.threadlocal.main_event_loop_pid = os.getpid()
         # Set the task mapping (used for the locals module)
         current_thread = threading.current_thread()
         if AsyncToSync.launch_map.get(source_task) == current_thread:
             # Our parent task was launched from this same thread, so don't make
             # a launch map entry - let it shortcut over us! (and stop infinite loops)
             parent_set = False
         else:
             self.launch_map[current_thread] = source_task
             parent_set = True
+        source_task = (
+            None  # allow the task to be garbage-collected in case of exceptions
+        )
         # Run the function
         try:
             # If we have an exception, run the function inside the except block
             # after raising it so exc_info is correctly populated.
             if exc_info[1]:
                 try:
                     raise exc_info[1]
@@ -491,15 +539,15 @@
         finally:
             # Only delete the launch_map parent if we set it, otherwise it is
             # from someone else.
             if parent_set:
                 del self.launch_map[current_thread]
 
     @staticmethod
-    def get_current_task():
+    def get_current_task() -> Optional["asyncio.Task[Any]"]:
         """
         Implementation of asyncio.current_task()
         that returns None if there is no task.
         """
         try:
             return asyncio.current_task()
         except RuntimeError:
@@ -508,35 +556,36 @@
 
 # Lowercase aliases (and decorator friendliness)
 async_to_sync = AsyncToSync
 
 
 @overload
 def sync_to_async(
-    func: None = None,
+    *,
     thread_sensitive: bool = True,
     executor: Optional["ThreadPoolExecutor"] = None,
-) -> Callable[[Callable[..., Any]], SyncToAsync]:
+) -> Callable[[Callable[_P, _R]], SyncToAsync[_P, _R]]:
     ...
 
 
 @overload
 def sync_to_async(
-    func: Callable[..., Any],
+    func: Callable[_P, _R],
+    *,
     thread_sensitive: bool = True,
     executor: Optional["ThreadPoolExecutor"] = None,
-) -> SyncToAsync:
+) -> SyncToAsync[_P, _R]:
     ...
 
 
 def sync_to_async(
-    func=None,
-    thread_sensitive=True,
-    executor=None,
-):
+    func: Optional[Callable[_P, _R]] = None,
+    thread_sensitive: bool = True,
+    executor: Optional["ThreadPoolExecutor"] = None,
+) -> Union[Callable[[Callable[_P, _R]], SyncToAsync[_P, _R]], SyncToAsync[_P, _R]]:
     if func is None:
         return lambda f: SyncToAsync(
             f,
             thread_sensitive=thread_sensitive,
             executor=executor,
         )
     return SyncToAsync(
```

### Comparing `asgiref-3.6.0/asgiref/testing.py` & `asgiref-3.7.0/asgiref/testing.py`

 * *Files identical despite different names*

### Comparing `asgiref-3.6.0/asgiref/timeout.py` & `asgiref-3.7.0/asgiref/timeout.py`

 * *Files identical despite different names*

### Comparing `asgiref-3.6.0/asgiref/typing.py` & `asgiref-3.7.0/asgiref/typing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,30 @@
 import sys
-from typing import Awaitable, Callable, Dict, Iterable, Optional, Tuple, Type, Union
+from typing import (
+    Any,
+    Awaitable,
+    Callable,
+    Dict,
+    Iterable,
+    Optional,
+    Tuple,
+    Type,
+    Union,
+)
 
 if sys.version_info >= (3, 8):
     from typing import Literal, Protocol, TypedDict
 else:
     from typing_extensions import Literal, Protocol, TypedDict
 
+if sys.version_info >= (3, 11):
+    from typing import NotRequired
+else:
+    from typing_extensions import NotRequired
+
 __all__ = (
     "ASGIVersions",
     "HTTPScope",
     "WebSocketScope",
     "LifespanScope",
     "WWWScope",
     "Scope",
@@ -58,14 +73,15 @@
     path: str
     raw_path: bytes
     query_string: bytes
     root_path: str
     headers: Iterable[Tuple[bytes, bytes]]
     client: Optional[Tuple[str, int]]
     server: Optional[Tuple[str, Optional[int]]]
+    state: NotRequired[Dict[str, Any]]
     extensions: Optional[Dict[str, Dict[object, object]]]
 
 
 class WebSocketScope(TypedDict):
     type: Literal["websocket"]
     asgi: ASGIVersions
     http_version: str
@@ -74,32 +90,39 @@
     raw_path: bytes
     query_string: bytes
     root_path: str
     headers: Iterable[Tuple[bytes, bytes]]
     client: Optional[Tuple[str, int]]
     server: Optional[Tuple[str, Optional[int]]]
     subprotocols: Iterable[str]
+    state: NotRequired[Dict[str, Any]]
     extensions: Optional[Dict[str, Dict[object, object]]]
 
 
 class LifespanScope(TypedDict):
     type: Literal["lifespan"]
     asgi: ASGIVersions
+    state: NotRequired[Dict[str, Any]]
 
 
 WWWScope = Union[HTTPScope, WebSocketScope]
 Scope = Union[HTTPScope, WebSocketScope, LifespanScope]
 
 
 class HTTPRequestEvent(TypedDict):
     type: Literal["http.request"]
     body: bytes
     more_body: bool
 
 
+class HTTPResponseDebugEvent(TypedDict):
+    type: Literal["http.response.debug"]
+    info: Dict[str, object]
+
+
 class HTTPResponseStartEvent(TypedDict):
     type: Literal["http.response.start"]
     status: int
     headers: Iterable[Tuple[bytes, bytes]]
     trailers: bool
```

### Comparing `asgiref-3.6.0/asgiref/wsgi.py` & `asgiref-3.7.0/asgiref/wsgi.py`

 * *Files identical despite different names*

### Comparing `asgiref-3.6.0/asgiref.egg-info/PKG-INFO` & `asgiref-3.7.0/asgiref.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asgiref
-Version: 3.6.0
+Version: 3.7.0
 Summary: ASGI specs, helper code, and adapters
 Home-page: https://github.com/django/asgiref/
 Author: Django Software Foundation
 Author-email: foundation@djangoproject.com
 License: BSD-3-Clause
 Project-URL: Documentation, https://asgi.readthedocs.io/
 Project-URL: Further Documentation, https://docs.djangoproject.com/en/stable/topics/async/#async-adapter-functions
```

### Comparing `asgiref-3.6.0/asgiref.egg-info/SOURCES.txt` & `asgiref-3.7.0/asgiref.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `asgiref-3.6.0/setup.cfg` & `asgiref-3.7.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 	Changelog = https://github.com/django/asgiref/blob/master/CHANGELOG.txt
 
 [options]
 python_requires = >=3.7
 packages = find:
 include_package_data = true
 install_requires = 
-	typing_extensions; python_version < "3.8"
+	typing_extensions; python_version < "3.11"
 zip_safe = false
 
 [options.extras_require]
 tests = 
 	pytest
 	pytest-asyncio
 	mypy>=0.800
```

### Comparing `asgiref-3.6.0/tests/test_compatibility.py` & `asgiref-3.7.0/tests/test_compatibility.py`

 * *Files identical despite different names*

### Comparing `asgiref-3.6.0/tests/test_local.py` & `asgiref-3.7.0/tests/test_local.py`

 * *Files identical despite different names*

### Comparing `asgiref-3.6.0/tests/test_server.py` & `asgiref-3.7.0/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `asgiref-3.6.0/tests/test_sync.py` & `asgiref-3.7.0/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `asgiref-3.6.0/tests/test_sync_contextvars.py` & `asgiref-3.7.0/tests/test_sync_contextvars.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import asyncio
+import contextvars
 import threading
 import time
 
 import pytest
 
 from asgiref.sync import ThreadSensitiveContext, async_to_sync, sync_to_async
 
-contextvars = pytest.importorskip("contextvars")
-
-foo = contextvars.ContextVar("foo")
+foo: "contextvars.ContextVar[str]" = contextvars.ContextVar("foo")
 
 
 @pytest.mark.asyncio
 async def test_thread_sensitive_with_context_different():
     result_1 = {}
     result_2 = {}
```

### Comparing `asgiref-3.6.0/tests/test_testing.py` & `asgiref-3.7.0/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `asgiref-3.6.0/tests/test_wsgi.py` & `asgiref-3.7.0/tests/test_wsgi.py`

 * *Files identical despite different names*

