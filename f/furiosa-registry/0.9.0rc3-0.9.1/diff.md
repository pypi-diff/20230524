# Comparing `tmp/furiosa-registry-0.9.0rc3.tar.gz` & `tmp/furiosa_registry-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "furiosa-registry-0.9.0rc3.tar", last modified: Fri Apr 14 21:25:12 2023, max compression
+gzip compressed data, was "furiosa_registry-0.9.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `furiosa-registry-0.9.0rc3.tar` & `furiosa_registry-0.9.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      353 2023-04-14 21:20:22.936569 furiosa-registry-0.9.0rc3/Makefile
--rw-r--r--   0        0        0     1623 2023-04-14 21:20:22.936569 furiosa-registry-0.9.0rc3/README.md
--rw-r--r--   0        0        0      223 2023-04-14 21:20:22.936569 furiosa-registry-0.9.0rc3/furiosa/registry/__init__.py
--rw-r--r--   0        0        0     2600 2023-04-14 21:20:22.940569 furiosa-registry-0.9.0rc3/furiosa/registry/client/__init__.py
--rw-r--r--   0        0        0     2986 2023-04-14 21:20:22.940569 furiosa-registry-0.9.0rc3/furiosa/registry/client/transport/__init__.py
--rw-r--r--   0        0        0     2059 2023-04-14 21:20:22.940569 furiosa-registry-0.9.0rc3/furiosa/registry/client/transport/base.py
--rw-r--r--   0        0        0     1543 2023-04-14 21:20:22.940569 furiosa-registry-0.9.0rc3/furiosa/registry/client/transport/file.py
--rw-r--r--   0        0        0     2720 2023-04-14 21:20:22.940569 furiosa-registry-0.9.0rc3/furiosa/registry/client/transport/github.py
--rw-r--r--   0        0        0     1569 2023-04-14 21:20:22.940569 furiosa-registry-0.9.0rc3/furiosa/registry/client/transport/http.py
--rw-r--r--   0        0        0     1293 2023-04-14 21:20:22.940569 furiosa-registry-0.9.0rc3/furiosa/registry/client/transport/s3.py
--rw-r--r--   0        0        0      535 2023-04-14 21:20:22.940569 furiosa-registry-0.9.0rc3/furiosa/registry/errors.py
--rw-r--r--   0        0        0       17 2023-04-14 21:21:40.667864 furiosa-registry-0.9.0rc3/furiosa/registry/git_version.txt
--rw-r--r--   0        0        0     2464 2023-04-14 21:20:22.940569 furiosa-registry-0.9.0rc3/furiosa/registry/model.py
--rw-r--r--   0        0        0        0 2023-04-14 21:20:22.940569 furiosa-registry-0.9.0rc3/furiosa/registry/py.typed
--rw-r--r--   0        0        0     1926 2023-04-14 21:20:22.940569 furiosa-registry-0.9.0rc3/furiosa/registry/utils.py
--rw-r--r--   0        0        0     3158 2023-04-14 21:20:22.940569 furiosa-registry-0.9.0rc3/model_schema.json
--rw-r--r--   0        0        0     2571 2023-04-14 21:20:22.940569 furiosa-registry-0.9.0rc3/pyproject.toml
--rw-r--r--   0        0        0      454 2023-04-14 21:20:22.940569 furiosa-registry-0.9.0rc3/tests/unit/conftest.py
--rw-r--r--   0        0        0      883 2023-04-14 21:20:22.940569 furiosa-registry-0.9.0rc3/tests/unit/fixtures/artifacts.py
--rw-r--r--   0        0        0    16154 2023-04-14 21:20:22.940569 furiosa-registry-0.9.0rc3/tests/unit/fixtures/models/MNISTnet_uint8_quant_without_softmax.dfg
--rw-r--r--   0        0        0   172884 2023-04-14 21:20:22.940569 furiosa-registry-0.9.0rc3/tests/unit/fixtures/models/MNISTnet_uint8_quant_without_softmax.enf
--rw-r--r--   0        0        0    18136 2023-04-14 21:20:22.940569 furiosa-registry-0.9.0rc3/tests/unit/fixtures/models/MNISTnet_uint8_quant_without_softmax.tflite
--rw-r--r--   0        0        0      927 2023-04-14 21:20:22.940569 furiosa-registry-0.9.0rc3/tests/unit/test_file_transport.py
--rw-r--r--   0        0        0     1623 2023-04-14 21:20:22.940569 furiosa-registry-0.9.0rc3/tests/unit/test_http_transport.py
--rw-r--r--   0        0        0     1182 2023-04-14 21:20:22.940569 furiosa-registry-0.9.0rc3/tests/unit/test_s3_transport.py
--rw-r--r--   0        0        0     3314 1970-01-01 00:00:00.000000 furiosa-registry-0.9.0rc3/PKG-INFO
+-rw-r--r--   0        0        0      353 2023-05-24 05:34:31.472839 furiosa_registry-0.9.1/Makefile
+-rw-r--r--   0        0        0     1623 2023-05-24 05:34:31.472839 furiosa_registry-0.9.1/README.md
+-rw-r--r--   0        0        0      223 2023-05-24 05:34:31.472839 furiosa_registry-0.9.1/furiosa/registry/__init__.py
+-rw-r--r--   0        0        0     2600 2023-05-24 05:34:31.472839 furiosa_registry-0.9.1/furiosa/registry/client/__init__.py
+-rw-r--r--   0        0        0     2986 2023-05-24 05:34:31.472839 furiosa_registry-0.9.1/furiosa/registry/client/transport/__init__.py
+-rw-r--r--   0        0        0     2059 2023-05-24 05:34:31.472839 furiosa_registry-0.9.1/furiosa/registry/client/transport/base.py
+-rw-r--r--   0        0        0     1543 2023-05-24 05:34:31.472839 furiosa_registry-0.9.1/furiosa/registry/client/transport/file.py
+-rw-r--r--   0        0        0     2720 2023-05-24 05:34:31.472839 furiosa_registry-0.9.1/furiosa/registry/client/transport/github.py
+-rw-r--r--   0        0        0     1569 2023-05-24 05:34:31.472839 furiosa_registry-0.9.1/furiosa/registry/client/transport/http.py
+-rw-r--r--   0        0        0     1293 2023-05-24 05:34:31.472839 furiosa_registry-0.9.1/furiosa/registry/client/transport/s3.py
+-rw-r--r--   0        0        0      535 2023-05-24 05:34:31.472839 furiosa_registry-0.9.1/furiosa/registry/errors.py
+-rw-r--r--   0        0        0       14 2023-05-24 05:36:12.260163 furiosa_registry-0.9.1/furiosa/registry/git_version.txt
+-rw-r--r--   0        0        0     2464 2023-05-24 05:34:31.472839 furiosa_registry-0.9.1/furiosa/registry/model.py
+-rw-r--r--   0        0        0        0 2023-05-24 05:34:31.472839 furiosa_registry-0.9.1/furiosa/registry/py.typed
+-rw-r--r--   0        0        0     1926 2023-05-24 05:34:31.472839 furiosa_registry-0.9.1/furiosa/registry/utils.py
+-rw-r--r--   0        0        0     3158 2023-05-24 05:34:31.472839 furiosa_registry-0.9.1/model_schema.json
+-rw-r--r--   0        0        0     2567 2023-05-24 05:34:31.472839 furiosa_registry-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      454 2023-05-24 05:34:31.472839 furiosa_registry-0.9.1/tests/unit/conftest.py
+-rw-r--r--   0        0        0      883 2023-05-24 05:34:31.472839 furiosa_registry-0.9.1/tests/unit/fixtures/artifacts.py
+-rw-r--r--   0        0        0    16154 2023-05-24 05:34:31.472839 furiosa_registry-0.9.1/tests/unit/fixtures/models/MNISTnet_uint8_quant_without_softmax.dfg
+-rw-r--r--   0        0        0   172884 2023-05-24 05:34:31.472839 furiosa_registry-0.9.1/tests/unit/fixtures/models/MNISTnet_uint8_quant_without_softmax.enf
+-rw-r--r--   0        0        0    18136 2023-05-24 05:34:31.472839 furiosa_registry-0.9.1/tests/unit/fixtures/models/MNISTnet_uint8_quant_without_softmax.tflite
+-rw-r--r--   0        0        0      927 2023-05-24 05:34:31.472839 furiosa_registry-0.9.1/tests/unit/test_file_transport.py
+-rw-r--r--   0        0        0     1623 2023-05-24 05:34:31.472839 furiosa_registry-0.9.1/tests/unit/test_http_transport.py
+-rw-r--r--   0        0        0     1182 2023-05-24 05:34:31.472839 furiosa_registry-0.9.1/tests/unit/test_s3_transport.py
+-rw-r--r--   0        0        0     3311 1970-01-01 00:00:00.000000 furiosa_registry-0.9.1/PKG-INFO
```

### Comparing `furiosa-registry-0.9.0rc3/README.md` & `furiosa_registry-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `furiosa-registry-0.9.0rc3/furiosa/registry/client/__init__.py` & `furiosa_registry-0.9.1/furiosa/registry/client/__init__.py`

 * *Files identical despite different names*

