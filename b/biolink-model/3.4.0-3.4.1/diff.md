# Comparing `tmp/biolink-model-3.4.0.tar.gz` & `tmp/biolink-model-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biolink-model-3.4.0.tar", last modified: Tue May 23 23:22:56 2023, max compression
+gzip compressed data, was "biolink-model-3.4.1.tar", last modified: Wed May 24 00:29:50 2023, max compression
```

## Comparing `biolink-model-3.4.0.tar` & `biolink-model-3.4.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:22:56.678416 biolink-model-3.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-23 23:22:49.000000 biolink-model-3.4.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-23 23:22:49.000000 biolink-model-3.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-05-23 23:22:56.678416 biolink-model-3.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-05-23 23:22:49.000000 biolink-model-3.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:22:56.678416 biolink-model-3.4.0/biolink/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-23 23:22:49.000000 biolink-model-3.4.0/biolink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   653399 2023-05-23 23:22:49.000000 biolink-model-3.4.0/biolink/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:22:56.678416 biolink-model-3.4.0/biolink_model.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-05-23 23:22:56.000000 biolink-model-3.4.0/biolink_model.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-23 23:22:56.000000 biolink-model-3.4.0/biolink_model.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 23:22:56.000000 biolink-model-3.4.0/biolink_model.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-23 23:22:56.000000 biolink-model-3.4.0/biolink_model.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-23 23:22:56.000000 biolink-model-3.4.0/biolink_model.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-23 23:22:49.000000 biolink-model-3.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-23 23:22:56.682417 biolink-model-3.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-23 23:22:49.000000 biolink-model-3.4.0/setup.py
+drwxr-xr-x   0 SMoxon     (502) staff       (20)        0 2023-05-24 00:29:50.820907 biolink-model-3.4.1/
+-rw-r--r--   0 SMoxon     (502) staff       (20)      762 2022-11-30 01:03:34.000000 biolink-model-3.4.1/AUTHORS
+-rw-r--r--   0 SMoxon     (502) staff       (20)      523 2022-11-03 00:23:30.000000 biolink-model-3.4.1/LICENSE
+-rw-r--r--   0 SMoxon     (502) staff       (20)     7187 2023-05-24 00:29:50.821058 biolink-model-3.4.1/PKG-INFO
+-rw-r--r--   0 SMoxon     (502) staff       (20)     6330 2023-05-16 23:18:34.000000 biolink-model-3.4.1/README.md
+drwxr-xr-x   0 SMoxon     (502) staff       (20)        0 2023-05-24 00:29:50.815277 biolink-model-3.4.1/biolink/
+-rw-r--r--   0 SMoxon     (502) staff       (20)      721 2022-11-03 00:23:30.000000 biolink-model-3.4.1/biolink/__init__.py
+-rw-r--r--   0 SMoxon     (502) staff       (20)   653399 2023-05-24 00:28:38.000000 biolink-model-3.4.1/biolink/model.py
+-rw-r--r--   0 SMoxon     (502) staff       (20)  1214949 2023-05-24 00:22:00.000000 biolink-model-3.4.1/biolink/pydanticmodel.py
+drwxr-xr-x   0 SMoxon     (502) staff       (20)        0 2023-05-24 00:29:50.820671 biolink-model-3.4.1/biolink_model.egg-info/
+-rw-r--r--   0 SMoxon     (502) staff       (20)     7187 2023-05-24 00:29:50.000000 biolink-model-3.4.1/biolink_model.egg-info/PKG-INFO
+-rw-r--r--   0 SMoxon     (502) staff       (20)      305 2023-05-24 00:29:50.000000 biolink-model-3.4.1/biolink_model.egg-info/SOURCES.txt
+-rw-r--r--   0 SMoxon     (502) staff       (20)        1 2023-05-24 00:29:50.000000 biolink-model-3.4.1/biolink_model.egg-info/dependency_links.txt
+-rw-r--r--   0 SMoxon     (502) staff       (20)       25 2023-05-24 00:29:50.000000 biolink-model-3.4.1/biolink_model.egg-info/requires.txt
+-rw-r--r--   0 SMoxon     (502) staff       (20)        8 2023-05-24 00:29:50.000000 biolink-model-3.4.1/biolink_model.egg-info/top_level.txt
+-rw-r--r--   0 SMoxon     (502) staff       (20)     1015 2023-05-23 23:04:16.000000 biolink-model-3.4.1/pyproject.toml
+-rw-r--r--   0 SMoxon     (502) staff       (20)      841 2023-05-24 00:29:50.821773 biolink-model-3.4.1/setup.cfg
+-rw-r--r--   0 SMoxon     (502) staff       (20)     1366 2023-05-24 00:28:08.000000 biolink-model-3.4.1/setup.py
```

### Comparing `biolink-model-3.4.0/AUTHORS` & `biolink-model-3.4.1/AUTHORS`

 * *Files identical despite different names*

### Comparing `biolink-model-3.4.0/LICENSE` & `biolink-model-3.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `biolink-model-3.4.0/PKG-INFO` & `biolink-model-3.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biolink-model
-Version: 3.4.0
+Version: 3.4.1
 Summary: 'A high level datamodel of biological entities and associations'
 Home-page: https://github.com/biolink/biolink-model
 Author: ('Deepak Unni', 'Sierra Moxon')
 Author-email: smoxon@lbl.gov
 License: BSD
 Keywords: NCATS NCATS-Translator Biolink-Model Biolink LinkML Datamodel
 Platform: UNKNOWN
```

