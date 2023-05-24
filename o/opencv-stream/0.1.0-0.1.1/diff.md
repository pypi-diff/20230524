# Comparing `tmp/opencv_stream-0.1.0.tar.gz` & `tmp/opencv_stream-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opencv_stream-0.1.0.tar", last modified: Tue May 23 22:09:23 2023, max compression
+gzip compressed data, was "opencv_stream-0.1.1.tar", last modified: Wed May 24 02:02:56 2023, max compression
```

## Comparing `opencv_stream-0.1.0.tar` & `opencv_stream-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 22:09:23.664319 opencv_stream-0.1.0/
--rw-rw-rw-   0        0        0     1067 2022-10-15 02:00:07.000000 opencv_stream-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     1337 2023-05-23 22:09:23.258573 opencv_stream-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      133 2022-12-27 12:01:00.000000 opencv_stream-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-23 22:09:23.245573 opencv_stream-0.1.0/opencv_stream/
--rw-rw-rw-   0        0        0      129 2023-05-23 22:03:36.000000 opencv_stream-0.1.0/opencv_stream/__init__.py
--rw-rw-rw-   0        0        0     1181 2022-11-02 14:30:35.000000 opencv_stream-0.1.0/opencv_stream/fps_drawer.py
--rw-rw-rw-   0        0        0     1027 2023-05-23 20:49:36.000000 opencv_stream-0.1.0/opencv_stream/model_schema.py
--rw-rw-rw-   0        0        0     1839 2022-11-02 14:30:13.000000 opencv_stream-0.1.0/opencv_stream/option.py
--rw-rw-rw-   0        0        0      667 2022-11-02 14:30:03.000000 opencv_stream-0.1.0/opencv_stream/utils.py
--rw-rw-rw-   0        0        0     3695 2023-05-23 22:05:44.000000 opencv_stream-0.1.0/opencv_stream/video.py
-drwxrwxrwx   0        0        0        0 2023-05-23 22:09:23.257571 opencv_stream-0.1.0/opencv_stream.egg-info/
--rw-rw-rw-   0        0        0     1337 2023-05-23 22:09:23.000000 opencv_stream-0.1.0/opencv_stream.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      364 2023-05-23 22:09:23.000000 opencv_stream-0.1.0/opencv_stream.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 22:09:23.000000 opencv_stream-0.1.0/opencv_stream.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-05-23 22:09:23.000000 opencv_stream-0.1.0/opencv_stream.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-23 22:09:23.000000 opencv_stream-0.1.0/opencv_stream.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-23 22:09:23.666318 opencv_stream-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1154 2023-05-23 22:09:21.000000 opencv_stream-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 02:02:56.112247 opencv_stream-0.1.1/
+-rw-rw-rw-   0        0        0     1067 2022-10-15 02:00:07.000000 opencv_stream-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     1337 2023-05-24 02:02:56.111248 opencv_stream-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      133 2022-12-27 12:01:00.000000 opencv_stream-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-24 02:02:56.099250 opencv_stream-0.1.1/opencv_stream/
+-rw-rw-rw-   0        0        0      129 2023-05-23 22:03:36.000000 opencv_stream-0.1.1/opencv_stream/__init__.py
+-rw-rw-rw-   0        0        0     1181 2022-11-02 14:30:35.000000 opencv_stream-0.1.1/opencv_stream/fps_drawer.py
+-rw-rw-rw-   0        0        0     1027 2023-05-23 20:49:36.000000 opencv_stream-0.1.1/opencv_stream/model_schema.py
+-rw-rw-rw-   0        0        0     1839 2022-11-02 14:30:13.000000 opencv_stream-0.1.1/opencv_stream/option.py
+-rw-rw-rw-   0        0        0      667 2022-11-02 14:30:03.000000 opencv_stream-0.1.1/opencv_stream/utils.py
+-rw-rw-rw-   0        0        0     5470 2023-05-24 02:02:35.000000 opencv_stream-0.1.1/opencv_stream/video.py
+drwxrwxrwx   0        0        0        0 2023-05-24 02:02:56.111248 opencv_stream-0.1.1/opencv_stream.egg-info/
+-rw-rw-rw-   0        0        0     1337 2023-05-24 02:02:56.000000 opencv_stream-0.1.1/opencv_stream.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      364 2023-05-24 02:02:56.000000 opencv_stream-0.1.1/opencv_stream.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 02:02:56.000000 opencv_stream-0.1.1/opencv_stream.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-05-24 02:02:56.000000 opencv_stream-0.1.1/opencv_stream.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-24 02:02:56.000000 opencv_stream-0.1.1/opencv_stream.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-24 02:02:56.112247 opencv_stream-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1154 2023-05-24 02:02:47.000000 opencv_stream-0.1.1/setup.py
```

### Comparing `opencv_stream-0.1.0/LICENSE` & `opencv_stream-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `opencv_stream-0.1.0/PKG-INFO` & `opencv_stream-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencv_stream
-Version: 0.1.0
+Version: 0.1.1
 Summary: Wrapper over opencv for video processing and API development
 Author: Olivier
 Author-email: luowensheng2018@gmail.com
 Keywords: python,video,stream,AI,API
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `opencv_stream-0.1.0/opencv_stream/fps_drawer.py` & `opencv_stream-0.1.1/opencv_stream/fps_drawer.py`

 * *Files identical despite different names*

### Comparing `opencv_stream-0.1.0/opencv_stream/model_schema.py` & `opencv_stream-0.1.1/opencv_stream/model_schema.py`

 * *Files identical despite different names*

### Comparing `opencv_stream-0.1.0/opencv_stream/option.py` & `opencv_stream-0.1.1/opencv_stream/option.py`

 * *Files identical despite different names*

### Comparing `opencv_stream-0.1.0/opencv_stream/utils.py` & `opencv_stream-0.1.1/opencv_stream/utils.py`

 * *Files identical despite different names*

### Comparing `opencv_stream-0.1.0/opencv_stream/video.py` & `opencv_stream-0.1.1/opencv_stream/video.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,84 @@
-from typing import Callable
+from typing import Callable, Protocol
 import cv2
 import numpy as np
 from typing import Optional
 from threading import Thread
 from queue import Queue
