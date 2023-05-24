# Comparing `tmp/pyopnsenseapi-0.0.1.tar.gz` & `tmp/pyopnsenseapi-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyopnsenseapi-0.0.1.tar", last modified: Tue May 23 15:22:38 2023, max compression
+gzip compressed data, was "pyopnsenseapi-0.1.0.tar", last modified: Wed May 24 09:35:32 2023, max compression
```

## Comparing `pyopnsenseapi-0.0.1.tar` & `pyopnsenseapi-0.1.0.tar`

### file list

```diff
@@ -1,49 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:22:38.085335 pyopnsenseapi-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:22:38.073334 pyopnsenseapi-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:22:38.077335 pyopnsenseapi-0.0.1/.github/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1327 2023-05-23 15:22:29.000000 pyopnsenseapi-0.0.1/.github/scripts/release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:22:38.077335 pyopnsenseapi-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-23 15:22:29.000000 pyopnsenseapi-0.0.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-23 15:22:29.000000 pyopnsenseapi-0.0.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-23 15:22:29.000000 pyopnsenseapi-0.0.1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:22:38.077335 pyopnsenseapi-0.0.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-23 15:22:29.000000 pyopnsenseapi-0.0.1/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-23 15:22:29.000000 pyopnsenseapi-0.0.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-23 15:22:29.000000 pyopnsenseapi-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-23 15:22:38.085335 pyopnsenseapi-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-05-23 15:22:29.000000 pyopnsenseapi-0.0.1/README
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:22:38.073334 pyopnsenseapi-0.0.1/doc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:22:38.081335 pyopnsenseapi-0.0.1/doc/source/
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-23 15:22:29.000000 pyopnsenseapi-0.0.1/doc/source/api.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     2708 2023-05-23 15:22:29.000000 pyopnsenseapi-0.0.1/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-23 15:22:29.000000 pyopnsenseapi-0.0.1/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-23 15:22:29.000000 pyopnsenseapi-0.0.1/doc/source/readme.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:22:38.081335 pyopnsenseapi-0.0.1/pyopnsenseapi/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-23 15:22:29.000000 pyopnsenseapi-0.0.1/pyopnsenseapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-23 15:22:29.000000 pyopnsenseapi-0.0.1/pyopnsenseapi/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:22:38.081335 pyopnsenseapi-0.0.1/pyopnsenseapi/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-23 15:22:29.000000 pyopnsenseapi-0.0.1/pyopnsenseapi/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-23 15:22:29.000000 pyopnsenseapi-0.0.1/pyopnsenseapi/modules/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:22:38.085335 pyopnsenseapi-0.0.1/pyopnsenseapi/modules/diagnostics/
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-23 15:22:29.000000 pyopnsenseapi-0.0.1/pyopnsenseapi/modules/diagnostics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-23 15:22:29.000000 pyopnsenseapi-0.0.1/pyopnsenseapi/modules/diagnostics/activity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-05-23 15:22:29.000000 pyopnsenseapi-0.0.1/pyopnsenseapi/modules/diagnostics/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-23 15:22:29.000000 pyopnsenseapi-0.0.1/pyopnsenseapi/modules/diagnostics/dns.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-23 15:22:29.000000 pyopnsenseapi-0.0.1/pyopnsenseapi/modules/diagnostics/dns_diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-05-23 15:22:29.000000 pyopnsenseapi-0.0.1/pyopnsenseapi/modules/diagnostics/firewall.py
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-05-23 15:22:29.000000 pyopnsenseapi-0.0.1/pyopnsenseapi/modules/diagnostics/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-23 15:22:29.000000 pyopnsenseapi-0.0.1/pyopnsenseapi/modules/diagnostics/netflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-23 15:22:29.000000 pyopnsenseapi-0.0.1/pyopnsenseapi/modules/diagnostics/networkinsight.py
--rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-05-23 15:22:29.000000 pyopnsenseapi-0.0.1/pyopnsenseapi/modules/diagnostics/packet_capture.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-23 15:22:29.000000 pyopnsenseapi-0.0.1/pyopnsenseapi/modules/diagnostics/system.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-23 15:22:29.000000 pyopnsenseapi-0.0.1/pyopnsenseapi/modules/diagnostics/systemhealth.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-23 15:22:29.000000 pyopnsenseapi-0.0.1/pyopnsenseapi/modules/diagnostics/traffic.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-23 15:22:29.000000 pyopnsenseapi-0.0.1/pyopnsenseapi/modules/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:22:38.081335 pyopnsenseapi-0.0.1/pyopnsenseapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-23 15:22:38.000000 pyopnsenseapi-0.0.1/pyopnsenseapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-23 15:22:38.000000 pyopnsenseapi-0.0.1/pyopnsenseapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 15:22:38.000000 pyopnsenseapi-0.0.1/pyopnsenseapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-23 15:22:38.000000 pyopnsenseapi-0.0.1/pyopnsenseapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-23 15:22:29.000000 pyopnsenseapi-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-23 15:22:29.000000 pyopnsenseapi-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-23 15:22:38.085335 pyopnsenseapi-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:35:32.526001 pyopnsenseapi-0.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:35:32.522001 pyopnsenseapi-0.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:35:32.522001 pyopnsenseapi-0.1.0/.github/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1327 2023-05-24 09:35:24.000000 pyopnsenseapi-0.1.0/.github/scripts/release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:35:32.522001 pyopnsenseapi-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-24 09:35:24.000000 pyopnsenseapi-0.1.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-24 09:35:24.000000 pyopnsenseapi-0.1.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-24 09:35:24.000000 pyopnsenseapi-0.1.0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:35:32.522001 pyopnsenseapi-0.1.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-24 09:35:24.000000 pyopnsenseapi-0.1.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-24 09:35:24.000000 pyopnsenseapi-0.1.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-24 09:35:24.000000 pyopnsenseapi-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-24 09:35:32.526001 pyopnsenseapi-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-05-24 09:35:24.000000 pyopnsenseapi-0.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:35:32.522001 pyopnsenseapi-0.1.0/doc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:35:32.522001 pyopnsenseapi-0.1.0/doc/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-24 09:35:24.000000 pyopnsenseapi-0.1.0/doc/source/api.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2708 2023-05-24 09:35:24.000000 pyopnsenseapi-0.1.0/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-24 09:35:24.000000 pyopnsenseapi-0.1.0/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-24 09:35:24.000000 pyopnsenseapi-0.1.0/doc/source/readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:35:32.522001 pyopnsenseapi-0.1.0/pyopnsenseapi/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-24 09:35:24.000000 pyopnsenseapi-0.1.0/pyopnsenseapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-24 09:35:24.000000 pyopnsenseapi-0.1.0/pyopnsenseapi/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:35:32.522001 pyopnsenseapi-0.1.0/pyopnsenseapi/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-24 09:35:24.000000 pyopnsenseapi-0.1.0/pyopnsenseapi/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-24 09:35:24.000000 pyopnsenseapi-0.1.0/pyopnsenseapi/modules/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:35:32.526001 pyopnsenseapi-0.1.0/pyopnsenseapi/modules/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-24 09:35:24.000000 pyopnsenseapi-0.1.0/pyopnsenseapi/modules/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-24 09:35:24.000000 pyopnsenseapi-0.1.0/pyopnsenseapi/modules/core/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-05-24 09:35:24.000000 pyopnsenseapi-0.1.0/pyopnsenseapi/modules/core/firmware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-24 09:35:24.000000 pyopnsenseapi-0.1.0/pyopnsenseapi/modules/core/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-24 09:35:24.000000 pyopnsenseapi-0.1.0/pyopnsenseapi/modules/core/system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:35:32.526001 pyopnsenseapi-0.1.0/pyopnsenseapi/modules/diagnostics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-24 09:35:24.000000 pyopnsenseapi-0.1.0/pyopnsenseapi/modules/diagnostics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-24 09:35:24.000000 pyopnsenseapi-0.1.0/pyopnsenseapi/modules/diagnostics/activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-05-24 09:35:24.000000 pyopnsenseapi-0.1.0/pyopnsenseapi/modules/diagnostics/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-24 09:35:24.000000 pyopnsenseapi-0.1.0/pyopnsenseapi/modules/diagnostics/dns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-24 09:35:24.000000 pyopnsenseapi-0.1.0/pyopnsenseapi/modules/diagnostics/dns_diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-05-24 09:35:24.000000 pyopnsenseapi-0.1.0/pyopnsenseapi/modules/diagnostics/firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-05-24 09:35:24.000000 pyopnsenseapi-0.1.0/pyopnsenseapi/modules/diagnostics/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-24 09:35:24.000000 pyopnsenseapi-0.1.0/pyopnsenseapi/modules/diagnostics/netflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-24 09:35:24.000000 pyopnsenseapi-0.1.0/pyopnsenseapi/modules/diagnostics/networkinsight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-05-24 09:35:24.000000 pyopnsenseapi-0.1.0/pyopnsenseapi/modules/diagnostics/packet_capture.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-24 09:35:24.000000 pyopnsenseapi-0.1.0/pyopnsenseapi/modules/diagnostics/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-24 09:35:24.000000 pyopnsenseapi-0.1.0/pyopnsenseapi/modules/diagnostics/systemhealth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-24 09:35:24.000000 pyopnsenseapi-0.1.0/pyopnsenseapi/modules/diagnostics/traffic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-24 09:35:24.000000 pyopnsenseapi-0.1.0/pyopnsenseapi/modules/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:35:32.522001 pyopnsenseapi-0.1.0/pyopnsenseapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-24 09:35:32.000000 pyopnsenseapi-0.1.0/pyopnsenseapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-24 09:35:32.000000 pyopnsenseapi-0.1.0/pyopnsenseapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 09:35:32.000000 pyopnsenseapi-0.1.0/pyopnsenseapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-24 09:35:32.000000 pyopnsenseapi-0.1.0/pyopnsenseapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-24 09:35:24.000000 pyopnsenseapi-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-24 09:35:24.000000 pyopnsenseapi-0.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-24 09:35:32.526001 pyopnsenseapi-0.1.0/setup.cfg
```

### Comparing `pyopnsenseapi-0.0.1/.github/scripts/release.py` & `pyopnsenseapi-0.1.0/.github/scripts/release.py`

 * *Files identical despite different names*

### Comparing `pyopnsenseapi-0.0.1/.gitignore` & `pyopnsenseapi-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pyopnsenseapi-0.0.1/LICENSE` & `pyopnsenseapi-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyopnsenseapi-0.0.1/PKG-INFO` & `pyopnsenseapi-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyopnsenseapi
-Version: 0.0.1
+Version: 0.1.0
 Summary: Another Python OPNsense API library
 Home-page: https://github.com/11harveyj/pyopnsenseapi
 Project-URL: Bug Tracker, https://github.com/11harveyj/pyopnsenseapi/issues
 Project-URL: Changelog, https://github.com/11harveyj/pyopnsenseapi/releases
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Developers
```

### Comparing `pyopnsenseapi-0.0.1/README` & `pyopnsenseapi-0.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `pyopnsenseapi-0.0.1/doc/source/api.rst` & `pyopnsenseapi-0.1.0/doc/source/api.rst`

 * *Files identical despite different names*

