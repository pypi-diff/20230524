# Comparing `tmp/cdsspy-1.2.64.tar.gz` & `tmp/cdsspy-1.2.66.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdsspy-1.2.64.tar", last modified: Fri Apr  7 23:23:32 2023, max compression
+gzip compressed data, was "cdsspy-1.2.66.tar", last modified: Wed May 24 15:30:02 2023, max compression
```

## Comparing `cdsspy-1.2.64.tar` & `cdsspy-1.2.66.tar`

### file list

```diff
@@ -1,15 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 23:23:32.628079 cdsspy-1.2.64/
--rw-rw-rw-   0        0        0     1059 2023-01-10 16:17:56.000000 cdsspy-1.2.64/LICENSE
--rw-rw-rw-   0        0        0    19401 2023-04-07 23:23:32.625080 cdsspy-1.2.64/PKG-INFO
--rw-rw-rw-   0        0        0    18980 2023-01-12 17:46:31.000000 cdsspy-1.2.64/README.md
-drwxrwxrwx   0        0        0        0 2023-04-07 23:23:32.588078 cdsspy-1.2.64/cdsspy/
-drwxrwxrwx   0        0        0        0 2023-04-07 23:23:32.621079 cdsspy-1.2.64/cdsspy/src/
-drwxrwxrwx   0        0        0        0 2023-04-07 23:23:32.620078 cdsspy-1.2.64/cdsspy/src/cdsspy.egg-info/
--rw-rw-rw-   0        0        0    19401 2023-04-07 23:23:32.000000 cdsspy-1.2.64/cdsspy/src/cdsspy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      455 2023-04-07 23:23:32.000000 cdsspy-1.2.64/cdsspy/src/cdsspy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 23:23:32.000000 cdsspy-1.2.64/cdsspy/src/cdsspy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-04-07 23:23:32.000000 cdsspy-1.2.64/cdsspy/src/cdsspy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-07 23:23:32.000000 cdsspy-1.2.64/cdsspy/src/cdsspy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0   209856 2023-04-07 23:21:33.000000 cdsspy-1.2.64/cdsspy/src/cdsspy.py
--rw-rw-rw-   0        0        0       42 2023-04-07 23:23:32.628079 cdsspy-1.2.64/setup.cfg
--rw-rw-rw-   0        0        0     1278 2023-04-07 23:21:38.000000 cdsspy-1.2.64/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:30:02.988235 cdsspy-1.2.66/
+-rw-rw-rw-   0        0        0     1059 2023-01-10 16:17:56.000000 cdsspy-1.2.66/LICENSE
+-rw-rw-rw-   0        0        0    19401 2023-05-24 15:30:02.987234 cdsspy-1.2.66/PKG-INFO
+-rw-rw-rw-   0        0        0    18980 2023-01-12 17:46:31.000000 cdsspy-1.2.66/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-24 15:30:02.988235 cdsspy-1.2.66/setup.cfg
+-rw-rw-rw-   0        0        0     1298 2023-05-24 15:29:41.000000 cdsspy-1.2.66/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:30:02.957237 cdsspy-1.2.66/src/
+drwxrwxrwx   0        0        0        0 2023-05-24 15:30:02.986235 cdsspy-1.2.66/src/cdsspy.egg-info/
+-rw-rw-rw-   0        0        0    19401 2023-05-24 15:30:02.000000 cdsspy-1.2.66/src/cdsspy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      195 2023-05-24 15:30:02.000000 cdsspy-1.2.66/src/cdsspy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 15:30:02.000000 cdsspy-1.2.66/src/cdsspy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-24 15:30:02.000000 cdsspy-1.2.66/src/cdsspy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-24 15:30:02.000000 cdsspy-1.2.66/src/cdsspy.egg-info/top_level.txt
```

### Comparing `cdsspy-1.2.64/LICENSE` & `cdsspy-1.2.66/LICENSE`

 * *Files identical despite different names*

### Comparing `cdsspy-1.2.64/PKG-INFO` & `cdsspy-1.2.66/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdsspy
-Version: 1.2.64
+Version: 1.2.66
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
-Metadata-Version: 2.1 Name: cdsspy Version: 1.2.64 Summary: Provides Python
+Metadata-Version: 2.1 Name: cdsspy Version: 1.2.66 Summary: Provides Python
 functions for discovering and requesting data from the CDSS REST API. Author:
 Angus Watters Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
 License-File: LICENSE # **cdsspy** [https://cdsspy-images.s3.us-west-
 1.amazonaws.com/co_dnr_div_cdss_cwcbdwr_transparent.png]  [![Dependencies]
 (https://img.shields.io/badge/dependencies-12/01-orange?style=flat)](#) [!
```

### Comparing `cdsspy-1.2.64/README.md` & `cdsspy-1.2.66/README.md`

 * *Files identical despite different names*

### Comparing `cdsspy-1.2.64/cdsspy/src/cdsspy.egg-info/PKG-INFO` & `cdsspy-1.2.66/src/cdsspy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdsspy
-Version: 1.2.64
+Version: 1.2.66
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
-Metadata-Version: 2.1 Name: cdsspy Version: 1.2.64 Summary: Provides Python
+Metadata-Version: 2.1 Name: cdsspy Version: 1.2.66 Summary: Provides Python
 functions for discovering and requesting data from the CDSS REST API. Author:
 Angus Watters Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
 License-File: LICENSE # **cdsspy** [https://cdsspy-images.s3.us-west-
 1.amazonaws.com/co_dnr_div_cdss_cwcbdwr_transparent.png]  [![Dependencies]
 (https://img.shields.io/badge/dependencies-12/01-orange?style=flat)](#) [!
```

### Comparing `cdsspy-1.2.64/setup.py` & `cdsspy-1.2.66/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="cdsspy",                     # This is the name of the package
-    version="1.2.64",                        # The initial release version
+    version="1.2.66",                        # The initial release version
     author="Angus Watters",                     # Full name of the author
     description="Provides Python functions for discovering and requesting data from the CDSS REST API.",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
-    packages=setuptools.find_packages(),    # List of all python modules to be installed
+    packages=setuptools.find_packages(exclude=["cdsspy.egg_info"]),    # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],                                      # Information to filter the project on PyPi website
     python_requires='>=3.6',                # Minimum version requirement of the package
     py_modules=["cdsspy"],             # Name of the python package
-    package_dir={'':'cdsspy/src'},     # Directory of the source code of the package
+    package_dir={'':'src'},     # Directory of the source code of the package
     install_requires=['pandas', 'datetime', 'requests', 'geopandas', 'shapely', 'pyproj']
 )
```

