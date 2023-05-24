# Comparing `tmp/eo-learn-coregistration-1.4.1.tar.gz` & `tmp/eo-learn-coregistration-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eo-learn-coregistration-1.4.1.tar", last modified: Tue Mar 14 10:32:58 2023, max compression
+gzip compressed data, was "eo-learn-coregistration-1.4.2.tar", last modified: Wed May 24 10:46:36 2023, max compression
```

## Comparing `eo-learn-coregistration-1.4.1.tar` & `eo-learn-coregistration-1.4.2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-03-14 10:32:58.083663 eo-learn-coregistration-1.4.1/
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1745 2023-03-14 10:32:57.000000 eo-learn-coregistration-1.4.1/LICENSE
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       84 2022-06-13 14:43:39.000000 eo-learn-coregistration-1.4.1/MANIFEST.in
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1812 2023-03-14 10:32:58.083663 eo-learn-coregistration-1.4.1/PKG-INFO
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      341 2023-03-14 10:22:12.000000 eo-learn-coregistration-1.4.1/README.md
-drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-03-14 10:32:58.079663 eo-learn-coregistration-1.4.1/eo_learn_coregistration.egg-info/
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1812 2023-03-14 10:32:57.000000 eo-learn-coregistration-1.4.1/eo_learn_coregistration.egg-info/PKG-INFO
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      431 2023-03-14 10:32:57.000000 eo-learn-coregistration-1.4.1/eo_learn_coregistration.egg-info/SOURCES.txt
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)        1 2023-03-14 10:32:57.000000 eo-learn-coregistration-1.4.1/eo_learn_coregistration.egg-info/dependency_links.txt
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)        1 2021-04-28 12:52:22.000000 eo-learn-coregistration-1.4.1/eo_learn_coregistration.egg-info/not-zip-safe
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       37 2023-03-14 10:32:57.000000 eo-learn-coregistration-1.4.1/eo_learn_coregistration.egg-info/requires.txt
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)        8 2023-03-14 10:32:57.000000 eo-learn-coregistration-1.4.1/eo_learn_coregistration.egg-info/top_level.txt
-drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-03-14 10:32:58.079663 eo-learn-coregistration-1.4.1/eolearn/
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       65 2022-05-03 09:13:51.000000 eo-learn-coregistration-1.4.1/eolearn/__init__.py
-drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-03-14 10:32:58.079663 eo-learn-coregistration-1.4.1/eolearn/coregistration/
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      154 2023-03-14 10:22:12.000000 eo-learn-coregistration-1.4.1/eolearn/coregistration/__init__.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     9750 2023-03-14 10:22:12.000000 eo-learn-coregistration-1.4.1/eolearn/coregistration/coregistration.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      103 2023-01-20 10:41:16.000000 eo-learn-coregistration-1.4.1/requirements.txt
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       38 2023-03-14 10:32:58.083663 eo-learn-coregistration-1.4.1/setup.cfg
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     2540 2023-01-20 10:41:16.000000 eo-learn-coregistration-1.4.1/setup.py
+drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-05-24 10:46:36.975288 eo-learn-coregistration-1.4.2/
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1745 2023-05-24 10:46:36.000000 eo-learn-coregistration-1.4.2/LICENSE
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      124 2023-05-24 10:35:48.000000 eo-learn-coregistration-1.4.2/MANIFEST.in
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1813 2023-05-24 10:46:36.975288 eo-learn-coregistration-1.4.2/PKG-INFO
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      341 2023-05-03 06:39:37.000000 eo-learn-coregistration-1.4.2/README.md
+drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-05-24 10:46:36.971288 eo-learn-coregistration-1.4.2/eo_learn_coregistration.egg-info/
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1813 2023-05-24 10:46:36.000000 eo-learn-coregistration-1.4.2/eo_learn_coregistration.egg-info/PKG-INFO
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      463 2023-05-24 10:46:36.000000 eo-learn-coregistration-1.4.2/eo_learn_coregistration.egg-info/SOURCES.txt
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)        1 2023-05-24 10:46:36.000000 eo-learn-coregistration-1.4.2/eo_learn_coregistration.egg-info/dependency_links.txt
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)        1 2021-04-28 12:52:22.000000 eo-learn-coregistration-1.4.2/eo_learn_coregistration.egg-info/not-zip-safe
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       37 2023-05-24 10:46:36.000000 eo-learn-coregistration-1.4.2/eo_learn_coregistration.egg-info/requires.txt
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)        8 2023-05-24 10:46:36.000000 eo-learn-coregistration-1.4.2/eo_learn_coregistration.egg-info/top_level.txt
+drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-05-24 10:46:36.971288 eo-learn-coregistration-1.4.2/eolearn/
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       65 2023-05-23 14:00:11.000000 eo-learn-coregistration-1.4.2/eolearn/__init__.py
+drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-05-24 10:46:36.975288 eo-learn-coregistration-1.4.2/eolearn/coregistration/
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      154 2023-05-24 10:35:48.000000 eo-learn-coregistration-1.4.2/eolearn/coregistration/__init__.py
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     9704 2023-05-24 10:35:48.000000 eo-learn-coregistration-1.4.2/eolearn/coregistration/coregistration.py
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)        0 2023-05-24 10:35:48.000000 eo-learn-coregistration-1.4.2/eolearn/coregistration/py.typed
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      103 2023-05-03 06:39:37.000000 eo-learn-coregistration-1.4.2/requirements.txt
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       38 2023-05-24 10:46:36.975288 eo-learn-coregistration-1.4.2/setup.cfg
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     2500 2023-05-24 10:35:48.000000 eo-learn-coregistration-1.4.2/setup.py
```

### Comparing `eo-learn-coregistration-1.4.1/LICENSE` & `eo-learn-coregistration-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `eo-learn-coregistration-1.4.1/PKG-INFO` & `eo-learn-coregistration-1.4.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eo-learn-coregistration
-Version: 1.4.1
+Version: 1.4.2
 Summary: A collection of image co-registration EOTasks
 Home-page: https://github.com/sentinel-hub/eo-learn
 Author: Sinergise EO research team
 Author-email: eoresearch@sinergise.com
 License: MIT
 Project-URL: Documentation, https://eo-learn.readthedocs.io
 Project-URL: Source Code, https://github.com/sentinel-hub/eo-learn
@@ -23,16 +23,16 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Scientific/Engineering :: Image Processing
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `eo-learn-coregistration-1.4.1/eo_learn_coregistration.egg-info/PKG-INFO` & `eo-learn-coregistration-1.4.2/eo_learn_coregistration.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eo-learn-coregistration
-Version: 1.4.1
+Version: 1.4.2
 Summary: A collection of image co-registration EOTasks
 Home-page: https://github.com/sentinel-hub/eo-learn
 Author: Sinergise EO research team
 Author-email: eoresearch@sinergise.com
 License: MIT
 Project-URL: Documentation, https://eo-learn.readthedocs.io
 Project-URL: Source Code, https://github.com/sentinel-hub/eo-learn
