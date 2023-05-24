# Comparing `tmp/quao-0.1.3.tar.gz` & `tmp/quao-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quao-0.1.3.tar", last modified: Wed May 24 07:35:17 2023, max compression
+gzip compressed data, was "quao-0.1.4.tar", last modified: Wed May 24 09:03:48 2023, max compression
```

## Comparing `quao-0.1.3.tar` & `quao-0.1.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 07:35:17.896626 quao-0.1.3/
--rw-rw-rw-   0        0        0     1111 2023-04-27 03:39:26.000000 quao-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     2839 2023-05-24 07:35:17.895628 quao-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1163 2023-04-27 03:33:31.000000 quao-0.1.3/README.md
--rw-rw-rw-   0        0        0      811 2023-05-24 07:34:57.000000 quao-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-24 07:35:17.897625 quao-0.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-24 07:35:17.851624 quao-0.1.3/src/
-drwxrwxrwx   0        0        0        0 2023-05-24 07:35:17.863626 quao-0.1.3/src/quao/
--rw-rw-rw-   0        0        0      134 2023-04-25 02:47:26.000000 quao-0.1.3/src/quao/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-24 07:35:17.888623 quao-0.1.3/src/quao/algorithms/
--rw-rw-rw-   0        0        0        2 2023-04-25 02:47:26.000000 quao-0.1.3/src/quao/algorithms/__init__.py
--rw-rw-rw-   0        0        0     5305 2023-04-25 02:47:26.000000 quao-0.1.3/src/quao/algorithms/shor.py
--rw-rw-rw-   0        0        0     2207 2023-05-24 04:52:27.000000 quao-0.1.3/src/quao/backend.py
--rw-rw-rw-   0        0        0      366 2023-04-28 02:04:51.000000 quao-0.1.3/src/quao/dataUtils.py
-drwxrwxrwx   0        0        0        0 2023-05-24 07:35:17.889625 quao-0.1.3/src/quao/enum/
--rw-rw-rw-   0        0        0      200 2023-05-24 01:59:39.000000 quao-0.1.3/src/quao/enum/providerType.py
-drwxrwxrwx   0        0        0        0 2023-05-24 07:35:17.892628 quao-0.1.3/src/quao/sdk/
--rw-rw-rw-   0        0        0        2 2023-04-25 02:47:26.000000 quao-0.1.3/src/quao/sdk/__init__.py
--rw-rw-rw-   0        0        0     3654 2023-05-24 02:12:26.000000 quao-0.1.3/src/quao/sdk/qiskit.py
--rw-rw-rw-   0        0        0     1304 2023-05-24 05:04:40.000000 quao-0.1.3/src/quao/utilities.py
-drwxrwxrwx   0        0        0        0 2023-05-24 07:35:17.885675 quao-0.1.3/src/quao.egg-info/
--rw-rw-rw-   0        0        0     2839 2023-05-24 07:35:17.000000 quao-0.1.3/src/quao.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      414 2023-05-24 07:35:17.000000 quao-0.1.3/src/quao.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 07:35:17.000000 quao-0.1.3/src/quao.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      100 2023-05-24 07:35:17.000000 quao-0.1.3/src/quao.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-05-24 07:35:17.000000 quao-0.1.3/src/quao.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-24 09:03:48.951317 quao-0.1.4/
+-rw-rw-rw-   0        0        0     1111 2023-04-27 03:39:26.000000 quao-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     2839 2023-05-24 09:03:48.950280 quao-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1163 2023-04-27 03:33:31.000000 quao-0.1.4/README.md
+-rw-rw-rw-   0        0        0      846 2023-05-24 08:54:10.000000 quao-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-24 09:03:48.952274 quao-0.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-24 09:03:48.845321 quao-0.1.4/src/
+drwxrwxrwx   0        0        0        0 2023-05-24 09:03:48.876287 quao-0.1.4/src/quao/
+-rw-rw-rw-   0        0        0      134 2023-04-25 02:47:26.000000 quao-0.1.4/src/quao/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:03:48.934527 quao-0.1.4/src/quao/algorithms/
+-rw-rw-rw-   0        0        0        2 2023-04-25 02:47:26.000000 quao-0.1.4/src/quao/algorithms/__init__.py
+-rw-rw-rw-   0        0        0     5305 2023-04-25 02:47:26.000000 quao-0.1.4/src/quao/algorithms/shor.py
+-rw-rw-rw-   0        0        0     2207 2023-05-24 04:52:27.000000 quao-0.1.4/src/quao/backend.py
+-rw-rw-rw-   0        0        0      366 2023-04-28 02:04:51.000000 quao-0.1.4/src/quao/dataUtils.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:03:48.938284 quao-0.1.4/src/quao/enum/
+-rw-rw-rw-   0        0        0      200 2023-05-24 01:59:39.000000 quao-0.1.4/src/quao/enum/providerType.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:03:48.945279 quao-0.1.4/src/quao/sdk/
+-rw-rw-rw-   0        0        0        2 2023-04-25 02:47:26.000000 quao-0.1.4/src/quao/sdk/__init__.py
+-rw-rw-rw-   0        0        0     5057 2023-05-24 08:54:51.000000 quao-0.1.4/src/quao/sdk/qiskit.py
+-rw-rw-rw-   0        0        0     1304 2023-05-24 05:04:40.000000 quao-0.1.4/src/quao/utilities.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:03:48.928283 quao-0.1.4/src/quao.egg-info/
+-rw-rw-rw-   0        0        0     2839 2023-05-24 09:03:48.000000 quao-0.1.4/src/quao.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      414 2023-05-24 09:03:48.000000 quao-0.1.4/src/quao.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 09:03:48.000000 quao-0.1.4/src/quao.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      127 2023-05-24 09:03:48.000000 quao-0.1.4/src/quao.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-05-24 09:03:48.000000 quao-0.1.4/src/quao.egg-info/top_level.txt
```

### Comparing `quao-0.1.3/LICENSE` & `quao-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `quao-0.1.3/PKG-INFO` & `quao-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quao
-Version: 0.1.3
+Version: 0.1.4
 Summary: Quao Library supporting Quao Platform for Quantum Computing
 Author-email: "CITYNOW Co. Ltd. " <corp@citynow.vn>
 License: The MIT License (MIT)
         Copyright © CITYNOW Co. Ltd. All rights reserved.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `quao-0.1.3/README.md` & `quao-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `quao-0.1.3/pyproject.toml` & `quao-0.1.4/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "quao"
-version = "0.1.3"
+version = "0.1.4"
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
     "qiskit==0.43.0",
     "qiskit_ibm_runtime==0.10.0",
+    "qiskit-ibm-provider==0.6.0",
     "numpy>=1.22.3",
 ]
 requires-python = ">=3.7"
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
```

