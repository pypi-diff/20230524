# Comparing `tmp/Preston-4.1.0.tar.gz` & `tmp/preston-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Preston-4.1.0.tar", last modified: Thu Apr 26 04:15:26 2018, max compression
+gzip compressed data, was "preston-4.1.1.tar", max compression
```

## Comparing `Preston-4.1.0.tar` & `preston-4.1.1.tar`

### file list

```diff
@@ -1,15 +1,7 @@
-drwxr-xr-x   0 arch      (1000) sudo      (1000)        0 2018-04-26 04:15:26.000000 Preston-4.1.0/
--rw-r--r--   0 arch      (1000) sudo      (1000)       79 2018-04-26 04:15:26.000000 Preston-4.1.0/setup.cfg
--rw-r--r--   0 arch      (1000) sudo      (1000)      497 2018-04-26 04:15:26.000000 Preston-4.1.0/PKG-INFO
-drwxr-xr-x   0 arch      (1000) sudo      (1000)        0 2018-04-26 04:15:26.000000 Preston-4.1.0/preston/
--rw-r--r--   0 arch      (1000) sudo      (1000)      136 2018-04-26 04:11:02.000000 Preston-4.1.0/preston/__init__.py
--rw-r--r--   0 arch      (1000) sudo      (1000)     3196 2018-04-12 03:26:22.000000 Preston-4.1.0/preston/cache.py
--rw-r--r--   0 arch      (1000) sudo      (1000)    11797 2018-04-26 04:10:19.000000 Preston-4.1.0/preston/preston.py
-drwxr-xr-x   0 arch      (1000) sudo      (1000)        0 2018-04-26 04:15:26.000000 Preston-4.1.0/Preston.egg-info/
--rw-r--r--   0 arch      (1000) sudo      (1000)        1 2018-04-26 04:15:26.000000 Preston-4.1.0/Preston.egg-info/dependency_links.txt
--rw-r--r--   0 arch      (1000) sudo      (1000)        8 2018-04-26 04:15:26.000000 Preston-4.1.0/Preston.egg-info/top_level.txt
--rw-r--r--   0 arch      (1000) sudo      (1000)       17 2018-04-26 04:15:26.000000 Preston-4.1.0/Preston.egg-info/requires.txt
--rw-r--r--   0 arch      (1000) sudo      (1000)      497 2018-04-26 04:15:26.000000 Preston-4.1.0/Preston.egg-info/PKG-INFO
--rw-r--r--   0 arch      (1000) sudo      (1000)      238 2018-04-26 04:15:26.000000 Preston-4.1.0/Preston.egg-info/SOURCES.txt
--rw-r--r--   0 arch      (1000) sudo      (1000)      769 2018-04-12 23:22:34.000000 Preston-4.1.0/setup.py
--rw-r--r--   0 arch      (1000) sudo      (1000)     4359 2018-04-26 04:13:08.000000 Preston-4.1.0/README.md
+-rw-r--r--   0        0        0     1085 2023-05-24 02:50:25.279805 preston-4.1.1/LICENSE
+-rw-r--r--   0        0        0     4914 2023-05-24 02:50:25.279805 preston-4.1.1/README.md
+-rw-r--r--   0        0        0      114 2023-05-24 02:50:25.279805 preston-4.1.1/preston/__init__.py
+-rw-r--r--   0        0        0     3202 2023-05-24 02:50:25.279805 preston-4.1.1/preston/cache.py
+-rw-r--r--   0        0        0    11863 2023-05-24 02:50:25.279805 preston-4.1.1/preston/preston.py
+-rw-r--r--   0        0        0      797 2023-05-24 03:01:50.489833 preston-4.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5833 1970-01-01 00:00:00.000000 preston-4.1.1/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `Preston-4.1.0/preston/cache.py` & `preston-4.1.1/preston/cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from typing import Optional
 from datetime import datetime
 import time
 import math
 
+from requests import Response
 
-class Cache:
 
+class Cache:
     def __init__(self):
         """Cache class.
 
         The cache is desgined to respect the caching rules of ESI as to
         not request a page more often than it is updated by the server.
 
         Args:
@@ -25,36 +26,35 @@
 
         Args:
             headers: dictionary of headers from ESI
 
         Returns:
             value of seconds from now the data expires
         """
-        expiration_str = headers.get('expires')
+        expiration_str = headers.get("expires")
         if not expiration_str:
             return 0
-        expiration = datetime.strptime(expiration_str, '%a, %d %b %Y %H:%M:%S %Z')
+        expiration = datetime.strptime(expiration_str, "%a, %d %b %Y %H:%M:%S %Z")
         delta = (expiration - datetime.utcnow()).total_seconds()
         return math.ceil(abs(delta))
 
-    def set(self, response: 'requests.Response') -> None:
+    def set(self, response: Response) -> None:
         """Adds a response to the cache.
 
         Args:
             response: response from ESI
 
         Returns:
             None
         """
         self.data[response.url] = SavedEndpoint(
-            response.json(),
-            self._get_expiration(response.headers)
+            response.json(), self._get_expiration(response.headers)
         )
 
-    def _check_expiration(self, url: str, data: 'SavedEndpoint') -> 'SavedEndpoint':
+    def _check_expiration(self, url: str, data: "SavedEndpoint") -> "SavedEndpoint":
         """Checks the expiration time for data for a url.
 
         If the data has expired, it is deleted from the cache.
 
         Args:
             url: url to check
             data: page of data for that url
@@ -95,15 +95,14 @@
         Returns:
             value of the number of keys in the data
         """
         return len(self.data.keys())
 
 
 class SavedEndpoint:
-
     def __init__(self, data: dict, expires_in: float) -> None:
         """SavedEndpoint class.
 
         A wrapper around a page from ESI that also includes the expiration time
         in seconds and the time after which the wrapped data expires.
 
         Args:
```

