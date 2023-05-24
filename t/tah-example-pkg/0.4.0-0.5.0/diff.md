# Comparing `tmp/tah_example_pkg-0.4.0.tar.gz` & `tmp/tah_example_pkg-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tah_example_pkg-0.4.0.tar", max compression
+gzip compressed data, was "tah_example_pkg-0.5.0.tar", max compression
```

## Comparing `tah_example_pkg-0.4.0.tar` & `tah_example_pkg-0.5.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      985 2023-05-11 12:40:46.475898 tah_example_pkg-0.4.0/README.md
--rw-r--r--   0        0        0      567 2023-05-23 20:03:09.809571 tah_example_pkg-0.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-23 20:02:32.889198 tah_example_pkg-0.4.0/src/tah_example_pkg/__init__.py
--rwxr-xr-x   0        0        0     1907 2023-05-15 14:40:02.436185 tah_example_pkg-0.4.0/src/tah_example_pkg/evaluate.py
--rw-r--r--   0        0        0     3994 2023-05-23 19:28:36.280423 tah_example_pkg-0.4.0/src/tah_example_pkg/helpers.py
--rw-r--r--   0        0        0     1630 2023-05-23 19:29:35.621312 tah_example_pkg-0.4.0/src/tah_example_pkg/model_class.py
--rwxr-xr-x   0        0        0     4709 2023-05-20 12:10:53.785322 tah_example_pkg-0.4.0/src/tah_example_pkg/onnx_base.py
--rwxr-xr-x   0        0        0     1797 2023-05-23 18:46:58.183819 tah_example_pkg-0.4.0/src/tah_example_pkg/predict.py
--rw-r--r--   0        0        0     1586 1970-01-01 00:00:00.000000 tah_example_pkg-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      985 2023-05-11 12:40:46.475898 tah_example_pkg-0.5.0/README.md
+-rw-r--r--   0        0        0      623 2023-05-24 13:41:55.458207 tah_example_pkg-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-23 20:02:32.889198 tah_example_pkg-0.5.0/src/tah_example_pkg/__init__.py
+-rwxr-xr-x   0        0        0     1907 2023-05-15 14:40:02.436185 tah_example_pkg-0.5.0/src/tah_example_pkg/evaluate.py
+-rw-r--r--   0        0        0     3994 2023-05-23 19:28:36.280423 tah_example_pkg-0.5.0/src/tah_example_pkg/helpers.py
+-rw-r--r--   0        0        0     3273 2023-05-24 13:41:11.081546 tah_example_pkg-0.5.0/src/tah_example_pkg/model_class.py
+-rwxr-xr-x   0        0        0     4709 2023-05-20 12:10:53.785322 tah_example_pkg-0.5.0/src/tah_example_pkg/onnx_base.py
+-rwxr-xr-x   0        0        0     1797 2023-05-23 18:46:58.183819 tah_example_pkg-0.5.0/src/tah_example_pkg/predict.py
+-rw-r--r--   0        0        0     1638 1970-01-01 00:00:00.000000 tah_example_pkg-0.5.0/PKG-INFO
```

### Comparing `tah_example_pkg-0.4.0/README.md` & `tah_example_pkg-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `tah_example_pkg-0.4.0/src/tah_example_pkg/evaluate.py` & `tah_example_pkg-0.5.0/src/tah_example_pkg/evaluate.py`

 * *Files identical despite different names*

### Comparing `tah_example_pkg-0.4.0/src/tah_example_pkg/helpers.py` & `tah_example_pkg-0.5.0/src/tah_example_pkg/helpers.py`

 * *Files identical despite different names*

### Comparing `tah_example_pkg-0.4.0/src/tah_example_pkg/onnx_base.py` & `tah_example_pkg-0.5.0/src/tah_example_pkg/onnx_base.py`

 * *Files identical despite different names*

### Comparing `tah_example_pkg-0.4.0/src/tah_example_pkg/predict.py` & `tah_example_pkg-0.5.0/src/tah_example_pkg/predict.py`

 * *Files identical despite different names*

### Comparing `tah_example_pkg-0.4.0/PKG-INFO` & `tah_example_pkg-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: tah-example-pkg
-Version: 0.4.0
+Version: 0.5.0
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: filetype (>=1.2.0,<2.0.0)
 Requires-Dist: onnxruntime (>=1.14.1,<2.0.0)
 Requires-Dist: opencv-python (>=4.7.0.72,<5.0.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
+Requires-Dist: tritonclient[grpc] (>=2.33.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Introduction 
 TODO: Give a short introduction of your project. Let this section explain the objectives or the motivation behind this project. 
 
 # Getting Started
 TODO: Guide users through getting your code up and running on their own system. In this section you can talk about:
```

