# Comparing `tmp/hibpwned-1.3.6.tar.gz` & `tmp/hibpwned-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hibpwned-1.3.6.tar", last modified: Mon Dec 19 17:07:52 2022, max compression
+gzip compressed data, was "hibpwned-1.3.7.tar", last modified: Tue May 23 23:44:15 2023, max compression
```

## Comparing `hibpwned-1.3.6.tar` & `hibpwned-1.3.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 17:07:52.714507 hibpwned-1.3.6/
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2022-12-19 17:07:46.000000 hibpwned-1.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3850 2022-12-19 17:07:52.714507 hibpwned-1.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2022-12-19 17:07:46.000000 hibpwned-1.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 17:07:52.714507 hibpwned-1.3.6/hibpwned/
--rw-r--r--   0 runner    (1001) docker     (123)    21511 2022-12-19 17:07:46.000000 hibpwned-1.3.6/hibpwned/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 17:07:52.714507 hibpwned-1.3.6/hibpwned.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3850 2022-12-19 17:07:52.000000 hibpwned-1.3.6/hibpwned.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      252 2022-12-19 17:07:52.000000 hibpwned-1.3.6/hibpwned.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-19 17:07:52.000000 hibpwned-1.3.6/hibpwned.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-19 17:07:52.000000 hibpwned-1.3.6/hibpwned.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        9 2022-12-19 17:07:52.000000 hibpwned-1.3.6/hibpwned.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2022-12-19 17:07:52.000000 hibpwned-1.3.6/hibpwned.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2022-12-19 17:07:46.000000 hibpwned-1.3.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-19 17:07:52.714507 hibpwned-1.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2022-12-19 17:07:46.000000 hibpwned-1.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:44:15.631300 hibpwned-1.3.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-23 23:44:09.000000 hibpwned-1.3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-05-23 23:44:15.631300 hibpwned-1.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-05-23 23:44:09.000000 hibpwned-1.3.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:44:15.631300 hibpwned-1.3.7/hibpwned/
+-rw-r--r--   0 runner    (1001) docker     (123)    21511 2023-05-23 23:44:09.000000 hibpwned-1.3.7/hibpwned/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:44:15.631300 hibpwned-1.3.7/hibpwned.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-05-23 23:44:15.000000 hibpwned-1.3.7/hibpwned.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-23 23:44:15.000000 hibpwned-1.3.7/hibpwned.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 23:44:15.000000 hibpwned-1.3.7/hibpwned.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 23:44:15.000000 hibpwned-1.3.7/hibpwned.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-23 23:44:15.000000 hibpwned-1.3.7/hibpwned.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-23 23:44:15.000000 hibpwned-1.3.7/hibpwned.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-23 23:44:09.000000 hibpwned-1.3.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 23:44:15.631300 hibpwned-1.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-23 23:44:09.000000 hibpwned-1.3.7/setup.py
```

### Comparing `hibpwned-1.3.6/LICENSE` & `hibpwned-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hibpwned-1.3.6/PKG-INFO` & `hibpwned-1.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: hibpwned
-Version: 1.3.6
+Version: 1.3.7
 Summary: A human friendly Python API wrapper for haveibeenpwned.com
 Home-page: https://github.com/plasticuproject/hibpwned
 Author: plasticuproject
 Author-email: plasticuproject@pm.me
 License: GPLv3
-Download-URL: https://github.com/plasticuproject/hibpwned/archive/v1.3.6.tar.gz
+Download-URL: https://github.com/plasticuproject/hibpwned/archive/v1.3.7.tar.gz
 Description: [![build](https://github.com/plasticuproject/hibpwned/actions/workflows/tests.yml/badge.svg)](https://github.com/plasticuproject/hibpwned/actions/workflows/tests.yml)
         [![Python 3.8](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/release/python-380/)
         [![License: LGPL v3](https://img.shields.io/badge/License-LGPL%20v3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0)
         [![PyPI version](https://badge.fury.io/py/hibpwned.svg)](https://badge.fury.io/py/hibpwned)
         [![Downloads](https://pepy.tech/badge/hibpwned)](https://pepy.tech/project/hibpwned)
         [![Coverage Status](https://coveralls.io/repos/github/plasticuproject/hibpwned/badge.svg?branch=master)](https://coveralls.io/github/plasticuproject/hibpwned?branch=master)
         [![CodeQL](https://github.com/plasticuproject/hibpwned/actions/workflows/codeql.yml/badge.svg)](https://github.com/plasticuproject/hibpwned/actions/workflows/codeql.yml)
```

### Comparing `hibpwned-1.3.6/README.md` & `hibpwned-1.3.7/README.md`

 * *Files identical despite different names*

### Comparing `hibpwned-1.3.6/hibpwned/__init__.py` & `hibpwned-1.3.7/hibpwned/__init__.py`

 * *Files identical despite different names*

### Comparing `hibpwned-1.3.6/hibpwned.egg-info/PKG-INFO` & `hibpwned-1.3.7/hibpwned.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: hibpwned
-Version: 1.3.6
+Version: 1.3.7
 Summary: A human friendly Python API wrapper for haveibeenpwned.com
 Home-page: https://github.com/plasticuproject/hibpwned
 Author: plasticuproject
 Author-email: plasticuproject@pm.me
 License: GPLv3
-Download-URL: https://github.com/plasticuproject/hibpwned/archive/v1.3.6.tar.gz
+Download-URL: https://github.com/plasticuproject/hibpwned/archive/v1.3.7.tar.gz
 Description: [![build](https://github.com/plasticuproject/hibpwned/actions/workflows/tests.yml/badge.svg)](https://github.com/plasticuproject/hibpwned/actions/workflows/tests.yml)
         [![Python 3.8](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/release/python-380/)
         [![License: LGPL v3](https://img.shields.io/badge/License-LGPL%20v3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0)
         [![PyPI version](https://badge.fury.io/py/hibpwned.svg)](https://badge.fury.io/py/hibpwned)
         [![Downloads](https://pepy.tech/badge/hibpwned)](https://pepy.tech/project/hibpwned)
         [![Coverage Status](https://coveralls.io/repos/github/plasticuproject/hibpwned/badge.svg?branch=master)](https://coveralls.io/github/plasticuproject/hibpwned?branch=master)
         [![CodeQL](https://github.com/plasticuproject/hibpwned/actions/workflows/codeql.yml/badge.svg)](https://github.com/plasticuproject/hibpwned/actions/workflows/codeql.yml)
```

### Comparing `hibpwned-1.3.6/setup.py` & `hibpwned-1.3.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Setup file"""
 from setuptools import setup  # type: ignore
 
-VERSION = "1.3.6"
+VERSION = "1.3.7"
 
 with open("README.md", "r", encoding="utf-8") as fh:
     LONG_DESCRIPTION = fh.read()
 
 setup(name="hibpwned",
       packages=["hibpwned"],
       version=VERSION,
```

