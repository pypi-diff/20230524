# Comparing `tmp/quick-pypi-test-0.0.3a2.tar.gz` & `tmp/quick-pypi-test-0.0.3a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quick-pypi-test-0.0.3a2.tar", last modified: Wed May 24 14:37:35 2023, max compression
+gzip compressed data, was "quick-pypi-test-0.0.3a3.tar", last modified: Wed May 24 14:39:29 2023, max compression
```

## Comparing `quick-pypi-test-0.0.3a2.tar` & `quick-pypi-test-0.0.3a3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 14:37:35.095254 quick-pypi-test-0.0.3a2/
--rw-rw-rw-   0        0        0     1106 2023-05-24 14:37:25.000000 quick-pypi-test-0.0.3a2/LICENSE
--rw-rw-rw-   0        0        0     2582 2023-05-24 14:37:35.095254 quick-pypi-test-0.0.3a2/PKG-INFO
--rw-rw-rw-   0        0        0      191 2023-05-24 14:37:25.000000 quick-pypi-test-0.0.3a2/README.md
--rw-rw-rw-   0        0        0     6384 2023-05-24 14:37:25.000000 quick-pypi-test-0.0.3a2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-24 14:37:35.095254 quick-pypi-test-0.0.3a2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-24 14:37:35.060554 quick-pypi-test-0.0.3a2/src/
-drwxrwxrwx   0        0        0        0 2023-05-24 14:37:35.077846 quick-pypi-test-0.0.3a2/src/quick_pypi_test/
--rw-rw-rw-   0        0        0        0 2023-05-24 10:26:00.000000 quick-pypi-test-0.0.3a2/src/quick_pypi_test/__init__.py
--rw-rw-rw-   0        0        0      105 2023-05-24 14:22:05.000000 quick-pypi-test-0.0.3a2/src/quick_pypi_test/lib.py
-drwxrwxrwx   0        0        0        0 2023-05-24 14:37:35.094256 quick-pypi-test-0.0.3a2/src/quick_pypi_test.egg-info/
--rw-rw-rw-   0        0        0     2582 2023-05-24 14:37:35.000000 quick-pypi-test-0.0.3a2/src/quick_pypi_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      351 2023-05-24 14:37:35.000000 quick-pypi-test-0.0.3a2/src/quick_pypi_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 14:37:35.000000 quick-pypi-test-0.0.3a2/src/quick_pypi_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-05-24 14:37:35.000000 quick-pypi-test-0.0.3a2/src/quick_pypi_test.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       49 2023-05-24 14:37:35.000000 quick-pypi-test-0.0.3a2/src/quick_pypi_test.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-24 14:37:35.000000 quick-pypi-test-0.0.3a2/src/quick_pypi_test.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-24 14:39:29.867447 quick-pypi-test-0.0.3a3/
+-rw-rw-rw-   0        0        0     1106 2023-05-24 14:39:20.000000 quick-pypi-test-0.0.3a3/LICENSE
+-rw-rw-rw-   0        0        0     2582 2023-05-24 14:39:29.866446 quick-pypi-test-0.0.3a3/PKG-INFO
+-rw-rw-rw-   0        0        0      191 2023-05-24 14:39:20.000000 quick-pypi-test-0.0.3a3/README.md
+-rw-rw-rw-   0        0        0     6384 2023-05-24 14:39:20.000000 quick-pypi-test-0.0.3a3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-24 14:39:29.868460 quick-pypi-test-0.0.3a3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-24 14:39:29.842444 quick-pypi-test-0.0.3a3/src/
+drwxrwxrwx   0        0        0        0 2023-05-24 14:39:29.847444 quick-pypi-test-0.0.3a3/src/quick_pypi_test/
+-rw-rw-rw-   0        0        0       47 2023-05-24 14:38:32.000000 quick-pypi-test-0.0.3a3/src/quick_pypi_test/__init__.py
+-rw-rw-rw-   0        0        0      105 2023-05-24 14:22:05.000000 quick-pypi-test-0.0.3a3/src/quick_pypi_test/lib.py
+drwxrwxrwx   0        0        0        0 2023-05-24 14:39:29.864452 quick-pypi-test-0.0.3a3/src/quick_pypi_test.egg-info/
+-rw-rw-rw-   0        0        0     2582 2023-05-24 14:39:29.000000 quick-pypi-test-0.0.3a3/src/quick_pypi_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      351 2023-05-24 14:39:29.000000 quick-pypi-test-0.0.3a3/src/quick_pypi_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 14:39:29.000000 quick-pypi-test-0.0.3a3/src/quick_pypi_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-05-24 14:39:29.000000 quick-pypi-test-0.0.3a3/src/quick_pypi_test.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       49 2023-05-24 14:39:29.000000 quick-pypi-test-0.0.3a3/src/quick_pypi_test.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-24 14:39:29.000000 quick-pypi-test-0.0.3a3/src/quick_pypi_test.egg-info/top_level.txt
```

### Comparing `quick-pypi-test-0.0.3a2/LICENSE` & `quick-pypi-test-0.0.3a3/LICENSE`

 * *Files identical despite different names*

### Comparing `quick-pypi-test-0.0.3a2/PKG-INFO` & `quick-pypi-test-0.0.3a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quick-pypi-test
-Version: 0.0.3a2
+Version: 0.0.3a3
 Summary: This is a quick-pypi-test package!
 Author-email: Donghua Chen <douglaschan@126.com>
 License: MIT License
         
         Copyright (c) 2023 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -47,12 +47,12 @@
 
 # A quick-pypi-test package!
 
 This is a quick-pypi-test package!
 
 ## Installation
 ```pip
-pip install quick-pypi-test==0.0.3a2
+pip install quick-pypi-test==0.0.3a3
 ```
 
 ## License
 This project follows the MIT license.
```

### Comparing `quick-pypi-test-0.0.3a2/pyproject.toml` & `quick-pypi-test-0.0.3a3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "quick-pypi-test"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "0.0.3a2"  # Required
+version = "0.0.3a3"  # Required
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "This is a quick-pypi-test package!"  # Optional
 
 # This is an optional longer description of your project that represents
```

### Comparing `quick-pypi-test-0.0.3a2/src/quick_pypi_test.egg-info/PKG-INFO` & `quick-pypi-test-0.0.3a3/src/quick_pypi_test.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quick-pypi-test
-Version: 0.0.3a2
+Version: 0.0.3a3
 Summary: This is a quick-pypi-test package!
 Author-email: Donghua Chen <douglaschan@126.com>
 License: MIT License
         
         Copyright (c) 2023 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -47,12 +47,12 @@
 
 # A quick-pypi-test package!
 
 This is a quick-pypi-test package!
 
 ## Installation
 ```pip
-pip install quick-pypi-test==0.0.3a2
+pip install quick-pypi-test==0.0.3a3
 ```
 
 ## License
 This project follows the MIT license.
```

