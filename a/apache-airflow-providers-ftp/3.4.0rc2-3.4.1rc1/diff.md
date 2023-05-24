# Comparing `tmp/apache-airflow-providers-ftp-3.4.0rc2.tar.gz` & `tmp/apache-airflow-providers-ftp-3.4.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-ftp-3.4.0rc2.tar", last modified: Fri May 19 17:52:25 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-ftp-3.4.1rc1.tar", last modified: Wed May 24 07:20:26 2023, max compression
```

## Comparing `apache-airflow-providers-ftp-3.4.0rc2.tar` & `apache-airflow-providers-ftp-3.4.1rc1.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:25.000000 apache-airflow-providers-ftp-3.4.0rc2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-ftp-3.4.0rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-19 17:52:24.000000 apache-airflow-providers-ftp-3.4.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-ftp-3.4.0rc2/NOTICE
--rw-r--r--   0 root         (0) root         (0)     9604 2023-05-19 17:52:25.000000 apache-airflow-providers-ftp-3.4.0rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8086 2023-05-19 17:52:24.000000 apache-airflow-providers-ftp-3.4.0rc2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:25.000000 apache-airflow-providers-ftp-3.4.0rc2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:25.000000 apache-airflow-providers-ftp-3.4.0rc2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:25.000000 apache-airflow-providers-ftp-3.4.0rc2/airflow/providers/ftp/
--rw-r--r--   0 root         (0) root         (0)     1528 2023-05-19 12:06:30.000000 apache-airflow-providers-ftp-3.4.0rc2/airflow/providers/ftp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2700 2023-05-19 17:52:24.000000 apache-airflow-providers-ftp-3.4.0rc2/airflow/providers/ftp/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:25.000000 apache-airflow-providers-ftp-3.4.0rc2/airflow/providers/ftp/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-ftp-3.4.0rc2/airflow/providers/ftp/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9842 2023-02-24 18:43:53.000000 apache-airflow-providers-ftp-3.4.0rc2/airflow/providers/ftp/hooks/ftp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:25.000000 apache-airflow-providers-ftp-3.4.0rc2/airflow/providers/ftp/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-ftp-3.4.0rc2/airflow/providers/ftp/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6093 2023-02-24 18:43:53.000000 apache-airflow-providers-ftp-3.4.0rc2/airflow/providers/ftp/operators/ftp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:25.000000 apache-airflow-providers-ftp-3.4.0rc2/airflow/providers/ftp/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-ftp-3.4.0rc2/airflow/providers/ftp/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3363 2023-02-24 18:43:53.000000 apache-airflow-providers-ftp-3.4.0rc2/airflow/providers/ftp/sensors/ftp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:25.000000 apache-airflow-providers-ftp-3.4.0rc2/apache_airflow_providers_ftp.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9604 2023-05-19 17:52:25.000000 apache-airflow-providers-ftp-3.4.0rc2/apache_airflow_providers_ftp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      699 2023-05-19 17:52:25.000000 apache-airflow-providers-ftp-3.4.0rc2/apache_airflow_providers_ftp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:52:25.000000 apache-airflow-providers-ftp-3.4.0rc2/apache_airflow_providers_ftp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      100 2023-05-19 17:52:25.000000 apache-airflow-providers-ftp-3.4.0rc2/apache_airflow_providers_ftp.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:52:25.000000 apache-airflow-providers-ftp-3.4.0rc2/apache_airflow_providers_ftp.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:52:25.000000 apache-airflow-providers-ftp-3.4.0rc2/apache_airflow_providers_ftp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-ftp-3.4.0rc2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1782 2023-05-19 17:52:25.000000 apache-airflow-providers-ftp-3.4.0rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1620 2023-05-19 17:52:24.000000 apache-airflow-providers-ftp-3.4.0rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:26.000000 apache-airflow-providers-ftp-3.4.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-05-23 11:35:15.000000 apache-airflow-providers-ftp-3.4.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-24 07:20:25.000000 apache-airflow-providers-ftp-3.4.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-05-23 11:35:15.000000 apache-airflow-providers-ftp-3.4.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     9972 2023-05-24 07:20:26.000000 apache-airflow-providers-ftp-3.4.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8403 2023-05-24 07:20:25.000000 apache-airflow-providers-ftp-3.4.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:26.000000 apache-airflow-providers-ftp-3.4.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:26.000000 apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:26.000000 apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/ftp/
+-rw-r--r--   0 root         (0) root         (0)     1528 2023-05-24 07:09:22.000000 apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/ftp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2744 2023-05-24 07:20:25.000000 apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/ftp/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:26.000000 apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/ftp/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-05-23 11:35:14.000000 apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/ftp/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9842 2023-05-23 11:35:14.000000 apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/ftp/hooks/ftp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:26.000000 apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/ftp/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-05-23 11:35:14.000000 apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/ftp/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6093 2023-05-23 11:35:14.000000 apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/ftp/operators/ftp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:26.000000 apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/ftp/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-05-23 11:35:14.000000 apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/ftp/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3363 2023-05-23 11:35:14.000000 apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/ftp/sensors/ftp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:26.000000 apache-airflow-providers-ftp-3.4.1rc1/apache_airflow_providers_ftp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9972 2023-05-24 07:20:26.000000 apache-airflow-providers-ftp-3.4.1rc1/apache_airflow_providers_ftp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      750 2023-05-24 07:20:26.000000 apache-airflow-providers-ftp-3.4.1rc1/apache_airflow_providers_ftp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 07:20:26.000000 apache-airflow-providers-ftp-3.4.1rc1/apache_airflow_providers_ftp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      100 2023-05-24 07:20:26.000000 apache-airflow-providers-ftp-3.4.1rc1/apache_airflow_providers_ftp.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 07:20:26.000000 apache-airflow-providers-ftp-3.4.1rc1/apache_airflow_providers_ftp.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       27 2023-05-24 07:20:26.000000 apache-airflow-providers-ftp-3.4.1rc1/apache_airflow_providers_ftp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-24 07:20:26.000000 apache-airflow-providers-ftp-3.4.1rc1/apache_airflow_providers_ftp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5338 2023-05-23 11:35:15.000000 apache-airflow-providers-ftp-3.4.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1850 2023-05-24 07:20:26.000000 apache-airflow-providers-ftp-3.4.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1620 2023-05-24 07:20:25.000000 apache-airflow-providers-ftp-3.4.1rc1/setup.py
```

### Comparing `apache-airflow-providers-ftp-3.4.0rc2/LICENSE` & `apache-airflow-providers-ftp-3.4.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.4.0rc2/MANIFEST.in` & `apache-airflow-providers-ftp-3.4.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.4.0rc2/PKG-INFO` & `apache-airflow-providers-ftp-3.4.1rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-ftp
-Version: 3.4.0rc2
+Version: 3.4.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-ftp package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-ftp/3.4.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-ftp/3.4.1/
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -21,14 +21,15 @@
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Monitoring
 Requires-Python: ~=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: NOTICE
 
 
