# Comparing `tmp/reportportal-client-5.3.2.tar.gz` & `tmp/reportportal-client-5.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reportportal-client-5.3.2.tar", last modified: Thu Apr 27 13:40:30 2023, max compression
+gzip compressed data, was "reportportal-client-5.3.3.tar", last modified: Wed May 24 11:55:43 2023, max compression
```

## Comparing `reportportal-client-5.3.2.tar` & `reportportal-client-5.3.3.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:40:30.858358 reportportal-client-5.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-04-27 13:40:30.858358 reportportal-client-5.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:40:30.850358 reportportal-client-5.3.2/reportportal_client/
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:40:30.854358 reportportal-client-5.3.2/reportportal_client/_local/
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/_local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18487 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/client.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:40:30.854358 reportportal-client-5.3.2/reportportal_client/core/
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/core/rp_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/core/rp_issues.py
--rw-r--r--   0 runner    (1001) docker     (123)    17526 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/core/rp_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/core/rp_responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     9243 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/core/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6985 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/core/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7366 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/helpers.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:40:30.858358 reportportal-client-5.3.2/reportportal_client/items/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/items/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/items/item_weight.py
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/items/rp_base_item.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:40:30.858358 reportportal-client-5.3.2/reportportal_client/items/rp_log_items/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/items/rp_log_items/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/items/rp_log_items/rp_log_item.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:40:30.858358 reportportal-client-5.3.2/reportportal_client/items/rp_test_items/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/items/rp_test_items/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/items/rp_test_items/rp_base_test_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/items/rp_test_items/rp_child_test_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/items/rp_test_items/rp_root_test_item.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:40:30.858358 reportportal-client-5.3.2/reportportal_client/logs/
--rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/logs/log_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:40:30.858358 reportportal-client-5.3.2/reportportal_client/services/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/services/client_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/services/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/services/statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:40:30.858358 reportportal-client-5.3.2/reportportal_client/static/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/static/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/static/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/static/defines.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/static/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:40:30.858358 reportportal-client-5.3.2/reportportal_client/steps/
--rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/steps/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:40:30.854358 reportportal-client-5.3.2/reportportal_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-04-27 13:40:30.000000 reportportal-client-5.3.2/reportportal_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-04-27 13:40:30.000000 reportportal-client-5.3.2/reportportal_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 13:40:30.000000 reportportal-client-5.3.2/reportportal_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-27 13:40:30.000000 reportportal-client-5.3.2/reportportal_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-27 13:40:30.000000 reportportal-client-5.3.2/reportportal_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-27 13:40:30.858358 reportportal-client-5.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:40:30.858358 reportportal-client-5.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/tests/test_client_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/tests/test_statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:55:43.504092 reportportal-client-5.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-05-24 11:55:36.000000 reportportal-client-5.3.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-24 11:55:36.000000 reportportal-client-5.3.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-24 11:55:36.000000 reportportal-client-5.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-05-24 11:55:43.504092 reportportal-client-5.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-05-24 11:55:36.000000 reportportal-client-5.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-24 11:55:36.000000 reportportal-client-5.3.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:55:43.496092 reportportal-client-5.3.3/reportportal_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-24 11:55:36.000000 reportportal-client-5.3.3/reportportal_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:55:43.496092 reportportal-client-5.3.3/reportportal_client/_local/
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-24 11:55:36.000000 reportportal-client-5.3.3/reportportal_client/_local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19275 2023-05-24 11:55:36.000000 reportportal-client-5.3.3/reportportal_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-05-24 11:55:36.000000 reportportal-client-5.3.3/reportportal_client/client.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:55:43.500092 reportportal-client-5.3.3/reportportal_client/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-24 11:55:36.000000 reportportal-client-5.3.3/reportportal_client/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-24 11:55:36.000000 reportportal-client-5.3.3/reportportal_client/core/rp_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-05-24 11:55:36.000000 reportportal-client-5.3.3/reportportal_client/core/rp_issues.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17526 2023-05-24 11:55:36.000000 reportportal-client-5.3.3/reportportal_client/core/rp_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-05-24 11:55:36.000000 reportportal-client-5.3.3/reportportal_client/core/rp_responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9243 2023-05-24 11:55:36.000000 reportportal-client-5.3.3/reportportal_client/core/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6985 2023-05-24 11:55:36.000000 reportportal-client-5.3.3/reportportal_client/core/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-24 11:55:36.000000 reportportal-client-5.3.3/reportportal_client/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7366 2023-05-24 11:55:36.000000 reportportal-client-5.3.3/reportportal_client/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-24 11:55:36.000000 reportportal-client-5.3.3/reportportal_client/helpers.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:55:43.500092 reportportal-client-5.3.3/reportportal_client/items/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-24 11:55:36.000000 reportportal-client-5.3.3/reportportal_client/items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-24 11:55:36.000000 reportportal-client-5.3.3/reportportal_client/items/item_weight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-05-24 11:55:36.000000 reportportal-client-5.3.3/reportportal_client/items/rp_base_item.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:55:43.500092 reportportal-client-5.3.3/reportportal_client/items/rp_log_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-24 11:55:36.000000 reportportal-client-5.3.3/reportportal_client/items/rp_log_items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-24 11:55:36.000000 reportportal-client-5.3.3/reportportal_client/items/rp_log_items/rp_log_item.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:55:43.500092 reportportal-client-5.3.3/reportportal_client/items/rp_test_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-24 11:55:36.000000 reportportal-client-5.3.3/reportportal_client/items/rp_test_items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-05-24 11:55:36.000000 reportportal-client-5.3.3/reportportal_client/items/rp_test_items/rp_base_test_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-05-24 11:55:36.000000 reportportal-client-5.3.3/reportportal_client/items/rp_test_items/rp_child_test_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-05-24 11:55:36.000000 reportportal-client-5.3.3/reportportal_client/items/rp_test_items/rp_root_test_item.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:55:43.500092 reportportal-client-5.3.3/reportportal_client/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-05-24 11:55:36.000000 reportportal-client-5.3.3/reportportal_client/logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-05-24 11:55:36.000000 reportportal-client-5.3.3/reportportal_client/logs/log_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:55:43.504092 reportportal-client-5.3.3/reportportal_client/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-24 11:55:36.000000 reportportal-client-5.3.3/reportportal_client/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-05-24 11:55:36.000000 reportportal-client-5.3.3/reportportal_client/services/client_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-24 11:55:36.000000 reportportal-client-5.3.3/reportportal_client/services/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-24 11:55:36.000000 reportportal-client-5.3.3/reportportal_client/services/statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:55:43.504092 reportportal-client-5.3.3/reportportal_client/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-24 11:55:36.000000 reportportal-client-5.3.3/reportportal_client/static/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-05-24 11:55:36.000000 reportportal-client-5.3.3/reportportal_client/static/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-24 11:55:36.000000 reportportal-client-5.3.3/reportportal_client/static/defines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-24 11:55:36.000000 reportportal-client-5.3.3/reportportal_client/static/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:55:43.504092 reportportal-client-5.3.3/reportportal_client/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-05-24 11:55:36.000000 reportportal-client-5.3.3/reportportal_client/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-05-24 11:55:36.000000 reportportal-client-5.3.3/reportportal_client/steps/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:55:43.496092 reportportal-client-5.3.3/reportportal_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-05-24 11:55:43.000000 reportportal-client-5.3.3/reportportal_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-05-24 11:55:43.000000 reportportal-client-5.3.3/reportportal_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 11:55:43.000000 reportportal-client-5.3.3/reportportal_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-24 11:55:43.000000 reportportal-client-5.3.3/reportportal_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-24 11:55:43.000000 reportportal-client-5.3.3/reportportal_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-24 11:55:36.000000 reportportal-client-5.3.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-24 11:55:43.504092 reportportal-client-5.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-24 11:55:36.000000 reportportal-client-5.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:55:43.504092 reportportal-client-5.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-05-24 11:55:36.000000 reportportal-client-5.3.3/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-05-24 11:55:36.000000 reportportal-client-5.3.3/tests/test_client_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-05-24 11:55:36.000000 reportportal-client-5.3.3/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-05-24 11:55:36.000000 reportportal-client-5.3.3/tests/test_statistics.py
```

### Comparing `reportportal-client-5.3.2/CONTRIBUTING.rst` & `reportportal-client-5.3.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.2/LICENSE.md` & `reportportal-client-5.3.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.2/PKG-INFO` & `reportportal-client-5.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: reportportal-client
-Version: 5.3.2
+Version: 5.3.3
 Summary: Python client for Report Portal v5.
 Home-page: https://github.com/reportportal/client-Python
