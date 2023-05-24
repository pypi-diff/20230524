# Comparing `tmp/chainlit-0.2.103.tar.gz` & `tmp/chainlit-0.2.104.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainlit-0.2.103.tar", max compression
+gzip compressed data, was "chainlit-0.2.104.tar", max compression
```

## Comparing `chainlit-0.2.103.tar` & `chainlit-0.2.104.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     2505 2023-05-24 11:39:08.538567 chainlit-0.2.103/README.md
--rw-r--r--   0        0        0    12914 2023-05-24 11:38:34.774310 chainlit-0.2.103/chainlit/__init__.py
--rw-r--r--   0        0        0       87 2023-05-24 11:38:34.774310 chainlit-0.2.103/chainlit/__main__.py
--rw-r--r--   0        0        0      765 2023-05-24 11:38:34.774310 chainlit-0.2.103/chainlit/action.py
--rw-r--r--   0        0        0     3527 2023-05-24 11:38:34.774310 chainlit-0.2.103/chainlit/cli/__init__.py
--rw-r--r--   0        0        0     4093 2023-05-24 11:38:34.778310 chainlit-0.2.103/chainlit/cli/auth.py
--rw-r--r--   0        0        0     2594 2023-05-24 11:38:34.778310 chainlit-0.2.103/chainlit/cli/deploy.py
--rw-r--r--   0        0        0      716 2023-05-24 11:38:34.778310 chainlit-0.2.103/chainlit/cli/utils.py
--rw-r--r--   0        0        0     6443 2023-05-24 11:38:34.778310 chainlit-0.2.103/chainlit/client.py
--rw-r--r--   0        0        0     6273 2023-05-24 11:38:34.778310 chainlit-0.2.103/chainlit/config.py
--rw-r--r--   0        0        0     3668 2023-05-24 11:38:34.778310 chainlit-0.2.103/chainlit/element.py
--rw-r--r--   0        0        0  2071443 2023-05-24 11:39:34.566763 chainlit-0.2.103/chainlit/frontend/dist/assets/index-489a68c3.js
--rw-r--r--   0        0        0     4317 2023-05-24 11:39:34.562763 chainlit-0.2.103/chainlit/frontend/dist/assets/index-bdffdaa0.css
--rw-r--r--   0        0        0     8889 2023-05-24 11:39:34.558763 chainlit-0.2.103/chainlit/frontend/dist/assets/logo_dark-bc7401f6.svg
--rw-r--r--   0        0        0     8891 2023-05-24 11:39:34.562763 chainlit-0.2.103/chainlit/frontend/dist/assets/logo_light-f19fc2ea.svg
--rw-r--r--   0        0        0     6455 2023-05-24 11:39:33.294753 chainlit-0.2.103/chainlit/frontend/dist/favicon.svg
--rw-r--r--   0        0        0      772 2023-05-24 11:39:34.566763 chainlit-0.2.103/chainlit/frontend/dist/index.html
--rw-r--r--   0        0        0      344 2023-05-24 11:38:34.782310 chainlit-0.2.103/chainlit/hello.py
--rw-r--r--   0        0        0        0 2023-05-24 11:38:34.782310 chainlit-0.2.103/chainlit/lc/__init__.py
--rw-r--r--   0        0        0     8077 2023-05-24 11:38:34.782310 chainlit-0.2.103/chainlit/lc/chainlit_handler.py
--rw-r--r--   0        0        0      863 2023-05-24 11:38:34.782310 chainlit-0.2.103/chainlit/lc/monkey.py
--rw-r--r--   0        0        0     5388 2023-05-24 11:38:34.782310 chainlit-0.2.103/chainlit/lc/new_monkey.py
--rw-r--r--   0        0        0     4129 2023-05-24 11:38:34.782310 chainlit-0.2.103/chainlit/lc/old_monkey.py
--rw-r--r--   0        0        0     1068 2023-05-24 11:38:34.782310 chainlit-0.2.103/chainlit/lc/utils.py
--rw-r--r--   0        0        0      398 2023-05-24 11:38:34.782310 chainlit-0.2.103/chainlit/logger.py
--rw-r--r--   0        0        0     1618 2023-05-24 11:38:34.782310 chainlit-0.2.103/chainlit/markdown.py
--rw-r--r--   0        0        0     6747 2023-05-24 11:38:34.782310 chainlit-0.2.103/chainlit/sdk.py
--rw-r--r--   0        0        0    10159 2023-05-24 11:38:34.782310 chainlit-0.2.103/chainlit/server.py
--rw-r--r--   0        0        0      813 2023-05-24 11:38:34.782310 chainlit-0.2.103/chainlit/session.py
--rw-r--r--   0        0        0     2161 2023-05-24 11:38:34.782310 chainlit-0.2.103/chainlit/telemetry.py
--rw-r--r--   0        0        0     1015 2023-05-24 11:38:34.782310 chainlit-0.2.103/chainlit/types.py
--rw-r--r--   0        0        0     1145 2023-05-24 11:38:34.782310 chainlit-0.2.103/chainlit/user_session.py
--rw-r--r--   0        0        0      196 2023-05-24 11:38:34.782310 chainlit-0.2.103/chainlit/version.py
--rw-r--r--   0        0        0     1551 2023-05-24 11:38:34.782310 chainlit-0.2.103/chainlit/watch.py
--rw-r--r--   0        0        0     1074 2023-05-24 11:38:34.782310 chainlit-0.2.103/pyproject.toml
--rw-r--r--   0        0        0     4013 1970-01-01 00:00:00.000000 chainlit-0.2.103/PKG-INFO
+-rw-r--r--   0        0        0     2505 2023-05-24 12:32:44.903319 chainlit-0.2.104/README.md
+-rw-r--r--   0        0        0    12914 2023-05-24 12:31:58.238385 chainlit-0.2.104/chainlit/__init__.py
+-rw-r--r--   0        0        0       87 2023-05-24 12:31:58.238385 chainlit-0.2.104/chainlit/__main__.py
+-rw-r--r--   0        0        0      765 2023-05-24 12:31:58.238385 chainlit-0.2.104/chainlit/action.py
+-rw-r--r--   0        0        0     3527 2023-05-24 12:31:58.238385 chainlit-0.2.104/chainlit/cli/__init__.py
+-rw-r--r--   0        0        0     4093 2023-05-24 12:31:58.238385 chainlit-0.2.104/chainlit/cli/auth.py
+-rw-r--r--   0        0        0     2594 2023-05-24 12:31:58.238385 chainlit-0.2.104/chainlit/cli/deploy.py
+-rw-r--r--   0        0        0      716 2023-05-24 12:31:58.238385 chainlit-0.2.104/chainlit/cli/utils.py
+-rw-r--r--   0        0        0     6443 2023-05-24 12:31:58.238385 chainlit-0.2.104/chainlit/client.py
+-rw-r--r--   0        0        0     6273 2023-05-24 12:31:58.238385 chainlit-0.2.104/chainlit/config.py
+-rw-r--r--   0        0        0     3703 2023-05-24 12:31:58.238385 chainlit-0.2.104/chainlit/element.py
+-rw-r--r--   0        0        0  2071443 2023-05-24 12:33:17.111949 chainlit-0.2.104/chainlit/frontend/dist/assets/index-489a68c3.js
+-rw-r--r--   0        0        0     4317 2023-05-24 12:33:17.111949 chainlit-0.2.104/chainlit/frontend/dist/assets/index-bdffdaa0.css
+-rw-r--r--   0        0        0     8889 2023-05-24 12:33:17.107949 chainlit-0.2.104/chainlit/frontend/dist/assets/logo_dark-bc7401f6.svg
+-rw-r--r--   0        0        0     8891 2023-05-24 12:33:17.111949 chainlit-0.2.104/chainlit/frontend/dist/assets/logo_light-f19fc2ea.svg
+-rw-r--r--   0        0        0     6455 2023-05-24 12:33:15.567919 chainlit-0.2.104/chainlit/frontend/dist/favicon.svg
+-rw-r--r--   0        0        0      772 2023-05-24 12:33:17.111949 chainlit-0.2.104/chainlit/frontend/dist/index.html
+-rw-r--r--   0        0        0      344 2023-05-24 12:31:58.242385 chainlit-0.2.104/chainlit/hello.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:31:58.242385 chainlit-0.2.104/chainlit/lc/__init__.py
+-rw-r--r--   0        0        0     8077 2023-05-24 12:31:58.242385 chainlit-0.2.104/chainlit/lc/chainlit_handler.py
+-rw-r--r--   0        0        0      863 2023-05-24 12:31:58.242385 chainlit-0.2.104/chainlit/lc/monkey.py
+-rw-r--r--   0        0        0     5388 2023-05-24 12:31:58.242385 chainlit-0.2.104/chainlit/lc/new_monkey.py
+-rw-r--r--   0        0        0     4129 2023-05-24 12:31:58.242385 chainlit-0.2.104/chainlit/lc/old_monkey.py
+-rw-r--r--   0        0        0     1068 2023-05-24 12:31:58.242385 chainlit-0.2.104/chainlit/lc/utils.py
+-rw-r--r--   0        0        0      398 2023-05-24 12:31:58.246386 chainlit-0.2.104/chainlit/logger.py
+-rw-r--r--   0        0        0     1618 2023-05-24 12:31:58.246386 chainlit-0.2.104/chainlit/markdown.py
+-rw-r--r--   0        0        0     6762 2023-05-24 12:31:58.246386 chainlit-0.2.104/chainlit/sdk.py
+-rw-r--r--   0        0        0    10159 2023-05-24 12:31:58.246386 chainlit-0.2.104/chainlit/server.py
+-rw-r--r--   0        0        0      813 2023-05-24 12:31:58.246386 chainlit-0.2.104/chainlit/session.py
+-rw-r--r--   0        0        0     2161 2023-05-24 12:31:58.246386 chainlit-0.2.104/chainlit/telemetry.py
+-rw-r--r--   0        0        0     1015 2023-05-24 12:31:58.246386 chainlit-0.2.104/chainlit/types.py
+-rw-r--r--   0        0        0     1145 2023-05-24 12:31:58.246386 chainlit-0.2.104/chainlit/user_session.py
+-rw-r--r--   0        0        0      196 2023-05-24 12:31:58.246386 chainlit-0.2.104/chainlit/version.py
+-rw-r--r--   0        0        0     1551 2023-05-24 12:31:58.246386 chainlit-0.2.104/chainlit/watch.py
+-rw-r--r--   0        0        0     1056 2023-05-24 12:31:58.246386 chainlit-0.2.104/pyproject.toml
+-rw-r--r--   0        0        0     3980 1970-01-01 00:00:00.000000 chainlit-0.2.104/PKG-INFO
```

### Comparing `chainlit-0.2.103/README.md` & `chainlit-0.2.104/README.md`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.103/chainlit/__init__.py` & `chainlit-0.2.104/chainlit/__init__.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.103/chainlit/action.py` & `chainlit-0.2.104/chainlit/action.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.103/chainlit/cli/__init__.py` & `chainlit-0.2.104/chainlit/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.103/chainlit/cli/auth.py` & `chainlit-0.2.104/chainlit/cli/auth.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.103/chainlit/cli/deploy.py` & `chainlit-0.2.104/chainlit/cli/deploy.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.103/chainlit/cli/utils.py` & `chainlit-0.2.104/chainlit/cli/utils.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.103/chainlit/client.py` & `chainlit-0.2.104/chainlit/client.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.103/chainlit/config.py` & `chainlit-0.2.104/chainlit/config.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.103/chainlit/element.py` & `chainlit-0.2.104/chainlit/element.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,18 +24,21 @@
 
     def before_emit(self, element: Dict) -> Dict:
         return element
 
     def send(self, for_id: str = None):
         sdk = get_sdk()
 
+        element = None
+
         # Cloud is enabled, upload the element to S3
         if sdk.client:
             element = self.persist(sdk.client, for_id)
-        else:
+
+        if not element:
             element = self.to_dict()
             if for_id:
                 element["forId"] = for_id
 
         if sdk.emit and element:
             trace_event(f"send {self.__class__.__name__}")
             element = self.before_emit(element)
```

