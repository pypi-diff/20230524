# Comparing `tmp/bluequbit-0.1.0b9.tar.gz` & `tmp/bluequbit-0.1.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/bluequbit-python-sdk/bluequbit-python-sdk/dist/.tmp-44vgbqfe/bluequbit-0.1.0b9.tar", last modified: Fri Mar 10 08:47:13 2023, max compression
+gzip compressed data, was "bluequbit-0.1.2b1.tar", last modified: Wed May 24 05:45:11 2023, max compression
```

## Comparing `bluequbit-0.1.0b9.tar` & `bluequbit-0.1.2b1.tar`

### file list

```diff
@@ -1,42 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 08:47:12.000000 bluequbit-0.1.0b9/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-10 08:46:57.000000 bluequbit-0.1.0b9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-10 08:46:57.000000 bluequbit-0.1.0b9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-03-10 08:47:12.000000 bluequbit-0.1.0b9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-03-10 08:46:57.000000 bluequbit-0.1.0b9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 08:47:12.000000 bluequbit-0.1.0b9/bluequbit/
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-03-10 08:46:57.000000 bluequbit-0.1.0b9/bluequbit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 08:47:12.000000 bluequbit-0.1.0b9/bluequbit/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 08:46:57.000000 bluequbit-0.1.0b9/bluequbit/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-03-10 08:46:57.000000 bluequbit-0.1.0b9/bluequbit/api/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-03-10 08:46:57.000000 bluequbit-0.1.0b9/bluequbit/backend_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-03-10 08:46:57.000000 bluequbit-0.1.0b9/bluequbit/bluequbit_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-03-10 08:46:57.000000 bluequbit-0.1.0b9/bluequbit/circuit_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-03-10 08:46:57.000000 bluequbit-0.1.0b9/bluequbit/estimate_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-03-10 08:46:57.000000 bluequbit-0.1.0b9/bluequbit/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-03-10 08:46:57.000000 bluequbit-0.1.0b9/bluequbit/http_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5461 2023-03-10 08:46:57.000000 bluequbit-0.1.0b9/bluequbit/job_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-03-10 08:46:57.000000 bluequbit-0.1.0b9/bluequbit/job_run_statuses.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-10 08:46:57.000000 bluequbit-0.1.0b9/bluequbit/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 08:47:12.000000 bluequbit-0.1.0b9/bluequbit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-03-10 08:47:12.000000 bluequbit-0.1.0b9/bluequbit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-03-10 08:47:12.000000 bluequbit-0.1.0b9/bluequbit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 08:47:12.000000 bluequbit-0.1.0b9/bluequbit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-10 08:47:12.000000 bluequbit-0.1.0b9/bluequbit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-10 08:47:12.000000 bluequbit-0.1.0b9/bluequbit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-03-10 08:46:57.000000 bluequbit-0.1.0b9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-10 08:46:57.000000 bluequbit-0.1.0b9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-10 08:47:12.000000 bluequbit-0.1.0b9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-03-10 08:46:57.000000 bluequbit-0.1.0b9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 08:47:12.000000 bluequbit-0.1.0b9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-03-10 08:46:57.000000 bluequbit-0.1.0b9/tests/test_basic_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-03-10 08:46:57.000000 bluequbit-0.1.0b9/tests/test_basic_large_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-03-10 08:46:57.000000 bluequbit-0.1.0b9/tests/test_cancel_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-03-10 08:46:57.000000 bluequbit-0.1.0b9/tests/test_circuit_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-03-10 08:46:57.000000 bluequbit-0.1.0b9/tests/test_get_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-03-10 08:46:57.000000 bluequbit-0.1.0b9/tests/test_gpu_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-03-10 08:46:57.000000 bluequbit-0.1.0b9/tests/test_job_estimate.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-03-10 08:46:57.000000 bluequbit-0.1.0b9/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-03-10 08:46:57.000000 bluequbit-0.1.0b9/tests/test_ok.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-03-10 08:46:57.000000 bluequbit-0.1.0b9/tests/test_quantum_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-03-10 08:46:57.000000 bluequbit-0.1.0b9/tests/test_stress_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-03-10 08:46:57.000000 bluequbit-0.1.0b9/tests/test_very_large_job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 05:45:11.254816 bluequbit-0.1.2b1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-24 05:45:11.254816 bluequbit-0.1.2b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 05:45:11.246816 bluequbit-0.1.2b1/bluequbit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/bluequbit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 05:45:11.250816 bluequbit-0.1.2b1/bluequbit/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/bluequbit/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/bluequbit/api/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/bluequbit/backend_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10137 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/bluequbit/bluequbit_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/bluequbit/check_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/bluequbit/circuit_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/bluequbit/estimate_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/bluequbit/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/bluequbit/http_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/bluequbit/job_metadata_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/bluequbit/job_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/bluequbit/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 05:45:11.246816 bluequbit-0.1.2b1/bluequbit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-24 05:45:11.000000 bluequbit-0.1.2b1/bluequbit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-24 05:45:11.000000 bluequbit-0.1.2b1/bluequbit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 05:45:11.000000 bluequbit-0.1.2b1/bluequbit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-24 05:45:11.000000 bluequbit-0.1.2b1/bluequbit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-24 05:45:11.000000 bluequbit-0.1.2b1/bluequbit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 05:45:11.254816 bluequbit-0.1.2b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 05:45:11.254816 bluequbit-0.1.2b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/tests/test_basic_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/tests/test_basic_large_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/tests/test_batch_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/tests/test_cancel_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/tests/test_circuit_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/tests/test_count_wrong.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/tests/test_get_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/tests/test_gpu_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/tests/test_job_estimate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/tests/test_ok.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/tests/test_quantum_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/tests/test_stress_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/tests/test_very_large_job.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `bluequbit-0.1.0b9/LICENSE` & `bluequbit-0.1.2b1/LICENSE`

 * *Files identical despite different names*

