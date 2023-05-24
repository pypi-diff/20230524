# Comparing `tmp/apache-airflow-providers-http-4.4.0rc2.tar.gz` & `tmp/apache-airflow-providers-http-4.4.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-http-4.4.0rc2.tar", last modified: Fri May 19 17:52:40 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-http-4.4.1rc1.tar", last modified: Wed May 24 07:20:34 2023, max compression
```

## Comparing `apache-airflow-providers-http-4.4.0rc2.tar` & `apache-airflow-providers-http-4.4.1rc1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:40.000000 apache-airflow-providers-http-4.4.0rc2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-http-4.4.0rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-19 17:52:39.000000 apache-airflow-providers-http-4.4.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-http-4.4.0rc2/NOTICE
--rw-r--r--   0 root         (0) root         (0)    12238 2023-05-19 17:52:40.000000 apache-airflow-providers-http-4.4.0rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10717 2023-05-19 17:52:39.000000 apache-airflow-providers-http-4.4.0rc2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:40.000000 apache-airflow-providers-http-4.4.0rc2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:40.000000 apache-airflow-providers-http-4.4.0rc2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:40.000000 apache-airflow-providers-http-4.4.0rc2/airflow/providers/http/
--rw-r--r--   0 root         (0) root         (0)     1529 2023-05-19 12:12:32.000000 apache-airflow-providers-http-4.4.0rc2/airflow/providers/http/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2950 2023-05-19 17:52:39.000000 apache-airflow-providers-http-4.4.0rc2/airflow/providers/http/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:40.000000 apache-airflow-providers-http-4.4.0rc2/airflow/providers/http/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-http-4.4.0rc2/airflow/providers/http/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16287 2023-04-24 21:04:25.000000 apache-airflow-providers-http-4.4.0rc2/airflow/providers/http/hooks/http.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:40.000000 apache-airflow-providers-http-4.4.0rc2/airflow/providers/http/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-http-4.4.0rc2/airflow/providers/http/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5828 2023-03-27 08:32:49.000000 apache-airflow-providers-http-4.4.0rc2/airflow/providers/http/operators/http.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:40.000000 apache-airflow-providers-http-4.4.0rc2/airflow/providers/http/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-http-4.4.0rc2/airflow/providers/http/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5885 2023-02-24 18:43:53.000000 apache-airflow-providers-http-4.4.0rc2/airflow/providers/http/sensors/http.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:40.000000 apache-airflow-providers-http-4.4.0rc2/apache_airflow_providers_http.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12238 2023-05-19 17:52:40.000000 apache-airflow-providers-http-4.4.0rc2/apache_airflow_providers_http.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      768 2023-05-19 17:52:40.000000 apache-airflow-providers-http-4.4.0rc2/apache_airflow_providers_http.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:52:40.000000 apache-airflow-providers-http-4.4.0rc2/apache_airflow_providers_http.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      101 2023-05-19 17:52:40.000000 apache-airflow-providers-http-4.4.0rc2/apache_airflow_providers_http.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:52:40.000000 apache-airflow-providers-http-4.4.0rc2/apache_airflow_providers_http.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       51 2023-05-19 17:52:40.000000 apache-airflow-providers-http-4.4.0rc2/apache_airflow_providers_http.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:52:40.000000 apache-airflow-providers-http-4.4.0rc2/apache_airflow_providers_http.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-http-4.4.0rc2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1843 2023-05-19 17:52:40.000000 apache-airflow-providers-http-4.4.0rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1626 2023-05-19 17:52:39.000000 apache-airflow-providers-http-4.4.0rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:34.000000 apache-airflow-providers-http-4.4.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-05-23 11:35:15.000000 apache-airflow-providers-http-4.4.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-24 07:20:33.000000 apache-airflow-providers-http-4.4.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-05-23 11:35:15.000000 apache-airflow-providers-http-4.4.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    12427 2023-05-24 07:20:34.000000 apache-airflow-providers-http-4.4.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10855 2023-05-24 07:20:33.000000 apache-airflow-providers-http-4.4.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:34.000000 apache-airflow-providers-http-4.4.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:34.000000 apache-airflow-providers-http-4.4.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:34.000000 apache-airflow-providers-http-4.4.1rc1/airflow/providers/http/
+-rw-r--r--   0 root         (0) root         (0)     1529 2023-05-24 07:09:22.000000 apache-airflow-providers-http-4.4.1rc1/airflow/providers/http/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3067 2023-05-24 07:20:33.000000 apache-airflow-providers-http-4.4.1rc1/airflow/providers/http/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:34.000000 apache-airflow-providers-http-4.4.1rc1/airflow/providers/http/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-05-23 11:35:14.000000 apache-airflow-providers-http-4.4.1rc1/airflow/providers/http/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16287 2023-05-23 11:35:14.000000 apache-airflow-providers-http-4.4.1rc1/airflow/providers/http/hooks/http.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:34.000000 apache-airflow-providers-http-4.4.1rc1/airflow/providers/http/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-05-23 11:35:14.000000 apache-airflow-providers-http-4.4.1rc1/airflow/providers/http/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5828 2023-05-23 11:35:14.000000 apache-airflow-providers-http-4.4.1rc1/airflow/providers/http/operators/http.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:34.000000 apache-airflow-providers-http-4.4.1rc1/airflow/providers/http/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-05-23 11:35:14.000000 apache-airflow-providers-http-4.4.1rc1/airflow/providers/http/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5885 2023-05-23 11:35:14.000000 apache-airflow-providers-http-4.4.1rc1/airflow/providers/http/sensors/http.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:34.000000 apache-airflow-providers-http-4.4.1rc1/apache_airflow_providers_http.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    12427 2023-05-24 07:20:34.000000 apache-airflow-providers-http-4.4.1rc1/apache_airflow_providers_http.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      768 2023-05-24 07:20:34.000000 apache-airflow-providers-http-4.4.1rc1/apache_airflow_providers_http.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 07:20:34.000000 apache-airflow-providers-http-4.4.1rc1/apache_airflow_providers_http.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      101 2023-05-24 07:20:34.000000 apache-airflow-providers-http-4.4.1rc1/apache_airflow_providers_http.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 07:20:34.000000 apache-airflow-providers-http-4.4.1rc1/apache_airflow_providers_http.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       78 2023-05-24 07:20:34.000000 apache-airflow-providers-http-4.4.1rc1/apache_airflow_providers_http.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-24 07:20:34.000000 apache-airflow-providers-http-4.4.1rc1/apache_airflow_providers_http.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5338 2023-05-23 11:35:15.000000 apache-airflow-providers-http-4.4.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1911 2023-05-24 07:20:34.000000 apache-airflow-providers-http-4.4.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1626 2023-05-24 07:20:33.000000 apache-airflow-providers-http-4.4.1rc1/setup.py
```

### Comparing `apache-airflow-providers-http-4.4.0rc2/LICENSE` & `apache-airflow-providers-http-4.4.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-http-4.4.0rc2/MANIFEST.in` & `apache-airflow-providers-http-4.4.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-http-4.4.0rc2/PKG-INFO` & `apache-airflow-providers-http-4.4.1rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-http
-Version: 4.4.0rc2
+Version: 4.4.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-http package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-http/4.4.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-http/4.4.1/
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
 
 
@@ -48,45 +49,46 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-http``
 
