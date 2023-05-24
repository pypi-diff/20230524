# Comparing `tmp/galaxykit-0.8.0.tar.gz` & `tmp/galaxykit-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galaxykit-0.8.0.tar", last modified: Wed Aug  3 16:14:55 2022, max compression
+gzip compressed data, was "galaxykit-0.9.0.tar", last modified: Fri Aug 12 03:16:13 2022, max compression
```

## Comparing `galaxykit-0.8.0.tar` & `galaxykit-0.9.0.tar`

### file list

```diff
@@ -1,27 +1,30 @@
-drwxrwxr-x   0 henderson  (1000) henderson  (1000)        0 2022-08-03 16:14:55.009281 galaxykit-0.8.0/
--rw-rw-r--   0 henderson  (1000) henderson  (1000)      718 2021-05-11 18:57:08.000000 galaxykit-0.8.0/LICENSE.md
--rw-rw-r--   0 henderson  (1000) henderson  (1000)     1011 2022-08-03 16:14:55.009281 galaxykit-0.8.0/PKG-INFO
--rw-r--r--   0 henderson  (1000) henderson  (1000)      720 2021-08-09 21:39:22.000000 galaxykit-0.8.0/README.md
-drwxrwxr-x   0 henderson  (1000) henderson  (1000)        0 2022-08-03 16:14:55.008281 galaxykit-0.8.0/galaxykit/
--rw-rw-r--   0 henderson  (1000) henderson  (1000)       67 2022-07-19 21:20:33.000000 galaxykit-0.8.0/galaxykit/__init__.py
--rw-rw-r--   0 henderson  (1000) henderson  (1000)       22 2022-08-03 16:08:11.000000 galaxykit-0.8.0/galaxykit/_version.py
--rw-rw-r--   0 henderson  (1000) henderson  (1000)     9711 2022-07-19 21:20:33.000000 galaxykit-0.8.0/galaxykit/client.py
--rw-rw-r--   0 henderson  (1000) henderson  (1000)     7103 2022-07-19 21:20:33.000000 galaxykit-0.8.0/galaxykit/collections.py
--rw-rw-r--   0 henderson  (1000) henderson  (1000)    23861 2022-07-19 21:20:33.000000 galaxykit-0.8.0/galaxykit/command.py
--rw-rw-r--   0 henderson  (1000) henderson  (1000)      274 2022-07-19 21:20:33.000000 galaxykit-0.8.0/galaxykit/container_images.py
--rw-rw-r--   0 henderson  (1000) henderson  (1000)     1221 2022-07-19 21:20:33.000000 galaxykit-0.8.0/galaxykit/containers.py
--rw-rw-r--   0 henderson  (1000) henderson  (1000)     2748 2022-07-19 21:20:33.000000 galaxykit-0.8.0/galaxykit/containerutils.py
--rw-rw-r--   0 henderson  (1000) henderson  (1000)     2809 2022-07-19 21:20:33.000000 galaxykit-0.8.0/galaxykit/groups.py
--rw-rw-r--   0 henderson  (1000) henderson  (1000)     2776 2022-07-19 21:20:33.000000 galaxykit-0.8.0/galaxykit/namespaces.py
--rw-rw-r--   0 henderson  (1000) henderson  (1000)      842 2022-07-19 21:20:33.000000 galaxykit-0.8.0/galaxykit/registries.py
--rw-rw-r--   0 henderson  (1000) henderson  (1000)     2729 2022-07-19 21:20:33.000000 galaxykit-0.8.0/galaxykit/users.py
--rw-rw-r--   0 henderson  (1000) henderson  (1000)     1190 2022-08-02 17:43:10.000000 galaxykit-0.8.0/galaxykit/utils.py
-drwxrwxr-x   0 henderson  (1000) henderson  (1000)        0 2022-08-03 16:14:55.009281 galaxykit-0.8.0/galaxykit.egg-info/
--rw-rw-r--   0 henderson  (1000) henderson  (1000)     1011 2022-08-03 16:14:54.000000 galaxykit-0.8.0/galaxykit.egg-info/PKG-INFO
--rw-rw-r--   0 henderson  (1000) henderson  (1000)      537 2022-08-03 16:14:55.000000 galaxykit-0.8.0/galaxykit.egg-info/SOURCES.txt
--rw-rw-r--   0 henderson  (1000) henderson  (1000)        1 2022-08-03 16:14:54.000000 galaxykit-0.8.0/galaxykit.egg-info/dependency_links.txt
--rw-rw-r--   0 henderson  (1000) henderson  (1000)       54 2022-08-03 16:14:54.000000 galaxykit-0.8.0/galaxykit.egg-info/entry_points.txt
--rw-rw-r--   0 henderson  (1000) henderson  (1000)       38 2022-08-03 16:14:54.000000 galaxykit-0.8.0/galaxykit.egg-info/requires.txt
--rw-rw-r--   0 henderson  (1000) henderson  (1000)       10 2022-08-03 16:14:54.000000 galaxykit-0.8.0/galaxykit.egg-info/top_level.txt
--rw-r--r--   0 henderson  (1000) henderson  (1000)      143 2022-08-03 16:14:55.009281 galaxykit-0.8.0/setup.cfg
--rw-rw-r--   0 henderson  (1000) henderson  (1000)      971 2022-07-19 21:20:33.000000 galaxykit-0.8.0/setup.py
+drwxrwxr-x   0 calvin    (1000) calvin    (1000)        0 2022-08-12 03:16:13.091639 galaxykit-0.9.0/
+-rw-rw-r--   0 calvin    (1000) calvin    (1000)     1214 2022-03-31 17:34:52.000000 galaxykit-0.9.0/.gitignore
+-rw-rw-r--   0 calvin    (1000) calvin    (1000)      124 2022-08-03 03:11:24.000000 galaxykit-0.9.0/.pre-commit-config.yaml
+-rw-rw-r--   0 calvin    (1000) calvin    (1000)     3532 2022-08-11 21:09:43.000000 galaxykit-0.9.0/CHANGES.md
+-rw-rw-r--   0 calvin    (1000) calvin    (1000)      718 2022-03-31 17:34:52.000000 galaxykit-0.9.0/LICENSE.md
+-rw-rw-r--   0 calvin    (1000) calvin    (1000)     1011 2022-08-12 03:16:13.091639 galaxykit-0.9.0/PKG-INFO
+-rw-rw-r--   0 calvin    (1000) calvin    (1000)      720 2022-03-31 17:34:52.000000 galaxykit-0.9.0/README.md
+drwxrwxr-x   0 calvin    (1000) calvin    (1000)        0 2022-08-12 03:16:13.090639 galaxykit-0.9.0/galaxykit/
+-rw-rw-r--   0 calvin    (1000) calvin    (1000)       67 2022-07-20 19:46:01.000000 galaxykit-0.9.0/galaxykit/__init__.py
+-rw-rw-r--   0 calvin    (1000) calvin    (1000)       22 2022-08-12 03:15:58.000000 galaxykit-0.9.0/galaxykit/_version.py
+-rw-rw-r--   0 calvin    (1000) calvin    (1000)    10230 2022-08-11 22:55:57.000000 galaxykit-0.9.0/galaxykit/client.py
+-rw-rw-r--   0 calvin    (1000) calvin    (1000)     7103 2022-07-20 19:46:01.000000 galaxykit-0.9.0/galaxykit/collections.py
+-rw-rw-r--   0 calvin    (1000) calvin    (1000)    23861 2022-07-20 19:46:01.000000 galaxykit-0.9.0/galaxykit/command.py
+-rw-rw-r--   0 calvin    (1000) calvin    (1000)      274 2022-07-20 19:46:01.000000 galaxykit-0.9.0/galaxykit/container_images.py
+-rw-rw-r--   0 calvin    (1000) calvin    (1000)     1221 2022-07-20 19:46:01.000000 galaxykit-0.9.0/galaxykit/containers.py
+-rw-rw-r--   0 calvin    (1000) calvin    (1000)     2748 2022-07-20 19:46:01.000000 galaxykit-0.9.0/galaxykit/containerutils.py
+-rw-rw-r--   0 calvin    (1000) calvin    (1000)     2809 2022-07-20 19:46:01.000000 galaxykit-0.9.0/galaxykit/groups.py
+-rw-rw-r--   0 calvin    (1000) calvin    (1000)     2776 2022-08-11 20:06:35.000000 galaxykit-0.9.0/galaxykit/namespaces.py
+-rw-rw-r--   0 calvin    (1000) calvin    (1000)      842 2022-07-20 19:46:01.000000 galaxykit-0.9.0/galaxykit/registries.py
+-rw-rw-r--   0 calvin    (1000) calvin    (1000)     2729 2022-07-20 19:46:01.000000 galaxykit-0.9.0/galaxykit/users.py
+-rw-rw-r--   0 calvin    (1000) calvin    (1000)     1190 2022-08-03 03:11:24.000000 galaxykit-0.9.0/galaxykit/utils.py
+drwxrwxr-x   0 calvin    (1000) calvin    (1000)        0 2022-08-12 03:16:13.090639 galaxykit-0.9.0/galaxykit.egg-info/
+-rwxr-xr-x   0 calvin    (1000) calvin    (1000)     1011 2022-08-12 03:16:12.000000 galaxykit-0.9.0/galaxykit.egg-info/PKG-INFO
+-rwxr-xr-x   0 calvin    (1000) calvin    (1000)      583 2022-08-12 03:16:13.000000 galaxykit-0.9.0/galaxykit.egg-info/SOURCES.txt
+-rwxr-xr-x   0 calvin    (1000) calvin    (1000)        1 2022-08-12 03:16:12.000000 galaxykit-0.9.0/galaxykit.egg-info/dependency_links.txt
+-rwxr-xr-x   0 calvin    (1000) calvin    (1000)       53 2022-08-12 03:16:12.000000 galaxykit-0.9.0/galaxykit.egg-info/entry_points.txt
+-rwxr-xr-x   0 calvin    (1000) calvin    (1000)       38 2022-08-12 03:16:12.000000 galaxykit-0.9.0/galaxykit.egg-info/requires.txt
+-rwxr-xr-x   0 calvin    (1000) calvin    (1000)       10 2022-08-12 03:16:12.000000 galaxykit-0.9.0/galaxykit.egg-info/top_level.txt
+-rw-rw-r--   0 calvin    (1000) calvin    (1000)      143 2022-08-12 03:16:13.091639 galaxykit-0.9.0/setup.cfg
+-rw-rw-r--   0 calvin    (1000) calvin    (1000)      971 2022-07-20 19:46:01.000000 galaxykit-0.9.0/setup.py
```

### Comparing `galaxykit-0.8.0/LICENSE.md` & `galaxykit-0.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `galaxykit-0.8.0/PKG-INFO` & `galaxykit-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxykit
-Version: 0.8.0
+Version: 0.9.0
 Summary: A small client library for testing galaxy_ng.
 Home-page: https://github.com/hendersonreed/galaxykit/
 Author: Red Hat PEAQE Team
 License: GPLv2
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `galaxykit-0.8.0/README.md` & `galaxykit-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `galaxykit-0.8.0/galaxykit/client.py` & `galaxykit-0.9.0/galaxykit/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 client.py contains the wrapping interface for all the other modules (aside from cli.py)
 """
+import logging
 import platform
 import sys
 from urllib.parse import urlparse, urljoin
 from simplejson.errors import JSONDecodeError
 from simplejson import dumps
 
 import requests
@@ -15,14 +16,17 @@
 from . import users
 from . import namespaces
 from . import collections
 from . import __version__ as VERSION
 from .utils import GalaxyClientError
 
 
+logger = logging.getLogger(__name__)
+
+
 def user_agent():
     """Returns a user agent used by ansible-galaxy to include the Ansible version, platform and python version."""
 
     python_version = sys.version_info
     return "galaxy-kit/{version} ({platform}; python:{py_major}.{py_minor}.{py_micro})".format(
         version=VERSION,
         platform=platform.system(),
@@ -36,14 +40,15 @@
     """
     The primary class for the client - this is the authenticated context from
     which all authentication flows.
     """
 
     headers = None
     galaxy_root = ""
+    original_token = None
     token = ""
     token_type = None
     container_client = None
     username = ""
     password = ""
 
     def __init__(
@@ -92,48 +97,27 @@
                 except Exception as e:
                     raise Exception(rr.text)
                 if "access_token" not in jdata:
                     raise Exception(rr.text)
                 self.token = jdata["access_token"]
 
             elif self.token and self.auth_url:
-                payload = "grant_type=refresh_token&client_id=%s&refresh_token=%s" % (
-                    "cloud-services",
-                    self.token,
-                )
-                headers = {
-                    "User-Agent": user_agent(),
-                    "Content-Type": "application/x-www-form-urlencoded",
-                }
-                resp = requests.post(
-                    self.auth_url,
-                    data=payload,
-                    verify=self.https_verify,
-                    headers=headers,
-                )
-                json = resp.json()
-                self.token = json["access_token"]
-                self.token_type = "Bearer"
+                self._refresh_jwt_token()
 
             elif self.token is None:
                 auth_url = urljoin(self.galaxy_root, "v3/auth/token/")
                 resp = requests.post(
                     auth_url, auth=(self.username, self.password), verify=False
                 )
                 try:
                     self.token = resp.json().get("token")
                 except JSONDecodeError:
                     print(f"Failed to fetch token: {resp.text}", file=sys.stderr)
 
-            self.headers.update(
-                {
-                    "Accept": "application/json",
-                    "Authorization": f"{self.token_type} {self.token}",
-                }
-            )
+            self._update_auth_headers()
 
             if container_engine:
                 if not (self.username and self.password):
                     raise ValueError(
                         "Cannot use container engine commands without username and password for authentication."
                     )
                 container_registry = (
@@ -143,28 +127,67 @@
 
                 self.container_client = containerutils.ContainerClient(
                     (self.username, self.password),
                     container_engine,
                     container_registry,
                     tls_verify=container_tls_verify,
                 )
+    
+    def _refresh_jwt_token(self):
+        if not self.original_token:
+            self.original_token = self.token
+        else:
+            logger.warning("Refreshing JWT Token and retrying request")
+
+        payload = "grant_type=refresh_token&client_id=%s&refresh_token=%s" % (
+            "cloud-services",
+            self.original_token,
+        )
+        headers = {
+            "User-Agent": user_agent(),
+            "Content-Type": "application/x-www-form-urlencoded",
+        }
+        resp = requests.post(
+            self.auth_url,
+            data=payload,
+            verify=self.https_verify,
+            headers=headers,
+        )
+        json = resp.json()
+        self.token = json["access_token"]
+        self.token_type = "Bearer"
+
+    def _update_auth_headers(self):
+        self.headers.update(
+            {
+                "Accept": "application/json",
+                "Authorization": f"{self.token_type} {self.token}",
+            }
+        )
 
     def _http(self, method, path, *args, **kwargs):
         url = urljoin(self.galaxy_root, path)
         headers = kwargs.pop("headers", self.headers)
         parse_json = kwargs.pop("parse_json", True)
 
         resp = requests.request(
             method, url, headers=headers, verify=self.https_verify, *args, **kwargs
         )
+
+        if 'Invalid JWT token' in resp.text and 'claim expired' in resp.text:
+            self._refresh_jwt_token()
+            self._update_auth_headers()
+            resp = requests.request(
+                method, url, headers=headers, verify=self.https_verify, *args, **kwargs
+            )
+
         if parse_json:
             try:
                 json = resp.json()
             except JSONDecodeError as exc:
-                print(resp.text)
                 raise ValueError("Failed to parse JSON response from API") from exc
             if "errors" in json:
                 # {'errors': [{'status': '403', 'code': 'not_authenticated', 'title': 'Authentication credentials were not provided.'}]}
                 raise GalaxyClientError(*json["errors"])
             return json
         else:
             return resp
```

