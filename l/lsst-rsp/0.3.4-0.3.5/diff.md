# Comparing `tmp/lsst-rsp-0.3.4.tar.gz` & `tmp/lsst-rsp-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsst-rsp-0.3.4.tar", last modified: Thu Apr 27 21:04:46 2023, max compression
+gzip compressed data, was "lsst-rsp-0.3.5.tar", last modified: Wed May 24 20:52:36 2023, max compression
```

## Comparing `lsst-rsp-0.3.4.tar` & `lsst-rsp-0.3.5.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:04:46.573356 lsst-rsp-0.3.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:04:46.569357 lsst-rsp-0.3.4/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-27 21:04:30.000000 lsst-rsp-0.3.4/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:04:46.569357 lsst-rsp-0.3.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-04-27 21:04:30.000000 lsst-rsp-0.3.4/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-27 21:04:30.000000 lsst-rsp-0.3.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-27 21:04:30.000000 lsst-rsp-0.3.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-27 21:04:30.000000 lsst-rsp-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:04:30.000000 lsst-rsp-0.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-27 21:04:30.000000 lsst-rsp-0.3.4/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-04-27 21:04:46.573356 lsst-rsp-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-27 21:04:30.000000 lsst-rsp-0.3.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-27 21:04:30.000000 lsst-rsp-0.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-04-27 21:04:46.573356 lsst-rsp-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-27 21:04:30.000000 lsst-rsp-0.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:04:46.569357 lsst-rsp-0.3.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:04:46.569357 lsst-rsp-0.3.4/src/jupyterlabutils/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-27 21:04:30.000000 lsst-rsp-0.3.4/src/jupyterlabutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:04:46.569357 lsst-rsp-0.3.4/src/jupyterlabutils/notebook/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-27 21:04:30.000000 lsst-rsp-0.3.4/src/jupyterlabutils/notebook/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:04:46.569357 lsst-rsp-0.3.4/src/lsst/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-27 21:04:30.000000 lsst-rsp-0.3.4/src/lsst/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:04:46.569357 lsst-rsp-0.3.4/src/lsst/rsp/
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-27 21:04:30.000000 lsst-rsp-0.3.4/src/lsst/rsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-04-27 21:04:30.000000 lsst-rsp-0.3.4/src/lsst/rsp/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-27 21:04:30.000000 lsst-rsp-0.3.4/src/lsst/rsp/forwarder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-04-27 21:04:30.000000 lsst-rsp-0.3.4/src/lsst/rsp/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-04-27 21:04:30.000000 lsst-rsp-0.3.4/src/lsst/rsp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:04:46.569357 lsst-rsp-0.3.4/src/lsst_rsp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-04-27 21:04:46.000000 lsst-rsp-0.3.4/src/lsst_rsp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-27 21:04:46.000000 lsst-rsp-0.3.4/src/lsst_rsp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 21:04:46.000000 lsst-rsp-0.3.4/src/lsst_rsp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 21:04:46.000000 lsst-rsp-0.3.4/src/lsst_rsp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-27 21:04:46.000000 lsst-rsp-0.3.4/src/lsst_rsp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-27 21:04:46.000000 lsst-rsp-0.3.4/src/lsst_rsp.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:04:46.573356 lsst-rsp-0.3.4/src/rubin_jupyter_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:04:30.000000 lsst-rsp-0.3.4/src/rubin_jupyter_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:04:46.573356 lsst-rsp-0.3.4/src/rubin_jupyter_utils/lab/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-27 21:04:30.000000 lsst-rsp-0.3.4/src/rubin_jupyter_utils/lab/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:04:46.573356 lsst-rsp-0.3.4/src/rubin_jupyter_utils/lab/notebook/
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-27 21:04:30.000000 lsst-rsp-0.3.4/src/rubin_jupyter_utils/lab/notebook/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:04:46.573356 lsst-rsp-0.3.4/src/rubin_jupyter_utils/lab/notebook/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-27 21:04:30.000000 lsst-rsp-0.3.4/src/rubin_jupyter_utils/lab/notebook/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:04:46.573356 lsst-rsp-0.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-27 21:04:30.000000 lsst-rsp-0.3.4/tests/utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-27 21:04:30.000000 lsst-rsp-0.3.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:52:36.148432 lsst-rsp-0.3.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:52:36.148432 lsst-rsp-0.3.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-24 20:52:21.000000 lsst-rsp-0.3.5/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:52:36.148432 lsst-rsp-0.3.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-05-24 20:52:21.000000 lsst-rsp-0.3.5/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-24 20:52:21.000000 lsst-rsp-0.3.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-24 20:52:21.000000 lsst-rsp-0.3.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-24 20:52:21.000000 lsst-rsp-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:52:21.000000 lsst-rsp-0.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-24 20:52:21.000000 lsst-rsp-0.3.5/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-05-24 20:52:36.148432 lsst-rsp-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-24 20:52:21.000000 lsst-rsp-0.3.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-24 20:52:21.000000 lsst-rsp-0.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-05-24 20:52:36.152432 lsst-rsp-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-24 20:52:21.000000 lsst-rsp-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:52:36.144432 lsst-rsp-0.3.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:52:36.148432 lsst-rsp-0.3.5/src/jupyterlabutils/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-24 20:52:21.000000 lsst-rsp-0.3.5/src/jupyterlabutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:52:36.148432 lsst-rsp-0.3.5/src/jupyterlabutils/notebook/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-24 20:52:21.000000 lsst-rsp-0.3.5/src/jupyterlabutils/notebook/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:52:36.148432 lsst-rsp-0.3.5/src/lsst/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-24 20:52:21.000000 lsst-rsp-0.3.5/src/lsst/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:52:36.148432 lsst-rsp-0.3.5/src/lsst/rsp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-24 20:52:21.000000 lsst-rsp-0.3.5/src/lsst/rsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-05-24 20:52:21.000000 lsst-rsp-0.3.5/src/lsst/rsp/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-05-24 20:52:21.000000 lsst-rsp-0.3.5/src/lsst/rsp/forwarder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-05-24 20:52:21.000000 lsst-rsp-0.3.5/src/lsst/rsp/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6090 2023-05-24 20:52:21.000000 lsst-rsp-0.3.5/src/lsst/rsp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:52:36.148432 lsst-rsp-0.3.5/src/lsst_rsp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-05-24 20:52:36.000000 lsst-rsp-0.3.5/src/lsst_rsp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-24 20:52:36.000000 lsst-rsp-0.3.5/src/lsst_rsp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 20:52:36.000000 lsst-rsp-0.3.5/src/lsst_rsp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 20:52:36.000000 lsst-rsp-0.3.5/src/lsst_rsp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-24 20:52:36.000000 lsst-rsp-0.3.5/src/lsst_rsp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-24 20:52:36.000000 lsst-rsp-0.3.5/src/lsst_rsp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:52:36.148432 lsst-rsp-0.3.5/src/rubin_jupyter_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:52:21.000000 lsst-rsp-0.3.5/src/rubin_jupyter_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:52:36.148432 lsst-rsp-0.3.5/src/rubin_jupyter_utils/lab/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-24 20:52:21.000000 lsst-rsp-0.3.5/src/rubin_jupyter_utils/lab/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:52:36.148432 lsst-rsp-0.3.5/src/rubin_jupyter_utils/lab/notebook/
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-24 20:52:21.000000 lsst-rsp-0.3.5/src/rubin_jupyter_utils/lab/notebook/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:52:36.148432 lsst-rsp-0.3.5/src/rubin_jupyter_utils/lab/notebook/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-24 20:52:21.000000 lsst-rsp-0.3.5/src/rubin_jupyter_utils/lab/notebook/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:52:36.148432 lsst-rsp-0.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-24 20:52:21.000000 lsst-rsp-0.3.5/tests/utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-24 20:52:21.000000 lsst-rsp-0.3.5/tox.ini
```

### Comparing `lsst-rsp-0.3.4/.github/workflows/ci.yaml` & `lsst-rsp-0.3.5/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `lsst-rsp-0.3.4/.gitignore` & `lsst-rsp-0.3.5/.gitignore`

 * *Files identical despite different names*

