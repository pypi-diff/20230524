# Comparing `tmp/randseal-3.2.0.tar.gz` & `tmp/randseal-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "randseal-3.2.0.tar", last modified: Fri Feb 17 16:16:16 2023, max compression
+gzip compressed data, was "randseal-3.3.0.tar", last modified: Wed May 24 18:57:42 2023, max compression
```

## Comparing `randseal-3.2.0.tar` & `randseal-3.3.0.tar`

### file list

```diff
@@ -1,23 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-02-17 16:16:16.943275 randseal-3.2.0/
--rw-rw-rw-   0        0        0     1073 2023-01-28 21:24:47.000000 randseal-3.2.0/LICENCE
--rw-rw-rw-   0        0        0       65 2023-01-19 20:30:45.000000 randseal-3.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1130 2023-02-17 16:16:16.951327 randseal-3.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      667 2023-01-04 03:58:05.000000 randseal-3.2.0/README.md
--rw-rw-rw-   0        0        0      174 2023-02-01 01:27:17.000000 randseal-3.2.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-02-17 16:16:16.912588 randseal-3.2.0/randseal/
--rw-rw-rw-   0        0        0     1193 2023-01-28 21:24:27.000000 randseal-3.2.0/randseal/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-17 16:16:16.943275 randseal-3.2.0/randseal/archive/
--rw-rw-rw-   0        0        0     1135 2023-01-28 21:25:20.000000 randseal-3.2.0/randseal/archive/__init__.py
--rw-rw-rw-   0        0        0     1382 2023-02-01 16:50:42.000000 randseal-3.2.0/randseal/archive/one.py
--rw-rw-rw-   0        0        0     6484 2023-02-01 16:35:33.000000 randseal-3.2.0/randseal/client.py
--rw-rw-rw-   0        0        0      427 2023-02-17 16:14:00.000000 randseal-3.2.0/randseal/errors.py
--rw-rw-rw-   0        0        0      826 2023-01-20 21:44:49.000000 randseal-3.2.0/randseal/iters.py
--rw-rw-rw-   0        0        0      379 2023-02-01 16:34:33.000000 randseal-3.2.0/randseal/protocols.py
--rw-rw-rw-   0        0        0     2011 2023-02-01 19:27:36.000000 randseal-3.2.0/randseal/timestamp.py
--rw-rw-rw-   0        0        0      281 2023-01-31 16:40:15.000000 randseal-3.2.0/randseal/vars.py
-drwxrwxrwx   0        0        0        0 2023-02-17 16:16:16.943275 randseal-3.2.0/randseal.egg-info/
--rw-rw-rw-   0        0        0     1130 2023-02-17 16:16:16.000000 randseal-3.2.0/randseal.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      373 2023-02-17 16:16:16.000000 randseal-3.2.0/randseal.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-17 16:16:16.000000 randseal-3.2.0/randseal.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-02-17 16:16:16.000000 randseal-3.2.0/randseal.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      561 2023-02-17 16:16:16.952100 randseal-3.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-24 18:57:42.821952 randseal-3.3.0/
+-rw-rw-rw-   0        0        0     1073 2023-01-28 21:24:47.000000 randseal-3.3.0/LICENCE
+-rw-rw-rw-   0        0        0       65 2023-01-19 20:30:45.000000 randseal-3.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1129 2023-05-24 18:57:42.821952 randseal-3.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      667 2023-01-04 03:58:05.000000 randseal-3.3.0/README.md
+-rw-rw-rw-   0        0        0      159 2023-05-24 18:56:43.000000 randseal-3.3.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-24 18:57:42.797748 randseal-3.3.0/randseal/
+-rw-rw-rw-   0        0        0     1171 2023-03-09 16:58:34.000000 randseal-3.3.0/randseal/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 18:57:42.821952 randseal-3.3.0/randseal/archive/
+-rw-rw-rw-   0        0        0     1135 2023-01-28 21:25:20.000000 randseal-3.3.0/randseal/archive/__init__.py
+-rw-rw-rw-   0        0        0     1715 2023-05-24 18:16:41.000000 randseal-3.3.0/randseal/archive/one.py
+-rw-rw-rw-   0        0        0     6526 2023-05-24 18:43:14.000000 randseal-3.3.0/randseal/client.py
+-rw-rw-rw-   0        0        0      539 2023-04-26 19:56:52.000000 randseal-3.3.0/randseal/errors.py
+-rw-rw-rw-   0        0        0      639 2023-03-10 16:48:34.000000 randseal-3.3.0/randseal/timestamp.py
+-rw-rw-rw-   0        0        0      787 2023-04-26 19:52:24.000000 randseal-3.3.0/randseal/vars.py
+drwxrwxrwx   0        0        0        0 2023-05-24 18:57:42.814231 randseal-3.3.0/randseal.egg-info/
+-rw-rw-rw-   0        0        0     1129 2023-05-24 18:57:42.000000 randseal-3.3.0/randseal.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      333 2023-05-24 18:57:42.000000 randseal-3.3.0/randseal.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 18:57:42.000000 randseal-3.3.0/randseal.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-24 18:57:42.000000 randseal-3.3.0/randseal.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      560 2023-05-24 18:57:42.830982 randseal-3.3.0/setup.cfg
```

### Comparing `randseal-3.2.0/LICENCE` & `randseal-3.3.0/LICENCE`

 * *Files identical despite different names*

### Comparing `randseal-3.2.0/PKG-INFO` & `randseal-3.3.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: randseal
-Version: 3.2.0
-Summary: Generates a random seal image for discord.py or py-cord
+Version: 3.3.0
+Summary: Generates random seal images for discord.py or py-cord
 Home-page: https://github.com/mariohero24/randseal
 Author: Guard Boi
 Author-email: guard@cowbot.xyz
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `randseal-3.2.0/README.md` & `randseal-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `randseal-3.2.0/randseal/__init__.py` & `randseal-3.3.0/randseal/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,13 +18,11 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
-
 from .client import *
 from .errors import *
 from .vars import *
