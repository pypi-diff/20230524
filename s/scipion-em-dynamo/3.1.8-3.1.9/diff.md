# Comparing `tmp/scipion-em-dynamo-3.1.8.tar.gz` & `tmp/scipion-em-dynamo-3.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-dynamo-3.1.8.tar", last modified: Mon Jan  9 16:38:31 2023, max compression
+gzip compressed data, was "scipion-em-dynamo-3.1.9.tar", last modified: Tue Jan 10 16:40:32 2023, max compression
```

## Comparing `scipion-em-dynamo-3.1.8.tar` & `scipion-em-dynamo-3.1.9.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 16:38:31.943767 scipion-em-dynamo-3.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-01-09 16:34:38.000000 scipion-em-dynamo-3.1.8/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-01-09 16:34:38.000000 scipion-em-dynamo-3.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-01-09 16:34:38.000000 scipion-em-dynamo-3.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-01-09 16:38:31.943767 scipion-em-dynamo-3.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-01-09 16:34:38.000000 scipion-em-dynamo-3.1.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 16:38:31.939767 scipion-em-dynamo-3.1.8/dynamo/
--rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-01-09 16:34:38.000000 scipion-em-dynamo-3.1.8/dynamo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-01-09 16:34:38.000000 scipion-em-dynamo-3.1.8/dynamo/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-01-09 16:34:38.000000 scipion-em-dynamo-3.1.8/dynamo/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 16:38:31.939767 scipion-em-dynamo-3.1.8/dynamo/convert/
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-01-09 16:34:38.000000 scipion-em-dynamo-3.1.8/dynamo/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10638 2023-01-09 16:34:38.000000 scipion-em-dynamo-3.1.8/dynamo/convert/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    48014 2023-01-09 16:34:38.000000 scipion-em-dynamo-3.1.8/dynamo/icon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 16:38:31.939767 scipion-em-dynamo-3.1.8/dynamo/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-01-09 16:34:38.000000 scipion-em-dynamo-3.1.8/dynamo/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6176 2023-01-09 16:34:38.000000 scipion-em-dynamo-3.1.8/dynamo/protocols/protocol_bin_tomograms.py
--rw-r--r--   0 runner    (1001) docker     (123)     8953 2023-01-09 16:34:38.000000 scipion-em-dynamo-3.1.8/dynamo/protocols/protocol_boxing.py
--rw-r--r--   0 runner    (1001) docker     (123)     7523 2023-01-09 16:34:38.000000 scipion-em-dynamo-3.1.8/dynamo/protocols/protocol_coords_to_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    14043 2023-01-09 16:34:38.000000 scipion-em-dynamo-3.1.8/dynamo/protocols/protocol_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-01-09 16:34:38.000000 scipion-em-dynamo-3.1.8/dynamo/protocols/protocol_import_subtomos.py
--rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-01-09 16:34:38.000000 scipion-em-dynamo-3.1.8/dynamo/protocols/protocol_import_tomograms.py
--rw-r--r--   0 runner    (1001) docker     (123)    22064 2023-01-09 16:34:38.000000 scipion-em-dynamo-3.1.8/dynamo/protocols/protocol_model_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     8751 2023-01-09 16:34:38.000000 scipion-em-dynamo-3.1.8/dynamo/protocols/protocol_subBoxing.py
--rw-r--r--   0 runner    (1001) docker     (123)    35543 2023-01-09 16:34:38.000000 scipion-em-dynamo-3.1.8/dynamo/protocols/protocol_subtomo_MRA.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-01-09 16:34:38.000000 scipion-em-dynamo-3.1.8/dynamo/protocols.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 16:38:31.939767 scipion-em-dynamo-3.1.8/dynamo/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-01-09 16:34:38.000000 scipion-em-dynamo-3.1.8/dynamo/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23232 2023-01-09 16:34:38.000000 scipion-em-dynamo-3.1.8/dynamo/tests/test_dynamo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 16:38:31.939767 scipion-em-dynamo-3.1.8/dynamo/viewers/
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-01-09 16:34:38.000000 scipion-em-dynamo-3.1.8/dynamo/viewers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-01-09 16:34:38.000000 scipion-em-dynamo-3.1.8/dynamo/viewers/viewers_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-01-09 16:34:38.000000 scipion-em-dynamo-3.1.8/dynamo/viewers/views_tkinter_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-01-09 16:34:38.000000 scipion-em-dynamo-3.1.8/dynamo/wizards.py
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-01-09 16:34:38.000000 scipion-em-dynamo-3.1.8/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 16:38:31.939767 scipion-em-dynamo-3.1.8/scipion_em_dynamo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-01-09 16:38:31.000000 scipion-em-dynamo-3.1.8/scipion_em_dynamo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-01-09 16:38:31.000000 scipion-em-dynamo-3.1.8/scipion_em_dynamo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-09 16:38:31.000000 scipion-em-dynamo-3.1.8/scipion_em_dynamo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-01-09 16:38:31.000000 scipion-em-dynamo-3.1.8/scipion_em_dynamo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-01-09 16:38:31.000000 scipion-em-dynamo-3.1.8/scipion_em_dynamo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-09 16:38:31.000000 scipion-em-dynamo-3.1.8/scipion_em_dynamo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-09 16:38:31.943767 scipion-em-dynamo-3.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-01-09 16:34:38.000000 scipion-em-dynamo-3.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 16:40:32.485641 scipion-em-dynamo-3.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-01-10 16:37:46.000000 scipion-em-dynamo-3.1.9/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-01-10 16:37:46.000000 scipion-em-dynamo-3.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-01-10 16:37:46.000000 scipion-em-dynamo-3.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-01-10 16:40:32.485641 scipion-em-dynamo-3.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-01-10 16:37:46.000000 scipion-em-dynamo-3.1.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 16:40:32.481641 scipion-em-dynamo-3.1.9/dynamo/
+-rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-01-10 16:37:46.000000 scipion-em-dynamo-3.1.9/dynamo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-01-10 16:37:46.000000 scipion-em-dynamo-3.1.9/dynamo/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-01-10 16:37:46.000000 scipion-em-dynamo-3.1.9/dynamo/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 16:40:32.481641 scipion-em-dynamo-3.1.9/dynamo/convert/
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-01-10 16:37:46.000000 scipion-em-dynamo-3.1.9/dynamo/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10638 2023-01-10 16:37:46.000000 scipion-em-dynamo-3.1.9/dynamo/convert/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48014 2023-01-10 16:37:46.000000 scipion-em-dynamo-3.1.9/dynamo/icon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 16:40:32.481641 scipion-em-dynamo-3.1.9/dynamo/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-01-10 16:37:46.000000 scipion-em-dynamo-3.1.9/dynamo/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6176 2023-01-10 16:37:46.000000 scipion-em-dynamo-3.1.9/dynamo/protocols/protocol_bin_tomograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8953 2023-01-10 16:37:46.000000 scipion-em-dynamo-3.1.9/dynamo/protocols/protocol_boxing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7523 2023-01-10 16:37:46.000000 scipion-em-dynamo-3.1.9/dynamo/protocols/protocol_coords_to_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14043 2023-01-10 16:37:46.000000 scipion-em-dynamo-3.1.9/dynamo/protocols/protocol_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-01-10 16:37:46.000000 scipion-em-dynamo-3.1.9/dynamo/protocols/protocol_import_subtomos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-01-10 16:37:46.000000 scipion-em-dynamo-3.1.9/dynamo/protocols/protocol_import_tomograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22064 2023-01-10 16:37:46.000000 scipion-em-dynamo-3.1.9/dynamo/protocols/protocol_model_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8751 2023-01-10 16:37:46.000000 scipion-em-dynamo-3.1.9/dynamo/protocols/protocol_subBoxing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35543 2023-01-10 16:37:46.000000 scipion-em-dynamo-3.1.9/dynamo/protocols/protocol_subtomo_MRA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-01-10 16:37:46.000000 scipion-em-dynamo-3.1.9/dynamo/protocols.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 16:40:32.481641 scipion-em-dynamo-3.1.9/dynamo/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-01-10 16:37:46.000000 scipion-em-dynamo-3.1.9/dynamo/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23232 2023-01-10 16:37:46.000000 scipion-em-dynamo-3.1.9/dynamo/tests/test_dynamo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 16:40:32.481641 scipion-em-dynamo-3.1.9/dynamo/viewers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-01-10 16:37:46.000000 scipion-em-dynamo-3.1.9/dynamo/viewers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-01-10 16:37:46.000000 scipion-em-dynamo-3.1.9/dynamo/viewers/viewers_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-01-10 16:37:46.000000 scipion-em-dynamo-3.1.9/dynamo/viewers/views_tkinter_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-01-10 16:37:46.000000 scipion-em-dynamo-3.1.9/dynamo/wizards.py
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-01-10 16:37:46.000000 scipion-em-dynamo-3.1.9/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 16:40:32.481641 scipion-em-dynamo-3.1.9/scipion_em_dynamo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-01-10 16:40:32.000000 scipion-em-dynamo-3.1.9/scipion_em_dynamo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-01-10 16:40:32.000000 scipion-em-dynamo-3.1.9/scipion_em_dynamo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-10 16:40:32.000000 scipion-em-dynamo-3.1.9/scipion_em_dynamo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-01-10 16:40:32.000000 scipion-em-dynamo-3.1.9/scipion_em_dynamo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-01-10 16:40:32.000000 scipion-em-dynamo-3.1.9/scipion_em_dynamo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-10 16:40:32.000000 scipion-em-dynamo-3.1.9/scipion_em_dynamo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-10 16:40:32.485641 scipion-em-dynamo-3.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-01-10 16:37:46.000000 scipion-em-dynamo-3.1.9/setup.py
```

### Comparing `scipion-em-dynamo-3.1.8/CHANGES.txt` & `scipion-em-dynamo-3.1.9/CHANGES.txt`

 * *Files identical despite different names*

### Comparing `scipion-em-dynamo-3.1.8/LICENSE` & `scipion-em-dynamo-3.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-dynamo-3.1.8/PKG-INFO` & `scipion-em-dynamo-3.1.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: scipion-em-dynamo
-Version: 3.1.8
+Version: 3.1.9
 Summary: Scipion plugin for dynamo.
 Home-page: https://github.com/scipion-em/scipion-em-dynamo
 Author: I2PC
 Author-email: scipion@cnb.csic.es
 License: UNKNOWN
 Description: =======================
         Scipion - Dynamo plugin
