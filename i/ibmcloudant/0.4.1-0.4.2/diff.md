# Comparing `tmp/ibmcloudant-0.4.1.tar.gz` & `tmp/ibmcloudant-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibmcloudant-0.4.1.tar", last modified: Tue Apr 25 09:05:09 2023, max compression
+gzip compressed data, was "ibmcloudant-0.4.2.tar", last modified: Wed May 24 10:03:03 2023, max compression
```

## Comparing `ibmcloudant-0.4.1.tar` & `ibmcloudant-0.4.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-25 09:05:09.503718 ibmcloudant-0.4.1/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11357 2023-04-25 08:48:06.000000 ibmcloudant-0.4.1/LICENSE
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)       70 2023-04-25 08:48:06.000000 ibmcloudant-0.4.1/MANIFEST.in
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    27202 2023-04-25 09:05:09.503718 ibmcloudant-0.4.1/PKG-INFO
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    26200 2023-04-25 08:51:15.000000 ibmcloudant-0.4.1/README.md
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-25 09:05:09.503718 ibmcloudant-0.4.1/ibmcloudant/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1596 2023-04-25 08:48:06.000000 ibmcloudant-0.4.1/ibmcloudant/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     6630 2023-04-25 08:48:06.000000 ibmcloudant-0.4.1/ibmcloudant/cloudant_base_service.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)   745079 2023-04-25 08:48:06.000000 ibmcloudant-0.4.1/ibmcloudant/cloudant_v1.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1811 2023-04-25 08:48:06.000000 ibmcloudant-0.4.1/ibmcloudant/common.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3396 2023-04-25 08:48:06.000000 ibmcloudant-0.4.1/ibmcloudant/couchdb_session_authenticator.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1543 2023-04-25 08:48:06.000000 ibmcloudant-0.4.1/ibmcloudant/couchdb_session_get_authenticator_patch.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3609 2023-04-25 08:48:06.000000 ibmcloudant-0.4.1/ibmcloudant/couchdb_session_token_manager.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      655 2023-04-25 08:51:15.000000 ibmcloudant-0.4.1/ibmcloudant/version.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-25 09:05:09.503718 ibmcloudant-0.4.1/ibmcloudant.egg-info/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    27202 2023-04-25 09:05:09.000000 ibmcloudant-0.4.1/ibmcloudant.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      558 2023-04-25 09:05:09.000000 ibmcloudant-0.4.1/ibmcloudant.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2023-04-25 09:05:09.000000 ibmcloudant-0.4.1/ibmcloudant.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)       97 2023-04-25 09:05:09.000000 ibmcloudant-0.4.1/ibmcloudant.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)       12 2023-04-25 09:05:09.000000 ibmcloudant-0.4.1/ibmcloudant.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2023-04-25 08:48:29.000000 ibmcloudant-0.4.1/ibmcloudant.egg-info/zip-safe
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      232 2023-04-25 08:48:06.000000 ibmcloudant-0.4.1/requirements-dev.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      135 2023-04-25 08:48:06.000000 ibmcloudant-0.4.1/requirements.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)       38 2023-04-25 09:05:09.503718 ibmcloudant-0.4.1/setup.cfg
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3435 2023-04-25 08:51:15.000000 ibmcloudant-0.4.1/setup.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-24 10:03:03.466310 ibmcloudant-0.4.2/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11357 2023-05-24 09:52:04.000000 ibmcloudant-0.4.2/LICENSE
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       70 2023-05-24 09:52:04.000000 ibmcloudant-0.4.2/MANIFEST.in
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    27205 2023-05-24 10:03:03.466310 ibmcloudant-0.4.2/PKG-INFO
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    26203 2023-05-24 09:54:50.000000 ibmcloudant-0.4.2/README.md
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-24 10:03:03.466310 ibmcloudant-0.4.2/ibmcloudant/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1596 2023-05-24 09:52:04.000000 ibmcloudant-0.4.2/ibmcloudant/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     6630 2023-05-24 09:52:04.000000 ibmcloudant-0.4.2/ibmcloudant/cloudant_base_service.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)   746253 2023-05-24 09:52:04.000000 ibmcloudant-0.4.2/ibmcloudant/cloudant_v1.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1811 2023-05-24 09:52:04.000000 ibmcloudant-0.4.2/ibmcloudant/common.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3396 2023-05-24 09:52:04.000000 ibmcloudant-0.4.2/ibmcloudant/couchdb_session_authenticator.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1543 2023-05-24 09:52:04.000000 ibmcloudant-0.4.2/ibmcloudant/couchdb_session_get_authenticator_patch.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3609 2023-05-24 09:52:04.000000 ibmcloudant-0.4.2/ibmcloudant/couchdb_session_token_manager.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      655 2023-05-24 09:54:50.000000 ibmcloudant-0.4.2/ibmcloudant/version.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-24 10:03:03.466310 ibmcloudant-0.4.2/ibmcloudant.egg-info/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    27205 2023-05-24 10:03:03.000000 ibmcloudant-0.4.2/ibmcloudant.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      558 2023-05-24 10:03:03.000000 ibmcloudant-0.4.2/ibmcloudant.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2023-05-24 10:03:03.000000 ibmcloudant-0.4.2/ibmcloudant.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       97 2023-05-24 10:03:03.000000 ibmcloudant-0.4.2/ibmcloudant.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       12 2023-05-24 10:03:03.000000 ibmcloudant-0.4.2/ibmcloudant.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2023-05-24 09:52:24.000000 ibmcloudant-0.4.2/ibmcloudant.egg-info/zip-safe
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      231 2023-05-24 09:52:04.000000 ibmcloudant-0.4.2/requirements-dev.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      135 2023-05-24 09:52:04.000000 ibmcloudant-0.4.2/requirements.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       38 2023-05-24 10:03:03.466310 ibmcloudant-0.4.2/setup.cfg
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3435 2023-05-24 09:54:50.000000 ibmcloudant-0.4.2/setup.py
```

### Comparing `ibmcloudant-0.4.1/LICENSE` & `ibmcloudant-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ibmcloudant-0.4.1/PKG-INFO` & `ibmcloudant-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibmcloudant
-Version: 0.4.1
+Version: 0.4.2
 Summary: Python client library for IBM Cloudant
 Home-page: https://github.com/IBM/cloudant-python-sdk
 Author: IBM
 Author-email: cldtsdks@us.ibm.com
 License: Apache 2.0
 Keywords: ibmcloudant
 Classifier: Programming Language :: Python