-from .iters import *
-from .protocols import *
+from .timestamp import *
```

### Comparing `randseal-3.2.0/randseal/archive/__init__.py` & `randseal-3.3.0/randseal/archive/__init__.py`

 * *Files identical despite different names*

### Comparing `randseal-3.2.0/randseal/archive/one.py` & `randseal-3.3.0/randseal/archive/one.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Removed features from the package"""
 
-import discord, io, random, aiohttp, asyncio, advlink
-from client import Client
+import discord, io, random, aiohttp, typing, advlink
+from client import Client as BaseClient
 
-class archiveClient(Client):
-	"""A subclass of :class:`Client`. Only features that have been reworked or removed are different."""
+class ArchiveClient(BaseClient):
+	"""A subclass of `Client`. Only features that have been reworked or removed are different."""
 	def __init__(self, session: aiohttp.ClientSession | None = None, session2: aiohttp.ClientSession | None = None):
-		super().__init__(session, session2)
+		super().__init__(session=session, session2=session2)
 
 	@property
 	def blank(self) -> discord.Colour:
 		"""A colour like an embed from discord"""
 		col = discord.Colour(0x2f3136)
 		return col
 
@@ -34,8 +34,17 @@
 		return advlink.Link(self.url, session=self.session, session2=self.session2)
 
 	@property
 	def url(self) -> str:
 		return f"https://raw.githubusercontent.com/mariohero24/randseal/fbba6657532d0b6db21c91986843a08a7ab19f26/randseal/00{self.number}.jpg"
 
 	def __str__(self):
-		return self.url
+		return self.url
+	
+	def __int__(self):
+		return int(self.number)
+	
+	def urls(self) -> typing.Iterable[str]:
+		return [f"https://raw.githubusercontent.com/mariohero24/randseal/fbba6657532d0b6db21c91986843a08a7ab19f26/randseal/00{e}.jpg" for e in range(1, 83)]
+	
+	def __iter__(self):
+		return self.urls().__iter__()
```

### Comparing `randseal-3.2.0/randseal/client.py` & `randseal-3.3.0/randseal/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,241 +1,229 @@
 """Client file"""
 
-from .iters import imgsITER
-from .protocols import AsyncFileOrPathLike, FileOrPathLike, FileLike, EmbedLike
-import aiohttp
-import aiofiles
-from datetime import datetime
+from .vars import AsyncFileOrPathLike, FileOrPathLike, File, Embed
+from aiohttp import ClientSession
+from aiofiles import open as iopen
 from io import BytesIO, TextIOWrapper
-import json
-import asyncio
-import random
-import advlink
-import time
-from .errors import StatusException, BaseException, WhatException
-from typing import overload, Literal
-from os import PathLike
-import os
+from asyncio import get_event_loop, AbstractEventLoop, iscoroutine
+from random import randrange
+from traceback import format_exception
+from json import loads, dumps, load, dump
+from typing import AsyncIterator, Iterator, Coroutine, Any
+from .errors import StatusException, BaseException, InvalidType
+from os import path
+from sys import stderr
 from aiofiles.threadpool.text import AsyncTextIOWrapper
 from .vars import MAX_NUMBER, BLANK
 
 class Client:
-	"""
-	The :class:`Client` class for this package.
+	"""The main `Client` class for this package
 
 	Parameters
-	-----------
-
-	session: :class:`aiohttp.ClientSession`
-		The main session used to obtain seal images (`auto_decompress=False`). You can input this or the package can create one.
-
-	session2: :class:`aiohttp.ClientSession`
-		The secondary session that is currently not used for anything. You can input this or the package can create one.
-
-	loop: :class:`asyncio.AbstractEventLoop`
-		The loop used for both sessions. You can input this or the package can create one.
-
-	Attributes
-	-----------
-
-	advlink: :class:`advlink.URL`
-		An :class:`advlink.URL` containing a seal image url.
-
-	url: :class:`str`
-		A simple :class:`str` containing a seal image url.
-	
-	number: :class:`str`
-		A number between 1 and `MAX_NUMBER`, used for getting a seal image by the package.
+	----------
+	session : ClientSession | None, optional
+		The session used to get images, by default None
+	session2 : ClientSession | None, optional
+		The session used to get text (unused), by default None
+	loop : AbstractEventLoop | None, optional
+		The loop used for the sessions, by default None
 	"""
