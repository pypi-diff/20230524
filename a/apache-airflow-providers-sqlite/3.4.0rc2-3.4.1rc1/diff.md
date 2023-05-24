# Comparing `tmp/apache-airflow-providers-sqlite-3.4.0rc2.tar.gz` & `tmp/apache-airflow-providers-sqlite-3.4.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-sqlite-3.4.0rc2.tar", last modified: Fri May 19 17:53:37 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-sqlite-3.4.1rc1.tar", last modified: Wed May 24 07:20:30 2023, max compression
```

## Comparing `apache-airflow-providers-sqlite-3.4.0rc2.tar` & `apache-airflow-providers-sqlite-3.4.1rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:37.000000 apache-airflow-providers-sqlite-3.4.0rc2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-sqlite-3.4.0rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-19 17:53:36.000000 apache-airflow-providers-sqlite-3.4.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-sqlite-3.4.0rc2/NOTICE
--rw-r--r--   0 root         (0) root         (0)    12928 2023-05-19 17:53:37.000000 apache-airflow-providers-sqlite-3.4.0rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11374 2023-05-19 17:53:36.000000 apache-airflow-providers-sqlite-3.4.0rc2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:37.000000 apache-airflow-providers-sqlite-3.4.0rc2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:37.000000 apache-airflow-providers-sqlite-3.4.0rc2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:37.000000 apache-airflow-providers-sqlite-3.4.0rc2/airflow/providers/sqlite/
--rw-r--r--   0 root         (0) root         (0)     1531 2023-05-19 12:22:06.000000 apache-airflow-providers-sqlite-3.4.0rc2/airflow/providers/sqlite/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2559 2023-05-19 17:53:36.000000 apache-airflow-providers-sqlite-3.4.0rc2/airflow/providers/sqlite/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:37.000000 apache-airflow-providers-sqlite-3.4.0rc2/airflow/providers/sqlite/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-sqlite-3.4.0rc2/airflow/providers/sqlite/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2400 2023-04-13 08:25:21.000000 apache-airflow-providers-sqlite-3.4.0rc2/airflow/providers/sqlite/hooks/sqlite.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:37.000000 apache-airflow-providers-sqlite-3.4.0rc2/airflow/providers/sqlite/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-sqlite-3.4.0rc2/airflow/providers/sqlite/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2227 2023-05-03 19:47:07.000000 apache-airflow-providers-sqlite-3.4.0rc2/airflow/providers/sqlite/operators/sqlite.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:37.000000 apache-airflow-providers-sqlite-3.4.0rc2/apache_airflow_providers_sqlite.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12928 2023-05-19 17:53:37.000000 apache-airflow-providers-sqlite-3.4.0rc2/apache_airflow_providers_sqlite.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      716 2023-05-19 17:53:37.000000 apache-airflow-providers-sqlite-3.4.0rc2/apache_airflow_providers_sqlite.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:53:37.000000 apache-airflow-providers-sqlite-3.4.0rc2/apache_airflow_providers_sqlite.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-05-19 17:53:37.000000 apache-airflow-providers-sqlite-3.4.0rc2/apache_airflow_providers_sqlite.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:53:37.000000 apache-airflow-providers-sqlite-3.4.0rc2/apache_airflow_providers_sqlite.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       98 2023-05-19 17:53:37.000000 apache-airflow-providers-sqlite-3.4.0rc2/apache_airflow_providers_sqlite.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:53:37.000000 apache-airflow-providers-sqlite-3.4.0rc2/apache_airflow_providers_sqlite.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-sqlite-3.4.0rc2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1849 2023-05-19 17:53:37.000000 apache-airflow-providers-sqlite-3.4.0rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1691 2023-05-19 17:53:36.000000 apache-airflow-providers-sqlite-3.4.0rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:30.000000 apache-airflow-providers-sqlite-3.4.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-05-23 11:35:15.000000 apache-airflow-providers-sqlite-3.4.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-24 07:20:29.000000 apache-airflow-providers-sqlite-3.4.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-05-23 11:35:15.000000 apache-airflow-providers-sqlite-3.4.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    13135 2023-05-24 07:20:30.000000 apache-airflow-providers-sqlite-3.4.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11530 2023-05-24 07:20:29.000000 apache-airflow-providers-sqlite-3.4.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:30.000000 apache-airflow-providers-sqlite-3.4.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:30.000000 apache-airflow-providers-sqlite-3.4.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:30.000000 apache-airflow-providers-sqlite-3.4.1rc1/airflow/providers/sqlite/
+-rw-r--r--   0 root         (0) root         (0)     1531 2023-05-24 07:09:22.000000 apache-airflow-providers-sqlite-3.4.1rc1/airflow/providers/sqlite/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2605 2023-05-24 07:20:29.000000 apache-airflow-providers-sqlite-3.4.1rc1/airflow/providers/sqlite/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:30.000000 apache-airflow-providers-sqlite-3.4.1rc1/airflow/providers/sqlite/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-05-23 11:35:15.000000 apache-airflow-providers-sqlite-3.4.1rc1/airflow/providers/sqlite/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2400 2023-05-23 11:35:15.000000 apache-airflow-providers-sqlite-3.4.1rc1/airflow/providers/sqlite/hooks/sqlite.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:30.000000 apache-airflow-providers-sqlite-3.4.1rc1/airflow/providers/sqlite/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-05-23 11:35:15.000000 apache-airflow-providers-sqlite-3.4.1rc1/airflow/providers/sqlite/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2227 2023-05-23 11:35:15.000000 apache-airflow-providers-sqlite-3.4.1rc1/airflow/providers/sqlite/operators/sqlite.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:30.000000 apache-airflow-providers-sqlite-3.4.1rc1/apache_airflow_providers_sqlite.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13135 2023-05-24 07:20:30.000000 apache-airflow-providers-sqlite-3.4.1rc1/apache_airflow_providers_sqlite.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      716 2023-05-24 07:20:30.000000 apache-airflow-providers-sqlite-3.4.1rc1/apache_airflow_providers_sqlite.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 07:20:30.000000 apache-airflow-providers-sqlite-3.4.1rc1/apache_airflow_providers_sqlite.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-05-24 07:20:30.000000 apache-airflow-providers-sqlite-3.4.1rc1/apache_airflow_providers_sqlite.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 07:20:30.000000 apache-airflow-providers-sqlite-3.4.1rc1/apache_airflow_providers_sqlite.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      125 2023-05-24 07:20:30.000000 apache-airflow-providers-sqlite-3.4.1rc1/apache_airflow_providers_sqlite.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-24 07:20:30.000000 apache-airflow-providers-sqlite-3.4.1rc1/apache_airflow_providers_sqlite.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5338 2023-05-23 11:35:15.000000 apache-airflow-providers-sqlite-3.4.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1917 2023-05-24 07:20:30.000000 apache-airflow-providers-sqlite-3.4.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1691 2023-05-24 07:20:29.000000 apache-airflow-providers-sqlite-3.4.1rc1/setup.py
```

### Comparing `apache-airflow-providers-sqlite-3.4.0rc2/LICENSE` & `apache-airflow-providers-sqlite-3.4.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sqlite-3.4.0rc2/MANIFEST.in` & `apache-airflow-providers-sqlite-3.4.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sqlite-3.4.0rc2/PKG-INFO` & `apache-airflow-providers-sqlite-3.4.1rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-sqlite
-Version: 3.4.0rc2
+Version: 3.4.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-sqlite package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-sqlite/3.4.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-sqlite/3.4.1/
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
 Provides-Extra: common.sql
 License-File: LICENSE
 License-File: NOTICE
 
