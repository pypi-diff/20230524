# Comparing `tmp/sap-business-document-processing-0.3.1.tar.gz` & `tmp/sap-business-document-processing-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sap-business-document-processing-0.3.1.tar", last modified: Thu May  4 09:16:18 2023, max compression
+gzip compressed data, was "sap-business-document-processing-0.3.2.tar", last modified: Wed May 24 11:44:10 2023, max compression
```

## Comparing `sap-business-document-processing-0.3.1.tar` & `sap-business-document-processing-0.3.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:16:18.956980 sap-business-document-processing-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11380 2023-05-04 09:15:53.000000 sap-business-document-processing-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-05-04 09:16:18.956980 sap-business-document-processing-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7814 2023-05-04 09:15:53.000000 sap-business-document-processing-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-04 09:16:06.000000 sap-business-document-processing-0.3.1/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:16:18.952980 sap-business-document-processing-0.3.1/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:16:18.956980 sap-business-document-processing-0.3.1/examples/document_information_extraction_examples/
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-05-04 09:15:53.000000 sap-business-document-processing-0.3.1/examples/document_information_extraction_examples/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-04 09:15:53.000000 sap-business-document-processing-0.3.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:16:18.956980 sap-business-document-processing-0.3.1/sap_business_document_processing/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-04 09:15:53.000000 sap-business-document-processing-0.3.1/sap_business_document_processing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:16:18.956980 sap-business-document-processing-0.3.1/sap_business_document_processing/common/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-04 09:15:53.000000 sap-business-document-processing-0.3.1/sap_business_document_processing/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-04 09:15:53.000000 sap-business-document-processing-0.3.1/sap_business_document_processing/common/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-04 09:15:53.000000 sap-business-document-processing-0.3.1/sap_business_document_processing/common/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-05-04 09:15:53.000000 sap-business-document-processing-0.3.1/sap_business_document_processing/common/http_client_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:16:18.956980 sap-business-document-processing-0.3.1/sap_business_document_processing/document_classification_client/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-04 09:15:53.000000 sap-business-document-processing-0.3.1/sap_business_document_processing/document_classification_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-04 09:15:53.000000 sap-business-document-processing-0.3.1/sap_business_document_processing/document_classification_client/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    27994 2023-05-04 09:15:53.000000 sap-business-document-processing-0.3.1/sap_business_document_processing/document_classification_client/dc_api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:16:18.956980 sap-business-document-processing-0.3.1/sap_business_document_processing/document_information_extraction_client/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-04 09:15:53.000000 sap-business-document-processing-0.3.1/sap_business_document_processing/document_information_extraction_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-04 09:15:53.000000 sap-business-document-processing-0.3.1/sap_business_document_processing/document_information_extraction_client/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    40365 2023-05-04 09:15:53.000000 sap-business-document-processing-0.3.1/sap_business_document_processing/document_information_extraction_client/dox_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-04 09:15:53.000000 sap-business-document-processing-0.3.1/sap_business_document_processing/document_information_extraction_client/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-05-04 09:15:53.000000 sap-business-document-processing-0.3.1/sap_business_document_processing/document_information_extraction_client/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:16:18.956980 sap-business-document-processing-0.3.1/sap_business_document_processing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-05-04 09:16:18.000000 sap-business-document-processing-0.3.1/sap_business_document_processing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-04 09:16:18.000000 sap-business-document-processing-0.3.1/sap_business_document_processing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 09:16:18.000000 sap-business-document-processing-0.3.1/sap_business_document_processing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-04 09:16:18.000000 sap-business-document-processing-0.3.1/sap_business_document_processing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-04 09:16:18.000000 sap-business-document-processing-0.3.1/sap_business_document_processing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-04 09:16:18.960980 sap-business-document-processing-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-04 09:15:53.000000 sap-business-document-processing-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:44:10.542035 sap-business-document-processing-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11380 2023-05-24 11:43:50.000000 sap-business-document-processing-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-05-24 11:44:10.542035 sap-business-document-processing-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7814 2023-05-24 11:43:50.000000 sap-business-document-processing-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-24 11:43:59.000000 sap-business-document-processing-0.3.2/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:44:10.538035 sap-business-document-processing-0.3.2/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:44:10.538035 sap-business-document-processing-0.3.2/examples/document_information_extraction_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-05-24 11:43:50.000000 sap-business-document-processing-0.3.2/examples/document_information_extraction_examples/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-24 11:43:50.000000 sap-business-document-processing-0.3.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:44:10.538035 sap-business-document-processing-0.3.2/sap_business_document_processing/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-24 11:43:50.000000 sap-business-document-processing-0.3.2/sap_business_document_processing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:44:10.538035 sap-business-document-processing-0.3.2/sap_business_document_processing/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-24 11:43:50.000000 sap-business-document-processing-0.3.2/sap_business_document_processing/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-24 11:43:50.000000 sap-business-document-processing-0.3.2/sap_business_document_processing/common/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-24 11:43:50.000000 sap-business-document-processing-0.3.2/sap_business_document_processing/common/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-05-24 11:43:50.000000 sap-business-document-processing-0.3.2/sap_business_document_processing/common/http_client_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:44:10.542035 sap-business-document-processing-0.3.2/sap_business_document_processing/document_classification_client/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-24 11:43:50.000000 sap-business-document-processing-0.3.2/sap_business_document_processing/document_classification_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-24 11:43:50.000000 sap-business-document-processing-0.3.2/sap_business_document_processing/document_classification_client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27994 2023-05-24 11:43:50.000000 sap-business-document-processing-0.3.2/sap_business_document_processing/document_classification_client/dc_api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:44:10.542035 sap-business-document-processing-0.3.2/sap_business_document_processing/document_information_extraction_client/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-24 11:43:50.000000 sap-business-document-processing-0.3.2/sap_business_document_processing/document_information_extraction_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-24 11:43:50.000000 sap-business-document-processing-0.3.2/sap_business_document_processing/document_information_extraction_client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40365 2023-05-24 11:43:50.000000 sap-business-document-processing-0.3.2/sap_business_document_processing/document_information_extraction_client/dox_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-24 11:43:50.000000 sap-business-document-processing-0.3.2/sap_business_document_processing/document_information_extraction_client/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-05-24 11:43:50.000000 sap-business-document-processing-0.3.2/sap_business_document_processing/document_information_extraction_client/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:44:10.538035 sap-business-document-processing-0.3.2/sap_business_document_processing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-05-24 11:44:10.000000 sap-business-document-processing-0.3.2/sap_business_document_processing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-24 11:44:10.000000 sap-business-document-processing-0.3.2/sap_business_document_processing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 11:44:10.000000 sap-business-document-processing-0.3.2/sap_business_document_processing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-24 11:44:10.000000 sap-business-document-processing-0.3.2/sap_business_document_processing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-24 11:44:10.000000 sap-business-document-processing-0.3.2/sap_business_document_processing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-24 11:44:10.542035 sap-business-document-processing-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-24 11:43:50.000000 sap-business-document-processing-0.3.2/setup.py
```

### Comparing `sap-business-document-processing-0.3.1/LICENSE` & `sap-business-document-processing-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sap-business-document-processing-0.3.1/PKG-INFO` & `sap-business-document-processing-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sap-business-document-processing
-Version: 0.3.1
+Version: 0.3.2
 Summary: Python client library for convenient usage of SAP Business Document Processing services
 Home-page: https://github.com/sap/business-document-processing
 Download-URL: https://pypi.org/project/sap-business-document-processing
 Author: Alexander Bolshakov
 Author-email: alexander.bolshakov@sap.com
 License: apache-2.0
 Keywords: SAP,business,document,processing,classification,information,extraction,machine learning