-	def __init__(self, *, session: aiohttp.ClientSession | None = None, session2: aiohttp.ClientSession | None = None, loop: asyncio.AbstractEventLoop | None = None):
-		self.loop = asyncio.get_event_loop() or loop
-		self.session = aiohttp.ClientSession(
-			auto_decompress=False, loop=self.loop) or session
-		self.session2 = aiohttp.ClientSession(loop=self.loop) or session2
+	def __init__(self, *, session: ClientSession | None = None, session2: ClientSession | None = None, loop: AbstractEventLoop | None = None):
+		self.loop = (get_event_loop() if loop is None else loop)
+		self.session = (ClientSession(
+			auto_decompress=False, loop=self.loop) if session is None else session)
+		self.session2 = (ClientSession(
+			auto_decompress=False, loop=self.loop) if session2 is None else session2)
 
-	async def File(self, cls: FileLike) -> FileLike:
+	async def File(self, cls: type[File]) -> File:
 		"""
 		Returns an `File` of a seal which can be used in a message (reworked in version 3.0.0)
 
 		Parameters
 		-----------
 
-		cls: :class:`FileLike`
+		cls: `FileLIke`
 			A py-cord `File` or a discord.py `File`
 		"""
-		async with self.session.get(self.url) as r:
-			if r.status == 200:
-				hi = BytesIO(await r.read())
-				return cls(fp=hi, filename=self.number + ".jpg")
-			else:
-				await self.on_error(StatusException)
+		if cls.__name__ != "File":
+			return await self.on_error(InvalidType(cls, "File"))
+		try:
+			async with self.session.get(self.url) as r:
+				if r.status == 200:
+					hi = BytesIO(await r.read())
+					return cls(fp=hi, filename=self.number + ".jpg")
+				else:
+					return await self.on_error(StatusException())
+		except Exception as exc:
+			await self.on_error(exc)
 
-	def Embed(self, cls: EmbedLike) -> EmbedLike:
+	def Embed(self, cls: type[Embed]) -> Embed:
 		"""
 		Returns an `Embed` of a seal which can be edited or used in a message (reworked in version 3.0.0)
 
 		Parameters
 		-----------
 
-		cls: :class:`EmbedLike`
+		cls: `type[Embed]`
 			A py-cord `Embed` or a discord.py `Embed`
 		"""
+		if cls.__name__ != "Embed":
+			return self.loop.run_until_complete(self.on_error(InvalidType(cls, "Embed")))
 		return cls(colour=BLANK).set_image(url=self.url)
 
 
 	@classmethod
-	async def jsonload(cls, fp: AsyncFileOrPathLike, **kwds,) -> dict:
+	async def jsonload(cls, fp: AsyncFileOrPathLike, **loading_kwargs,) -> dict:
 		"""
 		Asynchronous `json.load()` using the `aiofiles` package (New in 1.3.0)
 		"""
 		if isinstance(fp, AsyncTextIOWrapper):
 			s = await fp.read()
 		else:
