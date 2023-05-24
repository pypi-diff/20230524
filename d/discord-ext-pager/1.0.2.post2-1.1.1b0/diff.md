# Comparing `tmp/discord-ext-pager-1.0.2.post2.tar.gz` & `tmp/discord-ext-pager-1.1.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord-ext-pager-1.0.2.post2.tar", last modified: Mon May  8 15:01:06 2023, max compression
+gzip compressed data, was "discord-ext-pager-1.1.1b0.tar", last modified: Wed May 24 01:14:45 2023, max compression
```

## Comparing `discord-ext-pager-1.0.2.post2.tar` & `discord-ext-pager-1.1.1b0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:01:06.245339 discord-ext-pager-1.0.2.post2/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-05-08 15:00:51.000000 discord-ext-pager-1.0.2.post2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-05-08 15:01:06.245339 discord-ext-pager-1.0.2.post2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-05-08 15:00:51.000000 discord-ext-pager-1.0.2.post2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-08 15:00:51.000000 discord-ext-pager-1.0.2.post2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 15:01:06.245339 discord-ext-pager-1.0.2.post2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:01:06.241339 discord-ext-pager-1.0.2.post2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:01:06.241339 discord-ext-pager-1.0.2.post2/src/discord/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:01:06.241339 discord-ext-pager-1.0.2.post2/src/discord/ext/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:01:06.245339 discord-ext-pager-1.0.2.post2/src/discord/ext/pager/
--rw-r--r--   0 runner    (1001) docker     (123)    15645 2023-05-08 15:00:51.000000 discord-ext-pager-1.0.2.post2/src/discord/ext/pager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:01:06.245339 discord-ext-pager-1.0.2.post2/src/discord_ext_pager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-05-08 15:01:06.000000 discord-ext-pager-1.0.2.post2/src/discord_ext_pager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-08 15:01:06.000000 discord-ext-pager-1.0.2.post2/src/discord_ext_pager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 15:01:06.000000 discord-ext-pager-1.0.2.post2/src/discord_ext_pager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-08 15:01:06.000000 discord-ext-pager-1.0.2.post2/src/discord_ext_pager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-08 15:01:06.000000 discord-ext-pager-1.0.2.post2/src/discord_ext_pager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 01:14:45.414966 discord-ext-pager-1.1.1b0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-05-24 01:14:33.000000 discord-ext-pager-1.1.1b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-05-24 01:14:45.414966 discord-ext-pager-1.1.1b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-05-24 01:14:33.000000 discord-ext-pager-1.1.1b0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-24 01:14:33.000000 discord-ext-pager-1.1.1b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 01:14:45.414966 discord-ext-pager-1.1.1b0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 01:14:45.414966 discord-ext-pager-1.1.1b0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 01:14:45.410966 discord-ext-pager-1.1.1b0/src/discord/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 01:14:45.414966 discord-ext-pager-1.1.1b0/src/discord/ext/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 01:14:45.414966 discord-ext-pager-1.1.1b0/src/discord/ext/pager/
+-rw-r--r--   0 runner    (1001) docker     (123)    16861 2023-05-24 01:14:33.000000 discord-ext-pager-1.1.1b0/src/discord/ext/pager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 01:14:45.414966 discord-ext-pager-1.1.1b0/src/discord_ext_pager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-05-24 01:14:45.000000 discord-ext-pager-1.1.1b0/src/discord_ext_pager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-24 01:14:45.000000 discord-ext-pager-1.1.1b0/src/discord_ext_pager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 01:14:45.000000 discord-ext-pager-1.1.1b0/src/discord_ext_pager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-24 01:14:45.000000 discord-ext-pager-1.1.1b0/src/discord_ext_pager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-24 01:14:45.000000 discord-ext-pager-1.1.1b0/src/discord_ext_pager.egg-info/top_level.txt
```

### Comparing `discord-ext-pager-1.0.2.post2/LICENSE` & `discord-ext-pager-1.1.1b0/LICENSE`

 * *Files identical despite different names*

### Comparing `discord-ext-pager-1.0.2.post2/PKG-INFO` & `discord-ext-pager-1.1.1b0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-ext-pager
-Version: 1.0.2.post2
+Version: 1.1.1b0
 Summary: A view-based paginator library for discord.py 2.0
 Author: thegamecracks
 Project-URL: Homepage, https://github.com/thegamecracks/discord-ext-pager
 Keywords: discord,discord.py,paginator,view
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
@@ -43,35 +43,37 @@
   The base class for sources the paginator view can accept.
 - ListPageSource:
   The base class for formatting a list of items.
 - AsyncIteratorPageSource:
   The base class for formatting an asynchronous iterator of items.
 - PageOption:
   A subclass of `discord.SelectOption` used for presenting navigation options.
