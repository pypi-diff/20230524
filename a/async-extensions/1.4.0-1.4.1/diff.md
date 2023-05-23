# Comparing `tmp/async_extensions-1.4.0.tar.gz` & `tmp/async_extensions-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_extensions-1.4.0.tar", max compression
+gzip compressed data, was "async_extensions-1.4.1.tar", max compression
```

## Comparing `async_extensions-1.4.0.tar` & `async_extensions-1.4.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1092 2023-05-21 09:20:36.972542 async_extensions-1.4.0/LICENSE
--rw-r--r--   0        0        0     2578 2023-05-21 09:20:36.972542 async_extensions-1.4.0/README.md
--rw-r--r--   0        0        0     2968 2023-05-21 09:20:36.972542 async_extensions-1.4.0/async_extensions/__init__.py
--rw-r--r--   0        0        0      732 2023-05-21 09:20:36.972542 async_extensions-1.4.0/async_extensions/blocking.py
--rw-r--r--   0        0        0      431 2023-05-21 09:20:36.972542 async_extensions-1.4.0/async_extensions/cancel.py
--rw-r--r--   0        0        0     1174 2023-05-21 09:20:36.972542 async_extensions-1.4.0/async_extensions/channel.py
--rw-r--r--   0        0        0     1583 2023-05-21 09:20:36.972542 async_extensions-1.4.0/async_extensions/close.py
--rw-r--r--   0        0        0     7800 2023-05-21 09:20:36.972542 async_extensions-1.4.0/async_extensions/collect.py
--rw-r--r--   0        0        0      118 2023-05-21 09:20:36.972542 async_extensions-1.4.0/async_extensions/constants.py
--rw-r--r--   0        0        0       80 2023-05-21 09:20:36.972542 async_extensions-1.4.0/async_extensions/current.py
--rw-r--r--   0        0        0       88 2023-05-21 09:20:36.972542 async_extensions-1.4.0/async_extensions/errors.py
--rw-r--r--   0        0        0      101 2023-05-21 09:20:36.972542 async_extensions-1.4.0/async_extensions/file.py
--rw-r--r--   0        0        0      174 2023-05-21 09:20:36.972542 async_extensions-1.4.0/async_extensions/low_level.py
--rw-r--r--   0        0        0       44 2023-05-21 09:20:36.972542 async_extensions-1.4.0/async_extensions/path.py
--rw-r--r--   0        0        0       87 2023-05-21 09:20:36.972542 async_extensions-1.4.0/async_extensions/process.py
--rw-r--r--   0        0        0        0 2023-05-21 09:20:36.972542 async_extensions-1.4.0/async_extensions/py.typed
--rw-r--r--   0        0        0      396 2023-05-21 09:20:36.972542 async_extensions-1.4.0/async_extensions/run.py
--rw-r--r--   0        0        0       76 2023-05-21 09:20:36.972542 async_extensions-1.4.0/async_extensions/signal.py
--rw-r--r--   0        0        0       77 2023-05-21 09:20:36.972542 async_extensions-1.4.0/async_extensions/sleep.py
--rw-r--r--   0        0        0     1319 2023-05-21 09:20:36.972542 async_extensions-1.4.0/async_extensions/standard.py
--rw-r--r--   0        0        0      143 2023-05-21 09:20:36.972542 async_extensions-1.4.0/async_extensions/synchronization.py
--rw-r--r--   0        0        0      243 2023-05-21 09:20:36.972542 async_extensions-1.4.0/async_extensions/task_group.py
--rw-r--r--   0        0        0      176 2023-05-21 09:20:36.972542 async_extensions-1.4.0/async_extensions/types.py
--rw-r--r--   0        0        0      732 2023-05-21 09:20:36.972542 async_extensions-1.4.0/async_extensions/wait.py
--rw-r--r--   0        0        0     2498 2023-05-21 09:20:36.972542 async_extensions-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     3853 1970-01-01 00:00:00.000000 async_extensions-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-05-23 22:35:22.801587 async_extensions-1.4.1/LICENSE
+-rw-r--r--   0        0        0     2578 2023-05-23 22:35:22.801587 async_extensions-1.4.1/README.md
+-rw-r--r--   0        0        0     2968 2023-05-23 22:35:22.801587 async_extensions-1.4.1/async_extensions/__init__.py
+-rw-r--r--   0        0        0      732 2023-05-23 22:35:22.801587 async_extensions-1.4.1/async_extensions/blocking.py
+-rw-r--r--   0        0        0      431 2023-05-23 22:35:22.801587 async_extensions-1.4.1/async_extensions/cancel.py
+-rw-r--r--   0        0        0     1174 2023-05-23 22:35:22.801587 async_extensions-1.4.1/async_extensions/channel.py
+-rw-r--r--   0        0        0     1583 2023-05-23 22:35:22.801587 async_extensions-1.4.1/async_extensions/close.py
+-rw-r--r--   0        0        0     7821 2023-05-23 22:35:22.801587 async_extensions-1.4.1/async_extensions/collect.py
+-rw-r--r--   0        0        0      118 2023-05-23 22:35:22.801587 async_extensions-1.4.1/async_extensions/constants.py
+-rw-r--r--   0        0        0       80 2023-05-23 22:35:22.801587 async_extensions-1.4.1/async_extensions/current.py
+-rw-r--r--   0        0        0       88 2023-05-23 22:35:22.801587 async_extensions-1.4.1/async_extensions/errors.py
+-rw-r--r--   0        0        0      101 2023-05-23 22:35:22.801587 async_extensions-1.4.1/async_extensions/file.py
+-rw-r--r--   0        0        0      174 2023-05-23 22:35:22.801587 async_extensions-1.4.1/async_extensions/low_level.py
+-rw-r--r--   0        0        0       44 2023-05-23 22:35:22.801587 async_extensions-1.4.1/async_extensions/path.py
+-rw-r--r--   0        0        0       87 2023-05-23 22:35:22.801587 async_extensions-1.4.1/async_extensions/process.py
+-rw-r--r--   0        0        0        0 2023-05-23 22:35:22.801587 async_extensions-1.4.1/async_extensions/py.typed
+-rw-r--r--   0        0        0      396 2023-05-23 22:35:22.801587 async_extensions-1.4.1/async_extensions/run.py
+-rw-r--r--   0        0        0       76 2023-05-23 22:35:22.801587 async_extensions-1.4.1/async_extensions/signal.py
+-rw-r--r--   0        0        0       77 2023-05-23 22:35:22.801587 async_extensions-1.4.1/async_extensions/sleep.py
+-rw-r--r--   0        0        0     1319 2023-05-23 22:35:22.801587 async_extensions-1.4.1/async_extensions/standard.py
+-rw-r--r--   0        0        0      143 2023-05-23 22:35:22.801587 async_extensions-1.4.1/async_extensions/synchronization.py
+-rw-r--r--   0        0        0      243 2023-05-23 22:35:22.801587 async_extensions-1.4.1/async_extensions/task_group.py
+-rw-r--r--   0        0        0      176 2023-05-23 22:35:22.801587 async_extensions-1.4.1/async_extensions/types.py
+-rw-r--r--   0        0        0      732 2023-05-23 22:35:22.801587 async_extensions-1.4.1/async_extensions/wait.py
+-rw-r--r--   0        0        0     2498 2023-05-23 22:35:22.801587 async_extensions-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0     3853 1970-01-01 00:00:00.000000 async_extensions-1.4.1/PKG-INFO
```

### Comparing `async_extensions-1.4.0/LICENSE` & `async_extensions-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `async_extensions-1.4.0/README.md` & `async_extensions-1.4.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 $ poetry add async-extensions
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-async-extensions = "^1.4.0"
+async-extensions = "^1.4.1"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.async-extensions]
 git = "https://github.com/nekitdev/async-extensions.git"
```

