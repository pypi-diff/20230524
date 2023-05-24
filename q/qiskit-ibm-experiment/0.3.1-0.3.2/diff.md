# Comparing `tmp/qiskit-ibm-experiment-0.3.1.tar.gz` & `tmp/qiskit-ibm-experiment-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit-ibm-experiment-0.3.1.tar", last modified: Thu May  4 14:15:03 2023, max compression
+gzip compressed data, was "qiskit-ibm-experiment-0.3.2.tar", last modified: Wed May 24 12:08:38 2023, max compression
```

## Comparing `qiskit-ibm-experiment-0.3.1.tar` & `qiskit-ibm-experiment-0.3.2.tar`

### file list

```diff
@@ -1,53 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:15:03.159968 qiskit-ibm-experiment-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-05-04 14:15:03.159968 qiskit-ibm-experiment-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:15:03.155968 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:15:03.155968 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/accounts/
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/accounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/accounts/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/accounts/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/accounts/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/accounts/management.py
--rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/accounts/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:15:03.155968 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/client/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11400 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/client/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)    15604 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/client/experiment_rest_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)    27949 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/client/local_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15567 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/client/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:15:03.159968 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/service/
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/service/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/service/device_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/service/experiment_dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)    68992 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/service/ibm_experiment_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     8374 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/service/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:15:03.155968 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-05-04 14:15:02.000000 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-04 14:15:03.000000 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 14:15:02.000000 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 14:15:02.000000 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-04 14:15:02.000000 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 14:15:02.000000 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 14:15:03.159968 qiskit-ibm-experiment-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:15:03.159968 qiskit-ibm-experiment-0.3.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:15:03.159968 qiskit-ibm-experiment-0.3.1/test/service/
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/test/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/test/service/ibm_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/test/service/test_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)    21605 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/test/service/test_experiment_data_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    66547 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/test/service/test_experiment_server_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    17619 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/test/service/test_local_experiment_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:15:03.159968 qiskit-ibm-experiment-0.3.1/test/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/test/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/test/utils/program.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/test/utils/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/test/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:08:38.268434 qiskit-ibm-experiment-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-05-24 12:08:38.268434 qiskit-ibm-experiment-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:08:38.264434 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/VERSION.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:08:38.264434 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/accounts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/accounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/accounts/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/accounts/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/accounts/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/accounts/management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/accounts/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:08:38.264434 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11400 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/client/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15604 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/client/experiment_rest_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27949 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/client/local_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15567 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/client/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:08:38.264434 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/service/
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/service/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/service/device_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/service/experiment_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69035 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/service/ibm_experiment_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8374 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/service/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:08:38.264434 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-05-24 12:08:38.000000 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-24 12:08:38.000000 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 12:08:38.000000 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 12:08:38.000000 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-24 12:08:38.000000 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-24 12:08:38.000000 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 12:08:38.268434 qiskit-ibm-experiment-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:08:38.264434 qiskit-ibm-experiment-0.3.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:08:38.264434 qiskit-ibm-experiment-0.3.2/test/service/
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/test/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/test/service/ibm_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/test/service/test_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21605 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/test/service/test_experiment_data_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66547 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/test/service/test_experiment_server_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17739 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/test/service/test_local_experiment_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:08:38.268434 qiskit-ibm-experiment-0.3.2/test/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/test/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/test/utils/program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/test/utils/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/test/utils/utils.py
```

### Comparing `qiskit-ibm-experiment-0.3.1/LICENSE.txt` & `qiskit-ibm-experiment-0.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.1/PKG-INFO` & `qiskit-ibm-experiment-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-ibm-experiment
-Version: 0.3.1
+Version: 0.3.2
 Summary: Qiskit IBM Experiment service for accessing the quantum experiment interface at IBM
 Home-page: https://github.com/Qiskit/qiskit-ibm-experiment
 Author: Qiskit Development Team
 Author-email: hello@qiskit.org
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/Qiskit/qiskit-ibm-experiment/issues
 Project-URL: Documentation, https://qiskit.org/documentation/
