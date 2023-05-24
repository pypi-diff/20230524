# Comparing `tmp/quick-pypi-0.0.2.tar.gz` & `tmp/quick-pypi-0.0.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quick-pypi-0.0.2.tar", last modified: Fri Sep  2 04:49:22 2022, max compression
+gzip compressed data, was "quick-pypi-0.0.3a0.tar", last modified: Wed May 24 00:29:59 2023, max compression
```

## Comparing `quick-pypi-0.0.2.tar` & `quick-pypi-0.0.3a0.tar`

### file list

```diff
@@ -1,28 +1,32 @@
-drwxrwxrwx   0        0        0        0 2022-09-02 04:49:22.316953 quick-pypi-0.0.2/
--rw-rw-rw-   0        0        0     1086 2022-01-01 02:12:11.000000 quick-pypi-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      252 2022-01-17 11:10:09.000000 quick-pypi-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     4932 2022-09-02 04:49:22.316953 quick-pypi-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3705 2022-01-28 20:44:55.000000 quick-pypi-0.0.2/README.md
--rw-rw-rw-   0        0        0       81 2022-09-02 04:49:22.319945 quick-pypi-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     8561 2022-09-02 04:49:01.000000 quick-pypi-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2022-09-02 04:49:22.248483 quick-pypi-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2022-09-02 04:49:22.252472 quick-pypi-0.0.2/src/quick_pypi/
--rw-rw-rw-   0        0        0       21 2022-01-28 20:43:51.000000 quick-pypi-0.0.2/src/quick_pypi/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-02 04:49:22.273343 quick-pypi-0.0.2/src/quick_pypi/__pycache__/
--rw-rw-rw-   0        0        0      208 2022-01-28 18:44:01.000000 quick-pypi-0.0.2/src/quick_pypi/__pycache__/__init__.cpython-36.pyc
--rw-rw-rw-   0        0        0     6124 2022-01-28 19:04:43.000000 quick-pypi-0.0.2/src/quick_pypi/__pycache__/deploy.cpython-36.pyc
--rw-rw-rw-   0        0        0     9920 2022-09-02 04:49:01.000000 quick-pypi-0.0.2/src/quick_pypi/deploy.py
-drwxrwxrwx   0        0        0        0 2022-09-02 04:49:22.282029 quick-pypi-0.0.2/src/quick_pypi/template/
--rw-rw-rw-   0        0        0     1086 2022-01-01 02:12:11.000000 quick-pypi-0.0.2/src/quick_pypi/template/LICENSE
--rw-rw-rw-   0        0        0      276 2022-09-02 04:43:41.000000 quick-pypi-0.0.2/src/quick_pypi/template/MANIFEST.in
--rw-rw-rw-   0        0        0      148 2022-01-28 19:03:49.000000 quick-pypi-0.0.2/src/quick_pypi/template/README.md
--rw-rw-rw-   0        0        0      205 2022-01-28 16:39:43.000000 quick-pypi-0.0.2/src/quick_pypi/template/setup.cfg
--rw-rw-rw-   0        0        0     8397 2022-09-02 04:13:28.000000 quick-pypi-0.0.2/src/quick_pypi/template/setup.py
--rw-rw-rw-   0        0        0     8382 2022-09-02 04:13:28.000000 quick-pypi-0.0.2/src/quick_pypi/template/setup_no_urls.py
--rw-rw-rw-   0        0        0     8381 2022-09-02 04:12:11.000000 quick-pypi-0.0.2/src/quick_pypi/template/setup_with_only_project_url.py
-drwxrwxrwx   0        0        0        0 2022-09-02 04:49:22.259453 quick-pypi-0.0.2/src/quick_pypi.egg-info/
--rw-rw-rw-   0        0        0     4932 2022-09-02 04:49:21.000000 quick-pypi-0.0.2/src/quick_pypi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      654 2022-09-02 04:49:22.000000 quick-pypi-0.0.2/src/quick_pypi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-02 04:49:21.000000 quick-pypi-0.0.2/src/quick_pypi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2022-09-02 04:49:21.000000 quick-pypi-0.0.2/src/quick_pypi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2022-09-02 04:49:22.000000 quick-pypi-0.0.2/src/quick_pypi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-24 00:29:59.839199 quick-pypi-0.0.3a0/
+-rw-rw-rw-   0        0        0     1086 2022-01-01 02:12:11.000000 quick-pypi-0.0.3a0/LICENSE
+-rw-rw-rw-   0        0        0      252 2022-01-17 11:10:09.000000 quick-pypi-0.0.3a0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4911 2023-05-24 00:29:59.839199 quick-pypi-0.0.3a0/PKG-INFO
+-rw-rw-rw-   0        0        0     3705 2023-05-23 16:12:16.000000 quick-pypi-0.0.3a0/README.md
+-rw-rw-rw-   0        0        0       81 2023-05-24 00:29:59.854790 quick-pypi-0.0.3a0/setup.cfg
+-rw-rw-rw-   0        0        0     8547 2023-05-23 16:12:16.000000 quick-pypi-0.0.3a0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 00:29:59.651647 quick-pypi-0.0.3a0/src/
+drwxrwxrwx   0        0        0        0 2023-05-24 00:29:59.714285 quick-pypi-0.0.3a0/src/quick_pypi/
+-rw-rw-rw-   0        0        0       21 2022-01-28 20:43:51.000000 quick-pypi-0.0.3a0/src/quick_pypi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 00:29:59.729798 quick-pypi-0.0.3a0/src/quick_pypi/__pycache__/
+-rw-rw-rw-   0        0        0      208 2022-01-28 18:44:01.000000 quick-pypi-0.0.3a0/src/quick_pypi/__pycache__/__init__.cpython-36.pyc
+-rw-rw-rw-   0        0        0     6124 2022-01-28 19:04:43.000000 quick-pypi-0.0.3a0/src/quick_pypi/__pycache__/deploy.cpython-36.pyc
+-rw-rw-rw-   0        0        0     9920 2022-09-02 04:49:01.000000 quick-pypi-0.0.3a0/src/quick_pypi/deploy.py
+-rw-rw-rw-   0        0        0     9994 2023-05-23 16:12:16.000000 quick-pypi-0.0.3a0/src/quick_pypi/deploy_toml.py
+drwxrwxrwx   0        0        0        0 2023-05-24 00:29:59.839199 quick-pypi-0.0.3a0/src/quick_pypi/template/
+-rw-rw-rw-   0        0        0     1086 2022-01-01 02:12:11.000000 quick-pypi-0.0.3a0/src/quick_pypi/template/LICENSE
+-rw-rw-rw-   0        0        0      276 2022-09-02 04:43:41.000000 quick-pypi-0.0.3a0/src/quick_pypi/template/MANIFEST.in
+-rw-rw-rw-   0        0        0      148 2022-01-28 19:03:49.000000 quick-pypi-0.0.3a0/src/quick_pypi/template/README.md
+-rw-rw-rw-   0        0        0     6151 2023-05-23 16:12:16.000000 quick-pypi-0.0.3a0/src/quick_pypi/template/pyproject.toml
+-rw-rw-rw-   0        0        0     6159 2023-05-23 16:12:16.000000 quick-pypi-0.0.3a0/src/quick_pypi/template/pyproject_no_urls.toml
+-rw-rw-rw-   0        0        0     6155 2023-05-23 16:12:16.000000 quick-pypi-0.0.3a0/src/quick_pypi/template/pyproject_only_project_url.toml
+-rw-rw-rw-   0        0        0      205 2022-01-28 16:39:43.000000 quick-pypi-0.0.3a0/src/quick_pypi/template/setup.cfg
+-rw-rw-rw-   0        0        0     8397 2022-09-02 04:13:28.000000 quick-pypi-0.0.3a0/src/quick_pypi/template/setup.py
+-rw-rw-rw-   0        0        0     8382 2022-09-02 04:13:28.000000 quick-pypi-0.0.3a0/src/quick_pypi/template/setup_no_urls.py
+-rw-rw-rw-   0        0        0     8381 2022-09-02 04:12:11.000000 quick-pypi-0.0.3a0/src/quick_pypi/template/setup_with_only_project_url.py
+drwxrwxrwx   0        0        0        0 2023-05-24 00:29:59.729798 quick-pypi-0.0.3a0/src/quick_pypi.egg-info/
+-rw-rw-rw-   0        0        0     4911 2023-05-24 00:29:59.000000 quick-pypi-0.0.3a0/src/quick_pypi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      826 2023-05-24 00:29:59.000000 quick-pypi-0.0.3a0/src/quick_pypi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 00:29:59.000000 quick-pypi-0.0.3a0/src/quick_pypi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-05-24 00:29:59.000000 quick-pypi-0.0.3a0/src/quick_pypi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-24 00:29:59.000000 quick-pypi-0.0.3a0/src/quick_pypi.egg-info/top_level.txt
```

### Comparing `quick-pypi-0.0.2/LICENSE` & `quick-pypi-0.0.3a0/LICENSE`

 * *Files identical despite different names*

### Comparing `quick-pypi-0.0.2/PKG-INFO` & `quick-pypi-0.0.3a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: quick-pypi
-Version: 0.0.2
-Summary: The simplest and quickest way to build and upload a PyPI package
+Version: 0.0.3a0
+Summary: The simplest and quickest way to build and deploy a PyPI package
 Home-page: https://github.com/dhchenx/quick-pypi
 Author: Donghua Chen
 Author-email: douglaschan@126.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/dhchenx/quick-pypi/issues
 Project-URL: Source, https://github.com/dhchenx/quick-pypi
 Keywords: python package deployment,python library
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -24,15 +23,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
 # Quick-PyPI
 
