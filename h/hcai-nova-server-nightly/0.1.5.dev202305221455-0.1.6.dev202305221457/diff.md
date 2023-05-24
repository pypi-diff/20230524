# Comparing `tmp/hcai-nova-server-nightly-0.1.5.dev202305221455.tar.gz` & `tmp/hcai-nova-server-nightly-0.1.6.dev202305221457.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcai-nova-server-nightly-0.1.5.dev202305221455.tar", last modified: Mon May 22 14:55:43 2023, max compression
+gzip compressed data, was "hcai-nova-server-nightly-0.1.6.dev202305221457.tar", last modified: Mon May 22 14:57:07 2023, max compression
```

## Comparing `hcai-nova-server-nightly-0.1.5.dev202305221455.tar` & `hcai-nova-server-nightly-0.1.6.dev202305221457.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:55:43.559060 hcai-nova-server-nightly-0.1.5.dev202305221455/
--rw-r--r--   0 runner    (1001) docker     (122)      117 2023-05-22 14:55:33.000000 hcai-nova-server-nightly-0.1.5.dev202305221455/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1568 2023-05-22 14:55:43.559060 hcai-nova-server-nightly-0.1.5.dev202305221455/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      573 2023-05-22 14:55:33.000000 hcai-nova-server-nightly-0.1.5.dev202305221455/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:55:43.559060 hcai-nova-server-nightly-0.1.5.dev202305221455/hcai_nova_server_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1568 2023-05-22 14:55:43.000000 hcai-nova-server-nightly-0.1.5.dev202305221455/hcai_nova_server_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      944 2023-05-22 14:55:43.000000 hcai-nova-server-nightly-0.1.5.dev202305221455/hcai_nova_server_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-22 14:55:43.000000 hcai-nova-server-nightly-0.1.5.dev202305221455/hcai_nova_server_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       75 2023-05-22 14:55:43.000000 hcai-nova-server-nightly-0.1.5.dev202305221455/hcai_nova_server_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-22 14:55:43.000000 hcai-nova-server-nightly-0.1.5.dev202305221455/hcai_nova_server_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:55:43.559060 hcai-nova-server-nightly-0.1.5.dev202305221455/nova_server/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-22 14:55:33.000000 hcai-nova-server-nightly-0.1.5.dev202305221455/nova_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2568 2023-05-22 14:55:33.000000 hcai-nova-server-nightly-0.1.5.dev202305221455/nova_server/nova_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:55:43.559060 hcai-nova-server-nightly-0.1.5.dev202305221455/nova_server/route/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-22 14:55:33.000000 hcai-nova-server-nightly-0.1.5.dev202305221455/nova_server/route/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-05-22 14:55:33.000000 hcai-nova-server-nightly-0.1.5.dev202305221455/nova_server/route/cancel.py
--rw-r--r--   0 runner    (1001) docker     (122)    13062 2023-05-22 14:55:33.000000 hcai-nova-server-nightly-0.1.5.dev202305221455/nova_server/route/explain.py
--rw-r--r--   0 runner    (1001) docker     (122)     9891 2023-05-22 14:55:33.000000 hcai-nova-server-nightly-0.1.5.dev202305221455/nova_server/route/extract.py
--rw-r--r--   0 runner    (1001) docker     (122)      809 2023-05-22 14:55:33.000000 hcai-nova-server-nightly-0.1.5.dev202305221455/nova_server/route/log.py
--rw-r--r--   0 runner    (1001) docker     (122)     7040 2023-05-22 14:55:33.000000 hcai-nova-server-nightly-0.1.5.dev202305221455/nova_server/route/predict.py
--rw-r--r--   0 runner    (1001) docker     (122)      756 2023-05-22 14:55:33.000000 hcai-nova-server-nightly-0.1.5.dev202305221455/nova_server/route/status.py
--rw-r--r--   0 runner    (1001) docker     (122)     6075 2023-05-22 14:55:33.000000 hcai-nova-server-nightly-0.1.5.dev202305221455/nova_server/route/train.py
--rw-r--r--   0 runner    (1001) docker     (122)      351 2023-05-22 14:55:33.000000 hcai-nova-server-nightly-0.1.5.dev202305221455/nova_server/route/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:55:43.559060 hcai-nova-server-nightly-0.1.5.dev202305221455/nova_server/templates/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-22 14:55:33.000000 hcai-nova-server-nightly-0.1.5.dev202305221455/nova_server/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:55:43.559060 hcai-nova-server-nightly-0.1.5.dev202305221455/nova_server/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-22 14:55:33.000000 hcai-nova-server-nightly-0.1.5.dev202305221455/nova_server/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2254 2023-05-22 14:55:33.000000 hcai-nova-server-nightly-0.1.5.dev202305221455/nova_server/utils/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    12151 2023-05-22 14:55:33.000000 hcai-nova-server-nightly-0.1.5.dev202305221455/nova_server/utils/db_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1785 2023-05-22 14:55:33.000000 hcai-nova-server-nightly-0.1.5.dev202305221455/nova_server/utils/explain_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      447 2023-05-22 14:55:33.000000 hcai-nova-server-nightly-0.1.5.dev202305221455/nova_server/utils/img_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1233 2023-05-22 14:55:33.000000 hcai-nova-server-nightly-0.1.5.dev202305221455/nova_server/utils/import_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      983 2023-05-22 14:55:33.000000 hcai-nova-server-nightly-0.1.5.dev202305221455/nova_server/utils/key_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1375 2023-05-22 14:55:33.000000 hcai-nova-server-nightly-0.1.5.dev202305221455/nova_server/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-05-22 14:55:33.000000 hcai-nova-server-nightly-0.1.5.dev202305221455/nova_server/utils/status_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-05-22 14:55:33.000000 hcai-nova-server-nightly-0.1.5.dev202305221455/nova_server/utils/thread_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-05-22 14:55:33.000000 hcai-nova-server-nightly-0.1.5.dev202305221455/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-22 14:55:43.559060 hcai-nova-server-nightly-0.1.5.dev202305221455/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2383 2023-05-22 14:55:33.000000 hcai-nova-server-nightly-0.1.5.dev202305221455/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:57:07.361990 hcai-nova-server-nightly-0.1.6.dev202305221457/
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-05-22 14:56:55.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1568 2023-05-22 14:57:07.361990 hcai-nova-server-nightly-0.1.6.dev202305221457/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      573 2023-05-22 14:56:55.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:57:07.361990 hcai-nova-server-nightly-0.1.6.dev202305221457/hcai_nova_server_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1568 2023-05-22 14:57:07.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/hcai_nova_server_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      944 2023-05-22 14:57:07.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/hcai_nova_server_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-22 14:57:07.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/hcai_nova_server_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       75 2023-05-22 14:57:07.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/hcai_nova_server_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-22 14:57:07.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/hcai_nova_server_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:57:07.361990 hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-22 14:56:55.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2568 2023-05-22 14:56:55.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/nova_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:57:07.361990 hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/route/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-22 14:56:55.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/route/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-05-22 14:56:55.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/route/cancel.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13062 2023-05-22 14:56:55.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/route/explain.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9891 2023-05-22 14:56:55.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/route/extract.py
+-rw-r--r--   0 runner    (1001) docker     (122)      809 2023-05-22 14:56:55.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/route/log.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7040 2023-05-22 14:56:55.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/route/predict.py
+-rw-r--r--   0 runner    (1001) docker     (122)      756 2023-05-22 14:56:55.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/route/status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6075 2023-05-22 14:56:55.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/route/train.py
+-rw-r--r--   0 runner    (1001) docker     (122)      351 2023-05-22 14:56:55.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/route/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:57:07.361990 hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-22 14:56:55.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:57:07.361990 hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-22 14:56:55.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2254 2023-05-22 14:56:55.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/utils/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12151 2023-05-22 14:56:55.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/utils/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1785 2023-05-22 14:56:55.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/utils/explain_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      447 2023-05-22 14:56:55.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/utils/img_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1233 2023-05-22 14:56:55.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/utils/import_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      983 2023-05-22 14:56:55.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/utils/key_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1375 2023-05-22 14:56:55.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-05-22 14:56:55.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/utils/status_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-05-22 14:56:55.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/utils/thread_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-05-22 14:56:55.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-22 14:57:07.361990 hcai-nova-server-nightly-0.1.6.dev202305221457/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2383 2023-05-22 14:56:55.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/setup.py
```

### Comparing `hcai-nova-server-nightly-0.1.5.dev202305221455/PKG-INFO` & `hcai-nova-server-nightly-0.1.6.dev202305221457/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-nova-server-nightly
-Version: 0.1.5.dev202305221455
+Version: 0.1.6.dev202305221457
 Summary: !Alpha Version! - This repository contains code to setup a computational backend server for the nova annotation tool. You can use this backend to train models of your choosing or create explanations for existing models.
 Home-page: https://github.com/pypa/sampleproject
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `hcai-nova-server-nightly-0.1.5.dev202305221455/README.md` & `hcai-nova-server-nightly-0.1.6.dev202305221457/README.md`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.5.dev202305221455/hcai_nova_server_nightly.egg-info/PKG-INFO` & `hcai-nova-server-nightly-0.1.6.dev202305221457/hcai_nova_server_nightly.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-nova-server-nightly
-Version: 0.1.5.dev202305221455
+Version: 0.1.6.dev202305221457
 Summary: !Alpha Version! - This repository contains code to setup a computational backend server for the nova annotation tool. You can use this backend to train models of your choosing or create explanations for existing models.
 Home-page: https://github.com/pypa/sampleproject
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `hcai-nova-server-nightly-0.1.5.dev202305221455/hcai_nova_server_nightly.egg-info/SOURCES.txt` & `hcai-nova-server-nightly-0.1.6.dev202305221457/hcai_nova_server_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.5.dev202305221455/nova_server/nova_backend.py` & `hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/nova_backend.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.5.dev202305221455/nova_server/route/cancel.py` & `hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/route/cancel.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.5.dev202305221455/nova_server/route/explain.py` & `hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/route/explain.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.5.dev202305221455/nova_server/route/extract.py` & `hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/route/extract.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.5.dev202305221455/nova_server/route/log.py` & `hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/route/log.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.5.dev202305221455/nova_server/route/predict.py` & `hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/route/predict.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.5.dev202305221455/nova_server/route/status.py` & `hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/route/status.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.5.dev202305221455/nova_server/route/train.py` & `hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/route/train.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.5.dev202305221455/nova_server/utils/dataset_utils.py` & `hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/utils/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.5.dev202305221455/nova_server/utils/db_utils.py` & `hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.5.dev202305221455/nova_server/utils/explain_utils.py` & `hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/utils/explain_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.5.dev202305221455/nova_server/utils/import_utils.py` & `hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.5.dev202305221455/nova_server/utils/key_utils.py` & `hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/utils/key_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.5.dev202305221455/nova_server/utils/log_utils.py` & `hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.5.dev202305221455/nova_server/utils/status_utils.py` & `hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/utils/status_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.5.dev202305221455/nova_server/utils/thread_utils.py` & `hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/utils/thread_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.5.dev202305221455/setup.py` & `hcai-nova-server-nightly-0.1.6.dev202305221457/setup.py`

 * *Files identical despite different names*