### Comparing `Preston-4.1.0/preston/preston.py` & `preston-4.1.1/preston/preston.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,46 +36,46 @@
         refresh_token           if supplied, Preston will use it to get new
                                 access tokens; can be supplied with or without
                                 access_token and access_expiration
 
     Args:
         kwargs: various configuration options
     """
-    BASE_URL = 'https://esi.tech.ccp.is'
-    SPEC_URL = BASE_URL + '/_{}/swagger.json'
-    OAUTH_URL = 'https://login.eveonline.com/oauth/'
-    TOKEN_URL = OAUTH_URL + 'token'
-    AUTHORIZE_URL = OAUTH_URL + 'authorize'
-    WHOAMI_URL = OAUTH_URL + 'verify'
-    METHODS = ['get', 'post', 'put', 'delete']
-    OPERATION_ID_KEY = 'operationId'
-    VAR_REPLACE_REGEX = r'{(\w+)}'
 
-    def __init__(self, **kwargs: str) -> None:
+    BASE_URL = "https://esi.tech.ccp.is"
+    SPEC_URL = BASE_URL + "/_{}/swagger.json"
+    OAUTH_URL = "https://login.eveonline.com/oauth/"
+    TOKEN_URL = OAUTH_URL + "token"
+    AUTHORIZE_URL = OAUTH_URL + "authorize"
+    WHOAMI_URL = OAUTH_URL + "verify"
+    METHODS = ["get", "post", "put", "delete"]
+    OPERATION_ID_KEY = "operationId"
+    VAR_REPLACE_REGEX = r"{(\w+)}"
+
+    def __init__(self, **kwargs: Any) -> None:
         self.cache = Cache()
         self.spec = None
-        self.version = kwargs.get('version', 'latest')
+        self.version = kwargs.get("version", "latest")
         self.session = requests.Session()
-        self.session.headers.update({
-            'User-Agent': kwargs.get('user_agent', ''),
-            'Accept': 'application/json'
-        })
-        self.client_id = kwargs.get('client_id')
-        self.client_secret = kwargs.get('client_secret')
-        self.callback_url = kwargs.get('callback_url')
-        self.scope = kwargs.get('scope', '')
-        self.access_token = kwargs.get('access_token')
-        self.access_expiration = kwargs.get('access_expiration')
-        self.refresh_token = kwargs.get('refresh_token')
+        self.session.headers.update(
+            {"User-Agent": kwargs.get("user_agent", ""), "Accept": "application/json"}
+        )
+        self.client_id = kwargs.get("client_id")
+        self.client_secret = kwargs.get("client_secret")
+        self.callback_url = kwargs.get("callback_url")
+        self.scope = kwargs.get("scope", "")
+        self.access_token = kwargs.get("access_token")
+        self.access_expiration = kwargs.get("access_expiration")
+        self.refresh_token = kwargs.get("refresh_token")
         self._kwargs = kwargs
-        if not kwargs.get('no_update_token', False):
+        if not kwargs.get("no_update_token", False):
             self._try_refresh_access_token()
             self._update_access_token_header()
 
-    def copy(self) -> 'Preston':
+    def copy(self) -> "Preston":
         """Creates a copy of this Preston object.
 
         The returned instance is not connected to this, so you can set
         whichever headers or other data you want without impacting this instance.
 
         The configuration of the returned instance will match the (original)
         configuration of this instance - the kwargs are reused.
