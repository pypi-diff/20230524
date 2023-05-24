# Comparing `tmp/cp-mgmt-api-sdk-1.5.0.tar.gz` & `tmp/cp-mgmt-api-sdk-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cp-mgmt-api-sdk-1.5.0.tar", last modified: Thu Jul 28 07:56:56 2022, max compression
+gzip compressed data, was "cp-mgmt-api-sdk-1.6.0.tar", last modified: Thu Oct  6 13:27:36 2022, max compression
```

## Comparing `cp-mgmt-api-sdk-1.5.0.tar` & `cp-mgmt-api-sdk-1.6.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 07:56:56.575208 cp-mgmt-api-sdk-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-07-28 07:56:42.000000 cp-mgmt-api-sdk-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      760 2022-07-28 07:56:56.575208 cp-mgmt-api-sdk-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2480 2022-07-28 07:56:42.000000 cp-mgmt-api-sdk-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 07:56:56.575208 cp-mgmt-api-sdk-1.5.0/cp_mgmt_api_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      760 2022-07-28 07:56:56.000000 cp-mgmt-api-sdk-1.5.0/cp_mgmt_api_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      292 2022-07-28 07:56:56.000000 cp-mgmt-api-sdk-1.5.0/cp_mgmt_api_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-28 07:56:56.000000 cp-mgmt-api-sdk-1.5.0/cp_mgmt_api_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-07-28 07:56:56.000000 cp-mgmt-api-sdk-1.5.0/cp_mgmt_api_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 07:56:56.575208 cp-mgmt-api-sdk-1.5.0/cpapi/
--rw-r--r--   0 runner    (1001) docker     (121)      194 2022-07-28 07:56:42.000000 cp-mgmt-api-sdk-1.5.0/cpapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      527 2022-07-28 07:56:42.000000 cp-mgmt-api-sdk-1.5.0/cpapi/api_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     3846 2022-07-28 07:56:42.000000 cp-mgmt-api-sdk-1.5.0/cpapi/api_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12052 2022-07-28 07:56:42.000000 cp-mgmt-api-sdk-1.5.0/cpapi/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)    35813 2022-07-28 07:56:42.000000 cp-mgmt-api-sdk-1.5.0/cpapi/mgmt_api.py
--rw-r--r--   0 runner    (1001) docker     (121)      595 2022-07-28 07:56:42.000000 cp-mgmt-api-sdk-1.5.0/cpapi/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-28 07:56:56.575208 cp-mgmt-api-sdk-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1010 2022-07-28 07:56:42.000000 cp-mgmt-api-sdk-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 13:27:36.645695 cp-mgmt-api-sdk-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-10-06 13:27:23.000000 cp-mgmt-api-sdk-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      760 2022-10-06 13:27:36.645695 cp-mgmt-api-sdk-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2580 2022-10-06 13:27:23.000000 cp-mgmt-api-sdk-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 13:27:36.641694 cp-mgmt-api-sdk-1.6.0/cp_mgmt_api_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      760 2022-10-06 13:27:36.000000 cp-mgmt-api-sdk-1.6.0/cp_mgmt_api_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      292 2022-10-06 13:27:36.000000 cp-mgmt-api-sdk-1.6.0/cp_mgmt_api_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-06 13:27:36.000000 cp-mgmt-api-sdk-1.6.0/cp_mgmt_api_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2022-10-06 13:27:36.000000 cp-mgmt-api-sdk-1.6.0/cp_mgmt_api_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 13:27:36.645695 cp-mgmt-api-sdk-1.6.0/cpapi/
+-rw-r--r--   0 runner    (1001) docker     (121)      194 2022-10-06 13:27:23.000000 cp-mgmt-api-sdk-1.6.0/cpapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      527 2022-10-06 13:27:23.000000 cp-mgmt-api-sdk-1.6.0/cpapi/api_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3846 2022-10-06 13:27:23.000000 cp-mgmt-api-sdk-1.6.0/cpapi/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12052 2022-10-06 13:27:23.000000 cp-mgmt-api-sdk-1.6.0/cpapi/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)    35839 2022-10-06 13:27:23.000000 cp-mgmt-api-sdk-1.6.0/cpapi/mgmt_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)      595 2022-10-06 13:27:23.000000 cp-mgmt-api-sdk-1.6.0/cpapi/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-06 13:27:36.645695 cp-mgmt-api-sdk-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1010 2022-10-06 13:27:23.000000 cp-mgmt-api-sdk-1.6.0/setup.py
```

### Comparing `cp-mgmt-api-sdk-1.5.0/LICENSE` & `cp-mgmt-api-sdk-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cp-mgmt-api-sdk-1.5.0/PKG-INFO` & `cp-mgmt-api-sdk-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cp-mgmt-api-sdk
-Version: 1.5.0
+Version: 1.6.0
 Summary: Check Point Management API SDK
 Home-page: https://github.com/CheckPointSW/cp_mgmt_api_python_sdk.git
 Author: API team
 Author-email: api_team@checkpoint.com
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cp-mgmt-api-sdk-1.5.0/README.md` & `cp-mgmt-api-sdk-1.6.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -62,10 +62,11 @@
 
 Configure your environment variables
 ```
 export PYTHONPATH=$PYTHONPATH:<“CP-SDK” FULL PATH>
 ```
 For example, if you copied the SDK to the path “/home/admin/” the command will be: <br>
 ```export PYTHONPATH=$PYTHONPATH:/home/admin/cp_mgmt_api_python_sdk/```
