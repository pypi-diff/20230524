# Comparing `tmp/opencv_stream-0.0.9.tar.gz` & `tmp/opencv_stream-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opencv_stream-0.0.9.tar", last modified: Tue Dec 27 12:04:12 2022, max compression
+gzip compressed data, was "opencv_stream-0.1.0.tar", last modified: Tue May 23 22:09:23 2023, max compression
```

## Comparing `opencv_stream-0.0.9.tar` & `opencv_stream-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 oliverlaleau   (501) staff       (20)        0 2022-12-27 12:04:12.658231 opencv_stream-0.0.9/
--rw-r--r--   0 oliverlaleau   (501) staff       (20)     1067 2022-10-15 02:00:07.000000 opencv_stream-0.0.9/LICENSE
--rw-r--r--   0 oliverlaleau   (501) staff       (20)      877 2022-12-27 12:04:12.658100 opencv_stream-0.0.9/PKG-INFO
--rw-r--r--   0 oliverlaleau   (501) staff       (20)      133 2022-12-27 12:01:00.000000 opencv_stream-0.0.9/README.md
-drwxr-xr-x   0 oliverlaleau   (501) staff       (20)        0 2022-12-27 12:04:12.657143 opencv_stream-0.0.9/opencv_stream/
--rw-r--r--   0 oliverlaleau   (501) staff       (20)      129 2022-11-27 08:16:28.000000 opencv_stream-0.0.9/opencv_stream/__init__.py
--rw-r--r--   0 oliverlaleau   (501) staff       (20)     1181 2022-11-02 14:30:35.000000 opencv_stream-0.0.9/opencv_stream/fps_writer.py
--rw-r--r--   0 oliverlaleau   (501) staff       (20)      961 2022-11-02 14:30:25.000000 opencv_stream-0.0.9/opencv_stream/model_schema.py
--rw-r--r--   0 oliverlaleau   (501) staff       (20)     1839 2022-11-02 14:30:13.000000 opencv_stream-0.0.9/opencv_stream/option.py
--rw-r--r--   0 oliverlaleau   (501) staff       (20)      667 2022-11-02 14:30:03.000000 opencv_stream-0.0.9/opencv_stream/utils.py
--rw-r--r--   0 oliverlaleau   (501) staff       (20)     2809 2022-12-27 11:58:39.000000 opencv_stream-0.0.9/opencv_stream/video.py
-drwxr-xr-x   0 oliverlaleau   (501) staff       (20)        0 2022-12-27 12:04:12.657939 opencv_stream-0.0.9/opencv_stream.egg-info/
--rw-r--r--   0 oliverlaleau   (501) staff       (20)      877 2022-12-27 12:04:12.000000 opencv_stream-0.0.9/opencv_stream.egg-info/PKG-INFO
--rw-r--r--   0 oliverlaleau   (501) staff       (20)      364 2022-12-27 12:04:12.000000 opencv_stream-0.0.9/opencv_stream.egg-info/SOURCES.txt
--rw-r--r--   0 oliverlaleau   (501) staff       (20)        1 2022-12-27 12:04:12.000000 opencv_stream-0.0.9/opencv_stream.egg-info/dependency_links.txt
--rw-r--r--   0 oliverlaleau   (501) staff       (20)       20 2022-12-27 12:04:12.000000 opencv_stream-0.0.9/opencv_stream.egg-info/requires.txt
--rw-r--r--   0 oliverlaleau   (501) staff       (20)       14 2022-12-27 12:04:12.000000 opencv_stream-0.0.9/opencv_stream.egg-info/top_level.txt
--rw-r--r--   0 oliverlaleau   (501) staff       (20)       38 2022-12-27 12:04:12.658273 opencv_stream-0.0.9/setup.cfg
--rw-r--r--   0 oliverlaleau   (501) staff       (20)     1138 2022-12-27 12:02:51.000000 opencv_stream-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 22:09:23.664319 opencv_stream-0.1.0/
+-rw-rw-rw-   0        0        0     1067 2022-10-15 02:00:07.000000 opencv_stream-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     1337 2023-05-23 22:09:23.258573 opencv_stream-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      133 2022-12-27 12:01:00.000000 opencv_stream-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 22:09:23.245573 opencv_stream-0.1.0/opencv_stream/
+-rw-rw-rw-   0        0        0      129 2023-05-23 22:03:36.000000 opencv_stream-0.1.0/opencv_stream/__init__.py
+-rw-rw-rw-   0        0        0     1181 2022-11-02 14:30:35.000000 opencv_stream-0.1.0/opencv_stream/fps_drawer.py
+-rw-rw-rw-   0        0        0     1027 2023-05-23 20:49:36.000000 opencv_stream-0.1.0/opencv_stream/model_schema.py
+-rw-rw-rw-   0        0        0     1839 2022-11-02 14:30:13.000000 opencv_stream-0.1.0/opencv_stream/option.py
+-rw-rw-rw-   0        0        0      667 2022-11-02 14:30:03.000000 opencv_stream-0.1.0/opencv_stream/utils.py
+-rw-rw-rw-   0        0        0     3695 2023-05-23 22:05:44.000000 opencv_stream-0.1.0/opencv_stream/video.py
+drwxrwxrwx   0        0        0        0 2023-05-23 22:09:23.257571 opencv_stream-0.1.0/opencv_stream.egg-info/
+-rw-rw-rw-   0        0        0     1337 2023-05-23 22:09:23.000000 opencv_stream-0.1.0/opencv_stream.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      364 2023-05-23 22:09:23.000000 opencv_stream-0.1.0/opencv_stream.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 22:09:23.000000 opencv_stream-0.1.0/opencv_stream.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-05-23 22:09:23.000000 opencv_stream-0.1.0/opencv_stream.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-23 22:09:23.000000 opencv_stream-0.1.0/opencv_stream.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-23 22:09:23.666318 opencv_stream-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1154 2023-05-23 22:09:21.000000 opencv_stream-0.1.0/setup.py
```

### Comparing `opencv_stream-0.0.9/LICENSE` & `opencv_stream-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `opencv_stream-0.0.9/opencv_stream/fps_writer.py` & `opencv_stream-0.1.0/opencv_stream/fps_drawer.py`

 * *Files identical despite different names*

