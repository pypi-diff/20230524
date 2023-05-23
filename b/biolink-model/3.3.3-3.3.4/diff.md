# Comparing `tmp/biolink-model-3.3.3.tar.gz` & `tmp/biolink-model-3.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biolink-model-3.3.3.tar", last modified: Mon May  8 15:13:20 2023, max compression
+gzip compressed data, was "biolink-model-3.3.4.tar", last modified: Wed May 17 16:21:44 2023, max compression
```

## Comparing `biolink-model-3.3.3.tar` & `biolink-model-3.3.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:20.687583 biolink-model-3.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-08 15:13:10.000000 biolink-model-3.3.3/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-08 15:13:10.000000 biolink-model-3.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-05-08 15:13:20.687583 biolink-model-3.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-05-08 15:13:10.000000 biolink-model-3.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:20.683583 biolink-model-3.3.3/biolink/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-08 15:13:10.000000 biolink-model-3.3.3/biolink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   651883 2023-05-08 15:13:10.000000 biolink-model-3.3.3/biolink/model.py
--rw-r--r--   0 runner    (1001) docker     (123)  1193584 2023-05-08 15:13:10.000000 biolink-model-3.3.3/biolink/pydanticmodel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:20.687583 biolink-model-3.3.3/biolink_model.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-05-08 15:13:20.000000 biolink-model-3.3.3/biolink_model.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-08 15:13:20.000000 biolink-model-3.3.3/biolink_model.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 15:13:20.000000 biolink-model-3.3.3/biolink_model.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-08 15:13:20.000000 biolink-model-3.3.3/biolink_model.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-08 15:13:20.000000 biolink-model-3.3.3/biolink_model.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-08 15:13:11.000000 biolink-model-3.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-08 15:13:20.687583 biolink-model-3.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-08 15:13:11.000000 biolink-model-3.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:21:44.679115 biolink-model-3.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-17 16:21:39.000000 biolink-model-3.3.4/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-17 16:21:39.000000 biolink-model-3.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-05-17 16:21:44.679115 biolink-model-3.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-05-17 16:21:39.000000 biolink-model-3.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:21:44.675115 biolink-model-3.3.4/biolink/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-17 16:21:39.000000 biolink-model-3.3.4/biolink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   651883 2023-05-17 16:21:39.000000 biolink-model-3.3.4/biolink/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1193584 2023-05-17 16:21:39.000000 biolink-model-3.3.4/biolink/pydanticmodel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:21:44.679115 biolink-model-3.3.4/biolink_model.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-05-17 16:21:44.000000 biolink-model-3.3.4/biolink_model.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-17 16:21:44.000000 biolink-model-3.3.4/biolink_model.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 16:21:44.000000 biolink-model-3.3.4/biolink_model.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-17 16:21:44.000000 biolink-model-3.3.4/biolink_model.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-17 16:21:44.000000 biolink-model-3.3.4/biolink_model.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-17 16:21:39.000000 biolink-model-3.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-17 16:21:44.679115 biolink-model-3.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-17 16:21:39.000000 biolink-model-3.3.4/setup.py
```

### Comparing `biolink-model-3.3.3/AUTHORS` & `biolink-model-3.3.4/AUTHORS`

 * *Files identical despite different names*

### Comparing `biolink-model-3.3.3/LICENSE` & `biolink-model-3.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `biolink-model-3.3.3/PKG-INFO` & `biolink-model-3.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biolink-model
-Version: 3.3.3
+Version: 3.3.4
 Summary: 'A high level datamodel of biological entities and associations'
 Home-page: https://github.com/biolink/biolink-model
 Author: ('Deepak Unni', 'Sierra Moxon')
 Author-email: smoxon@lbl.gov
 License: BSD
 Keywords: NCATS NCATS-Translator Biolink-Model Biolink LinkML Datamodel
 Platform: UNKNOWN
```

### Comparing `biolink-model-3.3.3/README.md` & `biolink-model-3.3.4/README.md`

 * *Files identical despite different names*

### Comparing `biolink-model-3.3.3/biolink/__init__.py` & `biolink-model-3.3.4/biolink/__init__.py`

 * *Files identical despite different names*

### Comparing `biolink-model-3.3.3/biolink/model.py` & `biolink-model-3.3.4/biolink/model.py`

 * *Files identical despite different names*

### Comparing `biolink-model-3.3.3/biolink/pydanticmodel.py` & `biolink-model-3.3.4/biolink/pydanticmodel.py`

 * *Files identical despite different names*

### Comparing `biolink-model-3.3.3/biolink_model.egg-info/PKG-INFO` & `biolink-model-3.3.4/biolink_model.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biolink-model
-Version: 3.3.3
+Version: 3.3.4
 Summary: 'A high level datamodel of biological entities and associations'
 Home-page: https://github.com/biolink/biolink-model
 Author: ('Deepak Unni', 'Sierra Moxon')
 Author-email: smoxon@lbl.gov
 License: BSD
 Keywords: NCATS NCATS-Translator Biolink-Model Biolink LinkML Datamodel
 Platform: UNKNOWN
```

### Comparing `biolink-model-3.3.3/pyproject.toml` & `biolink-model-3.3.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "biolink-model"
-version = "0.0.0"
+version = "3.3.3.post25.dev0+93c02412c"
 description = "Entity and association taxonomy and datamodel for life-sciences data"
 authors = ["Sierra Taylor Moxon <sierra.taylor@gmail.com>"]
 license = "https://creativecommons.org/publicdomain/zero/1.0/"
 readme = "README.md"
 
 packages = [{include = "biolink"}]
 
@@ -14,15 +14,15 @@
 linkml = "^1.4"
 curies = "^0.5.2"
 prefixmaps = "^0.1.4"
 pytest = "^7.3.1"
 bs4 = "^0.0.1"
 
 [tool.poetry-dynamic-versioning]
-enable = true
+enable = false
 vcs = "git"
 style = "pep440"
 
 [tool.poetry.dev-dependencies]
 codespell = "^2.2.4"
 yamllint = "^1.30.0"
```

### Comparing `biolink-model-3.3.3/setup.cfg` & `biolink-model-3.3.4/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = biolink_model
 description = 'A high level datamodel of biological entities and associations'
-version = 3.3.3
+version = 3.3.4
 url = https://github.com/biolink/biolink-model
 author = Harold Solbrig
 author-email = smoxon@lbl.gov
 summary = Biolink Model
 home-page = https://biolink.github.io/biolink-model/docs/
 license = CC0 1.0 Universal
 python-requires = >=3.9
```

### Comparing `biolink-model-3.3.3/setup.py` & `biolink-model-3.3.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup, find_packages
 
 with open("requirements.txt", "r") as FH:
     REQUIREMENTS = FH.readlines()
 
 NAME = 'biolink-model'
-VERSION = '3.3.3'
+VERSION = '3.3.4'
 
 DESCRIPTION = 'Biolink Model: A high level datamodel of biological entities and associations'
 URL = 'https://github.com/biolink/biolink-model'
 AUTHOR = 'Deepak Unni', 'Sierra Moxon'
 EMAIL = 'smoxon@lbl.gov'
 REQUIRES_PYTHON = '>=3.9'
 LICENSE = 'BSD'
```

