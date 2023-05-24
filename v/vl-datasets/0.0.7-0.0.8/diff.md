# Comparing `tmp/vl_datasets-0.0.7-py3.9-none-any.whl.zip` & `tmp/vl_datasets-0.0.8-py3.9-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,13 @@
-Zip file size: 15231 bytes, number of entries: 10
--rw-r--r--  2.0 unx      141 b- defN 23-May-17 06:35 vl_datasets/__init__.py
--rw-r--r--  2.0 unx     4734 b- defN 23-May-17 06:35 vl_datasets/food101.py
--rw-r--r--  2.0 unx     2352 b- defN 23-May-17 06:35 vl_datasets/image_folder.py
--rw-r--r--  2.0 unx     4867 b- defN 23-May-17 06:35 vl_datasets/oxford_pet.py
--rw-r--r--  2.0 unx     1056 b- defN 23-May-17 06:35 vl_datasets/utils.py
--rw-r--r--  2.0 unx    11357 b- defN 23-May-17 06:35 vl_datasets-0.0.7.dist-info/LICENSE
--rw-r--r--  2.0 unx    17772 b- defN 23-May-17 06:35 vl_datasets-0.0.7.dist-info/METADATA
--rw-r--r--  2.0 unx      108 b- defN 23-May-17 06:35 vl_datasets-0.0.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-May-17 06:35 vl_datasets-0.0.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      810 b- defN 23-May-17 06:35 vl_datasets-0.0.7.dist-info/RECORD
-10 files, 43209 bytes uncompressed, 13857 bytes compressed:  67.9%
+Zip file size: 18216 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      193 b- defN 23-May-22 14:26 vl_datasets/__init__.py
+-rw-r--r--  2.0 unx     2352 b- defN 23-May-22 14:26 vl_datasets/image_folder.py
+-rw-r--r--  2.0 unx     4940 b- defN 23-May-22 14:26 vl_datasets/sentry.py
+-rw-r--r--  2.0 unx     1056 b- defN 23-May-22 14:26 vl_datasets/utils.py
+-rw-r--r--  2.0 unx     5099 b- defN 23-May-22 14:26 vl_datasets/vl_food101.py
+-rw-r--r--  2.0 unx     5008 b- defN 23-May-22 14:26 vl_datasets/vl_oxford_iiit_pet.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-May-22 14:26 vl_datasets-0.0.8.dist-info/LICENSE
+-rw-r--r--  2.0 unx    18977 b- defN 23-May-22 14:26 vl_datasets-0.0.8.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-May-22 14:26 vl_datasets-0.0.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-May-22 14:26 vl_datasets-0.0.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      899 b- defN 23-May-22 14:26 vl_datasets-0.0.8.dist-info/RECORD
+11 files, 50001 bytes uncompressed, 16702 bytes compressed:  66.6%
```

## zipnote {}

```diff
@@ -1,31 +1,34 @@
 Filename: vl_datasets/__init__.py
 Comment: 
 
-Filename: vl_datasets/food101.py
-Comment: 
-
 Filename: vl_datasets/image_folder.py
 Comment: 
 
-Filename: vl_datasets/oxford_pet.py
+Filename: vl_datasets/sentry.py
 Comment: 
 
 Filename: vl_datasets/utils.py
 Comment: 
 
-Filename: vl_datasets-0.0.7.dist-info/LICENSE
+Filename: vl_datasets/vl_food101.py
+Comment: 
+
+Filename: vl_datasets/vl_oxford_iiit_pet.py
+Comment: 
+
+Filename: vl_datasets-0.0.8.dist-info/LICENSE
 Comment: 
 
-Filename: vl_datasets-0.0.7.dist-info/METADATA
+Filename: vl_datasets-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: vl_datasets-0.0.7.dist-info/WHEEL
+Filename: vl_datasets-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: vl_datasets-0.0.7.dist-info/top_level.txt
+Filename: vl_datasets-0.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: vl_datasets-0.0.7.dist-info/RECORD
+Filename: vl_datasets-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vl_datasets/__init__.py

```diff
@@ -1,4 +1,7 @@
-__version__ = '0.0.7'
+__version__ = '0.0.8'
 from .image_folder import CleanImageFolder
-from .food101 import CleanFood101
-from .oxford_pet import CleanOxfordIIITPet
+from .vl_food101 import VLFood101
+from .vl_oxford_iiit_pet import VLOxfordIIITPet
+from .sentry import init_sentry
+
+init_sentry()
```

## Comparing `vl_datasets/food101.py` & `vl_datasets/vl_food101.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 
 from torchvision.datasets import Food101
 from typing import Any, Callable, Optional, TypeVar, Iterable
 from pathlib import Path
 import json
 import pandas as pd
 import requests
-
 import torchvision.transforms as transforms
+from vl_datasets.sentry import v1_sentry_handler, vl_capture_log_debug_state
+
 
 train_transform = transforms.Compose(
     [
         transforms.RandomResizedCrop(224),
         transforms.RandomHorizontalFlip(),
         transforms.ToTensor(),
         transforms.Normalize(mean=[0.485, 0.456, 0.406], std=[0.229, 0.224, 0.225]),
@@ -24,24 +25,26 @@
         transforms.CenterCrop(224),
         transforms.ToTensor(),
         transforms.Normalize(mean=[0.485, 0.456, 0.406], std=[0.229, 0.224, 0.225]),
     ]
 )
 
 
-class CleanFood101(Food101):
+class VLFood101(Food101):
+    @v1_sentry_handler
     def __init__(
         self,
         root: str,
         split: str = "train",
         transform: Optional[Callable] = None,
         target_transform: Optional[Callable] = None,
         download: bool = True,
         exclude_csv: Optional[str] = None
     ) -> None:
+        vl_capture_log_debug_state(locals())
         super().__init__(root, transform=transform, target_transform=target_transform, download=download)
         self._split = verify_str_arg(split, "split", ("train", "test"))
         self._base_folder = Path(self.root) / "food-101"
         self._meta_folder = self._base_folder / "meta"
         self._images_folder = self._base_folder / "images"
 
         if not self._check_exists():
@@ -68,15 +71,15 @@
             print(f"Using provided CSV file: {exclude_csv}")
             self.exclude_df = pd.read_csv(exclude_csv, header=0)
             self.exclude_set = set(self.exclude_df["filename"].tolist())
         
         # Otherwise, download the csv file
         elif exclude_csv is None:
             print("Downloading CSV file")
