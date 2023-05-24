# Comparing `tmp/mobilex-0.0.4a0.tar.gz` & `tmp/mobilex-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mobilex-0.0.4a0.tar", max compression
+gzip compressed data, was "mobilex-0.0.5.tar", max compression
```

## Comparing `mobilex-0.0.4a0.tar` & `mobilex-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1067 2023-05-23 05:26:17.390648 mobilex-0.0.4a0/LICENSE.txt
--rw-r--r--   0        0        0     1365 2023-05-23 05:26:31.482713 mobilex-0.0.4a0/README.md
--rw-r--r--   0        0        0      342 2023-05-23 05:26:17.390648 mobilex-0.0.4a0/mobilex/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 05:26:17.390648 mobilex-0.0.4a0/mobilex/cache/__init__.py
--rw-r--r--   0        0        0     3594 2023-05-23 05:26:17.390648 mobilex-0.0.4a0/mobilex/cache/base.py
--rw-r--r--   0        0        0     1880 2023-05-23 05:26:17.390648 mobilex-0.0.4a0/mobilex/cache/dict.py
--rw-r--r--   0        0        0     1765 2023-05-23 05:26:17.390648 mobilex-0.0.4a0/mobilex/cache/redis.py
--rw-r--r--   0        0        0      327 2023-05-23 05:26:17.390648 mobilex-0.0.4a0/mobilex/const.py
--rw-r--r--   0        0        0     4935 2023-05-23 05:26:17.390648 mobilex-0.0.4a0/mobilex/core.py
--rw-r--r--   0        0        0     1022 2023-05-23 05:26:17.390648 mobilex-0.0.4a0/mobilex/exc.py
--rw-r--r--   0        0        0     2516 2023-05-23 05:26:17.390648 mobilex-0.0.4a0/mobilex/response.py
--rw-r--r--   0        0        0     6057 2023-05-23 05:26:17.390648 mobilex-0.0.4a0/mobilex/router.py
--rw-r--r--   0        0        0      267 2023-05-23 05:26:17.390648 mobilex-0.0.4a0/mobilex/screens/__init__.py
--rw-r--r--   0        0        0    11671 2023-05-23 05:26:17.390648 mobilex-0.0.4a0/mobilex/screens/base.py
--rw-r--r--   0        0        0     6932 2023-05-23 05:26:17.390648 mobilex-0.0.4a0/mobilex/sessions.py
--rw-r--r--   0        0        0     1807 2023-05-23 05:26:17.390648 mobilex-0.0.4a0/mobilex/utils/__init__.py
--rw-r--r--   0        0        0     1881 2023-05-23 05:26:17.390648 mobilex-0.0.4a0/mobilex/utils/types.py
--rw-r--r--   0        0        0     1828 2023-05-23 05:26:17.390648 mobilex-0.0.4a0/pyproject.toml
--rw-r--r--   0        0        0     2167 1970-01-01 00:00:00.000000 mobilex-0.0.4a0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-24 19:02:48.099800 mobilex-0.0.5/LICENSE.txt
+-rw-r--r--   0        0        0     1361 2023-05-24 19:03:08.344431 mobilex-0.0.5/README.md
+-rw-r--r--   0        0        0      435 2023-05-24 19:02:48.099800 mobilex-0.0.5/mobilex/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 19:02:48.099800 mobilex-0.0.5/mobilex/cache/__init__.py
+-rw-r--r--   0        0        0     3594 2023-05-24 19:02:48.099800 mobilex-0.0.5/mobilex/cache/base.py
+-rw-r--r--   0        0        0     1880 2023-05-24 19:02:48.099800 mobilex-0.0.5/mobilex/cache/dict.py
+-rw-r--r--   0        0        0     1765 2023-05-24 19:02:48.099800 mobilex-0.0.5/mobilex/cache/redis.py
+-rw-r--r--   0        0        0      327 2023-05-24 19:02:48.099800 mobilex-0.0.5/mobilex/const.py
+-rw-r--r--   0        0        0     5402 2023-05-24 19:02:48.099800 mobilex-0.0.5/mobilex/core.py
+-rw-r--r--   0        0        0     1223 2023-05-24 19:02:48.099800 mobilex-0.0.5/mobilex/exc.py
+-rw-r--r--   0        0        0     2531 2023-05-24 19:02:48.099800 mobilex-0.0.5/mobilex/responses.py
+-rw-r--r--   0        0        0     5696 2023-05-24 19:02:48.099800 mobilex-0.0.5/mobilex/router.py
+-rw-r--r--   0        0        0      267 2023-05-24 19:02:48.103801 mobilex-0.0.5/mobilex/screens/__init__.py
+-rw-r--r--   0        0        0    11265 2023-05-24 19:02:48.103801 mobilex-0.0.5/mobilex/screens/base.py
+-rw-r--r--   0        0        0     6898 2023-05-24 19:02:48.103801 mobilex-0.0.5/mobilex/sessions.py
+-rw-r--r--   0        0        0     1807 2023-05-24 19:02:48.103801 mobilex-0.0.5/mobilex/utils/__init__.py
+-rw-r--r--   0        0        0     1881 2023-05-24 19:02:48.103801 mobilex-0.0.5/mobilex/utils/types.py
+-rw-r--r--   0        0        0     1826 2023-05-24 19:02:48.103801 mobilex-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2161 1970-01-01 00:00:00.000000 mobilex-0.0.5/PKG-INFO
```

### Comparing `mobilex-0.0.4a0/LICENSE.txt` & `mobilex-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mobilex-0.0.4a0/README.md` & `mobilex-0.0.5/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -38,8 +38,8 @@
 [pyversions-link]: https://pypi.python.org/pypi/mobilex
 [ci-image]: https://github.com/davidkyalo/python-mobilex/actions/workflows/workflow.yaml/badge.svg?event=push&branch=main
 [ci-link]: https://github.com/davidkyalo/python-mobilex/actions?query=workflow%3ACI%2FCD+event%3Apush+branch%3Amaster
 [codecov-image]: https://codecov.io/gh/davidkyalo/python-mobilex/branch/main/graph/badge.svg
 [codecov-link]: https://codecov.io/gh/davidkyalo/python-mobilex
 
 
