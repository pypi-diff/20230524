# Comparing `tmp/furiosa-quantizer-0.9.0rc3.tar.gz` & `tmp/furiosa_quantizer-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "furiosa-quantizer-0.9.0rc3.tar", last modified: Fri Apr 14 21:25:39 2023, max compression
+gzip compressed data, was "furiosa_quantizer-0.9.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `furiosa-quantizer-0.9.0rc3.tar` & `furiosa_quantizer-0.9.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1377 2023-04-14 21:20:22.936569 furiosa-quantizer-0.9.0rc3/.pylintrc
--rw-r--r--   0        0        0      388 2023-04-14 21:20:22.936569 furiosa-quantizer-0.9.0rc3/Makefile
--rw-r--r--   0        0        0       72 2023-04-14 21:20:22.936569 furiosa-quantizer-0.9.0rc3/README.md
--rw-r--r--   0        0        0     5470 2023-04-14 21:20:22.936569 furiosa-quantizer-0.9.0rc3/furiosa/quantizer/__init__.py
--rw-r--r--   0        0        0       17 2023-04-14 21:22:11.227588 furiosa-quantizer-0.9.0rc3/furiosa/quantizer/git_version.txt
--rw-r--r--   0        0        0     2393 2023-04-14 21:20:22.936569 furiosa-quantizer-0.9.0rc3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-14 21:20:22.936569 furiosa-quantizer-0.9.0rc3/tests/__init__.py
--rw-r--r--   0        0        0     1273 1970-01-01 00:00:00.000000 furiosa-quantizer-0.9.0rc3/PKG-INFO
+-rw-r--r--   0        0        0     1377 2023-05-24 05:34:31.468839 furiosa_quantizer-0.9.1/.pylintrc
+-rw-r--r--   0        0        0      388 2023-05-24 05:34:31.468839 furiosa_quantizer-0.9.1/Makefile
+-rw-r--r--   0        0        0       72 2023-05-24 05:34:31.472839 furiosa_quantizer-0.9.1/README.md
+-rw-r--r--   0        0        0     5709 2023-05-24 05:34:31.472839 furiosa_quantizer-0.9.1/furiosa/quantizer/__init__.py
+-rw-r--r--   0        0        0       14 2023-05-24 05:36:58.679852 furiosa_quantizer-0.9.1/furiosa/quantizer/git_version.txt
+-rw-r--r--   0        0        0     2389 2023-05-24 05:34:31.472839 furiosa_quantizer-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-24 05:34:31.472839 furiosa_quantizer-0.9.1/tests/__init__.py
+-rw-r--r--   0        0        0     1270 1970-01-01 00:00:00.000000 furiosa_quantizer-0.9.1/PKG-INFO
```

### Comparing `furiosa-quantizer-0.9.0rc3/.pylintrc` & `furiosa_quantizer-0.9.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `furiosa-quantizer-0.9.0rc3/furiosa/quantizer/__init__.py` & `furiosa_quantizer-0.9.1/furiosa/quantizer/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 import numpy as np
 import onnx
 
 import furiosa.common.utils
 
 __version__ = furiosa.common.utils.get_sdk_version(__name__)
 
+__full_version__ = f"Furiosa SDK Quantizer {__version__} (furiosa_quantizer_impl {furiosa_quantizer_impl.__version__} {furiosa_quantizer_impl.__git_short_hash__} {furiosa_quantizer_impl.__build_timestamp__})"  # pylint: disable=no-member
+
 __all__ = ["CalibrationMethod", "Calibrator", "Graph", "quantize"]
 
 
 CalibrationMethod = enum.IntEnum(
     "CalibrationMethod",
     # pylint: disable=no-member
     [
```

### Comparing `furiosa-quantizer-0.9.0rc3/pyproject.toml` & `furiosa_quantizer-0.9.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Custom backend from https://gitlab.com/ileixe/flit_ext to use setuptools-scm
 # Upstream flit does not support it. See https://github.com/pypa/flit/issues/257
 requires = ["flit_ext"]
 build-backend = "flit_ext:buildapi"
 
 [project]
 name = "furiosa-quantizer"
-version = "0.9.0.rc3"
+version = "0.9.1"
 authors = [{ name = "FurioaAI, Inc.", email = "pkg@furiosa.ai" }]
 readme = "README.md"
 license = { text = "Apache License 2.0" }
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Intended Audience :: Developers",
```

### Comparing `furiosa-quantizer-0.9.0rc3/PKG-INFO` & `furiosa_quantizer-0.9.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: furiosa-quantizer
-Version: 0.9.0rc3
+Version: 0.9.1
 Summary: A FuriosaAI qunatizer.
 Author-email: "FurioaAI, Inc." <pkg@furiosa.ai>
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