-            url = "https://drive.google.com/uc?export=download&id=1ZG5GvU342l4YmSeYo6v6LeKbMM5fwjjw" 
+            url = "https://drive.google.com/uc?export=download&id=1QaaNJif3qWC_AsOEugnnBASySZO0cLjW" 
             filename = "food-101.csv"
 
             try:
                 response = requests.get(url, stream=True)
                 with open(filename, "wb") as f:
                     for chunk in response.iter_content(chunk_size=1024):
                         f.write(chunk)
@@ -84,19 +87,24 @@
                 self.exclude_df = pd.read_csv(filename, header=0)
                 self.exclude_set = set(self.exclude_df["filename"].tolist())
 
             except Exception as e:
                 print("Error parsing CSV file")
                 print(e)
 
+        # A copy of self.exclude_set but without file extension
+        exclude_set_filenames = {
+            filename.split("/")[-2] + "/" + filename.split("/")[-1].split(".")[0] for filename in self.exclude_set
+        }
+
         self.excluded_files = []
         for class_label, im_rel_paths in metadata.items():
             for im_rel_path in im_rel_paths:
-                if f"{im_rel_path}.jpg" in self.exclude_set:
-                    # print(f"Excluding {im_rel_path}.jpg")
+                if f"{im_rel_path}" in exclude_set_filenames:
+                    print(f"Excluding {im_rel_path}.jpg")
                     self.excluded_files.append(f"{im_rel_path}.jpg")
                     continue
                 self._labels += [self.class_to_idx[class_label]]
                 self._image_files += [self._images_folder.joinpath(*f"{im_rel_path}.jpg".split("/"))]
 
         print(f"Excluded {len(self.excluded_files)} from the {split} set")
```

## Comparing `vl_datasets/oxford_pet.py` & `vl_datasets/vl_oxford_iiit_pet.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 import pathlib
 from typing import Callable, Optional, Union, Sequence
 from .utils import verify_str_arg
 from torchvision.datasets.vision import StandardTransform
 import pandas as pd
 import requests
 import torchvision.transforms as transforms
+from vl_datasets.sentry import v1_sentry_handler, vl_capture_log_debug_state
+
 
 
 train_transform = transforms.Compose(
     [
         transforms.RandomResizedCrop(224),
         transforms.RandomHorizontalFlip(),
         transforms.ToTensor(),
@@ -22,27 +24,28 @@
         transforms.Resize(256),
         transforms.CenterCrop(224),
         transforms.ToTensor(),
         transforms.Normalize(mean=[0.485, 0.456, 0.406], std=[0.229, 0.224, 0.225]),
     ]
 )
 
-
-class CleanOxfordIIITPet(OxfordIIITPet):
+class VLOxfordIIITPet(OxfordIIITPet):
+    @v1_sentry_handler
     def __init__(
         self,
         root: str,
         split: str = "trainval",
         target_types: Union[Sequence[str], str] = "category",
         transforms: Optional[Callable] = None,
         transform: Optional[Callable] = None,
         target_transform: Optional[Callable] = None,
         exclude_csv: Optional[str] = None,
         download: bool = True,
     ):
+        vl_capture_log_debug_state(locals())
         self._split = verify_str_arg(split, "split", ("trainval", "test"))
         if isinstance(target_types, str):
             target_types = [target_types]
         self._target_types = [
             verify_str_arg(target_type, "target_types", self._VALID_TARGET_TYPES)
             for target_type in target_types
         ]
@@ -82,15 +85,15 @@
         if exclude_csv:
             print(f"Using provided CSV file: {exclude_csv}")
             self.exclude_df = pd.read_csv(exclude_csv, header=0)
             self.exclude_set = set(self.exclude_df["filename"].tolist())
 
         elif exclude_csv is None:
             print("Downloading CSV file")
-            url = "https://drive.google.com/uc?export=download&id=1OLa8k4NITnmCHjeByzvGaWt3W7k6R1QL"
+            url = "https://drive.google.com/uc?export=download&id=1CZEYQF5BMAPajf67zYMn-IaaC2gMJj_H"
             filename = "oxford-pets.csv"
 
             try:
                 response = requests.get(url, stream=True)
                 with open(filename, "wb") as f:
                     for chunk in response.iter_content(chunk_size=1024):
                         f.write(chunk)
@@ -133,8 +136,8 @@
             )
         ]
         self.class_to_idx = dict(zip(self.classes, range(len(self.classes))))
 
         self._images = [
             self._images_folder / f"{image_id}.jpg" for image_id in image_ids
         ]