-See this release on GitHub: [v0.0.4a0](https://github.com/davidkyalo/python-mobilex/releases/tag/0.0.4a0)
+See this release on GitHub: [v0.0.5](https://github.com/davidkyalo/python-mobilex/releases/tag/0.0.5)
```

### Comparing `mobilex-0.0.4a0/mobilex/cache/base.py` & `mobilex-0.0.5/mobilex/cache/base.py`

 * *Files identical despite different names*

### Comparing `mobilex-0.0.4a0/mobilex/cache/dict.py` & `mobilex-0.0.5/mobilex/cache/dict.py`

 * *Files identical despite different names*

### Comparing `mobilex-0.0.4a0/mobilex/cache/redis.py` & `mobilex-0.0.5/mobilex/cache/redis.py`

 * *Files identical despite different names*

### Comparing `mobilex-0.0.4a0/mobilex/core.py` & `mobilex-0.0.5/mobilex/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 from collections import abc
 from datetime import timedelta
 from functools import cached_property
 
 from mobilex.utils.types import FrozenNamespaceDict
 
 from .router import Router
+from .screens import Screen
 from .sessions import History, Session, SessionManager
 from .utils import ArgumentVector, to_timedelta
 
 if t.TYPE_CHECKING:
     from .cache.base import BaseCache
-    from .response import Response
+    from .responses import Response
 
 
 class ConfigDict(t.TypedDict, total=False):
     max_page_length: int
     session_class: type[Session]
     session_key_prefix: str
     session_backend: type["BaseCache"]
@@ -75,22 +76,22 @@
 
     @cached_property
     def base_uri(self):
         return "*".join(filter(None, (self.service_code, self.initial_code)))
 
 
 class App:
-    router: Router
-    session_manager: "SessionManager"
+    router: t.Final[Router]
     name: t.Final[str]
-    _initial_config: dict[str, t.Any]
+    _initial_config: t.Final[dict[str, t.Any]]
 
-    def __init__(self, name: str = None, **config):
+    def __init__(self, name: str = None, router: Router = None, **config):
         self.name = "mobilex.app" if name is None else name
         self.has_booted = False
+        self.router = router or Router()
         self._initial_config = self.get_default_config().copy()
         config and self.configure(config)
 
     @cached_property
     def config(self):
         conf = self._initial_config
         del self._initial_config
@@ -139,34 +140,43 @@
             session_manager=SessionManager,
             history_key_prefix="state",
             history_backend=None,
             history_class=History,
             history_ttl=None,
         )
 
-    def setup(self):
-        assert (
-            not self.has_booted
-        ), f"{type(self).__name__}.boot() called multiple times."
-
-        self.config
-        self.router.run_embeded(self)
-        self.has_booted = True
-        return self
+    # def setup(self):
+    #     assert (
+    #         not self.has_booted
+    #     ), f"{type(self).__name__}.boot() called multiple times."
+
+    #     self.config
+    #     # self.router.run_embeded(self)
+    #     self.has_booted = True
+    #     return self
 
-    def include_router(self, router, name: t.Optional[str] = None):
-        self.router = router
+    # def include_router(self, router, name: t.Optional[str] = None):
+    #     self.router = router
 
     async def close_session(self, request: Request, response: "Response"):
         await self.session_manager.close(request, response)
 
     async def prepare_request(self, request: Request) -> Request:
         request.app = self
         await self.session_manager.open(request)
 
     async def teardown_request(self, request, response):
         await self.close_session(request, response)
 
-    async def adispatch(self, request, *args, **kwargs):
+    async def __call__(self, request, *args, **kwargs):
         await self.prepare_request(request)
         response = await self.router(request)
         return await self.teardown_request(request, response) or response
+
+    def screen(self, name: str, screen: type["Screen"] = None, **kwds):
+        return self.router.screen(name, screen, **kwds)
+
+    def entry_screen(self, name: str, screen: type[Screen] = None):
+        return self.router.entry_screen(name, screen)
+
+    def home_screen(self, name: str, screen: type[Screen] = None):
+        return self.router.home_screen(name, screen)
```

### Comparing `mobilex-0.0.4a0/mobilex/exc.py` & `mobilex-0.0.5/mobilex/exc.py`

 * *Files 24% similar despite different names*

```diff
@@ -40,7 +40,13 @@
 class InputError(ValidationError):
     pass
 
 
 class InvalidChoiceError(ValidationError):
     default_code = "invalid_choice"
     default_message = "Error! Invalid choice"
+
+
+class ScreenNotFoundError(LookupError):
+    def __init__(self, *args, name: str = None) -> None:
+        super().__init__(*(args if args else (repr(name),) if name else ()))
+        self.name = name
```

### Comparing `mobilex-0.0.4a0/mobilex/response.py` & `mobilex-0.0.5/mobilex/responses.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 import typing as t
-
-
 from collections import ChainMap
 from typing import Any
 
 from .const import ResponseType
 
-
 if t.TYPE_CHECKING:
     from . import Request
 
 
 class _ResponseMeta(type):
     def __new__(mcls, name, bases, dct):
         super_new = super(_ResponseMeta, mcls).__new__
@@ -40,29 +37,29 @@
         /,
         type: t.Optional[ResponseType] = None,
     ):
         self.content = content
         self.type = type or self.__class__.type
         self.ctx = ChainMap() if ctx is None else ChainMap({}, ctx)
 
