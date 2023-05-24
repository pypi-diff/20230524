# Comparing `tmp/meta_matching_tool-1.1.1.tar.gz` & `tmp/meta_matching_tool-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/meta_matching_tool-1.1.1.tar", last modified: Wed May 24 05:37:52 2023, max compression
+gzip compressed data, was "dist/meta_matching_tool-1.2.0.tar", last modified: Wed May 24 12:40:44 2023, max compression
```

## Comparing `meta_matching_tool-1.1.1.tar` & `meta_matching_tool-1.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 tlq        (501) staff       (20)        0 2023-05-24 05:37:52.496106 meta_matching_tool-1.1.1/
--rw-r--r--   0 tlq        (501) staff       (20)     1051 2023-05-23 05:05:05.000000 meta_matching_tool-1.1.1/LICENSE.txt
--rw-r--r--   0 tlq        (501) staff       (20)      271 2023-05-24 05:37:52.495572 meta_matching_tool-1.1.1/PKG-INFO
-drwxr-xr-x   0 tlq        (501) staff       (20)        0 2023-05-24 05:37:52.491700 meta_matching_tool-1.1.1/meta_matching_tool/
--rw-rw-r--   0 tlq        (501) staff       (20)       69 2023-04-22 11:36:33.000000 meta_matching_tool-1.1.1/meta_matching_tool/__init__.py
--rw-rw-r--   0 tlq        (501) staff       (20)     6737 2023-04-22 11:36:33.000000 meta_matching_tool-1.1.1/meta_matching_tool/model.py
--rw-rw-r--   0 tlq        (501) staff       (20)    12243 2023-04-22 11:36:33.000000 meta_matching_tool-1.1.1/meta_matching_tool/utils.py
-drwxr-xr-x   0 tlq        (501) staff       (20)        0 2023-05-24 05:37:52.494859 meta_matching_tool-1.1.1/meta_matching_tool.egg-info/
--rw-r--r--   0 tlq        (501) staff       (20)      271 2023-05-24 05:37:52.000000 meta_matching_tool-1.1.1/meta_matching_tool.egg-info/PKG-INFO
--rw-r--r--   0 tlq        (501) staff       (20)      357 2023-05-24 05:37:52.000000 meta_matching_tool-1.1.1/meta_matching_tool.egg-info/SOURCES.txt
--rw-r--r--   0 tlq        (501) staff       (20)        1 2023-05-24 05:37:52.000000 meta_matching_tool-1.1.1/meta_matching_tool.egg-info/dependency_links.txt
--rw-r--r--   0 tlq        (501) staff       (20)        1 2023-05-24 05:37:52.000000 meta_matching_tool-1.1.1/meta_matching_tool.egg-info/not-zip-safe
--rw-r--r--   0 tlq        (501) staff       (20)       84 2023-05-24 05:37:52.000000 meta_matching_tool-1.1.1/meta_matching_tool.egg-info/requires.txt
--rw-r--r--   0 tlq        (501) staff       (20)       19 2023-05-24 05:37:52.000000 meta_matching_tool-1.1.1/meta_matching_tool.egg-info/top_level.txt
--rw-r--r--   0 tlq        (501) staff       (20)       38 2023-05-24 05:37:52.496252 meta_matching_tool-1.1.1/setup.cfg
--rw-r--r--   0 tlq        (501) staff       (20)      705 2023-05-24 05:36:36.000000 meta_matching_tool-1.1.1/setup.py
+drwxr-xr-x   0 tlq        (501) staff       (20)        0 2023-05-24 12:40:44.075505 meta_matching_tool-1.2.0/
+-rw-r--r--   0 tlq        (501) staff       (20)     1051 2023-05-23 05:05:05.000000 meta_matching_tool-1.2.0/LICENSE.txt
+-rw-r--r--   0 tlq        (501) staff       (20)      271 2023-05-24 12:40:44.075110 meta_matching_tool-1.2.0/PKG-INFO
+drwxr-xr-x   0 tlq        (501) staff       (20)        0 2023-05-24 12:40:44.071262 meta_matching_tool-1.2.0/meta_matching_tool/
+-rw-rw-r--   0 tlq        (501) staff       (20)       69 2023-04-22 11:36:33.000000 meta_matching_tool-1.2.0/meta_matching_tool/__init__.py
+-rw-rw-r--   0 tlq        (501) staff       (20)     6737 2023-04-22 11:36:33.000000 meta_matching_tool-1.2.0/meta_matching_tool/model.py
+-rw-rw-r--   0 tlq        (501) staff       (20)    12243 2023-04-22 11:36:33.000000 meta_matching_tool-1.2.0/meta_matching_tool/utils.py
+drwxr-xr-x   0 tlq        (501) staff       (20)        0 2023-05-24 12:40:44.074734 meta_matching_tool-1.2.0/meta_matching_tool.egg-info/
+-rw-r--r--   0 tlq        (501) staff       (20)      271 2023-05-24 12:40:43.000000 meta_matching_tool-1.2.0/meta_matching_tool.egg-info/PKG-INFO
+-rw-r--r--   0 tlq        (501) staff       (20)      357 2023-05-24 12:40:43.000000 meta_matching_tool-1.2.0/meta_matching_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 tlq        (501) staff       (20)        1 2023-05-24 12:40:43.000000 meta_matching_tool-1.2.0/meta_matching_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 tlq        (501) staff       (20)        1 2023-05-24 12:40:43.000000 meta_matching_tool-1.2.0/meta_matching_tool.egg-info/not-zip-safe
+-rw-r--r--   0 tlq        (501) staff       (20)       96 2023-05-24 12:40:43.000000 meta_matching_tool-1.2.0/meta_matching_tool.egg-info/requires.txt
+-rw-r--r--   0 tlq        (501) staff       (20)       19 2023-05-24 12:40:43.000000 meta_matching_tool-1.2.0/meta_matching_tool.egg-info/top_level.txt
+-rw-r--r--   0 tlq        (501) staff       (20)       38 2023-05-24 12:40:44.075670 meta_matching_tool-1.2.0/setup.cfg
+-rw-r--r--   0 tlq        (501) staff       (20)      728 2023-05-24 12:37:11.000000 meta_matching_tool-1.2.0/setup.py
```

### Comparing `meta_matching_tool-1.1.1/LICENSE.txt` & `meta_matching_tool-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `meta_matching_tool-1.1.1/meta_matching_tool/model.py` & `meta_matching_tool-1.2.0/meta_matching_tool/model.py`

 * *Files identical despite different names*

