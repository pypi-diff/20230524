# Comparing `tmp/wraps-0.6.0.tar.gz` & `tmp/wraps-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wraps-0.6.0.tar", max compression
+gzip compressed data, was "wraps-0.6.1.tar", max compression
```

## Comparing `wraps-0.6.0.tar` & `wraps-0.6.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1092 2023-05-21 09:34:54.330970 wraps-0.6.0/LICENSE
--rw-r--r--   0        0        0     6517 2023-05-21 09:34:54.330970 wraps-0.6.0/README.md
--rw-r--r--   0        0        0     3331 2023-05-21 09:34:54.330970 wraps-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     2566 2023-05-21 09:34:54.330970 wraps-0.6.0/wraps/__init__.py
--rw-r--r--   0        0        0     2854 2023-05-21 09:34:54.330970 wraps-0.6.0/wraps/early.py
--rw-r--r--   0        0        0    15277 2023-05-21 09:34:54.330970 wraps-0.6.0/wraps/either.py
--rw-r--r--   0        0        0     1228 2023-05-21 09:34:54.330970 wraps-0.6.0/wraps/errors.py
--rw-r--r--   0        0        0     4379 2023-05-21 09:34:54.330970 wraps-0.6.0/wraps/future.py
--rw-r--r--   0        0        0     1360 2023-05-21 09:34:54.330970 wraps-0.6.0/wraps/future_either.py
--rw-r--r--   0        0        0    12016 2023-05-21 09:34:54.330970 wraps-0.6.0/wraps/future_option.py
--rw-r--r--   0        0        0    15809 2023-05-21 09:34:54.330970 wraps-0.6.0/wraps/future_result.py
--rw-r--r--   0        0        0      340 2023-05-21 09:34:54.330970 wraps-0.6.0/wraps/markers.py
--rw-r--r--   0        0        0    41151 2023-05-21 09:34:54.330970 wraps-0.6.0/wraps/option.py
--rw-r--r--   0        0        0        0 2023-05-21 09:34:54.330970 wraps-0.6.0/wraps/py.typed
--rw-r--r--   0        0        0     1811 2023-05-21 09:34:54.330970 wraps-0.6.0/wraps/reawaitable.py
--rw-r--r--   0        0        0    53509 2023-05-21 09:34:54.330970 wraps-0.6.0/wraps/result.py
--rw-r--r--   0        0        0      855 2023-05-21 09:34:54.330970 wraps-0.6.0/wraps/typing.py
--rw-r--r--   0        0        0      604 2023-05-21 09:34:54.330970 wraps-0.6.0/wraps/utils.py
--rw-r--r--   0        0        0     9424 2023-05-21 09:34:54.330970 wraps-0.6.0/wraps/wraps.py
--rw-r--r--   0        0        0     7767 1970-01-01 00:00:00.000000 wraps-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-05-23 23:17:12.662531 wraps-0.6.1/LICENSE
+-rw-r--r--   0        0        0     6517 2023-05-23 23:17:12.662531 wraps-0.6.1/README.md
+-rw-r--r--   0        0        0     3325 2023-05-23 23:17:12.662531 wraps-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     2566 2023-05-23 23:17:12.662531 wraps-0.6.1/wraps/__init__.py
+-rw-r--r--   0        0        0     2854 2023-05-23 23:17:12.662531 wraps-0.6.1/wraps/early.py
+-rw-r--r--   0        0        0    15277 2023-05-23 23:17:12.662531 wraps-0.6.1/wraps/either.py
+-rw-r--r--   0        0        0     1228 2023-05-23 23:17:12.662531 wraps-0.6.1/wraps/errors.py
+-rw-r--r--   0        0        0     4379 2023-05-23 23:17:12.662531 wraps-0.6.1/wraps/future.py
+-rw-r--r--   0        0        0     1360 2023-05-23 23:17:12.662531 wraps-0.6.1/wraps/future_either.py
+-rw-r--r--   0        0        0    12016 2023-05-23 23:17:12.662531 wraps-0.6.1/wraps/future_option.py
+-rw-r--r--   0        0        0    15809 2023-05-23 23:17:12.662531 wraps-0.6.1/wraps/future_result.py
+-rw-r--r--   0        0        0      340 2023-05-23 23:17:12.662531 wraps-0.6.1/wraps/markers.py
+-rw-r--r--   0        0        0    41147 2023-05-23 23:17:12.662531 wraps-0.6.1/wraps/option.py
+-rw-r--r--   0        0        0        0 2023-05-23 23:17:12.662531 wraps-0.6.1/wraps/py.typed
+-rw-r--r--   0        0        0     1811 2023-05-23 23:17:12.662531 wraps-0.6.1/wraps/reawaitable.py
+-rw-r--r--   0        0        0    53509 2023-05-23 23:17:12.666530 wraps-0.6.1/wraps/result.py
+-rw-r--r--   0        0        0      855 2023-05-23 23:17:12.666530 wraps-0.6.1/wraps/typing.py
+-rw-r--r--   0        0        0      604 2023-05-23 23:17:12.666530 wraps-0.6.1/wraps/utils.py
+-rw-r--r--   0        0        0     9424 2023-05-23 23:17:12.666530 wraps-0.6.1/wraps/wraps.py
+-rw-r--r--   0        0        0     7767 1970-01-01 00:00:00.000000 wraps-0.6.1/PKG-INFO
```

### Comparing `wraps-0.6.0/LICENSE` & `wraps-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wraps-0.6.0/README.md` & `wraps-0.6.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 $ poetry add wraps
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-wraps = "^0.6.0"
+wraps = "^0.6.1"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.wraps]
 git = "https://github.com/nekitdev/wraps.git"
