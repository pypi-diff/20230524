# Comparing `tmp/ai_transform-0.31.1.tar.gz` & `tmp/ai_transform-0.31.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_transform-0.31.1.tar", last modified: Fri May  5 02:23:05 2023, max compression
+gzip compressed data, was "ai_transform-0.31.2.tar", last modified: Wed May 24 02:24:50 2023, max compression
```

## Comparing `ai_transform-0.31.1.tar` & `ai_transform-0.31.2.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:23:05.548369 ai_transform-0.31.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-05-05 02:22:48.000000 ai_transform-0.31.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-05 02:23:05.548369 ai_transform-0.31.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-05-05 02:22:48.000000 ai_transform-0.31.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:23:05.544369 ai_transform-0.31.1/ai_transform/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:23:05.544369 ai_transform-0.31.1/ai_transform/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29452 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/api/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/api/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/api/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/api/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:23:05.544369 ai_transform-0.31.1/ai_transform/components/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/components/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:23:05.544369 ai_transform-0.31.1/ai_transform/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    15147 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/dataset/field.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:23:05.544369 ai_transform-0.31.1/ai_transform/engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15346 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/engine/abstract_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/engine/dense_output_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/engine/in_memory_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/engine/multipass_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/engine/small_batch_stable_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/engine/stable_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:23:05.544369 ai_transform-0.31.1/ai_transform/operator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/operator/abstract_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/operator/dense_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:23:05.544369 ai_transform-0.31.1/ai_transform/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/utils/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/utils/document_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/utils/encode_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/utils/example_documents.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/utils/json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/utils/keyphrase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:23:05.548369 ai_transform-0.31.1/ai_transform/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/workflow/abstract_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/workflow/context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/workflow/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:23:05.544369 ai_transform-0.31.1/ai_transform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-05 02:23:05.000000 ai_transform-0.31.1/ai_transform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-05-05 02:23:05.000000 ai_transform-0.31.1/ai_transform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 02:23:05.000000 ai_transform-0.31.1/ai_transform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-05 02:23:05.000000 ai_transform-0.31.1/ai_transform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-05 02:23:05.000000 ai_transform-0.31.1/ai_transform.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-05 02:22:48.000000 ai_transform-0.31.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 02:23:05.548369 ai_transform-0.31.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-05 02:22:48.000000 ai_transform-0.31.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:23:05.548369 ai_transform-0.31.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 02:22:48.000000 ai_transform-0.31.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-05 02:22:48.000000 ai_transform-0.31.1/tests/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    11140 2023-05-05 02:22:48.000000 ai_transform-0.31.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:23:05.548369 ai_transform-0.31.1/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 02:22:48.000000 ai_transform-0.31.1/tests/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:23:05.548369 ai_transform-0.31.1/tests/core/test_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 02:22:48.000000 ai_transform-0.31.1/tests/core/test_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-05 02:22:48.000000 ai_transform-0.31.1/tests/core/test_api/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-05 02:22:48.000000 ai_transform-0.31.1/tests/core/test_api/test_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-05 02:22:48.000000 ai_transform-0.31.1/tests/core/test_api/test_keyphrase.py
--rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-05-05 02:22:48.000000 ai_transform-0.31.1/tests/core/test_api/test_wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:23:05.548369 ai_transform-0.31.1/tests/core/test_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 02:22:48.000000 ai_transform-0.31.1/tests/core/test_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-05-05 02:22:48.000000 ai_transform-0.31.1/tests/core/test_dataset/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-05 02:22:48.000000 ai_transform-0.31.1/tests/core/test_dataset/test_field.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-05 02:22:48.000000 ai_transform-0.31.1/tests/core/test_dataset/test_keyphrase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:23:05.548369 ai_transform-0.31.1/tests/core/test_engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 02:22:48.000000 ai_transform-0.31.1/tests/core/test_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-05 02:22:48.000000 ai_transform-0.31.1/tests/core/test_engine/test_dense_output_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-05 02:22:48.000000 ai_transform-0.31.1/tests/core/test_engine/test_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-05 02:22:48.000000 ai_transform-0.31.1/tests/core/test_engine/test_engine_playground.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-05-05 02:22:48.000000 ai_transform-0.31.1/tests/core/test_engine/test_multipass_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-05 02:22:48.000000 ai_transform-0.31.1/tests/core/test_engine/test_stable_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:23:05.548369 ai_transform-0.31.1/tests/core/test_operator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 02:22:48.000000 ai_transform-0.31.1/tests/core/test_operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-05 02:22:48.000000 ai_transform-0.31.1/tests/core/test_operator/test_abstract_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-05 02:22:48.000000 ai_transform-0.31.1/tests/core/test_operator/test_document_diff.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:23:05.548369 ai_transform-0.31.1/tests/core/test_workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 02:22:48.000000 ai_transform-0.31.1/tests/core/test_workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-05 02:22:48.000000 ai_transform-0.31.1/tests/core/test_workflow/test_context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-05-05 02:22:48.000000 ai_transform-0.31.1/tests/core/test_workflow/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-05 02:22:48.000000 ai_transform-0.31.1/tests/test_connection_retry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 02:24:50.026236 ai_transform-0.31.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-05-24 02:24:28.000000 ai_transform-0.31.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-24 02:24:50.026236 ai_transform-0.31.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-05-24 02:24:28.000000 ai_transform-0.31.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 02:24:50.002236 ai_transform-0.31.2/ai_transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-24 02:24:28.000000 ai_transform-0.31.2/ai_transform/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 02:24:50.006236 ai_transform-0.31.2/ai_transform/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 02:24:28.000000 ai_transform-0.31.2/ai_transform/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29452 2023-05-24 02:24:28.000000 ai_transform-0.31.2/ai_transform/api/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-05-24 02:24:28.000000 ai_transform-0.31.2/ai_transform/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-24 02:24:28.000000 ai_transform-0.31.2/ai_transform/api/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-24 02:24:28.000000 ai_transform-0.31.2/ai_transform/api/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-24 02:24:28.000000 ai_transform-0.31.2/ai_transform/api/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 02:24:50.006236 ai_transform-0.31.2/ai_transform/components/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-24 02:24:28.000000 ai_transform-0.31.2/ai_transform/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-05-24 02:24:28.000000 ai_transform-0.31.2/ai_transform/components/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-05-24 02:24:28.000000 ai_transform-0.31.2/ai_transform/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-24 02:24:28.000000 ai_transform-0.31.2/ai_transform/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 02:24:50.006236 ai_transform-0.31.2/ai_transform/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 02:24:28.000000 ai_transform-0.31.2/ai_transform/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-05-24 02:24:28.000000 ai_transform-0.31.2/ai_transform/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15147 2023-05-24 02:24:28.000000 ai_transform-0.31.2/ai_transform/dataset/field.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 02:24:50.010236 ai_transform-0.31.2/ai_transform/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 02:24:28.000000 ai_transform-0.31.2/ai_transform/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15346 2023-05-24 02:24:28.000000 ai_transform-0.31.2/ai_transform/engine/abstract_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-05-24 02:24:28.000000 ai_transform-0.31.2/ai_transform/engine/dense_output_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-24 02:24:28.000000 ai_transform-0.31.2/ai_transform/engine/in_memory_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-05-24 02:24:28.000000 ai_transform-0.31.2/ai_transform/engine/multipass_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-05-24 02:24:28.000000 ai_transform-0.31.2/ai_transform/engine/small_batch_stable_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-05-24 02:24:28.000000 ai_transform-0.31.2/ai_transform/engine/stable_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-24 02:24:28.000000 ai_transform-0.31.2/ai_transform/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-24 02:24:28.000000 ai_transform-0.31.2/ai_transform/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 02:24:50.010236 ai_transform-0.31.2/ai_transform/operator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 02:24:28.000000 ai_transform-0.31.2/ai_transform/operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-05-24 02:24:28.000000 ai_transform-0.31.2/ai_transform/operator/abstract_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-24 02:24:28.000000 ai_transform-0.31.2/ai_transform/operator/dense_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-24 02:24:28.000000 ai_transform-0.31.2/ai_transform/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-24 02:24:28.000000 ai_transform-0.31.2/ai_transform/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 02:24:50.014236 ai_transform-0.31.2/ai_transform/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-24 02:24:28.000000 ai_transform-0.31.2/ai_transform/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-05-24 02:24:28.000000 ai_transform-0.31.2/ai_transform/utils/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-05-24 02:24:28.000000 ai_transform-0.31.2/ai_transform/utils/document_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-24 02:24:28.000000 ai_transform-0.31.2/ai_transform/utils/encode_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-05-24 02:24:28.000000 ai_transform-0.31.2/ai_transform/utils/example_documents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-24 02:24:28.000000 ai_transform-0.31.2/ai_transform/utils/json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-24 02:24:28.000000 ai_transform-0.31.2/ai_transform/utils/keyphrase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 02:24:50.014236 ai_transform-0.31.2/ai_transform/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-24 02:24:28.000000 ai_transform-0.31.2/ai_transform/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-05-24 02:24:28.000000 ai_transform-0.31.2/ai_transform/workflow/abstract_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-05-24 02:24:28.000000 ai_transform-0.31.2/ai_transform/workflow/context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-05-24 02:24:28.000000 ai_transform-0.31.2/ai_transform/workflow/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 02:24:50.002236 ai_transform-0.31.2/ai_transform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-24 02:24:49.000000 ai_transform-0.31.2/ai_transform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-05-24 02:24:49.000000 ai_transform-0.31.2/ai_transform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 02:24:49.000000 ai_transform-0.31.2/ai_transform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-24 02:24:49.000000 ai_transform-0.31.2/ai_transform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-24 02:24:49.000000 ai_transform-0.31.2/ai_transform.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-24 02:24:28.000000 ai_transform-0.31.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 02:24:50.026236 ai_transform-0.31.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-24 02:24:28.000000 ai_transform-0.31.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 02:24:50.014236 ai_transform-0.31.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 02:24:28.000000 ai_transform-0.31.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-24 02:24:28.000000 ai_transform-0.31.2/tests/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11140 2023-05-24 02:24:28.000000 ai_transform-0.31.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 02:24:50.018236 ai_transform-0.31.2/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 02:24:28.000000 ai_transform-0.31.2/tests/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 02:24:50.018236 ai_transform-0.31.2/tests/core/test_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 02:24:28.000000 ai_transform-0.31.2/tests/core/test_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-24 02:24:28.000000 ai_transform-0.31.2/tests/core/test_api/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-24 02:24:28.000000 ai_transform-0.31.2/tests/core/test_api/test_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-24 02:24:28.000000 ai_transform-0.31.2/tests/core/test_api/test_keyphrase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-05-24 02:24:28.000000 ai_transform-0.31.2/tests/core/test_api/test_wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 02:24:50.018236 ai_transform-0.31.2/tests/core/test_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 02:24:28.000000 ai_transform-0.31.2/tests/core/test_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-05-24 02:24:28.000000 ai_transform-0.31.2/tests/core/test_dataset/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-24 02:24:28.000000 ai_transform-0.31.2/tests/core/test_dataset/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-24 02:24:28.000000 ai_transform-0.31.2/tests/core/test_dataset/test_keyphrase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 02:24:50.022236 ai_transform-0.31.2/tests/core/test_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 02:24:28.000000 ai_transform-0.31.2/tests/core/test_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-24 02:24:28.000000 ai_transform-0.31.2/tests/core/test_engine/test_dense_output_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-24 02:24:28.000000 ai_transform-0.31.2/tests/core/test_engine/test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-24 02:24:28.000000 ai_transform-0.31.2/tests/core/test_engine/test_engine_playground.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-05-24 02:24:28.000000 ai_transform-0.31.2/tests/core/test_engine/test_multipass_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-24 02:24:28.000000 ai_transform-0.31.2/tests/core/test_engine/test_stable_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 02:24:50.026236 ai_transform-0.31.2/tests/core/test_operator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 02:24:28.000000 ai_transform-0.31.2/tests/core/test_operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-24 02:24:28.000000 ai_transform-0.31.2/tests/core/test_operator/test_abstract_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-24 02:24:28.000000 ai_transform-0.31.2/tests/core/test_operator/test_document_diff.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 02:24:50.026236 ai_transform-0.31.2/tests/core/test_workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 02:24:28.000000 ai_transform-0.31.2/tests/core/test_workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-24 02:24:28.000000 ai_transform-0.31.2/tests/core/test_workflow/test_context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-05-24 02:24:28.000000 ai_transform-0.31.2/tests/core/test_workflow/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-24 02:24:28.000000 ai_transform-0.31.2/tests/test_connection_retry.py
```

### Comparing `ai_transform-0.31.1/LICENSE` & `ai_transform-0.31.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.1/README.md` & `ai_transform-0.31.2/README.md`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.1/ai_transform/__init__.py` & `ai_transform-0.31.2/ai_transform/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.31.1"
+__version__ = "0.31.2"
 
 from ai_transform.timer import Timer
 
 _TIMER = Timer()
 _TIMER.start()
```

