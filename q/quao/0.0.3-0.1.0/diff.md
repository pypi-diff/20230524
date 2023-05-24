# Comparing `tmp/quao-0.0.3.tar.gz` & `tmp/quao-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quao-0.0.3.tar", last modified: Thu Apr 27 06:52:58 2023, max compression
+gzip compressed data, was "quao-0.1.0.tar", last modified: Wed May 24 04:14:10 2023, max compression
```

## Comparing `quao-0.0.3.tar` & `quao-0.1.0.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 06:52:58.285268 quao-0.0.3/
--rw-rw-rw-   0        0        0     1111 2023-04-27 03:39:26.000000 quao-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     2839 2023-04-27 06:52:58.284267 quao-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1163 2023-04-27 03:33:31.000000 quao-0.0.3/README.md
--rw-rw-rw-   0        0        0      892 2023-04-27 06:51:23.000000 quao-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-27 06:52:58.285268 quao-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-27 06:52:58.168270 quao-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-27 06:52:58.206390 quao-0.0.3/src/quao/
--rw-rw-rw-   0        0        0      134 2023-04-25 02:47:26.000000 quao-0.0.3/src/quao/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-27 06:52:58.245294 quao-0.0.3/src/quao/algorithms/
--rw-rw-rw-   0        0        0        2 2023-04-25 02:47:26.000000 quao-0.0.3/src/quao/algorithms/__init__.py
--rw-rw-rw-   0        0        0     5305 2023-04-25 02:47:26.000000 quao-0.0.3/src/quao/algorithms/shor.py
--rw-rw-rw-   0        0        0     2900 2023-04-26 11:10:24.000000 quao-0.0.3/src/quao/backend.py
--rw-rw-rw-   0        0        0      366 2023-04-26 11:27:39.000000 quao-0.0.3/src/quao/dataUtils.py
-drwxrwxrwx   0        0        0        0 2023-04-27 06:52:58.282267 quao-0.0.3/src/quao/sdk/
--rw-rw-rw-   0        0        0        2 2023-04-25 02:47:26.000000 quao-0.0.3/src/quao/sdk/__init__.py
--rw-rw-rw-   0        0        0     1805 2023-04-26 05:03:52.000000 quao-0.0.3/src/quao/sdk/braket.py
--rw-rw-rw-   0        0        0     1640 2023-04-26 05:03:52.000000 quao-0.0.3/src/quao/sdk/cirq.py
--rw-rw-rw-   0        0        0     2110 2023-04-26 10:35:09.000000 quao-0.0.3/src/quao/sdk/qiskit.py
--rw-rw-rw-   0        0        0     1218 2023-04-27 02:50:32.000000 quao-0.0.3/src/quao/sdk/qsharp.py
--rw-rw-rw-   0        0        0     2442 2023-04-26 10:59:14.000000 quao-0.0.3/src/quao/utilities.py
-drwxrwxrwx   0        0        0        0 2023-04-27 06:52:58.235267 quao-0.0.3/src/quao.egg-info/
--rw-rw-rw-   0        0        0     2839 2023-04-27 06:52:58.000000 quao-0.0.3/src/quao.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      451 2023-04-27 06:52:58.000000 quao-0.0.3/src/quao.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 06:52:58.000000 quao-0.0.3/src/quao.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      158 2023-04-27 06:52:58.000000 quao-0.0.3/src/quao.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-27 06:52:58.000000 quao-0.0.3/src/quao.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-24 04:14:10.309378 quao-0.1.0/
+-rw-rw-rw-   0        0        0     1111 2023-04-27 03:39:26.000000 quao-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     2839 2023-05-24 04:14:10.308376 quao-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1163 2023-04-27 03:33:31.000000 quao-0.1.0/README.md
+-rw-rw-rw-   0        0        0      927 2023-05-24 01:59:39.000000 quao-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-24 04:14:10.310378 quao-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-24 04:14:10.271376 quao-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-24 04:14:10.283379 quao-0.1.0/src/quao/
+-rw-rw-rw-   0        0        0      134 2023-04-25 02:47:26.000000 quao-0.1.0/src/quao/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 04:14:10.300377 quao-0.1.0/src/quao/algorithms/
+-rw-rw-rw-   0        0        0        2 2023-04-25 02:47:26.000000 quao-0.1.0/src/quao/algorithms/__init__.py
+-rw-rw-rw-   0        0        0     5305 2023-04-25 02:47:26.000000 quao-0.1.0/src/quao/algorithms/shor.py
+-rw-rw-rw-   0        0        0     2900 2023-04-26 11:10:24.000000 quao-0.1.0/src/quao/backend.py
+-rw-rw-rw-   0        0        0      366 2023-04-28 02:04:51.000000 quao-0.1.0/src/quao/dataUtils.py
+drwxrwxrwx   0        0        0        0 2023-05-24 04:14:10.302376 quao-0.1.0/src/quao/enum/
+-rw-rw-rw-   0        0        0      200 2023-05-24 01:59:39.000000 quao-0.1.0/src/quao/enum/providerType.py
+drwxrwxrwx   0        0        0        0 2023-05-24 04:14:10.307376 quao-0.1.0/src/quao/sdk/
+-rw-rw-rw-   0        0        0        2 2023-04-25 02:47:26.000000 quao-0.1.0/src/quao/sdk/__init__.py
+-rw-rw-rw-   0        0        0     1805 2023-04-26 05:03:52.000000 quao-0.1.0/src/quao/sdk/braket.py
+-rw-rw-rw-   0        0        0     1640 2023-04-26 05:03:52.000000 quao-0.1.0/src/quao/sdk/cirq.py
+-rw-rw-rw-   0        0        0     3654 2023-05-24 02:12:26.000000 quao-0.1.0/src/quao/sdk/qiskit.py
+-rw-rw-rw-   0        0        0     1218 2023-04-27 02:50:32.000000 quao-0.1.0/src/quao/sdk/qsharp.py
+-rw-rw-rw-   0        0        0     2531 2023-05-24 01:59:39.000000 quao-0.1.0/src/quao/utilities.py
+drwxrwxrwx   0        0        0        0 2023-05-24 04:14:10.298996 quao-0.1.0/src/quao.egg-info/
+-rw-rw-rw-   0        0        0     2839 2023-05-24 04:14:10.000000 quao-0.1.0/src/quao.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      481 2023-05-24 04:14:10.000000 quao-0.1.0/src/quao.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 04:14:10.000000 quao-0.1.0/src/quao.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      185 2023-05-24 04:14:10.000000 quao-0.1.0/src/quao.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-05-24 04:14:10.000000 quao-0.1.0/src/quao.egg-info/top_level.txt
```

### Comparing `quao-0.0.3/LICENSE` & `quao-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quao-0.0.3/PKG-INFO` & `quao-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quao
-Version: 0.0.3
+Version: 0.1.0
 Summary: Quao Library supporting Quao Platform for Quantum Computing
 Author-email: "CITYNOW Co. Ltd. " <corp@citynow.vn>
 License: The MIT License (MIT)
         Copyright © CITYNOW Co. Ltd. All rights reserved.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `quao-0.0.3/README.md` & `quao-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `quao-0.0.3/pyproject.toml` & `quao-0.1.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "quao"
