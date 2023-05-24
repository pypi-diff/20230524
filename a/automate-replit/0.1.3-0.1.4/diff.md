# Comparing `tmp/automate_replit-0.1.3.tar.gz` & `tmp/automate_replit-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automate_replit-0.1.3.tar", max compression
+gzip compressed data, was "automate_replit-0.1.4.tar", max compression
```

## Comparing `automate_replit-0.1.3.tar` & `automate_replit-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,24 @@
--rw-r--r--   0        0        0      956 2023-02-18 00:32:46.974921 automate_replit-0.1.3/README.md
--rw-r--r--   0        0        0      148 2023-02-13 18:11:50.861892 automate_replit-0.1.3/autoreplit/__init__.py
--rw-r--r--   0        0        0      584 2023-02-17 23:08:44.861565 automate_replit-0.1.3/autoreplit/classes/comments.py
--rw-r--r--   0        0        0     2174 2023-03-27 17:19:32.655645 automate_replit-0.1.3/autoreplit/classes/notifications.py
--rw-r--r--   0        0        0     1490 2023-03-16 20:19:44.525134 automate_replit-0.1.3/autoreplit/classes/queryResult.py
--rw-r--r--   0        0        0      229 2023-02-17 23:08:44.877565 automate_replit-0.1.3/autoreplit/classes/repl.py
--rw-r--r--   0        0        0     3319 2023-03-27 13:34:48.489445 automate_replit-0.1.3/autoreplit/classes/user.py
--rw-r--r--   0        0        0     6851 2023-03-18 21:58:55.084746 automate_replit-0.1.3/autoreplit/client.py
--rw-r--r--   0        0        0       56 2023-02-12 20:23:55.925669 automate_replit-0.1.3/autoreplit/commonTyping.py
--rw-r--r--   0        0        0       73 2023-02-12 21:19:41.303390 automate_replit-0.1.3/autoreplit/gql/currentUser.gql
--rw-r--r--   0        0        0     9261 2023-02-17 17:10:00.269304 automate_replit-0.1.3/autoreplit/gql/notifications.gql
--rw-r--r--   0        0        0       83 2023-02-12 20:57:36.573261 automate_replit-0.1.3/autoreplit/gql/updatePresence.gql
--rw-r--r--   0        0        0      840 2023-03-27 13:35:23.053398 automate_replit-0.1.3/autoreplit/gql/userByUsername.gql
--rw-r--r--   0        0        0      112 2023-02-12 22:21:31.400978 automate_replit-0.1.3/autoreplit/py.typed
--rw-r--r--   0        0        0      438 2023-02-13 23:41:52.591136 automate_replit-0.1.3/autoreplit/querys.py
--rw-r--r--   0        0        0      995 2023-03-27 21:38:42.775756 automate_replit-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1759 1970-01-01 00:00:00.000000 automate_replit-0.1.3/setup.py
--rw-r--r--   0        0        0     1668 1970-01-01 00:00:00.000000 automate_replit-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      956 2023-05-23 22:05:14.417575 automate_replit-0.1.4/README.md
+-rw-r--r--   0        0        0      174 2023-05-23 22:05:14.417575 automate_replit-0.1.4/autoreplit/__init__.py
+-rw-r--r--   0        0        0     1472 2023-05-23 22:13:05.036124 automate_replit-0.1.4/autoreplit/classes/__pycache__/basic.cpython-310.pyc
+-rw-r--r--   0        0        0     2343 2023-05-24 02:01:49.764857 automate_replit-0.1.4/autoreplit/classes/__pycache__/notifications.cpython-310.pyc
+-rw-r--r--   0        0        0     1956 2023-05-23 22:13:05.036124 automate_replit-0.1.4/autoreplit/classes/__pycache__/queryResult.cpython-310.pyc
+-rw-r--r--   0        0        0     2238 2023-05-23 22:13:05.048124 automate_replit-0.1.4/autoreplit/classes/__pycache__/repl.cpython-310.pyc
+-rw-r--r--   0        0        0     3185 2023-05-23 22:13:05.032124 automate_replit-0.1.4/autoreplit/classes/__pycache__/user.cpython-310.pyc
+-rw-r--r--   0        0        0      905 2023-05-23 22:05:14.417575 automate_replit-0.1.4/autoreplit/classes/basic.py
+-rw-r--r--   0        0        0      108 2023-05-23 22:05:14.417575 automate_replit-0.1.4/autoreplit/classes/comments.py
+-rw-r--r--   0        0        0     2203 2023-05-24 02:01:45.672864 automate_replit-0.1.4/autoreplit/classes/notifications.py
+-rw-r--r--   0        0        0     1481 2023-05-23 22:05:14.417575 automate_replit-0.1.4/autoreplit/classes/queryResult.py
+-rw-r--r--   0        0        0     1738 2023-05-23 22:05:14.417575 automate_replit-0.1.4/autoreplit/classes/repl.py
+-rw-r--r--   0        0        0     3200 2023-05-23 22:05:14.417575 automate_replit-0.1.4/autoreplit/classes/user.py
+-rw-r--r--   0        0        0     9513 2023-05-24 02:01:14.656919 automate_replit-0.1.4/autoreplit/client.py
+-rw-r--r--   0        0        0       56 2023-05-23 22:05:14.421575 automate_replit-0.1.4/autoreplit/commonTyping.py
+-rw-r--r--   0        0        0       73 2023-05-23 22:05:14.421575 automate_replit-0.1.4/autoreplit/gql/currentUser.gql
+-rw-r--r--   0        0        0     9261 2023-05-23 22:05:14.421575 automate_replit-0.1.4/autoreplit/gql/notifications.gql
+-rw-r--r--   0        0        0     2572 2023-05-23 22:07:04.353378 automate_replit-0.1.4/autoreplit/gql/repl.gql
+-rw-r--r--   0        0        0       83 2023-05-23 22:05:14.421575 automate_replit-0.1.4/autoreplit/gql/updatePresence.gql
+-rw-r--r--   0        0        0      840 2023-05-23 22:05:14.421575 automate_replit-0.1.4/autoreplit/gql/userByUsername.gql
+-rw-r--r--   0        0        0      112 2023-05-23 22:05:14.421575 automate_replit-0.1.4/autoreplit/py.typed
+-rw-r--r--   0        0        0      476 2023-05-23 22:05:14.421575 automate_replit-0.1.4/autoreplit/querys.py
+-rw-r--r--   0        0        0     1223 2023-05-24 02:06:12.048394 automate_replit-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1753 1970-01-01 00:00:00.000000 automate_replit-0.1.4/PKG-INFO
```

### Comparing `automate_replit-0.1.3/README.md` & `automate_replit-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `automate_replit-0.1.3/autoreplit/classes/notifications.py` & `automate_replit-0.1.4/autoreplit/classes/notifications.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from ..commonTyping import JsonType
-from .user import SimpleUser
+from .basic import SimpleUser, BasicComment
 from .queryResult import QueryResultBase
 from typing import List, Optional, cast
 from warnings import warn
-from .comments import BasicComment
 
 
 class CommonNotif(QueryResultBase):
     """The most common stucture for notifications. Look at ``notifications.gql`` for more details."""
 
     id: str  #: Notification id
     timeCreated: str  #: Time the notification was created
@@ -23,33 +22,34 @@
 
     def __init__(self, json: JsonType) -> None:
         json["type"] = json["__typename"]
         del json["__typename"]
         super().__init__(None, json)
         if not self.creator is None:
             self.creator = SimpleUser(
-                cast(JsonType, self.creator)["username"], cast(JsonType, self.creator)["id"]
+                cast(JsonType, self.creator)["username"],
+                cast(JsonType, self.creator)["id"],
             )
         if not self.replComment is None:
             self.replComment = BasicComment(cast(JsonType, self.replComment))
 
 
 class UnidentifiedNotif(QueryResultBase):
     """Unidentified notification. Will produce a warning, please featrue request support for the unidentified type."""
 
     def __init__(self, json: JsonType) -> None:
         json["type"] = json["__typename"]
         del json["__typename"]
         super().__init__(None, json)
 
 
-def makeNotification(json: JsonType) -> List[QueryResultBase]:
+def makeNotification(json: JsonType) -> List[CommonNotif | UnidentifiedNotif]:
     """Sort and type notif's."""
     data = json["data"]["notifications"]["items"]
-    result: List[QueryResultBase] = []
+    result: List[CommonNotif | UnidentifiedNotif] = []
     for item in data:
         match item["__typename"]:
             case "ReplCommentCreatedNotification" | "ReplCommentReplyCreatedNotification" | "ReplCommentMentionNotification" | "NewFollowerNotification":
                 result.append(CommonNotif(item))
             case _:
                 warn(f"Unwrapped and Unidentified notif {item['__typename']}")
                 result.append(UnidentifiedNotif(item))
```