```

### Comparing `scipion-em-dynamo-3.1.8/dynamo/__init__.py` & `scipion-em-dynamo-3.1.9/dynamo/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 from os.path import join
 import subprocess
 import pwem
 import pyworkflow.utils as pwutils
 from .constants import *
 
-__version__ = '3.1.8'
+__version__ = '3.1.9'
 _logo = "icon.png"
 _references = ['CASTANODIEZ2012139']
 
 class Plugin(pwem.Plugin):
     _homeVar = DYNAMO_HOME
     _pathVars = [DYNAMO_HOME]
     # _supportedVersions =
@@ -47,16 +47,19 @@
     def getEnviron(cls):
         """ Create the needed environment for Dynamo programs. """
         environ = pwutils.Environ(os.environ)
         dyn_home = cls.getHome()
         # For GPU, we need to add to LD_LIBRARY_PATH the path to Cuda/lib
         environ.update({
             'PATH': dyn_home + '/matlab/bin:' + dyn_home + '/matlab/src:' + dyn_home + '/cuda/bin:' + dyn_home + '/mpi',
-            'LD_LIBRARY_PATH': dyn_home + '/MCRLinux/runtime/glnxa64:' + dyn_home + '/MCRLinux/bin/glnxa64:' +
-                               dyn_home + '/MCRLinux/sys/os/glnxa64:' + pwem.Config.CUDA_LIB,
+            'LD_LIBRARY_PATH': ":".join(dyn_home + '/MCRLinux/runtime/glnxa64',
+                                        dyn_home + '/MCRLinux/bin/glnxa64',
+                                        dyn_home + '/MCRLinux/sys/os/glnxa64',
+                                        dyn_home + '/MCRLinux/sys/opengl/lib/glnxa64',
+                                        pwem.Config.CUDA_LIB),
             'DYNAMO_ROOT': dyn_home
         }, position=pwutils.Environ.BEGIN)
         return environ
 
     @classmethod
     def getDynamoProgram(cls):
         return join(cls.getHome(), 'matlab', 'bin', DYNAMO_PROGRAM)
