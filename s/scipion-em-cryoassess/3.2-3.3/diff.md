# Comparing `tmp/scipion-em-cryoassess-3.2.tar.gz` & `tmp/scipion-em-cryoassess-3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-cryoassess-3.2.tar", last modified: Tue Dec 27 17:01:57 2022, max compression
+gzip compressed data, was "scipion-em-cryoassess-3.3.tar", last modified: Wed May 24 17:48:15 2023, max compression
```

## Comparing `scipion-em-cryoassess-3.2.tar` & `scipion-em-cryoassess-3.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-27 17:01:57.547907 scipion-em-cryoassess-3.2/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2022-12-27 16:59:03.000000 scipion-em-cryoassess-3.2/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2022-12-27 16:59:03.000000 scipion-em-cryoassess-3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      179 2022-12-27 16:59:03.000000 scipion-em-cryoassess-3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2022-12-27 17:01:57.547907 scipion-em-cryoassess-3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2022-12-27 16:59:03.000000 scipion-em-cryoassess-3.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-27 17:01:57.543907 scipion-em-cryoassess-3.2/cryoassess/
--rw-r--r--   0 runner    (1001) docker     (123)     4723 2022-12-27 16:59:03.000000 scipion-em-cryoassess-3.2/cryoassess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2022-12-27 16:59:03.000000 scipion-em-cryoassess-3.2/cryoassess/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2022-12-27 16:59:03.000000 scipion-em-cryoassess-3.2/cryoassess/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-27 17:01:57.543907 scipion-em-cryoassess-3.2/cryoassess/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2022-12-27 16:59:03.000000 scipion-em-cryoassess-3.2/cryoassess/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8255 2022-12-27 16:59:03.000000 scipion-em-cryoassess-3.2/cryoassess/protocols/protocol_2dassess.py
--rw-r--r--   0 runner    (1001) docker     (123)    15099 2022-12-27 16:59:03.000000 scipion-em-cryoassess-3.2/cryoassess/protocols/protocol_micassess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-27 17:01:57.547907 scipion-em-cryoassess-3.2/cryoassess/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2022-12-27 16:59:03.000000 scipion-em-cryoassess-3.2/cryoassess/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2022-12-27 16:59:03.000000 scipion-em-cryoassess-3.2/cryoassess/tests/test_protocols_cryoassess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-27 17:01:57.547907 scipion-em-cryoassess-3.2/scipion_em_cryoassess.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2022-12-27 17:01:57.000000 scipion-em-cryoassess-3.2/scipion_em_cryoassess.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      584 2022-12-27 17:01:57.000000 scipion-em-cryoassess-3.2/scipion_em_cryoassess.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-27 17:01:57.000000 scipion-em-cryoassess-3.2/scipion_em_cryoassess.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2022-12-27 17:01:57.000000 scipion-em-cryoassess-3.2/scipion_em_cryoassess.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2022-12-27 17:01:57.000000 scipion-em-cryoassess-3.2/scipion_em_cryoassess.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2022-12-27 17:01:57.000000 scipion-em-cryoassess-3.2/scipion_em_cryoassess.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-27 17:01:57.547907 scipion-em-cryoassess-3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8494 2022-12-27 16:59:03.000000 scipion-em-cryoassess-3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:48:15.323823 scipion-em-cryoassess-3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-24 17:46:35.000000 scipion-em-cryoassess-3.3/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-24 17:46:35.000000 scipion-em-cryoassess-3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-24 17:46:35.000000 scipion-em-cryoassess-3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-05-24 17:48:15.323823 scipion-em-cryoassess-3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-05-24 17:46:35.000000 scipion-em-cryoassess-3.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:48:15.323823 scipion-em-cryoassess-3.3/cryoassess/
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-05-24 17:46:35.000000 scipion-em-cryoassess-3.3/cryoassess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-24 17:46:35.000000 scipion-em-cryoassess-3.3/cryoassess/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-24 17:46:35.000000 scipion-em-cryoassess-3.3/cryoassess/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:48:15.323823 scipion-em-cryoassess-3.3/cryoassess/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-24 17:46:35.000000 scipion-em-cryoassess-3.3/cryoassess/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-05-24 17:46:35.000000 scipion-em-cryoassess-3.3/cryoassess/protocols/protocol_2dassess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15057 2023-05-24 17:46:35.000000 scipion-em-cryoassess-3.3/cryoassess/protocols/protocol_micassess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:48:15.323823 scipion-em-cryoassess-3.3/cryoassess/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-24 17:46:35.000000 scipion-em-cryoassess-3.3/cryoassess/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-05-24 17:46:35.000000 scipion-em-cryoassess-3.3/cryoassess/tests/test_protocols_cryoassess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:48:15.323823 scipion-em-cryoassess-3.3/scipion_em_cryoassess.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-05-24 17:48:15.000000 scipion-em-cryoassess-3.3/scipion_em_cryoassess.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-24 17:48:15.000000 scipion-em-cryoassess-3.3/scipion_em_cryoassess.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 17:48:15.000000 scipion-em-cryoassess-3.3/scipion_em_cryoassess.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-24 17:48:15.000000 scipion-em-cryoassess-3.3/scipion_em_cryoassess.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-24 17:48:15.000000 scipion-em-cryoassess-3.3/scipion_em_cryoassess.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-24 17:48:15.000000 scipion-em-cryoassess-3.3/scipion_em_cryoassess.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 17:48:15.323823 scipion-em-cryoassess-3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8494 2023-05-24 17:46:35.000000 scipion-em-cryoassess-3.3/setup.py
```

### Comparing `scipion-em-cryoassess-3.2/LICENSE` & `scipion-em-cryoassess-3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-cryoassess-3.2/PKG-INFO` & `scipion-em-cryoassess-3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-cryoassess
-Version: 3.2
+Version: 3.3
 Summary: Plugin to use cryoassess within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-cryoassess
 Author: Grigory Sharov
 Author-email: sharov.grigory@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-cryoassess/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-cryoassess/
