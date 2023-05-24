# Comparing `tmp/pyMSVC-0.5.1.tar.gz` & `tmp/pyMSVC-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyMSVC-0.5.1.tar", last modified: Tue May 23 03:44:16 2023, max compression
+gzip compressed data, was "pyMSVC-0.5.2.tar", last modified: Wed May 24 03:55:59 2023, max compression
```

## Comparing `pyMSVC-0.5.1.tar` & `pyMSVC-0.5.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 03:44:16.202447 pyMSVC-0.5.1/
--rw-rw-rw-   0        0        0     1265 2022-08-01 05:24:54.000000 pyMSVC-0.5.1/LICENSE
--rw-rw-rw-   0        0        0      404 2023-05-23 03:44:16.201447 pyMSVC-0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     8235 2022-08-02 05:12:16.000000 pyMSVC-0.5.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-23 03:44:16.184936 pyMSVC-0.5.1/pyMSVC/
--rw-rw-rw-   0        0        0   127906 2023-05-23 03:35:27.000000 pyMSVC-0.5.1/pyMSVC/__init__.py
--rw-rw-rw-   0        0        0    43493 2022-10-20 23:05:10.000000 pyMSVC-0.5.1/pyMSVC/vswhere.py
-drwxrwxrwx   0        0        0        0 2023-05-23 03:44:16.200448 pyMSVC-0.5.1/pyMSVC.egg-info/
--rw-rw-rw-   0        0        0      404 2023-05-23 03:44:16.000000 pyMSVC-0.5.1/pyMSVC.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-05-23 03:44:16.000000 pyMSVC-0.5.1/pyMSVC.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 03:44:16.000000 pyMSVC-0.5.1/pyMSVC.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-23 03:44:16.000000 pyMSVC-0.5.1/pyMSVC.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-23 03:44:16.000000 pyMSVC-0.5.1/pyMSVC.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       88 2023-05-23 03:40:23.000000 pyMSVC-0.5.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-23 03:44:16.202447 pyMSVC-0.5.1/setup.cfg
--rw-rw-rw-   0        0        0      590 2023-05-23 03:35:27.000000 pyMSVC-0.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 03:55:59.506242 pyMSVC-0.5.2/
+-rw-rw-rw-   0        0        0     1265 2022-08-01 05:24:54.000000 pyMSVC-0.5.2/LICENSE
+-rw-rw-rw-   0        0        0      404 2023-05-24 03:55:59.506242 pyMSVC-0.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0     8235 2022-08-02 05:12:16.000000 pyMSVC-0.5.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-24 03:55:59.489228 pyMSVC-0.5.2/pyMSVC/
+-rw-rw-rw-   0        0        0   128072 2023-05-24 03:54:01.000000 pyMSVC-0.5.2/pyMSVC/__init__.py
+-rw-rw-rw-   0        0        0    43493 2022-10-20 23:05:10.000000 pyMSVC-0.5.2/pyMSVC/vswhere.py
+drwxrwxrwx   0        0        0        0 2023-05-24 03:55:59.505240 pyMSVC-0.5.2/pyMSVC.egg-info/
+-rw-rw-rw-   0        0        0      404 2023-05-24 03:55:59.000000 pyMSVC-0.5.2/pyMSVC.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-05-24 03:55:59.000000 pyMSVC-0.5.2/pyMSVC.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 03:55:59.000000 pyMSVC-0.5.2/pyMSVC.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-24 03:55:59.000000 pyMSVC-0.5.2/pyMSVC.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-24 03:55:59.000000 pyMSVC-0.5.2/pyMSVC.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       88 2023-05-23 03:40:23.000000 pyMSVC-0.5.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-24 03:55:59.507240 pyMSVC-0.5.2/setup.cfg
+-rw-rw-rw-   0        0        0      590 2023-05-24 03:54:01.000000 pyMSVC-0.5.2/setup.py
```

### Comparing `pyMSVC-0.5.1/LICENSE` & `pyMSVC-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyMSVC-0.5.1/README.md` & `pyMSVC-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `pyMSVC-0.5.1/pyMSVC/__init__.py` & `pyMSVC-0.5.2/pyMSVC/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 #
 # #############################################################################
 #
 # MIT License
 #
-# Copyright 2022  Kevin G. Schlosser
+# Copyright 2023  Kevin G. Schlosser
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -36,15 +36,15 @@
 import os
 import sys
 import ctypes
 import subprocess
 import winreg
 import logging
 from typing import Optional, Union
-__version__ = '0.5.1'
+__version__ = '0.5.2'
 
 _IS_WIN = sys.platform.startswith('win')
 
 logger = logging.getLogger(__name__)
 
 
 def _setup_logging():
@@ -925,15 +925,18 @@
     def _installed_c_paths(self):
         if self.__installed_versions is None:
             self.__installed_versions = {}
 
             def add(vers):
                 for base_pth, ver in vers:
                     if os.path.exists(base_pth):
-                        base_ver = float(int(ver.split('.')[0]))
+                        try:
+                            base_ver = float(int(ver.split('.')[0]))
+                        except ValueError:
+                            base_ver = float(int(ver.replace('vc', '').split('.')[0]))
 
                         self.__installed_versions[ver] = dict(
                             base=base_pth,
                             root=base_pth
                         )
                         self.__installed_versions[base_ver] = dict(
                             base=base_pth,
```

### Comparing `pyMSVC-0.5.1/pyMSVC/vswhere.py` & `pyMSVC-0.5.2/pyMSVC/vswhere.py`

 * *Files identical despite different names*

### Comparing `pyMSVC-0.5.1/setup.py` & `pyMSVC-0.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 from setuptools import setup
 
 
 setup(
     name='pyMSVC',
-    version='0.5.1',
+    version='0.5.2',
     url='https://github.com/kdschlosser/python_msvc',
     packages=['pyMSVC'],
     author='Kevin Schlosser',
     description='Simple to use MSVC build environment setup tool.',
     long_description=(
         'Distutils and setup tools not working properly to compile on Windows?\n'
         'Tired of having a new visual studio version break your setup program?\n'
```