@@ -49,45 +50,46 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-sqlite``
 
-Release: ``3.4.0rc2``
+Release: ``3.4.1rc1``
 
 
 `SQLite <https://www.sqlite.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``sqlite`` provider. All classes for this provider package
 are in ``airflow.providers.sqlite`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-sqlite/3.4.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-sqlite/3.4.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-sqlite``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.7,3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
+``apache-airflow``                       ``>=2.4.0``
 ``apache-airflow-providers-common-sql``  ``>=1.3.1``
 =======================================  ==================
 
 Cross provider package dependencies
 -----------------------------------
 
 Those are dependencies that might be needed in order to use all the features of the package.
@@ -128,14 +130,22 @@
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

### Comparing `apache-airflow-providers-sqlite-3.4.0rc2/README.rst` & `apache-airflow-providers-sqlite-3.4.1rc1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -15,45 +15,46 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-sqlite``
 
-Release: ``3.4.0rc2``
+Release: ``3.4.1rc1``
 
 
 `SQLite <https://www.sqlite.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``sqlite`` provider. All classes for this provider package
 are in ``airflow.providers.sqlite`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-sqlite/3.4.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-sqlite/3.4.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-sqlite``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.7,3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
+``apache-airflow``                       ``>=2.4.0``
 ``apache-airflow-providers-common-sql``  ``>=1.3.1``
 =======================================  ==================
 
 Cross provider package dependencies
 -----------------------------------
 
 Those are dependencies that might be needed in order to use all the features of the package.
@@ -94,14 +95,22 @@
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