### Comparing `furiosa-registry-0.9.0rc3/furiosa/registry/client/transport/__init__.py` & `furiosa_registry-0.9.1/furiosa/registry/client/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `furiosa-registry-0.9.0rc3/furiosa/registry/client/transport/base.py` & `furiosa_registry-0.9.1/furiosa/registry/client/transport/base.py`

 * *Files identical despite different names*

### Comparing `furiosa-registry-0.9.0rc3/furiosa/registry/client/transport/file.py` & `furiosa_registry-0.9.1/furiosa/registry/client/transport/file.py`

 * *Files identical despite different names*

### Comparing `furiosa-registry-0.9.0rc3/furiosa/registry/client/transport/github.py` & `furiosa_registry-0.9.1/furiosa/registry/client/transport/github.py`

 * *Files identical despite different names*

### Comparing `furiosa-registry-0.9.0rc3/furiosa/registry/client/transport/http.py` & `furiosa_registry-0.9.1/furiosa/registry/client/transport/http.py`

 * *Files identical despite different names*

### Comparing `furiosa-registry-0.9.0rc3/furiosa/registry/client/transport/s3.py` & `furiosa_registry-0.9.1/furiosa/registry/client/transport/s3.py`

 * *Files identical despite different names*

### Comparing `furiosa-registry-0.9.0rc3/furiosa/registry/errors.py` & `furiosa_registry-0.9.1/furiosa/registry/errors.py`

 * *Files identical despite different names*

