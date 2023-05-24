# Comparing `tmp/wsi-annotations-kit-1.0.1.1.tar.gz` & `tmp/wsi-annotations-kit-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\wsi-annotations-kit-1.0.1.1.tar", last modified: Wed May 24 18:26:36 2023, max compression
+gzip compressed data, was "dist\wsi-annotations-kit-1.1.tar", last modified: Wed May 24 18:49:44 2023, max compression
```

## Comparing `wsi-annotations-kit-1.0.1.1.tar` & `wsi-annotations-kit-1.1.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 18:26:36.000000 wsi-annotations-kit-1.0.1.1/
--rw-rw-rw-   0        0        0     1086 2023-05-17 21:36:33.000000 wsi-annotations-kit-1.0.1.1/LICENSE
--rw-rw-rw-   0        0        0      747 2023-05-24 18:26:36.000000 wsi-annotations-kit-1.0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      260 2023-05-24 18:16:19.000000 wsi-annotations-kit-1.0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-24 18:26:36.000000 wsi-annotations-kit-1.0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      703 2023-05-24 18:25:39.000000 wsi-annotations-kit-1.0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-24 18:26:36.000000 wsi-annotations-kit-1.0.1.1/wsi_annotations_kit.egg-info/
--rw-rw-rw-   0        0        0      747 2023-05-24 18:26:35.000000 wsi-annotations-kit-1.0.1.1/wsi_annotations_kit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      198 2023-05-24 18:26:35.000000 wsi-annotations-kit-1.0.1.1/wsi_annotations_kit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 18:26:35.000000 wsi-annotations-kit-1.0.1.1/wsi_annotations_kit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 18:26:35.000000 wsi-annotations-kit-1.0.1.1/wsi_annotations_kit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-24 18:49:44.000000 wsi-annotations-kit-1.1/
+-rw-rw-rw-   0        0        0     1086 2023-05-17 21:36:33.000000 wsi-annotations-kit-1.1/LICENSE
+-rw-rw-rw-   0        0        0      743 2023-05-24 18:49:44.000000 wsi-annotations-kit-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2023-05-24 18:16:19.000000 wsi-annotations-kit-1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-24 18:49:44.000000 wsi-annotations-kit-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      699 2023-05-24 18:49:01.000000 wsi-annotations-kit-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 18:49:44.000000 wsi-annotations-kit-1.1/wsi_annotations_kit/
+-rw-rw-rw-   0        0        0        0 2023-05-17 21:25:38.000000 wsi-annotations-kit-1.1/wsi_annotations_kit/__init__.py
+-rw-rw-rw-   0        0        0    21082 2023-05-19 18:42:29.000000 wsi-annotations-kit-1.1/wsi_annotations_kit/wsi_annotations_kit.py
+drwxrwxrwx   0        0        0        0 2023-05-24 18:49:44.000000 wsi-annotations-kit-1.1/wsi_annotations_kit.egg-info/
+-rw-rw-rw-   0        0        0      743 2023-05-24 18:49:43.000000 wsi-annotations-kit-1.1/wsi_annotations_kit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-05-24 18:49:44.000000 wsi-annotations-kit-1.1/wsi_annotations_kit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 18:49:43.000000 wsi-annotations-kit-1.1/wsi_annotations_kit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-05-24 18:49:43.000000 wsi-annotations-kit-1.1/wsi_annotations_kit.egg-info/top_level.txt
```

### Comparing `wsi-annotations-kit-1.0.1.1/LICENSE` & `wsi-annotations-kit-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wsi-annotations-kit-1.0.1.1/PKG-INFO` & `wsi-annotations-kit-1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wsi-annotations-kit
-Version: 1.0.1.1
+Version: 1.1
 Summary: Utility functions for generating, saving, and converting annotation files
 Home-page: https://github.com/spborder/wsi_annotations_kit
 Author: Sam Border
 Author-email: sam.border2256@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `wsi-annotations-kit-1.0.1.1/setup.py` & `wsi-annotations-kit-1.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="wsi-annotations-kit",
-    version="1.0.1.1",
+    version="1.1",
     author="Sam Border",
     author_email="sam.border2256@gmail.com",
     description="Utility functions for generating, saving, and converting annotation files",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/spborder/wsi_annotations_kit",
     packages=setuptools.find_packages(),
```

### Comparing `wsi-annotations-kit-1.0.1.1/wsi_annotations_kit.egg-info/PKG-INFO` & `wsi-annotations-kit-1.1/wsi_annotations_kit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wsi-annotations-kit
-Version: 1.0.1.1
+Version: 1.1
 Summary: Utility functions for generating, saving, and converting annotation files
 Home-page: https://github.com/spborder/wsi_annotations_kit
 Author: Sam Border
 Author-email: sam.border2256@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