-Download-URL: https://github.com/reportportal/client-Python/tarball/5.3.2
+Download-URL: https://github.com/reportportal/client-Python/tarball/5.3.3
 Author: Report Portal Team
 Author-email: support@reportportal.io
 License: Apache 2.0.
 Keywords: testing,reporting,reportportal,client
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `reportportal-client-5.3.2/README.md` & `reportportal-client-5.3.3/README.md`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.2/reportportal_client/__init__.py` & `reportportal-client-5.3.3/reportportal_client/__init__.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.2/reportportal_client/_local/__init__.py` & `reportportal-client-5.3.3/reportportal_client/_local/__init__.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.2/reportportal_client/client.py` & `reportportal-client-5.3.3/reportportal_client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,14 +94,16 @@
             self.endpoint, 'api/{}'.format(self.api_v2), self.project)
         self.is_skipped_an_issue = is_skipped_an_issue
         self.launch_id = launch_id
         self.log_batch_size = log_batch_size
         self.log_batch_payload_size = log_batch_payload_size
         self.token = token
         self.verify_ssl = verify_ssl
+        self.retries = retries
+        self.max_pool_size = max_pool_size
         self.http_timeout = http_timeout
         self.session = requests.Session()
         self.step_reporter = StepReporter(self)
         self._item_stack = []
         self.mode = mode
         self._skip_analytics = getenv('AGENT_NO_ANALYTICS')
 
