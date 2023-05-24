# Comparing `tmp/easyaiapi-0.0.2.tar.gz` & `tmp/easyaiapi-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyaiapi-0.0.2.tar", last modified: Tue Mar  7 05:07:57 2023, max compression
+gzip compressed data, was "easyaiapi-0.0.3.tar", last modified: Wed May 24 03:09:54 2023, max compression
```

## Comparing `easyaiapi-0.0.2.tar` & `easyaiapi-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-03-07 05:07:57.819632 easyaiapi-0.0.2/
--rw-rw-rw-   0        0        0     1067 2022-12-08 13:08:48.000000 easyaiapi-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      837 2023-03-07 05:07:57.816627 easyaiapi-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      298 2023-02-13 09:33:09.000000 easyaiapi-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-03-07 05:07:57.798627 easyaiapi-0.0.2/easyaiapi/
--rw-rw-rw-   0        0        0       98 2023-02-09 09:38:40.000000 easyaiapi-0.0.2/easyaiapi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-07 05:07:57.809627 easyaiapi-0.0.2/easyaiapi/client/
--rw-rw-rw-   0        0        0     1679 2023-03-07 03:34:03.000000 easyaiapi-0.0.2/easyaiapi/client/__init__.py
--rw-rw-rw-   0        0        0      828 2023-03-07 03:33:48.000000 easyaiapi-0.0.2/easyaiapi/client/source.py
--rw-rw-rw-   0        0        0     2212 2023-03-07 03:33:04.000000 easyaiapi-0.0.2/easyaiapi/model_endpoint.py
-drwxrwxrwx   0        0        0        0 2023-03-07 05:07:57.815625 easyaiapi-0.0.2/easyaiapi/server/
--rw-rw-rw-   0        0        0       26 2022-10-12 07:46:36.000000 easyaiapi-0.0.2/easyaiapi/server/__init__.py
--rw-rw-rw-   0        0        0     5116 2023-03-07 03:32:30.000000 easyaiapi-0.0.2/easyaiapi/server/wss.py
--rw-rw-rw-   0        0        0     1389 2023-03-07 03:33:29.000000 easyaiapi-0.0.2/easyaiapi/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-07 05:07:57.803627 easyaiapi-0.0.2/easyaiapi.egg-info/
--rw-rw-rw-   0        0        0      837 2023-03-07 05:07:57.000000 easyaiapi-0.0.2/easyaiapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      368 2023-03-07 05:07:57.000000 easyaiapi-0.0.2/easyaiapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-07 05:07:57.000000 easyaiapi-0.0.2/easyaiapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-03-07 05:07:57.000000 easyaiapi-0.0.2/easyaiapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-03-07 05:07:57.000000 easyaiapi-0.0.2/easyaiapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-07 05:07:57.819632 easyaiapi-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1031 2023-03-07 03:47:33.000000 easyaiapi-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 03:09:54.651690 easyaiapi-0.0.3/
+-rw-rw-rw-   0        0        0     1067 2022-12-08 13:08:48.000000 easyaiapi-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      837 2023-05-24 03:09:54.650289 easyaiapi-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      298 2023-02-13 09:33:09.000000 easyaiapi-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-24 03:09:54.619501 easyaiapi-0.0.3/easyaiapi/
+-rw-rw-rw-   0        0        0       98 2023-02-09 09:38:40.000000 easyaiapi-0.0.3/easyaiapi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 03:09:54.642288 easyaiapi-0.0.3/easyaiapi/client/
+-rw-rw-rw-   0        0        0     1679 2023-03-07 03:34:03.000000 easyaiapi-0.0.3/easyaiapi/client/__init__.py
+-rw-rw-rw-   0        0        0      830 2023-05-24 03:07:21.000000 easyaiapi-0.0.3/easyaiapi/client/source.py
+-rw-rw-rw-   0        0        0     2212 2023-03-07 03:33:04.000000 easyaiapi-0.0.3/easyaiapi/model_endpoint.py
+drwxrwxrwx   0        0        0        0 2023-05-24 03:09:54.649287 easyaiapi-0.0.3/easyaiapi/server/
+-rw-rw-rw-   0        0        0       26 2022-10-12 07:46:36.000000 easyaiapi-0.0.3/easyaiapi/server/__init__.py
+-rw-rw-rw-   0        0        0     5031 2023-05-24 03:09:21.000000 easyaiapi-0.0.3/easyaiapi/server/wss.py
+-rw-rw-rw-   0        0        0     1389 2023-03-07 03:33:29.000000 easyaiapi-0.0.3/easyaiapi/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-24 03:09:54.636287 easyaiapi-0.0.3/easyaiapi.egg-info/
+-rw-rw-rw-   0        0        0      837 2023-05-24 03:09:54.000000 easyaiapi-0.0.3/easyaiapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      368 2023-05-24 03:09:54.000000 easyaiapi-0.0.3/easyaiapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 03:09:54.000000 easyaiapi-0.0.3/easyaiapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-05-24 03:09:54.000000 easyaiapi-0.0.3/easyaiapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-24 03:09:54.000000 easyaiapi-0.0.3/easyaiapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-24 03:09:54.651690 easyaiapi-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1031 2023-05-24 03:06:48.000000 easyaiapi-0.0.3/setup.py
```

### Comparing `easyaiapi-0.0.2/LICENSE` & `easyaiapi-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `easyaiapi-0.0.2/PKG-INFO` & `easyaiapi-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyaiapi
-Version: 0.0.2
+Version: 0.0.3
 Summary: Easy ai api
 Author: Olivier
 Author-email: luowensheng2018@gmail.com
 Keywords: python,api,websocket,AI
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `easyaiapi-0.0.2/easyaiapi/client/__init__.py` & `easyaiapi-0.0.3/easyaiapi/client/__init__.py`

 * *Files identical despite different names*

### Comparing `easyaiapi-0.0.2/easyaiapi/client/source.py` & `easyaiapi-0.0.3/easyaiapi/client/source.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 class Video:
     
     def __init__(self, path:str, shape=None, show_video=True, window_name=None) -> None:
         self.path = path
         self.shape = shape
         self.show_video = show_video
