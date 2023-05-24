# Comparing `tmp/do_mpc-4.5.0.tar.gz` & `tmp/do_mpc-4.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "do_mpc-4.5.0.tar", last modified: Tue Mar 28 07:12:09 2023, max compression
+gzip compressed data, was "do_mpc-4.5.1.tar", last modified: Tue Mar 28 09:04:29 2023, max compression
```

## Comparing `do_mpc-4.5.0.tar` & `do_mpc-4.5.1.tar`

### file list

```diff
@@ -1,33 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 07:12:09.857758 do_mpc-4.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     7361 2023-03-28 07:11:53.000000 do_mpc-4.5.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-03-28 07:12:09.857758 do_mpc-4.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-03-28 07:11:53.000000 do_mpc-4.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 07:12:09.853758 do_mpc-4.5.0/do_mpc/
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-03-28 07:11:53.000000 do_mpc-4.5.0/do_mpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-28 07:11:53.000000 do_mpc-4.5.0/do_mpc/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    17565 2023-03-28 07:11:53.000000 do_mpc-4.5.0/do_mpc/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    22170 2023-03-28 07:11:53.000000 do_mpc-4.5.0/do_mpc/graphics.py
--rw-r--r--   0 runner    (1001) docker     (123)    47625 2023-03-28 07:11:53.000000 do_mpc-4.5.0/do_mpc/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 07:12:09.853758 do_mpc-4.5.0/do_mpc/sampling/
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-03-28 07:11:53.000000 do_mpc-4.5.0/do_mpc/sampling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13981 2023-03-28 07:11:53.000000 do_mpc-4.5.0/do_mpc/sampling/_datahandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9351 2023-03-28 07:11:53.000000 do_mpc-4.5.0/do_mpc/sampling/_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11259 2023-03-28 07:11:53.000000 do_mpc-4.5.0/do_mpc/sampling/_samplingplanner.py
--rw-r--r--   0 runner    (1001) docker     (123)    20976 2023-03-28 07:11:53.000000 do_mpc-4.5.0/do_mpc/simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 07:12:09.853758 do_mpc-4.5.0/do_mpc/sysid/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-03-28 07:11:53.000000 do_mpc-4.5.0/do_mpc/sysid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14882 2023-03-28 07:11:53.000000 do_mpc-4.5.0/do_mpc/sysid/_onnxconversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 07:12:09.857758 do_mpc-4.5.0/do_mpc/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-03-28 07:11:53.000000 do_mpc-4.5.0/do_mpc/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-03-28 07:11:53.000000 do_mpc-4.5.0/do_mpc/tools/_casstructure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-03-28 07:11:53.000000 do_mpc-4.5.0/do_mpc/tools/_indexedproperty.py
--rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-03-28 07:11:53.000000 do_mpc-4.5.0/do_mpc/tools/_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-03-28 07:11:53.000000 do_mpc-4.5.0/do_mpc/tools/_timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 07:12:09.853758 do_mpc-4.5.0/do_mpc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-03-28 07:12:09.000000 do_mpc-4.5.0/do_mpc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-03-28 07:12:09.000000 do_mpc-4.5.0/do_mpc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 07:12:09.000000 do_mpc-4.5.0/do_mpc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-28 07:12:09.000000 do_mpc-4.5.0/do_mpc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-28 07:12:09.000000 do_mpc-4.5.0/do_mpc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 07:12:09.857758 do_mpc-4.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-03-28 07:11:54.000000 do_mpc-4.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:04:29.693614 do_mpc-4.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     7361 2023-03-28 09:04:20.000000 do_mpc-4.5.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-03-28 09:04:29.693614 do_mpc-4.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-03-28 09:04:20.000000 do_mpc-4.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:04:29.693614 do_mpc-4.5.1/do_mpc/
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-03-28 09:04:20.000000 do_mpc-4.5.1/do_mpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-28 09:04:20.000000 do_mpc-4.5.1/do_mpc/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:04:29.693614 do_mpc-4.5.1/do_mpc/controller/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-03-28 09:04:20.000000 do_mpc-4.5.1/do_mpc/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21066 2023-03-28 09:04:20.000000 do_mpc-4.5.1/do_mpc/controller/_lqr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58653 2023-03-28 09:04:20.000000 do_mpc-4.5.1/do_mpc/controller/_mpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17565 2023-03-28 09:04:20.000000 do_mpc-4.5.1/do_mpc/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:04:29.693614 do_mpc-4.5.1/do_mpc/differentiator/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-03-28 09:04:20.000000 do_mpc-4.5.1/do_mpc/differentiator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-03-28 09:04:20.000000 do_mpc-4.5.1/do_mpc/differentiator/_nlpdifferentiator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7964 2023-03-28 09:04:20.000000 do_mpc-4.5.1/do_mpc/differentiator/_nlphandler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:04:29.693614 do_mpc-4.5.1/do_mpc/estimator/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-28 09:04:20.000000 do_mpc-4.5.1/do_mpc/estimator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-03-28 09:04:20.000000 do_mpc-4.5.1/do_mpc/estimator/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-03-28 09:04:20.000000 do_mpc-4.5.1/do_mpc/estimator/_ekf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55990 2023-03-28 09:04:20.000000 do_mpc-4.5.1/do_mpc/estimator/_mhe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22170 2023-03-28 09:04:20.000000 do_mpc-4.5.1/do_mpc/graphics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:04:29.693614 do_mpc-4.5.1/do_mpc/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-03-28 09:04:20.000000 do_mpc-4.5.1/do_mpc/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-03-28 09:04:20.000000 do_mpc-4.5.1/do_mpc/model/_dae2odeconversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6872 2023-03-28 09:04:20.000000 do_mpc-4.5.1/do_mpc/model/_iteratedvariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-03-28 09:04:20.000000 do_mpc-4.5.1/do_mpc/model/_linearize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15726 2023-03-28 09:04:20.000000 do_mpc-4.5.1/do_mpc/model/_linearmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46533 2023-03-28 09:04:20.000000 do_mpc-4.5.1/do_mpc/model/_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47625 2023-03-28 09:04:20.000000 do_mpc-4.5.1/do_mpc/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:04:29.693614 do_mpc-4.5.1/do_mpc/sampling/
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-03-28 09:04:20.000000 do_mpc-4.5.1/do_mpc/sampling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13981 2023-03-28 09:04:20.000000 do_mpc-4.5.1/do_mpc/sampling/_datahandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9351 2023-03-28 09:04:20.000000 do_mpc-4.5.1/do_mpc/sampling/_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11259 2023-03-28 09:04:20.000000 do_mpc-4.5.1/do_mpc/sampling/_samplingplanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20976 2023-03-28 09:04:20.000000 do_mpc-4.5.1/do_mpc/simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:04:29.693614 do_mpc-4.5.1/do_mpc/sysid/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-03-28 09:04:20.000000 do_mpc-4.5.1/do_mpc/sysid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14288 2023-03-28 09:04:20.000000 do_mpc-4.5.1/do_mpc/sysid/_onnxconversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:04:29.693614 do_mpc-4.5.1/do_mpc/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-03-28 09:04:20.000000 do_mpc-4.5.1/do_mpc/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-03-28 09:04:20.000000 do_mpc-4.5.1/do_mpc/tools/_casstructure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-03-28 09:04:20.000000 do_mpc-4.5.1/do_mpc/tools/_indexedproperty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-03-28 09:04:20.000000 do_mpc-4.5.1/do_mpc/tools/_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-03-28 09:04:20.000000 do_mpc-4.5.1/do_mpc/tools/_timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:04:29.693614 do_mpc-4.5.1/do_mpc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-03-28 09:04:29.000000 do_mpc-4.5.1/do_mpc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-03-28 09:04:29.000000 do_mpc-4.5.1/do_mpc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 09:04:29.000000 do_mpc-4.5.1/do_mpc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-28 09:04:29.000000 do_mpc-4.5.1/do_mpc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-28 09:04:29.000000 do_mpc-4.5.1/do_mpc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 09:04:29.693614 do_mpc-4.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-03-28 09:04:20.000000 do_mpc-4.5.1/setup.py
```

### Comparing `do_mpc-4.5.0/LICENSE.txt` & `do_mpc-4.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `do_mpc-4.5.0/PKG-INFO` & `do_mpc-4.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: do_mpc
-Version: 4.5.0
+Version: 4.5.1
 Home-page: https://www.do-mpc.com
 Author: Sergio Lucia and Felix Fiedler
 Author-email: sergio.lucia@tu-berlin.de
 License: GNU Lesser General Public License version 3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `do_mpc-4.5.0/README.md` & `do_mpc-4.5.1/README.md`

 * *Files identical despite different names*

### Comparing `do_mpc-4.5.0/do_mpc/__init__.py` & `do_mpc-4.5.1/do_mpc/__init__.py`

 * *Files identical despite different names*

### Comparing `do_mpc-4.5.0/do_mpc/data.py` & `do_mpc-4.5.1/do_mpc/data.py`

 * *Files identical despite different names*

### Comparing `do_mpc-4.5.0/do_mpc/graphics.py` & `do_mpc-4.5.1/do_mpc/graphics.py`

 * *Files identical despite different names*

### Comparing `do_mpc-4.5.0/do_mpc/optimizer.py` & `do_mpc-4.5.1/do_mpc/optimizer.py`

 * *Files identical despite different names*

### Comparing `do_mpc-4.5.0/do_mpc/sampling/__init__.py` & `do_mpc-4.5.1/do_mpc/sampling/__init__.py`

 * *Files identical despite different names*

### Comparing `do_mpc-4.5.0/do_mpc/sampling/_datahandler.py` & `do_mpc-4.5.1/do_mpc/sampling/_datahandler.py`

 * *Files identical despite different names*

### Comparing `do_mpc-4.5.0/do_mpc/sampling/_sampler.py` & `do_mpc-4.5.1/do_mpc/sampling/_sampler.py`

 * *Files identical despite different names*

### Comparing `do_mpc-4.5.0/do_mpc/sampling/_samplingplanner.py` & `do_mpc-4.5.1/do_mpc/sampling/_samplingplanner.py`

 * *Files identical despite different names*

### Comparing `do_mpc-4.5.0/do_mpc/simulator.py` & `do_mpc-4.5.1/do_mpc/simulator.py`

 * *Files identical despite different names*

### Comparing `do_mpc-4.5.0/do_mpc/sysid/_onnxconversion.py` & `do_mpc-4.5.1/do_mpc/sysid/_onnxconversion.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 import casadi
-import onnx
 import numpy as np
 import pdb