### Comparing `chainlit-0.2.103/chainlit/frontend/dist/assets/index-489a68c3.js` & `chainlit-0.2.104/chainlit/frontend/dist/assets/index-489a68c3.js`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.103/chainlit/frontend/dist/assets/index-bdffdaa0.css` & `chainlit-0.2.104/chainlit/frontend/dist/assets/index-bdffdaa0.css`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.103/chainlit/frontend/dist/assets/logo_dark-bc7401f6.svg` & `chainlit-0.2.104/chainlit/frontend/dist/assets/logo_dark-bc7401f6.svg`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.103/chainlit/frontend/dist/assets/logo_light-f19fc2ea.svg` & `chainlit-0.2.104/chainlit/frontend/dist/assets/logo_light-f19fc2ea.svg`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.103/chainlit/frontend/dist/favicon.svg` & `chainlit-0.2.104/chainlit/frontend/dist/favicon.svg`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.103/chainlit/frontend/dist/index.html` & `chainlit-0.2.104/chainlit/frontend/dist/index.html`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.103/chainlit/lc/chainlit_handler.py` & `chainlit-0.2.104/chainlit/lc/chainlit_handler.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.103/chainlit/lc/monkey.py` & `chainlit-0.2.104/chainlit/lc/monkey.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.103/chainlit/lc/new_monkey.py` & `chainlit-0.2.104/chainlit/lc/new_monkey.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.103/chainlit/lc/old_monkey.py` & `chainlit-0.2.104/chainlit/lc/old_monkey.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.103/chainlit/lc/utils.py` & `chainlit-0.2.104/chainlit/lc/utils.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.103/chainlit/markdown.py` & `chainlit-0.2.104/chainlit/markdown.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.103/chainlit/sdk.py` & `chainlit-0.2.104/chainlit/sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,16 @@
             "isError": is_error,
             "prompt": prompt,
             "llmSettings": llm_settings,
         }
         if self.client:
             message_id = self.client.create_message(msg)
             msg["id"] = message_id