-    def get_context(self, request, ctx: t.Optional[t.Mapping] = None):
-        return self.ctx.new(ctx)
+    # def get_context(self, request, ctx: t.Optional[t.Mapping] = None):
+    #     return self.ctx.new(ctx)
 
-    async def render_content(self, request, ctx: t.Optional[t.Mapping] = None):
-        return f"{self.type} {self.content}"
+    # async def render_content(self, request, ctx: t.Optional[t.Mapping] = None):
+    #     return f"{self.type} {self.content}"
 
     def __getstate__(self):
         return {n: getattr(self, n) for n in self.__state_attrs__}
 
-    def __setstate__(self, state):
-        for k, v in state.items():
-            setattr(self, k, v)
+    # def __setstate__(self, state):
+    #     for k, v in state.items():
+    #         setattr(self, k, v)
 
-    async def __call__(self, request, ctx: t.Optional[t.Mapping] = None):
-        return await self.render_content(request, ctx)
+    # async def __call__(self, request, ctx: t.Optional[t.Mapping] = None):
+    #     return await self.render_content(request, ctx)
 
 
 R_to = t.TypeVar("R_to", str, int)
 
 
 class RedirectResponse(t.Generic[R_to], Response):
     __state_attrs__ = ("to",)
```

### Comparing `mobilex-0.0.4a0/mobilex/screens/base.py` & `mobilex-0.0.5/mobilex/screens/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from copy import copy
 from inspect import isawaitable
 from logging import getLogger
 from operator import attrgetter
 from typing import Any, Iterator
 
 from .. import exc