### Comparing `galaxykit-0.8.0/galaxykit/collections.py` & `galaxykit-0.9.0/galaxykit/collections.py`

 * *Files identical despite different names*

### Comparing `galaxykit-0.8.0/galaxykit/command.py` & `galaxykit-0.9.0/galaxykit/command.py`

 * *Files identical despite different names*

### Comparing `galaxykit-0.8.0/galaxykit/containers.py` & `galaxykit-0.9.0/galaxykit/containers.py`

 * *Files identical despite different names*

### Comparing `galaxykit-0.8.0/galaxykit/containerutils.py` & `galaxykit-0.9.0/galaxykit/containerutils.py`

 * *Files identical despite different names*

### Comparing `galaxykit-0.8.0/galaxykit/groups.py` & `galaxykit-0.9.0/galaxykit/groups.py`

 * *Files identical despite different names*

### Comparing `galaxykit-0.8.0/galaxykit/namespaces.py` & `galaxykit-0.9.0/galaxykit/namespaces.py`

 * *Files identical despite different names*

### Comparing `galaxykit-0.8.0/galaxykit/registries.py` & `galaxykit-0.9.0/galaxykit/registries.py`

 * *Files identical despite different names*

### Comparing `galaxykit-0.8.0/galaxykit/users.py` & `galaxykit-0.9.0/galaxykit/users.py`

 * *Files identical despite different names*

### Comparing `galaxykit-0.8.0/galaxykit/utils.py` & `galaxykit-0.9.0/galaxykit/utils.py`

 * *Files identical despite different names*

### Comparing `galaxykit-0.8.0/galaxykit.egg-info/PKG-INFO` & `galaxykit-0.9.0/galaxykit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxykit
-Version: 0.8.0
+Version: 0.9.0
 Summary: A small client library for testing galaxy_ng.
 Home-page: https://github.com/hendersonreed/galaxykit/
 Author: Red Hat PEAQE Team
 License: GPLv2
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `galaxykit-0.8.0/setup.py` & `galaxykit-0.9.0/setup.py`

 * *Files identical despite different names*