-version = "0.0.3"
+version = "0.1.0"
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
     "qiskit==0.41.1",
+    "qiskit_ibm_runtime==0.10.0",
     "cirq==1.1.0",
     "amazon-braket-sdk==1.36.5",
     "numpy>=1.22.3",
     "strangeworks==0.4.1",
     "strangeworks-braket==1.0.3"
 ]
 requires-python = ">=3.7"
```

### Comparing `quao-0.0.3/src/quao/algorithms/shor.py` & `quao-0.1.0/src/quao/algorithms/shor.py`

 * *Files identical despite different names*

### Comparing `quao-0.0.3/src/quao/backend.py` & `quao-0.1.0/src/quao/backend.py`

 * *Files identical despite different names*

### Comparing `quao-0.0.3/src/quao/sdk/braket.py` & `quao-0.1.0/src/quao/sdk/braket.py`

 * *Files identical despite different names*

### Comparing `quao-0.0.3/src/quao/sdk/cirq.py` & `quao-0.1.0/src/quao/sdk/cirq.py`

 * *Files identical despite different names*

### Comparing `quao-0.0.3/src/quao/sdk/qsharp.py` & `quao-0.1.0/src/quao/sdk/qsharp.py`

 * *Files identical despite different names*

### Comparing `quao-0.0.3/src/quao/utilities.py` & `quao-0.1.0/src/quao/utilities.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,17 +18,19 @@
 
     @staticmethod
     def generate_response(job_response: JobResponse) -> dict:
         if job_response:
             status_code = 201  # not yet finished
             if job_response.job_status == "DONE":
                 status_code = 200
+            elif job_response.job_status == "ERROR":
+                status_code = 400
             job_dict = {
-                "jobStatus": job_response.job_status,
                 "providerJobId": job_response.provider_job_id,
+                "jobStatus": job_response.job_status,
                 "jobResult": job_response.job_result
             }  # Object to directory
             response = {"statusCode": status_code, "body": job_dict}
         else:
             response = {
                 "statusCode": 500,
                 "body": "Error in function code. Please contact the developer.",
```

### Comparing `quao-0.0.3/src/quao.egg-info/PKG-INFO` & `quao-0.1.0/src/quao.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quao
-Version: 0.0.3
+Version: 0.1.0
 Summary: Quao Library supporting Quao Platform for Quantum Computing
 Author-email: "CITYNOW Co. Ltd. " <corp@citynow.vn>
 License: The MIT License (MIT)
         Copyright © CITYNOW Co. Ltd. All rights reserved.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