### Comparing `ai_transform-0.31.1/ai_transform/api/api.py` & `ai_transform-0.31.2/ai_transform/api/api.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.1/ai_transform/api/client.py` & `ai_transform-0.31.2/ai_transform/api/client.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.1/ai_transform/api/helpers.py` & `ai_transform-0.31.2/ai_transform/api/helpers.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.1/ai_transform/api/wrappers.py` & `ai_transform-0.31.2/ai_transform/api/wrappers.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.1/ai_transform/components/components.py` & `ai_transform-0.31.2/ai_transform/components/components.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.1/ai_transform/config.py` & `ai_transform-0.31.2/ai_transform/config.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.1/ai_transform/dataset/dataset.py` & `ai_transform-0.31.2/ai_transform/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.1/ai_transform/dataset/field.py` & `ai_transform-0.31.2/ai_transform/dataset/field.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.1/ai_transform/engine/abstract_engine.py` & `ai_transform-0.31.2/ai_transform/engine/abstract_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.1/ai_transform/engine/dense_output_engine.py` & `ai_transform-0.31.2/ai_transform/engine/dense_output_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.1/ai_transform/engine/in_memory_engine.py` & `ai_transform-0.31.2/ai_transform/engine/in_memory_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.1/ai_transform/engine/multipass_engine.py` & `ai_transform-0.31.2/ai_transform/engine/multipass_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.1/ai_transform/engine/small_batch_stable_engine.py` & `ai_transform-0.31.2/ai_transform/engine/small_batch_stable_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.1/ai_transform/engine/stable_engine.py` & `ai_transform-0.31.2/ai_transform/engine/stable_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.1/ai_transform/errors.py` & `ai_transform-0.31.2/ai_transform/errors.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.1/ai_transform/logger.py` & `ai_transform-0.31.2/ai_transform/logger.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.1/ai_transform/operator/abstract_operator.py` & `ai_transform-0.31.2/ai_transform/operator/abstract_operator.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.1/ai_transform/operator/dense_operator.py` & `ai_transform-0.31.2/ai_transform/operator/dense_operator.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.1/ai_transform/timer.py` & `ai_transform-0.31.2/ai_transform/timer.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.1/ai_transform/types.py` & `ai_transform-0.31.2/ai_transform/types.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.1/ai_transform/utils/document.py` & `ai_transform-0.31.2/ai_transform/utils/document.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.1/ai_transform/utils/document_list.py` & `ai_transform-0.31.2/ai_transform/utils/document_list.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.1/ai_transform/utils/example_documents.py` & `ai_transform-0.31.2/ai_transform/utils/example_documents.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.1/ai_transform/utils/json_encoder.py` & `ai_transform-0.31.2/ai_transform/utils/json_encoder.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.1/ai_transform/utils/keyphrase.py` & `ai_transform-0.31.2/ai_transform/utils/keyphrase.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.1/ai_transform/workflow/abstract_workflow.py` & `ai_transform-0.31.2/ai_transform/workflow/abstract_workflow.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.1/ai_transform/workflow/context_manager.py` & `ai_transform-0.31.2/ai_transform/workflow/context_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 import os
-import logging
-import requests
 
 from inspect import Traceback
 from typing import Dict, Any, List
 
 from ai_transform.api.api import API
 from ai_transform.types import Credentials
 from ai_transform.dataset import dataset
 from ai_transform.operator import abstract_operator
 from ai_transform.engine import abstract_engine
