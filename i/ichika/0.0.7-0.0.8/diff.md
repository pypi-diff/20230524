# Comparing `tmp/ichika-0.0.7.tar.gz` & `tmp/ichika-0.0.8.tar.gz`

## Comparing `ichika-0.0.7.tar` & `ichika-0.0.8.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0      253 1970-01-01 00:00:00.000000 ichika-0.0.7/local_dependencies/pyo3-repr/Cargo.toml
--rw-r--r--   0     1001      123     4379 2023-05-23 10:09:26.000000 ichika-0.0.7/local_dependencies/pyo3-repr/src/lib.rs
--rw-r--r--   0        0        0      177 1970-01-01 00:00:00.000000 ichika-0.0.7/local_dependencies/t544_enc/Cargo.toml
--rw-r--r--   0     1001      123       19 2023-05-23 10:09:37.000000 ichika-0.0.7/local_dependencies/t544_enc/src/lib.rs
--rw-r--r--   0     1001      123       86 2023-05-23 10:09:37.000000 ichika-0.0.7/local_dependencies/t544_enc/src/t544_sign.rs
--rw-r--r--   0        0        0     1471 1970-01-01 00:00:00.000000 ichika-0.0.7/Cargo.toml
--rw-r--r--   0     1001      123     2004 2023-05-23 10:09:26.000000 ichika-0.0.7/README.md
--rw-r--r--   0     1001      123     3077 2023-05-23 10:09:26.000000 ichika-0.0.7/pyproject.toml
--rw-r--r--   0     1001      123      231 2023-05-23 10:09:26.000000 ichika-0.0.7/python/ichika/__init__.py
--rw-r--r--   0     1001      123     1052 2023-05-23 10:09:26.000000 ichika-0.0.7/python/ichika/build_info.py
--rw-r--r--   0     1001      123     7580 2023-05-23 10:09:26.000000 ichika-0.0.7/python/ichika/client.py
--rw-r--r--   0     1001      123    19186 2023-05-23 10:09:26.000000 ichika-0.0.7/python/ichika/core.pyi
--rw-r--r--   0     1001      123     4138 2023-05-23 10:09:26.000000 ichika-0.0.7/python/ichika/event_defs.py
--rw-r--r--   0     1001      123      266 2023-05-23 10:09:26.000000 ichika-0.0.7/python/ichika/exceptions.py
--rw-r--r--   0     1001      123     6253 2023-05-23 10:09:26.000000 ichika-0.0.7/python/ichika/graia/__init__.py
--rw-r--r--   0     1001      123     7214 2023-05-23 10:09:26.000000 ichika-0.0.7/python/ichika/graia/event.py
--rw-r--r--   0     1001      123     4832 2023-05-23 10:09:26.000000 ichika-0.0.7/python/ichika/login/__init__.py
--rw-r--r--   0     1001      123     3864 2023-05-23 10:09:26.000000 ichika-0.0.7/python/ichika/login/password.py
--rw-r--r--   0     1001      123     4115 2023-05-23 10:09:26.000000 ichika-0.0.7/python/ichika/login/qrcode/__init__.py
--rw-r--r--   0     1001      123      249 2023-05-23 10:09:26.000000 ichika-0.0.7/python/ichika/login/qrcode/render/__init__.py
--rw-r--r--   0     1001      123      794 2023-05-23 10:09:26.000000 ichika-0.0.7/python/ichika/login/qrcode/render/dense1x2.py
--rw-r--r--   0     1001      123     1017 2023-05-23 10:09:26.000000 ichika-0.0.7/python/ichika/message/__init__.py
--rw-r--r--   0     1001      123      290 2023-05-23 10:09:26.000000 ichika-0.0.7/python/ichika/message/_sealed.py
--rw-r--r--   0     1001      123     1935 2023-05-23 10:09:26.000000 ichika-0.0.7/python/ichika/message/_serializer.py
--rw-r--r--   0     1001      123    13966 2023-05-23 10:09:26.000000 ichika-0.0.7/python/ichika/message/elements.py
--rw-r--r--   0     1001      123        0 2023-05-23 10:09:26.000000 ichika-0.0.7/python/ichika/scripts/__init__.py
--rw-r--r--   0     1001      123     1227 2023-05-23 10:09:26.000000 ichika-0.0.7/python/ichika/scripts/device/__init__.py
--rw-r--r--   0     1001      123     1903 2023-05-23 10:09:26.000000 ichika-0.0.7/python/ichika/scripts/device/converter.py
--rw-r--r--   0     1001      123     5163 2023-05-23 10:09:26.000000 ichika-0.0.7/python/ichika/scripts/device/data.json
--rw-r--r--   0     1001      123     2305 2023-05-23 10:09:26.000000 ichika-0.0.7/python/ichika/scripts/device/generator.py
--rw-r--r--   0     1001      123      741 2023-05-23 10:09:26.000000 ichika-0.0.7/python/ichika/structs.py
--rw-r--r--   0     1001      123     1934 2023-05-23 10:09:26.000000 ichika-0.0.7/python/ichika/utils.py
--rw-r--r--   0     1001      123     1036 2023-05-23 10:09:26.000000 ichika-0.0.7/src/build_info.rs
--rw-r--r--   0     1001      123     5602 2023-05-23 10:09:26.000000 ichika-0.0.7/src/client/cached.rs
--rw-r--r--   0     1001      123     1834 2023-05-23 10:09:26.000000 ichika-0.0.7/src/client/http.rs
--rw-r--r--   0     1001      123    26119 2023-05-23 10:09:26.000000 ichika-0.0.7/src/client/mod.rs
--rw-r--r--   0     1001      123     4489 2023-05-23 10:09:26.000000 ichika-0.0.7/src/client/params.rs
--rw-r--r--   0     1001      123    10304 2023-05-23 10:09:26.000000 ichika-0.0.7/src/client/structs.rs
--rw-r--r--   0     1001      123    12632 2023-05-23 10:09:26.000000 ichika-0.0.7/src/events/converter.rs
--rw-r--r--   0     1001      123     4919 2023-05-23 10:09:26.000000 ichika-0.0.7/src/events/mod.rs
--rw-r--r--   0     1001      123     2301 2023-05-23 10:09:26.000000 ichika-0.0.7/src/exc.rs
--rw-r--r--   0     1001      123     1895 2023-05-23 10:09:26.000000 ichika-0.0.7/src/lib.rs
--rw-r--r--   0     1001      123     1779 2023-05-23 10:09:26.000000 ichika-0.0.7/src/login/connector.rs
--rw-r--r--   0     1001      123    21393 2023-05-23 10:09:26.000000 ichika-0.0.7/src/login/mod.rs
--rw-r--r--   0     1001      123     6625 2023-05-23 10:09:26.000000 ichika-0.0.7/src/loguru.rs
--rw-r--r--   0     1001      123    10122 2023-05-23 10:09:26.000000 ichika-0.0.7/src/message/convert.rs
--rw-r--r--   0     1001      123     1667 2023-05-23 10:09:26.000000 ichika-0.0.7/src/message/elements.rs
--rw-r--r--   0     1001      123       35 2023-05-23 10:09:26.000000 ichika-0.0.7/src/message/mod.rs
--rw-r--r--   0     1001      123     5649 2023-05-23 10:09:26.000000 ichika-0.0.7/src/utils.rs
--rw-r--r--   0     1001      123    57725 2023-05-23 10:10:05.000000 ichika-0.0.7/Cargo.lock
--rw-r--r--   0        0        0     3388 1970-01-01 00:00:00.000000 ichika-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      253 1970-01-01 00:00:00.000000 ichika-0.0.8/local_dependencies/pyo3-repr/Cargo.toml
+-rw-r--r--   0     1001      123     4379 2023-05-24 14:43:58.000000 ichika-0.0.8/local_dependencies/pyo3-repr/src/lib.rs
+-rw-r--r--   0        0        0      177 1970-01-01 00:00:00.000000 ichika-0.0.8/local_dependencies/t544_enc/Cargo.toml
+-rw-r--r--   0     1001      123       19 2023-05-24 14:44:06.000000 ichika-0.0.8/local_dependencies/t544_enc/src/lib.rs
+-rw-r--r--   0     1001      123       86 2023-05-24 14:44:06.000000 ichika-0.0.8/local_dependencies/t544_enc/src/t544_sign.rs
+-rw-r--r--   0        0        0     1471 1970-01-01 00:00:00.000000 ichika-0.0.8/Cargo.toml
+-rw-r--r--   0     1001      123     2004 2023-05-24 14:43:58.000000 ichika-0.0.8/README.md
+-rw-r--r--   0     1001      123     3077 2023-05-24 14:43:58.000000 ichika-0.0.8/pyproject.toml
+-rw-r--r--   0     1001      123      231 2023-05-24 14:43:58.000000 ichika-0.0.8/python/ichika/__init__.py
+-rw-r--r--   0     1001      123     1052 2023-05-24 14:43:58.000000 ichika-0.0.8/python/ichika/build_info.py
+-rw-r--r--   0     1001      123     8494 2023-05-24 14:43:58.000000 ichika-0.0.8/python/ichika/client.py
+-rw-r--r--   0     1001      123    19186 2023-05-24 14:43:58.000000 ichika-0.0.8/python/ichika/core.pyi
+-rw-r--r--   0     1001      123     4138 2023-05-24 14:43:58.000000 ichika-0.0.8/python/ichika/event_defs.py
+-rw-r--r--   0     1001      123      266 2023-05-24 14:43:58.000000 ichika-0.0.8/python/ichika/exceptions.py
+-rw-r--r--   0     1001      123     6253 2023-05-24 14:43:58.000000 ichika-0.0.8/python/ichika/graia/__init__.py
+-rw-r--r--   0     1001      123     7214 2023-05-24 14:43:58.000000 ichika-0.0.8/python/ichika/graia/event.py
+-rw-r--r--   0     1001      123     4832 2023-05-24 14:43:58.000000 ichika-0.0.8/python/ichika/login/__init__.py
+-rw-r--r--   0     1001      123     3864 2023-05-24 14:43:58.000000 ichika-0.0.8/python/ichika/login/password.py
+-rw-r--r--   0     1001      123     4115 2023-05-24 14:43:58.000000 ichika-0.0.8/python/ichika/login/qrcode/__init__.py
+-rw-r--r--   0     1001      123      249 2023-05-24 14:43:58.000000 ichika-0.0.8/python/ichika/login/qrcode/render/__init__.py
+-rw-r--r--   0     1001      123      794 2023-05-24 14:43:58.000000 ichika-0.0.8/python/ichika/login/qrcode/render/dense1x2.py
+-rw-r--r--   0     1001      123     1017 2023-05-24 14:43:58.000000 ichika-0.0.8/python/ichika/message/__init__.py
+-rw-r--r--   0     1001      123      290 2023-05-24 14:43:58.000000 ichika-0.0.8/python/ichika/message/_sealed.py
+-rw-r--r--   0     1001      123     1935 2023-05-24 14:43:58.000000 ichika-0.0.8/python/ichika/message/_serializer.py
+-rw-r--r--   0     1001      123    14317 2023-05-24 14:43:58.000000 ichika-0.0.8/python/ichika/message/elements.py
+-rw-r--r--   0     1001      123        0 2023-05-24 14:43:58.000000 ichika-0.0.8/python/ichika/scripts/__init__.py
+-rw-r--r--   0     1001      123     1227 2023-05-24 14:43:58.000000 ichika-0.0.8/python/ichika/scripts/device/__init__.py
+-rw-r--r--   0     1001      123     1903 2023-05-24 14:43:58.000000 ichika-0.0.8/python/ichika/scripts/device/converter.py
+-rw-r--r--   0     1001      123     5163 2023-05-24 14:43:58.000000 ichika-0.0.8/python/ichika/scripts/device/data.json
+-rw-r--r--   0     1001      123     2305 2023-05-24 14:43:58.000000 ichika-0.0.8/python/ichika/scripts/device/generator.py
+-rw-r--r--   0     1001      123      741 2023-05-24 14:43:58.000000 ichika-0.0.8/python/ichika/structs.py
+-rw-r--r--   0     1001      123     1934 2023-05-24 14:43:58.000000 ichika-0.0.8/python/ichika/utils.py
+-rw-r--r--   0     1001      123     1036 2023-05-24 14:43:58.000000 ichika-0.0.8/src/build_info.rs
+-rw-r--r--   0     1001      123     5602 2023-05-24 14:43:58.000000 ichika-0.0.8/src/client/cached.rs
+-rw-r--r--   0     1001      123     1834 2023-05-24 14:43:58.000000 ichika-0.0.8/src/client/http.rs
+-rw-r--r--   0     1001      123    26119 2023-05-24 14:43:58.000000 ichika-0.0.8/src/client/mod.rs
+-rw-r--r--   0     1001      123     4489 2023-05-24 14:43:58.000000 ichika-0.0.8/src/client/params.rs
+-rw-r--r--   0     1001      123    10304 2023-05-24 14:43:58.000000 ichika-0.0.8/src/client/structs.rs
+-rw-r--r--   0     1001      123    12632 2023-05-24 14:43:58.000000 ichika-0.0.8/src/events/converter.rs
+-rw-r--r--   0     1001      123     4919 2023-05-24 14:43:58.000000 ichika-0.0.8/src/events/mod.rs
+-rw-r--r--   0     1001      123     2301 2023-05-24 14:43:58.000000 ichika-0.0.8/src/exc.rs
+-rw-r--r--   0     1001      123     1895 2023-05-24 14:43:58.000000 ichika-0.0.8/src/lib.rs
+-rw-r--r--   0     1001      123     1779 2023-05-24 14:43:58.000000 ichika-0.0.8/src/login/connector.rs
+-rw-r--r--   0     1001      123    21411 2023-05-24 14:43:58.000000 ichika-0.0.8/src/login/mod.rs
+-rw-r--r--   0     1001      123     6625 2023-05-24 14:43:58.000000 ichika-0.0.8/src/loguru.rs
+-rw-r--r--   0     1001      123    10122 2023-05-24 14:43:58.000000 ichika-0.0.8/src/message/convert.rs
+-rw-r--r--   0     1001      123     1667 2023-05-24 14:43:58.000000 ichika-0.0.8/src/message/elements.rs
+-rw-r--r--   0     1001      123       35 2023-05-24 14:43:58.000000 ichika-0.0.8/src/message/mod.rs
+-rw-r--r--   0     1001      123     5649 2023-05-24 14:43:58.000000 ichika-0.0.8/src/utils.rs
+-rw-r--r--   0     1001      123    57725 2023-05-24 14:44:28.000000 ichika-0.0.8/Cargo.lock
+-rw-r--r--   0        0        0     3388 1970-01-01 00:00:00.000000 ichika-0.0.8/PKG-INFO
```

### Comparing `ichika-0.0.7/local_dependencies/pyo3-repr/src/lib.rs` & `ichika-0.0.8/local_dependencies/pyo3-repr/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ichika-0.0.7/Cargo.toml` & `ichika-0.0.8/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [package]
 name = "ichika"
 authors = ["BlueGlassBlock <blueglassblock@outlook.com>"]
