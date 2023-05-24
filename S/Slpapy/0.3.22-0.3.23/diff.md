# Comparing `tmp/Slpapy-0.3.22.tar.gz` & `tmp/Slpapy-0.3.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Slpapy-0.3.22.tar", last modified: Mon May 22 12:09:02 2023, max compression
+gzip compressed data, was "Slpapy-0.3.23.tar", last modified: Wed May 24 03:10:56 2023, max compression
```

## Comparing `Slpapy-0.3.22.tar` & `Slpapy-0.3.23.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 12:09:02.545856 Slpapy-0.3.22/
--rw-rw-rw-   0        0        0      160 2023-05-22 12:09:02.544857 Slpapy-0.3.22/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-22 12:09:02.507957 Slpapy-0.3.22/Slpapy/
--rw-rw-rw-   0        0        0     4837 2023-05-22 12:08:25.000000 Slpapy-0.3.22/Slpapy/Data_reconstruction.py
--rw-rw-rw-   0        0        0     2658 2023-05-12 06:14:48.000000 Slpapy-0.3.22/Slpapy/MZ_ppm_match.py
-drwxrwxrwx   0        0        0        0 2023-05-22 12:09:02.542864 Slpapy-0.3.22/Slpapy/Spatial_map_pic/
--rw-rw-rw-   0        0        0      662 2023-05-09 08:14:40.000000 Slpapy-0.3.22/Slpapy/Spatial_map_pic/Spatial_map.py
--rw-rw-rw-   0        0        0       52 2023-05-10 02:09:03.000000 Slpapy-0.3.22/Slpapy/Spatial_map_pic/__init__.py
--rw-rw-rw-   0        0        0      936 2023-03-31 06:05:23.000000 Slpapy-0.3.22/Slpapy/Spatial_map_pic/_compat.py
--rw-rw-rw-   0        0        0    13507 2023-03-31 06:05:23.000000 Slpapy-0.3.22/Slpapy/Spatial_map_pic/_docs.py
--rw-rw-rw-   0        0        0     1935 2023-03-31 06:05:23.000000 Slpapy-0.3.22/Slpapy/Spatial_map_pic/_rcmod.py
--rw-rw-rw-   0        0        0    15781 2023-04-18 09:43:06.000000 Slpapy-0.3.22/Slpapy/Spatial_map_pic/_settings.py
--rw-rw-rw-   0        0        0    38840 2023-04-18 09:54:49.000000 Slpapy-0.3.22/Slpapy/Spatial_map_pic/_utils.py
--rw-rw-rw-   0        0        0    26068 2023-04-18 09:48:59.000000 Slpapy-0.3.22/Slpapy/Spatial_map_pic/beats.py
--rw-rw-rw-   0        0        0     2817 2023-03-31 06:05:23.000000 Slpapy-0.3.22/Slpapy/Spatial_map_pic/is_constant.py
--rw-rw-rw-   0        0        0     8160 2023-04-18 09:54:49.000000 Slpapy-0.3.22/Slpapy/Spatial_map_pic/logging.py
--rw-rw-rw-   0        0        0     4615 2023-03-31 06:05:23.000000 Slpapy-0.3.22/Slpapy/Spatial_map_pic/palettes.py
--rw-rw-rw-   0        0        0    34738 2023-04-18 09:54:49.000000 Slpapy-0.3.22/Slpapy/Spatial_map_pic/readwrite.py
--rw-rw-rw-   0        0        0    43458 2023-05-09 09:26:02.000000 Slpapy-0.3.22/Slpapy/Spatial_map_pic/scatterplots.py
--rw-rw-rw-   0        0        0      263 2023-05-10 02:17:27.000000 Slpapy-0.3.22/Slpapy/__init__.py
--rw-rw-rw-   0        0        0     6754 2023-05-18 07:49:27.000000 Slpapy-0.3.22/Slpapy/processing_analyze.py
-drwxrwxrwx   0        0        0        0 2023-05-22 12:09:02.515935 Slpapy-0.3.22/Slpapy.egg-info/
--rw-rw-rw-   0        0        0      160 2023-05-22 12:09:02.000000 Slpapy-0.3.22/Slpapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      713 2023-05-22 12:09:02.000000 Slpapy-0.3.22/Slpapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 12:09:02.000000 Slpapy-0.3.22/Slpapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      127 2023-05-22 12:09:02.000000 Slpapy-0.3.22/Slpapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-22 12:09:02.000000 Slpapy-0.3.22/Slpapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 12:09:02.545856 Slpapy-0.3.22/setup.cfg
--rw-rw-rw-   0        0        0      512 2023-05-22 12:08:47.000000 Slpapy-0.3.22/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 03:10:56.647200 Slpapy-0.3.23/
+-rw-rw-rw-   0        0        0      160 2023-05-24 03:10:56.647200 Slpapy-0.3.23/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-24 03:10:56.605311 Slpapy-0.3.23/Slpapy/
+-rw-rw-rw-   0        0        0     4837 2023-05-22 12:08:25.000000 Slpapy-0.3.23/Slpapy/Data_reconstruction.py
+-rw-rw-rw-   0        0        0     2658 2023-05-12 06:14:48.000000 Slpapy-0.3.23/Slpapy/MZ_ppm_match.py
+drwxrwxrwx   0        0        0        0 2023-05-24 03:10:56.644207 Slpapy-0.3.23/Slpapy/Spatial_map_pic/
+-rw-rw-rw-   0        0        0      645 2023-05-24 03:09:49.000000 Slpapy-0.3.23/Slpapy/Spatial_map_pic/Spatial_map.py
+-rw-rw-rw-   0        0        0       52 2023-05-10 02:09:03.000000 Slpapy-0.3.23/Slpapy/Spatial_map_pic/__init__.py
+-rw-rw-rw-   0        0        0      936 2023-03-31 06:05:23.000000 Slpapy-0.3.23/Slpapy/Spatial_map_pic/_compat.py
+-rw-rw-rw-   0        0        0    13507 2023-03-31 06:05:23.000000 Slpapy-0.3.23/Slpapy/Spatial_map_pic/_docs.py
+-rw-rw-rw-   0        0        0     1935 2023-03-31 06:05:23.000000 Slpapy-0.3.23/Slpapy/Spatial_map_pic/_rcmod.py
+-rw-rw-rw-   0        0        0    15781 2023-04-18 09:43:06.000000 Slpapy-0.3.23/Slpapy/Spatial_map_pic/_settings.py
+-rw-rw-rw-   0        0        0    38840 2023-04-18 09:54:49.000000 Slpapy-0.3.23/Slpapy/Spatial_map_pic/_utils.py
+-rw-rw-rw-   0        0        0    26068 2023-04-18 09:48:59.000000 Slpapy-0.3.23/Slpapy/Spatial_map_pic/beats.py
+-rw-rw-rw-   0        0        0     2817 2023-03-31 06:05:23.000000 Slpapy-0.3.23/Slpapy/Spatial_map_pic/is_constant.py
+-rw-rw-rw-   0        0        0     8160 2023-04-18 09:54:49.000000 Slpapy-0.3.23/Slpapy/Spatial_map_pic/logging.py
+-rw-rw-rw-   0        0        0     4615 2023-03-31 06:05:23.000000 Slpapy-0.3.23/Slpapy/Spatial_map_pic/palettes.py
+-rw-rw-rw-   0        0        0    34738 2023-04-18 09:54:49.000000 Slpapy-0.3.23/Slpapy/Spatial_map_pic/readwrite.py
+-rw-rw-rw-   0        0        0    43450 2023-05-24 03:01:37.000000 Slpapy-0.3.23/Slpapy/Spatial_map_pic/scatterplots.py
+-rw-rw-rw-   0        0        0      263 2023-05-10 02:17:27.000000 Slpapy-0.3.23/Slpapy/__init__.py
+-rw-rw-rw-   0        0        0     6754 2023-05-18 07:49:27.000000 Slpapy-0.3.23/Slpapy/processing_analyze.py
+drwxrwxrwx   0        0        0        0 2023-05-24 03:10:56.616282 Slpapy-0.3.23/Slpapy.egg-info/
+-rw-rw-rw-   0        0        0      160 2023-05-24 03:10:56.000000 Slpapy-0.3.23/Slpapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      713 2023-05-24 03:10:56.000000 Slpapy-0.3.23/Slpapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 03:10:56.000000 Slpapy-0.3.23/Slpapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      127 2023-05-24 03:10:56.000000 Slpapy-0.3.23/Slpapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-24 03:10:56.000000 Slpapy-0.3.23/Slpapy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-24 03:10:56.647200 Slpapy-0.3.23/setup.cfg
+-rw-rw-rw-   0        0        0      512 2023-05-24 03:10:44.000000 Slpapy-0.3.23/setup.py
```

### Comparing `Slpapy-0.3.22/Slpapy/Data_reconstruction.py` & `Slpapy-0.3.23/Slpapy/Data_reconstruction.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.22/Slpapy/MZ_ppm_match.py` & `Slpapy-0.3.23/Slpapy/MZ_ppm_match.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.22/Slpapy/Spatial_map_pic/Spatial_map.py` & `Slpapy-0.3.23/Slpapy/Spatial_map_pic/Spatial_map.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,17 +11,18 @@
 
 
 
 def Spatial_class_location(
         adata: ad.AnnData,
         cls: str,  # TIC和XY文件路径
         *,
-        n: str = None,  # 每个像素点的面积
+        n: str = None,  # 不同的类别
 ) -> Optional[ad.AnnData]:
     cls = str(cls)
     if n is None:
