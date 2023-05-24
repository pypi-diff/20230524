# Comparing `tmp/wipac-rest-tools-1.4.8.tar.gz` & `tmp/wipac-rest-tools-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wipac-rest-tools-1.4.8.tar", last modified: Mon Feb  6 19:39:31 2023, max compression
+gzip compressed data, was "wipac-rest-tools-1.4.9.tar", last modified: Wed Feb 15 17:45:07 2023, max compression
```

## Comparing `wipac-rest-tools-1.4.8.tar` & `wipac-rest-tools-1.4.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 19:39:31.651109 wipac-rest-tools-1.4.8/
--rw-r--r--   0 root         (0) root         (0)     1070 2023-02-06 19:39:28.000000 wipac-rest-tools-1.4.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3324 2023-02-06 19:39:31.651109 wipac-rest-tools-1.4.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2326 2023-02-06 19:39:28.000000 wipac-rest-tools-1.4.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 19:39:31.647108 wipac-rest-tools-1.4.8/rest_tools/
--rw-r--r--   0 root         (0) root         (0)      513 2023-02-06 19:39:29.000000 wipac-rest-tools-1.4.8/rest_tools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 19:39:31.651109 wipac-rest-tools-1.4.8/rest_tools/client/
--rw-r--r--   0 root         (0) root         (0)      438 2023-02-06 19:39:28.000000 wipac-rest-tools-1.4.8/rest_tools/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9778 2023-02-06 19:39:28.000000 wipac-rest-tools-1.4.8/rest_tools/client/client.py
--rw-r--r--   0 root         (0) root         (0)     1885 2023-02-06 19:39:28.000000 wipac-rest-tools-1.4.8/rest_tools/client/client_credentials.py
--rw-r--r--   0 root         (0) root         (0)     6607 2023-02-06 19:39:28.000000 wipac-rest-tools-1.4.8/rest_tools/client/device_client.py
--rw-r--r--   0 root         (0) root         (0)     2973 2023-02-06 19:39:28.000000 wipac-rest-tools-1.4.8/rest_tools/client/openid_client.py
--rw-r--r--   0 root         (0) root         (0)     2569 2023-02-06 19:39:28.000000 wipac-rest-tools-1.4.8/rest_tools/client/session.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-06 19:39:28.000000 wipac-rest-tools-1.4.8/rest_tools/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 19:39:31.651109 wipac-rest-tools-1.4.8/rest_tools/server/
--rw-r--r--   0 root         (0) root         (0)      691 2023-02-06 19:39:28.000000 wipac-rest-tools-1.4.8/rest_tools/server/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8781 2023-02-06 19:39:28.000000 wipac-rest-tools-1.4.8/rest_tools/server/arghandler.py
--rw-r--r--   0 root         (0) root         (0)    12144 2023-02-06 19:39:28.000000 wipac-rest-tools-1.4.8/rest_tools/server/decorators.py
--rw-r--r--   0 root         (0) root         (0)    17905 2023-02-06 19:39:28.000000 wipac-rest-tools-1.4.8/rest_tools/server/handler.py
--rw-r--r--   0 root         (0) root         (0)     2249 2023-02-06 19:39:28.000000 wipac-rest-tools-1.4.8/rest_tools/server/server.py
--rw-r--r--   0 root         (0) root         (0)     2313 2023-02-06 19:39:28.000000 wipac-rest-tools-1.4.8/rest_tools/server/stats.py
--rw-r--r--   0 root         (0) root         (0)     1781 2023-02-06 19:39:28.000000 wipac-rest-tools-1.4.8/rest_tools/telemetry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 19:39:31.651109 wipac-rest-tools-1.4.8/rest_tools/utils/
--rw-r--r--   0 root         (0) root         (0)      252 2023-02-06 19:39:28.000000 wipac-rest-tools-1.4.8/rest_tools/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5334 2023-02-06 19:39:28.000000 wipac-rest-tools-1.4.8/rest_tools/utils/auth.py
--rw-r--r--   0 root         (0) root         (0)      136 2023-02-06 19:39:28.000000 wipac-rest-tools-1.4.8/rest_tools/utils/config.py
--rw-r--r--   0 root         (0) root         (0)     6123 2023-02-06 19:39:28.000000 wipac-rest-tools-1.4.8/rest_tools/utils/daemon.py
--rw-r--r--   0 root         (0) root         (0)     4833 2023-02-06 19:39:28.000000 wipac-rest-tools-1.4.8/rest_tools/utils/json_util.py
--rw-r--r--   0 root         (0) root         (0)     2123 2023-02-06 19:39:31.651109 wipac-rest-tools-1.4.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      104 2023-02-06 19:39:28.000000 wipac-rest-tools-1.4.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 19:39:31.651109 wipac-rest-tools-1.4.8/wipac_rest_tools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3324 2023-02-06 19:39:31.000000 wipac-rest-tools-1.4.8/wipac_rest_tools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      815 2023-02-06 19:39:31.000000 wipac-rest-tools-1.4.8/wipac_rest_tools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-06 19:39:31.000000 wipac-rest-tools-1.4.8/wipac_rest_tools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      353 2023-02-06 19:39:31.000000 wipac-rest-tools-1.4.8/wipac_rest_tools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-02-06 19:39:31.000000 wipac-rest-tools-1.4.8/wipac_rest_tools.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 17:45:07.883011 wipac-rest-tools-1.4.9/
+-rw-r--r--   0 root         (0) root         (0)     1070 2023-02-15 17:45:04.000000 wipac-rest-tools-1.4.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3324 2023-02-15 17:45:07.883011 wipac-rest-tools-1.4.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2326 2023-02-15 17:45:04.000000 wipac-rest-tools-1.4.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 17:45:07.879011 wipac-rest-tools-1.4.9/rest_tools/
+-rw-r--r--   0 root         (0) root         (0)      513 2023-02-15 17:45:05.000000 wipac-rest-tools-1.4.9/rest_tools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 17:45:07.879011 wipac-rest-tools-1.4.9/rest_tools/client/
+-rw-r--r--   0 root         (0) root         (0)      438 2023-02-15 17:45:04.000000 wipac-rest-tools-1.4.9/rest_tools/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9778 2023-02-15 17:45:04.000000 wipac-rest-tools-1.4.9/rest_tools/client/client.py
+-rw-r--r--   0 root         (0) root         (0)     1885 2023-02-15 17:45:04.000000 wipac-rest-tools-1.4.9/rest_tools/client/client_credentials.py
+-rw-r--r--   0 root         (0) root         (0)     6607 2023-02-15 17:45:04.000000 wipac-rest-tools-1.4.9/rest_tools/client/device_client.py
+-rw-r--r--   0 root         (0) root         (0)     2973 2023-02-15 17:45:04.000000 wipac-rest-tools-1.4.9/rest_tools/client/openid_client.py
+-rw-r--r--   0 root         (0) root         (0)     2569 2023-02-15 17:45:04.000000 wipac-rest-tools-1.4.9/rest_tools/client/session.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-02-15 17:45:04.000000 wipac-rest-tools-1.4.9/rest_tools/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 17:45:07.879011 wipac-rest-tools-1.4.9/rest_tools/server/
+-rw-r--r--   0 root         (0) root         (0)      691 2023-02-15 17:45:04.000000 wipac-rest-tools-1.4.9/rest_tools/server/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8781 2023-02-15 17:45:04.000000 wipac-rest-tools-1.4.9/rest_tools/server/arghandler.py
+-rw-r--r--   0 root         (0) root         (0)    12144 2023-02-15 17:45:04.000000 wipac-rest-tools-1.4.9/rest_tools/server/decorators.py
+-rw-r--r--   0 root         (0) root         (0)    18070 2023-02-15 17:45:04.000000 wipac-rest-tools-1.4.9/rest_tools/server/handler.py
+-rw-r--r--   0 root         (0) root         (0)     2249 2023-02-15 17:45:04.000000 wipac-rest-tools-1.4.9/rest_tools/server/server.py
+-rw-r--r--   0 root         (0) root         (0)     2313 2023-02-15 17:45:04.000000 wipac-rest-tools-1.4.9/rest_tools/server/stats.py
+-rw-r--r--   0 root         (0) root         (0)     1781 2023-02-15 17:45:04.000000 wipac-rest-tools-1.4.9/rest_tools/telemetry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 17:45:07.883011 wipac-rest-tools-1.4.9/rest_tools/utils/
+-rw-r--r--   0 root         (0) root         (0)      252 2023-02-15 17:45:04.000000 wipac-rest-tools-1.4.9/rest_tools/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5335 2023-02-15 17:45:04.000000 wipac-rest-tools-1.4.9/rest_tools/utils/auth.py
+-rw-r--r--   0 root         (0) root         (0)      136 2023-02-15 17:45:04.000000 wipac-rest-tools-1.4.9/rest_tools/utils/config.py
+-rw-r--r--   0 root         (0) root         (0)     6123 2023-02-15 17:45:04.000000 wipac-rest-tools-1.4.9/rest_tools/utils/daemon.py
+-rw-r--r--   0 root         (0) root         (0)     4833 2023-02-15 17:45:04.000000 wipac-rest-tools-1.4.9/rest_tools/utils/json_util.py
+-rw-r--r--   0 root         (0) root         (0)     2123 2023-02-15 17:45:07.883011 wipac-rest-tools-1.4.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      104 2023-02-15 17:45:04.000000 wipac-rest-tools-1.4.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 17:45:07.883011 wipac-rest-tools-1.4.9/wipac_rest_tools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3324 2023-02-15 17:45:07.000000 wipac-rest-tools-1.4.9/wipac_rest_tools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      815 2023-02-15 17:45:07.000000 wipac-rest-tools-1.4.9/wipac_rest_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-02-15 17:45:07.000000 wipac-rest-tools-1.4.9/wipac_rest_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      353 2023-02-15 17:45:07.000000 wipac-rest-tools-1.4.9/wipac_rest_tools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-02-15 17:45:07.000000 wipac-rest-tools-1.4.9/wipac_rest_tools.egg-info/top_level.txt
```

### Comparing `wipac-rest-tools-1.4.8/LICENSE` & `wipac-rest-tools-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.4.8/PKG-INFO` & `wipac-rest-tools-1.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wipac-rest-tools
-Version: 1.4.8
+Version: 1.4.9
 Summary: REST tools in python - common code for client and server
 Home-page: https://github.com/WIPACrepo/rest-tools
 Download-URL: https://pypi.org/project/wipac-rest-tools/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/WIPACrepo/rest-tools/issues