### Comparing `opencv_stream-0.0.9/opencv_stream/model_schema.py` & `opencv_stream-0.1.0/opencv_stream/model_schema.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 
+from typing import Any
 from .option import Option
 import numpy as np
+from abc import ABC, abstractmethod
 
     
         
-class Model:
+class Model(ABC):
     """
     Inherit from the class to define your model
     """
     
-    def __init__(self) -> None:
-        raise Exception("Cannot instanciate")
-    
-    def predict(self, image: np.ndarray)->Option:
+    @abstractmethod
+    def predict(self, image: np.ndarray)->"ModelOutput":
         raise NotImplementedError()
+    
+    def __call__(self, image: np.ndarray) -> Option:
+        return Option.wrap(self.predict)(image)
         
                
                
-class ModelOutput:
+class ModelOutput(ABC):
 
     """
     Inherit from this class to define your model output\n
     use the to_dict method to generate a json dictionary representation\n
     of you output. (For Apis)
 
     Use the draw function to define how the output should be drawn onto the screen
     """
-    
-    def __init__(self) -> None:
-        raise Exception("Cannot instanciate")    
-    
+
+    @abstractmethod
     def to_dict(self)->dict:
         raise NotImplementedError()           
-        
+
+    @abstractmethod    
     def draw(self, image:np.ndarray)->None:
         raise NotImplementedError()
```

### Comparing `opencv_stream-0.0.9/opencv_stream/option.py` & `opencv_stream-0.1.0/opencv_stream/option.py`

 * *Files identical despite different names*

### Comparing `opencv_stream-0.0.9/opencv_stream/utils.py` & `opencv_stream-0.1.0/opencv_stream/utils.py`

 * *Files identical despite different names*

### Comparing `opencv_stream-0.0.9/opencv_stream/video.py` & `opencv_stream-0.1.0/opencv_stream/video.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 from typing import Callable
 import cv2
 import numpy as np
 from typing import Optional
 from threading import Thread
