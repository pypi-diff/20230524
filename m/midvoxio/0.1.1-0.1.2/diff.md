# Comparing `tmp/midvoxio-0.1.1.tar.gz` & `tmp/midvoxio-0.1.2.tar.gz`

## Comparing `midvoxio-0.1.1.tar` & `midvoxio-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 midvoxio-0.1.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 midvoxio-0.1.1/assets/palette/cat.png
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 midvoxio-0.1.1/assets/palette/pal0.png
--rw-r--r--   0        0        0    20336 2020-02-02 00:00:00.000000 midvoxio-0.1.1/assets/vox/98/cat.vox
--rw-r--r--   0        0        0    29518 2020-02-02 00:00:00.000000 midvoxio-0.1.1/assets/vox/99/3x3x3.vox
--rw-r--r--   0        0        0    48186 2020-02-02 00:00:00.000000 midvoxio-0.1.1/assets/vox/99/cars.vox
--rw-r--r--   0        0        0    24193 2020-02-02 00:00:00.000000 midvoxio-0.1.1/assets/vox/voxedit/cat.vox
--rw-r--r--   0        0        0    35384 2020-02-02 00:00:00.000000 midvoxio-0.1.1/img/3x3x3.jpg
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 midvoxio-0.1.1/src/examples.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 midvoxio-0.1.1/src/midvoxio/__init__.py
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 midvoxio-0.1.1/src/midvoxio/config.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 midvoxio-0.1.1/src/midvoxio/exceptions.py
--rw-r--r--   0        0        0    12804 2020-02-02 00:00:00.000000 midvoxio-0.1.1/src/midvoxio/models.py
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 midvoxio-0.1.1/src/midvoxio/parser.py
--rw-r--r--   0        0        0     8072 2020-02-02 00:00:00.000000 midvoxio-0.1.1/src/midvoxio/vox.py
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 midvoxio-0.1.1/src/midvoxio/voxio.py
--rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 midvoxio-0.1.1/src/midvoxio/writer.py
--rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 midvoxio-0.1.1/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 midvoxio-0.1.1/LICENSE
--rw-r--r--   0        0        0     2882 2020-02-02 00:00:00.000000 midvoxio-0.1.1/README.md
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 midvoxio-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 midvoxio-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 midvoxio-0.1.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 midvoxio-0.1.2/assets/palette/cat.png
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 midvoxio-0.1.2/assets/palette/pal0.png
+-rw-r--r--   0        0        0    20336 2020-02-02 00:00:00.000000 midvoxio-0.1.2/assets/vox/98/cat.vox
+-rw-r--r--   0        0        0    29518 2020-02-02 00:00:00.000000 midvoxio-0.1.2/assets/vox/99/3x3x3.vox
+-rw-r--r--   0        0        0    48186 2020-02-02 00:00:00.000000 midvoxio-0.1.2/assets/vox/99/cars.vox
+-rw-r--r--   0        0        0    24193 2020-02-02 00:00:00.000000 midvoxio-0.1.2/assets/vox/voxedit/cat.vox
+-rw-r--r--   0        0        0    35384 2020-02-02 00:00:00.000000 midvoxio-0.1.2/img/3x3x3.jpg
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 midvoxio-0.1.2/src/examples.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 midvoxio-0.1.2/src/midvoxio/__init__.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 midvoxio-0.1.2/src/midvoxio/config.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 midvoxio-0.1.2/src/midvoxio/exceptions.py
+-rw-r--r--   0        0        0    12804 2020-02-02 00:00:00.000000 midvoxio-0.1.2/src/midvoxio/models.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 midvoxio-0.1.2/src/midvoxio/parser.py
+-rw-r--r--   0        0        0     8072 2020-02-02 00:00:00.000000 midvoxio-0.1.2/src/midvoxio/vox.py
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 midvoxio-0.1.2/src/midvoxio/voxio.py
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 midvoxio-0.1.2/src/midvoxio/writer.py
+-rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 midvoxio-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 midvoxio-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 midvoxio-0.1.2/README.md
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 midvoxio-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3473 2020-02-02 00:00:00.000000 midvoxio-0.1.2/PKG-INFO
```

### Comparing `midvoxio-0.1.1/.github/workflows/python-publish.yml` & `midvoxio-0.1.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `midvoxio-0.1.1/assets/vox/98/cat.vox` & `midvoxio-0.1.2/assets/vox/98/cat.vox`

 * *Files identical despite different names*