+- StopAction:
+  An enum for customizing PaginatorView's stop button behaviour.
 - TimeoutAction:
   An enum for customizing PaginatorView's timeout behaviour.
 
 [discord-ext-pager]: https://pypi.org/project/discord-ext-pager/
 [discord-ext-menus]: https://github.com/Rapptz/discord-ext-menus
 
 The `PaginatorView` can be instantiated and used by itself, but page formatting
 is handled by subclassing one of the `PageSource` base classes.
 
 ```py
-from typing import Any, List
-from discord.ext.pager import ListPageSource, PaginatorView
+from typing import List
+from discord.ext.pager import ListPageSource, PageSource, PaginatorView
 
-class EmbedListPageSource(ListPageSource[Any, None, PaginatorView]):
-    #                                   ^^^^^^^^^^^^^^^^^^^^^^^^^^
+class EmbedListPageSource(ListPageSource[object, PageSource, PaginatorView]):
+    #                                   ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
     #            These type parameters denote the page item type,
     #            source type for page options (demonstrated later),
     #            and view type. Only needed for static typing.
     """Takes a list of items and formats it in an embed."""
 
-    def format_page(self, view: PaginatorView, page: List[Any]):
+    def format_page(self, view: PaginatorView, page: List[object]):
         index = self.current_index * self.page_size
         description = "\n".join(
             f"{i}. {x}"
             for i, x in enumerate(page, start=index + 1)
         )
         return discord.Embed(description=description)
 
@@ -86,19 +88,19 @@
 should be overridden to return a list of `PageOption` objects for the user
 to select from:
 
 ```py
 from typing import List
 from discord.ext.pager import ListPageSource, PageOption, PageSource, PaginatorView
 
-class MessageSource(PageSource[str, None, PaginatorView]):
+class MessageSource(PageSource[str, PageSource, PaginatorView]):
     """A single page for displaying a string."""
 
-    def __init__(self, message: str, *, current_index: int = 0):
-        super().__init__(current_index=current_index)
+    def __init__(self, message: str):
+        super().__init__(current_index=0)
         self.message = message
 
     def get_page(self, index: int):
         return self.message
 
     def format_page(self, view: PaginatorView, page: str):
         # If we don't specify both content and embed, either will
```

### Comparing `discord-ext-pager-1.0.2.post2/README.md` & `discord-ext-pager-1.1.1b0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,35 +17,37 @@
   The base class for sources the paginator view can accept.
 - ListPageSource:
   The base class for formatting a list of items.
 - AsyncIteratorPageSource:
   The base class for formatting an asynchronous iterator of items.
 - PageOption:
   A subclass of `discord.SelectOption` used for presenting navigation options.
+- StopAction:
+  An enum for customizing PaginatorView's stop button behaviour.
 - TimeoutAction:
   An enum for customizing PaginatorView's timeout behaviour.
 
 [discord-ext-pager]: https://pypi.org/project/discord-ext-pager/
 [discord-ext-menus]: https://github.com/Rapptz/discord-ext-menus
 
 The `PaginatorView` can be instantiated and used by itself, but page formatting
 is handled by subclassing one of the `PageSource` base classes.
 
 ```py
-from typing import Any, List
-from discord.ext.pager import ListPageSource, PaginatorView
+from typing import List
+from discord.ext.pager import ListPageSource, PageSource, PaginatorView
 
-class EmbedListPageSource(ListPageSource[Any, None, PaginatorView]):
-    #                                   ^^^^^^^^^^^^^^^^^^^^^^^^^^
+class EmbedListPageSource(ListPageSource[object, PageSource, PaginatorView]):
+    #                                   ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
     #            These type parameters denote the page item type,
     #            source type for page options (demonstrated later),
     #            and view type. Only needed for static typing.
     """Takes a list of items and formats it in an embed."""
 
-    def format_page(self, view: PaginatorView, page: List[Any]):
+    def format_page(self, view: PaginatorView, page: List[object]):
         index = self.current_index * self.page_size
         description = "\n".join(
             f"{i}. {x}"
             for i, x in enumerate(page, start=index + 1)
         )
         return discord.Embed(description=description)
 
@@ -60,19 +62,19 @@
 should be overridden to return a list of `PageOption` objects for the user
 to select from:
 
 ```py
 from typing import List
 from discord.ext.pager import ListPageSource, PageOption, PageSource, PaginatorView
 
