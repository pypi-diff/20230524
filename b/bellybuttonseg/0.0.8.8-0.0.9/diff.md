# Comparing `tmp/bellybuttonseg-0.0.8.8.tar.gz` & `tmp/bellybuttonseg-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bellybuttonseg-0.0.8.8.tar", last modified: Thu Oct  6 16:01:26 2022, max compression
+gzip compressed data, was "bellybuttonseg-0.0.9.tar", last modified: Tue Oct 11 22:00:47 2022, max compression
```

## Comparing `bellybuttonseg-0.0.8.8.tar` & `bellybuttonseg-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 Sam        (501) staff       (20)        0 2022-10-06 16:01:26.101162 bellybuttonseg-0.0.8.8/
--rw-r--r--   0 Sam        (501) staff       (20)     1073 2022-09-14 15:42:50.000000 bellybuttonseg-0.0.8.8/LICENSE.txt
--rw-r--r--   0 Sam        (501) staff       (20)     8035 2022-10-06 16:01:26.101035 bellybuttonseg-0.0.8.8/PKG-INFO
--rw-r--r--   0 Sam        (501) staff       (20)     7433 2022-10-06 15:58:01.000000 bellybuttonseg-0.0.8.8/README.md
--rw-r--r--   0 Sam        (501) staff       (20)     1064 2022-10-06 15:58:07.000000 bellybuttonseg-0.0.8.8/pyproject.toml
--rw-r--r--   0 Sam        (501) staff       (20)       38 2022-10-06 16:01:26.101201 bellybuttonseg-0.0.8.8/setup.cfg
-drwxr-xr-x   0 Sam        (501) staff       (20)        0 2022-10-06 16:01:26.095898 bellybuttonseg-0.0.8.8/src/
-drwxr-xr-x   0 Sam        (501) staff       (20)        0 2022-10-06 16:01:26.100005 bellybuttonseg-0.0.8.8/src/bellybuttonseg/
--rw-r--r--   0 Sam        (501) staff       (20)    18008 2022-09-14 16:58:13.000000 bellybuttonseg-0.0.8.8/src/bellybuttonseg/BBHP_function.py
--rw-r--r--   0 Sam        (501) staff       (20)    33487 2022-09-08 18:31:46.000000 bellybuttonseg-0.0.8.8/src/bellybuttonseg/DataGenerator.py
--rw-r--r--   0 Sam        (501) staff       (20)     2229 2022-09-14 20:37:11.000000 bellybuttonseg-0.0.8.8/src/bellybuttonseg/__init__.py
--rw-r--r--   0 Sam        (501) staff       (20)     4812 2022-10-06 15:02:29.000000 bellybuttonseg-0.0.8.8/src/bellybuttonseg/createdir.py
--rw-r--r--   0 Sam        (501) staff       (20)       79 2022-10-05 15:29:42.000000 bellybuttonseg-0.0.8.8/src/bellybuttonseg/example1.py
--rw-r--r--   0 Sam        (501) staff       (20)     2975 2022-05-20 20:20:28.000000 bellybuttonseg-0.0.8.8/src/bellybuttonseg/generate_network.py
--rw-r--r--   0 Sam        (501) staff       (20)    13194 2022-09-14 19:05:56.000000 bellybuttonseg-0.0.8.8/src/bellybuttonseg/load_save_helpers.py
--rw-r--r--   0 Sam        (501) staff       (20)       79 2022-10-05 15:28:48.000000 bellybuttonseg-0.0.8.8/src/bellybuttonseg/newproject.py
--rw-r--r--   0 Sam        (501) staff       (20)     2780 2022-05-24 21:51:50.000000 bellybuttonseg-0.0.8.8/src/bellybuttonseg/run_BBHP.py
--rw-r--r--   0 Sam        (501) staff       (20)    12620 2022-10-06 15:33:38.000000 bellybuttonseg-0.0.8.8/src/bellybuttonseg/saved_model_functions.py
--rw-r--r--   0 Sam        (501) staff       (20)       70 2022-10-05 15:12:01.000000 bellybuttonseg-0.0.8.8/src/bellybuttonseg/train.py
-drwxr-xr-x   0 Sam        (501) staff       (20)        0 2022-10-06 16:01:26.100857 bellybuttonseg-0.0.8.8/src/bellybuttonseg.egg-info/
--rw-r--r--   0 Sam        (501) staff       (20)     8035 2022-10-06 16:01:26.000000 bellybuttonseg-0.0.8.8/src/bellybuttonseg.egg-info/PKG-INFO
--rw-r--r--   0 Sam        (501) staff       (20)      626 2022-10-06 16:01:26.000000 bellybuttonseg-0.0.8.8/src/bellybuttonseg.egg-info/SOURCES.txt
--rw-r--r--   0 Sam        (501) staff       (20)        1 2022-10-06 16:01:26.000000 bellybuttonseg-0.0.8.8/src/bellybuttonseg.egg-info/dependency_links.txt
--rw-r--r--   0 Sam        (501) staff       (20)       84 2022-10-06 16:01:26.000000 bellybuttonseg-0.0.8.8/src/bellybuttonseg.egg-info/requires.txt
--rw-r--r--   0 Sam        (501) staff       (20)       15 2022-10-06 16:01:26.000000 bellybuttonseg-0.0.8.8/src/bellybuttonseg.egg-info/top_level.txt
+drwxr-xr-x   0 Sam        (501) staff       (20)        0 2022-10-11 22:00:47.676300 bellybuttonseg-0.0.9/
+-rw-r--r--   0 Sam        (501) staff       (20)     1073 2022-09-14 15:42:50.000000 bellybuttonseg-0.0.9/LICENSE.txt
+-rw-r--r--   0 Sam        (501) staff       (20)     8033 2022-10-11 22:00:47.676188 bellybuttonseg-0.0.9/PKG-INFO
+-rw-r--r--   0 Sam        (501) staff       (20)     7433 2022-10-06 15:58:01.000000 bellybuttonseg-0.0.9/README.md
+-rw-r--r--   0 Sam        (501) staff       (20)     1062 2022-10-11 22:00:34.000000 bellybuttonseg-0.0.9/pyproject.toml
+-rw-r--r--   0 Sam        (501) staff       (20)       38 2022-10-11 22:00:47.676341 bellybuttonseg-0.0.9/setup.cfg
+drwxr-xr-x   0 Sam        (501) staff       (20)        0 2022-10-11 22:00:47.670494 bellybuttonseg-0.0.9/src/
+drwxr-xr-x   0 Sam        (501) staff       (20)        0 2022-10-11 22:00:47.675272 bellybuttonseg-0.0.9/src/bellybuttonseg/
+-rw-r--r--   0 Sam        (501) staff       (20)    18036 2022-10-11 21:57:58.000000 bellybuttonseg-0.0.9/src/bellybuttonseg/BBHP_function.py
+-rw-r--r--   0 Sam        (501) staff       (20)    33487 2022-09-08 18:31:46.000000 bellybuttonseg-0.0.9/src/bellybuttonseg/DataGenerator.py
+-rw-r--r--   0 Sam        (501) staff       (20)     2229 2022-09-14 20:37:11.000000 bellybuttonseg-0.0.9/src/bellybuttonseg/__init__.py
+-rw-r--r--   0 Sam        (501) staff       (20)     5407 2022-10-11 21:56:09.000000 bellybuttonseg-0.0.9/src/bellybuttonseg/createdir.py
+-rw-r--r--   0 Sam        (501) staff       (20)       79 2022-10-05 15:29:42.000000 bellybuttonseg-0.0.9/src/bellybuttonseg/example1.py
+-rw-r--r--   0 Sam        (501) staff       (20)     2975 2022-05-20 20:20:28.000000 bellybuttonseg-0.0.9/src/bellybuttonseg/generate_network.py
+-rw-r--r--   0 Sam        (501) staff       (20)    13194 2022-09-14 19:05:56.000000 bellybuttonseg-0.0.9/src/bellybuttonseg/load_save_helpers.py
+-rw-r--r--   0 Sam        (501) staff       (20)       79 2022-10-05 15:28:48.000000 bellybuttonseg-0.0.9/src/bellybuttonseg/newproject.py
+-rw-r--r--   0 Sam        (501) staff       (20)       96 2022-10-11 21:56:22.000000 bellybuttonseg-0.0.9/src/bellybuttonseg/predict.py
+-rw-r--r--   0 Sam        (501) staff       (20)     2780 2022-05-24 21:51:50.000000 bellybuttonseg-0.0.9/src/bellybuttonseg/run_BBHP.py
+-rw-r--r--   0 Sam        (501) staff       (20)    12620 2022-10-06 15:33:38.000000 bellybuttonseg-0.0.9/src/bellybuttonseg/saved_model_functions.py
+-rw-r--r--   0 Sam        (501) staff       (20)       98 2022-10-11 21:56:11.000000 bellybuttonseg-0.0.9/src/bellybuttonseg/train.py
+-rw-r--r--   0 Sam        (501) staff       (20)       95 2022-10-11 21:56:13.000000 bellybuttonseg-0.0.9/src/bellybuttonseg/trainandpredict.py
+drwxr-xr-x   0 Sam        (501) staff       (20)        0 2022-10-11 22:00:47.676018 bellybuttonseg-0.0.9/src/bellybuttonseg.egg-info/
+-rw-r--r--   0 Sam        (501) staff       (20)     8033 2022-10-11 22:00:47.000000 bellybuttonseg-0.0.9/src/bellybuttonseg.egg-info/PKG-INFO
+-rw-r--r--   0 Sam        (501) staff       (20)      694 2022-10-11 22:00:47.000000 bellybuttonseg-0.0.9/src/bellybuttonseg.egg-info/SOURCES.txt
+-rw-r--r--   0 Sam        (501) staff       (20)        1 2022-10-11 22:00:47.000000 bellybuttonseg-0.0.9/src/bellybuttonseg.egg-info/dependency_links.txt
+-rw-r--r--   0 Sam        (501) staff       (20)       84 2022-10-11 22:00:47.000000 bellybuttonseg-0.0.9/src/bellybuttonseg.egg-info/requires.txt
+-rw-r--r--   0 Sam        (501) staff       (20)       15 2022-10-11 22:00:47.000000 bellybuttonseg-0.0.9/src/bellybuttonseg.egg-info/top_level.txt
```

### Comparing `bellybuttonseg-0.0.8.8/LICENSE.txt` & `bellybuttonseg-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bellybuttonseg-0.0.8.8/PKG-INFO` & `bellybuttonseg-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bellybuttonseg
-Version: 0.0.8.8
+Version: 0.0.9
 Summary: An easy-to-use image segmentation package
 Author-email: Sam Dillavou <sam.dillavou@gmail.com>, Jesse Hanlan <jhanlan@sas.upenn.edu>
 License: MIT License
 Project-URL: Homepage, https://github.com/sdillavou/bellybuttonseg
 Project-URL: Bug Tracker, https://github.com/sdillavou/bellybuttonseg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bellybuttonseg-0.0.8.8/README.md` & `bellybuttonseg-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `bellybuttonseg-0.0.8.8/pyproject.toml` & `bellybuttonseg-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bellybuttonseg"