@@ -23,16 +23,16 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Scientific/Engineering :: Image Processing
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `eo-learn-coregistration-1.4.1/eolearn/coregistration/coregistration.py` & `eo-learn-coregistration-1.4.2/eolearn/coregistration/coregistration.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 This source code is licensed under the MIT license, see the LICENSE file in the root directory of this source tree.
 """
 from __future__ import annotations
 
 import logging
 import warnings
-from typing import Optional, Tuple
 
 import cv2
 import numpy as np
 
 from eolearn.core import EOPatch, EOTask, FeatureType
 from eolearn.core.exceptions import EORuntimeWarning
 from eolearn.core.types import FeaturesSpecification
@@ -33,18 +32,18 @@
     Each transformation is calculated using only a single channel of the images. If feature which contains masks of
     valid pixels is specified it is used during the estimation of the transformation. The estimated transformations
     are applied to each of the specified features.
     """
 
     def __init__(
         self,
-        registration_feature: Tuple[FeatureType, str],
-        reference_feature: Tuple[FeatureType, str],
+        registration_feature: tuple[FeatureType, str],
+        reference_feature: tuple[FeatureType, str],
         channel: int,
-        valid_mask_feature: Optional[Tuple[FeatureType, str]] = None,
+        valid_mask_feature: tuple[FeatureType, str] | None = None,
         apply_to_features: FeaturesSpecification = ...,
         interpolation_mode: int = cv2.INTER_LINEAR,
         warp_mode: int = cv2.MOTION_TRANSLATION,
         max_iter: int = 100,
         gauss_kernel_size: int = 1,
         border_mode: int = cv2.BORDER_REPLICATE,
         border_value: float = 0,
@@ -94,15 +93,15 @@
         self.num_threads = num_threads
         self.max_translation = max_translation
 
     def register(
         self,
         src: np.ndarray,
         trg: np.ndarray,
-        valid_mask: Optional[np.ndarray] = None,
+        valid_mask: np.ndarray | None = None,
         warp_mode: int = cv2.MOTION_TRANSLATION,
     ) -> np.ndarray:
         """Method that estimates the transformation between source and target image"""
         criteria = (cv2.TERM_CRITERIA_COUNT, self.max_iter, 0)
         warp_matrix_size = (3, 3) if warp_mode == cv2.MOTION_HOMOGRAPHY else (2, 3)
         warp_matrix = np.eye(*warp_matrix_size, dtype=np.float32)
 
@@ -156,15 +155,15 @@
                 new_eopatch[feature_type][feature_name][idx] = self.warp_feature(
                     eopatch[feature_type][feature_name][idx], warp_matrix
                 )
 
         new_eopatch[FeatureType.META_INFO, "warp_matrices"] = warp_matrices
         return new_eopatch
 
-    def warp(self, img: np.ndarray, warp_matrix: np.ndarray, shape: Tuple[int, int], flags: int) -> np.ndarray:
+    def warp(self, img: np.ndarray, warp_matrix: np.ndarray, shape: tuple[int, int], flags: int) -> np.ndarray:
         """Transform the target image with the estimated transformation matrix"""
         if warp_matrix.shape == (3, 3):
             return cv2.warpPerspective(
                 img.astype(np.float32),
                 warp_matrix,
                 shape,
                 flags=flags,
@@ -212,10 +211,9 @@
     better suited for co-registration
     """
     # Calculate the x and y gradients using Sobel operator
     src = src.astype(np.float32)
     grad_x = cv2.Sobel(src, cv2.CV_32F, 1, 0, ksize=3)
     grad_y = cv2.Sobel(src, cv2.CV_32F, 0, 1, ksize=3)
 
-    # Combine the two gradients
-    grad = cv2.addWeighted(np.absolute(grad_x), 0.5, np.absolute(grad_y), 0.5, 0)
-    return grad
+    # Combine and return the two gradients
+    return cv2.addWeighted(np.absolute(grad_x), 0.5, np.absolute(grad_y), 0.5, 0)
```