@@ -163,15 +165,15 @@
                          attributes=None,
                          description=None,
                          retry=False,
                          **kwargs):
         """Finish suite/case/step/nested step item.
 
         :param item_id:     ID of the test item
-        :param end_time:    Test item end time
+        :param end_time:    The item end time
         :param status:      Test status. Allowable values: "passed",
                             "failed", "stopped", "skipped", "interrupted",
                             "cancelled" or None
         :param attributes:  Test item attributes(tags). Pairs of key and value.
                             Override attributes on start
         :param description: Test item description. Overrides description
                             from start request.
@@ -193,15 +195,14 @@
             issue=issue,
             retry=retry
         ).payload
         response = HttpRequest(self.session.put, url=url, json=request_payload,
                                verify_ssl=self.verify_ssl).make()
         if not response:
             return
-        # noinspection PyUnresolvedReferences
         self._item_stack.pop() if len(self._item_stack) > 0 else None
         logger.debug('finish_test_item - ID: %s', item_id)
         logger.debug('response message: %s', response.message)
         return response.message
 
     def get_item_id_by_uuid(self, uuid):
         """Get test item ID by the given UUID.
@@ -277,17 +278,17 @@
                                verify_ssl=self.verify_ssl).make()
         return response.json if response else None
 
     def log(self, time, message, level=None, attachment=None, item_id=None):
         """Send log message to the Report Portal.
 
         :param time:       Time in UTC
-        :param message:    Log message
+        :param message:    Log message text
         :param level:      Message's log level
-        :param attachment: Message attachments
+        :param attachment: Message's attachments
         :param item_id:    ID of the RP item the message belongs to
         """
         self._log_manager.log(time, message, level, attachment, item_id)
 
     def start(self):
         """Start the client."""
         self._log_manager.start()