@@ -48,38 +49,47 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-ftp``
 
-Release: ``3.4.0rc2``
+Release: ``3.4.1rc1``
 
 
 `File Transfer Protocol (FTP) <https://tools.ietf.org/html/rfc114>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``ftp`` provider. All classes for this provider package
 are in ``airflow.providers.ftp`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-ftp/3.4.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-ftp/3.4.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-ftp``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.7,3.8,3.9,3.10,3.11
+
+Requirements
+------------
+
+==================  ==================
+PIP package         Version required
+==================  ==================
+``apache-airflow``  ``>=2.4.0``
+==================  ==================
 
  .. Licensed to the Apache Software Foundation (ASF) under one
     or more contributor license agreements.  See the NOTICE file
     distributed with this work for additional information
     regarding copyright ownership.  The ASF licenses this file
     to you under the Apache License, Version 2.0 (the
     "License"); you may not use this file except in compliance
@@ -99,14 +109,22 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.4.1
+.....
+
+Misc
+~~~~
+
+* ``Bring back min-airflow-version for preinstalled providers (#31469)``
+
 3.4.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-ftp-3.4.0rc2/README.rst` & `apache-airflow-providers-ftp-3.4.1rc1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -15,38 +15,47 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-ftp``
 
-Release: ``3.4.0rc2``
+Release: ``3.4.1rc1``
 
 
 `File Transfer Protocol (FTP) <https://tools.ietf.org/html/rfc114>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``ftp`` provider. All classes for this provider package
 are in ``airflow.providers.ftp`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-ftp/3.4.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-ftp/3.4.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-ftp``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.7,3.8,3.9,3.10,3.11
+
+Requirements
+------------
+
+==================  ==================
+PIP package         Version required
+==================  ==================
+``apache-airflow``  ``>=2.4.0``
+==================  ==================
 
  .. Licensed to the Apache Software Foundation (ASF) under one
     or more contributor license agreements.  See the NOTICE file
     distributed with this work for additional information
     regarding copyright ownership.  The ASF licenses this file
     to you under the Apache License, Version 2.0 (the
     "License"); you may not use this file except in compliance
@@ -66,14 +75,22 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.4.1
+.....
+
+Misc
+~~~~
+
+* ``Bring back min-airflow-version for preinstalled providers (#31469)``
+
 3.4.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-ftp-3.4.0rc2/airflow/providers/ftp/__init__.py` & `apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/ftp/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "3.4.0"
+__version__ = "3.4.1"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
```

### Comparing `apache-airflow-providers-ftp-3.4.0rc2/airflow/providers/ftp/get_provider_info.py` & `apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/ftp/get_provider_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-ftp",
         "name": "File Transfer Protocol (FTP)",
         "description": "`File Transfer Protocol (FTP) <https://tools.ietf.org/html/rfc114>`__\n",
         "suspended": False,
         "versions": [
+            "3.4.1",
             "3.4.0",
             "3.3.1",
             "3.3.0",
             "3.2.0",
             "3.1.0",
             "3.0.0",
             "2.1.2",
@@ -40,15 +41,15 @@
             "2.1.0",
             "2.0.1",
             "2.0.0",
             "1.1.0",
             "1.0.1",
             "1.0.0",
         ],
-        "dependencies": [],
+        "dependencies": ["apache-airflow>=2.4.0"],
         "integrations": [
             {
                 "integration-name": "File Transfer Protocol (FTP)",
                 "external-doc-url": "https://tools.ietf.org/html/rfc114",
                 "logo": "/integration-logos/ftp/FTP.png",
                 "tags": ["protocol"],
             }
```

### Comparing `apache-airflow-providers-ftp-3.4.0rc2/airflow/providers/ftp/hooks/__init__.py` & `apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/ftp/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.4.0rc2/airflow/providers/ftp/hooks/ftp.py` & `apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/ftp/hooks/ftp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.4.0rc2/airflow/providers/ftp/operators/__init__.py` & `apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/ftp/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.4.0rc2/airflow/providers/ftp/operators/ftp.py` & `apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/ftp/operators/ftp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.4.0rc2/airflow/providers/ftp/sensors/__init__.py` & `apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/ftp/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.4.0rc2/airflow/providers/ftp/sensors/ftp.py` & `apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/ftp/sensors/ftp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.4.0rc2/apache_airflow_providers_ftp.egg-info/PKG-INFO` & `apache-airflow-providers-ftp-3.4.1rc1/apache_airflow_providers_ftp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-ftp
-Version: 3.4.0rc2
+Version: 3.4.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-ftp package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-ftp/3.4.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-ftp/3.4.1/
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -21,14 +21,15 @@
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Monitoring
 Requires-Python: ~=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: NOTICE
 
 
@@ -48,38 +49,47 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-ftp``
 
-Release: ``3.4.0rc2``
+Release: ``3.4.1rc1``
 
 
 `File Transfer Protocol (FTP) <https://tools.ietf.org/html/rfc114>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``ftp`` provider. All classes for this provider package
 are in ``airflow.providers.ftp`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-ftp/3.4.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-ftp/3.4.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-ftp``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.7,3.8,3.9,3.10,3.11
+
+Requirements
+------------
+
+==================  ==================
+PIP package         Version required
+==================  ==================
+``apache-airflow``  ``>=2.4.0``
+==================  ==================
 
  .. Licensed to the Apache Software Foundation (ASF) under one
     or more contributor license agreements.  See the NOTICE file
     distributed with this work for additional information
     regarding copyright ownership.  The ASF licenses this file
     to you under the Apache License, Version 2.0 (the
     "License"); you may not use this file except in compliance
@@ -99,14 +109,22 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.4.1
+.....
+
+Misc
+~~~~
+
+* ``Bring back min-airflow-version for preinstalled providers (#31469)``
+
 3.4.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-ftp-3.4.0rc2/apache_airflow_providers_ftp.egg-info/SOURCES.txt` & `apache-airflow-providers-ftp-3.4.1rc1/apache_airflow_providers_ftp.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -14,8 +14,9 @@
 airflow/providers/ftp/sensors/__init__.py
 airflow/providers/ftp/sensors/ftp.py
 apache_airflow_providers_ftp.egg-info/PKG-INFO
 apache_airflow_providers_ftp.egg-info/SOURCES.txt
 apache_airflow_providers_ftp.egg-info/dependency_links.txt
 apache_airflow_providers_ftp.egg-info/entry_points.txt
 apache_airflow_providers_ftp.egg-info/not-zip-safe
+apache_airflow_providers_ftp.egg-info/requires.txt
 apache_airflow_providers_ftp.egg-info/top_level.txt
```

### Comparing `apache-airflow-providers-ftp-3.4.0rc2/pyproject.toml` & `apache-airflow-providers-ftp-3.4.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.4.0rc2/setup.cfg` & `apache-airflow-providers-ftp-3.4.1rc1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -21,17 +21,18 @@
 	Framework :: Apache Airflow
 	Framework :: Apache Airflow :: Provider
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-ftp/3.4.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-ftp/3.4.1/
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
@@ -42,19 +43,20 @@
 include_package_data = True
 python_requires = ~=3.7
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
+	apache-airflow>=2.4.0.dev0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.ftp.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.ftp
 
 [egg_info]
-tag_build = rc2
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-ftp-3.4.0rc2/setup.py` & `apache-airflow-providers-ftp-3.4.1rc1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-ftp package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "3.4.0"
+version = "3.4.1"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-ftp setup."""
     setup(
         version=version,
         extras_require={},
```