### Comparing `pyopnsenseapi-0.0.1/doc/source/conf.py` & `pyopnsenseapi-0.1.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `pyopnsenseapi-0.0.1/pyopnsenseapi/modules/__init__.py` & `pyopnsenseapi-0.1.0/pyopnsenseapi/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `pyopnsenseapi-0.0.1/pyopnsenseapi/modules/client.py` & `pyopnsenseapi-0.1.0/pyopnsenseapi/modules/client.py`

 * *Files identical despite different names*

### Comparing `pyopnsenseapi-0.0.1/pyopnsenseapi/modules/diagnostics/__init__.py` & `pyopnsenseapi-0.1.0/pyopnsenseapi/modules/diagnostics/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import sys
 import importlib
 import inspect
 import enum
 from pyopnsenseapi.modules import Modules
 from .const import DIAGNOSTICS
 
-
 class Diagnostics():
     """Diagnostics module."""
 
     is_module = True
 
     def _controller_discovery(self, base):
         """Discovers all controllers under this module."""
```

### Comparing `pyopnsenseapi-0.0.1/pyopnsenseapi/modules/diagnostics/activity.py` & `pyopnsenseapi-0.1.0/pyopnsenseapi/modules/diagnostics/activity.py`

 * *Files identical despite different names*

### Comparing `pyopnsenseapi-0.0.1/pyopnsenseapi/modules/diagnostics/const.py` & `pyopnsenseapi-0.1.0/pyopnsenseapi/modules/diagnostics/const.py`

 * *Files identical despite different names*

### Comparing `pyopnsenseapi-0.0.1/pyopnsenseapi/modules/diagnostics/dns_diagnostics.py` & `pyopnsenseapi-0.1.0/pyopnsenseapi/modules/diagnostics/dns_diagnostics.py`

 * *Files identical despite different names*

### Comparing `pyopnsenseapi-0.0.1/pyopnsenseapi/modules/diagnostics/firewall.py` & `pyopnsenseapi-0.1.0/pyopnsenseapi/modules/diagnostics/firewall.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,67 +18,58 @@
     """OPNsense diagnostics.firewall module."""
 
     is_controller = True
 
     def __init__(self, client) -> None:
         self._client = client
 