@@ -143,9 +143,9 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `qiskit-ibm-experiment-0.3.1/README.md` & `qiskit-ibm-experiment-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/__init__.py` & `qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/accounts/__init__.py` & `qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/accounts/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/accounts/account.py` & `qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/accounts/account.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/accounts/configuration.py` & `qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/accounts/configuration.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/accounts/exceptions.py` & `qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/accounts/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/accounts/management.py` & `qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/accounts/management.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/accounts/storage.py` & `qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/accounts/storage.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/client/__init__.py` & `qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/client/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/client/experiment.py` & `qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/client/experiment.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/client/experiment_rest_adapter.py` & `qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/client/experiment_rest_adapter.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/client/local_client.py` & `qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/client/local_client.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/client/session.py` & `qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/client/session.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/exceptions.py` & `qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/service/__init__.py` & `qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/service/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/service/constants.py` & `qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/service/constants.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/service/device_component.py` & `qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/service/device_component.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/service/experiment_dataclasses.py` & `qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/service/experiment_dataclasses.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/service/ibm_experiment_service.py` & `qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/service/ibm_experiment_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -367,22 +367,23 @@
             "uuid",
             "device_name",
             "group_id",
             "hub_id",
             "project_id",
             "type",
             "start_time",
+            "parent_experiment_uuid",
         ]
         for field_name in unused_fields:
             if field_name in api_data:
                 del api_data[field_name]
 
         if not data:
             logger.warning("update_experiment() called with nothing to update.")
-            return
+            return None
 
         with map_api_error(f"Experiment {data.experiment_id} update failed."):
             response_data = self._api_client.experiment_update(
                 data.experiment_id, json.dumps(api_data, cls=json_encoder)
             )
             return response_data
```

### Comparing `qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/service/utils.py` & `qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/service/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/version.py` & `qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/version.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment.egg-info/PKG-INFO` & `qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-ibm-experiment
-Version: 0.3.1
+Version: 0.3.2
 Summary: Qiskit IBM Experiment service for accessing the quantum experiment interface at IBM
 Home-page: https://github.com/Qiskit/qiskit-ibm-experiment
 Author: Qiskit Development Team
 Author-email: hello@qiskit.org
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/Qiskit/qiskit-ibm-experiment/issues
 Project-URL: Documentation, https://qiskit.org/documentation/
@@ -143,9 +143,9 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment.egg-info/SOURCES.txt` & `qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE.txt
 MANIFEST.in
 README.md
+pyproject.toml
 setup.py
 qiskit_ibm_experiment/VERSION.txt
 qiskit_ibm_experiment/__init__.py
 qiskit_ibm_experiment/exceptions.py
 qiskit_ibm_experiment/version.py
 qiskit_ibm_experiment.egg-info/PKG-INFO
 qiskit_ibm_experiment.egg-info/SOURCES.txt
```

### Comparing `qiskit-ibm-experiment-0.3.1/setup.py` & `qiskit-ibm-experiment-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         "Programming Language :: Python :: 3.9",
         "Topic :: Scientific/Engineering",
     ],
     keywords="qiskit sdk quantum api experiment ibm",
     packages=setuptools.find_packages(exclude=["test*"]),
     install_requires=REQUIREMENTS,
     include_package_data=True,
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     zip_safe=False,
     project_urls={
         "Bug Tracker": "https://github.com/Qiskit/qiskit-ibm-experiment/issues",
         "Documentation": "https://qiskit.org/documentation/",
         "Source Code": "https://github.com/Qiskit/qiskit-ibm-experiment",
     },
 )
```

### Comparing `qiskit-ibm-experiment-0.3.1/test/__init__.py` & `qiskit-ibm-experiment-0.3.2/test/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.1/test/service/ibm_test_case.py` & `qiskit-ibm-experiment-0.3.2/test/service/ibm_test_case.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.1/test/service/test_experiment.py` & `qiskit-ibm-experiment-0.3.2/test/service/test_experiment.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.1/test/service/test_experiment_data_integration.py` & `qiskit-ibm-experiment-0.3.2/test/service/test_experiment_data_integration.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.1/test/service/test_experiment_server_integration.py` & `qiskit-ibm-experiment-0.3.2/test/service/test_experiment_server_integration.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.1/test/service/test_local_experiment_client.py` & `qiskit-ibm-experiment-0.3.2/test/service/test_local_experiment_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     def test_create_experiment(self):
         """Tests creating an experiment"""
         data = ExperimentData(
             experiment_type="test_experiment",
             backend="ibmq_qasm_simulator",
             metadata={"float_data": 3.14, "string_data": "foo"},
         )