### Comparing `meta_matching_tool-1.1.1/meta_matching_tool/utils.py` & `meta_matching_tool-1.2.0/meta_matching_tool/utils.py`

 * *Files identical despite different names*

### Comparing `meta_matching_tool-1.1.1/setup.py` & `meta_matching_tool-1.2.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,26 +3,27 @@
 # @Author : Leqi Tian
 # @File : setup.py
 
 from setuptools import setup
 from setuptools import find_packages
 
 
-VERSION = '1.1.1'
+VERSION = '1.2.0'
 
 setup(
     name='meta_matching_tool',  # package name
     version=VERSION,  # package version
     description='An integrated deep learning framework for the interpretation of untargeted metabolomics data',  
     packages=find_packages(),
     author='Leqi Tian',
     author_email='leqitian@link.cuhk.edu.cn',
     python_requires=">=3.9",
     zip_safe=False,
     install_requires=[
-        'numpy>=1.21.5',
-        'pandas>=1.5.3',
-        'python_igraph>=0.10.4',
-       'scikit_learn>=1.0.2',
-        'torch>=1.11.0',
+        'numpy>=1.18.5',
+        'pandas>=1.0.5',
+        'python_igraph>=0.8.3',
+        'scikit_learn>=0.23.1',
+        'torch>=1.6.0',
+        'torch>=1.7.1'
     ],
 )
```

