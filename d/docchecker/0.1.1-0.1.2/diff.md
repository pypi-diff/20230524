# Comparing `tmp/docchecker-0.1.1.tar.gz` & `tmp/docchecker-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docchecker-0.1.1.tar", last modified: Mon May 22 05:05:16 2023, max compression
+gzip compressed data, was "docchecker-0.1.2.tar", last modified: Wed May 24 21:21:26 2023, max compression
```

## Comparing `docchecker-0.1.1.tar` & `docchecker-0.1.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 anhdtv7   (1001) anhdtv7   (1001)        0 2023-05-22 05:05:16.190297 docchecker-0.1.1/
--rw-rw-r--   0 anhdtv7   (1001) anhdtv7   (1001)     4766 2023-05-22 05:05:16.190297 docchecker-0.1.1/PKG-INFO
--rw-rw-r--   0 anhdtv7   (1001) anhdtv7   (1001)     4223 2023-05-22 02:55:56.000000 docchecker-0.1.1/README.md
--rw-rw-r--   0 anhdtv7   (1001) anhdtv7   (1001)      635 2023-05-22 05:04:27.000000 docchecker-0.1.1/pyproject.toml
--rw-rw-r--   0 anhdtv7   (1001) anhdtv7   (1001)       38 2023-05-22 05:05:16.190297 docchecker-0.1.1/setup.cfg
-drwxrwxr-x   0 anhdtv7   (1001) anhdtv7   (1001)        0 2023-05-22 05:05:16.186298 docchecker-0.1.1/src/
-drwxrwxr-x   0 anhdtv7   (1001) anhdtv7   (1001)        0 2023-05-22 05:05:16.186298 docchecker-0.1.1/src/DocChecker/
--rw-rw-r--   0 anhdtv7   (1001) anhdtv7   (1001)     4297 2023-05-22 05:03:21.000000 docchecker-0.1.1/src/DocChecker/DocCheckerNet.py
--rw-rw-r--   0 anhdtv7   (1001) anhdtv7   (1001)      106 2023-05-19 04:44:42.000000 docchecker-0.1.1/src/DocChecker/__init__.py
--rw-rw-r--   0 anhdtv7   (1001) anhdtv7   (1001)    19433 2023-05-08 12:43:08.000000 docchecker-0.1.1/src/DocChecker/model.py
-drwxrwxr-x   0 anhdtv7   (1001) anhdtv7   (1001)        0 2023-05-22 05:05:16.186298 docchecker-0.1.1/src/DocChecker/tree-sitter/
-drwxrwxr-x   0 anhdtv7   (1001) anhdtv7   (1001)        0 2023-05-22 05:05:16.186298 docchecker-0.1.1/src/DocChecker/tree-sitter/tree-sitter-python/
-drwxrwxr-x   0 anhdtv7   (1001) anhdtv7   (1001)        0 2023-05-22 05:05:16.186298 docchecker-0.1.1/src/DocChecker/tree-sitter/tree-sitter-python/examples/
--rw-rw-r--   0 anhdtv7   (1001) anhdtv7   (1001)       38 2023-05-17 05:00:42.000000 docchecker-0.1.1/src/DocChecker/tree-sitter/tree-sitter-python/examples/compound-statement-without-trailing-newline.py
--rw-rw-r--   0 anhdtv7   (1001) anhdtv7   (1001)       51 2023-05-17 05:00:42.000000 docchecker-0.1.1/src/DocChecker/tree-sitter/tree-sitter-python/examples/crlf-line-endings.py
--rw-rw-r--   0 anhdtv7   (1001) anhdtv7   (1001)       74 2023-05-17 05:00:42.000000 docchecker-0.1.1/src/DocChecker/tree-sitter/tree-sitter-python/examples/mixed-spaces-tabs.py
--rw-rw-r--   0 anhdtv7   (1001) anhdtv7   (1001)       73 2023-05-17 05:00:42.000000 docchecker-0.1.1/src/DocChecker/tree-sitter/tree-sitter-python/examples/multiple-newlines.py
--rw-rw-r--   0 anhdtv7   (1001) anhdtv7   (1001)    31929 2023-05-17 05:00:42.000000 docchecker-0.1.1/src/DocChecker/tree-sitter/tree-sitter-python/examples/python2-grammar-crlf.py
--rw-rw-r--   0 anhdtv7   (1001) anhdtv7   (1001)    30981 2023-05-17 05:00:42.000000 docchecker-0.1.1/src/DocChecker/tree-sitter/tree-sitter-python/examples/python2-grammar.py
--rw-rw-r--   0 anhdtv7   (1001) anhdtv7   (1001)    31722 2023-05-17 05:00:42.000000 docchecker-0.1.1/src/DocChecker/tree-sitter/tree-sitter-python/examples/python3-grammar-crlf.py
--rw-rw-r--   0 anhdtv7   (1001) anhdtv7   (1001)    30784 2023-05-17 05:00:42.000000 docchecker-0.1.1/src/DocChecker/tree-sitter/tree-sitter-python/examples/python3-grammar.py
--rw-rw-r--   0 anhdtv7   (1001) anhdtv7   (1001)    50403 2023-05-17 05:00:42.000000 docchecker-0.1.1/src/DocChecker/tree-sitter/tree-sitter-python/examples/python3.8_grammar.py
--rw-rw-r--   0 anhdtv7   (1001) anhdtv7   (1001)       16 2023-05-17 05:00:42.000000 docchecker-0.1.1/src/DocChecker/tree-sitter/tree-sitter-python/examples/simple-statements-without-trailing-newline.py
--rw-rw-r--   0 anhdtv7   (1001) anhdtv7   (1001)     1236 2023-05-17 05:00:42.000000 docchecker-0.1.1/src/DocChecker/tree-sitter/tree-sitter-python/examples/tabs.py
--rw-rw-r--   0 anhdtv7   (1001) anhdtv7   (1001)       58 2023-05-17 05:00:42.000000 docchecker-0.1.1/src/DocChecker/tree-sitter/tree-sitter-python/examples/trailing-whitespace.py
-drwxrwxr-x   0 anhdtv7   (1001) anhdtv7   (1001)        0 2023-05-22 05:05:16.186298 docchecker-0.1.1/src/DocChecker/tree-sitter/tree-sitter-python/test/
-drwxrwxr-x   0 anhdtv7   (1001) anhdtv7   (1001)        0 2023-05-22 05:05:16.186298 docchecker-0.1.1/src/DocChecker/tree-sitter/tree-sitter-python/test/highlight/
--rw-rw-r--   0 anhdtv7   (1001) anhdtv7   (1001)      352 2023-05-17 05:00:42.000000 docchecker-0.1.1/src/DocChecker/tree-sitter/tree-sitter-python/test/highlight/keywords.py
--rw-rw-r--   0 anhdtv7   (1001) anhdtv7   (1001)       99 2023-05-17 05:00:42.000000 docchecker-0.1.1/src/DocChecker/tree-sitter/tree-sitter-python/test/highlight/parameters.py
--rw-rw-r--   0 anhdtv7   (1001) anhdtv7   (1001)     1297 2023-05-17 05:00:42.000000 docchecker-0.1.1/src/DocChecker/tree-sitter/tree-sitter-python/test/highlight/pattern_matching.py
--rw-rw-r--   0 anhdtv7   (1001) anhdtv7   (1001)     5135 2023-05-22 05:03:17.000000 docchecker-0.1.1/src/DocChecker/utils.py
-drwxrwxr-x   0 anhdtv7   (1001) anhdtv7   (1001)        0 2023-05-22 05:05:16.190297 docchecker-0.1.1/src/docchecker.egg-info/
--rw-rw-r--   0 anhdtv7   (1001) anhdtv7   (1001)     4766 2023-05-22 05:05:16.000000 docchecker-0.1.1/src/docchecker.egg-info/PKG-INFO
--rw-rw-r--   0 anhdtv7   (1001) anhdtv7   (1001)     1480 2023-05-22 05:05:16.000000 docchecker-0.1.1/src/docchecker.egg-info/SOURCES.txt
--rw-rw-r--   0 anhdtv7   (1001) anhdtv7   (1001)        1 2023-05-22 05:05:16.000000 docchecker-0.1.1/src/docchecker.egg-info/dependency_links.txt
--rw-rw-r--   0 anhdtv7   (1001) anhdtv7   (1001)       11 2023-05-22 05:05:16.000000 docchecker-0.1.1/src/docchecker.egg-info/top_level.txt
-drwxrwxr-x   0 anhdtv7   (1001) anhdtv7   (1001)        0 2023-05-22 05:05:16.190297 docchecker-0.1.1/tests/
--rw-rw-r--   0 anhdtv7   (1001) anhdtv7   (1001)      391 2023-05-21 21:33:23.000000 docchecker-0.1.1/tests/test.py
+drwxrwxr-x   0 anhdtv7   (1001) anhdtv7   (1001)        0 2023-05-24 21:21:26.766547 docchecker-0.1.2/
+-rw-rw-r--   0 anhdtv7   (1001) anhdtv7   (1001)     4754 2023-05-24 21:21:26.766547 docchecker-0.1.2/PKG-INFO
+-rw-rw-r--   0 anhdtv7   (1001) anhdtv7   (1001)     4211 2023-05-24 18:18:01.000000 docchecker-0.1.2/README.md
+-rw-rw-r--   0 anhdtv7   (1001) anhdtv7   (1001)      636 2023-05-24 21:19:02.000000 docchecker-0.1.2/pyproject.toml
+-rw-rw-r--   0 anhdtv7   (1001) anhdtv7   (1001)       38 2023-05-24 21:21:26.766547 docchecker-0.1.2/setup.cfg
+drwxrwxr-x   0 anhdtv7   (1001) anhdtv7   (1001)        0 2023-05-24 21:21:26.762547 docchecker-0.1.2/src/
+drwxrwxr-x   0 anhdtv7   (1001) anhdtv7   (1001)        0 2023-05-24 21:21:26.762547 docchecker-0.1.2/src/DocChecker/
+-rw-rw-r--   0 anhdtv7   (1001) anhdtv7   (1001)     4296 2023-05-24 21:19:38.000000 docchecker-0.1.2/src/DocChecker/DocCheckerNet.py
+-rw-rw-r--   0 anhdtv7   (1001) anhdtv7   (1001)      106 2023-05-19 04:44:42.000000 docchecker-0.1.2/src/DocChecker/__init__.py
+-rw-rw-r--   0 anhdtv7   (1001) anhdtv7   (1001)    19433 2023-05-08 12:43:08.000000 docchecker-0.1.2/src/DocChecker/model.py
+drwxrwxr-x   0 anhdtv7   (1001) anhdtv7   (1001)        0 2023-05-24 21:21:26.762547 docchecker-0.1.2/src/DocChecker/tree-sitter/
+drwxrwxr-x   0 anhdtv7   (1001) anhdtv7   (1001)        0 2023-05-24 21:21:26.762547 docchecker-0.1.2/src/DocChecker/tree-sitter/tree-sitter-python/
+drwxrwxr-x   0 anhdtv7   (1001) anhdtv7   (1001)        0 2023-05-24 21:21:26.762547 docchecker-0.1.2/src/DocChecker/tree-sitter/tree-sitter-python/examples/
+-rw-rw-r--   0 anhdtv7   (1001) anhdtv7   (1001)       38 2023-05-24 18:31:50.000000 docchecker-0.1.2/src/DocChecker/tree-sitter/tree-sitter-python/examples/compound-statement-without-trailing-newline.py
+-rw-rw-r--   0 anhdtv7   (1001) anhdtv7   (1001)       51 2023-05-24 18:31:50.000000 docchecker-0.1.2/src/DocChecker/tree-sitter/tree-sitter-python/examples/crlf-line-endings.py
+-rw-rw-r--   0 anhdtv7   (1001) anhdtv7   (1001)       74 2023-05-24 18:31:50.000000 docchecker-0.1.2/src/DocChecker/tree-sitter/tree-sitter-python/examples/mixed-spaces-tabs.py
+-rw-rw-r--   0 anhdtv7   (1001) anhdtv7   (1001)       73 2023-05-24 18:31:50.000000 docchecker-0.1.2/src/DocChecker/tree-sitter/tree-sitter-python/examples/multiple-newlines.py
+-rw-rw-r--   0 anhdtv7   (1001) anhdtv7   (1001)    31929 2023-05-24 18:31:50.000000 docchecker-0.1.2/src/DocChecker/tree-sitter/tree-sitter-python/examples/python2-grammar-crlf.py
+-rw-rw-r--   0 anhdtv7   (1001) anhdtv7   (1001)    30981 2023-05-24 18:31:50.000000 docchecker-0.1.2/src/DocChecker/tree-sitter/tree-sitter-python/examples/python2-grammar.py
+-rw-rw-r--   0 anhdtv7   (1001) anhdtv7   (1001)    31722 2023-05-24 18:31:50.000000 docchecker-0.1.2/src/DocChecker/tree-sitter/tree-sitter-python/examples/python3-grammar-crlf.py
+-rw-rw-r--   0 anhdtv7   (1001) anhdtv7   (1001)    30784 2023-05-24 18:31:50.000000 docchecker-0.1.2/src/DocChecker/tree-sitter/tree-sitter-python/examples/python3-grammar.py
+-rw-rw-r--   0 anhdtv7   (1001) anhdtv7   (1001)    50403 2023-05-24 18:31:50.000000 docchecker-0.1.2/src/DocChecker/tree-sitter/tree-sitter-python/examples/python3.8_grammar.py
+-rw-rw-r--   0 anhdtv7   (1001) anhdtv7   (1001)       16 2023-05-24 18:31:50.000000 docchecker-0.1.2/src/DocChecker/tree-sitter/tree-sitter-python/examples/simple-statements-without-trailing-newline.py
+-rw-rw-r--   0 anhdtv7   (1001) anhdtv7   (1001)     1236 2023-05-24 18:31:50.000000 docchecker-0.1.2/src/DocChecker/tree-sitter/tree-sitter-python/examples/tabs.py
+-rw-rw-r--   0 anhdtv7   (1001) anhdtv7   (1001)       58 2023-05-24 18:31:50.000000 docchecker-0.1.2/src/DocChecker/tree-sitter/tree-sitter-python/examples/trailing-whitespace.py
+drwxrwxr-x   0 anhdtv7   (1001) anhdtv7   (1001)        0 2023-05-24 21:21:26.762547 docchecker-0.1.2/src/DocChecker/tree-sitter/tree-sitter-python/test/
+drwxrwxr-x   0 anhdtv7   (1001) anhdtv7   (1001)        0 2023-05-24 21:21:26.766547 docchecker-0.1.2/src/DocChecker/tree-sitter/tree-sitter-python/test/highlight/
+-rw-rw-r--   0 anhdtv7   (1001) anhdtv7   (1001)      352 2023-05-24 18:31:50.000000 docchecker-0.1.2/src/DocChecker/tree-sitter/tree-sitter-python/test/highlight/keywords.py
+-rw-rw-r--   0 anhdtv7   (1001) anhdtv7   (1001)       99 2023-05-24 18:31:50.000000 docchecker-0.1.2/src/DocChecker/tree-sitter/tree-sitter-python/test/highlight/parameters.py
+-rw-rw-r--   0 anhdtv7   (1001) anhdtv7   (1001)     1297 2023-05-24 18:31:50.000000 docchecker-0.1.2/src/DocChecker/tree-sitter/tree-sitter-python/test/highlight/pattern_matching.py
+-rw-rw-r--   0 anhdtv7   (1001) anhdtv7   (1001)     4971 2023-05-24 21:20:09.000000 docchecker-0.1.2/src/DocChecker/utils.py
+drwxrwxr-x   0 anhdtv7   (1001) anhdtv7   (1001)        0 2023-05-24 21:21:26.766547 docchecker-0.1.2/src/docchecker.egg-info/
+-rw-rw-r--   0 anhdtv7   (1001) anhdtv7   (1001)     4754 2023-05-24 21:21:26.000000 docchecker-0.1.2/src/docchecker.egg-info/PKG-INFO
+-rw-rw-r--   0 anhdtv7   (1001) anhdtv7   (1001)     1480 2023-05-24 21:21:26.000000 docchecker-0.1.2/src/docchecker.egg-info/SOURCES.txt
+-rw-rw-r--   0 anhdtv7   (1001) anhdtv7   (1001)        1 2023-05-24 21:21:26.000000 docchecker-0.1.2/src/docchecker.egg-info/dependency_links.txt
+-rw-rw-r--   0 anhdtv7   (1001) anhdtv7   (1001)       28 2023-05-24 21:21:26.000000 docchecker-0.1.2/src/docchecker.egg-info/top_level.txt
+drwxrwxr-x   0 anhdtv7   (1001) anhdtv7   (1001)        0 2023-05-24 21:21:26.766547 docchecker-0.1.2/tests/
+-rw-rw-r--   0 anhdtv7   (1001) anhdtv7   (1001)      391 2023-05-21 21:33:23.000000 docchecker-0.1.2/tests/test.py
```

### Comparing `docchecker-0.1.1/PKG-INFO` & `docchecker-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docchecker
-Version: 0.1.1
+Version: 0.1.2
 Summary: A tool to detect the inconsistent between code and text in your source code
 Author-email: "Anh T. V. Dau" <vananh09052000@gmail.com>
 Project-URL: Homepage, https://github.com/Fsoft-AIC/DocChecker
 Project-URL: Bug Tracker, https://github.com/Fsoft-AIC/DocChecker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -58,15 +58,15 @@
 ```python
 from DocChecker.utils import inference
 ```
 Parameters:
 + input_file_path (str): the file path that contains source code if users want to check all the functions in there.
 + raw_code (str): a sequence of source code if `input_file_path` is not given.
 + language (str, required): the programming language. We support 10 popular programming languages such as Java, JavaScript, Python, Ruby, Rust, Golang, C#, C++, C, and PHP.