-        exp_id = self.service.create_experiment(data)
+        exp_id = self.service.create_experiment(data)["uuid"]
         self.assertIsNotNone(exp_id)
 
         exp = self.service.experiment(experiment_id=exp_id)
         self.assertEqual(exp.experiment_type, "test_experiment")
         self.assertEqual(exp.backend, "ibmq_qasm_simulator")
         self.assertEqual(exp.metadata["float_data"], 3.14)
         self.assertEqual(exp.metadata["string_data"], "foo")
@@ -60,15 +60,15 @@
     def test_update_experiment(self):
         """Tests updating an experiment"""
         data = ExperimentData(
             experiment_type="test_experiment",
             backend="ibmq_qasm_simulator",
             metadata={"float_data": 3.14, "string_data": "foo"},
         )
-        exp_id = self.service.create_experiment(data)
+        exp_id = self.service.create_experiment(data)["uuid"]
         data = self.service.experiment(exp_id)
         data.metadata["float_data"] = 2.71
         data.experiment_type = "foo_type"  # this should NOT change
         data.notes = ["foo_note"]
         self.service.update_experiment(data)
         result = self.service.experiment(exp_id)
         self.assertEqual(result.metadata["float_data"], 2.71)
@@ -81,15 +81,15 @@
 
     def test_delete_experiment(self):
         """Tests deleting an experiment"""
         data = ExperimentData(
             experiment_type="test_experiment",
             backend="ibmq_qasm_simulator",
         )
-        exp_id = self.service.create_experiment(data)
+        exp_id = self.service.create_experiment(data)["uuid"]
         # Check the experiment exists
         self.service.experiment(experiment_id=exp_id)
         self.service.delete_experiment(exp_id)
         with self.assertRaises(IBMExperimentEntryNotFound):
             self.service.experiment(experiment_id=exp_id)
 
     def test_get_experiments(self):
@@ -120,15 +120,15 @@
 
     def test_create_analysis_result(self):
         """Tests creating an analysis result"""
         exp_id = self.service.create_experiment(
             ExperimentData(
                 experiment_type="test_experiment", backend="ibmq_qasm_simulator"
             )
-        )
+        )["uuid"]
         analysis_result_value = {"str": "foo", "float": 3.14}
         analysis_data = AnalysisResultData(
             experiment_id=exp_id,
             result_data=analysis_result_value,
             result_type="qiskit_test",
         )
         analysis_id = self.service.create_analysis_result(analysis_data)
@@ -139,15 +139,15 @@
 
     def test_get_analysis_results(self):
         """Tests getting an analysis result"""
         exp_id = self.service.create_experiment(
             ExperimentData(
                 experiment_type="test_experiment", backend="ibmq_qasm_simulator"
             )
-        )
+        )["uuid"]
         result_ids = ["00", "01", "10", "11"]
         for result_id in result_ids:
             analysis_result_value = {
                 "str": f"foo_{result_id}",
                 "float": 3.14 + int(result_id),
             }
             analysis_data = AnalysisResultData(
@@ -170,15 +170,15 @@
 
     def test_delete_analysis_result(self):
         """Tests deleting an analysis result"""
         exp_id = self.service.create_experiment(
             ExperimentData(
                 experiment_type="test_experiment", backend="ibmq_qasm_simulator"
             )
-        )
+        )["uuid"]
         analysis_data = AnalysisResultData(
             experiment_id=exp_id,
             result_data={"foo": "delete_bar"},
             result_type="test_result",
         )
         result_id = self.service.create_analysis_result(analysis_data)
         result = self.service.analysis_result(result_id)
