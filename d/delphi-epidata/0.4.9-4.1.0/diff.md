# Comparing `tmp/delphi_epidata-0.4.9.tar.gz` & `tmp/delphi_epidata-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delphi_epidata-0.4.9.tar", last modified: Wed Apr  5 15:40:12 2023, max compression
+gzip compressed data, was "delphi_epidata-4.1.0.tar", last modified: Wed May 24 15:24:40 2023, max compression
```

## Comparing `delphi_epidata-0.4.9.tar` & `delphi_epidata-4.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:40:12.578888 delphi_epidata-0.4.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-05 15:40:02.000000 delphi_epidata-0.4.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-05 15:40:12.578888 delphi_epidata-0.4.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-05 15:40:02.000000 delphi_epidata-0.4.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:40:12.578888 delphi_epidata-0.4.9/delphi_epidata/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-05 15:40:02.000000 delphi_epidata-0.4.9/delphi_epidata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24834 2023-04-05 15:40:11.000000 delphi_epidata-0.4.9/delphi_epidata/delphi_epidata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:40:12.578888 delphi_epidata-0.4.9/delphi_epidata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-05 15:40:12.000000 delphi_epidata-0.4.9/delphi_epidata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-05 15:40:12.000000 delphi_epidata-0.4.9/delphi_epidata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 15:40:12.000000 delphi_epidata-0.4.9/delphi_epidata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-05 15:40:12.000000 delphi_epidata-0.4.9/delphi_epidata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-05 15:40:12.000000 delphi_epidata-0.4.9/delphi_epidata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 15:40:12.578888 delphi_epidata-0.4.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-05 15:40:02.000000 delphi_epidata-0.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:40.041673 delphi_epidata-4.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-24 15:24:29.000000 delphi_epidata-4.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-24 15:24:40.041673 delphi_epidata-4.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-24 15:24:29.000000 delphi_epidata-4.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:40.041673 delphi_epidata-4.1.0/delphi_epidata/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-24 15:24:29.000000 delphi_epidata-4.1.0/delphi_epidata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25286 2023-05-24 15:24:38.000000 delphi_epidata-4.1.0/delphi_epidata/delphi_epidata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:40.041673 delphi_epidata-4.1.0/delphi_epidata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-24 15:24:39.000000 delphi_epidata-4.1.0/delphi_epidata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-24 15:24:40.000000 delphi_epidata-4.1.0/delphi_epidata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:24:39.000000 delphi_epidata-4.1.0/delphi_epidata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-24 15:24:39.000000 delphi_epidata-4.1.0/delphi_epidata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-24 15:24:39.000000 delphi_epidata-4.1.0/delphi_epidata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 15:24:40.041673 delphi_epidata-4.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-24 15:24:29.000000 delphi_epidata-4.1.0/setup.py
```

### Comparing `delphi_epidata-0.4.9/LICENSE` & `delphi_epidata-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `delphi_epidata-0.4.9/PKG-INFO` & `delphi_epidata-4.1.0/delphi_epidata.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: delphi_epidata
-Version: 0.4.9
+Name: delphi-epidata
+Version: 4.1.0
 Summary: A programmatic interface to Delphi's Epidata API.
 Home-page: https://github.com/cmu-delphi/delphi-epidata
 Author: David Farrow
 Author-email: dfarrow0@gmail.com
 License: UNKNOWN
 Description: # Delphi Epidata API Client
```

### Comparing `delphi_epidata-0.4.9/delphi_epidata/delphi_epidata.py` & `delphi_epidata-4.1.0/delphi_epidata/delphi_epidata.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,35 +9,36 @@
 """
 
 # External modules
 import requests
 import asyncio
 from tenacity import retry, stop_after_attempt
 
-from aiohttp import ClientSession, TCPConnector
+from aiohttp import ClientSession, TCPConnector, BasicAuth
 from pkg_resources import get_distribution, DistributionNotFound
 
 # Obtain package version for the user-agent. Uses the installed version by
 # preference, even if you've installed it and then use this script independently
 # by accident.
 try:
   _version = get_distribution('delphi-epidata').version
 except DistributionNotFound:
   _version = "0.script"
 
 _HEADERS = {
-  "user-agent": "delphi_epidata/" + _version
+  "user-agent": "delphi_epidata/" + _version + " (Python)"
 }
 
 # Because the API is stateless, the Epidata class only contains static methods
 class Epidata:
   """An interface to DELPHI's Epidata API."""
 
   # API base url
