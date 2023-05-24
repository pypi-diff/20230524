# Comparing `tmp/vl_datasets-0.0.8-py3.9-none-any.whl.zip` & `tmp/vl_datasets-0.0.9-py3.9-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 18216 bytes, number of entries: 11
--rw-r--r--  2.0 unx      193 b- defN 23-May-22 14:26 vl_datasets/__init__.py
--rw-r--r--  2.0 unx     2352 b- defN 23-May-22 14:26 vl_datasets/image_folder.py
--rw-r--r--  2.0 unx     4940 b- defN 23-May-22 14:26 vl_datasets/sentry.py
--rw-r--r--  2.0 unx     1056 b- defN 23-May-22 14:26 vl_datasets/utils.py
--rw-r--r--  2.0 unx     5099 b- defN 23-May-22 14:26 vl_datasets/vl_food101.py
--rw-r--r--  2.0 unx     5008 b- defN 23-May-22 14:26 vl_datasets/vl_oxford_iiit_pet.py
--rw-r--r--  2.0 unx    11357 b- defN 23-May-22 14:26 vl_datasets-0.0.8.dist-info/LICENSE
--rw-r--r--  2.0 unx    18977 b- defN 23-May-22 14:26 vl_datasets-0.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx      108 b- defN 23-May-22 14:26 vl_datasets-0.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-May-22 14:26 vl_datasets-0.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      899 b- defN 23-May-22 14:26 vl_datasets-0.0.8.dist-info/RECORD
-11 files, 50001 bytes uncompressed, 16702 bytes compressed:  66.6%
+Zip file size: 18301 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      193 b- defN 23-May-24 02:21 vl_datasets/__init__.py
+-rw-r--r--  2.0 unx     2352 b- defN 23-May-24 02:21 vl_datasets/image_folder.py
+-rw-r--r--  2.0 unx     4940 b- defN 23-May-24 02:21 vl_datasets/sentry.py
+-rw-r--r--  2.0 unx     1056 b- defN 23-May-24 02:21 vl_datasets/utils.py
+-rw-r--r--  2.0 unx     5099 b- defN 23-May-24 02:21 vl_datasets/vl_food101.py
+-rw-r--r--  2.0 unx     5008 b- defN 23-May-24 02:21 vl_datasets/vl_oxford_iiit_pet.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-May-24 02:21 vl_datasets-0.0.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx    19794 b- defN 23-May-24 02:21 vl_datasets-0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-May-24 02:21 vl_datasets-0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-May-24 02:21 vl_datasets-0.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      899 b- defN 23-May-24 02:21 vl_datasets-0.0.9.dist-info/RECORD
+11 files, 50818 bytes uncompressed, 16787 bytes compressed:  67.0%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: vl_datasets/vl_food101.py
 Comment: 
 
 Filename: vl_datasets/vl_oxford_iiit_pet.py
 Comment: 
 
-Filename: vl_datasets-0.0.8.dist-info/LICENSE
+Filename: vl_datasets-0.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: vl_datasets-0.0.8.dist-info/METADATA
+Filename: vl_datasets-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: vl_datasets-0.0.8.dist-info/WHEEL
+Filename: vl_datasets-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: vl_datasets-0.0.8.dist-info/top_level.txt
+Filename: vl_datasets-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: vl_datasets-0.0.8.dist-info/RECORD
+Filename: vl_datasets-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vl_datasets/__init__.py

```diff
@@ -1,7 +1,6 @@
-__version__ = '0.0.8'
+__version__ = '0.0.9'
+init_sentry()
 from .image_folder import CleanImageFolder
 from .vl_food101 import VLFood101
 from .vl_oxford_iiit_pet import VLOxfordIIITPet
 from .sentry import init_sentry
-
-init_sentry()
```

## Comparing `vl_datasets-0.0.8.dist-info/LICENSE` & `vl_datasets-0.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `vl_datasets-0.0.8.dist-info/METADATA` & `vl_datasets-0.0.9.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vl-datasets
-Version: 0.0.8
+Version: 0.0.9
 Summary: Open, Clean Datasets for Computer Vision.
 Home-page: https://github.com/visual-layer/vl-datasets
 Author: Visual Layer
 Author-email: info@visual-layer.com
 License: Apache-2.0
 Keywords: machine learning,computer vision,data-centric
 Platform: UNKNOWN