-    
     def delete_state(self, stateid: str, creatorid: str):
         """Deletes a given state."""
         return self._client.post(
             endpoint=ENDPOINTS.get(FIREWALL_DEL_STATE),
             body={"stateid": stateid, "creatorid": creatorid}
         )
 
-    
     def flush_sources(self):
         """Flushes sources."""
         return self._client.post(
             endpoint=ENDPOINTS.get(FIREWALL_FLUSH_SOURCES),
             body={}
         )
 
-    
     def flush_states(self):
         """Flushes states."""
         return self._client.post(
             endpoint=ENDPOINTS.get(FIREWALL_FLUSH_STATES),
             body={}
         )
 
-    
     def kill_states(self):
         """Kills states."""
         return self._client.post(
             endpoint=ENDPOINTS.get(FIREWALL_KILL_STATES),
             body={}
         )
 
-    
     def get_rule_ids(self):
         """Gets a list of rule IDs."""
         return self._client.get(ENDPOINTS.get(FIREWALL_LIST_RULE_IDS))
 
-    
     def get_firewall_log(self):
         """Returns the firewall log."""
         return self._client.get(ENDPOINTS.get(FIREWALL_LOG))
 
-    
     def get_firewall_log_filters(self):
         """Returns firewall log filters?."""
         return self._client.get(ENDPOINTS.get(FIREWALL_LOG_FILTERS))
 