```

### Comparing `sap-business-document-processing-0.3.1/README.md` & `sap-business-document-processing-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `sap-business-document-processing-0.3.1/examples/document_information_extraction_examples/utils.py` & `sap-business-document-processing-0.3.2/examples/document_information_extraction_examples/utils.py`

 * *Files identical despite different names*

### Comparing `sap-business-document-processing-0.3.1/sap_business_document_processing/common/exceptions.py` & `sap-business-document-processing-0.3.2/sap_business_document_processing/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `sap-business-document-processing-0.3.1/sap_business_document_processing/common/helpers.py` & `sap-business-document-processing-0.3.2/sap_business_document_processing/common/helpers.py`

 * *Files identical despite different names*

### Comparing `sap-business-document-processing-0.3.1/sap_business_document_processing/common/http_client_base.py` & `sap-business-document-processing-0.3.2/sap_business_document_processing/common/http_client_base.py`

 * *Files identical despite different names*

### Comparing `sap-business-document-processing-0.3.1/sap_business_document_processing/document_classification_client/constants.py` & `sap-business-document-processing-0.3.2/sap_business_document_processing/document_classification_client/constants.py`

 * *Files identical despite different names*

### Comparing `sap-business-document-processing-0.3.1/sap_business_document_processing/document_classification_client/dc_api_client.py` & `sap-business-document-processing-0.3.2/sap_business_document_processing/document_classification_client/dc_api_client.py`

 * *Files identical despite different names*