### Comparing `lsst-rsp-0.3.4/LICENSE` & `lsst-rsp-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lsst-rsp-0.3.4/PKG-INFO` & `lsst-rsp-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-rsp
-Version: 0.3.4
+Version: 0.3.5
 Summary: User-facing classes and functions for RSP notebooks
 Home-page: https://github.com/lsst-sqre/lsst-rsp
 Author: Association of Universities for Research in Astronomy, Inc. (AURA)
 Author-email: sqre-admin@lists.lsst.org
 Project-URL: Source code, https://github.com/lsst-sqre/lsst-rsp
 Project-URL: Issue tracker, https://github.com/lsst-sqre/lsst-rsp/issues
 Keywords: lsst
```

### Comparing `lsst-rsp-0.3.4/pyproject.toml` & `lsst-rsp-0.3.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lsst-rsp-0.3.4/setup.cfg` & `lsst-rsp-0.3.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `lsst-rsp-0.3.4/src/lsst/rsp/__init__.py` & `lsst-rsp-0.3.5/src/lsst/rsp/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 """
 Collection of utilities, formerly in rsp_jupyter_utils.lab and
 rsp_jupyter_utils.helper
 """
 from importlib.metadata import PackageNotFoundError, version
 
-from .catalog import get_catalog, get_tap_service, retrieve_query
+from .catalog import (
+    get_catalog,
+    get_obstap_service,
+    get_tap_service,
+    retrieve_query,
+)
 from .forwarder import Forwarder
 from .log import IPythonHandler, forward_lsst_log
 from .utils import (
     format_bytes,
     get_access_token,
     get_digest,
     get_hostname,
@@ -35,11 +40,12 @@
     "forward_lsst_log",
     "get_access_token",
     "get_catalog",
     "get_digest",
     "get_node",
     "get_pod",
     "get_tap_service",
+    "get_obstap_service",
     "retrieve_query",
     "get_hostname",
     "show_with_bokeh_server",
 ]
```