### Comparing `eo-learn-coregistration-1.4.1/setup.py` & `eo-learn-coregistration-1.4.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,17 +3,15 @@
 from setuptools import find_packages, setup
 
 
 def get_long_description():
     this_directory = os.path.abspath(os.path.dirname(__file__))
 
     with open(os.path.join(this_directory, "README.md"), encoding="utf-8") as f:
-        long_description = f.read()
-
-    return long_description
+        return f.read()
 
 
 def parse_requirements(file):
     with open(os.path.join(os.path.dirname(__file__), file)) as requirements_file:
         return sorted({line.partition("#")[0].strip() for line in requirements_file} - set(""))
 
 
@@ -25,15 +23,15 @@
                 version = line.split("=")[1].strip()
                 version = version.strip('"').strip("'")
     return version
 
 
 setup(
     name="eo-learn-coregistration",
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     version=get_version(),
     description="A collection of image co-registration EOTasks",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     url="https://github.com/sentinel-hub/eo-learn",
     project_urls={
         "Documentation": "https://eo-learn.readthedocs.io",
@@ -55,16 +53,16 @@
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
         "Operating System :: MacOS",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: Unix",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Scientific/Engineering",
         "Topic :: Scientific/Engineering :: GIS",
         "Topic :: Scientific/Engineering :: Image Processing",
     ],
 )
```