@@ -366,24 +367,24 @@
                         code_ref=None,
                         retry=False,
                         test_case_id=None,
                         **kwargs):
         """Start case/step/nested step item.
 
         :param name:           Name of the test item
-        :param start_time:     Test item start time
+        :param start_time:     The item start time
         :param item_type:      Type of the test item. Allowable values:
                                "suite", "story", "test", "scenario", "step",
                                "before_class", "before_groups",
                                "before_method", "before_suite",
                                "before_test", "after_class", "after_groups",
                                "after_method", "after_suite", "after_test"
         :param attributes:     Test item attributes
         :param code_ref:       Physical location of the test item
-        :param description:    Test item description
+        :param description:    The item description
         :param has_stats:      Set to False if test item is nested step
         :param parameters:     Set of parameters (for parametrized test items)
         :param parent_item_id: An ID of a parent SUITE / STEP
         :param retry:          Used to report retry of the test. Allowable
                                values: "True" or "False"
         :param test_case_id: A unique ID of the current step
         """
@@ -414,15 +415,14 @@
                                json=request_payload,
                                verify_ssl=self.verify_ssl).make()
         if not response:
             return
         item_id = response.id
         if item_id is not NOT_FOUND:
             logger.debug('start_test_item - ID: %s', item_id)
-            # noinspection PyUnresolvedReferences
             self._item_stack.append(item_id)
         else:
             logger.warning('start_test_item - invalid response: %s',
                            str(response.json))
         return item_id
 
     def terminate(self, *args, **kwargs):
@@ -448,9 +448,33 @@
         if not response:
             return
         logger.debug('update_test_item - Item: %s', item_id)
         return response.message
 
     def current_item(self):
         """Retrieve the last item reported by the client."""
-        # noinspection PyUnresolvedReferences
         return self._item_stack[-1] if len(self._item_stack) > 0 else None
+
+    def clone(self):
+        """Clone the client object, set current Item ID as cloned item ID.
+
+        :returns: Cloned client object
+        :rtype: RPClient
+        """
+        cloned = RPClient(
+            endpoint=self.endpoint,
+            project=self.project,
+            token=self.token,
+            log_batch_size=self.log_batch_size,
+            is_skipped_an_issue=self.is_skipped_an_issue,
+            verify_ssl=self.verify_ssl,
+            retries=self.retries,
+            max_pool_size=self.max_pool_size,
+            launch_id=self.launch_id,
+            http_timeout=self.http_timeout,
+            log_batch_payload_size=self.log_batch_payload_size,
+            mode=self.mode
+        )
+        current_item = self.current_item()
+        if current_item:
+            cloned._item_stack.append(current_item)
+        return cloned
```

### Comparing `reportportal-client-5.3.2/reportportal_client/client.pyi` & `reportportal-client-5.3.3/reportportal_client/client.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -20,32 +20,36 @@
     is_skipped_an_issue: bool = ...
     launch_id: Text = ...
     log_batch_size: int = ...
     log_batch_payload_size: int = ...
     project: Text = ...
     token: Text = ...
     verify_ssl: bool = ...
+    retries: int = ...
+    max_pool_size: int = ...
     http_timeout: Union[float, Tuple[float, float]] = ...
     session: Session = ...
     step_reporter: StepReporter = ...
     mode: str = ...
     _skip_analytics: Text = ...
+    _item_stack: List[Text] = ...
 
     def __init__(
             self,
             endpoint: Text,
             project: Text, token: Text,
             log_batch_size: int = ...,
             is_skipped_an_issue: bool = ...,
             verify_ssl: bool = ...,
             retries: int = ...,
             max_pool_size: int = ...,
             launch_id: Text = ...,
             http_timeout: Union[float, Tuple[float, float]] = ...,
-            log_batch_payload_size: int = ...
+            log_batch_payload_size: int = ...,
+            mode: str = ...
     ) -> None: ...
 
     def finish_launch(self,
                       end_time: Text,
                       status: Text = ...,
                       attributes: Optional[Union[List, Dict]] = ...,
                       **kwargs: Any) -> Dict: ...
