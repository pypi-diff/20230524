# Comparing `tmp/closet-engine-cv-0.0.6.tar.gz` & `tmp/closet-engine-cv-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "closet-engine-cv-0.0.6.tar", last modified: Thu Jan  5 12:40:57 2023, max compression
+gzip compressed data, was "closet-engine-cv-0.0.7.tar", last modified: Wed May 24 03:44:30 2023, max compression
```

## Comparing `closet-engine-cv-0.0.6.tar` & `closet-engine-cv-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ingunjon   (501) staff       (20)        0 2023-01-05 12:40:57.448561 closet-engine-cv-0.0.6/
--rw-r--r--   0 ingunjon   (501) staff       (20)     1073 2021-01-31 13:35:28.000000 closet-engine-cv-0.0.6/LICENSE
--rw-r--r--   0 ingunjon   (501) staff       (20)      610 2023-01-05 12:40:57.448197 closet-engine-cv-0.0.6/PKG-INFO
--rw-r--r--   0 ingunjon   (501) staff       (20)      186 2023-01-05 12:39:56.000000 closet-engine-cv-0.0.6/README.md
-drwxr-xr-x   0 ingunjon   (501) staff       (20)        0 2023-01-05 12:40:57.447174 closet-engine-cv-0.0.6/closet_engine_cv.egg-info/
--rw-r--r--   0 ingunjon   (501) staff       (20)      610 2023-01-05 12:40:57.000000 closet-engine-cv-0.0.6/closet_engine_cv.egg-info/PKG-INFO
--rw-r--r--   0 ingunjon   (501) staff       (20)      284 2023-01-05 12:40:57.000000 closet-engine-cv-0.0.6/closet_engine_cv.egg-info/SOURCES.txt
--rw-r--r--   0 ingunjon   (501) staff       (20)        1 2023-01-05 12:40:57.000000 closet-engine-cv-0.0.6/closet_engine_cv.egg-info/dependency_links.txt
--rw-r--r--   0 ingunjon   (501) staff       (20)       46 2023-01-05 12:40:57.000000 closet-engine-cv-0.0.6/closet_engine_cv.egg-info/entry_points.txt
--rw-r--r--   0 ingunjon   (501) staff       (20)       14 2023-01-05 12:40:57.000000 closet-engine-cv-0.0.6/closet_engine_cv.egg-info/requires.txt
--rw-r--r--   0 ingunjon   (501) staff       (20)        4 2023-01-05 12:40:57.000000 closet-engine-cv-0.0.6/closet_engine_cv.egg-info/top_level.txt
-drwxr-xr-x   0 ingunjon   (501) staff       (20)        0 2023-01-05 12:40:57.447672 closet-engine-cv-0.0.6/pkg/
--rw-r--r--   0 ingunjon   (501) staff       (20)     1275 2023-01-05 12:39:57.000000 closet-engine-cv-0.0.6/pkg/__init__.py
--rw-r--r--   0 ingunjon   (501) staff       (20)       38 2023-01-05 12:40:57.448675 closet-engine-cv-0.0.6/setup.cfg
--rwxr-xr-x   0 ingunjon   (501) staff       (20)      778 2022-12-08 08:55:00.000000 closet-engine-cv-0.0.6/setup.py
+drwxr-xr-x   0 cloremus   (501) staff       (20)        0 2023-05-24 03:44:30.092869 closet-engine-cv-0.0.7/
+-rw-r--r--   0 cloremus   (501) staff       (20)     1073 2023-05-23 21:52:08.000000 closet-engine-cv-0.0.7/LICENSE
+-rw-r--r--   0 cloremus   (501) staff       (20)      568 2023-05-24 03:44:30.092747 closet-engine-cv-0.0.7/PKG-INFO
+-rw-r--r--   0 cloremus   (501) staff       (20)      144 2023-05-23 21:52:08.000000 closet-engine-cv-0.0.7/README.md
+drwxr-xr-x   0 cloremus   (501) staff       (20)        0 2023-05-24 03:44:30.092352 closet-engine-cv-0.0.7/closet_engine_cv.egg-info/
+-rw-r--r--   0 cloremus   (501) staff       (20)      568 2023-05-24 03:44:30.000000 closet-engine-cv-0.0.7/closet_engine_cv.egg-info/PKG-INFO
+-rw-r--r--   0 cloremus   (501) staff       (20)      284 2023-05-24 03:44:30.000000 closet-engine-cv-0.0.7/closet_engine_cv.egg-info/SOURCES.txt
+-rw-r--r--   0 cloremus   (501) staff       (20)        1 2023-05-24 03:44:30.000000 closet-engine-cv-0.0.7/closet_engine_cv.egg-info/dependency_links.txt
+-rw-r--r--   0 cloremus   (501) staff       (20)       46 2023-05-24 03:44:30.000000 closet-engine-cv-0.0.7/closet_engine_cv.egg-info/entry_points.txt
+-rw-r--r--   0 cloremus   (501) staff       (20)       14 2023-05-24 03:44:30.000000 closet-engine-cv-0.0.7/closet_engine_cv.egg-info/requires.txt
+-rw-r--r--   0 cloremus   (501) staff       (20)        4 2023-05-24 03:44:30.000000 closet-engine-cv-0.0.7/closet_engine_cv.egg-info/top_level.txt
+drwxr-xr-x   0 cloremus   (501) staff       (20)        0 2023-05-24 03:44:30.092554 closet-engine-cv-0.0.7/pkg/
+-rw-r--r--   0 cloremus   (501) staff       (20)     1276 2023-05-23 22:25:08.000000 closet-engine-cv-0.0.7/pkg/__init__.py
+-rw-r--r--   0 cloremus   (501) staff       (20)       38 2023-05-24 03:44:30.092908 closet-engine-cv-0.0.7/setup.cfg
+-rwxr-xr-x   0 cloremus   (501) staff       (20)      778 2023-05-24 00:03:16.000000 closet-engine-cv-0.0.7/setup.py
```

### Comparing `closet-engine-cv-0.0.6/LICENSE` & `closet-engine-cv-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `closet-engine-cv-0.0.6/PKG-INFO` & `closet-engine-cv-0.0.7/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 Metadata-Version: 2.1
 Name: closet-engine-cv
-Version: 0.0.6
+Version: 0.0.7
 Summary: A small example package
 Home-page: https://github.com/pypa/sampleproject
 Author: Ingun Jon
 Author-email: ingun37@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 OpenCV tool for CLO web engine E2E Test
 
-https://pypi.org/project/closet-viewer-cv/
+https://pypi.org/project/closet-engine-cv/
 
 ## Install
 
 ```