```

### Comparing `scipion-em-dynamo-3.1.8/dynamo/bibtex.py` & `scipion-em-dynamo-3.1.9/dynamo/bibtex.py`

 * *Files identical despite different names*

### Comparing `scipion-em-dynamo-3.1.8/dynamo/constants.py` & `scipion-em-dynamo-3.1.9/dynamo/constants.py`

 * *Files identical despite different names*

### Comparing `scipion-em-dynamo-3.1.8/dynamo/convert/__init__.py` & `scipion-em-dynamo-3.1.9/dynamo/convert/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-dynamo-3.1.8/dynamo/convert/convert.py` & `scipion-em-dynamo-3.1.9/dynamo/convert/convert.py`

 * *Files identical despite different names*

### Comparing `scipion-em-dynamo-3.1.8/dynamo/icon.png` & `scipion-em-dynamo-3.1.9/dynamo/icon.png`

 * *Files identical despite different names*

### Comparing `scipion-em-dynamo-3.1.8/dynamo/protocols/__init__.py` & `scipion-em-dynamo-3.1.9/dynamo/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-dynamo-3.1.8/dynamo/protocols/protocol_bin_tomograms.py` & `scipion-em-dynamo-3.1.9/dynamo/protocols/protocol_bin_tomograms.py`

 * *Files identical despite different names*

### Comparing `scipion-em-dynamo-3.1.8/dynamo/protocols/protocol_boxing.py` & `scipion-em-dynamo-3.1.9/dynamo/protocols/protocol_boxing.py`

 * *Files identical despite different names*

### Comparing `scipion-em-dynamo-3.1.8/dynamo/protocols/protocol_coords_to_model.py` & `scipion-em-dynamo-3.1.9/dynamo/protocols/protocol_coords_to_model.py`

 * *Files identical despite different names*

### Comparing `scipion-em-dynamo-3.1.8/dynamo/protocols/protocol_extraction.py` & `scipion-em-dynamo-3.1.9/dynamo/protocols/protocol_extraction.py`

 * *Files identical despite different names*

### Comparing `scipion-em-dynamo-3.1.8/dynamo/protocols/protocol_import_subtomos.py` & `scipion-em-dynamo-3.1.9/dynamo/protocols/protocol_import_subtomos.py`

 * *Files identical despite different names*

### Comparing `scipion-em-dynamo-3.1.8/dynamo/protocols/protocol_import_tomograms.py` & `scipion-em-dynamo-3.1.9/dynamo/protocols/protocol_import_tomograms.py`

 * *Files identical despite different names*

### Comparing `scipion-em-dynamo-3.1.8/dynamo/protocols/protocol_model_workflow.py` & `scipion-em-dynamo-3.1.9/dynamo/protocols/protocol_model_workflow.py`

 * *Files identical despite different names*

### Comparing `scipion-em-dynamo-3.1.8/dynamo/protocols/protocol_subBoxing.py` & `scipion-em-dynamo-3.1.9/dynamo/protocols/protocol_subBoxing.py`

 * *Files identical despite different names*

### Comparing `scipion-em-dynamo-3.1.8/dynamo/protocols/protocol_subtomo_MRA.py` & `scipion-em-dynamo-3.1.9/dynamo/protocols/protocol_subtomo_MRA.py`

 * *Files identical despite different names*

### Comparing `scipion-em-dynamo-3.1.8/dynamo/protocols.conf` & `scipion-em-dynamo-3.1.9/dynamo/protocols.conf`

 * *Files identical despite different names*

### Comparing `scipion-em-dynamo-3.1.8/dynamo/tests/__init__.py` & `scipion-em-dynamo-3.1.9/dynamo/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-dynamo-3.1.8/dynamo/tests/test_dynamo.py` & `scipion-em-dynamo-3.1.9/dynamo/tests/test_dynamo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-dynamo-3.1.8/dynamo/viewers/__init__.py` & `scipion-em-dynamo-3.1.9/dynamo/viewers/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-dynamo-3.1.8/dynamo/viewers/viewers_data.py` & `scipion-em-dynamo-3.1.9/dynamo/viewers/viewers_data.py`

 * *Files identical despite different names*

### Comparing `scipion-em-dynamo-3.1.8/dynamo/viewers/views_tkinter_tree.py` & `scipion-em-dynamo-3.1.9/dynamo/viewers/views_tkinter_tree.py`

 * *Files identical despite different names*

### Comparing `scipion-em-dynamo-3.1.8/dynamo/wizards.py` & `scipion-em-dynamo-3.1.9/dynamo/wizards.py`

 * *Files identical despite different names*

### Comparing `scipion-em-dynamo-3.1.8/scipion_em_dynamo.egg-info/PKG-INFO` & `scipion-em-dynamo-3.1.9/scipion_em_dynamo.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: scipion-em-dynamo
-Version: 3.1.8
+Version: 3.1.9
 Summary: Scipion plugin for dynamo.
 Home-page: https://github.com/scipion-em/scipion-em-dynamo
 Author: I2PC
 Author-email: scipion@cnb.csic.es
 License: UNKNOWN
 Description: =======================
         Scipion - Dynamo plugin
```

### Comparing `scipion-em-dynamo-3.1.8/scipion_em_dynamo.egg-info/SOURCES.txt` & `scipion-em-dynamo-3.1.9/scipion_em_dynamo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scipion-em-dynamo-3.1.8/setup.py` & `scipion-em-dynamo-3.1.9/setup.py`

 * *Files identical despite different names*