@@ -102,7 +106,9 @@
     def update_test_item(self, item_uuid: Text,
                          attributes: Optional[Union[List, Dict]],
                          description: Optional[Text]) -> Text: ...
 
     def current_item(self) -> Text: ...
 
     def start(self) -> None : ...
+
+    def clone(self) -> RPClient: ...
```

### Comparing `reportportal-client-5.3.2/reportportal_client/core/__init__.py` & `reportportal-client-5.3.3/reportportal_client/core/__init__.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.2/reportportal_client/core/rp_file.py` & `reportportal-client-5.3.3/reportportal_client/core/rp_file.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.2/reportportal_client/core/rp_issues.py` & `reportportal-client-5.3.3/reportportal_client/core/rp_issues.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.2/reportportal_client/core/rp_requests.py` & `reportportal-client-5.3.3/reportportal_client/core/rp_requests.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.2/reportportal_client/core/rp_responses.py` & `reportportal-client-5.3.3/reportportal_client/core/rp_responses.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.2/reportportal_client/core/test_manager.py` & `reportportal-client-5.3.3/reportportal_client/core/test_manager.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.2/reportportal_client/core/worker.py` & `reportportal-client-5.3.3/reportportal_client/core/worker.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.2/reportportal_client/errors.py` & `reportportal-client-5.3.3/reportportal_client/errors.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.2/reportportal_client/helpers.py` & `reportportal-client-5.3.3/reportportal_client/helpers.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.2/reportportal_client/helpers.pyi` & `reportportal-client-5.3.3/reportportal_client/helpers.pyi`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.2/reportportal_client/items/__init__.py` & `reportportal-client-5.3.3/reportportal_client/items/__init__.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.2/reportportal_client/items/item_weight.py` & `reportportal-client-5.3.3/reportportal_client/items/item_weight.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.2/reportportal_client/items/rp_base_item.py` & `reportportal-client-5.3.3/reportportal_client/items/rp_base_item.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.2/reportportal_client/items/rp_log_items/__init__.py` & `reportportal-client-5.3.3/reportportal_client/items/rp_log_items/__init__.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.2/reportportal_client/items/rp_log_items/rp_log_item.py` & `reportportal-client-5.3.3/reportportal_client/items/rp_log_items/rp_log_item.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.2/reportportal_client/items/rp_test_items/__init__.py` & `reportportal-client-5.3.3/reportportal_client/items/rp_test_items/__init__.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.2/reportportal_client/items/rp_test_items/rp_base_test_item.py` & `reportportal-client-5.3.3/reportportal_client/items/rp_test_items/rp_base_test_item.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.2/reportportal_client/items/rp_test_items/rp_child_test_item.py` & `reportportal-client-5.3.3/reportportal_client/items/rp_test_items/rp_child_test_item.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.2/reportportal_client/items/rp_test_items/rp_root_test_item.py` & `reportportal-client-5.3.3/reportportal_client/items/rp_test_items/rp_root_test_item.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.2/reportportal_client/logs/__init__.py` & `reportportal-client-5.3.3/reportportal_client/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.2/reportportal_client/logs/log_manager.py` & `reportportal-client-5.3.3/reportportal_client/logs/log_manager.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.2/reportportal_client/services/__init__.py` & `reportportal-client-5.3.3/reportportal_client/services/__init__.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.2/reportportal_client/services/client_id.py` & `reportportal-client-5.3.3/reportportal_client/services/client_id.py`

 * *Files 7% similar despite different names*

```diff
@@ -75,15 +75,20 @@
                client_id)
     with open(RP_PROPERTIES_FILE_PATH, 'w') as fp:
         config.write(fp)
 
 
 def get_client_id():
     """Return unique client ID of the instance, generate new if not exists."""
-    client_id = _read_client_id()
+    client_id = None
+    try:
+        client_id = _read_client_id()
+    except (PermissionError, IOError) as error:
+        logger.exception('[%s] Unknown exception has occurred. '
+                         'Skipping client ID reading.', error)
     if not client_id:
         client_id = str(uuid4())
         try:
             _store_client_id(client_id)
         except (PermissionError, IOError) as error:
             logger.exception('[%s] Unknown exception has occurred. '
                              'Skipping client ID saving.', error)
```

