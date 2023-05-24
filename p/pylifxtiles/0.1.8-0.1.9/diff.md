# Comparing `tmp/pylifxtiles-0.1.8.tar.gz` & `tmp/pylifxtiles-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pylifxtiles-0.1.8.tar", last modified: Fri May 15 21:32:09 2020, max compression
+gzip compressed data, was "pylifxtiles-0.1.9.tar", last modified: Wed May 24 15:52:13 2023, max compression
```

## Comparing `pylifxtiles-0.1.8.tar` & `pylifxtiles-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 christopheryoung   (501) staff       (20)        0 2020-05-15 21:32:09.000000 pylifxtiles-0.1.8/
--rw-r--r--   0 christopheryoung   (501) staff       (20)     1364 2020-05-15 21:32:09.000000 pylifxtiles-0.1.8/PKG-INFO
--rw-r--r--   0 christopheryoung   (501) staff       (20)      468 2020-04-26 16:04:32.000000 pylifxtiles-0.1.8/README.rst
-drwxr-xr-x   0 christopheryoung   (501) staff       (20)        0 2020-05-15 21:32:09.000000 pylifxtiles-0.1.8/pylifxtiles/
--rw-r--r--   0 christopheryoung   (501) staff       (20)        0 2020-04-23 18:16:23.000000 pylifxtiles-0.1.8/pylifxtiles/__init__.py
--rw-r--r--   0 christopheryoung   (501) staff       (20)     4292 2020-05-15 21:32:03.000000 pylifxtiles-0.1.8/pylifxtiles/actions.py
--rw-r--r--   0 christopheryoung   (501) staff       (20)     3502 2020-04-23 18:16:23.000000 pylifxtiles-0.1.8/pylifxtiles/alphanum.py
--rw-r--r--   0 christopheryoung   (501) staff       (20)     1136 2020-04-23 18:16:23.000000 pylifxtiles-0.1.8/pylifxtiles/colors.py
--rw-r--r--   0 christopheryoung   (501) staff       (20)     1684 2020-04-26 14:10:07.000000 pylifxtiles-0.1.8/pylifxtiles/objects.py
--rw-r--r--   0 christopheryoung   (501) staff       (20)     8954 2020-04-24 15:15:47.000000 pylifxtiles-0.1.8/pylifxtiles/tiles.py
-drwxr-xr-x   0 christopheryoung   (501) staff       (20)        0 2020-05-15 21:32:09.000000 pylifxtiles-0.1.8/pylifxtiles.egg-info/
--rw-r--r--   0 christopheryoung   (501) staff       (20)     1364 2020-05-15 21:32:09.000000 pylifxtiles-0.1.8/pylifxtiles.egg-info/PKG-INFO
--rw-r--r--   0 christopheryoung   (501) staff       (20)      368 2020-05-15 21:32:09.000000 pylifxtiles-0.1.8/pylifxtiles.egg-info/SOURCES.txt
--rw-r--r--   0 christopheryoung   (501) staff       (20)        1 2020-05-15 21:32:09.000000 pylifxtiles-0.1.8/pylifxtiles.egg-info/dependency_links.txt
--rw-r--r--   0 christopheryoung   (501) staff       (20)       40 2020-05-15 21:32:09.000000 pylifxtiles-0.1.8/pylifxtiles.egg-info/entry_points.txt
--rw-r--r--   0 christopheryoung   (501) staff       (20)       87 2020-05-15 21:32:09.000000 pylifxtiles-0.1.8/pylifxtiles.egg-info/requires.txt
--rw-r--r--   0 christopheryoung   (501) staff       (20)       12 2020-05-15 21:32:09.000000 pylifxtiles-0.1.8/pylifxtiles.egg-info/top_level.txt
--rw-r--r--   0 christopheryoung   (501) staff       (20)       38 2020-05-15 21:32:09.000000 pylifxtiles-0.1.8/setup.cfg
--rw-r--r--   0 christopheryoung   (501) staff       (20)     4055 2020-05-15 21:32:03.000000 pylifxtiles-0.1.8/setup.py
+drwxr-xr-x   0 christopheryoung   (503) staff       (20)        0 2023-05-24 15:52:13.412511 pylifxtiles-0.1.9/
+-rw-r--r--   0 christopheryoung   (503) staff       (20)    11357 2023-03-05 19:40:11.000000 pylifxtiles-0.1.9/LICENSE
+-rw-r--r--   0 christopheryoung   (503) staff       (20)     1195 2023-05-24 15:52:13.412294 pylifxtiles-0.1.9/PKG-INFO
+-rw-r--r--   0 christopheryoung   (503) staff       (20)      468 2023-03-05 19:40:11.000000 pylifxtiles-0.1.9/README.rst
+drwxr-xr-x   0 christopheryoung   (503) staff       (20)        0 2023-05-24 15:52:13.411249 pylifxtiles-0.1.9/pylifxtiles/
+-rw-r--r--   0 christopheryoung   (503) staff       (20)        0 2023-03-05 19:40:11.000000 pylifxtiles-0.1.9/pylifxtiles/__init__.py
+-rw-r--r--   0 christopheryoung   (503) staff       (20)     4168 2023-03-05 19:40:11.000000 pylifxtiles-0.1.9/pylifxtiles/actions.py
+-rw-r--r--   0 christopheryoung   (503) staff       (20)     3502 2023-03-05 19:40:11.000000 pylifxtiles-0.1.9/pylifxtiles/alphanum.py
+-rw-r--r--   0 christopheryoung   (503) staff       (20)     1136 2023-03-05 19:40:11.000000 pylifxtiles-0.1.9/pylifxtiles/colors.py
+-rw-r--r--   0 christopheryoung   (503) staff       (20)     1684 2023-03-05 19:40:11.000000 pylifxtiles-0.1.9/pylifxtiles/objects.py
+-rw-r--r--   0 christopheryoung   (503) staff       (20)     8954 2023-03-05 19:40:11.000000 pylifxtiles-0.1.9/pylifxtiles/tiles.py
+drwxr-xr-x   0 christopheryoung   (503) staff       (20)        0 2023-05-24 15:52:13.412074 pylifxtiles-0.1.9/pylifxtiles.egg-info/
+-rw-r--r--   0 christopheryoung   (503) staff       (20)     1195 2023-05-24 15:52:13.000000 pylifxtiles-0.1.9/pylifxtiles.egg-info/PKG-INFO
+-rw-r--r--   0 christopheryoung   (503) staff       (20)      376 2023-05-24 15:52:13.000000 pylifxtiles-0.1.9/pylifxtiles.egg-info/SOURCES.txt
+-rw-r--r--   0 christopheryoung   (503) staff       (20)        1 2023-05-24 15:52:13.000000 pylifxtiles-0.1.9/pylifxtiles.egg-info/dependency_links.txt
+-rw-r--r--   0 christopheryoung   (503) staff       (20)       39 2023-05-24 15:52:13.000000 pylifxtiles-0.1.9/pylifxtiles.egg-info/entry_points.txt
+-rw-r--r--   0 christopheryoung   (503) staff       (20)       96 2023-05-24 15:52:13.000000 pylifxtiles-0.1.9/pylifxtiles.egg-info/requires.txt
+-rw-r--r--   0 christopheryoung   (503) staff       (20)       12 2023-05-24 15:52:13.000000 pylifxtiles-0.1.9/pylifxtiles.egg-info/top_level.txt
+-rw-r--r--   0 christopheryoung   (503) staff       (20)       38 2023-05-24 15:52:13.412557 pylifxtiles-0.1.9/setup.cfg
+-rw-r--r--   0 christopheryoung   (503) staff       (20)     4064 2023-05-24 15:52:10.000000 pylifxtiles-0.1.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pylifxtiles-0.1.8/PKG-INFO` & `pylifxtiles-0.1.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 Metadata-Version: 2.1
 Name: pylifxtiles
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python binding for LIFX Tiles
 Home-page: https://github.com/netmanchris/pylifxtiles
 Author: netmanchris
 Author-email: python@homekitgeek.com
 License: Apache2
