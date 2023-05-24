# Comparing `tmp/furiosa-tools-0.9.0rc3.tar.gz` & `tmp/furiosa_tools-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "furiosa-tools-0.9.0rc3.tar", last modified: Fri Apr 14 21:25:04 2023, max compression
+gzip compressed data, was "furiosa_tools-0.9.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `furiosa-tools-0.9.0rc3.tar` & `furiosa_tools-0.9.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      291 2023-04-14 21:20:23.064568 furiosa-tools-0.9.0rc3/Makefile
--rw-r--r--   0        0        0      176 2023-04-14 21:20:23.064568 furiosa-tools-0.9.0rc3/README.md
--rw-r--r--   0        0        0      112 2023-04-14 21:20:23.064568 furiosa-tools-0.9.0rc3/furiosa/tools/__init__.py
--rw-r--r--   0        0        0       39 2023-04-14 21:20:23.064568 furiosa-tools-0.9.0rc3/furiosa/tools/compiler/__init__.py
--rw-r--r--   0        0        0       84 2023-04-14 21:20:23.064568 furiosa-tools-0.9.0rc3/furiosa/tools/compiler/api/__init__.py
--rw-r--r--   0        0        0     4170 2023-04-14 21:20:23.064568 furiosa-tools-0.9.0rc3/furiosa/tools/compiler/api/errors.py
--rw-r--r--   0        0        0     8458 2023-04-14 21:20:23.064568 furiosa-tools-0.9.0rc3/furiosa/tools/compiler/api/v1.py
--rw-r--r--   0        0        0     7260 2023-04-14 21:20:23.064568 furiosa-tools-0.9.0rc3/furiosa/tools/compiler/main.py
--rw-r--r--   0        0        0       17 2023-04-14 21:21:34.271922 furiosa-tools-0.9.0rc3/furiosa/tools/git_version.txt
--rw-r--r--   0        0        0        0 2023-04-14 21:20:23.064568 furiosa-tools-0.9.0rc3/furiosa/tools/py.typed
--rw-r--r--   0        0        0     2345 2023-04-14 21:20:23.064568 furiosa-tools-0.9.0rc3/pyproject.toml
--rw-r--r--   0        0        0      115 2023-04-14 21:20:23.064568 furiosa-tools-0.9.0rc3/tests/__init__.py
--rw-r--r--   0        0        0     6164 2023-04-14 21:20:23.064568 furiosa-tools-0.9.0rc3/tests/tests_compile.py
--rw-r--r--   0        0        0     1250 1970-01-01 00:00:00.000000 furiosa-tools-0.9.0rc3/PKG-INFO
+-rw-r--r--   0        0        0      291 2023-05-24 05:34:31.612838 furiosa_tools-0.9.1/Makefile
+-rw-r--r--   0        0        0      176 2023-05-24 05:34:31.612838 furiosa_tools-0.9.1/README.md
+-rw-r--r--   0        0        0      112 2023-05-24 05:34:31.612838 furiosa_tools-0.9.1/furiosa/tools/__init__.py
+-rw-r--r--   0        0        0       39 2023-05-24 05:34:31.612838 furiosa_tools-0.9.1/furiosa/tools/compiler/__init__.py
+-rw-r--r--   0        0        0       84 2023-05-24 05:34:31.612838 furiosa_tools-0.9.1/furiosa/tools/compiler/api/__init__.py
+-rw-r--r--   0        0        0     4170 2023-05-24 05:34:31.612838 furiosa_tools-0.9.1/furiosa/tools/compiler/api/errors.py
+-rw-r--r--   0        0        0     8458 2023-05-24 05:34:31.612838 furiosa_tools-0.9.1/furiosa/tools/compiler/api/v1.py
+-rw-r--r--   0        0        0     7260 2023-05-24 05:34:31.612838 furiosa_tools-0.9.1/furiosa/tools/compiler/main.py
+-rw-r--r--   0        0        0       14 2023-05-24 05:36:02.756227 furiosa_tools-0.9.1/furiosa/tools/git_version.txt
+-rw-r--r--   0        0        0        0 2023-05-24 05:34:31.612838 furiosa_tools-0.9.1/furiosa/tools/py.typed
+-rw-r--r--   0        0        0     2341 2023-05-24 05:34:31.612838 furiosa_tools-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      115 2023-05-24 05:34:31.612838 furiosa_tools-0.9.1/tests/__init__.py
+-rw-r--r--   0        0        0     6164 2023-05-24 05:34:31.612838 furiosa_tools-0.9.1/tests/tests_compile.py
+-rw-r--r--   0        0        0     1247 1970-01-01 00:00:00.000000 furiosa_tools-0.9.1/PKG-INFO
```

### Comparing `furiosa-tools-0.9.0rc3/furiosa/tools/compiler/api/errors.py` & `furiosa_tools-0.9.1/furiosa/tools/compiler/api/errors.py`

 * *Files identical despite different names*

### Comparing `furiosa-tools-0.9.0rc3/furiosa/tools/compiler/api/v1.py` & `furiosa_tools-0.9.1/furiosa/tools/compiler/api/v1.py`

 * *Files identical despite different names*

### Comparing `furiosa-tools-0.9.0rc3/furiosa/tools/compiler/main.py` & `furiosa_tools-0.9.1/furiosa/tools/compiler/main.py`

 * *Files identical despite different names*

### Comparing `furiosa-tools-0.9.0rc3/pyproject.toml` & `furiosa_tools-0.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Custom backend from https://gitlab.com/ileixe/flit_ext to use setuptools-scm
 # Upstream flit does not support it. See https://github.com/pypa/flit/issues/257
 requires = ["flit_ext"]
 build-backend = "flit_ext:buildapi"
 
 [project]
 name = "furiosa-tools"
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

### Comparing `furiosa-tools-0.9.0rc3/tests/tests_compile.py` & `furiosa_tools-0.9.1/tests/tests_compile.py`

 * *Files identical despite different names*

### Comparing `furiosa-tools-0.9.0rc3/PKG-INFO` & `furiosa_tools-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: furiosa-tools
-Version: 0.9.0rc3
+Version: 0.9.1
 Summary: FuriosaAI tools
 Author-email: "FurioaAI, Inc." <pkg@furiosa.ai>
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

