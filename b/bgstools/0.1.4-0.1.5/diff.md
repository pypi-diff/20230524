# Comparing `tmp/bgstools-0.1.4.tar.gz` & `tmp/bgstools-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bgstools-0.1.4.tar", max compression
+gzip compressed data, was "bgstools-0.1.5.tar", max compression
```

## Comparing `bgstools-0.1.4.tar` & `bgstools-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       72 2023-05-22 09:38:31.760561 bgstools-0.1.4/README.md
--rw-r--r--   0        0        0        0 2023-05-03 11:32:59.064694 bgstools-0.1.4/bgstools/__init__.py
--rw-r--r--   0        0        0       64 2023-05-22 20:01:20.000000 bgstools-0.1.4/bgstools/datastorage/__init__.py
--rw-r--r--   0        0        0     5014 2023-05-22 20:29:18.000000 bgstools-0.1.4/bgstools/datastorage/datastorage.py
--rw-r--r--   0        0        0      165 2023-05-23 09:24:52.850097 bgstools-0.1.4/bgstools/io/__init__.py
--rw-r--r--   0        0        0     3990 2023-05-23 08:59:13.676273 bgstools-0.1.4/bgstools/io/io.py
--rw-r--r--   0        0        0     4820 2023-05-23 13:42:54.752929 bgstools-0.1.4/bgstools/io/media.py
--rw-r--r--   0        0        0      122 2023-05-22 20:28:18.000000 bgstools-0.1.4/bgstools/spatial/__init__.py
--rw-r--r--   0        0        0     2654 2023-05-22 17:37:56.000000 bgstools-0.1.4/bgstools/spatial/spatial.py
--rw-r--r--   0        0        0       39 2023-05-22 20:27:28.000000 bgstools-0.1.4/bgstools/stt/__init__.py
--rw-r--r--   0        0        0     2171 2023-05-23 06:03:13.166243 bgstools-0.1.4/bgstools/stt/stt.py
--rw-r--r--   0        0        0       99 2023-05-22 20:25:04.000000 bgstools-0.1.4/bgstools/utils/__init__.py
--rw-r--r--   0        0        0     2971 2023-05-22 20:24:36.000000 bgstools-0.1.4/bgstools/utils/utils.py
--rw-r--r--   0        0        0      418 2023-05-23 13:51:00.277544 bgstools-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 bgstools-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       72 2023-05-22 09:38:31.760561 bgstools-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2023-05-03 11:32:59.064694 bgstools-0.1.5/bgstools/__init__.py
+-rw-r--r--   0        0        0       64 2023-05-22 20:01:20.000000 bgstools-0.1.5/bgstools/datastorage/__init__.py
+-rw-r--r--   0        0        0     5014 2023-05-22 20:29:18.000000 bgstools-0.1.5/bgstools/datastorage/datastorage.py
+-rw-r--r--   0        0        0      165 2023-05-23 09:24:52.850097 bgstools-0.1.5/bgstools/io/__init__.py
+-rw-r--r--   0        0        0     3990 2023-05-23 08:59:13.676273 bgstools-0.1.5/bgstools/io/io.py
+-rw-r--r--   0        0        0     3770 2023-05-24 20:22:39.226612 bgstools-0.1.5/bgstools/io/media.py
+-rw-r--r--   0        0        0      122 2023-05-22 20:28:18.000000 bgstools-0.1.5/bgstools/spatial/__init__.py
+-rw-r--r--   0        0        0     2654 2023-05-22 17:37:56.000000 bgstools-0.1.5/bgstools/spatial/spatial.py
+-rw-r--r--   0        0        0       39 2023-05-22 20:27:28.000000 bgstools-0.1.5/bgstools/stt/__init__.py
+-rw-r--r--   0        0        0     2171 2023-05-23 06:03:13.166243 bgstools-0.1.5/bgstools/stt/stt.py
+-rw-r--r--   0        0        0       99 2023-05-22 20:25:04.000000 bgstools-0.1.5/bgstools/utils/__init__.py
+-rw-r--r--   0        0        0     2971 2023-05-22 20:24:36.000000 bgstools-0.1.5/bgstools/utils/utils.py
+-rw-r--r--   0        0        0      433 2023-05-24 20:24:05.236614 bgstools-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      681 1970-01-01 00:00:00.000000 bgstools-0.1.5/PKG-INFO
```

### Comparing `bgstools-0.1.4/bgstools/datastorage/datastorage.py` & `bgstools-0.1.5/bgstools/datastorage/datastorage.py`

 * *Files identical despite different names*

### Comparing `bgstools-0.1.4/bgstools/io/io.py` & `bgstools-0.1.5/bgstools/io/io.py`

 * *Files identical despite different names*

### Comparing `bgstools-0.1.4/bgstools/io/media.py` & `bgstools-0.1.5/bgstools/io/media.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import cv2
 import numpy as np