### Comparing `midvoxio-0.1.1/assets/vox/99/3x3x3.vox` & `midvoxio-0.1.2/assets/vox/99/3x3x3.vox`

 * *Files identical despite different names*

### Comparing `midvoxio-0.1.1/assets/vox/99/cars.vox` & `midvoxio-0.1.2/assets/vox/99/cars.vox`

 * *Files identical despite different names*

### Comparing `midvoxio-0.1.1/assets/vox/voxedit/cat.vox` & `midvoxio-0.1.2/assets/vox/voxedit/cat.vox`

 * *Files identical despite different names*

### Comparing `midvoxio-0.1.1/img/3x3x3.jpg` & `midvoxio-0.1.2/img/3x3x3.jpg`

 * *Files identical despite different names*

### Comparing `midvoxio-0.1.1/src/examples.py` & `midvoxio-0.1.2/src/examples.py`

 * *Files identical despite different names*

### Comparing `midvoxio-0.1.1/src/midvoxio/models.py` & `midvoxio-0.1.2/src/midvoxio/models.py`

 * *Files identical despite different names*

### Comparing `midvoxio-0.1.1/src/midvoxio/parser.py` & `midvoxio-0.1.2/src/midvoxio/parser.py`

 * *Files identical despite different names*

### Comparing `midvoxio-0.1.1/src/midvoxio/vox.py` & `midvoxio-0.1.2/src/midvoxio/vox.py`

 * *Files identical despite different names*

### Comparing `midvoxio-0.1.1/src/midvoxio/voxio.py` & `midvoxio-0.1.2/src/midvoxio/voxio.py`

 * *Files identical despite different names*

### Comparing `midvoxio-0.1.1/src/midvoxio/writer.py` & `midvoxio-0.1.2/src/midvoxio/writer.py`

 * *Files identical despite different names*

### Comparing `midvoxio-0.1.1/.gitignore` & `midvoxio-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `midvoxio-0.1.1/LICENSE` & `midvoxio-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `midvoxio-0.1.1/README.md` & `midvoxio-0.1.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -14,43 +14,43 @@
 - add the repo to path
 - Install numpy and matplotlib if you haven't
 
 ## Usage
 #### vox_to_arr()
 use `vox_to_arr()` to parse .vox file into numpy array.
 ```Python
-from voxio import vox_to_arr
+from midvoxio.voxio import vox_to_arr
 
 print(vox_to_arr('vox/99/3x3x3.vox').shape)
 ```
 result:
 ```Python
 (3, 3, 3, 4) # the four axis are (x,y,z,color), color is [r,g,b,a] here
 ```
 
 
 
 #### viz_vox()
 
 use `viz_vox()` to visualize your .vox file. It uses `matplotlib` to plot the file internally.
 ```Python
-from voxio import viz_vox
+from midvoxio.voxio import viz_vox
 
 viz_vox('vox/99/3x3x3.vox')
 ```
 then, the python will give you a 3d plot.
 <img src="/img/3x3x3.jpg" width="25%">
 
 
 
 #### get other info
 
 use `get_rendering_attributes()`,`get_cameras()`, and `get_materials()` to get vox info.
 ```Python
->>> from voxio import *
+>>> from midvoxio.voxio import *
 >>> print(get_cameras('vox/99/cars.vox')[0])
 {'id': (0,), 'attributes': {'_mode': 'pers', '_focus': '0 0 0', '_angle': '0 0 0', '_radius': '0', '_frustum': '0.414214', '_fov': '45'}}
 >>> print(get_rendering_attributes('vox/99/3x3x3.vox')[0])
 {'_type': '_inf', '_i': '0.6', '_k': '255 255 255', '_angle': '50 50', '_area': '0.07'}
 >>> print(get_materials('vox/99/3x3x3.vox')[0])
 {'id': (0,), 'properties': {'_type': '_diffuse', '_weight': '1', '_rough': '0.1', '_spec': '0.5', '_ior': '0.3'}}
 ```
