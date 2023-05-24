# Comparing `tmp/wipac-telemetry-0.2.6.tar.gz` & `tmp/wipac-telemetry-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wipac-telemetry-0.2.6.tar", last modified: Mon Apr  3 15:47:38 2023, max compression
+gzip compressed data, was "wipac-telemetry-0.2.7.tar", last modified: Wed May 24 15:06:21 2023, max compression
```

## Comparing `wipac-telemetry-0.2.6.tar` & `wipac-telemetry-0.2.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 15:47:38.776714 wipac-telemetry-0.2.6/
--rw-r--r--   0 root         (0) root         (0)     1103 2023-04-03 15:47:35.000000 wipac-telemetry-0.2.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3646 2023-04-03 15:47:38.776714 wipac-telemetry-0.2.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2688 2023-04-03 15:47:35.000000 wipac-telemetry-0.2.6/README.md
--rw-r--r--   0 root         (0) root         (0)     1702 2023-04-03 15:47:38.776714 wipac-telemetry-0.2.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      104 2023-04-03 15:47:35.000000 wipac-telemetry-0.2.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 15:47:38.776714 wipac-telemetry-0.2.6/wipac_telemetry/
--rw-r--r--   0 root         (0) root         (0)      603 2023-04-03 15:47:35.000000 wipac-telemetry-0.2.6/wipac_telemetry/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-03 15:47:35.000000 wipac-telemetry-0.2.6/wipac_telemetry/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 15:47:38.776714 wipac-telemetry-0.2.6/wipac_telemetry/tracing_tools/
--rw-r--r--   0 root         (0) root         (0)     5854 2023-04-03 15:47:35.000000 wipac-telemetry-0.2.6/wipac_telemetry/tracing_tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)      795 2023-04-03 15:47:35.000000 wipac-telemetry-0.2.6/wipac_telemetry/tracing_tools/config.py
--rw-r--r--   0 root         (0) root         (0)     3709 2023-04-03 15:47:35.000000 wipac-telemetry-0.2.6/wipac_telemetry/tracing_tools/events.py
--rw-r--r--   0 root         (0) root         (0)     3762 2023-04-03 15:47:35.000000 wipac-telemetry-0.2.6/wipac_telemetry/tracing_tools/propagations.py
--rw-r--r--   0 root         (0) root         (0)    20820 2023-04-03 15:47:35.000000 wipac-telemetry-0.2.6/wipac_telemetry/tracing_tools/spans.py
--rw-r--r--   0 root         (0) root         (0)     6433 2023-04-03 15:47:35.000000 wipac-telemetry-0.2.6/wipac_telemetry/tracing_tools/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 15:47:38.776714 wipac-telemetry-0.2.6/wipac_telemetry.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3646 2023-04-03 15:47:38.000000 wipac-telemetry-0.2.6/wipac_telemetry.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      529 2023-04-03 15:47:38.000000 wipac-telemetry-0.2.6/wipac_telemetry.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-03 15:47:38.000000 wipac-telemetry-0.2.6/wipac_telemetry.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      160 2023-04-03 15:47:38.000000 wipac-telemetry-0.2.6/wipac_telemetry.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-04-03 15:47:38.000000 wipac-telemetry-0.2.6/wipac_telemetry.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:06:21.888998 wipac-telemetry-0.2.7/
+-rw-r--r--   0 root         (0) root         (0)     1103 2023-05-24 15:06:19.000000 wipac-telemetry-0.2.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3646 2023-05-24 15:06:21.888998 wipac-telemetry-0.2.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2688 2023-05-24 15:06:19.000000 wipac-telemetry-0.2.7/README.md
+-rw-r--r--   0 root         (0) root         (0)     1702 2023-05-24 15:06:21.888998 wipac-telemetry-0.2.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      104 2023-05-24 15:06:19.000000 wipac-telemetry-0.2.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:06:21.884998 wipac-telemetry-0.2.7/wipac_telemetry/
+-rw-r--r--   0 root         (0) root         (0)      603 2023-05-24 15:06:19.000000 wipac-telemetry-0.2.7/wipac_telemetry/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 15:06:19.000000 wipac-telemetry-0.2.7/wipac_telemetry/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:06:21.888998 wipac-telemetry-0.2.7/wipac_telemetry/tracing_tools/
+-rw-r--r--   0 root         (0) root         (0)     5854 2023-05-24 15:06:19.000000 wipac-telemetry-0.2.7/wipac_telemetry/tracing_tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      795 2023-05-24 15:06:19.000000 wipac-telemetry-0.2.7/wipac_telemetry/tracing_tools/config.py
+-rw-r--r--   0 root         (0) root         (0)     3709 2023-05-24 15:06:19.000000 wipac-telemetry-0.2.7/wipac_telemetry/tracing_tools/events.py
+-rw-r--r--   0 root         (0) root         (0)     3762 2023-05-24 15:06:19.000000 wipac-telemetry-0.2.7/wipac_telemetry/tracing_tools/propagations.py
+-rw-r--r--   0 root         (0) root         (0)    20820 2023-05-24 15:06:19.000000 wipac-telemetry-0.2.7/wipac_telemetry/tracing_tools/spans.py
+-rw-r--r--   0 root         (0) root         (0)     6433 2023-05-24 15:06:19.000000 wipac-telemetry-0.2.7/wipac_telemetry/tracing_tools/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:06:21.884998 wipac-telemetry-0.2.7/wipac_telemetry.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3646 2023-05-24 15:06:21.000000 wipac-telemetry-0.2.7/wipac_telemetry.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      529 2023-05-24 15:06:21.000000 wipac-telemetry-0.2.7/wipac_telemetry.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 15:06:21.000000 wipac-telemetry-0.2.7/wipac_telemetry.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      160 2023-05-24 15:06:21.000000 wipac-telemetry-0.2.7/wipac_telemetry.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-05-24 15:06:21.000000 wipac-telemetry-0.2.7/wipac_telemetry.egg-info/top_level.txt
```

### Comparing `wipac-telemetry-0.2.6/LICENSE` & `wipac-telemetry-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `wipac-telemetry-0.2.6/PKG-INFO` & `wipac-telemetry-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wipac-telemetry
-Version: 0.2.6
+Version: 0.2.7
 Summary: WIPAC Telemetry: Monitoring/Tracing Applications, Supporting Infrastructures, and Services
 Home-page: https://github.com/WIPACrepo/wipac-telemetry
 Download-URL: https://pypi.org/project/wipac-telemetry/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/WIPACrepo/wipac-telemetry/issues
```