### Comparing `reportportal-client-5.3.2/reportportal_client/services/constants.py` & `reportportal-client-5.3.3/reportportal_client/services/constants.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.2/reportportal_client/services/statistics.py` & `reportportal-client-5.3.3/reportportal_client/services/statistics.py`

 * *Files 13% similar despite different names*

```diff
@@ -50,37 +50,37 @@
      Use client and agent versions with their names.
 
     :param event_name: Event name to be used
     :param agent_name: Name of the agent that uses the client
     :param agent_version: Version of the agent
     """
     client_name, client_version = _get_client_info()
-    params = {
+    request_params = {
         'client_name': client_name,
         'client_version': client_version,
         'interpreter': _get_platform_info(),
         'agent_name': agent_name,
         'agent_version': agent_version,
     }
 
     if agent_name:
-        params['agent_name'] = agent_name
+        request_params['agent_name'] = agent_name
     if agent_version:
-        params['agent_version'] = agent_version
+        request_params['agent_version'] = agent_version
 
     payload = {
         'client_id': get_client_id(),
         'events': [{
             'name': event_name,
-            'params': params
+            'params': request_params
         }]
     }
     headers = {'User-Agent': 'python-requests'}
-    params = {
+    query_params = {
         'measurement_id': ID,
         'api_secret': KEY
     }
     try:
         return requests.post(url=ENDPOINT, json=payload, headers=headers,
-                             params=params)
+                             params=query_params)
     except requests.exceptions.RequestException as err:
         logger.debug('Failed to send data to Statistics service: %s', str(err))
```

### Comparing `reportportal-client-5.3.2/reportportal_client/static/__init__.py` & `reportportal-client-5.3.3/reportportal_client/static/__init__.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.2/reportportal_client/static/abstract.py` & `reportportal-client-5.3.3/reportportal_client/static/abstract.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.2/reportportal_client/static/defines.py` & `reportportal-client-5.3.3/reportportal_client/static/defines.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.2/reportportal_client/static/errors.py` & `reportportal-client-5.3.3/reportportal_client/static/errors.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.2/reportportal_client/steps/__init__.py` & `reportportal-client-5.3.3/reportportal_client/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.2/reportportal_client/steps/__init__.pyi` & `reportportal-client-5.3.3/reportportal_client/steps/__init__.pyi`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.2/reportportal_client.egg-info/PKG-INFO` & `reportportal-client-5.3.3/reportportal_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: reportportal-client
-Version: 5.3.2
+Version: 5.3.3
 Summary: Python client for Report Portal v5.
 Home-page: https://github.com/reportportal/client-Python
-Download-URL: https://github.com/reportportal/client-Python/tarball/5.3.2
+Download-URL: https://github.com/reportportal/client-Python/tarball/5.3.3
 Author: Report Portal Team
 Author-email: support@reportportal.io
 License: Apache 2.0.
 Keywords: testing,reporting,reportportal,client
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `reportportal-client-5.3.2/reportportal_client.egg-info/SOURCES.txt` & `reportportal-client-5.3.3/reportportal_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.2/setup.py` & `reportportal-client-5.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Config for setup package client Python."""
 
 import os
 
 from setuptools import setup, find_packages
 
-__version__ = '5.3.2'
+__version__ = '5.3.3'
 
 TYPE_STUBS = ['*.pyi']
 
 
 def read_file(fname):
     """Read the given file.
```

### Comparing `reportportal-client-5.3.2/tests/test_client_id.py` & `reportportal-client-5.3.3/tests/test_client_id.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.2/tests/test_helpers.py` & `reportportal-client-5.3.3/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.2/tests/test_statistics.py` & `reportportal-client-5.3.3/tests/test_statistics.py`

 * *Files identical despite different names*