-class MessageSource(PageSource[str, None, PaginatorView]):
+class MessageSource(PageSource[str, PageSource, PaginatorView]):
     """A single page for displaying a string."""
 
-    def __init__(self, message: str, *, current_index: int = 0):
-        super().__init__(current_index=current_index)
+    def __init__(self, message: str):
+        super().__init__(current_index=0)
         self.message = message
 
     def get_page(self, index: int):
         return self.message
 
     def format_page(self, view: PaginatorView, page: str):
         # If we don't specify both content and embed, either will
```

### Comparing `discord-ext-pager-1.0.2.post2/pyproject.toml` & `discord-ext-pager-1.1.1b0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `discord-ext-pager-1.0.2.post2/src/discord/ext/pager/__init__.py` & `discord-ext-pager-1.1.1b0/src/discord/ext/pager/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,21 +23,22 @@
     Union,
     cast,
 )
 
 import discord
 from typing_extensions import TypeAlias
 
-__version__ = "1.0.2.post2"
+__version__ = "1.1.1b"
 
 __all__ = (
     "PageOption",
     "PageSource",
     "ListPageSource",
     "AsyncIteratorPageSource",
+    "StopAction",
     "TimeoutAction",
     "PaginatorView",
 )
 
 E = TypeVar("E")
 T = TypeVar("T")
 S_co = TypeVar("S_co", bound="PageSource", covariant=True)
@@ -171,16 +172,29 @@
         return self._cache[start:end]
 
     @property
     def max_pages(self) -> int:
         return self._max_index + (not self._exhausted)
 
 
+class StopAction(Enum):
+    """Specifies the action to take when the view is stopped."""
+
+    NONE = auto()
+    """On stop, no action will occur on the message."""
+    DISABLE = auto()
+    """On stop, all components will be disabled."""
+    CLEAR = auto()
+    """On stop, all components will be removed from the message."""
+    DELETE = auto()
+    """On stop, the message will be deleted."""
+
+
 class TimeoutAction(Enum):
-    """Specifies what action should be taken when the view times out."""
+    """Specifies the action to take when the view times out."""
 
     NONE = auto()
     """On timeout, no action will occur on the message."""
     DISABLE = auto()
     """On timeout, all components will be disabled."""
     CLEAR = auto()
     """On timeout, all components will be removed from the message."""
@@ -206,39 +220,45 @@
     different behavior entirely.
 
     Parameters
     ----------
     :param sources: The current stack of page sources.
     :param allowed_users: A collection of user IDs that are allowed
         to interact with this paginator. If None, any user can interact.
+    :param stop_action:
+        The action to do when the user clicks the stop button. This may
+        not have any effect if a subclass overrides the `stop_button()`
+        component.
     :param timeout_action:
         The action to do when the view times out. This may not have any
         effect if a subclass overrides the `on_timeout()` method.
 
     """
 
     def __init__(
         self,
         *args,
         sources: Union[
             Iterable[PageSource[T, S_co, V_contra]],
             PageSource[T, S_co, V_contra],
         ],
         allowed_users: Optional[Collection[int]] = None,
+        stop_action: StopAction = StopAction.DELETE,
         timeout_action: TimeoutAction = TimeoutAction.CLEAR,
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
         if isinstance(sources, PageSource):
             self.sources = [sources]
         else:
             self.sources = list(sources)
             if len(self.sources) == 0:
                 raise ValueError("must provide at least one page source")
         self.allowed_users = allowed_users
+        self.stop_action = stop_action
         self.timeout_action = timeout_action
 
         self.message: Optional[discord.Message] = None
         self.page: _PageParams = {}
         self.options: Sequence[PageOption[S_co]] = []
         self.option_sources: dict[str, PageSource] = {}
 
@@ -328,22 +348,24 @@
             return
 
         if action is TimeoutAction.CLEAR:
             await self.message.edit(view=None)
         elif action is TimeoutAction.DELETE:
             await self.message.delete()
         elif action is TimeoutAction.DISABLE:
-            for item in self.children:
-                if hasattr(item, "disabled"):
-                    item.disabled = True  # type: ignore
-
+            self._disable_components()
             await self.message.edit(view=self)
         else:
             raise TypeError(f"unknown timeout action: {action!r}")
 
+    def _disable_components(self) -> None:
+        for item in self.children:
+            if hasattr(item, "disabled"):
+                item.disabled = True  # type: ignore
+
     def _get_message_kwargs(self, *, initial_response: bool = False) -> Dict[str, Any]:
         # initial_response indicates if we can use view=None, necessary as
         # InteractionResponse.send_message() does not accept view=None
         kwargs = dict(self.page)
         max_pages = self.current_source.max_pages
         can_interact = self.can_navigate or self.can_paginate or self.can_go_back
 
@@ -473,17 +495,29 @@
         row=1,
     )
     async def stop_button(
         self,
         interaction: discord.Interaction,
         button: discord.ui.Button,
     ) -> None:
+        action = self.stop_action
         self.stop()
-        await interaction.response.defer()
-        await interaction.delete_original_response()
+
+        if action is StopAction.NONE:
+            return
+        elif action is StopAction.CLEAR:
+            await interaction.response.edit_message(view=None)
+        elif action is StopAction.DELETE:
+            await interaction.response.defer()
+            await interaction.delete_original_response()
+        elif action is StopAction.DISABLE:
+            self._disable_components()
+            await interaction.response.edit_message(view=self)
+        else:
+            raise TypeError(f"unknown stop action: {action!r}")
 
     @discord.ui.button(
         emoji="\N{LEFTWARDS ARROW WITH HOOK}",
         style=discord.ButtonStyle.blurple,
         row=2,
     )
     async def back_button(
```

