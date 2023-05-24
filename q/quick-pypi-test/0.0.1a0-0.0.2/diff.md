# Comparing `tmp/quick-pypi-test-0.0.1a0.tar.gz` & `tmp/quick-pypi-test-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\UIBE??\?????\????\quick-pypi\examples\dists\0.0.1a0\dist\tmpppx5lkyw\quick-pypi-test-0.0.1a0.tar", last modified: Fri Jan 28 19:04:58 2022, max compression
+gzip compressed data, was "quick-pypi-test-0.0.2.tar", last modified: Wed May 24 02:38:32 2023, max compression
```

## Comparing `quick-pypi-test-0.0.1a0.tar` & `quick-pypi-test-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2022-01-28 19:04:58.000000 quick-pypi-test-0.0.1a0/
--rw-rw-rw-   0        0        0     1086 2022-01-28 19:04:43.000000 quick-pypi-test-0.0.1a0/LICENSE
--rw-rw-rw-   0        0        0      266 2022-01-28 19:04:43.000000 quick-pypi-test-0.0.1a0/MANIFEST.in
--rw-rw-rw-   0        0        0     1059 2022-01-28 19:04:58.000000 quick-pypi-test-0.0.1a0/PKG-INFO
--rw-rw-rw-   0        0        0      180 2022-01-28 19:04:43.000000 quick-pypi-test-0.0.1a0/README.md
--rw-rw-rw-   0        0        0       81 2022-01-28 19:04:58.000000 quick-pypi-test-0.0.1a0/setup.cfg
--rw-rw-rw-   0        0        0     8618 2022-01-28 19:04:43.000000 quick-pypi-test-0.0.1a0/setup.py
-drwxrwxrwx   0        0        0        0 2022-01-28 19:04:58.000000 quick-pypi-test-0.0.1a0/src/
-drwxrwxrwx   0        0        0        0 2022-01-28 19:04:58.000000 quick-pypi-test-0.0.1a0/src/quick_pypi_test/
--rw-rw-rw-   0        0        0       40 2022-01-28 16:53:09.000000 quick-pypi-test-0.0.1a0/src/quick_pypi_test/test1.py
--rw-rw-rw-   0        0        0        0 2022-01-28 16:52:18.000000 quick-pypi-test-0.0.1a0/src/quick_pypi_test/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-28 19:04:58.000000 quick-pypi-test-0.0.1a0/src/quick_pypi_test.egg-info/
--rw-rw-rw-   0        0        0        1 2022-01-28 19:04:58.000000 quick-pypi-test-0.0.1a0/src/quick_pypi_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1059 2022-01-28 19:04:58.000000 quick-pypi-test-0.0.1a0/src/quick_pypi_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       39 2022-01-28 19:04:58.000000 quick-pypi-test-0.0.1a0/src/quick_pypi_test.egg-info/requires.txt
--rw-rw-rw-   0        0        0      323 2022-01-28 19:04:58.000000 quick-pypi-test-0.0.1a0/src/quick_pypi_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       16 2022-01-28 19:04:58.000000 quick-pypi-test-0.0.1a0/src/quick_pypi_test.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-24 02:38:32.035138 quick-pypi-test-0.0.2/
+-rw-rw-rw-   0        0        0     1086 2023-05-24 02:38:18.000000 quick-pypi-test-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      270 2023-05-24 02:38:18.000000 quick-pypi-test-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1012 2023-05-24 02:38:32.035138 quick-pypi-test-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-05-24 02:38:18.000000 quick-pypi-test-0.0.2/README.md
+-rw-rw-rw-   0        0        0       81 2023-05-24 02:38:32.039133 quick-pypi-test-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     8595 2023-05-24 02:38:18.000000 quick-pypi-test-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 02:38:32.008701 quick-pypi-test-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-24 02:38:32.018684 quick-pypi-test-0.0.2/src/quick_pypi_test/
+-rw-rw-rw-   0        0        0        0 2023-05-24 02:28:20.000000 quick-pypi-test-0.0.2/src/quick_pypi_test/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-24 02:27:50.000000 quick-pypi-test-0.0.2/src/quick_pypi_test/lib.py
+drwxrwxrwx   0        0        0        0 2023-05-24 02:38:32.034149 quick-pypi-test-0.0.2/src/quick_pypi_test.egg-info/
+-rw-rw-rw-   0        0        0     1012 2023-05-24 02:38:31.000000 quick-pypi-test-0.0.2/src/quick_pypi_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      321 2023-05-24 02:38:32.000000 quick-pypi-test-0.0.2/src/quick_pypi_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 02:38:31.000000 quick-pypi-test-0.0.2/src/quick_pypi_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-05-24 02:38:31.000000 quick-pypi-test-0.0.2/src/quick_pypi_test.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-24 02:38:31.000000 quick-pypi-test-0.0.2/src/quick_pypi_test.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `quick-pypi-test-0.0.1a0/LICENSE` & `quick-pypi-test-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `quick-pypi-test-0.0.1a0/PKG-INFO` & `quick-pypi-test-0.0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: quick-pypi-test
-Version: 0.0.1a0
+Version: 0.0.2
 Summary: This is a quick-pypi-test package!
-Home-page: UNKNOWN
 Author: Earthling
 Author-email: Earthling@Earth.org
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -25,14 +23,12 @@
 
 # quick-pypi-test
 
 This is a quick-pypi-test package!
 
 ## Installation
 ```pip
-pip install quick-pypi-test==0.0.1a0
+pip install quick-pypi-test==0.0.2
 ```
 
 ## License
 This project follows the MIT license.
-
-
```

### Comparing `quick-pypi-test-0.0.1a0/setup.py` & `quick-pypi-test-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.0.1a0',  # Required
+    version='0.0.2',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='This is a quick-pypi-test package!',  # Optional
 
     # This is an optional longer description of your project that represents
@@ -181,17 +181,17 @@
     # "scripts" keyword. Entry points provide cross-platform support and allow
     # `pip` to create the appropriate form of executable for the target
     # platform.
     #
     # For example, the following would provide a command called `sample` which
     # executes the function `main` from this package when invoked:
     entry_points={  # Optional
-        #'console_scripts': [
-        #    'sample=sample:main',
-        #],
+        'console_scripts': [
+            '',
+        ],
     },
 
     # List additional URLs that are relevant to your project as a dict.
     #
     # This field corresponds to the "Project-URL" metadata fields:
     # https://packaging.python.org/specifications/core-metadata/#project-url-multiple-use
     #
```

### Comparing `quick-pypi-test-0.0.1a0/src/quick_pypi_test.egg-info/PKG-INFO` & `quick-pypi-test-0.0.2/src/quick_pypi_test.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: quick-pypi-test
-Version: 0.0.1a0
+Version: 0.0.2
 Summary: This is a quick-pypi-test package!
-Home-page: UNKNOWN
 Author: Earthling
 Author-email: Earthling@Earth.org
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -25,14 +23,12 @@
 
 # quick-pypi-test
 
 This is a quick-pypi-test package!
 
 ## Installation
 ```pip
-pip install quick-pypi-test==0.0.1a0
+pip install quick-pypi-test==0.0.2
 ```
 
 ## License
 This project follows the MIT license.
-
-
```