-+ output_file_path (str): if `input_file_path` is given, the results from our tool will be written in this path; otherwise, they will be printed on the screen.
++ output_file_path (str): if it is not None, the results from our tool will be written in this path; otherwise, they will be printed on the screen.
 Returns:
 
 + list of dictionaries, including:
     - function_name: the name of each function in the raw code
     - code: code snippet
     - docstring: the docstring corresponding code snippet
     - predict: the prediction of DocChecker. It returns "Inconsistent!” for the inconsistent pair and “Consistent!” means the docstring is consistent with the code in a code-text pair
```

### Comparing `docchecker-0.1.1/README.md` & `docchecker-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 ```python
 from DocChecker.utils import inference
 ```
 Parameters:
 + input_file_path (str): the file path that contains source code if users want to check all the functions in there.
 + raw_code (str): a sequence of source code if `input_file_path` is not given.
 + language (str, required): the programming language. We support 10 popular programming languages such as Java, JavaScript, Python, Ruby, Rust, Golang, C#, C++, C, and PHP.
-+ output_file_path (str): if `input_file_path` is given, the results from our tool will be written in this path; otherwise, they will be printed on the screen.
++ output_file_path (str): if it is not None, the results from our tool will be written in this path; otherwise, they will be printed on the screen.
 Returns:
 
 + list of dictionaries, including:
     - function_name: the name of each function in the raw code
     - code: code snippet
     - docstring: the docstring corresponding code snippet
     - predict: the prediction of DocChecker. It returns "Inconsistent!” for the inconsistent pair and “Consistent!” means the docstring is consistent with the code in a code-text pair