-        else:
+
+        if not "id" in msg:
             message_id = uuid.uuid4().hex
             msg["tempId"] = message_id
 
         msg["createdAt"] = current_milli_time()
 
         if end_stream:
             self.stream_end(msg)
```

### Comparing `chainlit-0.2.103/chainlit/server.py` & `chainlit-0.2.104/chainlit/server.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.103/chainlit/session.py` & `chainlit-0.2.104/chainlit/session.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.103/chainlit/telemetry.py` & `chainlit-0.2.104/chainlit/telemetry.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.103/chainlit/types.py` & `chainlit-0.2.104/chainlit/types.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.103/chainlit/user_session.py` & `chainlit-0.2.104/chainlit/user_session.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.103/chainlit/watch.py` & `chainlit-0.2.104/chainlit/watch.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.103/pyproject.toml` & `chainlit-0.2.104/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chainlit"
-version = "0.2.103"
+version = "0.2.104"
 keywords = ['LLM', 'Agents', 'gen ai', 'chat ui', 'chatbot ui', 'langchain']
 description = "A faster way to build chatbot UIs."
 authors = ["Chainlit"]
 license = "Apache-2.0 license"
 repository = "https://github.com/Chainlit/chainlit"
 readme = "README.md"
 exclude = [
@@ -32,14 +32,13 @@
 gevent = "^22.10.2"
 gevent_websocket = "^0.10.1"
 pydantic = "^1.10.6"
 python-graphql-client = "^0.4.3"
 python-dotenv = "^1.0.0"
 auth0-python = "^4.1.1"
 uptrace = "^1.18.0"
-grpcio = "1.54.2"
 typing-inspect = "0.8.0"
 typing_extensions = "4.5.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `chainlit-0.2.103/PKG-INFO` & `chainlit-0.2.104/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainlit
-Version: 0.2.103
+Version: 0.2.104
 Summary: A faster way to build chatbot UIs.
 Home-page: https://github.com/Chainlit/chainlit
 License: Apache-2.0 license
 Keywords: LLM,Agents,gen ai,chat ui,chatbot ui,langchain
 Author: Chainlit
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
@@ -17,15 +17,14 @@
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: dataclasses_json (>=0.5.7,<0.6.0)
 Requires-Dist: flask-limiter (>=3.3.0,<4.0.0)
 Requires-Dist: flask_cors (>=3.0.10,<4.0.0)
 Requires-Dist: flask_socketio (>=5.3.3,<6.0.0)
 Requires-Dist: gevent (>=22.10.2,<23.0.0)
 Requires-Dist: gevent_websocket (>=0.10.1,<0.11.0)
-Requires-Dist: grpcio (==1.54.2)
 Requires-Dist: openai (>=0.27.2,<0.28.0)
 Requires-Dist: pydantic (>=1.10.6,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: python-graphql-client (>=0.4.3,<0.5.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Requires-Dist: typing-inspect (==0.8.0)
 Requires-Dist: typing_extensions (==4.5.0)
```

