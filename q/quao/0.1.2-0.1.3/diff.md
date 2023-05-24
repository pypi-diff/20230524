# Comparing `tmp/quao-0.1.2.tar.gz` & `tmp/quao-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quao-0.1.2.tar", last modified: Wed May 24 07:01:43 2023, max compression
+gzip compressed data, was "quao-0.1.3.tar", last modified: Wed May 24 07:35:17 2023, max compression
```

## Comparing `quao-0.1.2.tar` & `quao-0.1.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 07:01:43.154373 quao-0.1.2/
--rw-rw-rw-   0        0        0     1111 2023-04-27 03:39:26.000000 quao-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     2839 2023-05-24 07:01:43.153378 quao-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1163 2023-04-27 03:33:31.000000 quao-0.1.2/README.md
--rw-rw-rw-   0        0        0      811 2023-05-24 04:54:36.000000 quao-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-24 07:01:43.154373 quao-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-24 07:01:43.116373 quao-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-24 07:01:43.130374 quao-0.1.2/src/quao/
--rw-rw-rw-   0        0        0      134 2023-04-25 02:47:26.000000 quao-0.1.2/src/quao/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-24 07:01:43.146375 quao-0.1.2/src/quao/algorithms/
--rw-rw-rw-   0        0        0        2 2023-04-25 02:47:26.000000 quao-0.1.2/src/quao/algorithms/__init__.py
--rw-rw-rw-   0        0        0     5305 2023-04-25 02:47:26.000000 quao-0.1.2/src/quao/algorithms/shor.py
--rw-rw-rw-   0        0        0     2207 2023-05-24 04:52:27.000000 quao-0.1.2/src/quao/backend.py
--rw-rw-rw-   0        0        0      366 2023-04-28 02:04:51.000000 quao-0.1.2/src/quao/dataUtils.py
-drwxrwxrwx   0        0        0        0 2023-05-24 07:01:43.148373 quao-0.1.2/src/quao/enum/
--rw-rw-rw-   0        0        0      200 2023-05-24 01:59:39.000000 quao-0.1.2/src/quao/enum/providerType.py
-drwxrwxrwx   0        0        0        0 2023-05-24 07:01:43.151380 quao-0.1.2/src/quao/sdk/
--rw-rw-rw-   0        0        0        2 2023-04-25 02:47:26.000000 quao-0.1.2/src/quao/sdk/__init__.py
--rw-rw-rw-   0        0        0     3654 2023-05-24 02:12:26.000000 quao-0.1.2/src/quao/sdk/qiskit.py
--rw-rw-rw-   0        0        0     1304 2023-05-24 05:04:40.000000 quao-0.1.2/src/quao/utilities.py
-drwxrwxrwx   0        0        0        0 2023-05-24 07:01:43.143374 quao-0.1.2/src/quao.egg-info/
--rw-rw-rw-   0        0        0     2839 2023-05-24 07:01:43.000000 quao-0.1.2/src/quao.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      414 2023-05-24 07:01:43.000000 quao-0.1.2/src/quao.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 07:01:43.000000 quao-0.1.2/src/quao.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      100 2023-05-24 07:01:43.000000 quao-0.1.2/src/quao.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-05-24 07:01:43.000000 quao-0.1.2/src/quao.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-24 07:35:17.896626 quao-0.1.3/
+-rw-rw-rw-   0        0        0     1111 2023-04-27 03:39:26.000000 quao-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     2839 2023-05-24 07:35:17.895628 quao-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1163 2023-04-27 03:33:31.000000 quao-0.1.3/README.md
+-rw-rw-rw-   0        0        0      811 2023-05-24 07:34:57.000000 quao-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-24 07:35:17.897625 quao-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-24 07:35:17.851624 quao-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-24 07:35:17.863626 quao-0.1.3/src/quao/
+-rw-rw-rw-   0        0        0      134 2023-04-25 02:47:26.000000 quao-0.1.3/src/quao/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 07:35:17.888623 quao-0.1.3/src/quao/algorithms/
+-rw-rw-rw-   0        0        0        2 2023-04-25 02:47:26.000000 quao-0.1.3/src/quao/algorithms/__init__.py
+-rw-rw-rw-   0        0        0     5305 2023-04-25 02:47:26.000000 quao-0.1.3/src/quao/algorithms/shor.py
+-rw-rw-rw-   0        0        0     2207 2023-05-24 04:52:27.000000 quao-0.1.3/src/quao/backend.py
+-rw-rw-rw-   0        0        0      366 2023-04-28 02:04:51.000000 quao-0.1.3/src/quao/dataUtils.py
+drwxrwxrwx   0        0        0        0 2023-05-24 07:35:17.889625 quao-0.1.3/src/quao/enum/
+-rw-rw-rw-   0        0        0      200 2023-05-24 01:59:39.000000 quao-0.1.3/src/quao/enum/providerType.py
+drwxrwxrwx   0        0        0        0 2023-05-24 07:35:17.892628 quao-0.1.3/src/quao/sdk/
+-rw-rw-rw-   0        0        0        2 2023-04-25 02:47:26.000000 quao-0.1.3/src/quao/sdk/__init__.py
+-rw-rw-rw-   0        0        0     3654 2023-05-24 02:12:26.000000 quao-0.1.3/src/quao/sdk/qiskit.py
+-rw-rw-rw-   0        0        0     1304 2023-05-24 05:04:40.000000 quao-0.1.3/src/quao/utilities.py
+drwxrwxrwx   0        0        0        0 2023-05-24 07:35:17.885675 quao-0.1.3/src/quao.egg-info/
+-rw-rw-rw-   0        0        0     2839 2023-05-24 07:35:17.000000 quao-0.1.3/src/quao.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      414 2023-05-24 07:35:17.000000 quao-0.1.3/src/quao.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 07:35:17.000000 quao-0.1.3/src/quao.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      100 2023-05-24 07:35:17.000000 quao-0.1.3/src/quao.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-05-24 07:35:17.000000 quao-0.1.3/src/quao.egg-info/top_level.txt
```

### Comparing `quao-0.1.2/LICENSE` & `quao-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `quao-0.1.2/PKG-INFO` & `quao-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quao
-Version: 0.1.2
+Version: 0.1.3
 Summary: Quao Library supporting Quao Platform for Quantum Computing
 Author-email: "CITYNOW Co. Ltd. " <corp@citynow.vn>
 License: The MIT License (MIT)
         Copyright © CITYNOW Co. Ltd. All rights reserved.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `quao-0.1.2/README.md` & `quao-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `quao-0.1.2/pyproject.toml` & `quao-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "quao"
-version = "0.1.2"
+version = "0.1.3"
 description = "Quao Library supporting Quao Platform for Quantum Computing"
 readme = "README.md"
 authors = [{ name = "CITYNOW Co. Ltd. ", email = "corp@citynow.vn" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["quao", "quantum"]
 dependencies = [
-    "qiskit==0.41.1",
+    "qiskit==0.43.0",
     "qiskit_ibm_runtime==0.10.0",
     "numpy>=1.22.3",
 ]
 requires-python = ">=3.7"
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
```

### Comparing `quao-0.1.2/src/quao/algorithms/shor.py` & `quao-0.1.3/src/quao/algorithms/shor.py`

 * *Files identical despite different names*

### Comparing `quao-0.1.2/src/quao/backend.py` & `quao-0.1.3/src/quao/backend.py`

 * *Files identical despite different names*

### Comparing `quao-0.1.2/src/quao/sdk/qiskit.py` & `quao-0.1.3/src/quao/sdk/qiskit.py`

 * *Files identical despite different names*

### Comparing `quao-0.1.2/src/quao/utilities.py` & `quao-0.1.3/src/quao/utilities.py`

 * *Files identical despite different names*

### Comparing `quao-0.1.2/src/quao.egg-info/PKG-INFO` & `quao-0.1.3/src/quao.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quao
-Version: 0.1.2
+Version: 0.1.3
 Summary: Quao Library supporting Quao Platform for Quantum Computing
 Author-email: "CITYNOW Co. Ltd. " <corp@citynow.vn>
 License: The MIT License (MIT)
         Copyright © CITYNOW Co. Ltd. All rights reserved.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

