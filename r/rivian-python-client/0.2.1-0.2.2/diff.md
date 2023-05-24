# Comparing `tmp/rivian-python-client-0.2.1.tar.gz` & `tmp/rivian_python_client-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rivian-python-client-0.2.1.tar", max compression
+gzip compressed data, was "rivian_python_client-0.2.2.tar", max compression
```

## Comparing `rivian-python-client-0.2.1.tar` & `rivian_python_client-0.2.2.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0      325 2023-05-03 23:40:03.784370 rivian-python-client-0.2.1/README.md
--rw-r--r--   0        0        0      555 2023-05-03 23:40:03.784370 rivian-python-client-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      102 2023-05-03 23:40:03.784370 rivian-python-client-0.2.1/src/rivian/__init__.py
--rw-r--r--   0        0        0     2888 2023-05-03 23:40:03.784370 rivian-python-client-0.2.1/src/rivian/const.py
--rw-r--r--   0        0        0      779 2023-05-03 23:40:03.784370 rivian-python-client-0.2.1/src/rivian/exceptions.py
--rw-r--r--   0        0        0    23660 2023-05-03 23:40:03.784370 rivian-python-client-0.2.1/src/rivian/rivian.py
--rw-r--r--   0        0        0     6962 2023-05-03 23:40:03.784370 rivian-python-client-0.2.1/src/rivian/ws_monitor.py
--rw-r--r--   0        0        0     1045 2023-05-03 23:40:26.163903 rivian-python-client-0.2.1/setup.py
--rw-r--r--   0        0        0      832 2023-05-03 23:40:26.164202 rivian-python-client-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      325 2023-05-24 00:28:52.005462 rivian_python_client-0.2.2/README.md
+-rw-r--r--   0        0        0      555 2023-05-24 00:28:52.005462 rivian_python_client-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      102 2023-05-24 00:28:52.005462 rivian_python_client-0.2.2/src/rivian/__init__.py
+-rw-r--r--   0        0        0     2888 2023-05-24 00:28:52.005462 rivian_python_client-0.2.2/src/rivian/const.py
+-rw-r--r--   0        0        0      779 2023-05-24 00:28:52.005462 rivian_python_client-0.2.2/src/rivian/exceptions.py
+-rw-r--r--   0        0        0    23660 2023-05-24 00:28:52.005462 rivian_python_client-0.2.2/src/rivian/rivian.py
+-rw-r--r--   0        0        0     7280 2023-05-24 00:28:52.005462 rivian_python_client-0.2.2/src/rivian/ws_monitor.py
+-rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 rivian_python_client-0.2.2/PKG-INFO
```

### Comparing `rivian-python-client-0.2.1/pyproject.toml` & `rivian_python_client-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rivian-python-client"
-version = "0.2.1"
+version = "0.2.2"
 description = "Rivian API Client (Unofficial)"
 readme = "README.md"
 authors = ["Brian Retterer <bretterer@gmail.com>"]
 license = "MIT"
 packages = [
     { include = "rivian", from = "src" },
 ]
```

### Comparing `rivian-python-client-0.2.1/src/rivian/const.py` & `rivian_python_client-0.2.2/src/rivian/const.py`

 * *Files identical despite different names*

### Comparing `rivian-python-client-0.2.1/src/rivian/exceptions.py` & `rivian_python_client-0.2.2/src/rivian/exceptions.py`

 * *Files identical despite different names*

### Comparing `rivian-python-client-0.2.1/src/rivian/rivian.py` & `rivian_python_client-0.2.2/src/rivian/rivian.py`

 * *Files identical despite different names*

### Comparing `rivian-python-client-0.2.1/src/rivian/ws_monitor.py` & `rivian_python_client-0.2.2/src/rivian/ws_monitor.py`

 * *Files 3% similar despite different names*

```diff
@@ -110,16 +110,20 @@
 
     async def _subscribe(self, _id: str, payload: dict[str, Any]) -> None:
         """Send a subscribe request."""
         await self._ws.send_json({"id": _id, "payload": payload, "type": "subscribe"})
 
     async def _resubscribe_all(self) -> None:
         """Resubscribe all subscriptions."""
-        async with async_timeout.timeout(10):
-            await self.connection_ack.wait()
+        try:
+            async with async_timeout.timeout(10):
+                await self.connection_ack.wait()
+        except asyncio.TimeoutError:
+            _LOGGER.error("A timeout occurred while attempting to resubscribe")
+            return
         for _id, (_, payload) in self._subscriptions.items():
             await self._subscribe(_id, payload)
 
     async def _receiver(self) -> None:
         """Receive a message from a web socket."""
         if not (websocket := self._ws):
             return
@@ -149,14 +153,16 @@
         self._log_message("web socket stopped")
 
     async def _monitor(self) -> None:
         """Monitor a web socket connection."""
         attempt = 0
         while not self._disconnect:
             while self.connected or not self._subscriptions:
+                if self._receiver_task.done():  # Need to restart the receiver
+                    self._receiver_task = asyncio.ensure_future(self._receiver())
                 await asyncio.sleep(1)
             if not self._disconnect:
                 try:
                     await self.new_connection()
                 except Exception as ex:  # pylint: disable=broad-except
                     self._log_message(ex, True)
                 if not self._ws or self._ws.closed:
```

### Comparing `rivian-python-client-0.2.1/PKG-INFO` & `rivian_python_client-0.2.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: rivian-python-client
-Version: 0.2.1
+Version: 0.2.2
 Summary: Rivian API Client (Unofficial)
 License: MIT
 Author: Brian Retterer
 Author-email: bretterer@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.0.0)
 Requires-Dist: yarl (>=1.6.0)
 Description-Content-Type: text/markdown
 
 # Python: Rivian API Client
 
 Currently a Work In Progress
```