```

### Comparing `scipion-em-cryoassess-3.2/README.rst` & `scipion-em-cryoassess-3.3/README.rst`

 * *Files identical despite different names*

### Comparing `scipion-em-cryoassess-3.2/cryoassess/__init__.py` & `scipion-em-cryoassess-3.3/cryoassess/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,22 +28,22 @@
 import pwem
 import pyworkflow.utils as pwutils
 from pyworkflow import Config
 
 from .constants import *
 
 
-__version__ = '3.2'
+__version__ = '3.3'
 _references = ['Li2020']
 _logo = "cryoassess_logo.png"
 
 
 class Plugin(pwem.Plugin):
     _pathVars = [CRYOASSESS_MODELS]
-    _url = "https://github.com/cianfrocco-lab/Automatic-cryoEM-preprocessing"
+    _url = "https://github.com/scipion-em/scipion-em-cryoassess"
     _supportedVersions = VERSIONS
 
     @classmethod
     def _defineVariables(cls):
         cls._defineVar(CRYOASSESS_ENV_ACTIVATION, DEFAULT_ACTIVATION_CMD)
         cls._defineEmVar(CRYOASSESS_MODELS, 'cryoassess-models')
 
@@ -52,14 +52,20 @@
         """ Remove the scipion home and activate the conda environment. """
         activation = cls.getVar(CRYOASSESS_ENV_ACTIVATION)
         scipionHome = Config.SCIPION_HOME + os.path.sep
 
         return activation.replace(scipionHome, "", 1)
 
     @classmethod
+    def getActiveVersion(cls, *args):
+        """ Return the env name that is currently active. """
+        envVar = cls.getVar(CRYOASSESS_ENV_ACTIVATION)
+        return envVar.split()[-1].split("-")[-1]
+
+    @classmethod
     def getEnviron(cls):
         """ Setup the environment variables needed to launch cryoassess. """
         environ = pwutils.Environ(os.environ)
         if 'PYTHONPATH' in environ:
             # this is required for python virtual env to work
             del environ['PYTHONPATH']
         return environ
```

### Comparing `scipion-em-cryoassess-3.2/cryoassess/bibtex.py` & `scipion-em-cryoassess-3.3/cryoassess/bibtex.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryoassess-3.2/cryoassess/constants.py` & `scipion-em-cryoassess-3.3/cryoassess/constants.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryoassess-3.2/cryoassess/protocols/__init__.py` & `scipion-em-cryoassess-3.3/cryoassess/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryoassess-3.2/cryoassess/protocols/protocol_2dassess.py` & `scipion-em-cryoassess-3.3/cryoassess/protocols/protocol_2dassess.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryoassess-3.2/cryoassess/protocols/protocol_micassess.py` & `scipion-em-cryoassess-3.3/cryoassess/protocols/protocol_micassess.py`

 * *Files 0% similar despite different names*

```diff
@@ -277,15 +277,15 @@
         args = ['-i %s ' % os.path.basename(self.getInputFilename(numPass)),
                 '-o output%s ' % numPass,
                 '-m %s' % Plugin.getVar(CRYOASSESS_MODELS),
                 '-b %d' % self.batchSize.get(),
                 '--t1 %0.2f' % self.threshold.get(),
                 '--t2 %0.2f' % self.threshold2.get(),
                 '--threads %d' % self.numberOfThreads.get(),
-                '--gpus %s' % self.gpuList.get().strip().replace(" ", ",")]
+                '--gpus %(GPU)s']
 
         if self._getCameraType() is not None:
             args.append('-d %s' % self._getCameraType())
 
         return args
 
     def _getInputMicrographs(self):
```

### Comparing `scipion-em-cryoassess-3.2/cryoassess/tests/__init__.py` & `scipion-em-cryoassess-3.3/cryoassess/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryoassess-3.2/cryoassess/tests/test_protocols_cryoassess.py` & `scipion-em-cryoassess-3.3/cryoassess/tests/test_protocols_cryoassess.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryoassess-3.2/scipion_em_cryoassess.egg-info/PKG-INFO` & `scipion-em-cryoassess-3.3/scipion_em_cryoassess.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-cryoassess
-Version: 3.2
+Version: 3.3
 Summary: Plugin to use cryoassess within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-cryoassess
 Author: Grigory Sharov
 Author-email: sharov.grigory@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-cryoassess/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-cryoassess/
```

### Comparing `scipion-em-cryoassess-3.2/scipion_em_cryoassess.egg-info/SOURCES.txt` & `scipion-em-cryoassess-3.3/scipion_em_cryoassess.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scipion-em-cryoassess-3.2/setup.py` & `scipion-em-cryoassess-3.3/setup.py`

 * *Files identical despite different names*

