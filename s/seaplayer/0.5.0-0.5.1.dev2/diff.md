# Comparing `tmp/seaplayer-0.5.0.tar.gz` & `tmp/seaplayer-0.5.1.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seaplayer-0.5.0.tar", max compression
+gzip compressed data, was "seaplayer-0.5.1.dev2.tar", max compression
```

## Comparing `seaplayer-0.5.0.tar` & `seaplayer-0.5.1.dev2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     1064 2023-05-22 09:27:56.937522 seaplayer-0.5.0/LICENSE
--rw-r--r--   0        0        0     1304 2023-05-22 09:27:56.937522 seaplayer-0.5.0/README.md
--rw-r--r--   0        0        0     1445 2023-05-22 12:14:42.150487 seaplayer-0.5.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-22 09:27:56.937522 seaplayer-0.5.0/seaplayer/__init__.py
--rw-r--r--   0        0        0      331 2023-05-22 09:27:56.937522 seaplayer-0.5.0/seaplayer/__main__.py
--rw-r--r--   0        0        0    14705 2023-05-22 09:27:56.937522 seaplayer-0.5.0/seaplayer/assets/image-not-found.png
--rw-r--r--   0        0        0     2351 2023-05-22 09:27:56.937522 seaplayer-0.5.0/seaplayer/codecs/Any.py
--rw-r--r--   0        0        0      459 2023-05-22 09:27:56.940856 seaplayer-0.5.0/seaplayer/codecs/FLAC.py
--rw-r--r--   0        0        0     2732 2023-05-22 09:27:56.940856 seaplayer-0.5.0/seaplayer/codecs/MIDI.py
--rw-r--r--   0        0        0      455 2023-05-22 09:27:56.940856 seaplayer-0.5.0/seaplayer/codecs/MP3.py
--rw-r--r--   0        0        0      457 2023-05-22 09:27:56.940856 seaplayer-0.5.0/seaplayer/codecs/OGG.py
--rw-r--r--   0        0        0      574 2023-05-22 09:27:56.940856 seaplayer-0.5.0/seaplayer/codecs/WAV.py
--rw-r--r--   0        0        0      134 2023-05-22 09:27:56.940856 seaplayer-0.5.0/seaplayer/codecs/__init__.py
--rw-r--r--   0        0        0     1859 2023-05-22 09:27:56.940856 seaplayer-0.5.0/seaplayer/codeсbase.py
--rw-r--r--   0        0        0     5700 2023-05-22 09:27:56.940856 seaplayer-0.5.0/seaplayer/config.py
--rw-r--r--   0        0        0        0 2023-05-22 09:27:56.940856 seaplayer-0.5.0/seaplayer/css/configurate.css
--rw-r--r--   0        0        0     1491 2023-05-22 09:27:56.940856 seaplayer-0.5.0/seaplayer/css/objects.css
--rw-r--r--   0        0        0      555 2023-05-22 09:27:56.940856 seaplayer-0.5.0/seaplayer/css/seaplayer.css
--rw-r--r--   0        0        0      260 2023-05-22 09:27:56.940856 seaplayer-0.5.0/seaplayer/css/unknown.css
--rw-r--r--   0        0        0      374 2023-05-22 09:27:56.940856 seaplayer-0.5.0/seaplayer/exceptions.py
--rw-r--r--   0        0        0     1367 2023-05-22 09:27:56.940856 seaplayer-0.5.0/seaplayer/functions.py
--rw-r--r--   0        0        0        0 2023-05-22 09:27:56.940856 seaplayer-0.5.0/seaplayer/modules/__init__.py
--rw-r--r--   0        0        0     1975 2023-05-22 09:27:56.940856 seaplayer-0.5.0/seaplayer/modules/colorizer.py
--rw-r--r--   0        0        0      868 2023-05-22 09:27:56.940856 seaplayer-0.5.0/seaplayer/objects/Configurate.py
--rw-r--r--   0        0        0     2938 2023-05-22 09:27:56.940856 seaplayer-0.5.0/seaplayer/objects/Image.py
--rw-r--r--   0        0        0     1094 2023-05-22 09:27:56.940856 seaplayer-0.5.0/seaplayer/objects/Input.py
--rw-r--r--   0        0        0      950 2023-05-22 09:27:56.940856 seaplayer-0.5.0/seaplayer/objects/Log.py
--rw-r--r--   0        0        0     5430 2023-05-22 09:27:56.940856 seaplayer-0.5.0/seaplayer/objects/MusicList.py
--rw-r--r--   0        0        0      759 2023-05-22 09:27:56.940856 seaplayer-0.5.0/seaplayer/objects/Notification.py
--rw-r--r--   0        0        0     1240 2023-05-22 09:27:56.940856 seaplayer-0.5.0/seaplayer/objects/ProgressBar.py
--rw-r--r--   0        0        0      316 2023-05-22 09:27:56.940856 seaplayer-0.5.0/seaplayer/objects/__init__.py
--rw-r--r--   0        0        0       85 2023-05-22 09:37:07.994732 seaplayer-0.5.0/seaplayer/plug/__init__.py
--rw-r--r--   0        0        0      547 2023-05-22 11:43:33.516175 seaplayer-0.5.0/seaplayer/plug/pluginbase.py
--rw-r--r--   0        0        0      730 2023-05-22 11:43:57.779447 seaplayer-0.5.0/seaplayer/plug/pluginbase.pyi
--rw-r--r--   0        0        0     6978 2023-05-22 11:53:22.805667 seaplayer-0.5.0/seaplayer/plug/pluginloader.py
--rw-r--r--   0        0        0     2100 2023-05-22 11:41:34.889889 seaplayer-0.5.0/seaplayer/plug/pluginloader.pyi
--rw-r--r--   0        0        0     5729 2023-05-22 09:27:56.940856 seaplayer-0.5.0/seaplayer/screens/Configurate.py
--rw-r--r--   0        0        0      982 2023-05-22 09:27:56.940856 seaplayer-0.5.0/seaplayer/screens/Unknown.py
--rw-r--r--   0        0        0       83 2023-05-22 09:27:56.940856 seaplayer-0.5.0/seaplayer/screens/__init__.py
--rw-r--r--   0        0        0    19012 2023-05-22 12:12:29.419425 seaplayer-0.5.0/seaplayer/seaplayer.py
--rw-r--r--   0        0        0     2547 2023-05-22 09:27:56.940856 seaplayer-0.5.0/seaplayer/types/Convert.py
--rw-r--r--   0        0        0     1553 2023-05-22 09:27:56.940856 seaplayer-0.5.0/seaplayer/types/MusicList.py
--rw-r--r--   0        0        0       63 2023-05-22 09:27:56.940856 seaplayer-0.5.0/seaplayer/types/__init__.py
--rw-r--r--   0        0        0     1402 2023-05-22 12:14:15.214859 seaplayer-0.5.0/seaplayer/units.py
--rw-r--r--   0        0        0     2800 1970-01-01 00:00:00.000000 seaplayer-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/LICENSE
+-rw-r--r--   0        0        0     1304 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/README.md
+-rw-r--r--   0        0        0     1450 2023-05-24 20:48:50.932426 seaplayer-0.5.1.dev2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/__init__.py
+-rw-r--r--   0        0        0      331 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/__main__.py
+-rw-r--r--   0        0        0    14705 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/assets/image-not-found.png
+-rw-r--r--   0        0        0     2415 2023-05-24 19:25:42.492196 seaplayer-0.5.1.dev2/seaplayer/codecs/Any.py
+-rw-r--r--   0        0        0      459 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/codecs/FLAC.py
+-rw-r--r--   0        0        0     2860 2023-05-24 19:26:44.687111 seaplayer-0.5.1.dev2/seaplayer/codecs/MIDI.py
+-rw-r--r--   0        0        0      455 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/codecs/MP3.py
+-rw-r--r--   0        0        0      457 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/codecs/OGG.py
+-rw-r--r--   0        0        0      574 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/codecs/WAV.py
+-rw-r--r--   0        0        0      254 2023-05-24 15:00:37.735912 seaplayer-0.5.1.dev2/seaplayer/codecs/__init__.py
+-rw-r--r--   0        0        0     1859 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/codeсbase.py
+-rw-r--r--   0        0        0     6031 2023-05-24 19:05:33.708654 seaplayer-0.5.1.dev2/seaplayer/config.py
+-rw-r--r--   0        0        0        0 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/css/configurate.css
+-rw-r--r--   0        0        0     1491 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/css/objects.css
+-rw-r--r--   0        0        0      555 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/css/seaplayer.css
+-rw-r--r--   0        0        0      260 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/css/unknown.css
+-rw-r--r--   0        0        0      374 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/exceptions.py
+-rw-r--r--   0        0        0     1367 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/functions.py
+-rw-r--r--   0        0        0        0 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/modules/__init__.py
+-rw-r--r--   0        0        0     1975 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/modules/colorizer.py
+-rw-r--r--   0        0        0     1022 2023-05-24 15:31:52.607550 seaplayer-0.5.1.dev2/seaplayer/objects/Configurate.py
+-rw-r--r--   0        0        0     2938 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/objects/Image.py
+-rw-r--r--   0        0        0     1094 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/objects/Input.py
+-rw-r--r--   0        0        0      950 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/objects/Log.py
+-rw-r--r--   0        0        0     5430 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/objects/MusicList.py
+-rw-r--r--   0        0        0      759 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/objects/Notification.py
+-rw-r--r--   0        0        0     1240 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/objects/ProgressBar.py
+-rw-r--r--   0        0        0      316 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/objects/__init__.py
+-rw-r--r--   0        0        0       85 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/plug/__init__.py
+-rw-r--r--   0        0        0      547 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/plug/pluginbase.py
+-rw-r--r--   0        0        0      730 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/plug/pluginbase.pyi
+-rw-r--r--   0        0        0     6978 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/plug/pluginloader.py
+-rw-r--r--   0        0        0     2100 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/plug/pluginloader.pyi
+-rw-r--r--   0        0        0     9316 2023-05-24 20:38:01.064915 seaplayer-0.5.1.dev2/seaplayer/screens/Configurate.py
+-rw-r--r--   0        0        0      982 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/screens/Unknown.py
+-rw-r--r--   0        0        0       83 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/screens/__init__.py
+-rw-r--r--   0        0        0    18891 2023-05-24 20:28:20.713484 seaplayer-0.5.1.dev2/seaplayer/seaplayer.py
+-rw-r--r--   0        0        0     2547 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/types/Convert.py
+-rw-r--r--   0        0        0     1553 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/types/MusicList.py
+-rw-r--r--   0        0        0       63 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/types/__init__.py
+-rw-r--r--   0        0        0     1407 2023-05-24 20:49:18.523757 seaplayer-0.5.1.dev2/seaplayer/units.py
+-rw-r--r--   0        0        0     2653 1970-01-01 00:00:00.000000 seaplayer-0.5.1.dev2/PKG-INFO
```

### Comparing `seaplayer-0.5.0/LICENSE` & `seaplayer-0.5.1.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.0/README.md` & `seaplayer-0.5.1.dev2/README.md`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.0/pyproject.toml` & `seaplayer-0.5.1.dev2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "SeaPlayer"
-version = "0.5.0"
+version = "0.5.1.dev2"
 description = "SeaPlayer is a player that works in the terminal."
 repository = "https://github.com/romanin-rf/SeaPlayer"
 authors = ["Romanin <semina054@gmail.com>"]
 keywords = ["tui", "player", "seaplayer", "wav", "mp3", "ogg", "midi"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
```

