# Comparing `tmp/yunpancli-0.0.1.tar.gz` & `tmp/yunpancli-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yunpancli-0.0.1.tar", last modified: Wed May  3 10:21:51 2023, max compression
+gzip compressed data, was "yunpancli-0.0.2.tar", last modified: Wed May 24 10:16:11 2023, max compression
```

## Comparing `yunpancli-0.0.1.tar` & `yunpancli-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-03 10:21:51.561305 yunpancli-0.0.1/
--rw-r--r--   0 mac        (501) staff       (20)     1063 2023-05-02 10:51:07.000000 yunpancli-0.0.1/LICENSE
--rw-r--r--   0 mac        (501) staff       (20)      413 2023-05-03 10:21:51.561092 yunpancli-0.0.1/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-05-03 08:16:36.000000 yunpancli-0.0.1/README.md
--rw-r--r--   0 mac        (501) staff       (20)       38 2023-05-03 10:21:51.561374 yunpancli-0.0.1/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)      691 2023-05-03 08:20:21.000000 yunpancli-0.0.1/setup.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-03 10:21:51.559444 yunpancli-0.0.1/yunpancli/
--rw-r--r--   0 mac        (501) staff       (20)       39 2023-05-03 08:15:03.000000 yunpancli-0.0.1/yunpancli/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     8499 2023-05-03 10:18:36.000000 yunpancli-0.0.1/yunpancli/baidu_pan_sdk.py
--rw-r--r--   0 mac        (501) staff       (20)     6722 2023-05-03 10:08:39.000000 yunpancli-0.0.1/yunpancli/base.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-03 10:21:51.560850 yunpancli-0.0.1/yunpancli.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)      413 2023-05-03 10:21:51.000000 yunpancli-0.0.1/yunpancli.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      261 2023-05-03 10:21:51.000000 yunpancli-0.0.1/yunpancli.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-05-03 10:21:51.000000 yunpancli-0.0.1/yunpancli.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       45 2023-05-03 10:21:51.000000 yunpancli-0.0.1/yunpancli.egg-info/entry_points.txt
--rw-r--r--   0 mac        (501) staff       (20)       10 2023-05-03 10:21:51.000000 yunpancli-0.0.1/yunpancli.egg-info/top_level.txt
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-24 10:16:11.950970 yunpancli-0.0.2/
+-rw-r--r--   0 mac        (501) staff       (20)     1063 2023-05-02 10:51:07.000000 yunpancli-0.0.2/LICENSE
+-rw-r--r--   0 mac        (501) staff       (20)      413 2023-05-24 10:16:11.950795 yunpancli-0.0.2/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-05-03 08:16:36.000000 yunpancli-0.0.2/README.md
+-rw-r--r--   0 mac        (501) staff       (20)       38 2023-05-24 10:16:11.951019 yunpancli-0.0.2/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)      692 2023-05-24 10:15:55.000000 yunpancli-0.0.2/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-24 10:16:11.949968 yunpancli-0.0.2/yunpancli/
+-rw-r--r--   0 mac        (501) staff       (20)       39 2023-05-03 08:15:03.000000 yunpancli-0.0.2/yunpancli/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     8499 2023-05-03 10:18:36.000000 yunpancli-0.0.2/yunpancli/baidu_pan_sdk.py
+-rw-r--r--   0 mac        (501) staff       (20)     6723 2023-05-24 10:11:30.000000 yunpancli-0.0.2/yunpancli/base.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-24 10:16:11.950598 yunpancli-0.0.2/yunpancli.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)      413 2023-05-24 10:16:11.000000 yunpancli-0.0.2/yunpancli.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      261 2023-05-24 10:16:11.000000 yunpancli-0.0.2/yunpancli.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-05-24 10:16:11.000000 yunpancli-0.0.2/yunpancli.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       45 2023-05-24 10:16:11.000000 yunpancli-0.0.2/yunpancli.egg-info/entry_points.txt
+-rw-r--r--   0 mac        (501) staff       (20)       10 2023-05-24 10:16:11.000000 yunpancli-0.0.2/yunpancli.egg-info/top_level.txt
```

### Comparing `yunpancli-0.0.1/LICENSE` & `yunpancli-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yunpancli-0.0.1/setup.py` & `yunpancli-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="yunpancli",
     entry_points={"console_scripts": ["yunpancli=yunpancli:main"]},
-    version="0.0.1",
+    version="0.0.2",
     author="Tang Yubin",
     author_email="tang-yu-bin@qq.com",
     description="cloud storage CLI (Command Line Interface)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/aierwiki/yunpancli",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-)
+)
```

### Comparing `yunpancli-0.0.1/yunpancli/baidu_pan_sdk.py` & `yunpancli-0.0.2/yunpancli/baidu_pan_sdk.py`

 * *Files identical despite different names*

### Comparing `yunpancli-0.0.1/yunpancli/base.py` & `yunpancli-0.0.2/yunpancli/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import argparse
 import requests
 import json
 import os
 import hashlib
 from urllib.parse import urlencode
 # from yunpancli.baidu_pan_sdk import BaiduPanSDK
-from baidu_pan_sdk import BaiduPanSDK
+from .baidu_pan_sdk import BaiduPanSDK
 from loguru import logger
 # logger.remove(0)
 
 
 class PanCLI():
     ACCOUNT_CONFIG_FILE = os.path.expanduser('~/.cache/pancli/account_info.json')
```

