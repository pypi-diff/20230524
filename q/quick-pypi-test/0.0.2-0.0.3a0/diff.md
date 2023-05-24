# Comparing `tmp/quick-pypi-test-0.0.2.tar.gz` & `tmp/quick-pypi-test-0.0.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quick-pypi-test-0.0.2.tar", last modified: Wed May 24 02:38:32 2023, max compression
+gzip compressed data, was "quick-pypi-test-0.0.3a0.tar", last modified: Wed May 24 04:47:49 2023, max compression
```

## Comparing `quick-pypi-test-0.0.2.tar` & `quick-pypi-test-0.0.3a0.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 02:38:32.035138 quick-pypi-test-0.0.2/
--rw-rw-rw-   0        0        0     1086 2023-05-24 02:38:18.000000 quick-pypi-test-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      270 2023-05-24 02:38:18.000000 quick-pypi-test-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1012 2023-05-24 02:38:32.035138 quick-pypi-test-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-05-24 02:38:18.000000 quick-pypi-test-0.0.2/README.md
--rw-rw-rw-   0        0        0       81 2023-05-24 02:38:32.039133 quick-pypi-test-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     8595 2023-05-24 02:38:18.000000 quick-pypi-test-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-24 02:38:32.008701 quick-pypi-test-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-24 02:38:32.018684 quick-pypi-test-0.0.2/src/quick_pypi_test/
--rw-rw-rw-   0        0        0        0 2023-05-24 02:28:20.000000 quick-pypi-test-0.0.2/src/quick_pypi_test/__init__.py
--rw-rw-rw-   0        0        0        0 2023-05-24 02:27:50.000000 quick-pypi-test-0.0.2/src/quick_pypi_test/lib.py
-drwxrwxrwx   0        0        0        0 2023-05-24 02:38:32.034149 quick-pypi-test-0.0.2/src/quick_pypi_test.egg-info/
--rw-rw-rw-   0        0        0     1012 2023-05-24 02:38:31.000000 quick-pypi-test-0.0.2/src/quick_pypi_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      321 2023-05-24 02:38:32.000000 quick-pypi-test-0.0.2/src/quick_pypi_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 02:38:31.000000 quick-pypi-test-0.0.2/src/quick_pypi_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-05-24 02:38:31.000000 quick-pypi-test-0.0.2/src/quick_pypi_test.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-24 02:38:31.000000 quick-pypi-test-0.0.2/src/quick_pypi_test.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-24 04:47:49.984588 quick-pypi-test-0.0.3a0/
+-rw-rw-rw-   0        0        0     1086 2023-05-24 04:47:38.000000 quick-pypi-test-0.0.3a0/LICENSE
+-rw-rw-rw-   0        0        0     2582 2023-05-24 04:47:49.984588 quick-pypi-test-0.0.3a0/PKG-INFO
+-rw-rw-rw-   0        0        0      191 2023-05-24 04:47:38.000000 quick-pypi-test-0.0.3a0/README.md
+-rw-rw-rw-   0        0        0     6337 2023-05-24 04:47:38.000000 quick-pypi-test-0.0.3a0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-24 04:47:49.985584 quick-pypi-test-0.0.3a0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-24 04:47:49.961144 quick-pypi-test-0.0.3a0/src/
+drwxrwxrwx   0        0        0        0 2023-05-24 04:47:49.966127 quick-pypi-test-0.0.3a0/src/quick_pypi_test/
+-rw-rw-rw-   0        0        0        0 2023-05-24 02:28:20.000000 quick-pypi-test-0.0.3a0/src/quick_pypi_test/__init__.py
+-rw-rw-rw-   0        0        0       49 2023-05-24 02:40:30.000000 quick-pypi-test-0.0.3a0/src/quick_pypi_test/lib.py
+drwxrwxrwx   0        0        0        0 2023-05-24 04:47:49.983601 quick-pypi-test-0.0.3a0/src/quick_pypi_test.egg-info/
+-rw-rw-rw-   0        0        0     2582 2023-05-24 04:47:49.000000 quick-pypi-test-0.0.3a0/src/quick_pypi_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2023-05-24 04:47:49.000000 quick-pypi-test-0.0.3a0/src/quick_pypi_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 04:47:49.000000 quick-pypi-test-0.0.3a0/src/quick_pypi_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-05-24 04:47:49.000000 quick-pypi-test-0.0.3a0/src/quick_pypi_test.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-24 04:47:49.000000 quick-pypi-test-0.0.3a0/src/quick_pypi_test.egg-info/top_level.txt
```

### Comparing `quick-pypi-test-0.0.2/LICENSE` & `quick-pypi-test-0.0.3a0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 The Python Packaging Authority
+Copyright (c) 2023 The Python Packaging Authority
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