-The simplest and quickest way to build and upload a PyPI package
+The simplest and quickest way to build and deploy a PyPI package
 
 ## Installation
 ```pip
 pip install quick-pypi
 ```
 
 ## Minimum Example
@@ -130,9 +129,7 @@
 Then, you can manually build the package through twine in the directory of `dist1`. 
 
 An example using our toolkit to deploy in the PyPI platform is demonstrated [here](https://pypi.org/project/pyrefworks/).
 
 ## License
 The `quick-pypi` project is provided by [Donghua Chen](https://github.com/dhchenx). 
 
-
-
```

### Comparing `quick-pypi-0.0.2/README.md` & `quick-pypi-0.0.3a0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Quick-PyPI
 
-The simplest and quickest way to build and upload a PyPI package
+The simplest and quickest way to build and deploy a PyPI package
 
 ## Installation
 ```pip
 pip install quick-pypi
 ```
 
 ## Minimum Example
```

### Comparing `quick-pypi-0.0.2/setup.py` & `quick-pypi-0.0.3a0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """A setuptools based setup module.
 
-The simplest and quickest way to build a Pypi package and upload to Pypi Server
+The simplest and quickest way to build and deploy a PyPI package
 
 """
 
 # Always prefer setuptools over distutils
 from setuptools import setup, find_packages
 import pathlib
 
@@ -32,20 +32,20 @@
 
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.0.2',  # Required
+    version='0.0.3a0',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
-    description='The simplest and quickest way to build and upload a PyPI package',  # Optional
+    description='The simplest and quickest way to build and deploy a PyPI package',  # Optional
 
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
     # Often, this is the same as your README, so you can just read it in from
     # that file directly (as we have already done above)
     #
@@ -198,13 +198,12 @@
     # Examples listed include a pattern for specifying where the package tracks
     # issues, where the source is hosted, where to say thanks to the package
     # maintainers, and where to support the project financially. The key is
     # what's used to render the link text on PyPI.
 
     project_urls={  # Optional
         'Bug Reports': 'https://github.com/dhchenx/quick-pypi/issues',
-
         'Source': 'https://github.com/dhchenx/quick-pypi',
     },
 
 )
```

### Comparing `quick-pypi-0.0.2/src/quick_pypi/__pycache__/deploy.cpython-36.pyc` & `quick-pypi-0.0.3a0/src/quick_pypi/__pycache__/deploy.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `quick-pypi-0.0.2/src/quick_pypi/deploy.py` & `quick-pypi-0.0.3a0/src/quick_pypi/deploy.py`

 * *Files identical despite different names*

### Comparing `quick-pypi-0.0.2/src/quick_pypi/template/LICENSE` & `quick-pypi-0.0.3a0/src/quick_pypi/template/LICENSE`

 * *Files identical despite different names*

### Comparing `quick-pypi-0.0.2/src/quick_pypi/template/setup.py` & `quick-pypi-0.0.3a0/src/quick_pypi/template/setup.py`

 * *Files identical despite different names*

### Comparing `quick-pypi-0.0.2/src/quick_pypi/template/setup_no_urls.py` & `quick-pypi-0.0.3a0/src/quick_pypi/template/setup_no_urls.py`

 * *Files identical despite different names*

### Comparing `quick-pypi-0.0.2/src/quick_pypi/template/setup_with_only_project_url.py` & `quick-pypi-0.0.3a0/src/quick_pypi/template/setup_with_only_project_url.py`

 * *Files identical despite different names*

### Comparing `quick-pypi-0.0.2/src/quick_pypi.egg-info/PKG-INFO` & `quick-pypi-0.0.3a0/src/quick_pypi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: quick-pypi
-Version: 0.0.2
-Summary: The simplest and quickest way to build and upload a PyPI package
+Version: 0.0.3a0
+Summary: The simplest and quickest way to build and deploy a PyPI package
 Home-page: https://github.com/dhchenx/quick-pypi
 Author: Donghua Chen
 Author-email: douglaschan@126.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/dhchenx/quick-pypi/issues
 Project-URL: Source, https://github.com/dhchenx/quick-pypi
 Keywords: python package deployment,python library
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -24,15 +23,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
 # Quick-PyPI
 
-The simplest and quickest way to build and upload a PyPI package
+The simplest and quickest way to build and deploy a PyPI package
 
 ## Installation
 ```pip
 pip install quick-pypi
 ```
 
 ## Minimum Example
@@ -130,9 +129,7 @@
 Then, you can manually build the package through twine in the directory of `dist1`. 
 
 An example using our toolkit to deploy in the PyPI platform is demonstrated [here](https://pypi.org/project/pyrefworks/).
 
 ## License
 The `quick-pypi` project is provided by [Donghua Chen](https://github.com/dhchenx). 
 
-
-
```

### Comparing `quick-pypi-0.0.2/src/quick_pypi.egg-info/SOURCES.txt` & `quick-pypi-0.0.3a0/src/quick_pypi.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 src/quick_pypi/__init__.py
 src/quick_pypi/deploy.py
+src/quick_pypi/deploy_toml.py
 src/quick_pypi.egg-info/PKG-INFO
 src/quick_pypi.egg-info/SOURCES.txt
 src/quick_pypi.egg-info/dependency_links.txt
 src/quick_pypi.egg-info/requires.txt
 src/quick_pypi.egg-info/top_level.txt
 src/quick_pypi/__pycache__/__init__.cpython-36.pyc
 src/quick_pypi/__pycache__/deploy.cpython-36.pyc
 src/quick_pypi/template/LICENSE
 src/quick_pypi/template/MANIFEST.in
 src/quick_pypi/template/README.md
+src/quick_pypi/template/pyproject.toml
+src/quick_pypi/template/pyproject_no_urls.toml
+src/quick_pypi/template/pyproject_only_project_url.toml
 src/quick_pypi/template/setup.cfg
 src/quick_pypi/template/setup.py
 src/quick_pypi/template/setup_no_urls.py
 src/quick_pypi/template/setup_with_only_project_url.py
```

