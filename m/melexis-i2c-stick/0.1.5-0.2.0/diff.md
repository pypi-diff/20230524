# Comparing `tmp/melexis-i2c-stick-0.1.5.tar.gz` & `tmp/melexis-i2c-stick-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "melexis-i2c-stick-0.1.5.tar", last modified: Fri May 19 23:26:43 2023, max compression
+gzip compressed data, was "melexis-i2c-stick-0.2.0.tar", last modified: Tue May 23 22:02:31 2023, max compression
```

## Comparing `melexis-i2c-stick-0.1.5.tar` & `melexis-i2c-stick-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 23:26:43.611360 melexis-i2c-stick-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-19 23:26:24.000000 melexis-i2c-stick-0.1.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-19 23:26:24.000000 melexis-i2c-stick-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-19 23:26:24.000000 melexis-i2c-stick-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-19 23:26:24.000000 melexis-i2c-stick-0.1.5/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-19 23:26:43.611360 melexis-i2c-stick-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-19 23:26:24.000000 melexis-i2c-stick-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 23:26:43.607360 melexis-i2c-stick-0.1.5/melexis/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 23:26:43.607360 melexis-i2c-stick-0.1.5/melexis/i2c_stick/
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-19 23:26:24.000000 melexis-i2c-stick-0.1.5/melexis/i2c_stick/I2CStick.py
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-05-19 23:26:24.000000 melexis-i2c-stick-0.1.5/melexis/i2c_stick/MemoryFile.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-19 23:26:24.000000 melexis-i2c-stick-0.1.5/melexis/i2c_stick/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 23:26:43.611360 melexis-i2c-stick-0.1.5/melexis_i2c_stick.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-19 23:26:43.000000 melexis-i2c-stick-0.1.5/melexis_i2c_stick.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-19 23:26:43.000000 melexis-i2c-stick-0.1.5/melexis_i2c_stick.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 23:26:43.000000 melexis-i2c-stick-0.1.5/melexis_i2c_stick.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 23:26:43.000000 melexis-i2c-stick-0.1.5/melexis_i2c_stick.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-19 23:26:43.000000 melexis-i2c-stick-0.1.5/melexis_i2c_stick.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-19 23:26:24.000000 melexis-i2c-stick-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 23:26:43.611360 melexis-i2c-stick-0.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:02:31.384097 melexis-i2c-stick-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-23 22:02:12.000000 melexis-i2c-stick-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-23 22:02:12.000000 melexis-i2c-stick-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-23 22:02:12.000000 melexis-i2c-stick-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-23 22:02:12.000000 melexis-i2c-stick-0.2.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-23 22:02:31.384097 melexis-i2c-stick-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-23 22:02:12.000000 melexis-i2c-stick-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:02:31.380097 melexis-i2c-stick-0.2.0/melexis/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:02:31.384097 melexis-i2c-stick-0.2.0/melexis/i2c_stick/
+-rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-05-23 22:02:12.000000 melexis-i2c-stick-0.2.0/melexis/i2c_stick/I2CStick.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6083 2023-05-23 22:02:12.000000 melexis-i2c-stick-0.2.0/melexis/i2c_stick/MemoryFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-23 22:02:12.000000 melexis-i2c-stick-0.2.0/melexis/i2c_stick/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-23 22:02:12.000000 melexis-i2c-stick-0.2.0/melexis/i2c_stick/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:02:31.384097 melexis-i2c-stick-0.2.0/melexis_i2c_stick.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-23 22:02:31.000000 melexis-i2c-stick-0.2.0/melexis_i2c_stick.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-23 22:02:31.000000 melexis-i2c-stick-0.2.0/melexis_i2c_stick.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 22:02:31.000000 melexis-i2c-stick-0.2.0/melexis_i2c_stick.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-23 22:02:31.000000 melexis-i2c-stick-0.2.0/melexis_i2c_stick.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 22:02:31.000000 melexis-i2c-stick-0.2.0/melexis_i2c_stick.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-23 22:02:31.000000 melexis-i2c-stick-0.2.0/melexis_i2c_stick.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-23 22:02:12.000000 melexis-i2c-stick-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 22:02:31.384097 melexis-i2c-stick-0.2.0/setup.cfg
```

### Comparing `melexis-i2c-stick-0.1.5/CONTRIBUTING.md` & `melexis-i2c-stick-0.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `melexis-i2c-stick-0.1.5/LICENSE` & `melexis-i2c-stick-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `melexis-i2c-stick-0.1.5/PKG-INFO` & `melexis-i2c-stick-0.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: melexis-i2c-stick
-Version: 0.1.5
+Version: 0.2.0
 Summary: Melexis I2C Stick, python interface
 Author-email: Karel Vanroye <kva@melexis.com>
 License:    Copyright 2023 Melexis
         
            Licensed under the Apache License, Version 2.0 (the "License");
            you may not use this file except in compliance with the License.
            You may obtain a copy of the License at
@@ -24,14 +24,15 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.3
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 License-File: NOTICE
 
-# melexis-i2c-stick-py
+# melexis-i2c-stick
 
 Python interface for I2C Stick, it runs on the host computer to communicate with the I2C Stick over the UART.
 
+
 ## Getting started.
 
 todo...
```

### Comparing `melexis-i2c-stick-0.1.5/melexis_i2c_stick.egg-info/PKG-INFO` & `melexis-i2c-stick-0.2.0/melexis_i2c_stick.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: melexis-i2c-stick
-Version: 0.1.5
+Version: 0.2.0
 Summary: Melexis I2C Stick, python interface
 Author-email: Karel Vanroye <kva@melexis.com>
 License:    Copyright 2023 Melexis
         
            Licensed under the Apache License, Version 2.0 (the "License");
            you may not use this file except in compliance with the License.
            You may obtain a copy of the License at
@@ -24,14 +24,15 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.3
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 License-File: NOTICE
 
-# melexis-i2c-stick-py
+# melexis-i2c-stick
 
 Python interface for I2C Stick, it runs on the host computer to communicate with the I2C Stick over the UART.
 
+
 ## Getting started.
 
 todo...
```

### Comparing `melexis-i2c-stick-0.1.5/pyproject.toml` & `melexis-i2c-stick-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [build-system]
 requires      = ["setuptools>=63.2.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "melexis-i2c-stick"
-version = "0.1.5"
+version = "0.2.0"
 description = "Melexis I2C Stick, python interface"
 readme = "README.md"
 authors = [{ name = "Karel Vanroye", email = "kva@melexis.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
@@ -27,20 +27,20 @@
 
 [project.optional-dependencies]
 dev = []
 
 [project.urls]
 Homepage = "https://github.com/melexis/i2c-stick"
 
-# [project.scripts]
-# melexis_i2c_stick = "melexis.i2c_stick.__main__:main"
+[project.scripts]
+melexis_i2c_stick = "melexis.i2c_stick.__main__:main"
 
 
 [tool.bumpver]
-current_version = "0.1.5"
+current_version = "0.2.0"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = false
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