### Comparing `lsst-rsp-0.3.4/src/lsst/rsp/catalog.py` & `lsst-rsp-0.3.5/src/lsst/rsp/catalog.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,43 +6,35 @@
 import pyvo.auth.authsession
 import requests
 from deprecated import deprecated
 
 from .utils import get_access_token
 
 
-def _get_tap_url() -> str:
-    tapurl = os.getenv("EXTERNAL_TAP_URL")
+def _get_tap_url(env_var: str, url: str) -> str:
+    tapurl = os.getenv("EXTERNAL_" + env_var + "_URL")
     if not tapurl:
         tapurl = (os.getenv("EXTERNAL_INSTANCE_URL") or "") + (
-            os.getenv("TAP_ROUTE") or "/api/tap"
+            os.getenv(env_var + "_ROUTE") or "/api/" + url
         )
     return tapurl
 
 
-def _get_obstap_url() -> str:
-    obstapurl = os.getenv("EXTERNAL_OBSTAP_URL")
-    if not obstapurl:
-        obstapurl = (os.getenv("EXTERNAL_INSTANCE_URL") or "") + (
-            os.getenv("OBSTAP_ROUTE") or "/api/obstap"
-        )
-    return obstapurl
-
-
 def _get_datalink_url() -> str:
     return os.getenv("EXTERNAL_INSTANCE_URL", "") + "/api/datalink"
 
 
 def _get_cutout_url() -> str:
     return os.getenv("EXTERNAL_INSTANCE_URL", "") + "/api/cutout"
 
 
 def _get_auth() -> Optional[pyvo.auth.authsession.AuthSession]:
-    tap_url = _get_tap_url()
-    obstap_url = _get_obstap_url()
+    tap_url = _get_tap_url("TAP", "tap")
+    obstap_url = _get_tap_url("OBSTAP", "obstap")
+    ssotap_url = _get_tap_url("SSOTAP", "ssotap")
     s = requests.Session()
     tok = get_access_token()
     if not tok:
         return None
     s.headers["Authorization"] = "Bearer " + tok
     auth = pyvo.auth.authsession.AuthSession()
     auth.credentials.set("lsst-token", s)
@@ -52,52 +44,65 @@
     auth.add_security_method_for_url(tap_url + "/sync", "lsst-token")
     auth.add_security_method_for_url(tap_url + "/async", "lsst-token")
     auth.add_security_method_for_url(tap_url + "/tables", "lsst-token")
     auth.add_security_method_for_url(obstap_url, "lsst-token")
     auth.add_security_method_for_url(obstap_url + "/sync", "lsst-token")
     auth.add_security_method_for_url(obstap_url + "/async", "lsst-token")
     auth.add_security_method_for_url(obstap_url + "/tables", "lsst-token")