-pip3 install "closet-viewer-cv==0.0.6"
+pip3 install "closet-engine-cv==0.0.6"
 ```
-
-## TODO
-
-Change name to closet-engine-cv
```

### Comparing `closet-engine-cv-0.0.6/closet_engine_cv.egg-info/PKG-INFO` & `closet-engine-cv-0.0.7/closet_engine_cv.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 Metadata-Version: 2.1
 Name: closet-engine-cv
-Version: 0.0.6
+Version: 0.0.7
 Summary: A small example package
 Home-page: https://github.com/pypa/sampleproject
 Author: Ingun Jon
 Author-email: ingun37@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 OpenCV tool for CLO web engine E2E Test
 
-https://pypi.org/project/closet-viewer-cv/
+https://pypi.org/project/closet-engine-cv/
 
 ## Install
 
 ```
-pip3 install "closet-viewer-cv==0.0.6"
+pip3 install "closet-engine-cv==0.0.6"
 ```
-
-## TODO
-
-Change name to closet-engine-cv
```

### Comparing `closet-engine-cv-0.0.6/pkg/__init__.py` & `closet-engine-cv-0.0.7/pkg/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     combined_path:str = args.combined[0]
 
     # print(x_path, y_path, diff_path, highlight_path, combined_path)
 
 
     x = cv2.imread(x_path)
     y = cv2.imread(y_path)
-    diff = np.absolute(x-y)
+    diff = cv2.absdiff(x, y)
     res, thres_diff = cv2.threshold(diff, 0, 255, cv2.THRESH_BINARY)
     combined = np.concatenate((x, y, diff, thres_diff,), axis=1)
 
     # x_base = splitext(basename(x_path))[0]
     # y_base = splitext(basename(y_path))[0]
     # y_to_x = y_base + '-' + x_base
     cv2.imwrite(diff_path, diff)
```

### Comparing `closet-engine-cv-0.0.6/setup.py` & `closet-engine-cv-0.0.7/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="closet-engine-cv",
-    version="0.0.6",
+    version="0.0.7",
     author="Ingun Jon",
     author_email="ingun37@gmail.com",
     description="A small example package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pypa/sampleproject",
     packages=setuptools.find_packages(),
```