### Comparing `bluequbit-0.1.0b9/PKG-INFO` & `bluequbit-0.1.2b1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluequbit
-Version: 0.1.0b9
+Version: 0.1.2b1
 Summary: Python SDK to BlueQubit app
 Author: BlueQubit
 Author-email: hovnatan@bluequbit.io
 License: Apache 2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -34,14 +34,16 @@
 
     job_result = bq_client.run(qc_qiskit, job_name="testing_1")
 
     state_vector = job_result.get_statevector() 
     # returns a NumPy array of [0. +0.j 0. +0.j 0.70710677+0.j 0.70710677+0.j]
 ```
 
+The packages is tested extensively on Python 3.8.
+
 ## Full reference
 
 Please find detailed reference at https://app.bluequbit.io/sdk-docs.
 
 ## Questions and Issues
 
 Please submit questions and issues to info@bluequbit.io.
```

### Comparing `bluequbit-0.1.0b9/README.md` & `bluequbit-0.1.2b1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 
     job_result = bq_client.run(qc_qiskit, job_name="testing_1")
 
     state_vector = job_result.get_statevector() 
     # returns a NumPy array of [0. +0.j 0. +0.j 0.70710677+0.j 0.70710677+0.j]
 ```
 
+The packages is tested extensively on Python 3.8.
+
 ## Full reference
 
 Please find detailed reference at https://app.bluequbit.io/sdk-docs.
 
 ## Questions and Issues
 
 Please submit questions and issues to info@bluequbit.io.
```

### Comparing `bluequbit-0.1.0b9/bluequbit/__init__.py` & `bluequbit-0.1.2b1/bluequbit/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Mypy; for the `|` operator purpose
 # Remove this __future__ import once the oldest supported Python is 3.10
 from __future__ import annotations
 
 import logging
 
 from . import exceptions  # noqa: F401
+from . import job_metadata_constants  # noqa: F401
 from .bluequbit_client import BQClient
 from .estimate_result import EstimateResult  # noqa: F401
 from .job_result import JobResult  # noqa: F401
 from .version import __version__  # noqa: F401
 
 formatter = logging.Formatter(fmt="BQ-PYTHON-SDK - %(levelname)s - %(message)s")
 # formatter = logging.Formatter(fmt='%(asctime)s - %(levelname)s - %(module)s - %(message)s')
@@ -17,16 +18,18 @@
 handler.setFormatter(formatter)
 
 logger = logging.getLogger("bluequbit-python-sdk")
 logger.setLevel(logging.INFO)
 logger.addHandler(handler)
 
 
-def init(api_token: str | None = None) -> BQClient:
+def init(api_token: str | None = None, update_config_file: bool = True) -> BQClient:
     """Returns :class:`BQClient` instance for managing jobs on BlueQubit platform.
 
     :param api_token: API token of the user. If ``None``, the token will be looked
                       in default configuration file ``$HOME/.config/bluequbit/config.json``.
                       If not ``None``, the token will also be saved in the same
                       default configuration file.
+    :param update_config_file: if True, update default configuration file
+                               if api_token is not None.
     """
-    return BQClient(api_token)
+    return BQClient(api_token, update_config_file)
```

### Comparing `bluequbit-0.1.0b9/bluequbit/api/jobs.py` & `bluequbit-0.1.2b1/bluequbit/api/jobs.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,61 @@
 import datetime
+import json
 import logging
+import zlib
 
 import dateutil.parser
 
 from ..circuit_serialization import encode_circuit
-from ..exceptions import BQBaseError
+from ..exceptions import BQAPIError, BQError
 
 logger = logging.getLogger("bluequbit-python-sdk")
 
 _SINGLE_REQUEST_LIMIT = 100
 
 
-def search_jobs(_connection, run_status=None, created_later_than=None):
+def search_jobs(
+    _connection, run_status=None, created_later_than=None, job_ids=None, batch_id=None
+):
     if created_later_than is None:
         parsed_created_later_than = None
     elif isinstance(created_later_than, str):
         parsed_created_later_than = dateutil.parser.parse(created_later_than)
         if parsed_created_later_than.tzinfo is None:
             logger.warning(
-                "created_later_than is a str object without timezone info, assuming UTC timezone"
+                "created_later_than is a str object without timezone info, assuming UTC"
+                " timezone"
             )
             parsed_created_later_than = parsed_created_later_than.replace(
                 tzinfo=datetime.timezone.utc
             )
         parsed_created_later_than = parsed_created_later_than.isoformat()
     elif isinstance(created_later_than, datetime.datetime):
         if created_later_than.tzinfo is None:
-            raise BQBaseError(
-                0, "created_later_than is a datetime object without timezone info"
+            raise BQError(
+                "created_later_than is a datetime object without timezone info"
             )
         parsed_created_later_than = created_later_than.isoformat()
     else:
-        raise BQBaseError(
-            0, "created_later_than should be None, str, or datetime.datetime object"
+        raise BQError(
+            "created_later_than should be None, str, or datetime.datetime object"
         )
 
     params = {
         "limit": _SINGLE_REQUEST_LIMIT,
         "run_status": run_status,
         "created_later_than": parsed_created_later_than,
+        "job_ids": job_ids,
+        "batch_id": batch_id,
     }
     result_dict = {"data": []}
     while True:
         response = _connection.send_request(req_type="GET", path="/jobs", params=params)
         if not response.ok:
-            raise BQBaseError(
+            raise BQAPIError(
                 response.status_code, "Couldn't search jobs " + response.text
             )
         response = response.json()
 
         results = response["data"]
         result_dict["data"] += results
         result_dict["total_count"] = response["total_count"]
@@ -56,35 +63,50 @@
         if len(results) < _SINGLE_REQUEST_LIMIT:
             break
 
         params["offset"] = len(result_dict["data"])
     return result_dict
 
 
-def submit_job(_connection, circuit, device, job_name=None, estimate_only=False):
-    encoded_circuit = encode_circuit(circuit)
+def submit_jobs(
+    _connection,
+    circuits,
+    device,
+    job_name=None,
+    estimate_only=False,
+    shots=None,
+    asynchronous=False,
+):
+    if isinstance(circuits, list):
+        encoded_circuits = [encode_circuit(circuit) for circuit in circuits]
+    else:
+        encoded_circuits = encode_circuit(circuits)
+
     params = {
         "estimate_only": estimate_only,
-        "circuit": encoded_circuit,
+        "circuit": encoded_circuits,
         "job_name": job_name,
         "device": device,
+        "shots": shots,
+        "asynchronous": asynchronous,
     }
-    response = _connection.send_request(req_type="POST", path="/jobs", json_req=params)
-    if not response.ok:
-        raise BQBaseError(response.status_code, "Couldn't submit job " + response.text)
-    return response.json()["data"]
-
-
-def cancel_job(_connection, job_id):
+    data = json.dumps(params)
+    if len(data) > 2000:
+        data = zlib.compress(data.encode())
+        headers = {"content-encoding": "gzip"}
+    else:
+        headers = {"content-type": "application/json"}
     response = _connection.send_request(
-        req_type="PATCH", path=f"/jobs/{job_id}", json_req={"cancel": True}
+        req_type="POST", path="/jobs", data=data, headers=headers
     )
     if not response.ok:
-        raise BQBaseError(response.status_code, "Couldn't cancel job " + response.text)
+        raise BQAPIError(response.status_code, "Couldn't submit jobs " + response.text)
     return response.json()["data"]
 
 
-def get(_connection, job_id):
-    response = _connection.send_request(req_type="GET", path=f"/jobs/{job_id}")
+def cancel_jobs(_connection, job_ids):
+    response = _connection.send_request(
+        req_type="PATCH", path="/jobs", json_req={"job_ids": job_ids, "cancel": True}
+    )
     if not response.ok:
-        raise BQBaseError(response.status_code, "Couldn't get job " + response.text)
+        raise BQAPIError(response.status_code, "Couldn't cancel jobs " + response.text)
     return response.json()["data"]
```

### Comparing `bluequbit-0.1.0b9/bluequbit/backend_connection.py` & `bluequbit-0.1.2b1/bluequbit/backend_connection.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,20 @@
 import json
 import logging
-import os
 from pathlib import Path
 
-import requests
-import requests_toolbelt
-import urllib3
-
-from .exceptions import BQBaseError, BQUnauthorizedError
-from .http_adapter import TimeoutHTTPAdapter
+from .exceptions import BQAPIError, BQError, BQUnauthorizedAccessError
+from .http_utils import request_retriable
 from .version import __version__
 
 logger = logging.getLogger("bluequbit-python-sdk")
 
 
 class BackendConnection:
-    def __init__(self, api_token=None):
+    def __init__(self, api_token=None, update_config_file=True):
         config_dir = Path.home() / ".config" / "bluequbit"
         config_location = config_dir / "config.json"
 
         main_endpoint_from_config_file = None
         token_from_config_file = None
         ssl_verify_from_config_file = None
 
@@ -28,118 +23,128 @@
                 config = json.load(f)
             main_endpoint_from_config_file = config.get("main_endpoint")
             token_from_config_file = config.get("token")
             ssl_verify_from_config_file = config.get("ssl_verify")
 
         if api_token is None:
             if token_from_config_file is None:
-                raise BQBaseError(
-                    0,
-                    f"Please specify an API key to init() (or have config written in {config_location}). You can find your API key once you log in to https://app.bluequbit.io",
+                raise BQError(
+                    (
+                        "Please specify an API key to init() (or have config written"
+                        f" in {config_location}).You can find your API key once you log"
+                        " in to https://app.bluequbit.io"
+                    ),
                 )
-            else:
-                api_token = token_from_config_file
+            api_token = token_from_config_file
 
         self._api_config = {
             "token": api_token,
-            "main_endpoint": "https://app.bluequbit.io/api/v1"
-            if main_endpoint_from_config_file is None
-            else main_endpoint_from_config_file,
-            "ssl_verify": True
-            if ssl_verify_from_config_file is None
-            else ssl_verify_from_config_file,
+            "main_endpoint": (
+                "https://app.bluequbit.io/api/v1"
+                if main_endpoint_from_config_file is None
+                else main_endpoint_from_config_file
+            ),
+            "ssl_verify": (
+                True
+                if ssl_verify_from_config_file is None
+                else ssl_verify_from_config_file
+            ),
         }
 
-        if api_token is not None and api_token != token_from_config_file:
+        if (
+            api_token is not None
+            and api_token != token_from_config_file
+            and update_config_file
+        ):
             config_dir.mkdir(exist_ok=True, parents=True)
             self.update_config_file(self._api_config, config_location)
 
         try:
             self._token = self._api_config["token"]
         except KeyError:
-            raise BQBaseError(
-                0,
-                "Incorrect config file: 'token' key is not present in the config file "
-                + str(config_location),
+            raise BQError(
+                (
+                    "Incorrect config file: 'token' key is not present in the config"
+                    f" file {config_location}."
+                ),
             ) from None
 
-        try:
-            self._default_headers = {"Authorization": f"SDK {self._token}"}
-            self._default_headers["User-Agent"] = requests_toolbelt.user_agent(
-                "bluequbit", __version__
-            )
+        self._default_headers = {
+            "Authorization": f"SDK {self._token}",
+            "Connection": "close",
+            "User-Agent": f"BlueQubit SDK {__version__}",
+        }
 
-            self._main_endpoint = "https://app.bluequbit.io/api/v1"
-            if "main_endpoint" in self._api_config:
-                self._main_endpoint = self._api_config["main_endpoint"]
-            self._verify = True
-            if "ssl_verify" in self._api_config:
-                self._verify = self._api_config["ssl_verify"]
-            self._session = None
+        self._main_endpoint = "https://app.bluequbit.io/api/v1"
+        if (
+            "main_endpoint" in self._api_config
+            and self._main_endpoint != self._api_config["main_endpoint"]
+        ):
+            self._main_endpoint = self._api_config["main_endpoint"]
+            logger.warning("Using custom endpoint %s", self._main_endpoint)
+        self._verify = True
+        if "ssl_verify" in self._api_config:
+            self._verify = self._api_config["ssl_verify"]
+        self._session = None
+        self._authenticated = False
+        response = self.send_request(
+            req_type="GET",
+            path="/jobs",
+            params={"limit": 1},
+            authentication_request=True,
+        )
+
+        if response.ok:
             self._authenticated = True
-            response = self.send_request(
-                req_type="GET",
-                path="/jobs",
-                params={"limit": 1},
+        elif response.status_code == 401:
+            raise BQUnauthorizedAccessError
+        else:
+            raise BQAPIError(
+                response.status_code, f"Couldn't reach BlueQubit {response.text}."
             )
-            if not self._verify:
-                urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
-
-            if not response.ok:
-                self._authenticated = False
-                self._session = None
-                if response.status_code == 401:
-                    raise BQUnauthorizedError()
-                raise BQBaseError(0, "Couldn't reach BlueQubit " + response.text)
-        except:
-            self._authenticated = False
-            self._session = None
-            raise
 
     @staticmethod
     def update_config_file(content, config_location):
         with config_location.open("w", encoding="utf-8") as f:
             json.dump(content, f, indent=4)
         logger.info("Configuration file %s successfully updated.", config_location)
 
-    def send_request(self, req_type, path, params=None, json_req=None):
-        if not self._authenticated:
-            raise BQBaseError(
-                0,
-                "BQClient was not initialized. Please provide correct API token to BQClient(<token>).",
+    def send_request(
+        self,
+        req_type,
+        path,
+        params=None,
+        data=None,
+        json_req=None,
+        headers=None,
+        authentication_request=False,
+    ):
+        if not authentication_request and not self._authenticated:
+            raise BQError(
+                (
+                    "BQClient was not initialized. Please provide correct API token to"
+                    " BQClient(<token>)."
+                ),
             )
         url = self._main_endpoint + path
 
         if params is not None:
             for key, value in params.items():
                 if isinstance(value, str):
                     params[key] = value.replace("\\", "\\\\")
+                if isinstance(value, list):
+                    params[key] = ",".join(value)
 
-        req = requests.Request(method=req_type, url=url, json=json_req, params=params)
-        if self._session is None:
-            self._session = self._create_session()
-        prepared = self._session.prepare_request(req)
-        resp = self._session.send(request=prepared, verify=self._verify)
+        if headers is None:
+            headers_to_send = self._default_headers
+        else:
+            headers_to_send = dict(self._default_headers, **headers)
+
+        resp = request_retriable(
+            method=req_type,
+            url=url,
+            data=data,
+            json=json_req,
+            params=params,
+            headers=headers_to_send,
+        )
         return resp
-
-    def _create_session(self):
-        session = requests.Session()
-        adapter = TimeoutHTTPAdapter()
-        session.mount("https://", adapter)
-        session.mount("http://", adapter)
-        session.headers = self._default_headers
-
-        if "BLUEQUBIT_DEBUG" in os.environ:
-            session.hooks["response"].append(_log_requests)
-
-        return session
-
-
-if "BLUEQUBIT_DEBUG" in os.environ:
-    from requests_toolbelt.utils import dump
-
-    def _log_requests(response, *args, **kwargs):
-        data = dump.dump_all(response)
-        _log_requests.response_len += len(data)
-        logger.info("HTTP %s %s ", response.request.url, _log_requests.response_len)
-
-    _log_requests.response_len = 0
```

### Comparing `bluequbit-0.1.0b9/bluequbit/circuit_serialization.py` & `bluequbit-0.1.2b1/bluequbit/circuit_serialization.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,43 @@
 import base64
 import io
 
 
-def encode_circuit(qc):
+def cirq_to_qasm2(circuit):
+    import cirq
+    from cirq import ops
+
+    qubit_order = ops.QubitOrder.DEFAULT
+    qubits = ops.QubitOrder.as_qubit_order(qubit_order).order_for(circuit.all_qubits())
+    serialized = cirq.QasmOutput(
+        operations=circuit.all_operations(),
+        qubits=qubits,
+        header="Generated from Cirq via BlueQubit",
+        precision=10,
+        version="2.0",
+    )
+    return str(serialized)
+
+
+def encode_circuit(qc, use_cirq_qasm=False):
     """
     Encode a quantum circuit object from various quantum libraries to a
     portable format.
     """
     # We use the string representation of the object class so that we don't
     # have to require users to install Qiskit, Cirq, and Braket all at once.
     circuit_type = str(type(qc))
     if circuit_type == "<class 'cirq.circuits.circuit.Circuit'>":
+        if use_cirq_qasm:
+            # We serialize to OQ2 string
+            # https://quantumai.google/reference/python/cirq/QasmOutput
+            serialized = cirq_to_qasm2(qc)
+            return {"circuit_type": "Cirq_OQ2", "circuit": serialized}
+
+        # We use Cirq-specific serialization method.
         import cirq
 
         # https://quantumai.google/cirq/build/interop
         serialized = cirq.to_json(qc)
         return {"circuit_type": "Cirq", "circuit": serialized}
     elif circuit_type == "<class 'braket.circuits.circuit.Circuit'>":
         from braket.circuits.serialization import IRType
@@ -48,14 +71,18 @@
     if "circuit" not in data:
         raise Exception("Wrong data structure. 'circuit' must be present.")
     circuit_type = data["circuit_type"]
     if circuit_type == "Cirq":
         import cirq
 
         return cirq.read_json(json_text=data["circuit"])
+    elif circuit_type == "Cirq_OQ2":
+        from cirq.contrib.qasm_import import circuit_from_qasm
+
+        return circuit_from_qasm(data["circuit"])
     elif circuit_type == "Qiskit":
         from qiskit import qpy
 
         _bytes = str.encode(data["circuit"])
         _bytes = base64.b64decode(_bytes)
         with io.BytesIO(_bytes) as f:
             circuits = qpy.load(f)
```

### Comparing `bluequbit-0.1.0b9/bluequbit/estimate_result.py` & `bluequbit-0.1.2b1/bluequbit/estimate_result.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-class EstimateResult:
+class EstimateResult:  # pylint: disable=too-few-public-methods
     """This class contains information about the estimated runtime/cost that
     will be incurred from running the given circuit on the given quantum
     machine/simulator. `WARNING:` this is just an estimate, the actual runtime/cost
     may be less or more."""
 
     def __init__(self, data):
         self.device = data.get("device")
@@ -23,8 +23,11 @@
 
         #: str: error message if available
         self.error_message = data.get("error_message")
 
     def __repr__(self):
         if self.error_message is not None:
             return f"Estimation failed due to error: {self.error_message}."
-        return f"Estimated: runtime: {self.estimated_runtime} ms, cost: ${self.estimated_cost:.2f}. {self.warning_message}"
+        return (
+            f"Estimated: runtime: {self.estimated_runtime} ms, cost:"
+            f" ${self.estimated_cost:.2f}. {self.warning_message}"
+        )
```

### Comparing `bluequbit-0.1.0b9/bluequbit/job_result.py` & `bluequbit-0.1.2b1/bluequbit/job_result.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,40 @@
 import datetime
 from io import BytesIO
 from typing import Dict, Optional
 
 import numpy as np
 from dateutil.parser import parse
 
-from .exceptions import BQStatevectorTooLargeError
-from .http_adapter import HTTP_SESSION_WITH_TIMEOUT_AND_RETRY
+from . import job_metadata_constants
+from .exceptions import (
+    BQJobDoesNotContainCountsError,
+    BQJobHasNotFinishedYetError,
+    BQJobNotCompleteError,
+    BQJobStatevectorTooLargeError,
+)
+from .http_utils import request_retriable
 
 
 class JobResult:
     """This class contains information from a job run on quantum hardware or
     quantum simulators. Mainly it contains the resulting statevector from the
     run. It might contain only partial information, such as job ID,
     when :func:`BQClient.run` is called with ``asynchronous=True``."""
 
     def __init__(self, data):
         #: str: job id
         self.job_id = data.get("job_id")
 
-        #: str: job run status, can be one of ``"FAILED_VALIDATION"`` | ``"PENDING"`` | ``"QUEUED"`` | ``"RUNNING"`` | ``"TERMINATED"`` | ``"CANCELED"`` | ``"NOT_ENOUGH_FUNDS"`` | ``"COMPLETED"``
+        #: str: batch id
+        self.batch_id = data.get("batch_id")
+
+        #: str: job run status, can be one of ``"FAILED_VALIDATION"`` | ``"PENDING"`` |
+        #       ``"QUEUED"`` | ``"RUNNING"`` | ``"TERMINATED"`` | ``"CANCELED"`` |
+        #       ``"NOT_ENOUGH_FUNDS"`` | ``"COMPLETED"``
         self.run_status = data.get("run_status")
 
         #: str: job name
         self.job_name = data.get("job_name")
 
         #: str: run device
         self.device = data.get("device")
@@ -72,73 +83,81 @@
         self.error_message = data.get("error_message")
 
         #: float: job cost in US dollars
         self.cost = data.get("cost")
         if self.cost is not None:
             self.cost /= 100.0
         self._metadata = None
+
+        #: bool: if statevector available
+        self.has_statevector = data.get("has_statevector")
+
         self._statevector = None
 
     def get_statevector(self) -> np.array:
         """Return statevector of the job. If the statevector is too large then throws exception.
 
         :rtype: NumPy array
         """
+        if self.run_status in job_metadata_constants.JOB_NON_TERMINAL_STATES:
+            raise BQJobHasNotFinishedYetError(self.job_id, self.run_status)
+        elif not self.ok:
+            raise BQJobNotCompleteError(
+                self.job_id, self.run_status, self.error_message
+            )
+        elif self.has_statevector is False:
+            raise BQJobStatevectorTooLargeError(self.job_id, self.num_qubits)
 
         if self._statevector is None:
-            response = HTTP_SESSION_WITH_TIMEOUT_AND_RETRY.get(
-                self._results_path + "statevector.txt"
-            )
-            if response.ok:
-                data = response.content
-                self._statevector = np.loadtxt(BytesIO(data), dtype=np.complex_)
-        if self._statevector is not None:
-            return self._statevector
-        else:
-            raise BQStatevectorTooLargeError(self.num_qubits)
+            response = request_retriable("GET", self._results_path + "statevector.txt")
+            self._statevector = np.loadtxt(BytesIO(response.content), dtype=np.complex_)
+        return self._statevector
 
     def get_counts(self) -> Optional[Dict[str, float]]:
         """
         "counts" is the measurement probabilities of the computation result,
         without any statistical fluctuation. It is equivalent to what you would
         get from a Qiskit result if you do `get_counts` on it from a Qiskit
         simulation with 0 shot.
         """
         if self._metadata is None:
-            response = HTTP_SESSION_WITH_TIMEOUT_AND_RETRY.get(
-                self._results_path + "metadata.json"
-            )
+            response = request_retriable("GET", self._results_path + "metadata.json")
             self._metadata = response.json()
         if "counts" not in self._metadata:
-            raise RuntimeError("The job result metadata doesn't contain counts.")
+            raise BQJobDoesNotContainCountsError(self.job_id)
         return self._metadata["counts"]
 
     @property
-    def ok(self) -> bool:
+    def ok(self) -> bool:  # pylint: disable=invalid-name
         """``True``, if job's current run status is ``"COMPLETED"``,
         else ``False``."""
 
         return self.run_status == "COMPLETED"
 
     def __repr__(self):
-        repr = f"Job ID: {self.job_id}"
+        jr_repr = f"Job ID: {self.job_id}"
+        if self.batch_id is not None:
+            jr_repr += f" (batch ID: {self.batch_id})"
         if self.job_name is not None:
-            repr += f", name: {self.job_name}"
-        repr += f", device: {self.device}"
-        repr += f", run status: {self.run_status}, created on: {self.created_on.replace(microsecond=0, tzinfo=None)} UTC"
+            jr_repr += f", name: {self.job_name}"
+        jr_repr += f", device: {self.device}"
+        jr_repr += f", run status: {self.run_status}"
+        jr_repr += (
+            f", created on: {self.created_on.replace(microsecond=0, tzinfo=None)} UTC"
+        )
         if (
             self.run_status in ["PENDING", "QUEUED", "RUNNING"]
             and self.estimated_runtime is not None
         ):
-            repr += f", estimated runtime: {self.estimated_runtime} ms"
-            repr += f", estimated cost: ${self.estimated_cost:.2f}"
+            jr_repr += f", estimated runtime: {self.estimated_runtime} ms"
+            jr_repr += f", estimated cost: ${self.estimated_cost:.2f}"
         if self.cost is not None:
-            repr += f", cost: ${self.cost:.2f}"
+            jr_repr += f", cost: ${self.cost:.2f}"
         if self.run_time_ms is not None:
-            repr += f", run time: {self.run_time_ms} ms"
+            jr_repr += f", run time: {self.run_time_ms} ms"
         if self.queue_time_ms is not None:
-            repr += f", queue time: {self.queue_time_ms} ms"
+            jr_repr += f", queue time: {self.queue_time_ms} ms"
         if self.num_qubits is not None:
-            repr += f", num qubits: {self.num_qubits}"
+            jr_repr += f", num qubits: {self.num_qubits}"
         if self.error_message is not None:
-            repr += f", error_message: {self.error_message}"
-        return repr
+            jr_repr += f", error_message: {self.error_message}"
+        return jr_repr
```

### Comparing `bluequbit-0.1.0b9/bluequbit.egg-info/PKG-INFO` & `bluequbit-0.1.2b1/bluequbit.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluequbit
-Version: 0.1.0b9
+Version: 0.1.2b1
 Summary: Python SDK to BlueQubit app
 Author: BlueQubit
 Author-email: hovnatan@bluequbit.io
 License: Apache 2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -34,14 +34,16 @@
 
     job_result = bq_client.run(qc_qiskit, job_name="testing_1")
 
     state_vector = job_result.get_statevector() 
     # returns a NumPy array of [0. +0.j 0. +0.j 0.70710677+0.j 0.70710677+0.j]
 ```
 
+The packages is tested extensively on Python 3.8.
+
 ## Full reference
 
 Please find detailed reference at https://app.bluequbit.io/sdk-docs.
 
 ## Questions and Issues
 
 Please submit questions and issues to info@bluequbit.io.
```

### Comparing `bluequbit-0.1.0b9/bluequbit.egg-info/SOURCES.txt` & `bluequbit-0.1.2b1/bluequbit.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -3,32 +3,35 @@
 README.md
 pyproject.toml
 requirements.txt
 setup.py
 bluequbit/__init__.py
 bluequbit/backend_connection.py
 bluequbit/bluequbit_client.py
+bluequbit/check_version.py
 bluequbit/circuit_serialization.py
 bluequbit/estimate_result.py
 bluequbit/exceptions.py
-bluequbit/http_adapter.py
+bluequbit/http_utils.py
+bluequbit/job_metadata_constants.py
 bluequbit/job_result.py
-bluequbit/job_run_statuses.py
 bluequbit/version.py
 bluequbit.egg-info/PKG-INFO
 bluequbit.egg-info/SOURCES.txt
 bluequbit.egg-info/dependency_links.txt
 bluequbit.egg-info/requires.txt
 bluequbit.egg-info/top_level.txt
 bluequbit/api/__init__.py
 bluequbit/api/jobs.py
 tests/test_basic_jobs.py
 tests/test_basic_large_jobs.py
+tests/test_batch_jobs.py
 tests/test_cancel_job.py
 tests/test_circuit_serialization.py
+tests/test_count_wrong.py
 tests/test_get_job.py
 tests/test_gpu_job.py
 tests/test_job_estimate.py
 tests/test_metadata.py
 tests/test_ok.py
 tests/test_quantum_job.py
 tests/test_stress_jobs.py
```

### Comparing `bluequbit-0.1.0b9/setup.py` & `bluequbit-0.1.2b1/setup.py`

 * *Files identical despite different names*

### Comparing `bluequbit-0.1.0b9/tests/test_basic_jobs.py` & `bluequbit-0.1.2b1/tests/test_basic_jobs.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,9 +21,10 @@
     for result in results:
         if (
             job_result.job_id == result.job_id
             and job_result.job_name == "testing_basic_search_jobs"
         ):
             print(job_result)
             num_found += 1
+            assert job_result.batch_id is None
 
     assert num_found == 1
```

### Comparing `bluequbit-0.1.0b9/tests/test_basic_large_jobs.py` & `bluequbit-0.1.2b1/tests/test_basic_large_jobs.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,19 +23,20 @@
 
     res2 = dq_client2.wait(result2.job_id)
     assert res2.run_status == "COMPLETED"
     assert res2.error_message is None
     assert res2.job_id == result2.job_id
     print("Job2", res2)
     print("Downloading job 2")
-    with pytest.raises(bluequbit.exceptions.BQStatevectorTooLargeError) as e:
+    with pytest.raises(bluequbit.exceptions.BQJobStatevectorTooLargeError) as e:
         res2.get_statevector()
     assert (
         e.value.message
-        == f"Statevector is too large for {res2.num_qubits} qubits. Use .get_counts() instead."
+        == f"Statevector is too large for {res2.num_qubits} qubits (job:"
+        f" {res2.job_id}). Please use .get_counts() instead."
     )
 
 
 def test_very_large_job():
     dq = bluequbit.BQClient()
 
     qc_qiskit = qiskit.QuantumCircuit(40)
```

### Comparing `bluequbit-0.1.0b9/tests/test_cancel_job.py` & `bluequbit-0.1.2b1/tests/test_stress_jobs.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,53 +1,48 @@
-import os
+import threading
 
-import numpy as np
-import pytest
 import qiskit
 
 import bluequbit
 
+NUM_PER_THREAD = 2
+NUM_THREADS = 2
+
 qc_qiskit = qiskit.QuantumCircuit(2)
 qc_qiskit.h(0)
 qc_qiskit.x(1)
 
+job_ids = [[] for _ in range(NUM_THREADS)]
+
+
+def submit_task(dq_client, thread_no):
+    for _ in range(NUM_PER_THREAD):
+        job_ids[thread_no].append(dq_client.run(qc_qiskit, asynchronous=True).job_id)
+
 
-def test_basic_cancel_job():
+def test_stress_submit_jobs():
     dq_client = bluequbit.BQClient()
+    threads = []
+    for i in range(NUM_THREADS):
+        threads.append(
+            threading.Thread(
+                target=submit_task,
+                args=(
+                    dq_client,
+                    i,
+                ),
+            )
+        )
+        threads[-1].start()
+
+    for i in range(NUM_THREADS):
+        threads[i].join()
+
+    job_ids_flat = [item for sublist in job_ids for item in sublist]
+
+    assert len(job_ids_flat) == NUM_THREADS * NUM_PER_THREAD
 
-    jobs = []
-    num_jobs = 5
-    for _ in range(num_jobs):
-        jobs.append(dq_client.run(qc_qiskit, asynchronous=True))
-
-    dq_client.cancel(jobs[-1].job_id)
-
-    for job in jobs[:-1]:
-        res = dq_client.wait(job.job_id)
-        assert res.run_status == "COMPLETED"
-        assert res.error_message is None
-
-    with pytest.raises(bluequbit.exceptions.BQJobNotCompleteError) as e_info:
-        dq_client.wait(jobs[-1].job_id)
-    assert e_info.value.run_status == "CANCELED"
-
-
-@pytest.mark.skipif(
-    "BLUEQUBIT_STRESS_TESTS" not in os.environ, reason="Requires env variable to be set"
-)
-def test_long_running_cancel_job():
     dq_client = bluequbit.BQClient()
-    num_qubits = 29
-    qc_qiskit = qiskit.QuantumCircuit(num_qubits)
-    qc_qiskit.x(np.arange(num_qubits))
-
-    r = dq_client.run(qc_qiskit, asynchronous=True)
-    for _ in range(1200):
-        res = dq_client.get(r.job_id)
-        if res.run_status == "RUNNING":
-            break
-    else:
-        raise AssertionError()
-
-    r = dq_client.cancel(r.job_id)
-    assert r.run_status == "CANCELED"
-    assert r.error_message == "Canceled by user"
+    for job_id in job_ids_flat:
+        job_result = dq_client.wait(job_id)
+        assert job_result.run_status == "COMPLETED"
+        assert job_result.error_message is None
```

### Comparing `bluequbit-0.1.0b9/tests/test_get_job.py` & `bluequbit-0.1.2b1/tests/test_get_job.py`

 * *Files identical despite different names*

### Comparing `bluequbit-0.1.0b9/tests/test_gpu_job.py` & `bluequbit-0.1.2b1/tests/test_gpu_job.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,16 +23,19 @@
     job_result = dq_client.run(qc_qiskit, job_name="testing_gpu_qiskit", device="gpu")
     print(job_result)
 
     assert job_result.run_status == "COMPLETED"
 
 
 @pytest.mark.skipif(
-    "BLUEQUBIT_STRESS_TESTS" not in os.environ, reason="Requires env variable to be set"
+    "BLUEQUBIT_STRESS_TESTS" not in os.environ,
+    reason="Requires env variable to be set",
 )
+@pytest.mark.order(2)
+@pytest.mark.flaky(reruns=3, reruns_delay=2)
 def test_gpu_job_cirq_measure_gpu1():
     dq_client = bluequbit.BQClient()
     num_qubits = 32
     qc_cirq = cirq.Circuit()
     qubits = cirq.LineQubit.range(num_qubits)
     for i in range(num_qubits):
         qc_cirq.append(cirq.H(qubits[i]))
@@ -40,16 +43,20 @@
     assert job_result.run_status == "COMPLETED"
     print(job_result)
 
     assert job_result.run_time_ms < 13000  # tests 12651, 12708, 12683
 
 
 @pytest.mark.skipif(
-    "BLUEQUBIT_STRESS_TESTS" not in os.environ, reason="Requires env variable to be set"
+    "BLUEQUBIT_STRESS_TESTS" not in os.environ
+    and "BLUEQUBIT_FORCE_GPU2_TEST" not in os.environ,
+    reason="Requires env variable to be set",
 )
+@pytest.mark.order(1)
+@pytest.mark.flaky(reruns=3, reruns_delay=2)
 def test_gpu_job_cirq_measure_gpu2():
     dq_client = bluequbit.BQClient()
     num_qubits = 33
     qc_cirq = cirq.Circuit()
     qubits = cirq.LineQubit.range(num_qubits)
     for i in range(num_qubits):
         qc_cirq.append(cirq.H(qubits[i]))
@@ -59,14 +66,15 @@
 
     assert job_result.run_time_ms < 13300  # tests 12994, 12976, 13071
 
 
 @pytest.mark.skipif(
     "BLUEQUBIT_STRESS_TESTS" not in os.environ, reason="Requires env variable to be set"
 )
+@pytest.mark.flaky(reruns=3, reruns_delay=2)
 def test_gpu_job_cirq_measure_gpu4():
     dq_client = bluequbit.BQClient()
     num_qubits = 34
     qc_cirq = cirq.Circuit()
     qubits = cirq.LineQubit.range(num_qubits)
     for i in range(num_qubits):
         qc_cirq.append(cirq.H(qubits[i]))
@@ -76,14 +84,15 @@
 
     assert job_result.run_time_ms < 14000  # tests: 13726, 13743, 13728
 
 
 @pytest.mark.skipif(
     "BLUEQUBIT_STRESS_TESTS" not in os.environ, reason="Requires env variable to be set"
 )
+@pytest.mark.flaky(reruns=3, reruns_delay=2)
 def test_gpu_job_cirq_measure_gpu8():
     dq_client = bluequbit.BQClient()
     n = 35
     qc = cirq.Circuit()
     qs = cirq.LineQubit.range(n)
     for i in range(n):
         qc.append(cirq.H(qs[i]))
@@ -93,14 +102,15 @@
     assert job_result.run_time_ms < 15500  # tests: 15128, 15131, 15275
     print(job_result)
 
 
 @pytest.mark.skipif(
     "BLUEQUBIT_STRESS_TESTS" not in os.environ, reason="Requires env variable to be set"
 )
+@pytest.mark.flaky(reruns=3, reruns_delay=2)
 def test_gpu_job_cirq_measure_gpu16():
     dq_client = bluequbit.BQClient()
     n = 36
     qc = cirq.Circuit()
     qs = cirq.LineQubit.range(n)
     for i in range(n):
         qc.append(cirq.H(qs[i]))
```

### Comparing `bluequbit-0.1.0b9/tests/test_job_estimate.py` & `bluequbit-0.1.2b1/tests/test_job_estimate.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,45 @@
 import numpy as np
 import pytest
 import qiskit
 
 import bluequbit
+from bluequbit import job_metadata_constants
 
 
-def test_job_estimation():
-    dq_client = bluequbit.BQClient()
+def make_simple_circuit():
     qc_qiskit = qiskit.QuantumCircuit(2)
     qc_qiskit.h(0)
     qc_qiskit.x(1)
+    return qc_qiskit
+
+
+def test_job_estimation():
+    dq_client = bluequbit.BQClient()
+    qc_qiskit = make_simple_circuit()
     results = dq_client.estimate(qc_qiskit)
     assert results.estimated_runtime == 100
 
 
+def test_job_estimation_wrong_device_type():
+    dq_client = bluequbit.BQClient()
+    qc_qiskit = make_simple_circuit()
+    # Should work
+    dq_client.estimate(qc_qiskit, device="CPU")
+
+    # Should fail
+    with pytest.raises(Exception) as e_info:
+        dq_client.estimate(qc_qiskit, device="supercpu")
+    expected = "Invalid device type supercpu. Must be one of " + ", ".join(
+        job_metadata_constants.DEVICE_TYPES
+    )
+    print(e_info.value)
+    assert expected in str(e_info.value)
+
+
 def test_job_estimation_large():
     dq_client = bluequbit.BQClient()
     qc = qiskit.QuantumCircuit(24)
     qc.x(np.arange(24))
     results = dq_client.estimate(qc)
     assert results.estimated_runtime == 187
     # assert results.device == "qsim_simulator"
@@ -30,13 +52,26 @@
 
 def test_job_estimate_validation_too_many_qubits():
     # Too many qubits
     dq_client = bluequbit.BQClient()
     qc = qiskit.QuantumCircuit(38)
     qc.x(np.arange(38))
     result = dq_client.estimate(qc)
-    expected_message = "Circuit contains more than 34 qubits, which is not supported for CPU backend. See deqart.com/docs#supported-circuits for more details."
+    expected_message = (
+        "Circuit contains more than 34 qubits, which is not supported for CPU backend."
+        " See https://app.bluequbit.io/docs for more details."
+    )
     assert expected_message in result.error_message
 
     with pytest.raises(bluequbit.exceptions.BQJobNotCompleteError) as e_info:
         dq_client.run(qc)
     assert e_info.value.run_status == "FAILED_VALIDATION"
+
+
+def test_job_estimation_quantum():
+    dq_client = bluequbit.BQClient()
+    qc = qiskit.QuantumCircuit(24)
+    qc.x(np.arange(24))
+    qc.measure_all()
+    results = dq_client.estimate(qc, device="quantum")
+
+    assert results.estimated_runtime == 1
```

### Comparing `bluequbit-0.1.0b9/tests/test_metadata.py` & `bluequbit-0.1.2b1/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `bluequbit-0.1.0b9/tests/test_quantum_job.py` & `bluequbit-0.1.2b1/tests/test_quantum_job.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,25 +14,29 @@
 def test_quantum_job():
     dq_client = bluequbit.BQClient()
     # time_now = "2022-10-19T13:05:17.917290Z"
     qc_qiskit = qiskit.QuantumCircuit(2)
     qc_qiskit.h(0)
     qc_qiskit.x(1)
     qc_qiskit.measure_all()
-    job_result = dq_client.run(qc_qiskit, job_name="testing_quantum", device="quantum")
+    job_result = dq_client.run(
+        qc_qiskit, job_name="testing_quantum", device="quantum", shots=50
+    )
     assert job_result.error_message is None
     assert job_result.run_status == "COMPLETED"
     assert job_result.device == "quantum"
+    actual = sum(job_result.get_counts().values())
+    assert actual == 50
 
     counts = job_result.get_counts()
     print(counts)
     total_counts = 0
     for _, v in counts.items():
         total_counts += v
-    assert total_counts == 1000
+    assert total_counts == 50
 
 
 def test_quantum_job_no_measurement():
     dq_client = bluequbit.BQClient()
     qc_qiskit = qiskit.QuantumCircuit(2)
     qc_qiskit.h(0)
 
@@ -57,21 +61,36 @@
     dq_client = bluequbit.BQClient()
     # time_now = "2022-10-19T13:05:17.917290Z"
     num_qubits = 30
     qc_qiskit = qiskit.QuantumCircuit(num_qubits)
     qc_qiskit.x(np.arange(num_qubits))
     qc_qiskit.measure_all()
     with pytest.raises(bluequbit.exceptions.BQJobNotCompleteError) as e_info:
-        dq_client.run(
-            qc_qiskit, job_name="testing_quantum", device="quantum", asynchronous=True
-        )
+        dq_client.run(qc_qiskit, job_name="testing_quantum", device="quantum")
     assert e_info.value.run_status == "FAILED_VALIDATION"
 
 
 @pytest.mark.skipif(
+    check_aspen_time_availability() or "BLUEQUBIT_STRESS_TESTS" not in os.environ,
+    reason="Requires env variable to be set",
+)
+def test_quantum_async_job_when_aspen_not_available():
+    dq_client = bluequbit.BQClient()
+    # time_now = "2022-10-19T13:05:17.917290Z"
+    num_qubits = 30
+    qc_qiskit = qiskit.QuantumCircuit(num_qubits)
+    qc_qiskit.x(np.arange(num_qubits))
+    qc_qiskit.measure_all()
+    job_result = dq_client.run(
+        qc_qiskit, job_name="testing_quantum_async", device="quantum", asynchronous=True
+    )
+    assert job_result.run_status != "FAILED_VALIDATION"
+
+
+@pytest.mark.skipif(
     "BLUEQUBIT_STRESS_TESTS" not in os.environ, reason="Requires env variable to be set"
 )
 def test_cancel_quantum_job():
     dq_client = bluequbit.BQClient()
     # time_now = "2022-10-19T13:05:17.917290Z"
     num_qubits = 30
     qc_qiskit = qiskit.QuantumCircuit(num_qubits)
```

### Comparing `bluequbit-0.1.0b9/tests/test_very_large_job.py` & `bluequbit-0.1.2b1/tests/test_very_large_job.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,8 +14,8 @@
     dq_client = bluequbit.BQClient()
     num_qubits = 29
     qc_qiskit = qiskit.QuantumCircuit(num_qubits)
     qc_qiskit.x(np.arange(num_qubits))
 
     with pytest.raises(bluequbit.exceptions.BQJobNotCompleteError) as e:
         dq_client.run(qc_qiskit)
-    assert e.run_status == "TERMINATED"
+    assert e.value.run_status == "TERMINATED"
```