+from queue import Queue
+
+from .fps_drawer import FpsDrawer
+
+from .model_schema import Model, ModelOutput
 
 class InvalidInputError(Exception): ...
 
 def _assert_is_type(input, expected_type:type):
 
     if not isinstance(input, expected_type):
         raise InvalidInputError(f"Expected a '{expected_type}', received '{type(input)}'")
@@ -22,16 +27,14 @@
     def __init__(self, cap, window_name="video", waitkey=1) -> None:
         
       self.__cap = cap
       self.__tasks = []
       self.__pre_tasks = []
       self.window_name = window_name
       self.waitkey = waitkey
-      self.ret = None
-      self.frame = None
 
       
     def from_webcam(cam_index:int=0,window_name:str="video", waitkey:int=1):
 
         _assert_is_type(cam_index, int)
        
         return VideoStreamer(
@@ -43,29 +46,45 @@
     def on_next_frame(self, shape:Optional[tuple[int,int]]=None):
         """
         Use as a decorator to wrap your function\n
         The cam window is drawn automatically after the function has been called.\n
         Example: \n
 
         stream =  VideoStreamer.from_webcam()
-        @stream.on_next_frame
+        @stream.on_next_frame()
         def func(image):
              ...
 
 
         """
         if not shape is None:
            self.__pre_tasks.append(lambda img: cv2.resize(img, shape, interpolation=cv2.INTER_AREA))
            
         def inner(func:Callable[[np.ndarray], None]):
             self.__tasks.append(func)  
 
         return inner    
 
-        
+
+    def start_with_model(self, model: Model, fps_drawer:Optional[FpsDrawer]=FpsDrawer()):
+
+        if fps_drawer:  
+            @self.on_next_frame()
+            def fn(image: np.ndarray):
+                output = model.predict(image) 
+                output.draw(image)
+                fps_drawer.draw(image)
+        else:
+            @self.on_next_frame()
+            def fn(image: np.ndarray):
+                output = model.predict(image) 
+                output.draw(image)
+
+        self.start()
+
     def from_video_input(path, window_name="video", waitkey=1):
 
         _assert_is_type(path, str)
 
         return VideoStreamer(
             cap=cv2.VideoCapture(path),
            window_name=window_name, 
@@ -81,28 +100,41 @@
             cv2.imshow(self.window_name, frame)
             cv2.waitKey(self.waitkey)
         
     def start(self):
         """
         Using the method to start loading the next frames
         """
-
         
+        queue = Queue()
+
         def update():
         
             while True:
-                self.ret, self.frame = self.__cap.read()
-
-        Thread(target=update).start()  
+                ret, frame = self.__cap.read()
+                if ret:
+                   queue.put(frame)
+                else: 
+                   queue.put(None)
+
+        thread = Thread(target=update)
+        thread.daemon = True
+        thread.start()  
 
         while True:
-                print(self.ret)
-                if not self.ret: continue
 
-                frame = self.frame
-                for task in self.__pre_tasks:
-                    frame = task(frame)
+            if  queue.empty(): continue
+            
+            frame = queue.get()
+            if frame is None: return self.close()
+
+            for task in self.__pre_tasks:
+                frame = task(frame)
+
+            self.__step(frame)  
 
-                self.__step(frame)  
+    def close(self):
+        self.__cap.release()
+        cv2.destroyAllWindows()            
         
     
-    
+
```

### Comparing `opencv_stream-0.0.9/setup.py` & `opencv_stream-0.1.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,29 +5,30 @@
 
 cwd = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(cwd, "README.md"), encoding="utf-8") as f:
     long_description = "\n" + f.read()
     with open("./test.py") as p:
          long_description = long_description.format(python=p.read())
-    print(long_description)     
 
-VERSION = '0.0.9'
+
+REQUIREMENTS = open("./requirements.txt").read().splitlines()
+VERSION = '0.1.0'
 DESCRIPTION = 'Wrapper over opencv for video processing and API development'
 
 setup(
     name="opencv_stream",
     version=VERSION,
     author="Olivier",
     author_email="luowensheng2018@gmail.com",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
-    install_requires=['opencv-python', 'numpy'],
+    install_requires=REQUIREMENTS,
     keywords=['python', 'video', 'stream', "AI", "API"],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