-        self._segs = [self._segs_folder / f"{image_id}.png" for image_id in image_ids]
+        self._segs = [self._segs_folder / f"{image_id}.png" for image_id in image_ids]
```

## Comparing `vl_datasets-0.0.7.dist-info/LICENSE` & `vl_datasets-0.0.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `vl_datasets-0.0.7.dist-info/METADATA` & `vl_datasets-0.0.8.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vl-datasets
-Version: 0.0.7
+Version: 0.0.8
 Summary: Open, Clean Datasets for Computer Vision.
 Home-page: https://github.com/visual-layer/vl-datasets
 Author: Visual Layer
 Author-email: info@visual-layer.com
 License: Apache-2.0
 Keywords: machine learning,computer vision,data-centric
 Platform: UNKNOWN
@@ -16,14 +16,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch
 Requires-Dist: torchvision
 Requires-Dist: pandas
+Requires-Dist: sentry-sdk
 
 
 <!-- PROJECT SHIELDS -->
 <!--
 *** I'm using markdown "reference style" links for readability.
 *** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
 *** See the bottom of this document for the declaration of the reference variables
@@ -50,20 +51,19 @@
 [license-shield]: https://img.shields.io/badge/License-Apache%202.0-purple.svg?style=for-the-badge
 [license-url]: https://github.com/visual-layer/vl-datasets/blob/main/LICENSE
 
 
 <!-- PROJECT LOGO -->
 <br />
 <div align="center">
-
 <a href="https://www.visual-layer.com">
-  <img alt="Visual Layer Logo" src="https://raw.githubusercontent.com/visual-layer/fastdup/main/gallery/visual_layer_logo.png" alt="Logo" width="400">
+  <img alt="Visual Layer Logo" src="https://raw.githubusercontent.com/visual-layer/fastdup/main/gallery/visual_layer_logo.png" alt="Logo" width="350">
 </a>
-
-<h3 align="center">Open, Clean, Curated Datasets for Computer Vision</h3>
+<h3 align="center">VL-Datasets</h3>
+<h4 align="center">Open, Clean, Curated Datasets for Computer Vision</h4>
 
   <p align="center">
   <br />
     🔥 We use
     <a href="https://github.com/visual-layer/fastdup">fastdup</a> - a free tool to clean all datasets shared in this repo.
     <br />
     <a href="https://visual-layer.readme.io/" target="_blank" rel="noopener noreferrer"><strong>Explore the docs »</strong></a>
@@ -105,99 +105,104 @@
 
 We support some of the most widely used computer vision datasets.
 [Let us know](https://forms.gle/8jxPkyzeKj82kPed8) if you have additional request to support a new dataset.
 
 All the datasets are analyzed for issues such as: 
 
 + Duplicates.
++ Near Duplicates.
 + Broken images.
 + Outliers.
 + Dark/Bright/Blurry images.
++ Mislabels.
 
 ![image](./imgs/issues.png)
 
-`vl-datasets` provides a convenient way to access these cleaned datasets in Python.
 
-Alternatively, for each dataset in this repo, we provide a `.csv` file that lists the problematic images from the dataset.
-
-You can use the listed images in the `.csv` to improve the model by re-labeling the them or just simply remove it from the dataset.
 
 
 ## Why?
 
 Computer vision is an exciting and rapidly advancing field, with new techniques and models emerging now and then. 
 However, to develop and evaluate these models, it's essential to have reliable and standardized datasets to work with.
 
 Even with the recent success of generative models, data quality remains an issue that's [mainly overlooked](https://medium.com/@amiralush/large-image-datasets-today-are-a-mess-e3ea4c9e8d22).
 Training models will erroneours data impacts model accuracy, incurs costs in time, storage and computational resources.
 
 We believe that access to clean and high-quality computer vision datasets leads to accurate, non-biased, and efficient model.
 By providing public access to `vl-datasets` we hope it helps advance the field of computer vision.
 
 ## Datasets & Access
+
+`vl-datasets` provides a convenient way to access the cleaned version of the datasets in Python.
+
+Alternatively, for each dataset in this repo, we provide a `.csv` file that lists the problematic images from the dataset.
+
+You can use the listed images in the `.csv` to improve the model by re-labeling the them or just simply remove it from the dataset.
+
 We're a startup and we'd like to offer free access to the datasets as much as we can afford to. But in doing so, we'd also need your support.
 
 We're offering select `.csv` files completely free with no strings attached. 
 For access to our complete dataset and exclusive beta features, all we ask is that you [sign up](https://forms.gle/8jxPkyzeKj82kPed8) to be a beta tester – it's completely free and your feedback will help shape the future of our platform. 
 
 Here is a table of widely used computer vision datasets, issues we found and a link to access the `.csv` file.
 
 
-| Dataset                                                                 | Issues (WIP)                                                                                                                                                                                 | CSV                                                                                                | Class                |
+| Dataset                                                                 | Issues                                                                                                                                                                                 | CSV                                                                                                | Usage                |
 |-------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------|----------------------|
-| [Food-101](https://data.vision.ee.ethz.ch/cvl/datasets_extra/food-101/) | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Download [here](https://drive.google.com/uc?export=download&id=1ZG5GvU342l4YmSeYo6v6LeKbMM5fwjjw). | `CleanFood101`       |
-| [Oxford-IIIT Pet](https://www.robots.ox.ac.uk/~vgg/data/pets/)          | <ul><li>Duplicates - 1.021% (75)</li><li>Outliers - 0.095% (7)</li><li>Broken - 0.000% (0)</li><li>Blur - 0.000% (0)</li><li>Dark - 0.054% (4)</li><li>Bright - 0.000% (0)</li></ul>         | Download [here](https://drive.google.com/uc?export=download&id=1OLa8k4NITnmCHjeByzvGaWt3W7k6R1QL). | `CleanOxfordIIITPet` |
-| [LAION-1B](https://laion.ai/blog/laion-5b/)                             | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).                                        | WIP                  |
-| [Imagenet-21k](https://www.image-net.org/)                              | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).                                        | WIP                  |
-| [Imagenet-1k](https://www.image-net.org/)                               | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).                                        | WIP                  |
-| [KITTI](https://www.cvlibs.net/datasets/kitti/)                         | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).                                        | WIP                  |
-| [DeepFashion](http://mmlab.ie.cuhk.edu.hk/projects/DeepFashion.html)    | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).                                        | WIP                  |
-| [Places365](https://github.com/CSAILVision/places365)                   | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).                                        | WIP                  |
-| [CelebA-HQ](http://mmlab.ie.cuhk.edu.hk/projects/CelebA.html)           | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).                                        | WIP                  |
-| [ADE20K](https://groups.csail.mit.edu/vision/datasets/ADE20K/)          | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).                                        | WIP                  |
-| [COCO](https://cocodataset.org/#home)                                   | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).                                        | WIP                  |
+| [Food-101](./dataset_card/food101.md) | <ul><li>Duplicates - 0.233 % (235)</li><li>Outliers - 0.076 % (77)</li><li>Blur - Blur - 0.183 % (185)</li><li>Dark - 0.043 % (43)</li><li><b>Total</b> - 0.535 % (540)</li></ul> | Download [here](https://drive.google.com/uc?export=download&id=1ZG5GvU342l4YmSeYo6v6LeKbMM5fwjjw). | `from vl_datasets import VLFood101`       |
+| [Oxford-IIIT Pet](./dataset_card/oxford-iiit-pets.md)          | <ul><li>Duplicates - 1.021% (75)</li><li>Outliers - 0.095% (7)</li><li>Dark - 0.054% (4)</li><li><b>Total</b> - 1.170 % (86)</li></ul>         | Download [here](https://drive.google.com/uc?export=download&id=1OLa8k4NITnmCHjeByzvGaWt3W7k6R1QL). | `from vl_datasets import VLOxfordIIITPet` |
+| [LAION-1B](https://laion.ai/blog/laion-5b/)                             | <ul><li>Duplicates - WIP % (WIP)</li><li>Outliers - WIP % (WIP)</li><li>Broken - WIP % (WIP)</li><li>Blur - WIP % (WIP)</li><li>Dark - WIP % (WIP)</li><li>Bright - WIP % (WIP)</li></ul> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).                                        | WIP                  |
+| [ImageNet-21K](https://www.image-net.org/)                              | <ul><li>Duplicates - 11.853 % (1,559,120)</li><li>Outliers - 0.085 % (11,119)</li><li>Blur - 0.292 % (38,458)</li><li>Dark - 0.179 % (23,574)</li><li>Bright - 0.431 % (56,754)</li><li>Mislabels - 3.064 % (402,963)</li><li><b>Total</b> - 15.904 % (2,091,988)</li></ul> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).                                        | WIP                  |
+| [ImageNet-1K](https://www.image-net.org/)                               | <ul><li>Duplicates - 0.520 % (6,660)</li><li>Outliers - 0.090 % (1,150)</li><li>Blur - 0.200 % (2,554)</li><li>Dark - 0.244 % (2,997)</li><li>Bright - 0.058 % (746)</li><li>Mislabels - 0.119 % (1,518)</li><li><b>Total</b> - 1.221 % (15,625)</li></ul> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).                                        | WIP                  |
+| [KITTI](https://www.cvlibs.net/datasets/kitti/)                         | <ul><li>Duplicates - 15.294 % (2294)</li><li>Outliers - 0.107 % (16)</li><li><b>Total</b> - 15.401 % (2310)</li></ul> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).                                        | WIP                  |
+| [DeepFashion](http://mmlab.ie.cuhk.edu.hk/projects/DeepFashion.html)    | <ul><li>Duplicates - WIP % (WIP)</li><li>Outliers - WIP % (WIP)</li><li>Broken - WIP % (WIP)</li><li>Blur - WIP % (WIP)</li><li>Dark - WIP % (WIP)</li><li>Bright - WIP % (WIP)</li></ul> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).                                        | WIP                  |
+| [Places365](https://github.com/CSAILVision/places365)                   | <ul><li>Duplicates - WIP % (WIP)</li><li>Outliers - WIP % (WIP)</li><li>Broken - WIP % (WIP)</li><li>Blur - WIP % (WIP)</li><li>Dark - WIP % (WIP)</li><li>Bright - WIP % (WIP)</li></ul> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).                                        | WIP                  |
+| [CelebA-HQ](http://mmlab.ie.cuhk.edu.hk/projects/CelebA.html)           | <ul><li>Duplicates - 1.673 % (3,389)</li><li>Outliers - 0.077 % (157)</li><li>Blur - 0.512 % (1,037)</li><li>Dark - 0.009 % (18)</li><li>Mislabels - 0.006 % (13)</li><li><b>Total</b> - 2.277 % (4,614)</li></ul> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).                                        | WIP                  |
+| [ADE20K](https://groups.csail.mit.edu/vision/datasets/ADE20K/)          | <ul><li>Duplicates - WIP % (WIP)</li><li>Outliers - WIP % (WIP)</li><li>Broken - WIP % (WIP)</li><li>Blur - WIP % (WIP)</li><li>Dark - WIP % (WIP)</li><li>Bright - WIP % (WIP)</li></ul> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).                                        | WIP                  |
+| [COCO](https://cocodataset.org/#home)                                   | <ul><li>Duplicates - 0.123 % (201)</li><li>Outliers - 0.087 % (143)</li><li>Blur - 0.029 % (47)</li><li>Dark - 0.106 % (174)</li><li>Bright - 0.013 % (21)</li><li><b>Total</b> - 0.358 % (586)</li></ul> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).                                        | WIP                  |
 
 
 
 Learn more on how we clean the datasets using our profilling tool [here](https://visual-layer.link).
 
 
 ## Installation
 
-**Option 1** - Install `vl_datasets` package from PyPI:
+**Option 1** - Install `vl_datasets` package from [PyPI](https://pypi.org/project/vl-datasets/):
 
 ```shell
 pip install vl-datasets
 ```
 
 **Option 2** - Install the bleeding edge version on GitHub:
 ```
 pip install git+https://github.com/visual-layer/vl-datasets.git@main --upgrade
 ```
 
 ## Usage
 To start using `vl-datasets`, import the clean version of the dataset with:
 
 ```python