+import importlib
 
 
+# Import optional packages
+
+ONNX_INSTALLED = False
+
+if importlib.util.find_spec("onnx"):
+    import onnx
+    ONNX_INSTALLED = True
+
 class ONNXConversion:
     """ Transform `ONNX model <https://onnx.ai>`_. 
     The transformation returns a CasADi expression of the model and can be used e.g. in the :py:class:`do_mpc.model.Model` class.
 
     .. note::
 
         The feature is experimental and currently only has a limited number of supported operations.
@@ -82,39 +90,25 @@
     :param model_name: (Optional) name of the model
     :type model_name: str
     :param from_keras: (Optional) Flag to indicate that the model is a Keras model.
     :type from_keras: bool
 
     """
     
-    def __init__(self, model, model_name=None, from_keras=False):  
+    def __init__(self, model, model_name=None):  
+        if not ONNX_INSTALLED:
+            raise Exception("The package 'onnx' is not installed. Please install it..")
+
         # In case of a keras model as input, convert it to an ONNX model
-        if from_keras:
-            try:
-                import tf2onnx
-                import tensorflow as tf
-            except:
-                raise Exception("The package 'tf2onnx' or 'tensorflow' is not installed. Please install it..")
-
-            assert isinstance(model,(tf.keras.Model)), 'The input model is not a Keras model.'
-
-            model_input_signature = [tf.TensorSpec(np.array(self._determine_shape(inp_spec.shape)),
-                                        name=inp_spec.name) for inp_spec in model.input_spec]
-            self.onnx_model, _ = tf2onnx.convert.from_keras(model,output_path=None,
-                                                            input_signature=model_input_signature)
-            self.name = "casadi_model" if not isinstance(model_name, (str)) else model.name
         