-from ai_transform.logger import format_logging_info
-from ai_transform.api.wrappers import request_wrapper
-from ai_transform.errors import UserFacingError
 from ai_transform.logger import ic
 
-WORKFLOW_FAIL_MESSAGE = (
-    "Workflow processed {:.2f}%" + " of documents. This is less than the success threshold of {:.2f}%"
-)
+
+WORKFLOW_PROCESSED_MESSAGE = "Workflow processed {:.2f}%" + " of documents. "
+
+WORKFLOW_FAIL_MESSAGE = WORKFLOW_PROCESSED_MESSAGE + "This is less than the success threshold of {:.2f}%"
 
 
 class WorkflowContextManager:
 
     FAILED = "failed"
     COMPLETE = "complete"
     IN_PROGRESS = "inprogress"
@@ -190,14 +186,16 @@
         )
 
     def __exit__(self, exc_type: type, exc_value: BaseException, traceback: Traceback):
         regular_workflow_failed = False
         user_errors = None
 
         if self.engine is not None:
+            self.addtional_message = WORKFLOW_PROCESSED_MESSAGE.format(100 * self.engine.success_ratio)
+
             regular_workflow_failed = self.engine.success_ratio < self.success_threshold
 
             if regular_workflow_failed:
                 user_errors = WORKFLOW_FAIL_MESSAGE.format(
                     100 * self.engine.success_ratio, 100 * self.success_threshold
                 )