-from ..response import redirect
+from ..responses import Response, redirect
 from ..utils.types import NamespaceDict
 
 if t.TYPE_CHECKING:
     from mobilex import App, Request
     from mobilex.sessions import Session
 
 
@@ -122,42 +122,47 @@
     key: str = None
     name: str = None
 
     def handle(self, screen: "Screen", value: str):
         args, kwds = self.args or (), self.kwargs or {}
         if (to := self.screen) is not None:
             return redirect(to, *args, **kwds)
-        elif callable(func := self.handler):
+        elif callable(func := self.handler or "handle"):
             return func(screen, value, *args, **kwds)
         elif isinstance(func, str):
             return getattr(screen, func)(value, *args, **kwds)
 
     def __str__(self):
         return "" if self.key is None else f"{self.key:<2} {self.label}"
 
+    def __bool__(self):
+        return self.key is not None
 
-_null_action = Action(None)
+
+_null_act = Action(None)
 
 
 class _ActionDict(dict[str, _AT]):
     __slots__ = ()
 
 
 class ActionSet(abc.Set[_AT]):
     __slots__ = ("_chain", "_src")
-
+    _src: abc.Mapping[str, _AT]
     _chain: ChainMap[str, _AT]
 
     def __new__(cls, it: abc.Iterable[_AT] = ()):
-        self, named = object.__new__(cls), None
-        if isinstance(it, ActionSet):
-            it, named = it._chain.maps
-        src = _ActionDict(it if isinstance(it, _ActionDict) else cls._parse_src(it))
-        named = {o.name: o for o in src.values()} if named is None else copy(named)
-        self._chain, self._src = ChainMap(src, named), src
+        self = object.__new__(cls)
+        self._src = _ActionDict(
+            it._src
+            if isinstance(it, ActionSet)
+            else it
+            if isinstance(it, _ActionDict)
+            else cls._parse_src(it)
+        )
         return self
 
     @classmethod
     def _parse_src(cls, iterable: abc.Iterable[_AT]):
         seen, i = set(), 0
 
         for it in iterable:
@@ -182,36 +187,36 @@
         if not isinstance(x, ActionSet):
             if not isinstance(x, abc.Iterable):
                 return NotImplemented
             x = self.__class__(x)
         return self.__class__(_ActionDict(self._src | x._src))
 
     def __contains__(self, x: object) -> bool:
-        return self._to_key(x) in self._chain
+        return self._to_key(x) in self._src
 
     def __len__(self) -> int:
         return len(self._src)
 
     def __iter__(self) -> Iterator[_AT]:
         return iter(self._src.values())
 
     def __getitem__(self, key):
-        return self._chain[self._to_key(key)]
+        return self._src[self._to_key(key)]
 
     def __reduce__(self) -> str | tuple[Any, ...]:
         return self.__class__, (self._src,)
 
     def get(self, key, default: _DT = None):
-        return self._chain.get(self._to_key(key), default)
+        return self._src.get(self._to_key(key), default)
 
     def keys(self):
         return self._src.keys()
 
-    def names(self):
-        return self._chain.maps[1].keys()
+    # def names(self):
+    #     return self._src.maps[1].keys()
 
 
 class Screen(t.Generic[T], metaclass=ScreenType):
     # META_OPTIONS_CLASS = ScreenMetaOptions
 
     CON = CON
 
@@ -231,22 +236,25 @@
     _payload_class: type[UssdPayload] = UssdPayload
     _state_class: type[ScreenState] = ScreenState
     _has_actions: bool = False
 
     actions = None
 
     nav_actions = [
-        Action("Back", key="0", screen=-1, name="back"),
-        Action("Home", key="00", screen=0, name="home"),
+        Action("Back", key="0", screen=-1),
+        Action("Home", key="00", screen=0),
     ]
 
-    pagination_actions = [
-        Action("Back", key="0", name="prev"),
-        Action("More", key="99", name="next"),
-    ]
+    # pagination_actions = [
+    #     Action("Back", key="0", name="prev"),
+    #     Action("More", key="99", name="next"),
+    # ]
+
+    next_page_action = Action("More", key="99")
+    prev_page_action = Action("Back", key="0")
 
     def __init__(self, state):
         self.state = state
         self.payload = self._payload_class("")
 
     @t.overload
     def print(self, *objs, sep=" ", end=NL):
@@ -255,133 +263,121 @@
     @property
     def print(self):
         return self.payload.append
 
     def get_actions(self):
         return self.actions or ()
 
