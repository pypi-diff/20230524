# Comparing `tmp/mltu-1.0.7.tar.gz` & `tmp/mltu-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mltu-1.0.7.tar", last modified: Fri Apr 14 09:18:50 2023, max compression
+gzip compressed data, was "mltu-1.0.8.tar", last modified: Mon Apr 24 10:23:36 2023, max compression
```

## Comparing `mltu-1.0.7.tar` & `mltu-1.0.8.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-04-14 09:18:50.294796 mltu-1.0.7/
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     1062 2022-12-01 14:15:30.000000 mltu-1.0.7/LICENSE
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)       24 2023-03-21 13:22:41.000000 mltu-1.0.7/MANIFEST.in
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     2504 2023-04-14 09:18:50.290796 mltu-1.0.7/PKG-INFO
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     2054 2023-03-21 13:22:41.000000 mltu-1.0.7/README.md
-drwxr-xr-x   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-04-14 09:18:50.290796 mltu-1.0.7/mltu/
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)       59 2023-04-14 09:18:26.000000 mltu-1.0.7/mltu/__init__.py
-drwxr-xr-x   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-04-14 09:18:50.290796 mltu-1.0.7/mltu/annotations/
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-03-22 13:58:16.000000 mltu-1.0.7/mltu/annotations/__init__.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     3276 2023-03-22 13:58:36.000000 mltu-1.0.7/mltu/annotations/image.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)    11735 2023-04-13 14:05:02.000000 mltu-1.0.7/mltu/augmentors.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)      867 2023-03-21 13:22:41.000000 mltu-1.0.7/mltu/configs.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)    10449 2023-04-13 14:05:02.000000 mltu-1.0.7/mltu/dataProvider.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     2006 2023-03-21 13:22:41.000000 mltu-1.0.7/mltu/inferenceModel.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     6112 2023-03-22 13:58:36.000000 mltu-1.0.7/mltu/preprocessors.py
-drwxr-xr-x   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-04-14 09:18:50.290796 mltu-1.0.7/mltu/tensorflow/
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     2718 2023-03-22 13:58:41.000000 mltu-1.0.7/mltu/tensorflow/callbacks.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)      224 2023-03-21 13:22:41.000000 mltu-1.0.7/mltu/tensorflow/dataProvider.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     3702 2023-04-14 09:18:26.000000 mltu-1.0.7/mltu/tensorflow/layers.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)      896 2023-03-21 13:22:41.000000 mltu-1.0.7/mltu/tensorflow/losses.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)    12415 2023-03-21 13:22:41.000000 mltu-1.0.7/mltu/tensorflow/metrics.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     3402 2023-03-21 13:22:41.000000 mltu-1.0.7/mltu/tensorflow/model_utils.py
-drwxr-xr-x   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-04-14 09:18:50.290796 mltu-1.0.7/mltu/torch/
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-03-21 13:22:41.000000 mltu-1.0.7/mltu/torch/__init__.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)    14543 2023-03-21 13:22:41.000000 mltu-1.0.7/mltu/torch/callbacks.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     3810 2023-03-21 13:22:41.000000 mltu-1.0.7/mltu/torch/dataProvider.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     3691 2023-03-21 13:22:41.000000 mltu-1.0.7/mltu/torch/handlers.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     1154 2023-03-21 13:22:41.000000 mltu-1.0.7/mltu/torch/losses.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     5184 2023-03-21 13:22:41.000000 mltu-1.0.7/mltu/torch/metrics.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     8139 2023-03-21 13:22:41.000000 mltu-1.0.7/mltu/torch/model.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     6224 2023-03-22 13:58:16.000000 mltu-1.0.7/mltu/transformers.py
-drwxr-xr-x   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-04-14 09:18:50.290796 mltu-1.0.7/mltu/utils/
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-03-21 13:22:41.000000 mltu-1.0.7/mltu/utils/__init__.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     3938 2023-03-21 13:22:41.000000 mltu-1.0.7/mltu/utils/text_utils.py
-drwxr-xr-x   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-04-14 09:18:50.290796 mltu-1.0.7/mltu.egg-info/
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     2504 2023-04-14 09:18:50.000000 mltu-1.0.7/mltu.egg-info/PKG-INFO
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)      767 2023-04-14 09:18:50.000000 mltu-1.0.7/mltu.egg-info/SOURCES.txt
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        1 2023-04-14 09:18:50.000000 mltu-1.0.7/mltu.egg-info/dependency_links.txt
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)      118 2023-04-14 09:18:50.000000 mltu-1.0.7/mltu.egg-info/requires.txt
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        5 2023-04-14 09:18:50.000000 mltu-1.0.7/mltu.egg-info/top_level.txt
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)      128 2023-03-21 13:22:41.000000 mltu-1.0.7/requirements.txt
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)       38 2023-04-14 09:18:50.294796 mltu-1.0.7/setup.cfg
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     1654 2023-03-22 13:58:16.000000 mltu-1.0.7/setup.py
+drwxr-xr-x   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-04-24 10:23:36.463201 mltu-1.0.8/
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     1062 2022-12-01 14:15:30.000000 mltu-1.0.8/LICENSE
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)       24 2023-03-21 13:22:41.000000 mltu-1.0.8/MANIFEST.in
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     2504 2023-04-24 10:23:36.463201 mltu-1.0.8/PKG-INFO
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     2054 2023-03-21 13:22:41.000000 mltu-1.0.8/README.md
+drwxr-xr-x   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-04-24 10:23:36.459201 mltu-1.0.8/mltu/
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)       59 2023-04-24 10:23:12.000000 mltu-1.0.8/mltu/__init__.py
+drwxr-xr-x   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-04-24 10:23:36.459201 mltu-1.0.8/mltu/annotations/
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-03-22 13:58:16.000000 mltu-1.0.8/mltu/annotations/__init__.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     3276 2023-03-22 13:58:36.000000 mltu-1.0.8/mltu/annotations/image.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)    13996 2023-04-24 10:23:12.000000 mltu-1.0.8/mltu/augmentors.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)      867 2023-03-21 13:22:41.000000 mltu-1.0.8/mltu/configs.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)    10449 2023-04-13 14:05:02.000000 mltu-1.0.8/mltu/dataProvider.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     2006 2023-03-21 13:22:41.000000 mltu-1.0.8/mltu/inferenceModel.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     6112 2023-03-22 13:58:36.000000 mltu-1.0.8/mltu/preprocessors.py
+drwxr-xr-x   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-04-24 10:23:36.463201 mltu-1.0.8/mltu/tensorflow/
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     2718 2023-03-22 13:58:41.000000 mltu-1.0.8/mltu/tensorflow/callbacks.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)      224 2023-03-21 13:22:41.000000 mltu-1.0.8/mltu/tensorflow/dataProvider.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     7266 2023-04-24 10:23:12.000000 mltu-1.0.8/mltu/tensorflow/layers.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)      896 2023-03-21 13:22:41.000000 mltu-1.0.8/mltu/tensorflow/losses.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)    12415 2023-03-21 13:22:41.000000 mltu-1.0.8/mltu/tensorflow/metrics.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     3402 2023-03-21 13:22:41.000000 mltu-1.0.8/mltu/tensorflow/model_utils.py
+drwxr-xr-x   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-04-24 10:23:36.463201 mltu-1.0.8/mltu/torch/
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-03-21 13:22:41.000000 mltu-1.0.8/mltu/torch/__init__.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)    14543 2023-03-21 13:22:41.000000 mltu-1.0.8/mltu/torch/callbacks.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     3810 2023-03-21 13:22:41.000000 mltu-1.0.8/mltu/torch/dataProvider.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     3691 2023-03-21 13:22:41.000000 mltu-1.0.8/mltu/torch/handlers.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     1154 2023-03-21 13:22:41.000000 mltu-1.0.8/mltu/torch/losses.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     5184 2023-03-21 13:22:41.000000 mltu-1.0.8/mltu/torch/metrics.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     8139 2023-03-21 13:22:41.000000 mltu-1.0.8/mltu/torch/model.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     6224 2023-03-22 13:58:16.000000 mltu-1.0.8/mltu/transformers.py
+drwxr-xr-x   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-04-24 10:23:36.463201 mltu-1.0.8/mltu/utils/
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-03-21 13:22:41.000000 mltu-1.0.8/mltu/utils/__init__.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     3938 2023-03-21 13:22:41.000000 mltu-1.0.8/mltu/utils/text_utils.py
+drwxr-xr-x   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-04-24 10:23:36.459201 mltu-1.0.8/mltu.egg-info/
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     2504 2023-04-24 10:23:36.000000 mltu-1.0.8/mltu.egg-info/PKG-INFO
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)      767 2023-04-24 10:23:36.000000 mltu-1.0.8/mltu.egg-info/SOURCES.txt
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        1 2023-04-24 10:23:36.000000 mltu-1.0.8/mltu.egg-info/dependency_links.txt
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)      118 2023-04-24 10:23:36.000000 mltu-1.0.8/mltu.egg-info/requires.txt
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        5 2023-04-24 10:23:36.000000 mltu-1.0.8/mltu.egg-info/top_level.txt
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)      128 2023-03-21 13:22:41.000000 mltu-1.0.8/requirements.txt
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)       38 2023-04-24 10:23:36.463201 mltu-1.0.8/setup.cfg
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     1654 2023-03-22 13:58:16.000000 mltu-1.0.8/setup.py
```

### Comparing `mltu-1.0.7/LICENSE` & `mltu-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mltu-1.0.7/PKG-INFO` & `mltu-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mltu
-Version: 1.0.7
+Version: 1.0.8
 Summary: Machine Learning Training Utilities (MLTU) for TenosrFlow and PyTorch
 Home-page: https://pylessons.com/
 Author: PyLessons
 Author-email: pythonlessons0@gmail.com
 Project-URL: Source, https://github.com/pythonlessons/mltu/
 Project-URL: Tracker, https://github.com/pythonlessons/mltu/issues
 Requires-Python: >=3