```

### Comparing `ai_transform-0.31.1/ai_transform/workflow/helpers.py` & `ai_transform-0.31.2/ai_transform/workflow/helpers.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.1/ai_transform.egg-info/SOURCES.txt` & `ai_transform-0.31.2/ai_transform.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.1/setup.py` & `ai_transform-0.31.2/setup.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.1/tests/conftest.py` & `ai_transform-0.31.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.1/tests/core/test_api/test_client.py` & `ai_transform-0.31.2/tests/core/test_api/test_client.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.1/tests/core/test_api/test_endpoints.py` & `ai_transform-0.31.2/tests/core/test_api/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.1/tests/core/test_api/test_keyphrase.py` & `ai_transform-0.31.2/tests/core/test_api/test_keyphrase.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.1/tests/core/test_api/test_wrappers.py` & `ai_transform-0.31.2/tests/core/test_api/test_wrappers.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.1/tests/core/test_dataset/test_dataset.py` & `ai_transform-0.31.2/tests/core/test_dataset/test_dataset.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.1/tests/core/test_dataset/test_field.py` & `ai_transform-0.31.2/tests/core/test_dataset/test_field.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.1/tests/core/test_dataset/test_keyphrase.py` & `ai_transform-0.31.2/tests/core/test_dataset/test_keyphrase.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.1/tests/core/test_engine/test_dense_output_engine.py` & `ai_transform-0.31.2/tests/core/test_engine/test_dense_output_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.1/tests/core/test_engine/test_engine.py` & `ai_transform-0.31.2/tests/core/test_engine/test_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.1/tests/core/test_engine/test_engine_playground.py` & `ai_transform-0.31.2/tests/core/test_engine/test_engine_playground.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.1/tests/core/test_engine/test_multipass_engine.py` & `ai_transform-0.31.2/tests/core/test_engine/test_multipass_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.1/tests/core/test_engine/test_stable_engine.py` & `ai_transform-0.31.2/tests/core/test_engine/test_stable_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.1/tests/core/test_operator/test_abstract_operator.py` & `ai_transform-0.31.2/tests/core/test_operator/test_abstract_operator.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.1/tests/core/test_operator/test_document_diff.py` & `ai_transform-0.31.2/tests/core/test_operator/test_document_diff.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.1/tests/core/test_workflow/test_context_manager.py` & `ai_transform-0.31.2/tests/core/test_workflow/test_context_manager.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.1/tests/core/test_workflow/test_workflow.py` & `ai_transform-0.31.2/tests/core/test_workflow/test_workflow.py`

 * *Files identical despite different names*

