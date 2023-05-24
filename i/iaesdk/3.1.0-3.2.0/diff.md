# Comparing `tmp/iaesdk-3.1.0.tar.gz` & `tmp/iaesdk-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/iaesdk-3.1.0.tar", last modified: Thu Mar 23 09:27:24 2023, max compression
+gzip compressed data, was "dist/iaesdk-3.2.0.tar", last modified: Wed May 24 07:48:51 2023, max compression
```

## Comparing `iaesdk-3.1.0.tar` & `iaesdk-3.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-03-23 09:27:24.000000 iaesdk-3.1.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11357 2023-03-23 09:26:03.000000 iaesdk-3.1.0/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)       69 2023-03-23 09:26:03.000000 iaesdk-3.1.0/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     4261 2023-03-23 09:27:24.000000 iaesdk-3.1.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     3293 2023-03-23 09:26:03.000000 iaesdk-3.1.0/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-03-23 09:27:24.000000 iaesdk-3.1.0/iaesdk/
--rw-rw-r--   0 travis    (2000) travis    (2000)      966 2023-03-23 09:26:03.000000 iaesdk-3.1.0/iaesdk/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1570 2023-03-23 09:26:03.000000 iaesdk-3.1.0/iaesdk/common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   100693 2023-03-23 09:26:03.000000 iaesdk-3.1.0/iaesdk/ibm_analytics_engine_api_v2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   133056 2023-03-23 09:26:03.000000 iaesdk-3.1.0/iaesdk/ibm_analytics_engine_api_v3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       48 2023-03-23 09:26:03.000000 iaesdk-3.1.0/iaesdk/version.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-03-23 09:27:24.000000 iaesdk-3.1.0/iaesdk.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4261 2023-03-23 09:27:24.000000 iaesdk-3.1.0/iaesdk.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      395 2023-03-23 09:27:24.000000 iaesdk-3.1.0/iaesdk.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-03-23 09:27:24.000000 iaesdk-3.1.0/iaesdk.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      111 2023-03-23 09:27:24.000000 iaesdk-3.1.0/iaesdk.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        7 2023-03-23 09:27:24.000000 iaesdk-3.1.0/iaesdk.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-03-23 09:26:34.000000 iaesdk-3.1.0/iaesdk.egg-info/zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)       64 2023-03-23 09:26:03.000000 iaesdk-3.1.0/pyproject.toml
--rw-rw-r--   0 travis    (2000) travis    (2000)      166 2023-03-23 09:26:03.000000 iaesdk-3.1.0/requirements-dev.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      111 2023-03-23 09:26:03.000000 iaesdk-3.1.0/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2023-03-23 09:27:24.000000 iaesdk-3.1.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     2632 2023-03-23 09:26:03.000000 iaesdk-3.1.0/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-24 07:48:51.000000 iaesdk-3.2.0/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11357 2023-05-24 07:47:04.000000 iaesdk-3.2.0/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)       69 2023-05-24 07:47:04.000000 iaesdk-3.2.0/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4261 2023-05-24 07:48:51.000000 iaesdk-3.2.0/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3293 2023-05-24 07:47:04.000000 iaesdk-3.2.0/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-24 07:48:51.000000 iaesdk-3.2.0/iaesdk/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      966 2023-05-24 07:47:04.000000 iaesdk-3.2.0/iaesdk/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1570 2023-05-24 07:47:04.000000 iaesdk-3.2.0/iaesdk/common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   100693 2023-05-24 07:47:04.000000 iaesdk-3.2.0/iaesdk/ibm_analytics_engine_api_v2.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   140285 2023-05-24 07:47:04.000000 iaesdk-3.2.0/iaesdk/ibm_analytics_engine_api_v3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       48 2023-05-24 07:47:04.000000 iaesdk-3.2.0/iaesdk/version.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-24 07:48:51.000000 iaesdk-3.2.0/iaesdk.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4261 2023-05-24 07:48:50.000000 iaesdk-3.2.0/iaesdk.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      395 2023-05-24 07:48:50.000000 iaesdk-3.2.0/iaesdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-05-24 07:48:50.000000 iaesdk-3.2.0/iaesdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      111 2023-05-24 07:48:50.000000 iaesdk-3.2.0/iaesdk.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        7 2023-05-24 07:48:50.000000 iaesdk-3.2.0/iaesdk.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-05-24 07:47:33.000000 iaesdk-3.2.0/iaesdk.egg-info/zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)       64 2023-05-24 07:47:04.000000 iaesdk-3.2.0/pyproject.toml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      166 2023-05-24 07:47:04.000000 iaesdk-3.2.0/requirements-dev.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      111 2023-05-24 07:47:04.000000 iaesdk-3.2.0/requirements.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2023-05-24 07:48:51.000000 iaesdk-3.2.0/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2632 2023-05-24 07:47:04.000000 iaesdk-3.2.0/setup.py
```

### Comparing `iaesdk-3.1.0/LICENSE` & `iaesdk-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iaesdk-3.1.0/PKG-INFO` & `iaesdk-3.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iaesdk
-Version: 3.1.0
+Version: 3.2.0
 Summary: Python client library for IBM Cloud Analytics Engine Services
 Home-page: https://github.com/IBM/ibm-iae-python-sdk
 Author: IBM
 Author-email: surya.penumatcha@ibm.com
 License: Apache 2.0
 Keywords: iaesdk
 Classifier: Programming Language :: Python
