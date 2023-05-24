# Comparing `tmp/neural_anthropometer-0.0.2.tar.gz` & `tmp/neural_anthropometer-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neural_anthropometer-0.0.2.tar", last modified: Wed May 24 12:25:01 2023, max compression
+gzip compressed data, was "neural_anthropometer-0.0.3.tar", last modified: Wed May 24 15:13:25 2023, max compression
```

## Comparing `neural_anthropometer-0.0.2.tar` & `neural_anthropometer-0.0.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 neoglez   (1000) neoglez   (1000)        0 2023-05-24 12:25:01.260635 neural_anthropometer-0.0.2/
--rw-rw-r--   0 neoglez   (1000) neoglez   (1000)     3267 2022-01-27 14:34:00.000000 neural_anthropometer-0.0.2/LICENSE.md
--rw-rw-r--   0 neoglez   (1000) neoglez   (1000)    12321 2023-05-24 12:25:01.260635 neural_anthropometer-0.0.2/PKG-INFO
--rw-rw-r--   0 neoglez   (1000) neoglez   (1000)    11762 2022-01-27 14:34:00.000000 neural_anthropometer-0.0.2/README.md
-drwxrwxr-x   0 neoglez   (1000) neoglez   (1000)        0 2023-05-24 12:25:01.256635 neural_anthropometer-0.0.2/neural_anthropometer/
--rw-rw-r--   0 neoglez   (1000) neoglez   (1000)      286 2022-01-27 14:34:00.000000 neural_anthropometer-0.0.2/neural_anthropometer/__init__.py
-drwxrwxr-x   0 neoglez   (1000) neoglez   (1000)        0 2023-05-24 12:25:01.256635 neural_anthropometer-0.0.2/neural_anthropometer/annotate/
--rw-rw-r--   0 neoglez   (1000) neoglez   (1000)        0 2022-01-27 14:34:00.000000 neural_anthropometer-0.0.2/neural_anthropometer/annotate/__init__.py
--rwxrwxr-x   0 neoglez   (1000) neoglez   (1000)     4285 2022-01-27 14:34:00.000000 neural_anthropometer-0.0.2/neural_anthropometer/annotate/annotate_with_Sharmeam_and_Calvis.py
-drwxrwxr-x   0 neoglez   (1000) neoglez   (1000)        0 2023-05-24 12:25:01.256635 neural_anthropometer-0.0.2/neural_anthropometer/dataset/
--rwxrwxr-x   0 neoglez   (1000) neoglez   (1000)    21873 2022-12-05 11:44:13.000000 neural_anthropometer-0.0.2/neural_anthropometer/dataset/NeuralAnthropometerDataset.py
--rw-rw-r--   0 neoglez   (1000) neoglez   (1000)        0 2022-01-27 14:34:00.000000 neural_anthropometer-0.0.2/neural_anthropometer/dataset/__init__.py
-drwxrwxr-x   0 neoglez   (1000) neoglez   (1000)        0 2023-05-24 12:25:01.256635 neural_anthropometer-0.0.2/neural_anthropometer/display/
--rw-rw-r--   0 neoglez   (1000) neoglez   (1000)      116 2022-01-27 14:34:00.000000 neural_anthropometer-0.0.2/neural_anthropometer/display/__init__.py
--rw-rw-r--   0 neoglez   (1000) neoglez   (1000)     8282 2022-01-27 14:34:00.000000 neural_anthropometer-0.0.2/neural_anthropometer/display/display_image_grid.py
--rwxrwxr-x   0 neoglez   (1000) neoglez   (1000)     5506 2022-04-02 11:28:09.000000 neural_anthropometer-0.0.2/neural_anthropometer/display/display_subject_sharmean_and_calvis_with_vedo_and_trimesh.py
-drwxrwxr-x   0 neoglez   (1000) neoglez   (1000)        0 2023-05-24 12:25:01.256635 neural_anthropometer-0.0.2/neural_anthropometer/neural_anthropometer/
--rw-rw-r--   0 neoglez   (1000) neoglez   (1000)     2251 2022-09-01 15:25:30.000000 neural_anthropometer-0.0.2/neural_anthropometer/neural_anthropometer/NeuralAnthropometer.py
--rw-rw-r--   0 neoglez   (1000) neoglez   (1000)        0 2022-01-27 14:34:00.000000 neural_anthropometer-0.0.2/neural_anthropometer/neural_anthropometer/__init__.py
-drwxrwxr-x   0 neoglez   (1000) neoglez   (1000)        0 2023-05-24 12:25:01.260635 neural_anthropometer-0.0.2/neural_anthropometer/sharmeam/
--rw-rw-r--   0 neoglez   (1000) neoglez   (1000)        0 2022-01-27 14:34:00.000000 neural_anthropometer-0.0.2/neural_anthropometer/sharmeam/__init__.py
--rwxrwxr-x   0 neoglez   (1000) neoglez   (1000)    44444 2022-01-27 14:34:00.000000 neural_anthropometer-0.0.2/neural_anthropometer/sharmeam/sharmeam.py
-drwxrwxr-x   0 neoglez   (1000) neoglez   (1000)        0 2023-05-24 12:25:01.260635 neural_anthropometer-0.0.2/neural_anthropometer/smpl/
--rw-rw-r--   0 neoglez   (1000) neoglez   (1000)        0 2022-01-27 14:34:00.000000 neural_anthropometer-0.0.2/neural_anthropometer/smpl/__init__.py
--rwxrwxr-x   0 neoglez   (1000) neoglez   (1000)     7665 2022-01-27 14:34:00.000000 neural_anthropometer-0.0.2/neural_anthropometer/smpl/smpl.py
-drwxrwxr-x   0 neoglez   (1000) neoglez   (1000)        0 2023-05-24 12:25:01.260635 neural_anthropometer-0.0.2/neural_anthropometer/transform/
--rw-rw-r--   0 neoglez   (1000) neoglez   (1000)     5188 2023-05-24 12:04:47.000000 neural_anthropometer-0.0.2/neural_anthropometer/transform/NeuralAnthropometerTransform.py
--rw-rw-r--   0 neoglez   (1000) neoglez   (1000)        0 2022-01-27 14:34:00.000000 neural_anthropometer-0.0.2/neural_anthropometer/transform/__init__.py
-drwxrwxr-x   0 neoglez   (1000) neoglez   (1000)        0 2023-05-24 12:25:01.260635 neural_anthropometer-0.0.2/neural_anthropometer/utils/
--rw-rw-r--   0 neoglez   (1000) neoglez   (1000)        0 2022-01-27 14:34:00.000000 neural_anthropometer-0.0.2/neural_anthropometer/utils/__init__.py
--rwxrwxr-x   0 neoglez   (1000) neoglez   (1000)    10793 2022-01-27 14:34:00.000000 neural_anthropometer-0.0.2/neural_anthropometer/utils/utils.py
-drwxrwxr-x   0 neoglez   (1000) neoglez   (1000)        0 2023-05-24 12:25:01.256635 neural_anthropometer-0.0.2/neural_anthropometer.egg-info/
--rw-rw-r--   0 neoglez   (1000) neoglez   (1000)    12321 2023-05-24 12:25:01.000000 neural_anthropometer-0.0.2/neural_anthropometer.egg-info/PKG-INFO
--rw-rw-r--   0 neoglez   (1000) neoglez   (1000)     1128 2023-05-24 12:25:01.000000 neural_anthropometer-0.0.2/neural_anthropometer.egg-info/SOURCES.txt
--rw-rw-r--   0 neoglez   (1000) neoglez   (1000)        1 2023-05-24 12:25:01.000000 neural_anthropometer-0.0.2/neural_anthropometer.egg-info/dependency_links.txt
--rw-rw-r--   0 neoglez   (1000) neoglez   (1000)       20 2023-05-24 12:25:01.000000 neural_anthropometer-0.0.2/neural_anthropometer.egg-info/requires.txt
--rw-rw-r--   0 neoglez   (1000) neoglez   (1000)       21 2023-05-24 12:25:01.000000 neural_anthropometer-0.0.2/neural_anthropometer.egg-info/top_level.txt
--rw-rw-r--   0 neoglez   (1000) neoglez   (1000)       38 2023-05-24 12:25:01.260635 neural_anthropometer-0.0.2/setup.cfg
--rw-rw-r--   0 neoglez   (1000) neoglez   (1000)     1132 2023-05-24 12:24:05.000000 neural_anthropometer-0.0.2/setup.py
+drwxrwxr-x   0 neoglez   (1000) neoglez   (1000)        0 2023-05-24 15:13:25.419681 neural_anthropometer-0.0.3/
+-rw-rw-r--   0 neoglez   (1000) neoglez   (1000)     3267 2022-01-27 14:34:00.000000 neural_anthropometer-0.0.3/LICENSE.md
+-rw-rw-r--   0 neoglez   (1000) neoglez   (1000)    12321 2023-05-24 15:13:25.419681 neural_anthropometer-0.0.3/PKG-INFO
+-rw-rw-r--   0 neoglez   (1000) neoglez   (1000)    11762 2022-01-27 14:34:00.000000 neural_anthropometer-0.0.3/README.md
+drwxrwxr-x   0 neoglez   (1000) neoglez   (1000)        0 2023-05-24 15:13:25.419681 neural_anthropometer-0.0.3/neural_anthropometer/
+-rw-rw-r--   0 neoglez   (1000) neoglez   (1000)      286 2022-01-27 14:34:00.000000 neural_anthropometer-0.0.3/neural_anthropometer/__init__.py
+drwxrwxr-x   0 neoglez   (1000) neoglez   (1000)        0 2023-05-24 15:13:25.419681 neural_anthropometer-0.0.3/neural_anthropometer/annotate/
+-rw-rw-r--   0 neoglez   (1000) neoglez   (1000)        0 2022-01-27 14:34:00.000000 neural_anthropometer-0.0.3/neural_anthropometer/annotate/__init__.py
+-rwxrwxr-x   0 neoglez   (1000) neoglez   (1000)     4285 2022-01-27 14:34:00.000000 neural_anthropometer-0.0.3/neural_anthropometer/annotate/annotate_with_Sharmeam_and_Calvis.py
+drwxrwxr-x   0 neoglez   (1000) neoglez   (1000)        0 2023-05-24 15:13:25.419681 neural_anthropometer-0.0.3/neural_anthropometer/dataset/
+-rwxrwxr-x   0 neoglez   (1000) neoglez   (1000)    21873 2022-12-05 11:44:13.000000 neural_anthropometer-0.0.3/neural_anthropometer/dataset/NeuralAnthropometerDataset.py
+-rw-rw-r--   0 neoglez   (1000) neoglez   (1000)        0 2022-01-27 14:34:00.000000 neural_anthropometer-0.0.3/neural_anthropometer/dataset/__init__.py
+drwxrwxr-x   0 neoglez   (1000) neoglez   (1000)        0 2023-05-24 15:13:25.419681 neural_anthropometer-0.0.3/neural_anthropometer/display/
+-rw-rw-r--   0 neoglez   (1000) neoglez   (1000)      116 2022-01-27 14:34:00.000000 neural_anthropometer-0.0.3/neural_anthropometer/display/__init__.py
+-rw-rw-r--   0 neoglez   (1000) neoglez   (1000)     8282 2022-01-27 14:34:00.000000 neural_anthropometer-0.0.3/neural_anthropometer/display/display_image_grid.py
+-rwxrwxr-x   0 neoglez   (1000) neoglez   (1000)     5506 2022-04-02 11:28:09.000000 neural_anthropometer-0.0.3/neural_anthropometer/display/display_subject_sharmean_and_calvis_with_vedo_and_trimesh.py
+drwxrwxr-x   0 neoglez   (1000) neoglez   (1000)        0 2023-05-24 15:13:25.419681 neural_anthropometer-0.0.3/neural_anthropometer/neural_anthropometer/
+-rw-rw-r--   0 neoglez   (1000) neoglez   (1000)     2251 2022-09-01 15:25:30.000000 neural_anthropometer-0.0.3/neural_anthropometer/neural_anthropometer/NeuralAnthropometer.py
+-rw-rw-r--   0 neoglez   (1000) neoglez   (1000)        0 2022-01-27 14:34:00.000000 neural_anthropometer-0.0.3/neural_anthropometer/neural_anthropometer/__init__.py
+drwxrwxr-x   0 neoglez   (1000) neoglez   (1000)        0 2023-05-24 15:13:25.419681 neural_anthropometer-0.0.3/neural_anthropometer/sharmeam/
+-rw-rw-r--   0 neoglez   (1000) neoglez   (1000)        0 2022-01-27 14:34:00.000000 neural_anthropometer-0.0.3/neural_anthropometer/sharmeam/__init__.py
+-rwxrwxr-x   0 neoglez   (1000) neoglez   (1000)    44444 2022-01-27 14:34:00.000000 neural_anthropometer-0.0.3/neural_anthropometer/sharmeam/sharmeam.py
+drwxrwxr-x   0 neoglez   (1000) neoglez   (1000)        0 2023-05-24 15:13:25.419681 neural_anthropometer-0.0.3/neural_anthropometer/smpl/
+-rw-rw-r--   0 neoglez   (1000) neoglez   (1000)        0 2022-01-27 14:34:00.000000 neural_anthropometer-0.0.3/neural_anthropometer/smpl/__init__.py
+-rwxrwxr-x   0 neoglez   (1000) neoglez   (1000)     7665 2022-01-27 14:34:00.000000 neural_anthropometer-0.0.3/neural_anthropometer/smpl/smpl.py
+drwxrwxr-x   0 neoglez   (1000) neoglez   (1000)        0 2023-05-24 15:13:25.419681 neural_anthropometer-0.0.3/neural_anthropometer/transform/
+-rw-rw-r--   0 neoglez   (1000) neoglez   (1000)     5918 2023-05-24 14:07:51.000000 neural_anthropometer-0.0.3/neural_anthropometer/transform/NeuralAnthropometerTransform.py
+-rw-rw-r--   0 neoglez   (1000) neoglez   (1000)        0 2022-01-27 14:34:00.000000 neural_anthropometer-0.0.3/neural_anthropometer/transform/__init__.py
+drwxrwxr-x   0 neoglez   (1000) neoglez   (1000)        0 2023-05-24 15:13:25.419681 neural_anthropometer-0.0.3/neural_anthropometer/utils/
+-rw-rw-r--   0 neoglez   (1000) neoglez   (1000)        0 2022-01-27 14:34:00.000000 neural_anthropometer-0.0.3/neural_anthropometer/utils/__init__.py
+-rwxrwxr-x   0 neoglez   (1000) neoglez   (1000)    10793 2022-01-27 14:34:00.000000 neural_anthropometer-0.0.3/neural_anthropometer/utils/utils.py
+drwxrwxr-x   0 neoglez   (1000) neoglez   (1000)        0 2023-05-24 15:13:25.419681 neural_anthropometer-0.0.3/neural_anthropometer.egg-info/
+-rw-rw-r--   0 neoglez   (1000) neoglez   (1000)    12321 2023-05-24 15:13:25.000000 neural_anthropometer-0.0.3/neural_anthropometer.egg-info/PKG-INFO
+-rw-rw-r--   0 neoglez   (1000) neoglez   (1000)     1128 2023-05-24 15:13:25.000000 neural_anthropometer-0.0.3/neural_anthropometer.egg-info/SOURCES.txt
+-rw-rw-r--   0 neoglez   (1000) neoglez   (1000)        1 2023-05-24 15:13:25.000000 neural_anthropometer-0.0.3/neural_anthropometer.egg-info/dependency_links.txt
+-rw-rw-r--   0 neoglez   (1000) neoglez   (1000)       20 2023-05-24 15:13:25.000000 neural_anthropometer-0.0.3/neural_anthropometer.egg-info/requires.txt
+-rw-rw-r--   0 neoglez   (1000) neoglez   (1000)       21 2023-05-24 15:13:25.000000 neural_anthropometer-0.0.3/neural_anthropometer.egg-info/top_level.txt
+-rw-rw-r--   0 neoglez   (1000) neoglez   (1000)       38 2023-05-24 15:13:25.419681 neural_anthropometer-0.0.3/setup.cfg
+-rw-rw-r--   0 neoglez   (1000) neoglez   (1000)     1132 2023-05-24 15:07:01.000000 neural_anthropometer-0.0.3/setup.py
```

### Comparing `neural_anthropometer-0.0.2/LICENSE.md` & `neural_anthropometer-0.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neural_anthropometer-0.0.2/PKG-INFO` & `neural_anthropometer-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neural_anthropometer
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Neural Anthropometer Learning from Body Dimensions Computed on Human 3D Meshes
 Home-page: https://github.com/neoglez/neural-antropometer
 Author: ['Yansel González Tejeda', 'Helmut A. Mayer']
 Author-email: neoglez@gmail.com
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `neural_anthropometer-0.0.2/README.md` & `neural_anthropometer-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `neural_anthropometer-0.0.2/neural_anthropometer/annotate/annotate_with_Sharmeam_and_Calvis.py` & `neural_anthropometer-0.0.3/neural_anthropometer/annotate/annotate_with_Sharmeam_and_Calvis.py`

 * *Files identical despite different names*

### Comparing `neural_anthropometer-0.0.2/neural_anthropometer/dataset/NeuralAnthropometerDataset.py` & `neural_anthropometer-0.0.3/neural_anthropometer/dataset/NeuralAnthropometerDataset.py`

 * *Files identical despite different names*

### Comparing `neural_anthropometer-0.0.2/neural_anthropometer/display/display_image_grid.py` & `neural_anthropometer-0.0.3/neural_anthropometer/display/display_image_grid.py`

 * *Files identical despite different names*

### Comparing `neural_anthropometer-0.0.2/neural_anthropometer/display/display_subject_sharmean_and_calvis_with_vedo_and_trimesh.py` & `neural_anthropometer-0.0.3/neural_anthropometer/display/display_subject_sharmean_and_calvis_with_vedo_and_trimesh.py`

 * *Files identical despite different names*

### Comparing `neural_anthropometer-0.0.2/neural_anthropometer/neural_anthropometer/NeuralAnthropometer.py` & `neural_anthropometer-0.0.3/neural_anthropometer/neural_anthropometer/NeuralAnthropometer.py`

 * *Files identical despite different names*

### Comparing `neural_anthropometer-0.0.2/neural_anthropometer/sharmeam/sharmeam.py` & `neural_anthropometer-0.0.3/neural_anthropometer/sharmeam/sharmeam.py`

 * *Files identical despite different names*

### Comparing `neural_anthropometer-0.0.2/neural_anthropometer/smpl/smpl.py` & `neural_anthropometer-0.0.3/neural_anthropometer/smpl/smpl.py`

 * *Files identical despite different names*

### Comparing `neural_anthropometer-0.0.2/neural_anthropometer/transform/NeuralAnthropometerTransform.py` & `neural_anthropometer-0.0.3/neural_anthropometer/transform/NeuralAnthropometerTransform.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,24 +5,23 @@
 
 class TwoDToTensor(object):
     """Convert ndarrays in sample to Tensors."""
 
     def __call__(self, sample):
         
         pil2tensor = transforms.ToTensor()