### Comparing `quao-0.1.3/src/quao/algorithms/shor.py` & `quao-0.1.4/src/quao/algorithms/shor.py`

 * *Files identical despite different names*

### Comparing `quao-0.1.3/src/quao/backend.py` & `quao-0.1.4/src/quao/backend.py`

 * *Files identical despite different names*

### Comparing `quao-0.1.3/src/quao/sdk/qiskit.py` & `quao-0.1.4/src/quao/sdk/qiskit.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from qiskit import transpile
 from qiskit_aer import Aer
 from qiskit_ibm_runtime import QiskitRuntimeService, Options, Session, Sampler
+from qiskit_ibm_provider import IBMProvider
 import json
 
 from ..utilities import JobResponse
 from ..enum.providerType import ProviderType
 
 
 class QiskitFaaS:
@@ -15,42 +16,44 @@
         self.connection = backend_data.get("authentication")
 
     def get_aer_backend(self):
         return Aer.get_backend(self.device_name)
 
     def get_ibm_provider(self, channel):
         token = self.connection.get("token")
-        instance = self.connection.get("crn")
+        if channel == "ibm_cloud":
+            instance = self.connection.get("crn")
+            return QiskitRuntimeService(channel=channel, token=token, instance=instance)
+        elif channel == "ibm_quantum":
+            return IBMProvider(token=token)
 
-        return QiskitRuntimeService(channel=channel, token=token, instance=instance)
-
-    def run_circuit_on_ibm(self, provider, circuit, shots):
+    def run_circuit_on_ibm_cloud(self, provider, circuit, shots):
         options = Options(optimization_level=1)
         options.execution.shots = shots
 
         with Session(service=provider, backend=self.device_name) as session:
             sampler = Sampler(session=session, options=options)
             job = sampler.run(circuits=circuit)
 
             return job
 
     def is_simulator(self, provider):
         backend = provider.get_backend(self.device_name)
         return backend.configuration().simulator
 