### Comparing `biolink-model-3.4.0/README.md` & `biolink-model-3.4.1/README.md`

 * *Files identical despite different names*

### Comparing `biolink-model-3.4.0/biolink/__init__.py` & `biolink-model-3.4.1/biolink/__init__.py`

 * *Files identical despite different names*

### Comparing `biolink-model-3.4.0/biolink/model.py` & `biolink-model-3.4.1/biolink/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 00000000: 2320 4175 746f 2067 656e 6572 6174 6564  # Auto generated
 00000010: 2066 726f 6d20 6269 6f6c 696e 6b2d 6d6f   from biolink-mo
 00000020: 6465 6c2e 7961 6d6c 2062 7920 7079 7468  del.yaml by pyth
 00000030: 6f6e 6765 6e2e 7079 2076 6572 7369 6f6e  ongen.py version
 00000040: 3a20 302e 392e 300a 2320 4765 6e65 7261  : 0.9.0.# Genera
 00000050: 7469 6f6e 2064 6174 653a 2032 3032 332d  tion date: 2023-
-00000060: 3035 2d32 3354 3233 3a30 353a 3139 0a23  05-23T23:05:19.#
+00000060: 3035 2d32 3354 3233 3a32 333a 3330 0a23  05-23T23:23:30.#
 00000070: 2053 6368 656d 613a 2042 696f 6c69 6e6b   Schema: Biolink
 00000080: 2d4d 6f64 656c 0a23 0a23 2069 643a 2068  -Model.#.# id: h
 00000090: 7474 7073 3a2f 2f77 3369 642e 6f72 672f  ttps://w3id.org/
 000000a0: 6269 6f6c 696e 6b2f 6269 6f6c 696e 6b2d  biolink/biolink-
 000000b0: 6d6f 6465 6c0a 2320 6465 7363 7269 7074  model.# descript
 000000c0: 696f 6e3a 2045 6e74 6974 7920 616e 6420  ion: Entity and 
 000000d0: 6173 736f 6369 6174 696f 6e20 7461 786f  association taxo
```

### Comparing `biolink-model-3.4.0/biolink_model.egg-info/PKG-INFO` & `biolink-model-3.4.1/biolink_model.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biolink-model
-Version: 3.4.0
+Version: 3.4.1
 Summary: 'A high level datamodel of biological entities and associations'
 Home-page: https://github.com/biolink/biolink-model
 Author: ('Deepak Unni', 'Sierra Moxon')
 Author-email: smoxon@lbl.gov
 License: BSD
 Keywords: NCATS NCATS-Translator Biolink-Model Biolink LinkML Datamodel
 Platform: UNKNOWN
```

### Comparing `biolink-model-3.4.0/pyproject.toml` & `biolink-model-3.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `biolink-model-3.4.0/setup.cfg` & `biolink-model-3.4.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = biolink_model
 description = 'A high level datamodel of biological entities and associations'
-version = 3.4.0
+version = 3.4.1
 url = https://github.com/biolink/biolink-model
 author = Harold Solbrig
 author-email = smoxon@lbl.gov
 summary = Biolink Model
 home-page = https://biolink.github.io/biolink-model/docs/
 license = CC0 1.0 Universal
 python-requires = >=3.9
```

### Comparing `biolink-model-3.4.0/setup.py` & `biolink-model-3.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup, find_packages
 
 with open("requirements.txt", "r") as FH:
     REQUIREMENTS = FH.readlines()
 
 NAME = 'biolink-model'
-VERSION = '3.4.0'
+VERSION = '3.4.1'
 
 DESCRIPTION = 'Biolink Model: A high level datamodel of biological entities and associations'
 URL = 'https://github.com/biolink/biolink-model'
 AUTHOR = 'Deepak Unni', 'Sierra Moxon'
 EMAIL = 'smoxon@lbl.gov'
 REQUIRES_PYTHON = '>=3.9'
 LICENSE = 'BSD'
```

