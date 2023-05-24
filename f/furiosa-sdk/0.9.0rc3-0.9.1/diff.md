# Comparing `tmp/furiosa-sdk-0.9.0rc3.tar.gz` & `tmp/furiosa_sdk-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "furiosa-sdk-0.9.0rc3.tar", last modified: Fri Apr 14 21:26:11 2023, max compression
+gzip compressed data, was "furiosa_sdk-0.9.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `furiosa-sdk-0.9.0rc3.tar` & `furiosa_sdk-0.9.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      386 2023-04-14 21:20:22.940569 furiosa-sdk-0.9.0rc3/Makefile
--rw-r--r--   0        0        0     2542 2023-04-14 21:20:22.940569 furiosa-sdk-0.9.0rc3/README.md
--rw-r--r--   0        0        0     1107 2023-04-14 21:20:22.940569 furiosa-sdk-0.9.0rc3/docs/Makefile
--rw-r--r--   0        0        0     5330 2023-04-14 21:20:22.940569 furiosa-sdk-0.9.0rc3/docs/conf.py
--rw-r--r--   0        0        0      670 2023-04-14 21:20:22.940569 furiosa-sdk-0.9.0rc3/docs/furiosa.rst
--rw-r--r--   0        0        0      470 2023-04-14 21:20:22.944569 furiosa-sdk-0.9.0rc3/docs/index.rst
--rw-r--r--   0        0        0      795 2023-04-14 21:20:22.944569 furiosa-sdk-0.9.0rc3/docs/make.bat
--rw-r--r--   0        0        0       18 2023-04-14 21:20:22.944569 furiosa-sdk-0.9.0rc3/furiosa/sdk/__init__.py
--rw-r--r--   0        0        0     1833 2023-04-14 21:20:22.944569 furiosa-sdk-0.9.0rc3/pyproject.toml
--rw-r--r--   0        0        0     4820 1970-01-01 00:00:00.000000 furiosa-sdk-0.9.0rc3/PKG-INFO
+-rw-r--r--   0        0        0      386 2023-05-24 05:34:31.472839 furiosa_sdk-0.9.1/Makefile
+-rw-r--r--   0        0        0     2627 2023-05-24 05:34:31.472839 furiosa_sdk-0.9.1/README.md
+-rw-r--r--   0        0        0     1107 2023-05-24 05:34:31.472839 furiosa_sdk-0.9.1/docs/Makefile
+-rw-r--r--   0        0        0     5330 2023-05-24 05:34:31.472839 furiosa_sdk-0.9.1/docs/conf.py
+-rw-r--r--   0        0        0      670 2023-05-24 05:34:31.476839 furiosa_sdk-0.9.1/docs/furiosa.rst
+-rw-r--r--   0        0        0      470 2023-05-24 05:34:31.476839 furiosa_sdk-0.9.1/docs/index.rst
+-rw-r--r--   0        0        0      795 2023-05-24 05:34:31.476839 furiosa_sdk-0.9.1/docs/make.bat
+-rw-r--r--   0        0        0       18 2023-05-24 05:34:31.476839 furiosa_sdk-0.9.1/furiosa/sdk/__init__.py
+-rw-r--r--   0        0        0     1829 2023-05-24 05:34:31.476839 furiosa_sdk-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     4902 1970-01-01 00:00:00.000000 furiosa_sdk-0.9.1/PKG-INFO
```

### Comparing `furiosa-sdk-0.9.0rc3/README.md` & `furiosa_sdk-0.9.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,16 @@
 * litmus: Command line tool to check if a model is compatible with furiosa-sdk
 * models: Library which provides pretained models for Furiosa NPU
 * quantizer: Library which quantizes and optimizes DNN models
 * server: Serving framework enabling a DNN model to provide HTTP/GRPC endpoints
 * serving: FastAPI-based Serving Library
 
 ## Releases