```

### Comparing `wraps-0.6.0/pyproject.toml` & `wraps-0.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wraps"
-version = "0.6.0"
+version = "0.6.1"
 description = "Meaningful and safe wrapping types."
 authors = ["nekitdev"]
 license = "MIT"
 
 readme = "README.md"
 
 homepage = "https://github.com/nekitdev/wraps"
@@ -32,15 +32,15 @@
 [tool.poetry.dependencies]
 python = ">= 3.7"
 
 attrs = ">= 23.1.0"
 
 funcs = ">= 0.5.1"
 
-typing-aliases = ">= 1.1.0"
+typing-aliases = ">= 1.1.2"
 typing-extensions = ">= 4.5.0"
 
 [tool.poetry.group.format]
 optional = true
 
 [tool.poetry.group.format.dependencies]
 black = "23.3.0"
@@ -106,15 +106,15 @@
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
@@ -142,15 +142,15 @@
 warn_unreachable = true
 
 warn_redundant_casts = true
 warn_unused_ignores = false  # compatibility
 
 [tool.changelogging]
 name = "wraps"
-version = "0.6.0"
+version = "0.6.1"
 url = "https://github.com/nekitdev/wraps"
 directory = "changes"
 output = "CHANGELOG.md"
 
 start_string = "<!-- changelogging: start -->"
 
 title_format = "{version} ({date})"
```

### Comparing `wraps-0.6.0/wraps/__init__.py` & `wraps-0.6.1/wraps/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 __description__ = "Meaningful and safe wrapping types."
 __url__ = "https://github.com/nekitdev/wraps"
 
 __title__ = "wraps"
 __author__ = "nekitdev"
 __license__ = "MIT"
-__version__ = "0.6.0"
+__version__ = "0.6.1"
 
 from wraps.early import early_option, early_option_await, early_result, early_result_await
 from wraps.either import Either, Left, Right, is_left, is_right
 from wraps.errors import Panic, panic
 from wraps.future import Future
 from wraps.future_option import FutureOption
 from wraps.future_result import FutureResult