### Comparing `automate_replit-0.1.3/autoreplit/classes/queryResult.py` & `automate_replit-0.1.4/autoreplit/classes/queryResult.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,8 +45,7 @@
         # Tmp-fix, reduntant
         if not opname is None:
             data = json["data"][opname]
         else:
             data = json
         self.__slots__ = data.keys()
         super().__init__(opname, json)
-
```

### Comparing `automate_replit-0.1.3/autoreplit/classes/user.py` & `automate_replit-0.1.4/autoreplit/classes/user.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from dataclasses import dataclass
 from ..commonTyping import JsonType
 from .queryResult import QueryResultBase
-from .repl import BasicRepl
+from .basic import BasicRepl
 from typing import Dict, List, Optional
 
 
 @dataclass
 class Social:
     """Social contact object, like ``"github"``"""
 
@@ -20,22 +20,14 @@
 
     id: str
     name: str
     key: str
     tagline: str
 
 
-@dataclass
-class SimpleUser:
-    """A simple user object, provides username and id."""
-
-    username: str
-    id: str
-
-
 class User(QueryResultBase):
     """The user object. Contains user data."""
 
     id: int  #: User's id
     username: str  #: User's username
     image: str  #: User's pfp
     url: str  #: Path to the users profile
@@ -83,15 +75,15 @@
 
     __slots__ = locals()["__annotations__"].keys()
 
     def __makePublicRepls(self):
         pr = self.publicRepls
         self.publicRepls = []
         for item in pr["items"]:
-            self.publicRepls.append(BasicRepl(item["id"], item["title"], item["url"]))
+            self.publicRepls.append(BasicRepl(item["id"], item["url"], item["title"]))
 
     def __makePresenceStatus(self):
         for k, v in self.presenceStatus.items():
             self.__setattr__(k, v)
         self.presenceStatus = None
 
     def __makeRoles(self):
```

### Comparing `automate_replit-0.1.3/autoreplit/client.py` & `automate_replit-0.1.4/autoreplit/client.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,45 @@
 import asyncio, aiohttp, aiolimiter
 from .querys import querys
-from .classes.user import User, SimpleUser
-from .classes.queryResult import QueryResult, QueryResultBase
-from .classes.notifications import makeNotification
+from .classes.user import User
+from .classes.basic import SimpleUser
+from .classes.queryResult import QueryResult
+from .classes.notifications import makeNotification, UnidentifiedNotif, CommonNotif
+from .classes.repl import Repl
 from dataclasses import dataclass
+import traceback
+
 # Typing
 from types import CoroutineType
 from .commonTyping import JsonType
-from typing import Optional, Dict, Any, List
+from typing import Optional, Dict, Any, List, Callable
+from functools import wraps
+
 
 @dataclass
 class CachedRequest:
     """A cached request for better preformance."""
+
     fut: asyncio.Future
     json: JsonType
 
+
 class RequestError(Exception):
     """Replit api request error."""
 
     pass
 
