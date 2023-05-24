# Comparing `tmp/delphi_epidata-4.1.0.tar.gz` & `tmp/delphi_epidata-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delphi_epidata-4.1.0.tar", last modified: Wed May 24 15:24:40 2023, max compression
+gzip compressed data, was "delphi_epidata-4.1.1.tar", last modified: Wed May 24 20:29:07 2023, max compression
```

## Comparing `delphi_epidata-4.1.0.tar` & `delphi_epidata-4.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:40.041673 delphi_epidata-4.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-24 15:24:29.000000 delphi_epidata-4.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-24 15:24:40.041673 delphi_epidata-4.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-24 15:24:29.000000 delphi_epidata-4.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:40.041673 delphi_epidata-4.1.0/delphi_epidata/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-24 15:24:29.000000 delphi_epidata-4.1.0/delphi_epidata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25286 2023-05-24 15:24:38.000000 delphi_epidata-4.1.0/delphi_epidata/delphi_epidata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:40.041673 delphi_epidata-4.1.0/delphi_epidata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-24 15:24:39.000000 delphi_epidata-4.1.0/delphi_epidata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-24 15:24:40.000000 delphi_epidata-4.1.0/delphi_epidata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:24:39.000000 delphi_epidata-4.1.0/delphi_epidata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-24 15:24:39.000000 delphi_epidata-4.1.0/delphi_epidata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-24 15:24:39.000000 delphi_epidata-4.1.0/delphi_epidata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 15:24:40.041673 delphi_epidata-4.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-24 15:24:29.000000 delphi_epidata-4.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:29:07.746891 delphi_epidata-4.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-24 20:28:57.000000 delphi_epidata-4.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-24 20:29:07.746891 delphi_epidata-4.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-24 20:28:57.000000 delphi_epidata-4.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:29:07.746891 delphi_epidata-4.1.1/delphi_epidata/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-24 20:28:57.000000 delphi_epidata-4.1.1/delphi_epidata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25286 2023-05-24 20:29:07.000000 delphi_epidata-4.1.1/delphi_epidata/delphi_epidata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:29:07.746891 delphi_epidata-4.1.1/delphi_epidata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-24 20:29:07.000000 delphi_epidata-4.1.1/delphi_epidata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-24 20:29:07.000000 delphi_epidata-4.1.1/delphi_epidata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 20:29:07.000000 delphi_epidata-4.1.1/delphi_epidata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-24 20:29:07.000000 delphi_epidata-4.1.1/delphi_epidata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-24 20:29:07.000000 delphi_epidata-4.1.1/delphi_epidata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 20:29:07.746891 delphi_epidata-4.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-24 20:28:57.000000 delphi_epidata-4.1.1/setup.py
```

### Comparing `delphi_epidata-4.1.0/LICENSE` & `delphi_epidata-4.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `delphi_epidata-4.1.0/PKG-INFO` & `delphi_epidata-4.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delphi_epidata
-Version: 4.1.0
+Version: 4.1.1
 Summary: A programmatic interface to Delphi's Epidata API.
 Home-page: https://github.com/cmu-delphi/delphi-epidata
 Author: David Farrow
 Author-email: dfarrow0@gmail.com
 License: UNKNOWN
 Description: # Delphi Epidata API Client
```

### Comparing `delphi_epidata-4.1.0/delphi_epidata/delphi_epidata.py` & `delphi_epidata-4.1.1/delphi_epidata/delphi_epidata.py`

 * *Files identical despite different names*

### Comparing `delphi_epidata-4.1.0/delphi_epidata.egg-info/PKG-INFO` & `delphi_epidata-4.1.1/delphi_epidata.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delphi-epidata
-Version: 4.1.0
+Version: 4.1.1
 Summary: A programmatic interface to Delphi's Epidata API.
 Home-page: https://github.com/cmu-delphi/delphi-epidata
 Author: David Farrow
 Author-email: dfarrow0@gmail.com
 License: UNKNOWN
 Description: # Delphi Epidata API Client
```

### Comparing `delphi_epidata-4.1.0/setup.py` & `delphi_epidata-4.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="delphi_epidata",
-    version="4.1.0",
+    version="4.1.1",
     author="David Farrow",
     author_email="dfarrow0@gmail.com",
     description="A programmatic interface to Delphi's Epidata API.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cmu-delphi/delphi-epidata",
     packages=setuptools.find_packages(),
```