-    def run_ibm_job(self, channel, circuit, shots) -> JobResponse:
+    def run_ibm_cloud_job(self, channel, circuit, shots) -> JobResponse:
         provider_job_id = ''
         try:
             provider = self.get_ibm_provider(channel=channel)
-            job = self.run_circuit_on_ibm(provider=provider, circuit=circuit, shots=shots)
+            job = self.run_circuit_on_ibm_cloud(provider=provider, circuit=circuit, shots=shots)
             provider_job_id = job.job_id()
             job_status = job.status().name
             job_result = {}
             if self.is_simulator(provider) or job_status == "DONE":
-                job_result = job.result().to_dict()
+                job_result = job.result().__dict__
                 job_status = job.status().name
 
         except Exception as exception:
             job_result = {
                 "error": "Exception when invoke job on " + channel + " provider",
                 "exception": str(exception)
             }
@@ -58,14 +61,45 @@
 
         return JobResponse(
             provider_job_id=provider_job_id,
             job_status=job_status,
             job_result=json.dumps(job_result)
         )
 
+    def run_circuit_on_ibm_quantum(self, provider, circuit, shots):
+        backend = provider.get_backend(self.device_name)
+        transpile_circuit = transpile(circuit, backend)
+
+        return backend.run(transpile_circuit, shots=shots)
+
+    def run_ibm_quantum_job(self, circuit, shots) -> JobResponse:
+        provider_job_id = ''
+        try:
+            provider = self.get_ibm_provider('ibm_quantum')
+            job = self.run_circuit_on_ibm_quantum(provider=provider, circuit=circuit, shots=shots)
+            provider_job_id = job.job_id()
+            job_status = job.status().name
+            job_result = {}
+            if self.is_simulator(provider) or job_status == "DONE":
+                job_result = job.result().to_dict()
+                job_status = job.status().name
+
+        except Exception as exception:
+            job_result = {
+                "error": "Exception when invoke job on IBM Quantum provider",
+                "exception": str(exception)
+            }
+            job_status = "ERROR"
+
+        return JobResponse(
+            provider_job_id=provider_job_id,
+            job_status=job_status,
+            job_result=json.dumps(job_result)
+        )
+
     def submit_job(self, qcircuit, shots) -> JobResponse:
         if self.provider_tag == ProviderType.QUAO_QUANTUM_SIMULATOR.value:
             try:
                 backend = self.get_aer_backend()
                 transpile_circuit = transpile(qcircuit, backend)
 
                 job = backend.run(transpile_circuit, shots=shots)
@@ -79,15 +113,15 @@
                 job_status = "ERROR"
             return JobResponse(
                 provider_job_id="Internal-Qiskit-Simulation-Job",
                 job_status=job_status,
                 job_result=json.dumps(job_result),
             )
         elif self.provider_tag == ProviderType.IBM_QUANTUM.value:
-            return self.run_ibm_job(channel="ibm_quantum", circuit=qcircuit, shots=shots)
+            return self.run_ibm_quantum_job(circuit=qcircuit, shots=shots)
         elif self.provider_tag == ProviderType.IBM_CLOUD.value:
-            return self.run_ibm_job(channel="ibm_cloud", circuit=qcircuit, shots=shots)
+            return self.run_ibm_cloud_job(channel="ibm_cloud", circuit=qcircuit, shots=shots)
 
         return JobResponse(
             job_status="ERROR",
             job_result=json.dumps({"error": "Provider not supported"})
         )
```

### Comparing `quao-0.1.3/src/quao/utilities.py` & `quao-0.1.4/src/quao/utilities.py`

 * *Files identical despite different names*

### Comparing `quao-0.1.3/src/quao.egg-info/PKG-INFO` & `quao-0.1.4/src/quao.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quao
-Version: 0.1.3
+Version: 0.1.4
 Summary: Quao Library supporting Quao Platform for Quantum Computing
 Author-email: "CITYNOW Co. Ltd. " <corp@citynow.vn>
 License: The MIT License (MIT)
         Copyright © CITYNOW Co. Ltd. All rights reserved.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