-    def get_pagination_actions(self):
-        return self.pagination_actions or ()
+    # def get_pagination_actions(self):
+    #     return self.pagination_actions or ()
 
     def get_nav_actions(self):
         return self.nav_actions or ()
 
     def get_action_set(self):
         return ActionSet(self.get_actions())
 
-    def get_pagination_action_set(self):
-        return ActionSet(self.get_pagination_actions())
+    # def get_pagination_action_set(self):
+    #     return ActionSet(self.get_pagination_actions())
+
+    # def get_next_page_action(self):
+    #     return self.next_page_action or _null_action
+
+    # def get_prev_page_action(self):
+    #     return self.prev_page_action or _null_action
 
     def get_nav_action_set(self):
         return ActionSet(self.get_nav_actions())
 
     async def handle(self, inpt):
-        if self._has_actions:
-            self.print("Invalid choice!")
+        self._has_actions and self.print("Error! Invalid choice.")
 
     async def render(self):
-        return
+        pass
 
-    async def handle_exception(self, e, inpt=None):
-        if inpt is not None and isinstance(e, exc.ValidationError):
-            self.payload.prepend(e)
-            return await self._async_render()
-        else:
-            raise e
+    # async def handle_exception(self, e, inpt=None):
+    #     if inpt is not None and isinstance(e, exc.ValidationError):
+    #         self.payload.prepend(e)
+    #         return await self._async_render()
+    #     else:
+    #         raise e
 
     async def _async_init(self, inpt=None):
         rv = self.init(inpt)
         if isawaitable(rv):
             rv = await rv
         return rv
 
     async def _async_render(self):
         rv = self.render()
         if isawaitable(rv):
             rv = await rv
         return rv
 
-    async def _async_handle(self, inpt):
-        rv = self.handle(inpt)
-        if isawaitable(rv):
-            rv = await rv
-        return rv
-
-    async def _async_validate(self, inpt):
-        rv = self.validate(inpt)
-        if isawaitable(rv):
-            rv = await rv
-        return rv
+    # async def _async_handle(self, inpt):
+    #     rv = self.handle(inpt)
+    #     if isawaitable(rv):
+    #         rv = await rv
+    #     return rv
+
+    # async def _async_validate(self, inpt):
+    #     rv = self.validate(inpt)
+    #     if isawaitable(rv):
+    #         rv = await rv
+    #     return rv
 
     async def _async_handle_exception(self, e, inpt=None):
         rv = self.handle_exception(e, inpt)
         if isawaitable(rv):
             rv = await rv
         return rv
 
     def abort(self, *args, **kwargs):
         raise exc.ValidationError(*args, **kwargs)
 
-    async def __call__(self, request: "Request", input=None):
+    async def __call__(self, request: "Request", input: str = None):
         self.request = request
         rv, pages, i = None, self.state.get("_pages", []), 0
         current_page = self.state.get("_current_page", 0)
         key = input if input is None else f"{input}".strip()
 
-        # actions = self.get_action_set()
-        # if current_page == 0 and key is not None and key in actions:
-        #     if (rv := actions[key].handle(self, key)) is not None:
-        #         return rv
-        #     input = key = None
-
-        pg_acts = self.get_pagination_action_set()
-        next, prev = (pg_acts.get(k, _null_action) for k in ("next", "prev"))
-
-        if key is not None and len(pages) > 1 and key in pg_acts:
-            if key == prev.key and current_page > 0:
-                self.state._current_page = i = current_page - 1
-                rv = self.state._action
-            elif key == next.key and current_page < len(pages) - 1:
+        if not (was_ready := self.state.get("__initialized__")):
+            if self.init is not None:
+                rv = await self._async_init(input)
+            self.state.__initialized__ = True
+
+        next, prev = self.next_page_action, self.prev_page_action
+        if is_next := key and key == next.key:
+            if current_page < len(pages) - 1:
                 self.state._current_page = i = current_page + 1
                 rv = self.state._action
+        elif key == prev.key and current_page > 0:
+            self.state._current_page = i = current_page - 1
+            rv = self.state._action
 
         if rv is None:
