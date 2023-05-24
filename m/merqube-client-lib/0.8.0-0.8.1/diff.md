# Comparing `tmp/merqube_client_lib-0.8.0.tar.gz` & `tmp/merqube_client_lib-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "merqube_client_lib-0.8.0.tar", max compression
+gzip compressed data, was "merqube_client_lib-0.8.1.tar", max compression
```

## Comparing `merqube_client_lib-0.8.0.tar` & `merqube_client_lib-0.8.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    11357 2023-05-16 20:00:52.711122 merqube_client_lib-0.8.0/LICENSE
--rw-r--r--   0        0        0     5272 2023-05-16 20:00:52.711122 merqube_client_lib-0.8.0/README.md
--rw-r--r--   0        0        0        0 2023-05-16 20:00:52.711122 merqube_client_lib-0.8.0/merqube_client_lib/__init__.py
--rw-r--r--   0        0        0        0 2023-05-16 20:00:52.711122 merqube_client_lib-0.8.0/merqube_client_lib/api_client/__init__.py
--rw-r--r--   0        0        0     1129 2023-05-16 20:00:52.711122 merqube_client_lib-0.8.0/merqube_client_lib/api_client/base.py
--rw-r--r--   0        0        0     2535 2023-05-16 20:00:52.711122 merqube_client_lib-0.8.0/merqube_client_lib/api_client/indexapi.py
--rw-r--r--   0        0        0     6722 2023-05-16 20:00:52.711122 merqube_client_lib-0.8.0/merqube_client_lib/api_client/merqube_client.py
--rw-r--r--   0        0        0    11322 2023-05-16 20:00:52.711122 merqube_client_lib-0.8.0/merqube_client_lib/api_client/secapi.py
--rw-r--r--   0        0        0      367 2023-05-16 20:00:52.711122 merqube_client_lib-0.8.0/merqube_client_lib/constants.py
--rw-r--r--   0        0        0      482 2023-05-16 20:00:52.711122 merqube_client_lib-0.8.0/merqube_client_lib/exceptions.py
--rw-r--r--   0        0        0     1934 2023-05-16 20:00:52.711122 merqube_client_lib-0.8.0/merqube_client_lib/logging.py
--rw-r--r--   0        0        0     4170 2023-05-16 20:00:52.711122 merqube_client_lib-0.8.0/merqube_client_lib/mocker.py
--rw-r--r--   0        0        0        0 2023-05-16 20:00:52.711122 merqube_client_lib-0.8.0/merqube_client_lib/py.typed
--rw-r--r--   0        0        0    71154 2023-05-16 20:00:52.711122 merqube_client_lib-0.8.0/merqube_client_lib/pydantic_types.py
--rw-r--r--   0        0        0        0 2023-05-16 20:00:52.711122 merqube_client_lib-0.8.0/merqube_client_lib/secapi/__init__.py
--rw-r--r--   0        0        0    11497 2023-05-16 20:00:52.711122 merqube_client_lib-0.8.0/merqube_client_lib/session.py
--rw-r--r--   0        0        0      414 2023-05-16 20:00:52.711122 merqube_client_lib-0.8.0/merqube_client_lib/types/__init__.py
--rw-r--r--   0        0        0      418 2023-05-16 20:00:52.711122 merqube_client_lib-0.8.0/merqube_client_lib/types/secapi.py
--rw-r--r--   0        0        0      677 2023-05-16 20:00:52.711122 merqube_client_lib-0.8.0/merqube_client_lib/util.py
--rw-r--r--   0        0        0     1829 2023-05-16 20:00:52.715122 merqube_client_lib-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     6013 1970-01-01 00:00:00.000000 merqube_client_lib-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-24 12:45:17.984340 merqube_client_lib-0.8.1/LICENSE
+-rw-r--r--   0        0        0     5272 2023-05-24 12:45:17.984340 merqube_client_lib-0.8.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-24 12:45:17.988340 merqube_client_lib-0.8.1/merqube_client_lib/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:45:17.988340 merqube_client_lib-0.8.1/merqube_client_lib/api_client/__init__.py
+-rw-r--r--   0        0        0     1129 2023-05-24 12:45:17.988340 merqube_client_lib-0.8.1/merqube_client_lib/api_client/base.py
+-rw-r--r--   0        0        0     2535 2023-05-24 12:45:17.988340 merqube_client_lib-0.8.1/merqube_client_lib/api_client/indexapi.py
+-rw-r--r--   0        0        0     6722 2023-05-24 12:45:17.988340 merqube_client_lib-0.8.1/merqube_client_lib/api_client/merqube_client.py
+-rw-r--r--   0        0        0    11322 2023-05-24 12:45:17.988340 merqube_client_lib-0.8.1/merqube_client_lib/api_client/secapi.py
+-rw-r--r--   0        0        0      367 2023-05-24 12:45:17.988340 merqube_client_lib-0.8.1/merqube_client_lib/constants.py
+-rw-r--r--   0        0        0      595 2023-05-24 12:45:17.988340 merqube_client_lib-0.8.1/merqube_client_lib/exceptions.py
+-rw-r--r--   0        0        0     1934 2023-05-24 12:45:17.988340 merqube_client_lib-0.8.1/merqube_client_lib/logging.py
+-rw-r--r--   0        0        0     4170 2023-05-24 12:45:17.988340 merqube_client_lib-0.8.1/merqube_client_lib/mocker.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:45:17.988340 merqube_client_lib-0.8.1/merqube_client_lib/py.typed
+-rw-r--r--   0        0        0    71154 2023-05-24 12:45:17.988340 merqube_client_lib-0.8.1/merqube_client_lib/pydantic_types.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:45:17.988340 merqube_client_lib-0.8.1/merqube_client_lib/secapi/__init__.py
+-rw-r--r--   0        0        0    11638 2023-05-24 12:45:17.988340 merqube_client_lib-0.8.1/merqube_client_lib/session.py
+-rw-r--r--   0        0        0      414 2023-05-24 12:45:17.988340 merqube_client_lib-0.8.1/merqube_client_lib/types/__init__.py
+-rw-r--r--   0        0        0      418 2023-05-24 12:45:17.988340 merqube_client_lib-0.8.1/merqube_client_lib/types/secapi.py
+-rw-r--r--   0        0        0      677 2023-05-24 12:45:17.988340 merqube_client_lib-0.8.1/merqube_client_lib/util.py
+-rw-r--r--   0        0        0     1829 2023-05-24 12:45:17.988340 merqube_client_lib-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     6013 1970-01-01 00:00:00.000000 merqube_client_lib-0.8.1/PKG-INFO
```

### Comparing `merqube_client_lib-0.8.0/LICENSE` & `merqube_client_lib-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `merqube_client_lib-0.8.0/README.md` & `merqube_client_lib-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `merqube_client_lib-0.8.0/merqube_client_lib/api_client/base.py` & `merqube_client_lib-0.8.1/merqube_client_lib/api_client/base.py`

 * *Files identical despite different names*

### Comparing `merqube_client_lib-0.8.0/merqube_client_lib/api_client/indexapi.py` & `merqube_client_lib-0.8.1/merqube_client_lib/api_client/indexapi.py`

 * *Files identical despite different names*

### Comparing `merqube_client_lib-0.8.0/merqube_client_lib/api_client/merqube_client.py` & `merqube_client_lib-0.8.1/merqube_client_lib/api_client/merqube_client.py`

 * *Files identical despite different names*

### Comparing `merqube_client_lib-0.8.0/merqube_client_lib/api_client/secapi.py` & `merqube_client_lib-0.8.1/merqube_client_lib/api_client/secapi.py`

 * *Files identical despite different names*

### Comparing `merqube_client_lib-0.8.0/merqube_client_lib/logging.py` & `merqube_client_lib-0.8.1/merqube_client_lib/logging.py`

 * *Files identical despite different names*

### Comparing `merqube_client_lib-0.8.0/merqube_client_lib/mocker.py` & `merqube_client_lib-0.8.1/merqube_client_lib/mocker.py`

 * *Files identical despite different names*

### Comparing `merqube_client_lib-0.8.0/merqube_client_lib/pydantic_types.py` & `merqube_client_lib-0.8.1/merqube_client_lib/pydantic_types.py`

 * *Files identical despite different names*

### Comparing `merqube_client_lib-0.8.0/merqube_client_lib/session.py` & `merqube_client_lib-0.8.1/merqube_client_lib/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,31 +163,23 @@
             In [6]: urljoin("https://localhost:8080", "//resource")
             Out[6]: 'https://resource' # ??
         """
         assert params is None or options is None, "both params and options cannot be passed"
         if url.startswith("//"):
             logger.warning(f"URL {url} starts with //, this is probably a mistake")
 
-        headers = dict(headers) if headers is not None else {}
-
-        # Generate a new requestid if this call isnt being made in a chain that already has it.
-        # (eg client calls dataapi, dataapi calls secapi - we dont want the second call to overwrite the original)
-        # if this isnt set by a client making a call to one of our APIs, the API itself will generate one (eg customer call)
-        # order is: 1) explicitly specified 2) set via chain, 3) generate new
-        headers[REQUEST_ID_HEADER] = headers.get(
-            REQUEST_ID_HEADER, os.getenv(MERQ_REQUEST_ID_ENV_VAR, str(uuid.uuid4()))
-        )
-
+        headers = headers or {}
         if self.token:
             headers["Authorization"] = f"{self.token_type} {self.token}"
 
         options_st = "" if not options else ("?" + "&".join([f"{k}={v}" for k, v in options.items()]))
         url = urljoin(self._prefix_url, url)
         logger.debug(f"Performing {method} on {url}{options_st}")
         options_dict: dict[str, str] = options or {}
+
         return self.http_session.request(
             method=method.value, url=url, params=options_dict or params, data=data, headers=headers, **kwargs
         )
 
     def get(self, url: str, **kwargs: Any) -> Response:
         """
         requests.Session like http GET method
