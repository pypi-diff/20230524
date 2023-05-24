# Comparing `tmp/pysnc-1.1.4.tar.gz` & `tmp/pysnc-1.1.5a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysnc-1.1.4.tar", max compression
+gzip compressed data, was "pysnc-1.1.5a0.tar", max compression
```

## Comparing `pysnc-1.1.4.tar` & `pysnc-1.1.5a0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1052 2023-05-08 21:40:28.445381 pysnc-1.1.4/LICENSE
--rw-r--r--   0        0        0     1590 2023-05-08 21:40:28.445381 pysnc-1.1.4/README.md
--rw-r--r--   0        0        0     1056 2023-05-08 21:40:28.445381 pysnc-1.1.4/pyproject.toml
--rw-r--r--   0        0        0      129 2023-05-08 21:40:28.445381 pysnc-1.1.4/pysnc/__init__.py
--rw-r--r--   0        0        0       98 2023-05-08 21:40:28.445381 pysnc-1.1.4/pysnc/__version__.py
--rw-r--r--   0        0        0     9386 2023-05-08 21:40:28.445381 pysnc-1.1.4/pysnc/attachment.py
--rw-r--r--   0        0        0     3757 2023-05-08 21:40:28.445381 pysnc-1.1.4/pysnc/auth.py
--rw-r--r--   0        0        0    15815 2023-05-08 21:40:28.445381 pysnc-1.1.4/pysnc/client.py
--rw-r--r--   0        0        0     1002 2023-05-08 21:40:28.445381 pysnc-1.1.4/pysnc/exceptions.py
--rw-r--r--   0        0        0     3867 2023-05-08 21:40:28.445381 pysnc-1.1.4/pysnc/query.py
--rw-r--r--   0        0        0    37895 2023-05-08 21:40:28.445381 pysnc-1.1.4/pysnc/record.py
--rw-r--r--   0        0        0      846 2023-05-08 21:40:28.445381 pysnc-1.1.4/pysnc/utils.py
--rw-r--r--   0        0        0     2664 1970-01-01 00:00:00.000000 pysnc-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1052 2023-05-24 21:33:54.039764 pysnc-1.1.5a0/LICENSE
+-rw-r--r--   0        0        0     1590 2023-05-24 21:33:54.039764 pysnc-1.1.5a0/README.md
+-rw-r--r--   0        0        0     1058 2023-05-24 21:35:45.113412 pysnc-1.1.5a0/pyproject.toml
+-rw-r--r--   0        0        0      129 2023-05-24 21:33:54.039764 pysnc-1.1.5a0/pysnc/__init__.py
+-rw-r--r--   0        0        0       98 2023-05-24 21:33:54.039764 pysnc-1.1.5a0/pysnc/__version__.py
+-rw-r--r--   0        0        0     9386 2023-05-24 21:33:54.039764 pysnc-1.1.5a0/pysnc/attachment.py
+-rw-r--r--   0        0        0     3757 2023-05-24 21:33:54.039764 pysnc-1.1.5a0/pysnc/auth.py
+-rw-r--r--   0        0        0    15673 2023-05-24 21:33:54.039764 pysnc-1.1.5a0/pysnc/client.py
+-rw-r--r--   0        0        0     1002 2023-05-24 21:33:54.043763 pysnc-1.1.5a0/pysnc/exceptions.py
+-rw-r--r--   0        0        0     3867 2023-05-24 21:33:54.043763 pysnc-1.1.5a0/pysnc/query.py
+-rw-r--r--   0        0        0    38858 2023-05-24 21:33:54.043763 pysnc-1.1.5a0/pysnc/record.py
+-rw-r--r--   0        0        0      846 2023-05-24 21:33:54.043763 pysnc-1.1.5a0/pysnc/utils.py
+-rw-r--r--   0        0        0     2618 1970-01-01 00:00:00.000000 pysnc-1.1.5a0/PKG-INFO
```

### Comparing `pysnc-1.1.4/LICENSE` & `pysnc-1.1.5a0/LICENSE`

 * *Files identical despite different names*

### Comparing `pysnc-1.1.4/README.md` & `pysnc-1.1.5a0/README.md`

 * *Files identical despite different names*

### Comparing `pysnc-1.1.4/pyproject.toml` & `pysnc-1.1.5a0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysnc"
-version = "1.1.4"
+version = "1.1.5a0"
 description = "Python SNC (REST) API"
 authors = ["Matthew Gill <matthew.gill@servicenow.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ServiceNow/PySNC"
 documentation = "https://servicenow.github.io/PySNC/"
 keywords = ["servicenow", "snc"]
```

### Comparing `pysnc-1.1.4/pysnc/attachment.py` & `pysnc-1.1.5a0/pysnc/attachment.py`

 * *Files identical despite different names*

### Comparing `pysnc-1.1.4/pysnc/auth.py` & `pysnc-1.1.5a0/pysnc/auth.py`

 * *Files identical despite different names*

### Comparing `pysnc-1.1.4/pysnc/client.py` & `pysnc-1.1.5a0/pysnc/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,15 +206,15 @@
         req = requests.Request('GET', target_url, params=params)
         return self._send(req)
 
     def put(self, record: GlideRecord) -> requests.Response:
         return self.patch(record)
 
     def patch(self, record: GlideRecord) -> requests.Response:
-        body = record.serialize()
+        body = record.serialize(changes_only=True)
         params = self._set_params()
         target_url = self._target(record.table, record.sys_id)
         req = requests.Request('PATCH', target_url, params=params, json=body)
         return self._send(req)
 
     def post(self, record: GlideRecord) -> requests.Response:
         body = record.serialize()
@@ -355,23 +355,21 @@
         }
         r = self.session.post(self._batch_target(), json=body)
         self._validate_response(r)
         data = r.json()
         try:
             assert str(bid) == data['batch_request_id'], f"How did we get a response id different from {bid}"
 
