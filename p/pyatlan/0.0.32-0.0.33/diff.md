# Comparing `tmp/pyatlan-0.0.32.tar.gz` & `tmp/pyatlan-0.0.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyatlan-0.0.32.tar", last modified: Thu May 18 17:20:32 2023, max compression
+gzip compressed data, was "pyatlan-0.0.33.tar", last modified: Wed May 24 15:25:52 2023, max compression
```

## Comparing `pyatlan-0.0.32.tar` & `pyatlan-0.0.33.tar`

### file list

```diff
@@ -1,73 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:20:32.792536 pyatlan-0.0.32/
--rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-05-18 17:20:21.000000 pyatlan-0.0.32/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-18 17:20:21.000000 pyatlan-0.0.32/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-18 17:20:21.000000 pyatlan-0.0.32/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-18 17:20:32.792536 pyatlan-0.0.32/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-18 17:20:21.000000 pyatlan-0.0.32/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:20:32.784536 pyatlan-0.0.32/pyatlan/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-18 17:20:21.000000 pyatlan-0.0.32/pyatlan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:20:32.788536 pyatlan-0.0.32/pyatlan/cache/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-18 17:20:21.000000 pyatlan-0.0.32/pyatlan/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-18 17:20:21.000000 pyatlan-0.0.32/pyatlan/cache/classification_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    11601 2023-05-18 17:20:21.000000 pyatlan-0.0.32/pyatlan/cache/custom_metadata_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-18 17:20:21.000000 pyatlan-0.0.32/pyatlan/cache/enum_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-18 17:20:21.000000 pyatlan-0.0.32/pyatlan/cache/group_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-18 17:20:21.000000 pyatlan-0.0.32/pyatlan/cache/role_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:20:32.788536 pyatlan-0.0.32/pyatlan/client/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-18 17:20:21.000000 pyatlan-0.0.32/pyatlan/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34780 2023-05-18 17:20:21.000000 pyatlan-0.0.32/pyatlan/client/atlan.py
--rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-05-18 17:20:21.000000 pyatlan-0.0.32/pyatlan/client/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-05-18 17:20:21.000000 pyatlan-0.0.32/pyatlan/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-05-18 17:20:21.000000 pyatlan-0.0.32/pyatlan/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:20:32.788536 pyatlan-0.0.32/pyatlan/generator/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-18 17:20:21.000000 pyatlan-0.0.32/pyatlan/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5689 2023-05-18 17:20:21.000000 pyatlan-0.0.32/pyatlan/generator/generate_from_typdefs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:20:32.788536 pyatlan-0.0.32/pyatlan/generator/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-18 17:20:21.000000 pyatlan-0.0.32/pyatlan/generator/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:20:32.788536 pyatlan-0.0.32/pyatlan/model/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-18 17:20:21.000000 pyatlan-0.0.32/pyatlan/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   958128 2023-05-18 17:20:21.000000 pyatlan-0.0.32/pyatlan/model/assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-05-18 17:20:21.000000 pyatlan-0.0.32/pyatlan/model/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     9593 2023-05-18 17:20:21.000000 pyatlan-0.0.32/pyatlan/model/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-05-18 17:20:21.000000 pyatlan-0.0.32/pyatlan/model/group.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-18 17:20:21.000000 pyatlan-0.0.32/pyatlan/model/internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     8110 2023-05-18 17:20:21.000000 pyatlan-0.0.32/pyatlan/model/lineage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-05-18 17:20:21.000000 pyatlan-0.0.32/pyatlan/model/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-18 17:20:21.000000 pyatlan-0.0.32/pyatlan/model/role.py
--rw-r--r--   0 runner    (1001) docker     (123)    59796 2023-05-18 17:20:21.000000 pyatlan-0.0.32/pyatlan/model/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     8458 2023-05-18 17:20:21.000000 pyatlan-0.0.32/pyatlan/model/structs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24312 2023-05-18 17:20:21.000000 pyatlan-0.0.32/pyatlan/model/typedef.py
--rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-05-18 17:20:21.000000 pyatlan-0.0.32/pyatlan/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-18 17:20:21.000000 pyatlan-0.0.32/pyatlan/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:20:32.784536 pyatlan-0.0.32/pyatlan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-18 17:20:32.000000 pyatlan-0.0.32/pyatlan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-18 17:20:32.000000 pyatlan-0.0.32/pyatlan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 17:20:32.000000 pyatlan-0.0.32/pyatlan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 17:20:32.000000 pyatlan-0.0.32/pyatlan.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-18 17:20:32.000000 pyatlan-0.0.32/pyatlan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-18 17:20:32.000000 pyatlan-0.0.32/pyatlan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 17:20:32.792536 pyatlan-0.0.32/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-05-18 17:20:21.000000 pyatlan-0.0.32/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:20:32.788536 pyatlan-0.0.32/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-18 17:20:21.000000 pyatlan-0.0.32/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-18 17:20:21.000000 pyatlan-0.0.32/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:20:32.792536 pyatlan-0.0.32/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-18 17:20:21.000000 pyatlan-0.0.32/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-05-18 17:20:21.000000 pyatlan-0.0.32/tests/integration/admin_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-05-18 17:20:21.000000 pyatlan-0.0.32/tests/integration/classification_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-18 17:20:21.000000 pyatlan-0.0.32/tests/integration/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    35863 2023-05-18 17:20:21.000000 pyatlan-0.0.32/tests/integration/custom_metadata_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-05-18 17:20:21.000000 pyatlan-0.0.32/tests/integration/glossary_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-05-18 17:20:21.000000 pyatlan-0.0.32/tests/integration/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    34056 2023-05-18 17:20:21.000000 pyatlan-0.0.32/tests/integration/test_entity_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-05-18 17:20:21.000000 pyatlan-0.0.32/tests/integration/test_index_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:20:32.792536 pyatlan-0.0.32/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-18 17:20:21.000000 pyatlan-0.0.32/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-18 17:20:21.000000 pyatlan-0.0.32/tests/unit/test_classification_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     9647 2023-05-18 17:20:21.000000 pyatlan-0.0.32/tests/unit/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-05-18 17:20:21.000000 pyatlan-0.0.32/tests/unit/test_glossary_term.py
--rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-05-18 17:20:21.000000 pyatlan-0.0.32/tests/unit/test_lineage.py
--rw-r--r--   0 runner    (1001) docker     (123)    64373 2023-05-18 17:20:21.000000 pyatlan-0.0.32/tests/unit/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    31770 2023-05-18 17:20:21.000000 pyatlan-0.0.32/tests/unit/test_search_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-05-18 17:20:21.000000 pyatlan-0.0.32/tests/unit/test_typedef_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-18 17:20:21.000000 pyatlan-0.0.32/tests/unit/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:25:52.332696 pyatlan-0.0.33/
+-rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-05-24 15:25:40.000000 pyatlan-0.0.33/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-24 15:25:40.000000 pyatlan-0.0.33/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-24 15:25:40.000000 pyatlan-0.0.33/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-24 15:25:52.332696 pyatlan-0.0.33/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-24 15:25:40.000000 pyatlan-0.0.33/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:25:52.324695 pyatlan-0.0.33/pyatlan/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:25:52.324695 pyatlan-0.0.33/pyatlan/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/cache/classification_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11601 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/cache/custom_metadata_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/cache/enum_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/cache/group_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/cache/role_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/cache/user_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:25:52.324695 pyatlan-0.0.33/pyatlan/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40525 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/client/atlan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8442 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:25:52.324695 pyatlan-0.0.33/pyatlan/generator/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/generator/generate_from_typdefs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:25:52.324695 pyatlan-0.0.33/pyatlan/generator/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/generator/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:25:52.328695 pyatlan-0.0.33/pyatlan/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   828487 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/model/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/model/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9768 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/model/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/model/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/model/internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8110 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/model/lineage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/model/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/model/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59796 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/model/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8458 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/model/structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24322 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/model/typedef.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/model/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:25:52.324695 pyatlan-0.0.33/pyatlan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-24 15:25:52.000000 pyatlan-0.0.33/pyatlan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-24 15:25:52.000000 pyatlan-0.0.33/pyatlan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:25:52.000000 pyatlan-0.0.33/pyatlan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:25:52.000000 pyatlan-0.0.33/pyatlan.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-24 15:25:52.000000 pyatlan-0.0.33/pyatlan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-24 15:25:52.000000 pyatlan-0.0.33/pyatlan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 15:25:52.332696 pyatlan-0.0.33/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-05-24 15:25:40.000000 pyatlan-0.0.33/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:25:52.328695 pyatlan-0.0.33/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-24 15:25:40.000000 pyatlan-0.0.33/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-24 15:25:40.000000 pyatlan-0.0.33/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:25:52.328695 pyatlan-0.0.33/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-24 15:25:40.000000 pyatlan-0.0.33/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-05-24 15:25:40.000000 pyatlan-0.0.33/tests/integration/admin_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-05-24 15:25:40.000000 pyatlan-0.0.33/tests/integration/classification_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-24 15:25:40.000000 pyatlan-0.0.33/tests/integration/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37526 2023-05-24 15:25:40.000000 pyatlan-0.0.33/tests/integration/custom_metadata_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-05-24 15:25:40.000000 pyatlan-0.0.33/tests/integration/glossary_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-05-24 15:25:40.000000 pyatlan-0.0.33/tests/integration/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34056 2023-05-24 15:25:40.000000 pyatlan-0.0.33/tests/integration/test_entity_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-05-24 15:25:40.000000 pyatlan-0.0.33/tests/integration/test_index_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:25:52.332696 pyatlan-0.0.33/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-24 15:25:40.000000 pyatlan-0.0.33/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-24 15:25:40.000000 pyatlan-0.0.33/tests/unit/test_classification_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-05-24 15:25:40.000000 pyatlan-0.0.33/tests/unit/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-05-24 15:25:40.000000 pyatlan-0.0.33/tests/unit/test_glossary_term.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-05-24 15:25:40.000000 pyatlan-0.0.33/tests/unit/test_lineage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73762 2023-05-24 15:25:40.000000 pyatlan-0.0.33/tests/unit/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31770 2023-05-24 15:25:40.000000 pyatlan-0.0.33/tests/unit/test_search_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-05-24 15:25:40.000000 pyatlan-0.0.33/tests/unit/test_typedef_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-24 15:25:40.000000 pyatlan-0.0.33/tests/unit/test_utils.py
```

### Comparing `pyatlan-0.0.32/LICENSE` & `pyatlan-0.0.33/LICENSE`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.32/PKG-INFO` & `pyatlan-0.0.33/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatlan
-Version: 0.0.32
+Version: 0.0.33
 Summary: Atlan Python Client
 Home-page: https://github.com/atlanhq/atlan-python
 Author: Atlan Technologies Pvt Ltd
 Author-email: engineering@atlan.com
 License: Apache LICENSE 2.0
 Keywords: atlan client
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyatlan-0.0.32/README.md` & `pyatlan-0.0.33/README.md`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.32/pyatlan/cache/classification_cache.py` & `pyatlan-0.0.33/pyatlan/cache/classification_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.32/pyatlan/cache/custom_metadata_cache.py` & `pyatlan-0.0.33/pyatlan/cache/custom_metadata_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.32/pyatlan/cache/enum_cache.py` & `pyatlan-0.0.33/pyatlan/cache/enum_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.32/pyatlan/cache/group_cache.py` & `pyatlan-0.0.33/pyatlan/cache/group_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.32/pyatlan/cache/role_cache.py` & `pyatlan-0.0.33/pyatlan/cache/role_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.32/pyatlan/client/atlan.py` & `pyatlan-0.0.33/pyatlan/client/atlan.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,32 +17,42 @@
     validate_arguments,
 )
 from requests.adapters import HTTPAdapter
 from urllib3.util.retry import Retry
 
 from pyatlan.client.constants import (
     ADD_BUSINESS_ATTRIBUTE_BY_ID,
+    ADD_USER_TO_GROUPS,
     BULK_UPDATE,
+    CHANGE_USER_ROLE,
+    CREATE_GROUP,
     CREATE_TYPE_DEFS,
-    UPDATE_TYPE_DEFS,
+    CREATE_USERS,
     DELETE_ENTITY_BY_ATTRIBUTE,
     DELETE_ENTITY_BY_GUID,
+    DELETE_GROUP,
     DELETE_TYPE_DEF_BY_NAME,
+    DELETE_USER,
     GET_ALL_TYPE_DEFS,
+    GET_CURRENT_USER,
     GET_ENTITY_BY_GUID,
     GET_ENTITY_BY_UNIQUE_ATTRIBUTE,
+    GET_GROUP_MEMBERS,
+    GET_GROUPS,
     GET_LINEAGE,
     GET_ROLES,
-    GET_GROUPS,
+    GET_USER_GROUPS,
+    GET_USERS,
     INDEX_SEARCH,
     PARTIAL_UPDATE_ENTITY_BY_ATTRIBUTE,
+    REMOVE_USERS_FROM_GROUP,
     UPDATE_ENTITY_BY_ATTRIBUTE,
-    CREATE_GROUP,
-    DELETE_GROUP,
     UPDATE_GROUP,
+    UPDATE_TYPE_DEFS,
+    UPDATE_USER,
 )
 from pyatlan.error import AtlanError, NotFoundError
 from pyatlan.exceptions import AtlanServiceException, InvalidRequestException
 from pyatlan.model.assets import (
     Asset,
     AtlasGlossary,
     AtlasGlossaryCategory,
@@ -70,30 +80,39 @@
 from pyatlan.model.enums import (
     AtlanConnectorType,
     AtlanDeleteType,
     AtlanTypeCategory,
     CertificateStatus,
 )
 from pyatlan.model.group import (
-    GroupResponse,
     AtlanGroup,
-    CreateGroupResponse,
     CreateGroupRequest,
+    CreateGroupResponse,
+    GroupResponse,
+    RemoveFromGroupRequest,
 )
 from pyatlan.model.lineage import LineageRequest, LineageResponse
 from pyatlan.model.response import AssetMutationResponse
 from pyatlan.model.role import RoleResponse
 from pyatlan.model.search import DSL, IndexSearchRequest, Term
 from pyatlan.model.typedef import (
     ClassificationDef,
     CustomMetadataDef,
     EnumDef,
     TypeDef,
     TypeDefResponse,
 )
+from pyatlan.model.user import (
+    AddToGroupsRequest,
+    AtlanUser,
+    ChangeRoleRequest,
+    CreateUserRequest,
+    UserMinimalResponse,
+    UserResponse,
+)
 from pyatlan.utils import HTTPStatus, get_logger
 
 LOGGER = get_logger()
 T = TypeVar("T", bound=Referenceable)
 A = TypeVar("A", bound=Asset)
 Assets = Union[
     AtlasGlossary,
@@ -367,15 +386,17 @@
         return RoleResponse(**raw_json)
 
     def create_group(
         self,
         group: AtlanGroup,
         user_ids: Optional[list[str]] = None,
     ) -> CreateGroupResponse:
-        payload = CreateGroupRequest(group=group, user_ids=user_ids)
+        payload = CreateGroupRequest(group=group)
+        if user_ids:
+            payload.users = user_ids
         raw_json = self._call_api(CREATE_GROUP, request_obj=payload, exclude_unset=True)
         return CreateGroupResponse(**raw_json)
 
     def update_group(
         self,
         group: AtlanGroup,
     ) -> None:
@@ -444,14 +465,177 @@
             offset=0,
             limit=limit,
             post_filter='{"$and":[{"alias":{"$ilike":"%' + alias + '%"}}]}',
         ):
             return response.records
         return None
 
+    def get_group_members(self, guid: str) -> UserResponse:
+        """
+        Retrieves the members (users) of a group.
+        """
+        raw_json = self._call_api(GET_GROUP_MEMBERS.format_path({"group_guid": guid}))
+        return UserResponse(**raw_json)
+
+    def remove_users_from_group(self, guid: str, user_ids=list[str]) -> None:
+        """
+        Remove one or more users from a group.
+        """
+        rfgr = RemoveFromGroupRequest(users=user_ids)
+        self._call_api(
+            REMOVE_USERS_FROM_GROUP.format_path({"group_guid": guid}),
+            request_obj=rfgr,
+            exclude_unset=True,
+        )
+
+    def create_users(
+        self,
+        users: list[AtlanUser],
+    ) -> None:
+        from pyatlan.cache.role_cache import RoleCache
+
+        cur = CreateUserRequest(users=[])
+        for user in users:
+            role_name = str(user.workspace_role)
+            if role_id := RoleCache.get_id_for_name(role_name):
+                to_create = CreateUserRequest.CreateUser(
+                    email=user.email,
+                    role_name=role_name,
+                    role_id=role_id,
+                )
+                cur.users.append(to_create)
+        self._call_api(CREATE_USERS, request_obj=cur, exclude_unset=True)
+
+    def update_user(
+        self,
+        guid: str,
+        user: AtlanUser,
+    ) -> UserMinimalResponse:
+        raw_json = self._call_api(
+            UPDATE_USER.format_path_with_params(guid),
+            request_obj=user,
+            exclude_unset=True,
+        )
+        return UserMinimalResponse(**raw_json)
+
+    def purge_user(
+        self,
+        guid: str,
+    ) -> None:
+        self._call_api(DELETE_USER.format_path({"user_guid": guid}))
+
+    def get_groups_for_user(
+        self,
+        guid: str,
+    ) -> GroupResponse:
+        raw_json = self._call_api(GET_USER_GROUPS.format_path({"user_guid": guid}))
+        return GroupResponse(**raw_json)
+
+    def add_user_to_groups(
+        self,
+        guid: str,
+        group_ids: list[str],
+    ) -> None:
+        atgr = AddToGroupsRequest(groups=group_ids)
+        self._call_api(
+            ADD_USER_TO_GROUPS.format_path({"user_guid": guid}),
+            request_obj=atgr,
+            exclude_unset=True,
+        )
+
+    def change_user_role(
+        self,
+        guid: str,
+        role_id: str,
+    ) -> None:
+        crr = ChangeRoleRequest(role_id=role_id)
+        self._call_api(
+            CHANGE_USER_ROLE.format_path({"user_guid": guid}),
+            request_obj=crr,
+            exclude_unset=True,
+        )
+
+    def get_current_user(
+        self,
+    ) -> UserMinimalResponse:
+        raw_json = self._call_api(GET_CURRENT_USER)
+        return UserMinimalResponse(**raw_json)
+
+    def get_users(
+        self,
+        limit: Optional[int] = None,
+        post_filter: Optional[str] = None,
+        sort: Optional[str] = None,
+        count: bool = True,
+        offset: int = 0,
+    ) -> UserResponse:
+        query_params: dict[str, str] = {
+            "count": str(count),
+            "offset": str(offset),
+        }
+        if limit is not None:
+            query_params["limit"] = str(limit)
+        if post_filter is not None:
+            query_params["filter"] = post_filter
+        if sort is not None:
+            query_params["sort"] = sort
+        raw_json = self._call_api(GET_USERS.format_path_with_params(), query_params)
+        return UserResponse(**raw_json)
+
+    def get_all_users(self) -> list[AtlanUser]:
+        """
+        Retrieve all users defined in Atlan.
+        """
+        users: list[AtlanUser] = []
+        offset = 0
+        limit = 100
+        response: Optional[UserResponse] = self.get_users(
+            offset=offset, limit=limit, sort="username"
+        )
+        while response:
+            if page := response.records:
+                users.extend(page)
+                offset += limit
+                response = self.get_users(offset=offset, limit=limit, sort="username")
+            else:
+                response = None
+        return users
+
+    def get_users_by_email(
+        self, email: str, limit: int = 100
+    ) -> Optional[list[AtlanUser]]:
+        """
+        Retrieves all users with email addresses that contain the provided email.
+        (This could include a complete email address, in which case there should be at
+        most a single item in the returned list, or could be a partial email address
+        such as "@example.com" to retrieve all users with that domain in their email
+        address.)
+        """
+        if response := self.get_users(
+            offset=0,
+            limit=limit,
+            post_filter='{"email":{"$ilike":"%' + email + '%"}}',
+        ):
+            return response.records
+        return None
+
+    def get_user_by_username(self, username: str) -> Optional[AtlanUser]:
+        """
+        Retrieves a user based on the username. (This attempts an exact match on username
+        rather than a contains search.)
+        """
+        if response := self.get_users(
+            offset=0,
+            limit=5,
+            post_filter='{"username":"' + username + '"}',
+        ):
+            if response.records and len(response.records) >= 1:
+                return response.records[0]
+        return None
+
     @validate_arguments()
     def get_asset_by_qualified_name(
         self,
         qualified_name: str,
         asset_type: Type[A],
         min_ext_info: bool = False,
         ignore_relationships: bool = False,
@@ -885,20 +1069,20 @@
                 qualified_name=qualified_name, asset_type=asset_type
             )
         else:
             raise ValueError("Either guid or qualified name must be specified")
         if not terms:
             return asset
         replacement_terms: list[AtlasGlossaryTerm] = []
-        if existing_terms := asset.terms:
+        if existing_terms := asset.assigned_terms:
             replacement_terms.extend(
                 term for term in existing_terms if term.relationship_status != "DELETED"
             )
         replacement_terms.extend(terms)
-        asset.terms = replacement_terms
+        asset.assigned_terms = replacement_terms
         response = self.upsert(entity=asset)
         if assets := response.assets_updated(asset_type=asset_type):
             return assets[0]
         return asset
 
     @validate_arguments()
     def replace_terms(
@@ -916,52 +1100,52 @@
             asset = self.get_asset_by_guid(guid=guid, asset_type=asset_type)
         elif qualified_name:
             asset = self.get_asset_by_qualified_name(
                 qualified_name=qualified_name, asset_type=asset_type
             )
         else:
             raise ValueError("Either guid or qualified name must be specified")
-        asset.terms = terms
+        asset.assigned_terms = terms
         response = self.upsert(entity=asset)
         if assets := response.assets_updated(asset_type=asset_type):
             return assets[0]
         return asset
 
     @validate_arguments()
     def remove_terms(
         self,
         asset_type: Type[A],
         terms: list[AtlasGlossaryTerm],
         guid: Optional[str] = None,
         qualified_name: Optional[str] = None,
     ) -> A:
         if not terms:
-            raise ValueError("A list of terms to remove must be specified")
+            raise ValueError("A list of assigned_terms to remove must be specified")
         if guid:
             if qualified_name:
                 raise ValueError(
                     "Either guid or qualified_name can be be specified not both"
                 )
             asset = self.get_asset_by_guid(guid=guid, asset_type=asset_type)
         elif qualified_name:
             asset = self.get_asset_by_qualified_name(
                 qualified_name=qualified_name, asset_type=asset_type
             )
         else:
             raise ValueError("Either guid or qualified name must be specified")
         replacement_terms: list[AtlasGlossaryTerm] = []
         guids_to_be_removed = {t.guid for t in terms}
-        if existing_terms := asset.terms:
+        if existing_terms := asset.assigned_terms:
             replacement_terms.extend(
                 term
                 for term in existing_terms
                 if term.relationship_status != "DELETED"
                 and term.guid not in guids_to_be_removed
             )
-        asset.terms = replacement_terms
+        asset.assigned_terms = replacement_terms
         response = self.upsert(entity=asset)
         if assets := response.assets_updated(asset_type=asset_type):
             return assets[0]
         return asset
 
     @validate_arguments()
     def find_connections_by_name(
```

### Comparing `pyatlan-0.0.32/pyatlan/client/constants.py` & `pyatlan-0.0.33/pyatlan/client/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,23 +10,44 @@
     MULTIPART_FORM_DATA,
     HTTPMethod,
     HTTPStatus,
 )
 
 ROLE_API = f"{ADMIN_URI}roles"
 GROUP_API = f"{ADMIN_URI}groups"
+USER_API = f"{ADMIN_URI}users"
 
 # Role APIs
 GET_ROLES = API(ROLE_API, HTTPMethod.GET, HTTPStatus.OK)
 
 # Group APIs
 GET_GROUPS = API(GROUP_API, HTTPMethod.GET, HTTPStatus.OK)
 CREATE_GROUP = API(GROUP_API, HTTPMethod.POST, HTTPStatus.OK)
 UPDATE_GROUP = API(GROUP_API, HTTPMethod.POST, HTTPStatus.OK)
 DELETE_GROUP = API(GROUP_API + "/{group_guid}/delete", HTTPMethod.POST, HTTPStatus.OK)
+GET_GROUP_MEMBERS = API(
+    GROUP_API + "/{group_guid}/members", HTTPMethod.GET, HTTPStatus.OK
+)
+REMOVE_USERS_FROM_GROUP = API(
+    GROUP_API + "/{group_guid}/members/remove", HTTPMethod.POST, HTTPStatus.OK
+)
+
+# User APIs
+GET_USERS = API(USER_API, HTTPMethod.GET, HTTPStatus.OK)
+CREATE_USERS = API(USER_API, HTTPMethod.POST, HTTPStatus.OK)
+UPDATE_USER = API(USER_API, HTTPMethod.POST, HTTPStatus.OK)
+DELETE_USER = API(USER_API + "/{user_guid}/delete", HTTPMethod.POST, HTTPStatus.OK)
+GET_USER_GROUPS = API(USER_API + "/{user_guid}/groups", HTTPMethod.GET, HTTPStatus.OK)
+ADD_USER_TO_GROUPS = API(
+    USER_API + "/{user_guid}/groups", HTTPMethod.POST, HTTPStatus.OK
+)
+CHANGE_USER_ROLE = API(
+    USER_API + "/{user_guid}/roles/update", HTTPMethod.POST, HTTPStatus.OK
+)
+GET_CURRENT_USER = API(f"{USER_API}/current", HTTPMethod.GET, HTTPStatus.OK)
 
 ENTITY_API = f"{BASE_URI}entity/"
 PREFIX_ATTR = "attr:"
 PREFIX_ATTR_ = "attr_"
 ADMIN_API = f"{BASE_URI}admin/"
 ENTITY_PURGE_API = f"{ADMIN_API}purge/"
 ENTITY_BULK_API = f"{ENTITY_API}bulk/"
```

### Comparing `pyatlan-0.0.32/pyatlan/error.py` & `pyatlan-0.0.33/pyatlan/error.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.32/pyatlan/exceptions.py` & `pyatlan-0.0.33/pyatlan/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.32/pyatlan/generator/generate_from_typdefs.py` & `pyatlan-0.0.33/pyatlan/generator/generate_from_typdefs.py`

 * *Files 17% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     ("powerbi_endorsement", "PowerbiEndorsement"),
     ("kafka_topic_compression_type", "KafkaTopicCompressionType"),
     ("kafka_topic_cleanup_policy", "PowerbiEndorsement"),
     ("quick_sight_folder_type", "QuickSightFolderType"),
     ("quick_sight_dataset_field_type", "QuickSightDatasetFieldType"),
     ("quick_sight_analysis_status", "QuickSightAnalysisStatus"),
     ("quick_sight_dataset_import_mode", "QuickSightDatasetImportMode"),
+    ("file_type", "FileType"),
 ]
 ARRAY_REPLACEMENTS = [("array<string>", "set{string}")]
 
 
 def get_type(type_: str):
     ret_value = type_
 
@@ -131,23 +132,48 @@
         }
 
         for super_type in entity_def.super_types:
             merge_them(super_type, attributes)
         return list(attributes.values())
 
     def add_entity_def(self, entity_defs, name):
+        def get_ancestor_relationship_defs(
+            ancetor_name: str, ancestor_relationship_defs
+        ):
+            ancestor_entity_def = self.entity_defs[ancetor_name]
+            if not ancestor_entity_def.super_types or not ancetor_name:
+                return ancestor_relationship_defs
+            for relationship_def in (
+                ancestor_entity_def.relationship_attribute_defs or []
+            ):
+                ancestor_relationship_defs.add(relationship_def["name"])
+            return get_ancestor_relationship_defs(
+                ancestor_entity_def.super_types[0]
+                if ancestor_entity_def.super_types
+                else "",
+                ancestor_relationship_defs,
+            )
+
         entity_def = self.entity_defs[name]
         if len(entity_def.super_types) > 1:
             entity_def.attribute_defs = self.merge_attributes(entity_def)
         names = {attribute_def["name"] for attribute_def in entity_def.attribute_defs}
-        entity_def.relationship_attribute_defs = [
-            relationship_def
-            for relationship_def in entity_def.relationship_attribute_defs
-            if relationship_def["name"] not in names
-        ]
+        super_type_relationship_defs = (
+            get_ancestor_relationship_defs(entity_def.super_types[0], set())
+            if entity_def.super_types
+            else set()
+        )
+        entity_def.relationship_attribute_defs = list(
+            {
+                relationship_def["name"]: relationship_def
+                for relationship_def in entity_def.relationship_attribute_defs
+                if relationship_def["name"] not in names
+                and relationship_def["name"] not in super_type_relationship_defs
+            }.values()
+        )
         for parent in entity_def.super_types:
             if parent not in self.processed:
                 return
         entity_defs.append(entity_def)
         self.processed.add(name)
```

### Comparing `pyatlan-0.0.32/pyatlan/model/assets.py` & `pyatlan-0.0.33/pyatlan/model/assets.py`

 * *Files 20% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     ADLSProvisionState,
     ADLSReplicationType,
     ADLSStorageKind,
     AnnouncementType,
     AtlanConnectorType,
     CertificateStatus,
     EntityStatus,
+    FileType,
     GoogleDatastudioAssetType,
     IconType,
     KafkaTopicCompressionType,
     PowerbiEndorsement,
     QueryUsernameStrategy,
     QuickSightAnalysisStatus,
     QuickSightDatasetFieldType,
@@ -82,26 +83,26 @@
 
 
 class Referenceable(AtlanObject):
     """Description"""
 
     def __init__(__pydantic_self__, **data: Any) -> None:
         super().__init__(**data)
-        __pydantic_self__.__fields_set__.add("type_name")
+        __pydantic_self__.__fields_set__.update(["attributes", "type_name"])
 
     def __setattr__(self, name, value):
         if name in Referenceable._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "qualified_name",
         "replicated_from",
         "replicated_to",
-        "terms",
+        "assigned_terms",
     ]
 
     @property
     def qualified_name(self) -> str:
         return self.attributes.qualified_name
 
     @qualified_name.setter
@@ -127,24 +128,22 @@
     @replicated_to.setter
     def replicated_to(self, replicated_to: Optional[list[AtlasServer]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.replicated_to = replicated_to
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+    def assigned_terms(self) -> Optional[list[AtlasGlossaryTerm]]:
+        return self.attributes.meanings
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @assigned_terms.setter
+    def assigned_terms(self, assigned_terms: Optional[list[AtlasGlossaryTerm]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.meanings = assigned_terms
 
     class Attributes(AtlanObject):
         qualified_name: str = Field("", description="", alias="qualifiedName")
         replicated_from: Optional[list[AtlasServer]] = Field(
             None, description="", alias="replicatedFrom"
         )
         replicated_to: Optional[list[AtlasServer]] = Field(
@@ -154,15 +153,15 @@
             None, description="", alias="meanings"
         )  # relationship
 
         def validate_required(self):
             pass
 
     attributes: "Referenceable.Attributes" = Field(
-        None,
+        default_factory=lambda: Referenceable.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary "
         "by type, so are described in the sub-types of this schema.\n",
     )
     business_attributes: Optional[Dict[str, Any]] = Field(
         None,
         description="Map of custom metadata attributes and values defined on the entity.\n",
         alias="businessAttributes",
@@ -236,15 +235,15 @@
         description="Status of the relationship (when this is a related entity).\n",
     )
     relationship_type: Optional[str] = Field(
         None,
         description="Status of the relationship (when this is a related entity).\n",
     )
     meaning_names: Optional[list[str]] = Field(
-        None, description="Names of terms that have been linked to this asset."
+        None, description="Names of assigned_terms that have been linked to this asset."
     )
     meanings: Optional[list[Meaning]] = Field(None, description="", alias="meanings")
     custom_attributes: Optional[dict[str, Any]] = Field(
         None, description="", alias="customAttributes"
     )
     scrubbed: Optional[bool] = Field(
         None, description="", alias="fields removed from results"
@@ -418,15 +417,21 @@
         "asset_mc_monitor_types",
         "asset_mc_monitor_schedule_types",
         "asset_mc_incident_types",
         "asset_mc_incident_sub_types",
         "asset_mc_incident_severities",
         "asset_mc_incident_states",
         "asset_mc_last_sync_run_at",
-        "terms",
+        "mc_monitors",
+        "files",
+        "mc_incidents",
+        "links",
+        "metrics",
+        "readme",
+        "assigned_terms",
     ]
 
     @property
     def name(self) -> str:
         return self.attributes.name
 
     @name.setter
@@ -1661,24 +1666,82 @@
     @asset_mc_last_sync_run_at.setter
     def asset_mc_last_sync_run_at(self, asset_mc_last_sync_run_at: Optional[datetime]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.asset_mc_last_sync_run_at = asset_mc_last_sync_run_at
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def mc_monitors(self) -> Optional[list[MCMonitor]]:
+        return self.attributes.mc_monitors
+
+    @mc_monitors.setter
+    def mc_monitors(self, mc_monitors: Optional[list[MCMonitor]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.mc_monitors = mc_monitors
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def files(self) -> Optional[list[File]]:
+        return self.attributes.files
+
+    @files.setter
+    def files(self, files: Optional[list[File]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.files = files
+
+    @property
+    def mc_incidents(self) -> Optional[list[MCIncident]]:
+        return self.attributes.mc_incidents
+
+    @mc_incidents.setter
+    def mc_incidents(self, mc_incidents: Optional[list[MCIncident]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.mc_incidents = mc_incidents
+
+    @property
+    def links(self) -> Optional[list[Link]]:
+        return self.attributes.links
+
+    @links.setter
+    def links(self, links: Optional[list[Link]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.links = links
+
+    @property
+    def metrics(self) -> Optional[list[Metric]]:
+        return self.attributes.metrics
+
+    @metrics.setter
+    def metrics(self, metrics: Optional[list[Metric]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.metrics = metrics
+
+    @property
+    def readme(self) -> Optional[Readme]:
+        return self.attributes.readme
+
+    @readme.setter
+    def readme(self, readme: Optional[Readme]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.readme = readme
+
+    @property
+    def assigned_terms(self) -> Optional[list[AtlasGlossaryTerm]]:
+        return self.attributes.meanings
+
+    @assigned_terms.setter
+    def assigned_terms(self, assigned_terms: Optional[list[AtlasGlossaryTerm]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.meanings = assigned_terms
 
     _subtypes_: dict[str, type] = dict()
 
     def __init_subclass__(cls, type_name=None):
         cls._subtypes_[type_name or cls.__name__.lower()] = cls
 
     @classmethod
@@ -1707,14 +1770,15 @@
 
     @classmethod
     def __get_validators__(cls):
         yield cls._convert_to_real_type_
 
     @classmethod
     def _convert_to_real_type_(cls, data):
+
         if isinstance(data, Asset):
             return data
 
         data_type = (
             data.get("type_name") if "type_name" in data else data.get("typeName")
         )
 
@@ -2043,14 +2107,17 @@
         )
         asset_mc_last_sync_run_at: Optional[datetime] = Field(
             None, description="", alias="assetMcLastSyncRunAt"
         )
         mc_monitors: Optional[list[MCMonitor]] = Field(
             None, description="", alias="mcMonitors"
         )  # relationship
+        files: Optional[list[File]] = Field(
+            None, description="", alias="files"
+        )  # relationship
         mc_incidents: Optional[list[MCIncident]] = Field(
             None, description="", alias="mcIncidents"
         )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
@@ -2079,15 +2146,15 @@
 
         def remove_announcement(self):
             self.announcement_message = None
             self.announcement_title = None
             self.announcement_type = None
 
     attributes: "Asset.Attributes" = Field(
-        None,
+        default_factory=lambda: Asset.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
     def has_announcement(self) -> bool:
         return bool(
             self.attributes
@@ -2139,14 +2206,15 @@
     _convience_properties: ClassVar[list[str]] = [
         "short_description",
         "long_description",
         "language",
         "usage",
         "additional_attributes",
         "terms",
+        "categories",
     ]
 
     @property
     def short_description(self) -> Optional[str]:
         return self.attributes.short_description
 
     @short_description.setter
@@ -2192,24 +2260,32 @@
     @additional_attributes.setter
     def additional_attributes(self, additional_attributes: Optional[dict[str, str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.additional_attributes = additional_attributes
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def terms(self) -> Optional[list[AtlasGlossaryTerm]]:
+        return self.attributes.terms
+
+    @terms.setter
+    def terms(self, terms: Optional[list[AtlasGlossaryTerm]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.terms = terms
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def categories(self) -> Optional[list[AtlasGlossaryCategory]]:
+        return self.attributes.categories
+
+    @categories.setter
+    def categories(self, categories: Optional[list[AtlasGlossaryCategory]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.categories = categories
 
     type_name: str = Field("AtlasGlossary", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "AtlasGlossary":
             raise ValueError("must be AtlasGlossary")
@@ -2223,47 +2299,29 @@
             None, description="", alias="longDescription"
         )
         language: Optional[str] = Field(None, description="", alias="language")
         usage: Optional[str] = Field(None, description="", alias="usage")
         additional_attributes: Optional[dict[str, str]] = Field(
             None, description="", alias="additionalAttributes"
         )
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         terms: Optional[list[AtlasGlossaryTerm]] = Field(
             None, description="", alias="terms"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
         categories: Optional[list[AtlasGlossaryCategory]] = Field(
             None, description="", alias="categories"
         )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
 
         @classmethod
         # @validate_arguments()
         def create(cls, *, name: StrictStr) -> AtlasGlossary.Attributes:
             validate_required_fields(["name"], [name])
             return AtlasGlossary.Attributes(name=name, qualified_name=next_id())
 
     attributes: "AtlasGlossary.Attributes" = Field(
-        None,
+        default_factory=lambda: AtlasGlossary.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
     @root_validator()
     def update_qualified_name(cls, values):
         if (
@@ -2285,123 +2343,43 @@
     """Description"""
 
     def __setattr__(self, name, value):
         if name in DataSet._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
-    _convience_properties: ClassVar[list[str]] = [
-        "terms",
-    ]
-
-    @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
-
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+    _convience_properties: ClassVar[list[str]] = []
 
     type_name: str = Field("DataSet", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "DataSet":
             raise ValueError("must be DataSet")
         return v
 
-    class Attributes(Asset.Attributes):
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-
-    attributes: "DataSet.Attributes" = Field(
-        None,
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
 
 class ProcessExecution(Asset, type_name="ProcessExecution"):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in ProcessExecution._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
-    _convience_properties: ClassVar[list[str]] = [
-        "terms",
-    ]
-
-    @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
-
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+    _convience_properties: ClassVar[list[str]] = []
 
     type_name: str = Field("ProcessExecution", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "ProcessExecution":
             raise ValueError("must be ProcessExecution")
         return v
 
-    class Attributes(Asset.Attributes):
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-
-    attributes: "ProcessExecution.Attributes" = Field(
-        None,
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
 
 class AtlasGlossaryTerm(Asset, type_name="AtlasGlossaryTerm"):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in AtlasGlossaryTerm._convience_properties:
             return object.__setattr__(self, name, value)
@@ -2410,15 +2388,30 @@
     _convience_properties: ClassVar[list[str]] = [
         "short_description",
         "long_description",
         "examples",
         "abbreviation",
         "usage",
         "additional_attributes",
-        "terms",
+        "translation_terms",
+        "valid_values_for",
+        "synonyms",
+        "replaced_by",
+        "valid_values",
+        "replacement_terms",
+        "see_also",
+        "translated_terms",
+        "is_a",
+        "anchor",
+        "antonyms",
+        "assigned_entities",
+        "classifies",
+        "categories",
+        "preferred_to_terms",
+        "preferred_terms",
     ]
 
     @property
     def short_description(self) -> Optional[str]:
         return self.attributes.short_description
 
     @short_description.setter
@@ -2474,24 +2467,172 @@
     @additional_attributes.setter
     def additional_attributes(self, additional_attributes: Optional[dict[str, str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.additional_attributes = additional_attributes
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def translation_terms(self) -> Optional[list[AtlasGlossaryTerm]]:
+        return self.attributes.translation_terms
+
+    @translation_terms.setter
+    def translation_terms(self, translation_terms: Optional[list[AtlasGlossaryTerm]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.translation_terms = translation_terms
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def valid_values_for(self) -> Optional[list[AtlasGlossaryTerm]]:
+        return self.attributes.valid_values_for
+
+    @valid_values_for.setter
+    def valid_values_for(self, valid_values_for: Optional[list[AtlasGlossaryTerm]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.valid_values_for = valid_values_for
+
+    @property
+    def synonyms(self) -> Optional[list[AtlasGlossaryTerm]]:
+        return self.attributes.synonyms
+
+    @synonyms.setter
+    def synonyms(self, synonyms: Optional[list[AtlasGlossaryTerm]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.synonyms = synonyms
+
+    @property
+    def replaced_by(self) -> Optional[list[AtlasGlossaryTerm]]:
+        return self.attributes.replaced_by
+
+    @replaced_by.setter
+    def replaced_by(self, replaced_by: Optional[list[AtlasGlossaryTerm]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.replaced_by = replaced_by
+
+    @property
+    def valid_values(self) -> Optional[list[AtlasGlossaryTerm]]:
+        return self.attributes.valid_values
+
+    @valid_values.setter
+    def valid_values(self, valid_values: Optional[list[AtlasGlossaryTerm]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.valid_values = valid_values
+
+    @property
+    def replacement_terms(self) -> Optional[list[AtlasGlossaryTerm]]:
+        return self.attributes.replacement_terms
+
+    @replacement_terms.setter
+    def replacement_terms(self, replacement_terms: Optional[list[AtlasGlossaryTerm]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.replacement_terms = replacement_terms
+
+    @property
+    def see_also(self) -> Optional[list[AtlasGlossaryTerm]]:
+        return self.attributes.see_also
+
+    @see_also.setter
+    def see_also(self, see_also: Optional[list[AtlasGlossaryTerm]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.see_also = see_also
+
+    @property
+    def translated_terms(self) -> Optional[list[AtlasGlossaryTerm]]:
+        return self.attributes.translated_terms
+
+    @translated_terms.setter
+    def translated_terms(self, translated_terms: Optional[list[AtlasGlossaryTerm]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.translated_terms = translated_terms
+
+    @property
+    def is_a(self) -> Optional[list[AtlasGlossaryTerm]]:
+        return self.attributes.is_a
+
+    @is_a.setter
+    def is_a(self, is_a: Optional[list[AtlasGlossaryTerm]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.is_a = is_a
+
+    @property
+    def anchor(self) -> AtlasGlossary:
+        return self.attributes.anchor
+
+    @anchor.setter
+    def anchor(self, anchor: AtlasGlossary):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.anchor = anchor
+
+    @property
+    def antonyms(self) -> Optional[list[AtlasGlossaryTerm]]:
+        return self.attributes.antonyms
+
+    @antonyms.setter
+    def antonyms(self, antonyms: Optional[list[AtlasGlossaryTerm]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.antonyms = antonyms
+
+    @property
+    def assigned_entities(self) -> Optional[list[Referenceable]]:
+        return self.attributes.assigned_entities
+
+    @assigned_entities.setter
+    def assigned_entities(self, assigned_entities: Optional[list[Referenceable]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.assigned_entities = assigned_entities
+
+    @property
+    def classifies(self) -> Optional[list[AtlasGlossaryTerm]]:
+        return self.attributes.classifies
+
+    @classifies.setter
+    def classifies(self, classifies: Optional[list[AtlasGlossaryTerm]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.classifies = classifies
+
+    @property
+    def categories(self) -> Optional[list[AtlasGlossaryCategory]]:
+        return self.attributes.categories
+
+    @categories.setter
+    def categories(self, categories: Optional[list[AtlasGlossaryCategory]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.categories = categories
+
+    @property
+    def preferred_to_terms(self) -> Optional[list[AtlasGlossaryTerm]]:
+        return self.attributes.preferred_to_terms
+
+    @preferred_to_terms.setter
+    def preferred_to_terms(self, preferred_to_terms: Optional[list[AtlasGlossaryTerm]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.preferred_to_terms = preferred_to_terms
+
+    @property
+    def preferred_terms(self) -> Optional[list[AtlasGlossaryTerm]]:
+        return self.attributes.preferred_terms
+
+    @preferred_terms.setter
+    def preferred_terms(self, preferred_terms: Optional[list[AtlasGlossaryTerm]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.preferred_terms = preferred_terms
 
     type_name: str = Field("AtlasGlossaryTerm", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "AtlasGlossaryTerm":
             raise ValueError("must be AtlasGlossaryTerm")
@@ -2518,32 +2659,23 @@
         )  # relationship
         synonyms: Optional[list[AtlasGlossaryTerm]] = Field(
             None, description="", alias="synonyms"
         )  # relationship
         replaced_by: Optional[list[AtlasGlossaryTerm]] = Field(
             None, description="", alias="replacedBy"
         )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
         valid_values: Optional[list[AtlasGlossaryTerm]] = Field(
             None, description="", alias="validValues"
         )  # relationship
         replacement_terms: Optional[list[AtlasGlossaryTerm]] = Field(
             None, description="", alias="replacementTerms"
         )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
         see_also: Optional[list[AtlasGlossaryTerm]] = Field(
             None, description="", alias="seeAlso"
         )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         translated_terms: Optional[list[AtlasGlossaryTerm]] = Field(
             None, description="", alias="translatedTerms"
         )  # relationship
         is_a: Optional[list[AtlasGlossaryTerm]] = Field(
             None, description="", alias="isA"
         )  # relationship
         anchor: AtlasGlossary = Field(
@@ -2551,29 +2683,20 @@
         )  # relationship
         antonyms: Optional[list[AtlasGlossaryTerm]] = Field(
             None, description="", alias="antonyms"
         )  # relationship
         assigned_entities: Optional[list[Referenceable]] = Field(
             None, description="", alias="assignedEntities"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
         classifies: Optional[list[AtlasGlossaryTerm]] = Field(
             None, description="", alias="classifies"
         )  # relationship
         categories: Optional[list[AtlasGlossaryCategory]] = Field(
             None, description="", alias="categories"
         )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
         preferred_to_terms: Optional[list[AtlasGlossaryTerm]] = Field(
             None, description="", alias="preferredToTerms"
         )  # relationship
         preferred_terms: Optional[list[AtlasGlossaryTerm]] = Field(
             None, description="", alias="preferredTerms"
         )  # relationship
 
@@ -2603,15 +2726,15 @@
                 name=name,
                 anchor=anchor,
                 categories=categories,
                 qualified_name=next_id(),
             )
 
     attributes: "AtlasGlossaryTerm.Attributes" = Field(
-        None,
+        default_factory=lambda: AtlasGlossaryTerm.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
     @root_validator()
     def update_qualified_name(cls, values):
         if (
@@ -2668,123 +2791,43 @@
     """Description"""
 
     def __setattr__(self, name, value):
         if name in Cloud._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
-    _convience_properties: ClassVar[list[str]] = [
-        "terms",
-    ]
-
-    @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
-
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+    _convience_properties: ClassVar[list[str]] = []
 
     type_name: str = Field("Cloud", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Cloud":
             raise ValueError("must be Cloud")
         return v
 
-    class Attributes(Asset.Attributes):
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-
-    attributes: "Cloud.Attributes" = Field(
-        None,
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
 
 class Infrastructure(Asset, type_name="Infrastructure"):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in Infrastructure._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
-    _convience_properties: ClassVar[list[str]] = [
-        "terms",
-    ]
-
-    @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
-
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+    _convience_properties: ClassVar[list[str]] = []
 
     type_name: str = Field("Infrastructure", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Infrastructure":
             raise ValueError("must be Infrastructure")
         return v
 
-    class Attributes(Asset.Attributes):
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-
-    attributes: "Infrastructure.Attributes" = Field(
-        None,
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
 
 class Connection(Asset, type_name="Connection"):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in Connection._convience_properties:
             return object.__setattr__(self, name, value)
@@ -2808,15 +2851,15 @@
         "connector_icon",
         "connector_image",
         "source_logo",
         "is_sample_data_preview_enabled",
         "popularity_insights_timeframe",
         "has_popularity_insights",
         "connection_dbt_environments",
-        "terms",
+        "connection_s_s_o_credential_guid",
     ]
 
     @property
     def category(self) -> Optional[str]:
         return self.attributes.category
 
     @category.setter
@@ -3030,24 +3073,26 @@
         self, connection_dbt_environments: Optional[set[str]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.connection_dbt_environments = connection_dbt_environments
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+    def connection_s_s_o_credential_guid(self) -> Optional[str]:
+        return self.attributes.connection_s_s_o_credential_guid
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @connection_s_s_o_credential_guid.setter
+    def connection_s_s_o_credential_guid(
+        self, connection_s_s_o_credential_guid: Optional[str]
+    ):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.connection_s_s_o_credential_guid = (
+            connection_s_s_o_credential_guid
+        )
 
     type_name: str = Field("Connection", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Connection":
             raise ValueError("must be Connection")
@@ -3097,32 +3142,17 @@
         )
         has_popularity_insights: Optional[bool] = Field(
             None, description="", alias="hasPopularityInsights"
         )
         connection_dbt_environments: Optional[set[str]] = Field(
             None, description="", alias="connectionDbtEnvironments"
         )
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
+        connection_s_s_o_credential_guid: Optional[str] = Field(
+            None, description="", alias="connectionSSOCredentialGuid"
+        )
 
         def validate_required(self):
             if not self.name:
                 raise ValueError("name is required")
             if not self.admin_roles and not self.admin_groups and not self.admin_users:
                 raise ValueError(
                     "One of admin_user, admin_groups or admin_roles is required"
@@ -3160,15 +3190,15 @@
                 )
             else:
                 raise ValueError(
                     "One of admin_user, admin_groups or admin_roles is required"
                 )
 
     attributes: "Connection.Attributes" = Field(
-        None,
+        default_factory=lambda: Connection.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
     @classmethod
     # @validate_arguments()
     def create(
@@ -3210,15 +3240,15 @@
 
     _convience_properties: ClassVar[list[str]] = [
         "inputs",
         "outputs",
         "code",
         "sql",
         "ast",
-        "terms",
+        "column_processes",
     ]
 
     @property
     def inputs(self) -> Optional[list[Catalog]]:
         return self.attributes.inputs
 
     @inputs.setter
@@ -3264,24 +3294,22 @@
     @ast.setter
     def ast(self, ast: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.ast = ast
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+    def column_processes(self) -> Optional[list[ColumnProcess]]:
+        return self.attributes.column_processes
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @column_processes.setter
+    def column_processes(self, column_processes: Optional[list[ColumnProcess]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.column_processes = column_processes
 
     type_name: str = Field("Process", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Process":
             raise ValueError("must be Process")
@@ -3289,35 +3317,17 @@
 
     class Attributes(Asset.Attributes):
         inputs: Optional[list[Catalog]] = Field(None, description="", alias="inputs")
         outputs: Optional[list[Catalog]] = Field(None, description="", alias="outputs")
         code: Optional[str] = Field(None, description="", alias="code")
         sql: Optional[str] = Field(None, description="", alias="sql")
         ast: Optional[str] = Field(None, description="", alias="ast")
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
         column_processes: Optional[list[ColumnProcess]] = Field(
             None, description="", alias="columnProcesses"
         )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
 
         @staticmethod
         def generate_qualified_name(
             name: str,
             connection_qualified_name: str,
             inputs: list["Catalog"],
             outputs: list["Catalog"],
@@ -3376,15 +3386,15 @@
                 connector_name=connector_name,
                 connection_qualified_name=connection_qualified_name,
                 inputs=inputs,
                 outputs=outputs,
             )
 
     attributes: "Process.Attributes" = Field(
-        None,
+        default_factory=lambda: Process.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
     @classmethod
     def create(
         cls,
@@ -3416,14 +3426,17 @@
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "short_description",
         "long_description",
         "additional_attributes",
         "terms",
+        "anchor",
+        "parent_category",
+        "children_categories",
     ]
 
     @property
     def short_description(self) -> Optional[str]:
         return self.attributes.short_description
 
     @short_description.setter
@@ -3449,24 +3462,54 @@
     @additional_attributes.setter
     def additional_attributes(self, additional_attributes: Optional[dict[str, str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.additional_attributes = additional_attributes
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def terms(self) -> Optional[list[AtlasGlossaryTerm]]:
+        return self.attributes.terms
+
+    @terms.setter
+    def terms(self, terms: Optional[list[AtlasGlossaryTerm]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.terms = terms
+
+    @property
+    def anchor(self) -> AtlasGlossary:
+        return self.attributes.anchor
+
+    @anchor.setter
+    def anchor(self, anchor: AtlasGlossary):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.anchor = anchor
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def parent_category(self) -> Optional[AtlasGlossaryCategory]:
+        return self.attributes.parent_category
+
+    @parent_category.setter
+    def parent_category(self, parent_category: Optional[AtlasGlossaryCategory]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.parent_category = parent_category
+
+    @property
+    def children_categories(self) -> Optional[list[AtlasGlossaryCategory]]:
+        return self.attributes.children_categories
+
+    @children_categories.setter
+    def children_categories(
+        self, children_categories: Optional[list[AtlasGlossaryCategory]]
+    ):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.children_categories = children_categories
 
     type_name: str = Field("AtlasGlossaryCategory", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "AtlasGlossaryCategory":
             raise ValueError("must be AtlasGlossaryCategory")
@@ -3478,44 +3521,26 @@
         )
         long_description: Optional[str] = Field(
             None, description="", alias="longDescription"
         )
         additional_attributes: Optional[dict[str, str]] = Field(
             None, description="", alias="additionalAttributes"
         )
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         terms: Optional[list[AtlasGlossaryTerm]] = Field(
             None, description="", alias="terms"
         )  # relationship
         anchor: AtlasGlossary = Field(
             None, description="", alias="anchor"
         )  # relationship
         parent_category: Optional[AtlasGlossaryCategory] = Field(
             None, description="", alias="parentCategory"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
         children_categories: Optional[list[AtlasGlossaryCategory]] = Field(
             None, description="", alias="childrenCategories"
         )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
 
         @classmethod
         # @validate_arguments()
         def create(
             cls,
             *,
             name: StrictStr,
@@ -3527,15 +3552,15 @@
                 name=name,
                 anchor=anchor,
                 parent_category=parent_category,
                 qualified_name=next_id(),
             )
 
     attributes: "AtlasGlossaryCategory.Attributes" = Field(
-        None,
+        default_factory=lambda: AtlasGlossaryCategory.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
     @root_validator()
     def update_qualified_name(cls, values):
         if (
@@ -3570,15 +3595,14 @@
         if name in Badge._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "badge_conditions",
         "badge_metadata_attribute",
-        "terms",
     ]
 
     @property
     def badge_conditions(self) -> Optional[list[BadgeCondition]]:
         return self.attributes.badge_conditions
 
     @badge_conditions.setter
@@ -3593,26 +3617,14 @@
 
     @badge_metadata_attribute.setter
     def badge_metadata_attribute(self, badge_metadata_attribute: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.badge_metadata_attribute = badge_metadata_attribute
 
-    @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
-
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.meanings = terms
-
     type_name: str = Field("Badge", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Badge":
             raise ValueError("must be Badge")
         return v
@@ -3639,32 +3651,14 @@
     class Attributes(Asset.Attributes):
         badge_conditions: Optional[list[BadgeCondition]] = Field(
             None, description="", alias="badgeConditions"
         )
         badge_metadata_attribute: Optional[str] = Field(
             None, description="", alias="badgeMetadataAttribute"
         )
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
 
         @classmethod
         # @validate_arguments()
         def create(
             cls,
             *,
             name: StrictStr,
@@ -3686,145 +3680,127 @@
                 name=name,
                 qualified_name=f"badges/global/{cm_id}.{cm_attr_id}",
                 badge_metadata_attribute=f"{cm_id}.{cm_attr_id}",
                 badge_conditions=badge_conditions,
             )
 
     attributes: "Badge.Attributes" = Field(
-        None,
+        default_factory=lambda: Badge.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class Namespace(Asset, type_name="Namespace"):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in Namespace._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
-        "terms",
+        "children_queries",
+        "children_folders",
     ]
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def children_queries(self) -> Optional[list[Query]]:
+        return self.attributes.children_queries
+
+    @children_queries.setter
+    def children_queries(self, children_queries: Optional[list[Query]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.children_queries = children_queries
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def children_folders(self) -> Optional[list[Folder]]:
+        return self.attributes.children_folders
+
+    @children_folders.setter
+    def children_folders(self, children_folders: Optional[list[Folder]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.children_folders = children_folders
 
     type_name: str = Field("Namespace", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Namespace":
             raise ValueError("must be Namespace")
         return v
 
     class Attributes(Asset.Attributes):
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         children_queries: Optional[list[Query]] = Field(
             None, description="", alias="childrenQueries"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
         children_folders: Optional[list[Folder]] = Field(
             None, description="", alias="childrenFolders"
         )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
 
     attributes: "Namespace.Attributes" = Field(
-        None,
+        default_factory=lambda: Namespace.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class Catalog(Asset, type_name="Catalog"):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in Catalog._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
-        "terms",
+        "input_to_processes",
+        "output_from_processes",
     ]
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def input_to_processes(self) -> Optional[list[Process]]:
+        return self.attributes.input_to_processes
+
+    @input_to_processes.setter
+    def input_to_processes(self, input_to_processes: Optional[list[Process]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.input_to_processes = input_to_processes
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def output_from_processes(self) -> Optional[list[Process]]:
+        return self.attributes.output_from_processes
+
+    @output_from_processes.setter
+    def output_from_processes(self, output_from_processes: Optional[list[Process]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.output_from_processes = output_from_processes
 
     type_name: str = Field("Catalog", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Catalog":
             raise ValueError("must be Catalog")
         return v
 
     class Attributes(Asset.Attributes):
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
         output_from_processes: Optional[list[Process]] = Field(
             None, description="", alias="outputFromProcesses"
         )  # relationship
 
     attributes: "Catalog.Attributes" = Field(
-        None,
+        default_factory=lambda: Catalog.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class Google(Cloud):
     """Description"""
@@ -3839,15 +3815,14 @@
         "google_project_name",
         "google_project_id",
         "google_project_number",
         "google_location",
         "google_location_type",
         "google_labels",
         "google_tags",
-        "terms",
     ]
 
     @property
     def google_service(self) -> Optional[str]:
         return self.attributes.google_service
 
     @google_service.setter
@@ -3922,26 +3897,14 @@
 
     @google_tags.setter
     def google_tags(self, google_tags: Optional[list[GoogleTag]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.google_tags = google_tags
 
-    @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
-
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.meanings = terms
-
     type_name: str = Field("Google", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Google":
             raise ValueError("must be Google")
         return v
@@ -3967,35 +3930,17 @@
         )
         google_labels: Optional[list[GoogleLabel]] = Field(
             None, description="", alias="googleLabels"
         )
         google_tags: Optional[list[GoogleTag]] = Field(
             None, description="", alias="googleTags"
         )
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
 
     attributes: "Google.Attributes" = Field(
-        None,
+        default_factory=lambda: Google.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class Azure(Cloud):
     """Description"""
@@ -4006,15 +3951,14 @@
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "azure_resource_id",
         "azure_location",
         "adls_account_secondary_location",
         "azure_tags",
-        "terms",
     ]
 
     @property
     def azure_resource_id(self) -> Optional[str]:
         return self.attributes.azure_resource_id
 
     @azure_resource_id.setter
@@ -4053,26 +3997,14 @@
 
     @azure_tags.setter
     def azure_tags(self, azure_tags: Optional[list[AzureTag]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.azure_tags = azure_tags
 
-    @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
-
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.meanings = terms
-
     type_name: str = Field("Azure", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Azure":
             raise ValueError("must be Azure")
         return v
@@ -4086,35 +4018,17 @@
         )
         adls_account_secondary_location: Optional[str] = Field(
             None, description="", alias="adlsAccountSecondaryLocation"
         )
         azure_tags: Optional[list[AzureTag]] = Field(
             None, description="", alias="azureTags"
         )
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
 
     attributes: "Azure.Attributes" = Field(
-        None,
+        default_factory=lambda: Azure.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class AWS(Cloud):
     """Description"""
@@ -4130,15 +4044,14 @@
         "aws_service",
         "aws_region",
         "aws_account_id",
         "aws_resource_id",
         "aws_owner_name",
         "aws_owner_id",
         "aws_tags",
-        "terms",
     ]
 
     @property
     def aws_arn(self) -> Optional[str]:
         return self.attributes.aws_arn
 
     @aws_arn.setter
@@ -4223,26 +4136,14 @@
 
     @aws_tags.setter
     def aws_tags(self, aws_tags: Optional[list[AwsTag]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.aws_tags = aws_tags
 
-    @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
-
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.meanings = terms
-
     type_name: str = Field("AWS", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "AWS":
             raise ValueError("must be AWS")
         return v
@@ -4259,131 +4160,121 @@
             None, description="", alias="awsResourceId"
         )
         aws_owner_name: Optional[str] = Field(
             None, description="", alias="awsOwnerName"
         )
         aws_owner_id: Optional[str] = Field(None, description="", alias="awsOwnerId")
         aws_tags: Optional[list[AwsTag]] = Field(None, description="", alias="awsTags")
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
 
     attributes: "AWS.Attributes" = Field(
-        None,
+        default_factory=lambda: AWS.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class BIProcess(Process):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in BIProcess._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
-        "terms",
+        "outputs",
+        "inputs",
     ]
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def outputs(self) -> Optional[list[Catalog]]:
+        return self.attributes.outputs
+
+    @outputs.setter
+    def outputs(self, outputs: Optional[list[Catalog]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.outputs = outputs
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def inputs(self) -> Optional[list[Catalog]]:
+        return self.attributes.inputs
+
+    @inputs.setter
+    def inputs(self, inputs: Optional[list[Catalog]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.inputs = inputs
 
     type_name: str = Field("BIProcess", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "BIProcess":
             raise ValueError("must be BIProcess")
         return v
 
     class Attributes(Process.Attributes):
         outputs: Optional[list[Catalog]] = Field(
             None, description="", alias="outputs"
         )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         inputs: Optional[list[Catalog]] = Field(
             None, description="", alias="inputs"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        column_processes: Optional[list[ColumnProcess]] = Field(
-            None, description="", alias="columnProcesses"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
 
     attributes: "BIProcess.Attributes" = Field(
-        None,
+        default_factory=lambda: BIProcess.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class ColumnProcess(Process):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in ColumnProcess._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
-        "terms",
+        "outputs",
+        "process",
+        "inputs",
     ]
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def outputs(self) -> Optional[list[Catalog]]:
+        return self.attributes.outputs
+
+    @outputs.setter
+    def outputs(self, outputs: Optional[list[Catalog]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.outputs = outputs
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def process(self) -> Optional[Process]:
+        return self.attributes.process
+
+    @process.setter
+    def process(self, process: Optional[Process]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.process = process
+
+    @property
+    def inputs(self) -> Optional[list[Catalog]]:
+        return self.attributes.inputs
+
+    @inputs.setter
+    def inputs(self, inputs: Optional[list[Catalog]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.inputs = inputs
 
     type_name: str = Field("ColumnProcess", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "ColumnProcess":
             raise ValueError("must be ColumnProcess")
@@ -4392,41 +4283,20 @@
     class Attributes(Process.Attributes):
         outputs: Optional[list[Catalog]] = Field(
             None, description="", alias="outputs"
         )  # relationship
         process: Optional[Process] = Field(
             None, description="", alias="process"
         )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         inputs: Optional[list[Catalog]] = Field(
             None, description="", alias="inputs"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        column_processes: Optional[list[ColumnProcess]] = Field(
-            None, description="", alias="columnProcesses"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
 
     attributes: "ColumnProcess.Attributes" = Field(
-        None,
+        default_factory=lambda: ColumnProcess.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class Collection(Namespace):
     """Description"""
@@ -4435,15 +4305,14 @@
         if name in Collection._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "icon",
         "icon_type",
-        "terms",
     ]
 
     @property
     def icon(self) -> Optional[str]:
         return self.attributes.icon
 
     @icon.setter
@@ -4458,64 +4327,28 @@
 
     @icon_type.setter
     def icon_type(self, icon_type: Optional[IconType]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.icon_type = icon_type
 
-    @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
-
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.meanings = terms
-
     type_name: str = Field("Collection", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Collection":
             raise ValueError("must be Collection")
         return v
 
     class Attributes(Namespace.Attributes):
         icon: Optional[str] = Field(None, description="", alias="icon")
         icon_type: Optional[IconType] = Field(None, description="", alias="iconType")
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        children_queries: Optional[list[Query]] = Field(
-            None, description="", alias="childrenQueries"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        children_folders: Optional[list[Folder]] = Field(
-            None, description="", alias="childrenFolders"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
 
     attributes: "Collection.Attributes" = Field(
-        None,
+        default_factory=lambda: Collection.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class Folder(Namespace):
     """Description"""
@@ -4524,15 +4357,15 @@
         if name in Folder._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "parent_qualified_name",
         "collection_qualified_name",
-        "terms",
+        "parent",
     ]
 
     @property
     def parent_qualified_name(self) -> str:
         return self.attributes.parent_qualified_name
 
     @parent_qualified_name.setter
@@ -4548,24 +4381,22 @@
     @collection_qualified_name.setter
     def collection_qualified_name(self, collection_qualified_name: str):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.collection_qualified_name = collection_qualified_name
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+    def parent(self) -> Namespace:
+        return self.attributes.parent
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @parent.setter
+    def parent(self, parent: Namespace):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.parent = parent
 
     type_name: str = Field("Folder", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Folder":
             raise ValueError("must be Folder")
@@ -4575,370 +4406,116 @@
         parent_qualified_name: str = Field(
             None, description="", alias="parentQualifiedName"
         )
         collection_qualified_name: str = Field(
             None, description="", alias="collectionQualifiedName"
         )
         parent: Namespace = Field(None, description="", alias="parent")  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        children_queries: Optional[list[Query]] = Field(
-            None, description="", alias="childrenQueries"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        children_folders: Optional[list[Folder]] = Field(
-            None, description="", alias="childrenFolders"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
 
     attributes: "Folder.Attributes" = Field(
-        None,
+        default_factory=lambda: Folder.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class EventStore(Catalog):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in EventStore._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
-    _convience_properties: ClassVar[list[str]] = [
-        "terms",
-    ]
-
-    @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
-
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+    _convience_properties: ClassVar[list[str]] = []
 
     type_name: str = Field("EventStore", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "EventStore":
             raise ValueError("must be EventStore")
         return v
 
-    class Attributes(Catalog.Attributes):
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
-
-    attributes: "EventStore.Attributes" = Field(
-        None,
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
 
 class ObjectStore(Catalog):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in ObjectStore._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
-    _convience_properties: ClassVar[list[str]] = [
-        "terms",
-    ]
-
-    @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
-
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+    _convience_properties: ClassVar[list[str]] = []
 
     type_name: str = Field("ObjectStore", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "ObjectStore":
             raise ValueError("must be ObjectStore")
         return v
 
-    class Attributes(Catalog.Attributes):
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
-
-    attributes: "ObjectStore.Attributes" = Field(
-        None,
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
 
 class DataQuality(Catalog):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in DataQuality._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
-    _convience_properties: ClassVar[list[str]] = [
-        "terms",
-    ]
-
-    @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
-
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+    _convience_properties: ClassVar[list[str]] = []
 
     type_name: str = Field("DataQuality", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "DataQuality":
             raise ValueError("must be DataQuality")
         return v
 
-    class Attributes(Catalog.Attributes):
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
-
-    attributes: "DataQuality.Attributes" = Field(
-        None,
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
 
 class BI(Catalog):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in BI._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
-    _convience_properties: ClassVar[list[str]] = [
-        "terms",
-    ]
-
-    @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
-
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+    _convience_properties: ClassVar[list[str]] = []
 
     type_name: str = Field("BI", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "BI":
             raise ValueError("must be BI")
         return v
 
-    class Attributes(Catalog.Attributes):
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
-
-    attributes: "BI.Attributes" = Field(
-        None,
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
 
 class SaaS(Catalog):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in SaaS._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
-    _convience_properties: ClassVar[list[str]] = [
-        "terms",
-    ]
-
-    @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
-
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+    _convience_properties: ClassVar[list[str]] = []
 
     type_name: str = Field("SaaS", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "SaaS":
             raise ValueError("must be SaaS")
         return v
 
-    class Attributes(Catalog.Attributes):
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
-
-    attributes: "SaaS.Attributes" = Field(
-        None,
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
 
 class Dbt(Catalog):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in Dbt._convience_properties:
             return object.__setattr__(self, name, value)
@@ -4959,15 +4536,14 @@
         "dbt_job_next_run",
         "dbt_job_next_run_humanized",
         "dbt_environment_name",
         "dbt_environment_dbt_version",
         "dbt_tags",
         "dbt_connection_context",
         "dbt_semantic_layer_proxy_url",
-        "terms",
     ]
 
     @property
     def dbt_alias(self) -> Optional[str]:
         return self.attributes.dbt_alias
 
     @dbt_alias.setter
@@ -5146,26 +4722,14 @@
 
     @dbt_semantic_layer_proxy_url.setter
     def dbt_semantic_layer_proxy_url(self, dbt_semantic_layer_proxy_url: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_semantic_layer_proxy_url = dbt_semantic_layer_proxy_url
 
-    @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
-
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.meanings = terms
-
     type_name: str = Field("Dbt", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Dbt":
             raise ValueError("must be Dbt")
         return v
@@ -5211,41 +4775,17 @@
         dbt_tags: Optional[set[str]] = Field(None, description="", alias="dbtTags")
         dbt_connection_context: Optional[str] = Field(
             None, description="", alias="dbtConnectionContext"
         )
         dbt_semantic_layer_proxy_url: Optional[str] = Field(
             None, description="", alias="dbtSemanticLayerProxyUrl"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "Dbt.Attributes" = Field(
-        None,
+        default_factory=lambda: Dbt.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class Resource(Catalog):
     """Description"""
@@ -5256,15 +4796,14 @@
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "link",
         "is_global",
         "reference",
         "resource_metadata",
-        "terms",
     ]
 
     @property
     def link(self) -> Optional[str]:
         return self.attributes.link
 
     @link.setter
@@ -5299,26 +4838,14 @@
 
     @resource_metadata.setter
     def resource_metadata(self, resource_metadata: Optional[dict[str, str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.resource_metadata = resource_metadata
 
-    @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
-
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.meanings = terms
-
     type_name: str = Field("Resource", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Resource":
             raise ValueError("must be Resource")
         return v
@@ -5326,110 +4853,40 @@
     class Attributes(Catalog.Attributes):
         link: Optional[str] = Field(None, description="", alias="link")
         is_global: Optional[bool] = Field(None, description="", alias="isGlobal")
         reference: Optional[str] = Field(None, description="", alias="reference")
         resource_metadata: Optional[dict[str, str]] = Field(
             None, description="", alias="resourceMetadata"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "Resource.Attributes" = Field(
-        None,
+        default_factory=lambda: Resource.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class Insight(Catalog):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in Insight._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
-    _convience_properties: ClassVar[list[str]] = [
-        "terms",
-    ]
-
-    @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
-
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+    _convience_properties: ClassVar[list[str]] = []
 
     type_name: str = Field("Insight", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Insight":
             raise ValueError("must be Insight")
         return v
 
-    class Attributes(Catalog.Attributes):
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
-
-    attributes: "Insight.Attributes" = Field(
-        None,
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
 
 class API(Catalog):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in API._convience_properties:
             return object.__setattr__(self, name, value)
@@ -5438,15 +4895,14 @@
     _convience_properties: ClassVar[list[str]] = [
         "api_spec_type",
         "api_spec_version",
         "api_spec_name",
         "api_spec_qualified_name",
         "api_external_docs",
         "api_is_auth_optional",
-        "terms",
     ]
 
     @property
     def api_spec_type(self) -> Optional[str]:
         return self.attributes.api_spec_type
 
     @api_spec_type.setter
@@ -5501,26 +4957,14 @@
 
     @api_is_auth_optional.setter
     def api_is_auth_optional(self, api_is_auth_optional: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.api_is_auth_optional = api_is_auth_optional
 
-    @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
-
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.meanings = terms
-
     type_name: str = Field("API", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "API":
             raise ValueError("must be API")
         return v
@@ -5536,41 +4980,17 @@
         )
         api_external_docs: Optional[dict[str, str]] = Field(
             None, description="", alias="apiExternalDocs"
         )
         api_is_auth_optional: Optional[bool] = Field(
             None, description="", alias="apiIsAuthOptional"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "API.Attributes" = Field(
-        None,
+        default_factory=lambda: API.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class Tag(Catalog):
     """Description"""
@@ -5581,15 +5001,14 @@
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "tag_id",
         "tag_attributes",
         "tag_allowed_values",
         "mapped_classification_name",
-        "terms",
     ]
 
     @property
     def tag_id(self) -> Optional[str]:
         return self.attributes.tag_id
 
     @tag_id.setter
@@ -5624,26 +5043,14 @@
 
     @mapped_classification_name.setter
     def mapped_classification_name(self, mapped_classification_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mapped_classification_name = mapped_classification_name
 
-    @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
-
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.meanings = terms
-
     type_name: str = Field("Tag", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Tag":
             raise ValueError("must be Tag")
         return v
@@ -5655,41 +5062,17 @@
         )
         tag_allowed_values: Optional[set[str]] = Field(
             None, description="", alias="tagAllowedValues"
         )
         mapped_classification_name: Optional[str] = Field(
             None, description="", alias="mappedClassificationName"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "Tag.Attributes" = Field(
-        None,
+        default_factory=lambda: Tag.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class SQL(Catalog):
     """Description"""
@@ -5710,15 +5093,18 @@
         "schema_qualified_name",
         "table_name",
         "table_qualified_name",
         "view_name",
         "view_qualified_name",
         "is_profiled",
         "last_profiled_at",
-        "terms",
+        "dbt_sources",
+        "sql_dbt_models",
+        "sql_dbt_sources",
+        "dbt_models",
     ]
 
     @property
     def query_count(self) -> Optional[int]:
         return self.attributes.query_count
 
     @query_count.setter
@@ -5854,24 +5240,52 @@
     @last_profiled_at.setter
     def last_profiled_at(self, last_profiled_at: Optional[datetime]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.last_profiled_at = last_profiled_at
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def dbt_sources(self) -> Optional[list[DbtSource]]:
+        return self.attributes.dbt_sources
+
+    @dbt_sources.setter
+    def dbt_sources(self, dbt_sources: Optional[list[DbtSource]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.dbt_sources = dbt_sources
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def sql_dbt_models(self) -> Optional[list[DbtModel]]:
+        return self.attributes.sql_dbt_models
+
+    @sql_dbt_models.setter
+    def sql_dbt_models(self, sql_dbt_models: Optional[list[DbtModel]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.sql_dbt_models = sql_dbt_models
+
+    @property
+    def sql_dbt_sources(self) -> Optional[list[DbtSource]]:
+        return self.attributes.sql_dbt_sources
+
+    @sql_dbt_sources.setter
+    def sql_dbt_sources(self, sql_dbt_sources: Optional[list[DbtSource]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.sql_dbt_sources = sql_dbt_sources
+
+    @property
+    def dbt_models(self) -> Optional[list[DbtModel]]:
+        return self.attributes.dbt_models
+
+    @dbt_models.setter
+    def dbt_models(self, dbt_models: Optional[list[DbtModel]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.dbt_models = dbt_models
 
     type_name: str = Field("SQL", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "SQL":
             raise ValueError("must be SQL")
@@ -5904,53 +5318,29 @@
         view_qualified_name: Optional[str] = Field(
             None, description="", alias="viewQualifiedName"
         )
         is_profiled: Optional[bool] = Field(None, description="", alias="isProfiled")
         last_profiled_at: Optional[datetime] = Field(
             None, description="", alias="lastProfiledAt"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        dbt_models: Optional[list[DbtModel]] = Field(
-            None, description="", alias="dbtModels"
-        )  # relationship
         dbt_sources: Optional[list[DbtSource]] = Field(
             None, description="", alias="dbtSources"
         )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
         sql_dbt_models: Optional[list[DbtModel]] = Field(
             None, description="", alias="sqlDbtModels"
         )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
         sql_dbt_sources: Optional[list[DbtSource]] = Field(
             None, description="", alias="sqlDBTSources"
         )  # relationship
+        dbt_models: Optional[list[DbtModel]] = Field(
+            None, description="", alias="dbtModels"
+        )  # relationship
 
     attributes: "SQL.Attributes" = Field(
-        None,
+        default_factory=lambda: SQL.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class DataStudio(Google):
     """Description"""
@@ -5965,15 +5355,16 @@
         "google_project_name",
         "google_project_id",
         "google_project_number",
         "google_location",
         "google_location_type",
         "google_labels",
         "google_tags",
-        "terms",
+        "input_to_processes",
+        "output_from_processes",
     ]
 
     @property
     def google_service(self) -> Optional[str]:
         return self.attributes.google_service
 
     @google_service.setter
@@ -6049,24 +5440,32 @@
     @google_tags.setter
     def google_tags(self, google_tags: Optional[list[GoogleTag]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.google_tags = google_tags
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def input_to_processes(self) -> Optional[list[Process]]:
+        return self.attributes.input_to_processes
+
+    @input_to_processes.setter
+    def input_to_processes(self, input_to_processes: Optional[list[Process]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.input_to_processes = input_to_processes
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def output_from_processes(self) -> Optional[list[Process]]:
+        return self.attributes.output_from_processes
+
+    @output_from_processes.setter
+    def output_from_processes(self, output_from_processes: Optional[list[Process]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.output_from_processes = output_from_processes
 
     type_name: str = Field("DataStudio", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "DataStudio":
             raise ValueError("must be DataStudio")
@@ -6096,38 +5495,20 @@
         )
         google_tags: Optional[list[GoogleTag]] = Field(
             None, description="", alias="googleTags"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
         output_from_processes: Optional[list[Process]] = Field(
             None, description="", alias="outputFromProcesses"
         )  # relationship
 
     attributes: "DataStudio.Attributes" = Field(
-        None,
+        default_factory=lambda: DataStudio.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class GCS(Google):
     """Description"""
@@ -6148,15 +5529,16 @@
         "google_project_name",
         "google_project_id",
         "google_project_number",
         "google_location",
         "google_location_type",
         "google_labels",
         "google_tags",
-        "terms",
+        "input_to_processes",
+        "output_from_processes",
     ]
 
     @property
     def gcs_storage_class(self) -> Optional[str]:
         return self.attributes.gcs_storage_class
 
     @gcs_storage_class.setter
@@ -6292,24 +5674,32 @@
     @google_tags.setter
     def google_tags(self, google_tags: Optional[list[GoogleTag]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.google_tags = google_tags
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def input_to_processes(self) -> Optional[list[Process]]:
+        return self.attributes.input_to_processes
+
+    @input_to_processes.setter
+    def input_to_processes(self, input_to_processes: Optional[list[Process]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.input_to_processes = input_to_processes
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def output_from_processes(self) -> Optional[list[Process]]:
+        return self.attributes.output_from_processes
+
+    @output_from_processes.setter
+    def output_from_processes(self, output_from_processes: Optional[list[Process]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.output_from_processes = output_from_processes
 
     type_name: str = Field("GCS", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "GCS":
             raise ValueError("must be GCS")
@@ -6355,38 +5745,20 @@
         )
         google_tags: Optional[list[GoogleTag]] = Field(
             None, description="", alias="googleTags"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
         output_from_processes: Optional[list[Process]] = Field(
             None, description="", alias="outputFromProcesses"
         )  # relationship
 
     attributes: "GCS.Attributes" = Field(
-        None,
+        default_factory=lambda: GCS.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class DataStudioAsset(DataStudio):
     """Description"""
@@ -6405,15 +5777,14 @@
         "google_project_name",
         "google_project_id",
         "google_project_number",
         "google_location",
         "google_location_type",
         "google_labels",
         "google_tags",
-        "terms",
     ]
 
     @property
     def data_studio_asset_type(self) -> Optional[GoogleDatastudioAssetType]:
         return self.attributes.data_studio_asset_type
 
     @data_studio_asset_type.setter
@@ -6532,26 +5903,14 @@
 
     @google_tags.setter
     def google_tags(self, google_tags: Optional[list[GoogleTag]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.google_tags = google_tags
 
-    @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
-
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.meanings = terms
-
     type_name: str = Field("DataStudioAsset", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "DataStudioAsset":
             raise ValueError("must be DataStudioAsset")
         return v
@@ -6589,41 +5948,17 @@
         )
         google_labels: Optional[list[GoogleLabel]] = Field(
             None, description="", alias="googleLabels"
         )
         google_tags: Optional[list[GoogleTag]] = Field(
             None, description="", alias="googleTags"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "DataStudioAsset.Attributes" = Field(
-        None,
+        default_factory=lambda: DataStudioAsset.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class ADLS(ObjectStore):
     """Description"""
@@ -6635,15 +5970,14 @@
 
     _convience_properties: ClassVar[list[str]] = [
         "adls_account_qualified_name",
         "azure_resource_id",
         "azure_location",
         "adls_account_secondary_location",
         "azure_tags",
-        "terms",
     ]
 
     @property
     def adls_account_qualified_name(self) -> Optional[str]:
         return self.attributes.adls_account_qualified_name
 
     @adls_account_qualified_name.setter
@@ -6692,26 +6026,14 @@
 
     @azure_tags.setter
     def azure_tags(self, azure_tags: Optional[list[AzureTag]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.azure_tags = azure_tags
 
-    @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
-
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.meanings = terms
-
     type_name: str = Field("ADLS", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "ADLS":
             raise ValueError("must be ADLS")
         return v
@@ -6728,41 +6050,17 @@
         )
         adls_account_secondary_location: Optional[str] = Field(
             None, description="", alias="adlsAccountSecondaryLocation"
         )
         azure_tags: Optional[list[AzureTag]] = Field(
             None, description="", alias="azureTags"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "ADLS.Attributes" = Field(
-        None,
+        default_factory=lambda: ADLS.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class S3(ObjectStore):
     """Description"""
@@ -6780,15 +6078,14 @@
         "aws_service",
         "aws_region",
         "aws_account_id",
         "aws_resource_id",
         "aws_owner_name",
         "aws_owner_id",
         "aws_tags",
-        "terms",
     ]
 
     @property
     def s3_e_tag(self) -> Optional[str]:
         return self.attributes.s3_e_tag
 
     @s3_e_tag.setter
@@ -6893,26 +6190,14 @@
 
     @aws_tags.setter
     def aws_tags(self, aws_tags: Optional[list[AwsTag]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.aws_tags = aws_tags
 
-    @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
-
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.meanings = terms
-
     type_name: str = Field("S3", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "S3":
             raise ValueError("must be S3")
         return v
@@ -6931,41 +6216,17 @@
             None, description="", alias="awsResourceId"
         )
         aws_owner_name: Optional[str] = Field(
             None, description="", alias="awsOwnerName"
         )
         aws_owner_id: Optional[str] = Field(None, description="", alias="awsOwnerId")
         aws_tags: Optional[list[AwsTag]] = Field(None, description="", alias="awsTags")
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "S3.Attributes" = Field(
-        None,
+        default_factory=lambda: S3.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class DbtColumnProcess(Dbt):
     """Description"""
@@ -6996,15 +6257,16 @@
         "dbt_connection_context",
         "dbt_semantic_layer_proxy_url",
         "inputs",
         "outputs",
         "code",
         "sql",
         "ast",
-        "terms",
+        "process",
+        "column_processes",
     ]
 
     @property
     def dbt_column_process_job_status(self) -> Optional[str]:
         return self.attributes.dbt_column_process_job_status
 
     @dbt_column_process_job_status.setter
@@ -7246,24 +6508,32 @@
     @ast.setter
     def ast(self, ast: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.ast = ast
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def process(self) -> Optional[Process]:
+        return self.attributes.process
+
+    @process.setter
+    def process(self, process: Optional[Process]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.process = process
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def column_processes(self) -> Optional[list[ColumnProcess]]:
+        return self.attributes.column_processes
+
+    @column_processes.setter
+    def column_processes(self, column_processes: Optional[list[ColumnProcess]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.column_processes = column_processes
 
     type_name: str = Field("DbtColumnProcess", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "DbtColumnProcess":
             raise ValueError("must be DbtColumnProcess")
@@ -7318,129 +6588,58 @@
             None, description="", alias="dbtSemanticLayerProxyUrl"
         )
         inputs: Optional[list[Catalog]] = Field(None, description="", alias="inputs")
         outputs: Optional[list[Catalog]] = Field(None, description="", alias="outputs")
         code: Optional[str] = Field(None, description="", alias="code")
         sql: Optional[str] = Field(None, description="", alias="sql")
         ast: Optional[str] = Field(None, description="", alias="ast")
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         process: Optional[Process] = Field(
             None, description="", alias="process"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
         column_processes: Optional[list[ColumnProcess]] = Field(
             None, description="", alias="columnProcesses"
         )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "DbtColumnProcess.Attributes" = Field(
-        None,
+        default_factory=lambda: DbtColumnProcess.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class Kafka(EventStore):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in Kafka._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
-    _convience_properties: ClassVar[list[str]] = [
-        "terms",
-    ]
-
-    @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
-
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+    _convience_properties: ClassVar[list[str]] = []
 
     type_name: str = Field("Kafka", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Kafka":
             raise ValueError("must be Kafka")
         return v
 
-    class Attributes(EventStore.Attributes):
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
-
-    attributes: "Kafka.Attributes" = Field(
-        None,
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
 
 class MonteCarlo(DataQuality):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in MonteCarlo._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "mc_labels",
         "mc_asset_qualified_names",
-        "terms",
     ]
 
     @property
     def mc_labels(self) -> Optional[set[str]]:
         return self.attributes.mc_labels
 
     @mc_labels.setter
@@ -7455,66 +6654,30 @@
 
     @mc_asset_qualified_names.setter
     def mc_asset_qualified_names(self, mc_asset_qualified_names: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mc_asset_qualified_names = mc_asset_qualified_names
 
-    @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
-
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.meanings = terms
-
     type_name: str = Field("MonteCarlo", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "MonteCarlo":
             raise ValueError("must be MonteCarlo")
         return v
 
     class Attributes(DataQuality.Attributes):
         mc_labels: Optional[set[str]] = Field(None, description="", alias="mcLabels")
         mc_asset_qualified_names: Optional[set[str]] = Field(
             None, description="", alias="mcAssetQualifiedNames"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "MonteCarlo.Attributes" = Field(
-        None,
+        default_factory=lambda: MonteCarlo.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class Metric(DataQuality):
     """Description"""
@@ -7525,15 +6688,17 @@
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "metric_type",
         "metric_s_q_l",
         "metric_filters",
         "metric_time_grains",
-        "terms",
+        "assets",
+        "metric_dimension_columns",
+        "metric_timestamp_column",
     ]
 
     @property
     def metric_type(self) -> Optional[str]:
         return self.attributes.metric_type
 
     @metric_type.setter
@@ -7569,24 +6734,44 @@
     @metric_time_grains.setter
     def metric_time_grains(self, metric_time_grains: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.metric_time_grains = metric_time_grains
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def assets(self) -> Optional[list[Asset]]:
+        return self.attributes.assets
+
+    @assets.setter
+    def assets(self, assets: Optional[list[Asset]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.assets = assets
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def metric_dimension_columns(self) -> Optional[list[Column]]:
+        return self.attributes.metric_dimension_columns
+
+    @metric_dimension_columns.setter
+    def metric_dimension_columns(
+        self, metric_dimension_columns: Optional[list[Column]]
+    ):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.metric_dimension_columns = metric_dimension_columns
+
+    @property
+    def metric_timestamp_column(self) -> Optional[Column]:
+        return self.attributes.metric_timestamp_column
+
+    @metric_timestamp_column.setter
+    def metric_timestamp_column(self, metric_timestamp_column: Optional[Column]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.metric_timestamp_column = metric_timestamp_column
 
     type_name: str = Field("Metric", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Metric":
             raise ValueError("must be Metric")
@@ -7597,50 +6782,26 @@
         metric_s_q_l: Optional[str] = Field(None, description="", alias="metricSQL")
         metric_filters: Optional[str] = Field(
             None, description="", alias="metricFilters"
         )
         metric_time_grains: Optional[set[str]] = Field(
             None, description="", alias="metricTimeGrains"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         assets: Optional[list[Asset]] = Field(
             None, description="", alias="assets"
         )  # relationship
         metric_dimension_columns: Optional[list[Column]] = Field(
             None, description="", alias="metricDimensionColumns"
         )  # relationship
         metric_timestamp_column: Optional[Column] = Field(
             None, description="", alias="metricTimestampColumn"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "Metric.Attributes" = Field(
-        None,
+        default_factory=lambda: Metric.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class Metabase(BI):
     """Description"""
@@ -7649,15 +6810,14 @@
         if name in Metabase._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "metabase_collection_name",
         "metabase_collection_qualified_name",
-        "terms",
     ]
 
     @property
     def metabase_collection_name(self) -> Optional[str]:
         return self.attributes.metabase_collection_name
 
     @metabase_collection_name.setter
@@ -7676,26 +6836,14 @@
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.metabase_collection_qualified_name = (
             metabase_collection_qualified_name
         )
 
-    @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
-
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.meanings = terms
-
     type_name: str = Field("Metabase", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Metabase":
             raise ValueError("must be Metabase")
         return v
@@ -7703,41 +6851,17 @@
     class Attributes(BI.Attributes):
         metabase_collection_name: Optional[str] = Field(
             None, description="", alias="metabaseCollectionName"
         )
         metabase_collection_qualified_name: Optional[str] = Field(
             None, description="", alias="metabaseCollectionQualifiedName"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "Metabase.Attributes" = Field(
-        None,
+        default_factory=lambda: Metabase.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class QuickSight(BI):
     """Description"""
@@ -7747,15 +6871,14 @@
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "quick_sight_id",
         "quick_sight_sheet_id",
         "quick_sight_sheet_name",
-        "terms",
     ]
 
     @property
     def quick_sight_id(self) -> Optional[str]:
         return self.attributes.quick_sight_id
 
     @quick_sight_id.setter
@@ -7780,26 +6903,14 @@
 
     @quick_sight_sheet_name.setter
     def quick_sight_sheet_name(self, quick_sight_sheet_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.quick_sight_sheet_name = quick_sight_sheet_name
 
-    @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
-
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.meanings = terms
-
     type_name: str = Field("QuickSight", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "QuickSight":
             raise ValueError("must be QuickSight")
         return v
@@ -7810,41 +6921,17 @@
         )
         quick_sight_sheet_id: Optional[str] = Field(
             None, description="", alias="quickSightSheetId"
         )
         quick_sight_sheet_name: Optional[str] = Field(
             None, description="", alias="quickSightSheetName"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "QuickSight.Attributes" = Field(
-        None,
+        default_factory=lambda: QuickSight.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class Thoughtspot(BI):
     """Description"""
@@ -7853,15 +6940,14 @@
         if name in Thoughtspot._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "thoughtspot_chart_type",
         "thoughtspot_question_text",
-        "terms",
     ]
 
     @property
     def thoughtspot_chart_type(self) -> Optional[str]:
         return self.attributes.thoughtspot_chart_type
 
     @thoughtspot_chart_type.setter
@@ -7876,26 +6962,14 @@
 
     @thoughtspot_question_text.setter
     def thoughtspot_question_text(self, thoughtspot_question_text: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.thoughtspot_question_text = thoughtspot_question_text
 
-    @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
-
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.meanings = terms
-
     type_name: str = Field("Thoughtspot", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Thoughtspot":
             raise ValueError("must be Thoughtspot")
         return v
@@ -7903,41 +6977,17 @@
     class Attributes(BI.Attributes):
         thoughtspot_chart_type: Optional[str] = Field(
             None, description="", alias="thoughtspotChartType"
         )
         thoughtspot_question_text: Optional[str] = Field(
             None, description="", alias="thoughtspotQuestionText"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "Thoughtspot.Attributes" = Field(
-        None,
+        default_factory=lambda: Thoughtspot.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class PowerBI(BI):
     """Description"""
@@ -7948,15 +6998,14 @@
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "power_b_i_is_hidden",
         "power_b_i_table_qualified_name",
         "power_b_i_format_string",
         "power_b_i_endorsement",
-        "terms",
     ]
 
     @property
     def power_b_i_is_hidden(self) -> Optional[bool]:
         return self.attributes.power_b_i_is_hidden
 
     @power_b_i_is_hidden.setter
@@ -7995,26 +7044,14 @@
     def power_b_i_endorsement(
         self, power_b_i_endorsement: Optional[PowerbiEndorsement]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.power_b_i_endorsement = power_b_i_endorsement
 
-    @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
-
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.meanings = terms
-
     type_name: str = Field("PowerBI", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "PowerBI":
             raise ValueError("must be PowerBI")
         return v
@@ -8028,41 +7065,17 @@
         )
         power_b_i_format_string: Optional[str] = Field(
             None, description="", alias="powerBIFormatString"
         )
         power_b_i_endorsement: Optional[PowerbiEndorsement] = Field(
             None, description="", alias="powerBIEndorsement"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "PowerBI.Attributes" = Field(
-        None,
+        default_factory=lambda: PowerBI.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class Preset(BI):
     """Description"""
@@ -8073,15 +7086,14 @@
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "preset_workspace_id",
         "preset_workspace_qualified_name",
         "preset_dashboard_id",
         "preset_dashboard_qualified_name",
-        "terms",
     ]
 
     @property
     def preset_workspace_id(self) -> Optional[int]:
         return self.attributes.preset_workspace_id
 
     @preset_workspace_id.setter
@@ -8124,26 +7136,14 @@
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.preset_dashboard_qualified_name = (
             preset_dashboard_qualified_name
         )
 
-    @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
-
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.meanings = terms
-
     type_name: str = Field("Preset", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Preset":
             raise ValueError("must be Preset")
         return v
@@ -8157,41 +7157,17 @@
         )
         preset_dashboard_id: Optional[int] = Field(
             None, description="", alias="presetDashboardId"
         )
         preset_dashboard_qualified_name: Optional[str] = Field(
             None, description="", alias="presetDashboardQualifiedName"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "Preset.Attributes" = Field(
-        None,
+        default_factory=lambda: Preset.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class Mode(BI):
     """Description"""
@@ -8207,15 +7183,14 @@
         "mode_workspace_name",
         "mode_workspace_username",
         "mode_workspace_qualified_name",
         "mode_report_name",
         "mode_report_qualified_name",
         "mode_query_name",
         "mode_query_qualified_name",
-        "terms",
     ]
 
     @property
     def mode_id(self) -> Optional[str]:
         return self.attributes.mode_id
 
     @mode_id.setter
@@ -8302,26 +7277,14 @@
 
     @mode_query_qualified_name.setter
     def mode_query_qualified_name(self, mode_query_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mode_query_qualified_name = mode_query_qualified_name
 
-    @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
-
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.meanings = terms
-
     type_name: str = Field("Mode", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Mode":
             raise ValueError("must be Mode")
         return v
@@ -8346,41 +7309,17 @@
         )
         mode_query_name: Optional[str] = Field(
             None, description="", alias="modeQueryName"
         )
         mode_query_qualified_name: Optional[str] = Field(
             None, description="", alias="modeQueryQualifiedName"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "Mode.Attributes" = Field(
-        None,
+        default_factory=lambda: Mode.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class Sigma(BI):
     """Description"""
@@ -8393,15 +7332,14 @@
     _convience_properties: ClassVar[list[str]] = [
         "sigma_workbook_qualified_name",
         "sigma_workbook_name",
         "sigma_page_qualified_name",
         "sigma_page_name",
         "sigma_data_element_qualified_name",
         "sigma_data_element_name",
-        "terms",
     ]
 
     @property
     def sigma_workbook_qualified_name(self) -> Optional[str]:
         return self.attributes.sigma_workbook_qualified_name
 
     @sigma_workbook_qualified_name.setter
@@ -8462,26 +7400,14 @@
 
     @sigma_data_element_name.setter
     def sigma_data_element_name(self, sigma_data_element_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sigma_data_element_name = sigma_data_element_name
 
-    @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
-
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.meanings = terms
-
     type_name: str = Field("Sigma", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Sigma":
             raise ValueError("must be Sigma")
         return v
@@ -8501,41 +7427,17 @@
         )
         sigma_data_element_qualified_name: Optional[str] = Field(
             None, description="", alias="sigmaDataElementQualifiedName"
         )
         sigma_data_element_name: Optional[str] = Field(
             None, description="", alias="sigmaDataElementName"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "Sigma.Attributes" = Field(
-        None,
+        default_factory=lambda: Sigma.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class Qlik(BI):
     """Description"""
@@ -8550,15 +7452,14 @@
         "qlik_q_r_i",
         "qlik_space_id",
         "qlik_space_qualified_name",
         "qlik_app_id",
         "qlik_app_qualified_name",
         "qlik_owner_id",
         "qlik_is_published",
-        "terms",
     ]
 
     @property
     def qlik_id(self) -> Optional[str]:
         return self.attributes.qlik_id
 
     @qlik_id.setter
@@ -8633,26 +7534,14 @@
 
     @qlik_is_published.setter
     def qlik_is_published(self, qlik_is_published: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.qlik_is_published = qlik_is_published
 
-    @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
-
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.meanings = terms
-
     type_name: str = Field("Qlik", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Qlik":
             raise ValueError("must be Qlik")
         return v
@@ -8668,250 +7557,97 @@
         qlik_app_qualified_name: Optional[str] = Field(
             None, description="", alias="qlikAppQualifiedName"
         )
         qlik_owner_id: Optional[str] = Field(None, description="", alias="qlikOwnerId")
         qlik_is_published: Optional[bool] = Field(
             None, description="", alias="qlikIsPublished"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "Qlik.Attributes" = Field(
-        None,
+        default_factory=lambda: Qlik.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class Tableau(BI):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in Tableau._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
-    _convience_properties: ClassVar[list[str]] = [
-        "terms",
-    ]
-
-    @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
-
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+    _convience_properties: ClassVar[list[str]] = []
 
     type_name: str = Field("Tableau", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Tableau":
             raise ValueError("must be Tableau")
         return v
 
-    class Attributes(BI.Attributes):
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
-
-    attributes: "Tableau.Attributes" = Field(
-        None,
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
 
 class Looker(BI):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in Looker._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
-    _convience_properties: ClassVar[list[str]] = [
-        "terms",
-    ]
-
-    @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
-
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+    _convience_properties: ClassVar[list[str]] = []
 
     type_name: str = Field("Looker", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Looker":
             raise ValueError("must be Looker")
         return v
 
-    class Attributes(BI.Attributes):
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
-
-    attributes: "Looker.Attributes" = Field(
-        None,
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
 
 class Redash(BI):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in Redash._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "redash_is_published",
-        "terms",
     ]
 
     @property
     def redash_is_published(self) -> Optional[bool]:
         return self.attributes.redash_is_published
 
     @redash_is_published.setter
     def redash_is_published(self, redash_is_published: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.redash_is_published = redash_is_published
 
-    @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
-
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.meanings = terms
-
     type_name: str = Field("Redash", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Redash":
             raise ValueError("must be Redash")
         return v
 
     class Attributes(BI.Attributes):
         redash_is_published: Optional[bool] = Field(
             None, description="", alias="redashIsPublished"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "Redash.Attributes" = Field(
-        None,
+        default_factory=lambda: Redash.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class Salesforce(SaaS):
     """Description"""
@@ -8920,15 +7656,14 @@
         if name in Salesforce._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "organization_qualified_name",
         "api_name",
-        "terms",
     ]
 
     @property
     def organization_qualified_name(self) -> Optional[str]:
         return self.attributes.organization_qualified_name
 
     @organization_qualified_name.setter
@@ -8943,66 +7678,30 @@
 
     @api_name.setter
     def api_name(self, api_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.api_name = api_name
 
-    @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
-
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.meanings = terms
-
     type_name: str = Field("Salesforce", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Salesforce":
             raise ValueError("must be Salesforce")
         return v
 
     class Attributes(SaaS.Attributes):
         organization_qualified_name: Optional[str] = Field(
             None, description="", alias="organizationQualifiedName"
         )
         api_name: Optional[str] = Field(None, description="", alias="apiName")
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "Salesforce.Attributes" = Field(
-        None,
+        default_factory=lambda: Salesforce.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class DbtModelColumn(Dbt):
     """Description"""
@@ -9012,15 +7711,17 @@
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "dbt_model_qualified_name",
         "dbt_model_column_data_type",
         "dbt_model_column_order",
-        "terms",
+        "dbt_model_column_sql_columns",
+        "sql_column",
+        "dbt_model",
     ]
 
     @property
     def dbt_model_qualified_name(self) -> Optional[str]:
         return self.attributes.dbt_model_qualified_name
 
     @dbt_model_qualified_name.setter
@@ -9046,24 +7747,44 @@
     @dbt_model_column_order.setter
     def dbt_model_column_order(self, dbt_model_column_order: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_model_column_order = dbt_model_column_order
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def dbt_model_column_sql_columns(self) -> Optional[list[Column]]:
+        return self.attributes.dbt_model_column_sql_columns
+
+    @dbt_model_column_sql_columns.setter
+    def dbt_model_column_sql_columns(
+        self, dbt_model_column_sql_columns: Optional[list[Column]]
+    ):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.dbt_model_column_sql_columns = dbt_model_column_sql_columns
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def sql_column(self) -> Optional[Column]:
+        return self.attributes.sql_column
+
+    @sql_column.setter
+    def sql_column(self, sql_column: Optional[Column]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.sql_column = sql_column
+
+    @property
+    def dbt_model(self) -> Optional[DbtModel]:
+        return self.attributes.dbt_model
+
+    @dbt_model.setter
+    def dbt_model(self, dbt_model: Optional[DbtModel]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.dbt_model = dbt_model
 
     type_name: str = Field("DbtModelColumn", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "DbtModelColumn":
             raise ValueError("must be DbtModelColumn")
@@ -9078,47 +7799,23 @@
         )
         dbt_model_column_order: Optional[int] = Field(
             None, description="", alias="dbtModelColumnOrder"
         )
         dbt_model_column_sql_columns: Optional[list[Column]] = Field(
             None, description="", alias="dbtModelColumnSqlColumns"
         )  # relationship
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         sql_column: Optional[Column] = Field(
             None, description="", alias="sqlColumn"
         )  # relationship
         dbt_model: Optional[DbtModel] = Field(
             None, description="", alias="dbtModel"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "DbtModelColumn.Attributes" = Field(
-        None,
+        default_factory=lambda: DbtModelColumn.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class DbtModel(Dbt):
     """Description"""
@@ -9138,15 +7835,18 @@
         "dbt_model_compile_started_at",
         "dbt_model_compile_completed_at",
         "dbt_model_execute_started_at",
         "dbt_model_execute_completed_at",
         "dbt_model_execution_time",
         "dbt_model_run_generated_at",
         "dbt_model_run_elapsed_time",
-        "terms",
+        "dbt_metrics",
+        "dbt_model_sql_assets",
+        "dbt_model_columns",
+        "sql_asset",
     ]
 
     @property
     def dbt_status(self) -> Optional[str]:
         return self.attributes.dbt_status
 
     @dbt_status.setter
@@ -9282,24 +7982,52 @@
     @dbt_model_run_elapsed_time.setter
     def dbt_model_run_elapsed_time(self, dbt_model_run_elapsed_time: Optional[float]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_model_run_elapsed_time = dbt_model_run_elapsed_time
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def dbt_metrics(self) -> Optional[list[DbtMetric]]:
+        return self.attributes.dbt_metrics
+
+    @dbt_metrics.setter
+    def dbt_metrics(self, dbt_metrics: Optional[list[DbtMetric]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.dbt_metrics = dbt_metrics
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def dbt_model_sql_assets(self) -> Optional[list[SQL]]:
+        return self.attributes.dbt_model_sql_assets
+
+    @dbt_model_sql_assets.setter
+    def dbt_model_sql_assets(self, dbt_model_sql_assets: Optional[list[SQL]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.dbt_model_sql_assets = dbt_model_sql_assets
+
+    @property
+    def dbt_model_columns(self) -> Optional[list[DbtModelColumn]]:
+        return self.attributes.dbt_model_columns
+
+    @dbt_model_columns.setter
+    def dbt_model_columns(self, dbt_model_columns: Optional[list[DbtModelColumn]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.dbt_model_columns = dbt_model_columns
+
+    @property
+    def sql_asset(self) -> Optional[SQL]:
+        return self.attributes.sql_asset
+
+    @sql_asset.setter
+    def sql_asset(self, sql_asset: Optional[SQL]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.sql_asset = sql_asset
 
     type_name: str = Field("DbtModel", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "DbtModel":
             raise ValueError("must be DbtModel")
@@ -9333,53 +8061,29 @@
         )
         dbt_model_run_generated_at: Optional[datetime] = Field(
             None, description="", alias="dbtModelRunGeneratedAt"
         )
         dbt_model_run_elapsed_time: Optional[float] = Field(
             None, description="", alias="dbtModelRunElapsedTime"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
         dbt_metrics: Optional[list[DbtMetric]] = Field(
             None, description="", alias="dbtMetrics"
         )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         dbt_model_sql_assets: Optional[list[SQL]] = Field(
             None, description="", alias="dbtModelSqlAssets"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
         dbt_model_columns: Optional[list[DbtModelColumn]] = Field(
             None, description="", alias="dbtModelColumns"
         )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
         sql_asset: Optional[SQL] = Field(
             None, description="", alias="sqlAsset"
         )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "DbtModel.Attributes" = Field(
-        None,
+        default_factory=lambda: DbtModel.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class DbtMetric(Dbt):
     """Description"""
@@ -9409,15 +8113,19 @@
         "dbt_tags",
         "dbt_connection_context",
         "dbt_semantic_layer_proxy_url",
         "metric_type",
         "metric_s_q_l",
         "metric_filters",
         "metric_time_grains",
-        "terms",
+        "metric_timestamp_column",
+        "dbt_model",
+        "assets",
+        "metric_dimension_columns",
+        "dbt_metric_filter_columns",
     ]
 
     @property
     def dbt_metric_filters(self) -> Optional[list[DbtMetricFilter]]:
         return self.attributes.dbt_metric_filters
 
     @dbt_metric_filters.setter
@@ -9647,24 +8355,66 @@
     @metric_time_grains.setter
     def metric_time_grains(self, metric_time_grains: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.metric_time_grains = metric_time_grains
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def metric_timestamp_column(self) -> Optional[Column]:
+        return self.attributes.metric_timestamp_column
+
+    @metric_timestamp_column.setter
+    def metric_timestamp_column(self, metric_timestamp_column: Optional[Column]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.metric_timestamp_column = metric_timestamp_column
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def dbt_model(self) -> Optional[DbtModel]:
+        return self.attributes.dbt_model
+
+    @dbt_model.setter
+    def dbt_model(self, dbt_model: Optional[DbtModel]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.dbt_model = dbt_model
+
+    @property
+    def assets(self) -> Optional[list[Asset]]:
+        return self.attributes.assets
+
+    @assets.setter
+    def assets(self, assets: Optional[list[Asset]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.assets = assets
+
+    @property
+    def metric_dimension_columns(self) -> Optional[list[Column]]:
+        return self.attributes.metric_dimension_columns
+
+    @metric_dimension_columns.setter
+    def metric_dimension_columns(
+        self, metric_dimension_columns: Optional[list[Column]]
+    ):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.metric_dimension_columns = metric_dimension_columns
+
+    @property
+    def dbt_metric_filter_columns(self) -> Optional[list[Column]]:
+        return self.attributes.dbt_metric_filter_columns
+
+    @dbt_metric_filter_columns.setter
+    def dbt_metric_filter_columns(
+        self, dbt_metric_filter_columns: Optional[list[Column]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.dbt_metric_filter_columns = dbt_metric_filter_columns
 
     type_name: str = Field("DbtMetric", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "DbtMetric":
             raise ValueError("must be DbtMetric")
@@ -9722,56 +8472,32 @@
         metric_s_q_l: Optional[str] = Field(None, description="", alias="metricSQL")
         metric_filters: Optional[str] = Field(
             None, description="", alias="metricFilters"
         )
         metric_time_grains: Optional[set[str]] = Field(
             None, description="", alias="metricTimeGrains"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
         metric_timestamp_column: Optional[Column] = Field(
             None, description="", alias="metricTimestampColumn"
         )  # relationship
         dbt_model: Optional[DbtModel] = Field(
             None, description="", alias="dbtModel"
         )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         assets: Optional[list[Asset]] = Field(
             None, description="", alias="assets"
         )  # relationship
         metric_dimension_columns: Optional[list[Column]] = Field(
             None, description="", alias="metricDimensionColumns"
         )  # relationship
         dbt_metric_filter_columns: Optional[list[Column]] = Field(
             None, description="", alias="dbtMetricFilterColumns"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "DbtMetric.Attributes" = Field(
-        None,
+        default_factory=lambda: DbtMetric.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class DbtSource(Dbt):
     """Description"""
@@ -9780,15 +8506,16 @@
         if name in DbtSource._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "dbt_state",
         "dbt_freshness_criteria",
-        "terms",
+        "sql_assets",
+        "sql_asset",
     ]
 
     @property
     def dbt_state(self) -> Optional[str]:
         return self.attributes.dbt_state
 
     @dbt_state.setter
@@ -9804,71 +8531,55 @@
     @dbt_freshness_criteria.setter
     def dbt_freshness_criteria(self, dbt_freshness_criteria: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_freshness_criteria = dbt_freshness_criteria
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def sql_assets(self) -> Optional[list[SQL]]:
+        return self.attributes.sql_assets
+
+    @sql_assets.setter
+    def sql_assets(self, sql_assets: Optional[list[SQL]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.sql_assets = sql_assets
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def sql_asset(self) -> Optional[SQL]:
+        return self.attributes.sql_asset
+
+    @sql_asset.setter
+    def sql_asset(self, sql_asset: Optional[SQL]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.sql_asset = sql_asset
 
     type_name: str = Field("DbtSource", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "DbtSource":
             raise ValueError("must be DbtSource")
         return v
 
     class Attributes(Dbt.Attributes):
         dbt_state: Optional[str] = Field(None, description="", alias="dbtState")
         dbt_freshness_criteria: Optional[str] = Field(
             None, description="", alias="dbtFreshnessCriteria"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         sql_assets: Optional[list[SQL]] = Field(
             None, description="", alias="sqlAssets"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
         sql_asset: Optional[SQL] = Field(
             None, description="", alias="sqlAsset"
         )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "DbtSource.Attributes" = Field(
-        None,
+        default_factory=lambda: DbtSource.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class DbtProcess(Dbt):
     """Description"""
@@ -9899,15 +8610,15 @@
         "dbt_connection_context",
         "dbt_semantic_layer_proxy_url",
         "inputs",
         "outputs",
         "code",
         "sql",
         "ast",
-        "terms",
+        "column_processes",
     ]
 
     @property
     def dbt_process_job_status(self) -> Optional[str]:
         return self.attributes.dbt_process_job_status
 
     @dbt_process_job_status.setter
@@ -10147,24 +8858,22 @@
     @ast.setter
     def ast(self, ast: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.ast = ast
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+    def column_processes(self) -> Optional[list[ColumnProcess]]:
+        return self.attributes.column_processes
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @column_processes.setter
+    def column_processes(self, column_processes: Optional[list[ColumnProcess]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.column_processes = column_processes
 
     type_name: str = Field("DbtProcess", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "DbtProcess":
             raise ValueError("must be DbtProcess")
@@ -10219,44 +8928,20 @@
             None, description="", alias="dbtSemanticLayerProxyUrl"
         )
         inputs: Optional[list[Catalog]] = Field(None, description="", alias="inputs")
         outputs: Optional[list[Catalog]] = Field(None, description="", alias="outputs")
         code: Optional[str] = Field(None, description="", alias="code")
         sql: Optional[str] = Field(None, description="", alias="sql")
         ast: Optional[str] = Field(None, description="", alias="ast")
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
         column_processes: Optional[list[ColumnProcess]] = Field(
             None, description="", alias="columnProcesses"
         )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "DbtProcess.Attributes" = Field(
-        None,
+        default_factory=lambda: DbtProcess.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class ReadmeTemplate(Resource):
     """Description"""
@@ -10265,15 +8950,14 @@
         if name in ReadmeTemplate._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "icon",
         "icon_type",
-        "terms",
     ]
 
     @property
     def icon(self) -> Optional[str]:
         return self.attributes.icon
 
     @icon.setter
@@ -10288,92 +8972,76 @@
 
     @icon_type.setter
     def icon_type(self, icon_type: Optional[IconType]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.icon_type = icon_type
 
-    @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
-
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.meanings = terms
-
     type_name: str = Field("ReadmeTemplate", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "ReadmeTemplate":
             raise ValueError("must be ReadmeTemplate")
         return v
 
     class Attributes(Resource.Attributes):
         icon: Optional[str] = Field(None, description="", alias="icon")
         icon_type: Optional[IconType] = Field(None, description="", alias="iconType")
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "ReadmeTemplate.Attributes" = Field(
-        None,
+        default_factory=lambda: ReadmeTemplate.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class Readme(Resource):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in Readme._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
-        "terms",
+        "internal",
+        "asset",
+        "see_also",
     ]
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def internal(self) -> Optional[Internal]:
+        return self.attributes.internal
+
+    @internal.setter
+    def internal(self, internal: Optional[Internal]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.internal = internal
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def asset(self) -> Optional[Asset]:
+        return self.attributes.asset
+
+    @asset.setter
+    def asset(self, asset: Optional[Asset]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.asset = asset
+
+    @property
+    def see_also(self) -> Optional[list[Readme]]:
+        return self.attributes.see_also
+
+    @see_also.setter
+    def see_also(self, see_also: Optional[list[Readme]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.see_also = see_also
 
     type_name: str = Field("Readme", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Readme":
             raise ValueError("must be Readme")
@@ -10400,47 +9068,23 @@
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.description = (
             quote(description) if description is not None else description
         )
 
     class Attributes(Resource.Attributes):
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         internal: Optional[Internal] = Field(
             None, description="", alias="__internal"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
         asset: Optional[Asset] = Field(
             None, description="", alias="asset"
         )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
         see_also: Optional[list[Readme]] = Field(
             None, description="", alias="seeAlso"
         )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
         @classmethod
         # @validate_arguments()
         def create(
             cls, *, asset: Asset, content: str, asset_name: Optional[str] = None
         ) -> Readme.Attributes:
             validate_required_fields(["asset", "content"], [asset, content])
@@ -10459,15 +9103,81 @@
                 qualified_name=f"{asset.guid}/readme",
                 name=f"{asset_name} Readme",
                 asset=asset,
                 description=quote(content),
             )
 
     attributes: "Readme.Attributes" = Field(
-        None,
+        default_factory=lambda: Readme.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
+class File(Resource):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in File._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "file_type",
+        "file_path",
+        "file_assets",
+    ]
+
+    @property
+    def file_type(self) -> Optional[FileType]:
+        return self.attributes.file_type
+
+    @file_type.setter
+    def file_type(self, file_type: Optional[FileType]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.file_type = file_type
+
+    @property
+    def file_path(self) -> Optional[str]:
+        return self.attributes.file_path
+
+    @file_path.setter
+    def file_path(self, file_path: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.file_path = file_path
+
+    @property
+    def file_assets(self) -> Optional[Asset]:
+        return self.attributes.file_assets
+
+    @file_assets.setter
+    def file_assets(self, file_assets: Optional[Asset]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.file_assets = file_assets
+
+    type_name: str = Field("File", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "File":
+            raise ValueError("must be File")
+        return v
+
+    class Attributes(Resource.Attributes):
+        file_type: Optional[FileType] = Field(None, description="", alias="fileType")
+        file_path: Optional[str] = Field(None, description="", alias="filePath")
+        file_assets: Optional[Asset] = Field(
+            None, description="", alias="fileAssets"
+        )  # relationship
+
+    attributes: "File.Attributes" = Field(
+        default_factory=lambda: File.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class Link(Resource):
     """Description"""
@@ -10476,15 +9186,16 @@
         if name in Link._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "icon",
         "icon_type",
-        "terms",
+        "internal",
+        "asset",
     ]
 
     @property
     def icon(self) -> Optional[str]:
         return self.attributes.icon
 
     @icon.setter
@@ -10500,69 +9211,53 @@
     @icon_type.setter
     def icon_type(self, icon_type: Optional[IconType]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.icon_type = icon_type
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def internal(self) -> Optional[Internal]:
+        return self.attributes.internal
+
+    @internal.setter
+    def internal(self, internal: Optional[Internal]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.internal = internal
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def asset(self) -> Optional[Asset]:
+        return self.attributes.asset
+
+    @asset.setter
+    def asset(self, asset: Optional[Asset]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.asset = asset
 
     type_name: str = Field("Link", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Link":
             raise ValueError("must be Link")
         return v
 
     class Attributes(Resource.Attributes):
         icon: Optional[str] = Field(None, description="", alias="icon")
         icon_type: Optional[IconType] = Field(None, description="", alias="iconType")
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
         internal: Optional[Internal] = Field(
             None, description="", alias="internal"
         )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
         asset: Optional[Asset] = Field(
             None, description="", alias="asset"
         )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "Link.Attributes" = Field(
-        None,
+        default_factory=lambda: Link.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class APISpec(API):
     """Description"""
@@ -10577,15 +9272,15 @@
         "api_spec_contact_email",
         "api_spec_contact_name",
         "api_spec_contact_url",
         "api_spec_license_name",
         "api_spec_license_url",
         "api_spec_contract_version",
         "api_spec_service_alias",
-        "terms",
+        "api_paths",
     ]
 
     @property
     def api_spec_terms_of_service_url(self) -> Optional[str]:
         return self.attributes.api_spec_terms_of_service_url
 
     @api_spec_terms_of_service_url.setter
@@ -10663,24 +9358,22 @@
     @api_spec_service_alias.setter
     def api_spec_service_alias(self, api_spec_service_alias: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.api_spec_service_alias = api_spec_service_alias
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+    def api_paths(self) -> Optional[list[APIPath]]:
+        return self.attributes.api_paths
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @api_paths.setter
+    def api_paths(self, api_paths: Optional[list[APIPath]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.api_paths = api_paths
 
     type_name: str = Field("APISpec", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "APISpec":
             raise ValueError("must be APISpec")
@@ -10707,44 +9400,20 @@
         )
         api_spec_contract_version: Optional[str] = Field(
             None, description="", alias="apiSpecContractVersion"
         )
         api_spec_service_alias: Optional[str] = Field(
             None, description="", alias="apiSpecServiceAlias"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         api_paths: Optional[list[APIPath]] = Field(
             None, description="", alias="apiPaths"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "APISpec.Attributes" = Field(
-        None,
+        default_factory=lambda: APISpec.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class APIPath(API):
     """Description"""
@@ -10757,15 +9426,15 @@
     _convience_properties: ClassVar[list[str]] = [
         "api_path_summary",
         "api_path_raw_u_r_i",
         "api_path_is_templated",
         "api_path_available_operations",
         "api_path_available_response_codes",
         "api_path_is_ingress_exposed",
-        "terms",
+        "api_spec",
     ]
 
     @property
     def api_path_summary(self) -> Optional[str]:
         return self.attributes.api_path_summary
 
     @api_path_summary.setter
@@ -10827,24 +9496,22 @@
     @api_path_is_ingress_exposed.setter
     def api_path_is_ingress_exposed(self, api_path_is_ingress_exposed: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.api_path_is_ingress_exposed = api_path_is_ingress_exposed
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+    def api_spec(self) -> Optional[APISpec]:
+        return self.attributes.api_spec
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @api_spec.setter
+    def api_spec(self, api_spec: Optional[APISpec]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.api_spec = api_spec
 
     type_name: str = Field("APIPath", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "APIPath":
             raise ValueError("must be APIPath")
@@ -10865,44 +9532,20 @@
         )
         api_path_available_response_codes: Optional[dict[str, str]] = Field(
             None, description="", alias="apiPathAvailableResponseCodes"
         )
         api_path_is_ingress_exposed: Optional[bool] = Field(
             None, description="", alias="apiPathIsIngressExposed"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
         api_spec: Optional[APISpec] = Field(
             None, description="", alias="apiSpec"
         )  # relationship
 
     attributes: "APIPath.Attributes" = Field(
-        None,
+        default_factory=lambda: APIPath.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class SnowflakeTag(Tag):
     """Description"""
@@ -10927,15 +9570,19 @@
         "schema_qualified_name",
         "table_name",
         "table_qualified_name",
         "view_name",
         "view_qualified_name",
         "is_profiled",
         "last_profiled_at",
-        "terms",
+        "dbt_sources",
+        "sql_dbt_models",
+        "sql_dbt_sources",
+        "dbt_models",
+        "atlan_schema",
     ]
 
     @property
     def tag_id(self) -> Optional[str]:
         return self.attributes.tag_id
 
     @tag_id.setter
@@ -11111,24 +9758,62 @@
     @last_profiled_at.setter
     def last_profiled_at(self, last_profiled_at: Optional[datetime]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.last_profiled_at = last_profiled_at
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def dbt_sources(self) -> Optional[list[DbtSource]]:
+        return self.attributes.dbt_sources
+
+    @dbt_sources.setter
+    def dbt_sources(self, dbt_sources: Optional[list[DbtSource]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.dbt_sources = dbt_sources
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def sql_dbt_models(self) -> Optional[list[DbtModel]]:
+        return self.attributes.sql_dbt_models
+
+    @sql_dbt_models.setter
+    def sql_dbt_models(self, sql_dbt_models: Optional[list[DbtModel]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.sql_dbt_models = sql_dbt_models
+
+    @property
+    def sql_dbt_sources(self) -> Optional[list[DbtSource]]:
+        return self.attributes.sql_dbt_sources
+
+    @sql_dbt_sources.setter
+    def sql_dbt_sources(self, sql_dbt_sources: Optional[list[DbtSource]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.sql_dbt_sources = sql_dbt_sources
+
+    @property
+    def dbt_models(self) -> Optional[list[DbtModel]]:
+        return self.attributes.dbt_models
+
+    @dbt_models.setter
+    def dbt_models(self, dbt_models: Optional[list[DbtModel]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.dbt_models = dbt_models
+
+    @property
+    def atlan_schema(self) -> Optional[Schema]:
+        return self.attributes.atlan_schema
+
+    @atlan_schema.setter
+    def atlan_schema(self, atlan_schema: Optional[Schema]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.atlan_schema = atlan_schema
 
     type_name: str = Field("SnowflakeTag", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "SnowflakeTag":
             raise ValueError("must be SnowflakeTag")
@@ -11171,56 +9856,32 @@
         view_qualified_name: Optional[str] = Field(
             None, description="", alias="viewQualifiedName"
         )
         is_profiled: Optional[bool] = Field(None, description="", alias="isProfiled")
         last_profiled_at: Optional[datetime] = Field(
             None, description="", alias="lastProfiledAt"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
         dbt_sources: Optional[list[DbtSource]] = Field(
             None, description="", alias="dbtSources"
         )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
         sql_dbt_models: Optional[list[DbtModel]] = Field(
             None, description="", alias="sqlDbtModels"
         )  # relationship
         sql_dbt_sources: Optional[list[DbtSource]] = Field(
             None, description="", alias="sqlDBTSources"
         )  # relationship
         dbt_models: Optional[list[DbtModel]] = Field(
             None, description="", alias="dbtModels"
         )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         atlan_schema: Optional[Schema] = Field(
             None, description="", alias="atlanSchema"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "SnowflakeTag.Attributes" = Field(
-        None,
+        default_factory=lambda: SnowflakeTag.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class TablePartition(SQL):
     """Description"""
@@ -11242,15 +9903,16 @@
         "external_location",
         "external_location_region",
         "external_location_format",
         "is_partitioned",
         "partition_strategy",
         "partition_count",
         "partition_list",
-        "terms",
+        "columns",
+        "parent_table",
     ]
 
     @property
     def constraint(self) -> Optional[str]:
         return self.attributes.constraint
 
     @constraint.setter
@@ -11396,24 +10058,32 @@
     @partition_list.setter
     def partition_list(self, partition_list: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.partition_list = partition_list
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def columns(self) -> Optional[list[Column]]:
+        return self.attributes.columns
+
+    @columns.setter
+    def columns(self, columns: Optional[list[Column]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.columns = columns
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def parent_table(self) -> Optional[Table]:
+        return self.attributes.parent_table
+
+    @parent_table.setter
+    def parent_table(self, parent_table: Optional[Table]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.parent_table = parent_table
 
     type_name: str = Field("TablePartition", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "TablePartition":
             raise ValueError("must be TablePartition")
@@ -11449,59 +10119,23 @@
         )
         partition_count: Optional[int] = Field(
             None, description="", alias="partitionCount"
         )
         partition_list: Optional[str] = Field(
             None, description="", alias="partitionList"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        dbt_sources: Optional[list[DbtSource]] = Field(
-            None, description="", alias="dbtSources"
-        )  # relationship
         columns: Optional[list[Column]] = Field(
             None, description="", alias="columns"
         )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        sql_dbt_models: Optional[list[DbtModel]] = Field(
-            None, description="", alias="sqlDbtModels"
-        )  # relationship
-        sql_dbt_sources: Optional[list[DbtSource]] = Field(
-            None, description="", alias="sqlDBTSources"
-        )  # relationship
-        dbt_models: Optional[list[DbtModel]] = Field(
-            None, description="", alias="dbtModels"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
         parent_table: Optional[Table] = Field(
             None, description="", alias="parentTable"
         )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "TablePartition.Attributes" = Field(
-        None,
+        default_factory=lambda: TablePartition.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class Table(SQL):
     """Description"""
@@ -11522,15 +10156,18 @@
         "external_location",
         "external_location_region",
         "external_location_format",
         "is_partitioned",
         "partition_strategy",
         "partition_count",
         "partition_list",
-        "terms",
+        "partitions",
+        "columns",
+        "queries",
+        "atlan_schema",
     ]
 
     @property
     def column_count(self) -> Optional[int]:
         return self.attributes.column_count
 
     @column_count.setter
@@ -11666,24 +10303,52 @@
     @partition_list.setter
     def partition_list(self, partition_list: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.partition_list = partition_list
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def partitions(self) -> Optional[list[TablePartition]]:
+        return self.attributes.partitions
+
+    @partitions.setter
+    def partitions(self, partitions: Optional[list[TablePartition]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.partitions = partitions
+
+    @property
+    def columns(self) -> Optional[list[Column]]:
+        return self.attributes.columns
+
+    @columns.setter
+    def columns(self, columns: Optional[list[Column]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.columns = columns
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def queries(self) -> Optional[list[Query]]:
+        return self.attributes.queries
+
+    @queries.setter
+    def queries(self, queries: Optional[list[Query]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.queries = queries
+
+    @property
+    def atlan_schema(self) -> Optional[Schema]:
+        return self.attributes.atlan_schema
+
+    @atlan_schema.setter
+    def atlan_schema(self, atlan_schema: Optional[Schema]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.atlan_schema = atlan_schema
 
     type_name: str = Field("Table", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Table":
             raise ValueError("must be Table")
@@ -11721,59 +10386,23 @@
         )
         partition_list: Optional[str] = Field(
             None, description="", alias="partitionList"
         )
         partitions: Optional[list[TablePartition]] = Field(
             None, description="", alias="partitions"
         )  # relationship
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        dbt_sources: Optional[list[DbtSource]] = Field(
-            None, description="", alias="dbtSources"
-        )  # relationship
         columns: Optional[list[Column]] = Field(
             None, description="", alias="columns"
         )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
         queries: Optional[list[Query]] = Field(
             None, description="", alias="queries"
         )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        sql_dbt_models: Optional[list[DbtModel]] = Field(
-            None, description="", alias="sqlDbtModels"
-        )  # relationship
-        sql_dbt_sources: Optional[list[DbtSource]] = Field(
-            None, description="", alias="sqlDBTSources"
-        )  # relationship
-        dbt_models: Optional[list[DbtModel]] = Field(
-            None, description="", alias="dbtModels"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         atlan_schema: Optional[Schema] = Field(
             None, description="", alias="atlanSchema"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
         @classmethod
         # @validate_arguments()
         def create(cls, *, name: str, schema_qualified_name: str) -> Table.Attributes:
             if not name:
                 raise ValueError("name cannot be blank")
             validate_required_fields(["schema_qualified_name"], [schema_qualified_name])
@@ -11793,15 +10422,15 @@
                 schema_qualified_name=schema_qualified_name,
                 schema_name=fields[4],
                 connector_name=connector_type.value,
                 atlan_schema=Schema.ref_by_qualified_name(schema_qualified_name),
             )
 
     attributes: "Table.Attributes" = Field(
-        None,
+        default_factory=lambda: Table.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
     @classmethod
     # @validate_arguments()
     def create(cls, *, name: str, schema_qualified_name: str) -> Table:
@@ -11829,15 +10458,18 @@
         "variables_schema_base64",
         "is_private",
         "is_sql_snippet",
         "parent_qualified_name",
         "collection_qualified_name",
         "is_visual_query",
         "visual_builder_schema_base64",
-        "terms",
+        "parent",
+        "columns",
+        "tables",
+        "views",
     ]
 
     @property
     def raw_query(self) -> Optional[str]:
         return self.attributes.raw_query
 
     @raw_query.setter
@@ -11939,24 +10571,52 @@
     @visual_builder_schema_base64.setter
     def visual_builder_schema_base64(self, visual_builder_schema_base64: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.visual_builder_schema_base64 = visual_builder_schema_base64
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def parent(self) -> Namespace:
+        return self.attributes.parent
+
+    @parent.setter
+    def parent(self, parent: Namespace):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.parent = parent
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def columns(self) -> Optional[list[Column]]:
+        return self.attributes.columns
+
+    @columns.setter
+    def columns(self, columns: Optional[list[Column]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.columns = columns
+
+    @property
+    def tables(self) -> Optional[list[Table]]:
+        return self.attributes.tables
+
+    @tables.setter
+    def tables(self, tables: Optional[list[Table]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.tables = tables
+
+    @property
+    def views(self) -> Optional[list[View]]:
+        return self.attributes.views
+
+    @views.setter
+    def views(self, views: Optional[list[View]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.views = views
 
     type_name: str = Field("Query", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Query":
             raise ValueError("must be Query")
@@ -11985,63 +10645,27 @@
         )
         is_visual_query: Optional[bool] = Field(
             None, description="", alias="isVisualQuery"
         )
         visual_builder_schema_base64: Optional[str] = Field(
             None, description="", alias="visualBuilderSchemaBase64"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
         parent: Namespace = Field(None, description="", alias="parent")  # relationship
-        dbt_sources: Optional[list[DbtSource]] = Field(
-            None, description="", alias="dbtSources"
-        )  # relationship
         columns: Optional[list[Column]] = Field(
             None, description="", alias="columns"
         )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        sql_dbt_models: Optional[list[DbtModel]] = Field(
-            None, description="", alias="sqlDbtModels"
-        )  # relationship
-        sql_dbt_sources: Optional[list[DbtSource]] = Field(
-            None, description="", alias="sqlDBTSources"
-        )  # relationship
-        dbt_models: Optional[list[DbtModel]] = Field(
-            None, description="", alias="dbtModels"
-        )  # relationship
         tables: Optional[list[Table]] = Field(
             None, description="", alias="tables"
         )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
         views: Optional[list[View]] = Field(
             None, description="", alias="views"
         )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "Query.Attributes" = Field(
-        None,
+        default_factory=lambda: Query.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class Column(SQL):
     """Description"""
@@ -12093,15 +10717,26 @@
         "column_mins",
         "column_missing_values_count",
         "column_missing_values_count_long",
         "column_missing_values_percentage",
         "column_uniqueness_percentage",
         "column_variance",
         "column_top_values",
-        "terms",
+        "view",
+        "data_quality_metric_dimensions",
+        "dbt_model_columns",
+        "table",
+        "column_dbt_model_columns",
+        "materialised_view",
+        "queries",
+        "metric_timestamps",
+        "foreign_key_to",
+        "foreign_key_from",
+        "dbt_metrics",
+        "table_partition",
     ]
 
     @property
     def data_type(self) -> Optional[str]:
         return self.attributes.data_type
 
     @data_type.setter
@@ -12573,24 +11208,136 @@
         self, column_top_values: Optional[list[ColumnValueFrequencyMap]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.column_top_values = column_top_values
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def view(self) -> Optional[View]:
+        return self.attributes.view
+
+    @view.setter
+    def view(self, view: Optional[View]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.view = view
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def data_quality_metric_dimensions(self) -> Optional[list[Metric]]:
+        return self.attributes.data_quality_metric_dimensions
+
+    @data_quality_metric_dimensions.setter
+    def data_quality_metric_dimensions(
+        self, data_quality_metric_dimensions: Optional[list[Metric]]
+    ):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.data_quality_metric_dimensions = data_quality_metric_dimensions
+
+    @property
+    def dbt_model_columns(self) -> Optional[list[DbtModelColumn]]:
+        return self.attributes.dbt_model_columns
+
+    @dbt_model_columns.setter
+    def dbt_model_columns(self, dbt_model_columns: Optional[list[DbtModelColumn]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.dbt_model_columns = dbt_model_columns
+
+    @property
+    def table(self) -> Optional[Table]:
+        return self.attributes.table
+
+    @table.setter
+    def table(self, table: Optional[Table]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.table = table
+
+    @property
+    def column_dbt_model_columns(self) -> Optional[list[DbtModelColumn]]:
+        return self.attributes.column_dbt_model_columns
+
+    @column_dbt_model_columns.setter
+    def column_dbt_model_columns(
+        self, column_dbt_model_columns: Optional[list[DbtModelColumn]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.column_dbt_model_columns = column_dbt_model_columns
+
+    @property
+    def materialised_view(self) -> Optional[MaterialisedView]:
+        return self.attributes.materialised_view
+
+    @materialised_view.setter
+    def materialised_view(self, materialised_view: Optional[MaterialisedView]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.materialised_view = materialised_view
+
+    @property
+    def queries(self) -> Optional[list[Query]]:
+        return self.attributes.queries
+
+    @queries.setter
+    def queries(self, queries: Optional[list[Query]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.queries = queries
+
+    @property
+    def metric_timestamps(self) -> Optional[list[Metric]]:
+        return self.attributes.metric_timestamps
+
+    @metric_timestamps.setter
+    def metric_timestamps(self, metric_timestamps: Optional[list[Metric]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.metric_timestamps = metric_timestamps
+
+    @property
+    def foreign_key_to(self) -> Optional[list[Column]]:
+        return self.attributes.foreign_key_to
+
+    @foreign_key_to.setter
+    def foreign_key_to(self, foreign_key_to: Optional[list[Column]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.foreign_key_to = foreign_key_to
+
+    @property
+    def foreign_key_from(self) -> Optional[Column]:
+        return self.attributes.foreign_key_from
+
+    @foreign_key_from.setter
+    def foreign_key_from(self, foreign_key_from: Optional[Column]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.foreign_key_from = foreign_key_from
+
+    @property
+    def dbt_metrics(self) -> Optional[list[DbtMetric]]:
+        return self.attributes.dbt_metrics
+
+    @dbt_metrics.setter
+    def dbt_metrics(self, dbt_metrics: Optional[list[DbtMetric]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.dbt_metrics = dbt_metrics
+
+    @property
+    def table_partition(self) -> Optional[TablePartition]:
+        return self.attributes.table_partition
+
+    @table_partition.setter
+    def table_partition(self, table_partition: Optional[TablePartition]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.table_partition = table_partition
 
     type_name: str = Field("Column", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Column":
             raise ValueError("must be Column")
@@ -12686,84 +11433,48 @@
         )
         column_variance: Optional[float] = Field(
             None, description="", alias="columnVariance"
         )
         column_top_values: Optional[list[ColumnValueFrequencyMap]] = Field(
             None, description="", alias="columnTopValues"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
+        view: Optional[View] = Field(None, description="", alias="view")  # relationship
+        data_quality_metric_dimensions: Optional[list[Metric]] = Field(
+            None, description="", alias="dataQualityMetricDimensions"
         )  # relationship
-        dbt_sources: Optional[list[DbtSource]] = Field(
-            None, description="", alias="dbtSources"
+        dbt_model_columns: Optional[list[DbtModelColumn]] = Field(
+            None, description="", alias="dbtModelColumns"
+        )  # relationship
+        table: Optional[Table] = Field(
+            None, description="", alias="table"
+        )  # relationship
+        column_dbt_model_columns: Optional[list[DbtModelColumn]] = Field(
+            None, description="", alias="columnDbtModelColumns"
         )  # relationship
         materialised_view: Optional[MaterialisedView] = Field(
             None, description="", alias="materialisedView"
         )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
         queries: Optional[list[Query]] = Field(
             None, description="", alias="queries"
         )  # relationship
         metric_timestamps: Optional[list[Metric]] = Field(
             None, description="", alias="metricTimestamps"
         )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        sql_dbt_models: Optional[list[DbtModel]] = Field(
-            None, description="", alias="sqlDbtModels"
-        )  # relationship
         foreign_key_to: Optional[list[Column]] = Field(
             None, description="", alias="foreignKeyTo"
         )  # relationship
-        sql_dbt_sources: Optional[list[DbtSource]] = Field(
-            None, description="", alias="sqlDBTSources"
-        )  # relationship
         foreign_key_from: Optional[Column] = Field(
             None, description="", alias="foreignKeyFrom"
         )  # relationship
         dbt_metrics: Optional[list[DbtMetric]] = Field(
             None, description="", alias="dbtMetrics"
         )  # relationship
-        dbt_models: Optional[list[DbtModel]] = Field(
-            None, description="", alias="dbtModels"
-        )  # relationship
-        view: Optional[View] = Field(None, description="", alias="view")  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
         table_partition: Optional[TablePartition] = Field(
             None, description="", alias="tablePartition"
         )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        data_quality_metric_dimensions: Optional[list[Metric]] = Field(
-            None, description="", alias="dataQualityMetricDimensions"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        dbt_model_columns: Optional[list[DbtModelColumn]] = Field(
-            None, description="", alias="dbtModelColumns"
-        )  # relationship
-        table: Optional[Table] = Field(
-            None, description="", alias="table"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
-        column_dbt_model_columns: Optional[list[DbtModelColumn]] = Field(
-            None, description="", alias="columnDbtModelColumns"
-        )  # relationship
 
         @classmethod
         # @validate_arguments()
         def create(
             cls, *, name: str, parent_qualified_name: str, parent_type: type, order: int
         ) -> Column.Attributes:
             if not name:
@@ -12815,15 +11526,15 @@
                 parent_qualified_name=parent_qualified_name,
                 parent_type=parent_type,
                 order=order,
             )
         )
 
     attributes: "Column.Attributes" = Field(
-        None,
+        default_factory=lambda: Column.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class Schema(SQL):
     """Description"""
@@ -12832,15 +11543,22 @@
         if name in Schema._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "table_count",
         "views_count",
-        "terms",
+        "snowflake_tags",
+        "materialised_views",
+        "tables",
+        "database",
+        "snowflake_pipes",
+        "snowflake_streams",
+        "procedures",
+        "views",
     ]
 
     @property
     def table_count(self) -> Optional[int]:
         return self.attributes.table_count
 
     @table_count.setter
@@ -12856,24 +11574,92 @@
     @views_count.setter
     def views_count(self, views_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.views_count = views_count
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def snowflake_tags(self) -> Optional[list[SnowflakeTag]]:
+        return self.attributes.snowflake_tags
+
+    @snowflake_tags.setter
+    def snowflake_tags(self, snowflake_tags: Optional[list[SnowflakeTag]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.snowflake_tags = snowflake_tags
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def materialised_views(self) -> Optional[list[MaterialisedView]]:
+        return self.attributes.materialised_views
+
+    @materialised_views.setter
+    def materialised_views(self, materialised_views: Optional[list[MaterialisedView]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.materialised_views = materialised_views
+
+    @property
+    def tables(self) -> Optional[list[Table]]:
+        return self.attributes.tables
+
+    @tables.setter
+    def tables(self, tables: Optional[list[Table]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.tables = tables
+
+    @property
+    def database(self) -> Optional[Database]:
+        return self.attributes.database
+
+    @database.setter
+    def database(self, database: Optional[Database]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.database = database
+
+    @property
+    def snowflake_pipes(self) -> Optional[list[SnowflakePipe]]:
+        return self.attributes.snowflake_pipes
+
+    @snowflake_pipes.setter
+    def snowflake_pipes(self, snowflake_pipes: Optional[list[SnowflakePipe]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.snowflake_pipes = snowflake_pipes
+
+    @property
+    def snowflake_streams(self) -> Optional[list[SnowflakeStream]]:
+        return self.attributes.snowflake_streams
+
+    @snowflake_streams.setter
+    def snowflake_streams(self, snowflake_streams: Optional[list[SnowflakeStream]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.snowflake_streams = snowflake_streams
+
+    @property
+    def procedures(self) -> Optional[list[Procedure]]:
+        return self.attributes.procedures
+
+    @procedures.setter
+    def procedures(self, procedures: Optional[list[Procedure]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.procedures = procedures
+
+    @property
+    def views(self) -> Optional[list[View]]:
+        return self.attributes.views
+
+    @views.setter
+    def views(self, views: Optional[list[View]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.views = views
 
     type_name: str = Field("Schema", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Schema":
             raise ValueError("must be Schema")
@@ -12884,68 +11670,32 @@
         views_count: Optional[int] = Field(None, description="", alias="viewsCount")
         snowflake_tags: Optional[list[SnowflakeTag]] = Field(
             None, description="", alias="snowflakeTags"
         )  # relationship
         materialised_views: Optional[list[MaterialisedView]] = Field(
             None, description="", alias="materialisedViews"
         )  # relationship
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        dbt_sources: Optional[list[DbtSource]] = Field(
-            None, description="", alias="dbtSources"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        sql_dbt_models: Optional[list[DbtModel]] = Field(
-            None, description="", alias="sqlDbtModels"
-        )  # relationship
-        sql_dbt_sources: Optional[list[DbtSource]] = Field(
-            None, description="", alias="sqlDBTSources"
-        )  # relationship
-        dbt_models: Optional[list[DbtModel]] = Field(
-            None, description="", alias="dbtModels"
-        )  # relationship
         tables: Optional[list[Table]] = Field(
             None, description="", alias="tables"
         )  # relationship
         database: Optional[Database] = Field(
             None, description="", alias="database"
         )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         snowflake_pipes: Optional[list[SnowflakePipe]] = Field(
             None, description="", alias="snowflakePipes"
         )  # relationship
         snowflake_streams: Optional[list[SnowflakeStream]] = Field(
             None, description="", alias="snowflakeStreams"
         )  # relationship
         procedures: Optional[list[Procedure]] = Field(
             None, description="", alias="procedures"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
         views: Optional[list[View]] = Field(
             None, description="", alias="views"
         )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
         @classmethod
         # @validate_arguments()
         def create(
             cls, *, name: str, database_qualified_name: str
         ) -> Schema.Attributes:
             if not name:
@@ -12967,15 +11717,15 @@
                 database_qualified_name=database_qualified_name,
                 qualified_name=f"{database_qualified_name}/{name}",
                 connector_name=connector_type.value,
                 database=Database.ref_by_qualified_name(database_qualified_name),
             )
 
     attributes: "Schema.Attributes" = Field(
-        None,
+        default_factory=lambda: Schema.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
     @classmethod
     # @validate_arguments()
     def create(cls, *, name: str, database_qualified_name: str) -> Schema:
@@ -12998,15 +11748,15 @@
 
     _convience_properties: ClassVar[list[str]] = [
         "snowflake_stream_type",
         "snowflake_stream_source_type",
         "snowflake_stream_mode",
         "snowflake_stream_is_stale",
         "snowflake_stream_stale_after",
-        "terms",
+        "atlan_schema",
     ]
 
     @property
     def snowflake_stream_type(self) -> Optional[str]:
         return self.attributes.snowflake_stream_type
 
     @snowflake_stream_type.setter
@@ -13054,24 +11804,22 @@
         self, snowflake_stream_stale_after: Optional[datetime]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.snowflake_stream_stale_after = snowflake_stream_stale_after
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+    def atlan_schema(self) -> Optional[Schema]:
+        return self.attributes.atlan_schema
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @atlan_schema.setter
+    def atlan_schema(self, atlan_schema: Optional[Schema]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.atlan_schema = atlan_schema
 
     type_name: str = Field("SnowflakeStream", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "SnowflakeStream":
             raise ValueError("must be SnowflakeStream")
@@ -13089,56 +11837,20 @@
         )
         snowflake_stream_is_stale: Optional[bool] = Field(
             None, description="", alias="snowflakeStreamIsStale"
         )
         snowflake_stream_stale_after: Optional[datetime] = Field(
             None, description="", alias="snowflakeStreamStaleAfter"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        dbt_sources: Optional[list[DbtSource]] = Field(
-            None, description="", alias="dbtSources"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        sql_dbt_models: Optional[list[DbtModel]] = Field(
-            None, description="", alias="sqlDbtModels"
-        )  # relationship
-        sql_dbt_sources: Optional[list[DbtSource]] = Field(
-            None, description="", alias="sqlDBTSources"
-        )  # relationship
-        dbt_models: Optional[list[DbtModel]] = Field(
-            None, description="", alias="dbtModels"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         atlan_schema: Optional[Schema] = Field(
             None, description="", alias="atlanSchema"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "SnowflakeStream.Attributes" = Field(
-        None,
+        default_factory=lambda: SnowflakeStream.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class SnowflakePipe(SQL):
     """Description"""
@@ -13148,15 +11860,15 @@
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "definition",
         "snowflake_pipe_is_auto_ingest_enabled",
         "snowflake_pipe_notification_channel_name",
-        "terms",
+        "atlan_schema",
     ]
 
     @property
     def definition(self) -> Optional[str]:
         return self.attributes.definition
 
     @definition.setter
@@ -13190,24 +11902,22 @@
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.snowflake_pipe_notification_channel_name = (
             snowflake_pipe_notification_channel_name
         )
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+    def atlan_schema(self) -> Optional[Schema]:
+        return self.attributes.atlan_schema
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @atlan_schema.setter
+    def atlan_schema(self, atlan_schema: Optional[Schema]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.atlan_schema = atlan_schema
 
     type_name: str = Field("SnowflakePipe", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "SnowflakePipe":
             raise ValueError("must be SnowflakePipe")
@@ -13217,56 +11927,20 @@
         definition: Optional[str] = Field(None, description="", alias="definition")
         snowflake_pipe_is_auto_ingest_enabled: Optional[bool] = Field(
             None, description="", alias="snowflakePipeIsAutoIngestEnabled"
         )
         snowflake_pipe_notification_channel_name: Optional[str] = Field(
             None, description="", alias="snowflakePipeNotificationChannelName"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        dbt_sources: Optional[list[DbtSource]] = Field(
-            None, description="", alias="dbtSources"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        sql_dbt_models: Optional[list[DbtModel]] = Field(
-            None, description="", alias="sqlDbtModels"
-        )  # relationship
-        sql_dbt_sources: Optional[list[DbtSource]] = Field(
-            None, description="", alias="sqlDBTSources"
-        )  # relationship
-        dbt_models: Optional[list[DbtModel]] = Field(
-            None, description="", alias="dbtModels"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         atlan_schema: Optional[Schema] = Field(
             None, description="", alias="atlanSchema"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "SnowflakePipe.Attributes" = Field(
-        None,
+        default_factory=lambda: SnowflakePipe.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class Database(SQL):
     """Description"""
@@ -13274,88 +11948,50 @@
     def __setattr__(self, name, value):
         if name in Database._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "schema_count",
-        "terms",
+        "schemas",
     ]
 
     @property
     def schema_count(self) -> Optional[int]:
         return self.attributes.schema_count
 
     @schema_count.setter
     def schema_count(self, schema_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.schema_count = schema_count
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+    def schemas(self) -> Optional[list[Schema]]:
+        return self.attributes.schemas
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @schemas.setter
+    def schemas(self, schemas: Optional[list[Schema]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.schemas = schemas
 
     type_name: str = Field("Database", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Database":
             raise ValueError("must be Database")
         return v
 
     class Attributes(SQL.Attributes):
         schema_count: Optional[int] = Field(None, description="", alias="schemaCount")
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        dbt_sources: Optional[list[DbtSource]] = Field(
-            None, description="", alias="dbtSources"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        sql_dbt_models: Optional[list[DbtModel]] = Field(
-            None, description="", alias="sqlDbtModels"
-        )  # relationship
-        sql_dbt_sources: Optional[list[DbtSource]] = Field(
-            None, description="", alias="sqlDBTSources"
-        )  # relationship
-        dbt_models: Optional[list[DbtModel]] = Field(
-            None, description="", alias="dbtModels"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         schemas: Optional[list[Schema]] = Field(
             None, description="", alias="schemas"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
         @classmethod
         # @validate_arguments()
         def create(
             cls, name: str, connection_qualified_name: str
         ) -> Database.Attributes:
             if not name:
@@ -13374,15 +12010,15 @@
                 name=name,
                 connection_qualified_name=connection_qualified_name,
                 qualified_name=f"{connection_qualified_name}/{name}",
                 connector_name=connector_type.value,
             )
 
     attributes: "Database.Attributes" = Field(
-        None,
+        default_factory=lambda: Database.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
     @classmethod
     # @validate_arguments()
     def create(cls, *, name: str, connection_qualified_name: str) -> Database:
@@ -13413,91 +12049,53 @@
     def __setattr__(self, name, value):
         if name in Procedure._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "definition",
-        "terms",
+        "atlan_schema",
     ]
 
     @property
     def definition(self) -> str:
         return self.attributes.definition
 
     @definition.setter
     def definition(self, definition: str):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.definition = definition
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+    def atlan_schema(self) -> Optional[Schema]:
+        return self.attributes.atlan_schema
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @atlan_schema.setter
+    def atlan_schema(self, atlan_schema: Optional[Schema]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.atlan_schema = atlan_schema
 
     type_name: str = Field("Procedure", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Procedure":
             raise ValueError("must be Procedure")
         return v
 
     class Attributes(SQL.Attributes):
         definition: str = Field(None, description="", alias="definition")
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        dbt_sources: Optional[list[DbtSource]] = Field(
-            None, description="", alias="dbtSources"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        sql_dbt_models: Optional[list[DbtModel]] = Field(
-            None, description="", alias="sqlDbtModels"
-        )  # relationship
-        sql_dbt_sources: Optional[list[DbtSource]] = Field(
-            None, description="", alias="sqlDBTSources"
-        )  # relationship
-        dbt_models: Optional[list[DbtModel]] = Field(
-            None, description="", alias="dbtModels"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         atlan_schema: Optional[Schema] = Field(
             None, description="", alias="atlanSchema"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "Procedure.Attributes" = Field(
-        None,
+        default_factory=lambda: Procedure.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class View(SQL):
     """Description"""
@@ -13512,15 +12110,17 @@
         "row_count",
         "size_bytes",
         "is_query_preview",
         "query_preview_config",
         "alias",
         "is_temporary",
         "definition",
-        "terms",
+        "columns",
+        "queries",
+        "atlan_schema",
     ]
 
     @property
     def column_count(self) -> Optional[int]:
         return self.attributes.column_count
 
     @column_count.setter
@@ -13596,24 +12196,42 @@
     @definition.setter
     def definition(self, definition: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.definition = definition
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def columns(self) -> Optional[list[Column]]:
+        return self.attributes.columns
+
+    @columns.setter
+    def columns(self, columns: Optional[list[Column]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.columns = columns
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def queries(self) -> Optional[list[Query]]:
+        return self.attributes.queries
+
+    @queries.setter
+    def queries(self, queries: Optional[list[Query]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.queries = queries
+
+    @property
+    def atlan_schema(self) -> Optional[Schema]:
+        return self.attributes.atlan_schema
+
+    @atlan_schema.setter
+    def atlan_schema(self, atlan_schema: Optional[Schema]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.atlan_schema = atlan_schema
 
     type_name: str = Field("View", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "View":
             raise ValueError("must be View")
@@ -13628,59 +12246,23 @@
         )
         query_preview_config: Optional[dict[str, str]] = Field(
             None, description="", alias="queryPreviewConfig"
         )
         alias: Optional[str] = Field(None, description="", alias="alias")
         is_temporary: Optional[bool] = Field(None, description="", alias="isTemporary")
         definition: Optional[str] = Field(None, description="", alias="definition")
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        dbt_sources: Optional[list[DbtSource]] = Field(
-            None, description="", alias="dbtSources"
-        )  # relationship
         columns: Optional[list[Column]] = Field(
             None, description="", alias="columns"
         )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
         queries: Optional[list[Query]] = Field(
             None, description="", alias="queries"
         )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        sql_dbt_models: Optional[list[DbtModel]] = Field(
-            None, description="", alias="sqlDbtModels"
-        )  # relationship
-        sql_dbt_sources: Optional[list[DbtSource]] = Field(
-            None, description="", alias="sqlDBTSources"
-        )  # relationship
-        dbt_models: Optional[list[DbtModel]] = Field(
-            None, description="", alias="dbtModels"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         atlan_schema: Optional[Schema] = Field(
             None, description="", alias="atlanSchema"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
         @classmethod
         # @validate_arguments()
         def create(cls, *, name: str, schema_qualified_name: str) -> View.Attributes:
             if not name:
                 raise ValueError("name cannot be blank")
             validate_required_fields(["schema_qualified_name"], [schema_qualified_name])
@@ -13700,15 +12282,15 @@
                 schema_qualified_name=schema_qualified_name,
                 schema_name=fields[4],
                 connector_name=connector_type.value,
                 atlan_schema=Schema.ref_by_qualified_name(schema_qualified_name),
             )
 
     attributes: "View.Attributes" = Field(
-        None,
+        default_factory=lambda: View.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
     @classmethod
     # @validate_arguments()
     def create(cls, *, name: str, schema_qualified_name: str) -> View:
@@ -13738,15 +12320,16 @@
         "row_count",
         "size_bytes",
         "is_query_preview",
         "query_preview_config",
         "alias",
         "is_temporary",
         "definition",
-        "terms",
+        "columns",
+        "atlan_schema",
     ]
 
     @property
     def refresh_mode(self) -> Optional[str]:
         return self.attributes.refresh_mode
 
     @refresh_mode.setter
@@ -13862,24 +12445,32 @@
     @definition.setter
     def definition(self, definition: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.definition = definition
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def columns(self) -> Optional[list[Column]]:
+        return self.attributes.columns
+
+    @columns.setter
+    def columns(self, columns: Optional[list[Column]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.columns = columns
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def atlan_schema(self) -> Optional[Schema]:
+        return self.attributes.atlan_schema
+
+    @atlan_schema.setter
+    def atlan_schema(self, atlan_schema: Optional[Schema]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.atlan_schema = atlan_schema
 
     type_name: str = Field("MaterialisedView", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "MaterialisedView":
             raise ValueError("must be MaterialisedView")
@@ -13902,59 +12493,23 @@
         )
         query_preview_config: Optional[dict[str, str]] = Field(
             None, description="", alias="queryPreviewConfig"
         )
         alias: Optional[str] = Field(None, description="", alias="alias")
         is_temporary: Optional[bool] = Field(None, description="", alias="isTemporary")
         definition: Optional[str] = Field(None, description="", alias="definition")
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        dbt_sources: Optional[list[DbtSource]] = Field(
-            None, description="", alias="dbtSources"
-        )  # relationship
         columns: Optional[list[Column]] = Field(
             None, description="", alias="columns"
         )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        sql_dbt_models: Optional[list[DbtModel]] = Field(
-            None, description="", alias="sqlDbtModels"
-        )  # relationship
-        sql_dbt_sources: Optional[list[DbtSource]] = Field(
-            None, description="", alias="sqlDBTSources"
-        )  # relationship
-        dbt_models: Optional[list[DbtModel]] = Field(
-            None, description="", alias="dbtModels"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         atlan_schema: Optional[Schema] = Field(
             None, description="", alias="atlanSchema"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "MaterialisedView.Attributes" = Field(
-        None,
+        default_factory=lambda: MaterialisedView.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class GCSObject(GCS):
     """Description"""
@@ -13976,15 +12531,15 @@
         "gcs_object_m_d5_hash",
         "gcs_object_data_last_modified_time",
         "gcs_object_content_type",
         "gcs_object_content_encoding",
         "gcs_object_content_disposition",
         "gcs_object_content_language",
         "gcs_object_retention_expiration_date",
-        "terms",
+        "gcs_bucket",
     ]
 
     @property
     def gcs_bucket_name(self) -> Optional[str]:
         return self.attributes.gcs_bucket_name
 
     @gcs_bucket_name.setter
@@ -14140,24 +12695,22 @@
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.gcs_object_retention_expiration_date = (
             gcs_object_retention_expiration_date
         )
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+    def gcs_bucket(self) -> Optional[GCSBucket]:
+        return self.attributes.gcs_bucket
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @gcs_bucket.setter
+    def gcs_bucket(self, gcs_bucket: Optional[GCSBucket]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.gcs_bucket = gcs_bucket
 
     type_name: str = Field("GCSObject", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "GCSObject":
             raise ValueError("must be GCSObject")
@@ -14205,44 +12758,20 @@
         )
         gcs_object_content_language: Optional[str] = Field(
             None, description="", alias="gcsObjectContentLanguage"
         )
         gcs_object_retention_expiration_date: Optional[datetime] = Field(
             None, description="", alias="gcsObjectRetentionExpirationDate"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         gcs_bucket: Optional[GCSBucket] = Field(
             None, description="", alias="gcsBucket"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "GCSObject.Attributes" = Field(
-        None,
+        default_factory=lambda: GCSObject.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class GCSBucket(GCS):
     """Description"""
@@ -14256,15 +12785,15 @@
         "gcs_object_count",
         "gcs_bucket_versioning_enabled",
         "gcs_bucket_retention_locked",
         "gcs_bucket_retention_period",
         "gcs_bucket_retention_effective_time",
         "gcs_bucket_lifecycle_rules",
         "gcs_bucket_retention_policy",
-        "terms",
+        "gcs_objects",
     ]
 
     @property
     def gcs_object_count(self) -> Optional[int]:
         return self.attributes.gcs_object_count
 
     @gcs_object_count.setter
@@ -14336,24 +12865,22 @@
     @gcs_bucket_retention_policy.setter
     def gcs_bucket_retention_policy(self, gcs_bucket_retention_policy: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.gcs_bucket_retention_policy = gcs_bucket_retention_policy
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+    def gcs_objects(self) -> Optional[list[GCSObject]]:
+        return self.attributes.gcs_objects
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @gcs_objects.setter
+    def gcs_objects(self, gcs_objects: Optional[list[GCSObject]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.gcs_objects = gcs_objects
 
     type_name: str = Field("GCSBucket", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "GCSBucket":
             raise ValueError("must be GCSBucket")
@@ -14377,44 +12904,20 @@
         )
         gcs_bucket_lifecycle_rules: Optional[str] = Field(
             None, description="", alias="gcsBucketLifecycleRules"
         )
         gcs_bucket_retention_policy: Optional[str] = Field(
             None, description="", alias="gcsBucketRetentionPolicy"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
         gcs_objects: Optional[list[GCSObject]] = Field(
             None, description="", alias="gcsObjects"
         )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "GCSBucket.Attributes" = Field(
-        None,
+        default_factory=lambda: GCSBucket.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class ADLSAccount(ADLS):
     """Description"""
@@ -14431,15 +12934,15 @@
         "adls_account_subscription",
         "adls_account_performance",
         "adls_account_replication",
         "adls_account_kind",
         "adls_primary_disk_state",
         "adls_account_provision_state",
         "adls_account_access_tier",
-        "terms",
+        "adls_containers",
     ]
 
     @property
     def adls_e_tag(self) -> Optional[str]:
         return self.attributes.adls_e_tag
 
     @adls_e_tag.setter
@@ -14545,24 +13048,22 @@
         self, adls_account_access_tier: Optional[ADLSAccessTier]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.adls_account_access_tier = adls_account_access_tier
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+    def adls_containers(self) -> Optional[list[ADLSContainer]]:
+        return self.attributes.adls_containers
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @adls_containers.setter
+    def adls_containers(self, adls_containers: Optional[list[ADLSContainer]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.adls_containers = adls_containers
 
     type_name: str = Field("ADLSAccount", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "ADLSAccount":
             raise ValueError("must be ADLSAccount")
@@ -14593,44 +13094,20 @@
         )
         adls_account_provision_state: Optional[ADLSProvisionState] = Field(
             None, description="", alias="adlsAccountProvisionState"
         )
         adls_account_access_tier: Optional[ADLSAccessTier] = Field(
             None, description="", alias="adlsAccountAccessTier"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
         adls_containers: Optional[list[ADLSContainer]] = Field(
             None, description="", alias="adlsContainers"
         )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "ADLSAccount.Attributes" = Field(
-        None,
+        default_factory=lambda: ADLSAccount.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class ADLSContainer(ADLS):
     """Description"""
@@ -14643,15 +13120,16 @@
     _convience_properties: ClassVar[list[str]] = [
         "adls_container_url",
         "adls_container_lease_state",
         "adls_container_lease_status",
         "adls_container_encryption_scope",
         "adls_container_version_level_immutability_support",
         "adls_object_count",
-        "terms",
+        "adls_objects",
+        "adls_account",
     ]
 
     @property
     def adls_container_url(self) -> Optional[str]:
         return self.attributes.adls_container_url
 
     @adls_container_url.setter
@@ -14719,24 +13197,32 @@
     @adls_object_count.setter
     def adls_object_count(self, adls_object_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.adls_object_count = adls_object_count
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def adls_objects(self) -> Optional[list[ADLSObject]]:
+        return self.attributes.adls_objects
+
+    @adls_objects.setter
+    def adls_objects(self, adls_objects: Optional[list[ADLSObject]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.adls_objects = adls_objects
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def adls_account(self) -> Optional[ADLSAccount]:
+        return self.attributes.adls_account
+
+    @adls_account.setter
+    def adls_account(self, adls_account: Optional[ADLSAccount]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.adls_account = adls_account
 
     type_name: str = Field("ADLSContainer", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "ADLSContainer":
             raise ValueError("must be ADLSContainer")
@@ -14760,44 +13246,20 @@
         )
         adls_object_count: Optional[int] = Field(
             None, description="", alias="adlsObjectCount"
         )
         adls_objects: Optional[list[ADLSObject]] = Field(
             None, description="", alias="adlsObjects"
         )  # relationship
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         adls_account: Optional[ADLSAccount] = Field(
             None, description="", alias="adlsAccount"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "ADLSContainer.Attributes" = Field(
-        None,
+        default_factory=lambda: ADLSContainer.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class ADLSObject(ADLS):
     """Description"""
@@ -14821,15 +13283,15 @@
         "adls_object_content_type",
         "adls_object_content_m_d5_hash",
         "adls_object_content_language",
         "adls_object_lease_status",
         "adls_object_lease_state",
         "adls_object_metadata",
         "adls_container_qualified_name",
-        "terms",
+        "adls_container",
     ]
 
     @property
     def adls_object_url(self) -> Optional[str]:
         return self.attributes.adls_object_url
 
     @adls_object_url.setter
@@ -15017,24 +13479,22 @@
         self, adls_container_qualified_name: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.adls_container_qualified_name = adls_container_qualified_name
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+    def adls_container(self) -> Optional[ADLSContainer]:
+        return self.attributes.adls_container
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @adls_container.setter
+    def adls_container(self, adls_container: Optional[ADLSContainer]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.adls_container = adls_container
 
     type_name: str = Field("ADLSObject", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "ADLSObject":
             raise ValueError("must be ADLSObject")
@@ -15088,44 +13548,20 @@
         )
         adls_object_metadata: Optional[dict[str, str]] = Field(
             None, description="", alias="adlsObjectMetadata"
         )
         adls_container_qualified_name: Optional[str] = Field(
             None, description="", alias="adlsContainerQualifiedName"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
         adls_container: Optional[ADLSContainer] = Field(
             None, description="", alias="adlsContainer"
         )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "ADLSObject.Attributes" = Field(
-        None,
+        default_factory=lambda: ADLSObject.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class S3Bucket(S3):
     """Description"""
@@ -15134,15 +13570,15 @@
         if name in S3Bucket._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "s3_object_count",
         "s3_bucket_versioning_enabled",
-        "terms",
+        "objects",
     ]
 
     @property
     def s3_object_count(self) -> Optional[int]:
         return self.attributes.s3_object_count
 
     @s3_object_count.setter
@@ -15160,24 +13596,22 @@
         self, s3_bucket_versioning_enabled: Optional[bool]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.s3_bucket_versioning_enabled = s3_bucket_versioning_enabled
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+    def objects(self) -> Optional[list[S3Object]]:
+        return self.attributes.objects
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @objects.setter
+    def objects(self, objects: Optional[list[S3Object]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.objects = objects
 
     type_name: str = Field("S3Bucket", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "S3Bucket":
             raise ValueError("must be S3Bucket")
@@ -15186,41 +13620,17 @@
     class Attributes(S3.Attributes):
         s3_object_count: Optional[int] = Field(
             None, description="", alias="s3ObjectCount"
         )
         s3_bucket_versioning_enabled: Optional[bool] = Field(
             None, description="", alias="s3BucketVersioningEnabled"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         objects: Optional[list[S3Object]] = Field(
             None, description="", alias="objects"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
         @classmethod
         # @validate_arguments()
         def create(
             cls, *, name: str, connection_qualified_name: str, aws_arn: str
         ) -> S3Bucket.Attributes:
             validate_required_fields(
@@ -15243,15 +13653,15 @@
                 name=name,
                 connection_qualified_name=connection_qualified_name,
                 qualified_name=f"{connection_qualified_name}/{aws_arn}",
                 connector_name=connector_type.value,
             )
 
     attributes: "S3Bucket.Attributes" = Field(
-        None,
+        default_factory=lambda: S3Bucket.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
     @classmethod
     # @validate_arguments()
     def create(
@@ -15283,15 +13693,15 @@
         "s3_bucket_qualified_name",
         "s3_object_size",
         "s3_object_storage_class",
         "s3_object_key",
         "s3_object_content_type",
         "s3_object_content_disposition",
         "s3_object_version_id",
-        "terms",
+        "bucket",
     ]
 
     @property
     def s3_object_last_modified_time(self) -> Optional[datetime]:
         return self.attributes.s3_object_last_modified_time
 
     @s3_object_last_modified_time.setter
@@ -15381,24 +13791,22 @@
     @s3_object_version_id.setter
     def s3_object_version_id(self, s3_object_version_id: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.s3_object_version_id = s3_object_version_id
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+    def bucket(self) -> Optional[S3Bucket]:
+        return self.attributes.bucket
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @bucket.setter
+    def bucket(self, bucket: Optional[S3Bucket]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.bucket = bucket
 
     type_name: str = Field("S3Object", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "S3Object":
             raise ValueError("must be S3Object")
@@ -15429,38 +13837,14 @@
         )
         s3_object_version_id: Optional[str] = Field(
             None, description="", alias="s3ObjectVersionId"
         )
         bucket: Optional[S3Bucket] = Field(
             None, description="", alias="bucket"
         )  # relationship
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
         @classmethod
         # @validate_arguments()
         def create(
             cls,
             *,
             name: str,
@@ -15489,15 +13873,15 @@
                 connection_qualified_name=connection_qualified_name,
                 qualified_name=f"{connection_qualified_name}/{aws_arn}",
                 connector_name=connector_type.value,
                 s3_bucket_qualified_name=s3_bucket_qualified_name,
             )
 
     attributes: "S3Object.Attributes" = Field(
-        None,
+        default_factory=lambda: S3Object.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
     @classmethod
     # @validate_arguments()
     def create(
@@ -15534,15 +13918,15 @@
         "kafka_topic_compression_type",
         "kafka_topic_replication_factor",
         "kafka_topic_segment_bytes",
         "kafka_topic_partitions_count",
         "kafka_topic_size_in_bytes",
         "kafka_topic_record_count",
         "kafka_topic_cleanup_policy",
-        "terms",
+        "kafka_consumer_groups",
     ]
 
     @property
     def kafka_topic_is_internal(self) -> Optional[bool]:
         return self.attributes.kafka_topic_is_internal
 
     @kafka_topic_is_internal.setter
@@ -15624,24 +14008,24 @@
         self, kafka_topic_cleanup_policy: Optional[PowerbiEndorsement]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.kafka_topic_cleanup_policy = kafka_topic_cleanup_policy
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+    def kafka_consumer_groups(self) -> Optional[list[KafkaConsumerGroup]]:
+        return self.attributes.kafka_consumer_groups
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @kafka_consumer_groups.setter
+    def kafka_consumer_groups(
+        self, kafka_consumer_groups: Optional[list[KafkaConsumerGroup]]
+    ):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.kafka_consumer_groups = kafka_consumer_groups
 
     type_name: str = Field("KafkaTopic", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "KafkaTopic":
             raise ValueError("must be KafkaTopic")
@@ -15668,44 +14052,20 @@
         )
         kafka_topic_record_count: Optional[int] = Field(
             None, description="", alias="kafkaTopicRecordCount"
         )
         kafka_topic_cleanup_policy: Optional[PowerbiEndorsement] = Field(
             None, description="", alias="kafkaTopicCleanupPolicy"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         kafka_consumer_groups: Optional[list[KafkaConsumerGroup]] = Field(
             None, description="", alias="kafkaConsumerGroups"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "KafkaTopic.Attributes" = Field(
-        None,
+        default_factory=lambda: KafkaTopic.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class KafkaConsumerGroup(Kafka):
     """Description"""
@@ -15716,15 +14076,15 @@
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "kafka_consumer_group_topic_consumption_properties",
         "kafka_consumer_group_member_count",
         "kafka_topic_names",
         "kafka_topic_qualified_names",
-        "terms",
+        "kafka_topics",
     ]
 
     @property
     def kafka_consumer_group_topic_consumption_properties(
         self,
     ) -> Optional[list[KafkaTopicConsumption]]:
         return self.attributes.kafka_consumer_group_topic_consumption_properties
@@ -15775,24 +14135,22 @@
         self, kafka_topic_qualified_names: Optional[set[str]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.kafka_topic_qualified_names = kafka_topic_qualified_names
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+    def kafka_topics(self) -> Optional[list[KafkaTopic]]:
+        return self.attributes.kafka_topics
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @kafka_topics.setter
+    def kafka_topics(self, kafka_topics: Optional[list[KafkaTopic]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.kafka_topics = kafka_topics
 
     type_name: str = Field("KafkaConsumerGroup", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "KafkaConsumerGroup":
             raise ValueError("must be KafkaConsumerGroup")
@@ -15809,44 +14167,20 @@
         )
         kafka_topic_names: Optional[set[str]] = Field(
             None, description="", alias="kafkaTopicNames"
         )
         kafka_topic_qualified_names: Optional[set[str]] = Field(
             None, description="", alias="kafkaTopicQualifiedNames"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
         kafka_topics: Optional[list[KafkaTopic]] = Field(
             None, description="", alias="kafkaTopics"
         )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "KafkaConsumerGroup.Attributes" = Field(
-        None,
+        default_factory=lambda: KafkaConsumerGroup.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class MCIncident(MonteCarlo):
     """Description"""
@@ -15859,15 +14193,16 @@
     _convience_properties: ClassVar[list[str]] = [
         "mc_incident_id",
         "mc_incident_type",
         "mc_incident_sub_types",
         "mc_incident_severity",
         "mc_incident_state",
         "mc_incident_warehouse",
-        "terms",
+        "mc_incident_assets",
+        "mc_monitor",
     ]
 
     @property
     def mc_incident_id(self) -> Optional[str]:
         return self.attributes.mc_incident_id
 
     @mc_incident_id.setter
@@ -15923,24 +14258,32 @@
     @mc_incident_warehouse.setter
     def mc_incident_warehouse(self, mc_incident_warehouse: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mc_incident_warehouse = mc_incident_warehouse
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def mc_incident_assets(self) -> Optional[list[Asset]]:
+        return self.attributes.mc_incident_assets
+
+    @mc_incident_assets.setter
+    def mc_incident_assets(self, mc_incident_assets: Optional[list[Asset]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.mc_incident_assets = mc_incident_assets
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def mc_monitor(self) -> Optional[MCMonitor]:
+        return self.attributes.mc_monitor
+
+    @mc_monitor.setter
+    def mc_monitor(self, mc_monitor: Optional[MCMonitor]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.mc_monitor = mc_monitor
 
     type_name: str = Field("MCIncident", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "MCIncident":
             raise ValueError("must be MCIncident")
@@ -15961,47 +14304,23 @@
         )
         mc_incident_state: Optional[str] = Field(
             None, description="", alias="mcIncidentState"
         )
         mc_incident_warehouse: Optional[str] = Field(
             None, description="", alias="mcIncidentWarehouse"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
         mc_incident_assets: Optional[list[Asset]] = Field(
             None, description="", alias="mcIncidentAssets"
         )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         mc_monitor: Optional[MCMonitor] = Field(
             None, description="", alias="mcMonitor"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "MCIncident.Attributes" = Field(
-        None,
+        default_factory=lambda: MCIncident.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class MCMonitor(MonteCarlo):
     """Description"""
@@ -16025,15 +14344,15 @@
         "mc_monitor_alert_condition",
         "mc_monitor_rule_next_execution_time",
         "mc_monitor_rule_previous_execution_time",
         "mc_monitor_rule_comparisons",
         "mc_monitor_rule_is_snoozed",
         "mc_monitor_breach_rate",
         "mc_monitor_incident_count",
-        "terms",
+        "mc_monitor_assets",
     ]
 
     @property
     def mc_monitor_id(self) -> Optional[str]:
         return self.attributes.mc_monitor_id
 
     @mc_monitor_id.setter
@@ -16217,24 +14536,22 @@
     @mc_monitor_incident_count.setter
     def mc_monitor_incident_count(self, mc_monitor_incident_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mc_monitor_incident_count = mc_monitor_incident_count
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+    def mc_monitor_assets(self) -> Optional[list[Asset]]:
+        return self.attributes.mc_monitor_assets
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @mc_monitor_assets.setter
+    def mc_monitor_assets(self, mc_monitor_assets: Optional[list[Asset]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.mc_monitor_assets = mc_monitor_assets
 
     type_name: str = Field("MCMonitor", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "MCMonitor":
             raise ValueError("must be MCMonitor")
@@ -16286,44 +14603,20 @@
         )
         mc_monitor_breach_rate: Optional[float] = Field(
             None, description="", alias="mcMonitorBreachRate"
         )
         mc_monitor_incident_count: Optional[int] = Field(
             None, description="", alias="mcMonitorIncidentCount"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
         mc_monitor_assets: Optional[list[Asset]] = Field(
             None, description="", alias="mcMonitorAssets"
         )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "MCMonitor.Attributes" = Field(
-        None,
+        default_factory=lambda: MCMonitor.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class MetabaseQuestion(Metabase):
     """Description"""
@@ -16333,15 +14626,16 @@
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "metabase_dashboard_count",
         "metabase_query_type",
         "metabase_query",
-        "terms",
+        "metabase_dashboards",
+        "metabase_collection",
     ]
 
     @property
     def metabase_dashboard_count(self) -> Optional[int]:
         return self.attributes.metabase_dashboard_count
 
     @metabase_dashboard_count.setter
@@ -16367,24 +14661,34 @@
     @metabase_query.setter
     def metabase_query(self, metabase_query: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.metabase_query = metabase_query
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def metabase_dashboards(self) -> Optional[list[MetabaseDashboard]]:
+        return self.attributes.metabase_dashboards
+
+    @metabase_dashboards.setter
+    def metabase_dashboards(
+        self, metabase_dashboards: Optional[list[MetabaseDashboard]]
+    ):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.metabase_dashboards = metabase_dashboards
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def metabase_collection(self) -> Optional[MetabaseCollection]:
+        return self.attributes.metabase_collection
+
+    @metabase_collection.setter
+    def metabase_collection(self, metabase_collection: Optional[MetabaseCollection]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.metabase_collection = metabase_collection
 
     type_name: str = Field("MetabaseQuestion", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "MetabaseQuestion":
             raise ValueError("must be MetabaseQuestion")
@@ -16396,47 +14700,23 @@
         )
         metabase_query_type: Optional[str] = Field(
             None, description="", alias="metabaseQueryType"
         )
         metabase_query: Optional[str] = Field(
             None, description="", alias="metabaseQuery"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         metabase_dashboards: Optional[list[MetabaseDashboard]] = Field(
             None, description="", alias="metabaseDashboards"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
         metabase_collection: Optional[MetabaseCollection] = Field(
             None, description="", alias="metabaseCollection"
         )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "MetabaseQuestion.Attributes" = Field(
-        None,
+        default_factory=lambda: MetabaseQuestion.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class MetabaseCollection(Metabase):
     """Description"""
@@ -16447,15 +14727,16 @@
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "metabase_slug",
         "metabase_color",
         "metabase_namespace",
         "metabase_is_personal_collection",
-        "terms",
+        "metabase_dashboards",
+        "metabase_questions",
     ]
 
     @property
     def metabase_slug(self) -> Optional[str]:
         return self.attributes.metabase_slug
 
     @metabase_slug.setter
@@ -16495,24 +14776,34 @@
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.metabase_is_personal_collection = (
             metabase_is_personal_collection
         )
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def metabase_dashboards(self) -> Optional[list[MetabaseDashboard]]:
+        return self.attributes.metabase_dashboards
+
+    @metabase_dashboards.setter
+    def metabase_dashboards(
+        self, metabase_dashboards: Optional[list[MetabaseDashboard]]
+    ):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.metabase_dashboards = metabase_dashboards
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def metabase_questions(self) -> Optional[list[MetabaseQuestion]]:
+        return self.attributes.metabase_questions
+
+    @metabase_questions.setter
+    def metabase_questions(self, metabase_questions: Optional[list[MetabaseQuestion]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.metabase_questions = metabase_questions
 
     type_name: str = Field("MetabaseCollection", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "MetabaseCollection":
             raise ValueError("must be MetabaseCollection")
@@ -16525,47 +14816,23 @@
         )
         metabase_namespace: Optional[str] = Field(
             None, description="", alias="metabaseNamespace"
         )
         metabase_is_personal_collection: Optional[bool] = Field(
             None, description="", alias="metabaseIsPersonalCollection"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         metabase_dashboards: Optional[list[MetabaseDashboard]] = Field(
             None, description="", alias="metabaseDashboards"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
         metabase_questions: Optional[list[MetabaseQuestion]] = Field(
             None, description="", alias="metabaseQuestions"
         )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "MetabaseCollection.Attributes" = Field(
-        None,
+        default_factory=lambda: MetabaseCollection.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class MetabaseDashboard(Metabase):
     """Description"""
@@ -16573,84 +14840,69 @@
     def __setattr__(self, name, value):
         if name in MetabaseDashboard._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "metabase_question_count",
-        "terms",
+        "metabase_questions",
+        "metabase_collection",
     ]
 
     @property
     def metabase_question_count(self) -> Optional[int]:
         return self.attributes.metabase_question_count
 
     @metabase_question_count.setter
     def metabase_question_count(self, metabase_question_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.metabase_question_count = metabase_question_count
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def metabase_questions(self) -> Optional[list[MetabaseQuestion]]:
+        return self.attributes.metabase_questions
+
+    @metabase_questions.setter
+    def metabase_questions(self, metabase_questions: Optional[list[MetabaseQuestion]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.metabase_questions = metabase_questions
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def metabase_collection(self) -> Optional[MetabaseCollection]:
+        return self.attributes.metabase_collection
+
+    @metabase_collection.setter
+    def metabase_collection(self, metabase_collection: Optional[MetabaseCollection]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.metabase_collection = metabase_collection
 
     type_name: str = Field("MetabaseDashboard", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "MetabaseDashboard":
             raise ValueError("must be MetabaseDashboard")
         return v
 
     class Attributes(Metabase.Attributes):
         metabase_question_count: Optional[int] = Field(
             None, description="", alias="metabaseQuestionCount"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
         metabase_questions: Optional[list[MetabaseQuestion]] = Field(
             None, description="", alias="metabaseQuestions"
         )  # relationship
         metabase_collection: Optional[MetabaseCollection] = Field(
             None, description="", alias="metabaseCollection"
         )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "MetabaseDashboard.Attributes" = Field(
-        None,
+        default_factory=lambda: MetabaseDashboard.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class QuickSightFolder(QuickSight):
     """Description"""
@@ -16659,15 +14911,17 @@
         if name in QuickSightFolder._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "quick_sight_folder_type",
         "quick_sight_folder_hierarchy",
-        "terms",
+        "quick_sight_dashboards",
+        "quick_sight_analyses",
+        "quick_sight_datasets",
     ]
 
     @property
     def quick_sight_folder_type(self) -> Optional[QuickSightFolderType]:
         return self.attributes.quick_sight_folder_type
 
     @quick_sight_folder_type.setter
@@ -16687,24 +14941,48 @@
         self, quick_sight_folder_hierarchy: Optional[list[dict[str, str]]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.quick_sight_folder_hierarchy = quick_sight_folder_hierarchy
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def quick_sight_dashboards(self) -> Optional[list[QuickSightDashboard]]:
+        return self.attributes.quick_sight_dashboards
+
+    @quick_sight_dashboards.setter
+    def quick_sight_dashboards(
+        self, quick_sight_dashboards: Optional[list[QuickSightDashboard]]
+    ):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.quick_sight_dashboards = quick_sight_dashboards
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def quick_sight_analyses(self) -> Optional[list[QuickSightAnalysis]]:
+        return self.attributes.quick_sight_analyses
+
+    @quick_sight_analyses.setter
+    def quick_sight_analyses(
+        self, quick_sight_analyses: Optional[list[QuickSightAnalysis]]
+    ):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.quick_sight_analyses = quick_sight_analyses
+
+    @property
+    def quick_sight_datasets(self) -> Optional[list[QuickSightDataset]]:
+        return self.attributes.quick_sight_datasets
+
+    @quick_sight_datasets.setter
+    def quick_sight_datasets(
+        self, quick_sight_datasets: Optional[list[QuickSightDataset]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.quick_sight_datasets = quick_sight_datasets
 
     type_name: str = Field("QuickSightFolder", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "QuickSightFolder":
             raise ValueError("must be QuickSightFolder")
@@ -16716,47 +14994,23 @@
         )
         quick_sight_folder_hierarchy: Optional[list[dict[str, str]]] = Field(
             None, description="", alias="quickSightFolderHierarchy"
         )
         quick_sight_dashboards: Optional[list[QuickSightDashboard]] = Field(
             None, description="", alias="quickSightDashboards"
         )  # relationship
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         quick_sight_analyses: Optional[list[QuickSightAnalysis]] = Field(
             None, description="", alias="quickSightAnalyses"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
         quick_sight_datasets: Optional[list[QuickSightDataset]] = Field(
             None, description="", alias="quickSightDatasets"
         )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "QuickSightFolder.Attributes" = Field(
-        None,
+        default_factory=lambda: QuickSightFolder.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class QuickSightDashboardVisual(QuickSight):
     """Description"""
@@ -16764,15 +15018,15 @@
     def __setattr__(self, name, value):
         if name in QuickSightDashboardVisual._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "quick_sight_dashboard_qualified_name",
-        "terms",
+        "quick_sight_dashboard",
     ]
 
     @property
     def quick_sight_dashboard_qualified_name(self) -> Optional[str]:
         return self.attributes.quick_sight_dashboard_qualified_name
 
     @quick_sight_dashboard_qualified_name.setter
@@ -16782,67 +15036,43 @@
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.quick_sight_dashboard_qualified_name = (
             quick_sight_dashboard_qualified_name
         )
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+    def quick_sight_dashboard(self) -> Optional[QuickSightDashboard]:
+        return self.attributes.quick_sight_dashboard
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @quick_sight_dashboard.setter
+    def quick_sight_dashboard(
+        self, quick_sight_dashboard: Optional[QuickSightDashboard]
+    ):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.quick_sight_dashboard = quick_sight_dashboard
 
     type_name: str = Field("QuickSightDashboardVisual", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "QuickSightDashboardVisual":
             raise ValueError("must be QuickSightDashboardVisual")
         return v
 
     class Attributes(QuickSight.Attributes):
         quick_sight_dashboard_qualified_name: Optional[str] = Field(
             None, description="", alias="quickSightDashboardQualifiedName"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
         quick_sight_dashboard: Optional[QuickSightDashboard] = Field(
             None, description="", alias="quickSightDashboard"
         )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "QuickSightDashboardVisual.Attributes" = Field(
-        None,
+        default_factory=lambda: QuickSightDashboardVisual.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class QuickSightAnalysisVisual(QuickSight):
     """Description"""
@@ -16850,15 +15080,15 @@
     def __setattr__(self, name, value):
         if name in QuickSightAnalysisVisual._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "quick_sight_analysis_qualified_name",
-        "terms",
+        "quick_sight_analysis",
     ]
 
     @property
     def quick_sight_analysis_qualified_name(self) -> Optional[str]:
         return self.attributes.quick_sight_analysis_qualified_name
 
     @quick_sight_analysis_qualified_name.setter
@@ -16868,67 +15098,41 @@
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.quick_sight_analysis_qualified_name = (
             quick_sight_analysis_qualified_name
         )
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+    def quick_sight_analysis(self) -> Optional[QuickSightAnalysis]:
+        return self.attributes.quick_sight_analysis
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @quick_sight_analysis.setter
+    def quick_sight_analysis(self, quick_sight_analysis: Optional[QuickSightAnalysis]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.quick_sight_analysis = quick_sight_analysis
 
     type_name: str = Field("QuickSightAnalysisVisual", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "QuickSightAnalysisVisual":
             raise ValueError("must be QuickSightAnalysisVisual")
         return v
 
     class Attributes(QuickSight.Attributes):
         quick_sight_analysis_qualified_name: Optional[str] = Field(
             None, description="", alias="quickSightAnalysisQualifiedName"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
         quick_sight_analysis: Optional[QuickSightAnalysis] = Field(
             None, description="", alias="quickSightAnalysis"
         )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "QuickSightAnalysisVisual.Attributes" = Field(
-        None,
+        default_factory=lambda: QuickSightAnalysisVisual.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class QuickSightDatasetField(QuickSight):
     """Description"""
@@ -16937,15 +15141,15 @@
         if name in QuickSightDatasetField._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "quick_sight_dataset_field_type",
         "quick_sight_dataset_qualified_name",
-        "terms",
+        "quick_sight_dataset",
     ]
 
     @property
     def quick_sight_dataset_field_type(self) -> Optional[QuickSightDatasetFieldType]:
         return self.attributes.quick_sight_dataset_field_type
 
     @quick_sight_dataset_field_type.setter
@@ -16967,24 +15171,22 @@
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.quick_sight_dataset_qualified_name = (
             quick_sight_dataset_qualified_name
         )
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+    def quick_sight_dataset(self) -> Optional[QuickSightDataset]:
+        return self.attributes.quick_sight_dataset
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @quick_sight_dataset.setter
+    def quick_sight_dataset(self, quick_sight_dataset: Optional[QuickSightDataset]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.quick_sight_dataset = quick_sight_dataset
 
     type_name: str = Field("QuickSightDatasetField", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "QuickSightDatasetField":
             raise ValueError("must be QuickSightDatasetField")
@@ -16993,44 +15195,20 @@
     class Attributes(QuickSight.Attributes):
         quick_sight_dataset_field_type: Optional[QuickSightDatasetFieldType] = Field(
             None, description="", alias="quickSightDatasetFieldType"
         )
         quick_sight_dataset_qualified_name: Optional[str] = Field(
             None, description="", alias="quickSightDatasetQualifiedName"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
         quick_sight_dataset: Optional[QuickSightDataset] = Field(
             None, description="", alias="quickSightDataset"
         )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "QuickSightDatasetField.Attributes" = Field(
-        None,
+        default_factory=lambda: QuickSightDatasetField.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class QuickSightAnalysis(QuickSight):
     """Description"""
@@ -17041,15 +15219,16 @@
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "quick_sight_analysis_status",
         "quick_sight_analysis_calculated_fields",
         "quick_sight_analysis_parameter_declarations",
         "quick_sight_analysis_filter_groups",
-        "terms",
+        "quick_sight_analysis_visuals",
+        "quick_sight_analysis_folders",
     ]
 
     @property
     def quick_sight_analysis_status(self) -> Optional[QuickSightAnalysisStatus]:
         return self.attributes.quick_sight_analysis_status
 
     @quick_sight_analysis_status.setter
@@ -17099,24 +15278,36 @@
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.quick_sight_analysis_filter_groups = (
             quick_sight_analysis_filter_groups
         )
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def quick_sight_analysis_visuals(self) -> Optional[list[QuickSightAnalysisVisual]]:
+        return self.attributes.quick_sight_analysis_visuals
+
+    @quick_sight_analysis_visuals.setter
+    def quick_sight_analysis_visuals(
+        self, quick_sight_analysis_visuals: Optional[list[QuickSightAnalysisVisual]]
+    ):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.quick_sight_analysis_visuals = quick_sight_analysis_visuals
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def quick_sight_analysis_folders(self) -> Optional[list[QuickSightFolder]]:
+        return self.attributes.quick_sight_analysis_folders
+
+    @quick_sight_analysis_folders.setter
+    def quick_sight_analysis_folders(
+        self, quick_sight_analysis_folders: Optional[list[QuickSightFolder]]
+    ):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.quick_sight_analysis_folders = quick_sight_analysis_folders
 
     type_name: str = Field("QuickSightAnalysis", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "QuickSightAnalysis":
             raise ValueError("must be QuickSightAnalysis")
@@ -17131,47 +15322,23 @@
         )
         quick_sight_analysis_parameter_declarations: Optional[set[str]] = Field(
             None, description="", alias="quickSightAnalysisParameterDeclarations"
         )
         quick_sight_analysis_filter_groups: Optional[set[str]] = Field(
             None, description="", alias="quickSightAnalysisFilterGroups"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
         quick_sight_analysis_visuals: Optional[list[QuickSightAnalysisVisual]] = Field(
             None, description="", alias="quickSightAnalysisVisuals"
         )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
         quick_sight_analysis_folders: Optional[list[QuickSightFolder]] = Field(
             None, description="", alias="quickSightAnalysisFolders"
         )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "QuickSightAnalysis.Attributes" = Field(
-        None,
+        default_factory=lambda: QuickSightAnalysis.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class QuickSightDashboard(QuickSight):
     """Description"""
@@ -17180,15 +15347,16 @@
         if name in QuickSightDashboard._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "quick_sight_dashboard_published_version_number",
         "quick_sight_dashboard_last_published_time",
-        "terms",
+        "quick_sight_dashboard_folders",
+        "quick_sight_dashboard_visuals",
     ]
 
     @property
     def quick_sight_dashboard_published_version_number(self) -> Optional[int]:
         return self.attributes.quick_sight_dashboard_published_version_number
 
     @quick_sight_dashboard_published_version_number.setter
@@ -17212,24 +15380,38 @@
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.quick_sight_dashboard_last_published_time = (
             quick_sight_dashboard_last_published_time
         )
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def quick_sight_dashboard_folders(self) -> Optional[list[QuickSightFolder]]:
+        return self.attributes.quick_sight_dashboard_folders
+
+    @quick_sight_dashboard_folders.setter
+    def quick_sight_dashboard_folders(
+        self, quick_sight_dashboard_folders: Optional[list[QuickSightFolder]]
+    ):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.quick_sight_dashboard_folders = quick_sight_dashboard_folders
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def quick_sight_dashboard_visuals(
+        self,
+    ) -> Optional[list[QuickSightDashboardVisual]]:
+        return self.attributes.quick_sight_dashboard_visuals
+
+    @quick_sight_dashboard_visuals.setter
+    def quick_sight_dashboard_visuals(
+        self, quick_sight_dashboard_visuals: Optional[list[QuickSightDashboardVisual]]
+    ):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.quick_sight_dashboard_visuals = quick_sight_dashboard_visuals
 
     type_name: str = Field("QuickSightDashboard", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "QuickSightDashboard":
             raise ValueError("must be QuickSightDashboard")
@@ -17238,49 +15420,25 @@
     class Attributes(QuickSight.Attributes):
         quick_sight_dashboard_published_version_number: Optional[int] = Field(
             None, description="", alias="quickSightDashboardPublishedVersionNumber"
         )
         quick_sight_dashboard_last_published_time: Optional[datetime] = Field(
             None, description="", alias="quickSightDashboardLastPublishedTime"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         quick_sight_dashboard_folders: Optional[list[QuickSightFolder]] = Field(
             None, description="", alias="quickSightDashboardFolders"
         )  # relationship
         quick_sight_dashboard_visuals: Optional[
             list[QuickSightDashboardVisual]
         ] = Field(
             None, description="", alias="quickSightDashboardVisuals"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "QuickSightDashboard.Attributes" = Field(
-        None,
+        default_factory=lambda: QuickSightDashboard.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class QuickSightDataset(QuickSight):
     """Description"""
@@ -17289,15 +15447,16 @@
         if name in QuickSightDataset._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "quick_sight_dataset_import_mode",
         "quick_sight_dataset_column_count",
-        "terms",
+        "quick_sight_dataset_folders",
+        "quick_sight_dataset_fields",
     ]
 
     @property
     def quick_sight_dataset_import_mode(self) -> Optional[QuickSightDatasetImportMode]:
         return self.attributes.quick_sight_dataset_import_mode
 
     @quick_sight_dataset_import_mode.setter
@@ -17321,24 +15480,36 @@
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.quick_sight_dataset_column_count = (
             quick_sight_dataset_column_count
         )
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def quick_sight_dataset_folders(self) -> Optional[list[QuickSightFolder]]:
+        return self.attributes.quick_sight_dataset_folders
+
+    @quick_sight_dataset_folders.setter
+    def quick_sight_dataset_folders(
+        self, quick_sight_dataset_folders: Optional[list[QuickSightFolder]]
+    ):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.quick_sight_dataset_folders = quick_sight_dataset_folders
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def quick_sight_dataset_fields(self) -> Optional[list[QuickSightDatasetField]]:
+        return self.attributes.quick_sight_dataset_fields
+
+    @quick_sight_dataset_fields.setter
+    def quick_sight_dataset_fields(
+        self, quick_sight_dataset_fields: Optional[list[QuickSightDatasetField]]
+    ):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.quick_sight_dataset_fields = quick_sight_dataset_fields
 
     type_name: str = Field("QuickSightDataset", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "QuickSightDataset":
             raise ValueError("must be QuickSightDataset")
@@ -17347,115 +15518,67 @@
     class Attributes(QuickSight.Attributes):
         quick_sight_dataset_import_mode: Optional[QuickSightDatasetImportMode] = Field(
             None, description="", alias="quickSightDatasetImportMode"
         )
         quick_sight_dataset_column_count: Optional[int] = Field(
             None, description="", alias="quickSightDatasetColumnCount"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         quick_sight_dataset_folders: Optional[list[QuickSightFolder]] = Field(
             None, description="", alias="quickSightDatasetFolders"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
         quick_sight_dataset_fields: Optional[list[QuickSightDatasetField]] = Field(
             None, description="", alias="quickSightDatasetFields"
         )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "QuickSightDataset.Attributes" = Field(
-        None,
+        default_factory=lambda: QuickSightDataset.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class ThoughtspotLiveboard(Thoughtspot):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in ThoughtspotLiveboard._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
-        "terms",
+        "thoughtspot_dashlets",
     ]
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+    def thoughtspot_dashlets(self) -> Optional[list[ThoughtspotDashlet]]:
+        return self.attributes.thoughtspot_dashlets
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @thoughtspot_dashlets.setter
+    def thoughtspot_dashlets(
+        self, thoughtspot_dashlets: Optional[list[ThoughtspotDashlet]]
+    ):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.thoughtspot_dashlets = thoughtspot_dashlets
 
     type_name: str = Field("ThoughtspotLiveboard", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "ThoughtspotLiveboard":
             raise ValueError("must be ThoughtspotLiveboard")
         return v
 
     class Attributes(Thoughtspot.Attributes):
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         thoughtspot_dashlets: Optional[list[ThoughtspotDashlet]] = Field(
             None, description="", alias="thoughtspotDashlets"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "ThoughtspotLiveboard.Attributes" = Field(
-        None,
+        default_factory=lambda: ThoughtspotLiveboard.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class ThoughtspotDashlet(Thoughtspot):
     """Description"""
@@ -17464,15 +15587,15 @@
         if name in ThoughtspotDashlet._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "thoughtspot_liveboard_name",
         "thoughtspot_liveboard_qualified_name",
-        "terms",
+        "thoughtspot_liveboard",
     ]
 
     @property
     def thoughtspot_liveboard_name(self) -> Optional[str]:
         return self.attributes.thoughtspot_liveboard_name
 
     @thoughtspot_liveboard_name.setter
@@ -17492,24 +15615,24 @@
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.thoughtspot_liveboard_qualified_name = (
             thoughtspot_liveboard_qualified_name
         )
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+    def thoughtspot_liveboard(self) -> Optional[ThoughtspotLiveboard]:
+        return self.attributes.thoughtspot_liveboard
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @thoughtspot_liveboard.setter
+    def thoughtspot_liveboard(
+        self, thoughtspot_liveboard: Optional[ThoughtspotLiveboard]
+    ):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.thoughtspot_liveboard = thoughtspot_liveboard
 
     type_name: str = Field("ThoughtspotDashlet", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "ThoughtspotDashlet":
             raise ValueError("must be ThoughtspotDashlet")
@@ -17518,128 +15641,61 @@
     class Attributes(Thoughtspot.Attributes):
         thoughtspot_liveboard_name: Optional[str] = Field(
             None, description="", alias="thoughtspotLiveboardName"
         )
         thoughtspot_liveboard_qualified_name: Optional[str] = Field(
             None, description="", alias="thoughtspotLiveboardQualifiedName"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         thoughtspot_liveboard: Optional[ThoughtspotLiveboard] = Field(
             None, description="", alias="thoughtspotLiveboard"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "ThoughtspotDashlet.Attributes" = Field(
-        None,
+        default_factory=lambda: ThoughtspotDashlet.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class ThoughtspotAnswer(Thoughtspot):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in ThoughtspotAnswer._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
-    _convience_properties: ClassVar[list[str]] = [
-        "terms",
-    ]
-
-    @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
-
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+    _convience_properties: ClassVar[list[str]] = []
 
     type_name: str = Field("ThoughtspotAnswer", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "ThoughtspotAnswer":
             raise ValueError("must be ThoughtspotAnswer")
         return v
 
-    class Attributes(Thoughtspot.Attributes):
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
-
-    attributes: "ThoughtspotAnswer.Attributes" = Field(
-        None,
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
 
 class PowerBIReport(PowerBI):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in PowerBIReport._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "workspace_qualified_name",
         "dataset_qualified_name",
         "web_url",
         "page_count",
-        "terms",
+        "workspace",
+        "tiles",
+        "pages",
+        "dataset",
     ]
 
     @property
     def workspace_qualified_name(self) -> Optional[str]:
         return self.attributes.workspace_qualified_name
 
     @workspace_qualified_name.setter
@@ -17675,24 +15731,52 @@
     @page_count.setter
     def page_count(self, page_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.page_count = page_count
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def workspace(self) -> Optional[PowerBIWorkspace]:
+        return self.attributes.workspace
+
+    @workspace.setter
+    def workspace(self, workspace: Optional[PowerBIWorkspace]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.workspace = workspace
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def tiles(self) -> Optional[list[PowerBITile]]:
+        return self.attributes.tiles
+
+    @tiles.setter
+    def tiles(self, tiles: Optional[list[PowerBITile]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.tiles = tiles
+
+    @property
+    def pages(self) -> Optional[list[PowerBIPage]]:
+        return self.attributes.pages
+
+    @pages.setter
+    def pages(self, pages: Optional[list[PowerBIPage]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.pages = pages
+
+    @property
+    def dataset(self) -> Optional[PowerBIDataset]:
+        return self.attributes.dataset
+
+    @dataset.setter
+    def dataset(self, dataset: Optional[PowerBIDataset]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.dataset = dataset
 
     type_name: str = Field("PowerBIReport", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "PowerBIReport":
             raise ValueError("must be PowerBIReport")
@@ -17703,53 +15787,29 @@
             None, description="", alias="workspaceQualifiedName"
         )
         dataset_qualified_name: Optional[str] = Field(
             None, description="", alias="datasetQualifiedName"
         )
         web_url: Optional[str] = Field(None, description="", alias="webUrl")
         page_count: Optional[int] = Field(None, description="", alias="pageCount")
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        tiles: Optional[list[PowerBITile]] = Field(
-            None, description="", alias="tiles"
-        )  # relationship
         workspace: Optional[PowerBIWorkspace] = Field(
             None, description="", alias="workspace"
         )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
+        tiles: Optional[list[PowerBITile]] = Field(
+            None, description="", alias="tiles"
         )  # relationship
         pages: Optional[list[PowerBIPage]] = Field(
             None, description="", alias="pages"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
         dataset: Optional[PowerBIDataset] = Field(
             None, description="", alias="dataset"
         )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "PowerBIReport.Attributes" = Field(
-        None,
+        default_factory=lambda: PowerBIReport.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class PowerBIMeasure(PowerBI):
     """Description"""
@@ -17760,15 +15820,15 @@
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "workspace_qualified_name",
         "dataset_qualified_name",
         "power_b_i_measure_expression",
         "power_b_i_is_external_measure",
-        "terms",
+        "table",
     ]
 
     @property
     def workspace_qualified_name(self) -> Optional[str]:
         return self.attributes.workspace_qualified_name
 
     @workspace_qualified_name.setter
@@ -17806,24 +15866,22 @@
         self, power_b_i_is_external_measure: Optional[bool]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.power_b_i_is_external_measure = power_b_i_is_external_measure
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+    def table(self) -> Optional[PowerBITable]:
+        return self.attributes.table
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @table.setter
+    def table(self, table: Optional[PowerBITable]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.table = table
 
     type_name: str = Field("PowerBIMeasure", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "PowerBIMeasure":
             raise ValueError("must be PowerBIMeasure")
@@ -17838,44 +15896,20 @@
         )
         power_b_i_measure_expression: Optional[str] = Field(
             None, description="", alias="powerBIMeasureExpression"
         )
         power_b_i_is_external_measure: Optional[bool] = Field(
             None, description="", alias="powerBIIsExternalMeasure"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
         table: Optional[PowerBITable] = Field(
             None, description="", alias="table"
         )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "PowerBIMeasure.Attributes" = Field(
-        None,
+        default_factory=lambda: PowerBIMeasure.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class PowerBIColumn(PowerBI):
     """Description"""
@@ -17888,15 +15922,15 @@
     _convience_properties: ClassVar[list[str]] = [
         "workspace_qualified_name",
         "dataset_qualified_name",
         "power_b_i_column_data_category",
         "power_b_i_column_data_type",
         "power_b_i_sort_by_column",
         "power_b_i_column_summarize_by",
-        "terms",
+        "table",
     ]
 
     @property
     def workspace_qualified_name(self) -> Optional[str]:
         return self.attributes.workspace_qualified_name
 
     @workspace_qualified_name.setter
@@ -17956,24 +15990,22 @@
         self, power_b_i_column_summarize_by: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.power_b_i_column_summarize_by = power_b_i_column_summarize_by
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+    def table(self) -> Optional[PowerBITable]:
+        return self.attributes.table
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @table.setter
+    def table(self, table: Optional[PowerBITable]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.table = table
 
     type_name: str = Field("PowerBIColumn", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "PowerBIColumn":
             raise ValueError("must be PowerBIColumn")
@@ -17994,44 +16026,20 @@
         )
         power_b_i_sort_by_column: Optional[str] = Field(
             None, description="", alias="powerBISortByColumn"
         )
         power_b_i_column_summarize_by: Optional[str] = Field(
             None, description="", alias="powerBIColumnSummarizeBy"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
         table: Optional[PowerBITable] = Field(
             None, description="", alias="table"
         )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "PowerBIColumn.Attributes" = Field(
-        None,
+        default_factory=lambda: PowerBIColumn.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class PowerBITable(PowerBI):
     """Description"""
@@ -18043,15 +16051,17 @@
 
     _convience_properties: ClassVar[list[str]] = [
         "workspace_qualified_name",
         "dataset_qualified_name",
         "power_b_i_table_source_expressions",
         "power_b_i_table_column_count",
         "power_b_i_table_measure_count",
-        "terms",
+        "measures",
+        "columns",
+        "dataset",
     ]
 
     @property
     def workspace_qualified_name(self) -> Optional[str]:
         return self.attributes.workspace_qualified_name
 
     @workspace_qualified_name.setter
@@ -18103,24 +16113,42 @@
         self, power_b_i_table_measure_count: Optional[int]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.power_b_i_table_measure_count = power_b_i_table_measure_count
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def measures(self) -> Optional[list[PowerBIMeasure]]:
+        return self.attributes.measures
+
+    @measures.setter
+    def measures(self, measures: Optional[list[PowerBIMeasure]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.measures = measures
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def columns(self) -> Optional[list[PowerBIColumn]]:
+        return self.attributes.columns
+
+    @columns.setter
+    def columns(self, columns: Optional[list[PowerBIColumn]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.columns = columns
+
+    @property
+    def dataset(self) -> Optional[PowerBIDataset]:
+        return self.attributes.dataset
+
+    @dataset.setter
+    def dataset(self, dataset: Optional[PowerBIDataset]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.dataset = dataset
 
     type_name: str = Field("PowerBITable", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "PowerBITable":
             raise ValueError("must be PowerBITable")
@@ -18138,50 +16166,26 @@
         )
         power_b_i_table_column_count: Optional[int] = Field(
             None, description="", alias="powerBITableColumnCount"
         )
         power_b_i_table_measure_count: Optional[int] = Field(
             None, description="", alias="powerBITableMeasureCount"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
         measures: Optional[list[PowerBIMeasure]] = Field(
             None, description="", alias="measures"
         )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         columns: Optional[list[PowerBIColumn]] = Field(
             None, description="", alias="columns"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
         dataset: Optional[PowerBIDataset] = Field(
             None, description="", alias="dataset"
         )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "PowerBITable.Attributes" = Field(
-        None,
+        default_factory=lambda: PowerBITable.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class PowerBITile(PowerBI):
     """Description"""
@@ -18190,15 +16194,17 @@
         if name in PowerBITile._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "workspace_qualified_name",
         "dashboard_qualified_name",
-        "terms",
+        "report",
+        "dataset",
+        "dashboard",
     ]
 
     @property
     def workspace_qualified_name(self) -> Optional[str]:
         return self.attributes.workspace_qualified_name
 
     @workspace_qualified_name.setter
@@ -18214,24 +16220,42 @@
     @dashboard_qualified_name.setter
     def dashboard_qualified_name(self, dashboard_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dashboard_qualified_name = dashboard_qualified_name
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def report(self) -> Optional[PowerBIReport]:
+        return self.attributes.report
+
+    @report.setter
+    def report(self, report: Optional[PowerBIReport]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.report = report
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def dataset(self) -> Optional[PowerBIDataset]:
+        return self.attributes.dataset
+
+    @dataset.setter
+    def dataset(self, dataset: Optional[PowerBIDataset]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.dataset = dataset
+
+    @property
+    def dashboard(self) -> Optional[PowerBIDashboard]:
+        return self.attributes.dashboard
+
+    @dashboard.setter
+    def dashboard(self, dashboard: Optional[PowerBIDashboard]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.dashboard = dashboard
 
     type_name: str = Field("PowerBITile", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "PowerBITile":
             raise ValueError("must be PowerBITile")
@@ -18240,50 +16264,26 @@
     class Attributes(PowerBI.Attributes):
         workspace_qualified_name: Optional[str] = Field(
             None, description="", alias="workspaceQualifiedName"
         )
         dashboard_qualified_name: Optional[str] = Field(
             None, description="", alias="dashboardQualifiedName"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         report: Optional[PowerBIReport] = Field(
             None, description="", alias="report"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
         dataset: Optional[PowerBIDataset] = Field(
             None, description="", alias="dataset"
         )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
         dashboard: Optional[PowerBIDashboard] = Field(
             None, description="", alias="dashboard"
         )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "PowerBITile.Attributes" = Field(
-        None,
+        default_factory=lambda: PowerBITile.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class PowerBIDatasource(PowerBI):
     """Description"""
@@ -18291,81 +16291,55 @@
     def __setattr__(self, name, value):
         if name in PowerBIDatasource._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "connection_details",
-        "terms",
+        "datasets",
     ]
 
     @property
     def connection_details(self) -> Optional[dict[str, str]]:
         return self.attributes.connection_details
 
     @connection_details.setter
     def connection_details(self, connection_details: Optional[dict[str, str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.connection_details = connection_details
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+    def datasets(self) -> Optional[list[PowerBIDataset]]:
+        return self.attributes.datasets
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @datasets.setter
+    def datasets(self, datasets: Optional[list[PowerBIDataset]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.datasets = datasets
 
     type_name: str = Field("PowerBIDatasource", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "PowerBIDatasource":
             raise ValueError("must be PowerBIDatasource")
         return v
 
     class Attributes(PowerBI.Attributes):
         connection_details: Optional[dict[str, str]] = Field(
             None, description="", alias="connectionDetails"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
         datasets: Optional[list[PowerBIDataset]] = Field(
             None, description="", alias="datasets"
         )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "PowerBIDatasource.Attributes" = Field(
-        None,
+        default_factory=lambda: PowerBIDatasource.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class PowerBIWorkspace(PowerBI):
     """Description"""
@@ -18377,15 +16351,18 @@
 
     _convience_properties: ClassVar[list[str]] = [
         "web_url",
         "report_count",
         "dashboard_count",
         "dataset_count",
         "dataflow_count",
-        "terms",
+        "reports",
+        "datasets",
+        "dashboards",
+        "dataflows",
     ]
 
     @property
     def web_url(self) -> Optional[str]:
         return self.attributes.web_url
 
     @web_url.setter
@@ -18431,24 +16408,52 @@
     @dataflow_count.setter
     def dataflow_count(self, dataflow_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dataflow_count = dataflow_count
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def reports(self) -> Optional[list[PowerBIReport]]:
+        return self.attributes.reports
+
+    @reports.setter
+    def reports(self, reports: Optional[list[PowerBIReport]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.reports = reports
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def datasets(self) -> Optional[list[PowerBIDataset]]:
+        return self.attributes.datasets
+
+    @datasets.setter
+    def datasets(self, datasets: Optional[list[PowerBIDataset]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.datasets = datasets
+
+    @property
+    def dashboards(self) -> Optional[list[PowerBIDashboard]]:
+        return self.attributes.dashboards
+
+    @dashboards.setter
+    def dashboards(self, dashboards: Optional[list[PowerBIDashboard]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.dashboards = dashboards
+
+    @property
+    def dataflows(self) -> Optional[list[PowerBIDataflow]]:
+        return self.attributes.dataflows
+
+    @dataflows.setter
+    def dataflows(self, dataflows: Optional[list[PowerBIDataflow]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.dataflows = dataflows
 
     type_name: str = Field("PowerBIWorkspace", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "PowerBIWorkspace":
             raise ValueError("must be PowerBIWorkspace")
@@ -18460,53 +16465,29 @@
         dashboard_count: Optional[int] = Field(
             None, description="", alias="dashboardCount"
         )
         dataset_count: Optional[int] = Field(None, description="", alias="datasetCount")
         dataflow_count: Optional[int] = Field(
             None, description="", alias="dataflowCount"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
         reports: Optional[list[PowerBIReport]] = Field(
             None, description="", alias="reports"
         )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
         datasets: Optional[list[PowerBIDataset]] = Field(
             None, description="", alias="datasets"
         )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
         dashboards: Optional[list[PowerBIDashboard]] = Field(
             None, description="", alias="dashboards"
         )  # relationship
         dataflows: Optional[list[PowerBIDataflow]] = Field(
             None, description="", alias="dataflows"
         )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "PowerBIWorkspace.Attributes" = Field(
-        None,
+        default_factory=lambda: PowerBIWorkspace.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class PowerBIDataset(PowerBI):
     """Description"""
@@ -18515,15 +16496,20 @@
         if name in PowerBIDataset._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "workspace_qualified_name",
         "web_url",
-        "terms",
+        "reports",
+        "workspace",
+        "dataflows",
+        "tiles",
+        "tables",
+        "datasources",
     ]
 
     @property
     def workspace_qualified_name(self) -> Optional[str]:
         return self.attributes.workspace_qualified_name
 
     @workspace_qualified_name.setter
@@ -18539,83 +16525,107 @@
     @web_url.setter
     def web_url(self, web_url: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.web_url = web_url
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def reports(self) -> Optional[list[PowerBIReport]]:
+        return self.attributes.reports
+
+    @reports.setter
+    def reports(self, reports: Optional[list[PowerBIReport]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.reports = reports
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def workspace(self) -> Optional[PowerBIWorkspace]:
+        return self.attributes.workspace
+
+    @workspace.setter
+    def workspace(self, workspace: Optional[PowerBIWorkspace]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.workspace = workspace
+
+    @property
+    def dataflows(self) -> Optional[list[PowerBIDataflow]]:
+        return self.attributes.dataflows
+
+    @dataflows.setter
+    def dataflows(self, dataflows: Optional[list[PowerBIDataflow]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.dataflows = dataflows
+
+    @property
+    def tiles(self) -> Optional[list[PowerBITile]]:
+        return self.attributes.tiles
+
+    @tiles.setter
+    def tiles(self, tiles: Optional[list[PowerBITile]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.tiles = tiles
+
+    @property
+    def tables(self) -> Optional[list[PowerBITable]]:
+        return self.attributes.tables
+
+    @tables.setter
+    def tables(self, tables: Optional[list[PowerBITable]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.tables = tables
+
+    @property
+    def datasources(self) -> Optional[list[PowerBIDatasource]]:
+        return self.attributes.datasources
+
+    @datasources.setter
+    def datasources(self, datasources: Optional[list[PowerBIDatasource]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.datasources = datasources
 
     type_name: str = Field("PowerBIDataset", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "PowerBIDataset":
             raise ValueError("must be PowerBIDataset")
         return v
 
     class Attributes(PowerBI.Attributes):
         workspace_qualified_name: Optional[str] = Field(
             None, description="", alias="workspaceQualifiedName"
         )
         web_url: Optional[str] = Field(None, description="", alias="webUrl")
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
         reports: Optional[list[PowerBIReport]] = Field(
             None, description="", alias="reports"
         )  # relationship
         workspace: Optional[PowerBIWorkspace] = Field(
             None, description="", alias="workspace"
         )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
         dataflows: Optional[list[PowerBIDataflow]] = Field(
             None, description="", alias="dataflows"
         )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
         tiles: Optional[list[PowerBITile]] = Field(
             None, description="", alias="tiles"
         )  # relationship
         tables: Optional[list[PowerBITable]] = Field(
             None, description="", alias="tables"
         )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         datasources: Optional[list[PowerBIDatasource]] = Field(
             None, description="", alias="datasources"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "PowerBIDataset.Attributes" = Field(
-        None,
+        default_factory=lambda: PowerBIDataset.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class PowerBIDashboard(PowerBI):
     """Description"""
@@ -18625,15 +16635,16 @@
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "workspace_qualified_name",
         "web_url",
         "tile_count",
-        "terms",
+        "tiles",
+        "workspace",
     ]
 
     @property
     def workspace_qualified_name(self) -> Optional[str]:
         return self.attributes.workspace_qualified_name
 
     @workspace_qualified_name.setter
@@ -18659,24 +16670,32 @@
     @tile_count.setter
     def tile_count(self, tile_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.tile_count = tile_count
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def tiles(self) -> Optional[list[PowerBITile]]:
+        return self.attributes.tiles
+
+    @tiles.setter
+    def tiles(self, tiles: Optional[list[PowerBITile]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.tiles = tiles
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def workspace(self) -> Optional[PowerBIWorkspace]:
+        return self.attributes.workspace
+
+    @workspace.setter
+    def workspace(self, workspace: Optional[PowerBIWorkspace]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.workspace = workspace
 
     type_name: str = Field("PowerBIDashboard", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "PowerBIDashboard":
             raise ValueError("must be PowerBIDashboard")
@@ -18684,47 +16703,23 @@
 
     class Attributes(PowerBI.Attributes):
         workspace_qualified_name: Optional[str] = Field(
             None, description="", alias="workspaceQualifiedName"
         )
         web_url: Optional[str] = Field(None, description="", alias="webUrl")
         tile_count: Optional[int] = Field(None, description="", alias="tileCount")
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
         tiles: Optional[list[PowerBITile]] = Field(
             None, description="", alias="tiles"
         )  # relationship
         workspace: Optional[PowerBIWorkspace] = Field(
             None, description="", alias="workspace"
         )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "PowerBIDashboard.Attributes" = Field(
-        None,
+        default_factory=lambda: PowerBIDashboard.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class PowerBIDataflow(PowerBI):
     """Description"""
@@ -18733,15 +16728,16 @@
         if name in PowerBIDataflow._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "workspace_qualified_name",
         "web_url",
-        "terms",
+        "workspace",
+        "datasets",
     ]
 
     @property
     def workspace_qualified_name(self) -> Optional[str]:
         return self.attributes.workspace_qualified_name
 
     @workspace_qualified_name.setter
@@ -18757,71 +16753,55 @@
     @web_url.setter
     def web_url(self, web_url: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.web_url = web_url
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def workspace(self) -> Optional[PowerBIWorkspace]:
+        return self.attributes.workspace
+
+    @workspace.setter
+    def workspace(self, workspace: Optional[PowerBIWorkspace]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.workspace = workspace
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def datasets(self) -> Optional[list[PowerBIDataset]]:
+        return self.attributes.datasets
+
+    @datasets.setter
+    def datasets(self, datasets: Optional[list[PowerBIDataset]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.datasets = datasets
 
     type_name: str = Field("PowerBIDataflow", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "PowerBIDataflow":
             raise ValueError("must be PowerBIDataflow")
         return v
 
     class Attributes(PowerBI.Attributes):
         workspace_qualified_name: Optional[str] = Field(
             None, description="", alias="workspaceQualifiedName"
         )
         web_url: Optional[str] = Field(None, description="", alias="webUrl")
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
         workspace: Optional[PowerBIWorkspace] = Field(
             None, description="", alias="workspace"
         )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
         datasets: Optional[list[PowerBIDataset]] = Field(
             None, description="", alias="datasets"
         )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "PowerBIDataflow.Attributes" = Field(
-        None,
+        default_factory=lambda: PowerBIDataflow.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class PowerBIPage(PowerBI):
     """Description"""
@@ -18830,15 +16810,15 @@
         if name in PowerBIPage._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "workspace_qualified_name",
         "report_qualified_name",
-        "terms",
+        "report",
     ]
 
     @property
     def workspace_qualified_name(self) -> Optional[str]:
         return self.attributes.workspace_qualified_name
 
     @workspace_qualified_name.setter
@@ -18854,24 +16834,22 @@
     @report_qualified_name.setter
     def report_qualified_name(self, report_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.report_qualified_name = report_qualified_name
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+    def report(self) -> Optional[PowerBIReport]:
+        return self.attributes.report
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @report.setter
+    def report(self, report: Optional[PowerBIReport]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.report = report
 
     type_name: str = Field("PowerBIPage", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "PowerBIPage":
             raise ValueError("must be PowerBIPage")
@@ -18880,44 +16858,20 @@
     class Attributes(PowerBI.Attributes):
         workspace_qualified_name: Optional[str] = Field(
             None, description="", alias="workspaceQualifiedName"
         )
         report_qualified_name: Optional[str] = Field(
             None, description="", alias="reportQualifiedName"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         report: Optional[PowerBIReport] = Field(
             None, description="", alias="report"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "PowerBIPage.Attributes" = Field(
-        None,
+        default_factory=lambda: PowerBIPage.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class PresetChart(Preset):
     """Description"""
@@ -18926,15 +16880,15 @@
         if name in PresetChart._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "preset_chart_description_markdown",
         "preset_chart_form_data",
-        "terms",
+        "preset_dashboard",
     ]
 
     @property
     def preset_chart_description_markdown(self) -> Optional[str]:
         return self.attributes.preset_chart_description_markdown
 
     @preset_chart_description_markdown.setter
@@ -18954,24 +16908,22 @@
     @preset_chart_form_data.setter
     def preset_chart_form_data(self, preset_chart_form_data: Optional[dict[str, str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.preset_chart_form_data = preset_chart_form_data
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+    def preset_dashboard(self) -> Optional[PresetDashboard]:
+        return self.attributes.preset_dashboard
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @preset_dashboard.setter
+    def preset_dashboard(self, preset_dashboard: Optional[PresetDashboard]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.preset_dashboard = preset_dashboard
 
     type_name: str = Field("PresetChart", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "PresetChart":
             raise ValueError("must be PresetChart")
@@ -18980,44 +16932,20 @@
     class Attributes(Preset.Attributes):
         preset_chart_description_markdown: Optional[str] = Field(
             None, description="", alias="presetChartDescriptionMarkdown"
         )
         preset_chart_form_data: Optional[dict[str, str]] = Field(
             None, description="", alias="presetChartFormData"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
         preset_dashboard: Optional[PresetDashboard] = Field(
             None, description="", alias="presetDashboard"
         )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "PresetChart.Attributes" = Field(
-        None,
+        default_factory=lambda: PresetChart.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class PresetDataset(Preset):
     """Description"""
@@ -19027,15 +16955,15 @@
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "preset_dataset_datasource_name",
         "preset_dataset_id",
         "preset_dataset_type",
-        "terms",
+        "preset_dashboard",
     ]
 
     @property
     def preset_dataset_datasource_name(self) -> Optional[str]:
         return self.attributes.preset_dataset_datasource_name
 
     @preset_dataset_datasource_name.setter
@@ -19063,24 +16991,22 @@
     @preset_dataset_type.setter
     def preset_dataset_type(self, preset_dataset_type: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.preset_dataset_type = preset_dataset_type
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+    def preset_dashboard(self) -> Optional[PresetDashboard]:
+        return self.attributes.preset_dashboard
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @preset_dashboard.setter
+    def preset_dashboard(self, preset_dashboard: Optional[PresetDashboard]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.preset_dashboard = preset_dashboard
 
     type_name: str = Field("PresetDataset", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "PresetDataset":
             raise ValueError("must be PresetDataset")
@@ -19092,44 +17018,20 @@
         )
         preset_dataset_id: Optional[int] = Field(
             None, description="", alias="presetDatasetId"
         )
         preset_dataset_type: Optional[str] = Field(
             None, description="", alias="presetDatasetType"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
         preset_dashboard: Optional[PresetDashboard] = Field(
             None, description="", alias="presetDashboard"
         )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "PresetDataset.Attributes" = Field(
-        None,
+        default_factory=lambda: PresetDataset.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class PresetDashboard(Preset):
     """Description"""
@@ -19142,15 +17044,17 @@
     _convience_properties: ClassVar[list[str]] = [
         "preset_dashboard_changed_by_name",
         "preset_dashboard_changed_by_url",
         "preset_dashboard_is_managed_externally",
         "preset_dashboard_is_published",
         "preset_dashboard_thumbnail_url",
         "preset_dashboard_chart_count",
-        "terms",
+        "preset_datasets",
+        "preset_charts",
+        "preset_workspace",
     ]
 
     @property
     def preset_dashboard_changed_by_name(self) -> Optional[str]:
         return self.attributes.preset_dashboard_changed_by_name
 
     @preset_dashboard_changed_by_name.setter
@@ -19222,24 +17126,42 @@
     @preset_dashboard_chart_count.setter
     def preset_dashboard_chart_count(self, preset_dashboard_chart_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.preset_dashboard_chart_count = preset_dashboard_chart_count
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def preset_datasets(self) -> Optional[list[PresetDataset]]:
+        return self.attributes.preset_datasets
+
+    @preset_datasets.setter
+    def preset_datasets(self, preset_datasets: Optional[list[PresetDataset]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.preset_datasets = preset_datasets
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def preset_charts(self) -> Optional[list[PresetChart]]:
+        return self.attributes.preset_charts
+
+    @preset_charts.setter
+    def preset_charts(self, preset_charts: Optional[list[PresetChart]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.preset_charts = preset_charts
+
+    @property
+    def preset_workspace(self) -> Optional[PresetWorkspace]:
+        return self.attributes.preset_workspace
+
+    @preset_workspace.setter
+    def preset_workspace(self, preset_workspace: Optional[PresetWorkspace]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.preset_workspace = preset_workspace
 
     type_name: str = Field("PresetDashboard", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "PresetDashboard":
             raise ValueError("must be PresetDashboard")
@@ -19263,47 +17185,23 @@
         )
         preset_dashboard_chart_count: Optional[int] = Field(
             None, description="", alias="presetDashboardChartCount"
         )
         preset_datasets: Optional[list[PresetDataset]] = Field(
             None, description="", alias="presetDatasets"
         )  # relationship
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         preset_charts: Optional[list[PresetChart]] = Field(
             None, description="", alias="presetCharts"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
         preset_workspace: Optional[PresetWorkspace] = Field(
             None, description="", alias="presetWorkspace"
         )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "PresetDashboard.Attributes" = Field(
-        None,
+        default_factory=lambda: PresetDashboard.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class PresetWorkspace(Preset):
     """Description"""
@@ -19319,15 +17217,15 @@
         "preset_workspace_hostname",
         "preset_workspace_is_in_maintenance_mode",
         "preset_workspace_region",
         "preset_workspace_status",
         "preset_workspace_deployment_id",
         "preset_workspace_dashboard_count",
         "preset_workspace_dataset_count",
-        "terms",
+        "preset_dashboards",
     ]
 
     @property
     def preset_workspace_public_dashboards_allowed(self) -> Optional[bool]:
         return self.attributes.preset_workspace_public_dashboards_allowed
 
     @preset_workspace_public_dashboards_allowed.setter
@@ -19429,24 +17327,22 @@
         self, preset_workspace_dataset_count: Optional[int]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.preset_workspace_dataset_count = preset_workspace_dataset_count
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+    def preset_dashboards(self) -> Optional[list[PresetDashboard]]:
+        return self.attributes.preset_dashboards
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @preset_dashboards.setter
+    def preset_dashboards(self, preset_dashboards: Optional[list[PresetDashboard]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.preset_dashboards = preset_dashboards
 
     type_name: str = Field("PresetWorkspace", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "PresetWorkspace":
             raise ValueError("must be PresetWorkspace")
@@ -19479,41 +17375,17 @@
         )
         preset_workspace_dataset_count: Optional[int] = Field(
             None, description="", alias="presetWorkspaceDatasetCount"
         )
         preset_dashboards: Optional[list[PresetDashboard]] = Field(
             None, description="", alias="presetDashboards"
         )  # relationship
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "PresetWorkspace.Attributes" = Field(
-        None,
+        default_factory=lambda: PresetWorkspace.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class ModeReport(Mode):
     """Description"""
@@ -19527,15 +17399,16 @@
         "mode_collection_token",
         "mode_report_published_at",
         "mode_query_count",
         "mode_chart_count",
         "mode_query_preview",
         "mode_is_public",
         "mode_is_shared",
-        "terms",
+        "mode_collections",
+        "mode_queries",
     ]
 
     @property
     def mode_collection_token(self) -> Optional[str]:
         return self.attributes.mode_collection_token
 
     @mode_collection_token.setter
@@ -19601,24 +17474,32 @@
     @mode_is_shared.setter
     def mode_is_shared(self, mode_is_shared: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mode_is_shared = mode_is_shared
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def mode_collections(self) -> Optional[list[ModeCollection]]:
+        return self.attributes.mode_collections
+
+    @mode_collections.setter
+    def mode_collections(self, mode_collections: Optional[list[ModeCollection]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.mode_collections = mode_collections
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def mode_queries(self) -> Optional[list[ModeQuery]]:
+        return self.attributes.mode_queries
+
+    @mode_queries.setter
+    def mode_queries(self, mode_queries: Optional[list[ModeQuery]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.mode_queries = mode_queries
 
     type_name: str = Field("ModeReport", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "ModeReport":
             raise ValueError("must be ModeReport")
@@ -19642,47 +17523,23 @@
         )
         mode_is_public: Optional[bool] = Field(
             None, description="", alias="modeIsPublic"
         )
         mode_is_shared: Optional[bool] = Field(
             None, description="", alias="modeIsShared"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         mode_collections: Optional[list[ModeCollection]] = Field(
             None, description="", alias="modeCollections"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
         mode_queries: Optional[list[ModeQuery]] = Field(
             None, description="", alias="modeQueries"
         )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "ModeReport.Attributes" = Field(
-        None,
+        default_factory=lambda: ModeReport.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class ModeQuery(Mode):
     """Description"""
@@ -19691,15 +17548,16 @@
         if name in ModeQuery._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "mode_raw_query",
         "mode_report_import_count",
-        "terms",
+        "mode_charts",
+        "mode_report",
     ]
 
     @property
     def mode_raw_query(self) -> Optional[str]:
         return self.attributes.mode_raw_query
 
     @mode_raw_query.setter
@@ -19715,24 +17573,32 @@
     @mode_report_import_count.setter
     def mode_report_import_count(self, mode_report_import_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mode_report_import_count = mode_report_import_count
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def mode_charts(self) -> Optional[list[ModeChart]]:
+        return self.attributes.mode_charts
+
+    @mode_charts.setter
+    def mode_charts(self, mode_charts: Optional[list[ModeChart]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.mode_charts = mode_charts
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def mode_report(self) -> Optional[ModeReport]:
+        return self.attributes.mode_report
+
+    @mode_report.setter
+    def mode_report(self, mode_report: Optional[ModeReport]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.mode_report = mode_report
 
     type_name: str = Field("ModeQuery", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "ModeQuery":
             raise ValueError("must be ModeQuery")
@@ -19744,44 +17610,20 @@
         )
         mode_report_import_count: Optional[int] = Field(
             None, description="", alias="modeReportImportCount"
         )
         mode_charts: Optional[list[ModeChart]] = Field(
             None, description="", alias="modeCharts"
         )  # relationship
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
         mode_report: Optional[ModeReport] = Field(
             None, description="", alias="modeReport"
         )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "ModeQuery.Attributes" = Field(
-        None,
+        default_factory=lambda: ModeQuery.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class ModeChart(Mode):
     """Description"""
@@ -19789,81 +17631,55 @@
     def __setattr__(self, name, value):
         if name in ModeChart._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "mode_chart_type",
-        "terms",
+        "mode_query",
     ]
 
     @property
     def mode_chart_type(self) -> Optional[str]:
         return self.attributes.mode_chart_type
 
     @mode_chart_type.setter
     def mode_chart_type(self, mode_chart_type: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mode_chart_type = mode_chart_type
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+    def mode_query(self) -> Optional[ModeQuery]:
+        return self.attributes.mode_query
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @mode_query.setter
+    def mode_query(self, mode_query: Optional[ModeQuery]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.mode_query = mode_query
 
     type_name: str = Field("ModeChart", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "ModeChart":
             raise ValueError("must be ModeChart")
         return v
 
     class Attributes(Mode.Attributes):
         mode_chart_type: Optional[str] = Field(
             None, description="", alias="modeChartType"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
         mode_query: Optional[ModeQuery] = Field(
             None, description="", alias="modeQuery"
         )  # relationship
 
     attributes: "ModeChart.Attributes" = Field(
-        None,
+        default_factory=lambda: ModeChart.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class ModeWorkspace(Mode):
     """Description"""
@@ -19871,81 +17687,55 @@
     def __setattr__(self, name, value):
         if name in ModeWorkspace._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "mode_collection_count",
-        "terms",
+        "mode_collections",
     ]
 
     @property
     def mode_collection_count(self) -> Optional[int]:
         return self.attributes.mode_collection_count
 
     @mode_collection_count.setter
     def mode_collection_count(self, mode_collection_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mode_collection_count = mode_collection_count
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+    def mode_collections(self) -> Optional[list[ModeCollection]]:
+        return self.attributes.mode_collections
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @mode_collections.setter
+    def mode_collections(self, mode_collections: Optional[list[ModeCollection]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.mode_collections = mode_collections
 
     type_name: str = Field("ModeWorkspace", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "ModeWorkspace":
             raise ValueError("must be ModeWorkspace")
         return v
 
     class Attributes(Mode.Attributes):
         mode_collection_count: Optional[int] = Field(
             None, description="", alias="modeCollectionCount"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         mode_collections: Optional[list[ModeCollection]] = Field(
             None, description="", alias="modeCollections"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "ModeWorkspace.Attributes" = Field(
-        None,
+        default_factory=lambda: ModeWorkspace.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class ModeCollection(Mode):
     """Description"""
@@ -19954,15 +17744,16 @@
         if name in ModeCollection._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "mode_collection_type",
         "mode_collection_state",
-        "terms",
+        "mode_workspace",
+        "mode_reports",
     ]
 
     @property
     def mode_collection_type(self) -> Optional[str]:
         return self.attributes.mode_collection_type
 
     @mode_collection_type.setter
@@ -19978,24 +17769,32 @@
     @mode_collection_state.setter
     def mode_collection_state(self, mode_collection_state: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mode_collection_state = mode_collection_state
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def mode_workspace(self) -> Optional[ModeWorkspace]:
+        return self.attributes.mode_workspace
+
+    @mode_workspace.setter
+    def mode_workspace(self, mode_workspace: Optional[ModeWorkspace]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.mode_workspace = mode_workspace
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def mode_reports(self) -> Optional[list[ModeReport]]:
+        return self.attributes.mode_reports
+
+    @mode_reports.setter
+    def mode_reports(self, mode_reports: Optional[list[ModeReport]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.mode_reports = mode_reports
 
     type_name: str = Field("ModeCollection", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "ModeCollection":
             raise ValueError("must be ModeCollection")
@@ -20004,47 +17803,23 @@
     class Attributes(Mode.Attributes):
         mode_collection_type: Optional[str] = Field(
             None, description="", alias="modeCollectionType"
         )
         mode_collection_state: Optional[str] = Field(
             None, description="", alias="modeCollectionState"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
         mode_workspace: Optional[ModeWorkspace] = Field(
             None, description="", alias="modeWorkspace"
         )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
         mode_reports: Optional[list[ModeReport]] = Field(
             None, description="", alias="modeReports"
         )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "ModeCollection.Attributes" = Field(
-        None,
+        default_factory=lambda: ModeCollection.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class SigmaDatasetColumn(Sigma):
     """Description"""
@@ -20053,15 +17828,15 @@
         if name in SigmaDatasetColumn._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "sigma_dataset_qualified_name",
         "sigma_dataset_name",
-        "terms",
+        "sigma_dataset",
     ]
 
     @property
     def sigma_dataset_qualified_name(self) -> Optional[str]:
         return self.attributes.sigma_dataset_qualified_name
 
     @sigma_dataset_qualified_name.setter
@@ -20077,24 +17852,22 @@
     @sigma_dataset_name.setter
     def sigma_dataset_name(self, sigma_dataset_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sigma_dataset_name = sigma_dataset_name
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+    def sigma_dataset(self) -> Optional[SigmaDataset]:
+        return self.attributes.sigma_dataset
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @sigma_dataset.setter
+    def sigma_dataset(self, sigma_dataset: Optional[SigmaDataset]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.sigma_dataset = sigma_dataset
 
     type_name: str = Field("SigmaDatasetColumn", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "SigmaDatasetColumn":
             raise ValueError("must be SigmaDatasetColumn")
@@ -20103,44 +17876,20 @@
     class Attributes(Sigma.Attributes):
         sigma_dataset_qualified_name: Optional[str] = Field(
             None, description="", alias="sigmaDatasetQualifiedName"
         )
         sigma_dataset_name: Optional[str] = Field(
             None, description="", alias="sigmaDatasetName"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         sigma_dataset: Optional[SigmaDataset] = Field(
             None, description="", alias="sigmaDataset"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "SigmaDatasetColumn.Attributes" = Field(
-        None,
+        default_factory=lambda: SigmaDatasetColumn.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class SigmaDataset(Sigma):
     """Description"""
@@ -20148,81 +17897,57 @@
     def __setattr__(self, name, value):
         if name in SigmaDataset._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "sigma_dataset_column_count",
-        "terms",
+        "sigma_dataset_columns",
     ]
 
     @property
     def sigma_dataset_column_count(self) -> Optional[int]:
         return self.attributes.sigma_dataset_column_count
 
     @sigma_dataset_column_count.setter
     def sigma_dataset_column_count(self, sigma_dataset_column_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sigma_dataset_column_count = sigma_dataset_column_count
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+    def sigma_dataset_columns(self) -> Optional[list[SigmaDatasetColumn]]:
+        return self.attributes.sigma_dataset_columns
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @sigma_dataset_columns.setter
+    def sigma_dataset_columns(
+        self, sigma_dataset_columns: Optional[list[SigmaDatasetColumn]]
+    ):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.sigma_dataset_columns = sigma_dataset_columns
 
     type_name: str = Field("SigmaDataset", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "SigmaDataset":
             raise ValueError("must be SigmaDataset")
         return v
 
     class Attributes(Sigma.Attributes):
         sigma_dataset_column_count: Optional[int] = Field(
             None, description="", alias="sigmaDatasetColumnCount"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
         sigma_dataset_columns: Optional[list[SigmaDatasetColumn]] = Field(
             None, description="", alias="sigmaDatasetColumns"
         )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "SigmaDataset.Attributes" = Field(
-        None,
+        default_factory=lambda: SigmaDataset.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class SigmaWorkbook(Sigma):
     """Description"""
@@ -20230,81 +17955,55 @@
     def __setattr__(self, name, value):
         if name in SigmaWorkbook._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "sigma_page_count",
-        "terms",
+        "sigma_pages",
     ]
 
     @property
     def sigma_page_count(self) -> Optional[int]:
         return self.attributes.sigma_page_count
 
     @sigma_page_count.setter
     def sigma_page_count(self, sigma_page_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sigma_page_count = sigma_page_count
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+    def sigma_pages(self) -> Optional[list[SigmaPage]]:
+        return self.attributes.sigma_pages
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @sigma_pages.setter
+    def sigma_pages(self, sigma_pages: Optional[list[SigmaPage]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.sigma_pages = sigma_pages
 
     type_name: str = Field("SigmaWorkbook", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "SigmaWorkbook":
             raise ValueError("must be SigmaWorkbook")
         return v
 
     class Attributes(Sigma.Attributes):
         sigma_page_count: Optional[int] = Field(
             None, description="", alias="sigmaPageCount"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         sigma_pages: Optional[list[SigmaPage]] = Field(
             None, description="", alias="sigmaPages"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "SigmaWorkbook.Attributes" = Field(
-        None,
+        default_factory=lambda: SigmaWorkbook.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class SigmaDataElementField(Sigma):
     """Description"""
@@ -20313,15 +18012,15 @@
         if name in SigmaDataElementField._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "sigma_data_element_field_is_hidden",
         "sigma_data_element_field_formula",
-        "terms",
+        "sigma_data_element",
     ]
 
     @property
     def sigma_data_element_field_is_hidden(self) -> Optional[bool]:
         return self.attributes.sigma_data_element_field_is_hidden
 
     @sigma_data_element_field_is_hidden.setter
@@ -20345,24 +18044,22 @@
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sigma_data_element_field_formula = (
             sigma_data_element_field_formula
         )
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+    def sigma_data_element(self) -> Optional[SigmaDataElement]:
+        return self.attributes.sigma_data_element
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @sigma_data_element.setter
+    def sigma_data_element(self, sigma_data_element: Optional[SigmaDataElement]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.sigma_data_element = sigma_data_element
 
     type_name: str = Field("SigmaDataElementField", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "SigmaDataElementField":
             raise ValueError("must be SigmaDataElementField")
@@ -20371,44 +18068,20 @@
     class Attributes(Sigma.Attributes):
         sigma_data_element_field_is_hidden: Optional[bool] = Field(
             None, description="", alias="sigmaDataElementFieldIsHidden"
         )
         sigma_data_element_field_formula: Optional[str] = Field(
             None, description="", alias="sigmaDataElementFieldFormula"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         sigma_data_element: Optional[SigmaDataElement] = Field(
             None, description="", alias="sigmaDataElement"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "SigmaDataElementField.Attributes" = Field(
-        None,
+        default_factory=lambda: SigmaDataElementField.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class SigmaPage(Sigma):
     """Description"""
@@ -20416,38 +18089,49 @@
     def __setattr__(self, name, value):
         if name in SigmaPage._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "sigma_data_element_count",
-        "terms",
+        "sigma_data_elements",
+        "sigma_workbook",
     ]
 
     @property
     def sigma_data_element_count(self) -> Optional[int]:
         return self.attributes.sigma_data_element_count
 
     @sigma_data_element_count.setter
     def sigma_data_element_count(self, sigma_data_element_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sigma_data_element_count = sigma_data_element_count
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def sigma_data_elements(self) -> Optional[list[SigmaDataElement]]:
+        return self.attributes.sigma_data_elements
+
+    @sigma_data_elements.setter
+    def sigma_data_elements(
+        self, sigma_data_elements: Optional[list[SigmaDataElement]]
+    ):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.sigma_data_elements = sigma_data_elements
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def sigma_workbook(self) -> Optional[SigmaWorkbook]:
+        return self.attributes.sigma_workbook
+
+    @sigma_workbook.setter
+    def sigma_workbook(self, sigma_workbook: Optional[SigmaWorkbook]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.sigma_workbook = sigma_workbook
 
     type_name: str = Field("SigmaPage", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "SigmaPage":
             raise ValueError("must be SigmaPage")
@@ -20456,44 +18140,20 @@
     class Attributes(Sigma.Attributes):
         sigma_data_element_count: Optional[int] = Field(
             None, description="", alias="sigmaDataElementCount"
         )
         sigma_data_elements: Optional[list[SigmaDataElement]] = Field(
             None, description="", alias="sigmaDataElements"
         )  # relationship
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
         sigma_workbook: Optional[SigmaWorkbook] = Field(
             None, description="", alias="sigmaWorkbook"
         )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "SigmaPage.Attributes" = Field(
-        None,
+        default_factory=lambda: SigmaPage.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class SigmaDataElement(Sigma):
     """Description"""
@@ -20503,15 +18163,16 @@
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "sigma_data_element_query",
         "sigma_data_element_type",
         "sigma_data_element_field_count",
-        "terms",
+        "sigma_page",
+        "sigma_data_element_fields",
     ]
 
     @property
     def sigma_data_element_query(self) -> Optional[str]:
         return self.attributes.sigma_data_element_query
 
     @sigma_data_element_query.setter
@@ -20539,24 +18200,34 @@
         self, sigma_data_element_field_count: Optional[int]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sigma_data_element_field_count = sigma_data_element_field_count
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def sigma_page(self) -> Optional[SigmaPage]:
+        return self.attributes.sigma_page
+
+    @sigma_page.setter
+    def sigma_page(self, sigma_page: Optional[SigmaPage]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.sigma_page = sigma_page
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def sigma_data_element_fields(self) -> Optional[list[SigmaDataElementField]]:
+        return self.attributes.sigma_data_element_fields
+
+    @sigma_data_element_fields.setter
+    def sigma_data_element_fields(
+        self, sigma_data_element_fields: Optional[list[SigmaDataElementField]]
+    ):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.sigma_data_element_fields = sigma_data_element_fields
 
     type_name: str = Field("SigmaDataElement", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "SigmaDataElement":
             raise ValueError("must be SigmaDataElement")
@@ -20568,47 +18239,23 @@
         )
         sigma_data_element_type: Optional[str] = Field(
             None, description="", alias="sigmaDataElementType"
         )
         sigma_data_element_field_count: Optional[int] = Field(
             None, description="", alias="sigmaDataElementFieldCount"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
         sigma_page: Optional[SigmaPage] = Field(
             None, description="", alias="sigmaPage"
         )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
         sigma_data_element_fields: Optional[list[SigmaDataElementField]] = Field(
             None, description="", alias="sigmaDataElementFields"
         )  # relationship
 
     attributes: "SigmaDataElement.Attributes" = Field(
-        None,
+        default_factory=lambda: SigmaDataElement.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class QlikSpace(Qlik):
     """Description"""
@@ -20616,84 +18263,69 @@
     def __setattr__(self, name, value):
         if name in QlikSpace._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "qlik_space_type",
-        "terms",
+        "qlik_datasets",
+        "qlik_apps",
     ]
 
     @property
     def qlik_space_type(self) -> Optional[str]:
         return self.attributes.qlik_space_type
 
     @qlik_space_type.setter
     def qlik_space_type(self, qlik_space_type: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.qlik_space_type = qlik_space_type
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def qlik_datasets(self) -> Optional[list[QlikDataset]]:
+        return self.attributes.qlik_datasets
+
+    @qlik_datasets.setter
+    def qlik_datasets(self, qlik_datasets: Optional[list[QlikDataset]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.qlik_datasets = qlik_datasets
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def qlik_apps(self) -> Optional[list[QlikApp]]:
+        return self.attributes.qlik_apps
+
+    @qlik_apps.setter
+    def qlik_apps(self, qlik_apps: Optional[list[QlikApp]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.qlik_apps = qlik_apps
 
     type_name: str = Field("QlikSpace", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "QlikSpace":
             raise ValueError("must be QlikSpace")
         return v
 
     class Attributes(Qlik.Attributes):
         qlik_space_type: Optional[str] = Field(
             None, description="", alias="qlikSpaceType"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
         qlik_datasets: Optional[list[QlikDataset]] = Field(
             None, description="", alias="qlikDatasets"
         )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
         qlik_apps: Optional[list[QlikApp]] = Field(
             None, description="", alias="qlikApps"
         )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "QlikSpace.Attributes" = Field(
-        None,
+        default_factory=lambda: QlikSpace.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class QlikApp(Qlik):
     """Description"""
@@ -20705,15 +18337,16 @@
 
     _convience_properties: ClassVar[list[str]] = [
         "qlik_has_section_access",
         "qlik_origin_app_id",
         "qlik_is_encrypted",
         "qlik_is_direct_query_mode",
         "qlik_app_static_byte_size",
-        "terms",
+        "qlik_space",
+        "qlik_sheets",
     ]
 
     @property
     def qlik_has_section_access(self) -> Optional[bool]:
         return self.attributes.qlik_has_section_access
 
     @qlik_has_section_access.setter
@@ -20759,24 +18392,32 @@
     @qlik_app_static_byte_size.setter
     def qlik_app_static_byte_size(self, qlik_app_static_byte_size: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.qlik_app_static_byte_size = qlik_app_static_byte_size
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def qlik_space(self) -> Optional[QlikSpace]:
+        return self.attributes.qlik_space
+
+    @qlik_space.setter
+    def qlik_space(self, qlik_space: Optional[QlikSpace]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.qlik_space = qlik_space
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def qlik_sheets(self) -> Optional[list[QlikSheet]]:
+        return self.attributes.qlik_sheets
+
+    @qlik_sheets.setter
+    def qlik_sheets(self, qlik_sheets: Optional[list[QlikSheet]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.qlik_sheets = qlik_sheets
 
     type_name: str = Field("QlikApp", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "QlikApp":
             raise ValueError("must be QlikApp")
@@ -20794,47 +18435,23 @@
         )
         qlik_is_direct_query_mode: Optional[bool] = Field(
             None, description="", alias="qlikIsDirectQueryMode"
         )
         qlik_app_static_byte_size: Optional[int] = Field(
             None, description="", alias="qlikAppStaticByteSize"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         qlik_space: Optional[QlikSpace] = Field(
             None, description="", alias="qlikSpace"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
         qlik_sheets: Optional[list[QlikSheet]] = Field(
             None, description="", alias="qlikSheets"
         )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "QlikApp.Attributes" = Field(
-        None,
+        default_factory=lambda: QlikApp.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class QlikChart(Qlik):
     """Description"""
@@ -20845,15 +18462,15 @@
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "qlik_chart_subtitle",
         "qlik_chart_footnote",
         "qlik_chart_orientation",
         "qlik_chart_type",
-        "terms",
+        "qlik_sheet",
     ]
 
     @property
     def qlik_chart_subtitle(self) -> Optional[str]:
         return self.attributes.qlik_chart_subtitle
 
     @qlik_chart_subtitle.setter
@@ -20889,24 +18506,22 @@
     @qlik_chart_type.setter
     def qlik_chart_type(self, qlik_chart_type: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.qlik_chart_type = qlik_chart_type
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+    def qlik_sheet(self) -> Optional[QlikSheet]:
+        return self.attributes.qlik_sheet
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @qlik_sheet.setter
+    def qlik_sheet(self, qlik_sheet: Optional[QlikSheet]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.qlik_sheet = qlik_sheet
 
     type_name: str = Field("QlikChart", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "QlikChart":
             raise ValueError("must be QlikChart")
@@ -20921,44 +18536,20 @@
         )
         qlik_chart_orientation: Optional[str] = Field(
             None, description="", alias="qlikChartOrientation"
         )
         qlik_chart_type: Optional[str] = Field(
             None, description="", alias="qlikChartType"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         qlik_sheet: Optional[QlikSheet] = Field(
             None, description="", alias="qlikSheet"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "QlikChart.Attributes" = Field(
-        None,
+        default_factory=lambda: QlikChart.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class QlikDataset(Qlik):
     """Description"""
@@ -20969,15 +18560,15 @@
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "qlik_dataset_technical_name",
         "qlik_dataset_type",
         "qlik_dataset_uri",
         "qlik_dataset_subtype",
-        "terms",
+        "qlik_space",
     ]
 
     @property
     def qlik_dataset_technical_name(self) -> Optional[str]:
         return self.attributes.qlik_dataset_technical_name
 
     @qlik_dataset_technical_name.setter
@@ -21013,24 +18604,22 @@
     @qlik_dataset_subtype.setter
     def qlik_dataset_subtype(self, qlik_dataset_subtype: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.qlik_dataset_subtype = qlik_dataset_subtype
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+    def qlik_space(self) -> Optional[QlikSpace]:
+        return self.attributes.qlik_space
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @qlik_space.setter
+    def qlik_space(self, qlik_space: Optional[QlikSpace]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.qlik_space = qlik_space
 
     type_name: str = Field("QlikDataset", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "QlikDataset":
             raise ValueError("must be QlikDataset")
@@ -21045,44 +18634,20 @@
         )
         qlik_dataset_uri: Optional[str] = Field(
             None, description="", alias="qlikDatasetUri"
         )
         qlik_dataset_subtype: Optional[str] = Field(
             None, description="", alias="qlikDatasetSubtype"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         qlik_space: Optional[QlikSpace] = Field(
             None, description="", alias="qlikSpace"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "QlikDataset.Attributes" = Field(
-        None,
+        default_factory=lambda: QlikDataset.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class QlikSheet(Qlik):
     """Description"""
@@ -21090,38 +18655,47 @@
     def __setattr__(self, name, value):
         if name in QlikSheet._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "qlik_sheet_is_approved",
-        "terms",
+        "qlik_app",
+        "qlik_charts",
     ]
 
     @property
     def qlik_sheet_is_approved(self) -> Optional[bool]:
         return self.attributes.qlik_sheet_is_approved
 
     @qlik_sheet_is_approved.setter
     def qlik_sheet_is_approved(self, qlik_sheet_is_approved: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.qlik_sheet_is_approved = qlik_sheet_is_approved
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def qlik_app(self) -> Optional[QlikApp]:
+        return self.attributes.qlik_app
+
+    @qlik_app.setter
+    def qlik_app(self, qlik_app: Optional[QlikApp]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.qlik_app = qlik_app
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def qlik_charts(self) -> Optional[list[QlikChart]]:
+        return self.attributes.qlik_charts
+
+    @qlik_charts.setter
+    def qlik_charts(self, qlik_charts: Optional[list[QlikChart]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.qlik_charts = qlik_charts
 
     type_name: str = Field("QlikSheet", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "QlikSheet":
             raise ValueError("must be QlikSheet")
@@ -21130,44 +18704,20 @@
     class Attributes(Qlik.Attributes):
         qlik_sheet_is_approved: Optional[bool] = Field(
             None, description="", alias="qlikSheetIsApproved"
         )
         qlik_app: Optional[QlikApp] = Field(
             None, description="", alias="qlikApp"
         )  # relationship
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         qlik_charts: Optional[list[QlikChart]] = Field(
             None, description="", alias="qlikCharts"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "QlikSheet.Attributes" = Field(
-        None,
+        default_factory=lambda: QlikSheet.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class TableauWorkbook(Tableau):
     """Description"""
@@ -21179,15 +18729,18 @@
 
     _convience_properties: ClassVar[list[str]] = [
         "site_qualified_name",
         "project_qualified_name",
         "top_level_project_name",
         "top_level_project_qualified_name",
         "project_hierarchy",
-        "terms",
+        "project",
+        "dashboards",
+        "worksheets",
+        "datasources",
     ]
 
     @property
     def site_qualified_name(self) -> Optional[str]:
         return self.attributes.site_qualified_name
 
     @site_qualified_name.setter
@@ -21237,24 +18790,52 @@
     @project_hierarchy.setter
     def project_hierarchy(self, project_hierarchy: Optional[list[dict[str, str]]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.project_hierarchy = project_hierarchy
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def project(self) -> Optional[TableauProject]:
+        return self.attributes.project
+
+    @project.setter
+    def project(self, project: Optional[TableauProject]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.project = project
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def dashboards(self) -> Optional[list[TableauDashboard]]:
+        return self.attributes.dashboards
+
+    @dashboards.setter
+    def dashboards(self, dashboards: Optional[list[TableauDashboard]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.dashboards = dashboards
+
+    @property
+    def worksheets(self) -> Optional[list[TableauWorksheet]]:
+        return self.attributes.worksheets
+
+    @worksheets.setter
+    def worksheets(self, worksheets: Optional[list[TableauWorksheet]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.worksheets = worksheets
+
+    @property
+    def datasources(self) -> Optional[list[TableauDatasource]]:
+        return self.attributes.datasources
+
+    @datasources.setter
+    def datasources(self, datasources: Optional[list[TableauDatasource]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.datasources = datasources
 
     type_name: str = Field("TableauWorkbook", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "TableauWorkbook":
             raise ValueError("must be TableauWorkbook")
@@ -21272,53 +18853,29 @@
         )
         top_level_project_qualified_name: Optional[str] = Field(
             None, description="", alias="topLevelProjectQualifiedName"
         )
         project_hierarchy: Optional[list[dict[str, str]]] = Field(
             None, description="", alias="projectHierarchy"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        worksheets: Optional[list[TableauWorksheet]] = Field(
-            None, description="", alias="worksheets"
-        )  # relationship
-        datasources: Optional[list[TableauDatasource]] = Field(
-            None, description="", alias="datasources"
-        )  # relationship
         project: Optional[TableauProject] = Field(
             None, description="", alias="project"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
         dashboards: Optional[list[TableauDashboard]] = Field(
             None, description="", alias="dashboards"
         )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
+        worksheets: Optional[list[TableauWorksheet]] = Field(
+            None, description="", alias="worksheets"
         )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
+        datasources: Optional[list[TableauDatasource]] = Field(
+            None, description="", alias="datasources"
         )  # relationship
 
     attributes: "TableauWorkbook.Attributes" = Field(
-        None,
+        default_factory=lambda: TableauWorkbook.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class TableauDatasourceField(Tableau):
     """Description"""
@@ -21341,15 +18898,16 @@
         "tableau_datasource_field_data_type",
         "upstream_tables",
         "tableau_datasource_field_formula",
         "tableau_datasource_field_bin_size",
         "upstream_columns",
         "upstream_fields",
         "datasource_field_type",
-        "terms",
+        "worksheets",
+        "datasource",
     ]
 
     @property
     def site_qualified_name(self) -> Optional[str]:
         return self.attributes.site_qualified_name
 
     @site_qualified_name.setter
@@ -21527,24 +19085,32 @@
     @datasource_field_type.setter
     def datasource_field_type(self, datasource_field_type: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.datasource_field_type = datasource_field_type
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def worksheets(self) -> Optional[list[TableauWorksheet]]:
+        return self.attributes.worksheets
+
+    @worksheets.setter
+    def worksheets(self, worksheets: Optional[list[TableauWorksheet]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.worksheets = worksheets
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def datasource(self) -> Optional[TableauDatasource]:
+        return self.attributes.datasource
+
+    @datasource.setter
+    def datasource(self, datasource: Optional[TableauDatasource]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.datasource = datasource
 
     type_name: str = Field("TableauDatasourceField", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "TableauDatasourceField":
             raise ValueError("must be TableauDatasourceField")
@@ -21595,47 +19161,23 @@
         )
         upstream_fields: Optional[list[dict[str, str]]] = Field(
             None, description="", alias="upstreamFields"
         )
         datasource_field_type: Optional[str] = Field(
             None, description="", alias="datasourceFieldType"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         worksheets: Optional[list[TableauWorksheet]] = Field(
             None, description="", alias="worksheets"
         )  # relationship
         datasource: Optional[TableauDatasource] = Field(
             None, description="", alias="datasource"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "TableauDatasourceField.Attributes" = Field(
-        None,
+        default_factory=lambda: TableauDatasourceField.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class TableauCalculatedField(Tableau):
     """Description"""
@@ -21653,15 +19195,16 @@
         "datasource_qualified_name",
         "project_hierarchy",
         "data_category",
         "role",
         "tableau_data_type",
         "formula",
         "upstream_fields",
-        "terms",
+        "worksheets",
+        "datasource",
     ]
 
     @property
     def site_qualified_name(self) -> Optional[str]:
         return self.attributes.site_qualified_name
 
     @site_qualified_name.setter
@@ -21771,24 +19314,32 @@
     @upstream_fields.setter
     def upstream_fields(self, upstream_fields: Optional[list[dict[str, str]]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.upstream_fields = upstream_fields
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def worksheets(self) -> Optional[list[TableauWorksheet]]:
+        return self.attributes.worksheets
+
+    @worksheets.setter
+    def worksheets(self, worksheets: Optional[list[TableauWorksheet]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.worksheets = worksheets
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def datasource(self) -> Optional[TableauDatasource]:
+        return self.attributes.datasource
+
+    @datasource.setter
+    def datasource(self, datasource: Optional[TableauDatasource]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.datasource = datasource
 
     type_name: str = Field("TableauCalculatedField", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "TableauCalculatedField":
             raise ValueError("must be TableauCalculatedField")
@@ -21818,47 +19369,23 @@
         tableau_data_type: Optional[str] = Field(
             None, description="", alias="tableauDataType"
         )
         formula: Optional[str] = Field(None, description="", alias="formula")
         upstream_fields: Optional[list[dict[str, str]]] = Field(
             None, description="", alias="upstreamFields"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         worksheets: Optional[list[TableauWorksheet]] = Field(
             None, description="", alias="worksheets"
         )  # relationship
         datasource: Optional[TableauDatasource] = Field(
             None, description="", alias="datasource"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "TableauCalculatedField.Attributes" = Field(
-        None,
+        default_factory=lambda: TableauCalculatedField.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class TableauProject(Tableau):
     """Description"""
@@ -21869,15 +19396,20 @@
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "site_qualified_name",
         "top_level_project_qualified_name",
         "is_top_level_project",
         "project_hierarchy",
-        "terms",
+        "parent_project",
+        "workbooks",
+        "site",
+        "datasources",
+        "flows",
+        "child_projects",
     ]
 
     @property
     def site_qualified_name(self) -> Optional[str]:
         return self.attributes.site_qualified_name
 
     @site_qualified_name.setter
@@ -21917,24 +19449,72 @@
     @project_hierarchy.setter
     def project_hierarchy(self, project_hierarchy: Optional[list[dict[str, str]]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.project_hierarchy = project_hierarchy
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def parent_project(self) -> Optional[TableauProject]:
+        return self.attributes.parent_project
+
+    @parent_project.setter
+    def parent_project(self, parent_project: Optional[TableauProject]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.parent_project = parent_project
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def workbooks(self) -> Optional[list[TableauWorkbook]]:
+        return self.attributes.workbooks
+
+    @workbooks.setter
+    def workbooks(self, workbooks: Optional[list[TableauWorkbook]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.workbooks = workbooks
+
+    @property
+    def site(self) -> Optional[TableauSite]:
+        return self.attributes.site
+
+    @site.setter
+    def site(self, site: Optional[TableauSite]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.site = site
+
+    @property
+    def datasources(self) -> Optional[list[TableauDatasource]]:
+        return self.attributes.datasources
+
+    @datasources.setter
+    def datasources(self, datasources: Optional[list[TableauDatasource]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.datasources = datasources
+
+    @property
+    def flows(self) -> Optional[list[TableauFlow]]:
+        return self.attributes.flows
+
+    @flows.setter
+    def flows(self, flows: Optional[list[TableauFlow]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.flows = flows
+
+    @property
+    def child_projects(self) -> Optional[list[TableauProject]]:
+        return self.attributes.child_projects
+
+    @child_projects.setter
+    def child_projects(self, child_projects: Optional[list[TableauProject]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.child_projects = child_projects
 
     type_name: str = Field("TableauProject", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "TableauProject":
             raise ValueError("must be TableauProject")
@@ -21949,59 +19529,35 @@
         )
         is_top_level_project: Optional[bool] = Field(
             None, description="", alias="isTopLevelProject"
         )
         project_hierarchy: Optional[list[dict[str, str]]] = Field(
             None, description="", alias="projectHierarchy"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
         parent_project: Optional[TableauProject] = Field(
             None, description="", alias="parentProject"
         )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
         workbooks: Optional[list[TableauWorkbook]] = Field(
             None, description="", alias="workbooks"
         )  # relationship
         site: Optional[TableauSite] = Field(
             None, description="", alias="site"
         )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         datasources: Optional[list[TableauDatasource]] = Field(
             None, description="", alias="datasources"
         )  # relationship
         flows: Optional[list[TableauFlow]] = Field(
             None, description="", alias="flows"
         )  # relationship
         child_projects: Optional[list[TableauProject]] = Field(
             None, description="", alias="childProjects"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "TableauProject.Attributes" = Field(
-        None,
+        default_factory=lambda: TableauProject.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class TableauMetric(Tableau):
     """Description"""
@@ -22012,15 +19568,15 @@
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "site_qualified_name",
         "project_qualified_name",
         "top_level_project_qualified_name",
         "project_hierarchy",
-        "terms",
+        "project",
     ]
 
     @property
     def site_qualified_name(self) -> Optional[str]:
         return self.attributes.site_qualified_name
 
     @site_qualified_name.setter
@@ -22060,24 +19616,22 @@
     @project_hierarchy.setter
     def project_hierarchy(self, project_hierarchy: Optional[list[dict[str, str]]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.project_hierarchy = project_hierarchy
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+    def project(self) -> Optional[TableauProject]:
+        return self.attributes.project
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @project.setter
+    def project(self, project: Optional[TableauProject]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.project = project
 
     type_name: str = Field("TableauMetric", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "TableauMetric":
             raise ValueError("must be TableauMetric")
@@ -22092,112 +19646,62 @@
         )
         top_level_project_qualified_name: Optional[str] = Field(
             None, description="", alias="topLevelProjectQualifiedName"
         )
         project_hierarchy: Optional[list[dict[str, str]]] = Field(
             None, description="", alias="projectHierarchy"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         project: Optional[TableauProject] = Field(
             None, description="", alias="project"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "TableauMetric.Attributes" = Field(
-        None,
+        default_factory=lambda: TableauMetric.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class TableauSite(Tableau):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in TableauSite._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
-        "terms",
+        "projects",
     ]
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+    def projects(self) -> Optional[list[TableauProject]]:
+        return self.attributes.projects
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @projects.setter
+    def projects(self, projects: Optional[list[TableauProject]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.projects = projects
 
     type_name: str = Field("TableauSite", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "TableauSite":
             raise ValueError("must be TableauSite")
         return v
 
     class Attributes(Tableau.Attributes):
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         projects: Optional[list[TableauProject]] = Field(
             None, description="", alias="projects"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "TableauSite.Attributes" = Field(
-        None,
+        default_factory=lambda: TableauSite.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class TableauDatasource(Tableau):
     """Description"""
@@ -22217,15 +19721,17 @@
         "has_extracts",
         "is_certified",
         "certifier",
         "certification_note",
         "certifier_display_name",
         "upstream_tables",
         "upstream_datasources",
-        "terms",
+        "workbook",
+        "project",
+        "fields",
     ]
 
     @property
     def site_qualified_name(self) -> Optional[str]:
         return self.attributes.site_qualified_name
 
     @site_qualified_name.setter
@@ -22357,24 +19863,42 @@
         self, upstream_datasources: Optional[list[dict[str, str]]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.upstream_datasources = upstream_datasources
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def workbook(self) -> Optional[TableauWorkbook]:
+        return self.attributes.workbook
+
+    @workbook.setter
+    def workbook(self, workbook: Optional[TableauWorkbook]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.workbook = workbook
+
+    @property
+    def project(self) -> Optional[TableauProject]:
+        return self.attributes.project
+
+    @project.setter
+    def project(self, project: Optional[TableauProject]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.project = project
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def fields(self) -> Optional[list[TableauDatasourceField]]:
+        return self.attributes.fields
+
+    @fields.setter
+    def fields(self, fields: Optional[list[TableauDatasourceField]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.fields = fields
 
     type_name: str = Field("TableauDatasource", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "TableauDatasource":
             raise ValueError("must be TableauDatasource")
@@ -22413,47 +19937,23 @@
         )
         upstream_datasources: Optional[list[dict[str, str]]] = Field(
             None, description="", alias="upstreamDatasources"
         )
         workbook: Optional[TableauWorkbook] = Field(
             None, description="", alias="workbook"
         )  # relationship
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         project: Optional[TableauProject] = Field(
             None, description="", alias="project"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
         fields: Optional[list[TableauDatasourceField]] = Field(
             None, description="", alias="fields"
         )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "TableauDatasource.Attributes" = Field(
-        None,
+        default_factory=lambda: TableauDatasource.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class TableauDashboard(Tableau):
     """Description"""
@@ -22465,15 +19965,16 @@
 
     _convience_properties: ClassVar[list[str]] = [
         "site_qualified_name",
         "project_qualified_name",
         "workbook_qualified_name",
         "top_level_project_qualified_name",
         "project_hierarchy",
-        "terms",
+        "workbook",
+        "worksheets",
     ]
 
     @property
     def site_qualified_name(self) -> Optional[str]:
         return self.attributes.site_qualified_name
 
     @site_qualified_name.setter
@@ -22523,24 +20024,32 @@
     @project_hierarchy.setter
     def project_hierarchy(self, project_hierarchy: Optional[list[dict[str, str]]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.project_hierarchy = project_hierarchy
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def workbook(self) -> Optional[TableauWorkbook]:
+        return self.attributes.workbook
+
+    @workbook.setter
+    def workbook(self, workbook: Optional[TableauWorkbook]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.workbook = workbook
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def worksheets(self) -> Optional[list[TableauWorksheet]]:
+        return self.attributes.worksheets
+
+    @worksheets.setter
+    def worksheets(self, worksheets: Optional[list[TableauWorksheet]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.worksheets = worksheets
 
     type_name: str = Field("TableauDashboard", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "TableauDashboard":
             raise ValueError("must be TableauDashboard")
@@ -22561,44 +20070,20 @@
         )
         project_hierarchy: Optional[list[dict[str, str]]] = Field(
             None, description="", alias="projectHierarchy"
         )
         workbook: Optional[TableauWorkbook] = Field(
             None, description="", alias="workbook"
         )  # relationship
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         worksheets: Optional[list[TableauWorksheet]] = Field(
             None, description="", alias="worksheets"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "TableauDashboard.Attributes" = Field(
-        None,
+        default_factory=lambda: TableauDashboard.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class TableauFlow(Tableau):
     """Description"""
@@ -22612,15 +20097,15 @@
         "site_qualified_name",
         "project_qualified_name",
         "top_level_project_qualified_name",
         "project_hierarchy",
         "input_fields",
         "output_fields",
         "output_steps",
-        "terms",
+        "project",
     ]
 
     @property
     def site_qualified_name(self) -> Optional[str]:
         return self.attributes.site_qualified_name
 
     @site_qualified_name.setter
@@ -22690,24 +20175,22 @@
     @output_steps.setter
     def output_steps(self, output_steps: Optional[list[dict[str, str]]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.output_steps = output_steps
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+    def project(self) -> Optional[TableauProject]:
+        return self.attributes.project
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @project.setter
+    def project(self, project: Optional[TableauProject]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.project = project
 
     type_name: str = Field("TableauFlow", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "TableauFlow":
             raise ValueError("must be TableauFlow")
@@ -22731,44 +20214,20 @@
         )
         output_fields: Optional[list[dict[str, str]]] = Field(
             None, description="", alias="outputFields"
         )
         output_steps: Optional[list[dict[str, str]]] = Field(
             None, description="", alias="outputSteps"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         project: Optional[TableauProject] = Field(
             None, description="", alias="project"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "TableauFlow.Attributes" = Field(
-        None,
+        default_factory=lambda: TableauFlow.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class TableauWorksheet(Tableau):
     """Description"""
@@ -22780,15 +20239,18 @@
 
     _convience_properties: ClassVar[list[str]] = [
         "site_qualified_name",
         "project_qualified_name",
         "top_level_project_qualified_name",
         "project_hierarchy",
         "workbook_qualified_name",
-        "terms",
+        "workbook",
+        "datasource_fields",
+        "calculated_fields",
+        "dashboards",
     ]
 
     @property
     def site_qualified_name(self) -> Optional[str]:
         return self.attributes.site_qualified_name
 
     @site_qualified_name.setter
@@ -22838,24 +20300,56 @@
     @workbook_qualified_name.setter
     def workbook_qualified_name(self, workbook_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.workbook_qualified_name = workbook_qualified_name
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def workbook(self) -> Optional[TableauWorkbook]:
+        return self.attributes.workbook
+
+    @workbook.setter
+    def workbook(self, workbook: Optional[TableauWorkbook]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.workbook = workbook
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def datasource_fields(self) -> Optional[list[TableauDatasourceField]]:
+        return self.attributes.datasource_fields
+
+    @datasource_fields.setter
+    def datasource_fields(
+        self, datasource_fields: Optional[list[TableauDatasourceField]]
+    ):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.datasource_fields = datasource_fields
+
+    @property
+    def calculated_fields(self) -> Optional[list[TableauCalculatedField]]:
+        return self.attributes.calculated_fields
+
+    @calculated_fields.setter
+    def calculated_fields(
+        self, calculated_fields: Optional[list[TableauCalculatedField]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.calculated_fields = calculated_fields
+
+    @property
+    def dashboards(self) -> Optional[list[TableauDashboard]]:
+        return self.attributes.dashboards
+
+    @dashboards.setter
+    def dashboards(self, dashboards: Optional[list[TableauDashboard]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.dashboards = dashboards
 
     type_name: str = Field("TableauWorksheet", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "TableauWorksheet":
             raise ValueError("must be TableauWorksheet")
@@ -22876,50 +20370,26 @@
         )
         workbook_qualified_name: Optional[str] = Field(
             None, description="", alias="workbookQualifiedName"
         )
         workbook: Optional[TableauWorkbook] = Field(
             None, description="", alias="workbook"
         )  # relationship
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         datasource_fields: Optional[list[TableauDatasourceField]] = Field(
             None, description="", alias="datasourceFields"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
         calculated_fields: Optional[list[TableauCalculatedField]] = Field(
             None, description="", alias="calculatedFields"
         )  # relationship
         dashboards: Optional[list[TableauDashboard]] = Field(
             None, description="", alias="dashboards"
         )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "TableauWorksheet.Attributes" = Field(
-        None,
+        default_factory=lambda: TableauWorksheet.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class LookerLook(Looker):
     """Description"""
@@ -22935,15 +20405,19 @@
         "source_view_count",
         "sourcelast_updater_id",
         "source_last_accessed_at",
         "source_last_viewed_at",
         "source_content_metadata_id",
         "source_query_id",
         "model_name",
-        "terms",
+        "query",
+        "folder",
+        "tile",
+        "model",
+        "dashboard",
     ]
 
     @property
     def folder_name(self) -> Optional[str]:
         return self.attributes.folder_name
 
     @folder_name.setter
@@ -23029,24 +20503,62 @@
     @model_name.setter
     def model_name(self, model_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.model_name = model_name
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def query(self) -> Optional[LookerQuery]:
+        return self.attributes.query
+
+    @query.setter
+    def query(self, query: Optional[LookerQuery]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.query = query
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def folder(self) -> Optional[LookerFolder]:
+        return self.attributes.folder
+
+    @folder.setter
+    def folder(self, folder: Optional[LookerFolder]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.folder = folder
+
+    @property
+    def tile(self) -> Optional[LookerTile]:
+        return self.attributes.tile
+
+    @tile.setter
+    def tile(self, tile: Optional[LookerTile]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.tile = tile
+
+    @property
+    def model(self) -> Optional[LookerModel]:
+        return self.attributes.model
+
+    @model.setter
+    def model(self, model: Optional[LookerModel]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.model = model
+
+    @property
+    def dashboard(self) -> Optional[LookerDashboard]:
+        return self.attributes.dashboard
+
+    @dashboard.setter
+    def dashboard(self, dashboard: Optional[LookerDashboard]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.dashboard = dashboard
 
     type_name: str = Field("LookerLook", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "LookerLook":
             raise ValueError("must be LookerLook")
@@ -23072,56 +20584,32 @@
         source_content_metadata_id: Optional[int] = Field(
             None, description="", alias="sourceContentMetadataId"
         )
         source_query_id: Optional[int] = Field(
             None, description="", alias="sourceQueryId"
         )
         model_name: Optional[str] = Field(None, description="", alias="modelName")
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
         query: Optional[LookerQuery] = Field(
             None, description="", alias="query"
         )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         folder: Optional[LookerFolder] = Field(
             None, description="", alias="folder"
         )  # relationship
         tile: Optional[LookerTile] = Field(
             None, description="", alias="tile"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
         model: Optional[LookerModel] = Field(
             None, description="", alias="model"
         )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
         dashboard: Optional[LookerDashboard] = Field(
             None, description="", alias="dashboard"
         )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "LookerLook.Attributes" = Field(
-        None,
+        default_factory=lambda: LookerLook.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class LookerDashboard(Looker):
     """Description"""
@@ -23135,15 +20623,17 @@
         "folder_name",
         "source_user_id",
         "source_view_count",
         "source_metadata_id",
         "sourcelast_updater_id",
         "source_last_accessed_at",
         "source_last_viewed_at",
-        "terms",
+        "tiles",
+        "looks",
+        "folder",
     ]
 
     @property
     def folder_name(self) -> Optional[str]:
         return self.attributes.folder_name
 
     @folder_name.setter
@@ -23209,24 +20699,42 @@
     @source_last_viewed_at.setter
     def source_last_viewed_at(self, source_last_viewed_at: Optional[datetime]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.source_last_viewed_at = source_last_viewed_at
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def tiles(self) -> Optional[list[LookerTile]]:
+        return self.attributes.tiles
+
+    @tiles.setter
+    def tiles(self, tiles: Optional[list[LookerTile]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.tiles = tiles
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def looks(self) -> Optional[list[LookerLook]]:
+        return self.attributes.looks
+
+    @looks.setter
+    def looks(self, looks: Optional[list[LookerLook]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.looks = looks
+
+    @property
+    def folder(self) -> Optional[LookerFolder]:
+        return self.attributes.folder
+
+    @folder.setter
+    def folder(self, folder: Optional[LookerFolder]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.folder = folder
 
     type_name: str = Field("LookerDashboard", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "LookerDashboard":
             raise ValueError("must be LookerDashboard")
@@ -23248,50 +20756,26 @@
         )
         source_last_accessed_at: Optional[datetime] = Field(
             None, description="", alias="sourceLastAccessedAt"
         )
         source_last_viewed_at: Optional[datetime] = Field(
             None, description="", alias="sourceLastViewedAt"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
         tiles: Optional[list[LookerTile]] = Field(
             None, description="", alias="tiles"
         )  # relationship
         looks: Optional[list[LookerLook]] = Field(
             None, description="", alias="looks"
         )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         folder: Optional[LookerFolder] = Field(
             None, description="", alias="folder"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "LookerDashboard.Attributes" = Field(
-        None,
+        default_factory=lambda: LookerDashboard.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class LookerFolder(Looker):
     """Description"""
@@ -23302,15 +20786,16 @@
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "source_content_metadata_id",
         "source_creator_id",
         "source_child_count",
         "source_parent_i_d",
-        "terms",
+        "looks",
+        "dashboards",
     ]
 
     @property
     def source_content_metadata_id(self) -> Optional[int]:
         return self.attributes.source_content_metadata_id
 
     @source_content_metadata_id.setter
@@ -23346,24 +20831,32 @@
     @source_parent_i_d.setter
     def source_parent_i_d(self, source_parent_i_d: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.source_parent_i_d = source_parent_i_d
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def looks(self) -> Optional[list[LookerLook]]:
+        return self.attributes.looks
+
+    @looks.setter
+    def looks(self, looks: Optional[list[LookerLook]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.looks = looks
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def dashboards(self) -> Optional[list[LookerDashboard]]:
+        return self.attributes.dashboards
+
+    @dashboards.setter
+    def dashboards(self, dashboards: Optional[list[LookerDashboard]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.dashboards = dashboards
 
     type_name: str = Field("LookerFolder", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "LookerFolder":
             raise ValueError("must be LookerFolder")
@@ -23378,47 +20871,23 @@
         )
         source_child_count: Optional[int] = Field(
             None, description="", alias="sourceChildCount"
         )
         source_parent_i_d: Optional[int] = Field(
             None, description="", alias="sourceParentID"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
         looks: Optional[list[LookerLook]] = Field(
             None, description="", alias="looks"
         )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
         dashboards: Optional[list[LookerDashboard]] = Field(
             None, description="", alias="dashboards"
         )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "LookerFolder.Attributes" = Field(
-        None,
+        default_factory=lambda: LookerFolder.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class LookerTile(Looker):
     """Description"""
@@ -23432,15 +20901,17 @@
         "lookml_link_id",
         "merge_result_id",
         "note_text",
         "query_i_d",
         "result_maker_i_d",
         "subtitle_text",
         "look_id",
-        "terms",
+        "query",
+        "look",
+        "dashboard",
     ]
 
     @property
     def lookml_link_id(self) -> Optional[str]:
         return self.attributes.lookml_link_id
 
     @lookml_link_id.setter
@@ -23506,24 +20977,42 @@
     @look_id.setter
     def look_id(self, look_id: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.look_id = look_id
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def query(self) -> Optional[LookerQuery]:
+        return self.attributes.query
+
+    @query.setter
+    def query(self, query: Optional[LookerQuery]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.query = query
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def look(self) -> Optional[LookerLook]:
+        return self.attributes.look
+
+    @look.setter
+    def look(self, look: Optional[LookerLook]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.look = look
+
+    @property
+    def dashboard(self) -> Optional[LookerDashboard]:
+        return self.attributes.dashboard
+
+    @dashboard.setter
+    def dashboard(self, dashboard: Optional[LookerDashboard]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.dashboard = dashboard
 
     type_name: str = Field("LookerTile", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "LookerTile":
             raise ValueError("must be LookerTile")
@@ -23539,50 +21028,26 @@
         note_text: Optional[str] = Field(None, description="", alias="noteText")
         query_i_d: Optional[int] = Field(None, description="", alias="queryID")
         result_maker_i_d: Optional[int] = Field(
             None, description="", alias="resultMakerID"
         )
         subtitle_text: Optional[str] = Field(None, description="", alias="subtitleText")
         look_id: Optional[int] = Field(None, description="", alias="lookId")
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         query: Optional[LookerQuery] = Field(
             None, description="", alias="query"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
         look: Optional[LookerLook] = Field(
             None, description="", alias="look"
         )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
         dashboard: Optional[LookerDashboard] = Field(
             None, description="", alias="dashboard"
         )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "LookerTile.Attributes" = Field(
-        None,
+        default_factory=lambda: LookerTile.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class LookerModel(Looker):
     """Description"""
@@ -23590,91 +21055,109 @@
     def __setattr__(self, name, value):
         if name in LookerModel._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "project_name",
-        "terms",
+        "explores",
+        "project",
+        "look",
+        "queries",
+        "fields",
     ]
 
     @property
     def project_name(self) -> Optional[str]:
         return self.attributes.project_name
 
     @project_name.setter
     def project_name(self, project_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.project_name = project_name
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def explores(self) -> Optional[list[LookerExplore]]:
+        return self.attributes.explores
+
+    @explores.setter
+    def explores(self, explores: Optional[list[LookerExplore]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.explores = explores
+
+    @property
+    def project(self) -> Optional[LookerProject]:
+        return self.attributes.project
+
+    @project.setter
+    def project(self, project: Optional[LookerProject]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.project = project
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def look(self) -> Optional[LookerLook]:
+        return self.attributes.look
+
+    @look.setter
+    def look(self, look: Optional[LookerLook]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.look = look
+
+    @property
+    def queries(self) -> Optional[list[LookerQuery]]:
+        return self.attributes.queries
+
+    @queries.setter
+    def queries(self, queries: Optional[list[LookerQuery]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.queries = queries
+
+    @property
+    def fields(self) -> Optional[list[LookerField]]:
+        return self.attributes.fields
+
+    @fields.setter
+    def fields(self, fields: Optional[list[LookerField]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.fields = fields
 
     type_name: str = Field("LookerModel", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "LookerModel":
             raise ValueError("must be LookerModel")
         return v
 
     class Attributes(Looker.Attributes):
         project_name: Optional[str] = Field(None, description="", alias="projectName")
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
         explores: Optional[list[LookerExplore]] = Field(
             None, description="", alias="explores"
         )  # relationship
         project: Optional[LookerProject] = Field(
             None, description="", alias="project"
         )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
         look: Optional[LookerLook] = Field(
             None, description="", alias="look"
         )  # relationship
         queries: Optional[list[LookerQuery]] = Field(
             None, description="", alias="queries"
         )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
         fields: Optional[list[LookerField]] = Field(
             None, description="", alias="fields"
         )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "LookerModel.Attributes" = Field(
-        None,
+        default_factory=lambda: LookerModel.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class LookerExplore(Looker):
     """Description"""
@@ -23686,15 +21169,17 @@
 
     _convience_properties: ClassVar[list[str]] = [
         "project_name",
         "model_name",
         "source_connection_name",
         "view_name",
         "sql_table_name",
-        "terms",
+        "project",
+        "model",
+        "fields",
     ]
 
     @property
     def project_name(self) -> Optional[str]:
         return self.attributes.project_name
 
     @project_name.setter
@@ -23740,24 +21225,42 @@
     @sql_table_name.setter
     def sql_table_name(self, sql_table_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sql_table_name = sql_table_name
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def project(self) -> Optional[LookerProject]:
+        return self.attributes.project
+
+    @project.setter
+    def project(self, project: Optional[LookerProject]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.project = project
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def model(self) -> Optional[LookerModel]:
+        return self.attributes.model
+
+    @model.setter
+    def model(self, model: Optional[LookerModel]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.model = model
+
+    @property
+    def fields(self) -> Optional[list[LookerField]]:
+        return self.attributes.fields
+
+    @fields.setter
+    def fields(self, fields: Optional[list[LookerField]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.fields = fields
 
     type_name: str = Field("LookerExplore", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "LookerExplore":
             raise ValueError("must be LookerExplore")
@@ -23769,127 +21272,110 @@
         source_connection_name: Optional[str] = Field(
             None, description="", alias="sourceConnectionName"
         )
         view_name: Optional[str] = Field(None, description="", alias="viewName")
         sql_table_name: Optional[str] = Field(
             None, description="", alias="sqlTableName"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         project: Optional[LookerProject] = Field(
             None, description="", alias="project"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
         model: Optional[LookerModel] = Field(
             None, description="", alias="model"
         )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
         fields: Optional[list[LookerField]] = Field(
             None, description="", alias="fields"
         )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "LookerExplore.Attributes" = Field(
-        None,
+        default_factory=lambda: LookerExplore.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class LookerProject(Looker):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in LookerProject._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
-        "terms",
+        "models",
+        "explores",
+        "fields",
+        "views",
     ]
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def models(self) -> Optional[list[LookerModel]]:
+        return self.attributes.models
+
+    @models.setter
+    def models(self, models: Optional[list[LookerModel]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.models = models
+
+    @property
+    def explores(self) -> Optional[list[LookerExplore]]:
+        return self.attributes.explores
+
+    @explores.setter
+    def explores(self, explores: Optional[list[LookerExplore]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.explores = explores
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def fields(self) -> Optional[list[LookerField]]:
+        return self.attributes.fields
+
+    @fields.setter
+    def fields(self, fields: Optional[list[LookerField]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.fields = fields
+
+    @property
+    def views(self) -> Optional[list[LookerView]]:
+        return self.attributes.views
+
+    @views.setter
+    def views(self, views: Optional[list[LookerView]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.views = views
 
     type_name: str = Field("LookerProject", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "LookerProject":
             raise ValueError("must be LookerProject")
         return v
 
     class Attributes(Looker.Attributes):
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
         models: Optional[list[LookerModel]] = Field(
             None, description="", alias="models"
         )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         explores: Optional[list[LookerExplore]] = Field(
             None, description="", alias="explores"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
         fields: Optional[list[LookerField]] = Field(
             None, description="", alias="fields"
         )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
         views: Optional[list[LookerView]] = Field(
             None, description="", alias="views"
         )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "LookerProject.Attributes" = Field(
-        None,
+        default_factory=lambda: LookerProject.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class LookerQuery(Looker):
     """Description"""
@@ -23900,15 +21386,17 @@
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "source_definition",
         "source_definition_database",
         "source_definition_schema",
         "fields",
-        "terms",
+        "tiles",
+        "looks",
+        "model",
     ]
 
     @property
     def source_definition(self) -> Optional[str]:
         return self.attributes.source_definition
 
     @source_definition.setter
@@ -23944,24 +21432,42 @@
     @fields.setter
     def fields(self, fields: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.fields = fields
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def tiles(self) -> Optional[list[LookerTile]]:
+        return self.attributes.tiles
+
+    @tiles.setter
+    def tiles(self, tiles: Optional[list[LookerTile]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.tiles = tiles
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def looks(self) -> Optional[list[LookerLook]]:
+        return self.attributes.looks
+
+    @looks.setter
+    def looks(self, looks: Optional[list[LookerLook]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.looks = looks
+
+    @property
+    def model(self) -> Optional[LookerModel]:
+        return self.attributes.model
+
+    @model.setter
+    def model(self, model: Optional[LookerModel]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.model = model
 
     type_name: str = Field("LookerQuery", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "LookerQuery":
             raise ValueError("must be LookerQuery")
@@ -23974,50 +21480,26 @@
         source_definition_database: Optional[str] = Field(
             None, description="", alias="sourceDefinitionDatabase"
         )
         source_definition_schema: Optional[str] = Field(
             None, description="", alias="sourceDefinitionSchema"
         )
         fields: Optional[set[str]] = Field(None, description="", alias="fields")
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
         tiles: Optional[list[LookerTile]] = Field(
             None, description="", alias="tiles"
         )  # relationship
         looks: Optional[list[LookerLook]] = Field(
             None, description="", alias="looks"
         )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
         model: Optional[LookerModel] = Field(
             None, description="", alias="model"
         )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "LookerQuery.Attributes" = Field(
-        None,
+        default_factory=lambda: LookerQuery.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class LookerField(Looker):
     """Description"""
@@ -24031,15 +21513,18 @@
         "project_name",
         "looker_explore_qualified_name",
         "looker_view_qualified_name",
         "model_name",
         "source_definition",
         "looker_field_data_type",
         "looker_times_used",
-        "terms",
+        "explore",
+        "project",
+        "view",
+        "model",
     ]
 
     @property
     def project_name(self) -> Optional[str]:
         return self.attributes.project_name
 
     @project_name.setter
@@ -24107,24 +21592,52 @@
     @looker_times_used.setter
     def looker_times_used(self, looker_times_used: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.looker_times_used = looker_times_used
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def explore(self) -> Optional[LookerExplore]:
+        return self.attributes.explore
+
+    @explore.setter
+    def explore(self, explore: Optional[LookerExplore]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.explore = explore
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def project(self) -> Optional[LookerProject]:
+        return self.attributes.project
+
+    @project.setter
+    def project(self, project: Optional[LookerProject]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.project = project
+
+    @property
+    def view(self) -> Optional[LookerView]:
+        return self.attributes.view
+
+    @view.setter
+    def view(self, view: Optional[LookerView]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.view = view
+
+    @property
+    def model(self) -> Optional[LookerModel]:
+        return self.attributes.model
+
+    @model.setter
+    def model(self, model: Optional[LookerModel]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.model = model
 
     type_name: str = Field("LookerField", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "LookerField":
             raise ValueError("must be LookerField")
@@ -24144,53 +21657,29 @@
         )
         looker_field_data_type: Optional[str] = Field(
             None, description="", alias="lookerFieldDataType"
         )
         looker_times_used: Optional[int] = Field(
             None, description="", alias="lookerTimesUsed"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        view: Optional[LookerView] = Field(
-            None, description="", alias="view"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         explore: Optional[LookerExplore] = Field(
             None, description="", alias="explore"
         )  # relationship
         project: Optional[LookerProject] = Field(
             None, description="", alias="project"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
+        view: Optional[LookerView] = Field(
+            None, description="", alias="view"
         )  # relationship
         model: Optional[LookerModel] = Field(
             None, description="", alias="model"
         )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "LookerField.Attributes" = Field(
-        None,
+        default_factory=lambda: LookerField.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class LookerView(Looker):
     """Description"""
@@ -24198,82 +21687,67 @@
     def __setattr__(self, name, value):
         if name in LookerView._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "project_name",
-        "terms",
+        "project",
+        "fields",
     ]
 
     @property
     def project_name(self) -> Optional[str]:
         return self.attributes.project_name
 
     @project_name.setter
     def project_name(self, project_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.project_name = project_name
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def project(self) -> Optional[LookerProject]:
+        return self.attributes.project
+
+    @project.setter
+    def project(self, project: Optional[LookerProject]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.project = project
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def fields(self) -> Optional[list[LookerField]]:
+        return self.attributes.fields
+
+    @fields.setter
+    def fields(self, fields: Optional[list[LookerField]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.fields = fields
 
     type_name: str = Field("LookerView", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "LookerView":
             raise ValueError("must be LookerView")
         return v
 
     class Attributes(Looker.Attributes):
         project_name: Optional[str] = Field(None, description="", alias="projectName")
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         project: Optional[LookerProject] = Field(
             None, description="", alias="project"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
         fields: Optional[list[LookerField]] = Field(
             None, description="", alias="fields"
         )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "LookerView.Attributes" = Field(
-        None,
+        default_factory=lambda: LookerView.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class RedashDashboard(Redash):
     """Description"""
@@ -24281,80 +21755,43 @@
     def __setattr__(self, name, value):
         if name in RedashDashboard._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "redash_dashboard_widget_count",
-        "terms",
     ]
 
     @property
     def redash_dashboard_widget_count(self) -> Optional[int]:
         return self.attributes.redash_dashboard_widget_count
 
     @redash_dashboard_widget_count.setter
     def redash_dashboard_widget_count(
         self, redash_dashboard_widget_count: Optional[int]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.redash_dashboard_widget_count = redash_dashboard_widget_count
 
-    @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
-
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.meanings = terms
-
     type_name: str = Field("RedashDashboard", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "RedashDashboard":
             raise ValueError("must be RedashDashboard")
         return v
 
     class Attributes(Redash.Attributes):
         redash_dashboard_widget_count: Optional[int] = Field(
             None, description="", alias="redashDashboardWidgetCount"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "RedashDashboard.Attributes" = Field(
-        None,
+        default_factory=lambda: RedashDashboard.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class RedashQuery(Redash):
     """Description"""
@@ -24367,15 +21804,15 @@
     _convience_properties: ClassVar[list[str]] = [
         "redash_query_s_q_l",
         "redash_query_parameters",
         "redash_query_schedule",
         "redash_query_last_execution_runtime",
         "redash_query_last_executed_at",
         "redash_query_schedule_humanized",
-        "terms",
+        "redash_visualizations",
     ]
 
     @property
     def redash_query_s_q_l(self) -> Optional[str]:
         return self.attributes.redash_query_s_q_l
 
     @redash_query_s_q_l.setter
@@ -24441,24 +21878,24 @@
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.redash_query_schedule_humanized = (
             redash_query_schedule_humanized
         )
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+    def redash_visualizations(self) -> Optional[list[RedashVisualization]]:
+        return self.attributes.redash_visualizations
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @redash_visualizations.setter
+    def redash_visualizations(
+        self, redash_visualizations: Optional[list[RedashVisualization]]
+    ):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.redash_visualizations = redash_visualizations
 
     type_name: str = Field("RedashQuery", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "RedashQuery":
             raise ValueError("must be RedashQuery")
@@ -24479,44 +21916,20 @@
         )
         redash_query_last_executed_at: Optional[datetime] = Field(
             None, description="", alias="redashQueryLastExecutedAt"
         )
         redash_query_schedule_humanized: Optional[str] = Field(
             None, description="", alias="redashQueryScheduleHumanized"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         redash_visualizations: Optional[list[RedashVisualization]] = Field(
             None, description="", alias="redashVisualizations"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "RedashQuery.Attributes" = Field(
-        None,
+        default_factory=lambda: RedashQuery.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class RedashVisualization(Redash):
     """Description"""
@@ -24526,15 +21939,15 @@
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "redash_visualization_type",
         "redash_query_name",
         "redash_query_qualified_name",
-        "terms",
+        "redash_query",
     ]
 
     @property
     def redash_visualization_type(self) -> Optional[str]:
         return self.attributes.redash_visualization_type
 
     @redash_visualization_type.setter
@@ -24560,24 +21973,22 @@
     @redash_query_qualified_name.setter
     def redash_query_qualified_name(self, redash_query_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.redash_query_qualified_name = redash_query_qualified_name
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+    def redash_query(self) -> Optional[RedashQuery]:
+        return self.attributes.redash_query
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @redash_query.setter
+    def redash_query(self, redash_query: Optional[RedashQuery]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.redash_query = redash_query
 
     type_name: str = Field("RedashVisualization", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "RedashVisualization":
             raise ValueError("must be RedashVisualization")
@@ -24589,44 +22000,20 @@
         )
         redash_query_name: Optional[str] = Field(
             None, description="", alias="redashQueryName"
         )
         redash_query_qualified_name: Optional[str] = Field(
             None, description="", alias="redashQueryQualifiedName"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
         redash_query: Optional[RedashQuery] = Field(
             None, description="", alias="redashQuery"
         )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "RedashVisualization.Attributes" = Field(
-        None,
+        default_factory=lambda: RedashVisualization.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class SalesforceObject(Salesforce):
     """Description"""
@@ -24637,15 +22024,17 @@
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "is_custom",
         "is_mergable",
         "is_queryable",
         "field_count",
-        "terms",
+        "organization",
+        "lookup_fields",
+        "fields",
     ]
 
     @property
     def is_custom(self) -> Optional[bool]:
         return self.attributes.is_custom
 
     @is_custom.setter
@@ -24681,74 +22070,68 @@
     @field_count.setter
     def field_count(self, field_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.field_count = field_count
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def organization(self) -> Optional[SalesforceOrganization]:
+        return self.attributes.organization
+
+    @organization.setter
+    def organization(self, organization: Optional[SalesforceOrganization]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.organization = organization
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def lookup_fields(self) -> Optional[list[SalesforceField]]:
+        return self.attributes.lookup_fields
+
+    @lookup_fields.setter
+    def lookup_fields(self, lookup_fields: Optional[list[SalesforceField]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.lookup_fields = lookup_fields
+
+    @property
+    def fields(self) -> Optional[list[SalesforceField]]:
+        return self.attributes.fields
+
+    @fields.setter
+    def fields(self, fields: Optional[list[SalesforceField]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.fields = fields
 
     type_name: str = Field("SalesforceObject", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "SalesforceObject":
             raise ValueError("must be SalesforceObject")
         return v
 
     class Attributes(Salesforce.Attributes):
         is_custom: Optional[bool] = Field(None, description="", alias="isCustom")
         is_mergable: Optional[bool] = Field(None, description="", alias="isMergable")
         is_queryable: Optional[bool] = Field(None, description="", alias="isQueryable")
         field_count: Optional[int] = Field(None, description="", alias="fieldCount")
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         organization: Optional[SalesforceOrganization] = Field(
             None, description="", alias="organization"
         )  # relationship
         lookup_fields: Optional[list[SalesforceField]] = Field(
             None, description="", alias="lookupFields"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
         fields: Optional[list[SalesforceField]] = Field(
             None, description="", alias="fields"
         )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "SalesforceObject.Attributes" = Field(
-        None,
+        default_factory=lambda: SalesforceObject.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class SalesforceField(Salesforce):
     """Description"""
@@ -24771,15 +22154,16 @@
         "is_nullable",
         "precision",
         "numeric_scale",
         "is_unique",
         "picklist_values",
         "is_polymorphic_foreign_key",
         "default_value_formula",
-        "terms",
+        "lookup_objects",
+        "object",
     ]
 
     @property
     def data_type(self) -> Optional[str]:
         return self.attributes.data_type
 
     @data_type.setter
@@ -24935,24 +22319,32 @@
     @default_value_formula.setter
     def default_value_formula(self, default_value_formula: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.default_value_formula = default_value_formula
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def lookup_objects(self) -> Optional[list[SalesforceObject]]:
+        return self.attributes.lookup_objects
+
+    @lookup_objects.setter
+    def lookup_objects(self, lookup_objects: Optional[list[SalesforceObject]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.lookup_objects = lookup_objects
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def object(self) -> Optional[SalesforceObject]:
+        return self.attributes.object
+
+    @object.setter
+    def object(self, object: Optional[SalesforceObject]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.object = object
 
     type_name: str = Field("SalesforceField", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "SalesforceField":
             raise ValueError("must be SalesforceField")
@@ -24987,47 +22379,23 @@
         )
         is_polymorphic_foreign_key: Optional[bool] = Field(
             None, description="", alias="isPolymorphicForeignKey"
         )
         default_value_formula: Optional[str] = Field(
             None, description="", alias="defaultValueFormula"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         lookup_objects: Optional[list[SalesforceObject]] = Field(
             None, description="", alias="lookupObjects"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
         object: Optional[SalesforceObject] = Field(
             None, description="", alias="object"
         )  # relationship
 
     attributes: "SalesforceField.Attributes" = Field(
-        None,
+        default_factory=lambda: SalesforceField.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class SalesforceOrganization(Salesforce):
     """Description"""
@@ -25035,85 +22403,81 @@
     def __setattr__(self, name, value):
         if name in SalesforceOrganization._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "source_id",
-        "terms",
+        "reports",
+        "objects",
+        "dashboards",
     ]
 
     @property
     def source_id(self) -> Optional[str]:
         return self.attributes.source_id
 
     @source_id.setter
     def source_id(self, source_id: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.source_id = source_id
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def reports(self) -> Optional[list[SalesforceReport]]:
+        return self.attributes.reports
+
+    @reports.setter
+    def reports(self, reports: Optional[list[SalesforceReport]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.reports = reports
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def objects(self) -> Optional[list[SalesforceObject]]:
+        return self.attributes.objects
+
+    @objects.setter
+    def objects(self, objects: Optional[list[SalesforceObject]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.objects = objects
+
+    @property
+    def dashboards(self) -> Optional[list[SalesforceDashboard]]:
+        return self.attributes.dashboards
+
+    @dashboards.setter
+    def dashboards(self, dashboards: Optional[list[SalesforceDashboard]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.dashboards = dashboards
 
     type_name: str = Field("SalesforceOrganization", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "SalesforceOrganization":
             raise ValueError("must be SalesforceOrganization")
         return v
 
     class Attributes(Salesforce.Attributes):
         source_id: Optional[str] = Field(None, description="", alias="sourceId")
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
         reports: Optional[list[SalesforceReport]] = Field(
             None, description="", alias="reports"
         )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         objects: Optional[list[SalesforceObject]] = Field(
             None, description="", alias="objects"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
         dashboards: Optional[list[SalesforceDashboard]] = Field(
             None, description="", alias="dashboards"
         )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "SalesforceOrganization.Attributes" = Field(
-        None,
+        default_factory=lambda: SalesforceOrganization.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class SalesforceDashboard(Salesforce):
     """Description"""
@@ -25123,15 +22487,16 @@
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "source_id",
         "dashboard_type",
         "report_count",
-        "terms",
+        "reports",
+        "organization",
     ]
 
     @property
     def source_id(self) -> Optional[str]:
         return self.attributes.source_id
 
     @source_id.setter
@@ -25157,24 +22522,32 @@
     @report_count.setter
     def report_count(self, report_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.report_count = report_count
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def reports(self) -> Optional[list[SalesforceReport]]:
+        return self.attributes.reports
+
+    @reports.setter
+    def reports(self, reports: Optional[list[SalesforceReport]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.reports = reports
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def organization(self) -> Optional[SalesforceOrganization]:
+        return self.attributes.organization
+
+    @organization.setter
+    def organization(self, organization: Optional[SalesforceOrganization]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.organization = organization
 
     type_name: str = Field("SalesforceDashboard", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "SalesforceDashboard":
             raise ValueError("must be SalesforceDashboard")
@@ -25182,47 +22555,23 @@
 
     class Attributes(Salesforce.Attributes):
         source_id: Optional[str] = Field(None, description="", alias="sourceId")
         dashboard_type: Optional[str] = Field(
             None, description="", alias="dashboardType"
         )
         report_count: Optional[int] = Field(None, description="", alias="reportCount")
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
         reports: Optional[list[SalesforceReport]] = Field(
             None, description="", alias="reports"
         )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         organization: Optional[SalesforceOrganization] = Field(
             None, description="", alias="organization"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "SalesforceDashboard.Attributes" = Field(
-        None,
+        default_factory=lambda: SalesforceDashboard.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class SalesforceReport(Salesforce):
     """Description"""
@@ -25232,15 +22581,16 @@
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "source_id",
         "report_type",
         "detail_columns",
-        "terms",
+        "organization",
+        "dashboards",
     ]
 
     @property
     def source_id(self) -> Optional[str]:
         return self.attributes.source_id
 
     @source_id.setter
@@ -25266,24 +22616,32 @@
     @detail_columns.setter
     def detail_columns(self, detail_columns: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.detail_columns = detail_columns
 
     @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
+    def organization(self) -> Optional[SalesforceOrganization]:
+        return self.attributes.organization
+
+    @organization.setter
+    def organization(self, organization: Optional[SalesforceOrganization]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
+        self.attributes.organization = organization
 
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
+    @property
+    def dashboards(self) -> Optional[list[SalesforceDashboard]]:
+        return self.attributes.dashboards
+
+    @dashboards.setter
+    def dashboards(self, dashboards: Optional[list[SalesforceDashboard]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+        self.attributes.dashboards = dashboards
 
     type_name: str = Field("SalesforceReport", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "SalesforceReport":
             raise ValueError("must be SalesforceReport")
@@ -25293,122 +22651,46 @@
         source_id: Optional[str] = Field(None, description="", alias="sourceId")
         report_type: Optional[dict[str, str]] = Field(
             None, description="", alias="reportType"
         )
         detail_columns: Optional[set[str]] = Field(
             None, description="", alias="detailColumns"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
         organization: Optional[SalesforceOrganization] = Field(
             None, description="", alias="organization"
         )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
         dashboards: Optional[list[SalesforceDashboard]] = Field(
             None, description="", alias="dashboards"
         )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "SalesforceReport.Attributes" = Field(
-        None,
+        default_factory=lambda: SalesforceReport.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class QlikStream(QlikSpace):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in QlikStream._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
-    _convience_properties: ClassVar[list[str]] = [
-        "terms",
-    ]
-
-    @property
-    def terms(self) -> list[AtlasGlossaryTerm]:
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        return [] if self.attributes.meanings is None else self.attributes.meanings
-
-    @terms.setter
-    def terms(self, terms: list[AtlasGlossaryTerm]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.meanings = terms
+    _convience_properties: ClassVar[list[str]] = []
 
     type_name: str = Field("QlikStream", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "QlikStream":
             raise ValueError("must be QlikStream")
         return v
 
-    class Attributes(QlikSpace.Attributes):
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        mc_monitors: Optional[list[MCMonitor]] = Field(
-            None, description="", alias="mcMonitors"
-        )  # relationship
-        qlik_datasets: Optional[list[QlikDataset]] = Field(
-            None, description="", alias="qlikDatasets"
-        )  # relationship
-        mc_incidents: Optional[list[MCIncident]] = Field(
-            None, description="", alias="mcIncidents"
-        )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        qlik_apps: Optional[list[QlikApp]] = Field(
-            None, description="", alias="qlikApps"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
-
-    attributes: "QlikStream.Attributes" = Field(
-        None,
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
 
 Referenceable.update_forward_refs()
 AtlasGlossary.update_forward_refs()
 
 Referenceable.Attributes.update_forward_refs()
 
 Asset.Attributes.update_forward_refs()
@@ -25525,14 +22807,16 @@
 
 DbtProcess.Attributes.update_forward_refs()
 
 ReadmeTemplate.Attributes.update_forward_refs()
 
 Readme.Attributes.update_forward_refs()
 
+File.Attributes.update_forward_refs()
+
 Link.Attributes.update_forward_refs()
 
 APISpec.Attributes.update_forward_refs()
 
 APIPath.Attributes.update_forward_refs()
 
 SnowflakeTag.Attributes.update_forward_refs()
```

### Comparing `pyatlan-0.0.32/pyatlan/model/core.py` & `pyatlan-0.0.33/pyatlan/model/core.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.32/pyatlan/model/enums.py` & `pyatlan-0.0.33/pyatlan/model/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -332,11 +332,23 @@
 class BadgeConditionColor(str, Enum):
     GREEN = "#047960"
     YELLOW = "#F7B43D"
     RED = "#BF1B1B"
     GREY = "#525C73"
 
 
+class FileType(str, Enum):
+    CSV = "csv"
+    DOC = "doc"
+    JSON = "json"
+    PDF = "pdf"
+    PPT = "ppt"
+    TXT = "txt"
+    XLS = "xls"
+    XML = "xml"
+    ZIP = "zip"
+
+
 class AtlanClassificationColor(str, Enum):
     GREEN = "Green"
     YELLOW = "Yellow"
     RED = "Red"
```

### Comparing `pyatlan-0.0.32/pyatlan/model/group.py` & `pyatlan-0.0.33/pyatlan/model/group.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     )
     user_count: Optional[int] = Field(description="Number of users in the group.")
 
     def is_default(self) -> bool:
         return (
             self.attributes is not None
             and self.attributes.is_default is not None
-            and self.attributes.is_default == "true"
+            and self.attributes.is_default == ["true"]
         )
 
     @staticmethod
     def create(
         alias: str,
     ) -> AtlanGroup:
         from pyatlan.model.assets import validate_required_fields
```

### Comparing `pyatlan-0.0.32/pyatlan/model/lineage.py` & `pyatlan-0.0.33/pyatlan/model/lineage.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.32/pyatlan/model/response.py` & `pyatlan-0.0.33/pyatlan/model/response.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.32/pyatlan/model/role.py` & `pyatlan-0.0.33/pyatlan/model/role.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.32/pyatlan/model/search.py` & `pyatlan-0.0.33/pyatlan/model/search.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.32/pyatlan/model/structs.py` & `pyatlan-0.0.33/pyatlan/model/structs.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.32/pyatlan/model/typedef.py` & `pyatlan-0.0.33/pyatlan/model/typedef.py`

 * *Files 0% similar despite different names*

```diff
@@ -248,15 +248,15 @@
         allow_filtering: bool = Field(
             description="Whether this attribute should appear in the filterable facets of discovery (true) or not "
             "(false).",
         )
         multi_value_select: bool = Field(
             description="Whether this attribute can have multiple values (true) or only a single value (false).",
         )
-        show_in_overview: bool = Field(
+        show_in_overview: Optional[bool] = Field(
             description="Whether users will see this attribute in the overview tab of the sidebar (true) or not "
             "(false).",
         )
         is_deprecated: Optional[str] = Field(
             description="Whether the attribute is deprecated ('true') or not (None or 'false')."
         )
         is_enum: Optional[bool] = Field(
```

### Comparing `pyatlan-0.0.32/pyatlan/utils.py` & `pyatlan-0.0.33/pyatlan/utils.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.32/pyatlan.egg-info/PKG-INFO` & `pyatlan-0.0.33/pyatlan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatlan
-Version: 0.0.32
+Version: 0.0.33
 Summary: Atlan Python Client
 Home-page: https://github.com/atlanhq/atlan-python
 Author: Atlan Technologies Pvt Ltd
 Author-email: engineering@atlan.com
 License: Apache LICENSE 2.0
 Keywords: atlan client
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyatlan-0.0.32/pyatlan.egg-info/SOURCES.txt` & `pyatlan-0.0.33/pyatlan.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 pyatlan.egg-info/top_level.txt
 pyatlan/cache/__init__.py
 pyatlan/cache/classification_cache.py
 pyatlan/cache/custom_metadata_cache.py
 pyatlan/cache/enum_cache.py
 pyatlan/cache/group_cache.py
 pyatlan/cache/role_cache.py
+pyatlan/cache/user_cache.py
 pyatlan/client/__init__.py
 pyatlan/client/atlan.py
 pyatlan/client/constants.py
 pyatlan/generator/__init__.py
 pyatlan/generator/generate_from_typdefs.py
 pyatlan/generator/templates/__init__.py
 pyatlan/model/__init__.py
@@ -34,14 +35,15 @@
 pyatlan/model/internal.py
 pyatlan/model/lineage.py
 pyatlan/model/response.py
 pyatlan/model/role.py
 pyatlan/model/search.py
 pyatlan/model/structs.py
 pyatlan/model/typedef.py
+pyatlan/model/user.py
 tests/__init__.py
 tests/conftest.py
 tests/integration/__init__.py
 tests/integration/admin_test.py
 tests/integration/classification_test.py
 tests/integration/client.py
 tests/integration/custom_metadata_test.py
```

### Comparing `pyatlan-0.0.32/setup.py` & `pyatlan-0.0.33/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import io
 import os
 
 from setuptools import find_packages, setup
 
 # External dependencies
-requirements = ["requests>=2.24", "pydantic>=1.10.4", "jinja2>=3.1.2"]
+requirements = ["requests>=2.24", "pydantic>=1.10.8", "jinja2>=3.1.2"]
 
 
 def read(file_name):
     """Read a text file and return the content as a string."""
     with io.open(
         os.path.join(os.path.dirname(__file__), file_name), encoding="utf-8"
     ) as f:
@@ -55,24 +55,25 @@
         "Operating System :: OS Independent",
         "Development Status :: 4 - Beta",
     ],
     packages=find_packages(),
     install_requires=requirements,
     extra_requires={
         "dev": [
-            "pytest>=7.2.0",
+            "pytest>=7.3.1",
             "flake8>=5.0.4",
             "mypy>=0.991",
             "black>=22.10.0",
-            "types-requests>=2.28.11.4",
+            "types-requests>=2.28.11.17",
             "pre-commit>=2.20.0",
             "deepdiff>=6.2.1",
             "pytest-cov>=4.0.0",
             "pytest-order==1.1.0",
             "retry==0.9.2",
+            "types-retry==0.9.9.3",
             "twine>=4.0.2",
         ]
     },
     include_package_data=True,
     zip_safe=False,
     keywords="atlan client",
     python_requires=">=3.9",
```

### Comparing `pyatlan-0.0.32/tests/integration/classification_test.py` & `pyatlan-0.0.33/tests/integration/classification_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.32/tests/integration/client.py` & `pyatlan-0.0.33/tests/integration/client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.32/tests/integration/custom_metadata_test.py` & `pyatlan-0.0.33/tests/integration/custom_metadata_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # SPDX-License-Identifier: Apache-2.0
 # Copyright 2022 Atlan Pte. Ltd.
 import logging
 import time
-from typing import Generator, List, Optional
+from typing import Generator, List, Optional, Tuple
 
 import pytest
 
 from pyatlan.cache.custom_metadata_cache import CustomMetadataCache
 from pyatlan.client.atlan import AtlanClient
 from pyatlan.error import NotFoundError
 from pyatlan.model.assets import (
@@ -19,18 +19,20 @@
 from pyatlan.model.core import CustomMetadata, to_snake_case
 from pyatlan.model.enums import (
     AtlanCustomAttributePrimitiveType,
     AtlanTypeCategory,
     BadgeComparisonOperator,
     BadgeConditionColor,
 )
+from pyatlan.model.group import AtlanGroup, CreateGroupResponse
 from pyatlan.model.search import DSL, Bool, Exists, IndexSearchRequest, Term
 from pyatlan.model.typedef import AttributeDef, CustomMetadataDef, EnumDef
 from tests.integration.client import delete_asset
 from tests.integration.glossary_test import create_glossary, create_term
+from tests.integration.admin_test import create_group, delete_group
 
 LOGGER = logging.getLogger(__name__)
 
 PREFIX = "psdk-"
 CM_PREFIX = f"{PREFIX}CM"
 FIXED_USER = "ernest"
 
@@ -75,16 +77,16 @@
     "Uniqueness",
 ]
 
 CM_ATTR_QUALITY_COUNT_RENAMED = to_snake_case(CM_ATTR_QUALITY_COUNT)
 CM_ATTR_QUALITY_SQL_RENAMED = to_snake_case(CM_ATTR_QUALITY_SQL)
 CM_ATTR_QUALITY_TYPE_RENAMED = to_snake_case(CM_ATTR_QUALITY_TYPE)
 
-GROUP_NAME1 = f"{PREFIX}1"
-GROUP_NAME2 = f"{PREFIX}2"
+GROUP_NAME1 = f"{CM_PREFIX}1"
+GROUP_NAME2 = f"{CM_PREFIX}2"
 
 _removal_epoch: Optional[int]
 
 
 def create_custom_metadata(
     client: AtlanClient,
     name: str,
@@ -354,31 +356,59 @@
     cm_dq: CustomMetadataDef,
 ) -> Generator[AtlasGlossaryTerm, None, None]:
     t = create_term(client, name=CM_PREFIX, glossary_guid=glossary.guid)
     yield t
     delete_asset(client, guid=t.guid, asset_type=AtlasGlossaryTerm)
 
 
-# TODO: create the groups, once they're modeled in the SDK...
-# @pytest.fixure
-# def groups(client: AtlanClient) -> Generator[List[], None, None]:
+@pytest.fixture(scope="module")
+def groups(
+    client: AtlanClient,
+    glossary: AtlasGlossary,
+    term: AtlasGlossaryTerm,
+    cm_raci: CustomMetadataDef,
+    cm_ipr: CustomMetadataDef,
+    cm_dq: CustomMetadataDef,
+) -> Generator[List[CreateGroupResponse], None, None]:
+    g1 = create_group(client, GROUP_NAME1)
+    g2 = create_group(client, GROUP_NAME2)
+    yield [g1, g2]
+    delete_group(client, g1.group)
+    delete_group(client, g2.group)
+
+
+def _get_groups(client: AtlanClient) -> Tuple[AtlanGroup, AtlanGroup]:
+    candidates = client.get_group_by_name(GROUP_NAME1)
+    assert candidates
+    assert len(candidates) == 1
+    group1 = candidates[0]
+    candidates = client.get_group_by_name(GROUP_NAME2)
+    assert candidates
+    assert len(candidates) == 1
+    group2 = candidates[0]
+    return group1, group2
 
 
 def test_add_term_cm_raci(
-    client: AtlanClient, cm_raci: CustomMetadataDef, term: AtlasGlossaryTerm
+    client: AtlanClient,
+    cm_raci: CustomMetadataDef,
+    term: AtlasGlossaryTerm,
+    groups: List[AtlanGroup],
 ):
     raci_attrs = term.get_custom_metadata(CM_RACI)
     _validate_raci_empty(raci_attrs)
+    group1, group2 = _get_groups(client)
     setattr(raci_attrs, CM_ATTR_RACI_RESPONSIBLE_RENAMED, [FIXED_USER])
     setattr(raci_attrs, CM_ATTR_RACI_ACCOUNTABLE_RENAMED, FIXED_USER)
-    # TODO: set Consulted and Informed once groups are available
+    setattr(raci_attrs, CM_ATTR_RACI_CONSULTED_RENAMED, [group1.name])
+    setattr(raci_attrs, CM_ATTR_RACI_INFORMED_RENAMED, [group1.name, group2.name])
     client.update_custom_metadata_attributes(term.guid, raci_attrs)
     t = client.retrieve_minimal(guid=term.guid, asset_type=AtlasGlossaryTerm)
     assert t
-    _validate_raci_attributes(t.get_custom_metadata(name=CM_RACI))
+    _validate_raci_attributes(client, t.get_custom_metadata(name=CM_RACI))
 
 
 def test_add_term_cm_ipr(
     client: AtlanClient, cm_ipr: CustomMetadataDef, term: AtlasGlossaryTerm
 ):
     ipr_attrs = term.get_custom_metadata(CM_IPR)
     _validate_ipr_empty(ipr_attrs)
@@ -418,43 +448,45 @@
     ipr = term.get_custom_metadata(CM_IPR)
     # Note: MUST access the getter / setter, not the underlying store
     setattr(ipr, CM_ATTR_IPR_MANDATORY_RENAMED, False)
     client.update_custom_metadata_attributes(term.guid, ipr)
     t = client.retrieve_minimal(guid=term.guid, asset_type=AtlasGlossaryTerm)
     assert t
     _validate_ipr_attributes(t.get_custom_metadata(name=CM_IPR), mandatory=False)
-    _validate_raci_attributes(t.get_custom_metadata(name=CM_RACI))
+    _validate_raci_attributes(client, t.get_custom_metadata(name=CM_RACI))
     _validate_dq_attributes(t.get_custom_metadata(name=CM_QUALITY))
 
 
 @pytest.mark.order(after="test_update_term_cm_ipr")
 def test_replace_term_cm_raci(
     client: AtlanClient, cm_raci: CustomMetadataDef, term: AtlasGlossaryTerm
 ):
     raci = term.get_custom_metadata(CM_RACI)
+    group1, group2 = _get_groups(client)
     # Note: MUST access the getter / setter, not the underlying store
-    setattr(raci, CM_ATTR_RACI_RESPONSIBLE_RENAMED, None)
+    setattr(raci, CM_ATTR_RACI_RESPONSIBLE_RENAMED, [FIXED_USER])
     setattr(raci, CM_ATTR_RACI_ACCOUNTABLE_RENAMED, FIXED_USER)
-    # TODO: replace consulted or informed (not yet defined, waiting on groups support)
+    setattr(raci, CM_ATTR_RACI_CONSULTED_RENAMED, None)
+    setattr(raci, CM_ATTR_RACI_INFORMED_RENAMED, [group1.name, group2.name])
     client.replace_custom_metadata(term.guid, raci)
     t = client.retrieve_minimal(guid=term.guid, asset_type=AtlasGlossaryTerm)
     assert t
-    _validate_raci_attributes_replacement(t.get_custom_metadata(name=CM_RACI))
+    _validate_raci_attributes_replacement(client, t.get_custom_metadata(name=CM_RACI))
     _validate_ipr_attributes(t.get_custom_metadata(name=CM_IPR), mandatory=False)
     _validate_dq_attributes(t.get_custom_metadata(name=CM_QUALITY))
 
 
 @pytest.mark.order(after="test_replace_term_cm_raci")
 def test_replace_term_cm_ipr(
     client: AtlanClient, cm_ipr: CustomMetadataDef, term: AtlasGlossaryTerm
 ):
     client.replace_custom_metadata(term.guid, term.get_custom_metadata(CM_IPR))
     t = client.retrieve_minimal(guid=term.guid, asset_type=AtlasGlossaryTerm)
     assert t
-    _validate_raci_attributes_replacement(t.get_custom_metadata(name=CM_RACI))
+    _validate_raci_attributes_replacement(client, t.get_custom_metadata(name=CM_RACI))
     _validate_dq_attributes(t.get_custom_metadata(name=CM_QUALITY))
     _validate_ipr_empty(t.get_custom_metadata(name=CM_IPR))
 
 
 @pytest.mark.order(after="test_replace_term_cm_ipr")
 def test_search_by_any_accountable(
     client: AtlanClient,
@@ -691,17 +723,19 @@
     glossary: AtlasGlossary,
     cm_raci: CustomMetadataDef,
     cm_ipr: CustomMetadataDef,
     cm_dq: CustomMetadataDef,
     client: AtlanClient,
 ):
     raci = term.get_custom_metadata(CM_RACI)
+    group1, group2 = _get_groups(client)
     setattr(raci, CM_ATTR_RACI_RESPONSIBLE_RENAMED, [FIXED_USER])
     setattr(raci, CM_ATTR_RACI_ACCOUNTABLE_RENAMED, FIXED_USER)
-    # TODO: set consulted and informed once groups are available
+    setattr(raci, CM_ATTR_RACI_CONSULTED_RENAMED, [group1.name])
+    setattr(raci, CM_ATTR_RACI_INFORMED_RENAMED, [group1.name, group2.name])
     setattr(raci, CM_ATTR_RACI_EXTRA_RENAMED, "something extra...")
     to_update = AtlasGlossaryTerm.create_for_modification(
         qualified_name=term.qualified_name, name=term.name, glossary_guid=glossary.guid
     )
     to_update.set_custom_metadata(custom_metadata=raci)
     response = client.upsert_replacing_cm(to_update, replace_classifications=False)
     assert response
@@ -715,15 +749,15 @@
     x = client.get_asset_by_qualified_name(
         qualified_name=term.qualified_name, asset_type=AtlasGlossaryTerm
     )
     assert x
     assert not x.is_incomplete
     assert x.qualified_name == term.qualified_name
     raci = x.get_custom_metadata(CM_RACI)
-    _validate_raci_attributes(raci)
+    _validate_raci_attributes(client, raci)
     assert getattr(raci, CM_ATTR_RACI_EXTRA_RENAMED) == "something extra..."
     _validate_ipr_empty(x.get_custom_metadata(CM_IPR))
     _validate_dq_empty(x.get_custom_metadata(CM_QUALITY))
 
 
 # TODO: test entity audit retrieval and parsing, once available
 
@@ -731,36 +765,45 @@
 def test_get_custom_metadata_when_name_is_invalid_then_raises_not_found_error():
     with pytest.raises(
         NotFoundError, match="Custom metadata with name Bogs does not exist"
     ):
         CustomMetadataCache.get_custom_metadata(name="Bogs", asset_type=Table)
 
 
-def _validate_raci_attributes(cma: CustomMetadata):
+def _validate_raci_attributes(client: AtlanClient, cma: CustomMetadata):
     assert cma
     # Note: MUST access the getter / setter, not the underlying store
     responsible = getattr(cma, CM_ATTR_RACI_RESPONSIBLE_RENAMED)
     accountable = getattr(cma, CM_ATTR_RACI_ACCOUNTABLE_RENAMED)
+    consulted = getattr(cma, CM_ATTR_RACI_CONSULTED_RENAMED)
+    informed = getattr(cma, CM_ATTR_RACI_INFORMED_RENAMED)
+    group1, group2 = _get_groups(client)
     assert responsible
     assert len(responsible) == 1
     assert FIXED_USER in responsible
     assert accountable
     assert accountable == FIXED_USER
-    # TODO: validate consulted and informed, once groups are included
+    assert consulted == [group1.name]
+    assert informed == [group1.name, group2.name]
 
 
-def _validate_raci_attributes_replacement(cma: CustomMetadata):
+def _validate_raci_attributes_replacement(client: AtlanClient, cma: CustomMetadata):
     assert cma
     # Note: MUST access the getter / setter, not the underlying store
     responsible = getattr(cma, CM_ATTR_RACI_RESPONSIBLE_RENAMED)
     accountable = getattr(cma, CM_ATTR_RACI_ACCOUNTABLE_RENAMED)
-    assert not responsible
+    consulted = getattr(cma, CM_ATTR_RACI_CONSULTED_RENAMED)
+    informed = getattr(cma, CM_ATTR_RACI_INFORMED_RENAMED)
+    group1, group2 = _get_groups(client)
+    assert responsible
+    assert responsible == [FIXED_USER]
     assert accountable
     assert accountable == FIXED_USER
-    # TODO: validate consulted and informed, once groups are included
+    assert not consulted
+    assert informed == [group1.name, group2.name]
 
 
 def _validate_raci_empty(raci_attrs: CustomMetadata):
     assert hasattr(raci_attrs, CM_ATTR_RACI_RESPONSIBLE_RENAMED)
     assert hasattr(raci_attrs, CM_ATTR_RACI_ACCOUNTABLE_RENAMED)
     assert hasattr(raci_attrs, CM_ATTR_RACI_CONSULTED_RENAMED)
     assert hasattr(raci_attrs, CM_ATTR_RACI_INFORMED_RENAMED)
```

### Comparing `pyatlan-0.0.32/tests/integration/glossary_test.py` & `pyatlan-0.0.33/tests/integration/glossary_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 # SPDX-License-Identifier: Apache-2.0
 # Copyright 2022 Atlan Pte. Ltd.
-from typing import Generator, Type
+import logging
+from typing import Generator
 
 import pytest
 from pydantic import StrictStr
 
 from pyatlan.client.atlan import AtlanClient
 from pyatlan.model.assets import AtlasGlossary, AtlasGlossaryTerm
-
-import logging
-
 from tests.integration.client import delete_asset
 
 LOGGER = logging.getLogger(__name__)
 
 PREFIX = "psdk-Glossary"
 
 GLOSSARY_NAME = f"{PREFIX} Traversable"
@@ -101,11 +99,10 @@
 ):
     g = client.get_asset_by_guid(glossary.guid, asset_type=AtlasGlossary)
     assert g
     assert isinstance(g, AtlasGlossary)
     assert g.guid == glossary.guid
     assert g.qualified_name == glossary.qualified_name
     assert g.name == glossary.name
-    # TODO: should we be able to flatten this to g.terms (?)
-    terms = g.attributes.terms
+    terms = g.terms
     assert terms
     assert len(terms) == 2
```

### Comparing `pyatlan-0.0.32/tests/integration/test_client.py` & `pyatlan-0.0.33/tests/integration/test_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -93,16 +93,17 @@
 
     assert (
         database := m_client.append_terms(
             guid=database.guid, asset_type=Database, terms=[term]
         )
     )
     database = m_client.get_asset_by_guid(guid=database.guid, asset_type=Database)
-    assert len(database.terms) == 1
-    assert database.terms[0].guid == term.guid
+    assert database.assigned_terms
+    assert len(database.assigned_terms) == 1
+    assert database.assigned_terms[0].guid == term.guid
 
 
 def test_append_terms_with_qualified_name(
     m_client: AtlanClient,
     make_term: Callable[[str], AtlasGlossaryTerm],
     database: Database,
 ):
@@ -110,16 +111,17 @@
 
     assert (
         database := m_client.append_terms(
             qualified_name=database.qualified_name, asset_type=Database, terms=[term]
         )
     )
     database = m_client.get_asset_by_guid(guid=database.guid, asset_type=Database)
-    assert len(database.terms) == 1
-    assert database.terms[0].guid == term.guid
+    assert database.assigned_terms
+    assert len(database.assigned_terms) == 1
+    assert database.assigned_terms[0].guid == term.guid
 
 
 def test_append_terms_using_ref_by_guid_for_term(
     m_client: AtlanClient,
     make_term: Callable[[str], AtlasGlossaryTerm],
     database: Database,
 ):
@@ -129,16 +131,17 @@
         database := m_client.append_terms(
             qualified_name=database.qualified_name,
             asset_type=Database,
             terms=[AtlasGlossaryTerm.ref_by_guid(guid=term.guid)],
         )
     )
     database = m_client.get_asset_by_guid(guid=database.guid, asset_type=Database)
-    assert len(database.terms) == 1
-    assert database.terms[0].guid == term.guid
+    assert database.assigned_terms
+    assert len(database.assigned_terms) == 1
+    assert database.assigned_terms[0].guid == term.guid
 
 
 def test_replace_a_term(
     m_client: AtlanClient,
     make_term: Callable[[str], AtlasGlossaryTerm],
     database: Database,
 ):
@@ -155,19 +158,24 @@
     assert (
         database := m_client.replace_terms(
             guid=database.guid, asset_type=Database, terms=[replacemant_term]
         )
     )
 
     database = m_client.get_asset_by_guid(guid=database.guid, asset_type=Database)
-    assert len(database.terms) == 2
-    deleted_terms = [t for t in database.terms if t.relationship_status == "DELETED"]
+    assert database.assigned_terms
+    assert len(database.assigned_terms) == 2
+    deleted_terms = [
+        t for t in database.assigned_terms if t.relationship_status == "DELETED"
+    ]
     assert len(deleted_terms) == 1
     assert deleted_terms[0].guid == original_term.guid
-    active_terms = [t for t in database.terms if t.relationship_status != "DELETED"]
+    active_terms = [
+        t for t in database.assigned_terms if t.relationship_status != "DELETED"
+    ]
     assert len(active_terms) == 1
     assert active_terms[0].guid == replacemant_term.guid
 
 
 def test_replace_all_term(
     m_client: AtlanClient,
     make_term: Callable[[str], AtlasGlossaryTerm],
@@ -185,16 +193,19 @@
     assert (
         database := m_client.replace_terms(
             guid=database.guid, asset_type=Database, terms=[]
         )
     )
 
     database = m_client.get_asset_by_guid(guid=database.guid, asset_type=Database)
-    assert len(database.terms) == 1
-    deleted_terms = [t for t in database.terms if t.relationship_status == "DELETED"]
+    assert database.assigned_terms
+    assert len(database.assigned_terms) == 1
+    deleted_terms = [
+        t for t in database.assigned_terms if t.relationship_status == "DELETED"
+    ]
     assert len(deleted_terms) == 1
     assert deleted_terms[0].guid == original_term.guid
 
 
 def test_remove_term(
     m_client: AtlanClient,
     make_term: Callable[[str], AtlasGlossaryTerm],
@@ -218,19 +229,24 @@
             guid=database.guid,
             asset_type=Database,
             terms=[AtlasGlossaryTerm.ref_by_guid(original_term.guid)],
         )
     )
 
     database = m_client.get_asset_by_guid(guid=database.guid, asset_type=Database)
-    assert len(database.terms) == 2
-    deleted_terms = [t for t in database.terms if t.relationship_status == "DELETED"]
+    assert database.assigned_terms
+    assert len(database.assigned_terms) == 2
+    deleted_terms = [
+        t for t in database.assigned_terms if t.relationship_status == "DELETED"
+    ]
     assert len(deleted_terms) == 1
     assert deleted_terms[0].guid == original_term.guid
-    active_terms = [t for t in database.terms if t.relationship_status != "DELETED"]
+    active_terms = [
+        t for t in database.assigned_terms if t.relationship_status != "DELETED"
+    ]
     assert active_terms[0].guid == another_term.guid
 
 
 def test_find_connections_by_name(m_client: AtlanClient):
     connections = m_client.find_connections_by_name(
         name="Test Connection",
         connector_type=AtlanConnectorType.SNOWFLAKE,
```

### Comparing `pyatlan-0.0.32/tests/integration/test_entity_model.py` & `pyatlan-0.0.33/tests/integration/test_entity_model.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.32/tests/integration/test_index_search.py` & `pyatlan-0.0.33/tests/integration/test_index_search.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.32/tests/unit/test_classification_name.py` & `pyatlan-0.0.33/tests/unit/test_classification_name.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.32/tests/unit/test_client.py` & `pyatlan-0.0.33/tests/unit/test_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import pytest
 
 from pyatlan.client.atlan import AtlanClient
 from pyatlan.model.assets import AtlasGlossaryTerm, Table
 
 
 @pytest.mark.parametrize(
-    "guid, qualified_name, asset_type, terms, message",
+    "guid, qualified_name, asset_type, assigned_terms, message",
     [
         (
             "123",
             None,
             Table,
             None,
             "1 validation error for AppendTerms\\nterms\\n  none is not an allowed value ",
@@ -41,25 +41,28 @@
         ),
     ],
 )
 def test_append_terms_with_invalid_parameter_raises_valueerror(
     guid,
     qualified_name,
     asset_type,
-    terms,
+    assigned_terms,
     message,
     monkeypatch,
 ):
     monkeypatch.setenv("ATLAN_BASE_URL", "https://name.atlan.com")
     monkeypatch.setenv("ATLAN_API_KEY", "abkj")
     client = AtlanClient()
 
     with pytest.raises(ValueError, match=message):
         client.append_terms(
-            guid=guid, qualified_name=qualified_name, asset_type=asset_type, terms=terms
+            guid=guid,
+            qualified_name=qualified_name,
+            asset_type=asset_type,
+            terms=assigned_terms,
         )
 
 
 def test_append_with_valid_guid_and_no_terms_returns_asset(monkeypatch):
     monkeypatch.setenv("ATLAN_BASE_URL", "https://name.atlan.com")
     monkeypatch.setenv("ATLAN_API_KEY", "abkj")
     asset_type = Table
@@ -93,15 +96,15 @@
         client = AtlanClient()
         guid = "123"
         terms = [AtlasGlossaryTerm()]
 
         assert (
             asset := client.append_terms(guid=guid, asset_type=asset_type, terms=terms)
         )
-        assert asset.terms == terms
+        assert asset.assigned_terms == terms
 
 
 def test_append_with_valid_guid_when_deleted_terms_present_returns_asset_with_given_terms(
     monkeypatch,
 ):
     monkeypatch.setenv("ATLAN_BASE_URL", "https://name.atlan.com")
     monkeypatch.setenv("ATLAN_API_KEY", "abkj")
@@ -118,15 +121,15 @@
         client = AtlanClient()
         guid = "123"
         terms = [AtlasGlossaryTerm()]
 
         assert (
             asset := client.append_terms(guid=guid, asset_type=asset_type, terms=terms)
         )
-        assert asset.terms == terms
+        assert asset.assigned_terms == terms
 
 
 def test_append_with_valid_guid_when_terms_present_returns_asset_with_combined_terms(
     monkeypatch,
 ):
     monkeypatch.setenv("ATLAN_BASE_URL", "https://name.atlan.com")
     monkeypatch.setenv("ATLAN_API_KEY", "abkj")
@@ -144,22 +147,22 @@
 
         new_term = AtlasGlossaryTerm()
         terms = [new_term]
 
         assert (
             asset := client.append_terms(guid=guid, asset_type=asset_type, terms=terms)
         )
-        assert (updated_terms := asset.terms)
+        assert (updated_terms := asset.assigned_terms)
         assert len(updated_terms) == 2
         assert exisiting_term in updated_terms
         assert new_term in updated_terms
 
 
 @pytest.mark.parametrize(
-    "guid, qualified_name, asset_type, terms, message",
+    "guid, qualified_name, asset_type, assigned_terms, message",
     [
         (
             None,
             None,
             Table,
             [AtlasGlossaryTerm()],
             "Either guid or qualified name must be specified",
@@ -187,25 +190,28 @@
         ),
     ],
 )
 def test_replace_terms_with_invalid_parameter_raises_valueerror(
     guid,
     qualified_name,
     asset_type,
-    terms,
+    assigned_terms,
     message,
     monkeypatch,
 ):
     monkeypatch.setenv("ATLAN_BASE_URL", "https://name.atlan.com")
     monkeypatch.setenv("ATLAN_API_KEY", "abkj")
     client = AtlanClient()
 
     with pytest.raises(ValueError, match=message):
         client.replace_terms(
-            guid=guid, qualified_name=qualified_name, asset_type=asset_type, terms=terms
+            guid=guid,
+            qualified_name=qualified_name,
+            asset_type=asset_type,
+            terms=assigned_terms,
         )
 
 
 def test_replace_terms(
     monkeypatch,
 ):
     monkeypatch.setenv("ATLAN_BASE_URL", "https://name.atlan.com")
@@ -220,19 +226,19 @@
         client = AtlanClient()
         guid = "123"
         terms = [AtlasGlossaryTerm()]
 
         assert (
             asset := client.replace_terms(guid=guid, asset_type=asset_type, terms=terms)
         )
-        assert asset.terms == terms
+        assert asset.assigned_terms == terms
 
 
 @pytest.mark.parametrize(
-    "guid, qualified_name, asset_type, terms, message",
+    "guid, qualified_name, asset_type, assigned_terms, message",
     [
         (
             None,
             None,
             Table,
             [AtlasGlossaryTerm()],
             "Either guid or qualified name must be specified",
@@ -259,33 +265,36 @@
             "1 validation error for RemoveTerms\\nterms\\n  none is not an allowed value ",
         ),
         (
             "123",
             None,
             Table,
             [],
-            "A list of terms to remove must be specified",
+            "A list of assigned_terms to remove must be specified",
         ),
     ],
 )
 def test_remove_terms_with_invalid_parameter_raises_valueerror(
     guid,
     qualified_name,
     asset_type,
-    terms,
+    assigned_terms,
     message,
     monkeypatch,
 ):
     monkeypatch.setenv("ATLAN_BASE_URL", "https://name.atlan.com")
     monkeypatch.setenv("ATLAN_API_KEY", "abkj")
     client = AtlanClient()
 
     with pytest.raises(ValueError, match=message):
         client.remove_terms(
-            guid=guid, qualified_name=qualified_name, asset_type=asset_type, terms=terms
+            guid=guid,
+            qualified_name=qualified_name,
+            asset_type=asset_type,
+            terms=assigned_terms,
         )
 
 
 def test_remove_with_valid_guid_when_terms_present_returns_asset_with_terms_removed(
     monkeypatch,
 ):
     monkeypatch.setenv("ATLAN_BASE_URL", "https://name.atlan.com")
@@ -306,10 +315,10 @@
         guid = "123"
 
         assert (
             asset := client.remove_terms(
                 guid=guid, asset_type=asset_type, terms=[exisiting_term]
             )
         )
-        assert (updated_terms := asset.terms)
+        assert (updated_terms := asset.assigned_terms)
         assert len(updated_terms) == 1
         assert other_term in updated_terms
```

### Comparing `pyatlan-0.0.32/tests/unit/test_glossary_term.py` & `pyatlan-0.0.33/tests/unit/test_glossary_term.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.32/tests/unit/test_lineage.py` & `pyatlan-0.0.33/tests/unit/test_lineage.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.32/tests/unit/test_model.py` & `pyatlan-0.0.33/tests/unit/test_model.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,41 +11,142 @@
 from deepdiff import DeepDiff
 from pydantic.error_wrappers import ValidationError
 
 import pyatlan.cache.classification_cache
 from pyatlan.cache.custom_metadata_cache import CustomMetadataCache
 from pyatlan.error import NotFoundError
 from pyatlan.model.assets import (
+    SQL,
+    ADLSAccount,
     ADLSAccountStatus,
+    ADLSContainer,
     ADLSEncryptionTypes,
+    ADLSObject,
     ADLSReplicationType,
+    APIPath,
+    APISpec,
     Asset,
     AtlasGlossary,
     AtlasGlossaryCategory,
     AtlasGlossaryTerm,
     AtlasServer,
     AwsTag,
     AzureTag,
     Badge,
     BadgeCondition,
     Catalog,
+    Column,
+    ColumnProcess,
     ColumnValueFrequencyMap,
     Connection,
     Database,
+    DbtMetric,
     DbtMetricFilter,
+    DbtModel,
+    DbtModelColumn,
+    DbtSource,
+    File,
+    Folder,
+    GCSBucket,
+    GCSObject,
     GoogleLabel,
     GoogleTag,
     Histogram,
+    Internal,
+    KafkaConsumerGroup,
+    KafkaTopic,
+    Link,
+    LookerDashboard,
+    LookerExplore,
+    LookerField,
+    LookerFolder,
+    LookerLook,
+    LookerModel,
+    LookerProject,
+    LookerQuery,
+    LookerTile,
+    LookerView,
+    MaterialisedView,
+    MCIncident,
+    MCMonitor,
+    MetabaseCollection,
+    MetabaseDashboard,
+    MetabaseQuestion,
+    Metric,
+    ModeChart,
+    ModeCollection,
+    ModeQuery,
+    ModeReport,
+    ModeWorkspace,
+    Namespace,
     PopularityInsights,
+    PowerBIColumn,
+    PowerBIDashboard,
+    PowerBIDataflow,
+    PowerBIDataset,
+    PowerBIDatasource,
+    PowerBIMeasure,
+    PowerBIPage,
+    PowerBIReport,
+    PowerBITable,
+    PowerBITile,
+    PowerBIWorkspace,
+    PresetChart,
+    PresetDashboard,
+    PresetDataset,
+    PresetWorkspace,
+    Procedure,
     Process,
+    QlikApp,
+    QlikChart,
+    QlikDataset,
+    QlikSheet,
+    QlikSpace,
+    Query,
+    QuickSightAnalysis,
+    QuickSightAnalysisVisual,
+    QuickSightDashboard,
+    QuickSightDashboardVisual,
+    QuickSightDataset,
+    QuickSightDatasetField,
+    QuickSightFolder,
     Readme,
+    RedashQuery,
+    RedashVisualization,
+    Referenceable,
     S3Bucket,
     S3Object,
+    SalesforceDashboard,
+    SalesforceField,
+    SalesforceObject,
+    SalesforceOrganization,
+    SalesforceReport,
     Schema,
+    SigmaDataElement,
+    SigmaDataElementField,
+    SigmaDataset,
+    SigmaDatasetColumn,
+    SigmaPage,
+    SigmaWorkbook,
+    SnowflakePipe,
+    SnowflakeStream,
+    SnowflakeTag,
     Table,
+    TableauCalculatedField,
+    TableauDashboard,
+    TableauDatasource,
+    TableauDatasourceField,
+    TableauFlow,
+    TableauProject,
+    TableauSite,
+    TableauWorkbook,
+    TableauWorksheet,
+    TablePartition,
+    ThoughtspotDashlet,
+    ThoughtspotLiveboard,
     View,
     validate_single_required_field,
 )
 from pyatlan.model.core import Announcement, AssetResponse
 from pyatlan.model.enums import (
     ADLSAccessTier,
     ADLSLeaseState,
@@ -56,14 +157,15 @@
     ADLSProvisionState,
     ADLSStorageKind,
     AnnouncementType,
     AtlanConnectorType,
     BadgeComparisonOperator,
     BadgeConditionColor,
     CertificateStatus,
+    FileType,
     GoogleDatastudioAssetType,
     IconType,
     KafkaTopicCompressionType,
     PowerbiEndorsement,
     QueryUsernameStrategy,
     QuickSightAnalysisStatus,
     QuickSightDatasetFieldType,
@@ -153,14 +255,167 @@
     "Optional[list[MCRuleComparison]]": [MCRuleComparison()],
     "Optional[QuickSightFolderType]": QuickSightFolderType.SHARED,
     "Optional[QuickSightDatasetFieldType]": QuickSightDatasetFieldType.STRING,
     "Optional[QuickSightAnalysisStatus]": QuickSightAnalysisStatus.CREATION_FAILED,
     "Optional[QuickSightDatasetImportMode]": QuickSightDatasetImportMode.SPICE,
     "Optional[list[KafkaTopicConsumption]]": [KafkaTopicConsumption()],
     "list[AtlasGlossaryTerm]": [AtlasGlossaryTerm()],
+    "Optional[list[AtlasGlossaryTerm]]": [AtlasGlossaryTerm()],
+    "Optional[list[AtlasGlossaryCategory]]": [AtlasGlossaryCategory()],
+    "Optional[list[File]]": [File()],
+    "Optional[list[Link]]": [Link()],
+    "Optional[list[MCIncident]]": [MCIncident()],
+    "Optional[list[MCMonitor]]": [MCMonitor()],
+    "Optional[list[Metric]]": [Metric()],
+    "Optional[Readme]": Readme(),
+    "AtlasGlossary": AtlasGlossary(),
+    "Optional[list[Referenceable]]": [Referenceable()],
+    "Optional[list[Process]]": [Process()],
+    "Optional[GCSBucket]": GCSBucket(),
+    "Optional[list[GCSObject]]": [GCSObject()],
+    "Optional[list[ColumnProcess]]": [ColumnProcess()],
+    "Optional[Process]": Process(),
+    "Optional[AtlasGlossaryCategory]": AtlasGlossaryCategory(),
+    "Optional[list[Folder]]": [Folder()],
+    "Optional[list[Query]]": [Query()],
+    "Namespace": Namespace(),
+    "Optional[list[KafkaConsumerGroup]]": [KafkaConsumerGroup()],
+    "Optional[list[KafkaTopic]]": [KafkaTopic()],
+    "Optional[list[ADLSContainer]]": [ADLSContainer()],
+    "Optional[ADLSAccount]": ADLSAccount(),
+    "Optional[list[ADLSObject]]": [ADLSObject()],
+    "Optional[ADLSContainer]": ADLSContainer(),
+    "Optional[list[S3Object]]": [S3Object()],
+    "Optional[S3Bucket]": S3Bucket(),
+    "Optional[list[Asset]]": [Asset()],
+    "Optional[MCMonitor]": MCMonitor(),
+    "Optional[list[Column]]": [Column()],
+    "Optional[Column]": Column(),
+    "Optional[MetabaseCollection]": MetabaseCollection(),
+    "Optional[list[MetabaseDashboard]]": [MetabaseDashboard()],
+    "Optional[list[MetabaseQuestion]]": [MetabaseQuestion()],
+    "Optional[list[QuickSightAnalysis]]": [QuickSightAnalysis()],
+    "Optional[list[QuickSightDashboard]]": [QuickSightDashboard()],
+    "Optional[list[QuickSightDataset]]": [QuickSightDataset()],
+    "Optional[QuickSightDataset]": QuickSightDataset(),
+    "Optional[list[QuickSightFolder]]": [QuickSightFolder()],
+    "Optional[list[QuickSightAnalysisVisual]]": [QuickSightAnalysisVisual()],
+    "Optional[list[QuickSightDashboardVisual]]": [QuickSightDashboardVisual()],
+    "Optional[list[QuickSightDatasetField]]": [QuickSightDatasetField()],
+    "Optional[QuickSightDashboard]": QuickSightDashboard(),
+    "Optional[QuickSightAnalysis]": QuickSightAnalysis(),
+    "Optional[list[ThoughtspotDashlet]]": [ThoughtspotDashlet()],
+    "Optional[ThoughtspotLiveboard]": ThoughtspotLiveboard(),
+    "Optional[PowerBIDataset]": PowerBIDataset(),
+    "Optional[list[PowerBIPage]]": [PowerBIPage()],
+    "Optional[list[PowerBITile]]": [PowerBITile()],
+    "Optional[PowerBIWorkspace]": PowerBIWorkspace(),
+    "Optional[PowerBITable]": PowerBITable(),
+    "Optional[list[PowerBIColumn]]": [PowerBIColumn()],
+    "Optional[list[PowerBIMeasure]]": [PowerBIMeasure()],
+    "Optional[PowerBIDashboard]": PowerBIDashboard(),
+    "Optional[PowerBIReport]": PowerBIReport(),
+    "Optional[list[PowerBIDataset]]": [PowerBIDataset()],
+    "Optional[list[PowerBIDashboard]]": [PowerBIDashboard()],
+    "Optional[list[PowerBIDataflow]]": [PowerBIDataflow()],
+    "Optional[list[PowerBIReport]]": [PowerBIReport()],
+    "Optional[list[PowerBIDatasource]]": [PowerBIDatasource()],
+    "Optional[list[PowerBITable]]": [PowerBITable()],
+    "Optional[PresetDashboard]": PresetDashboard(),
+    "Optional[list[PresetChart]]": [PresetChart()],
+    "Optional[list[PresetDataset]]": [PresetDataset()],
+    "Optional[PresetWorkspace]": PresetWorkspace(),
+    "Optional[list[PresetDashboard]]": [PresetDashboard()],
+    "Optional[list[ModeCollection]]": [ModeCollection()],
+    "Optional[list[ModeQuery]]": [ModeQuery()],
+    "Optional[list[ModeChart]]": [ModeChart()],
+    "Optional[ModeReport]": ModeReport(),
+    "Optional[ModeQuery]": ModeQuery(),
+    "Optional[list[ModeReport]]": [ModeReport()],
+    "Optional[ModeWorkspace]": ModeWorkspace(),
+    "Optional[SigmaDataset]": SigmaDataset(),
+    "Optional[list[SigmaDatasetColumn]]": [SigmaDatasetColumn()],
+    "Optional[list[SigmaPage]]": [SigmaPage()],
+    "Optional[SigmaDataElement]": SigmaDataElement(),
+    "Optional[list[SigmaDataElement]]": [SigmaDataElement()],
+    "Optional[SigmaWorkbook]": SigmaWorkbook(),
+    "Optional[list[SigmaDataElementField]]": [SigmaDataElementField()],
+    "Optional[SigmaPage]": SigmaPage(),
+    "Optional[list[QlikApp]]": [QlikApp()],
+    "Optional[list[QlikDataset]]": [QlikDataset()],
+    "Optional[list[QlikSheet]]": [QlikSheet()],
+    "Optional[QlikSpace]": QlikSpace(),
+    "Optional[QlikSheet]": QlikSheet(),
+    "Optional[QlikApp]": QlikApp(),
+    "Optional[list[QlikChart]]": [QlikChart()],
+    "Optional[list[TableauDashboard]]": [TableauDashboard()],
+    "Optional[list[TableauDatasource]]": [TableauDatasource()],
+    "Optional[TableauProject]": TableauProject(),
+    "Optional[list[TableauWorksheet]]": [TableauWorksheet()],
+    "Optional[TableauDatasource]": TableauDatasource(),
+    "Optional[list[TableauProject]]": [TableauProject()],
+    "Optional[list[TableauFlow]]": [TableauFlow()],
+    "Optional[TableauSite]": TableauSite(),
+    "Optional[list[TableauWorkbook]]": [TableauWorkbook()],
+    "Optional[list[TableauDatasourceField]]": [TableauDatasourceField()],
+    "Optional[TableauWorkbook]": TableauWorkbook(),
+    "Optional[list[TableauCalculatedField]]": [TableauCalculatedField()],
+    "Optional[LookerDashboard]": LookerDashboard(),
+    "Optional[LookerFolder]": LookerFolder(),
+    "Optional[LookerModel]": LookerModel(),
+    "Optional[LookerQuery]": LookerQuery(),
+    "Optional[LookerTile]": LookerTile(),
+    "Optional[list[LookerTile]]": [LookerTile()],
+    "Optional[list[LookerDashboard]]": [LookerDashboard()],
+    "Optional[list[LookerLook]]": [LookerLook()],
+    "Optional[LookerLook]": LookerLook(),
+    "Optional[list[LookerExplore]]": [LookerExplore()],
+    "Optional[list[LookerField]]": [LookerField()],
+    "Optional[LookerProject]": LookerProject(),
+    "Optional[list[LookerQuery]]": [LookerQuery()],
+    "Optional[list[LookerModel]]": [LookerModel()],
+    "Optional[list[LookerView]]": [LookerView()],
+    "Optional[LookerView]": LookerView(),
+    "Optional[LookerExplore]": LookerExplore(),
+    "Optional[list[RedashVisualization]]": [RedashVisualization()],
+    "Optional[RedashQuery]": RedashQuery(),
+    "Optional[list[SalesforceField]]": [SalesforceField()],
+    "Optional[SalesforceOrganization]": SalesforceOrganization(),
+    "Optional[list[SalesforceObject]]": [SalesforceObject()],
+    "Optional[SalesforceObject]": SalesforceObject(),
+    "Optional[list[SalesforceDashboard]]": [SalesforceDashboard()],
+    "Optional[list[SalesforceReport]]": [SalesforceReport()],
+    "Optional[DbtModel]": DbtModel(),
+    "Optional[list[DbtMetric]]": [DbtMetric()],
+    "Optional[list[DbtModelColumn]]": [DbtModelColumn()],
+    "Optional[list[SQL]]": [SQL()],
+    "Optional[SQL]": SQL(),
+    "Optional[Asset]": Asset(),
+    "Optional[Internal]": Internal(),
+    "Optional[list[Readme]]": [Readme()],
+    "Optional[FileType]": FileType.CSV,
+    "Optional[list[APIPath]]": [APIPath()],
+    "Optional[APISpec]": APISpec(),
+    "Optional[Schema]": Schema(),
+    "Optional[list[DbtModel]]": [DbtModel()],
+    "Optional[list[DbtSource]]": [DbtSource()],
+    "Optional[Table]": Table(),
+    "Optional[list[TablePartition]]": [TablePartition()],
+    "Optional[list[Table]]": [Table()],
+    "Optional[list[View]]": [View()],
+    "Optional[MaterialisedView]": MaterialisedView(),
+    "Optional[TablePartition]": TablePartition(),
+    "Optional[View]": View(),
+    "Optional[Database]": Database(),
+    "Optional[list[MaterialisedView]]": [MaterialisedView()],
+    "Optional[list[Procedure]]": [Procedure()],
+    "Optional[list[SnowflakePipe]]": [SnowflakePipe()],
+    "Optional[list[SnowflakeStream]]": [SnowflakeStream()],
+    "Optional[list[SnowflakeTag]]": [SnowflakeTag()],
+    "Optional[list[Schema]]": [Schema()],
 }
 
 
 def load_json(filename):
     with (DATA_DIR / filename).open() as input_file:
         return json.load(input_file)
 
@@ -1339,15 +1594,15 @@
     exec(
         f"ret_value = sut.{property_name}",
         {"sut": sut, "property_name": property_name},
         local_ns,
     )
     assert attribute_value == local_ns["ret_value"]
     exec(
-        f"ret_value = sut.attributes.{property_name if property_name != 'terms' else 'meanings'}",
+        f"ret_value = sut.attributes.{property_name if property_name != 'assigned_terms' else 'meanings'}",
         {"sut": sut, "property_name": property_name},
         local_ns,
     )
     assert attribute_value == local_ns["ret_value"]
 
 
 @pytest.mark.parametrize(
@@ -1386,21 +1641,14 @@
     [
         (None, "stuff", None, ValueError, "asset is required"),
         (table, None, None, ValueError, "content is required"),
         (
             Table(),
             "stuff",
             None,
-            AttributeError,
-            "'NoneType' object has no attribute 'name'",
-        ),
-        (
-            Table(attributes=Table.Attributes()),
-            "stuff",
-            None,
             ValueError,
             "asset_name is required when name is not available from asset",
         ),
     ],
 )
 def test_create_readme_attributes_without_required_parameters_raises_exception(
     asset, content, asset_name, error, message
@@ -1423,21 +1671,14 @@
             ValueError,
             "content is required",
         ),
         (
             Table(),
             "stuff",
             None,
-            AttributeError,
-            "'NoneType' object has no attribute 'name'",
-        ),
-        (
-            Table(attributes=Table.Attributes()),
-            "stuff",
-            None,
             ValueError,
             "asset_name is required when name is not available from asset",
         ),
     ],
 )
 def test_create_readme_without_required_parameters_raises_exception(
     asset, content, asset_name, error, message
```

### Comparing `pyatlan-0.0.32/tests/unit/test_search_model.py` & `pyatlan-0.0.33/tests/unit/test_search_model.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.32/tests/unit/test_typedef_model.py` & `pyatlan-0.0.33/tests/unit/test_typedef_model.py`

 * *Files identical despite different names*

