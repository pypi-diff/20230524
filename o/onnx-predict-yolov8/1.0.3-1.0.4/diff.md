# Comparing `tmp/onnx-predict-yolov8-1.0.3.tar.gz` & `tmp/onnx-predict-yolov8-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnx-predict-yolov8-1.0.3.tar", last modified: Wed May 24 06:57:37 2023, max compression
+gzip compressed data, was "onnx-predict-yolov8-1.0.4.tar", last modified: Wed May 24 13:20:11 2023, max compression
```

## Comparing `onnx-predict-yolov8-1.0.3.tar` & `onnx-predict-yolov8-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 06:57:37.743885 onnx-predict-yolov8-1.0.3/
--rw-rw-rw-   0        0        0     1096 2023-05-23 12:24:50.000000 onnx-predict-yolov8-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     1895 2023-05-24 06:57:37.743885 onnx-predict-yolov8-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      141 2023-05-23 12:46:17.000000 onnx-predict-yolov8-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-24 06:57:37.738873 onnx-predict-yolov8-1.0.3/onnx_predict_yolov8.egg-info/
--rw-rw-rw-   0        0        0     1895 2023-05-24 06:57:37.000000 onnx-predict-yolov8-1.0.3/onnx_predict_yolov8.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      313 2023-05-24 06:57:37.000000 onnx-predict-yolov8-1.0.3/onnx_predict_yolov8.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 06:57:37.000000 onnx-predict-yolov8-1.0.3/onnx_predict_yolov8.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-05-24 06:57:37.000000 onnx-predict-yolov8-1.0.3/onnx_predict_yolov8.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-24 06:57:37.000000 onnx-predict-yolov8-1.0.3/onnx_predict_yolov8.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-24 06:57:37.742874 onnx-predict-yolov8-1.0.3/opyv8/
--rw-rw-rw-   0        0        0       61 2023-05-23 09:27:35.000000 onnx-predict-yolov8-1.0.3/opyv8/__init__.py
--rw-rw-rw-   0        0        0     1147 2023-05-23 11:03:26.000000 onnx-predict-yolov8-1.0.3/opyv8/model.py
--rw-rw-rw-   0        0        0     2438 2023-05-24 06:56:23.000000 onnx-predict-yolov8-1.0.3/opyv8/predictor.py
--rw-rw-rw-   0        0        0     2318 2023-05-23 12:58:13.000000 onnx-predict-yolov8-1.0.3/opyv8/utils.py
--rw-rw-rw-   0        0        0      630 2023-05-24 06:57:20.000000 onnx-predict-yolov8-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-24 06:57:37.744873 onnx-predict-yolov8-1.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-24 13:20:11.658432 onnx-predict-yolov8-1.0.4/
+-rw-rw-rw-   0        0        0     1096 2023-05-23 12:24:50.000000 onnx-predict-yolov8-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     2467 2023-05-24 13:20:11.657436 onnx-predict-yolov8-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      714 2023-05-24 08:47:57.000000 onnx-predict-yolov8-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-24 13:20:11.633282 onnx-predict-yolov8-1.0.4/onnx_predict_yolov8.egg-info/
+-rw-rw-rw-   0        0        0     2467 2023-05-24 13:20:11.000000 onnx-predict-yolov8-1.0.4/onnx_predict_yolov8.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      313 2023-05-24 13:20:11.000000 onnx-predict-yolov8-1.0.4/onnx_predict_yolov8.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 13:20:11.000000 onnx-predict-yolov8-1.0.4/onnx_predict_yolov8.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-05-24 13:20:11.000000 onnx-predict-yolov8-1.0.4/onnx_predict_yolov8.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-24 13:20:11.000000 onnx-predict-yolov8-1.0.4/onnx_predict_yolov8.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-24 13:20:11.655423 onnx-predict-yolov8-1.0.4/opyv8/
+-rw-rw-rw-   0        0        0       61 2023-05-23 09:27:35.000000 onnx-predict-yolov8-1.0.4/opyv8/__init__.py
+-rw-rw-rw-   0        0        0     1185 2023-05-24 09:41:37.000000 onnx-predict-yolov8-1.0.4/opyv8/model.py
+-rw-rw-rw-   0        0        0     2501 2023-05-24 09:57:12.000000 onnx-predict-yolov8-1.0.4/opyv8/predictor.py
+-rw-rw-rw-   0        0        0     2362 2023-05-24 09:57:28.000000 onnx-predict-yolov8-1.0.4/opyv8/utils.py
+-rw-rw-rw-   0        0        0      629 2023-05-24 09:46:17.000000 onnx-predict-yolov8-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-24 13:20:11.658432 onnx-predict-yolov8-1.0.4/setup.cfg
```

### Comparing `onnx-predict-yolov8-1.0.3/LICENSE` & `onnx-predict-yolov8-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `onnx-predict-yolov8-1.0.3/PKG-INFO` & `onnx-predict-yolov8-1.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnx-predict-yolov8
-Version: 1.0.3
+Version: 1.0.4
 Author-email: Kasper Fromm Pedersen <kasperf@cs.aau.dk>, Kristian Torp <torp@cs.aau.dk>
 Maintainer-email: Kasper Fromm Pedersen <kasperf@cs.aau.dk>
 License: MIT License
         
         Copyright (c) 2023 Aalborg University
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -24,13 +24,34 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: homepage, https://www.cs.aau.dk/
 Project-URL: repository, https://github.com/fromm1990/onnx-predict-yolov8
 Keywords: ONNX,YOLOv8,onnxruntime,vision
-Requires-Python: <3.11.0,>3.8
+Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ONNX-PREDICT-YOLOV8
 This repository is a light weight library to ease the use of ONNX models exported by the Ultralytics YOLOv8 framework.
+
+## Example Usage
+```python
+from onnxruntime import InferenceSession
+from PIL import Image
+from opyv8 import Predictor
+
+model = Path("path/to/file.onnx")
+# List of classes where the index match the class id in the ONNX network
+classes = model.parent.joinpath("classes.names").read_text().split("\n")
+session = InferenceSession(
+    model.as_posix(),
+    providers=[
+        "CUDAExecutionProvider",
+        "CPUExecutionProvider",
+    ],
+)
+predictor = Predictor(session, classes)
+img = Image.open("path/to/image.jpg")
+print(predictor.predict(img))
+```
```

