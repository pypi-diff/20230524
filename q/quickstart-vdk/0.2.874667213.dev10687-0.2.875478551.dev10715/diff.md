# Comparing `tmp/quickstart-vdk-0.2.874667213.dev10687.tar.gz` & `tmp/quickstart-vdk-0.2.875478551.dev10715.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickstart-vdk-0.2.874667213.dev10687.tar", last modified: Mon May 22 12:58:39 2023, max compression
+gzip compressed data, was "quickstart-vdk-0.2.875478551.dev10715.tar", last modified: Tue May 23 04:22:54 2023, max compression
```

## Comparing `quickstart-vdk-0.2.874667213.dev10687.tar` & `quickstart-vdk-0.2.875478551.dev10715.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 12:58:39.918709 quickstart-vdk-0.2.874667213.dev10687/
--rw-r--r--   0 root         (0) root         (0)     1017 2023-05-22 12:58:39.918709 quickstart-vdk-0.2.874667213.dev10687/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      386 2023-05-22 12:58:19.000000 quickstart-vdk-0.2.874667213.dev10687/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 12:58:39.918709 quickstart-vdk-0.2.874667213.dev10687/quickstart_vdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1017 2023-05-22 12:58:39.000000 quickstart-vdk-0.2.874667213.dev10687/quickstart_vdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      227 2023-05-22 12:58:39.000000 quickstart-vdk-0.2.874667213.dev10687/quickstart_vdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 12:58:39.000000 quickstart-vdk-0.2.874667213.dev10687/quickstart_vdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      105 2023-05-22 12:58:39.000000 quickstart-vdk-0.2.874667213.dev10687/quickstart_vdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-05-22 12:58:39.000000 quickstart-vdk-0.2.874667213.dev10687/quickstart_vdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-22 12:58:39.918709 quickstart-vdk-0.2.874667213.dev10687/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1300 2023-05-22 12:58:29.000000 quickstart-vdk-0.2.874667213.dev10687/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 12:58:39.918709 quickstart-vdk-0.2.874667213.dev10687/tests/
--rw-rw-rw-   0 root         (0) root         (0)      114 2023-05-22 12:58:19.000000 quickstart-vdk-0.2.874667213.dev10687/tests/test_dummy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 04:22:54.818367 quickstart-vdk-0.2.875478551.dev10715/
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-05-23 04:22:54.818367 quickstart-vdk-0.2.875478551.dev10715/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      386 2023-05-23 04:20:03.000000 quickstart-vdk-0.2.875478551.dev10715/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 04:22:54.818367 quickstart-vdk-0.2.875478551.dev10715/quickstart_vdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-05-23 04:22:54.000000 quickstart-vdk-0.2.875478551.dev10715/quickstart_vdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      227 2023-05-23 04:22:54.000000 quickstart-vdk-0.2.875478551.dev10715/quickstart_vdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 04:22:54.000000 quickstart-vdk-0.2.875478551.dev10715/quickstart_vdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2023-05-23 04:22:54.000000 quickstart-vdk-0.2.875478551.dev10715/quickstart_vdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-05-23 04:22:54.000000 quickstart-vdk-0.2.875478551.dev10715/quickstart_vdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-23 04:22:54.818367 quickstart-vdk-0.2.875478551.dev10715/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1300 2023-05-23 04:22:44.000000 quickstart-vdk-0.2.875478551.dev10715/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 04:22:54.818367 quickstart-vdk-0.2.875478551.dev10715/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      114 2023-05-23 04:20:03.000000 quickstart-vdk-0.2.875478551.dev10715/tests/test_dummy.py
```

### Comparing `quickstart-vdk-0.2.874667213.dev10687/PKG-INFO` & `quickstart-vdk-0.2.875478551.dev10715/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstart-vdk
-Version: 0.2.874667213.dev10687
+Version: 0.2.875478551.dev10715
 Summary: Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quickstart-vdk-0.2.874667213.dev10687/quickstart_vdk.egg-info/PKG-INFO` & `quickstart-vdk-0.2.875478551.dev10715/quickstart_vdk.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstart-vdk
-Version: 0.2.874667213.dev10687
+Version: 0.2.875478551.dev10715
 Summary: Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quickstart-vdk-0.2.874667213.dev10687/setup.py` & `quickstart-vdk-0.2.875478551.dev10715/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import pathlib
 
 import setuptools
 
 
-__version__ = "0.2.874667213.dev10687"
+__version__ = "0.2.875478551.dev10715"
 
 setuptools.setup(
     name="quickstart-vdk",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.",
     long_description=pathlib.Path("README.md").read_text(),
```