### Comparing `furiosa-registry-0.9.0rc3/furiosa/registry/model.py` & `furiosa_registry-0.9.1/furiosa/registry/model.py`

 * *Files identical despite different names*

### Comparing `furiosa-registry-0.9.0rc3/furiosa/registry/utils.py` & `furiosa_registry-0.9.1/furiosa/registry/utils.py`

 * *Files identical despite different names*

### Comparing `furiosa-registry-0.9.0rc3/model_schema.json` & `furiosa_registry-0.9.1/model_schema.json`

 * *Files identical despite different names*

### Comparing `furiosa-registry-0.9.0rc3/pyproject.toml` & `furiosa_registry-0.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Custom backend from https://gitlab.com/ileixe/flit_ext to use setuptools-scm
 # Upstream flit does not support it. See https://github.com/pypa/flit/issues/257
 requires = ["flit_ext"]
 build-backend = "flit_ext:buildapi"
 
 [project]
 name = "furiosa-registry"
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

### Comparing `furiosa-registry-0.9.0rc3/tests/unit/fixtures/artifacts.py` & `furiosa_registry-0.9.1/tests/unit/fixtures/artifacts.py`

 * *Files identical despite different names*

### Comparing `furiosa-registry-0.9.0rc3/tests/unit/fixtures/models/MNISTnet_uint8_quant_without_softmax.dfg` & `furiosa_registry-0.9.1/tests/unit/fixtures/models/MNISTnet_uint8_quant_without_softmax.dfg`

 * *Files identical despite different names*

### Comparing `furiosa-registry-0.9.0rc3/tests/unit/fixtures/models/MNISTnet_uint8_quant_without_softmax.enf` & `furiosa_registry-0.9.1/tests/unit/fixtures/models/MNISTnet_uint8_quant_without_softmax.enf`

 * *Files identical despite different names*

### Comparing `furiosa-registry-0.9.0rc3/tests/unit/fixtures/models/MNISTnet_uint8_quant_without_softmax.tflite` & `furiosa_registry-0.9.1/tests/unit/fixtures/models/MNISTnet_uint8_quant_without_softmax.tflite`

 * *Files identical despite different names*

### Comparing `furiosa-registry-0.9.0rc3/tests/unit/test_file_transport.py` & `furiosa_registry-0.9.1/tests/unit/test_file_transport.py`

 * *Files identical despite different names*

### Comparing `furiosa-registry-0.9.0rc3/tests/unit/test_http_transport.py` & `furiosa_registry-0.9.1/tests/unit/test_http_transport.py`

 * *Files identical despite different names*

### Comparing `furiosa-registry-0.9.0rc3/tests/unit/test_s3_transport.py` & `furiosa_registry-0.9.1/tests/unit/test_s3_transport.py`

 * *Files identical despite different names*

### Comparing `furiosa-registry-0.9.0rc3/PKG-INFO` & `furiosa_registry-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: furiosa-registry
-Version: 0.9.0rc3
+Version: 0.9.1
 Summary: FuriosaAI model registry
 Author-email: "FurioaAI, Inc." <pkg@furiosa.ai>
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