-            try:
-                if not self.state.get("__initialized__"):
-                    if self.init is not None:
-                        rv = await self._async_init(input)
-                    self.state.__initialized__ = True
-
-                # ACTIONS HERE
-                acts, nav_acts = self.get_action_set(), self.get_nav_action_set()
-                self._has_actions = not not acts
-
-                if key is not None:
-                    if act := acts.get(key) or nav_acts.get(key):
-                        rv = act.handle(self, key)
-
-                if rv is None and input is not None:
-                    if self.validate is not None:
-                        input = await self._async_validate(input)
-
-                    if input is not None:
-                        rv = await self._async_handle(input)
-
-                rv is None and (rv := await self._async_render())
-            except Exception as e:
-                rv = await self._async_handle_exception(e, input)
+            acts, nav_acts = self.get_action_set(), self.get_nav_action_set()
+            self._has_actions = not not acts
+            if not (key is None or is_next):
+                act = acts.get(key) or nav_acts.get(key) or _null_act
+                if isawaitable(rv := act.handle(self, input)):
+                    rv = await rv
 
             if rv is None:
-                rv = self.exit_code
+                if isawaitable(rv := self.render()):
+                    rv = await rv
 
-            if rv in (self.CON, self.END):
-                payload = self.payload
-                acts and payload.append(*acts, sep=NL)
-                nav_acts = [] if rv == self.END else nav_acts
-                mx_page_len = request.app.config.max_page_length - 4
-                pages = list(payload.paginate(mx_page_len, next, prev, nav_acts))
-                self.state._action, self.state._pages = rv, pages
-                self.state._current_page = i = 0
-            else:
+            if isinstance(rv, Response):
                 return rv
 
-        return rv, pages[i]
+            if rv is None:
+                rv = self.exit_code
+
+            payload = self.payload
+            acts and payload.append(*acts, sep=NL)
+            nav_acts = [] if rv == self.END else nav_acts
+            mx_page_len = request.app.config.max_page_length - 4
+            pages = list(payload.paginate(mx_page_len, next, prev, nav_acts))
+            self.state._action, self.state._pages = rv, pages
+            self.state._current_page = i = 1 if is_next and len(pages) > 1 else 0
+
+        return f"{rv} {pages[i]}"
```

### Comparing `mobilex-0.0.4a0/mobilex/sessions.py` & `mobilex-0.0.5/mobilex/sessions.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,15 +192,14 @@
         del self.stack, self.background
         background and await asyncio.gather(*background)
 
     def __len__(self):
         return len(self.stack)
 
     async def pop(self, k: int = None):
-        # k is None and (k := -1)
         k = -1 if k is None else k + 1 if k > -1 else k
         stack = self.stack
         stack[k:] = []
         if id := stack[-1]:
             return await self.backend.get(self.make_key(id))
 
     async def push(self, res: "Response"):
```

### Comparing `mobilex-0.0.4a0/mobilex/utils/__init__.py` & `mobilex-0.0.5/mobilex/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mobilex-0.0.4a0/mobilex/utils/types.py` & `mobilex-0.0.5/mobilex/utils/types.py`

 * *Files identical despite different names*

### Comparing `mobilex-0.0.4a0/pyproject.toml` & `mobilex-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mobilex"
-version = "0.0.4a0"
+version = "0.0.5"
 description = "USSD and SMS exchange framework"
 authors = ["David Kyalo <davidmkyalo@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/davidkyalo/python-mobilex"
 documentation = "https://davidkyalo.github.io/python-mobilex"
 keywords = [
```

### Comparing `mobilex-0.0.4a0/PKG-INFO` & `mobilex-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mobilex
-Version: 0.0.4a0
+Version: 0.0.5
 Summary: USSD and SMS exchange framework
 Home-page: https://github.com/davidkyalo/python-mobilex
 License: MIT
 Keywords: mobilex,mobile,USSD,SMS
 Author: David Kyalo
 Author-email: davidmkyalo@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -59,9 +59,9 @@
 [pyversions-link]: https://pypi.python.org/pypi/mobilex
 [ci-image]: https://github.com/davidkyalo/python-mobilex/actions/workflows/workflow.yaml/badge.svg?event=push&branch=main
 [ci-link]: https://github.com/davidkyalo/python-mobilex/actions?query=workflow%3ACI%2FCD+event%3Apush+branch%3Amaster
 [codecov-image]: https://codecov.io/gh/davidkyalo/python-mobilex/branch/main/graph/badge.svg
 [codecov-link]: https://codecov.io/gh/davidkyalo/python-mobilex
 
 
-See this release on GitHub: [v0.0.4a0](https://github.com/davidkyalo/python-mobilex/releases/tag/0.0.4a0)
+See this release on GitHub: [v0.0.5](https://github.com/davidkyalo/python-mobilex/releases/tag/0.0.5)
```

