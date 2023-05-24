# Comparing `tmp/pvbm-2.1.6.tar.gz` & `tmp/pvbm-2.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pvbm-2.1.6.tar", last modified: Wed May 24 15:32:41 2023, max compression
+gzip compressed data, was "pvbm-2.1.7.tar", last modified: Wed May 24 15:39:55 2023, max compression
```

## Comparing `pvbm-2.1.6.tar` & `pvbm-2.1.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-05-24 15:32:41.024038 pvbm-2.1.6/
--rw-r--r--   0 jonathanfhima   (501) staff       (20)     4040 2023-05-24 15:32:41.023920 pvbm-2.1.6/PKG-INFO
-drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-05-24 15:32:41.021901 pvbm-2.1.6/PVBM/
--rw-r--r--   0 jonathanfhima   (501) staff       (20)    11109 2023-05-17 16:00:48.000000 pvbm-2.1.6/PVBM/FractalAnalysis.py
--rw-r--r--   0 jonathanfhima   (501) staff       (20)     4844 2023-05-24 15:31:59.000000 pvbm-2.1.6/PVBM/GeometricalAnalysis.py
--rw-r--r--   0 jonathanfhima   (501) staff       (20)        1 2023-05-04 16:40:03.000000 pvbm-2.1.6/PVBM/__init__.py
-drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-05-24 15:32:41.023015 pvbm-2.1.6/PVBM/helpers/
--rw-r--r--   0 jonathanfhima   (501) staff       (20)        1 2023-05-04 16:40:03.000000 pvbm-2.1.6/PVBM/helpers/__init__.py
--rw-r--r--   0 jonathanfhima   (501) staff       (20)     5391 2023-04-15 11:00:40.000000 pvbm-2.1.6/PVBM/helpers/branching2.py
--rw-r--r--   0 jonathanfhima   (501) staff       (20)     6285 2023-05-17 15:55:49.000000 pvbm-2.1.6/PVBM/helpers/branching_angle.py
--rw-r--r--   0 jonathanfhima   (501) staff       (20)     1209 2023-05-24 15:27:09.000000 pvbm-2.1.6/PVBM/helpers/perimeter.py
--rw-r--r--   0 jonathanfhima   (501) staff       (20)     2265 2023-04-13 10:18:09.000000 pvbm-2.1.6/PVBM/helpers/tortuosity.py
--rw-r--r--   0 jonathanfhima   (501) staff       (20)     3778 2023-05-17 15:59:09.000000 pvbm-2.1.6/README.md
-drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-05-24 15:32:41.023754 pvbm-2.1.6/pvbm.egg-info/
--rw-r--r--   0 jonathanfhima   (501) staff       (20)     4040 2023-05-24 15:32:40.000000 pvbm-2.1.6/pvbm.egg-info/PKG-INFO
--rw-r--r--   0 jonathanfhima   (501) staff       (20)      363 2023-05-24 15:32:41.000000 pvbm-2.1.6/pvbm.egg-info/SOURCES.txt
--rw-r--r--   0 jonathanfhima   (501) staff       (20)        1 2023-05-24 15:32:40.000000 pvbm-2.1.6/pvbm.egg-info/dependency_links.txt
--rw-r--r--   0 jonathanfhima   (501) staff       (20)       32 2023-05-24 15:32:40.000000 pvbm-2.1.6/pvbm.egg-info/requires.txt
--rw-r--r--   0 jonathanfhima   (501) staff       (20)        5 2023-05-24 15:32:40.000000 pvbm-2.1.6/pvbm.egg-info/top_level.txt
--rw-r--r--   0 jonathanfhima   (501) staff       (20)       38 2023-05-24 15:32:41.024072 pvbm-2.1.6/setup.cfg
--rw-r--r--   0 jonathanfhima   (501) staff       (20)      696 2023-05-24 15:32:27.000000 pvbm-2.1.6/setup.py
+drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-05-24 15:39:55.860971 pvbm-2.1.7/
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     4040 2023-05-24 15:39:55.860853 pvbm-2.1.7/PKG-INFO
+drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-05-24 15:39:55.858714 pvbm-2.1.7/PVBM/
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)    11109 2023-05-17 16:00:48.000000 pvbm-2.1.7/PVBM/FractalAnalysis.py
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     4853 2023-05-24 15:39:34.000000 pvbm-2.1.7/PVBM/GeometricalAnalysis.py
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)        1 2023-05-04 16:40:03.000000 pvbm-2.1.7/PVBM/__init__.py
+drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-05-24 15:39:55.859851 pvbm-2.1.7/PVBM/helpers/
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)        1 2023-05-04 16:40:03.000000 pvbm-2.1.7/PVBM/helpers/__init__.py
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     5391 2023-04-15 11:00:40.000000 pvbm-2.1.7/PVBM/helpers/branching2.py
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     6285 2023-05-17 15:55:49.000000 pvbm-2.1.7/PVBM/helpers/branching_angle.py
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     1209 2023-05-24 15:27:09.000000 pvbm-2.1.7/PVBM/helpers/perimeter.py
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     2265 2023-04-13 10:18:09.000000 pvbm-2.1.7/PVBM/helpers/tortuosity.py
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     3778 2023-05-17 15:59:09.000000 pvbm-2.1.7/README.md
+drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-05-24 15:39:55.860667 pvbm-2.1.7/pvbm.egg-info/
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     4040 2023-05-24 15:39:55.000000 pvbm-2.1.7/pvbm.egg-info/PKG-INFO
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)      363 2023-05-24 15:39:55.000000 pvbm-2.1.7/pvbm.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)        1 2023-05-24 15:39:55.000000 pvbm-2.1.7/pvbm.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)       32 2023-05-24 15:39:55.000000 pvbm-2.1.7/pvbm.egg-info/requires.txt
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)        5 2023-05-24 15:39:55.000000 pvbm-2.1.7/pvbm.egg-info/top_level.txt
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)       38 2023-05-24 15:39:55.861009 pvbm-2.1.7/setup.cfg
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)      696 2023-05-24 15:39:53.000000 pvbm-2.1.7/setup.py
```

### Comparing `pvbm-2.1.6/PKG-INFO` & `pvbm-2.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pvbm
-Version: 2.1.6
+Version: 2.1.7
 Summary: Python Vasculature Biomarker toolbox
 Home-page: https://github.com/aim-lab/PVBM
 Author: Jonathan Fhima, Yevgeniy Men
 Author-email: jonathanfh@campus.technion.ac.il
 Description-Content-Type: text/markdown
 
 # Python Vasculature BioMarker toolbox documentation
