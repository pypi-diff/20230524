# Comparing `tmp/versium-reach-sdk-1.0.0.tar.gz` & `tmp/versium-reach-sdk-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "versium-reach-sdk-1.0.0.tar", last modified: Thu Dec  8 21:17:34 2022, max compression
+gzip compressed data, was "versium-reach-sdk-1.1.0.tar", last modified: Wed May 24 18:17:34 2023, max compression
```

## Comparing `versium-reach-sdk-1.0.0.tar` & `versium-reach-sdk-1.1.0.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 mbaumgartner   (502) staff       (20)        0 2022-12-08 21:17:34.625187 versium-reach-sdk-1.0.0/
--rw-r--r--   0 mbaumgartner   (502) staff       (20)     1474 2022-09-08 12:45:20.000000 versium-reach-sdk-1.0.0/LICENSE
--rw-r--r--   0 mbaumgartner   (502) staff       (20)       24 2022-12-06 22:42:05.000000 versium-reach-sdk-1.0.0/MANIFEST.in
--rw-r--r--   0 mbaumgartner   (502) staff       (20)     5406 2022-12-08 21:17:34.625053 versium-reach-sdk-1.0.0/PKG-INFO
--rwxr-xr-x   0 mbaumgartner   (502) staff       (20)     2797 2022-12-08 21:13:03.000000 versium-reach-sdk-1.0.0/README.md
--rw-r--r--   0 mbaumgartner   (502) staff       (20)      976 2022-12-06 22:35:01.000000 versium-reach-sdk-1.0.0/pyproject.toml
-drwxr-xr-x   0 mbaumgartner   (502) staff       (20)        0 2022-12-08 21:17:34.623099 versium-reach-sdk-1.0.0/reach/
--rwxr-xr-x   0 mbaumgartner   (502) staff       (20)       66 2022-12-01 19:50:32.000000 versium-reach-sdk-1.0.0/reach/__init__.py
--rwxr-xr-x   0 mbaumgartner   (502) staff       (20)     4320 2022-12-01 19:07:23.000000 versium-reach-sdk-1.0.0/reach/append.py
--rw-r--r--   0 mbaumgartner   (502) staff       (20)     2199 2022-12-01 19:35:36.000000 versium-reach-sdk-1.0.0/reach/query_data.py
--rw-r--r--   0 mbaumgartner   (502) staff       (20)     2473 2022-12-01 19:07:23.000000 versium-reach-sdk-1.0.0/reach/rate_limiter.py
--rwxr-xr-x   0 mbaumgartner   (502) staff       (20)     3536 2022-12-01 19:07:23.000000 versium-reach-sdk-1.0.0/reach/reach.py
--rwxr-xr-x   0 mbaumgartner   (502) staff       (20)       14 2022-12-01 01:40:48.000000 versium-reach-sdk-1.0.0/requirements.txt
--rw-r--r--   0 mbaumgartner   (502) staff       (20)       38 2022-12-08 21:17:34.625223 versium-reach-sdk-1.0.0/setup.cfg
--rw-r--r--   0 mbaumgartner   (502) staff       (20)     2710 2022-12-06 22:20:24.000000 versium-reach-sdk-1.0.0/setup.py
-drwxr-xr-x   0 mbaumgartner   (502) staff       (20)        0 2022-12-08 21:17:34.624045 versium-reach-sdk-1.0.0/tests/
--rw-r--r--   0 mbaumgartner   (502) staff       (20)        0 2022-09-23 01:22:32.000000 versium-reach-sdk-1.0.0/tests/__init__.py
--rw-r--r--   0 mbaumgartner   (502) staff       (20)    17208 2022-12-01 19:16:18.000000 versium-reach-sdk-1.0.0/tests/responses.py
--rwxr-xr-x   0 mbaumgartner   (502) staff       (20)     2013 2022-12-01 01:50:48.000000 versium-reach-sdk-1.0.0/tests/test_append.py
--rw-r--r--   0 mbaumgartner   (502) staff       (20)     5888 2022-12-01 19:16:18.000000 versium-reach-sdk-1.0.0/tests/utils.py
-drwxr-xr-x   0 mbaumgartner   (502) staff       (20)        0 2022-12-08 21:17:34.624880 versium-reach-sdk-1.0.0/versium_reach_sdk.egg-info/
--rw-r--r--   0 mbaumgartner   (502) staff       (20)     5406 2022-12-08 21:17:34.000000 versium-reach-sdk-1.0.0/versium_reach_sdk.egg-info/PKG-INFO
--rw-r--r--   0 mbaumgartner   (502) staff       (20)      478 2022-12-08 21:17:34.000000 versium-reach-sdk-1.0.0/versium_reach_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 mbaumgartner   (502) staff       (20)        1 2022-12-08 21:17:34.000000 versium-reach-sdk-1.0.0/versium_reach_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 mbaumgartner   (502) staff       (20)        1 2022-12-06 22:37:10.000000 versium-reach-sdk-1.0.0/versium_reach_sdk.egg-info/not-zip-safe
--rw-r--r--   0 mbaumgartner   (502) staff       (20)       15 2022-12-08 21:17:34.000000 versium-reach-sdk-1.0.0/versium_reach_sdk.egg-info/requires.txt
--rw-r--r--   0 mbaumgartner   (502) staff       (20)       12 2022-12-08 21:17:34.000000 versium-reach-sdk-1.0.0/versium_reach_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 mbaumgartner   (502) staff       (20)        0 2023-05-24 18:17:34.657229 versium-reach-sdk-1.1.0/
+-rw-r--r--   0 mbaumgartner   (502) staff       (20)     1474 2022-09-08 12:45:20.000000 versium-reach-sdk-1.1.0/LICENSE
+-rw-r--r--   0 mbaumgartner   (502) staff       (20)       24 2022-12-08 21:42:49.000000 versium-reach-sdk-1.1.0/MANIFEST.in
+-rw-r--r--   0 mbaumgartner   (502) staff       (20)     5474 2023-05-24 18:17:34.657074 versium-reach-sdk-1.1.0/PKG-INFO
+-rwxr-xr-x   0 mbaumgartner   (502) staff       (20)     2865 2023-05-24 17:57:16.000000 versium-reach-sdk-1.1.0/README.md
+-rw-r--r--   0 mbaumgartner   (502) staff       (20)      976 2023-05-24 17:57:16.000000 versium-reach-sdk-1.1.0/pyproject.toml
+drwxr-xr-x   0 mbaumgartner   (502) staff       (20)        0 2023-05-24 18:17:34.654264 versium-reach-sdk-1.1.0/reach/
+-rwxr-xr-x   0 mbaumgartner   (502) staff       (20)       66 2022-12-01 19:50:32.000000 versium-reach-sdk-1.1.0/reach/__init__.py
+-rwxr-xr-x   0 mbaumgartner   (502) staff       (20)     7305 2023-05-24 17:57:16.000000 versium-reach-sdk-1.1.0/reach/append.py
+-rw-r--r--   0 mbaumgartner   (502) staff       (20)     2304 2023-05-24 17:57:16.000000 versium-reach-sdk-1.1.0/reach/query_data.py
+-rw-r--r--   0 mbaumgartner   (502) staff       (20)     3470 2023-05-24 17:57:16.000000 versium-reach-sdk-1.1.0/reach/rate_limiter.py
+-rwxr-xr-x   0 mbaumgartner   (502) staff       (20)     3904 2023-05-24 17:57:16.000000 versium-reach-sdk-1.1.0/reach/reach.py
+-rwxr-xr-x   0 mbaumgartner   (502) staff       (20)       14 2022-12-01 01:40:48.000000 versium-reach-sdk-1.1.0/requirements.txt
+-rw-r--r--   0 mbaumgartner   (502) staff       (20)       38 2023-05-24 18:17:34.657271 versium-reach-sdk-1.1.0/setup.cfg
+-rw-r--r--   0 mbaumgartner   (502) staff       (20)     2710 2023-05-24 17:57:16.000000 versium-reach-sdk-1.1.0/setup.py
+drwxr-xr-x   0 mbaumgartner   (502) staff       (20)        0 2023-05-24 18:17:34.655941 versium-reach-sdk-1.1.0/tests/
+-rw-r--r--   0 mbaumgartner   (502) staff       (20)        0 2022-09-23 01:22:32.000000 versium-reach-sdk-1.1.0/tests/__init__.py
+-rw-r--r--   0 mbaumgartner   (502) staff       (20)     1491 2023-05-24 17:57:16.000000 versium-reach-sdk-1.1.0/tests/base.py
+-rw-r--r--   0 mbaumgartner   (502) staff       (20)    17208 2022-12-01 19:16:18.000000 versium-reach-sdk-1.1.0/tests/responses.py
+-rwxr-xr-x   0 mbaumgartner   (502) staff       (20)     4453 2023-05-24 17:57:16.000000 versium-reach-sdk-1.1.0/tests/test_append.py
+-rwxr-xr-x   0 mbaumgartner   (502) staff       (20)      673 2023-05-24 17:57:16.000000 versium-reach-sdk-1.1.0/tests/test_reach_client.py
+-rw-r--r--   0 mbaumgartner   (502) staff       (20)     6345 2023-05-24 17:57:16.000000 versium-reach-sdk-1.1.0/tests/utils.py
+drwxr-xr-x   0 mbaumgartner   (502) staff       (20)        0 2023-05-24 18:17:34.656878 versium-reach-sdk-1.1.0/versium_reach_sdk.egg-info/
+-rw-r--r--   0 mbaumgartner   (502) staff       (20)     5474 2023-05-24 18:17:34.000000 versium-reach-sdk-1.1.0/versium_reach_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 mbaumgartner   (502) staff       (20)      519 2023-05-24 18:17:34.000000 versium-reach-sdk-1.1.0/versium_reach_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 mbaumgartner   (502) staff       (20)        1 2023-05-24 18:17:34.000000 versium-reach-sdk-1.1.0/versium_reach_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 mbaumgartner   (502) staff       (20)        1 2022-12-06 22:37:10.000000 versium-reach-sdk-1.1.0/versium_reach_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 mbaumgartner   (502) staff       (20)       15 2023-05-24 18:17:34.000000 versium-reach-sdk-1.1.0/versium_reach_sdk.egg-info/requires.txt
+-rw-r--r--   0 mbaumgartner   (502) staff       (20)       12 2023-05-24 18:17:34.000000 versium-reach-sdk-1.1.0/versium_reach_sdk.egg-info/top_level.txt
```

### Comparing `versium-reach-sdk-1.0.0/LICENSE` & `versium-reach-sdk-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `versium-reach-sdk-1.0.0/PKG-INFO` & `versium-reach-sdk-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: versium-reach-sdk
-Version: 1.0.0
+Version: 1.1.0
 Summary: Python SDK for querying Versium Reach APIs
 Home-page: https://github.com/VersiumAnalytics/reach-api-python-sdk
 Author: Versium Analytics, Inc.
 Author-email: "Versium Analytics, Inc." <opensource@versium.com>
 License: Copyright 2022 Versium Analytics, Inc.
         
         Redistribution and use in source and binary forms, with or without
@@ -70,15 +70,15 @@
 
 1) Import ReachClient into your program
 ```python
 from reach import ReachClient
 ```
 2) Pass your [API Key](https://app.versium.com/account/manage-api-keys) to the ReachClient constructor.
 ```python