-  BASE_URL = 'https://delphi.cmu.edu/epidata/api.php'
+  BASE_URL = 'https://api.delphi.cmu.edu/epidata/api.php'
+  auth = None
 
   client_version = _version
 
   # Helper function to cast values and/or ranges to strings
   @staticmethod
   def _listitem(value):
     """Cast values and/or range to a string."""
@@ -54,35 +55,40 @@
       values = [values]
     return ','.join([Epidata._listitem(value) for value in values])
 
   @staticmethod
   @retry(reraise=True, stop=stop_after_attempt(2))
   def _request_with_retry(params):
     """Make request with a retry if an exception is thrown."""
-    req = requests.get(Epidata.BASE_URL, params, headers=_HEADERS)
+    req = requests.get(Epidata.BASE_URL, params, auth=Epidata.auth, headers=_HEADERS)
     if req.status_code == 414:
-      req = requests.post(Epidata.BASE_URL, params, headers=_HEADERS)
+      req = requests.post(Epidata.BASE_URL, params, auth=Epidata.auth, headers=_HEADERS)
+    # handle 401 and 429
+    req.raise_for_status()
     return req
 
   @staticmethod
   def _request(params):
     """Request and parse epidata.
 
     We default to GET since it has better caching and logging
     capabilities, but fall back to POST if the request is too
     long and returns a 414.
     """
     try:
       result = Epidata._request_with_retry(params)
-      if params is not None and "format" in params and params["format"]=="csv":
-        return result.text
-      else:
-        return result.json()
     except Exception as e:
       return {'result': 0, 'message': 'error: ' + str(e)}
+    if params is not None and "format" in params and params["format"]=="csv":
+      return result.text
+    else:
+      try:
+        return result.json()
+      except requests.exceptions.JSONDecodeError:
+        return {'result': 0, 'message': 'error decoding json: ' + result.text}
 
   # Raise an Exception on error, otherwise return epidata
   @staticmethod
   def check(resp):
     """Raise an Exception on error, otherwise return epidata."""
     if resp['result'] != 1:
       msg, code = resp['message'], resp['result']
@@ -732,15 +738,19 @@
         response.raise_for_status()
         return await response.json(), params
 
     async def async_make_calls(param_combos):
       """Helper function to asynchronously make and aggregate Epidata GET requests."""
       tasks = []
       connector = TCPConnector(limit=batch_size)
-      async with ClientSession(connector=connector, headers=_HEADERS) as session:
+      if isinstance(Epidata.auth, tuple):
+        auth = BasicAuth(login=Epidata.auth[0], password=Epidata.auth[1], encoding='utf-8')
+      else:
+        auth = Epidata.auth
+      async with ClientSession(connector=connector, headers=_HEADERS, auth=auth) as session:
         for param in param_combos:
           task = asyncio.ensure_future(async_get(param, session))
           tasks.append(task)
         responses = await asyncio.gather(*tasks)
         return responses
 
     loop = asyncio.get_event_loop()
```

### Comparing `delphi_epidata-0.4.9/delphi_epidata.egg-info/PKG-INFO` & `delphi_epidata-4.1.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: delphi-epidata
-Version: 0.4.9
+Name: delphi_epidata
+Version: 4.1.0
 Summary: A programmatic interface to Delphi's Epidata API.
 Home-page: https://github.com/cmu-delphi/delphi-epidata
 Author: David Farrow
 Author-email: dfarrow0@gmail.com
 License: UNKNOWN
 Description: # Delphi Epidata API Client
```

### Comparing `delphi_epidata-0.4.9/setup.py` & `delphi_epidata-4.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="delphi_epidata",
-    version="0.4.9",
+    version="4.1.0",
     author="David Farrow",
     author_email="dfarrow0@gmail.com",
     description="A programmatic interface to Delphi's Epidata API.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cmu-delphi/delphi-epidata",
     packages=setuptools.find_packages(),
```