-        for i in range(adata.obs['leiden'].values.codes.max() + 1):
+        for i in adata.obs[cls].values.categories.values:
             Spatial_class(adata, cls, i)
 
     else:
         Spatial_class(adata, cls, n)
 
+
```

### Comparing `Slpapy-0.3.22/Slpapy/Spatial_map_pic/_compat.py` & `Slpapy-0.3.23/Slpapy/Spatial_map_pic/_compat.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.22/Slpapy/Spatial_map_pic/_docs.py` & `Slpapy-0.3.23/Slpapy/Spatial_map_pic/_docs.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.22/Slpapy/Spatial_map_pic/_rcmod.py` & `Slpapy-0.3.23/Slpapy/Spatial_map_pic/_rcmod.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.22/Slpapy/Spatial_map_pic/_settings.py` & `Slpapy-0.3.23/Slpapy/Spatial_map_pic/_settings.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.22/Slpapy/Spatial_map_pic/_utils.py` & `Slpapy-0.3.23/Slpapy/Spatial_map_pic/_utils.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.22/Slpapy/Spatial_map_pic/beats.py` & `Slpapy-0.3.23/Slpapy/Spatial_map_pic/beats.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.22/Slpapy/Spatial_map_pic/is_constant.py` & `Slpapy-0.3.23/Slpapy/Spatial_map_pic/is_constant.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.22/Slpapy/Spatial_map_pic/logging.py` & `Slpapy-0.3.23/Slpapy/Spatial_map_pic/logging.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.22/Slpapy/Spatial_map_pic/palettes.py` & `Slpapy-0.3.23/Slpapy/Spatial_map_pic/palettes.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.22/Slpapy/Spatial_map_pic/readwrite.py` & `Slpapy-0.3.23/Slpapy/Spatial_map_pic/readwrite.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.22/Slpapy/Spatial_map_pic/scatterplots.py` & `Slpapy-0.3.23/Slpapy/Spatial_map_pic/scatterplots.py`

 * *Files 0% similar despite different names*

```diff
@@ -1361,12 +1361,12 @@
     )
 
 def Spatial_class(adata, cls, n):
     cls = str(cls)
 
     for j in adata.obs_names:
         if adata.obs.loc[j, f'{cls}'] == str(n):
-            adata.obs.loc[j, 'leidens'] = str(n)
+            adata.obs.loc[j, 'class'] = str(n)
         else:
-            adata.obs.loc[j, 'leidens'] = 'background'
-    embedding(adata, basis='X_spacial', color='leidens', frameon=False, save=f'_spacial_{cls}_{n}.png')
-    del adata.obs['leidens']
+            adata.obs.loc[j, 'class'] = 'background'
+    embedding(adata, basis='X_spacial', color='class', frameon=False, save=f'_spacial_{cls}_{n}.png')
+    del adata.obs['class']
```

### Comparing `Slpapy-0.3.22/Slpapy/processing_analyze.py` & `Slpapy-0.3.23/Slpapy/processing_analyze.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.22/Slpapy.egg-info/SOURCES.txt` & `Slpapy-0.3.23/Slpapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.22/setup.py` & `Slpapy-0.3.23/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Slpapy',
-    version='0.3.22',
+    version='0.3.23',
     author='yifan xu',
     author_email='xuyifan@westlake.edu.cn',
     description='Spatial_lipomic_and_proteomic_analysis',
     packages=find_packages(),
     install_requires=[
         'scanpy>=1.9.1',
         'anndata>=0.8.0',
```

