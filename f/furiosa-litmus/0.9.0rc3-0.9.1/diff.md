# Comparing `tmp/furiosa-litmus-0.9.0rc3.tar.gz` & `tmp/furiosa_litmus-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "furiosa-litmus-0.9.0rc3.tar", last modified: Fri Apr 14 21:25:44 2023, max compression
+gzip compressed data, was "furiosa_litmus-0.9.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `furiosa-litmus-0.9.0rc3.tar` & `furiosa_litmus-0.9.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      353 2023-04-14 21:20:22.712571 furiosa-litmus-0.9.0rc3/Makefile
--rw-r--r--   0        0        0      224 2023-04-14 21:20:22.712571 furiosa-litmus-0.9.0rc3/README.md
--rw-r--r--   0        0        0     7304 2023-04-14 21:20:22.712571 furiosa-litmus-0.9.0rc3/furiosa/litmus/__init__.py
--rw-r--r--   0        0        0       17 2023-04-14 21:22:15.679548 furiosa-litmus-0.9.0rc3/furiosa/litmus/git_version.txt
--rw-r--r--   0        0        0     2418 2023-04-14 21:20:22.712571 furiosa-litmus-0.9.0rc3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-14 21:20:22.712571 furiosa-litmus-0.9.0rc3/tests/__init__.py
--rw-r--r--   0        0        0      878 2023-04-14 21:20:22.712571 furiosa-litmus-0.9.0rc3/tests/test_litmus.py
--rw-r--r--   0        0        0     1466 1970-01-01 00:00:00.000000 furiosa-litmus-0.9.0rc3/PKG-INFO
+-rw-r--r--   0        0        0      353 2023-05-24 05:34:31.220841 furiosa_litmus-0.9.1/Makefile
+-rw-r--r--   0        0        0      224 2023-05-24 05:34:31.220841 furiosa_litmus-0.9.1/README.md
+-rw-r--r--   0        0        0     7334 2023-05-24 05:34:31.220841 furiosa_litmus-0.9.1/furiosa/litmus/__init__.py
+-rw-r--r--   0        0        0       14 2023-05-24 05:37:05.075809 furiosa_litmus-0.9.1/furiosa/litmus/git_version.txt
+-rw-r--r--   0        0        0     2413 2023-05-24 05:34:31.220841 furiosa_litmus-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-24 05:34:31.220841 furiosa_litmus-0.9.1/tests/__init__.py
+-rw-r--r--   0        0        0      878 2023-05-24 05:34:31.220841 furiosa_litmus-0.9.1/tests/test_litmus.py
+-rw-r--r--   0        0        0     1463 1970-01-01 00:00:00.000000 furiosa_litmus-0.9.1/PKG-INFO
```

### Comparing `furiosa-litmus-0.9.0rc3/furiosa/litmus/__init__.py` & `furiosa_litmus-0.9.1/furiosa/litmus/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     Returns:
         A dict mapping tensors in the model to their minimum and maximum values.
     """
     calibrator = Calibrator(model, CalibrationMethod.MIN_MAX_ASYM)
     initializers = set(tensor.name for tensor in model.graph.initializer)
     rng = np.random.default_rng()
     for _ in range(dataset_size):
+        inputs = []
         for value_info in model.graph.input:
             if value_info.name in initializers:
                 continue
             # https://github.com/onnx/onnx/blob/master/docs/IR.md#static-tensor-shapes
             #
             # > The static shape is defined by 'TensorShapeProto':
             # >
@@ -73,26 +74,26 @@
                     shape.append(dimension.dim_value)
                 else:
                     raise RuntimeError(
                         f"The static shape of tensor '{value_info.name}' must be provided"
                     )
             np_dtype = onnx.mapping.TENSOR_TYPE_TO_NP_TYPE[value_info.type.tensor_type.elem_type]
             if np.issubdtype(np_dtype, np.floating):
-                inputs = rng.standard_normal(size=shape, dtype=np_dtype)
+                inputs.append(rng.standard_normal(size=shape, dtype=np_dtype))
             elif np.issubdtype(np_dtype, np.integer):
                 iinfo = np.iinfo(np_dtype)
-                inputs = rng.integers(
-                    iinfo.min, iinfo.max, size=shape, dtype=np_dtype, endpoint=True
+                inputs.append(
+                    rng.integers(iinfo.min, iinfo.max, size=shape, dtype=np_dtype, endpoint=True)
                 )
             else:
                 elem_type = onnx.TensorProto.DataType.Name(value_info.type.tensor_type.elem_type)
                 raise NotImplementedError(
                     f"tensor '{value_info.name}' is of {elem_type} but a model whose input tensor is of {elem_type} cannot be randomly calibrated yet"
                 )
-        calibrator.collect_data([[inputs]])
+        calibrator.collect_data([inputs])
     return calibrator.compute_range()
 
 
 def validate(model_path: Path, verbose: bool, target_npu: str):
     """
     Validate a given model
```

### Comparing `furiosa-litmus-0.9.0rc3/pyproject.toml` & `furiosa_litmus-0.9.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Custom backend from https://gitlab.com/ileixe/flit_ext to use setuptools-scm
 # Upstream flit does not support it. See https://github.com/pypa/flit/issues/257
 requires = ["flit_ext"]
 build-backend = "flit_ext:buildapi"
 
 [project]
 name = "furiosa-litmus"
-version = "0.9.0.rc3"
+version = "0.9.1"
 authors = [{ name = "FurioaAI, Inc.", email = "pkg@furiosa.ai" }]
 readme = "README.md"
 license = { text = "Apache License 2.0" }
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Intended Audience :: Developers",
@@ -23,15 +23,15 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 dynamic = ["description"]
 requires-python = "~=3.8"
 dependencies = [
     "furiosa-runtime == 0.9.*",
-    "furiosa-tools == 0.9.*", 
+    "furiosa-tools == 0.9.*",
     "furiosa-quantizer == 0.9.*"
 ]
 
 [project.optional-dependencies]
 test = []
 
 [project.urls]
```

### Comparing `furiosa-litmus-0.9.0rc3/tests/test_litmus.py` & `furiosa_litmus-0.9.1/tests/test_litmus.py`

 * *Files identical despite different names*

### Comparing `furiosa-litmus-0.9.0rc3/PKG-INFO` & `furiosa_litmus-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: furiosa-litmus
-Version: 0.9.0rc3
+Version: 0.9.1
 Summary: Furiosa Litmus, which readily checks whether a given model can be compiled with Furiosa SDK
 Author-email: "FurioaAI, Inc." <pkg@furiosa.ai>
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