-version = "0.0.8.8"
+version = "0.0.9"
 authors = [
   { name="Sam Dillavou", email="sam.dillavou@gmail.com" },
   { name="Jesse Hanlan", email="jhanlan@sas.upenn.edu " },
 ]
 
 
 dependencies = [
```

### Comparing `bellybuttonseg-0.0.8.8/src/bellybuttonseg/BBHP_function.py` & `bellybuttonseg-0.0.9/src/bellybuttonseg/BBHP_function.py`

 * *Files 2% similar despite different names*

```diff
@@ -307,15 +307,15 @@
         
         print(results)
 
 
         # save results
         save_parameters(results_filename,list(results.keys()),list(results.values()))
 
-    elif num_epochs==0:
+    if num_epochs==0 or not (predict_path is None):
         if os.path.isdir(HP_output_folder)==False:
             print('Original training never made predictions, creating prediction folder now...')
             os.mkdir(HP_output_folder)
 
         # generator for prediction data
         if predict_path is None or predict_path == 'predict_images':
             subfolder = 'predict_images'
```

### Comparing `bellybuttonseg-0.0.8.8/src/bellybuttonseg/DataGenerator.py` & `bellybuttonseg-0.0.9/src/bellybuttonseg/DataGenerator.py`

 * *Files identical despite different names*

### Comparing `bellybuttonseg-0.0.8.8/src/bellybuttonseg/__init__.py` & `bellybuttonseg-0.0.9/src/bellybuttonseg/__init__.py`

 * *Files identical despite different names*

### Comparing `bellybuttonseg-0.0.8.8/src/bellybuttonseg/createdir.py` & `bellybuttonseg-0.0.9/src/bellybuttonseg/createdir.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,21 +5,45 @@
 from load_save_helpers import create_default_params, save_parameters, load_parameters
 from BBHP_function import param_types, BBHP
 from PIL import Image
 import requests 
 
 base_param_name = 'base_parameters'
 
-def runBB():
+# Shell function to run the training and/or prediction using Bellybutton
+def runBB(train=True, predict=False):
     
     
     file_path = get_filepath()
+    dt_string = None
+    predict_path = None
+   
+    idx = file_path[:-1].rfind('/')
+
+    # we are being asked to load a network, change file_path to base folder name and store dt_string
+    if file_path[idx+1:idx+9] == 'outputs_':
+        dt_string = file_path[idx+9:-1]
+        file_path = file_path[:idx+1]
+
     param = load_parameters(file_path+base_param_name,param_types)
 
-    BBHP(file_path,param)#, train_img_count = train_img_count)#,dt_string='22_06_06_20_44_28');#,train_img_count=train_img_count,test_img_count=test_img_count,dt_string=dt_string)
+    
+    if not train:
+        param['HP_train_epochs'] = 0
+
+    if predict:
+        predict_path = 'predict_images'
+
+    
+
+
+    BBHP(file_path,param,predict_path=predict_path,dt_string=dt_string)
+    #, train_img_count = train_img_count)
+    #,dt_string='22_06_06_20_44_28');
+    #,train_img_count=train_img_count,test_img_count=test_img_count,dt_string=dt_string)
 
 
 # returns images of a list of filenames for a given folder
 def createdir(example=0):
     
     # request filepath from user
     file_path = get_filepath()
```

### Comparing `bellybuttonseg-0.0.8.8/src/bellybuttonseg/generate_network.py` & `bellybuttonseg-0.0.9/src/bellybuttonseg/generate_network.py`

 * *Files identical despite different names*

### Comparing `bellybuttonseg-0.0.8.8/src/bellybuttonseg/load_save_helpers.py` & `bellybuttonseg-0.0.9/src/bellybuttonseg/load_save_helpers.py`

 * *Files identical despite different names*

### Comparing `bellybuttonseg-0.0.8.8/src/bellybuttonseg/run_BBHP.py` & `bellybuttonseg-0.0.9/src/bellybuttonseg/run_BBHP.py`

 * *Files identical despite different names*

### Comparing `bellybuttonseg-0.0.8.8/src/bellybuttonseg/saved_model_functions.py` & `bellybuttonseg-0.0.9/src/bellybuttonseg/saved_model_functions.py`

 * *Files identical despite different names*

### Comparing `bellybuttonseg-0.0.8.8/src/bellybuttonseg.egg-info/PKG-INFO` & `bellybuttonseg-0.0.9/src/bellybuttonseg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bellybuttonseg
-Version: 0.0.8.8
+Version: 0.0.9
 Summary: An easy-to-use image segmentation package
 Author-email: Sam Dillavou <sam.dillavou@gmail.com>, Jesse Hanlan <jhanlan@sas.upenn.edu>
 License: MIT License
 Project-URL: Homepage, https://github.com/sdillavou/bellybuttonseg
 Project-URL: Bug Tracker, https://github.com/sdillavou/bellybuttonseg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bellybuttonseg-0.0.8.8/src/bellybuttonseg.egg-info/SOURCES.txt` & `bellybuttonseg-0.0.9/src/bellybuttonseg.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 src/bellybuttonseg/DataGenerator.py
 src/bellybuttonseg/__init__.py
 src/bellybuttonseg/createdir.py
 src/bellybuttonseg/example1.py
 src/bellybuttonseg/generate_network.py
 src/bellybuttonseg/load_save_helpers.py
 src/bellybuttonseg/newproject.py
+src/bellybuttonseg/predict.py
 src/bellybuttonseg/run_BBHP.py
 src/bellybuttonseg/saved_model_functions.py
 src/bellybuttonseg/train.py
+src/bellybuttonseg/trainandpredict.py
 src/bellybuttonseg.egg-info/PKG-INFO
 src/bellybuttonseg.egg-info/SOURCES.txt
 src/bellybuttonseg.egg-info/dependency_links.txt
 src/bellybuttonseg.egg-info/requires.txt
 src/bellybuttonseg.egg-info/top_level.txt
```