### Comparing `sap-business-document-processing-0.3.1/sap_business_document_processing/document_information_extraction_client/constants.py` & `sap-business-document-processing-0.3.2/sap_business_document_processing/document_information_extraction_client/constants.py`

 * *Files identical despite different names*

### Comparing `sap-business-document-processing-0.3.1/sap_business_document_processing/document_information_extraction_client/dox_api_client.py` & `sap-business-document-processing-0.3.2/sap_business_document_processing/document_information_extraction_client/dox_api_client.py`

 * *Files identical despite different names*

### Comparing `sap-business-document-processing-0.3.1/sap_business_document_processing/document_information_extraction_client/endpoints.py` & `sap-business-document-processing-0.3.2/sap_business_document_processing/document_information_extraction_client/endpoints.py`

 * *Files identical despite different names*

### Comparing `sap-business-document-processing-0.3.1/sap_business_document_processing/document_information_extraction_client/helpers.py` & `sap-business-document-processing-0.3.2/sap_business_document_processing/document_information_extraction_client/helpers.py`

 * *Files identical despite different names*

### Comparing `sap-business-document-processing-0.3.1/sap_business_document_processing.egg-info/PKG-INFO` & `sap-business-document-processing-0.3.2/sap_business_document_processing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sap-business-document-processing
-Version: 0.3.1
+Version: 0.3.2
 Summary: Python client library for convenient usage of SAP Business Document Processing services
 Home-page: https://github.com/sap/business-document-processing
 Download-URL: https://pypi.org/project/sap-business-document-processing
 Author: Alexander Bolshakov
 Author-email: alexander.bolshakov@sap.com
 License: apache-2.0
 Keywords: SAP,business,document,processing,classification,information,extraction,machine learning
```

### Comparing `sap-business-document-processing-0.3.1/sap_business_document_processing.egg-info/SOURCES.txt` & `sap-business-document-processing-0.3.2/sap_business_document_processing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sap-business-document-processing-0.3.1/setup.cfg` & `sap-business-document-processing-0.3.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3
 
 [options]
 packages = find_namespace:
 include_package_data = True
 install_requires = 
-	urllib3 ~= 1.26.0
-	requests ~= 2.29.0
-	requests_oauthlib ~= 1.3.0
+	urllib3 ~= 1.26
+	requests ~= 2.31
+	requests_oauthlib ~= 1.3
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

