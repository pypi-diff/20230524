# Comparing `tmp/airflow_mcd-0.0.7.tar.gz` & `tmp/airflow_mcd-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/airflow_mcd-0.0.7.tar", last modified: Thu Sep  8 20:00:26 2022, max compression
+gzip compressed data, was "dist/airflow_mcd-0.0.8.tar", last modified: Wed May 24 15:04:11 2023, max compression
```

## Comparing `airflow_mcd-0.0.7.tar` & `airflow_mcd-0.0.8.tar`

### file list

```diff
@@ -1,44 +1,51 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-08 20:00:26.343683 airflow_mcd-0.0.7/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-08 20:00:26.339683 airflow_mcd-0.0.7/.circleci/
--rw-r--r--   0 root         (0) root         (0)      168 2022-09-08 19:59:33.000000 airflow_mcd-0.0.7/.circleci/README
--rw-r--r--   0 root         (0) root         (0)     3102 2022-09-08 19:59:33.000000 airflow_mcd-0.0.7/.circleci/config.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-08 20:00:26.339683 airflow_mcd-0.0.7/.circleci/trufflehog_config/
--rw-r--r--   0 root         (0) root         (0)      377 2022-09-08 19:59:33.000000 airflow_mcd-0.0.7/.circleci/trufflehog_config/allowlist.json
--rw-r--r--   0 root         (0) root         (0)       29 2022-09-08 19:59:33.000000 airflow_mcd-0.0.7/.coveragerc
--rw-r--r--   0 root         (0) root         (0)     1818 2022-09-08 19:59:33.000000 airflow_mcd-0.0.7/.gitignore
--rw-r--r--   0 root         (0) root         (0)    11357 2022-09-08 19:59:33.000000 airflow_mcd-0.0.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1129 2022-09-08 19:59:33.000000 airflow_mcd-0.0.7/Makefile
--rw-r--r--   0 root         (0) root         (0)     5259 2022-09-08 20:00:26.343683 airflow_mcd-0.0.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      958 2022-09-08 19:59:33.000000 airflow_mcd-0.0.7/README-dev.md
--rw-r--r--   0 root         (0) root         (0)     4445 2022-09-08 19:59:33.000000 airflow_mcd-0.0.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-08 20:00:26.339683 airflow_mcd-0.0.7/airflow_mcd/
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-08 19:59:33.000000 airflow_mcd-0.0.7/airflow_mcd/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-08 20:00:26.343683 airflow_mcd-0.0.7/airflow_mcd/hooks/
--rw-r--r--   0 root         (0) root         (0)       55 2022-09-08 19:59:33.000000 airflow_mcd-0.0.7/airflow_mcd/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2773 2022-09-08 19:59:33.000000 airflow_mcd-0.0.7/airflow_mcd/hooks/session_hook.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-08 20:00:26.343683 airflow_mcd-0.0.7/airflow_mcd/operators/
--rw-r--r--   0 root         (0) root         (0)       89 2022-09-08 19:59:33.000000 airflow_mcd-0.0.7/airflow_mcd/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)      703 2022-09-08 19:59:33.000000 airflow_mcd-0.0.7/airflow_mcd/operators/base_operator.py
--rw-r--r--   0 root         (0) root         (0)     3895 2022-09-08 19:59:33.000000 airflow_mcd-0.0.7/airflow_mcd/operators/circuit_breaker_operators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-08 20:00:26.343683 airflow_mcd-0.0.7/airflow_mcd.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5259 2022-09-08 20:00:26.000000 airflow_mcd-0.0.7/airflow_mcd.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      816 2022-09-08 20:00:26.000000 airflow_mcd-0.0.7/airflow_mcd.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-08 20:00:26.000000 airflow_mcd-0.0.7/airflow_mcd.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2022-09-08 20:00:26.000000 airflow_mcd-0.0.7/airflow_mcd.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-09-08 20:00:26.000000 airflow_mcd-0.0.7/airflow_mcd.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-08 20:00:26.343683 airflow_mcd-0.0.7/examples/
--rw-r--r--   0 root         (0) root         (0)     2050 2022-09-08 19:59:33.000000 airflow_mcd-0.0.7/examples/sample_circuit_dag.py
--rw-r--r--   0 root         (0) root         (0)       45 2022-09-08 19:59:33.000000 airflow_mcd-0.0.7/requirements-ci.txt
--rw-r--r--   0 root         (0) root         (0)       25 2022-09-08 19:59:33.000000 airflow_mcd-0.0.7/requirements-dev.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-09-08 19:59:33.000000 airflow_mcd-0.0.7/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       79 2022-09-08 20:00:26.343683 airflow_mcd-0.0.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1484 2022-09-08 19:59:33.000000 airflow_mcd-0.0.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-08 20:00:26.343683 airflow_mcd-0.0.7/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-08 19:59:33.000000 airflow_mcd-0.0.7/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-08 20:00:26.343683 airflow_mcd-0.0.7/tests/hooks/
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-08 19:59:33.000000 airflow_mcd-0.0.7/tests/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3780 2022-09-08 19:59:33.000000 airflow_mcd-0.0.7/tests/hooks/test_session_hook.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-08 20:00:26.343683 airflow_mcd-0.0.7/tests/operators/
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-08 19:59:33.000000 airflow_mcd-0.0.7/tests/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)      719 2022-09-08 19:59:33.000000 airflow_mcd-0.0.7/tests/operators/test_base_op.py
--rw-r--r--   0 root         (0) root         (0)     5843 2022-09-08 19:59:33.000000 airflow_mcd-0.0.7/tests/operators/test_circuit_breaker_op.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:04:11.973982 airflow_mcd-0.0.8/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:04:11.973982 airflow_mcd-0.0.8/.circleci/
+-rw-r--r--   0 root         (0) root         (0)      168 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/.circleci/README
+-rw-r--r--   0 root         (0) root         (0)     3102 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/.circleci/config.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:04:11.973982 airflow_mcd-0.0.8/.circleci/trufflehog_config/
+-rw-r--r--   0 root         (0) root         (0)      377 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/.circleci/trufflehog_config/allowlist.json
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/.coveragerc
+-rw-r--r--   0 root         (0) root         (0)     1818 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/.gitignore
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1129 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/Makefile
+-rw-r--r--   0 root         (0) root         (0)     5259 2023-05-24 15:04:11.973982 airflow_mcd-0.0.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      958 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/README-dev.md
+-rw-r--r--   0 root         (0) root         (0)     4445 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:04:11.973982 airflow_mcd-0.0.8/airflow_mcd/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/airflow_mcd/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:04:11.973982 airflow_mcd-0.0.8/airflow_mcd/callbacks/
+-rw-r--r--   0 root         (0) root         (0)     5457 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/airflow_mcd/callbacks/client.py
+-rw-r--r--   0 root         (0) root         (0)     5476 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/airflow_mcd/callbacks/mcd_callbacks.py
+-rw-r--r--   0 root         (0) root         (0)     4690 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/airflow_mcd/callbacks/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:04:11.973982 airflow_mcd-0.0.8/airflow_mcd/hooks/
+-rw-r--r--   0 root         (0) root         (0)       55 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/airflow_mcd/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2773 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/airflow_mcd/hooks/session_hook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:04:11.973982 airflow_mcd-0.0.8/airflow_mcd/operators/
+-rw-r--r--   0 root         (0) root         (0)       89 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/airflow_mcd/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      703 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/airflow_mcd/operators/base_operator.py
+-rw-r--r--   0 root         (0) root         (0)     3895 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/airflow_mcd/operators/circuit_breaker_operators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:04:11.973982 airflow_mcd-0.0.8/airflow_mcd.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5259 2023-05-24 15:04:11.000000 airflow_mcd-0.0.8/airflow_mcd.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      980 2023-05-24 15:04:11.000000 airflow_mcd-0.0.8/airflow_mcd.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 15:04:11.000000 airflow_mcd-0.0.8/airflow_mcd.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-05-24 15:04:11.000000 airflow_mcd-0.0.8/airflow_mcd.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-05-24 15:04:11.000000 airflow_mcd-0.0.8/airflow_mcd.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:04:11.973982 airflow_mcd-0.0.8/examples/
+-rw-r--r--   0 root         (0) root         (0)     2050 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/examples/sample_circuit_dag.py
+-rw-r--r--   0 root         (0) root         (0)       45 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/requirements-ci.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/requirements-dev.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2023-05-24 15:04:11.977982 airflow_mcd-0.0.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1484 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:04:11.973982 airflow_mcd-0.0.8/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:04:11.973982 airflow_mcd-0.0.8/tests/callbacks/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/tests/callbacks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10230 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/tests/callbacks/test_callbacks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:04:11.973982 airflow_mcd-0.0.8/tests/hooks/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/tests/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3780 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/tests/hooks/test_session_hook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:04:11.973982 airflow_mcd-0.0.8/tests/operators/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/tests/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      719 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/tests/operators/test_base_op.py
+-rw-r--r--   0 root         (0) root         (0)     5843 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/tests/operators/test_circuit_breaker_op.py
```

### Comparing `airflow_mcd-0.0.7/.circleci/config.yml` & `airflow_mcd-0.0.8/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.0.7/.gitignore` & `airflow_mcd-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.0.7/LICENSE` & `airflow_mcd-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.0.7/Makefile` & `airflow_mcd-0.0.8/Makefile`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.0.7/PKG-INFO` & `airflow_mcd-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow_mcd
-Version: 0.0.7
+Version: 0.0.8
 Summary: Monte Carlo's Apache Airflow Provider
 Home-page: https://www.montecarlodata.com/
 Author: Monte Carlo Data, Inc
 Author-email: info@montecarlodata.com
 License: Apache Software License (Apache 2.0)
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `airflow_mcd-0.0.7/README-dev.md` & `airflow_mcd-0.0.8/README-dev.md`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.0.7/README.md` & `airflow_mcd-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.0.7/airflow_mcd/hooks/session_hook.py` & `airflow_mcd-0.0.8/airflow_mcd/hooks/session_hook.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.0.7/airflow_mcd/operators/base_operator.py` & `airflow_mcd-0.0.8/airflow_mcd/operators/base_operator.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.0.7/airflow_mcd/operators/circuit_breaker_operators.py` & `airflow_mcd-0.0.8/airflow_mcd/operators/circuit_breaker_operators.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.0.7/airflow_mcd.egg-info/PKG-INFO` & `airflow_mcd-0.0.8/airflow_mcd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-mcd
-Version: 0.0.7
+Version: 0.0.8
 Summary: Monte Carlo's Apache Airflow Provider
 Home-page: https://www.montecarlodata.com/
 Author: Monte Carlo Data, Inc
 Author-email: info@montecarlodata.com
 License: Apache Software License (Apache 2.0)
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `airflow_mcd-0.0.7/airflow_mcd.egg-info/SOURCES.txt` & `airflow_mcd-0.0.8/airflow_mcd.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -14,19 +14,24 @@
 .circleci/trufflehog_config/allowlist.json
 airflow_mcd/__init__.py
 airflow_mcd.egg-info/PKG-INFO
 airflow_mcd.egg-info/SOURCES.txt
 airflow_mcd.egg-info/dependency_links.txt
 airflow_mcd.egg-info/requires.txt
 airflow_mcd.egg-info/top_level.txt