### Comparing `apache-airflow-providers-sqlite-3.4.0rc2/airflow/providers/sqlite/__init__.py` & `apache-airflow-providers-sqlite-3.4.1rc1/airflow/providers/sqlite/__init__.py`

 * *Files 0% similar despite different names*

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

### Comparing `apache-airflow-providers-sqlite-3.4.0rc2/airflow/providers/sqlite/get_provider_info.py` & `apache-airflow-providers-sqlite-3.4.1rc1/airflow/providers/sqlite/get_provider_info.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-sqlite",
         "name": "SQLite",
         "description": "`SQLite <https://www.sqlite.org/>`__\n",
         "suspended": False,
         "versions": [
+            "3.4.1",
             "3.4.0",
             "3.3.2",
             "3.3.1",
             "3.3.0",
             "3.2.1",
             "3.2.0",
             "3.1.0",
@@ -43,15 +44,15 @@
             "2.1.0",
             "2.0.1",
             "2.0.0",
             "1.0.2",
             "1.0.1",
             "1.0.0",
         ],
-        "dependencies": ["apache-airflow-providers-common-sql>=1.3.1"],
+        "dependencies": ["apache-airflow>=2.4.0", "apache-airflow-providers-common-sql>=1.3.1"],
         "integrations": [
             {
                 "integration-name": "SQLite",
                 "external-doc-url": "https://www.sqlite.org/index.html",
                 "how-to-guide": ["/docs/apache-airflow-providers-sqlite/operators.rst"],
                 "logo": "/integration-logos/sqlite/SQLite.png",
                 "tags": ["software"],
```

### Comparing `apache-airflow-providers-sqlite-3.4.0rc2/airflow/providers/sqlite/hooks/__init__.py` & `apache-airflow-providers-sqlite-3.4.1rc1/airflow/providers/sqlite/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sqlite-3.4.0rc2/airflow/providers/sqlite/hooks/sqlite.py` & `apache-airflow-providers-sqlite-3.4.1rc1/airflow/providers/sqlite/hooks/sqlite.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sqlite-3.4.0rc2/airflow/providers/sqlite/operators/__init__.py` & `apache-airflow-providers-sqlite-3.4.1rc1/airflow/providers/sqlite/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sqlite-3.4.0rc2/airflow/providers/sqlite/operators/sqlite.py` & `apache-airflow-providers-sqlite-3.4.1rc1/airflow/providers/sqlite/operators/sqlite.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sqlite-3.4.0rc2/apache_airflow_providers_sqlite.egg-info/PKG-INFO` & `apache-airflow-providers-sqlite-3.4.1rc1/apache_airflow_providers_sqlite.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-sqlite
-Version: 3.4.0rc2
+Version: 3.4.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-sqlite package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-sqlite/3.4.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-sqlite/3.4.1/
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
 Provides-Extra: common.sql
 License-File: LICENSE
 License-File: NOTICE
 
@@ -49,45 +50,46 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-sqlite``
 
-Release: ``3.4.0rc2``
+Release: ``3.4.1rc1``
 
 
 `SQLite <https://www.sqlite.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``sqlite`` provider. All classes for this provider package
 are in ``airflow.providers.sqlite`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-sqlite/3.4.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-sqlite/3.4.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-sqlite``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.7,3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
+``apache-airflow``                       ``>=2.4.0``
 ``apache-airflow-providers-common-sql``  ``>=1.3.1``
 =======================================  ==================
 
 Cross provider package dependencies
 -----------------------------------
 
 Those are dependencies that might be needed in order to use all the features of the package.
@@ -128,14 +130,22 @@
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

### Comparing `apache-airflow-providers-sqlite-3.4.0rc2/apache_airflow_providers_sqlite.egg-info/SOURCES.txt` & `apache-airflow-providers-sqlite-3.4.1rc1/apache_airflow_providers_sqlite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sqlite-3.4.0rc2/pyproject.toml` & `apache-airflow-providers-sqlite-3.4.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sqlite-3.4.0rc2/setup.cfg` & `apache-airflow-providers-sqlite-3.4.1rc1/setup.cfg`

 * *Files 3% similar despite different names*

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-sqlite/3.4.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-sqlite/3.4.1/
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
@@ -43,19 +44,20 @@
 python_requires = ~=3.7
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
 	apache-airflow-providers-common-sql>=1.3.1.dev0
+	apache-airflow>=2.4.0.dev0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.sqlite.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.sqlite
 
 [egg_info]
-tag_build = rc2
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-sqlite-3.4.0rc2/setup.py` & `apache-airflow-providers-sqlite-3.4.1rc1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-sqlite package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "3.4.0"
+version = "3.4.1"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-sqlite setup."""
     setup(
         version=version,
         extras_require={"common.sql": ["apache-airflow-providers-common-sql"]},
```