+def requiresSid(f: Callable) -> Callable:
+    """Decorator to make a function require a sid to run."""
+    @wraps(f)
+    def inner(self, *args, **kwargs: Any) -> Any:
+        if self.sid is None:
+            raise ValueError("This method requries a sid in the client.")
+        return f(self, *args, **kwargs)
+    return inner
 
 class ReplitClient:
     """The replit client object.
     This class is the centerpiece or the library,
     almost all of the functions are of this class.
     This should be the only object you need to import.
 
@@ -52,52 +68,79 @@
             "sec-fetch-mode": "cors",
             "sec-fetch-site": "same-origin",
             "sec-gpc": "1",
             "x-requested-with": "XMLHttpRequest",
         }
         self.limiter = aiolimiter.AsyncLimiter(5, 1)  # Current rate-limit is 5/s
         self.requestCache: List[CachedRequest] = []
+        # self.activeRequestCalls: int = 0
 
     async def __clearCache(self) -> None:
         """Clear the cache and request data in groups of 5"""
         amount = min(5, len(self.requestCache))
         session = self.client
         rqs = self.requestCache[:amount]
-        del self.requestCache[:amount]
         if len(rqs) == 0:
             return
         # print("Emptying cached objects")
         rjson = [rq.json for rq in rqs]
         async with session.post(
             "https://replit.com/graphql", json=rjson, headers=self.headers
         ) as response:
+            # print("Request made")
             if response.status != 200:
-                raise RequestError(await response.text())  # Raise request errors
+                errText = await response.text()
+                for rq in rqs:
+                    # print("Resolving errored hash (L93)", hash(rq.fut))
+
+                    rq.fut.set_exception(
+                        RequestError(errText)
+                    )  # Raise request errors for the batch
+                    # assert rq.fut.done()
+                    self.requestCache.remove(rq)
+                # print("Futures Errored")
+                # del self.requestCache[:amount]
+                return
+
             json = await response.json()
+            # print("Json parsed")
             # print("Packed and requested:", len(json), ". Futures left:", len(self.requestCache))
             for result, rq in zip(json, rqs):
+                if not rq in self.requestCache[:amount]:
+                    continue
                 if "errors" in result:  # Raise other errors
-                    rq.fut.set_exception(RequestError(result["errors"]["message"]))
+                    # print(result["errors"])
+                    # print("Resolving errored hash (L110)", hash(rq.fut))
+
+                    rq.fut.set_exception(RequestError(result["errors"][0]["message"]))
+                    # print(rq.fut.done())
                 else:
+                    # print("Resolving hash (L115)", hash(rq.fut))
+
                     rq.fut.set_result(result)
+                # assert self.requestCache.find(rq.fut).done()
+                self.requestCache.remove(rq)
+
+            # del self.requestCache[:amount]
 
     async def __request(self) -> bool:
         """Request a cache clearing, returns false if the request was dissmissed."""
         # print("Request: Awaiting limiter", self.limiter.has_capacity())
         if len(self.requestCache) < 1:
             # print("Request Dismissed")
             return False
         await self.limiter.acquire()
         # print("Limiter aquired")
         if len(self.requestCache) > 0:
             # print("Clearing cache")
             await self.__clearCache()
+
             return True
+
         return False
-            
 
     async def start(self) -> None:
         """Start the client, needs to be used first, before any other functions.
 
         .. warning::
            Never use with :meth:`autoreplit.ReplitClient.run`
         """
@@ -124,30 +167,47 @@
             try:
                 await mainfunc
             finally:
                 await self.close()
 
         asyncio.run(inner())
 
+    def __checkTask(self, task):
+        task.remove_done_callback(self.__checkTask)
+        exc = task.exception()
+        if exc is not None:
+            amount = min(5, len(self.requestCache))
+            rqs = self.requestCache[:amount]
+            for rq in rqs:
+
+                err = RequestError("Failed to send end request: \n" + "".join(traceback.format_exception(exc)))
+                # print("Resolving errored hash ", hash(rq.fut))
+                rq.fut.set_exception(err)
+                self.requestCache.remove(rq)
+            raise exc
+        # print("Task ended, current futures left: ", len(self.requestCache))
+
     def __gqlQuery(
         self, query: str, vars: JsonType, opname: Optional[str] = None
     ) -> asyncio.Future[JsonType]:
         # Query replit graphql
         json: Dict[str, Any] = {}
         if opname != None:
             json["operationName"] = opname
         json = {"query": query, "variables": vars}
-        
+
         loop = asyncio.get_running_loop()
         fut = loop.create_future()
         self.requestCache.append(CachedRequest(fut, json))
         # print("Added to cache, now requesting")
-        loop.create_task(self.__request())
+        # print("Task created")
+        task = loop.create_task(self.__request())
+        task.add_done_callback(self.__checkTask)
+        # await self.__request()
         return fut
-        
 
     async def rawQuery(
         self, queryname: str, query: str, vars: JsonType = {}
     ) -> QueryResult:
         """Use a raw gql query on the api. Returns a QueryResult object.
 
         :param queryname: The name of the query, for example ``UserByUsername``
@@ -160,27 +220,42 @@
 
     async def getUserByName(self, name: str) -> User:
         """Get a user by name. Returns an user object."""
         query = querys["userByUsername"]
         result = await self.__gqlQuery(query, {"username": name}, "userByUsername")
         return User(result)
 
+    @requiresSid
     async def getCurrentUser(self) -> SimpleUser:
         """Get the current user. Returns a ``SimpleUser``"""
         query = querys["currentUser"]
         result = await self.__gqlQuery(query, {}, "UpgradeModal")
         result = result["data"]["currentUser"]
         return SimpleUser(result["username"], result["id"])
 
