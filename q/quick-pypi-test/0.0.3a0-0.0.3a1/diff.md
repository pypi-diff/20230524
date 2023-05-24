# Comparing `tmp/quick-pypi-test-0.0.3a0.tar.gz` & `tmp/quick-pypi-test-0.0.3a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quick-pypi-test-0.0.3a0.tar", last modified: Wed May 24 04:47:49 2023, max compression
+gzip compressed data, was "quick-pypi-test-0.0.3a1.tar", last modified: Wed May 24 14:22:19 2023, max compression
```

## Comparing `quick-pypi-test-0.0.3a0.tar` & `quick-pypi-test-0.0.3a1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 04:47:49.984588 quick-pypi-test-0.0.3a0/
--rw-rw-rw-   0        0        0     1086 2023-05-24 04:47:38.000000 quick-pypi-test-0.0.3a0/LICENSE
--rw-rw-rw-   0        0        0     2582 2023-05-24 04:47:49.984588 quick-pypi-test-0.0.3a0/PKG-INFO
--rw-rw-rw-   0        0        0      191 2023-05-24 04:47:38.000000 quick-pypi-test-0.0.3a0/README.md
--rw-rw-rw-   0        0        0     6337 2023-05-24 04:47:38.000000 quick-pypi-test-0.0.3a0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-24 04:47:49.985584 quick-pypi-test-0.0.3a0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-24 04:47:49.961144 quick-pypi-test-0.0.3a0/src/
-drwxrwxrwx   0        0        0        0 2023-05-24 04:47:49.966127 quick-pypi-test-0.0.3a0/src/quick_pypi_test/
--rw-rw-rw-   0        0        0        0 2023-05-24 02:28:20.000000 quick-pypi-test-0.0.3a0/src/quick_pypi_test/__init__.py
--rw-rw-rw-   0        0        0       49 2023-05-24 02:40:30.000000 quick-pypi-test-0.0.3a0/src/quick_pypi_test/lib.py
-drwxrwxrwx   0        0        0        0 2023-05-24 04:47:49.983601 quick-pypi-test-0.0.3a0/src/quick_pypi_test.egg-info/
--rw-rw-rw-   0        0        0     2582 2023-05-24 04:47:49.000000 quick-pypi-test-0.0.3a0/src/quick_pypi_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2023-05-24 04:47:49.000000 quick-pypi-test-0.0.3a0/src/quick_pypi_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 04:47:49.000000 quick-pypi-test-0.0.3a0/src/quick_pypi_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-05-24 04:47:49.000000 quick-pypi-test-0.0.3a0/src/quick_pypi_test.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-24 04:47:49.000000 quick-pypi-test-0.0.3a0/src/quick_pypi_test.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-24 14:22:19.063489 quick-pypi-test-0.0.3a1/
+-rw-rw-rw-   0        0        0     1106 2023-05-24 14:22:08.000000 quick-pypi-test-0.0.3a1/LICENSE
+-rw-rw-rw-   0        0        0     2582 2023-05-24 14:22:19.063489 quick-pypi-test-0.0.3a1/PKG-INFO
+-rw-rw-rw-   0        0        0      191 2023-05-24 14:22:08.000000 quick-pypi-test-0.0.3a1/README.md
+-rw-rw-rw-   0        0        0     6365 2023-05-24 14:22:08.000000 quick-pypi-test-0.0.3a1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-24 14:22:19.063489 quick-pypi-test-0.0.3a1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-24 14:22:19.011230 quick-pypi-test-0.0.3a1/src/
+drwxrwxrwx   0        0        0        0 2023-05-24 14:22:19.014240 quick-pypi-test-0.0.3a1/src/quick_pypi_test/
+-rw-rw-rw-   0        0        0        0 2023-05-24 10:26:00.000000 quick-pypi-test-0.0.3a1/src/quick_pypi_test/__init__.py
+-rw-rw-rw-   0        0        0      105 2023-05-24 14:22:05.000000 quick-pypi-test-0.0.3a1/src/quick_pypi_test/lib.py
+drwxrwxrwx   0        0        0        0 2023-05-24 14:22:19.032393 quick-pypi-test-0.0.3a1/src/quick_pypi_test.egg-info/
+-rw-rw-rw-   0        0        0     2582 2023-05-24 14:22:18.000000 quick-pypi-test-0.0.3a1/src/quick_pypi_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      351 2023-05-24 14:22:18.000000 quick-pypi-test-0.0.3a1/src/quick_pypi_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 14:22:18.000000 quick-pypi-test-0.0.3a1/src/quick_pypi_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-05-24 14:22:18.000000 quick-pypi-test-0.0.3a1/src/quick_pypi_test.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       49 2023-05-24 14:22:18.000000 quick-pypi-test-0.0.3a1/src/quick_pypi_test.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-24 14:22:18.000000 quick-pypi-test-0.0.3a1/src/quick_pypi_test.egg-info/top_level.txt
```

### Comparing `quick-pypi-test-0.0.3a0/LICENSE` & `quick-pypi-test-0.0.3a1/LICENSE`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 The Python Packaging Authority
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2023 The Python Packaging Authority
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `quick-pypi-test-0.0.3a0/PKG-INFO` & `quick-pypi-test-0.0.3a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quick-pypi-test
-Version: 0.0.3a0
+Version: 0.0.3a1
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
-pip install quick-pypi-test==0.0.3a0
+pip install quick-pypi-test==0.0.3a1
 ```
 
 ## License
 This project follows the MIT license.
```

### Comparing `quick-pypi-test-0.0.3a0/pyproject.toml` & `quick-pypi-test-0.0.3a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "quick-pypi-test"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "0.0.3a0"  # Required
+version = "0.0.3a1"  # Required
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "This is a quick-pypi-test package!"  # Optional
 
 # This is an optional longer description of your project that represents
@@ -134,15 +134,15 @@
 # "Funding" = "https://donate.pypi.org"
 # "Say Thanks!" = "http://saythanks.io/to/example"
 "Source" = "https://github.com/dhchenx/quick-pypi-test/"
 
 # The following would provide a command line executable called `sample`
 # which executes the function `main` from this package when invoked.
 [project.scripts]  # Optional
-
+quick-pypi-test = 'lib:main'
 
 # This is configuration specific to the `setuptools` build backend.
 # If you are using a different build backend, you will need to change this.
 [tool.setuptools]
 # If there are data files included in your packages that need to be
 # installed, specify them here.
 # package-data = {"sample" = ["*.dat"]}
```

### Comparing `quick-pypi-test-0.0.3a0/src/quick_pypi_test.egg-info/PKG-INFO` & `quick-pypi-test-0.0.3a1/src/quick_pypi_test.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quick-pypi-test
-Version: 0.0.3a0
+Version: 0.0.3a1
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
-pip install quick-pypi-test==0.0.3a0
+pip install quick-pypi-test==0.0.3a1
 ```
 
 ## License
 This project follows the MIT license.
```