### Comparing `onnx-predict-yolov8-1.0.3/onnx_predict_yolov8.egg-info/PKG-INFO` & `onnx-predict-yolov8-1.0.4/onnx_predict_yolov8.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnx-predict-yolov8
-Version: 1.0.3
+Version: 1.0.4
 Author-email: Kasper Fromm Pedersen <kasperf@cs.aau.dk>, Kristian Torp <torp@cs.aau.dk>
 Maintainer-email: Kasper Fromm Pedersen <kasperf@cs.aau.dk>
 License: MIT License
         
         Copyright (c) 2023 Aalborg University
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -24,13 +24,34 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: homepage, https://www.cs.aau.dk/
 Project-URL: repository, https://github.com/fromm1990/onnx-predict-yolov8
 Keywords: ONNX,YOLOv8,onnxruntime,vision
-Requires-Python: <3.11.0,>3.8
+Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ONNX-PREDICT-YOLOV8
 This repository is a light weight library to ease the use of ONNX models exported by the Ultralytics YOLOv8 framework.
+
+## Example Usage
+```python
+from onnxruntime import InferenceSession
+from PIL import Image
+from opyv8 import Predictor
+
+model = Path("path/to/file.onnx")
+# List of classes where the index match the class id in the ONNX network
+classes = model.parent.joinpath("classes.names").read_text().split("\n")
+session = InferenceSession(
+    model.as_posix(),
+    providers=[
+        "CUDAExecutionProvider",
+        "CPUExecutionProvider",
+    ],
+)
+predictor = Predictor(session, classes)
+img = Image.open("path/to/image.jpg")
+print(predictor.predict(img))
+```
```

### Comparing `onnx-predict-yolov8-1.0.3/opyv8/model.py` & `onnx-predict-yolov8-1.0.4/opyv8/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from dataclasses import dataclass
 from typing import Any, Optional, Protocol, Sequence, runtime_checkable
 
 from numpy import ndarray
 
 
 class PNodeArg(Protocol):