-            for response in data['serviced_requests']:
+            for response in data['serviced_requests'] + data['unserviced_requests']:
                 response_id = response['id']
                 assert response_id in self.__hooks, f"Somehow has no hook for {response_id}"
                 assert response_id in self.__stored_requests, f"Somehow we did not store request for {response_id}"
                 self.__hooks[response['id']](self._transform_response(self.__stored_requests[response_id], response))
 
-            for response_id in data['unserviced_requests']:
-                assert response_id in self.__hooks, f"Somehow has no hook for {response_id}"
-                self.__hooks[response_id]()  # just call it with no args...
+            return bid
         finally:
             self.__stored_requests = {}
             self.__requests = []
             self.__hooks = {}
 
     def get(self, record: GlideRecord, sys_id: str, hook: Callable) -> None:
         params = self._set_params(record)
@@ -381,15 +379,15 @@
         req = requests.Request('GET', target_url, params=params)
         self._add_request(req, hook)
 
     def put(self, record: GlideRecord, hook: Callable) -> None:
         self.patch(record, hook)
 
     def patch(self, record: GlideRecord, hook: Callable) -> None:
-        body = record.serialize()
+        body = record.serialize(changes_only=True)
         params = self._set_params()
         target_url = self._table_target(record.table, record.sys_id)
         req = requests.Request('PATCH', target_url, params=params, json=body)
         self._add_request(req, hook)
 
     def post(self, record: GlideRecord, hook: Callable):
         body = record.serialize()
```

### Comparing `pysnc-1.1.4/pysnc/exceptions.py` & `pysnc-1.1.5a0/pysnc/exceptions.py`

 * *Files identical despite different names*

### Comparing `pysnc-1.1.4/pysnc/query.py` & `pysnc-1.1.5a0/pysnc/query.py`

 * *Files identical despite different names*

### Comparing `pysnc-1.1.4/pysnc/record.py` & `pysnc-1.1.5a0/pysnc/record.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,18 +11,23 @@
 
 TIMESTAMP_FORMAT = "%Y-%m-%d %H:%M:%S%z"
 
 if TYPE_CHECKING:  # for mypy
     from .client import ServiceNowClient
     from .attachment import Attachment
 
-class GlideElement(object):
+
+class GlideElement(str):
     """
     Object backing the value/display values of a given record entry.
     """
+
+    def __new__(cls, name, value, *args, **kwargs):
+        return super(GlideElement, cls).__new__(cls, value)
+
     def __init__(self, name: str, value=None, display_value=None, parent_record=None):
         self._name = name
         self._value = None
         self._display_value = None
         self._changed = False
         if isinstance(value, dict):
             self._value = value['value']
@@ -131,15 +136,15 @@
 
     def __str__(self):
         #if self._display_value and self._value != self._display_value:
         #    return dict(value=self._value, display_value=self._display_value)
         return str(self.get_value())
 
     def __repr__(self):
-        return f"record.GlideElement(value={self._value!r}, name={self._name!r}, display_value={self._display_value!r}, changed={self._changed!r})"
+        return f"GlideElement({self._value!r})"
 
     def __bool__(self):
         # help with the truthiness of true/false fields
         # theoretically could have a false case if we're a string with the value false since we dont know our types
         if self.get_value() == 'false':
             return False
         return bool(self.get_value())