@@ -110,14 +110,15 @@
 
 + Duplicates.
 + Near Duplicates.
 + Broken images.
 + Outliers.
 + Dark/Bright/Blurry images.
 + Mislabels.
++ Data Leakage.
 
 ![image](./imgs/issues.png)
 
 
 
 
 ## Why?
@@ -142,29 +143,28 @@
 We're a startup and we'd like to offer free access to the datasets as much as we can afford to. But in doing so, we'd also need your support.
 
 We're offering select `.csv` files completely free with no strings attached. 
 For access to our complete dataset and exclusive beta features, all we ask is that you [sign up](https://forms.gle/8jxPkyzeKj82kPed8) to be a beta tester – it's completely free and your feedback will help shape the future of our platform. 
 
 Here is a table of widely used computer vision datasets, issues we found and a link to access the `.csv` file.
 
-
-| Dataset                                                                 | Issues                                                                                                                                                                                 | CSV                                                                                                | Usage                |
+| Dataset                                                                 | Issues                                                                                                                                                                                 | CSV                                                                                                | Import Statement                |
 |-------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------|----------------------|
-| [Food-101](./dataset_card/food101.md) | <ul><li>Duplicates - 0.233 % (235)</li><li>Outliers - 0.076 % (77)</li><li>Blur - Blur - 0.183 % (185)</li><li>Dark - 0.043 % (43)</li><li><b>Total</b> - 0.535 % (540)</li></ul> | Download [here](https://drive.google.com/uc?export=download&id=1ZG5GvU342l4YmSeYo6v6LeKbMM5fwjjw). | `from vl_datasets import VLFood101`       |
-| [Oxford-IIIT Pet](./dataset_card/oxford-iiit-pets.md)          | <ul><li>Duplicates - 1.021% (75)</li><li>Outliers - 0.095% (7)</li><li>Dark - 0.054% (4)</li><li><b>Total</b> - 1.170 % (86)</li></ul>         | Download [here](https://drive.google.com/uc?export=download&id=1OLa8k4NITnmCHjeByzvGaWt3W7k6R1QL). | `from vl_datasets import VLOxfordIIITPet` |
-| [LAION-1B](https://laion.ai/blog/laion-5b/)                             | <ul><li>Duplicates - WIP % (WIP)</li><li>Outliers - WIP % (WIP)</li><li>Broken - WIP % (WIP)</li><li>Blur - WIP % (WIP)</li><li>Dark - WIP % (WIP)</li><li>Bright - WIP % (WIP)</li></ul> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).                                        | WIP                  |
-| [ImageNet-21K](https://www.image-net.org/)                              | <ul><li>Duplicates - 11.853 % (1,559,120)</li><li>Outliers - 0.085 % (11,119)</li><li>Blur - 0.292 % (38,458)</li><li>Dark - 0.179 % (23,574)</li><li>Bright - 0.431 % (56,754)</li><li>Mislabels - 3.064 % (402,963)</li><li><b>Total</b> - 15.904 % (2,091,988)</li></ul> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).                                        | WIP                  |
-| [ImageNet-1K](https://www.image-net.org/)                               | <ul><li>Duplicates - 0.520 % (6,660)</li><li>Outliers - 0.090 % (1,150)</li><li>Blur - 0.200 % (2,554)</li><li>Dark - 0.244 % (2,997)</li><li>Bright - 0.058 % (746)</li><li>Mislabels - 0.119 % (1,518)</li><li><b>Total</b> - 1.221 % (15,625)</li></ul> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).                                        | WIP                  |
-| [KITTI](https://www.cvlibs.net/datasets/kitti/)                         | <ul><li>Duplicates - 15.294 % (2294)</li><li>Outliers - 0.107 % (16)</li><li><b>Total</b> - 15.401 % (2310)</li></ul> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).                                        | WIP                  |
-| [DeepFashion](http://mmlab.ie.cuhk.edu.hk/projects/DeepFashion.html)    | <ul><li>Duplicates - WIP % (WIP)</li><li>Outliers - WIP % (WIP)</li><li>Broken - WIP % (WIP)</li><li>Blur - WIP % (WIP)</li><li>Dark - WIP % (WIP)</li><li>Bright - WIP % (WIP)</li></ul> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).                                        | WIP                  |
+| [Food-101](./dataset_card/food101/card.md) | <ul><li>Duplicates - 0.233 % (235)</li><li>Outliers - 0.076 % (77)</li><li>Blur - Blur - 0.183 % (185)</li><li>Dark - 0.043 % (43)</li><li><b>Total</b> - 0.535 % (540)</li></ul><div align="right"><a href="./dataset_card/food101/card.md"><strong>More »</strong></a></div>| Download [here](https://drive.google.com/uc?export=download&id=1ZG5GvU342l4YmSeYo6v6LeKbMM5fwjjw). | `from vl_datasets import VLFood101`       |
+| [Oxford-IIIT Pet](./dataset_card/oxford-iiit-pets/card.md)          | <ul><li>Duplicates - 1.021% (75)</li><li>Outliers - 0.095% (7)</li><li>Dark - 0.054% (4)</li><li><b>Total</b> - 1.170 % (86)</li></ul><div align="right"><a href="./dataset_card/oxford-iiit-pets/card.md"><strong>More »</strong></a></div>         | Download [here](https://drive.google.com/uc?export=download&id=1OLa8k4NITnmCHjeByzvGaWt3W7k6R1QL). | `from vl_datasets import VLOxfordIIITPet` |
+| [LAION-1B](./dataset_card/laion-1b/card.md)                            | <ul><li>Duplicates - WIP % (WIP)</li><li>Outliers - WIP % (WIP)</li><li>Broken - WIP % (WIP)</li><li>Blur - WIP % (WIP)</li><li>Dark - WIP % (WIP)</li><li>Bright - WIP % (WIP)</li></ul><div align="right"><a href="./dataset_card/laion-1b/card.md"><strong>More »</strong></a></div> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).                                        | WIP                  |
+| [ImageNet-21K](./dataset_card/imagenet-1k/card.md)                              | <ul><li>Duplicates - 11.853 % (1,559,120)</li><li>Outliers - 0.085 % (11,119)</li><li>Blur - 0.292 % (38,458)</li><li>Dark - 0.179 % (23,574)</li><li>Bright - 0.431 % (56,754)</li><li>Mislabels - 3.064 % (402,963)</li><li><b>Total</b> - 15.904 % (2,091,988)</li></ul><div align="right"><a href="./dataset_card/imagenet-1k/card.md"><strong>More »</strong></a></div> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).                                        | WIP                  |
+| [ImageNet-1K](./dataset_card/imagenet-21k/card.md)                                | <ul><li>Duplicates - 0.520 % (6,660)</li><li>Outliers - 0.090 % (1,150)</li><li>Blur - 0.200 % (2,554)</li><li>Dark - 0.244 % (2,997)</li><li>Bright - 0.058 % (746)</li><li>Mislabels - 0.119 % (1,518)</li><li><b>Total</b> - 1.221 % (15,625)</li></ul><div align="right"><a href="./dataset_card/imagenet-21k/card.md"><strong>More »</strong></a></div> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).                                        | WIP                  |
+| [KITTI](./dataset_card/kitti/card.md)                          | <ul><li>Duplicates - 15.294 % (2294)</li><li>Outliers - 0.107 % (16)</li><li><b>Total</b> - 15.401 % (2310)</li></ul><div align="right"><a href="./dataset_card/kitti/card.md"><strong>More »</strong></a></div> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).                                        | WIP                  |
+| [DeepFashion](./dataset_card/deep-fashion/card.md)     | <ul><li>Duplicates - 5.114 % (14,772)</li><li>Outliers - 0.037 % (107)</li><b>Total</b> - 5.151 % (14,879)</li></ul><div align="right"><a href="./dataset_card/deep-fashion/card.md"><strong>More »</strong></a></div> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).                                        | WIP                  |
+| [CelebA-HQ](./dataset_card/celeb-a-hq/card.md)           | <ul><li>Duplicates - 1.673 % (3,389)</li><li>Outliers - 0.077 % (157)</li><li>Blur - 0.512 % (1,037)</li><li>Dark - 0.009 % (18)</li><li>Mislabels - 0.006 % (13)</li><li><b>Total</b> - 2.277 % (4,614)</li></ul><div align="right"><a href="./dataset_card/celeb-a-hq/card.md"><strong>More »</strong></a></div> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).                                        | WIP                  |
+| [COCO](./dataset_card/coco/card.md)                                   | <ul><li>Duplicates - 0.123 % (201)</li><li>Outliers - 0.087 % (143)</li><li>Blur - 0.029 % (47)</li><li>Dark - 0.106 % (174)</li><li>Bright - 0.013 % (21)</li><li><b>Total</b> - 0.358 % (586)</li></ul><div align="right"><a href="./dataset_card/coco/card.md"><strong>More »</strong></a></div> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).                                        | WIP                  |
+<!-- | [ADE20K](https://groups.csail.mit.edu/vision/datasets/ADE20K/)          | <ul><li>Duplicates - WIP % (WIP)</li><li>Outliers - WIP % (WIP)</li><li>Broken - WIP % (WIP)</li><li>Blur - WIP % (WIP)</li><li>Dark - WIP % (WIP)</li><li>Bright - WIP % (WIP)</li></ul> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).                                        | WIP                  |
 | [Places365](https://github.com/CSAILVision/places365)                   | <ul><li>Duplicates - WIP % (WIP)</li><li>Outliers - WIP % (WIP)</li><li>Broken - WIP % (WIP)</li><li>Blur - WIP % (WIP)</li><li>Dark - WIP % (WIP)</li><li>Bright - WIP % (WIP)</li></ul> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).                                        | WIP                  |
-| [CelebA-HQ](http://mmlab.ie.cuhk.edu.hk/projects/CelebA.html)           | <ul><li>Duplicates - 1.673 % (3,389)</li><li>Outliers - 0.077 % (157)</li><li>Blur - 0.512 % (1,037)</li><li>Dark - 0.009 % (18)</li><li>Mislabels - 0.006 % (13)</li><li><b>Total</b> - 2.277 % (4,614)</li></ul> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).                                        | WIP                  |
-| [ADE20K](https://groups.csail.mit.edu/vision/datasets/ADE20K/)          | <ul><li>Duplicates - WIP % (WIP)</li><li>Outliers - WIP % (WIP)</li><li>Broken - WIP % (WIP)</li><li>Blur - WIP % (WIP)</li><li>Dark - WIP % (WIP)</li><li>Bright - WIP % (WIP)</li></ul> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).                                        | WIP                  |
-| [COCO](https://cocodataset.org/#home)                                   | <ul><li>Duplicates - 0.123 % (201)</li><li>Outliers - 0.087 % (143)</li><li>Blur - 0.029 % (47)</li><li>Dark - 0.106 % (174)</li><li>Bright - 0.013 % (21)</li><li><b>Total</b> - 0.358 % (586)</li></ul> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).                                        | WIP                  |
-
+ -->
 
 
 Learn more on how we clean the datasets using our profilling tool [here](https://visual-layer.link).
 
 
 ## Installation
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vl-datasets Version: 0.0.8 Summary: Open, Clean
+Metadata-Version: 2.1 Name: vl-datasets Version: 0.0.9 Summary: Open, Clean
 Datasets for Computer Vision. Home-page: https://github.com/visual-layer/vl-
 datasets Author: Visual Layer Author-email: info@visual-layer.com License:
 Apache-2.0 Keywords: machine learning,computer vision,data-centric Platform:
 UNKNOWN Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Operating System
@@ -33,128 +33,120 @@
 computer vision datasets with only 2 lines of code. For example, to get access
 to the clean version of the [Food-101](https://data.vision.ee.ethz.ch/cvl/
 datasets_extra/food-101/) dataset simply run: ![image](./imgs/usage.png) We
 support some of the most widely used computer vision datasets. [Let us know]
 (https://forms.gle/8jxPkyzeKj82kPed8) if you have additional request to support
 a new dataset. All the datasets are analyzed for issues such as: + Duplicates.
 + Near Duplicates. + Broken images. + Outliers. + Dark/Bright/Blurry images. +
-Mislabels. ![image](./imgs/issues.png) ## Why? Computer vision is an exciting
-and rapidly advancing field, with new techniques and models emerging now and
-then. However, to develop and evaluate these models, it's essential to have
-reliable and standardized datasets to work with. Even with the recent success
-of generative models, data quality remains an issue that's [mainly overlooked]
-(https://medium.com/@amiralush/large-image-datasets-today-are-a-mess-
-e3ea4c9e8d22). Training models will erroneours data impacts model accuracy,
-incurs costs in time, storage and computational resources. We believe that
-access to clean and high-quality computer vision datasets leads to accurate,
-non-biased, and efficient model. By providing public access to `vl-datasets` we
-hope it helps advance the field of computer vision. ## Datasets & Access `vl-
-datasets` provides a convenient way to access the cleaned version of the
-datasets in Python. Alternatively, for each dataset in this repo, we provide a
-`.csv` file that lists the problematic images from the dataset. You can use the
-listed images in the `.csv` to improve the model by re-labeling the them or
-just simply remove it from the dataset. We're a startup and we'd like to offer
-free access to the datasets as much as we can afford to. But in doing so, we'd
-also need your support. We're offering select `.csv` files completely free with
-no strings attached. For access to our complete dataset and exclusive beta
-features, all we ask is that you [sign up](https://forms.gle/8jxPkyzeKj82kPed8)
-to be a beta tester â it's completely free and your feedback will help shape
-the future of our platform. Here is a table of widely used computer vision
-datasets, issues we found and a link to access the `.csv` file. | Dataset |
-Issues | CSV | Usage | |-------------------------------------------------------
-------------------|------------------------------------------------------------
+Mislabels. + Data Leakage. ![image](./imgs/issues.png) ## Why? Computer vision
+is an exciting and rapidly advancing field, with new techniques and models
+emerging now and then. However, to develop and evaluate these models, it's
+essential to have reliable and standardized datasets to work with. Even with
+the recent success of generative models, data quality remains an issue that's
+[mainly overlooked](https://medium.com/@amiralush/large-image-datasets-today-
+are-a-mess-e3ea4c9e8d22). Training models will erroneours data impacts model
+accuracy, incurs costs in time, storage and computational resources. We believe
+that access to clean and high-quality computer vision datasets leads to
+accurate, non-biased, and efficient model. By providing public access to `vl-
+datasets` we hope it helps advance the field of computer vision. ## Datasets &
+Access `vl-datasets` provides a convenient way to access the cleaned version of
+the datasets in Python. Alternatively, for each dataset in this repo, we
+provide a `.csv` file that lists the problematic images from the dataset. You
+can use the listed images in the `.csv` to improve the model by re-labeling the
+them or just simply remove it from the dataset. We're a startup and we'd like
+to offer free access to the datasets as much as we can afford to. But in doing
+so, we'd also need your support. We're offering select `.csv` files completely
+free with no strings attached. For access to our complete dataset and exclusive
+beta features, all we ask is that you [sign up](https://forms.gle/
+8jxPkyzeKj82kPed8) to be a beta tester â it's completely free and your
+feedback will help shape the future of our platform. Here is a table of widely
+used computer vision datasets, issues we found and a link to access the `.csv`
+file. | Dataset | Issues | CSV | Import Statement | |--------------------------
+-----------------------------------------------|-------------------------------
 -------------------------------------------------------------------------------
----------------------------------------------------|---------------------------
--------------------------------------------------------------------------|-----
------------------| | [Food-101](./dataset_card/food101.md) |
+-------------------------------------------------------------------------------
+-|-----------------------------------------------------------------------------
+-----------------------|----------------------| | [Food-101](./dataset_card/
+food101/card.md) |
     * Duplicates - 0.233 % (235)
     * Outliers - 0.076 % (77)
     * Blur - Blur - 0.183 % (185)
     * Dark - 0.043 % (43)
     * Total - 0.535 % (540)
+                                                                        More_Â»
 | Download [here](https://drive.google.com/
 uc?export=download&id=1ZG5GvU342l4YmSeYo6v6LeKbMM5fwjjw). | `from vl_datasets
-import VLFood101` | | [Oxford-IIIT Pet](./dataset_card/oxford-iiit-pets.md) |
+import VLFood101` | | [Oxford-IIIT Pet](./dataset_card/oxford-iiit-pets/
+card.md) |
     * Duplicates - 1.021% (75)
     * Outliers - 0.095% (7)
     * Dark - 0.054% (4)
     * Total - 1.170 % (86)
+                                                                        More_Â»
 | Download [here](https://drive.google.com/
 uc?export=download&id=1OLa8k4NITnmCHjeByzvGaWt3W7k6R1QL). | `from vl_datasets
-import VLOxfordIIITPet` | | [LAION-1B](https://laion.ai/blog/laion-5b/) |
+import VLOxfordIIITPet` | | [LAION-1B](./dataset_card/laion-1b/card.md) |
     * Duplicates - WIP % (WIP)
     * Outliers - WIP % (WIP)
     * Broken - WIP % (WIP)
     * Blur - WIP % (WIP)
     * Dark - WIP % (WIP)
     * Bright - WIP % (WIP)
+                                                                        More_Â»
 | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8). | WIP | |
-[ImageNet-21K](https://www.image-net.org/) |
+[ImageNet-21K](./dataset_card/imagenet-1k/card.md) |
     * Duplicates - 11.853 % (1,559,120)
     * Outliers - 0.085 % (11,119)
     * Blur - 0.292 % (38,458)
     * Dark - 0.179 % (23,574)
     * Bright - 0.431 % (56,754)
     * Mislabels - 3.064 % (402,963)
     * Total - 15.904 % (2,091,988)
+                                                                        More_Â»
 | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8). | WIP | |
-[ImageNet-1K](https://www.image-net.org/) |
+[ImageNet-1K](./dataset_card/imagenet-21k/card.md) |
     * Duplicates - 0.520 % (6,660)
     * Outliers - 0.090 % (1,150)
     * Blur - 0.200 % (2,554)
     * Dark - 0.244 % (2,997)
     * Bright - 0.058 % (746)
     * Mislabels - 0.119 % (1,518)
     * Total - 1.221 % (15,625)
+                                                                        More_Â»
 | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8). | WIP | | [KITTI]
-(https://www.cvlibs.net/datasets/kitti/) |
+(./dataset_card/kitti/card.md) |
     * Duplicates - 15.294 % (2294)
     * Outliers - 0.107 % (16)
     * Total - 15.401 % (2310)
+                                                                        More_Â»
 | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8). | WIP | |
-[DeepFashion](http://mmlab.ie.cuhk.edu.hk/projects/DeepFashion.html) |
-    * Duplicates - WIP % (WIP)
-    * Outliers - WIP % (WIP)
-    * Broken - WIP % (WIP)
-    * Blur - WIP % (WIP)
-    * Dark - WIP % (WIP)
-    * Bright - WIP % (WIP)
+[DeepFashion](./dataset_card/deep-fashion/card.md) |
+    * Duplicates - 5.114 % (14,772)
+    * Outliers - 0.037 % (107)
+    * Total - 5.151 % (14,879)
+                                                                        More_Â»
 | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8). | WIP | |
-[Places365](https://github.com/CSAILVision/places365) |
-    * Duplicates - WIP % (WIP)
-    * Outliers - WIP % (WIP)
-    * Broken - WIP % (WIP)
-    * Blur - WIP % (WIP)
-    * Dark - WIP % (WIP)
-    * Bright - WIP % (WIP)
-| Request access [here](https://forms.gle/8jxPkyzeKj82kPed8). | WIP | |
-[CelebA-HQ](http://mmlab.ie.cuhk.edu.hk/projects/CelebA.html) |
+[CelebA-HQ](./dataset_card/celeb-a-hq/card.md) |
     * Duplicates - 1.673 % (3,389)
     * Outliers - 0.077 % (157)
     * Blur - 0.512 % (1,037)
     * Dark - 0.009 % (18)
     * Mislabels - 0.006 % (13)
     * Total - 2.277 % (4,614)
-| Request access [here](https://forms.gle/8jxPkyzeKj82kPed8). | WIP | |
-[ADE20K](https://groups.csail.mit.edu/vision/datasets/ADE20K/) |
-    * Duplicates - WIP % (WIP)
-    * Outliers - WIP % (WIP)
-    * Broken - WIP % (WIP)
-    * Blur - WIP % (WIP)
-    * Dark - WIP % (WIP)
-    * Bright - WIP % (WIP)
+                                                                        More_Â»
 | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8). | WIP | | [COCO]
-(https://cocodataset.org/#home) |
+(./dataset_card/coco/card.md) |
     * Duplicates - 0.123 % (201)
     * Outliers - 0.087 % (143)
     * Blur - 0.029 % (47)
     * Dark - 0.106 % (174)
     * Bright - 0.013 % (21)
     * Total - 0.358 % (586)
-| Request access [here](https://forms.gle/8jxPkyzeKj82kPed8). | WIP | Learn
+                                                                        More_Â»
+| Request access [here](https://forms.gle/8jxPkyzeKj82kPed8). | WIP |  Learn
 more on how we clean the datasets using our profilling tool [here](https://
 visual-layer.link). ## Installation **Option 1** - Install `vl_datasets`
 package from [PyPI](https://pypi.org/project/vl-datasets/): ```shell pip
 install vl-datasets ``` **Option 2** - Install the bleeding edge version on
 GitHub: ``` pip install git+https://github.com/visual-layer/vl-
 datasets.git@main --upgrade ``` ## Usage To start using `vl-datasets`, import
 the clean version of the dataset with: ```python from vl_datasets import
```

## Comparing `vl_datasets-0.0.8.dist-info/RECORD` & `vl_datasets-0.0.9.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-vl_datasets/__init__.py,sha256=5lSjEKpAZplC0Hgvbpfp4h_PsyugEhyNyr9tSDA3gsE,193
+vl_datasets/__init__.py,sha256=3F0M0HNOUbubEz96EBDOV7vHK6NpAGjKiOlGpbNNHoo,193
 vl_datasets/image_folder.py,sha256=qjhkPSbGeK5pcYL7t1md5b4RDUPUuo5MrCdtt0LrNYQ,2352
 vl_datasets/sentry.py,sha256=aDwvaApepFq2MQSXxxcIux684aG18v8tSO94-E8mzs8,4940
 vl_datasets/utils.py,sha256=JXQ9pMvbIwr92FYlNEZJXuScF9OkBrE8Bs8faWQoj_w,1056
 vl_datasets/vl_food101.py,sha256=kaIVaU-uPku5mwaSwTxxF0wJ6dX89hJAoKsBWjGAq0U,5099
 vl_datasets/vl_oxford_iiit_pet.py,sha256=PJb3cd-Bpyu7XzXBf0YYLl_bCFPQgSjxukLTAe_qY1k,5008
-vl_datasets-0.0.8.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-vl_datasets-0.0.8.dist-info/METADATA,sha256=SaDFMfVgm-8_BONchxXzzOcA6wTcigUrQrbeSKqzjUY,18977
-vl_datasets-0.0.8.dist-info/WHEEL,sha256=YT1wPceIeW2Q5XD-ypzUqEKq0BMVsXhboTN8eU2aMIk,108
-vl_datasets-0.0.8.dist-info/top_level.txt,sha256=XbUC34rGj0OLHbugO4YnVobn0t02Nc-NM3F4pwV-j8g,12
-vl_datasets-0.0.8.dist-info/RECORD,,
+vl_datasets-0.0.9.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+vl_datasets-0.0.9.dist-info/METADATA,sha256=__lc5Vl2ZBQemjKNOhUfwz4LAw_2GGADC2Ef6at_6OQ,19794
+vl_datasets-0.0.9.dist-info/WHEEL,sha256=YT1wPceIeW2Q5XD-ypzUqEKq0BMVsXhboTN8eU2aMIk,108
+vl_datasets-0.0.9.dist-info/top_level.txt,sha256=XbUC34rGj0OLHbugO4YnVobn0t02Nc-NM3F4pwV-j8g,12
+vl_datasets-0.0.9.dist-info/RECORD,,
```