### Comparing `async_extensions-1.4.0/async_extensions/__init__.py` & `async_extensions-1.4.1/async_extensions/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 __description__ = "Asynchronous extensions."
 __url__ = "https://github.com/nekitdev/async-extensions"
 
 __title__ = "async_extensions"
 __author__ = "nekitdev"
 __license__ = "MIT"
-__version__ = "1.4.0"
+__version__ = "1.4.1"
 
 from async_extensions.blocking import run_blocking_in_process, run_blocking_in_thread
 from async_extensions.cancel import CancelScope, create_cancel_scope, shield
 from async_extensions.channel import (
     MemoryChannel,
     MemoryChannelFactory,
     MemoryReceiveChannel,
```

### Comparing `async_extensions-1.4.0/async_extensions/blocking.py` & `async_extensions-1.4.1/async_extensions/blocking.py`

 * *Files identical despite different names*

### Comparing `async_extensions-1.4.0/async_extensions/channel.py` & `async_extensions-1.4.1/async_extensions/channel.py`

 * *Files identical despite different names*

### Comparing `async_extensions-1.4.0/async_extensions/close.py` & `async_extensions-1.4.1/async_extensions/close.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from abc import abstractmethod as required
 from types import TracebackType as Traceback
-from typing import AsyncContextManager, Awaitable, Optional, Type, TypeVar, final
+from typing import AsyncContextManager, Awaitable, Optional, Type, TypeVar
 
 from attrs import frozen
 from typing_aliases import AnyError
-from typing_extensions import Protocol, runtime_checkable
+from typing_extensions import Protocol, final, runtime_checkable
 
 from async_extensions.cancel import create_cancel_scope
 
 __all__ = (
     "AsyncCloseable",
     "AsyncClosing",
     "async_close",
```

### Comparing `async_extensions-1.4.0/async_extensions/collect.py` & `async_extensions-1.4.1/async_extensions/collect.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 from typing import Any, AsyncIterable, AsyncIterator, Awaitable, List, Tuple, TypeVar, overload
 
 from typing_aliases import (
-    AnyError, AnyIterable, DynamicTuple, EmptyTuple, is_async_iterable, is_iterable
+    AnyError,
+    AnyIterable,
+    DynamicTuple,
+    EmptyTuple,
+    is_async_iterable,
+    is_iterable,
 )
 from wraps.result import Error, Ok, Result
 
 from async_extensions.standard import iter_to_async_iter
 from async_extensions.task_group import create_task_group
 
 __all__ = ("collect", "collect_results", "collect_iterable", "collect_iterable_results")
```

### Comparing `async_extensions-1.4.0/async_extensions/standard.py` & `async_extensions-1.4.1/async_extensions/standard.py`

 * *Files identical despite different names*

### Comparing `async_extensions-1.4.0/async_extensions/wait.py` & `async_extensions-1.4.1/async_extensions/wait.py`

 * *Files identical despite different names*

### Comparing `async_extensions-1.4.0/pyproject.toml` & `async_extensions-1.4.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "async-extensions"
-version = "1.4.0"
+version = "1.4.1"
 description = "Asynchronous extensions."
 authors = ["nekitdev"]
 license = "MIT"
 
 readme = "README.md"
 
 homepage = "https://github.com/nekitdev/async-extensions"
@@ -31,17 +31,17 @@
 [tool.poetry.dependencies]
 python = ">= 3.7"
 
 attrs = ">= 23.1.0"
 
 anyio = ">= 3.6.2"
 solus = ">= 1.1.0"
-wraps = ">= 0.5.0"
+wraps = ">= 0.6.0"
 
-typing-aliases = ">= 1.1.0"
+typing-aliases = ">= 1.1.2"
 typing-extensions = ">= 4.5.0"
 
 [tool.poetry.group.format]
 optional = true
 
 [tool.poetry.group.format.dependencies]
 black = "23.3.0"
@@ -58,15 +58,15 @@
 [tool.poetry.group.check]
 optional = true
 
 [tool.poetry.group.check.dependencies]
 mypy = "1.3.0"
 
 [tool.poetry.group.dev.dependencies]
-changelogging = "1.2.0"
+changelogging = "1.3.0"
 
 [tool.black]
 line_length = 100
 
 [tool.flake8]
 max_line_length = 100
 
@@ -97,15 +97,15 @@
 warn_unreachable = true
 
 warn_redundant_casts = true
 warn_unused_ignores = false  # compatibility
 
 [tool.changelogging]
 name = "async-extensions"
-version = "1.4.0"
+version = "1.4.1"
 url = "https://github.com/nekitdev/async-extensions"
 directory = "changes"
 output = "CHANGELOG.md"
 
 start_string = "<!-- changelogging: start -->"
 
 title_format = "{version} ({date})"
@@ -114,9 +114,9 @@
 bullet = "-"
 wrap = true
 wrap_size = 100
 
 display = ["feature", "change", "fix", "security", "deprecation", "removal", "internal"]
 
 [build-system]
-requires = ["poetry-core >= 1.4.0"]
+requires = ["poetry-core >= 1.5.2"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `async_extensions-1.4.0/PKG-INFO` & `async_extensions-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-extensions
-Version: 1.4.0
+Version: 1.4.1
 Summary: Asynchronous extensions.
 Home-page: https://github.com/nekitdev/async-extensions
 License: MIT
 Keywords: python,async,extensions
 Author: nekitdev
 Requires-Python: >=3.7
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,17 +18,17 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Dist: anyio (>=3.6.2)
 Requires-Dist: attrs (>=23.1.0)
 Requires-Dist: solus (>=1.1.0)
-Requires-Dist: typing-aliases (>=1.1.0)
+Requires-Dist: typing-aliases (>=1.1.2)
 Requires-Dist: typing-extensions (>=4.5.0)
-Requires-Dist: wraps (>=0.5.0)
+Requires-Dist: wraps (>=0.6.0)
 Project-URL: Discord, https://nekit.dev/discord
 Project-URL: Funding, https://patreon.com/nekitdev
 Project-URL: Issues, https://github.com/nekitdev/solus/issues
 Project-URL: Repository, https://github.com/nekitdev/async-extensions
 Description-Content-Type: text/markdown
 
 # `async-extensions`
@@ -69,15 +69,15 @@
 $ poetry add async-extensions
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-async-extensions = "^1.4.0"
+async-extensions = "^1.4.1"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.async-extensions]
 git = "https://github.com/nekitdev/async-extensions.git"
```