-			if not os.path.exists(fp):
-				async with aiofiles.open(fp, "w") as f:
+			if not path.exists(fp):
+				async with iopen(fp, "w") as f:
 					s = "{}"
 					await f.write(s)
 			else:
-				async with aiofiles.open(fp) as f:
+				async with iopen(fp) as f:
 					s = await f.read()
-		return json.loads(s)
+		return loads(s, **loading_kwargs)
 
 	@classmethod
 	async def jsondump(
 			cls,
 			obj: dict,
 			fp: AsyncFileOrPathLike,
-			**kwds
+			**dumping_kwargs
 	) -> None:
 		"""
 		Asynchronous `json.dump()` using the `aiofiles` package (New in 1.3.0)
 		"""
 		if isinstance(fp, AsyncTextIOWrapper):
-			e = json.dumps(obj, **kwds)
+			e = dumps(obj, **dumping_kwargs)
 			await fp.write(e)
 		else:
-			async with aiofiles.open(fp, "w") as f:
-				e = json.dumps(obj, **kwds)
+			async with iopen(fp, "w") as f:
+				e = dumps(obj, **dumping_kwargs)
 				await f.write(e)
 
 	@classmethod
 	async def jsonupdate(cls, fp: AsyncFileOrPathLike, data: dict, **dumping_kwargs) -> dict:
 		"""
-		A combination of `.jsondump` and `.jsonload` to update json files asynchronously. Returns the updated :class:`dict`.
+		A combination of `.jsondump` and `.jsonload` to update json files asynchronously. Returns the updated `dict`.
 		"""
 		e = await cls.jsonload(fp)
 		e.update(data)
 		await cls.jsondump(e, fp, **dumping_kwargs)
 		return e
 
 	@classmethod
 	def sync_jsonupdate(cls, fp: FileOrPathLike, data: dict, **dumping_kwargs) -> dict:
 		"""
 		A non-asynchronous version of `Client.jsonupdate`.
 		"""
 		if isinstance(fp, TextIOWrapper):
 			pf = fp
 		else:
-			if not os.path.exists(fp):
+			if not path.exists(fp):
 				with open(fp, "w") as f:
 					f.write("{}")
 					return {}
 			else:
 				with open(fp) as f:
 					pf = f
-		e: dict = json.load(pf)
+		e: dict = load(pf)
 		e.update(data)
-		json.dump(e, pf, **dumping_kwargs)
+		dump(e, pf, **dumping_kwargs)
 		return e
 
-	def __hash__(self) -> int:
-		return hash(self)
-
-	def __eq__(self, __o: object) -> bool:
-		return hash(self) == hash(__o)
-
-	def __ne__(self, __o: object) -> bool:
-		return not self.__eq__(__o)
-
-	@property
-	def advlink(self) -> advlink.Link:
-		"""
-		An :class:`advlink.Link` containing a seal image url
-		"""
-		return advlink.Link(self.url, session=self.session, session2=self.session2)
-
 	@property
 	def url(self) -> str:
 		"""
 		A seal image url
 		"""
 		return f"https://raw.githubusercontent.com/mariohero24/randsealimgs/main/{self.number}.jpg"
 
 
 	@property
 	def number(self) -> str:
 		"""
 		A seal number
 		"""
-		return f"{random.randrange(0, MAX_NUMBER)}"
+		return f"{randrange(0, MAX_NUMBER)}"
 
-	def __str__(self):
+	def __str__(self) -> str:
 		return self.url
 
-	def __int__(self):
+	def __int__(self) -> int:
 		return int(self.number)
