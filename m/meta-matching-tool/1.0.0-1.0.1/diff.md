# Comparing `tmp/meta_matching_tool-1.0.0.tar.gz` & `tmp/meta_matching_tool-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/meta_matching_tool-1.0.0.tar", last modified: Tue May 23 06:20:47 2023, max compression
+gzip compressed data, was "dist/meta_matching_tool-1.0.1.tar", last modified: Wed May 24 05:01:26 2023, max compression
```

## Comparing `meta_matching_tool-1.0.0.tar` & `meta_matching_tool-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 tlq        (501) staff       (20)        0 2023-05-23 06:20:47.078042 meta_matching_tool-1.0.0/
--rw-r--r--   0 tlq        (501) staff       (20)      320 2023-05-23 06:20:47.077731 meta_matching_tool-1.0.0/PKG-INFO
-drwxr-xr-x   0 tlq        (501) staff       (20)        0 2023-05-23 06:20:47.071381 meta_matching_tool-1.0.0/meta_matching_tool/
--rw-rw-r--   0 tlq        (501) staff       (20)       69 2023-04-22 11:36:33.000000 meta_matching_tool-1.0.0/meta_matching_tool/__init__.py
--rw-rw-r--   0 tlq        (501) staff       (20)     6737 2023-04-22 11:36:33.000000 meta_matching_tool-1.0.0/meta_matching_tool/model.py
--rw-rw-r--   0 tlq        (501) staff       (20)    12243 2023-04-22 11:36:33.000000 meta_matching_tool-1.0.0/meta_matching_tool/utils.py
-drwxr-xr-x   0 tlq        (501) staff       (20)        0 2023-05-23 06:20:47.077053 meta_matching_tool-1.0.0/meta_matching_tool.egg-info/
--rw-r--r--   0 tlq        (501) staff       (20)      320 2023-05-23 06:20:47.000000 meta_matching_tool-1.0.0/meta_matching_tool.egg-info/PKG-INFO
--rw-r--r--   0 tlq        (501) staff       (20)      345 2023-05-23 06:20:47.000000 meta_matching_tool-1.0.0/meta_matching_tool.egg-info/SOURCES.txt
--rw-r--r--   0 tlq        (501) staff       (20)        1 2023-05-23 06:20:47.000000 meta_matching_tool-1.0.0/meta_matching_tool.egg-info/dependency_links.txt
--rw-r--r--   0 tlq        (501) staff       (20)        1 2023-05-23 06:20:47.000000 meta_matching_tool-1.0.0/meta_matching_tool.egg-info/not-zip-safe
--rw-r--r--   0 tlq        (501) staff       (20)       84 2023-05-23 06:20:47.000000 meta_matching_tool-1.0.0/meta_matching_tool.egg-info/requires.txt
--rw-r--r--   0 tlq        (501) staff       (20)       19 2023-05-23 06:20:47.000000 meta_matching_tool-1.0.0/meta_matching_tool.egg-info/top_level.txt
--rw-r--r--   0 tlq        (501) staff       (20)       38 2023-05-23 06:20:47.078157 meta_matching_tool-1.0.0/setup.cfg
--rw-r--r--   0 tlq        (501) staff       (20)      705 2023-05-23 06:20:18.000000 meta_matching_tool-1.0.0/setup.py
+drwxr-xr-x   0 tlq        (501) staff       (20)        0 2023-05-24 05:01:26.333252 meta_matching_tool-1.0.1/
+-rw-r--r--   0 tlq        (501) staff       (20)      320 2023-05-24 05:01:26.332963 meta_matching_tool-1.0.1/PKG-INFO
+drwxr-xr-x   0 tlq        (501) staff       (20)        0 2023-05-24 05:01:26.329361 meta_matching_tool-1.0.1/meta_matching_tool/
+-rw-rw-r--   0 tlq        (501) staff       (20)       69 2023-04-22 11:36:33.000000 meta_matching_tool-1.0.1/meta_matching_tool/__init__.py
+-rw-rw-r--   0 tlq        (501) staff       (20)     6737 2023-04-22 11:36:33.000000 meta_matching_tool-1.0.1/meta_matching_tool/model.py
+-rw-rw-r--   0 tlq        (501) staff       (20)    12243 2023-04-22 11:36:33.000000 meta_matching_tool-1.0.1/meta_matching_tool/utils.py
+drwxr-xr-x   0 tlq        (501) staff       (20)        0 2023-05-24 05:01:26.332535 meta_matching_tool-1.0.1/meta_matching_tool.egg-info/
+-rw-r--r--   0 tlq        (501) staff       (20)      320 2023-05-24 05:01:26.000000 meta_matching_tool-1.0.1/meta_matching_tool.egg-info/PKG-INFO
+-rw-r--r--   0 tlq        (501) staff       (20)      345 2023-05-24 05:01:26.000000 meta_matching_tool-1.0.1/meta_matching_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 tlq        (501) staff       (20)        1 2023-05-24 05:01:26.000000 meta_matching_tool-1.0.1/meta_matching_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 tlq        (501) staff       (20)        1 2023-05-24 04:59:54.000000 meta_matching_tool-1.0.1/meta_matching_tool.egg-info/not-zip-safe
+-rw-r--r--   0 tlq        (501) staff       (20)       84 2023-05-24 05:01:26.000000 meta_matching_tool-1.0.1/meta_matching_tool.egg-info/requires.txt
+-rw-r--r--   0 tlq        (501) staff       (20)       19 2023-05-24 05:01:26.000000 meta_matching_tool-1.0.1/meta_matching_tool.egg-info/top_level.txt
+-rw-r--r--   0 tlq        (501) staff       (20)       38 2023-05-24 05:01:26.333344 meta_matching_tool-1.0.1/setup.cfg
+-rw-r--r--   0 tlq        (501) staff       (20)      705 2023-05-24 04:58:52.000000 meta_matching_tool-1.0.1/setup.py
```

### Comparing `meta_matching_tool-1.0.0/meta_matching_tool/model.py` & `meta_matching_tool-1.0.1/meta_matching_tool/model.py`

 * *Files identical despite different names*

### Comparing `meta_matching_tool-1.0.0/meta_matching_tool/utils.py` & `meta_matching_tool-1.0.1/meta_matching_tool/utils.py`

 * *Files identical despite different names*

### Comparing `meta_matching_tool-1.0.0/setup.py` & `meta_matching_tool-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # @Author : Leqi Tian
 # @File : setup.py
 
 from setuptools import setup
 from setuptools import find_packages
 
 
-VERSION = '1.0.0'
+VERSION = '1.0.1'
 
 setup(
     name='meta_matching_tool',  # package name
     version=VERSION,  # package version
     description='An integrated deep learning framework for the interpretation of untargeted metabolomics data',  
     packages=find_packages(),
     author='Leqi Tian',
```