### Comparing `discord-ext-pager-1.0.2.post2/src/discord_ext_pager.egg-info/PKG-INFO` & `discord-ext-pager-1.1.1b0/src/discord_ext_pager.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-ext-pager
-Version: 1.0.2.post2
+Version: 1.1.1b0
 Summary: A view-based paginator library for discord.py 2.0
 Author: thegamecracks
 Project-URL: Homepage, https://github.com/thegamecracks/discord-ext-pager
 Keywords: discord,discord.py,paginator,view
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
@@ -43,35 +43,37 @@
   The base class for sources the paginator view can accept.
 - ListPageSource:
   The base class for formatting a list of items.
 - AsyncIteratorPageSource:
   The base class for formatting an asynchronous iterator of items.
 - PageOption:
   A subclass of `discord.SelectOption` used for presenting navigation options.
+- StopAction:
+  An enum for customizing PaginatorView's stop button behaviour.
 - TimeoutAction:
   An enum for customizing PaginatorView's timeout behaviour.
 
 [discord-ext-pager]: https://pypi.org/project/discord-ext-pager/
 [discord-ext-menus]: https://github.com/Rapptz/discord-ext-menus
 
 The `PaginatorView` can be instantiated and used by itself, but page formatting
 is handled by subclassing one of the `PageSource` base classes.
 
 ```py
-from typing import Any, List
-from discord.ext.pager import ListPageSource, PaginatorView
+from typing import List
+from discord.ext.pager import ListPageSource, PageSource, PaginatorView
 
-class EmbedListPageSource(ListPageSource[Any, None, PaginatorView]):
-    #                                   ^^^^^^^^^^^^^^^^^^^^^^^^^^
+class EmbedListPageSource(ListPageSource[object, PageSource, PaginatorView]):
+    #                                   ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
     #            These type parameters denote the page item type,
     #            source type for page options (demonstrated later),
     #            and view type. Only needed for static typing.
     """Takes a list of items and formats it in an embed."""
 
-    def format_page(self, view: PaginatorView, page: List[Any]):
+    def format_page(self, view: PaginatorView, page: List[object]):
         index = self.current_index * self.page_size
         description = "\n".join(
             f"{i}. {x}"
             for i, x in enumerate(page, start=index + 1)
         )
         return discord.Embed(description=description)
 
@@ -86,19 +88,19 @@
 should be overridden to return a list of `PageOption` objects for the user
 to select from:
 
 ```py
 from typing import List
 from discord.ext.pager import ListPageSource, PageOption, PageSource, PaginatorView
 
-class MessageSource(PageSource[str, None, PaginatorView]):
+class MessageSource(PageSource[str, PageSource, PaginatorView]):
     """A single page for displaying a string."""
 
-    def __init__(self, message: str, *, current_index: int = 0):
-        super().__init__(current_index=current_index)
+    def __init__(self, message: str):
+        super().__init__(current_index=0)
         self.message = message
 
     def get_page(self, index: int):
         return self.message
 
     def format_page(self, view: PaginatorView, page: str):
         # If we don't specify both content and embed, either will
```

