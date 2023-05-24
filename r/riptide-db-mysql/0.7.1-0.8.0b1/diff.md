# Comparing `tmp/riptide_db_mysql-0.7.1-py3-none-any.whl.zip` & `tmp/riptide_db_mysql-0.8.0b1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 5122 bytes, number of entries: 8
--rw-r--r--  2.0 unx        0 b- defN 22-Jan-12 09:04 riptide_db_mysql/__init__.py
--rw-r--r--  2.0 unx     4152 b- defN 22-Jan-12 09:04 riptide_db_mysql/mysql.py
--rw-r--r--  2.0 unx     1070 b- defN 22-Jan-12 09:05 riptide_db_mysql-0.7.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     4486 b- defN 22-Jan-12 09:05 riptide_db_mysql-0.7.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Jan-12 09:05 riptide_db_mysql-0.7.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       84 b- defN 22-Jan-12 09:05 riptide_db_mysql-0.7.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       17 b- defN 22-Jan-12 09:05 riptide_db_mysql-0.7.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      699 b- defN 22-Jan-12 09:05 riptide_db_mysql-0.7.1.dist-info/RECORD
-8 files, 10600 bytes uncompressed, 3880 bytes compressed:  63.4%
+Zip file size: 5064 bytes, number of entries: 8
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 15:06 riptide_db_mysql/__init__.py
+-rw-r--r--  2.0 unx     4152 b- defN 23-May-24 15:06 riptide_db_mysql/mysql.py
+-rw-r--r--  2.0 unx     1070 b- defN 23-May-24 15:07 riptide_db_mysql-0.8.0b1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4235 b- defN 23-May-24 15:07 riptide_db_mysql-0.8.0b1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-24 15:07 riptide_db_mysql-0.8.0b1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       65 b- defN 23-May-24 15:07 riptide_db_mysql-0.8.0b1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       17 b- defN 23-May-24 15:07 riptide_db_mysql-0.8.0b1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      711 b- defN 23-May-24 15:07 riptide_db_mysql-0.8.0b1.dist-info/RECORD
+8 files, 10342 bytes uncompressed, 3798 bytes compressed:  63.3%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: riptide_db_mysql/__init__.py
 Comment: 
 
 Filename: riptide_db_mysql/mysql.py
 Comment: 
 
-Filename: riptide_db_mysql-0.7.1.dist-info/LICENSE
+Filename: riptide_db_mysql-0.8.0b1.dist-info/LICENSE
 Comment: 
 
-Filename: riptide_db_mysql-0.7.1.dist-info/METADATA
+Filename: riptide_db_mysql-0.8.0b1.dist-info/METADATA
 Comment: 
 
-Filename: riptide_db_mysql-0.7.1.dist-info/WHEEL
+Filename: riptide_db_mysql-0.8.0b1.dist-info/WHEEL
 Comment: 
 
-Filename: riptide_db_mysql-0.7.1.dist-info/entry_points.txt
+Filename: riptide_db_mysql-0.8.0b1.dist-info/entry_points.txt
 Comment: 
 
-Filename: riptide_db_mysql-0.7.1.dist-info/top_level.txt
+Filename: riptide_db_mysql-0.8.0b1.dist-info/top_level.txt
 Comment: 
 
-Filename: riptide_db_mysql-0.7.1.dist-info/RECORD
+Filename: riptide_db_mysql-0.8.0b1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `riptide_db_mysql-0.7.1.dist-info/LICENSE` & `riptide_db_mysql-0.8.0b1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `riptide_db_mysql-0.7.1.dist-info/METADATA` & `riptide_db_mysql-0.8.0b1.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 Metadata-Version: 2.1
 Name: riptide-db-mysql
-Version: 0.7.1
+Version: 0.8.0b1
 Summary: Tool to manage development environments for web applications using containers - MySQL Database Drvier
 Home-page: https://github.com/theCapypara/riptide-db-mysql/
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: riptide-lib (<0.8,>=0.7)
+Requires-Dist: riptide-lib (<0.9,>=0.8.0b1)
 Requires-Dist: schema (>=0.7)
 
 |Riptide|
 =========
 
 .. |Riptide| image:: https://riptide-docs.readthedocs.io/en/latest/_images/logo.png
     :alt: Riptide
@@ -47,28 +44,24 @@
 .. _docs:           https://github.com/theCapypara/riptide-docs
 .. _repo:           https://github.com/theCapypara/riptide-repo
 .. _docker_images:  https://github.com/theCapypara/riptide-docker-images
 .. _php_xdebug:     https://github.com/theCapypara/riptide-plugin-php-xdebug
 .. _k8s_client:     https://github.com/theCapypara/riptide-k8s-client
 .. _k8s_controller: https://github.com/theCapypara/riptide-k8s-controller
 
-|build| |docs| |pypi-version| |pypi-downloads| |pypi-license| |pypi-pyversions| |slack|
+|build| |docs| |pypi-version| |pypi-downloads| |pypi-license| |pypi-pyversions|
 
-.. |build| image:: https://img.shields.io/github/workflow/status/theCapypara/riptide-db-mysql/Build,%20test%20and%20publish
+.. |build| image:: https://img.shields.io/github/actions/workflow/status/theCapypara/riptide-db-mysql/build.yml
     :target: https://github.com/theCapypara/riptide-db-mysql/actions
     :alt: Build Status
 
 .. |docs| image:: https://readthedocs.org/projects/riptide-docs/badge/?version=latest
     :target: https://riptide-docs.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
-.. |slack| image:: https://slack.riptide.theCapypara.de/badge.svg
-    :target: https://slack.riptide.theCapypara.de
-    :alt: Join our Slack workspace
-
 .. |pypi-version| image:: https://img.shields.io/pypi/v/riptide-db-mysql
     :target: https://pypi.org/project/riptide-db-mysql/
     :alt: Version
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/riptide-db-mysql
     :target: https://pypi.org/project/riptide-db-mysql/
     :alt: Downloads
@@ -95,8 +88,7 @@
 with MySQL-compatible databases. This allows users to manage MySQL databases within
 Riptide projects via the Riptide CLI.
 
 Documentation
 -------------
 
 The complete documentation for Riptide can be found at `Read the Docs <https://riptide-docs.readthedocs.io/en/latest/>`_.
-
```