@@ -96,35 +96,34 @@
         Args:
             None
 
         Returns:
             new access token and expiration time (from now)
         """
         headers = self._get_authorization_headers()
-        data = {
-            'grant_type': 'refresh_token',
-            'refresh_token': self.refresh_token
-        }
+        data = {"grant_type": "refresh_token", "refresh_token": self.refresh_token}
         r = self.session.post(self.TOKEN_URL, headers=headers, data=data)
         response_data = r.json()
-        return (response_data['access_token'], response_data['expires_in'])
+        return (response_data["access_token"], response_data["expires_in"])
 
     def _get_authorization_headers(self) -> dict:
         """Constructs and returns the Authorization header for the client app.
 
         Args:
             None
 
         Returns:
             header dict for communicating with the authorization endpoints
         """
-        auth = base64.encodestring((self.client_id + ':' + self.client_secret).encode('latin-1')).decode('latin-1')
-        auth = auth.replace('\n', '').replace(' ', '')
-        auth = 'Basic {}'.format(auth)
-        headers = {'Authorization': auth}
+        auth = base64.encodebytes(
+            bytes(f"{self.client_id}:{self.client_secret}", "latin-1")
+        ).decode("latin-1")
+        auth = auth.replace("\n", "").replace(" ", "")
+        auth = "Basic {}".format(auth)
+        headers = {"Authorization": auth}
         return headers
 
     def _try_refresh_access_token(self) -> None:
         """Attempts to get a new access token using the refresh token, if needed.
 
         If the access token is expired and this instance has a stored refresh token,
         then the refresh token is in the API call to get a new access token. If
@@ -134,15 +133,18 @@
             None
 
         Returns:
             None
         """
         if self.refresh_token:
             if not self.access_token or self._is_access_token_expired():
-                self.access_token, self.access_expiration = self._get_access_from_refresh()
+                (
+                    self.access_token,
+                    self.access_expiration,
+                ) = self._get_access_from_refresh()
                 self.access_expiration = time.time() + self.access_expiration
 
     def _is_access_token_expired(self) -> bool:
         """Returns true if the stored access token has expired.
 
         Args:
             None
@@ -162,19 +164,19 @@
         Args:
             None
 
         Returns:
             URL
         """
         return (
-            f'{self.AUTHORIZE_URL}?response_type=code&redirect_uri={self.callback_url}'
-            f'&client_id={self.client_id}&scope={self.scope}'
+            f"{self.AUTHORIZE_URL}?response_type=code&redirect_uri={self.callback_url}"
+            f"&client_id={self.client_id}&scope={self.scope}"
         )
 
-    def authenticate(self, code: str) -> 'Preston':
+    def authenticate(self, code: str) -> "Preston":
         """Authenticates using the code from the EVE SSO.
 
         A new Preston object is returned; this object is not modified.
 
         The intended usage is:
 
             auth = preston.authenticate('some_code_here')
@@ -182,26 +184,27 @@
         Args:
             code: SSO code
 
         Returns:
             new Preston, authenticated
         """
         headers = self._get_authorization_headers()
-        data = {
-            'grant_type': 'authorization_code',
-            'code': code
-        }
+        data = {"grant_type": "authorization_code", "code": code}
         r = self.session.post(self.TOKEN_URL, headers=headers, data=data)
         if not r.status_code == 200:
-            raise Exception(f'Could not authenticate, got repsonse code {r.status_code}')
+            raise Exception(
+                f"Could not authenticate, got repsonse code {r.status_code}"
+            )
         new_kwargs = dict(self._kwargs)
         response_data = r.json()
-        new_kwargs['access_token'] = response_data['access_token']
-        new_kwargs['access_expiration'] = time.time() + float(response_data['expires_in'])
-        new_kwargs['refresh_token'] = response_data['refresh_token']
+        new_kwargs["access_token"] = response_data["access_token"]
+        new_kwargs["access_expiration"] = time.time() + float(
+            response_data["expires_in"]
+        )
+        new_kwargs["refresh_token"] = response_data["refresh_token"]
         return Preston(**new_kwargs)
 
     def _update_access_token_header(self) -> None:
         """Updates the requests session with the access token header.
 
         This method does nothing if this instance does not have a
         stored access token.