-Description: PYLIFXTILES
-        
-        **READ THIS FIRST**
-        This library is currently in alpha state and should not be used for production installations.
-        Support is not offered at this time, but GITHUB issues are welcome if bugs or potential feature
-        enhancements are found.
-        
-        ##Description
-        
-        This is a sample python language binding for the LIFX Tiles products.
-        
-        Installation
-        
-        Product should be on pip. Can also be installed directly using the typical ways.
-        
-        `pip install -r requirements.txt`
-        
-        
-        
-        
-        
 Keywords: lifx,tiles,api,python
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: dev
 Provides-Extra: test
+License-File: LICENSE
+
+PYLIFXTILES
+
+**READ THIS FIRST**
+This library is currently in alpha state and should not be used for production installations.
+Support is not offered at this time, but GITHUB issues are welcome if bugs or potential feature
+enhancements are found.
+
+##Description
+
+This is a sample python language binding for the LIFX Tiles products.
+
+Installation
+
+Product should be on pip. Can also be installed directly using the typical ways.
+
+`pip install -r requirements.txt`
+
+
+
+
```

### Comparing `pylifxtiles-0.1.8/pylifxtiles/actions.py` & `pylifxtiles-0.1.9/pylifxtiles/actions.py`

 * *Files 10% similar despite different names*

```diff
@@ -55,25 +55,24 @@
     # load the image
     my_image = Image.open(image_to_display)
     # report the size of the image
     # print(my_image.size)
     # resize image and ignore original aspect ratio
     img_resized = my_image.resize(image_size)
     # changing the file extension from jpg to png changes output brightness. You might need to play with this.
-    img_resized.save('./resized_image.jpg')
-    data = image.imread('./resized_image.jpg')
+    data = asarray(img_resized)
     target_tcs = []
     for row in data:
         temp_row = []
         for pixel in row:
             temp_row.append(RGBtoHSBK(pixel))
         target_tcs.append(temp_row)
     # print ("length of target_tcs is " + str(len(target_tcs)))
     tcsplit = tiles.split_tilechains(target_tcs)