-from osgeo import gdal
+
 
 def convert_image_frame(frame, output_path, format='png', compression=False, jpeg_quality=95, tiff_metadata=None):
     """
     Converts an image frame to the specified format (PNG, JPEG, GeoTIFF).
 
     Args:
         frame (numpy.ndarray): The image frame as a NumPy array.
@@ -30,29 +30,14 @@
         cv2.imwrite(output_path, frame)
     elif format.lower() == 'jpeg' or format.lower() == 'jpg':
         if compression:
             params = [cv2.IMWRITE_JPEG_QUALITY, jpeg_quality]
             cv2.imwrite(output_path, frame, params)
         else:
             cv2.imwrite(output_path, frame)
-    elif format.lower() == 'geotiff' or format.lower() == 'gtiff' or format.lower() == 'tiff':
-        if frame.ndim == 2:
-            frame = np.expand_dims(frame, axis=2)
-        if tiff_metadata is None:
-            tiff_metadata = {}
-        driver = gdal.GetDriverByName('GTiff')
-        height, width, channels = frame.shape
-        dataset = driver.Create(output_path, width, height, channels, gdal.GDT_Byte)
-        for i in range(channels):
-            band = dataset.GetRasterBand(i + 1)
-            band.WriteArray(frame[:, :, i])
-        for key, value in tiff_metadata.items():
-            dataset.SetMetadataItem(key, value)
-        dataset.FlushCache()
-        dataset = None
     else:
         raise ValueError("Unsupported output format: {}".format(format))
 
 
 
 
 def load_big_tiff(path):
@@ -128,23 +113,8 @@
 
     Args:
         image (numpy.ndarray): The processed image as a NumPy array.
         output_path (str): The output file path for the exported .tiff file.
     """
     cv2.imwrite(output_path, image)
 
-import numpy as np
-import cv2
-
-
-def load_big_tiff(path):
-    """
-    Loads a big .tiff image using memory-mapped files.
 
-    Args:
-        path (str): The path to the .tiff image.
-
-    Returns:
-        numpy.ndarray: The image as a NumPy array.
-    """
-    img = cv2.imread(path, cv2.IMREAD_UNCHANGED | cv2.IMREAD_ANYDEPTH)
-    return img
```

### Comparing `bgstools-0.1.4/bgstools/spatial/spatial.py` & `bgstools-0.1.5/bgstools/spatial/spatial.py`

 * *Files identical despite different names*

### Comparing `bgstools-0.1.4/bgstools/stt/stt.py` & `bgstools-0.1.5/bgstools/stt/stt.py`

 * *Files identical despite different names*

### Comparing `bgstools-0.1.4/bgstools/utils/utils.py` & `bgstools-0.1.5/bgstools/utils/utils.py`

 * *Files identical despite different names*

### Comparing `bgstools-0.1.4/PKG-INFO` & `bgstools-0.1.5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: bgstools
-Version: 0.1.4
-Summary: 
+Version: 0.1.5
+Summary: BeGeoSpatial Development Tools
 Author: José Beltrán
 Author-email: 102664984+jose-begeospatial@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: certifi (>=2023.5.7,<2024.0.0)
-Requires-Dist: gdal (>=3.6.2,<4.0.0)
 Requires-Dist: h3 (>=3.7.6,<4.0.0)
 Requires-Dist: opencv-python (>=4.7.0.72,<5.0.0.0)
 Requires-Dist: pyproj (>=3.5.0,<4.0.0)
 Description-Content-Type: text/markdown
 
 # Be GeoSpatial development tools
```