+    @requiresSid
     async def updatePresence(self) -> None:
         """Update your bot's presence, will set you to ``Online``"""
         query = querys["updatePresence"]
         await self.__gqlQuery(query, {}, "SitePresenceUpdate")
 
+
+    async def getReplById(self, id: str) -> Repl:
+        query = querys["repl"]
+        result = await self.__gqlQuery(query, {"id": id}, "repl")
+        return Repl(result)
+
+    async def getReplByUrl(self, url: str) -> Repl:
+        query = querys["repl"]
+        result = await self.__gqlQuery(query, {"url": url}, "repl")
+        return Repl(result)
+
+    @requiresSid
     async def getNotifications(
         self, count: int = 10, seen: bool = False
-    ) -> List[QueryResultBase]:
+    ) -> List[CommonNotif | UnidentifiedNotif]:
+        """Get ``count`` amount of notifications for the current user."""
         query = querys["notifications"]
         result = await self.__gqlQuery(
             query, {"count": count, "seen": seen}, "notifications"
         )
         return makeNotification(result)
```

### Comparing `automate_replit-0.1.3/autoreplit/gql/notifications.gql` & `automate_replit-0.1.4/autoreplit/gql/notifications.gql`

 * *Files identical despite different names*

### Comparing `automate_replit-0.1.3/autoreplit/gql/userByUsername.gql` & `automate_replit-0.1.4/autoreplit/gql/userByUsername.gql`

 * *Files identical despite different names*

### Comparing `automate_replit-0.1.3/pyproject.toml` & `automate_replit-0.1.4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,47 @@
 [tool.poetry]
 name = "automate-replit"
-version = "0.1.3"
+version = "0.1.4"
 description = "Automate your replit account using this replit api wrapper!"
 authors = ["thatrandomperson5"]
 packages = [
-    { include = "autoreplit" },
+    { include = "autoreplit" }
 ] 
 readme = "README.md"
 include = ["autoreplit/gql/*.gql"]
 repository = "https://github.com/thatrandomperson5/automate-replit"
 homepage = "https://github.com/thatrandomperson5/automate-replit"
 documentation = "http://automate-replit.rtfd.io/"
 keywords = ["replit", "async", "asyncio", "aiohttp", "api", "api-wrapper"]
 
+[tool.poetry.scripts]
+schema-gen = "autoreplit.schemagen:main"
+
 [tool.poetry.dependencies]
 python = "^3.10.0"
 aiohttp = "^3.8.3"
-aiolimiter = "1.0.0"
+aiolimiter = ">=1.0.0"
+
+graphql-py =  { version = ">=0.8.1", optional = true }
+
+
+
+[tool.poetry.extras]
+schemagen = ["graphql-py"]
 
 [tool.poetry.dev-dependencies]
 debugpy = "^1.6.2"
 black = "^23.1.0"
 replit-python-lsp-server = {extras = ["yapf", "rope", "pyflakes"], version = "^1.5.9"}
 mypy = "^1.0.0"
 pytest = "^7.2.1"
 pytest-mypy = "^0.10.3"
 
+[tool.poetry.group.dev.dependencies]
+poetry = "^1.5.0"
+
 [tool.pytest.ini_options]
 filterwarnings = ["ignore::DeprecationWarning"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `automate_replit-0.1.3/PKG-INFO` & `automate_replit-0.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: automate-replit
-Version: 0.1.3
+Version: 0.1.4
 Summary: Automate your replit account using this replit api wrapper!
 Home-page: https://github.com/thatrandomperson5/automate-replit
 Keywords: replit,async,asyncio,aiohttp,api,api-wrapper
 Author: thatrandomperson5
 Requires-Python: >=3.10.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: schemagen
 Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
-Requires-Dist: aiolimiter (==1.0.0)
+Requires-Dist: aiolimiter (>=1.0.0)
+Requires-Dist: graphql-py (>=0.8.1) ; extra == "schemagen"
 Project-URL: Documentation, http://automate-replit.rtfd.io/
 Project-URL: Repository, https://github.com/thatrandomperson5/automate-replit
 Description-Content-Type: text/markdown
 
 # Automate Replit
 [![Documentation Status](https://readthedocs.org/projects/automate-replit/badge/?version=latest)](https://automate-replit.readthedocs.io/en/latest/?badge=latest)
```

