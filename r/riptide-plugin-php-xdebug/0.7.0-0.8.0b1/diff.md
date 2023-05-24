# Comparing `tmp/riptide_plugin_php_xdebug-0.7.0-py3-none-any.whl.zip` & `tmp/riptide_plugin_php_xdebug-0.8.0b1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 6970 bytes, number of entries: 8
--rw-r--r--  2.0 unx        0 b- defN 22-Jan-05 16:55 riptide_plugin_php_xdebug/__init__.py
--rw-r--r--  2.0 unx     9248 b- defN 22-Jan-05 16:55 riptide_plugin_php_xdebug/plugin.py
--rw-r--r--  2.0 unx     1070 b- defN 22-Jan-05 16:55 riptide_plugin_php_xdebug-0.7.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     4693 b- defN 22-Jan-05 16:55 riptide_plugin_php_xdebug-0.7.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Jan-05 16:55 riptide_plugin_php_xdebug-0.7.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       98 b- defN 22-Jan-05 16:55 riptide_plugin_php_xdebug-0.7.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       26 b- defN 22-Jan-05 16:55 riptide_plugin_php_xdebug-0.7.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      772 b- defN 22-Jan-05 16:55 riptide_plugin_php_xdebug-0.7.0.dist-info/RECORD
-8 files, 15999 bytes uncompressed, 5582 bytes compressed:  65.1%
+Zip file size: 6909 bytes, number of entries: 8
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 15:06 riptide_plugin_php_xdebug/__init__.py
+-rw-r--r--  2.0 unx     9248 b- defN 23-May-24 15:06 riptide_plugin_php_xdebug/plugin.py
+-rw-r--r--  2.0 unx     1070 b- defN 23-May-24 15:07 riptide_plugin_php_xdebug-0.8.0b1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4463 b- defN 23-May-24 15:07 riptide_plugin_php_xdebug-0.8.0b1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-24 15:07 riptide_plugin_php_xdebug-0.8.0b1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       79 b- defN 23-May-24 15:07 riptide_plugin_php_xdebug-0.8.0b1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       26 b- defN 23-May-24 15:07 riptide_plugin_php_xdebug-0.8.0b1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      784 b- defN 23-May-24 15:07 riptide_plugin_php_xdebug-0.8.0b1.dist-info/RECORD
+8 files, 15762 bytes uncompressed, 5497 bytes compressed:  65.1%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: riptide_plugin_php_xdebug/__init__.py
 Comment: 
 
 Filename: riptide_plugin_php_xdebug/plugin.py
 Comment: 
 
-Filename: riptide_plugin_php_xdebug-0.7.0.dist-info/LICENSE
+Filename: riptide_plugin_php_xdebug-0.8.0b1.dist-info/LICENSE
 Comment: 
 
-Filename: riptide_plugin_php_xdebug-0.7.0.dist-info/METADATA
+Filename: riptide_plugin_php_xdebug-0.8.0b1.dist-info/METADATA
 Comment: 
 
-Filename: riptide_plugin_php_xdebug-0.7.0.dist-info/WHEEL
+Filename: riptide_plugin_php_xdebug-0.8.0b1.dist-info/WHEEL
 Comment: 
 
-Filename: riptide_plugin_php_xdebug-0.7.0.dist-info/entry_points.txt
+Filename: riptide_plugin_php_xdebug-0.8.0b1.dist-info/entry_points.txt
 Comment: 
 
-Filename: riptide_plugin_php_xdebug-0.7.0.dist-info/top_level.txt
+Filename: riptide_plugin_php_xdebug-0.8.0b1.dist-info/top_level.txt
 Comment: 
 
-Filename: riptide_plugin_php_xdebug-0.7.0.dist-info/RECORD
+Filename: riptide_plugin_php_xdebug-0.8.0b1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `riptide_plugin_php_xdebug-0.7.0.dist-info/LICENSE` & `riptide_plugin_php_xdebug-0.8.0b1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `riptide_plugin_php_xdebug-0.7.0.dist-info/METADATA` & `riptide_plugin_php_xdebug-0.8.0b1.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 Metadata-Version: 2.1
 Name: riptide-plugin-php-xdebug
-Version: 0.7.0
+Version: 0.8.0b1
 Summary: Tool to manage development environments for web applications using containers - PHP Xdebug integration
 Home-page: https://github.com/theCapypara/riptide-plugin-php-xdebug/
 Author: Marco "theCapypara" Köpcke
 License: MIT
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
-Requires-Dist: riptide-cli (<0.8,>=0.7)
+Requires-Dist: riptide-lib (<0.9,>=0.8.0b1)
+Requires-Dist: riptide-cli (<0.9,>=0.8.0b1)
 Requires-Dist: Click (>=7.0)
 
 |Riptide|
 =========
 
 .. |Riptide| image:: https://riptide-docs.readthedocs.io/en/latest/_images/logo.png
     :alt: Riptide
@@ -49,28 +47,24 @@
 .. _docs:           https://github.com/theCapypara/riptide-docs
 .. _repo:           https://github.com/theCapypara/riptide-repo
 .. _docker_images:  https://github.com/theCapypara/riptide-docker-images
 .. _php_xdebug:     https://github.com/theCapypara/riptide-plugin-php-xdebug
 .. _k8s_client:     https://github.com/theCapypara/riptide-k8s-client
 .. _k8s_controller: https://github.com/theCapypara/riptide-k8s-controller
 
-|build| |docs| |pypi-version| |pypi-downloads| |pypi-license| |pypi-pyversions| |slack|
+|build| |docs| |pypi-version| |pypi-downloads| |pypi-license| |pypi-pyversions|
 
-.. |build| image:: https://img.shields.io/github/workflow/status/theCapypara/riptide-plugin-php-xdebug/Build,%20test%20and%20publish
+.. |build| image:: https://img.shields.io/github/actions/workflow/status/theCapypara/riptide-plugin-php-xdebug/build.yml
     :target: https://github.com/theCapypara/riptide-plugin-php-xdebug/actions
     :alt: Build Status
 
 .. |docs| image:: https://readthedocs.org/projects/riptide-docs/badge/?version=latest
     :target: https://riptide-docs.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
-.. |slack| image:: https://slack.riptide.theCapypara.de/badge.svg
-    :target: https://slack.riptide.theCapypara.de
-    :alt: Join our Slack workspace
-
 .. |pypi-version| image:: https://img.shields.io/pypi/v/riptide-plugin-php-xdebug
     :target: https://pypi.org/project/riptide-plugin-php-xdebug/
     :alt: Version
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/riptide-plugin-php-xdebug
     :target: https://pypi.org/project/riptide-plugin-php-xdebug/
     :alt: Downloads
@@ -104,8 +98,7 @@
 Sets the flag ``php-xdebug.enabled``, which can be read from Riptide configuration files to
 enable or disable Xdebug.
 
 Documentation
 -------------
 
 The complete documentation for Riptide can be found at `Read the Docs <https://riptide-docs.readthedocs.io/en/latest/>`_.
-
```