+###### Note: When downloading the repository, directory name will be cp_mgmt_api_python_sdk-master.
 
 ## Development Environment
 The kit is developed using Python versions 2.7 and 3.7
```

### Comparing `cp-mgmt-api-sdk-1.5.0/cp_mgmt_api_sdk.egg-info/PKG-INFO` & `cp-mgmt-api-sdk-1.6.0/cp_mgmt_api_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cp-mgmt-api-sdk
-Version: 1.5.0
+Version: 1.6.0
 Summary: Check Point Management API SDK
 Home-page: https://github.com/CheckPointSW/cp_mgmt_api_python_sdk.git
 Author: API team
 Author-email: api_team@checkpoint.com
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cp-mgmt-api-sdk-1.5.0/cpapi/api_exceptions.py` & `cp-mgmt-api-sdk-1.6.0/cpapi/api_exceptions.py`

 * *Files identical despite different names*

### Comparing `cp-mgmt-api-sdk-1.5.0/cpapi/api_response.py` & `cp-mgmt-api-sdk-1.6.0/cpapi/api_response.py`

 * *Files identical despite different names*

### Comparing `cp-mgmt-api-sdk-1.5.0/cpapi/cli.py` & `cp-mgmt-api-sdk-1.6.0/cpapi/cli.py`

 * *Files identical despite different names*

### Comparing `cp-mgmt-api-sdk-1.5.0/cpapi/mgmt_api.py` & `cp-mgmt-api-sdk-1.6.0/cpapi/mgmt_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -345,15 +345,15 @@
             if err.args[0] == "Fingerprint value mismatch":
                 err_message = "Error: Fingerprint value mismatch:\n" + " Expecting : {}\n".format(
                     err.args[1]) + " Got: {}\n".format(
                     err.args[2]) + "If you trust the new fingerprint, edit the 'fingerprints.txt' file."
                 res = APIResponse("", False, err_message=err_message)
             else:
                 res = APIResponse("", False, err_message=err)
-        except (http_client.CannotSendRequest, http_client.BadStatusLine, ConnectionAbortedError) as e:
+        except (http_client.CannotSendRequest, http_client.BadStatusLine, ConnectionAbortedError, BrokenPipeError, IOError) as e:
             self.conn = self.create_https_connection()
             self.conn.request("POST", url, _data, _headers)
             response = self.conn.getresponse()
             res = APIResponse.from_http_response(response)
         except Exception as err:
             res = APIResponse("", False, err_message=err)
         finally:
```

### Comparing `cp-mgmt-api-sdk-1.5.0/cpapi/utils.py` & `cp-mgmt-api-sdk-1.6.0/cpapi/utils.py`

 * *Files identical despite different names*

### Comparing `cp-mgmt-api-sdk-1.5.0/setup.py` & `cp-mgmt-api-sdk-1.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 from setuptools import setup
 
 setup(
     name="cp-mgmt-api-sdk",
-    version="1.5.0",
+    version="1.6.0",
     author="API team",
     author_email="api_team@checkpoint.com",
     license='Apache 2.0',
     description="Check Point Management API SDK",
     long_description="Check Point API Python Development Kit simplifies the usage of the Check Point Management APIs. "
                      "The kit contains the API library project, "
                      "and sample projects demonstrating the capabilities of the library. "
```