@@ -23,15 +23,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Build Status](https://github.com/IBM/cloudant-python-sdk/actions/workflows/test.yml/badge.svg?branch=main&event=push)](https://github.com/IBM/cloudant-python-sdk/actions/workflows/test.yml)
 [![Release](https://img.shields.io/github/v/release/IBM/cloudant-python-sdk?include_prereleases&sort=semver)](https://github.com/IBM/cloudant-python-sdk/releases/latest)
 [![Docs](https://img.shields.io/static/v1?label=Pydoc&message=latest&color=blue)](https://ibm.github.io/cloudant-python-sdk/)
 
-# IBM Cloudant Python SDK Version 0.4.1
+# IBM Cloudant Python SDK Version 0.4.2
 
 IBM Cloudant Python SDK is a client library that interacts with the
 [IBM Cloudant APIs](https://cloud.ibm.com/apidocs/cloudant?code=python).
 
 Disclaimer: This library is still a 0.x release. We do consider this
 library production-ready and capable, but there are still some
 limitations we’re working to resolve, and refinements we want to
@@ -123,21 +123,21 @@
 - Python 3.7 or above.
 
 ## Installation
 
 To install, use `pip` or `easy_install`:
 
 ```bash
-pip install --upgrade "ibmcloudant>=0.4.1"
+pip install --upgrade "ibmcloudant>=0.4.2"
 ```
 
 or
 
 ```bash
-easy_install --upgrade "ibmcloudant>=0.4.1"
+easy_install --upgrade "ibmcloudant>=0.4.2"
 ```
 
 ## Authentication
 
 [service-credentials]: https://cloud.ibm.com/docs/Cloudant?topic=Cloudant-locating-your-service-credentials
 [cloud-IAM-mgmt]: https://cloud.ibm.com/docs/Cloudant?topic=Cloudant-managing-access-for-cloudant#introduction-iam-ai
 [couch-cookie-auth]: https://docs.couchdb.org/en/stable/api/server/authn.html#cookie-authentication
@@ -245,27 +245,27 @@
 The [request timeout](https://github.com/IBM/ibm-cloud-sdk-common/blob/main/README.md) section contains details on how to change the value.
 
 **Note:** System settings may take precedence over configured timeout values.
 
 ### Code examples
 
 The following code examples
-[authenticate with the environment variables](#authenticate-with-environment-variables).
+[authenticate with the environment variables](#authentication-with-environment-variables).
 
 #### 1. Create a database and add a document
 
 **Note:** This example code assumes that `orders` database does not exist in your account.
 
 This example code creates `orders` database and adds a new document "example"
 into it. To connect, you must set your environment variables with
 the *service url*, *authentication type* and *authentication credentials*
 of your Cloudant service.
 
 Cloudant environment variable naming starts with a *service name* prefix that identifies your service.
-By default this is `CLOUDANT`, see the settings in the
+By default, this is `CLOUDANT`, see the settings in the
 [authentication with environment variables section](#authentication-with-environment-variables).
 
 If you would like to rename your Cloudant service from `CLOUDANT`,
 you must use your defined service name as the prefix for all Cloudant related environment variables.
 
 Once the environment variables are set, you can try out the code examples.
```

### Comparing `ibmcloudant-0.4.1/README.md` & `ibmcloudant-0.4.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [![Build Status](https://github.com/IBM/cloudant-python-sdk/actions/workflows/test.yml/badge.svg?branch=main&event=push)](https://github.com/IBM/cloudant-python-sdk/actions/workflows/test.yml)
 [![Release](https://img.shields.io/github/v/release/IBM/cloudant-python-sdk?include_prereleases&sort=semver)](https://github.com/IBM/cloudant-python-sdk/releases/latest)
 [![Docs](https://img.shields.io/static/v1?label=Pydoc&message=latest&color=blue)](https://ibm.github.io/cloudant-python-sdk/)
 
-# IBM Cloudant Python SDK Version 0.4.1
+# IBM Cloudant Python SDK Version 0.4.2
 
 IBM Cloudant Python SDK is a client library that interacts with the
 [IBM Cloudant APIs](https://cloud.ibm.com/apidocs/cloudant?code=python).
 
 Disclaimer: This library is still a 0.x release. We do consider this
 library production-ready and capable, but there are still some
 limitations we’re working to resolve, and refinements we want to
@@ -98,21 +98,21 @@
 - Python 3.7 or above.
 
 ## Installation
 
 To install, use `pip` or `easy_install`:
 
 ```bash
-pip install --upgrade "ibmcloudant>=0.4.1"
+pip install --upgrade "ibmcloudant>=0.4.2"
 ```
 
 or
 
 ```bash
-easy_install --upgrade "ibmcloudant>=0.4.1"
+easy_install --upgrade "ibmcloudant>=0.4.2"
 ```
 
 ## Authentication
 
 [service-credentials]: https://cloud.ibm.com/docs/Cloudant?topic=Cloudant-locating-your-service-credentials
 [cloud-IAM-mgmt]: https://cloud.ibm.com/docs/Cloudant?topic=Cloudant-managing-access-for-cloudant#introduction-iam-ai
 [couch-cookie-auth]: https://docs.couchdb.org/en/stable/api/server/authn.html#cookie-authentication
@@ -220,27 +220,27 @@
 The [request timeout](https://github.com/IBM/ibm-cloud-sdk-common/blob/main/README.md) section contains details on how to change the value.
 
 **Note:** System settings may take precedence over configured timeout values.
 
 ### Code examples
 
 The following code examples
-[authenticate with the environment variables](#authenticate-with-environment-variables).
+[authenticate with the environment variables](#authentication-with-environment-variables).
 
 #### 1. Create a database and add a document
 
 **Note:** This example code assumes that `orders` database does not exist in your account.
 
 This example code creates `orders` database and adds a new document "example"
 into it. To connect, you must set your environment variables with
 the *service url*, *authentication type* and *authentication credentials*
 of your Cloudant service.
 
 Cloudant environment variable naming starts with a *service name* prefix that identifies your service.
-By default this is `CLOUDANT`, see the settings in the
+By default, this is `CLOUDANT`, see the settings in the
 [authentication with environment variables section](#authentication-with-environment-variables).
 
 If you would like to rename your Cloudant service from `CLOUDANT`,
 you must use your defined service name as the prefix for all Cloudant related environment variables.
 
 Once the environment variables are set, you can try out the code examples.
```

### Comparing `ibmcloudant-0.4.1/ibmcloudant/__init__.py` & `ibmcloudant-0.4.2/ibmcloudant/__init__.py`

 * *Files identical despite different names*

### Comparing `ibmcloudant-0.4.1/ibmcloudant/cloudant_base_service.py` & `ibmcloudant-0.4.2/ibmcloudant/cloudant_base_service.py`

 * *Files identical despite different names*

### Comparing `ibmcloudant-0.4.1/ibmcloudant/cloudant_v1.py` & `ibmcloudant-0.4.2/ibmcloudant/cloudant_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -12652,20 +12652,23 @@
         return not self == other
 
 
 class ExplainResult:
     """
     Schema for information about the index used for a find query.
 
-    :attr str dbname: dbname.
-    :attr List[str] fields: fields.
+    :attr bool covered: When `true`, the query is answered using the index only and
+          no documents are fetched.
+    :attr str dbname: Name of database.
+    :attr List[str] fields: Fields to be returned by the query.
     :attr IndexInformation index: Schema for information about an index.
-    :attr int limit: limit.
-    :attr dict opts: opts.
-    :attr ExplainResultRange range: (optional) range.
+    :attr int limit: The used maximum number of results returned.
+    :attr dict opts: Query options used.
+    :attr ExplainResultRange range: (optional) Range parameters passed to the
+          underlying view.
     :attr dict selector: JSON object describing criteria used to select documents.
           The selector specifies fields in the document, and provides an expression to
           evaluate with the field content or other data.
           The selector object must:
             * Be structured as valid JSON.
             * Contain a valid query expression.
           Using a selector is significantly more efficient than using a JavaScript filter
@@ -12687,37 +12690,40 @@
           the specified field contains a value that is equal to the supplied argument.
           * Only equality operators such as `$eq`, `$gt`, `$gte`, `$lt`, and `$lte` (but
           not `$ne`) can be used as the basis of a query. You should include at least one
           of these in a selector.
           For further reference see
           [selector
           syntax](https://cloud.ibm.com/docs/Cloudant?topic=Cloudant-query#selector-syntax).
-    :attr int skip: skip.
+    :attr int skip: Skip parameter used.
     """
 
     def __init__(
         self,
+        covered: bool,
         dbname: str,
         fields: List[str],
         index: 'IndexInformation',
         limit: int,
         opts: dict,
         selector: dict,
         skip: int,
         *,
         range: 'ExplainResultRange' = None,
     ) -> None:
         """
         Initialize a ExplainResult object.
 
-        :param str dbname: dbname.
-        :param List[str] fields: fields.
+        :param bool covered: When `true`, the query is answered using the index
+               only and no documents are fetched.
+        :param str dbname: Name of database.
+        :param List[str] fields: Fields to be returned by the query.
         :param IndexInformation index: Schema for information about an index.
-        :param int limit: limit.
-        :param dict opts: opts.
+        :param int limit: The used maximum number of results returned.
+        :param dict opts: Query options used.
         :param dict selector: JSON object describing criteria used to select
                documents. The selector specifies fields in the document, and provides an
                expression to evaluate with the field content or other data.
                The selector object must:
                  * Be structured as valid JSON.
                  * Contain a valid query expression.
                Using a selector is significantly more efficient than using a JavaScript
@@ -12741,30 +12747,36 @@
                supplied argument.
                * Only equality operators such as `$eq`, `$gt`, `$gte`, `$lt`, and `$lte`
                (but not `$ne`) can be used as the basis of a query. You should include at
                least one of these in a selector.
                For further reference see
                [selector
                syntax](https://cloud.ibm.com/docs/Cloudant?topic=Cloudant-query#selector-syntax).
-        :param int skip: skip.
-        :param ExplainResultRange range: (optional) range.
+        :param int skip: Skip parameter used.
+        :param ExplainResultRange range: (optional) Range parameters passed to the
+               underlying view.
         """
+        self.covered = covered
         self.dbname = dbname
         self.fields = fields
         self.index = index
         self.limit = limit
         self.opts = opts
         self.range = range
         self.selector = selector
         self.skip = skip
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'ExplainResult':
         """Initialize a ExplainResult object from a json dictionary."""
         args = {}
+        if 'covered' in _dict:
+            args['covered'] = _dict.get('covered')
+        else:
+            raise ValueError('Required property \'covered\' not present in ExplainResult JSON')
         if 'dbname' in _dict:
             args['dbname'] = _dict.get('dbname')
         else:
             raise ValueError('Required property \'dbname\' not present in ExplainResult JSON')
         if 'fields' in _dict:
             args['fields'] = _dict.get('fields')
         else:
@@ -12797,14 +12809,16 @@
     def _from_dict(cls, _dict):
         """Initialize a ExplainResult object from a json dictionary."""
         return cls.from_dict(_dict)
 
     def to_dict(self) -> Dict:
         """Return a json dictionary representing this model."""
         _dict = {}
+        if hasattr(self, 'covered') and self.covered is not None:
+            _dict['covered'] = self.covered
         if hasattr(self, 'dbname') and self.dbname is not None:
             _dict['dbname'] = self.dbname
         if hasattr(self, 'fields') and self.fields is not None:
             _dict['fields'] = self.fields
         if hasattr(self, 'index') and self.index is not None:
             if isinstance(self.index, dict):
                 _dict['index'] = self.index
@@ -12842,31 +12856,35 @@
     def __ne__(self, other: 'ExplainResult') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
 
 class ExplainResultRange:
     """
-    range.
+    Range parameters passed to the underlying view.
 
-    :attr List[object] end_key: (optional) end_key.
-    :attr List[object] start_key: (optional) start_key.
+    :attr List[object] end_key: (optional) End key parameter passed to the
+          underlying view.
+    :attr List[object] start_key: (optional) Start key parameter passed to the
+          underlying view.
     """
 
     def __init__(
         self,
         *,
         end_key: List[object] = None,
         start_key: List[object] = None,
     ) -> None:
         """
         Initialize a ExplainResultRange object.
 
-        :param List[object] end_key: (optional) end_key.
-        :param List[object] start_key: (optional) start_key.
+        :param List[object] end_key: (optional) End key parameter passed to the
+               underlying view.
+        :param List[object] start_key: (optional) Start key parameter passed to the
+               underlying view.
         """
         self.end_key = end_key
         self.start_key = start_key
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'ExplainResultRange':
         """Initialize a ExplainResultRange object from a json dictionary."""
```

### Comparing `ibmcloudant-0.4.1/ibmcloudant/common.py` & `ibmcloudant-0.4.2/ibmcloudant/common.py`

 * *Files identical despite different names*

### Comparing `ibmcloudant-0.4.1/ibmcloudant/couchdb_session_authenticator.py` & `ibmcloudant-0.4.2/ibmcloudant/couchdb_session_authenticator.py`

 * *Files identical despite different names*

### Comparing `ibmcloudant-0.4.1/ibmcloudant/couchdb_session_get_authenticator_patch.py` & `ibmcloudant-0.4.2/ibmcloudant/couchdb_session_get_authenticator_patch.py`

 * *Files identical despite different names*

### Comparing `ibmcloudant-0.4.1/ibmcloudant/couchdb_session_token_manager.py` & `ibmcloudant-0.4.2/ibmcloudant/couchdb_session_token_manager.py`

 * *Files identical despite different names*

### Comparing `ibmcloudant-0.4.1/ibmcloudant/version.py` & `ibmcloudant-0.4.2/ibmcloudant/version.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Version of ibmcloudant
 """
-__version__ = '0.4.1'
+__version__ = '0.4.2'
```

### Comparing `ibmcloudant-0.4.1/ibmcloudant.egg-info/PKG-INFO` & `ibmcloudant-0.4.2/ibmcloudant.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibmcloudant
-Version: 0.4.1
+Version: 0.4.2
 Summary: Python client library for IBM Cloudant
 Home-page: https://github.com/IBM/cloudant-python-sdk
 Author: IBM
 Author-email: cldtsdks@us.ibm.com
 License: Apache 2.0
 Keywords: ibmcloudant
 Classifier: Programming Language :: Python
@@ -23,15 +23,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Build Status](https://github.com/IBM/cloudant-python-sdk/actions/workflows/test.yml/badge.svg?branch=main&event=push)](https://github.com/IBM/cloudant-python-sdk/actions/workflows/test.yml)
 [![Release](https://img.shields.io/github/v/release/IBM/cloudant-python-sdk?include_prereleases&sort=semver)](https://github.com/IBM/cloudant-python-sdk/releases/latest)
 [![Docs](https://img.shields.io/static/v1?label=Pydoc&message=latest&color=blue)](https://ibm.github.io/cloudant-python-sdk/)
 
-# IBM Cloudant Python SDK Version 0.4.1
+# IBM Cloudant Python SDK Version 0.4.2
 
 IBM Cloudant Python SDK is a client library that interacts with the
 [IBM Cloudant APIs](https://cloud.ibm.com/apidocs/cloudant?code=python).
 
 Disclaimer: This library is still a 0.x release. We do consider this
 library production-ready and capable, but there are still some
 limitations we’re working to resolve, and refinements we want to
@@ -123,21 +123,21 @@
 - Python 3.7 or above.
 
 ## Installation
 
 To install, use `pip` or `easy_install`:
 
 ```bash
-pip install --upgrade "ibmcloudant>=0.4.1"
+pip install --upgrade "ibmcloudant>=0.4.2"
 ```
 
 or
 
 ```bash
-easy_install --upgrade "ibmcloudant>=0.4.1"
+easy_install --upgrade "ibmcloudant>=0.4.2"
 ```
 
 ## Authentication
 
 [service-credentials]: https://cloud.ibm.com/docs/Cloudant?topic=Cloudant-locating-your-service-credentials
 [cloud-IAM-mgmt]: https://cloud.ibm.com/docs/Cloudant?topic=Cloudant-managing-access-for-cloudant#introduction-iam-ai
 [couch-cookie-auth]: https://docs.couchdb.org/en/stable/api/server/authn.html#cookie-authentication
@@ -245,27 +245,27 @@
 The [request timeout](https://github.com/IBM/ibm-cloud-sdk-common/blob/main/README.md) section contains details on how to change the value.
 
 **Note:** System settings may take precedence over configured timeout values.
 
 ### Code examples
 
 The following code examples
-[authenticate with the environment variables](#authenticate-with-environment-variables).
+[authenticate with the environment variables](#authentication-with-environment-variables).
 
 #### 1. Create a database and add a document
 
 **Note:** This example code assumes that `orders` database does not exist in your account.
 
 This example code creates `orders` database and adds a new document "example"
 into it. To connect, you must set your environment variables with
 the *service url*, *authentication type* and *authentication credentials*
 of your Cloudant service.
 
 Cloudant environment variable naming starts with a *service name* prefix that identifies your service.
-By default this is `CLOUDANT`, see the settings in the
+By default, this is `CLOUDANT`, see the settings in the
 [authentication with environment variables section](#authentication-with-environment-variables).
 
 If you would like to rename your Cloudant service from `CLOUDANT`,
 you must use your defined service name as the prefix for all Cloudant related environment variables.
 
 Once the environment variables are set, you can try out the code examples.
```

### Comparing `ibmcloudant-0.4.1/ibmcloudant.egg-info/SOURCES.txt` & `ibmcloudant-0.4.2/ibmcloudant.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ibmcloudant-0.4.1/setup.py` & `ibmcloudant-0.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 from setuptools import setup
 from setuptools.command.test import test as TestCommand
 import os
 import sys
 import pkg_resources
 
-__version__ = '0.4.1'
+__version__ = '0.4.2'
 PACKAGE_NAME = 'ibmcloudant'
 PACKAGE_DESC = 'Python client library for IBM Cloudant'
 
 with open('requirements.txt') as f:
     install_requires = [str(req) for req in pkg_resources.parse_requirements(f)]
 with open('requirements-dev.txt') as f:
     tests_require = [str(req) for req in pkg_resources.parse_requirements(f)]
```

