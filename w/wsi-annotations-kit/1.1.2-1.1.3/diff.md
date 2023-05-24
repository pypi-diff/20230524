# Comparing `tmp/wsi-annotations-kit-1.1.2.tar.gz` & `tmp/wsi-annotations-kit-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\wsi-annotations-kit-1.1.2.tar", last modified: Wed May 24 19:04:08 2023, max compression
+gzip compressed data, was "dist\wsi-annotations-kit-1.1.3.tar", last modified: Wed May 24 19:06:53 2023, max compression
```

## Comparing `wsi-annotations-kit-1.1.2.tar` & `wsi-annotations-kit-1.1.3.tar`

### file list

```diff
@@ -1,15 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 19:04:08.000000 wsi-annotations-kit-1.1.2/
--rw-rw-rw-   0        0        0     1086 2023-05-17 21:36:33.000000 wsi-annotations-kit-1.1.2/LICENSE
--rw-rw-rw-   0        0        0      745 2023-05-24 19:04:08.000000 wsi-annotations-kit-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      260 2023-05-24 18:16:19.000000 wsi-annotations-kit-1.1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-24 19:04:08.000000 wsi-annotations-kit-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      841 2023-05-24 19:03:57.000000 wsi-annotations-kit-1.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-24 19:04:08.000000 wsi-annotations-kit-1.1.2/wsi_annotations_kit/
--rw-rw-rw-   0        0        0        0 2023-05-17 21:25:38.000000 wsi-annotations-kit-1.1.2/wsi_annotations_kit/__init__.py
--rw-rw-rw-   0        0        0    21082 2023-05-19 18:42:29.000000 wsi-annotations-kit-1.1.2/wsi_annotations_kit/wsi_annotations_kit.py
-drwxrwxrwx   0        0        0        0 2023-05-24 19:04:08.000000 wsi-annotations-kit-1.1.2/wsi_annotations_kit.egg-info/
--rw-rw-rw-   0        0        0      745 2023-05-24 19:04:08.000000 wsi-annotations-kit-1.1.2/wsi_annotations_kit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2023-05-24 19:04:08.000000 wsi-annotations-kit-1.1.2/wsi_annotations_kit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 19:04:08.000000 wsi-annotations-kit-1.1.2/wsi_annotations_kit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-05-24 19:04:08.000000 wsi-annotations-kit-1.1.2/wsi_annotations_kit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-05-24 19:04:08.000000 wsi-annotations-kit-1.1.2/wsi_annotations_kit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-24 19:06:53.000000 wsi-annotations-kit-1.1.3/
+-rw-rw-rw-   0        0        0     1086 2023-05-17 21:36:33.000000 wsi-annotations-kit-1.1.3/LICENSE
+-rw-rw-rw-   0        0        0      745 2023-05-24 19:06:52.000000 wsi-annotations-kit-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2023-05-24 18:16:19.000000 wsi-annotations-kit-1.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-24 19:06:53.000000 wsi-annotations-kit-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      866 2023-05-24 19:06:14.000000 wsi-annotations-kit-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 19:06:52.000000 wsi-annotations-kit-1.1.3/wsi_annotations_kit.egg-info/
+-rw-rw-rw-   0        0        0      745 2023-05-24 19:06:52.000000 wsi-annotations-kit-1.1.3/wsi_annotations_kit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2023-05-24 19:06:52.000000 wsi-annotations-kit-1.1.3/wsi_annotations_kit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 19:06:52.000000 wsi-annotations-kit-1.1.3/wsi_annotations_kit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-24 19:06:52.000000 wsi-annotations-kit-1.1.3/wsi_annotations_kit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 19:06:52.000000 wsi-annotations-kit-1.1.3/wsi_annotations_kit.egg-info/top_level.txt
```

### Comparing `wsi-annotations-kit-1.1.2/LICENSE` & `wsi-annotations-kit-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wsi-annotations-kit-1.1.2/PKG-INFO` & `wsi-annotations-kit-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wsi-annotations-kit
-Version: 1.1.2
+Version: 1.1.3
 Summary: Utility functions for generating, saving, and converting annotation files
 Home-page: https://github.com/spborder/wsi_annotations_kit
 Author: Sam Border
 Author-email: sam.border2256@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `wsi-annotations-kit-1.1.2/setup.py` & `wsi-annotations-kit-1.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="wsi-annotations-kit",
-    version="1.1.2",
+    version="1.1.3",
     author="Sam Border",
     author_email="sam.border2256@gmail.com",
     description="Utility functions for generating, saving, and converting annotation files",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/spborder/wsi_annotations_kit",
     install_requires=[
         "lxml",
         "geojson",
         "shapely",
         "tqdm",
         "numpy",
-        "uuid"
+        "uuid",
+        "scikit-image"
     ],
     packages=setuptools.find_packages(),
     classifiers=(
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ),
```

### Comparing `wsi-annotations-kit-1.1.2/wsi_annotations_kit.egg-info/PKG-INFO` & `wsi-annotations-kit-1.1.3/wsi_annotations_kit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wsi-annotations-kit
-Version: 1.1.2
+Version: 1.1.3
 Summary: Utility functions for generating, saving, and converting annotation files
 Home-page: https://github.com/spborder/wsi_annotations_kit
 Author: Sam Border
 Author-email: sam.border2256@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