@@ -20,15 +20,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Build Status](https://api.travis-ci.com/IBM/ibm-iae-python-sdk.svg?branch=master)](https://app.travis-ci.com/IBM/ibm-iae-python-sdk)
 [![semantic-release](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/semantic-release/semantic-release)
-# IBM Cloud Analytics Engine Python SDK Version 3.1.0
+# IBM Cloud Analytics Engine Python SDK Version 3.2.0
 
 Python client library to interact with various [iaesdk Service APIs](https://cloud.ibm.com/apidocs/ibm-analytics-engine).
 
 ## Table of Contents
 
 - [Overview](#overview)
 - [Prerequisites](#prerequisites)
@@ -67,21 +67,21 @@
 * Python 3.7 or above.
 
 ## Installation
 
 To install, use `pip` or `easy_install`:
 
 ```bash
-pip install --upgrade "iaesdk>=3.1.0"
+pip install --upgrade "iaesdk>=3.2.0"
 ```
 
 or
 
 ```bash
-easy_install --upgrade "iaesdk>=3.1.0"
+easy_install --upgrade "iaesdk>=3.2.0"
 ```
 
 ## Using the SDK
 For general SDK usage information, please see [this link](https://github.com/IBM/ibm-cloud-sdk-common/blob/master/README.md)
 
 In [setting client options programatically](https://github.com/IBM/ibm-cloud-sdk-common/blob/master/README.md#setting-client-options-programmatically) to instantiate the class, provide the following two values:
 1. [IAM API Key](https://cloud.ibm.com/docs/iam?topic=iam-userapikey#create_user_key)
```

### Comparing `iaesdk-3.1.0/README.md` & `iaesdk-3.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [![Build Status](https://api.travis-ci.com/IBM/ibm-iae-python-sdk.svg?branch=master)](https://app.travis-ci.com/IBM/ibm-iae-python-sdk)
 [![semantic-release](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/semantic-release/semantic-release)
-# IBM Cloud Analytics Engine Python SDK Version 3.1.0
+# IBM Cloud Analytics Engine Python SDK Version 3.2.0
 
 Python client library to interact with various [iaesdk Service APIs](https://cloud.ibm.com/apidocs/ibm-analytics-engine).
 
 ## Table of Contents
 
 - [Overview](#overview)
 - [Prerequisites](#prerequisites)
@@ -43,21 +43,21 @@
 * Python 3.7 or above.
 
 ## Installation
 
 To install, use `pip` or `easy_install`:
 
 ```bash
-pip install --upgrade "iaesdk>=3.1.0"
+pip install --upgrade "iaesdk>=3.2.0"
 ```
 
 or
 
 ```bash
-easy_install --upgrade "iaesdk>=3.1.0"
+easy_install --upgrade "iaesdk>=3.2.0"
 ```
 
 ## Using the SDK
 For general SDK usage information, please see [this link](https://github.com/IBM/ibm-cloud-sdk-common/blob/master/README.md)
 
 In [setting client options programatically](https://github.com/IBM/ibm-cloud-sdk-common/blob/master/README.md#setting-client-options-programmatically) to instantiate the class, provide the following two values:
 1. [IAM API Key](https://cloud.ibm.com/docs/iam?topic=iam-userapikey#create_user_key)
```

### Comparing `iaesdk-3.1.0/iaesdk/__init__.py` & `iaesdk-3.2.0/iaesdk/__init__.py`

 * *Files identical despite different names*

### Comparing `iaesdk-3.1.0/iaesdk/common.py` & `iaesdk-3.2.0/iaesdk/common.py`

 * *Files identical despite different names*

### Comparing `iaesdk-3.1.0/iaesdk/ibm_analytics_engine_api_v2.py` & `iaesdk-3.2.0/iaesdk/ibm_analytics_engine_api_v2.py`

 * *Files identical despite different names*

### Comparing `iaesdk-3.1.0/iaesdk/ibm_analytics_engine_api_v3.py` & `iaesdk-3.2.0/iaesdk/ibm_analytics_engine_api_v3.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,44 +27,39 @@
 from typing import Dict, List
 import json
 import logging
 
 from ibm_cloud_sdk_core import BaseService, DetailedResponse
 from ibm_cloud_sdk_core.authenticators.authenticator import Authenticator
 from ibm_cloud_sdk_core.get_authenticator import get_authenticator_from_environment
-from ibm_cloud_sdk_core.utils import (
-    convert_list,
-    convert_model,
-    datetime_to_string,
-    string_to_datetime,
-)
+from ibm_cloud_sdk_core.utils import convert_list, convert_model, datetime_to_string, string_to_datetime
 
 from .common import get_sdk_headers
 
 ##############################################################################
 # Service
 ##############################################################################
 
 
 class IbmAnalyticsEngineApiV3(BaseService):
     """The IBM Analytics Engine API V3 service."""
 
-    DEFAULT_SERVICE_URL = "https://api.us-south.ae.cloud.ibm.com"
-    DEFAULT_SERVICE_NAME = "ibm_analytics_engine_api"
+    DEFAULT_SERVICE_URL = 'https://api.us-south.ae.cloud.ibm.com'
+    DEFAULT_SERVICE_NAME = 'ibm_analytics_engine_api'
 
     REGIONAL_ENDPOINTS = {
-        "us-south": "https://api.us-south.ae.cloud.ibm.com",
-        "eu-de": "https://api.eu-de.ae.cloud.ibm.com",
+        'us-south': 'https://api.us-south.ae.cloud.ibm.com',
+        'eu-de': 'https://api.eu-de.ae.cloud.ibm.com',
     }
 
     @classmethod
     def new_instance(
         cls,
         service_name: str = DEFAULT_SERVICE_NAME,
-    ) -> "IbmAnalyticsEngineApiV3":
+    ) -> 'IbmAnalyticsEngineApiV3':
         """
         Return a new client for the IBM Analytics Engine API service using the
                specified parameters and external configuration.
         """
         authenticator = get_authenticator_from_environment(service_name)
         service = cls(authenticator)
         service.configure_service(service_name)
@@ -111,33 +106,31 @@
                retrieve.
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `Instance` object
         """
 
         if not instance_id:
-            raise ValueError("instance_id must be provided")
+            raise ValueError('instance_id must be provided')
         headers = {}
         sdk_headers = get_sdk_headers(
-            service_name=self.DEFAULT_SERVICE_NAME,
-            service_version="V3",
-            operation_id="get_instance",
+            service_name=self.DEFAULT_SERVICE_NAME, service_version='V3', operation_id='get_instance'
         )
         headers.update(sdk_headers)
 
-        if "headers" in kwargs:
-            headers.update(kwargs.get("headers"))
-            del kwargs["headers"]
-        headers["Accept"] = "application/json"
+        if 'headers' in kwargs:
+            headers.update(kwargs.get('headers'))
+            del kwargs['headers']
+        headers['Accept'] = 'application/json'
 
-        path_param_keys = ["instance_id"]
+        path_param_keys = ['instance_id']
         path_param_values = self.encode_path_vars(instance_id)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
-        url = "/v3/analytics_engines/{instance_id}".format(**path_param_dict)
-        request = self.prepare_request(method="GET", url=url, headers=headers)
+        url = '/v3/analytics_engines/{instance_id}'.format(**path_param_dict)
+        request = self.prepare_request(method='GET', url=url, headers=headers)
 
         response = self.send(request, **kwargs)
         return response
 
     def get_instance_state(self, instance_id: str, **kwargs) -> DetailedResponse:
         """
         Find Analytics Engine state by id.
@@ -148,33 +141,31 @@
                retrieve state.
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `InstanceGetStateResponse` object
         """
 
         if not instance_id:
-            raise ValueError("instance_id must be provided")
+            raise ValueError('instance_id must be provided')
         headers = {}
         sdk_headers = get_sdk_headers(
-            service_name=self.DEFAULT_SERVICE_NAME,
-            service_version="V3",
-            operation_id="get_instance_state",
+            service_name=self.DEFAULT_SERVICE_NAME, service_version='V3', operation_id='get_instance_state'
         )
         headers.update(sdk_headers)
 
-        if "headers" in kwargs:
-            headers.update(kwargs.get("headers"))
-            del kwargs["headers"]
-        headers["Accept"] = "application/json"
+        if 'headers' in kwargs:
+            headers.update(kwargs.get('headers'))
+            del kwargs['headers']
+        headers['Accept'] = 'application/json'
 
-        path_param_keys = ["instance_id"]
+        path_param_keys = ['instance_id']
         path_param_values = self.encode_path_vars(instance_id)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
-        url = "/v3/analytics_engines/{instance_id}/state".format(**path_param_dict)
-        request = self.prepare_request(method="GET", url=url, headers=headers)
+        url = '/v3/analytics_engines/{instance_id}/state'.format(**path_param_dict)
+        request = self.prepare_request(method='GET', url=url, headers=headers)
 
         response = self.send(request, **kwargs)
         return response
 
     def set_instance_home(
         self,
         instance_id: str,
@@ -182,15 +173,15 @@
         new_instance_id: str = None,
         new_provider: str = None,
         new_type: str = None,
         new_region: str = None,
         new_endpoint: str = None,
         new_hmac_access_key: str = None,
         new_hmac_secret_key: str = None,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Set instance home.
 
         Provide the details of the Cloud Object Storage instance to associate with the
         Analytics Engine instance and use as 'instance home' if 'instance home' has not
         already been set.
@@ -212,46 +203,44 @@
         :param str new_hmac_secret_key: (optional) Cloud Object Storage secret key.
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `InstanceHomeResponse` object
         """
 
         if not instance_id:
-            raise ValueError("instance_id must be provided")
+            raise ValueError('instance_id must be provided')
         headers = {}
         sdk_headers = get_sdk_headers(
-            service_name=self.DEFAULT_SERVICE_NAME,
-            service_version="V3",
-            operation_id="set_instance_home",
+            service_name=self.DEFAULT_SERVICE_NAME, service_version='V3', operation_id='set_instance_home'
         )
         headers.update(sdk_headers)
 
         data = {
-            "instance_id": new_instance_id,
-            "provider": new_provider,
-            "type": new_type,
-            "region": new_region,
-            "endpoint": new_endpoint,
-            "hmac_access_key": new_hmac_access_key,
-            "hmac_secret_key": new_hmac_secret_key,
+            'instance_id': new_instance_id,
+            'provider': new_provider,
+            'type': new_type,
+            'region': new_region,
+            'endpoint': new_endpoint,
+            'hmac_access_key': new_hmac_access_key,
+            'hmac_secret_key': new_hmac_secret_key,
         }
         data = {k: v for (k, v) in data.items() if v is not None}
         data = json.dumps(data)
-        headers["content-type"] = "application/json"
+        headers['content-type'] = 'application/json'
 
-        if "headers" in kwargs:
-            headers.update(kwargs.get("headers"))
-            del kwargs["headers"]
-        headers["Accept"] = "application/json"
+        if 'headers' in kwargs:
+            headers.update(kwargs.get('headers'))
+            del kwargs['headers']
+        headers['Accept'] = 'application/json'
 
-        path_param_keys = ["instance_id"]
+        path_param_keys = ['instance_id']
         path_param_values = self.encode_path_vars(instance_id)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
-        url = "/v3/analytics_engines/{instance_id}/instance_home".format(**path_param_dict)
-        request = self.prepare_request(method="PUT", url=url, headers=headers, data=data)
+        url = '/v3/analytics_engines/{instance_id}/instance_home'.format(**path_param_dict)
+        request = self.prepare_request(method='PUT', url=url, headers=headers, data=data)
 
         response = self.send(request, **kwargs)
         return response
 
     def update_instance_home_credentials(
         self, instance_id: str, hmac_access_key: str, hmac_secret_key: str, **kwargs
     ) -> DetailedResponse:
@@ -270,45 +259,45 @@
         :param str hmac_secret_key: Cloud Object Storage secret key.
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `InstanceHomeResponse` object
         """
 
         if not instance_id:
-            raise ValueError("instance_id must be provided")
+            raise ValueError('instance_id must be provided')
         if hmac_access_key is None:
-            raise ValueError("hmac_access_key must be provided")
+            raise ValueError('hmac_access_key must be provided')
         if hmac_secret_key is None:
-            raise ValueError("hmac_secret_key must be provided")
+            raise ValueError('hmac_secret_key must be provided')
         headers = {}
         sdk_headers = get_sdk_headers(
             service_name=self.DEFAULT_SERVICE_NAME,
-            service_version="V3",
-            operation_id="update_instance_home_credentials",
+            service_version='V3',
+            operation_id='update_instance_home_credentials',
         )
         headers.update(sdk_headers)
 
         data = {
-            "hmac_access_key": hmac_access_key,
-            "hmac_secret_key": hmac_secret_key,
+            'hmac_access_key': hmac_access_key,
+            'hmac_secret_key': hmac_secret_key,
         }
         data = {k: v for (k, v) in data.items() if v is not None}
         data = json.dumps(data)
-        headers["content-type"] = "application/json"
+        headers['content-type'] = 'application/json'
 
-        if "headers" in kwargs:
-            headers.update(kwargs.get("headers"))
-            del kwargs["headers"]
-        headers["Accept"] = "application/json"
+        if 'headers' in kwargs:
+            headers.update(kwargs.get('headers'))
+            del kwargs['headers']
+        headers['Accept'] = 'application/json'
 
-        path_param_keys = ["instance_id"]
+        path_param_keys = ['instance_id']
         path_param_values = self.encode_path_vars(instance_id)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
-        url = "/v3/analytics_engines/{instance_id}/instance_home".format(**path_param_dict)
-        request = self.prepare_request(method="PATCH", url=url, headers=headers, data=data)
+        url = '/v3/analytics_engines/{instance_id}/instance_home'.format(**path_param_dict)
+        request = self.prepare_request(method='PATCH', url=url, headers=headers, data=data)
 
         response = self.send(request, **kwargs)
         return response
 
     def get_instance_default_configs(self, instance_id: str, **kwargs) -> DetailedResponse:
         """
         Get instance default Spark configurations.
@@ -319,33 +308,31 @@
         :param str instance_id: The ID of the Analytics Engine instance.
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result
         """
 
         if not instance_id:
-            raise ValueError("instance_id must be provided")
+            raise ValueError('instance_id must be provided')
         headers = {}
         sdk_headers = get_sdk_headers(
-            service_name=self.DEFAULT_SERVICE_NAME,
-            service_version="V3",
-            operation_id="get_instance_default_configs",
+            service_name=self.DEFAULT_SERVICE_NAME, service_version='V3', operation_id='get_instance_default_configs'
         )
         headers.update(sdk_headers)
 
-        if "headers" in kwargs:
-            headers.update(kwargs.get("headers"))
-            del kwargs["headers"]
-        headers["Accept"] = "application/json"
+        if 'headers' in kwargs:
+            headers.update(kwargs.get('headers'))
+            del kwargs['headers']
+        headers['Accept'] = 'application/json'
 
-        path_param_keys = ["instance_id"]
+        path_param_keys = ['instance_id']
         path_param_values = self.encode_path_vars(instance_id)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
-        url = "/v3/analytics_engines/{instance_id}/default_configs".format(**path_param_dict)
-        request = self.prepare_request(method="GET", url=url, headers=headers)
+        url = '/v3/analytics_engines/{instance_id}/default_configs'.format(**path_param_dict)
+        request = self.prepare_request(method='GET', url=url, headers=headers)
 
         response = self.send(request, **kwargs)
         return response
 
     def replace_instance_default_configs(self, instance_id: str, body: dict, **kwargs) -> DetailedResponse:
         """
         Replace instance default Spark configurations.
@@ -358,38 +345,38 @@
                instance default Spark configurations.
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result
         """
 
         if not instance_id:
-            raise ValueError("instance_id must be provided")
+            raise ValueError('instance_id must be provided')
         if body is None:
-            raise ValueError("body must be provided")
+            raise ValueError('body must be provided')
         headers = {}
         sdk_headers = get_sdk_headers(
             service_name=self.DEFAULT_SERVICE_NAME,
-            service_version="V3",
-            operation_id="replace_instance_default_configs",
+            service_version='V3',
+            operation_id='replace_instance_default_configs',
         )
         headers.update(sdk_headers)
 
         data = json.dumps(body)
-        headers["content-type"] = "application/json"
+        headers['content-type'] = 'application/json'
 
-        if "headers" in kwargs:
-            headers.update(kwargs.get("headers"))
-            del kwargs["headers"]
-        headers["Accept"] = "application/json"
+        if 'headers' in kwargs:
+            headers.update(kwargs.get('headers'))
+            del kwargs['headers']
+        headers['Accept'] = 'application/json'
 
-        path_param_keys = ["instance_id"]
+        path_param_keys = ['instance_id']
         path_param_values = self.encode_path_vars(instance_id)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
-        url = "/v3/analytics_engines/{instance_id}/default_configs".format(**path_param_dict)
-        request = self.prepare_request(method="PUT", url=url, headers=headers, data=data)
+        url = '/v3/analytics_engines/{instance_id}/default_configs'.format(**path_param_dict)
+        request = self.prepare_request(method='PUT', url=url, headers=headers, data=data)
 
         response = self.send(request, **kwargs)
         return response
 
     def update_instance_default_configs(self, instance_id: str, body: dict, **kwargs) -> DetailedResponse:
         """
         Update instance default Spark configurations.
@@ -403,38 +390,36 @@
                to `null` in order to unset it.
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result
         """
 
         if not instance_id:
-            raise ValueError("instance_id must be provided")
+            raise ValueError('instance_id must be provided')
         if body is None:
-            raise ValueError("body must be provided")
+            raise ValueError('body must be provided')
         headers = {}
         sdk_headers = get_sdk_headers(
-            service_name=self.DEFAULT_SERVICE_NAME,
-            service_version="V3",
-            operation_id="update_instance_default_configs",
+            service_name=self.DEFAULT_SERVICE_NAME, service_version='V3', operation_id='update_instance_default_configs'
         )
         headers.update(sdk_headers)
 
         data = json.dumps(body)
-        headers["content-type"] = "application/merge-patch+json"
+        headers['content-type'] = 'application/merge-patch+json'
 
-        if "headers" in kwargs:
-            headers.update(kwargs.get("headers"))
-            del kwargs["headers"]
-        headers["Accept"] = "application/json"
+        if 'headers' in kwargs:
+            headers.update(kwargs.get('headers'))
+            del kwargs['headers']
+        headers['Accept'] = 'application/json'
 
-        path_param_keys = ["instance_id"]
+        path_param_keys = ['instance_id']
         path_param_values = self.encode_path_vars(instance_id)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
-        url = "/v3/analytics_engines/{instance_id}/default_configs".format(**path_param_dict)
-        request = self.prepare_request(method="PATCH", url=url, headers=headers, data=data)
+        url = '/v3/analytics_engines/{instance_id}/default_configs'.format(**path_param_dict)
+        request = self.prepare_request(method='PATCH', url=url, headers=headers, data=data)
 
         response = self.send(request, **kwargs)
         return response
 
     def get_instance_default_runtime(self, instance_id: str, **kwargs) -> DetailedResponse:
         """
         Get instance default runtime.
@@ -445,33 +430,31 @@
         :param str instance_id: The ID of the Analytics Engine instance.
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `Runtime` object
         """
 
         if not instance_id:
-            raise ValueError("instance_id must be provided")
+            raise ValueError('instance_id must be provided')
         headers = {}
         sdk_headers = get_sdk_headers(
-            service_name=self.DEFAULT_SERVICE_NAME,
-            service_version="V3",
-            operation_id="get_instance_default_runtime",
+            service_name=self.DEFAULT_SERVICE_NAME, service_version='V3', operation_id='get_instance_default_runtime'
         )
         headers.update(sdk_headers)
 
-        if "headers" in kwargs:
-            headers.update(kwargs.get("headers"))
-            del kwargs["headers"]
-        headers["Accept"] = "application/json"
+        if 'headers' in kwargs:
+            headers.update(kwargs.get('headers'))
+            del kwargs['headers']
+        headers['Accept'] = 'application/json'
 
-        path_param_keys = ["instance_id"]
+        path_param_keys = ['instance_id']
         path_param_values = self.encode_path_vars(instance_id)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
-        url = "/v3/analytics_engines/{instance_id}/default_runtime".format(**path_param_dict)
-        request = self.prepare_request(method="GET", url=url, headers=headers)
+        url = '/v3/analytics_engines/{instance_id}/default_runtime'.format(**path_param_dict)
+        request = self.prepare_request(method='GET', url=url, headers=headers)
 
         response = self.send(request, **kwargs)
         return response
 
     def replace_instance_default_runtime(
         self, instance_id: str, *, spark_version: str = None, **kwargs
     ) -> DetailedResponse:
@@ -486,46 +469,46 @@
                environment.
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `Runtime` object
         """
 
         if not instance_id:
-            raise ValueError("instance_id must be provided")
+            raise ValueError('instance_id must be provided')
         headers = {}
         sdk_headers = get_sdk_headers(
             service_name=self.DEFAULT_SERVICE_NAME,
-            service_version="V3",
-            operation_id="replace_instance_default_runtime",
+            service_version='V3',
+            operation_id='replace_instance_default_runtime',
         )
         headers.update(sdk_headers)
 
         data = {
-            "spark_version": spark_version,
+            'spark_version': spark_version,
         }
         data = {k: v for (k, v) in data.items() if v is not None}
         data = json.dumps(data)
-        headers["content-type"] = "application/json"
+        headers['content-type'] = 'application/json'
 
-        if "headers" in kwargs:
-            headers.update(kwargs.get("headers"))
-            del kwargs["headers"]
-        headers["Accept"] = "application/json"
+        if 'headers' in kwargs:
+            headers.update(kwargs.get('headers'))
+            del kwargs['headers']
+        headers['Accept'] = 'application/json'
 
-        path_param_keys = ["instance_id"]
+        path_param_keys = ['instance_id']
         path_param_values = self.encode_path_vars(instance_id)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
-        url = "/v3/analytics_engines/{instance_id}/default_runtime".format(**path_param_dict)
-        request = self.prepare_request(method="PUT", url=url, headers=headers, data=data)
+        url = '/v3/analytics_engines/{instance_id}/default_runtime'.format(**path_param_dict)
+        request = self.prepare_request(method='PUT', url=url, headers=headers, data=data)
 
         response = self.send(request, **kwargs)
         return response
 
     def create_application(
-        self, instance_id: str, *, application_details: "ApplicationRequestApplicationDetails" = None, **kwargs
+        self, instance_id: str, *, application_details: 'ApplicationRequestApplicationDetails' = None, **kwargs
     ) -> DetailedResponse:
         """
         Deploy a Spark application.
 
         Deploys a Spark application on a given serverless Spark instance.
 
         :param str instance_id: The identifier of the Analytics Engine instance
@@ -534,86 +517,90 @@
                Application details.
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `ApplicationResponse` object
         """
 
         if not instance_id:
-            raise ValueError("instance_id must be provided")
+            raise ValueError('instance_id must be provided')
         if application_details is not None:
             application_details = convert_model(application_details)
         headers = {}
         sdk_headers = get_sdk_headers(
-            service_name=self.DEFAULT_SERVICE_NAME,
-            service_version="V3",
-            operation_id="create_application",
+            service_name=self.DEFAULT_SERVICE_NAME, service_version='V3', operation_id='create_application'
         )
         headers.update(sdk_headers)
 
         data = {
-            "application_details": application_details,
+            'application_details': application_details,
         }
         data = {k: v for (k, v) in data.items() if v is not None}
         data = json.dumps(data)
-        headers["content-type"] = "application/json"
+        headers['content-type'] = 'application/json'
 
-        if "headers" in kwargs:
-            headers.update(kwargs.get("headers"))
-            del kwargs["headers"]
-        headers["Accept"] = "application/json"
+        if 'headers' in kwargs:
+            headers.update(kwargs.get('headers'))
+            del kwargs['headers']
+        headers['Accept'] = 'application/json'
 
-        path_param_keys = ["instance_id"]
+        path_param_keys = ['instance_id']
         path_param_values = self.encode_path_vars(instance_id)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
-        url = "/v3/analytics_engines/{instance_id}/spark_applications".format(**path_param_dict)
-        request = self.prepare_request(method="POST", url=url, headers=headers, data=data)
+        url = '/v3/analytics_engines/{instance_id}/spark_applications'.format(**path_param_dict)
+        request = self.prepare_request(method='POST', url=url, headers=headers, data=data)
 
         response = self.send(request, **kwargs)
         return response
 
-    def list_applications(self, instance_id: str, *, state: List[str] = None, **kwargs) -> DetailedResponse:
+    def list_applications(
+        self, instance_id: str, *, state: List[str] = None, limit: int = None, start: str = None, **kwargs
+    ) -> DetailedResponse:
         """
         List all Spark applications.
 
         Returns a list of all Spark applications submitted to the specified Analytics
         Engine instance. The result can be filtered by specifying query parameters.
 
         :param str instance_id: The identifier of the Analytics Engine instance
                associated with the Spark application(s).
         :param List[str] state: (optional) List of Spark application states that
                will be used to filter the response.
+        :param int limit: (optional) Number of application entries to be included
+               in the response.
+        :param str start: (optional) Token used to fetch the next or the previous
+               page of the applications list.
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `ApplicationCollection` object
         """
 
         if not instance_id:
-            raise ValueError("instance_id must be provided")
+            raise ValueError('instance_id must be provided')
         headers = {}
         sdk_headers = get_sdk_headers(
-            service_name=self.DEFAULT_SERVICE_NAME,
-            service_version="V3",
-            operation_id="list_applications",
+            service_name=self.DEFAULT_SERVICE_NAME, service_version='V3', operation_id='list_applications'
         )
         headers.update(sdk_headers)
 
         params = {
-            "state": convert_list(state),
+            'state': convert_list(state),
+            'limit': limit,
+            'start': start,
         }
 
-        if "headers" in kwargs:
-            headers.update(kwargs.get("headers"))
-            del kwargs["headers"]
-        headers["Accept"] = "application/json"
+        if 'headers' in kwargs:
+            headers.update(kwargs.get('headers'))
+            del kwargs['headers']
+        headers['Accept'] = 'application/json'
 
-        path_param_keys = ["instance_id"]
+        path_param_keys = ['instance_id']
         path_param_values = self.encode_path_vars(instance_id)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
-        url = "/v3/analytics_engines/{instance_id}/spark_applications".format(**path_param_dict)
-        request = self.prepare_request(method="GET", url=url, headers=headers, params=params)
+        url = '/v3/analytics_engines/{instance_id}/spark_applications'.format(**path_param_dict)
+        request = self.prepare_request(method='GET', url=url, headers=headers, params=params)
 
         response = self.send(request, **kwargs)
         return response
 
     def get_application(self, instance_id: str, application_id: str, **kwargs) -> DetailedResponse:
         """
         Retrieve the details of a given Spark application.
@@ -626,35 +613,33 @@
                are requested.
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `ApplicationGetResponse` object
         """
 
         if not instance_id:
-            raise ValueError("instance_id must be provided")
+            raise ValueError('instance_id must be provided')
         if not application_id:
-            raise ValueError("application_id must be provided")
+            raise ValueError('application_id must be provided')
         headers = {}
         sdk_headers = get_sdk_headers(
-            service_name=self.DEFAULT_SERVICE_NAME,
-            service_version="V3",
-            operation_id="get_application",
+            service_name=self.DEFAULT_SERVICE_NAME, service_version='V3', operation_id='get_application'
         )
         headers.update(sdk_headers)
 
-        if "headers" in kwargs:
-            headers.update(kwargs.get("headers"))
-            del kwargs["headers"]
-        headers["Accept"] = "application/json"
+        if 'headers' in kwargs:
+            headers.update(kwargs.get('headers'))
+            del kwargs['headers']
+        headers['Accept'] = 'application/json'
 
-        path_param_keys = ["instance_id", "application_id"]
+        path_param_keys = ['instance_id', 'application_id']
         path_param_values = self.encode_path_vars(instance_id, application_id)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
-        url = "/v3/analytics_engines/{instance_id}/spark_applications/{application_id}".format(**path_param_dict)
-        request = self.prepare_request(method="GET", url=url, headers=headers)
+        url = '/v3/analytics_engines/{instance_id}/spark_applications/{application_id}'.format(**path_param_dict)
+        request = self.prepare_request(method='GET', url=url, headers=headers)
 
         response = self.send(request, **kwargs)
         return response
 
     def delete_application(self, instance_id: str, application_id: str, **kwargs) -> DetailedResponse:
         """
         Stop application.
@@ -669,34 +654,32 @@
                stopped.
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse
         """
 
         if not instance_id:
-            raise ValueError("instance_id must be provided")
+            raise ValueError('instance_id must be provided')
         if not application_id:
-            raise ValueError("application_id must be provided")
+            raise ValueError('application_id must be provided')
         headers = {}
         sdk_headers = get_sdk_headers(
-            service_name=self.DEFAULT_SERVICE_NAME,
-            service_version="V3",
-            operation_id="delete_application",
+            service_name=self.DEFAULT_SERVICE_NAME, service_version='V3', operation_id='delete_application'
         )
         headers.update(sdk_headers)
 
-        if "headers" in kwargs:
-            headers.update(kwargs.get("headers"))
-            del kwargs["headers"]
+        if 'headers' in kwargs:
+            headers.update(kwargs.get('headers'))
+            del kwargs['headers']
 
-        path_param_keys = ["instance_id", "application_id"]
+        path_param_keys = ['instance_id', 'application_id']
         path_param_values = self.encode_path_vars(instance_id, application_id)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
-        url = "/v3/analytics_engines/{instance_id}/spark_applications/{application_id}".format(**path_param_dict)
-        request = self.prepare_request(method="DELETE", url=url, headers=headers)
+        url = '/v3/analytics_engines/{instance_id}/spark_applications/{application_id}'.format(**path_param_dict)
+        request = self.prepare_request(method='DELETE', url=url, headers=headers)
 
         response = self.send(request, **kwargs)
         return response
 
     def get_application_state(self, instance_id: str, application_id: str, **kwargs) -> DetailedResponse:
         """
         Get the status of the application.
@@ -709,35 +692,33 @@
                are requested.
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `ApplicationGetStateResponse` object
         """
 
         if not instance_id:
-            raise ValueError("instance_id must be provided")
+            raise ValueError('instance_id must be provided')
         if not application_id:
-            raise ValueError("application_id must be provided")
+            raise ValueError('application_id must be provided')
         headers = {}
         sdk_headers = get_sdk_headers(
-            service_name=self.DEFAULT_SERVICE_NAME,
-            service_version="V3",
-            operation_id="get_application_state",
+            service_name=self.DEFAULT_SERVICE_NAME, service_version='V3', operation_id='get_application_state'
         )
         headers.update(sdk_headers)
 
-        if "headers" in kwargs:
-            headers.update(kwargs.get("headers"))
-            del kwargs["headers"]
-        headers["Accept"] = "application/json"
+        if 'headers' in kwargs:
+            headers.update(kwargs.get('headers'))
+            del kwargs['headers']
+        headers['Accept'] = 'application/json'
 
-        path_param_keys = ["instance_id", "application_id"]
+        path_param_keys = ['instance_id', 'application_id']
         path_param_values = self.encode_path_vars(instance_id, application_id)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
-        url = "/v3/analytics_engines/{instance_id}/spark_applications/{application_id}/state".format(**path_param_dict)
-        request = self.prepare_request(method="GET", url=url, headers=headers)
+        url = '/v3/analytics_engines/{instance_id}/spark_applications/{application_id}/state'.format(**path_param_dict)
+        request = self.prepare_request(method='GET', url=url, headers=headers)
 
         response = self.send(request, **kwargs)
         return response
 
     def get_current_resource_consumption(self, instance_id: str, **kwargs) -> DetailedResponse:
         """
         Get current resource consumption.
@@ -753,33 +734,33 @@
         :param str instance_id: ID of the Analytics Engine instance.
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `CurrentResourceConsumptionResponse` object
         """
 
         if not instance_id:
-            raise ValueError("instance_id must be provided")
+            raise ValueError('instance_id must be provided')
         headers = {}
         sdk_headers = get_sdk_headers(
             service_name=self.DEFAULT_SERVICE_NAME,
-            service_version="V3",
-            operation_id="get_current_resource_consumption",
+            service_version='V3',
+            operation_id='get_current_resource_consumption',
         )
         headers.update(sdk_headers)
 
-        if "headers" in kwargs:
-            headers.update(kwargs.get("headers"))
-            del kwargs["headers"]
-        headers["Accept"] = "application/json"
+        if 'headers' in kwargs:
+            headers.update(kwargs.get('headers'))
+            del kwargs['headers']
+        headers['Accept'] = 'application/json'
 
-        path_param_keys = ["instance_id"]
+        path_param_keys = ['instance_id']
         path_param_values = self.encode_path_vars(instance_id)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
-        url = "/v3/analytics_engines/{instance_id}/current_resource_consumption".format(**path_param_dict)
-        request = self.prepare_request(method="GET", url=url, headers=headers)
+        url = '/v3/analytics_engines/{instance_id}/current_resource_consumption'.format(**path_param_dict)
+        request = self.prepare_request(method='GET', url=url, headers=headers)
 
         response = self.send(request, **kwargs)
         return response
 
     def get_resource_consumption_limits(self, instance_id: str, **kwargs) -> DetailedResponse:
         """
         Get resource consumption limits.
@@ -790,33 +771,31 @@
         :param str instance_id: ID of the Analytics Engine instance.
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `ResourceConsumptionLimitsResponse` object
         """
 
         if not instance_id:
-            raise ValueError("instance_id must be provided")
+            raise ValueError('instance_id must be provided')
         headers = {}
         sdk_headers = get_sdk_headers(
-            service_name=self.DEFAULT_SERVICE_NAME,
-            service_version="V3",
-            operation_id="get_resource_consumption_limits",
+            service_name=self.DEFAULT_SERVICE_NAME, service_version='V3', operation_id='get_resource_consumption_limits'
         )
         headers.update(sdk_headers)
 
-        if "headers" in kwargs:
-            headers.update(kwargs.get("headers"))
-            del kwargs["headers"]
-        headers["Accept"] = "application/json"
+        if 'headers' in kwargs:
+            headers.update(kwargs.get('headers'))
+            del kwargs['headers']
+        headers['Accept'] = 'application/json'
 
-        path_param_keys = ["instance_id"]
+        path_param_keys = ['instance_id']
         path_param_values = self.encode_path_vars(instance_id)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
-        url = "/v3/analytics_engines/{instance_id}/resource_consumption_limits".format(**path_param_dict)
-        request = self.prepare_request(method="GET", url=url, headers=headers)
+        url = '/v3/analytics_engines/{instance_id}/resource_consumption_limits'.format(**path_param_dict)
+        request = self.prepare_request(method='GET', url=url, headers=headers)
 
         response = self.send(request, **kwargs)
         return response
 
     def replace_log_forwarding_config(
         self, instance_id: str, *, enabled: bool = None, sources: List[str] = None, tags: List[str] = None, **kwargs
     ) -> DetailedResponse:
@@ -835,42 +814,40 @@
                Analysis server.
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `LogForwardingConfigResponse` object
         """
 
         if not instance_id:
-            raise ValueError("instance_id must be provided")
+            raise ValueError('instance_id must be provided')
         headers = {}
         sdk_headers = get_sdk_headers(
-            service_name=self.DEFAULT_SERVICE_NAME,
-            service_version="V3",
-            operation_id="replace_log_forwarding_config",
+            service_name=self.DEFAULT_SERVICE_NAME, service_version='V3', operation_id='replace_log_forwarding_config'
         )
         headers.update(sdk_headers)
 
         data = {
-            "enabled": enabled,
-            "sources": sources,
-            "tags": tags,
+            'enabled': enabled,
+            'sources': sources,
+            'tags': tags,
         }
         data = {k: v for (k, v) in data.items() if v is not None}
         data = json.dumps(data)
-        headers["content-type"] = "application/json"
+        headers['content-type'] = 'application/json'
 
-        if "headers" in kwargs:
-            headers.update(kwargs.get("headers"))
-            del kwargs["headers"]
-        headers["Accept"] = "application/json"
+        if 'headers' in kwargs:
+            headers.update(kwargs.get('headers'))
+            del kwargs['headers']
+        headers['Accept'] = 'application/json'
 
-        path_param_keys = ["instance_id"]
+        path_param_keys = ['instance_id']
         path_param_values = self.encode_path_vars(instance_id)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
-        url = "/v3/analytics_engines/{instance_id}/log_forwarding_config".format(**path_param_dict)
-        request = self.prepare_request(method="PUT", url=url, headers=headers, data=data)
+        url = '/v3/analytics_engines/{instance_id}/log_forwarding_config'.format(**path_param_dict)
+        request = self.prepare_request(method='PUT', url=url, headers=headers, data=data)
 
         response = self.send(request, **kwargs)
         return response
 
     def get_log_forwarding_config(self, instance_id: str, **kwargs) -> DetailedResponse:
         """
         Get log forwarding configuration.
@@ -880,33 +857,31 @@
         :param str instance_id: ID of the Analytics Engine instance.
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `LogForwardingConfigResponse` object
         """
 
         if not instance_id:
-            raise ValueError("instance_id must be provided")
+            raise ValueError('instance_id must be provided')
         headers = {}
         sdk_headers = get_sdk_headers(
-            service_name=self.DEFAULT_SERVICE_NAME,
-            service_version="V3",
-            operation_id="get_log_forwarding_config",
+            service_name=self.DEFAULT_SERVICE_NAME, service_version='V3', operation_id='get_log_forwarding_config'
         )
         headers.update(sdk_headers)
 
-        if "headers" in kwargs:
-            headers.update(kwargs.get("headers"))
-            del kwargs["headers"]
-        headers["Accept"] = "application/json"
+        if 'headers' in kwargs:
+            headers.update(kwargs.get('headers'))
+            del kwargs['headers']
+        headers['Accept'] = 'application/json'
 
-        path_param_keys = ["instance_id"]
+        path_param_keys = ['instance_id']
         path_param_values = self.encode_path_vars(instance_id)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
-        url = "/v3/analytics_engines/{instance_id}/log_forwarding_config".format(**path_param_dict)
-        request = self.prepare_request(method="GET", url=url, headers=headers)
+        url = '/v3/analytics_engines/{instance_id}/log_forwarding_config'.format(**path_param_dict)
+        request = self.prepare_request(method='GET', url=url, headers=headers)
 
         response = self.send(request, **kwargs)
         return response
 
     def configure_platform_logging(self, instance_guid: str, *, enable: bool = None, **kwargs) -> DetailedResponse:
         """
         Enable or disable log forwarding.
@@ -921,43 +896,41 @@
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `LoggingConfigurationResponse` object
 
         Deprecated: this method is deprecated and may be removed in a future release.
         """
 
-        logging.warning("A deprecated operation has been invoked: configure_platform_logging")
+        logging.warning('A deprecated operation has been invoked: configure_platform_logging')
 
         if not instance_guid:
-            raise ValueError("instance_guid must be provided")
+            raise ValueError('instance_guid must be provided')
         headers = {}
         sdk_headers = get_sdk_headers(
-            service_name=self.DEFAULT_SERVICE_NAME,
-            service_version="V3",
-            operation_id="configure_platform_logging",
+            service_name=self.DEFAULT_SERVICE_NAME, service_version='V3', operation_id='configure_platform_logging'
         )
         headers.update(sdk_headers)
 
         data = {
-            "enable": enable,
+            'enable': enable,
         }
         data = {k: v for (k, v) in data.items() if v is not None}
         data = json.dumps(data)
-        headers["content-type"] = "application/json"
+        headers['content-type'] = 'application/json'
 
-        if "headers" in kwargs:
-            headers.update(kwargs.get("headers"))
-            del kwargs["headers"]
-        headers["Accept"] = "application/json"
+        if 'headers' in kwargs:
+            headers.update(kwargs.get('headers'))
+            del kwargs['headers']
+        headers['Accept'] = 'application/json'
 
-        path_param_keys = ["instance_guid"]
+        path_param_keys = ['instance_guid']
         path_param_values = self.encode_path_vars(instance_guid)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
-        url = "/v3/analytics_engines/{instance_guid}/logging".format(**path_param_dict)
-        request = self.prepare_request(method="PUT", url=url, headers=headers, data=data)
+        url = '/v3/analytics_engines/{instance_guid}/logging'.format(**path_param_dict)
+        request = self.prepare_request(method='PUT', url=url, headers=headers, data=data)
 
         response = self.send(request, **kwargs)
         return response
 
     def get_logging_configuration(self, instance_guid: str, **kwargs) -> DetailedResponse:
         """
         Retrieve the logging configuration for a given instance id.
@@ -970,36 +943,34 @@
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `LoggingConfigurationResponse` object
 
         Deprecated: this method is deprecated and may be removed in a future release.
         """
 
-        logging.warning("A deprecated operation has been invoked: get_logging_configuration")
+        logging.warning('A deprecated operation has been invoked: get_logging_configuration')
 
         if not instance_guid:
-            raise ValueError("instance_guid must be provided")
+            raise ValueError('instance_guid must be provided')
         headers = {}
         sdk_headers = get_sdk_headers(
-            service_name=self.DEFAULT_SERVICE_NAME,
-            service_version="V3",
-            operation_id="get_logging_configuration",
+            service_name=self.DEFAULT_SERVICE_NAME, service_version='V3', operation_id='get_logging_configuration'
         )
         headers.update(sdk_headers)
 
-        if "headers" in kwargs:
-            headers.update(kwargs.get("headers"))
-            del kwargs["headers"]
-        headers["Accept"] = "application/json"
+        if 'headers' in kwargs:
+            headers.update(kwargs.get('headers'))
+            del kwargs['headers']
+        headers['Accept'] = 'application/json'
 
-        path_param_keys = ["instance_guid"]
+        path_param_keys = ['instance_guid']
         path_param_values = self.encode_path_vars(instance_guid)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
-        url = "/v3/analytics_engines/{instance_guid}/logging".format(**path_param_dict)
-        request = self.prepare_request(method="GET", url=url, headers=headers)
+        url = '/v3/analytics_engines/{instance_guid}/logging'.format(**path_param_dict)
+        request = self.prepare_request(method='GET', url=url, headers=headers)
 
         response = self.send(request, **kwargs)
         return response
 
     def start_spark_history_server(self, instance_id: str, **kwargs) -> DetailedResponse:
         """
         Start Spark history server.
@@ -1010,33 +981,31 @@
                the Spark history server belongs.
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `SparkHistoryServerResponse` object
         """
 
         if not instance_id:
-            raise ValueError("instance_id must be provided")
+            raise ValueError('instance_id must be provided')
         headers = {}
         sdk_headers = get_sdk_headers(
-            service_name=self.DEFAULT_SERVICE_NAME,
-            service_version="V3",
-            operation_id="start_spark_history_server",
+            service_name=self.DEFAULT_SERVICE_NAME, service_version='V3', operation_id='start_spark_history_server'
         )
         headers.update(sdk_headers)
 
-        if "headers" in kwargs:
-            headers.update(kwargs.get("headers"))
-            del kwargs["headers"]
-        headers["Accept"] = "application/json"
+        if 'headers' in kwargs:
+            headers.update(kwargs.get('headers'))
+            del kwargs['headers']
+        headers['Accept'] = 'application/json'
 
-        path_param_keys = ["instance_id"]
+        path_param_keys = ['instance_id']
         path_param_values = self.encode_path_vars(instance_id)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
-        url = "/v3/analytics_engines/{instance_id}/spark_history_server".format(**path_param_dict)
-        request = self.prepare_request(method="POST", url=url, headers=headers)
+        url = '/v3/analytics_engines/{instance_id}/spark_history_server'.format(**path_param_dict)
+        request = self.prepare_request(method='POST', url=url, headers=headers)
 
         response = self.send(request, **kwargs)
         return response
 
     def get_spark_history_server(self, instance_id: str, **kwargs) -> DetailedResponse:
         """
         Get Spark history server details.
@@ -1048,33 +1017,31 @@
                the Spark history server belongs.
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `SparkHistoryServerResponse` object
         """
 
         if not instance_id:
-            raise ValueError("instance_id must be provided")
+            raise ValueError('instance_id must be provided')
         headers = {}
         sdk_headers = get_sdk_headers(
-            service_name=self.DEFAULT_SERVICE_NAME,
-            service_version="V3",
-            operation_id="get_spark_history_server",
+            service_name=self.DEFAULT_SERVICE_NAME, service_version='V3', operation_id='get_spark_history_server'
         )
         headers.update(sdk_headers)
 
-        if "headers" in kwargs:
-            headers.update(kwargs.get("headers"))
-            del kwargs["headers"]
-        headers["Accept"] = "application/json"
+        if 'headers' in kwargs:
+            headers.update(kwargs.get('headers'))
+            del kwargs['headers']
+        headers['Accept'] = 'application/json'
 
-        path_param_keys = ["instance_id"]
+        path_param_keys = ['instance_id']
         path_param_values = self.encode_path_vars(instance_id)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
-        url = "/v3/analytics_engines/{instance_id}/spark_history_server".format(**path_param_dict)
-        request = self.prepare_request(method="GET", url=url, headers=headers)
+        url = '/v3/analytics_engines/{instance_id}/spark_history_server'.format(**path_param_dict)
+        request = self.prepare_request(method='GET', url=url, headers=headers)
 
         response = self.send(request, **kwargs)
         return response
 
     def stop_spark_history_server(self, instance_id: str, **kwargs) -> DetailedResponse:
         """
         Stop Spark history server.
@@ -1085,32 +1052,30 @@
                the Spark history server belongs.
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse
         """
 
         if not instance_id:
-            raise ValueError("instance_id must be provided")
+            raise ValueError('instance_id must be provided')
         headers = {}
         sdk_headers = get_sdk_headers(
-            service_name=self.DEFAULT_SERVICE_NAME,
-            service_version="V3",
-            operation_id="stop_spark_history_server",
+            service_name=self.DEFAULT_SERVICE_NAME, service_version='V3', operation_id='stop_spark_history_server'
         )
         headers.update(sdk_headers)
 
-        if "headers" in kwargs:
-            headers.update(kwargs.get("headers"))
-            del kwargs["headers"]
+        if 'headers' in kwargs:
+            headers.update(kwargs.get('headers'))
+            del kwargs['headers']
 
-        path_param_keys = ["instance_id"]
+        path_param_keys = ['instance_id']
         path_param_values = self.encode_path_vars(instance_id)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
-        url = "/v3/analytics_engines/{instance_id}/spark_history_server".format(**path_param_dict)
-        request = self.prepare_request(method="DELETE", url=url, headers=headers)
+        url = '/v3/analytics_engines/{instance_id}/spark_history_server'.format(**path_param_dict)
+        request = self.prepare_request(method='DELETE', url=url, headers=headers)
 
         response = self.send(request, **kwargs)
         return response
 
 
 class ListApplicationsEnums:
     """
@@ -1118,21 +1083,21 @@
     """
 
     class State(str, Enum):
         """
         List of Spark application states that will be used to filter the response.
         """
 
-        FINISHED = "finished"
-        RUNNING = "running"
-        FAILED = "failed"
-        ACCEPTED = "accepted"
-        STOPPED = "stopped"
-        AUTO_TERMINATED = "auto_terminated"
-        OPS_TERMINATED = "ops_terminated"
+        FINISHED = 'finished'
+        RUNNING = 'running'
+        FAILED = 'failed'
+        ACCEPTED = 'accepted'
+        STOPPED = 'stopped'
+        AUTO_TERMINATED = 'auto_terminated'
+        OPS_TERMINATED = 'ops_terminated'
 
 
 ##############################################################################
 # Models
 ##############################################################################
 
 
@@ -1163,24 +1128,24 @@
     """
 
     def __init__(
         self,
         *,
         id: str = None,
         href: str = None,
-        runtime: "Runtime" = None,
+        runtime: 'Runtime' = None,
         spark_application_id: str = None,
         spark_application_name: str = None,
         state: str = None,
         spark_ui: str = None,
         submission_time: datetime = None,
         start_time: datetime = None,
         end_time: datetime = None,
         finish_time: datetime = None,
-        auto_termination_time: datetime = None
+        auto_termination_time: datetime = None,
     ) -> None:
         """
         Initialize a Application object.
 
         :param str id: (optional) Identifier provided by Analytics Engine service
                for the Spark application.
         :param str href: (optional) Full URL of the resource.
@@ -1214,168 +1179,223 @@
         self.submission_time = submission_time
         self.start_time = start_time
         self.end_time = end_time
         self.finish_time = finish_time
         self.auto_termination_time = auto_termination_time
 
     @classmethod
-    def from_dict(cls, _dict: Dict) -> "Application":
+    def from_dict(cls, _dict: Dict) -> 'Application':
         """Initialize a Application object from a json dictionary."""
         args = {}
-        if "id" in _dict:
-            args["id"] = _dict.get("id")
-        if "href" in _dict:
-            args["href"] = _dict.get("href")
-        if "runtime" in _dict:
-            args["runtime"] = Runtime.from_dict(_dict.get("runtime"))
-        if "spark_application_id" in _dict:
-            args["spark_application_id"] = _dict.get("spark_application_id")
-        if "spark_application_name" in _dict:
-            args["spark_application_name"] = _dict.get("spark_application_name")
-        if "state" in _dict:
-            args["state"] = _dict.get("state")
-        if "spark_ui" in _dict:
-            args["spark_ui"] = _dict.get("spark_ui")
-        if "submission_time" in _dict:
-            args["submission_time"] = string_to_datetime(_dict.get("submission_time"))
-        if "start_time" in _dict:
-            args["start_time"] = string_to_datetime(_dict.get("start_time"))
-        if "end_time" in _dict:
-            args["end_time"] = string_to_datetime(_dict.get("end_time"))
-        if "finish_time" in _dict:
-            args["finish_time"] = string_to_datetime(_dict.get("finish_time"))
-        if "auto_termination_time" in _dict:
-            args["auto_termination_time"] = string_to_datetime(_dict.get("auto_termination_time"))
+        if 'id' in _dict:
+            args['id'] = _dict.get('id')
+        if 'href' in _dict:
+            args['href'] = _dict.get('href')
+        if 'runtime' in _dict:
+            args['runtime'] = Runtime.from_dict(_dict.get('runtime'))
+        if 'spark_application_id' in _dict:
+            args['spark_application_id'] = _dict.get('spark_application_id')
+        if 'spark_application_name' in _dict:
+            args['spark_application_name'] = _dict.get('spark_application_name')
+        if 'state' in _dict:
+            args['state'] = _dict.get('state')
+        if 'spark_ui' in _dict:
+            args['spark_ui'] = _dict.get('spark_ui')
+        if 'submission_time' in _dict:
+            args['submission_time'] = string_to_datetime(_dict.get('submission_time'))
+        if 'start_time' in _dict:
+            args['start_time'] = string_to_datetime(_dict.get('start_time'))
+        if 'end_time' in _dict:
+            args['end_time'] = string_to_datetime(_dict.get('end_time'))
+        if 'finish_time' in _dict:
+            args['finish_time'] = string_to_datetime(_dict.get('finish_time'))
+        if 'auto_termination_time' in _dict:
+            args['auto_termination_time'] = string_to_datetime(_dict.get('auto_termination_time'))
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a Application object from a json dictionary."""
         return cls.from_dict(_dict)
 
     def to_dict(self) -> Dict:
         """Return a json dictionary representing this model."""
         _dict = {}
-        if hasattr(self, "id") and self.id is not None:
-            _dict["id"] = self.id
-        if hasattr(self, "href") and self.href is not None:
-            _dict["href"] = self.href
-        if hasattr(self, "runtime") and self.runtime is not None:
+        if hasattr(self, 'id') and self.id is not None:
+            _dict['id'] = self.id
+        if hasattr(self, 'href') and self.href is not None:
+            _dict['href'] = self.href
+        if hasattr(self, 'runtime') and self.runtime is not None:
             if isinstance(self.runtime, dict):
-                _dict["runtime"] = self.runtime
+                _dict['runtime'] = self.runtime
             else:
-                _dict["runtime"] = self.runtime.to_dict()
-        if hasattr(self, "spark_application_id") and self.spark_application_id is not None:
-            _dict["spark_application_id"] = self.spark_application_id
-        if hasattr(self, "spark_application_name") and self.spark_application_name is not None:
-            _dict["spark_application_name"] = self.spark_application_name
-        if hasattr(self, "state") and self.state is not None:
-            _dict["state"] = self.state
-        if hasattr(self, "spark_ui") and self.spark_ui is not None:
-            _dict["spark_ui"] = self.spark_ui
-        if hasattr(self, "submission_time") and self.submission_time is not None:
-            _dict["submission_time"] = datetime_to_string(self.submission_time)
-        if hasattr(self, "start_time") and self.start_time is not None:
-            _dict["start_time"] = datetime_to_string(self.start_time)
-        if hasattr(self, "end_time") and self.end_time is not None:
-            _dict["end_time"] = datetime_to_string(self.end_time)
-        if hasattr(self, "finish_time") and self.finish_time is not None:
-            _dict["finish_time"] = datetime_to_string(self.finish_time)
-        if hasattr(self, "auto_termination_time") and self.auto_termination_time is not None:
-            _dict["auto_termination_time"] = datetime_to_string(self.auto_termination_time)
+                _dict['runtime'] = self.runtime.to_dict()
+        if hasattr(self, 'spark_application_id') and self.spark_application_id is not None:
+            _dict['spark_application_id'] = self.spark_application_id
+        if hasattr(self, 'spark_application_name') and self.spark_application_name is not None:
+            _dict['spark_application_name'] = self.spark_application_name
+        if hasattr(self, 'state') and self.state is not None:
+            _dict['state'] = self.state
+        if hasattr(self, 'spark_ui') and self.spark_ui is not None:
+            _dict['spark_ui'] = self.spark_ui
+        if hasattr(self, 'submission_time') and self.submission_time is not None:
+            _dict['submission_time'] = datetime_to_string(self.submission_time)
+        if hasattr(self, 'start_time') and self.start_time is not None:
+            _dict['start_time'] = datetime_to_string(self.start_time)
+        if hasattr(self, 'end_time') and self.end_time is not None:
+            _dict['end_time'] = datetime_to_string(self.end_time)
+        if hasattr(self, 'finish_time') and self.finish_time is not None:
+            _dict['finish_time'] = datetime_to_string(self.finish_time)
+        if hasattr(self, 'auto_termination_time') and self.auto_termination_time is not None:
+            _dict['auto_termination_time'] = datetime_to_string(self.auto_termination_time)
         return _dict
 
     def _to_dict(self):
         """Return a json dictionary representing this model."""
         return self.to_dict()
 
     def __str__(self) -> str:
         """Return a `str` version of this Application object."""
         return json.dumps(self.to_dict(), indent=2)
 
-    def __eq__(self, other: "Application") -> bool:
+    def __eq__(self, other: 'Application') -> bool:
         """Return `true` when self and other are equal, false otherwise."""
         if not isinstance(other, self.__class__):
             return False
         return self.__dict__ == other.__dict__
 
-    def __ne__(self, other: "Application") -> bool:
+    def __ne__(self, other: 'Application') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
     class StateEnum(str, Enum):
         """
         State of the Spark application.
         """
 
-        FINISHED = "finished"
-        RUNNING = "running"
-        FAILED = "failed"
-        ACCEPTED = "accepted"
-        STOPPED = "stopped"
-        AUTO_TERMINATED = "auto_terminated"
-        OPS_TERMINATED = "ops_terminated"
+        FINISHED = 'finished'
+        RUNNING = 'running'
+        FAILED = 'failed'
+        ACCEPTED = 'accepted'
+        STOPPED = 'stopped'
+        AUTO_TERMINATED = 'auto_terminated'
+        OPS_TERMINATED = 'ops_terminated'
 
 
 class ApplicationCollection:
     """
-    An array of application details.
+    A paginated collection of applications.
 
-    :attr List[Application] applications: (optional) List of applications.
+    :attr List[Application] applications: List of applications.
+    :attr PageLink first: (optional) A reference to a page in a paginated
+          collection.
+    :attr PageLink next: (optional) A reference to a page in a paginated collection.
+    :attr PageLink previous: (optional) A reference to a page in a paginated
+          collection.
+    :attr int limit: The maximum number of results in this page of the collection.
     """
 
-    def __init__(self, *, applications: List["Application"] = None) -> None:
+    def __init__(
+        self,
+        applications: List['Application'],
+        limit: int,
+        *,
+        first: 'PageLink' = None,
+        next: 'PageLink' = None,
+        previous: 'PageLink' = None,
+    ) -> None:
         """
         Initialize a ApplicationCollection object.
 
-        :param List[Application] applications: (optional) List of applications.
+        :param List[Application] applications: List of applications.
+        :param int limit: The maximum number of results in this page of the
+               collection.
+        :param PageLink first: (optional) A reference to a page in a paginated
+               collection.
+        :param PageLink next: (optional) A reference to a page in a paginated
+               collection.
+        :param PageLink previous: (optional) A reference to a page in a paginated
+               collection.
         """
         self.applications = applications
+        self.first = first
+        self.next = next
+        self.previous = previous
+        self.limit = limit
 
     @classmethod
-    def from_dict(cls, _dict: Dict) -> "ApplicationCollection":
+    def from_dict(cls, _dict: Dict) -> 'ApplicationCollection':
         """Initialize a ApplicationCollection object from a json dictionary."""
         args = {}
-        if "applications" in _dict:
-            args["applications"] = [Application.from_dict(v) for v in _dict.get("applications")]
+        if 'applications' in _dict:
+            args['applications'] = [Application.from_dict(v) for v in _dict.get('applications')]
+        else:
+            raise ValueError('Required property \'applications\' not present in ApplicationCollection JSON')
+        if 'first' in _dict:
+            args['first'] = PageLink.from_dict(_dict.get('first'))
+        if 'next' in _dict:
+            args['next'] = PageLink.from_dict(_dict.get('next'))
+        if 'previous' in _dict:
+            args['previous'] = PageLink.from_dict(_dict.get('previous'))
+        if 'limit' in _dict:
+            args['limit'] = _dict.get('limit')
+        else:
+            raise ValueError('Required property \'limit\' not present in ApplicationCollection JSON')
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a ApplicationCollection object from a json dictionary."""
         return cls.from_dict(_dict)
 
     def to_dict(self) -> Dict:
         """Return a json dictionary representing this model."""
         _dict = {}
-        if hasattr(self, "applications") and self.applications is not None:
+        if hasattr(self, 'applications') and self.applications is not None:
             applications_list = []
             for v in self.applications:
                 if isinstance(v, dict):
                     applications_list.append(v)
                 else:
                     applications_list.append(v.to_dict())
-            _dict["applications"] = applications_list
+            _dict['applications'] = applications_list
+        if hasattr(self, 'first') and self.first is not None:
+            if isinstance(self.first, dict):
+                _dict['first'] = self.first
+            else:
+                _dict['first'] = self.first.to_dict()
+        if hasattr(self, 'next') and self.next is not None:
+            if isinstance(self.next, dict):
+                _dict['next'] = self.next
+            else:
+                _dict['next'] = self.next.to_dict()
+        if hasattr(self, 'previous') and self.previous is not None:
+            if isinstance(self.previous, dict):
+                _dict['previous'] = self.previous
+            else:
+                _dict['previous'] = self.previous.to_dict()
+        if hasattr(self, 'limit') and self.limit is not None:
+            _dict['limit'] = self.limit
         return _dict
 
     def _to_dict(self):
         """Return a json dictionary representing this model."""
         return self.to_dict()
 
     def __str__(self) -> str:
         """Return a `str` version of this ApplicationCollection object."""
         return json.dumps(self.to_dict(), indent=2)
 
-    def __eq__(self, other: "ApplicationCollection") -> bool:
+    def __eq__(self, other: 'ApplicationCollection') -> bool:
         """Return `true` when self and other are equal, false otherwise."""
         if not isinstance(other, self.__class__):
             return False
         return self.__dict__ == other.__dict__
 
-    def __ne__(self, other: "ApplicationCollection") -> bool:
+    def __ne__(self, other: 'ApplicationCollection') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
 
 class ApplicationDetails:
     """
     Application details.
@@ -1403,25 +1423,25 @@
           for a list of the supported variables.
     """
 
     def __init__(
         self,
         *,
         application: str = None,
-        runtime: "Runtime" = None,
+        runtime: 'Runtime' = None,
         jars: str = None,
         packages: str = None,
         repositories: str = None,
         files: str = None,
         archives: str = None,
         name: str = None,
         class_: str = None,
         arguments: List[str] = None,
         conf: dict = None,
-        env: dict = None
+        env: dict = None,
     ) -> None:
         """
         Initialize a ApplicationDetails object.
 
         :param str application: (optional) Path of the application to run.
         :param Runtime runtime: (optional) Runtime enviroment for applications and
                other workloads.
@@ -1455,95 +1475,95 @@
         self.name = name
         self.class_ = class_
         self.arguments = arguments
         self.conf = conf
         self.env = env
 
     @classmethod
-    def from_dict(cls, _dict: Dict) -> "ApplicationDetails":
+    def from_dict(cls, _dict: Dict) -> 'ApplicationDetails':
         """Initialize a ApplicationDetails object from a json dictionary."""
         args = {}
-        if "application" in _dict:
-            args["application"] = _dict.get("application")
-        if "runtime" in _dict:
-            args["runtime"] = Runtime.from_dict(_dict.get("runtime"))
-        if "jars" in _dict:
-            args["jars"] = _dict.get("jars")
-        if "packages" in _dict:
-            args["packages"] = _dict.get("packages")
-        if "repositories" in _dict:
-            args["repositories"] = _dict.get("repositories")
-        if "files" in _dict:
-            args["files"] = _dict.get("files")
-        if "archives" in _dict:
-            args["archives"] = _dict.get("archives")
-        if "name" in _dict:
-            args["name"] = _dict.get("name")
-        if "class" in _dict:
-            args["class_"] = _dict.get("class")
-        if "arguments" in _dict:
-            args["arguments"] = _dict.get("arguments")
-        if "conf" in _dict:
-            args["conf"] = _dict.get("conf")
-        if "env" in _dict:
-            args["env"] = _dict.get("env")
+        if 'application' in _dict:
+            args['application'] = _dict.get('application')
+        if 'runtime' in _dict:
+            args['runtime'] = Runtime.from_dict(_dict.get('runtime'))
+        if 'jars' in _dict:
+            args['jars'] = _dict.get('jars')
+        if 'packages' in _dict:
+            args['packages'] = _dict.get('packages')
+        if 'repositories' in _dict:
+            args['repositories'] = _dict.get('repositories')
+        if 'files' in _dict:
+            args['files'] = _dict.get('files')
+        if 'archives' in _dict:
+            args['archives'] = _dict.get('archives')
+        if 'name' in _dict:
+            args['name'] = _dict.get('name')
+        if 'class' in _dict:
+            args['class_'] = _dict.get('class')
+        if 'arguments' in _dict:
+            args['arguments'] = _dict.get('arguments')
+        if 'conf' in _dict:
+            args['conf'] = _dict.get('conf')
+        if 'env' in _dict:
+            args['env'] = _dict.get('env')
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a ApplicationDetails object from a json dictionary."""
         return cls.from_dict(_dict)
 
     def to_dict(self) -> Dict:
         """Return a json dictionary representing this model."""
         _dict = {}
-        if hasattr(self, "application") and self.application is not None:
-            _dict["application"] = self.application
-        if hasattr(self, "runtime") and self.runtime is not None:
+        if hasattr(self, 'application') and self.application is not None:
+            _dict['application'] = self.application
+        if hasattr(self, 'runtime') and self.runtime is not None:
             if isinstance(self.runtime, dict):
-                _dict["runtime"] = self.runtime
+                _dict['runtime'] = self.runtime
             else:
-                _dict["runtime"] = self.runtime.to_dict()
-        if hasattr(self, "jars") and self.jars is not None:
-            _dict["jars"] = self.jars
-        if hasattr(self, "packages") and self.packages is not None:
-            _dict["packages"] = self.packages
-        if hasattr(self, "repositories") and self.repositories is not None:
-            _dict["repositories"] = self.repositories
-        if hasattr(self, "files") and self.files is not None:
-            _dict["files"] = self.files
-        if hasattr(self, "archives") and self.archives is not None:
-            _dict["archives"] = self.archives
-        if hasattr(self, "name") and self.name is not None:
-            _dict["name"] = self.name
-        if hasattr(self, "class_") and self.class_ is not None:
-            _dict["class"] = self.class_
-        if hasattr(self, "arguments") and self.arguments is not None:
-            _dict["arguments"] = self.arguments
-        if hasattr(self, "conf") and self.conf is not None:
-            _dict["conf"] = self.conf
-        if hasattr(self, "env") and self.env is not None:
-            _dict["env"] = self.env
+                _dict['runtime'] = self.runtime.to_dict()
+        if hasattr(self, 'jars') and self.jars is not None:
+            _dict['jars'] = self.jars
+        if hasattr(self, 'packages') and self.packages is not None:
+            _dict['packages'] = self.packages
+        if hasattr(self, 'repositories') and self.repositories is not None:
+            _dict['repositories'] = self.repositories
+        if hasattr(self, 'files') and self.files is not None:
+            _dict['files'] = self.files
+        if hasattr(self, 'archives') and self.archives is not None:
+            _dict['archives'] = self.archives
+        if hasattr(self, 'name') and self.name is not None:
+            _dict['name'] = self.name
+        if hasattr(self, 'class_') and self.class_ is not None:
+            _dict['class'] = self.class_
+        if hasattr(self, 'arguments') and self.arguments is not None:
+            _dict['arguments'] = self.arguments
+        if hasattr(self, 'conf') and self.conf is not None:
+            _dict['conf'] = self.conf
+        if hasattr(self, 'env') and self.env is not None:
+            _dict['env'] = self.env
         return _dict
 
     def _to_dict(self):
         """Return a json dictionary representing this model."""
         return self.to_dict()
 
     def __str__(self) -> str:
         """Return a `str` version of this ApplicationDetails object."""
         return json.dumps(self.to_dict(), indent=2)
 
-    def __eq__(self, other: "ApplicationDetails") -> bool:
+    def __eq__(self, other: 'ApplicationDetails') -> bool:
         """Return `true` when self and other are equal, false otherwise."""
         if not isinstance(other, self.__class__):
             return False
         return self.__dict__ == other.__dict__
 
-    def __ne__(self, other: "ApplicationDetails") -> bool:
+    def __ne__(self, other: 'ApplicationDetails') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
 
 class ApplicationGetResponse:
     """
     Response of the Application Get API.
@@ -1569,26 +1589,26 @@
     :attr datetime auto_termination_time: (optional) Time when the application will
           be automatically stopped by the service.
     """
 
     def __init__(
         self,
         *,
-        application_details: "ApplicationDetails" = None,
+        application_details: 'ApplicationDetails' = None,
         id: str = None,
         spark_application_id: str = None,
         spark_application_name: str = None,
         state: str = None,
         spark_ui: str = None,
-        state_details: List["ApplicationGetResponseStateDetailsItem"] = None,
+        state_details: List['ApplicationGetResponseStateDetailsItem'] = None,
         submission_time: datetime = None,
         start_time: datetime = None,
         end_time: datetime = None,
         finish_time: datetime = None,
-        auto_termination_time: datetime = None
+        auto_termination_time: datetime = None,
     ) -> None:
         """
         Initialize a ApplicationGetResponse object.
 
         :param ApplicationDetails application_details: (optional) Application
                details.
         :param str id: (optional) Application ID.
@@ -1623,118 +1643,118 @@
         self.submission_time = submission_time
         self.start_time = start_time
         self.end_time = end_time
         self.finish_time = finish_time
         self.auto_termination_time = auto_termination_time
 
     @classmethod
-    def from_dict(cls, _dict: Dict) -> "ApplicationGetResponse":
+    def from_dict(cls, _dict: Dict) -> 'ApplicationGetResponse':
         """Initialize a ApplicationGetResponse object from a json dictionary."""
         args = {}
-        if "application_details" in _dict:
-            args["application_details"] = ApplicationDetails.from_dict(_dict.get("application_details"))
-        if "id" in _dict:
-            args["id"] = _dict.get("id")
-        if "spark_application_id" in _dict:
-            args["spark_application_id"] = _dict.get("spark_application_id")
-        if "spark_application_name" in _dict:
-            args["spark_application_name"] = _dict.get("spark_application_name")
-        if "state" in _dict:
-            args["state"] = _dict.get("state")
-        if "spark_ui" in _dict:
-            args["spark_ui"] = _dict.get("spark_ui")
-        if "state_details" in _dict:
-            args["state_details"] = [
-                ApplicationGetResponseStateDetailsItem.from_dict(v) for v in _dict.get("state_details")
+        if 'application_details' in _dict:
+            args['application_details'] = ApplicationDetails.from_dict(_dict.get('application_details'))
+        if 'id' in _dict:
+            args['id'] = _dict.get('id')
+        if 'spark_application_id' in _dict:
+            args['spark_application_id'] = _dict.get('spark_application_id')
+        if 'spark_application_name' in _dict:
+            args['spark_application_name'] = _dict.get('spark_application_name')
+        if 'state' in _dict:
+            args['state'] = _dict.get('state')
+        if 'spark_ui' in _dict:
+            args['spark_ui'] = _dict.get('spark_ui')
+        if 'state_details' in _dict:
+            args['state_details'] = [
+                ApplicationGetResponseStateDetailsItem.from_dict(v) for v in _dict.get('state_details')
             ]
-        if "submission_time" in _dict:
-            args["submission_time"] = string_to_datetime(_dict.get("submission_time"))
-        if "start_time" in _dict:
-            args["start_time"] = string_to_datetime(_dict.get("start_time"))
-        if "end_time" in _dict:
-            args["end_time"] = string_to_datetime(_dict.get("end_time"))
-        if "finish_time" in _dict:
-            args["finish_time"] = string_to_datetime(_dict.get("finish_time"))
-        if "auto_termination_time" in _dict:
-            args["auto_termination_time"] = string_to_datetime(_dict.get("auto_termination_time"))
+        if 'submission_time' in _dict:
+            args['submission_time'] = string_to_datetime(_dict.get('submission_time'))
+        if 'start_time' in _dict:
+            args['start_time'] = string_to_datetime(_dict.get('start_time'))
+        if 'end_time' in _dict:
+            args['end_time'] = string_to_datetime(_dict.get('end_time'))
+        if 'finish_time' in _dict:
+            args['finish_time'] = string_to_datetime(_dict.get('finish_time'))
+        if 'auto_termination_time' in _dict:
+            args['auto_termination_time'] = string_to_datetime(_dict.get('auto_termination_time'))
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a ApplicationGetResponse object from a json dictionary."""
         return cls.from_dict(_dict)
 
     def to_dict(self) -> Dict:
         """Return a json dictionary representing this model."""
         _dict = {}
-        if hasattr(self, "application_details") and self.application_details is not None:
+        if hasattr(self, 'application_details') and self.application_details is not None:
             if isinstance(self.application_details, dict):
-                _dict["application_details"] = self.application_details
+                _dict['application_details'] = self.application_details
             else:
-                _dict["application_details"] = self.application_details.to_dict()
-        if hasattr(self, "id") and self.id is not None:
-            _dict["id"] = self.id
-        if hasattr(self, "spark_application_id") and self.spark_application_id is not None:
-            _dict["spark_application_id"] = self.spark_application_id
-        if hasattr(self, "spark_application_name") and self.spark_application_name is not None:
-            _dict["spark_application_name"] = self.spark_application_name
-        if hasattr(self, "state") and self.state is not None:
-            _dict["state"] = self.state
-        if hasattr(self, "spark_ui") and self.spark_ui is not None:
-            _dict["spark_ui"] = self.spark_ui
-        if hasattr(self, "state_details") and self.state_details is not None:
+                _dict['application_details'] = self.application_details.to_dict()
+        if hasattr(self, 'id') and self.id is not None:
+            _dict['id'] = self.id
+        if hasattr(self, 'spark_application_id') and self.spark_application_id is not None:
+            _dict['spark_application_id'] = self.spark_application_id
+        if hasattr(self, 'spark_application_name') and self.spark_application_name is not None:
+            _dict['spark_application_name'] = self.spark_application_name
+        if hasattr(self, 'state') and self.state is not None:
+            _dict['state'] = self.state
+        if hasattr(self, 'spark_ui') and self.spark_ui is not None:
+            _dict['spark_ui'] = self.spark_ui
+        if hasattr(self, 'state_details') and self.state_details is not None:
             state_details_list = []
             for v in self.state_details:
                 if isinstance(v, dict):
                     state_details_list.append(v)
                 else:
                     state_details_list.append(v.to_dict())
-            _dict["state_details"] = state_details_list
-        if hasattr(self, "submission_time") and self.submission_time is not None:
-            _dict["submission_time"] = datetime_to_string(self.submission_time)
-        if hasattr(self, "start_time") and self.start_time is not None:
-            _dict["start_time"] = datetime_to_string(self.start_time)
-        if hasattr(self, "end_time") and self.end_time is not None:
-            _dict["end_time"] = datetime_to_string(self.end_time)
-        if hasattr(self, "finish_time") and self.finish_time is not None:
-            _dict["finish_time"] = datetime_to_string(self.finish_time)
-        if hasattr(self, "auto_termination_time") and self.auto_termination_time is not None:
-            _dict["auto_termination_time"] = datetime_to_string(self.auto_termination_time)
+            _dict['state_details'] = state_details_list
+        if hasattr(self, 'submission_time') and self.submission_time is not None:
+            _dict['submission_time'] = datetime_to_string(self.submission_time)
+        if hasattr(self, 'start_time') and self.start_time is not None:
+            _dict['start_time'] = datetime_to_string(self.start_time)
+        if hasattr(self, 'end_time') and self.end_time is not None:
+            _dict['end_time'] = datetime_to_string(self.end_time)
+        if hasattr(self, 'finish_time') and self.finish_time is not None:
+            _dict['finish_time'] = datetime_to_string(self.finish_time)
+        if hasattr(self, 'auto_termination_time') and self.auto_termination_time is not None:
+            _dict['auto_termination_time'] = datetime_to_string(self.auto_termination_time)
         return _dict
 
     def _to_dict(self):
         """Return a json dictionary representing this model."""
         return self.to_dict()
 
     def __str__(self) -> str:
         """Return a `str` version of this ApplicationGetResponse object."""
         return json.dumps(self.to_dict(), indent=2)
 
-    def __eq__(self, other: "ApplicationGetResponse") -> bool:
+    def __eq__(self, other: 'ApplicationGetResponse') -> bool:
         """Return `true` when self and other are equal, false otherwise."""
         if not isinstance(other, self.__class__):
             return False
         return self.__dict__ == other.__dict__
 
-    def __ne__(self, other: "ApplicationGetResponse") -> bool:
+    def __ne__(self, other: 'ApplicationGetResponse') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
     class StateEnum(str, Enum):
         """
         State of the Spark application.
         """
 
-        FINISHED = "finished"
-        RUNNING = "running"
-        FAILED = "failed"
-        ACCEPTED = "accepted"
-        STOPPED = "stopped"
-        AUTO_TERMINATED = "auto_terminated"
-        OPS_TERMINATED = "ops_terminated"
+        FINISHED = 'finished'
+        RUNNING = 'running'
+        FAILED = 'failed'
+        ACCEPTED = 'accepted'
+        STOPPED = 'stopped'
+        AUTO_TERMINATED = 'auto_terminated'
+        OPS_TERMINATED = 'ops_terminated'
 
 
 class ApplicationGetResponseStateDetailsItem:
     """
     Additional information message on the current state of the application.
 
     :attr str type: (optional) Type of the message.
@@ -1753,67 +1773,67 @@
                information on the current application state.
         """
         self.type = type
         self.code = code
         self.message = message
 
     @classmethod
-    def from_dict(cls, _dict: Dict) -> "ApplicationGetResponseStateDetailsItem":
+    def from_dict(cls, _dict: Dict) -> 'ApplicationGetResponseStateDetailsItem':
         """Initialize a ApplicationGetResponseStateDetailsItem object from a json dictionary."""
         args = {}
-        if "type" in _dict:
-            args["type"] = _dict.get("type")
-        if "code" in _dict:
-            args["code"] = _dict.get("code")
-        if "message" in _dict:
-            args["message"] = _dict.get("message")
+        if 'type' in _dict:
+            args['type'] = _dict.get('type')
+        if 'code' in _dict:
+            args['code'] = _dict.get('code')
+        if 'message' in _dict:
+            args['message'] = _dict.get('message')
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a ApplicationGetResponseStateDetailsItem object from a json dictionary."""
         return cls.from_dict(_dict)
 
     def to_dict(self) -> Dict:
         """Return a json dictionary representing this model."""
         _dict = {}
-        if hasattr(self, "type") and self.type is not None:
-            _dict["type"] = self.type
-        if hasattr(self, "code") and self.code is not None:
-            _dict["code"] = self.code
-        if hasattr(self, "message") and self.message is not None:
-            _dict["message"] = self.message
+        if hasattr(self, 'type') and self.type is not None:
+            _dict['type'] = self.type
+        if hasattr(self, 'code') and self.code is not None:
+            _dict['code'] = self.code
+        if hasattr(self, 'message') and self.message is not None:
+            _dict['message'] = self.message
         return _dict
 
     def _to_dict(self):
         """Return a json dictionary representing this model."""
         return self.to_dict()
 
     def __str__(self) -> str:
         """Return a `str` version of this ApplicationGetResponseStateDetailsItem object."""
         return json.dumps(self.to_dict(), indent=2)
 
-    def __eq__(self, other: "ApplicationGetResponseStateDetailsItem") -> bool:
+    def __eq__(self, other: 'ApplicationGetResponseStateDetailsItem') -> bool:
         """Return `true` when self and other are equal, false otherwise."""
         if not isinstance(other, self.__class__):
             return False
         return self.__dict__ == other.__dict__
 
-    def __ne__(self, other: "ApplicationGetResponseStateDetailsItem") -> bool:
+    def __ne__(self, other: 'ApplicationGetResponseStateDetailsItem') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
     class TypeEnum(str, Enum):
         """
         Type of the message.
         """
 
-        USER_ERROR = "user_error"
-        SERVER_ERROR = "server_error"
-        INFO = "info"
+        USER_ERROR = 'user_error'
+        SERVER_ERROR = 'server_error'
+        INFO = 'info'
 
 
 class ApplicationGetStateResponse:
     """
     State of a given application.
 
     :attr str id: (optional) Identifier of the application.
@@ -1831,15 +1851,15 @@
         self,
         *,
         id: str = None,
         state: str = None,
         start_time: datetime = None,
         end_time: datetime = None,
         finish_time: datetime = None,
-        auto_termination_time: datetime = None
+        auto_termination_time: datetime = None,
     ) -> None:
         """
         Initialize a ApplicationGetStateResponse object.
 
         :param str id: (optional) Identifier of the application.
         :param str state: (optional) State of the Spark application.
         :param datetime start_time: (optional) Time when the application was
@@ -1855,83 +1875,83 @@
         self.state = state
         self.start_time = start_time
         self.end_time = end_time
         self.finish_time = finish_time
         self.auto_termination_time = auto_termination_time
 
     @classmethod
-    def from_dict(cls, _dict: Dict) -> "ApplicationGetStateResponse":
+    def from_dict(cls, _dict: Dict) -> 'ApplicationGetStateResponse':
         """Initialize a ApplicationGetStateResponse object from a json dictionary."""
         args = {}
-        if "id" in _dict:
-            args["id"] = _dict.get("id")
-        if "state" in _dict:
-            args["state"] = _dict.get("state")
-        if "start_time" in _dict:
-            args["start_time"] = string_to_datetime(_dict.get("start_time"))
-        if "end_time" in _dict:
-            args["end_time"] = string_to_datetime(_dict.get("end_time"))
-        if "finish_time" in _dict:
-            args["finish_time"] = string_to_datetime(_dict.get("finish_time"))
-        if "auto_termination_time" in _dict:
-            args["auto_termination_time"] = string_to_datetime(_dict.get("auto_termination_time"))
+        if 'id' in _dict:
+            args['id'] = _dict.get('id')
+        if 'state' in _dict:
+            args['state'] = _dict.get('state')
+        if 'start_time' in _dict:
+            args['start_time'] = string_to_datetime(_dict.get('start_time'))
+        if 'end_time' in _dict:
+            args['end_time'] = string_to_datetime(_dict.get('end_time'))
+        if 'finish_time' in _dict:
+            args['finish_time'] = string_to_datetime(_dict.get('finish_time'))
+        if 'auto_termination_time' in _dict:
+            args['auto_termination_time'] = string_to_datetime(_dict.get('auto_termination_time'))
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a ApplicationGetStateResponse object from a json dictionary."""
         return cls.from_dict(_dict)
 
     def to_dict(self) -> Dict:
         """Return a json dictionary representing this model."""
         _dict = {}
-        if hasattr(self, "id") and self.id is not None:
-            _dict["id"] = self.id
-        if hasattr(self, "state") and self.state is not None:
-            _dict["state"] = self.state
-        if hasattr(self, "start_time") and self.start_time is not None:
-            _dict["start_time"] = datetime_to_string(self.start_time)
-        if hasattr(self, "end_time") and self.end_time is not None:
-            _dict["end_time"] = datetime_to_string(self.end_time)
-        if hasattr(self, "finish_time") and self.finish_time is not None:
-            _dict["finish_time"] = datetime_to_string(self.finish_time)
-        if hasattr(self, "auto_termination_time") and self.auto_termination_time is not None:
-            _dict["auto_termination_time"] = datetime_to_string(self.auto_termination_time)
+        if hasattr(self, 'id') and self.id is not None:
+            _dict['id'] = self.id
+        if hasattr(self, 'state') and self.state is not None:
+            _dict['state'] = self.state
+        if hasattr(self, 'start_time') and self.start_time is not None:
+            _dict['start_time'] = datetime_to_string(self.start_time)
+        if hasattr(self, 'end_time') and self.end_time is not None:
+            _dict['end_time'] = datetime_to_string(self.end_time)
+        if hasattr(self, 'finish_time') and self.finish_time is not None:
+            _dict['finish_time'] = datetime_to_string(self.finish_time)
+        if hasattr(self, 'auto_termination_time') and self.auto_termination_time is not None:
+            _dict['auto_termination_time'] = datetime_to_string(self.auto_termination_time)
         return _dict
 
     def _to_dict(self):
         """Return a json dictionary representing this model."""
         return self.to_dict()
 
     def __str__(self) -> str:
         """Return a `str` version of this ApplicationGetStateResponse object."""
         return json.dumps(self.to_dict(), indent=2)
 
-    def __eq__(self, other: "ApplicationGetStateResponse") -> bool:
+    def __eq__(self, other: 'ApplicationGetStateResponse') -> bool:
         """Return `true` when self and other are equal, false otherwise."""
         if not isinstance(other, self.__class__):
             return False
         return self.__dict__ == other.__dict__
 
-    def __ne__(self, other: "ApplicationGetStateResponse") -> bool:
+    def __ne__(self, other: 'ApplicationGetStateResponse') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
     class StateEnum(str, Enum):
         """
         State of the Spark application.
         """
 
-        FINISHED = "finished"
-        RUNNING = "running"
-        FAILED = "failed"
-        ACCEPTED = "accepted"
-        STOPPED = "stopped"
-        AUTO_TERMINATED = "auto_terminated"
-        OPS_TERMINATED = "ops_terminated"
+        FINISHED = 'finished'
+        RUNNING = 'running'
+        FAILED = 'failed'
+        ACCEPTED = 'accepted'
+        STOPPED = 'stopped'
+        AUTO_TERMINATED = 'auto_terminated'
+        OPS_TERMINATED = 'ops_terminated'
 
 
 class ApplicationRequestApplicationDetails:
     """
     Application details.
 
     :attr str application: (optional) Path of the application to run.
@@ -1957,25 +1977,25 @@
           for a list of the supported variables.
     """
 
     def __init__(
         self,
         *,
         application: str = None,
-        runtime: "Runtime" = None,
+        runtime: 'Runtime' = None,
         jars: str = None,
         packages: str = None,
         repositories: str = None,
         files: str = None,
         archives: str = None,
         name: str = None,
         class_: str = None,
         arguments: List[str] = None,
         conf: dict = None,
-        env: dict = None
+        env: dict = None,
     ) -> None:
         """
         Initialize a ApplicationRequestApplicationDetails object.
 
         :param str application: (optional) Path of the application to run.
         :param Runtime runtime: (optional) Runtime enviroment for applications and
                other workloads.
@@ -2009,95 +2029,95 @@
         self.name = name
         self.class_ = class_
         self.arguments = arguments
         self.conf = conf
         self.env = env
 
     @classmethod
-    def from_dict(cls, _dict: Dict) -> "ApplicationRequestApplicationDetails":
+    def from_dict(cls, _dict: Dict) -> 'ApplicationRequestApplicationDetails':
         """Initialize a ApplicationRequestApplicationDetails object from a json dictionary."""
         args = {}
-        if "application" in _dict:
-            args["application"] = _dict.get("application")
-        if "runtime" in _dict:
-            args["runtime"] = Runtime.from_dict(_dict.get("runtime"))
-        if "jars" in _dict:
-            args["jars"] = _dict.get("jars")
-        if "packages" in _dict:
-            args["packages"] = _dict.get("packages")
-        if "repositories" in _dict:
-            args["repositories"] = _dict.get("repositories")
-        if "files" in _dict:
-            args["files"] = _dict.get("files")
-        if "archives" in _dict:
-            args["archives"] = _dict.get("archives")
-        if "name" in _dict:
-            args["name"] = _dict.get("name")
-        if "class" in _dict:
-            args["class_"] = _dict.get("class")
-        if "arguments" in _dict:
-            args["arguments"] = _dict.get("arguments")
-        if "conf" in _dict:
-            args["conf"] = _dict.get("conf")
-        if "env" in _dict:
-            args["env"] = _dict.get("env")
+        if 'application' in _dict:
+            args['application'] = _dict.get('application')
+        if 'runtime' in _dict:
+            args['runtime'] = Runtime.from_dict(_dict.get('runtime'))
+        if 'jars' in _dict:
+            args['jars'] = _dict.get('jars')
+        if 'packages' in _dict:
+            args['packages'] = _dict.get('packages')
+        if 'repositories' in _dict:
+            args['repositories'] = _dict.get('repositories')
+        if 'files' in _dict:
+            args['files'] = _dict.get('files')
+        if 'archives' in _dict:
+            args['archives'] = _dict.get('archives')
+        if 'name' in _dict:
+            args['name'] = _dict.get('name')
+        if 'class' in _dict:
+            args['class_'] = _dict.get('class')
+        if 'arguments' in _dict:
+            args['arguments'] = _dict.get('arguments')
+        if 'conf' in _dict:
+            args['conf'] = _dict.get('conf')
+        if 'env' in _dict:
+            args['env'] = _dict.get('env')
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a ApplicationRequestApplicationDetails object from a json dictionary."""
         return cls.from_dict(_dict)
 
     def to_dict(self) -> Dict:
         """Return a json dictionary representing this model."""
         _dict = {}
-        if hasattr(self, "application") and self.application is not None:
-            _dict["application"] = self.application
-        if hasattr(self, "runtime") and self.runtime is not None:
+        if hasattr(self, 'application') and self.application is not None:
+            _dict['application'] = self.application
+        if hasattr(self, 'runtime') and self.runtime is not None:
             if isinstance(self.runtime, dict):
-                _dict["runtime"] = self.runtime
+                _dict['runtime'] = self.runtime
             else:
-                _dict["runtime"] = self.runtime.to_dict()
-        if hasattr(self, "jars") and self.jars is not None:
-            _dict["jars"] = self.jars
-        if hasattr(self, "packages") and self.packages is not None:
-            _dict["packages"] = self.packages
-        if hasattr(self, "repositories") and self.repositories is not None:
-            _dict["repositories"] = self.repositories
-        if hasattr(self, "files") and self.files is not None:
-            _dict["files"] = self.files
-        if hasattr(self, "archives") and self.archives is not None:
-            _dict["archives"] = self.archives
-        if hasattr(self, "name") and self.name is not None:
-            _dict["name"] = self.name
-        if hasattr(self, "class_") and self.class_ is not None:
-            _dict["class"] = self.class_
-        if hasattr(self, "arguments") and self.arguments is not None:
-            _dict["arguments"] = self.arguments
-        if hasattr(self, "conf") and self.conf is not None:
-            _dict["conf"] = self.conf
-        if hasattr(self, "env") and self.env is not None:
-            _dict["env"] = self.env
+                _dict['runtime'] = self.runtime.to_dict()
+        if hasattr(self, 'jars') and self.jars is not None:
+            _dict['jars'] = self.jars
+        if hasattr(self, 'packages') and self.packages is not None:
+            _dict['packages'] = self.packages
+        if hasattr(self, 'repositories') and self.repositories is not None:
+            _dict['repositories'] = self.repositories
+        if hasattr(self, 'files') and self.files is not None:
+            _dict['files'] = self.files
+        if hasattr(self, 'archives') and self.archives is not None:
+            _dict['archives'] = self.archives
+        if hasattr(self, 'name') and self.name is not None:
+            _dict['name'] = self.name
+        if hasattr(self, 'class_') and self.class_ is not None:
+            _dict['class'] = self.class_
+        if hasattr(self, 'arguments') and self.arguments is not None:
+            _dict['arguments'] = self.arguments
+        if hasattr(self, 'conf') and self.conf is not None:
+            _dict['conf'] = self.conf
+        if hasattr(self, 'env') and self.env is not None:
+            _dict['env'] = self.env
         return _dict
 
     def _to_dict(self):
         """Return a json dictionary representing this model."""
         return self.to_dict()
 
     def __str__(self) -> str:
         """Return a `str` version of this ApplicationRequestApplicationDetails object."""
         return json.dumps(self.to_dict(), indent=2)
 
-    def __eq__(self, other: "ApplicationRequestApplicationDetails") -> bool:
+    def __eq__(self, other: 'ApplicationRequestApplicationDetails') -> bool:
         """Return `true` when self and other are equal, false otherwise."""
         if not isinstance(other, self.__class__):
             return False
         return self.__dict__ == other.__dict__
 
-    def __ne__(self, other: "ApplicationRequestApplicationDetails") -> bool:
+    def __ne__(self, other: 'ApplicationRequestApplicationDetails') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
 
 class ApplicationResponse:
     """
     Application response details.
@@ -2113,67 +2133,67 @@
         :param str id: (optional) Identifier of the application that was submitted.
         :param str state: (optional) State of the Spark application.
         """
         self.id = id
         self.state = state
 
     @classmethod
-    def from_dict(cls, _dict: Dict) -> "ApplicationResponse":
+    def from_dict(cls, _dict: Dict) -> 'ApplicationResponse':
         """Initialize a ApplicationResponse object from a json dictionary."""
         args = {}
-        if "id" in _dict:
-            args["id"] = _dict.get("id")
-        if "state" in _dict:
-            args["state"] = _dict.get("state")
+        if 'id' in _dict:
+            args['id'] = _dict.get('id')
+        if 'state' in _dict:
+            args['state'] = _dict.get('state')
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a ApplicationResponse object from a json dictionary."""
         return cls.from_dict(_dict)
 
     def to_dict(self) -> Dict:
         """Return a json dictionary representing this model."""
         _dict = {}
-        if hasattr(self, "id") and self.id is not None:
-            _dict["id"] = self.id
-        if hasattr(self, "state") and self.state is not None:
-            _dict["state"] = self.state
+        if hasattr(self, 'id') and self.id is not None:
+            _dict['id'] = self.id
+        if hasattr(self, 'state') and self.state is not None:
+            _dict['state'] = self.state
         return _dict
 
     def _to_dict(self):
         """Return a json dictionary representing this model."""
         return self.to_dict()
 
     def __str__(self) -> str:
         """Return a `str` version of this ApplicationResponse object."""
         return json.dumps(self.to_dict(), indent=2)
 
-    def __eq__(self, other: "ApplicationResponse") -> bool:
+    def __eq__(self, other: 'ApplicationResponse') -> bool:
         """Return `true` when self and other are equal, false otherwise."""
         if not isinstance(other, self.__class__):
             return False
         return self.__dict__ == other.__dict__
 
-    def __ne__(self, other: "ApplicationResponse") -> bool:
+    def __ne__(self, other: 'ApplicationResponse') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
     class StateEnum(str, Enum):
         """
         State of the Spark application.
         """
 
-        FINISHED = "finished"
-        RUNNING = "running"
-        FAILED = "failed"
-        ACCEPTED = "accepted"
-        STOPPED = "stopped"
-        AUTO_TERMINATED = "auto_terminated"
-        OPS_TERMINATED = "ops_terminated"
+        FINISHED = 'finished'
+        RUNNING = 'running'
+        FAILED = 'failed'
+        ACCEPTED = 'accepted'
+        STOPPED = 'stopped'
+        AUTO_TERMINATED = 'auto_terminated'
+        OPS_TERMINATED = 'ops_terminated'
 
 
 class CurrentResourceConsumptionResponse:
     """
     Current resource consumption of the instance.
 
     :attr str cores: (optional) Number of virtual processor cores used.
@@ -2187,52 +2207,52 @@
         :param str cores: (optional) Number of virtual processor cores used.
         :param str memory: (optional) Amount of memory used.
         """
         self.cores = cores
         self.memory = memory
 
     @classmethod
-    def from_dict(cls, _dict: Dict) -> "CurrentResourceConsumptionResponse":
+    def from_dict(cls, _dict: Dict) -> 'CurrentResourceConsumptionResponse':
         """Initialize a CurrentResourceConsumptionResponse object from a json dictionary."""
         args = {}
-        if "cores" in _dict:
-            args["cores"] = _dict.get("cores")
-        if "memory" in _dict:
-            args["memory"] = _dict.get("memory")
+        if 'cores' in _dict:
+            args['cores'] = _dict.get('cores')
+        if 'memory' in _dict:
+            args['memory'] = _dict.get('memory')
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a CurrentResourceConsumptionResponse object from a json dictionary."""
         return cls.from_dict(_dict)
 
     def to_dict(self) -> Dict:
         """Return a json dictionary representing this model."""
         _dict = {}
-        if hasattr(self, "cores") and self.cores is not None:
-            _dict["cores"] = self.cores
-        if hasattr(self, "memory") and self.memory is not None:
-            _dict["memory"] = self.memory
+        if hasattr(self, 'cores') and self.cores is not None:
+            _dict['cores'] = self.cores
+        if hasattr(self, 'memory') and self.memory is not None:
+            _dict['memory'] = self.memory
         return _dict
 
     def _to_dict(self):
         """Return a json dictionary representing this model."""
         return self.to_dict()
 
     def __str__(self) -> str:
         """Return a `str` version of this CurrentResourceConsumptionResponse object."""
         return json.dumps(self.to_dict(), indent=2)
 
-    def __eq__(self, other: "CurrentResourceConsumptionResponse") -> bool:
+    def __eq__(self, other: 'CurrentResourceConsumptionResponse') -> bool:
         """Return `true` when self and other are equal, false otherwise."""
         if not isinstance(other, self.__class__):
             return False
         return self.__dict__ == other.__dict__
 
-    def __ne__(self, other: "CurrentResourceConsumptionResponse") -> bool:
+    def __ne__(self, other: 'CurrentResourceConsumptionResponse') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
 
 class Instance:
     """
     Details of Analytics Engine instance.
@@ -2253,17 +2273,17 @@
     def __init__(
         self,
         *,
         id: str = None,
         href: str = None,
         state: str = None,
         state_change_time: datetime = None,
-        default_runtime: "Runtime" = None,
-        instance_home: "InstanceHome" = None,
-        default_config: "InstanceDefaultConfig" = None
+        default_runtime: 'Runtime' = None,
+        instance_home: 'InstanceHome' = None,
+        default_config: 'InstanceDefaultConfig' = None,
     ) -> None:
         """
         Initialize a Instance object.
 
         :param str id: (optional) GUID of the Analytics Engine instance.
         :param str href: (optional) Full URL of the resource.
         :param str state: (optional) State of the Analytics Engine instance.
@@ -2281,96 +2301,96 @@
         self.state = state
         self.state_change_time = state_change_time
         self.default_runtime = default_runtime
         self.instance_home = instance_home
         self.default_config = default_config
 
     @classmethod
-    def from_dict(cls, _dict: Dict) -> "Instance":
+    def from_dict(cls, _dict: Dict) -> 'Instance':
         """Initialize a Instance object from a json dictionary."""
         args = {}
-        if "id" in _dict:
-            args["id"] = _dict.get("id")
-        if "href" in _dict:
-            args["href"] = _dict.get("href")
-        if "state" in _dict:
-            args["state"] = _dict.get("state")
-        if "state_change_time" in _dict:
-            args["state_change_time"] = string_to_datetime(_dict.get("state_change_time"))
-        if "default_runtime" in _dict:
-            args["default_runtime"] = Runtime.from_dict(_dict.get("default_runtime"))
-        if "instance_home" in _dict:
-            args["instance_home"] = InstanceHome.from_dict(_dict.get("instance_home"))
-        if "default_config" in _dict:
-            args["default_config"] = InstanceDefaultConfig.from_dict(_dict.get("default_config"))
+        if 'id' in _dict:
+            args['id'] = _dict.get('id')
+        if 'href' in _dict:
+            args['href'] = _dict.get('href')
+        if 'state' in _dict:
+            args['state'] = _dict.get('state')
+        if 'state_change_time' in _dict:
+            args['state_change_time'] = string_to_datetime(_dict.get('state_change_time'))
+        if 'default_runtime' in _dict:
+            args['default_runtime'] = Runtime.from_dict(_dict.get('default_runtime'))
+        if 'instance_home' in _dict:
+            args['instance_home'] = InstanceHome.from_dict(_dict.get('instance_home'))
+        if 'default_config' in _dict:
+            args['default_config'] = InstanceDefaultConfig.from_dict(_dict.get('default_config'))
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a Instance object from a json dictionary."""
         return cls.from_dict(_dict)
 
     def to_dict(self) -> Dict:
         """Return a json dictionary representing this model."""
         _dict = {}
-        if hasattr(self, "id") and self.id is not None:
-            _dict["id"] = self.id
-        if hasattr(self, "href") and self.href is not None:
-            _dict["href"] = self.href
-        if hasattr(self, "state") and self.state is not None:
-            _dict["state"] = self.state
-        if hasattr(self, "state_change_time") and self.state_change_time is not None:
-            _dict["state_change_time"] = datetime_to_string(self.state_change_time)
-        if hasattr(self, "default_runtime") and self.default_runtime is not None:
+        if hasattr(self, 'id') and self.id is not None:
+            _dict['id'] = self.id
+        if hasattr(self, 'href') and self.href is not None:
+            _dict['href'] = self.href
+        if hasattr(self, 'state') and self.state is not None:
+            _dict['state'] = self.state
+        if hasattr(self, 'state_change_time') and self.state_change_time is not None:
+            _dict['state_change_time'] = datetime_to_string(self.state_change_time)
+        if hasattr(self, 'default_runtime') and self.default_runtime is not None:
             if isinstance(self.default_runtime, dict):
-                _dict["default_runtime"] = self.default_runtime
+                _dict['default_runtime'] = self.default_runtime
             else:
-                _dict["default_runtime"] = self.default_runtime.to_dict()
-        if hasattr(self, "instance_home") and self.instance_home is not None:
+                _dict['default_runtime'] = self.default_runtime.to_dict()
+        if hasattr(self, 'instance_home') and self.instance_home is not None:
             if isinstance(self.instance_home, dict):
-                _dict["instance_home"] = self.instance_home
+                _dict['instance_home'] = self.instance_home
             else:
-                _dict["instance_home"] = self.instance_home.to_dict()
-        if hasattr(self, "default_config") and self.default_config is not None:
+                _dict['instance_home'] = self.instance_home.to_dict()
+        if hasattr(self, 'default_config') and self.default_config is not None:
             if isinstance(self.default_config, dict):
-                _dict["default_config"] = self.default_config
+                _dict['default_config'] = self.default_config
             else:
-                _dict["default_config"] = self.default_config.to_dict()
+                _dict['default_config'] = self.default_config.to_dict()
         return _dict
 
     def _to_dict(self):
         """Return a json dictionary representing this model."""
         return self.to_dict()
 
     def __str__(self) -> str:
         """Return a `str` version of this Instance object."""
         return json.dumps(self.to_dict(), indent=2)
 
-    def __eq__(self, other: "Instance") -> bool:
+    def __eq__(self, other: 'Instance') -> bool:
         """Return `true` when self and other are equal, false otherwise."""
         if not isinstance(other, self.__class__):
             return False
         return self.__dict__ == other.__dict__
 
-    def __ne__(self, other: "Instance") -> bool:
+    def __ne__(self, other: 'Instance') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
     class StateEnum(str, Enum):
         """
         State of the Analytics Engine instance.
         """
 
-        CREATION_ACCEPTED = "creation_accepted"
-        INITIALIZED = "initialized"
-        PREPARING = "preparing"
-        ACTIVE = "active"
-        DELETED = "deleted"
-        DISABLED = "disabled"
-        CREATION_FAILED = "creation_failed"
+        CREATION_ACCEPTED = 'creation_accepted'
+        INITIALIZED = 'initialized'
+        PREPARING = 'preparing'
+        ACTIVE = 'active'
+        DELETED = 'deleted'
+        DISABLED = 'disabled'
+        CREATION_FAILED = 'creation_failed'
 
 
 class InstanceDefaultConfig:
     """
     Instance level default configuration for Spark workloads.
 
     :attr str key: (optional) Value of the Spark configuration key.
@@ -2381,48 +2401,48 @@
         Initialize a InstanceDefaultConfig object.
 
         :param str key: (optional) Value of the Spark configuration key.
         """
         self.key = key
 
     @classmethod
-    def from_dict(cls, _dict: Dict) -> "InstanceDefaultConfig":
+    def from_dict(cls, _dict: Dict) -> 'InstanceDefaultConfig':
         """Initialize a InstanceDefaultConfig object from a json dictionary."""
         args = {}
-        if "key" in _dict:
-            args["key"] = _dict.get("key")
+        if 'key' in _dict:
+            args['key'] = _dict.get('key')
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a InstanceDefaultConfig object from a json dictionary."""
         return cls.from_dict(_dict)
 
     def to_dict(self) -> Dict:
         """Return a json dictionary representing this model."""
         _dict = {}
-        if hasattr(self, "key") and self.key is not None:
-            _dict["key"] = self.key
+        if hasattr(self, 'key') and self.key is not None:
+            _dict['key'] = self.key
         return _dict
 
     def _to_dict(self):
         """Return a json dictionary representing this model."""
         return self.to_dict()
 
     def __str__(self) -> str:
         """Return a `str` version of this InstanceDefaultConfig object."""
         return json.dumps(self.to_dict(), indent=2)
 
-    def __eq__(self, other: "InstanceDefaultConfig") -> bool:
+    def __eq__(self, other: 'InstanceDefaultConfig') -> bool:
         """Return `true` when self and other are equal, false otherwise."""
         if not isinstance(other, self.__class__):
             return False
         return self.__dict__ == other.__dict__
 
-    def __ne__(self, other: "InstanceDefaultConfig") -> bool:
+    def __ne__(self, other: 'InstanceDefaultConfig') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
 
 class InstanceGetStateResponse:
     """
     State details of Analytics Engine instance.
@@ -2438,67 +2458,67 @@
         :param str id: (optional) GUID of the Analytics Engine instance.
         :param str state: (optional) State of the Analytics Engine instance.
         """
         self.id = id
         self.state = state
 
     @classmethod
-    def from_dict(cls, _dict: Dict) -> "InstanceGetStateResponse":
+    def from_dict(cls, _dict: Dict) -> 'InstanceGetStateResponse':
         """Initialize a InstanceGetStateResponse object from a json dictionary."""
         args = {}
-        if "id" in _dict:
-            args["id"] = _dict.get("id")
-        if "state" in _dict:
-            args["state"] = _dict.get("state")
+        if 'id' in _dict:
+            args['id'] = _dict.get('id')
+        if 'state' in _dict:
+            args['state'] = _dict.get('state')
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a InstanceGetStateResponse object from a json dictionary."""
         return cls.from_dict(_dict)
 
     def to_dict(self) -> Dict:
         """Return a json dictionary representing this model."""
         _dict = {}
-        if hasattr(self, "id") and self.id is not None:
-            _dict["id"] = self.id
-        if hasattr(self, "state") and self.state is not None:
-            _dict["state"] = self.state
+        if hasattr(self, 'id') and self.id is not None:
+            _dict['id'] = self.id
+        if hasattr(self, 'state') and self.state is not None:
+            _dict['state'] = self.state
         return _dict
 
     def _to_dict(self):
         """Return a json dictionary representing this model."""
         return self.to_dict()
 
     def __str__(self) -> str:
         """Return a `str` version of this InstanceGetStateResponse object."""
         return json.dumps(self.to_dict(), indent=2)
 
-    def __eq__(self, other: "InstanceGetStateResponse") -> bool:
+    def __eq__(self, other: 'InstanceGetStateResponse') -> bool:
         """Return `true` when self and other are equal, false otherwise."""
         if not isinstance(other, self.__class__):
             return False
         return self.__dict__ == other.__dict__
 
-    def __ne__(self, other: "InstanceGetStateResponse") -> bool:
+    def __ne__(self, other: 'InstanceGetStateResponse') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
     class StateEnum(str, Enum):
         """
         State of the Analytics Engine instance.
         """
 
-        CREATION_ACCEPTED = "creation_accepted"
-        INITIALIZED = "initialized"
-        PREPARING = "preparing"
-        ACTIVE = "active"
-        DELETED = "deleted"
-        DISABLED = "disabled"
-        CREATION_FAILED = "creation_failed"
+        CREATION_ACCEPTED = 'creation_accepted'
+        INITIALIZED = 'initialized'
+        PREPARING = 'preparing'
+        ACTIVE = 'active'
+        DELETED = 'deleted'
+        DISABLED = 'disabled'
+        CREATION_FAILED = 'creation_failed'
 
 
 class InstanceHome:
     """
     Object storage instance that acts as the home for custom libraries and Spark events.
 
     :attr str id: (optional) UUID of the instance home storage instance.
@@ -2522,15 +2542,15 @@
         id: str = None,
         provider: str = None,
         type: str = None,
         region: str = None,
         endpoint: str = None,
         bucket: str = None,
         hmac_access_key: str = None,
-        hmac_secret_key: str = None
+        hmac_secret_key: str = None,
     ) -> None:
         """
         Initialize a InstanceHome object.
 
         :param str id: (optional) UUID of the instance home storage instance.
         :param str provider: (optional) Currently only ibm-cos (IBM Cloud Object
                Storage) is supported.
@@ -2552,76 +2572,76 @@
         self.region = region
         self.endpoint = endpoint
         self.bucket = bucket
         self.hmac_access_key = hmac_access_key
         self.hmac_secret_key = hmac_secret_key
 
     @classmethod
-    def from_dict(cls, _dict: Dict) -> "InstanceHome":
+    def from_dict(cls, _dict: Dict) -> 'InstanceHome':
         """Initialize a InstanceHome object from a json dictionary."""
         args = {}
-        if "id" in _dict:
-            args["id"] = _dict.get("id")
-        if "provider" in _dict:
-            args["provider"] = _dict.get("provider")
-        if "type" in _dict:
-            args["type"] = _dict.get("type")
-        if "region" in _dict:
-            args["region"] = _dict.get("region")
-        if "endpoint" in _dict:
-            args["endpoint"] = _dict.get("endpoint")
-        if "bucket" in _dict:
-            args["bucket"] = _dict.get("bucket")
-        if "hmac_access_key" in _dict:
-            args["hmac_access_key"] = _dict.get("hmac_access_key")
-        if "hmac_secret_key" in _dict:
-            args["hmac_secret_key"] = _dict.get("hmac_secret_key")
+        if 'id' in _dict:
+            args['id'] = _dict.get('id')
+        if 'provider' in _dict:
+            args['provider'] = _dict.get('provider')
+        if 'type' in _dict:
+            args['type'] = _dict.get('type')
+        if 'region' in _dict:
+            args['region'] = _dict.get('region')
+        if 'endpoint' in _dict:
+            args['endpoint'] = _dict.get('endpoint')
+        if 'bucket' in _dict:
+            args['bucket'] = _dict.get('bucket')
+        if 'hmac_access_key' in _dict:
+            args['hmac_access_key'] = _dict.get('hmac_access_key')
+        if 'hmac_secret_key' in _dict:
+            args['hmac_secret_key'] = _dict.get('hmac_secret_key')
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a InstanceHome object from a json dictionary."""
         return cls.from_dict(_dict)
 
     def to_dict(self) -> Dict:
         """Return a json dictionary representing this model."""
         _dict = {}
-        if hasattr(self, "id") and self.id is not None:
-            _dict["id"] = self.id
-        if hasattr(self, "provider") and self.provider is not None:
-            _dict["provider"] = self.provider
-        if hasattr(self, "type") and self.type is not None:
-            _dict["type"] = self.type
-        if hasattr(self, "region") and self.region is not None:
-            _dict["region"] = self.region
-        if hasattr(self, "endpoint") and self.endpoint is not None:
-            _dict["endpoint"] = self.endpoint
-        if hasattr(self, "bucket") and self.bucket is not None:
-            _dict["bucket"] = self.bucket
-        if hasattr(self, "hmac_access_key") and self.hmac_access_key is not None:
-            _dict["hmac_access_key"] = self.hmac_access_key
-        if hasattr(self, "hmac_secret_key") and self.hmac_secret_key is not None:
-            _dict["hmac_secret_key"] = self.hmac_secret_key
+        if hasattr(self, 'id') and self.id is not None:
+            _dict['id'] = self.id
+        if hasattr(self, 'provider') and self.provider is not None:
+            _dict['provider'] = self.provider
+        if hasattr(self, 'type') and self.type is not None:
+            _dict['type'] = self.type
+        if hasattr(self, 'region') and self.region is not None:
+            _dict['region'] = self.region
+        if hasattr(self, 'endpoint') and self.endpoint is not None:
+            _dict['endpoint'] = self.endpoint
+        if hasattr(self, 'bucket') and self.bucket is not None:
+            _dict['bucket'] = self.bucket
+        if hasattr(self, 'hmac_access_key') and self.hmac_access_key is not None:
+            _dict['hmac_access_key'] = self.hmac_access_key
+        if hasattr(self, 'hmac_secret_key') and self.hmac_secret_key is not None:
+            _dict['hmac_secret_key'] = self.hmac_secret_key
         return _dict
 
     def _to_dict(self):
         """Return a json dictionary representing this model."""
         return self.to_dict()
 
     def __str__(self) -> str:
         """Return a `str` version of this InstanceHome object."""
         return json.dumps(self.to_dict(), indent=2)
 
-    def __eq__(self, other: "InstanceHome") -> bool:
+    def __eq__(self, other: 'InstanceHome') -> bool:
         """Return `true` when self and other are equal, false otherwise."""
         if not isinstance(other, self.__class__):
             return False
         return self.__dict__ == other.__dict__
 
-    def __ne__(self, other: "InstanceHome") -> bool:
+    def __ne__(self, other: 'InstanceHome') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
 
 class InstanceHomeResponse:
     """
     Response of Instance home API.
@@ -2643,15 +2663,15 @@
         *,
         instance_id: str = None,
         provider: str = None,
         type: str = None,
         region: str = None,
         endpoint: str = None,
         hmac_access_key: str = None,
-        hmac_secret_key: str = None
+        hmac_secret_key: str = None,
     ) -> None:
         """
         Initialize a InstanceHomeResponse object.
 
         :param str instance_id: (optional) UUID of the instance home storage
                instance.
         :param str provider: (optional) Currently only ibm-cos (IBM Cloud Object
@@ -2669,72 +2689,72 @@
         self.type = type
         self.region = region
         self.endpoint = endpoint
         self.hmac_access_key = hmac_access_key
         self.hmac_secret_key = hmac_secret_key
 
     @classmethod
-    def from_dict(cls, _dict: Dict) -> "InstanceHomeResponse":
+    def from_dict(cls, _dict: Dict) -> 'InstanceHomeResponse':
         """Initialize a InstanceHomeResponse object from a json dictionary."""
         args = {}
-        if "instance_id" in _dict:
-            args["instance_id"] = _dict.get("instance_id")
-        if "provider" in _dict:
-            args["provider"] = _dict.get("provider")
-        if "type" in _dict:
-            args["type"] = _dict.get("type")
-        if "region" in _dict:
-            args["region"] = _dict.get("region")
-        if "endpoint" in _dict:
-            args["endpoint"] = _dict.get("endpoint")
-        if "hmac_access_key" in _dict:
-            args["hmac_access_key"] = _dict.get("hmac_access_key")
-        if "hmac_secret_key" in _dict:
-            args["hmac_secret_key"] = _dict.get("hmac_secret_key")
+        if 'instance_id' in _dict:
+            args['instance_id'] = _dict.get('instance_id')
+        if 'provider' in _dict:
+            args['provider'] = _dict.get('provider')
+        if 'type' in _dict:
+            args['type'] = _dict.get('type')
+        if 'region' in _dict:
+            args['region'] = _dict.get('region')
+        if 'endpoint' in _dict:
+            args['endpoint'] = _dict.get('endpoint')
+        if 'hmac_access_key' in _dict:
+            args['hmac_access_key'] = _dict.get('hmac_access_key')
+        if 'hmac_secret_key' in _dict:
+            args['hmac_secret_key'] = _dict.get('hmac_secret_key')
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a InstanceHomeResponse object from a json dictionary."""
         return cls.from_dict(_dict)
 
     def to_dict(self) -> Dict:
         """Return a json dictionary representing this model."""
         _dict = {}
-        if hasattr(self, "instance_id") and self.instance_id is not None:
-            _dict["instance_id"] = self.instance_id
-        if hasattr(self, "provider") and self.provider is not None:
-            _dict["provider"] = self.provider
-        if hasattr(self, "type") and self.type is not None:
-            _dict["type"] = self.type
-        if hasattr(self, "region") and self.region is not None:
-            _dict["region"] = self.region
-        if hasattr(self, "endpoint") and self.endpoint is not None:
-            _dict["endpoint"] = self.endpoint
-        if hasattr(self, "hmac_access_key") and self.hmac_access_key is not None:
-            _dict["hmac_access_key"] = self.hmac_access_key
-        if hasattr(self, "hmac_secret_key") and self.hmac_secret_key is not None:
-            _dict["hmac_secret_key"] = self.hmac_secret_key
+        if hasattr(self, 'instance_id') and self.instance_id is not None:
+            _dict['instance_id'] = self.instance_id
+        if hasattr(self, 'provider') and self.provider is not None:
+            _dict['provider'] = self.provider
+        if hasattr(self, 'type') and self.type is not None:
+            _dict['type'] = self.type
+        if hasattr(self, 'region') and self.region is not None:
+            _dict['region'] = self.region
+        if hasattr(self, 'endpoint') and self.endpoint is not None:
+            _dict['endpoint'] = self.endpoint
+        if hasattr(self, 'hmac_access_key') and self.hmac_access_key is not None:
+            _dict['hmac_access_key'] = self.hmac_access_key
+        if hasattr(self, 'hmac_secret_key') and self.hmac_secret_key is not None:
+            _dict['hmac_secret_key'] = self.hmac_secret_key
         return _dict
 
     def _to_dict(self):
         """Return a json dictionary representing this model."""
         return self.to_dict()
 
     def __str__(self) -> str:
         """Return a `str` version of this InstanceHomeResponse object."""
         return json.dumps(self.to_dict(), indent=2)
 
-    def __eq__(self, other: "InstanceHomeResponse") -> bool:
+    def __eq__(self, other: 'InstanceHomeResponse') -> bool:
         """Return `true` when self and other are equal, false otherwise."""
         if not isinstance(other, self.__class__):
             return False
         return self.__dict__ == other.__dict__
 
-    def __ne__(self, other: "InstanceHomeResponse") -> bool:
+    def __ne__(self, other: 'InstanceHomeResponse') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
 
 class LogForwardingConfigResponse:
     """
     Log forwarding configuration details.
@@ -2750,16 +2770,16 @@
     """
 
     def __init__(
         self,
         *,
         sources: List[str] = None,
         tags: List[str] = None,
-        log_server: "LogForwardingConfigResponseLogServer" = None,
-        enabled: bool = None
+        log_server: 'LogForwardingConfigResponseLogServer' = None,
+        enabled: bool = None,
     ) -> None:
         """
         Initialize a LogForwardingConfigResponse object.
 
         :param List[str] sources: (optional) List of sources of logs that are being
                forwarded.
         :param List[str] tags: (optional) List of tags that are applied to the logs
@@ -2771,63 +2791,63 @@
         """
         self.sources = sources
         self.tags = tags
         self.log_server = log_server
         self.enabled = enabled
 
     @classmethod
-    def from_dict(cls, _dict: Dict) -> "LogForwardingConfigResponse":
+    def from_dict(cls, _dict: Dict) -> 'LogForwardingConfigResponse':
         """Initialize a LogForwardingConfigResponse object from a json dictionary."""
         args = {}
-        if "sources" in _dict:
-            args["sources"] = _dict.get("sources")
-        if "tags" in _dict:
-            args["tags"] = _dict.get("tags")
-        if "log_server" in _dict:
-            args["log_server"] = LogForwardingConfigResponseLogServer.from_dict(_dict.get("log_server"))
-        if "enabled" in _dict:
-            args["enabled"] = _dict.get("enabled")
+        if 'sources' in _dict:
+            args['sources'] = _dict.get('sources')
+        if 'tags' in _dict:
+            args['tags'] = _dict.get('tags')
+        if 'log_server' in _dict:
+            args['log_server'] = LogForwardingConfigResponseLogServer.from_dict(_dict.get('log_server'))
+        if 'enabled' in _dict:
+            args['enabled'] = _dict.get('enabled')
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a LogForwardingConfigResponse object from a json dictionary."""
         return cls.from_dict(_dict)
 
     def to_dict(self) -> Dict:
         """Return a json dictionary representing this model."""
         _dict = {}
-        if hasattr(self, "sources") and self.sources is not None:
-            _dict["sources"] = self.sources
-        if hasattr(self, "tags") and self.tags is not None:
-            _dict["tags"] = self.tags
-        if hasattr(self, "log_server") and self.log_server is not None:
+        if hasattr(self, 'sources') and self.sources is not None:
+            _dict['sources'] = self.sources
+        if hasattr(self, 'tags') and self.tags is not None:
+            _dict['tags'] = self.tags
+        if hasattr(self, 'log_server') and self.log_server is not None:
             if isinstance(self.log_server, dict):
-                _dict["log_server"] = self.log_server
+                _dict['log_server'] = self.log_server
             else:
-                _dict["log_server"] = self.log_server.to_dict()
-        if hasattr(self, "enabled") and self.enabled is not None:
-            _dict["enabled"] = self.enabled
+                _dict['log_server'] = self.log_server.to_dict()
+        if hasattr(self, 'enabled') and self.enabled is not None:
+            _dict['enabled'] = self.enabled
         return _dict
 
     def _to_dict(self):
         """Return a json dictionary representing this model."""
         return self.to_dict()
 
     def __str__(self) -> str:
         """Return a `str` version of this LogForwardingConfigResponse object."""
         return json.dumps(self.to_dict(), indent=2)
 
-    def __eq__(self, other: "LogForwardingConfigResponse") -> bool:
+    def __eq__(self, other: 'LogForwardingConfigResponse') -> bool:
         """Return `true` when self and other are equal, false otherwise."""
         if not isinstance(other, self.__class__):
             return False
         return self.__dict__ == other.__dict__
 
-    def __ne__(self, other: "LogForwardingConfigResponse") -> bool:
+    def __ne__(self, other: 'LogForwardingConfigResponse') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
 
 class LogForwardingConfigResponseLogServer:
     """
     Log server properties.
@@ -2840,48 +2860,48 @@
         Initialize a LogForwardingConfigResponseLogServer object.
 
         :param str type: (optional) Type of the log server.
         """
         self.type = type
 
     @classmethod
-    def from_dict(cls, _dict: Dict) -> "LogForwardingConfigResponseLogServer":
+    def from_dict(cls, _dict: Dict) -> 'LogForwardingConfigResponseLogServer':
         """Initialize a LogForwardingConfigResponseLogServer object from a json dictionary."""
         args = {}
-        if "type" in _dict:
-            args["type"] = _dict.get("type")
+        if 'type' in _dict:
+            args['type'] = _dict.get('type')
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a LogForwardingConfigResponseLogServer object from a json dictionary."""
         return cls.from_dict(_dict)
 
     def to_dict(self) -> Dict:
         """Return a json dictionary representing this model."""
         _dict = {}
-        if hasattr(self, "type") and self.type is not None:
-            _dict["type"] = self.type
+        if hasattr(self, 'type') and self.type is not None:
+            _dict['type'] = self.type
         return _dict
 
     def _to_dict(self):
         """Return a json dictionary representing this model."""
         return self.to_dict()
 
     def __str__(self) -> str:
         """Return a `str` version of this LogForwardingConfigResponseLogServer object."""
         return json.dumps(self.to_dict(), indent=2)
 
-    def __eq__(self, other: "LogForwardingConfigResponseLogServer") -> bool:
+    def __eq__(self, other: 'LogForwardingConfigResponseLogServer') -> bool:
         """Return `true` when self and other are equal, false otherwise."""
         if not isinstance(other, self.__class__):
             return False
         return self.__dict__ == other.__dict__
 
-    def __ne__(self, other: "LogForwardingConfigResponseLogServer") -> bool:
+    def __ne__(self, other: 'LogForwardingConfigResponseLogServer') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
 
 class LoggingConfigurationResponse:
     """
     (deprecated) Response of logging API.
@@ -2892,75 +2912,75 @@
     :attr bool enable: (optional) enable.
     """
 
     def __init__(
         self,
         *,
         components: List[str] = None,
-        log_server: "LoggingConfigurationResponseLogServer" = None,
-        enable: bool = None
+        log_server: 'LoggingConfigurationResponseLogServer' = None,
+        enable: bool = None,
     ) -> None:
         """
         Initialize a LoggingConfigurationResponse object.
 
         :param List[str] components: (optional) component array.
         :param LoggingConfigurationResponseLogServer log_server: (optional) log
                server properties.
         :param bool enable: (optional) enable.
         """
         self.components = components
         self.log_server = log_server
         self.enable = enable
 
     @classmethod
-    def from_dict(cls, _dict: Dict) -> "LoggingConfigurationResponse":
+    def from_dict(cls, _dict: Dict) -> 'LoggingConfigurationResponse':
         """Initialize a LoggingConfigurationResponse object from a json dictionary."""
         args = {}
-        if "components" in _dict:
-            args["components"] = _dict.get("components")
-        if "log_server" in _dict:
-            args["log_server"] = LoggingConfigurationResponseLogServer.from_dict(_dict.get("log_server"))
-        if "enable" in _dict:
-            args["enable"] = _dict.get("enable")
+        if 'components' in _dict:
+            args['components'] = _dict.get('components')
+        if 'log_server' in _dict:
+            args['log_server'] = LoggingConfigurationResponseLogServer.from_dict(_dict.get('log_server'))
+        if 'enable' in _dict:
+            args['enable'] = _dict.get('enable')
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a LoggingConfigurationResponse object from a json dictionary."""
         return cls.from_dict(_dict)
 
     def to_dict(self) -> Dict:
         """Return a json dictionary representing this model."""
         _dict = {}
-        if hasattr(self, "components") and self.components is not None:
-            _dict["components"] = self.components
-        if hasattr(self, "log_server") and self.log_server is not None:
+        if hasattr(self, 'components') and self.components is not None:
+            _dict['components'] = self.components
+        if hasattr(self, 'log_server') and self.log_server is not None:
             if isinstance(self.log_server, dict):
-                _dict["log_server"] = self.log_server
+                _dict['log_server'] = self.log_server
             else:
-                _dict["log_server"] = self.log_server.to_dict()
-        if hasattr(self, "enable") and self.enable is not None:
-            _dict["enable"] = self.enable
+                _dict['log_server'] = self.log_server.to_dict()
+        if hasattr(self, 'enable') and self.enable is not None:
+            _dict['enable'] = self.enable
         return _dict
 
     def _to_dict(self):
         """Return a json dictionary representing this model."""
         return self.to_dict()
 
     def __str__(self) -> str:
         """Return a `str` version of this LoggingConfigurationResponse object."""
         return json.dumps(self.to_dict(), indent=2)
 
-    def __eq__(self, other: "LoggingConfigurationResponse") -> bool:
+    def __eq__(self, other: 'LoggingConfigurationResponse') -> bool:
         """Return `true` when self and other are equal, false otherwise."""
         if not isinstance(other, self.__class__):
             return False
         return self.__dict__ == other.__dict__
 
-    def __ne__(self, other: "LoggingConfigurationResponse") -> bool:
+    def __ne__(self, other: 'LoggingConfigurationResponse') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
 
 class LoggingConfigurationResponseLogServer:
     """
     log server properties.
@@ -2973,48 +2993,113 @@
         Initialize a LoggingConfigurationResponseLogServer object.
 
         :param str type: (optional) type of log server.
         """
         self.type = type
 
     @classmethod
-    def from_dict(cls, _dict: Dict) -> "LoggingConfigurationResponseLogServer":
+    def from_dict(cls, _dict: Dict) -> 'LoggingConfigurationResponseLogServer':
         """Initialize a LoggingConfigurationResponseLogServer object from a json dictionary."""
         args = {}
-        if "type" in _dict:
-            args["type"] = _dict.get("type")
+        if 'type' in _dict:
+            args['type'] = _dict.get('type')
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a LoggingConfigurationResponseLogServer object from a json dictionary."""
         return cls.from_dict(_dict)
 
     def to_dict(self) -> Dict:
         """Return a json dictionary representing this model."""
         _dict = {}
-        if hasattr(self, "type") and self.type is not None:
-            _dict["type"] = self.type
+        if hasattr(self, 'type') and self.type is not None:
+            _dict['type'] = self.type
         return _dict
 
     def _to_dict(self):
         """Return a json dictionary representing this model."""
         return self.to_dict()
 
     def __str__(self) -> str:
         """Return a `str` version of this LoggingConfigurationResponseLogServer object."""
         return json.dumps(self.to_dict(), indent=2)
 
-    def __eq__(self, other: "LoggingConfigurationResponseLogServer") -> bool:
+    def __eq__(self, other: 'LoggingConfigurationResponseLogServer') -> bool:
         """Return `true` when self and other are equal, false otherwise."""
         if not isinstance(other, self.__class__):
             return False
         return self.__dict__ == other.__dict__
 
-    def __ne__(self, other: "LoggingConfigurationResponseLogServer") -> bool:
+    def __ne__(self, other: 'LoggingConfigurationResponseLogServer') -> bool:
+        """Return `true` when self and other are not equal, false otherwise."""
+        return not self == other
+
+
+class PageLink:
+    """
+    A reference to a page in a paginated collection.
+
+    :attr str href: A url which returns a specific page of a collection.
+    :attr str start: (optional) A token which loads a specific page of a collection
+          when it is provided the url of the collection.
+    """
+
+    def __init__(self, href: str, *, start: str = None) -> None:
+        """
+        Initialize a PageLink object.
+
+        :param str href: A url which returns a specific page of a collection.
+        :param str start: (optional) A token which loads a specific page of a
+               collection when it is provided the url of the collection.
+        """
+        self.href = href
+        self.start = start
+
+    @classmethod
+    def from_dict(cls, _dict: Dict) -> 'PageLink':
+        """Initialize a PageLink object from a json dictionary."""
+        args = {}
+        if 'href' in _dict:
+            args['href'] = _dict.get('href')
+        else:
+            raise ValueError('Required property \'href\' not present in PageLink JSON')
+        if 'start' in _dict:
+            args['start'] = _dict.get('start')
+        return cls(**args)
+
+    @classmethod
+    def _from_dict(cls, _dict):
+        """Initialize a PageLink object from a json dictionary."""
+        return cls.from_dict(_dict)
+
+    def to_dict(self) -> Dict:
+        """Return a json dictionary representing this model."""
+        _dict = {}
+        if hasattr(self, 'href') and self.href is not None:
+            _dict['href'] = self.href
+        if hasattr(self, 'start') and self.start is not None:
+            _dict['start'] = self.start
+        return _dict
+
+    def _to_dict(self):
+        """Return a json dictionary representing this model."""
+        return self.to_dict()
+
+    def __str__(self) -> str:
+        """Return a `str` version of this PageLink object."""
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __eq__(self, other: 'PageLink') -> bool:
+        """Return `true` when self and other are equal, false otherwise."""
+        if not isinstance(other, self.__class__):
+            return False
+        return self.__dict__ == other.__dict__
+
+    def __ne__(self, other: 'PageLink') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
 
 class ResourceConsumptionLimitsResponse:
     """
     Resource consumption limits for the instance.
@@ -3034,52 +3119,52 @@
         :param str max_memory: (optional) Maximum memory that can be used in the
                instance.
         """
         self.max_cores = max_cores
         self.max_memory = max_memory
 
     @classmethod
-    def from_dict(cls, _dict: Dict) -> "ResourceConsumptionLimitsResponse":
+    def from_dict(cls, _dict: Dict) -> 'ResourceConsumptionLimitsResponse':
         """Initialize a ResourceConsumptionLimitsResponse object from a json dictionary."""
         args = {}
-        if "max_cores" in _dict:
-            args["max_cores"] = _dict.get("max_cores")
-        if "max_memory" in _dict:
-            args["max_memory"] = _dict.get("max_memory")
+        if 'max_cores' in _dict:
+            args['max_cores'] = _dict.get('max_cores')
+        if 'max_memory' in _dict:
+            args['max_memory'] = _dict.get('max_memory')
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a ResourceConsumptionLimitsResponse object from a json dictionary."""
         return cls.from_dict(_dict)
 
     def to_dict(self) -> Dict:
         """Return a json dictionary representing this model."""
         _dict = {}
-        if hasattr(self, "max_cores") and self.max_cores is not None:
-            _dict["max_cores"] = self.max_cores
-        if hasattr(self, "max_memory") and self.max_memory is not None:
-            _dict["max_memory"] = self.max_memory
+        if hasattr(self, 'max_cores') and self.max_cores is not None:
+            _dict['max_cores'] = self.max_cores
+        if hasattr(self, 'max_memory') and self.max_memory is not None:
+            _dict['max_memory'] = self.max_memory
         return _dict
 
     def _to_dict(self):
         """Return a json dictionary representing this model."""
         return self.to_dict()
 
     def __str__(self) -> str:
         """Return a `str` version of this ResourceConsumptionLimitsResponse object."""
         return json.dumps(self.to_dict(), indent=2)
 
-    def __eq__(self, other: "ResourceConsumptionLimitsResponse") -> bool:
+    def __eq__(self, other: 'ResourceConsumptionLimitsResponse') -> bool:
         """Return `true` when self and other are equal, false otherwise."""
         if not isinstance(other, self.__class__):
             return False
         return self.__dict__ == other.__dict__
 
-    def __ne__(self, other: "ResourceConsumptionLimitsResponse") -> bool:
+    def __ne__(self, other: 'ResourceConsumptionLimitsResponse') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
 
 class Runtime:
     """
     Runtime enviroment for applications and other workloads.
@@ -3093,48 +3178,48 @@
 
         :param str spark_version: (optional) Spark version of the runtime
                environment.
         """
         self.spark_version = spark_version
 
     @classmethod
-    def from_dict(cls, _dict: Dict) -> "Runtime":
+    def from_dict(cls, _dict: Dict) -> 'Runtime':
         """Initialize a Runtime object from a json dictionary."""
         args = {}
-        if "spark_version" in _dict:
-            args["spark_version"] = _dict.get("spark_version")
+        if 'spark_version' in _dict:
+            args['spark_version'] = _dict.get('spark_version')
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a Runtime object from a json dictionary."""
         return cls.from_dict(_dict)
 
     def to_dict(self) -> Dict:
         """Return a json dictionary representing this model."""
         _dict = {}
-        if hasattr(self, "spark_version") and self.spark_version is not None:
-            _dict["spark_version"] = self.spark_version
+        if hasattr(self, 'spark_version') and self.spark_version is not None:
+            _dict['spark_version'] = self.spark_version
         return _dict
 
     def _to_dict(self):
         """Return a json dictionary representing this model."""
         return self.to_dict()
 
     def __str__(self) -> str:
         """Return a `str` version of this Runtime object."""
         return json.dumps(self.to_dict(), indent=2)
 
-    def __eq__(self, other: "Runtime") -> bool:
+    def __eq__(self, other: 'Runtime') -> bool:
         """Return `true` when self and other are equal, false otherwise."""
         if not isinstance(other, self.__class__):
             return False
         return self.__dict__ == other.__dict__
 
-    def __ne__(self, other: "Runtime") -> bool:
+    def __ne__(self, other: 'Runtime') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
 
 class SparkHistoryServerResponse:
     """
     Status of the Spark history server.
@@ -3155,15 +3240,15 @@
         self,
         *,
         state: str = None,
         cores: str = None,
         memory: str = None,
         start_time: datetime = None,
         stop_time: datetime = None,
-        auto_termination_time: datetime = None
+        auto_termination_time: datetime = None,
     ) -> None:
         """
         Initialize a SparkHistoryServerResponse object.
 
         :param str state: (optional) State of the Spark history server.
         :param str cores: (optional) Number of cpu cores used by the Spark history
                server.
@@ -3180,71 +3265,151 @@
         self.cores = cores
         self.memory = memory
         self.start_time = start_time
         self.stop_time = stop_time
         self.auto_termination_time = auto_termination_time
 
     @classmethod
-    def from_dict(cls, _dict: Dict) -> "SparkHistoryServerResponse":
+    def from_dict(cls, _dict: Dict) -> 'SparkHistoryServerResponse':
         """Initialize a SparkHistoryServerResponse object from a json dictionary."""
         args = {}
-        if "state" in _dict:
-            args["state"] = _dict.get("state")
-        if "cores" in _dict:
-            args["cores"] = _dict.get("cores")
-        if "memory" in _dict:
-            args["memory"] = _dict.get("memory")
-        if "start_time" in _dict:
-            args["start_time"] = string_to_datetime(_dict.get("start_time"))
-        if "stop_time" in _dict:
-            args["stop_time"] = string_to_datetime(_dict.get("stop_time"))
-        if "auto_termination_time" in _dict:
-            args["auto_termination_time"] = string_to_datetime(_dict.get("auto_termination_time"))
+        if 'state' in _dict:
+            args['state'] = _dict.get('state')
+        if 'cores' in _dict:
+            args['cores'] = _dict.get('cores')
+        if 'memory' in _dict:
+            args['memory'] = _dict.get('memory')
+        if 'start_time' in _dict:
+            args['start_time'] = string_to_datetime(_dict.get('start_time'))
+        if 'stop_time' in _dict:
+            args['stop_time'] = string_to_datetime(_dict.get('stop_time'))
+        if 'auto_termination_time' in _dict:
+            args['auto_termination_time'] = string_to_datetime(_dict.get('auto_termination_time'))
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a SparkHistoryServerResponse object from a json dictionary."""
         return cls.from_dict(_dict)
 
     def to_dict(self) -> Dict:
         """Return a json dictionary representing this model."""
         _dict = {}
-        if hasattr(self, "state") and self.state is not None:
-            _dict["state"] = self.state
-        if hasattr(self, "cores") and self.cores is not None:
-            _dict["cores"] = self.cores
-        if hasattr(self, "memory") and self.memory is not None:
-            _dict["memory"] = self.memory
-        if hasattr(self, "start_time") and self.start_time is not None:
-            _dict["start_time"] = datetime_to_string(self.start_time)
-        if hasattr(self, "stop_time") and self.stop_time is not None:
-            _dict["stop_time"] = datetime_to_string(self.stop_time)
-        if hasattr(self, "auto_termination_time") and self.auto_termination_time is not None:
-            _dict["auto_termination_time"] = datetime_to_string(self.auto_termination_time)
+        if hasattr(self, 'state') and self.state is not None:
+            _dict['state'] = self.state
+        if hasattr(self, 'cores') and self.cores is not None:
+            _dict['cores'] = self.cores
+        if hasattr(self, 'memory') and self.memory is not None:
+            _dict['memory'] = self.memory
+        if hasattr(self, 'start_time') and self.start_time is not None:
+            _dict['start_time'] = datetime_to_string(self.start_time)
+        if hasattr(self, 'stop_time') and self.stop_time is not None:
+            _dict['stop_time'] = datetime_to_string(self.stop_time)
+        if hasattr(self, 'auto_termination_time') and self.auto_termination_time is not None:
+            _dict['auto_termination_time'] = datetime_to_string(self.auto_termination_time)
         return _dict
 
     def _to_dict(self):
         """Return a json dictionary representing this model."""
         return self.to_dict()
 
     def __str__(self) -> str:
         """Return a `str` version of this SparkHistoryServerResponse object."""
         return json.dumps(self.to_dict(), indent=2)
 
-    def __eq__(self, other: "SparkHistoryServerResponse") -> bool:
+    def __eq__(self, other: 'SparkHistoryServerResponse') -> bool:
         """Return `true` when self and other are equal, false otherwise."""
         if not isinstance(other, self.__class__):
             return False
         return self.__dict__ == other.__dict__
 
-    def __ne__(self, other: "SparkHistoryServerResponse") -> bool:
+    def __ne__(self, other: 'SparkHistoryServerResponse') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
     class StateEnum(str, Enum):
         """
         State of the Spark history server.
         """
 
-        STARTED = "started"
-        STOPPED = "stopped"
+        STARTED = 'started'
+        STOPPED = 'stopped'
+
+
+##############################################################################
+# Pagers
+##############################################################################
+
+
+class ApplicationsPager:
+    """
+    ApplicationsPager can be used to simplify the use of the "list_applications" method.
+    """
+
+    def __init__(
+        self,
+        *,
+        client: IbmAnalyticsEngineApiV3,
+        instance_id: str,
+        state: List[str] = None,
+        limit: int = None,
+    ) -> None:
+        """
+        Initialize a ApplicationsPager object.
+        :param str instance_id: The identifier of the Analytics Engine instance
+               associated with the Spark application(s).
+        :param List[str] state: (optional) List of Spark application states that
+               will be used to filter the response.
+        :param int limit: (optional) Number of application entries to be included
+               in the response.
+        """
+        self._has_next = True
+        self._client = client
+        self._page_context = {'next': None}
+        self._instance_id = instance_id
+        self._state = state
+        self._limit = limit
+
+    def has_next(self) -> bool:
+        """
+        Returns true if there are potentially more results to be retrieved.
+        """
+        return self._has_next
+
+    def get_next(self) -> List[dict]:
+        """
+        Returns the next page of results.
+        :return: A List[dict], where each element is a dict that represents an instance of Application.
+        :rtype: List[dict]
+        """
+        if not self.has_next():
+            raise StopIteration(message='No more results available')
+
+        result = self._client.list_applications(
+            instance_id=self._instance_id,
+            state=self._state,
+            limit=self._limit,
+            start=self._page_context.get('next'),
+        ).get_result()
+
+        next = None
+        next_page_link = result.get('next')
+        if next_page_link is not None:
+            next = next_page_link.get('start')
+        self._page_context['next'] = next
+        if next is None:
+            self._has_next = False
+
+        return result.get('applications')
+
+    def get_all(self) -> List[dict]:
+        """
+        Returns all results by invoking get_next() repeatedly
+        until all pages of results have been retrieved.
+        :return: A List[dict], where each element is a dict that represents an instance of Application.
+        :rtype: List[dict]
+        """
+        results = []
+        while self.has_next():
+            next_page = self.get_next()
+            results.extend(next_page)
+        return results
```

### Comparing `iaesdk-3.1.0/iaesdk.egg-info/PKG-INFO` & `iaesdk-3.2.0/iaesdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iaesdk
-Version: 3.1.0
+Version: 3.2.0
 Summary: Python client library for IBM Cloud Analytics Engine Services
 Home-page: https://github.com/IBM/ibm-iae-python-sdk
 Author: IBM
 Author-email: surya.penumatcha@ibm.com
 License: Apache 2.0
 Keywords: iaesdk
 Classifier: Programming Language :: Python
@@ -20,15 +20,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Build Status](https://api.travis-ci.com/IBM/ibm-iae-python-sdk.svg?branch=master)](https://app.travis-ci.com/IBM/ibm-iae-python-sdk)
 [![semantic-release](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/semantic-release/semantic-release)
-# IBM Cloud Analytics Engine Python SDK Version 3.1.0
+# IBM Cloud Analytics Engine Python SDK Version 3.2.0
 
 Python client library to interact with various [iaesdk Service APIs](https://cloud.ibm.com/apidocs/ibm-analytics-engine).
 
 ## Table of Contents
 
 - [Overview](#overview)
 - [Prerequisites](#prerequisites)
@@ -67,21 +67,21 @@
 * Python 3.7 or above.
 
 ## Installation
 
 To install, use `pip` or `easy_install`:
 
 ```bash
-pip install --upgrade "iaesdk>=3.1.0"
+pip install --upgrade "iaesdk>=3.2.0"
 ```
 
 or
 
 ```bash
-easy_install --upgrade "iaesdk>=3.1.0"
+easy_install --upgrade "iaesdk>=3.2.0"
 ```
 
 ## Using the SDK
 For general SDK usage information, please see [this link](https://github.com/IBM/ibm-cloud-sdk-common/blob/master/README.md)
 
 In [setting client options programatically](https://github.com/IBM/ibm-cloud-sdk-common/blob/master/README.md#setting-client-options-programmatically) to instantiate the class, provide the following two values:
 1. [IAM API Key](https://cloud.ibm.com/docs/iam?topic=iam-userapikey#create_user_key)
```

### Comparing `iaesdk-3.1.0/setup.py` & `iaesdk-3.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from setuptools import setup
 from setuptools.command.test import test as TestCommand
 import os
 import sys
 import pkg_resources
 
-__version__ = '3.1.0'
+__version__ = '3.2.0'
 PACKAGE_NAME = 'iaesdk'
 PACKAGE_DESC = 'Python client library for IBM Cloud Analytics Engine Services'
 
 with open("requirements.txt") as f:
     install_requires = [str(req) for req in pkg_resources.parse_requirements(f)]
 with open("requirements-dev.txt") as f:
     tests_require = [str(req) for req in pkg_resources.parse_requirements(f)]
```

