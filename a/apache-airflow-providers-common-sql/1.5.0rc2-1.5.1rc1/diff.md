# Comparing `tmp/apache-airflow-providers-common-sql-1.5.0rc2.tar.gz` & `tmp/apache-airflow-providers-common-sql-1.5.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-common-sql-1.5.0rc2.tar", last modified: Fri May 19 17:52:07 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-common-sql-1.5.1rc1.tar", last modified: Wed May 24 07:20:32 2023, max compression
```

## Comparing `apache-airflow-providers-common-sql-1.5.0rc2.tar` & `apache-airflow-providers-common-sql-1.5.1rc1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:07.000000 apache-airflow-providers-common-sql-1.5.0rc2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-common-sql-1.5.0rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-19 17:52:06.000000 apache-airflow-providers-common-sql-1.5.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-common-sql-1.5.0rc2/NOTICE
--rw-r--r--   0 root         (0) root         (0)    10376 2023-05-19 17:52:07.000000 apache-airflow-providers-common-sql-1.5.0rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8814 2023-05-19 17:52:06.000000 apache-airflow-providers-common-sql-1.5.0rc2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:07.000000 apache-airflow-providers-common-sql-1.5.0rc2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:07.000000 apache-airflow-providers-common-sql-1.5.0rc2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:07.000000 apache-airflow-providers-common-sql-1.5.0rc2/airflow/providers/common/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:07.000000 apache-airflow-providers-common-sql-1.5.0rc2/airflow/providers/common/sql/
--rw-r--r--   0 root         (0) root         (0)     1535 2023-05-19 12:04:34.000000 apache-airflow-providers-common-sql-1.5.0rc2/airflow/providers/common/sql/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2511 2023-05-19 17:52:06.000000 apache-airflow-providers-common-sql-1.5.0rc2/airflow/providers/common/sql/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:07.000000 apache-airflow-providers-common-sql-1.5.0rc2/airflow/providers/common/sql/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-common-sql-1.5.0rc2/airflow/providers/common/sql/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21739 2023-03-06 20:52:28.000000 apache-airflow-providers-common-sql-1.5.0rc2/airflow/providers/common/sql/hooks/sql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:07.000000 apache-airflow-providers-common-sql-1.5.0rc2/airflow/providers/common/sql/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-common-sql-1.5.0rc2/airflow/providers/common/sql/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44516 2023-05-12 08:38:07.000000 apache-airflow-providers-common-sql-1.5.0rc2/airflow/providers/common/sql/operators/sql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:07.000000 apache-airflow-providers-common-sql-1.5.0rc2/airflow/providers/common/sql/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-common-sql-1.5.0rc2/airflow/providers/common/sql/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4691 2023-02-24 18:43:53.000000 apache-airflow-providers-common-sql-1.5.0rc2/airflow/providers/common/sql/sensors/sql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:07.000000 apache-airflow-providers-common-sql-1.5.0rc2/apache_airflow_providers_common_sql.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10376 2023-05-19 17:52:07.000000 apache-airflow-providers-common-sql-1.5.0rc2/apache_airflow_providers_common_sql.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      855 2023-05-19 17:52:07.000000 apache-airflow-providers-common-sql-1.5.0rc2/apache_airflow_providers_common_sql.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:52:07.000000 apache-airflow-providers-common-sql-1.5.0rc2/apache_airflow_providers_common_sql.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-05-19 17:52:07.000000 apache-airflow-providers-common-sql-1.5.0rc2/apache_airflow_providers_common_sql.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:52:07.000000 apache-airflow-providers-common-sql-1.5.0rc2/apache_airflow_providers_common_sql.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       41 2023-05-19 17:52:07.000000 apache-airflow-providers-common-sql-1.5.0rc2/apache_airflow_providers_common_sql.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:52:07.000000 apache-airflow-providers-common-sql-1.5.0rc2/apache_airflow_providers_common_sql.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-common-sql-1.5.0rc2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1841 2023-05-19 17:52:07.000000 apache-airflow-providers-common-sql-1.5.0rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1690 2023-05-19 17:52:06.000000 apache-airflow-providers-common-sql-1.5.0rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:32.000000 apache-airflow-providers-common-sql-1.5.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-05-23 11:35:15.000000 apache-airflow-providers-common-sql-1.5.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-24 07:20:31.000000 apache-airflow-providers-common-sql-1.5.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-05-23 11:35:15.000000 apache-airflow-providers-common-sql-1.5.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    10587 2023-05-24 07:20:32.000000 apache-airflow-providers-common-sql-1.5.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8974 2023-05-24 07:20:31.000000 apache-airflow-providers-common-sql-1.5.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:32.000000 apache-airflow-providers-common-sql-1.5.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:32.000000 apache-airflow-providers-common-sql-1.5.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:32.000000 apache-airflow-providers-common-sql-1.5.1rc1/airflow/providers/common/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:32.000000 apache-airflow-providers-common-sql-1.5.1rc1/airflow/providers/common/sql/
+-rw-r--r--   0 root         (0) root         (0)     1535 2023-05-24 07:09:22.000000 apache-airflow-providers-common-sql-1.5.1rc1/airflow/providers/common/sql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2557 2023-05-24 07:20:31.000000 apache-airflow-providers-common-sql-1.5.1rc1/airflow/providers/common/sql/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:32.000000 apache-airflow-providers-common-sql-1.5.1rc1/airflow/providers/common/sql/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-05-23 11:35:14.000000 apache-airflow-providers-common-sql-1.5.1rc1/airflow/providers/common/sql/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21739 2023-05-23 11:35:14.000000 apache-airflow-providers-common-sql-1.5.1rc1/airflow/providers/common/sql/hooks/sql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:32.000000 apache-airflow-providers-common-sql-1.5.1rc1/airflow/providers/common/sql/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-05-23 11:35:14.000000 apache-airflow-providers-common-sql-1.5.1rc1/airflow/providers/common/sql/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44516 2023-05-23 11:35:14.000000 apache-airflow-providers-common-sql-1.5.1rc1/airflow/providers/common/sql/operators/sql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:32.000000 apache-airflow-providers-common-sql-1.5.1rc1/airflow/providers/common/sql/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-05-23 11:35:14.000000 apache-airflow-providers-common-sql-1.5.1rc1/airflow/providers/common/sql/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4691 2023-05-23 11:35:14.000000 apache-airflow-providers-common-sql-1.5.1rc1/airflow/providers/common/sql/sensors/sql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:32.000000 apache-airflow-providers-common-sql-1.5.1rc1/apache_airflow_providers_common_sql.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10587 2023-05-24 07:20:32.000000 apache-airflow-providers-common-sql-1.5.1rc1/apache_airflow_providers_common_sql.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      855 2023-05-24 07:20:32.000000 apache-airflow-providers-common-sql-1.5.1rc1/apache_airflow_providers_common_sql.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 07:20:32.000000 apache-airflow-providers-common-sql-1.5.1rc1/apache_airflow_providers_common_sql.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-05-24 07:20:32.000000 apache-airflow-providers-common-sql-1.5.1rc1/apache_airflow_providers_common_sql.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 07:20:32.000000 apache-airflow-providers-common-sql-1.5.1rc1/apache_airflow_providers_common_sql.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       68 2023-05-24 07:20:32.000000 apache-airflow-providers-common-sql-1.5.1rc1/apache_airflow_providers_common_sql.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-24 07:20:32.000000 apache-airflow-providers-common-sql-1.5.1rc1/apache_airflow_providers_common_sql.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5338 2023-05-23 11:35:15.000000 apache-airflow-providers-common-sql-1.5.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1909 2023-05-24 07:20:32.000000 apache-airflow-providers-common-sql-1.5.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1690 2023-05-24 07:20:31.000000 apache-airflow-providers-common-sql-1.5.1rc1/setup.py
```

### Comparing `apache-airflow-providers-common-sql-1.5.0rc2/LICENSE` & `apache-airflow-providers-common-sql-1.5.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.5.0rc2/MANIFEST.in` & `apache-airflow-providers-common-sql-1.5.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.5.0rc2/PKG-INFO` & `apache-airflow-providers-common-sql-1.5.1rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-common-sql
-Version: 1.5.0rc2
+Version: 1.5.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-common-sql package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.5.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.5.1/
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
 Provides-Extra: pandas
 License-File: LICENSE
 License-File: NOTICE
 
