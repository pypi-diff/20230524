# Comparing `tmp/baichat_py-0.2.1.tar.gz` & `tmp/baichat_py-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baichat_py-0.2.1.tar", max compression
+gzip compressed data, was "baichat_py-0.2.2.tar", max compression
```

## Comparing `baichat_py-0.2.1.tar` & `baichat_py-0.2.2.tar`

### file list

```diff
@@ -1,5 +1,4 @@
--rw-r--r--   0        0        0     1062 2023-04-27 10:27:07.676039 baichat_py-0.2.1/README.md
--rw-r--r--   0        0        0     5807 2023-04-27 10:32:59.034118 baichat_py-0.2.1/baichat_py/__init__.py
--rw-r--r--   0        0        0     1040 2023-04-27 10:33:03.116176 baichat_py-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1761 1970-01-01 00:00:00.000000 baichat_py-0.2.1/setup.py
--rw-r--r--   0        0        0     2170 1970-01-01 00:00:00.000000 baichat_py-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1162 2023-05-24 19:17:37.396739 baichat_py-0.2.2/README.md
+-rw-r--r--   0        0        0     5807 2023-05-24 19:17:37.397739 baichat_py-0.2.2/baichat_py/__init__.py
+-rw-r--r--   0        0        0     1198 2023-05-24 19:17:37.398739 baichat_py-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2318 1970-01-01 00:00:00.000000 baichat_py-0.2.2/PKG-INFO
```

### Comparing `baichat_py-0.2.1/README.md` & `baichat_py-0.2.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 # BAIChat API Python
 
 ## Installation
 
-You can install it from PyPi
+### Pypi
 
 ``` shell
 pip install baichat-py
 ```
 
+### Codeberg
+
+``` shell
+pip install --index-url https://codeberg.org/api/packages/Bavarder/pypi/simple/ baichat-py
+```
+
 ## Usage
 
 ### Async
 
 ``` python
 import asyncio
```

### Comparing `baichat_py-0.2.1/baichat_py/__init__.py` & `baichat_py-0.2.2/baichat_py/__init__.py`

 * *Files identical despite different names*

### Comparing `baichat_py-0.2.1/PKG-INFO` & `baichat_py-0.2.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: baichat-py
-Version: 0.2.1
+Version: 0.2.2
 Summary: 
-Home-page: https://github.com/Bavarder/baichat-py
+Home-page: https://codeberg.org/Bavarder/baichat-py
 License: GPL-3.0-or-later
 Keywords: openai,gpt3,baichat,chat
 Author: 0xMRTT
 Author-email: 0xMRTT@proton.me
 Maintainer: 0xMRTT
 Maintainer-email: 0xMRTT@proton.me
 Requires-Python: >=3.10,<4.0
@@ -16,30 +16,37 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
-Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
-Project-URL: Bug Tracker, https://github.com/Bavarder/baichat-py/issues
-Project-URL: Documentation, https://github.com/Bavarder/baichat-py
+Requires-Dist: aiohttp (>=3.8.0,<4.0.0)
+Requires-Dist: requests (>=2.29.0,<3.0.0)
+Project-URL: Bug Tracker, https://codeberg.org/Bavarder/baichat-py/issues
+Project-URL: Documentation, https://codeberg.org/Bavarder/baichat-py
 Project-URL: Repository, https://github.com/Bavarder/baichat-py
 Description-Content-Type: text/markdown
 
 # BAIChat API Python
 
 ## Installation
 
-You can install it from PyPi
+### Pypi
 
 ``` shell
 pip install baichat-py
 ```
 
+### Codeberg
+
+``` shell
+pip install --index-url https://codeberg.org/api/packages/Bavarder/pypi/simple/ baichat-py
+```
+
 ## Usage
 
 ### Async
 
 ``` python
 import asyncio
```