@@ -58,15 +58,15 @@
 
 
 #### write_list_to_vox()
 
 use `write_list_to_vox` to generate vox file from exist python list. You can use this function to export the python list as vox file, so you will be able to edit vox file in python.
 
 ```Python
-from voxio import write_list_to_vox,plot_3d
+from midvoxio.voxio import write_list_to_vox,plot_3d
 
 arr=[] # define your python list that represent the 3d model here
 
 # define your palette that relate to your model here
 # palette will be able to be automatically generated in the future
 palette=[]
```

### Comparing `midvoxio-0.1.1/pyproject.toml` & `midvoxio-0.1.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "midvoxio"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Midstream", email="midstream.lou@gmail.com" },
 ]
 description = "A python io to load/write/visualize vox files (MagicalVoxel's .vox format)."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 
 [project.urls]
-"Homepage" = "https://github.com/midstreeeam/PyVox"
-"Bug Tracker" = "https://github.com/midstreeeam/PyVox/issues"
+"Homepage" = "https://github.com/midstreeeam/MidVoxIO"
+"Bug Tracker" = "https://github.com/midstreeeam/MidVoxIO/issues"
```

### Comparing `midvoxio-0.1.1/PKG-INFO` & `midvoxio-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: midvoxio
-Version: 0.1.1
+Version: 0.1.2
 Summary: A python io to load/write/visualize vox files (MagicalVoxel's .vox format).
-Project-URL: Homepage, https://github.com/midstreeeam/PyVox
-Project-URL: Bug Tracker, https://github.com/midstreeeam/PyVox/issues
+Project-URL: Homepage, https://github.com/midstreeeam/MidVoxIO
+Project-URL: Bug Tracker, https://github.com/midstreeeam/MidVoxIO/issues
 Author-email: Midstream <midstream.lou@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -28,43 +28,43 @@
 - add the repo to path
 - Install numpy and matplotlib if you haven't
 
 ## Usage
 #### vox_to_arr()
 use `vox_to_arr()` to parse .vox file into numpy array.
 ```Python
-from voxio import vox_to_arr
+from midvoxio.voxio import vox_to_arr
 
 print(vox_to_arr('vox/99/3x3x3.vox').shape)
 ```
 result:
 ```Python
 (3, 3, 3, 4) # the four axis are (x,y,z,color), color is [r,g,b,a] here
 ```
 
 
 
 #### viz_vox()
 
 use `viz_vox()` to visualize your .vox file. It uses `matplotlib` to plot the file internally.
 ```Python
-from voxio import viz_vox
+from midvoxio.voxio import viz_vox
 
 viz_vox('vox/99/3x3x3.vox')
 ```
 then, the python will give you a 3d plot.
 <img src="/img/3x3x3.jpg" width="25%">
 
 
 
 #### get other info
 
 use `get_rendering_attributes()`,`get_cameras()`, and `get_materials()` to get vox info.
 ```Python
->>> from voxio import *
+>>> from midvoxio.voxio import *
 >>> print(get_cameras('vox/99/cars.vox')[0])
 {'id': (0,), 'attributes': {'_mode': 'pers', '_focus': '0 0 0', '_angle': '0 0 0', '_radius': '0', '_frustum': '0.414214', '_fov': '45'}}
 >>> print(get_rendering_attributes('vox/99/3x3x3.vox')[0])
 {'_type': '_inf', '_i': '0.6', '_k': '255 255 255', '_angle': '50 50', '_area': '0.07'}
 >>> print(get_materials('vox/99/3x3x3.vox')[0])
 {'id': (0,), 'properties': {'_type': '_diffuse', '_weight': '1', '_rough': '0.1', '_spec': '0.5', '_ior': '0.3'}}
 ```
@@ -72,15 +72,15 @@
 
 
 #### write_list_to_vox()
 
 use `write_list_to_vox` to generate vox file from exist python list. You can use this function to export the python list as vox file, so you will be able to edit vox file in python.
 
 ```Python
-from voxio import write_list_to_vox,plot_3d
+from midvoxio.voxio import write_list_to_vox,plot_3d
 
 arr=[] # define your python list that represent the 3d model here
 
 # define your palette that relate to your model here
 # palette will be able to be automatically generated in the future
 palette=[]
```