```

### Comparing `wipac-rest-tools-1.4.8/README.md` & `wipac-rest-tools-1.4.9/README.md`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.4.8/rest_tools/__init__.py` & `wipac-rest-tools-1.4.9/rest_tools/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # version is a human-readable version number.
 
 # version_info is a four-tuple for programmatic comparison. The first
 # three numbers are the components of the version number. The fourth
 # is zero for an official release, positive for a development branch,
 # or negative for a release candidate or beta (after the base version
 # number has been incremented)
-__version__ = "1.4.8"
+__version__ = "1.4.9"
 version_info = (
     int(__version__.split(".")[0]),
     int(__version__.split(".")[1]),
     int(__version__.split(".")[2]),
     0,
 )
```

### Comparing `wipac-rest-tools-1.4.8/rest_tools/client/client.py` & `wipac-rest-tools-1.4.9/rest_tools/client/client.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.4.8/rest_tools/client/client_credentials.py` & `wipac-rest-tools-1.4.9/rest_tools/client/client_credentials.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.4.8/rest_tools/client/device_client.py` & `wipac-rest-tools-1.4.9/rest_tools/client/device_client.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.4.8/rest_tools/client/openid_client.py` & `wipac-rest-tools-1.4.9/rest_tools/client/openid_client.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.4.8/rest_tools/client/session.py` & `wipac-rest-tools-1.4.9/rest_tools/client/session.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.4.8/rest_tools/server/__init__.py` & `wipac-rest-tools-1.4.9/rest_tools/server/__init__.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.4.8/rest_tools/server/arghandler.py` & `wipac-rest-tools-1.4.9/rest_tools/server/arghandler.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.4.8/rest_tools/server/decorators.py` & `wipac-rest-tools-1.4.9/rest_tools/server/decorators.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.4.8/rest_tools/server/handler.py` & `wipac-rest-tools-1.4.9/rest_tools/server/handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -270,15 +270,18 @@
 
 class OpenIDWebHandlerMixin:
     """Load current user from `OpenIDLoginHandler` cookies."""
     def get_current_user(self):
         """Get the current user, and set auth-related attributes."""
         try:
             access_token = self.get_secure_cookie('access_token')