-        self.window_name = self.path or "webcam"
+        self.window_name = window_name or "webcam"
         self.pre_process = lambda img: img if self.shape is None else cv2.resize(img, self.shape, interpolation=cv2.INTER_AREA)
         self.__load_video()
 
     def __load_video(self):    
         self.vid = cv2.VideoCapture(self.path)
 
     def read(self):
```

### Comparing `easyaiapi-0.0.2/easyaiapi/model_endpoint.py` & `easyaiapi-0.0.3/easyaiapi/model_endpoint.py`

 * *Files identical despite different names*

### Comparing `easyaiapi-0.0.2/easyaiapi/server/wss.py` & `easyaiapi-0.0.3/easyaiapi/server/wss.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
     def stream(self, endpoint: str, on_received:Callable[[str], Any]=lambda x: Option(x), on_connect:Callable[[str], None]=None, on_disconnect:Callable[[str], None]=None):
         
         on_connect = on_connect if callable(on_connect) else lambda _ : None
         on_disconnect = on_disconnect if callable(on_disconnect) else lambda _ : None
         def wrapper(func:Callable[[Any, str], None]):
             
-            @self.websocket(f"{endpoint}/ws")
+            @self.websocket(f"{endpoint}")
             async def websocket_index(websocket: WebSocket):
 
                 client_address = websocket.client or f"id: {uuid.uuid4()}"
                 print(f"{client_address} HAS ARRIVED")
                 
                 await websocket.accept()
                 on_connect(client_address)
@@ -49,15 +49,14 @@
                         
                             await websocket.send_json(
                                 func(result.unwrap(), client_address)
                             )
                 
                 except Exception as e:
                     raise (e)
-                    # print(e.with_traceback(None))
                 finally:
                     await websocket.close()
                     on_disconnect(client_address)
 
                     cv2.destroyAllWindows()
         
         return  lambda f: wrapper(f)   
@@ -70,43 +69,44 @@
 
     def create_model_enpoint(self, endpoint, model: Model, window_name=None, draw=True, resize_shape:Optional[tuple[int, int]]=None):
     
         window_name = endpoint if window_name is None else window_name
         utils = {"prev_draw": lambda img: None}
         fps = FpsDrawer()
 
-        def _draw_fn(image, result: Option=None):
+        def _draw_fn(image, client_address:str, result: Option=None):
             if result.is_ok():
                 result.unwrap().draw(image)  
                 utils['prev_draw'] = result.unwrap().draw
             else:    
                 utils['prev_draw'](image)
-
+            
+            fps.draw(image) 
+            cv2.imshow(f"{window_name} @ {client_address}", image)
+            cv2.waitKey(1)  
+        
         def _no_draw(*args, **kwargs):...
 
         draw_fn = _draw_fn if draw else _no_draw
         
         @self.videostream(endpoint, resize_shape)
         def index(image: np.ndarray, client_address):
             
-            result: Option = model.predict(image)
+            result = model(image)
 
             if not result.is_ok():
-                output =  {"success": False, "message": str(result.exception)}
-                draw_fn(image, result)
-            
+                output =  {"success": False, "message": str(result.exception)}            
             else:
-                output: ModelOutput = result.unwrap()
-                draw_fn(image, output.to_dict())
-            
-            cv2.imshow(f"{window_name} @ {client_address}", image)
-            cv2.waitKey(1)            
+                output = result.unwrap().to_dict()
+
+            draw_fn(image, client_address, result)
+                      
             return output
 
-    def create_model_enpoint_multi_client(self, endpoint, get_model_fn: Callable[[], Model], window_name=None, draw=True, resize_shape:Optional[tuple[int, int]]=None):
+    def create_model_enpoint_multi_client(self, endpoint, get_model_fn: Callable[[], Model], window_name=None, resize_shape:Optional[tuple[int, int]]=None):
         
         window_name = endpoint if window_name is None else window_name
         models: dict[str, Model] = {}
 
         def on_connect(client_address:str):
             models[client_address] = get_model_fn()
 
@@ -120,11 +120,9 @@
 
             if not result.is_ok():
                 output =  {"success": False, "message": result.msg}
             else:
                 data: ModelOutput = result.unwrap()
                 output = data.to_dict()
 
-
-            # cv2.waitKey(10)
             return output
```

### Comparing `easyaiapi-0.0.2/easyaiapi/utils.py` & `easyaiapi-0.0.3/easyaiapi/utils.py`

 * *Files identical despite different names*

### Comparing `easyaiapi-0.0.2/easyaiapi.egg-info/PKG-INFO` & `easyaiapi-0.0.3/easyaiapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyaiapi
-Version: 0.0.2
+Version: 0.0.3
 Summary: Easy ai api
 Author: Olivier
 Author-email: luowensheng2018@gmail.com
 Keywords: python,api,websocket,AI
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `easyaiapi-0.0.2/setup.py` & `easyaiapi-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 cwd = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(cwd, "README.md"), encoding="utf-8") as f:
     long_description = "\n" + f.read()
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'Easy ai api'
 install_requires = [r for r in open(os.path.join(cwd, "requirements.txt")).read().splitlines() ]
 
 setup(
     name="easyaiapi",
     version=VERSION,
     author="Olivier",
```