-version = "0.0.7"
+version = "0.0.8"
 license = "AGPL-3.0"
 edition = "2021"
 include = [
     "/python",
     "/src",
     "Cargo.lock",
     "pyproject.toml",
```

### Comparing `ichika-0.0.7/README.md` & `ichika-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `ichika-0.0.7/pyproject.toml` & `ichika-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ichika-0.0.7/python/ichika/build_info.py` & `ichika-0.0.8/python/ichika/build_info.py`

 * *Files identical despite different names*

### Comparing `ichika-0.0.7/python/ichika/client.py` & `ichika-0.0.8/python/ichika/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """基于 `ichika.core.PlumbingClient` 封装的高层 API"""
 from __future__ import annotations
 
-from typing import Any, Awaitable, Callable, Literal, Protocol
+from typing import Any, Awaitable, Callable, Iterable, Literal, Protocol
 from weakref import WeakValueDictionary
 
 from graia.amnesia.message import Element, MessageChain
 
-from .core import PlumbingClient, RawMessageReceipt
+from .core import Friend, Group, PlumbingClient, RawMessageReceipt
 from .message import _serialize_message as _serialize_msg
 from .message.elements import (
     At,
     AtAll,
     Audio,
     Face,
     FlashImage,
@@ -37,62 +37,75 @@
         :param body: 请求体
 
         :return: 响应体
         """
         ...
 
 
+def _uin(obj: Friend | Group | int) -> int:
+    return obj if isinstance(obj, int) else obj.uin
+
+
+def _chain_coerce(msg: str | Element | MessageChain | Iterable[str | Element]) -> MessageChain:
+    if isinstance(msg, MessageChain):
+        return msg
+    if isinstance(msg, (str, Element)):
+        msg = [msg]
+    if isinstance(msg, Iterable):
+        return MessageChain([Text(e) if isinstance(e, str) else e for e in msg])
+
+
 class Client(PlumbingClient):
     """基于 [`PlumbingClient`][ichika.core.PlumbingClient] 封装的高层 API"""
 
-    async def upload_friend_image(self, uin: int, data: bytes) -> Image:
+    async def upload_friend_image(self, friend: int | Friend, data: bytes) -> Image:
         """上传好友图片
 
-        :param uin: 好友 QQ 号
+        :param friend: 好友 QQ 号或好友对象
         :param data: 图片数据
 
         :return: 图片元素
         """
-        image_dict = await super().upload_friend_image(uin, data)
+        image_dict = await super().upload_friend_image(_uin(friend), data)
         image_dict.pop("type")
         return Image(**image_dict)
 
-    async def upload_friend_audio(self, uin: int, data: bytes) -> Audio:
+    async def upload_friend_audio(self, friend: int | Friend, data: bytes) -> Audio:
         """上传好友语音
 
-        :param uin: 好友 QQ 号
+        :param friend: 好友 QQ 号或好友对象
         :param data: 语音数据，应为 SILK/AMR 编码的音频数据
 
         :return: 语音元素
         """
-        audio_dict = await super().upload_friend_audio(uin, data)
+        audio_dict = await super().upload_friend_audio(_uin(friend), data)
         audio_dict.pop("type")
         return Audio(**audio_dict)
 
-    async def upload_group_image(self, uin: int, data: bytes) -> Image:
+    async def upload_group_image(self, group: int | Group, data: bytes) -> Image:
         """上传群图片
 
-        :param uin: 群号
+        :param group: 群号或群对象
         :param data: 图片数据
 
         :return: 图片元素
         """
-        image_dict = await super().upload_group_image(uin, data)
+        image_dict = await super().upload_group_image(_uin(group), data)
         image_dict.pop("type")
         return Image(**image_dict)
 
-    async def upload_group_audio(self, uin: int, data: bytes) -> Audio:
+    async def upload_group_audio(self, group: int | Group, data: bytes) -> Audio:
         """上传群语音
 
-        :param uin: 群号
+        :param group: 群号或群对象
         :param data: 语音数据，应为 SILK/AMR 编码的音频数据
 
         :return: 语音元素
         """
-        audio_dict = await super().upload_group_audio(uin, data)
+        audio_dict = await super().upload_group_audio(_uin(group), data)
         audio_dict.pop("type")
         return Audio(**audio_dict)
 
     @classmethod
     def _parse_downloaded_fwd(cls, content: dict) -> ForwardMessage:
         if content.pop("type") == "Forward":
             content["content"] = [cls._parse_downloaded_fwd(sub) for sub in content.pop("content")]
@@ -145,24 +158,24 @@
             )
             data["content"] = _serialize_msg(content)
         else:
             data["type"] = "Forward"
             data["content"] = [await self._prepare_forward(uin, f) for f in fwd.content]
         return data
 
-    async def upload_forward_msg(self, group_uin: int, msgs: list[ForwardMessage]) -> ForwardCard:
+    async def upload_forward_msg(self, group: int | Group, msgs: list[ForwardMessage]) -> ForwardCard:
         """上传合并转发消息
 
-        :param group_uin: 用于标记的原始群号
+        :param group: 用于标记的原始群号或群对象
         :param msgs: 转发消息列表
 
         :return: 转发卡片元素
         """
         res_id, file_name, content = await super().upload_forward_msg(
-            group_uin, [await self._prepare_forward(group_uin, msg) for msg in msgs]
+            _uin(group), [await self._prepare_forward(_uin(group), msg) for msg in msgs]
         )
         return ForwardCard(res_id, file_name, content)
 
     async def _send_special_element(self, uin: int, kind: str, element: Element) -> RawMessageReceipt:
         if Audio._check(element):
             if element.raw is None:
                 uploader = self.upload_friend_audio if kind == "friend" else self.upload_group_audio
@@ -174,36 +187,44 @@
 
         if isinstance(element, MusicShare):
             sender = self.send_friend_music_share if kind == "friend" else self.send_group_music_share
             return await sender(uin, element)
 
         raise TypeError(f"无法发送元素: {element!r}")
 
-    async def send_group_message(self, uin: int, chain: MessageChain) -> RawMessageReceipt:
+    async def send_group_message(
+        self, group: int | Group, chain: str | Element | MessageChain | Iterable[str | Element]
+    ) -> RawMessageReceipt:
         """发送群消息
 
-        :param uin: 群号
+        :param group: 群号或群对象
         :param chain: 消息链
 
         :return: 消息发送凭据，可用于撤回
         """
+        uin: int = _uin(group)
+        chain = _chain_coerce(chain)
         if isinstance(validated := self._validate_chain(chain), Element):
             return await self._send_special_element(uin, "group", validated)
         for idx, elem in enumerate(chain):
             chain.content[idx] = await self._validate_mm(uin, elem, self.upload_group_image)
         return await super().send_group_message(uin, _serialize_msg(chain))
 
-    async def send_friend_message(self, uin: int, chain: MessageChain) -> RawMessageReceipt:
+    async def send_friend_message(
+        self, friend: int | Friend, chain: str | Element | MessageChain | Iterable[str | Element]
+    ) -> RawMessageReceipt:
         """发送好友消息
 
-        :param uin: 好友 QQ 号
+        :param friend: 好友 QQ 号或好友对象
         :param chain: 消息链
 
         :return: 消息发送凭据，可用于撤回
         """
+        uin: int = _uin(friend)
+        chain = _chain_coerce(chain)
         if isinstance(validated := self._validate_chain(chain), Element):
             return await self._send_special_element(uin, "friend", validated)
         for idx, elem in enumerate(chain):
             chain.content[idx] = await self._validate_mm(uin, elem, self.upload_friend_image)
         return await super().send_friend_message(uin, _serialize_msg(chain))
```

### Comparing `ichika-0.0.7/python/ichika/core.pyi` & `ichika-0.0.8/python/ichika/core.pyi`

 * *Files identical despite different names*

### Comparing `ichika-0.0.7/python/ichika/event_defs.py` & `ichika-0.0.8/python/ichika/event_defs.py`

 * *Files identical despite different names*

### Comparing `ichika-0.0.7/python/ichika/graia/__init__.py` & `ichika-0.0.8/python/ichika/graia/__init__.py`

 * *Files identical despite different names*

### Comparing `ichika-0.0.7/python/ichika/graia/event.py` & `ichika-0.0.8/python/ichika/graia/event.py`

 * *Files identical despite different names*

### Comparing `ichika-0.0.7/python/ichika/login/__init__.py` & `ichika-0.0.8/python/ichika/login/__init__.py`

 * *Files identical despite different names*

### Comparing `ichika-0.0.7/python/ichika/login/password.py` & `ichika-0.0.8/python/ichika/login/password.py`

 * *Files identical despite different names*

### Comparing `ichika-0.0.7/python/ichika/login/qrcode/__init__.py` & `ichika-0.0.8/python/ichika/login/qrcode/__init__.py`

 * *Files identical despite different names*

### Comparing `ichika-0.0.7/python/ichika/login/qrcode/render/dense1x2.py` & `ichika-0.0.8/python/ichika/login/qrcode/render/dense1x2.py`

 * *Files identical despite different names*

### Comparing `ichika-0.0.7/python/ichika/message/__init__.py` & `ichika-0.0.8/python/ichika/message/__init__.py`

 * *Files identical despite different names*

### Comparing `ichika-0.0.7/python/ichika/message/_serializer.py` & `ichika-0.0.8/python/ichika/message/_serializer.py`

 * *Files identical despite different names*

### Comparing `ichika-0.0.7/python/ichika/message/elements.py` & `ichika-0.0.8/python/ichika/message/elements.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,14 +49,18 @@
 
     参见 [#59](https://github.com/BlueGlassBlock/Ichika/issues/59)
     """
 
     def __str__(self) -> str:
         return self.display or f"@{self.target}"
 
+    @classmethod
+    def build(cls, obj: core.Member) -> At:
+        return cls(obj.uin, obj.card_name)
+
 
 @dataclass
 class AtAll(Element):
     """@全体成员元素"""
 
     def __str__(self) -> str:
         return "@全体成员"
@@ -230,14 +234,18 @@
     time: datetime
     """发送时间"""
     sender_name: str
     """发送者昵称"""
     content: MessageChain | list[ForwardMessage]
     """消息内容"""
 
+    @classmethod
+    def build(cls, sender: core.Friend | core.Member, time: datetime, content: MessageChain) -> ForwardMessage:
+        return cls(sender.uin, time, sender.card_name if isinstance(sender, core.Member) else sender.nick, content)
+
 
 @dataclass
 class RichMessage(Element):
     """卡片消息"""
 
     service_id: int
     """服务 ID"""
```

### Comparing `ichika-0.0.7/python/ichika/scripts/device/__init__.py` & `ichika-0.0.8/python/ichika/scripts/device/__init__.py`

 * *Files identical despite different names*

### Comparing `ichika-0.0.7/python/ichika/scripts/device/converter.py` & `ichika-0.0.8/python/ichika/scripts/device/converter.py`

 * *Files identical despite different names*

### Comparing `ichika-0.0.7/python/ichika/scripts/device/data.json` & `ichika-0.0.8/python/ichika/scripts/device/data.json`

 * *Files identical despite different names*

### Comparing `ichika-0.0.7/python/ichika/scripts/device/generator.py` & `ichika-0.0.8/python/ichika/scripts/device/generator.py`

 * *Files identical despite different names*

### Comparing `ichika-0.0.7/python/ichika/structs.py` & `ichika-0.0.8/python/ichika/structs.py`

 * *Files identical despite different names*

### Comparing `ichika-0.0.7/python/ichika/utils.py` & `ichika-0.0.8/python/ichika/utils.py`

 * *Files identical despite different names*

### Comparing `ichika-0.0.7/src/build_info.rs` & `ichika-0.0.8/src/build_info.rs`

 * *Files identical despite different names*

### Comparing `ichika-0.0.7/src/client/cached.rs` & `ichika-0.0.8/src/client/cached.rs`

 * *Files identical despite different names*

### Comparing `ichika-0.0.7/src/client/http.rs` & `ichika-0.0.8/src/client/http.rs`

 * *Files identical despite different names*

### Comparing `ichika-0.0.7/src/client/mod.rs` & `ichika-0.0.8/src/client/mod.rs`

 * *Files identical despite different names*

### Comparing `ichika-0.0.7/src/client/params.rs` & `ichika-0.0.8/src/client/params.rs`

 * *Files identical despite different names*

### Comparing `ichika-0.0.7/src/client/structs.rs` & `ichika-0.0.8/src/client/structs.rs`

 * *Files identical despite different names*

### Comparing `ichika-0.0.7/src/events/converter.rs` & `ichika-0.0.8/src/events/converter.rs`

 * *Files identical despite different names*

### Comparing `ichika-0.0.7/src/events/mod.rs` & `ichika-0.0.8/src/events/mod.rs`

 * *Files identical despite different names*

### Comparing `ichika-0.0.7/src/exc.rs` & `ichika-0.0.8/src/exc.rs`

 * *Files identical despite different names*

### Comparing `ichika-0.0.7/src/lib.rs` & `ichika-0.0.8/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ichika-0.0.7/src/login/connector.rs` & `ichika-0.0.8/src/login/connector.rs`

 * *Files identical despite different names*

### Comparing `ichika-0.0.7/src/login/mod.rs` & `ichika-0.0.8/src/login/mod.rs`

 * *Files 0% similar despite different names*

```diff
@@ -195,15 +195,15 @@
 fn parse_login_args<'py>(
     py: Python<'py>,
     uin: i64,
     protocol: String,
     store: &'py PyAny,
     queues: &'py PyList,
 ) -> PyResult<(Version, PyHandler, Device, TokenRW, TaskLocals)> {
-    let task_locals = TaskLocals::with_running_loop(py)?; // Necessary since retrieving task locals at handling time is already insufficient
+    let task_locals = TaskLocals::with_running_loop(py)?.copy_context(py)?; // Necessary since retrieving task locals at handling time is already insufficient
     let handler = PyHandler::new(queues.into_py(py), task_locals.clone(), uin);
 
     let get_token = partial(py).call1((store.getattr("get_token")?, uin, &protocol))?;
     let write_token = partial(py).call1((store.getattr("write_token")?, uin, &protocol))?;
 
     let device = store.getattr("get_device")?.call1((uin, &protocol))?; // JSON
     let device: Device = depythonize(device)
```

### Comparing `ichika-0.0.7/src/loguru.rs` & `ichika-0.0.8/src/loguru.rs`

 * *Files identical despite different names*

### Comparing `ichika-0.0.7/src/message/convert.rs` & `ichika-0.0.8/src/message/convert.rs`

 * *Files identical despite different names*

### Comparing `ichika-0.0.7/src/message/elements.rs` & `ichika-0.0.8/src/message/elements.rs`

 * *Files identical despite different names*

### Comparing `ichika-0.0.7/src/utils.rs` & `ichika-0.0.8/src/utils.rs`

 * *Files identical despite different names*

### Comparing `ichika-0.0.7/Cargo.lock` & `ichika-0.0.8/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -762,15 +762,15 @@
 dependencies = [
  "cxx",
  "cxx-build",
 ]
 
 [[package]]
 name = "ichika"
-version = "0.0.7"
+version = "0.0.8"
 dependencies = [
  "async-trait",
  "backon",
  "built",
  "bytes",
  "futures-util",
  "hex",
```

### Comparing `ichika-0.0.7/PKG-INFO` & `ichika-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ichika
-Version: 0.0.7
+Version: 0.0.8
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Communications
 Classifier: Programming Language :: Python :: 3
```