```

### Comparing `mltu-1.0.7/README.md` & `mltu-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `mltu-1.0.7/mltu/annotations/image.py` & `mltu-1.0.8/mltu/annotations/image.py`

 * *Files identical despite different names*

### Comparing `mltu-1.0.7/mltu/augmentors.py` & `mltu-1.0.8/mltu/augmentors.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 """ Implemented augmentors:
 - RandomBrightness
 - RandomRotate
 - RandomErodeDilate
 - RandomSharpen
 - RandomGaussianBlur
+- RandomSaltAndPepper
 """
 
 def randomness_decorator(func):
     """ Decorator for randomness """
     def wrapper(self, image: Image, annotation: typing.Any) -> typing.Tuple[Image, typing.Any]:
         """ Decorator for randomness and type checking
 
@@ -315,8 +316,64 @@
             image (Image): Blurred image
             annotation (typing.Any): Blurred annotation if necessary
         """
         img = cv2.GaussianBlur(image.numpy(), (0, 0), self.sigma)
 
         image.update(img)
 
+        return image, annotation
+    
+
+class RandomSaltAndPepper(Augmentor):
+    """ Randomly add Salt and Pepper noise to image"""
+    def __init__(
+        self, 
+        random_chance: float = 0.5,
+        log_level: int = logging.INFO,
+        salt_vs_pepper: float = 0.5,
+        amount: float = 0.1,
+        ) -> None:
+        """ Randomly add Salt and Pepper noise to image
+        
+        Args:
+            random_chance (float): Float between 0.0 and 1.0 setting bounds for random probability. Defaults to 0.5.
+            log_level (int): Log level for the augmentor. Defaults to logging.INFO.
+            salt_vs_pepper (float): ratio of salt vs pepper. Defaults to 0.5.
+            amount (float): proportion of the image to be salted and peppered. Defaults to 0.1.
+        """
+        super(RandomSaltAndPepper, self).__init__(random_chance, log_level)
+        self.salt_vs_pepper = salt_vs_pepper
+        self.amount = amount
+        
+        assert 0 <= salt_vs_pepper <= 1.0, "salt_vs_pepper must be between 0.0 and 1.0"
+        assert 0 <= amount <= 1.0, "amount must be between 0.0 and 1.0"
+
+    @randomness_decorator
+    def __call__(self, image: Image, annotation: typing.Any) -> typing.Tuple[Image, typing.Any]:
+        """ Randomly add salt and pepper noise to an image
+
+        Args:
+            image (Image): Image to be noised
+            annotation (typing.Any): Annotation to be noised
+
+        Returns:
+            image (Image): Noised image
+            annotation (typing.Any): Noised annotation if necessary
+        """
+        img = image.numpy()
+        height, width, channels = img.shape
+
+        # Salt mode
+        num_salt = int(self.amount * height * width * self.salt_vs_pepper)
+        row_coords = np.random.randint(0, height, size=num_salt)
+        col_coords = np.random.randint(0, width, size=num_salt)
+        img[row_coords, col_coords, :] = [255, 255, channels]
+
+        # Pepper mode
+        num_pepper = int(self.amount * height * width * (1.0 - self.salt_vs_pepper))
+        row_coords = np.random.randint(0, height, size=num_pepper)
+        col_coords = np.random.randint(0, width, size=num_pepper)
+        img[row_coords, col_coords, :] = [0, 0, channels]
+
+        image.update(img)
+
         return image, annotation
```

### Comparing `mltu-1.0.7/mltu/configs.py` & `mltu-1.0.8/mltu/configs.py`

 * *Files identical despite different names*

### Comparing `mltu-1.0.7/mltu/dataProvider.py` & `mltu-1.0.8/mltu/dataProvider.py`

 * *Files identical despite different names*

### Comparing `mltu-1.0.7/mltu/inferenceModel.py` & `mltu-1.0.8/mltu/inferenceModel.py`

 * *Files identical despite different names*

### Comparing `mltu-1.0.7/mltu/preprocessors.py` & `mltu-1.0.8/mltu/preprocessors.py`

 * *Files identical despite different names*

### Comparing `mltu-1.0.7/mltu/tensorflow/callbacks.py` & `mltu-1.0.8/mltu/tensorflow/callbacks.py`

 * *Files identical despite different names*

### Comparing `mltu-1.0.7/mltu/tensorflow/losses.py` & `mltu-1.0.8/mltu/tensorflow/losses.py`

 * *Files identical despite different names*

### Comparing `mltu-1.0.7/mltu/tensorflow/metrics.py` & `mltu-1.0.8/mltu/tensorflow/metrics.py`

 * *Files identical despite different names*

### Comparing `mltu-1.0.7/mltu/tensorflow/model_utils.py` & `mltu-1.0.8/mltu/tensorflow/model_utils.py`

 * *Files identical despite different names*

### Comparing `mltu-1.0.7/mltu/torch/callbacks.py` & `mltu-1.0.8/mltu/torch/callbacks.py`

 * *Files identical despite different names*

### Comparing `mltu-1.0.7/mltu/torch/dataProvider.py` & `mltu-1.0.8/mltu/torch/dataProvider.py`

 * *Files identical despite different names*

### Comparing `mltu-1.0.7/mltu/torch/handlers.py` & `mltu-1.0.8/mltu/torch/handlers.py`

 * *Files identical despite different names*

### Comparing `mltu-1.0.7/mltu/torch/losses.py` & `mltu-1.0.8/mltu/torch/losses.py`

 * *Files identical despite different names*

### Comparing `mltu-1.0.7/mltu/torch/metrics.py` & `mltu-1.0.8/mltu/torch/metrics.py`

 * *Files identical despite different names*

### Comparing `mltu-1.0.7/mltu/torch/model.py` & `mltu-1.0.8/mltu/torch/model.py`

 * *Files identical despite different names*

### Comparing `mltu-1.0.7/mltu/transformers.py` & `mltu-1.0.8/mltu/transformers.py`

 * *Files identical despite different names*

### Comparing `mltu-1.0.7/mltu/utils/text_utils.py` & `mltu-1.0.8/mltu/utils/text_utils.py`

 * *Files identical despite different names*

### Comparing `mltu-1.0.7/mltu.egg-info/PKG-INFO` & `mltu-1.0.8/mltu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mltu
-Version: 1.0.7
+Version: 1.0.8
 Summary: Machine Learning Training Utilities (MLTU) for TenosrFlow and PyTorch
 Home-page: https://pylessons.com/
 Author: PyLessons
 Author-email: pythonlessons0@gmail.com
 Project-URL: Source, https://github.com/pythonlessons/mltu/
 Project-URL: Tracker, https://github.com/pythonlessons/mltu/issues
 Requires-Python: >=3
```

### Comparing `mltu-1.0.7/mltu.egg-info/SOURCES.txt` & `mltu-1.0.8/mltu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mltu-1.0.7/setup.py` & `mltu-1.0.8/setup.py`

 * *Files identical despite different names*