@@ -209,17 +212,17 @@
         Args:
             None
 
         Returns:
             None
         """
         if self.access_token:
-            self.session.headers.update({
-                'Authorization': f'Bearer {self.access_token}'
-            })
+            self.session.headers.update(
+                {"Authorization": f"Bearer {self.access_token}"}
+            )
 
     def _get_spec(self) -> dict:
         """Fetches the OpenAPI spec from the server.
 
         If the spec has already been fetched, the cached version is returned instead.
 
         ArgS:
@@ -238,15 +241,15 @@
 
         Args:
             id: operation id
 
         Returns:
             path to the endpoint, or None if not found
         """
-        for path_key, path_value in self._get_spec()['paths'].items():
+        for path_key, path_value in self._get_spec()["paths"].items():
             for method in self.METHODS:
                 if method in path_value:
                     if self.OPERATION_ID_KEY in path_value[method]:
                         if path_value[method][self.OPERATION_ID_KEY] == id:
                             return path_key
         return None
 
@@ -323,15 +326,17 @@
 
         Returns:
             ESI data
         """
         path = self._get_path_for_op_id(id)
         return self.get_path(path, kwargs)
 
-    def post_path(self, path: str, path_data: Union[dict, None], post_data: Any) -> dict:
+    def post_path(
+        self, path: str, path_data: Union[dict, None], post_data: Any
+    ) -> dict:
         """Modifies the ESI by an endpoint URL.
 
         This method is not marked "private" as it _can_ be used
         by consuming code, but it's probably easier to call the
         `get_op` method instead.
 
         Args:
```

### Comparing `Preston-4.1.0/README.md` & `preston-4.1.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,30 @@
 # Preston
 
-[![Build Status](https://travis-ci.org/Celeo/Preston.svg?branch=master)](https://travis-ci.org/Celeo/Preston)
-[![codecov](https://codecov.io/gh/Celeo/Preston/branch/master/graph/badge.svg)](https://codecov.io/gh/Celeo/Preston)
+[![CI](https://github.com/Celeo/preston/workflows/CI/badge.svg?branch=master)](https://github.com/Celeo/preston/actions?query=workflow%3ACI)
+[![codecov](https://codecov.io/gh/Celeo/preston/branch/master/graph/badge.svg?token=2R9RY3P229)](https://codecov.io/gh/Celeo/preston)
+[![Python version](https://img.shields.io/badge/Python-3.6+-blue)](https://www.python.org/)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![License](https://img.shields.io/badge/License-MIT-green)](LICENSE)
 
 Preston is a Python library for accessing EVE Online's ESI API.
 
 ## Quick links
 
-* EVE ESI: https://esi.tech.ccp.is/
-* EVE third-party documentation: http://eveonline-third-party-documentation.readthedocs.io
-* EVE developers: https://developers.eveonline.com/
+* EVE ESI: <https://esi.tech.ccp.is/>
+* EVE developers: <https://developers.eveonline.com/>
 
 ## Installation
 
 From [pip](https://pip.pypa.io/en/stable/):
 
-```bash
+```sh
 pip install preston
 ```
 
-From GitHub:
-
-```bash
-git clone https://github.com/Celeo/Preston.git
-cd Preston
-python setup.py install
-```
-
 ## Initialization
 
 ```python
 from preston import Preston
 
 preston = Preston()
 ```
@@ -114,10 +108,40 @@
 ```
 
 Preston will take the refresh token and attempt to get a new access token from it.
 
 On that note, you can also pass the `access_token` to a new Preston instance, but there's less of a use case for that, as either you have an app with scopes, yielding a refresh token,
 or an authentication-only app where you only use the access token to verify identity and some basic information before moving on.
 
+## Developing
+
+### Building
+
+### Requirements
+
+* Git
+* Poetry
+* Python 3.6+
+
+### Steps
+
+```sh
+git clone https://github.com/Celeo/preston
+cd preston
+poetry install
+```
+
+### Running tests
+
+| | |
+| --- | --- |
+| No coverage | `poetry run pytest`
+| Coverage printout | `poetry run pytest --cov=preston` |
+| Coverage report | `poetry run pytest --cov=preston --cov-report=html` |
+
+## License
+
+Licensed under MIT ([LICENSE](LICENSE)).
+
 ## Contributing
 
 PRs are welcome. Please follow PEP8 (I'm lenient on E501) and use [Google-style docstrings](https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_google.html).
```