-
+import os
 from .fps_drawer import FpsDrawer
 
 from .model_schema import Model, ModelOutput
 
 class InvalidInputError(Exception): ...
 
 def _assert_is_type(input, expected_type:type):
 
     if not isinstance(input, expected_type):
         raise InvalidInputError(f"Expected a '{expected_type}', received '{type(input)}'")
 
+class VideoStream(Protocol):
+    """
+    Interface to generate a stream of images
+
+    def read(self)->tuple[bool, Optional[np.ndarray]]:
+        TODO: Add your logic
+
+    def release(self):
+        TODO: Add your logic
+    """
+    def read(self)->tuple[bool, Optional[np.ndarray]]:
+        pass
+
+    def release(self):
+        pass
+
+
+class ImageFolderStream:
+    def __init__(self, dir_path:str, exts:set[str], repeat:bool=True) -> None:
+        
+        if not os.path.isdir(dir_path):
+            raise Exception(f"{dir_path} is not a directory")
+        
+        self.__repeat = repeat
+        self.__index = 0
+        self.__paths = []
+        
+        for path in os.listdir(dir_path):
+            _, ext = path.split(".")
+            if not ext in exts:
+                continue  
+            full_path = os.path.join(dir_path, path) 
+            self.__paths.append(full_path)
+
+        self.__max_index = len(self.__paths) -1
+
+
+    def read(self)->tuple[bool, np.ndarray]:
+        if self.__index == self.__max_index:
+            if not self.__repeat:
+                return False, None
+            else:
+                self.__index = 0
+        image = cv2.imread(self.__paths[self.__index])
+        self.__index += 1 
+        return True, image     
+
+    def release(self):
+        self.__index = self.__max_index
+        self.__repeat = False
 
 class VideoStreamer:
     """
     Use this class the read videos from path or from webcam
     Use the on_next_frame method as a decorator to wrap  
 
     """
 
-    def __init__(self, cap, window_name="video", waitkey=1) -> None:
+    def __init__(self, cap: VideoStream, window_name="video", waitkey=1) -> None:
         
       self.__cap = cap
       self.__tasks = []
       self.__pre_tasks = []
       self.window_name = window_name
       self.waitkey = waitkey
 
@@ -38,15 +88,24 @@
         _assert_is_type(cam_index, int)
        
         return VideoStreamer(
            cap = cv2.VideoCapture(cam_index),
            window_name=window_name, 
            waitkey=waitkey 
        )
+    
+    def from_folder(path: str, exts=["jpg", "jpeg", "png"], repeat:bool=True, window_name:str="video", waitkey:int=1):
+
+        _assert_is_type(path, str)
        
+        return VideoStreamer(
+           cap = ImageFolderStream(path, exts, repeat=repeat),
+           window_name=window_name, 
+           waitkey=waitkey 
+       )   
     def on_next_frame(self, shape:Optional[tuple[int,int]]=None):
         """
         Use as a decorator to wrap your function\n
         The cam window is drawn automatically after the function has been called.\n
         Example: \n
 
         stream =  VideoStreamer.from_webcam()
```

### Comparing `opencv_stream-0.1.0/opencv_stream.egg-info/PKG-INFO` & `opencv_stream-0.1.1/opencv_stream.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencv-stream
-Version: 0.1.0
+Version: 0.1.1
 Summary: Wrapper over opencv for video processing and API development
 Author: Olivier
 Author-email: luowensheng2018@gmail.com
 Keywords: python,video,stream,AI,API
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `opencv_stream-0.1.0/setup.py` & `opencv_stream-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 with codecs.open(os.path.join(cwd, "README.md"), encoding="utf-8") as f:
     long_description = "\n" + f.read()
     with open("./test.py") as p:
          long_description = long_description.format(python=p.read())
 
 
 REQUIREMENTS = open("./requirements.txt").read().splitlines()
-VERSION = '0.1.0'
+VERSION = '0.1.1'
 DESCRIPTION = 'Wrapper over opencv for video processing and API development'
 
 setup(
     name="opencv_stream",
     version=VERSION,
     author="Olivier",
     author_email="luowensheng2018@gmail.com",
```