@@ -49,47 +50,48 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-common-sql``
 
-Release: ``1.5.0rc2``
+Release: ``1.5.1rc1``
 
 
 `Common SQL Provider <https://en.wikipedia.org/wiki/SQL>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``common.sql`` provider. All classes for this provider package
 are in ``airflow.providers.common.sql`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.5.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.5.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-common-sql``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.7,3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
-=============  ==================
-PIP package    Version required
-=============  ==================
-``sqlparse``   ``>=0.4.2``
-=============  ==================
+==================  ==================
+PIP package         Version required
+==================  ==================
+``apache-airflow``  ``>=2.4.0``
+``sqlparse``        ``>=0.4.2``
+==================  ==================
 
  .. Licensed to the Apache Software Foundation (ASF) under one
     or more contributor license agreements.  See the NOTICE file
     distributed with this work for additional information
     regarding copyright ownership.  The ASF licenses this file
     to you under the Apache License, Version 2.0 (the
     "License"); you may not use this file except in compliance
@@ -109,14 +111,22 @@
     and you want to add an explanation to the users on how they are supposed to deal with them.
     The changelog is updated and maintained semi-automatically by release manager.
 
 
 Changelog
 ---------
 
+1.5.1
+.....
+
+Misc
+~~~~
+
+* ``Bring back min-airflow-version for preinstalled providers (#31469)``
+
 1.5.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-common-sql-1.5.0rc2/README.rst` & `apache-airflow-providers-common-sql-1.5.1rc1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -15,47 +15,48 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-common-sql``
 
-Release: ``1.5.0rc2``
+Release: ``1.5.1rc1``
 
 
 `Common SQL Provider <https://en.wikipedia.org/wiki/SQL>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``common.sql`` provider. All classes for this provider package
 are in ``airflow.providers.common.sql`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.5.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.5.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-common-sql``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.7,3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
-=============  ==================
-PIP package    Version required
-=============  ==================
-``sqlparse``   ``>=0.4.2``
-=============  ==================
+==================  ==================
+PIP package         Version required
+==================  ==================
+``apache-airflow``  ``>=2.4.0``
+``sqlparse``        ``>=0.4.2``
+==================  ==================
 
  .. Licensed to the Apache Software Foundation (ASF) under one
     or more contributor license agreements.  See the NOTICE file
     distributed with this work for additional information
     regarding copyright ownership.  The ASF licenses this file
     to you under the Apache License, Version 2.0 (the
     "License"); you may not use this file except in compliance
@@ -75,14 +76,22 @@
     and you want to add an explanation to the users on how they are supposed to deal with them.
     The changelog is updated and maintained semi-automatically by release manager.
 
 
 Changelog
 ---------
 
+1.5.1
+.....
+
+Misc
+~~~~
+
+* ``Bring back min-airflow-version for preinstalled providers (#31469)``
+
 1.5.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-common-sql-1.5.0rc2/airflow/providers/common/sql/__init__.py` & `apache-airflow-providers-common-sql-1.5.1rc1/airflow/providers/common/sql/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "1.5.0"
+__version__ = "1.5.1"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
```

### Comparing `apache-airflow-providers-common-sql-1.5.0rc2/airflow/providers/common/sql/get_provider_info.py` & `apache-airflow-providers-common-sql-1.5.1rc1/airflow/providers/common/sql/get_provider_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,26 +25,27 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-common-sql",
         "name": "Common SQL",
         "description": "`Common SQL Provider <https://en.wikipedia.org/wiki/SQL>`__\n",
         "suspended": False,
         "versions": [
+            "1.5.1",
             "1.5.0",
             "1.4.0",
             "1.3.4",
             "1.3.3",
             "1.3.2",
             "1.3.1",
             "1.3.0",
             "1.2.0",
             "1.1.0",
             "1.0.0",
         ],
-        "dependencies": ["sqlparse>=0.4.2"],
+        "dependencies": ["apache-airflow>=2.4.0", "sqlparse>=0.4.2"],
         "additional-extras": [{"name": "pandas", "dependencies": ["pandas>=0.17.1"]}],
         "integrations": [
             {
                 "integration-name": "Common SQL",
                 "external-doc-url": "https://en.wikipedia.org/wiki/SQL",
                 "how-to-guide": ["/docs/apache-airflow-providers-common-sql/operators.rst"],
                 "logo": "/integration-logos/common/sql/sql.png",
```

### Comparing `apache-airflow-providers-common-sql-1.5.0rc2/airflow/providers/common/sql/hooks/__init__.py` & `apache-airflow-providers-common-sql-1.5.1rc1/airflow/providers/common/sql/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.5.0rc2/airflow/providers/common/sql/hooks/sql.py` & `apache-airflow-providers-common-sql-1.5.1rc1/airflow/providers/common/sql/hooks/sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.5.0rc2/airflow/providers/common/sql/operators/__init__.py` & `apache-airflow-providers-common-sql-1.5.1rc1/airflow/providers/common/sql/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.5.0rc2/airflow/providers/common/sql/operators/sql.py` & `apache-airflow-providers-common-sql-1.5.1rc1/airflow/providers/common/sql/operators/sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.5.0rc2/airflow/providers/common/sql/sensors/__init__.py` & `apache-airflow-providers-common-sql-1.5.1rc1/airflow/providers/common/sql/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.5.0rc2/airflow/providers/common/sql/sensors/sql.py` & `apache-airflow-providers-common-sql-1.5.1rc1/airflow/providers/common/sql/sensors/sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.5.0rc2/apache_airflow_providers_common_sql.egg-info/PKG-INFO` & `apache-airflow-providers-common-sql-1.5.1rc1/apache_airflow_providers_common_sql.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-common-sql
-Version: 1.5.0rc2
+Version: 1.5.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-common-sql package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.5.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.5.1/
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
 Provides-Extra: pandas
 License-File: LICENSE
 License-File: NOTICE
 
@@ -49,47 +50,48 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-common-sql``
 
-Release: ``1.5.0rc2``
+Release: ``1.5.1rc1``
 
 
 `Common SQL Provider <https://en.wikipedia.org/wiki/SQL>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``common.sql`` provider. All classes for this provider package
 are in ``airflow.providers.common.sql`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.5.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.5.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-common-sql``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.7,3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
-=============  ==================
-PIP package    Version required
-=============  ==================
-``sqlparse``   ``>=0.4.2``
-=============  ==================
+==================  ==================
+PIP package         Version required
+==================  ==================
+``apache-airflow``  ``>=2.4.0``
+``sqlparse``        ``>=0.4.2``
+==================  ==================
 
  .. Licensed to the Apache Software Foundation (ASF) under one
     or more contributor license agreements.  See the NOTICE file
     distributed with this work for additional information
     regarding copyright ownership.  The ASF licenses this file
     to you under the Apache License, Version 2.0 (the
     "License"); you may not use this file except in compliance
@@ -109,14 +111,22 @@
     and you want to add an explanation to the users on how they are supposed to deal with them.
     The changelog is updated and maintained semi-automatically by release manager.
 
 
 Changelog
 ---------
 
+1.5.1
+.....
+
+Misc
+~~~~
+
+* ``Bring back min-airflow-version for preinstalled providers (#31469)``
+
 1.5.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-common-sql-1.5.0rc2/apache_airflow_providers_common_sql.egg-info/SOURCES.txt` & `apache-airflow-providers-common-sql-1.5.1rc1/apache_airflow_providers_common_sql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.5.0rc2/pyproject.toml` & `apache-airflow-providers-common-sql-1.5.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.5.0rc2/setup.cfg` & `apache-airflow-providers-common-sql-1.5.1rc1/setup.cfg`

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.5.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.5.1/
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
@@ -42,20 +43,21 @@
 include_package_data = True
 python_requires = ~=3.7
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
+	apache-airflow>=2.4.0.dev0
 	sqlparse>=0.4.2
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.common.sql.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.common.sql
 
 [egg_info]
-tag_build = rc2
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-common-sql-1.5.0rc2/setup.py` & `apache-airflow-providers-common-sql-1.5.1rc1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-common-sql package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "1.5.0"
+version = "1.5.1"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-common-sql setup."""
     setup(
         version=version,
         extras_require={"pandas": ["pandas>=0.17.1"]},
```