+airflow_mcd/callbacks/client.py
+airflow_mcd/callbacks/mcd_callbacks.py
+airflow_mcd/callbacks/utils.py
 airflow_mcd/hooks/__init__.py
 airflow_mcd/hooks/session_hook.py
 airflow_mcd/operators/__init__.py
 airflow_mcd/operators/base_operator.py
 airflow_mcd/operators/circuit_breaker_operators.py
 examples/sample_circuit_dag.py
 tests/__init__.py
+tests/callbacks/__init__.py
+tests/callbacks/test_callbacks.py
 tests/hooks/__init__.py
 tests/hooks/test_session_hook.py
 tests/operators/__init__.py
 tests/operators/test_base_op.py
 tests/operators/test_circuit_breaker_op.py
```

### Comparing `airflow_mcd-0.0.7/examples/sample_circuit_dag.py` & `airflow_mcd-0.0.8/examples/sample_circuit_dag.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.0.7/setup.py` & `airflow_mcd-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.0.7/tests/hooks/test_session_hook.py` & `airflow_mcd-0.0.8/tests/hooks/test_session_hook.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.0.7/tests/operators/test_base_op.py` & `airflow_mcd-0.0.8/tests/operators/test_base_op.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.0.7/tests/operators/test_circuit_breaker_op.py` & `airflow_mcd-0.0.8/tests/operators/test_circuit_breaker_op.py`

 * *Files identical despite different names*