-from vl_datasets import CleanFood101
+from vl_datasets import VLFood101
 ```
 
 This should import the clean version of the `Food101` dataset.
 
 Next, you can load the dataset as a PyTorch `Dataset`.
 
 ```python
-train_dataset = CleanFood101('./', split='train')
-valid_dataset = CleanFood101('./', split='test')
+train_dataset = VLFood101('./', split='train')
+valid_dataset = VLFood101('./', split='test')
 ```
 
 If you have a custom `.csv` file you can optionally pass in the file:
 
 ```python
-train_dataset = CleanFood101('./', split='train', exclude_csv='my-file.csv')
+train_dataset = VLFood101('./', split='train', exclude_csv='my-file.csv')
 ```
 The filenames listed in the `.csv` will be excluded in the dataset.
 
 Next, you can load the train and validation datasets in a PyTorch training loop.
 
 See the [Learn from Examples](#learn-from-examples) section to learn more.
 
@@ -213,15 +218,15 @@
 		<td rowspan="4" width="160">
 			<a href="https://visual-layer.readme.io/docs/getting-started">
 				<img src="./imgs/food.jpg" width="256" />
 			</a>
 		</td>
 		<td rowspan="4">
 			<ul>
-				<li><b>Dataset:</b> <code>CleanFood101</code></li>
+				<li><b>Dataset:</b> <code>VLFood101</code></li>
 				<li><b>Framework:</b> PyTorch.</li>
 				<li><b>Description:</b> Load a dataset and train a PyTorch model.</li>
 			</ul>
 		</td>
 		<td align="center" width="80">
 			<a href="https://nbviewer.org/github/visual-layer/vl-datasets/blob/main/notebooks/train-pytorch.ipynb">
 				<img src="./imgs/nbviewer_logo.svg" height="34" />
@@ -254,15 +259,15 @@
 		<td rowspan="4" width="160">
 			<a href="https://visual-layer.readme.io/docs/objects-and-bounding-boxes">
 				<img src="./imgs/pet.jpg" width="256" />
 			</a>
 		</td>
 		<td rowspan="4">
 			<ul>
-				<li><b>Dataset:</b> <code>CleanOxfordIIITPet</code></li>
+				<li><b>Dataset:</b> <code>VLOxfordIIITPet</code></li>
 				<li><b>Framework:</b> fast.ai.</li>
 				<li><b>Description:</b> Finetune a pretrained TIMM model using fastai.</li>
 			</ul>
 		</td>
 		<td align="center" width="80">
 			<a href="https://nbviewer.org/github/visual-layer/vl-datasets/blob/main/notebooks/train-fastai.ipynb">
 				<img src="./imgs/nbviewer_logo.svg" height="34" />
@@ -295,14 +300,28 @@
 
 
 ## License
 `vl-datasets` is licensed under the Apache 2.0 License. See [LICENSE](./LICENSE).
 
 However, you are bound to the usage license of the original dataset. It is your responsibility to determine whether you have permission to use the dataset under the dataset's license. We provide no warranty or guarantee of accuracy or completeness.
 
+## Usage Tracking
+This repository incorporates usage tracking using [Sentry.io](https://sentry.io/) to monitor and collect valuable information about the usage of the application.
+
+Usage tracking allows us to gain insights into how the application is being used in real-world scenarios. It provides us with valuable information that helps in understanding user behavior, identifying potential issues, and making informed decisions to improve the application.
+
+We DO NOT collect folder names, user names, image names, image content and other personaly identifiable information.
+
+What data is tracked?
++ **Errors and Exceptions**: Sentry captures errors and exceptions that occur in the application, providing detailed stack traces and relevant information to help diagnose and fix issues.
++ **Performance Metrics**: Sentry collects performance metrics, such as response times, latency, and resource usage, enabling us to monitor and optimize the application's performance.
+
+Read more on Sentry's official [webpage](https://sentry.io/welcome/).
+
+
 ## Getting Help
 Get help from the Visual Layer team or community members via the following channels -
 + [Slack](https://visualdatabase.slack.com/join/shared_invite/zt-19jaydbjn-lNDEDkgvSI1QwbTXSY6dlA#/shared-invite/email).
 + GitHub [issues](https://github.com/visual-layer/vl-datasets/issues).
 + Discussion [forum](https://visual-layer.readme.io/discuss).
 
 ## About Visual-Layer
```