```

### Comparing `pvbm-2.1.6/PVBM/FractalAnalysis.py` & `pvbm-2.1.7/PVBM/FractalAnalysis.py`

 * *Files identical despite different names*

### Comparing `pvbm-2.1.6/PVBM/GeometricalAnalysis.py` & `pvbm-2.1.7/PVBM/GeometricalAnalysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         - The perimeter (in pixel)
         - A matrix containing the edges of the segmentation.
     
     :rtype: (float, np.ndarray)
     """
     
         filter_ = np.array([[-1, -1, -1], [-1, 8, -1], [-1, -1, -1]])
-        derivative = convolve2d(img.T,filter_, mode="same")
+        derivative = convolve2d(segmentation.T,filter_, mode="same")
         border = derivative>0
         segmentation_skeleton = skeletonize(np.ascontiguousarray(border.T)).T
         perim,_ = compute_perimeter_(segmentation_skeleton)
         return perim,segmentation_skeleton.T
     
     def compute_branching_angles(self,segmentation_skeleton):
         """
```

### Comparing `pvbm-2.1.6/PVBM/helpers/branching2.py` & `pvbm-2.1.7/PVBM/helpers/branching2.py`

 * *Files identical despite different names*

### Comparing `pvbm-2.1.6/PVBM/helpers/branching_angle.py` & `pvbm-2.1.7/PVBM/helpers/branching_angle.py`

 * *Files identical despite different names*

### Comparing `pvbm-2.1.6/PVBM/helpers/perimeter.py` & `pvbm-2.1.7/PVBM/helpers/perimeter.py`

 * *Files identical despite different names*

### Comparing `pvbm-2.1.6/PVBM/helpers/tortuosity.py` & `pvbm-2.1.7/PVBM/helpers/tortuosity.py`

 * *Files identical despite different names*

### Comparing `pvbm-2.1.6/README.md` & `pvbm-2.1.7/README.md`

 * *Files identical despite different names*

### Comparing `pvbm-2.1.6/pvbm.egg-info/PKG-INFO` & `pvbm-2.1.7/pvbm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pvbm
-Version: 2.1.6
+Version: 2.1.7
 Summary: Python Vasculature Biomarker toolbox
 Home-page: https://github.com/aim-lab/PVBM
 Author: Jonathan Fhima, Yevgeniy Men
 Author-email: jonathanfh@campus.technion.ac.il
 Description-Content-Type: text/markdown
 
 # Python Vasculature BioMarker toolbox documentation
```

### Comparing `pvbm-2.1.6/setup.py` & `pvbm-2.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
         return file.read()
 
 long_description = read_readme("README.md")
 
 
 setup(
     name='pvbm',
-    version='2.1.6',
+    version='2.1.7',
     packages=find_packages(),
     install_requires=[
         "numpy",
         "scipy",
         "scikit-image",
         "pillow"
```

