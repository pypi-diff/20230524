# Comparing `tmp/wipac-dev-tools-1.6.8.tar.gz` & `tmp/wipac-dev-tools-1.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wipac-dev-tools-1.6.8.tar", last modified: Mon Nov 14 22:19:42 2022, max compression
+gzip compressed data, was "wipac-dev-tools-1.6.9.tar", last modified: Mon Nov 14 22:25:07 2022, max compression
```

## Comparing `wipac-dev-tools-1.6.8.tar` & `wipac-dev-tools-1.6.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 22:19:42.984488 wipac-dev-tools-1.6.8/
--rw-r--r--   0 root         (0) root         (0)     1102 2022-11-14 22:19:40.000000 wipac-dev-tools-1.6.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)    10585 2022-11-14 22:19:42.984488 wipac-dev-tools-1.6.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9523 2022-11-14 22:19:40.000000 wipac-dev-tools-1.6.8/README.md
--rw-r--r--   0 root         (0) root         (0)     2039 2022-11-14 22:19:42.988488 wipac-dev-tools-1.6.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      104 2022-11-14 22:19:40.000000 wipac-dev-tools-1.6.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 22:19:42.984488 wipac-dev-tools-1.6.8/wipac_dev_tools/
--rw-r--r--   0 root         (0) root         (0)      882 2022-11-14 22:19:40.000000 wipac-dev-tools-1.6.8/wipac_dev_tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1172 2022-11-14 22:19:40.000000 wipac-dev-tools-1.6.8/wipac_dev_tools/argparse_tools.py
--rw-r--r--   0 root         (0) root         (0)    13574 2022-11-14 22:19:40.000000 wipac-dev-tools-1.6.8/wipac_dev_tools/enviro_tools.py
--rw-r--r--   0 root         (0) root         (0)     5935 2022-11-14 22:19:40.000000 wipac-dev-tools-1.6.8/wipac_dev_tools/logging_tools.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 22:19:40.000000 wipac-dev-tools-1.6.8/wipac_dev_tools/py.typed
--rw-r--r--   0 root         (0) root         (0)    13540 2022-11-14 22:19:40.000000 wipac-dev-tools-1.6.8/wipac_dev_tools/setup_tools.py
--rw-r--r--   0 root         (0) root         (0)      705 2022-11-14 22:19:40.000000 wipac-dev-tools-1.6.8/wipac_dev_tools/strtobool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 22:19:42.984488 wipac-dev-tools-1.6.8/wipac_dev_tools.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10585 2022-11-14 22:19:42.000000 wipac-dev-tools-1.6.8/wipac_dev_tools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      442 2022-11-14 22:19:42.000000 wipac-dev-tools-1.6.8/wipac_dev_tools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-14 22:19:42.000000 wipac-dev-tools-1.6.8/wipac_dev_tools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      103 2022-11-14 22:19:42.000000 wipac-dev-tools-1.6.8/wipac_dev_tools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2022-11-14 22:19:42.000000 wipac-dev-tools-1.6.8/wipac_dev_tools.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 22:25:07.528720 wipac-dev-tools-1.6.9/
+-rw-r--r--   0 root         (0) root         (0)     1102 2022-11-14 22:25:03.000000 wipac-dev-tools-1.6.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    10585 2022-11-14 22:25:07.528720 wipac-dev-tools-1.6.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9523 2022-11-14 22:25:03.000000 wipac-dev-tools-1.6.9/README.md
+-rw-r--r--   0 root         (0) root         (0)     2039 2022-11-14 22:25:07.528720 wipac-dev-tools-1.6.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      104 2022-11-14 22:25:03.000000 wipac-dev-tools-1.6.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 22:25:07.528720 wipac-dev-tools-1.6.9/wipac_dev_tools/
+-rw-r--r--   0 root         (0) root         (0)      882 2022-11-14 22:25:04.000000 wipac-dev-tools-1.6.9/wipac_dev_tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1172 2022-11-14 22:25:03.000000 wipac-dev-tools-1.6.9/wipac_dev_tools/argparse_tools.py
+-rw-r--r--   0 root         (0) root         (0)    13574 2022-11-14 22:25:03.000000 wipac-dev-tools-1.6.9/wipac_dev_tools/enviro_tools.py
+-rw-r--r--   0 root         (0) root         (0)     5935 2022-11-14 22:25:03.000000 wipac-dev-tools-1.6.9/wipac_dev_tools/logging_tools.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 22:25:03.000000 wipac-dev-tools-1.6.9/wipac_dev_tools/py.typed
+-rw-r--r--   0 root         (0) root         (0)    13540 2022-11-14 22:25:03.000000 wipac-dev-tools-1.6.9/wipac_dev_tools/setup_tools.py
+-rw-r--r--   0 root         (0) root         (0)      705 2022-11-14 22:25:03.000000 wipac-dev-tools-1.6.9/wipac_dev_tools/strtobool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 22:25:07.528720 wipac-dev-tools-1.6.9/wipac_dev_tools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10585 2022-11-14 22:25:07.000000 wipac-dev-tools-1.6.9/wipac_dev_tools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      442 2022-11-14 22:25:07.000000 wipac-dev-tools-1.6.9/wipac_dev_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-14 22:25:07.000000 wipac-dev-tools-1.6.9/wipac_dev_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2022-11-14 22:25:07.000000 wipac-dev-tools-1.6.9/wipac_dev_tools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2022-11-14 22:25:07.000000 wipac-dev-tools-1.6.9/wipac_dev_tools.egg-info/top_level.txt
```

### Comparing `wipac-dev-tools-1.6.8/LICENSE` & `wipac-dev-tools-1.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `wipac-dev-tools-1.6.8/PKG-INFO` & `wipac-dev-tools-1.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wipac-dev-tools
-Version: 1.6.8
+Version: 1.6.9
 Summary: Common, basic, and reusable development tools
 Home-page: https://github.com/WIPACrepo/wipac-dev-tools
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Download-URL: https://pypi.org/project/wipac-dev-tools/
 Project-URL: Tracker, https://github.com/WIPACrepo/wipac-dev-tools/issues
```