@@ -245,57 +245,57 @@
 
     def test_figure(self):
         """Test getting a figure."""
         exp_id = self.service.create_experiment(
             ExperimentData(
                 experiment_type="test_experiment", backend="ibmq_qasm_simulator"
             )
-        )
+        )["uuid"]
         hello_bytes = str.encode("hello world")
         figure_name = "hello.svg"
         self.service.create_figure(
             experiment_id=exp_id, figure=hello_bytes, figure_name=figure_name
         )
         fig = self.service.figure(exp_id, figure_name)
         self.assertEqual(fig, hello_bytes)
 
     def test_files(self):
         """Test upload and download of files"""
         exp_id = self.service.create_experiment(
             ExperimentData(
                 experiment_type="test_experiment", backend="ibmq_qasm_simulator"
             )
-        )
+        )["uuid"]
         hello_data = {"hello": "world", "foo": "bar"}
         filename = "test_file.json"
         self.service.file_upload(exp_id, filename, hello_data)
         rfile_data = self.service.file_download(exp_id, filename)
         self.assertEqual(hello_data, rfile_data)
         self.assertTrue(self.service.experiment_has_file(exp_id, filename))
         file_list = self.service.files(exp_id)["files"]
         self.assertEqual(len(file_list), 1)
         self.assertEqual(file_list[0]["Key"], filename)
 
         exp_id2 = self.service.create_experiment(
             ExperimentData(
                 experiment_type="test_experiment", backend="ibmq_qasm_simulator"
             )
-        )
+        )["uuid"]
         file_list = self.service.files(exp_id2)["files"]
         self.assertEqual(len(file_list), 0)
 
     def test_server_setting_start_time(self):
         """Tests that start time is initialized by the server unless already present"""
         ref_start_dt = datetime.now() - timedelta(days=1)
         exp_id = self.service.create_experiment(
             ExperimentData(
                 experiment_type="qiskit_time_test",
                 backend="ibmq_qasm_simulator",
             )
-        )
+        )["uuid"]
         experiments = self.service.experiments(
             start_datetime_after=ref_start_dt,
             experiment_type="qiskit_time_test",
         )
         found = False
         for exp in experiments:
             if exp.experiment_id == exp_id:
@@ -308,15 +308,15 @@
         ref_start_dt = ref_start_dt.replace(tzinfo=tz.tzlocal())
         exp_id = self.service.create_experiment(
             ExperimentData(
                 experiment_type="qiskit_test",
                 backend="ibmq_qasm_simulator",
                 start_datetime=ref_start_dt,
             )
-        )
+        )["uuid"]
 
         before_start = ref_start_dt - timedelta(hours=1)
         after_start = ref_start_dt + timedelta(hours=1)
 
         sub_tests = [
             (before_start, None, True, "before start, None"),
             (None, after_start, True, "None, after start"),
@@ -353,29 +353,29 @@
         tags = [str(uuid.uuid4())]
         exp1 = self.service.create_experiment(
             ExperimentData(
                 tags=tags,
                 experiment_type="qiskit_test_1",
                 start_datetime=datetime.now() - timedelta(hours=1),
             )
-        )
+        )["uuid"]
         exp2 = self.service.create_experiment(
             ExperimentData(
                 tags=tags,
                 experiment_type="qiskit_test_2",
                 start_datetime=datetime.now(),
             )
-        )
+        )["uuid"]
         exp3 = self.service.create_experiment(
             ExperimentData(
                 tags=tags,
                 experiment_type="qiskit_test_1",
                 start_datetime=datetime.now() - timedelta(hours=2),
             )
-        )
+        )["uuid"]
 
         subtests = [
             (
                 ["experiment_type:asc"],
                 [exp1, exp3, exp2] if exp1 < exp3 else [exp3, exp1, exp2],
             ),
             (
@@ -410,15 +410,15 @@
         experiment_type = experiment_type or "qiskit_test"
         exp_id = self.service.create_experiment(
             ExperimentData(
                 experiment_type=experiment_type,
                 **kwargs,
             ),
             json_encoder=json_encoder,
-        )
+        )["uuid"]
         return exp_id
 
     def _create_analysis_result(
         self,
         exp_id: Optional[str] = None,
         result_type: Optional[str] = None,
         result_data: Optional[Dict] = None,
```

### Comparing `qiskit-ibm-experiment-0.3.1/test/utils/program.py` & `qiskit-ibm-experiment-0.3.2/test/utils/program.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.1/test/utils/templates.py` & `qiskit-ibm-experiment-0.3.2/test/utils/templates.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.1/test/utils/utils.py` & `qiskit-ibm-experiment-0.3.2/test/utils/utils.py`

 * *Files identical despite different names*