```

### Comparing `docchecker-0.1.1/pyproject.toml` & `docchecker-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "docchecker"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Anh T. V. Dau", email="vananh09052000@gmail.com"},
 ]
 description = "A tool to detect the inconsistent between code and text in your source code"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
+
 [project.urls]
 "Homepage" = "https://github.com/Fsoft-AIC/DocChecker"
 "Bug Tracker" = "https://github.com/Fsoft-AIC/DocChecker/issues"
```

### Comparing `docchecker-0.1.1/src/DocChecker/DocCheckerNet.py` & `docchecker-0.1.2/src/DocChecker/DocCheckerNet.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 import os
 import torch
-from .model import Seq2Seq
+from model import Seq2Seq
 from transformers import (RobertaConfig, RobertaModel, RobertaTokenizer)
 import torch.nn as nn
 import gdown 
 
 class DocCheckerNet(nn.Module):
 
     def __init__(self):
```

### Comparing `docchecker-0.1.1/src/DocChecker/model.py` & `docchecker-0.1.2/src/DocChecker/model.py`

 * *Files identical despite different names*

### Comparing `docchecker-0.1.1/src/DocChecker/tree-sitter/tree-sitter-python/examples/python2-grammar-crlf.py` & `docchecker-0.1.2/src/DocChecker/tree-sitter/tree-sitter-python/examples/python2-grammar-crlf.py`

 * *Files identical despite different names*

### Comparing `docchecker-0.1.1/src/DocChecker/tree-sitter/tree-sitter-python/examples/python2-grammar.py` & `docchecker-0.1.2/src/DocChecker/tree-sitter/tree-sitter-python/examples/python2-grammar.py`

 * *Files identical despite different names*

### Comparing `docchecker-0.1.1/src/DocChecker/tree-sitter/tree-sitter-python/examples/python3-grammar-crlf.py` & `docchecker-0.1.2/src/DocChecker/tree-sitter/tree-sitter-python/examples/python3-grammar-crlf.py`

 * *Files identical despite different names*

### Comparing `docchecker-0.1.1/src/DocChecker/tree-sitter/tree-sitter-python/examples/python3-grammar.py` & `docchecker-0.1.2/src/DocChecker/tree-sitter/tree-sitter-python/examples/python3-grammar.py`

 * *Files identical despite different names*

### Comparing `docchecker-0.1.1/src/DocChecker/tree-sitter/tree-sitter-python/examples/python3.8_grammar.py` & `docchecker-0.1.2/src/DocChecker/tree-sitter/tree-sitter-python/examples/python3.8_grammar.py`

 * *Files identical despite different names*

### Comparing `docchecker-0.1.1/src/DocChecker/tree-sitter/tree-sitter-python/examples/tabs.py` & `docchecker-0.1.2/src/DocChecker/tree-sitter/tree-sitter-python/examples/tabs.py`

 * *Files identical despite different names*

### Comparing `docchecker-0.1.1/src/DocChecker/tree-sitter/tree-sitter-python/test/highlight/pattern_matching.py` & `docchecker-0.1.2/src/DocChecker/tree-sitter/tree-sitter-python/test/highlight/pattern_matching.py`

 * *Files identical despite different names*

### Comparing `docchecker-0.1.1/src/DocChecker/utils.py` & `docchecker-0.1.2/src/DocChecker/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 from codetext.utils import parse_code
 from codetext.parser import GoParser, PhpParser, RubyParser, JavaParser, JavascriptParser, \
     PythonParser, CppParser, CsharpParser, RustParser
 from codetext.parser.language_parser import get_node_text
 import os