### html2text {}

```diff
@@ -1,198 +1,209 @@
-Metadata-Version: 2.1 Name: vl-datasets Version: 0.0.7 Summary: Open, Clean
+Metadata-Version: 2.1 Name: vl-datasets Version: 0.0.8 Summary: Open, Clean
 Datasets for Computer Vision. Home-page: https://github.com/visual-layer/vl-
 datasets Author: Visual Layer Author-email: info@visual-layer.com License:
 Apache-2.0 Keywords: machine learning,computer vision,data-centric Platform:
 UNKNOWN Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Operating System
 :: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: torch Requires-Dist: torchvision
-Requires-Dist: pandas   [![PyPi][pypi-shield]][pypi-url] [![PyPi][pypiversion-
-shield]][pypi-url] [![PyPi][downloads-shield]][downloads-url] [![License]
-[license-shield]][license-url]    [pypi-shield]: https://img.shields.io/badge/
-Python-3.7%20--%203.11-blue?style=for-the-badge [pypi-url]: https://pypi.org/
-project/vl-datasets/ [pypiversion-shield]: https://img.shields.io/pypi/v/vl-
-datasets?style=for-the-badge [downloads-shield]: https://img.shields.io/badge/
-dynamic/json?style=for-the-
+Requires-Dist: pandas Requires-Dist: sentry-sdk   [![PyPi][pypi-shield]][pypi-
+url] [![PyPi][pypiversion-shield]][pypi-url] [![PyPi][downloads-shield]]
+[downloads-url] [![License][license-shield]][license-url]    [pypi-shield]:
+https://img.shields.io/badge/Python-3.7%20--%203.11-blue?style=for-the-badge
+[pypi-url]: https://pypi.org/project/vl-datasets/ [pypiversion-shield]: https:/
+/img.shields.io/pypi/v/vl-datasets?style=for-the-badge [downloads-shield]:
+https://img.shields.io/badge/dynamic/json?style=for-the-
 badge&label=downloads&query=%24.total_downloads&url=https%3A%2F%2Fapi.pepy.tech%2Fapi%2Fprojects%2Fvl-
 datasets&color=lightblue [downloads-url]: https://pypi.org/project/vl-datasets/
 [license-shield]: https://img.shields.io/badge/License-Apache%202.0-
 purple.svg?style=for-the-badge [license-url]: https://github.com/visual-layer/
 vl-datasets/blob/main/LICENSE
                               [Visual_Layer_Logo]
-          **** Open, Clean, Curated Datasets for Computer Vision ****
+                             **** VL-Datasets ****
+           *** Open, Clean, Curated Datasets for Computer Vision ***
 
  ð¥ We use fastdup - a free tool to clean all datasets shared in this repo.
                              Explore_the_docs_Â»
             Report_Issues Â· Read_Blog Â· Get_In_Touch Â· About_Us
 
                       [Logo] [Logo] [Logo] [Logo] [Logo]
 ## Description `vl-datasets` is a Python package that provides access to clean
 computer vision datasets with only 2 lines of code. For example, to get access
 to the clean version of the [Food-101](https://data.vision.ee.ethz.ch/cvl/
 datasets_extra/food-101/) dataset simply run: ![image](./imgs/usage.png) We
 support some of the most widely used computer vision datasets. [Let us know]
 (https://forms.gle/8jxPkyzeKj82kPed8) if you have additional request to support
 a new dataset. All the datasets are analyzed for issues such as: + Duplicates.
-+ Broken images. + Outliers. + Dark/Bright/Blurry images. ![image](./imgs/
-issues.png) `vl-datasets` provides a convenient way to access these cleaned
-datasets in Python. Alternatively, for each dataset in this repo, we provide a
-`.csv` file that lists the problematic images from the dataset. You can use the
-listed images in the `.csv` to improve the model by re-labeling the them or
-just simply remove it from the dataset. ## Why? Computer vision is an exciting
++ Near Duplicates. + Broken images. + Outliers. + Dark/Bright/Blurry images. +
+Mislabels. ![image](./imgs/issues.png) ## Why? Computer vision is an exciting
 and rapidly advancing field, with new techniques and models emerging now and
 then. However, to develop and evaluate these models, it's essential to have
 reliable and standardized datasets to work with. Even with the recent success
 of generative models, data quality remains an issue that's [mainly overlooked]
 (https://medium.com/@amiralush/large-image-datasets-today-are-a-mess-
 e3ea4c9e8d22). Training models will erroneours data impacts model accuracy,
 incurs costs in time, storage and computational resources. We believe that
 access to clean and high-quality computer vision datasets leads to accurate,
 non-biased, and efficient model. By providing public access to `vl-datasets` we
-hope it helps advance the field of computer vision. ## Datasets & Access We're
-a startup and we'd like to offer free access to the datasets as much as we can
-afford to. But in doing so, we'd also need your support. We're offering select
-`.csv` files completely free with no strings attached. For access to our
-complete dataset and exclusive beta features, all we ask is that you [sign up]
-(https://forms.gle/8jxPkyzeKj82kPed8) to be a beta tester â it's completely
-free and your feedback will help shape the future of our platform. Here is a
-table of widely used computer vision datasets, issues we found and a link to
-access the `.csv` file. | Dataset | Issues (WIP) | CSV | Class | |-------------
-------------------------------------------------------------|------------------
--------------------------------------------------------------------------------
+hope it helps advance the field of computer vision. ## Datasets & Access `vl-
+datasets` provides a convenient way to access the cleaned version of the
+datasets in Python. Alternatively, for each dataset in this repo, we provide a
+`.csv` file that lists the problematic images from the dataset. You can use the
+listed images in the `.csv` to improve the model by re-labeling the them or
+just simply remove it from the dataset. We're a startup and we'd like to offer
+free access to the datasets as much as we can afford to. But in doing so, we'd
+also need your support. We're offering select `.csv` files completely free with
+no strings attached. For access to our complete dataset and exclusive beta
+features, all we ask is that you [sign up](https://forms.gle/8jxPkyzeKj82kPed8)
+to be a beta tester â it's completely free and your feedback will help shape
+the future of our platform. Here is a table of widely used computer vision
+datasets, issues we found and a link to access the `.csv` file. | Dataset |
+Issues | CSV | Usage | |-------------------------------------------------------
+------------------|------------------------------------------------------------
 -------------------------------------------------------------------------------
---------------|----------------------------------------------------------------
-------------------------------------|----------------------| | [Food-101]
-(https://data.vision.ee.ethz.ch/cvl/datasets_extra/food-101/) |
-    * Duplicates - 0.24% (12,345)
-    * Outliers - 0.85% (456)
-    * Broken - 0.85% (456)
-    * Blur - 0.85% (456)
-    * Dark - 0.85% (456)
-    * Bright - 0.85% (456)
+---------------------------------------------------|---------------------------
+-------------------------------------------------------------------------|-----
+-----------------| | [Food-101](./dataset_card/food101.md) |
+    * Duplicates - 0.233 % (235)
+    * Outliers - 0.076 % (77)
+    * Blur - Blur - 0.183 % (185)
+    * Dark - 0.043 % (43)
+    * Total - 0.535 % (540)
 | Download [here](https://drive.google.com/
-uc?export=download&id=1ZG5GvU342l4YmSeYo6v6LeKbMM5fwjjw). | `CleanFood101` | |
-[Oxford-IIIT Pet](https://www.robots.ox.ac.uk/~vgg/data/pets/) |
+uc?export=download&id=1ZG5GvU342l4YmSeYo6v6LeKbMM5fwjjw). | `from vl_datasets
+import VLFood101` | | [Oxford-IIIT Pet](./dataset_card/oxford-iiit-pets.md) |
     * Duplicates - 1.021% (75)
     * Outliers - 0.095% (7)
-    * Broken - 0.000% (0)
-    * Blur - 0.000% (0)
     * Dark - 0.054% (4)
-    * Bright - 0.000% (0)
+    * Total - 1.170 % (86)
 | Download [here](https://drive.google.com/
-uc?export=download&id=1OLa8k4NITnmCHjeByzvGaWt3W7k6R1QL). |
-`CleanOxfordIIITPet` | | [LAION-1B](https://laion.ai/blog/laion-5b/) |
-    * Duplicates - 0.24% (12,345)
-    * Outliers - 0.85% (456)
-    * Broken - 0.85% (456)
-    * Blur - 0.85% (456)
-    * Dark - 0.85% (456)
-    * Bright - 0.85% (456)
-| Request access [here](https://forms.gle/8jxPkyzeKj82kPed8). | WIP | |
-[Imagenet-21k](https://www.image-net.org/) |
-    * Duplicates - 0.24% (12,345)
-    * Outliers - 0.85% (456)
-    * Broken - 0.85% (456)
-    * Blur - 0.85% (456)
-    * Dark - 0.85% (456)
-    * Bright - 0.85% (456)
-| Request access [here](https://forms.gle/8jxPkyzeKj82kPed8). | WIP | |
-[Imagenet-1k](https://www.image-net.org/) |
-    * Duplicates - 0.24% (12,345)
-    * Outliers - 0.85% (456)
-    * Broken - 0.85% (456)
-    * Blur - 0.85% (456)
-    * Dark - 0.85% (456)
-    * Bright - 0.85% (456)
+uc?export=download&id=1OLa8k4NITnmCHjeByzvGaWt3W7k6R1QL). | `from vl_datasets
+import VLOxfordIIITPet` | | [LAION-1B](https://laion.ai/blog/laion-5b/) |
+    * Duplicates - WIP % (WIP)
+    * Outliers - WIP % (WIP)
+    * Broken - WIP % (WIP)
+    * Blur - WIP % (WIP)
+    * Dark - WIP % (WIP)
+    * Bright - WIP % (WIP)
+| Request access [here](https://forms.gle/8jxPkyzeKj82kPed8). | WIP | |
+[ImageNet-21K](https://www.image-net.org/) |
+    * Duplicates - 11.853 % (1,559,120)
+    * Outliers - 0.085 % (11,119)
+    * Blur - 0.292 % (38,458)
+    * Dark - 0.179 % (23,574)
+    * Bright - 0.431 % (56,754)
+    * Mislabels - 3.064 % (402,963)
+    * Total - 15.904 % (2,091,988)
+| Request access [here](https://forms.gle/8jxPkyzeKj82kPed8). | WIP | |
+[ImageNet-1K](https://www.image-net.org/) |
+    * Duplicates - 0.520 % (6,660)
+    * Outliers - 0.090 % (1,150)
+    * Blur - 0.200 % (2,554)
+    * Dark - 0.244 % (2,997)
+    * Bright - 0.058 % (746)
+    * Mislabels - 0.119 % (1,518)
+    * Total - 1.221 % (15,625)
 | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8). | WIP | | [KITTI]
 (https://www.cvlibs.net/datasets/kitti/) |
-    * Duplicates - 0.24% (12,345)
-    * Outliers - 0.85% (456)
-    * Broken - 0.85% (456)
-    * Blur - 0.85% (456)
-    * Dark - 0.85% (456)
-    * Bright - 0.85% (456)
+    * Duplicates - 15.294 % (2294)
+    * Outliers - 0.107 % (16)
+    * Total - 15.401 % (2310)
 | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8). | WIP | |
 [DeepFashion](http://mmlab.ie.cuhk.edu.hk/projects/DeepFashion.html) |
-    * Duplicates - 0.24% (12,345)
-    * Outliers - 0.85% (456)
-    * Broken - 0.85% (456)
-    * Blur - 0.85% (456)
-    * Dark - 0.85% (456)
-    * Bright - 0.85% (456)
+    * Duplicates - WIP % (WIP)
+    * Outliers - WIP % (WIP)
+    * Broken - WIP % (WIP)
+    * Blur - WIP % (WIP)
+    * Dark - WIP % (WIP)
+    * Bright - WIP % (WIP)
 | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8). | WIP | |
 [Places365](https://github.com/CSAILVision/places365) |
-    * Duplicates - 0.24% (12,345)
-    * Outliers - 0.85% (456)
-    * Broken - 0.85% (456)
-    * Blur - 0.85% (456)
-    * Dark - 0.85% (456)
-    * Bright - 0.85% (456)
+    * Duplicates - WIP % (WIP)
+    * Outliers - WIP % (WIP)
+    * Broken - WIP % (WIP)
+    * Blur - WIP % (WIP)
+    * Dark - WIP % (WIP)
+    * Bright - WIP % (WIP)
 | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8). | WIP | |
 [CelebA-HQ](http://mmlab.ie.cuhk.edu.hk/projects/CelebA.html) |
-    * Duplicates - 0.24% (12,345)
-    * Outliers - 0.85% (456)
-    * Broken - 0.85% (456)
-    * Blur - 0.85% (456)
-    * Dark - 0.85% (456)
-    * Bright - 0.85% (456)
+    * Duplicates - 1.673 % (3,389)
+    * Outliers - 0.077 % (157)
+    * Blur - 0.512 % (1,037)
+    * Dark - 0.009 % (18)
+    * Mislabels - 0.006 % (13)
+    * Total - 2.277 % (4,614)
 | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8). | WIP | |
 [ADE20K](https://groups.csail.mit.edu/vision/datasets/ADE20K/) |
-    * Duplicates - 0.24% (12,345)
-    * Outliers - 0.85% (456)
-    * Broken - 0.85% (456)
-    * Blur - 0.85% (456)
-    * Dark - 0.85% (456)
-    * Bright - 0.85% (456)
+    * Duplicates - WIP % (WIP)
+    * Outliers - WIP % (WIP)
+    * Broken - WIP % (WIP)
+    * Blur - WIP % (WIP)
+    * Dark - WIP % (WIP)
+    * Bright - WIP % (WIP)
 | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8). | WIP | | [COCO]
 (https://cocodataset.org/#home) |
-    * Duplicates - 0.24% (12,345)
-    * Outliers - 0.85% (456)
-    * Broken - 0.85% (456)
-    * Blur - 0.85% (456)
-    * Dark - 0.85% (456)
-    * Bright - 0.85% (456)
+    * Duplicates - 0.123 % (201)
+    * Outliers - 0.087 % (143)
+    * Blur - 0.029 % (47)
+    * Dark - 0.106 % (174)
+    * Bright - 0.013 % (21)
+    * Total - 0.358 % (586)
 | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8). | WIP | Learn
 more on how we clean the datasets using our profilling tool [here](https://
 visual-layer.link). ## Installation **Option 1** - Install `vl_datasets`
-package from PyPI: ```shell pip install vl-datasets ``` **Option 2** - Install
-the bleeding edge version on GitHub: ``` pip install git+https://github.com/
-visual-layer/vl-datasets.git@main --upgrade ``` ## Usage To start using `vl-
-datasets`, import the clean version of the dataset with: ```python from
-vl_datasets import CleanFood101 ``` This should import the clean version of the
-`Food101` dataset. Next, you can load the dataset as a PyTorch `Dataset`.
-```python train_dataset = CleanFood101('./', split='train') valid_dataset =
-CleanFood101('./', split='test') ``` If you have a custom `.csv` file you can
-optionally pass in the file: ```python train_dataset = CleanFood101('./',
-split='train', exclude_csv='my-file.csv') ``` The filenames listed in the
-`.csv` will be excluded in the dataset. Next, you can load the train and
-validation datasets in a PyTorch training loop. See the [Learn from Examples]
-(#learn-from-examples) section to learn more. > **NOTE**: Sign up [here](https:
-//forms.gle/8jxPkyzeKj82kPed8) for free to be our beta testers and get full
-access to the all the `.csv` files for the dataset listed in this repo. With
-the dataset loaded you can train a model using PyTorch training loop. ## Learn
-from Examples
-                      * Dataset: CleanFood101       [./imgs/nbviewer_logo.svg]
+package from [PyPI](https://pypi.org/project/vl-datasets/): ```shell pip
+install vl-datasets ``` **Option 2** - Install the bleeding edge version on
+GitHub: ``` pip install git+https://github.com/visual-layer/vl-
+datasets.git@main --upgrade ``` ## Usage To start using `vl-datasets`, import
+the clean version of the dataset with: ```python from vl_datasets import
+VLFood101 ``` This should import the clean version of the `Food101` dataset.
+Next, you can load the dataset as a PyTorch `Dataset`. ```python train_dataset
+= VLFood101('./', split='train') valid_dataset = VLFood101('./', split='test')
+``` If you have a custom `.csv` file you can optionally pass in the file:
+```python train_dataset = VLFood101('./', split='train', exclude_csv='my-
+file.csv') ``` The filenames listed in the `.csv` will be excluded in the
+dataset. Next, you can load the train and validation datasets in a PyTorch
+training loop. See the [Learn from Examples](#learn-from-examples) section to
+learn more. > **NOTE**: Sign up [here](https://forms.gle/8jxPkyzeKj82kPed8) for
+free to be our beta testers and get full access to the all the `.csv` files for
+the dataset listed in this repo. With the dataset loaded you can train a model
+using PyTorch training loop. ## Learn from Examples
+                      * Dataset: VLFood101          [./imgs/nbviewer_logo.svg]
 [./imgs/food.jpg]     * Framework: PyTorch.          [./imgs/github_logo.png]
                       * Description: Load a dataset   [./imgs/colab_logo.png]
                         and train a PyTorch model.   [./imgs/kaggle_logo.png]
-                      * Dataset: CleanOxfordIIITPet [./imgs/nbviewer_logo.svg]
+                      * Dataset: VLOxfordIIITPet    [./imgs/nbviewer_logo.svg]
                       * Framework: fast.ai.          [./imgs/github_logo.png]
 [./imgs/pet.jpg]      * Description: Finetune a       [./imgs/colab_logo.png]
                         pretrained TIMM model using  [./imgs/kaggle_logo.png]
                         fastai.
 ## License `vl-datasets` is licensed under the Apache 2.0 License. See
 [LICENSE](./LICENSE). However, you are bound to the usage license of the
 original dataset. It is your responsibility to determine whether you have
 permission to use the dataset under the dataset's license. We provide no
-warranty or guarantee of accuracy or completeness. ## Getting Help Get help
-from the Visual Layer team or community members via the following channels - +
-[Slack](https://visualdatabase.slack.com/join/shared_invite/zt-19jaydbjn-
+warranty or guarantee of accuracy or completeness. ## Usage Tracking This
+repository incorporates usage tracking using [Sentry.io](https://sentry.io/) to
+monitor and collect valuable information about the usage of the application.
+Usage tracking allows us to gain insights into how the application is being
+used in real-world scenarios. It provides us with valuable information that
+helps in understanding user behavior, identifying potential issues, and making
+informed decisions to improve the application. We DO NOT collect folder names,
+user names, image names, image content and other personaly identifiable
+information. What data is tracked? + **Errors and Exceptions**: Sentry captures
+errors and exceptions that occur in the application, providing detailed stack
+traces and relevant information to help diagnose and fix issues. +
+**Performance Metrics**: Sentry collects performance metrics, such as response
+times, latency, and resource usage, enabling us to monitor and optimize the
+application's performance. Read more on Sentry's official [webpage](https://
+sentry.io/welcome/). ## Getting Help Get help from the Visual Layer team or
+community members via the following channels - + [Slack](https://
+visualdatabase.slack.com/join/shared_invite/zt-19jaydbjn-
 lNDEDkgvSI1QwbTXSY6dlA#/shared-invite/email). + GitHub [issues](https://
 github.com/visual-layer/vl-datasets/issues). + Discussion [forum](https://
 visual-layer.readme.io/discuss). ## About Visual-Layer
                               [Visual_Layer_Logo]
 Visual Layer is founded by the authors of [XGBoost](https://github.com/apache/
 tvm), [Apache TVM](https://github.com/apache/tvm) & [Turi Create](https://
 github.com/apple/turicreate) - [Danny Bickson](https://www.linkedin.com/in/dr-
```

## Comparing `vl_datasets-0.0.7.dist-info/RECORD` & `vl_datasets-0.0.8.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-vl_datasets/__init__.py,sha256=yv-iuT9v_UIquIEFyOlnCbn6fCGpZNoaVYdsGdZbYoo,141
-vl_datasets/food101.py,sha256=JX3uO3J234GIHFRZlBfg0Qt74AXqbbD0yCVErFZa1Gs,4734
+vl_datasets/__init__.py,sha256=5lSjEKpAZplC0Hgvbpfp4h_PsyugEhyNyr9tSDA3gsE,193
 vl_datasets/image_folder.py,sha256=qjhkPSbGeK5pcYL7t1md5b4RDUPUuo5MrCdtt0LrNYQ,2352
-vl_datasets/oxford_pet.py,sha256=8MwaNtwVqNSbxYMqgaEcVMw09n5qwYu3hHsrLnJDfis,4867
+vl_datasets/sentry.py,sha256=aDwvaApepFq2MQSXxxcIux684aG18v8tSO94-E8mzs8,4940
 vl_datasets/utils.py,sha256=JXQ9pMvbIwr92FYlNEZJXuScF9OkBrE8Bs8faWQoj_w,1056
-vl_datasets-0.0.7.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-vl_datasets-0.0.7.dist-info/METADATA,sha256=WsQPccBqbgjlm2D-wyUnxvsaRqc5GNg7gEz_yxrcY2g,17772
-vl_datasets-0.0.7.dist-info/WHEEL,sha256=YT1wPceIeW2Q5XD-ypzUqEKq0BMVsXhboTN8eU2aMIk,108
-vl_datasets-0.0.7.dist-info/top_level.txt,sha256=XbUC34rGj0OLHbugO4YnVobn0t02Nc-NM3F4pwV-j8g,12
-vl_datasets-0.0.7.dist-info/RECORD,,
+vl_datasets/vl_food101.py,sha256=kaIVaU-uPku5mwaSwTxxF0wJ6dX89hJAoKsBWjGAq0U,5099
+vl_datasets/vl_oxford_iiit_pet.py,sha256=PJb3cd-Bpyu7XzXBf0YYLl_bCFPQgSjxukLTAe_qY1k,5008
+vl_datasets-0.0.8.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+vl_datasets-0.0.8.dist-info/METADATA,sha256=SaDFMfVgm-8_BONchxXzzOcA6wTcigUrQrbeSKqzjUY,18977
+vl_datasets-0.0.8.dist-info/WHEEL,sha256=YT1wPceIeW2Q5XD-ypzUqEKq0BMVsXhboTN8eU2aMIk,108
+vl_datasets-0.0.8.dist-info/top_level.txt,sha256=XbUC34rGj0OLHbugO4YnVobn0t02Nc-NM3F4pwV-j8g,12
+vl_datasets-0.0.8.dist-info/RECORD,,
```