-    
     def get_pf_statistics(self, section: str="null"):
         """Returns pfStatistics."""
         return self._client.get(str(ENDPOINTS.get(FIREWALL_PF_STATS)).format(section))
 
-    
     def search_pf_top(self,
                       row_count: int = 500,
                       current_page: int = 1,
                       rule_id: str = "",
                       sort: str = "",
                       search_phrase: str = ""):
         """Returns pfTop."""
@@ -88,15 +79,14 @@
                 "searchPhrase": search_phrase,
                 "rowCount": row_count,
                 "current": current_page,
                 "ruleid": rule_id,
                 "sort": sort
             })
 
-    
     def search_states(self,
                       row_count: int = 500,
                       current_page: int = 1,
                       rule_id: str = "",
                       sort: str = "",
                       search_phrase: str = ""):
         """Returns pfTop."""
@@ -106,11 +96,10 @@
                 "searchPhrase": search_phrase,
                 "rowCount": row_count,
                 "current": current_page,
                 "ruleid": rule_id,
                 "sort": sort
             })
 
-    
     def get_statistics(self):
         """Returns statistics."""
         return self._client.get(ENDPOINTS.get(FIREWALL_STATS))
```

### Comparing `pyopnsenseapi-0.0.1/pyopnsenseapi/modules/diagnostics/interface.py` & `pyopnsenseapi-0.1.0/pyopnsenseapi/modules/diagnostics/interface.py`

 * *Files identical despite different names*

### Comparing `pyopnsenseapi-0.0.1/pyopnsenseapi/modules/diagnostics/netflow.py` & `pyopnsenseapi-0.1.0/pyopnsenseapi/modules/diagnostics/netflow.py`

 * *Files identical despite different names*

### Comparing `pyopnsenseapi-0.0.1/pyopnsenseapi/modules/diagnostics/networkinsight.py` & `pyopnsenseapi-0.1.0/pyopnsenseapi/modules/diagnostics/networkinsight.py`

 * *Files identical despite different names*

### Comparing `pyopnsenseapi-0.0.1/pyopnsenseapi/modules/diagnostics/packet_capture.py` & `pyopnsenseapi-0.1.0/pyopnsenseapi/modules/diagnostics/packet_capture.py`

 * *Files identical despite different names*

### Comparing `pyopnsenseapi-0.0.1/pyopnsenseapi/modules/diagnostics/systemhealth.py` & `pyopnsenseapi-0.1.0/pyopnsenseapi/modules/diagnostics/systemhealth.py`

 * *Files identical despite different names*

### Comparing `pyopnsenseapi-0.0.1/pyopnsenseapi/modules/diagnostics/traffic.py` & `pyopnsenseapi-0.1.0/pyopnsenseapi/modules/diagnostics/traffic.py`

 * *Files identical despite different names*

### Comparing `pyopnsenseapi-0.0.1/pyopnsenseapi.egg-info/PKG-INFO` & `pyopnsenseapi-0.1.0/pyopnsenseapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyopnsenseapi
-Version: 0.0.1
+Version: 0.1.0
 Summary: Another Python OPNsense API library
 Home-page: https://github.com/11harveyj/pyopnsenseapi
 Project-URL: Bug Tracker, https://github.com/11harveyj/pyopnsenseapi/issues
 Project-URL: Changelog, https://github.com/11harveyj/pyopnsenseapi/releases
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Developers
```

### Comparing `pyopnsenseapi-0.0.1/pyopnsenseapi.egg-info/SOURCES.txt` & `pyopnsenseapi-0.1.0/pyopnsenseapi.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .gitignore
 LICENSE