-from .DocCheckerNet import DocCheckerNet
+from DocCheckerNet import DocCheckerNet
 import torch
 import json
 
 SUPPORTED_LANGUAGE = ['python', 'java', 'javascript', 'ruby', 'go', 'c', 'c++', 'c#', 'php', 'rust']
 
 def get_language_parser(language):
     if language == 'python':
@@ -84,29 +84,23 @@
         with open(input_file_path, 'r') as f:
             for line in f:
                 raw_code += line
 
     root = parse_code(raw_code, language) 
     root_node = root.root_node
     function_list = Parser.get_function_list(root_node)
-    print(function_list)
-    print(raw_code)
-    if output_file_path is None:
-        output_file_path = "./out.json"
+    # if output_file_path is None:
+        # output_file_path = "./out.json"
     codes  = []
     docstrings = []
     func_names = []
     for function in function_list:
         raw_code = get_node_text(function)
         code_tree = parse_code(raw_code, language)
         code_tree_node = code_tree.root_node
-        print(raw_code)
-        print(code_tree_node)
-        print(Parser.get_function_list(code_tree_node))
-        print('----')
         code_snippet = Parser.get_function_list(code_tree_node)[0]
         docstring = get_comment(Parser,code_snippet)
         metadata = Parser.get_function_metadata(code_snippet)
 
         code = raw_code.replace(docstring,"")
         docstring = docstring.strip('"').strip("'").strip("#")
         codes.append(code)