```

### Comparing `onnx-predict-yolov8-1.0.3/opyv8/predictor.py` & `onnx-predict-yolov8-1.0.4/opyv8/predictor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,20 @@
+from __future__ import annotations
+
 from pathlib import Path
-from typing import cast
+from typing import List, cast
 
 import numpy
-import utils
-from model import Label, LabelImage, PInferenceSession
 from numpy import ndarray
 from PIL import Image as ImageModule
 from PIL.Image import Image
 
+from opyv8 import utils
+from opyv8.model import Label, LabelImage, PInferenceSession
+
 
 class Predictor:
     def __init__(
         self,
         model: PInferenceSession,
         names: list[str],
         conf_threshold: float = 0.25,
@@ -27,15 +30,15 @@
             img = Path(img)
         if isinstance(img, Path):
             img = ImageModule.open(img)
         if not isinstance(img, Image):
             raise ValueError("img must be an PIL Image, Path or string")
 
         tensor = utils.image_to_tensor(img, self.__model)
-        results = cast(list[ndarray], self.__model.run(None, {"images": tensor.data}))
+        results = cast(List[ndarray], self.__model.run(None, {"images": tensor.data}))
         predictions = numpy.squeeze(results[0]).T
 
         scores = numpy.max(predictions[:, 4:], axis=1)
         keep = scores > self.__conf_threshold
         predictions = predictions[keep, :]
         scores = scores[keep]
         class_ids = numpy.argmax(predictions[:, 4:], axis=1)
```

### Comparing `onnx-predict-yolov8-1.0.3/opyv8/utils.py` & `onnx-predict-yolov8-1.0.4/opyv8/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+from __future__ import annotations
+
 import numpy
 from numpy import float32, float64, int32, int64
 from numpy.typing import NDArray
 from PIL import ImageOps
 from PIL.Image import Image, Resampling
 
-from model import ImageTensor, PInferenceSession
+from opyv8.model import ImageTensor, PInferenceSession
 
 
 def compute_iou(box: NDArray[int32], boxes: NDArray[int32]) -> NDArray[float64]:
     # Compute xmin, ymin, xmax, ymax for both boxes
     xmin = numpy.minimum(box[0], boxes[:, 0])
     ymin = numpy.minimum(box[1], boxes[:, 1])
     xmax = numpy.maximum(box[0] + box[2], boxes[:, 0] + boxes[:, 2])
```

### Comparing `onnx-predict-yolov8-1.0.3/pyproject.toml` & `onnx-predict-yolov8-1.0.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [project]
 name = "onnx-predict-yolov8"
-version = "1.0.3"
+version = "1.0.4"
 description = ""
 readme = "README.md"
 authors = [
     {name = "Kasper Fromm Pedersen", email = "kasperf@cs.aau.dk"},
     {name = "Kristian Torp", email = "torp@cs.aau.dk"}
 ]
 maintainers = [
     {name = "Kasper Fromm Pedersen", email = "kasperf@cs.aau.dk"},
 ]
 license = { file = "LICENSE"}
 keywords = ["ONNX", "YOLOv8", "onnxruntime", "vision"]
-requires-python = ">3.8,<3.11.0"
+requires-python = ">=3.8,<3.11"
 dependencies = [
     "numpy>=1.20",
     "Pillow>=9.1.0",
 ]
 
 [project.urls]
 homepage = "https://www.cs.aau.dk/"
```