-README
+README.rst
 pyproject.toml
 requirements.txt
 setup.cfg
 .github/scripts/release.py
 .github/workflows/publish.yml
 .github/workflows/release.yml
 .vscode/launch.json
@@ -18,14 +18,19 @@
 pyopnsenseapi.egg-info/PKG-INFO
 pyopnsenseapi.egg-info/SOURCES.txt
 pyopnsenseapi.egg-info/dependency_links.txt
 pyopnsenseapi.egg-info/top_level.txt
 pyopnsenseapi/modules/__init__.py
 pyopnsenseapi/modules/client.py
 pyopnsenseapi/modules/enums.py
+pyopnsenseapi/modules/core/__init__.py
+pyopnsenseapi/modules/core/const.py
+pyopnsenseapi/modules/core/firmware.py
+pyopnsenseapi/modules/core/service.py
+pyopnsenseapi/modules/core/system.py
 pyopnsenseapi/modules/diagnostics/__init__.py
 pyopnsenseapi/modules/diagnostics/activity.py
 pyopnsenseapi/modules/diagnostics/const.py
 pyopnsenseapi/modules/diagnostics/dns.py
 pyopnsenseapi/modules/diagnostics/dns_diagnostics.py
 pyopnsenseapi/modules/diagnostics/firewall.py
 pyopnsenseapi/modules/diagnostics/interface.py
```