+            logging.debug('access_token: %r', access_token)
             refresh_token = self.get_secure_cookie('refresh_token')
+            if isinstance(access_token, str):
+                access_token = access_token.encode('utf8')
             data = self.auth.validate(access_token)
             self.auth_data = data
             self.auth_key = access_token
             self.auth_refresh_token = refresh_token
             return data['sub']
         # Auth Failed
         except Exception:
```

### Comparing `wipac-rest-tools-1.4.8/rest_tools/server/server.py` & `wipac-rest-tools-1.4.9/rest_tools/server/server.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.4.8/rest_tools/server/stats.py` & `wipac-rest-tools-1.4.9/rest_tools/server/stats.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.4.8/rest_tools/telemetry.py` & `wipac-rest-tools-1.4.9/rest_tools/telemetry.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.4.8/rest_tools/utils/auth.py` & `wipac-rest-tools-1.4.9/rest_tools/utils/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         self.algorithms = algorithms if algorithms else ['RS256','RS512']
 
     def _validate(self, token, key, **kwargs):
         options = {}
 
         # required claims
         claims = ['exp', 'iat', 'iss']
-        claims.extend(kwargs.pop('require', []))
+        claims.extend(kwargs.pop('required', []))
         options['require'] = claims
 
         # configure the audience to validate
         audience = kwargs.pop('audience', None)
         if not audience:
             audience = self.audience
         if not audience:
```

### Comparing `wipac-rest-tools-1.4.8/rest_tools/utils/daemon.py` & `wipac-rest-tools-1.4.9/rest_tools/utils/daemon.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.4.8/rest_tools/utils/json_util.py` & `wipac-rest-tools-1.4.9/rest_tools/utils/json_util.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.4.8/setup.cfg` & `wipac-rest-tools-1.4.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.4.8/wipac_rest_tools.egg-info/PKG-INFO` & `wipac-rest-tools-1.4.9/wipac_rest_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wipac-rest-tools
-Version: 1.4.8
+Version: 1.4.9
 Summary: REST tools in python - common code for client and server
 Home-page: https://github.com/WIPACrepo/rest-tools
 Download-URL: https://pypi.org/project/wipac-rest-tools/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/WIPACrepo/rest-tools/issues
```

### Comparing `wipac-rest-tools-1.4.8/wipac_rest_tools.egg-info/SOURCES.txt` & `wipac-rest-tools-1.4.9/wipac_rest_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