-    # print ("length of tcssplit is " + str(len(tcsplit)))
+    # print ("legnth of tcssplit is " + str(len(tcsplit)))
     # print ("length tilelist is " + str(len(tilechain_list)))
     for tile in range(len(tilechain_list)):
         print(tile)
         tilechain_list[tile].set_tilechain_colors(tiles.split_combined_matrix(tcsplit[tile]), rapid=True)
 
 
 def display_png_image(image_to_display, image_size, tilechain_list):
@@ -89,16 +88,15 @@
     # load the image
     my_image = Image.open(image_to_display)
     # report the size of the image
     # print(my_image.size)
     # resize image and ignore original aspect ratio
     img_resized = my_image.resize(image_size)
     # changing the file extension from jpg to png changes output brightness. You might need to play with this.
-    img_resized.save('./resized_image.png')
-    data = image.imread('./resized_image.png')
+    data = asarray(image)
     target_tcs = []
     for row in data:
         temp_row = []
         for pixel in row:
             temp_row.append(RGBtoHSBK(pixel))
         target_tcs.append(temp_row)
     # print ("length of target_tcs is " + str(len(target_tcs)))
```

### Comparing `pylifxtiles-0.1.8/pylifxtiles/alphanum.py` & `pylifxtiles-0.1.9/pylifxtiles/alphanum.py`

 * *Files identical despite different names*

### Comparing `pylifxtiles-0.1.8/pylifxtiles/colors.py` & `pylifxtiles-0.1.9/pylifxtiles/colors.py`

 * *Files identical despite different names*

### Comparing `pylifxtiles-0.1.8/pylifxtiles/objects.py` & `pylifxtiles-0.1.9/pylifxtiles/objects.py`

 * *Files identical despite different names*

### Comparing `pylifxtiles-0.1.8/pylifxtiles/tiles.py` & `pylifxtiles-0.1.9/pylifxtiles/tiles.py`

 * *Files identical despite different names*

### Comparing `pylifxtiles-0.1.8/pylifxtiles.egg-info/PKG-INFO` & `pylifxtiles-0.1.9/pylifxtiles.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 Metadata-Version: 2.1
 Name: pylifxtiles
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python binding for LIFX Tiles
 Home-page: https://github.com/netmanchris/pylifxtiles
 Author: netmanchris
 Author-email: python@homekitgeek.com
 License: Apache2
-Description: PYLIFXTILES
-        
-        **READ THIS FIRST**
-        This library is currently in alpha state and should not be used for production installations.
-        Support is not offered at this time, but GITHUB issues are welcome if bugs or potential feature
-        enhancements are found.
-        
-        ##Description
-        
-        This is a sample python language binding for the LIFX Tiles products.
-        
-        Installation
-        
-        Product should be on pip. Can also be installed directly using the typical ways.
-        
-        `pip install -r requirements.txt`
-        
-        
-        
-        
-        
 Keywords: lifx,tiles,api,python
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: dev
 Provides-Extra: test
+License-File: LICENSE
+
+PYLIFXTILES
+
+**READ THIS FIRST**
+This library is currently in alpha state and should not be used for production installations.
+Support is not offered at this time, but GITHUB issues are welcome if bugs or potential feature
+enhancements are found.
+
+##Description
+
+This is a sample python language binding for the LIFX Tiles products.
+
+Installation
+
+Product should be on pip. Can also be installed directly using the typical ways.
+
+`pip install -r requirements.txt`
+
+
+
+
```

### Comparing `pylifxtiles-0.1.8/setup.py` & `pylifxtiles-0.1.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 setup(
         name='pylifxtiles',
 
         # Versions should comply with PEP440.  For a discussion on single-sourcing
         # the version across test_machine.py and the project code, see
         # https://packaging.python.org/en/latest/single_source_version.html
-        version='0.1.8',
+        version='0.1.9',
 
         description='Python binding for LIFX Tiles',
         long_description=long_description,
 
         # The project's main homepage.
         url='https://github.com/netmanchris/pylifxtiles',
 
@@ -68,15 +68,15 @@
         # this:
         #   py_modules=["my_module"],
 
         # List run-time dependencies here.  These will be installed by pip when
         # your project is installed. For an analysis of "install_requires" vs pip's
         # requirements files see:
         # https://packaging.python.org/en/latest/requirements.html
-        install_requires=['requests', 'lifxlan', 'jupyter', 'nose', 'matplotlib', 'Pillow'],
+        install_requires=['requests', 'lifxlan', 'bitstring==3.1.9', 'nose', 'matplotlib', 'Pillow'],
 
         # List additional groups of dependencies here (e.g. development
         # dependencies). You can install these using the following syntax,
         # for example:
         # $ pip install -e .[dev,test]
         extras_require={
             'dev': ['check-manifest'],
```

