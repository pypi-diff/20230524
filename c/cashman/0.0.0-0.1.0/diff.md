# Comparing `tmp/cashman-0.0.0.tar.gz` & `tmp/cashman-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cashman-0.0.0.tar", last modified: Wed Apr 26 02:10:36 2023, max compression
+gzip compressed data, was "cashman-0.1.0.tar", last modified: Wed May 24 03:58:51 2023, max compression
```

## Comparing `cashman-0.0.0.tar` & `cashman-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 jaybee    (1000) jaybee    (1000)        0 2023-04-26 02:10:36.608842 cashman-0.0.0/
--rw-rw-r--   0 jaybee    (1000) jaybee    (1000)     1058 2023-04-26 02:10:36.608842 cashman-0.0.0/PKG-INFO
--rw-rw-r--   0 jaybee    (1000) jaybee    (1000)      401 2023-04-26 00:48:15.000000 cashman-0.0.0/README.md
-drwxrwxr-x   0 jaybee    (1000) jaybee    (1000)        0 2023-04-26 02:10:36.608842 cashman-0.0.0/cashman/
--rw-rw-r--   0 jaybee    (1000) jaybee    (1000)        0 2023-04-26 01:43:51.000000 cashman-0.0.0/cashman/__init__.py
--rw-rw-r--   0 jaybee    (1000) jaybee    (1000)      123 2023-04-26 01:53:40.000000 cashman-0.0.0/cashman/__main__.py
-drwxrwxr-x   0 jaybee    (1000) jaybee    (1000)        0 2023-04-26 02:10:36.608842 cashman-0.0.0/cashman.egg-info/
--rw-rw-r--   0 jaybee    (1000) jaybee    (1000)     1058 2023-04-26 02:10:36.000000 cashman-0.0.0/cashman.egg-info/PKG-INFO
--rw-rw-r--   0 jaybee    (1000) jaybee    (1000)      246 2023-04-26 02:10:36.000000 cashman-0.0.0/cashman.egg-info/SOURCES.txt
--rw-rw-r--   0 jaybee    (1000) jaybee    (1000)        1 2023-04-26 02:10:36.000000 cashman-0.0.0/cashman.egg-info/dependency_links.txt
--rw-rw-r--   0 jaybee    (1000) jaybee    (1000)       51 2023-04-26 02:10:36.000000 cashman-0.0.0/cashman.egg-info/entry_points.txt
--rw-rw-r--   0 jaybee    (1000) jaybee    (1000)       58 2023-04-26 02:10:36.000000 cashman-0.0.0/cashman.egg-info/requires.txt
--rw-rw-r--   0 jaybee    (1000) jaybee    (1000)        8 2023-04-26 02:10:36.000000 cashman-0.0.0/cashman.egg-info/top_level.txt
--rw-rw-r--   0 jaybee    (1000) jaybee    (1000)       38 2023-04-26 02:10:36.608842 cashman-0.0.0/setup.cfg
--rw-rw-r--   0 jaybee    (1000) jaybee    (1000)     1170 2023-04-26 02:10:15.000000 cashman-0.0.0/setup.py
+drwxrwxr-x   0 jaybee    (1000) jaybee    (1000)        0 2023-05-24 03:58:51.489489 cashman-0.1.0/
+-rw-rw-r--   0 jaybee    (1000) jaybee    (1000)     1031 2023-05-24 03:58:51.489489 cashman-0.1.0/PKG-INFO
+-rw-rw-r--   0 jaybee    (1000) jaybee    (1000)      401 2023-04-26 00:48:15.000000 cashman-0.1.0/README.md
+drwxrwxr-x   0 jaybee    (1000) jaybee    (1000)        0 2023-05-24 03:58:51.489489 cashman-0.1.0/cashman/
+-rw-rw-r--   0 jaybee    (1000) jaybee    (1000)        0 2023-04-26 01:43:51.000000 cashman-0.1.0/cashman/__init__.py
+-rw-rw-r--   0 jaybee    (1000) jaybee    (1000)     3560 2023-05-24 03:48:09.000000 cashman-0.1.0/cashman/__main__.py
+drwxrwxr-x   0 jaybee    (1000) jaybee    (1000)        0 2023-05-24 03:58:51.489489 cashman-0.1.0/cashman.egg-info/
+-rw-rw-r--   0 jaybee    (1000) jaybee    (1000)     1031 2023-05-24 03:58:51.000000 cashman-0.1.0/cashman.egg-info/PKG-INFO
+-rw-rw-r--   0 jaybee    (1000) jaybee    (1000)      256 2023-05-24 03:58:51.000000 cashman-0.1.0/cashman.egg-info/SOURCES.txt
+-rw-rw-r--   0 jaybee    (1000) jaybee    (1000)        1 2023-05-24 03:58:51.000000 cashman-0.1.0/cashman.egg-info/dependency_links.txt
+-rw-rw-r--   0 jaybee    (1000) jaybee    (1000)       53 2023-05-24 03:58:51.000000 cashman-0.1.0/cashman.egg-info/entry_points.txt
+-rw-rw-r--   0 jaybee    (1000) jaybee    (1000)       72 2023-05-24 03:58:51.000000 cashman-0.1.0/cashman.egg-info/requires.txt
+-rw-rw-r--   0 jaybee    (1000) jaybee    (1000)        8 2023-05-24 03:58:51.000000 cashman-0.1.0/cashman.egg-info/top_level.txt
+-rw-rw-r--   0 jaybee    (1000) jaybee    (1000)      960 2023-05-24 03:58:51.489489 cashman-0.1.0/setup.cfg
+-rw-rw-r--   0 jaybee    (1000) jaybee    (1000)       69 2023-05-22 06:21:34.000000 cashman-0.1.0/setup.py
```

### Comparing `cashman-0.0.0/PKG-INFO` & `cashman-0.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: cashman
-Version: 0.0.0
-Summary: A cli tool to track personal expenses
+Version: 0.1.0
+Summary: A cli personal expenses tracker
 Home-page: https://github.com/LordUbuntu/cash-man
 Author: Jacobus Burger
 Author-email: therealjacoburger@gmail.com
-License: Unlicense
+License: MIT
 Keywords: python,expense tracker,personal finance,finance,cli
-Platform: any
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Utilities
 Classifier: Environment :: Console
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -27,9 +26,7 @@
 Cashman uses rich and click to provide a straight-forward eye-candy cli experience for users. Expenses are tracked using CSV files to ensure maximum portability and interoperability for any personal financial workflow.
 
 For usage info, run `cashman --help`
 
 ## Notes
 
 May switch to Poetry for packaging in the future...
-
-
```

### Comparing `cashman-0.0.0/cashman.egg-info/PKG-INFO` & `cashman-0.1.0/cashman.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: cashman
-Version: 0.0.0
-Summary: A cli tool to track personal expenses
+Version: 0.1.0
+Summary: A cli personal expenses tracker
 Home-page: https://github.com/LordUbuntu/cash-man
 Author: Jacobus Burger
 Author-email: therealjacoburger@gmail.com
-License: Unlicense
+License: MIT
 Keywords: python,expense tracker,personal finance,finance,cli
-Platform: any
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Utilities
 Classifier: Environment :: Console
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -27,9 +26,7 @@
 Cashman uses rich and click to provide a straight-forward eye-candy cli experience for users. Expenses are tracked using CSV files to ensure maximum portability and interoperability for any personal financial workflow.
 
 For usage info, run `cashman --help`
 
 ## Notes
 
 May switch to Poetry for packaging in the future...
-
-
```