+    auth.add_security_method_for_url(ssotap_url, "lsst-token")
+    auth.add_security_method_for_url(ssotap_url + "/sync", "lsst-token")
+    auth.add_security_method_for_url(ssotap_url + "/async", "lsst-token")
+    auth.add_security_method_for_url(ssotap_url + "/tables", "lsst-token")
     return auth
 
 
-def get_tap_service() -> pyvo.dal.TAPService:
-    #
-    # This is not ideal, but warning appears because require pyvo does
-    # not register uws:Sync and uws:Async.  It's harmless.  The broadness
-    # of the warning is unfortunately necessary since pyvo just uses
-    # warnings.warn():
-    # https://github.com/astropy/pyvo/blob/
-    # 81a50d7fd24428f17104a075bc0e1ac661ed6ea0/pyvo/utils/xml/elements.py#L418
-    #
-    with warnings.catch_warnings():
-        warnings.simplefilter("ignore", category=UserWarning)
-        ts = pyvo.dal.TAPService(_get_tap_url(), _get_auth())
-    return ts
+@deprecated(reason='Please use get_tap_service("tap")')
+def get_catalog() -> pyvo.dal.TAPService:
+    return get_tap_service("tap")
 
 
+@deprecated(reason='Please use get_tap_service("obstap")')
 def get_obstap_service() -> pyvo.dal.TAPService:
+    return get_tap_service("obstap")
+
+
+def get_tap_service(*args: str) -> pyvo.dal.TAPService:
+    if len(args) == 0:
+        warnings.warn(
+            'get_tap_service() is deprecated, use get_tap_service("tap")',
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        database = "tap"
+    else:
+        database = args[0]
+
+    if database == "tap":
+        tap_url = _get_tap_url("TAP", "tap")
+    elif database == "obstap":
+        tap_url = _get_tap_url("OBSTAP", "obstap")
+    elif database == "ssotap":
+        tap_url = _get_tap_url("SSOTAP", "ssotap")
+    else:
+        raise Exception(database + " is not a valid tap service")
+
     #
     # This is not ideal, but warning appears because require pyvo does
     # not register uws:Sync and uws:Async.  It's harmless.  The broadness
     # of the warning is unfortunately necessary since pyvo just uses
     # warnings.warn():
     # https://github.com/astropy/pyvo/blob/
     # 81a50d7fd24428f17104a075bc0e1ac661ed6ea0/pyvo/utils/xml/elements.py#L418
     #
     with warnings.catch_warnings():
         warnings.simplefilter("ignore", category=UserWarning)
-        ts = pyvo.dal.TAPService(_get_obstap_url(), _get_auth())
+        ts = pyvo.dal.TAPService(tap_url, _get_auth())
     return ts
 
 
-@deprecated(reason="Please use get_tap_service()")
-def get_catalog() -> pyvo.dal.TAPService:
-    return get_tap_service()
-
-
 def retrieve_query(query_url: str) -> pyvo.dal.AsyncTAPJob:
     #
     # This is not ideal, but warning appears because require pyvo does
     # not register uws:Sync and uws:Async.  It's harmless.  The broadness
     # of the warning is unfortunately necessary since pyvo just uses
     # warnings.warn():
     # https://github.com/astropy/pyvo/blob/
```

### Comparing `lsst-rsp-0.3.4/src/lsst/rsp/forwarder.py` & `lsst-rsp-0.3.5/src/lsst/rsp/forwarder.py`

 * *Files identical despite different names*

### Comparing `lsst-rsp-0.3.4/src/lsst/rsp/log.py` & `lsst-rsp-0.3.5/src/lsst/rsp/log.py`

 * *Files identical despite different names*

### Comparing `lsst-rsp-0.3.4/src/lsst/rsp/utils.py` & `lsst-rsp-0.3.5/src/lsst/rsp/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -84,18 +84,23 @@
     # The type: ignore is needed because the alternate form of notebook_url
     # (https://docs.bokeh.org/en/latest/docs/reference/io.html#bokeh.io.show)
     # isn't in bokeh's type hints.
     bokeh.io.show(obj=obj, notebook_url=jupyter_proxy_url)  # type:ignore
 
 
 def get_pod() -> Optional[client.V1Pod]:
-    """Try to get pod record.  If you don't have K8s or you can't use it
-    (e.g. nubladov3 does not grant any K8s access to the Lab pod) then
-    return None."""
+    """Get the Kubernetes object for the pod in which this is running.
 
+    Returns
+    -------
+    kubernetes.client.V1Pod or None
+        Kubernetes object for the pod in which this code is running, or `None`
+        if not running inside Kubernetes or running without access to the
+        Kubernetes API (the normal case for Nublado v3 and later).
+    """
     if _NO_K8S:
         return None
     try:
         config.load_incluster_config()
     except ConfigException:
         # We have the K8S libraries, but we don't have in-cluster config.
         return None
@@ -113,40 +118,61 @@
     except ApiException:
         # Well, that didn't work.
         return None
     return pod
 
 
 def get_node() -> str:
-    """Extract node name from pod, or the empty string if we can't
-    determine it."""
+    """Return the name of the current Kubernetes node.
+
+    Returns
+    -------
+    str
+        Name of the Kubernetes node on which this code is running, or the
+        empty string if the node could not be determined.
+    """
+    node = os.environ.get("KUBERNETES_NODE_NAME")
+    if node:
+        return node
+
+    # Fallback for Nublado v2, which got this information from the Kubernetes
+    # API (and therefore had to have access to the Kubernetes API).
     pod = get_pod()
     if pod is not None:
         return pod.spec.node_name
-    # In Nublado v3, we push this into the environment as K8S_NODE_NAME
-    return os.environ.get("K8S_NODE_NAME", "")
+    else:
+        return ""
 
 
 def get_digest() -> str:
-    """Extract image digest from pod, if we can.  Return the empty string
-    if we cannot."""
-    pod = get_pod()
-    # Image ID looks like host/[project/]owner/repo@sha256:hash
-    if pod is None:
-        # In Nublado v3 we push the digest directly into the image spec
-        image_id = os.environ.get("JUPYTER_IMAGE_SPEC", "")
-    else:
-        try:
-            image_id = pod.status.container_statuses[0].image_id
-        except Exception:
-            image_id = ""
+    """Return the digest of the current Docker image.
+
+    Returns
+    -------
+    str
+        Digest of the Docker image this code is running inside, or the empty
+        string if the digest could not be determined.
+    """
+    reference = os.environ.get("JUPYTER_IMAGE_SPEC", "")
+
+    # Fallback for Nublado v2, which got this information from the Kubernetes
+    # API (and therefore had to have access to the Kubernetes API).
+    if not reference:
+        pod = get_pod()
+        if pod:
+            try:
+                reference = pod.status.container_statuses[0].image_id
+            except Exception:
+                pass
+
     try:
-        return (image_id.split("@")[-1]).split(":")[-1]
+        # Reference looks like host/[project/]owner/repo@sha256:hash
+        return (reference.split("@")[-1]).split(":")[-1]
     except Exception:
-        return ""  # We will just return the empty string
+        return ""
 
 
 def get_access_token(
     tokenfile: Optional[Union[str, Path]] = None, log: Optional[Any] = None
 ) -> str:
     """Determine the access token from the mounted location (nublado
     3/2) or environment (any).  Prefer the mounted version since it
```

### Comparing `lsst-rsp-0.3.4/src/lsst_rsp.egg-info/PKG-INFO` & `lsst-rsp-0.3.5/src/lsst_rsp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-rsp
-Version: 0.3.4
+Version: 0.3.5
 Summary: User-facing classes and functions for RSP notebooks
 Home-page: https://github.com/lsst-sqre/lsst-rsp
 Author: Association of Universities for Research in Astronomy, Inc. (AURA)
 Author-email: sqre-admin@lists.lsst.org
 Project-URL: Source code, https://github.com/lsst-sqre/lsst-rsp
 Project-URL: Issue tracker, https://github.com/lsst-sqre/lsst-rsp/issues
 Keywords: lsst
```

### Comparing `lsst-rsp-0.3.4/src/lsst_rsp.egg-info/SOURCES.txt` & `lsst-rsp-0.3.5/src/lsst_rsp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lsst-rsp-0.3.4/src/rubin_jupyter_utils/lab/notebook/__init__.py` & `lsst-rsp-0.3.5/src/rubin_jupyter_utils/lab/notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-rsp-0.3.4/tox.ini` & `lsst-rsp-0.3.5/tox.ini`

 * *Files identical despite different names*