-        #tensor2pil = transforms.ToPILImage()
-        #sample["image"] = image
-        #sample["imagefile"] = imagefile
         hbd = []
         # Use this parameter to control the tensor dtype.
         tensor_dtype = torch.float32
-        if "image" in sample:
+        if 'image' in sample:
             image = sample["image"]
-            sample["image"] = pil2tensor(image)
-        if (type(sample['annotations']['human_dimensions'])
+            sample['image'] = pil2tensor(image)
+        if ('annotations' in sample and
+            'human_dimensions' in sample['annotations'] and
+            type(sample['annotations']['human_dimensions'])
             is not torch.Tensor):
             
             for i, e in enumerate(
                     ['chest_circumference', 'height', 'inseam',
                      'left_arm_length', 'pelvis_circumference', 
                      'right_arm_length', 'shoulder_width',
                      'waist_circumference']):
@@ -54,64 +53,67 @@
         #     },
         #     "imagefile": sample["imagefile"],
         #     "annotation_file": sample["annotation_file"],
         # }
         
         return sample
 
-    class SquareAndGrayscaleImage(object):
-        """Transform an image such as it can be feed to the neural
-            anthropometer. Usually that implies escaling the image
-            keeping its aspect ratio and converting the image to
-            greyscale.
-            Code heavily inspired on
-            https://note.nkmk.me/en/python-pillow-add-margin-expand-canvas/
-        """
-        
-        def __init__(self, shape=(200,200), background_color=(0,0,0)):
-            self.shape = shape
-            self.background_color
-    
-        def __call__(self, sample):
-            wasTensor = False
-            if "image" in sample:
-                image = sample["image"]
-                
-                # If the image is not PIL, we have to conver it.
-                if (torch.is_tensor(image)):
-                    toPIL = transforms.ToPILImage()
-                    image = toPIL(image)
-                    wasTensor = True
-                # At this point we assume it is a PIL image.
-                
-                # 1.- Scale
-                image.thumbnail(self.shape, Image.Resampling.LANCZOS)
-                
-                # 2.- Reshape to square size                
-                width, height = image.size
-                # if the image is already square is OK
-                if width != height:
-                    if width > height:
-                        result = Image.new(image.mode, (width, width),
-                                           self.background_color)
-                        result.paste(image, (0, (width - height) // 2))
-                    else:
-                        result = Image.new(image.mode, (height, height),
-                                           self.background_color)
-                        result.paste(image, ((height - width) // 2, 0))
-                
-                pil2tensor = transforms.ToTensor()
-                sample["image"] = pil2tensor(result) if wasTensor else result          
+class SquareAndGreyscaleImage(object):
+    """Transform an image such as it can be feed to the neural
+        anthropometer. Usually that implies escaling the image
+        keeping its aspect ratio and converting the image to
+        greyscale.
+        Code heavily inspired on
+        https://note.nkmk.me/en/python-pillow-add-margin-expand-canvas/
+    """
+    
+    def __init__(self, shape=(200,200), background_color=(0,0,0)):
+        self.shape = shape
+        self.background_color = background_color
+
+    def __call__(self, sample):
+        wasTensor = False
+        if "image" in sample:
+            image = sample["image"]
+            
+            # If the image is not PIL, we have to conver it.
+            if (torch.is_tensor(image)):
+                toPIL = transforms.ToPILImage()
+                image = toPIL(image)
+                wasTensor = True
+            # At this point we assume it is a PIL image.
+            
+            # 1.- Scale
+            image.thumbnail(self.shape, Image.Resampling.LANCZOS)
             
-            return sample
+            # 2.- Reshape to square size                
+            width, height = image.size
+            # if the image is already square is OK
+            if width != height:
+                if width > height:
+                    result = Image.new(image.mode, (width, width),
+                                       self.background_color)
+                    result.paste(image, (0, (width - height) // 2))
+                else:
+                    result = Image.new(image.mode, (height, height),
+                                       self.background_color)
+                    result.paste(image, ((height - width) // 2, 0))
+            
+            # 3.- Convert to greyscale
+            result = result.convert("L")
+            
+            pil2tensor = transforms.ToTensor()
+            sample["image"] = pil2tensor(result) if wasTensor else result          
+        
+        return sample
 
 
 if __name__ == "__main__":
     simulated_sample = {
-        "image": np.random.randint(low=0, high=254, size=(5, 7), dtype=np.int),
+        "image": np.random.randint(low=0, high=254, size=(500, 700), dtype=np.int16),
         "annotations": {"human_dimensions": {"dim1": 1, "dim2": 2, "dim3": 3}},
         "imagefile": "simulated_image_filename.png",
         "annotation_file": "simulated_annotation_filename.json",
     }
     transform = TwoDToTensor()
 
     print(type(simulated_sample))
@@ -126,7 +128,33 @@
     print(type(simulated_sample))
     print(type(trasformed_sample["image"]))
     print(type(trasformed_sample["annotations"]["human_dimensions"]))
     print(trasformed_sample["annotations"]["human_dimensions"])
 
     print(trasformed_sample["image"].shape)
     print(trasformed_sample["annotations"]["human_dimensions"].shape)
+    
+    # RGB image
+    simulated_sample = {
+        "image": np.random.randint(low=0, high=128, size=(500, 700, 3), dtype=np.uint8)
+    }
+    transform = transforms.Compose([TwoDToTensor(), SquareAndGreyscaleImage()])
+    
+    trasformed_sample = transform(simulated_sample)
+
+    print(type(simulated_sample))
+    print(type(trasformed_sample["image"]))
+    
+    # greyscale image
+    simulated_sample = {
+        "image": np.random.randint(low=0, high=255, size=(5, 7), dtype=np.int16)
+    }
+    transform = transforms.Compose([
+        TwoDToTensor(),
+        # one background color
+        SquareAndGreyscaleImage(background_color=(0))])
+    
+    trasformed_sample = transform(simulated_sample)
+
+    print(type(simulated_sample))
+    print(type(trasformed_sample["image"]))
+
```

### Comparing `neural_anthropometer-0.0.2/neural_anthropometer/utils/utils.py` & `neural_anthropometer-0.0.3/neural_anthropometer/utils/utils.py`

 * *Files identical despite different names*

### Comparing `neural_anthropometer-0.0.2/neural_anthropometer.egg-info/PKG-INFO` & `neural_anthropometer-0.0.3/neural_anthropometer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neural-anthropometer
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Neural Anthropometer Learning from Body Dimensions Computed on Human 3D Meshes
 Home-page: https://github.com/neoglez/neural-antropometer
 Author: ['Yansel González Tejeda', 'Helmut A. Mayer']
 Author-email: neoglez@gmail.com
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `neural_anthropometer-0.0.2/neural_anthropometer.egg-info/SOURCES.txt` & `neural_anthropometer-0.0.3/neural_anthropometer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neural_anthropometer-0.0.2/setup.py` & `neural_anthropometer-0.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 00000060: 200d 0a52 4551 5549 5245 4d45 4e54 5320   ..REQUIREMENTS 
 00000070: 3d20 5b22 6e75 6d70 7922 2c20 226f 7065  = ["numpy", "ope
 00000080: 6e63 762d 7079 7468 6f6e 225d 0d0a 0d0a  ncv-python"]....
 00000090: 7365 7475 7074 6f6f 6c73 2e73 6574 7570  setuptools.setup
 000000a0: 280d 0a20 2020 2020 6e61 6d65 3d27 6e65  (..     name='ne
 000000b0: 7572 616c 5f61 6e74 6872 6f70 6f6d 6574  ural_anthropomet
 000000c0: 6572 272c 2020 0d0a 2020 2020 2076 6572  er',  ..     ver
-000000d0: 7369 6f6e 3d27 302e 302e 3227 2c0d 0a20  sion='0.0.2',.. 
+000000d0: 7369 6f6e 3d27 302e 302e 3327 2c0d 0a20  sion='0.0.3',.. 
 000000e0: 2020 2020 2373 6372 6970 7473 3d5b 2727      #scripts=[''
 000000f0: 5d2c 0d0a 2020 2020 2061 7574 686f 723d  ],..     author=
 00000100: 5b22 5961 6e73 656c 2047 6f6e 7ac3 a16c  ["Yansel Gonz..l
 00000110: 657a 2054 656a 6564 6122 2c20 2248 656c  ez Tejeda", "Hel
 00000120: 6d75 7420 412e 204d 6179 6572 225d 2c0d  mut A. Mayer"],.
 00000130: 0a20 2020 2020 6175 7468 6f72 5f65 6d61  .     author_ema
 00000140: 696c 3d22 6e65 6f67 6c65 7a40 676d 6169  il="neoglez@gmai
```