@@ -155,14 +160,17 @@
 
     def __ne__(self, other):
         return self.__magic('__ne__', other)
 
     def __len__(self):
         return self.__magic('__len__')
 
+    def __length_hint__(self):
+        return self.__magic('__length_hint__')
+
     def __iter__(self):
         # unfortunately i don't think we'll ever be smart enough to auto-support List columns
         return self.__magic('__iter__')
 
     def __next__(self):
         return self.__magic('__next__')
 
@@ -182,14 +190,32 @@
 
     def __le__(self, other):
         return self.__magic('__le__', other)
 
     def __ge__(self, other):
         return self.__magic('__ge__', other)
 
+    def __contains__(self, other):
+        return self.__magic('__contains__', other)
+
+    def __getitem__(self, index):
+        return self.__magic('__getitem__', index)
+
+    def __hash__(self):
+        return self.__magic('__hash__')
+
+    def __int__(self):
+        return int(self.get_value())
+
+    def __float__(self):
+        return float(self.get_value())
+
+    def __complex__(self):
+        return complex(self.get_value())
+
     def __getattr__(self, item):
         if item in GlideElement.__class__.__dict__:
             return self.__getattribute__(item)
 
         if self._parent_record:
             if tv := self._parent_record.get_element(f"{self._name}.{item}"):
                 return tv
@@ -455,29 +481,42 @@
 
     def rewind(self):
         """
         Rewinds the record so it may be iterated upon again. Not required to be called if iterating in the pythonic method.
         """
         self.__current = -1
 
+    def changes(self) -> bool:
+        """
+        Determines weather any of the fields in the record have changed
+        """
+        obj = self._current()
+        if obj:
+            has_changed = False
+            for key, value in obj.items():
+                has_changed ^= value.changes()
+            return has_changed
+        return False
+
+
     def query(self, query=None):
         """
         Query the table - executes a GET
 
         :raise:
             :AuthenticationException: If we do not have rights
             :RequestException: If the transaction is canceled due to execution time
         """
         stored = self.__query
         if query:
             assert isinstance(query, Query), 'cannot query with a non query object'
             self.__query = query
         try:
             short_len = len('&'.join([ f"{x}={y}" for (x,y) in self._parameters().items() ]))
-            if short_len > 20000:  # just the approx limit, but a few thousand below (i hope/think)
+            if short_len > 10000:  # just the approx limit, but a few thousand below (i hope/think)
 
                 def on_resp(r):
                     nonlocal response
                     response = r
                 self._client.batch_api.list(self, on_resp)
                 self._client.batch_api.execute()
             else:
@@ -615,26 +654,27 @@
                 allRecordsWereDeleted = False
 
         for e in self:
             self._client.batch_api.delete(e, handle)
         self._client.batch_api.execute()
         return allRecordsWereDeleted
 
-    def update_multiple(self) -> bool:
+    def update_multiple(self, custom_handler=None) -> bool:
         """
         Updates multiple records at once
         """
         updated = True
         def handle(response):
             nonlocal updated
             if response.status_code != 200:
                 updated = False
 
         for e in self:
-            self._client.batch_api.put(e, handle)
+            if e.changes():
+                self._client.batch_api.put(e, custom_handler if custom_handler else handle)
 
         self._client.batch_api.execute()
         return updated
 
     def _get_value(self, item, key='value'):
         obj = self._current()
         if obj is None:
```

### Comparing `pysnc-1.1.4/pysnc/utils.py` & `pysnc-1.1.5a0/pysnc/utils.py`

 * *Files identical despite different names*

### Comparing `pysnc-1.1.4/PKG-INFO` & `pysnc-1.1.5a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysnc
-Version: 1.1.4
+Version: 1.1.5a0
 Summary: Python SNC (REST) API
 Home-page: https://github.com/ServiceNow/PySNC
 License: MIT
 Keywords: servicenow,snc
 Author: Matthew Gill
 Author-email: matthew.gill@servicenow.com
 Requires-Python: >=3.8,<4.0
@@ -13,15 +13,14 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Provides-Extra: oauth
 Requires-Dist: requests (>=2.8.1)
 Requires-Dist: requests-oauthlib (>=1.2.0) ; extra == "oauth"
 Project-URL: Documentation, https://servicenow.github.io/PySNC/
 Project-URL: Repository, https://github.com/ServiceNow/PySNC
 Description-Content-Type: text/markdown
```