@@ -232,32 +224,42 @@
         self,
         token: str | None = None,
         **kwargs: Any,
     ):
         """can specify your own oauth token,default is no token (only public APIs)"""
         super().__init__(token=token, **kwargs)
 
-    def handle_nonrecoverable(self, res: Response, e: Exception) -> None:
+    def handle_nonrecoverable(self, res: Response, exc: Exception, req_id: str) -> None:
         """helper function that handles a non recoverable error"""
-        logger.exception(e)
+        logger.exception(exc)
         try:
             # we may not have a json depending on the response
             rj = res.json()
         except (AttributeError, json.decoder.JSONDecodeError):
             rj = {}
-        logger.debug(f"Request failed with status {res.status_code}: {rj}")
-        raise APIError(code=res.status_code, response_json=rj)
+        logger.debug(f"Request failed with status {res.status_code}: {rj}. Request ID: {req_id}")
+        raise APIError(code=res.status_code, response_json=rj, request_id=req_id)
 
     def request_raise(self, method: httpm, url: str, **kwargs: Any) -> Response:
         """request method that logs the status code and raises on non 2XX"""
-        res = self.request(method, url, **kwargs)
+
+        # Generate a new requestid if this call isnt being made in a chain that already has it.
+        # (eg client calls dataapi, dataapi calls secapi - we dont want the second call to overwrite the original)
+        # if this isnt set by a client making a call to one of our APIs, the API itself will generate one (eg customer call)
+        # order is: 1) explicitly specified 2) set via chain, 3) generate new
+        headers = kwargs.pop("headers", {}) or {}
+        headers[REQUEST_ID_HEADER] = (
+            req_id := headers.get(REQUEST_ID_HEADER, os.getenv(MERQ_REQUEST_ID_ENV_VAR, str(uuid.uuid4())))
+        )
+
+        res = self.request(method=method, url=url, headers=headers, **kwargs)
         try:
             res.raise_for_status()
         except HTTPError as e:
-            self.handle_nonrecoverable(res, e)
+            self.handle_nonrecoverable(res=res, exc=e, req_id=req_id)
 
         return res
 
     def get(self, url: str, **kwargs: Any) -> Response:
         return self.request_raise(httpm.GET, url, **kwargs)
 
     def put(self, url: str, **kwargs: Any) -> Response:
```

### Comparing `merqube_client_lib-0.8.0/merqube_client_lib/util.py` & `merqube_client_lib-0.8.1/merqube_client_lib/util.py`

 * *Files identical despite different names*

### Comparing `merqube_client_lib-0.8.0/pyproject.toml` & `merqube_client_lib-0.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "merqube-client-lib"
-version = "0.8.0"
+version = "0.8.1"
 description = "MerQube IndexAPI + SecAPI client library"
 authors = ["Merqube"]
 readme = "README.md"
 license = "APACHE-2.0"
 homepage = "https://github.com/merqube/merqube-client-lib"
 include = [
     "LICENSE",
```

### Comparing `merqube_client_lib-0.8.0/PKG-INFO` & `merqube_client_lib-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merqube-client-lib
-Version: 0.8.0
+Version: 0.8.1
 Summary: MerQube IndexAPI + SecAPI client library
 Home-page: https://github.com/merqube/merqube-client-lib
 License: Apache-2.0
 Author: Merqube
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