-* [Furiosa SDK 0.8.2](https://github.com/furiosa-ai/furiosa-sdk/releases/tag/0.8.2) (Latest)
+* [Furiosa SDK 0.9.0](https://github.com/furiosa-ai/furiosa-sdk/releases/tag/v0.9.0) (Latest)
+* [Furiosa SDK 0.8.2](https://github.com/furiosa-ai/furiosa-sdk/releases/tag/0.8.2)
 * [Furiosa SDK 0.7.0](https://github.com/furiosa-ai/furiosa-sdk/releases/tag/v0.7.0)
 * [Furiosa SDK 0.6.3](https://github.com/furiosa-ai/furiosa-sdk/releases/tag/v0.6.3)
 * [Furiosa SDK 0.6.0](https://github.com/furiosa-ai/furiosa-sdk/releases/tag/v0.6.0)
 * [Furiosa SDK 0.5.2](https://github.com/furiosa-ai/furiosa-sdk/releases/tag/v0.5.2)
 * [Furiosa SDK 0.5.1](https://github.com/furiosa-ai/furiosa-sdk/releases/tag/v0.5.1)
 * [Furiosa SDK 0.5.0](https://github.com/furiosa-ai/furiosa-sdk/releases/tag/v0.5.0)
 * [Furiosa SDK 0.4.0](https://github.com/furiosa-ai/furiosa-sdk/releases/tag/v0.4.0)
```

### Comparing `furiosa-sdk-0.9.0rc3/docs/Makefile` & `furiosa_sdk-0.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `furiosa-sdk-0.9.0rc3/docs/conf.py` & `furiosa_sdk-0.9.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `furiosa-sdk-0.9.0rc3/docs/furiosa.rst` & `furiosa_sdk-0.9.1/docs/furiosa.rst`

 * *Files identical despite different names*

### Comparing `furiosa-sdk-0.9.0rc3/docs/make.bat` & `furiosa_sdk-0.9.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `furiosa-sdk-0.9.0rc3/pyproject.toml` & `furiosa_sdk-0.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "furiosa-sdk"
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

### Comparing `furiosa-sdk-0.9.0rc3/PKG-INFO` & `furiosa_sdk-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: furiosa-sdk
-Version: 0.9.0rc3
+Version: 0.9.1
 Summary: Furiosa SDK
 Author-email: "FurioaAI, Inc." <pkg@furiosa.ai>
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -75,15 +75,16 @@
 * litmus: Command line tool to check if a model is compatible with furiosa-sdk
 * models: Library which provides pretained models for Furiosa NPU
 * quantizer: Library which quantizes and optimizes DNN models
 * server: Serving framework enabling a DNN model to provide HTTP/GRPC endpoints
 * serving: FastAPI-based Serving Library
 
 ## Releases
-* [Furiosa SDK 0.8.2](https://github.com/furiosa-ai/furiosa-sdk/releases/tag/0.8.2) (Latest)
+* [Furiosa SDK 0.9.0](https://github.com/furiosa-ai/furiosa-sdk/releases/tag/v0.9.0) (Latest)
+* [Furiosa SDK 0.8.2](https://github.com/furiosa-ai/furiosa-sdk/releases/tag/0.8.2)
 * [Furiosa SDK 0.7.0](https://github.com/furiosa-ai/furiosa-sdk/releases/tag/v0.7.0)
 * [Furiosa SDK 0.6.3](https://github.com/furiosa-ai/furiosa-sdk/releases/tag/v0.6.3)
 * [Furiosa SDK 0.6.0](https://github.com/furiosa-ai/furiosa-sdk/releases/tag/v0.6.0)
 * [Furiosa SDK 0.5.2](https://github.com/furiosa-ai/furiosa-sdk/releases/tag/v0.5.2)
 * [Furiosa SDK 0.5.1](https://github.com/furiosa-ai/furiosa-sdk/releases/tag/v0.5.1)
 * [Furiosa SDK 0.5.0](https://github.com/furiosa-ai/furiosa-sdk/releases/tag/v0.5.0)
 * [Furiosa SDK 0.4.0](https://github.com/furiosa-ai/furiosa-sdk/releases/tag/v0.4.0)
```

