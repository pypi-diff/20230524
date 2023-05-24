# Comparing `tmp/cdsspy-1.2.66.tar.gz` & `tmp/cdsspy-1.2.67.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdsspy-1.2.66.tar", last modified: Wed May 24 15:30:02 2023, max compression
+gzip compressed data, was "cdsspy-1.2.67.tar", last modified: Wed May 24 15:57:21 2023, max compression
```

## Comparing `cdsspy-1.2.66.tar` & `cdsspy-1.2.67.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 15:30:02.988235 cdsspy-1.2.66/
--rw-rw-rw-   0        0        0     1059 2023-01-10 16:17:56.000000 cdsspy-1.2.66/LICENSE
--rw-rw-rw-   0        0        0    19401 2023-05-24 15:30:02.987234 cdsspy-1.2.66/PKG-INFO
--rw-rw-rw-   0        0        0    18980 2023-01-12 17:46:31.000000 cdsspy-1.2.66/README.md
--rw-rw-rw-   0        0        0       42 2023-05-24 15:30:02.988235 cdsspy-1.2.66/setup.cfg
--rw-rw-rw-   0        0        0     1298 2023-05-24 15:29:41.000000 cdsspy-1.2.66/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-24 15:30:02.957237 cdsspy-1.2.66/src/
-drwxrwxrwx   0        0        0        0 2023-05-24 15:30:02.986235 cdsspy-1.2.66/src/cdsspy.egg-info/
--rw-rw-rw-   0        0        0    19401 2023-05-24 15:30:02.000000 cdsspy-1.2.66/src/cdsspy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      195 2023-05-24 15:30:02.000000 cdsspy-1.2.66/src/cdsspy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 15:30:02.000000 cdsspy-1.2.66/src/cdsspy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-24 15:30:02.000000 cdsspy-1.2.66/src/cdsspy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-24 15:30:02.000000 cdsspy-1.2.66/src/cdsspy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-24 15:57:21.418125 cdsspy-1.2.67/
+-rw-rw-rw-   0        0        0     1059 2023-01-10 16:17:56.000000 cdsspy-1.2.67/LICENSE
+-rw-rw-rw-   0        0        0    19401 2023-05-24 15:57:21.418125 cdsspy-1.2.67/PKG-INFO
+-rw-rw-rw-   0        0        0    18980 2023-01-12 17:46:31.000000 cdsspy-1.2.67/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-24 15:57:21.419093 cdsspy-1.2.67/setup.cfg
+-rw-rw-rw-   0        0        0     1351 2023-05-24 15:52:06.000000 cdsspy-1.2.67/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:57:21.397442 cdsspy-1.2.67/src/
+drwxrwxrwx   0        0        0        0 2023-05-24 15:57:21.398442 cdsspy-1.2.67/src/cdsspy/
+drwxrwxrwx   0        0        0        0 2023-05-24 15:57:21.415471 cdsspy-1.2.67/src/cdsspy/cdsspy.egg-info/
+-rw-rw-rw-   0        0        0    19401 2023-05-24 15:57:21.000000 cdsspy-1.2.67/src/cdsspy/cdsspy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      434 2023-05-24 15:57:21.000000 cdsspy-1.2.67/src/cdsspy/cdsspy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 15:57:21.000000 cdsspy-1.2.67/src/cdsspy/cdsspy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-24 15:57:21.000000 cdsspy-1.2.67/src/cdsspy/cdsspy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 15:57:21.000000 cdsspy-1.2.67/src/cdsspy/cdsspy.egg-info/top_level.txt
```

### Comparing `cdsspy-1.2.66/LICENSE` & `cdsspy-1.2.67/LICENSE`

 * *Files identical despite different names*

### Comparing `cdsspy-1.2.66/PKG-INFO` & `cdsspy-1.2.67/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdsspy
-Version: 1.2.66
+Version: 1.2.67
 Summary: Provides Python functions for discovering and requesting data from the CDSS REST API.
 Author: Angus Watters
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cdsspy Version: 1.2.66 Summary: Provides Python
+Metadata-Version: 2.1 Name: cdsspy Version: 1.2.67 Summary: Provides Python
 functions for discovering and requesting data from the CDSS REST API. Author:
 Angus Watters Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
 License-File: LICENSE # **cdsspy** [https://cdsspy-images.s3.us-west-
 1.amazonaws.com/co_dnr_div_cdss_cwcbdwr_transparent.png]  [![Dependencies]
 (https://img.shields.io/badge/dependencies-12/01-orange?style=flat)](#) [!
```

### Comparing `cdsspy-1.2.66/README.md` & `cdsspy-1.2.67/README.md`

 * *Files identical despite different names*

### Comparing `cdsspy-1.2.66/setup.py` & `cdsspy-1.2.67/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="cdsspy",                     # This is the name of the package
-    version="1.2.66",                        # The initial release version
+    version="1.2.67",                        # The initial release version
     author="Angus Watters",                     # Full name of the author
     description="Provides Python functions for discovering and requesting data from the CDSS REST API.",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
-    packages=setuptools.find_packages(exclude=["cdsspy.egg_info"]),    # List of all python modules to be installed
+    packages=setuptools.find_packages(),
+    # packages=setuptools.find_packages(exclude=["cdsspy.egg_info"]),    # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],                                      # Information to filter the project on PyPi website
     python_requires='>=3.6',                # Minimum version requirement of the package
-    py_modules=["cdsspy"],             # Name of the python package
-    package_dir={'':'src'},     # Directory of the source code of the package
+    # py_modules=["cdsspy"],             # Name of the python package
+    package_dir={'':'src/cdsspy'},     # Directory of the source code of the package
     install_requires=['pandas', 'datetime', 'requests', 'geopandas', 'shapely', 'pyproj']
 )
```

### Comparing `cdsspy-1.2.66/src/cdsspy.egg-info/PKG-INFO` & `cdsspy-1.2.67/src/cdsspy/cdsspy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdsspy
-Version: 1.2.66
+Version: 1.2.67
 Summary: Provides Python functions for discovering and requesting data from the CDSS REST API.
 Author: Angus Watters
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cdsspy Version: 1.2.66 Summary: Provides Python
+Metadata-Version: 2.1 Name: cdsspy Version: 1.2.67 Summary: Provides Python
 functions for discovering and requesting data from the CDSS REST API. Author:
 Angus Watters Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
 License-File: LICENSE # **cdsspy** [https://cdsspy-images.s3.us-west-
 1.amazonaws.com/co_dnr_div_cdss_cwcbdwr_transparent.png]  [![Dependencies]
 (https://img.shields.io/badge/dependencies-12/01-orange?style=flat)](#) [!
```