### Comparing `wipac-telemetry-0.2.6/README.md` & `wipac-telemetry-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `wipac-telemetry-0.2.6/setup.cfg` & `wipac-telemetry-0.2.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `wipac-telemetry-0.2.6/wipac_telemetry/__init__.py` & `wipac-telemetry-0.2.7/wipac_telemetry/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Top-Level Init."""
 
 from . import tracing_tools  # noqa
 
 __all__ = ["tracing_tools"]
 
 # version is a human-readable version number.
-__version__ = "0.2.6"
+__version__ = "0.2.7"
 
 # version_info is a four-tuple for programmatic comparison. The first
 # three numbers are the components of the version number. The fourth
 # is zero for an official release, positive for a development branch,
 # or negative for a release candidate or beta (after the base version
 # number has been incremented)
```

### Comparing `wipac-telemetry-0.2.6/wipac_telemetry/tracing_tools/__init__.py` & `wipac-telemetry-0.2.7/wipac_telemetry/tracing_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `wipac-telemetry-0.2.6/wipac_telemetry/tracing_tools/config.py` & `wipac-telemetry-0.2.7/wipac_telemetry/tracing_tools/config.py`

 * *Files identical despite different names*

### Comparing `wipac-telemetry-0.2.6/wipac_telemetry/tracing_tools/events.py` & `wipac-telemetry-0.2.7/wipac_telemetry/tracing_tools/events.py`

 * *Files identical despite different names*

### Comparing `wipac-telemetry-0.2.6/wipac_telemetry/tracing_tools/propagations.py` & `wipac-telemetry-0.2.7/wipac_telemetry/tracing_tools/propagations.py`

 * *Files identical despite different names*

### Comparing `wipac-telemetry-0.2.6/wipac_telemetry/tracing_tools/spans.py` & `wipac-telemetry-0.2.7/wipac_telemetry/tracing_tools/spans.py`

 * *Files identical despite different names*

### Comparing `wipac-telemetry-0.2.6/wipac_telemetry/tracing_tools/utils.py` & `wipac-telemetry-0.2.7/wipac_telemetry/tracing_tools/utils.py`

 * *Files identical despite different names*

### Comparing `wipac-telemetry-0.2.6/wipac_telemetry.egg-info/PKG-INFO` & `wipac-telemetry-0.2.7/wipac_telemetry.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wipac-telemetry
-Version: 0.2.6
+Version: 0.2.7
 Summary: WIPAC Telemetry: Monitoring/Tracing Applications, Supporting Infrastructures, and Services
 Home-page: https://github.com/WIPACrepo/wipac-telemetry
 Download-URL: https://pypi.org/project/wipac-telemetry/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/WIPACrepo/wipac-telemetry/issues
```

### Comparing `wipac-telemetry-0.2.6/wipac_telemetry.egg-info/SOURCES.txt` & `wipac-telemetry-0.2.7/wipac_telemetry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