### Comparing `seaplayer-0.5.0/seaplayer/assets/image-not-found.png` & `seaplayer-0.5.1.dev2/seaplayer/assets/image-not-found.png`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.0/seaplayer/codecs/Any.py` & `seaplayer-0.5.1.dev2/seaplayer/codecs/Any.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 from ..codeсbase import CodecBase
 
 
 class AnyCodec(CodecBase):
     codec_name: str = "Any"
     
     # ! Initialized
-    def __init__(self, path: str, **kwargs) -> None:
+    def __init__(self, path: str, sound_device_id: Optional[int]=None, **kwargs) -> None:
         self.name = os.path.abspath(path)
-        self._sound = Sound(self.name)
+        self._sound = Sound(self.name, device_id=sound_device_id)
     
     def __sha1__(self, buffer_size: int) -> str:
         sha1 = hashlib.sha1()
         with open(self.name, "rb") as file:
             while True:
                 data = file.read(buffer_size)
                 if not data: break
```

### Comparing `seaplayer-0.5.0/seaplayer/codecs/MIDI.py` & `seaplayer-0.5.1.dev2/seaplayer/codecs/MIDI.py`

 * *Files 17% similar despite different names*

```diff
@@ -71,17 +71,17 @@
     
     @staticmethod
     async def aio_is_this_codec(path: str) -> bool:
         async with aiofiles.open(path, 'rb') as file:
             return await file.read(4) == b"MThd"
     
     # ! Initialized