@@ -121,17 +115,17 @@
         item['function_name'] = func_names[id]
         item['code'] = codes[id]
         item['docstring'] = docstrings[id]
         item['predict'] = results[id]['predict']
         item['recommended_docstring'] = results[id]['recommended_docstring']
         output.append(item)
 
-    if input_file_path is not None:
+    if output_file_path is not None:
         with open(output_file_path, "w") as fo:
-                json.dumps(output, fo, ensure_ascii=False)
+                json.dump(output, fo)
     else:
         print(output)
 
 if __name__ == "__main__":
     # inference(input_file_path='../../tests/test.py', language='python')
 
     
@@ -140,8 +134,8 @@
             # This method should be called every time 
             # we finish writing into a file and consider it done .
             if basename:
                 path = os.path.basename(path)
             return os.path.splitext(path)
                 }
         """
-    inference(raw_code=code,language='python')
+    inference(raw_code=code,language='python',output_file_path='./out.json')
```

### Comparing `docchecker-0.1.1/src/docchecker.egg-info/PKG-INFO` & `docchecker-0.1.2/src/docchecker.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docchecker
-Version: 0.1.1
+Version: 0.1.2
 Summary: A tool to detect the inconsistent between code and text in your source code
 Author-email: "Anh T. V. Dau" <vananh09052000@gmail.com>
 Project-URL: Homepage, https://github.com/Fsoft-AIC/DocChecker
 Project-URL: Bug Tracker, https://github.com/Fsoft-AIC/DocChecker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -58,15 +58,15 @@
 ```python
 from DocChecker.utils import inference
 ```
 Parameters:
 + input_file_path (str): the file path that contains source code if users want to check all the functions in there.
 + raw_code (str): a sequence of source code if `input_file_path` is not given.
 + language (str, required): the programming language. We support 10 popular programming languages such as Java, JavaScript, Python, Ruby, Rust, Golang, C#, C++, C, and PHP.
-+ output_file_path (str): if `input_file_path` is given, the results from our tool will be written in this path; otherwise, they will be printed on the screen.
++ output_file_path (str): if it is not None, the results from our tool will be written in this path; otherwise, they will be printed on the screen.
 Returns:
 
 + list of dictionaries, including:
     - function_name: the name of each function in the raw code
     - code: code snippet
     - docstring: the docstring corresponding code snippet
     - predict: the prediction of DocChecker. It returns "Inconsistent!” for the inconsistent pair and “Consistent!” means the docstring is consistent with the code in a code-text pair
```

### Comparing `docchecker-0.1.1/src/docchecker.egg-info/SOURCES.txt` & `docchecker-0.1.2/src/docchecker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