+	
+	async def flatten(self) -> list[str | int | None]:
+		"""Flatten the iter into a list.
 
-	def urls(self, *, limit: int = MAX_NUMBER, url: bool=True) -> imgsITER:
-		"""
-		Returns an :class:`AsyncIterator` for every seal image.
-
-		Parameters
-		-----------
-
-		url: :class:`bool`
-			If set to ``False``, :class:`bytes` are returned instead of :class:`str`. Defaults to ``True``.
-		
-		limit: :class:`int`
-			How many seal images to return. Defaults to `MAX_NUMBER`.
+		Returns
+		-------
+		list[Any]
+			The flattened list.
+		"""
+		return [e async for e in self]
+
+	def flatten_all(self) -> list[str]:
+		return [e for e in self]
+
+	def __aiter__(self) -> AsyncIterator[str | int | None]:
+		self.anumber = 0
+		return self
+
+	async def __anext__(self) -> str | int | None:
+		if self.anumber >= MAX_NUMBER:
+			raise StopAsyncIteration
+		self.anumber += 1
+		async with self.session.get(f"https://raw.githubusercontent.com/mariohero24/randsealimgs/main/{self.anumber}.jpg") as r:
+			if r.status == 200:
+				if self.url:
+					return f"https://raw.githubusercontent.com/mariohero24/randsealimgs/main/{self.anumber}.jpg"
+				else:
+					byte = await r.read()
+					return byte
 
-		Examples
-		-----------
-		```py
-		# Using for loop
-		async for url in urls():
-			print(url)
-
-		# Flattening into a list
-		urlist = await urls().flatten()
-		print(urlist)
-		```
-		"""
-		return imgsITER(url=url, session=self.session, limit=limit)
+	def __iter__(self) -> Iterator[str]:
+		self.number = 0
+		return self
+	
+	def __next__(self) -> str:
+		if self.number >= MAX_NUMBER:
+			raise StopIteration
+		self.number += 1
+		return f"https://raw.githubusercontent.com/mariohero24/randsealimgs/main/{self.number}.jpg"
 
 	async def tobytes(self, bytesio: bool=False) -> bytes | BytesIO | None:
 		async with self.session.get(self.url) as r:
 			if r.status == 200:
 				if bytesio:
 					n = await r.read()
 					hi = BytesIO(n)
 				else:
 					hi = await r.read()
 				return hi
 			else:
-				await self.on_error(StatusException)
+				await self.on_error(StatusException(r.status))
 
-	async def on_error(self, exception: BaseException) -> None:
-		"""
-		Error handler that can be overridden via subclassing `Client`.
+	async def on_error(self, exception: Exception) -> None:
+		"""|coro|
+
+		Error handler that can be overridden via subclassing `Client`
 
 		Parameters
 		-----------
 