-client = ReachClient('path-key-012345678')
+client = ReachClient('api-key-012345678')
 ```
 3) Run the `append` method of your `ReachClient` object with the API name, input records, desired outputs (if applicable),
 and any extra config parameters you wish to pass.
 ```python
 records = [{"first": "John", 
             "last": "Smith",
             "address": "123 Main St.",
@@ -122,11 +122,14 @@
         The body of the response as raw bytes
 
 
 - **request_error**:
         If the client errored out during a request, this stores the error object
 
 
+- **error_msg**:
+        Stores additional info about query errors.
+
 # Things to keep in mind
 - The default rate limit for Reach APIs is 20 queries per second
 - You must have a provisioned API key for this function to work. If you are unsure where to find your API key, 
 look at our [API key documentation](https://api-documentation.versium.com/docs/find-your-api-key)
```

### Comparing `versium-reach-sdk-1.0.0/README.md` & `versium-reach-sdk-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 1) Import ReachClient into your program
 ```python
 from reach import ReachClient
 ```
 2) Pass your [API Key](https://app.versium.com/account/manage-api-keys) to the ReachClient constructor.
 ```python
-client = ReachClient('path-key-012345678')
+client = ReachClient('api-key-012345678')
 ```
 3) Run the `append` method of your `ReachClient` object with the API name, input records, desired outputs (if applicable),
 and any extra config parameters you wish to pass.
 ```python
 records = [{"first": "John", 
             "last": "Smith",
             "address": "123 Main St.",
@@ -77,11 +77,14 @@
         The body of the response as raw bytes
 
 
 - **request_error**:
         If the client errored out during a request, this stores the error object
 
 
+- **error_msg**:
+        Stores additional info about query errors.
+
 # Things to keep in mind
 - The default rate limit for Reach APIs is 20 queries per second
 - You must have a provisioned API key for this function to work. If you are unsure where to find your API key, 
 look at our [API key documentation](https://api-documentation.versium.com/docs/find-your-api-key)
```

### Comparing `versium-reach-sdk-1.0.0/pyproject.toml` & `versium-reach-sdk-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "versium-reach-sdk"
-version = "1.0.0"
+version = "1.1.0"
 authors = [
   { name="Versium Analytics, Inc.", email="opensource@versium.com" },
 ]
 description = "Python SDK for querying Versium Reach APIs"
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.7"
```

### Comparing `versium-reach-sdk-1.0.0/reach/query_data.py` & `versium-reach-sdk-1.1.0/reach/query_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,29 +40,33 @@
         The headers of the response.
 
     body_raw: bytes
         The body of the response as raw bytes
 
     request_error: aiohttp.ClientError
         If the client errored out during a request, this stores the error object
+
+    error_msg: string
+        Additional error message
     """
 
     def __init__(self, body=None, success=False, match_found=False, *, http_status=None, reason=None, headers=None,
-                 body_raw=None, request_error=None):
+                 body_raw=None, request_error=None, error_msg=""):
         if body is None:
             body = {}
         self.body = body
         self.success = success
         self.match_found = match_found
         self.http_status = http_status
         self.headers = headers
         self.body = body
         self.body_raw = body_raw
         self.request_error = request_error
         self.reason = reason
+        self.error_msg = error_msg
 
     def __repr__(self):
         headers = str(self.headers)
         if len(headers) > 60:
             headers = headers[:60] + '...'
 
         body = str(self.body)
```

### Comparing `versium-reach-sdk-1.0.0/reach/rate_limiter.py` & `versium-reach-sdk-1.1.0/reach/rate_limiter.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import asyncio
+import logging
 import time
 
+logger = logging.getLogger(__name__)
+
 
 class RateLimiter(object):
     """ Limits the number of calls to a function within a timeframe. Also limits the number of total active function calls.
 
     Parameters
     ----------
     max_calls : int
@@ -30,34 +33,61 @@
         self.retry_wait_time = retry_wait_time
         self.clock = time.monotonic
         self.last_reset = 0
         self.num_calls = 0
         self.sem = asyncio.Semaphore(n_connections)
 
     def __call__(self, func):
+        """
+
+        Parameters
+        ----------
+        func : Callable
+            function that returns a QueryResult object
+
+        Returns
+        -------
+        Callable: Input function wrapped with a rate limiting functionality
+        """
 
         async def wrapper(*args, **kwargs):
             # Semaphore will block more than {self.max_connections} from happening at once.
             self.last_reset = self.clock()
             async with self.sem:
                 for i in range(self.n_retry + 1):
                     while self.num_calls >= self.max_calls:
                         await asyncio.sleep(self.__period_remaining())
 
                     self.num_calls += 1
-                    result = await func(*args, attempts_left=self.n_retry - i, **kwargs)
-                    if not result.success and self.n_retry - i > 0:
-                        await asyncio.sleep(self.retry_wait_time * i)
+                    result = await func(*args, **kwargs)
+                    if result.success:
+                        return result
 
+                    if (result.http_status in (429, 500)) and (self.n_retry - i > 0):
+                        logger.error(result.error_msg + f"\n\tAttempts Left: {self.n_retry - i: d}")
+                        await asyncio.sleep(self.retry_wait_time * i)
+                        continue
+                    elif self.n_retry - i <= 0:
+                        logger.error(result.error_msg + f"\n\tNo attempts left.")
                     else:
-                        return result
+                        logger.error(result.error_msg + f"\n\tNot retrying for http status: {result.http_status}")
+
+                    return result
 
         return wrapper
 
     def __period_remaining(self):
+        """ Gets the amount of time remaining in the period. If there is no time remaining, resets the call counter and updates the reset
+        timer.
+
+        Returns
+        -------
+        float: Amount of time remaining in this period
+
+        """
         elapsed = self.clock() - self.last_reset
         period_remaining = self.period - elapsed
         if period_remaining <= 0:
             self.num_calls = 0
             self.last_reset = self.clock()
             period_remaining = self.period
         return max(period_remaining, 0)
```

### Comparing `versium-reach-sdk-1.0.0/reach/reach.py` & `versium-reach-sdk-1.1.0/reach/reach.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from .append import query_api
 import logging
 
+CLIENT_SERVER_TIMEOUT_PADDING = 0.2
+
 logger = logging.getLogger(__name__)
 
 
 class ReachClient:
     """Client for querying Versium Reach APIs
 
     Parameters
@@ -36,14 +38,17 @@
         self.headers = {'Accept': 'application/json', 'x-versium-api-key': api_key}
         self.queries_per_second = queries_per_second
         self.n_connections = n_connections
         self.timeout = timeout
         self.n_retry = n_retry
         self.retry_wait_time = retry_wait_time
 
+        if timeout <= 0:
+            raise ValueError(f"`timeout` must be greater than 0! Instead got {timeout}.")
+
     def append(self, api_name, input_records, outputs=(), config_params=None):
         """Perform an append on the input records and return the results.
 
         Parameters
         ----------
         api_name : string
             Name of the api you wish to use (e.g. 'contact', 'demographic', 'firmographic', etc.).
@@ -59,19 +64,21 @@
         config_params: dict
             Configuration parameters to pass to each API call. See the Configuration Parameters section of https://api-documentation.versium.com/reference/common-api-inputs-and-options
 
         Returns
         -------
         list[QueryResult]: A list of QueryResult objects
         """
-        query_params = dict()
+        query_params = {"cfg_max_recs": 1}
         if config_params is None:
             config_params = dict()
 
         query_params.update(config_params)
+        # Pad the server-side timeout to be slightly less than client to get a response back.
+        query_params['rcfg_max_time'] = self.timeout - min(self.timeout/2.0, CLIENT_SERVER_TIMEOUT_PADDING)
 
         query_params["output[]"] = list(set(outputs))  # remove duplicate outputs
 
         logger.info(f"Reach API set to {api_name}.")
         logger.info(f"API outputs set to {outputs}.")
         logger.info(f"API config params set to {config_params}")
```

### Comparing `versium-reach-sdk-1.0.0/setup.py` & `versium-reach-sdk-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     with open(path.join(here, 'requirements.txt'), encoding='utf-8') as f:
         required_packages = f.read().splitlines()
 
     cmdclass = {'clean': CleanCommand}
 
     setup(
             name='versium-reach-sdk',
-            version='1.0.0',
+            version='1.1.0',
             description='Python SDK for querying Versium Reach APIs',
             long_description=long_description,
             url='https://github.com/VersiumAnalytics/reach-api-python-sdk',
             author='Versium Analytics, Inc.',
             author_email='opensource@versium.com',
             classifiers=[
                 "Programming Language :: Python :: 3",
```

### Comparing `versium-reach-sdk-1.0.0/tests/responses.py` & `versium-reach-sdk-1.1.0/tests/responses.py`

 * *Files identical despite different names*

### Comparing `versium-reach-sdk-1.0.0/tests/utils.py` & `versium-reach-sdk-1.1.0/tests/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+import itertools
 import logging
 import sys
 import time
 from asyncio import sleep
 from functools import partial
 
 from aiohttp import web
 
-from .responses import MOCK_RESPONSES, GENERIC_RESPONSE
+from .responses import MOCK_RESPONSES
 
 
 class RateLimitExceededError(RuntimeError):
     pass
 
 
 class LowQPSError(RuntimeError):
@@ -122,46 +123,61 @@
         elif self.highest_connections < self.min_connections:
             raise UnusedConnectionsError(f"Unused connections. Min number of connections was: {self.min_connections}. Instead got "
                                          f" {self.highest_connections} connections.")
 
 
 class RequestHandler:
 
-    def __init__(self, rate_checker, response_time=0.0):
+    def __init__(self, rate_checker, response_time=0.0, http_status=200, store_requests=True):
         self.rate_checker = rate_checker
         self.response_time = response_time
+        self.http_status = http_status
+        self.store_requests = store_requests
+        self.requests = []
 
-    async def test_ratelimit(self, request):
+    @property
+    def http_status(self):
+        return self._http_status
+
+    @http_status.setter
+    def http_status(self, value):
+        # Make http_status into an iterable
+        try:
+            iter(value)
+        except TypeError:
+            value = [value]
+        self._http_status = itertools.cycle(value)
+
+    async def handle_request(self, api, request):
+        if self.store_requests:
+            self.requests += [request]
+        response = MOCK_RESPONSES[api.lower()]
         self.rate_checker.add_connection()
         try:
             self.rate_checker()
             await sleep(self.response_time)
-            return web.json_response(GENERIC_RESPONSE)
+            return web.json_response(response, status=next(self.http_status))
         finally:
             self.rate_checker.remove_connection()
 
-    async def handle_request(self, api, request):
-        return MOCK_RESPONSES[api.tolower()]
-
     async def handle_request_delayed(self, api, request):
         await sleep(self.response_time)
         return self.handle_request(api, request)
 
 
 def make_app(rh: RequestHandler):
     logger = logging.getLogger(__name__)
     logger.setLevel('DEBUG')
     sh = logging.StreamHandler(sys.stderr)
     logger.addHandler(sh)
     logger.handlers = []
 
     app = web.Application(logger=logger)
     app.router.add_routes(
-        [web.post('/v2/test_rate_limit', rh.test_ratelimit),
-         web.post('/v2/contact', partial(rh.handle_request, 'contact')),
+        [web.post('/v2/contact', partial(rh.handle_request, 'contact')),
          web.post('/v2/demographic', partial(rh.handle_request, 'demographic')),
          web.post('/v2/b2cOnlineAudience', partial(rh.handle_request, 'b2cOnlineAudience')),
          web.post('/v2/b2bOnlineAudience', partial(rh.handle_request, 'b2bOnlineAudience')),
          web.post('/v2/firmographic', partial(rh.handle_request, 'firmographic')),
          web.post('/v2/c2b', partial(rh.handle_request, 'c2b')),
          web.post('/v2/iptodomain', partial(rh.handle_request, 'iptodomain')),
          web.post('/v2/hemtobusinessdomain', partial(rh.handle_request, 'hemtobusinessdomain'))])
```

### Comparing `versium-reach-sdk-1.0.0/versium_reach_sdk.egg-info/PKG-INFO` & `versium-reach-sdk-1.1.0/versium_reach_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: versium-reach-sdk
-Version: 1.0.0
+Version: 1.1.0
 Summary: Python SDK for querying Versium Reach APIs
 Home-page: https://github.com/VersiumAnalytics/reach-api-python-sdk
 Author: Versium Analytics, Inc.
 Author-email: "Versium Analytics, Inc." <opensource@versium.com>
 License: Copyright 2022 Versium Analytics, Inc.
         
         Redistribution and use in source and binary forms, with or without
@@ -70,15 +70,15 @@
 
 1) Import ReachClient into your program
 ```python
 from reach import ReachClient
 ```
 2) Pass your [API Key](https://app.versium.com/account/manage-api-keys) to the ReachClient constructor.
 ```python
-client = ReachClient('path-key-012345678')
+client = ReachClient('api-key-012345678')
 ```
 3) Run the `append` method of your `ReachClient` object with the API name, input records, desired outputs (if applicable),
 and any extra config parameters you wish to pass.
 ```python
 records = [{"first": "John", 
             "last": "Smith",
             "address": "123 Main St.",
@@ -122,11 +122,14 @@
         The body of the response as raw bytes
 
 
 - **request_error**:
         If the client errored out during a request, this stores the error object
 
 
+- **error_msg**:
+        Stores additional info about query errors.
+
 # Things to keep in mind
 - The default rate limit for Reach APIs is 20 queries per second
 - You must have a provisioned API key for this function to work. If you are unsure where to find your API key, 
 look at our [API key documentation](https://api-documentation.versium.com/docs/find-your-api-key)
```