### Comparing `wipac-dev-tools-1.6.8/README.md` & `wipac-dev-tools-1.6.9/README.md`

 * *Files identical despite different names*

### Comparing `wipac-dev-tools-1.6.8/setup.cfg` & `wipac-dev-tools-1.6.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `wipac-dev-tools-1.6.8/wipac_dev_tools/__init__.py` & `wipac-dev-tools-1.6.9/wipac_dev_tools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     "SetupShop",
     "logging_tools",
     "strtobool",
     "argparse_tools",
 ]
 
 # version is a human-readable version number.
-__version__ = "1.6.8"
+__version__ = "1.6.9"
 
 # version_info is a four-tuple for programmatic comparison. The first
 # three numbers are the components of the version number. The fourth
 # is zero for an official release, positive for a development branch,
 # or negative for a release candidate or beta (after the base version
 # number has been incremented)
 version_info = (
```

### Comparing `wipac-dev-tools-1.6.8/wipac_dev_tools/argparse_tools.py` & `wipac-dev-tools-1.6.9/wipac_dev_tools/argparse_tools.py`

 * *Files identical despite different names*

### Comparing `wipac-dev-tools-1.6.8/wipac_dev_tools/enviro_tools.py` & `wipac-dev-tools-1.6.9/wipac_dev_tools/enviro_tools.py`

 * *Files identical despite different names*

### Comparing `wipac-dev-tools-1.6.8/wipac_dev_tools/logging_tools.py` & `wipac-dev-tools-1.6.9/wipac_dev_tools/logging_tools.py`

 * *Files identical despite different names*

### Comparing `wipac-dev-tools-1.6.8/wipac_dev_tools/setup_tools.py` & `wipac-dev-tools-1.6.9/wipac_dev_tools/setup_tools.py`

 * *Files identical despite different names*

### Comparing `wipac-dev-tools-1.6.8/wipac_dev_tools/strtobool.py` & `wipac-dev-tools-1.6.9/wipac_dev_tools/strtobool.py`

 * *Files identical despite different names*

### Comparing `wipac-dev-tools-1.6.8/wipac_dev_tools.egg-info/PKG-INFO` & `wipac-dev-tools-1.6.9/wipac_dev_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wipac-dev-tools
-Version: 1.6.8
+Version: 1.6.9
 Summary: Common, basic, and reusable development tools
 Home-page: https://github.com/WIPACrepo/wipac-dev-tools
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Download-URL: https://pypi.org/project/wipac-dev-tools/
 Project-URL: Tracker, https://github.com/WIPACrepo/wipac-dev-tools/issues
```