-    def __init__(self, path: str, aio_init: bool=False, **kwargs) -> None:
+    def __init__(self, path: str, aio_init: bool=False, sound_device_id: Optional[int]=None, **kwargs) -> None:
         self.name = os.path.abspath(path)
         if not aio_init:
-            self._sound = MIDISound.from_midi(self.name, **kwargs)
+            self._sound = MIDISound.from_midi(self.name, device_id=sound_device_id, **kwargs)
     
     @staticmethod
-    async def __aio_init__(path: str, **kwargs):
+    async def __aio_init__(path: str, sound_device_id: Optional[int]=None, **kwargs):
         self = MIDICodec(path, aio_init=True)
-        self._sound = await MIDISound.aio_from_midi(self.name, **kwargs)
+        self._sound = await MIDISound.aio_from_midi(self.name, device_id=sound_device_id, **kwargs)
         return self
```

### Comparing `seaplayer-0.5.0/seaplayer/codecs/WAV.py` & `seaplayer-0.5.1.dev2/seaplayer/codecs/WAV.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.0/seaplayer/codeсbase.py` & `seaplayer-0.5.1.dev2/seaplayer/codeсbase.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.0/seaplayer/config.py` & `seaplayer-0.5.1.dev2/seaplayer/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Dict, Any, Optional, TypeVar, Union, Literal
 
 T = TypeVar("T")
 
 DEFAULT_CONFIG_DATA = {
     "sound": {
         "sound_font_path": None,                # * Optional[str]
+        "output_sound_device_id": None,         # * Optional[int]
     },
     "image": {
         "image_update_method": "sync",          # * Literal["sync", "async"]
         "image_resample_method": "bilinear",    # * Literal["nearest", "bilinear", "bicubic", "lanczos", "hamming", "box"]
     },
     "playback": {
         "volume_change_percent": 0.05,
@@ -79,14 +80,19 @@
     
     # ! Sound
     @property
     def sound_font_path(self) -> Optional[str]: return self.get("sound.sound_font_path")
     @sound_font_path.setter
     def sound_font_path(self, value: Optional[str]): self.set("sound.sound_font_path", value)
     
+    @property
+    def output_sound_device_id(self) -> Optional[int]: return self.get("sound.output_sound_device_id")
+    @output_sound_device_id.setter
+    def output_sound_device_id(self, value: Optional[int]): self.set("sound.output_sound_device_id", value)
+    
     # ! Image
     @property
     def image_update_method(self) -> Literal["sync", "async"]: return self.get("image.image_update_method")
     @image_update_method.setter
     def image_update_method(self, value: Literal["sync", "async"]): self.set("image.image_update_method", value)
     
     @property
```

### Comparing `seaplayer-0.5.0/seaplayer/css/objects.css` & `seaplayer-0.5.1.dev2/seaplayer/css/objects.css`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.0/seaplayer/css/seaplayer.css` & `seaplayer-0.5.1.dev2/seaplayer/css/seaplayer.css`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.0/seaplayer/functions.py` & `seaplayer-0.5.1.dev2/seaplayer/functions.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.0/seaplayer/modules/colorizer.py` & `seaplayer-0.5.1.dev2/seaplayer/modules/colorizer.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.0/seaplayer/objects/Configurate.py` & `seaplayer-0.5.1.dev2/seaplayer/objects/Configurate.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 from textual.containers import ScrollableContainer, Container
 # > Typing
-from typing import Optional
+from typing import Optional, Union
 
 
 class ConfigurateListItem(Container):
     def __init__(
         self,
         *children,
         title: str="",
         desc: str="",
+        width: Union[int, str]="1fr",
+        height: Union[int, str]="1fr",
         **kwargs
     ):
         kwargs["classes"] = "configurate-list-view-item"
         super().__init__(*children, **kwargs)
         self.border_title = title
         self.border_subtitle = desc
+        self.styles.width = width
+        self.styles.height = height
     
     async def updating(self, title: Optional[str]="", desc: Optional[str]="") -> None:
         if title is not None: self.border_title = title
         if desc is not None: self.border_subtitle = desc
 
 class ConfigurateList(ScrollableContainer):
     def __init__(self, *children, **kwargs):
```

### Comparing `seaplayer-0.5.0/seaplayer/objects/Image.py` & `seaplayer-0.5.1.dev2/seaplayer/objects/Image.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.0/seaplayer/objects/Input.py` & `seaplayer-0.5.1.dev2/seaplayer/objects/Input.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.0/seaplayer/objects/Log.py` & `seaplayer-0.5.1.dev2/seaplayer/objects/Log.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.0/seaplayer/objects/MusicList.py` & `seaplayer-0.5.1.dev2/seaplayer/objects/MusicList.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.0/seaplayer/objects/Notification.py` & `seaplayer-0.5.1.dev2/seaplayer/objects/Notification.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.0/seaplayer/objects/ProgressBar.py` & `seaplayer-0.5.1.dev2/seaplayer/objects/ProgressBar.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.0/seaplayer/plug/pluginbase.py` & `seaplayer-0.5.1.dev2/seaplayer/plug/pluginbase.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.0/seaplayer/plug/pluginbase.pyi` & `seaplayer-0.5.1.dev2/seaplayer/plug/pluginbase.pyi`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.0/seaplayer/plug/pluginloader.py` & `seaplayer-0.5.1.dev2/seaplayer/plug/pluginloader.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.0/seaplayer/plug/pluginloader.pyi` & `seaplayer-0.5.1.dev2/seaplayer/plug/pluginloader.pyi`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.0/seaplayer/screens/Unknown.py` & `seaplayer-0.5.1.dev2/seaplayer/screens/Unknown.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.0/seaplayer/seaplayer.py` & `seaplayer-0.5.1.dev2/seaplayer/seaplayer.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # > Typing
 from typing import Optional, Literal, Tuple, List, Type
 # > Local Imports
 from .config import *
 from .plug import PluginLoader
 from .codeсbase import CodecBase
 from .screens import Unknown, Configurate, UNKNOWN_OPEN_KEY
-from .codecs import MP3Codec, WAVECodec, OGGCodec, MIDICodec, FLACCodec
+from .codecs import codecs
 from .functions import (
     aiter,
     check_status,
     rich_exception,
     image_from_bytes,
     get_sound_basename
 )
@@ -42,17 +42,15 @@
     __email__,
     __url__,
     CSS_LOCALDIR,
     CONFIG_FILEPATH,
     ASSETS_DIRPATH,
     IMGPATH_IMAGE_NOT_FOUND,
     RESAMPLING_SAFE,
-    LOCALDIR,
-    PLUGINS_CONFIG_PATH,
-    PLUGINS_DIRPATH
+    LOCALDIR
 )
 
 # ! Main Functions
 def build_bindings(config: SeaPlayerConfig):
     yield Binding(config.key_quit, "quit", "Quit")
     yield Binding("c,с", "push_screen('configurate')", "Configurate")
     if config.log_menu_enable:
@@ -93,16 +91,19 @@
     last_playback_status: Optional[Literal["Stoped", "Playing", "Paused"]] = None
     playback_mode: int = 0
     playback_mode_blocked: bool = False
     last_paths_globalized: List[str] = []
     started: bool = True
     
     # ! Codecs Configuration
-    CODECS: List[Type[CodecBase]] = [ MP3Codec, WAVECodec, OGGCodec, MIDICodec, FLACCodec ]
-    CODECS_KWARGS: Dict[str, Any] = {"sound_fonts_path": config.sound_font_path}
+    CODECS: List[Type[CodecBase]] = [ *codecs ]
+    CODECS_KWARGS: Dict[str, Any] = {
+        "sound_fonts_path": config.sound_font_path,
+        "sound_device_id": config.output_sound_device_id
+    }
     
     # ! Init Objects
     log_menu = LogMenu(enable_logging=config.log_menu_enable, wrap=True, highlight=True, markup=True)
     
     # ! Log Functions
     info = log_menu.info
     error = log_menu.error
@@ -207,22 +208,22 @@
                 
                 self.last_playback_status = status
             await asyncio.sleep(0.2)
     
     def compose(self) -> ComposeResult:     
         # * Other
         self.info(f"{__title__} v{__version__} from {__author__} ({__email__})")
-        self.info(f"Source              : {__url__}")
-        self.info(f"Codecs              : {repr(self.CODECS)}")
-        self.info(f"Config Path         : {repr(self.config.filepath)}")
-        self.info(f"CSS Dirpath         : {repr(CSS_LOCALDIR)}")
-        self.info(f"Assets Dirpath      : {repr(ASSETS_DIRPATH)}")
-        self.info(f"Codecs Kwargs       : {repr(self.CODECS_KWARGS)}")
-        self.info(f"Plugins Dirpath     : {repr(PLUGINS_DIRPATH)}")
-        self.info(f"Plugins Config Path : {repr(PLUGINS_CONFIG_PATH)}")
+        self.info(f"Source          : {__url__}")
+        self.info(f"Codecs          : {repr(self.CODECS)}")
+        self.info(f"Config Path     : {repr(self.config.filepath)}")
+        self.info(f"CSS Dirpath     : {repr(CSS_LOCALDIR)}")
+        self.info(f"Assets Dirpath  : {repr(ASSETS_DIRPATH)}")
+        self.info(f"Codecs Kwargs   : {repr(self.CODECS_KWARGS)}")
+        self.info(f"Sound Device ID : {repr(self.config.output_sound_device_id)}")
+        self.info(f"")
         
         # * Play Screen
         self.music_play_screen = Static(classes="screen-box")
         self.music_play_screen.border_title = "Player"
         
         # * Image Object Init
         self.music_selected_label = Label(self.get_sound_selected_label_text(), classes="music-selected-label")
```

### Comparing `seaplayer-0.5.0/seaplayer/types/Convert.py` & `seaplayer-0.5.1.dev2/seaplayer/types/Convert.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.0/seaplayer/types/MusicList.py` & `seaplayer-0.5.1.dev2/seaplayer/types/MusicList.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.0/seaplayer/units.py` & `seaplayer-0.5.1.dev2/seaplayer/units.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 from platformdirs import user_config_dir
 # > Image Works
 from PIL.Image import Resampling
 
 # ! Metadata
 __title__ = "SeaPlayer"
-__version__ = "0.5.0"
+__version__ = "0.5.1.dev2"
 __author__ = "Romanin"
 __email__ = "semina054@gmail.com"
 __url__ = "https://github.com/romanin-rf/SeaPlayer"
 
 # ! Paths
 if getattr(sys, 'frozen', False) and hasattr(sys, '_MEIPASS'):
     LOCALDIR = os.path.dirname(sys.executable)
```

### Comparing `seaplayer-0.5.0/PKG-INFO` & `seaplayer-0.5.1.dev2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seaplayer
-Version: 0.5.0
+Version: 0.5.1.dev2
 Summary: SeaPlayer is a player that works in the terminal.
 Home-page: https://github.com/romanin-rf/SeaPlayer
 License: MIT
 Keywords: tui,player,seaplayer,wav,mp3,ogg,midi
 Author: Romanin
 Author-email: semina054@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -14,17 +14,14 @@
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: aiofiles (>=23.1.0,<24.0.0)
 Requires-Dist: mutagen (==1.45.1)
 Requires-Dist: pillow (>=9.5.0,<10.0.0)
 Requires-Dist: platformdirs (>=3.5.1,<4.0.0)
 Requires-Dist: playsoundsimple-py (==0.7.0)
 Requires-Dist: properties-py (==1.1.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
```