-        elif isinstance(model,(onnx.onnx_ml_pb2.ModelProto)):
+        if isinstance(model,(onnx.onnx_ml_pb2.ModelProto)):
             self.onnx_model = model
             self.name = "casadi_model" if not isinstance(model_name, (str)) else model_name
-
         else:
             raise Exception("Please pass a keras or onnx model as input. Please use the from_keras flag to convert a keras model to an onnx model.")
-            
-        
         
         # From the ONNX model the graph and the nodes and the initializers are directly inherited
         self.graph = self.onnx_model.graph
         self.nodes = list(self.graph.node)
         onnx_initializers = list(self.graph.initializer)
         
         # The initialized tensors are converted into the numpy readable format  before assignment
```

### Comparing `do_mpc-4.5.0/do_mpc/tools/__init__.py` & `do_mpc-4.5.1/do_mpc/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `do_mpc-4.5.0/do_mpc/tools/_casstructure.py` & `do_mpc-4.5.1/do_mpc/tools/_casstructure.py`

 * *Files identical despite different names*

### Comparing `do_mpc-4.5.0/do_mpc/tools/_indexedproperty.py` & `do_mpc-4.5.1/do_mpc/tools/_indexedproperty.py`

 * *Files identical despite different names*

### Comparing `do_mpc-4.5.0/do_mpc/tools/_structure.py` & `do_mpc-4.5.1/do_mpc/tools/_structure.py`

 * *Files identical despite different names*

### Comparing `do_mpc-4.5.0/do_mpc/tools/_timer.py` & `do_mpc-4.5.1/do_mpc/tools/_timer.py`

 * *Files identical despite different names*

### Comparing `do_mpc-4.5.0/do_mpc.egg-info/PKG-INFO` & `do_mpc-4.5.1/do_mpc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: do-mpc
-Version: 4.5.0
+Version: 4.5.1
 Home-page: https://www.do-mpc.com
 Author: Sergio Lucia and Felix Fiedler
 Author-email: sergio.lucia@tu-berlin.de
 License: GNU Lesser General Public License version 3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