```

### Comparing `wraps-0.6.0/wraps/early.py` & `wraps-0.6.1/wraps/early.py`

 * *Files identical despite different names*

### Comparing `wraps-0.6.0/wraps/either.py` & `wraps-0.6.1/wraps/either.py`

 * *Files identical despite different names*

### Comparing `wraps-0.6.0/wraps/errors.py` & `wraps-0.6.1/wraps/errors.py`

 * *Files identical despite different names*

### Comparing `wraps-0.6.0/wraps/future.py` & `wraps-0.6.1/wraps/future.py`

 * *Files identical despite different names*

### Comparing `wraps-0.6.0/wraps/future_either.py` & `wraps-0.6.1/wraps/future_either.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Future either values."""
 
 from __future__ import annotations
 
-from typing import Awaitable, TypeVar, final
+from typing import Awaitable, TypeVar
 
 from attrs import field, frozen
-from typing_extensions import Never
+from typing_extensions import Never, final
 
 from wraps.either import Either, Left, Right
 from wraps.future import Future
 from wraps.reawaitable import ReAwaitable
 
 __all__ = ("FutureEither",)
```

### Comparing `wraps-0.6.0/wraps/future_option.py` & `wraps-0.6.1/wraps/future_option.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """Future optional values."""
 
 from __future__ import annotations
 
-from typing import Awaitable, Optional, Tuple, TypeVar, final
+from typing import Awaitable, Optional, Tuple, TypeVar
 
 from attrs import field, frozen
 from typing_aliases import (
     AsyncBinary,
     AsyncInspect,
     AsyncNullary,
     AsyncPredicate,
     AsyncUnary,
     Binary,
     Inspect,
     Nullary,
     Predicate,
     Unary,
 )
-from typing_extensions import Never
+from typing_extensions import Never, final
 
 from wraps.future import Future, identity
 from wraps.option import Null, Option, Some
 from wraps.reawaitable import ReAwaitable
 from wraps.result import Result
 
 __all__ = ("FutureOption",)
```

### Comparing `wraps-0.6.0/wraps/future_result.py` & `wraps-0.6.1/wraps/future_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """Future error handling."""
 
 from __future__ import annotations
 
-from typing import Awaitable, TypeVar, final
+from typing import Awaitable, TypeVar
 
 from attrs import field, frozen
 from typing_aliases import (
     AnyError,
     AsyncInspect,
     AsyncNullary,
     AsyncPredicate,
     AsyncUnary,
     Inspect,
     Nullary,
     Predicate,
     Unary,
 )
-from typing_extensions import Never
+from typing_extensions import Never, final
 
 from wraps.either import Either
 from wraps.future import Future
 from wraps.option import Option
 from wraps.reawaitable import ReAwaitable
 from wraps.result import Error, Ok, Result
 from wraps.utils import identity
```

### Comparing `wraps-0.6.0/wraps/option.py` & `wraps-0.6.1/wraps/option.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,14 @@
     AsyncIterator,
     Iterable,
     Iterator,
     Optional,
     Tuple,
     TypeVar,
     Union,
-    final,
     overload,
 )
 
 from attrs import frozen
 from typing_aliases import (
     AsyncBinary,
     AsyncInspect,
@@ -75,15 +74,15 @@
     AsyncUnary,
     Binary,
     Inspect,
     Nullary,
     Predicate,
     Unary,
 )
-from typing_extensions import Literal, Never, Protocol, TypeGuard
+from typing_extensions import Literal, Never, Protocol, TypeGuard, final
 
 from wraps.errors import EarlyOption, panic
 from wraps.utils import async_empty, async_once, empty, identity, once
 
 __all__ = ("Option", "Some", "Null", "is_some", "is_null")
 
 T = TypeVar("T", covariant=True)
```

### Comparing `wraps-0.6.0/wraps/reawaitable.py` & `wraps-0.6.1/wraps/reawaitable.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from typing import Awaitable, Callable, Generator, TypeVar, final
+from typing import Awaitable, Callable, Generator, TypeVar
 
 from attrs import define, field
 from funcs.decorators import wraps
 from typing_aliases import AsyncCallable
-from typing_extensions import ParamSpec
+from typing_extensions import ParamSpec, final
 
 from wraps.option import Null, Option, Some
 
 __all__ = ("ReAwaitable", "reawaitable")
 
 P = ParamSpec("P")
```

### Comparing `wraps-0.6.0/wraps/result.py` & `wraps-0.6.1/wraps/result.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,29 +41,29 @@
         print(error)
 ```
 """
 
 from __future__ import annotations
 
 from abc import abstractmethod as required