-		exception: :class:`BaseException`
-			The exception that was encountered. Can be determined using `isinstance(exception, {example})`.
+		exception: `Exception`
+			The exception that was encountered. Can be determined using `isinstance()`.
 		"""
-		if isinstance(exception, BaseException):
-			raise WhatException()
-		else:
-			raise exception
+		print(self.format_exception(exception), file=stderr)
+		
+
+	@classmethod
+	def format_exception(cls, exception: Exception) -> str:
+		return "".join(format_exception(exception))
 
 # python3 -m twine upload --repository pypi dist/*
```

### Comparing `randseal-3.2.0/randseal.egg-info/PKG-INFO` & `randseal-3.3.0/randseal.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: randseal
-Version: 3.2.0
-Summary: Generates a random seal image for discord.py or py-cord
+Version: 3.3.0
+Summary: Generates random seal images for discord.py or py-cord
 Home-page: https://github.com/mariohero24/randseal
 Author: Guard Boi
 Author-email: guard@cowbot.xyz
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `randseal-3.2.0/setup.cfg` & `randseal-3.3.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2072 616e 6473 6561 6c0d 0a76 6572   = randseal..ver
-00000020: 7369 6f6e 203d 2033 2e32 2e30 0d0a 6175  sion = 3.2.0..au
+00000020: 7369 6f6e 203d 2033 2e33 2e30 0d0a 6175  sion = 3.3.0..au
 00000030: 7468 6f72 203d 2047 7561 7264 2042 6f69  thor = Guard Boi
 00000040: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000050: 2067 7561 7264 4063 6f77 626f 742e 7879   guard@cowbot.xy
 00000060: 7a0d 0a64 6573 6372 6970 7469 6f6e 203d  z..description =
-00000070: 2047 656e 6572 6174 6573 2061 2072 616e   Generates a ran
-00000080: 646f 6d20 7365 616c 2069 6d61 6765 2066  dom seal image f
-00000090: 6f72 2064 6973 636f 7264 2e70 7920 6f72  or discord.py or
-000000a0: 2070 792d 636f 7264 0d0a 6c6f 6e67 5f64   py-cord..long_d
-000000b0: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
-000000c0: 653a 2052 4541 444d 452e 6d64 0d0a 6c6f  e: README.md..lo
-000000d0: 6e67 5f64 6573 6372 6970 7469 6f6e 5f63  ng_description_c
-000000e0: 6f6e 7465 6e74 5f74 7970 6520 3d20 7465  ontent_type = te
-000000f0: 7874 2f6d 6172 6b64 6f77 6e0d 0a75 726c  xt/markdown..url
-00000100: 203d 2068 7474 7073 3a2f 2f67 6974 6875   = https://githu
-00000110: 622e 636f 6d2f 6d61 7269 6f68 6572 6f32  b.com/mariohero2
-00000120: 342f 7261 6e64 7365 616c 0d0a 636c 6173  4/randseal..clas
-00000130: 7369 6669 6572 7320 3d20 0d0a 0950 726f  sifiers = ...Pro
-00000140: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000150: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000160: 0d0a 094c 6963 656e 7365 203a 3a20 4f53  ...License :: OS
-00000170: 4920 4170 7072 6f76 6564 203a 3a20 4d49  I Approved :: MI
-00000180: 5420 4c69 6365 6e73 650d 0a09 4f70 6572  T License...Oper
-00000190: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
-000001a0: 4f53 2049 6e64 6570 656e 6465 6e74 0d0a  OS Independent..
-000001b0: 0d0a 5b6f 7074 696f 6e73 5d0d 0a70 6163  ..[options]..pac
-000001c0: 6b61 6765 7320 3d20 6669 6e64 3a0d 0a70  kages = find:..p
-000001d0: 7974 686f 6e5f 7265 7175 6972 6573 203d  ython_requires =
-000001e0: 203e 3d33 2e38 0d0a 696e 636c 7564 655f   >=3.8..include_
-000001f0: 7061 636b 6167 655f 6461 7461 203d 2054  package_data = T
-00000200: 7275 650d 0a0d 0a5b 6567 675f 696e 666f  rue....[egg_info
-00000210: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
-00000220: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
-00000230: 0a                                       .
+00000070: 2047 656e 6572 6174 6573 2072 616e 646f   Generates rando
+00000080: 6d20 7365 616c 2069 6d61 6765 7320 666f  m seal images fo
+00000090: 7220 6469 7363 6f72 642e 7079 206f 7220  r discord.py or 
+000000a0: 7079 2d63 6f72 640d 0a6c 6f6e 675f 6465  py-cord..long_de
+000000b0: 7363 7269 7074 696f 6e20 3d20 6669 6c65  scription = file
+000000c0: 3a20 5245 4144 4d45 2e6d 640d 0a6c 6f6e  : README.md..lon
+000000d0: 675f 6465 7363 7269 7074 696f 6e5f 636f  g_description_co
+000000e0: 6e74 656e 745f 7479 7065 203d 2074 6578  ntent_type = tex
+000000f0: 742f 6d61 726b 646f 776e 0d0a 7572 6c20  t/markdown..url 
+00000100: 3d20 6874 7470 733a 2f2f 6769 7468 7562  = https://github
+00000110: 2e63 6f6d 2f6d 6172 696f 6865 726f 3234  .com/mariohero24
+00000120: 2f72 616e 6473 6561 6c0d 0a63 6c61 7373  /randseal..class
+00000130: 6966 6965 7273 203d 200d 0a09 5072 6f67  ifiers = ...Prog
+00000140: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000150: 203a 3a20 5079 7468 6f6e 203a 3a20 330d   :: Python :: 3.
+00000160: 0a09 4c69 6365 6e73 6520 3a3a 204f 5349  ..License :: OSI
+00000170: 2041 7070 726f 7665 6420 3a3a 204d 4954   Approved :: MIT
+00000180: 204c 6963 656e 7365 0d0a 094f 7065 7261   License...Opera
+00000190: 7469 6e67 2053 7973 7465 6d20 3a3a 204f  ting System :: O
+000001a0: 5320 496e 6465 7065 6e64 656e 740d 0a0d  S Independent...
+000001b0: 0a5b 6f70 7469 6f6e 735d 0d0a 7061 636b  .[options]..pack
+000001c0: 6167 6573 203d 2066 696e 643a 0d0a 7079  ages = find:..py
+000001d0: 7468 6f6e 5f72 6571 7569 7265 7320 3d20  thon_requires = 
+000001e0: 3e3d 332e 380d 0a69 6e63 6c75 6465 5f70  >=3.8..include_p
+000001f0: 6163 6b61 6765 5f64 6174 6120 3d20 5472  ackage_data = Tr
+00000200: 7565 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  ue....[egg_info]
+00000210: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
+00000220: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
```