-Release: ``4.4.0rc2``
+Release: ``4.4.1rc1``
 
 
 `Hypertext Transfer Protocol (HTTP) <https://www.w3.org/Protocols/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``http`` provider. All classes for this provider package
 are in ``airflow.providers.http`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-http/4.4.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-http/4.4.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-http``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.7,3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =====================  ==================
 PIP package            Version required
 =====================  ==================
+``apache-airflow``     ``>=2.4.0``
 ``requests``           ``>=2.26.0``
 ``requests_toolbelt``
 ``aiohttp``
 ``asgiref``
 =====================  ==================
 
  .. Licensed to the Apache Software Foundation (ASF) under one
@@ -111,14 +113,22 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+4.4.1
+.....
+
+Misc
+~~~~
+
+* ``Bring back min-airflow-version for preinstalled providers (#31469)``
+
 4.4.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-http-4.4.0rc2/README.rst` & `apache-airflow-providers-http-4.4.1rc1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -15,45 +15,46 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-http``
 
-Release: ``4.4.0rc2``
+Release: ``4.4.1rc1``
 
 
 `Hypertext Transfer Protocol (HTTP) <https://www.w3.org/Protocols/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``http`` provider. All classes for this provider package
 are in ``airflow.providers.http`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-http/4.4.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-http/4.4.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-http``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.7,3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =====================  ==================
 PIP package            Version required
 =====================  ==================
+``apache-airflow``     ``>=2.4.0``
 ``requests``           ``>=2.26.0``
 ``requests_toolbelt``
 ``aiohttp``
 ``asgiref``
 =====================  ==================
 
  .. Licensed to the Apache Software Foundation (ASF) under one
@@ -78,14 +79,22 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+4.4.1
+.....
+
+Misc
+~~~~
+
+* ``Bring back min-airflow-version for preinstalled providers (#31469)``
+
 4.4.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-http-4.4.0rc2/airflow/providers/http/__init__.py` & `apache-airflow-providers-http-4.4.1rc1/airflow/providers/http/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "4.4.0"
+__version__ = "4.4.1"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
```

### Comparing `apache-airflow-providers-http-4.4.0rc2/airflow/providers/http/get_provider_info.py` & `apache-airflow-providers-http-4.4.1rc1/airflow/providers/http/get_provider_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-http",
         "name": "Hypertext Transfer Protocol (HTTP)",
         "description": "`Hypertext Transfer Protocol (HTTP) <https://www.w3.org/Protocols/>`__\n",
         "suspended": False,
         "versions": [
+            "4.4.1",
             "4.4.0",
             "4.3.0",
             "4.2.0",
             "4.1.1",
             "4.1.0",
             "4.0.0",
             "3.0.0",
@@ -43,15 +44,21 @@
             "2.0.2",
             "2.0.1",
             "2.0.0",
             "1.1.1",
             "1.1.0",
             "1.0.0",
         ],
-        "dependencies": ["requests>=2.26.0", "requests_toolbelt", "aiohttp", "asgiref"],
+        "dependencies": [
+            "apache-airflow>=2.4.0",
+            "requests>=2.26.0",
+            "requests_toolbelt",
+            "aiohttp",
+            "asgiref",
+        ],
         "integrations": [
             {
                 "integration-name": "Hypertext Transfer Protocol (HTTP)",
                 "external-doc-url": "https://www.w3.org/Protocols/",
                 "how-to-guide": ["/docs/apache-airflow-providers-http/operators.rst"],
                 "logo": "/integration-logos/http/HTTP.png",
                 "tags": ["protocol"],
```

### Comparing `apache-airflow-providers-http-4.4.0rc2/airflow/providers/http/hooks/__init__.py` & `apache-airflow-providers-http-4.4.1rc1/airflow/providers/http/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-http-4.4.0rc2/airflow/providers/http/hooks/http.py` & `apache-airflow-providers-http-4.4.1rc1/airflow/providers/http/hooks/http.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-http-4.4.0rc2/airflow/providers/http/operators/__init__.py` & `apache-airflow-providers-http-4.4.1rc1/airflow/providers/http/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-http-4.4.0rc2/airflow/providers/http/operators/http.py` & `apache-airflow-providers-http-4.4.1rc1/airflow/providers/http/operators/http.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-http-4.4.0rc2/airflow/providers/http/sensors/__init__.py` & `apache-airflow-providers-http-4.4.1rc1/airflow/providers/http/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-http-4.4.0rc2/airflow/providers/http/sensors/http.py` & `apache-airflow-providers-http-4.4.1rc1/airflow/providers/http/sensors/http.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-http-4.4.0rc2/apache_airflow_providers_http.egg-info/PKG-INFO` & `apache-airflow-providers-http-4.4.1rc1/apache_airflow_providers_http.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-http
-Version: 4.4.0rc2
+Version: 4.4.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-http package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-http/4.4.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-http/4.4.1/
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
 
 
@@ -48,45 +49,46 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-http``
 
-Release: ``4.4.0rc2``
+Release: ``4.4.1rc1``
 
 
 `Hypertext Transfer Protocol (HTTP) <https://www.w3.org/Protocols/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``http`` provider. All classes for this provider package
 are in ``airflow.providers.http`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-http/4.4.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-http/4.4.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-http``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.7,3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =====================  ==================
 PIP package            Version required
 =====================  ==================
+``apache-airflow``     ``>=2.4.0``
 ``requests``           ``>=2.26.0``
 ``requests_toolbelt``
 ``aiohttp``
 ``asgiref``
 =====================  ==================
 
  .. Licensed to the Apache Software Foundation (ASF) under one
@@ -111,14 +113,22 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+4.4.1
+.....
+
+Misc
+~~~~
+
+* ``Bring back min-airflow-version for preinstalled providers (#31469)``
+
 4.4.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-http-4.4.0rc2/apache_airflow_providers_http.egg-info/SOURCES.txt` & `apache-airflow-providers-http-4.4.1rc1/apache_airflow_providers_http.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-http-4.4.0rc2/pyproject.toml` & `apache-airflow-providers-http-4.4.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-http-4.4.0rc2/setup.cfg` & `apache-airflow-providers-http-4.4.1rc1/setup.cfg`

 * *Files 2% similar despite different names*

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-http/4.4.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-http/4.4.1/
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
@@ -43,22 +44,23 @@
 python_requires = ~=3.7
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
 	aiohttp
+	apache-airflow>=2.4.0.dev0
 	asgiref
 	requests>=2.26.0
 	requests_toolbelt
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.http.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.http
 
 [egg_info]
-tag_build = rc2
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-http-4.4.0rc2/setup.py` & `apache-airflow-providers-http-4.4.1rc1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-http package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "4.4.0"
+version = "4.4.1"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-http setup."""
     setup(
         version=version,
         extras_require={},
```