-from typing import AsyncIterable, AsyncIterator, Iterable, Iterator, TypeVar, Union, final
+from typing import AsyncIterable, AsyncIterator, Iterable, Iterator, TypeVar, Union
 
 from attrs import frozen
 from typing_aliases import (
     AnyError,
     AsyncInspect,
     AsyncNullary,
     AsyncPredicate,
     AsyncUnary,
     Inspect,
     Nullary,
     Predicate,
     Unary,
 )
-from typing_extensions import Literal, Never, ParamSpec, Protocol, TypeGuard
+from typing_extensions import Literal, Never, ParamSpec, Protocol, TypeGuard, final
 
 from wraps.errors import EarlyResult, panic
 from wraps.option import Null, Option, Some
 from wraps.utils import async_empty, async_once, empty, identity, once
 
 __all__ = ("Result", "Ok", "Error", "is_ok", "is_error")
```

### Comparing `wraps-0.6.0/wraps/typing.py` & `wraps-0.6.1/wraps/typing.py`

 * *Files identical despite different names*

### Comparing `wraps-0.6.0/wraps/utils.py` & `wraps-0.6.1/wraps/utils.py`

 * *Files identical despite different names*

### Comparing `wraps-0.6.0/wraps/wraps.py` & `wraps-0.6.1/wraps/wraps.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Highly composable wrapping decorators."""
 
 from __future__ import annotations
 
-from typing import Callable, Generic, Optional, Type, TypeVar, final
+from typing import Callable, Generic, Optional, Type, TypeVar
 
 from attrs import frozen
 from funcs.decorators import wraps
 from typing_aliases import AnyError, AsyncCallable, NormalError
-from typing_extensions import ParamSpec
+from typing_extensions import ParamSpec, final
 
 from wraps.either import Either
 from wraps.future import Future
 from wraps.future_either import FutureEither
 from wraps.future_option import FutureOption
 from wraps.future_result import FutureResult
 from wraps.option import Null, Option, Some
```

### Comparing `wraps-0.6.0/PKG-INFO` & `wraps-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wraps
-Version: 0.6.0
+Version: 0.6.1
 Summary: Meaningful and safe wrapping types.
 Home-page: https://github.com/nekitdev/wraps
 License: MIT
 Keywords: python,future,either,option,result
 Author: nekitdev
 Requires-Python: >=3.7
 Classifier: Development Status :: 4 - Beta
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Dist: attrs (>=23.1.0)
 Requires-Dist: funcs (>=0.5.1)
-Requires-Dist: typing-aliases (>=1.1.0)
+Requires-Dist: typing-aliases (>=1.1.2)
 Requires-Dist: typing-extensions (>=4.5.0)
 Project-URL: Documentation, https://nekitdev.github.io/wraps
 Project-URL: Discord, https://nekit.dev/discord
 Project-URL: Funding, https://patreon.com/nekitdev
 Project-URL: Issues, https://github.com/nekitdev/wraps/issues
 Project-URL: Repository, https://github.com/nekitdev/wraps
 Description-Content-Type: text/markdown
@@ -72,15 +72,15 @@
 $ poetry add wraps
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-wraps = "^0.6.0"
+wraps = "^0.6.1"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.wraps]
 git = "https://github.com/nekitdev/wraps.git"
```

