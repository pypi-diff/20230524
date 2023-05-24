# Comparing `tmp/riptide_all-0.7.0-py3-none-any.whl.zip` & `tmp/riptide_all-0.8.0b1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 3110 bytes, number of entries: 5
--rw-r--r--  2.0 unx     1070 b- defN 22-Jan-05 17:18 riptide_all-0.7.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     4416 b- defN 22-Jan-05 17:18 riptide_all-0.7.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Jan-05 17:18 riptide_all-0.7.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 22-Jan-05 17:18 riptide_all-0.7.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      405 b- defN 22-Jan-05 17:18 riptide_all-0.7.0.dist-info/RECORD
-5 files, 5984 bytes uncompressed, 2350 bytes compressed:  60.7%
+Zip file size: 3058 bytes, number of entries: 5
+-rw-r--r--  2.0 unx     1070 b- defN 23-May-24 15:13 riptide_all-0.8.0b1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4230 b- defN 23-May-24 15:13 riptide_all-0.8.0b1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-24 15:13 riptide_all-0.8.0b1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-May-24 15:13 riptide_all-0.8.0b1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      415 b- defN 23-May-24 15:13 riptide_all-0.8.0b1.dist-info/RECORD
+5 files, 5808 bytes uncompressed, 2278 bytes compressed:  60.8%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
-Filename: riptide_all-0.7.0.dist-info/LICENSE
+Filename: riptide_all-0.8.0b1.dist-info/LICENSE
 Comment: 
 
-Filename: riptide_all-0.7.0.dist-info/METADATA
+Filename: riptide_all-0.8.0b1.dist-info/METADATA
 Comment: 
 
-Filename: riptide_all-0.7.0.dist-info/WHEEL
+Filename: riptide_all-0.8.0b1.dist-info/WHEEL
 Comment: 
 
-Filename: riptide_all-0.7.0.dist-info/top_level.txt
+Filename: riptide_all-0.8.0b1.dist-info/top_level.txt
 Comment: 
 
-Filename: riptide_all-0.7.0.dist-info/RECORD
+Filename: riptide_all-0.8.0b1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `riptide_all-0.7.0.dist-info/LICENSE` & `riptide_all-0.8.0b1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `riptide_all-0.7.0.dist-info/METADATA` & `riptide_all-0.8.0b1.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 Metadata-Version: 2.1
 Name: riptide-all
-Version: 0.7.0
+Version: 0.8.0b1
 Summary: Tool to manage development environments for web applications using containers - Meta Package
 Home-page: https://github.com/Parakoopa/riptide-all/
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
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: riptide-lib (<0.8,>=0.7.0)
-Requires-Dist: riptide-cli (<0.8,>=0.7.0)
-Requires-Dist: riptide-proxy (<0.8,>=0.7.0)
-Requires-Dist: riptide-engine-docker (<0.8,>=0.7.0)
-Requires-Dist: riptide-db-mysql (<0.8,>=0.7.0)
-Requires-Dist: riptide-plugin-php-xdebug (<0.8,>=0.7.0)
+Requires-Dist: riptide-lib (<0.9,>=0.8.0b1)
+Requires-Dist: riptide-cli (<0.9,>=0.8.0b1)
+Requires-Dist: riptide-proxy (<0.9,>=0.8.0b1)
+Requires-Dist: riptide-engine-docker (<0.9,>=0.8.0b1)
+Requires-Dist: riptide-db-mysql (<0.9,>=0.8.0b1)
+Requires-Dist: riptide-plugin-php-xdebug (<0.9,>=0.8.0b1)
 
 |Riptide|
 =========
 
 .. |Riptide| image:: https://riptide-docs.readthedocs.io/en/latest/_images/logo.png
     :alt: Riptide
 
@@ -50,28 +48,24 @@
 .. _docs:           https://github.com/Parakoopa/riptide-docs
 .. _repo:           https://github.com/Parakoopa/riptide-repo
 .. _docker_images:  https://github.com/Parakoopa/riptide-docker-images
 .. _php_xdebug:     https://github.com/Parakoopa/riptide-plugin-php-xdebug
 .. _k8s_client:     https://github.com/Parakoopa/riptide-k8s-client
 .. _k8s_controller: https://github.com/Parakoopa/riptide-k8s-controller
 
-|build| |docs| |pypi-version| |pypi-downloads| |pypi-license| |pypi-pyversions| |slack|
+|build| |docs| |pypi-version| |pypi-downloads| |pypi-license| |pypi-pyversions|
 
-.. |build| image:: https://img.shields.io/github/workflow/status/Parakoopa/riptide-all/Build,%20test%20and%20publish
+.. |build| image:: https://img.shields.io/github/actions/workflow/status/theCapypara/riptide-all/build.yml
     :target: https://github.com/Parakoopa/riptide-all/actions
     :alt: Build Status
 
 .. |docs| image:: https://readthedocs.org/projects/riptide-docs/badge/?version=latest
     :target: https://riptide-docs.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
-.. |slack| image:: https://slack.riptide.parakoopa.de/badge.svg
-    :target: https://slack.riptide.parakoopa.de
-    :alt: Join our Slack workspace
-
 .. |pypi-version| image:: https://img.shields.io/pypi/v/riptide-all
     :target: https://pypi.org/project/riptide-all/
     :alt: Version
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/riptide-all
     :target: https://pypi.org/project/riptide-all/
     :alt: Downloads
@@ -96,8 +90,7 @@
 
 Installing this package will install all Riptide components in the matching version numbers.
 
 Documentation
 -------------
 
 The complete documentation for Riptide can be found at `Read the Docs <https://riptide-docs.readthedocs.io/en/latest/>`_.
-
```

