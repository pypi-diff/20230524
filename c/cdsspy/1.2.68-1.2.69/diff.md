# Comparing `tmp/cdsspy-1.2.68.tar.gz` & `tmp/cdsspy-1.2.69.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdsspy-1.2.68.tar", last modified: Wed May 24 16:17:55 2023, max compression
+gzip compressed data, was "cdsspy-1.2.69.tar", last modified: Wed May 24 16:51:40 2023, max compression
```

## Comparing `cdsspy-1.2.68.tar` & `cdsspy-1.2.69.tar`

### file list

```diff
@@ -1,14 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 16:17:55.099105 cdsspy-1.2.68/
--rw-rw-rw-   0        0        0     1059 2023-01-10 16:17:56.000000 cdsspy-1.2.68/LICENSE
--rw-rw-rw-   0        0        0    19401 2023-05-24 16:17:55.099105 cdsspy-1.2.68/PKG-INFO
--rw-rw-rw-   0        0        0    18980 2023-01-12 17:46:31.000000 cdsspy-1.2.68/README.md
-drwxrwxrwx   0        0        0        0 2023-05-24 16:17:55.073106 cdsspy-1.2.68/cdsspy/
-drwxrwxrwx   0        0        0        0 2023-05-24 16:17:55.073106 cdsspy-1.2.68/cdsspy/src/
-drwxrwxrwx   0        0        0        0 2023-05-24 16:17:55.097106 cdsspy-1.2.68/cdsspy/src/cdsspy.egg-info/
--rw-rw-rw-   0        0        0    19401 2023-05-24 16:17:54.000000 cdsspy-1.2.68/cdsspy/src/cdsspy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-05-24 16:17:55.000000 cdsspy-1.2.68/cdsspy/src/cdsspy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 16:17:54.000000 cdsspy-1.2.68/cdsspy/src/cdsspy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-24 16:17:54.000000 cdsspy-1.2.68/cdsspy/src/cdsspy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-24 16:17:54.000000 cdsspy-1.2.68/cdsspy/src/cdsspy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-24 16:17:55.099105 cdsspy-1.2.68/setup.cfg
--rw-rw-rw-   0        0        0     1349 2023-05-24 16:17:52.000000 cdsspy-1.2.68/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 16:51:40.360302 cdsspy-1.2.69/
+-rw-rw-rw-   0        0        0     1059 2023-01-10 16:17:56.000000 cdsspy-1.2.69/LICENSE
+-rw-rw-rw-   0        0        0    19401 2023-05-24 16:51:40.359301 cdsspy-1.2.69/PKG-INFO
+-rw-rw-rw-   0        0        0    18980 2023-01-12 17:46:31.000000 cdsspy-1.2.69/README.md
+drwxrwxrwx   0        0        0        0 2023-05-24 16:51:40.341303 cdsspy-1.2.69/cdsspy/
+-rw-rw-rw-   0        0        0      293 2023-05-24 16:49:46.000000 cdsspy-1.2.69/cdsspy/__init__.py
+-rw-rw-rw-   0        0        0     5079 2023-05-20 13:48:43.000000 cdsspy-1.2.69/cdsspy/admin_calls.py
+-rw-rw-rw-   0        0        0    34260 2023-05-24 14:28:36.000000 cdsspy-1.2.69/cdsspy/analysis_services.py
+-rw-rw-rw-   0        0        0    23277 2023-05-20 13:48:50.000000 cdsspy-1.2.69/cdsspy/climate.py
+-rw-rw-rw-   0        0        0    15846 2023-05-20 13:48:51.000000 cdsspy-1.2.69/cdsspy/gw.py
+-rw-rw-rw-   0        0        0    25374 2023-05-20 13:48:53.000000 cdsspy-1.2.69/cdsspy/reference_tbl.py
+-rw-rw-rw-   0        0        0    34635 2023-05-20 13:48:53.000000 cdsspy-1.2.69/cdsspy/structures.py
+-rw-rw-rw-   0        0        0    24840 2023-05-20 13:48:54.000000 cdsspy-1.2.69/cdsspy/sw.py
+-rw-rw-rw-   0        0        0    11248 2023-05-20 13:48:55.000000 cdsspy-1.2.69/cdsspy/telemetry.py
+-rw-rw-rw-   0        0        0    33575 2023-05-24 14:30:00.000000 cdsspy-1.2.69/cdsspy/utils.py
+-rw-rw-rw-   0        0        0     9924 2023-05-20 13:48:57.000000 cdsspy-1.2.69/cdsspy/water_rights.py
+drwxrwxrwx   0        0        0        0 2023-05-24 16:51:40.358302 cdsspy-1.2.69/cdsspy.egg-info/
+-rw-rw-rw-   0        0        0    19401 2023-05-24 16:51:40.000000 cdsspy-1.2.69/cdsspy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      392 2023-05-24 16:51:40.000000 cdsspy-1.2.69/cdsspy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 16:51:40.000000 cdsspy-1.2.69/cdsspy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-24 16:51:40.000000 cdsspy-1.2.69/cdsspy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-24 16:51:40.000000 cdsspy-1.2.69/cdsspy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-24 16:51:40.360302 cdsspy-1.2.69/setup.cfg
+-rw-rw-rw-   0        0        0     1356 2023-05-24 16:50:36.000000 cdsspy-1.2.69/setup.py
```

### Comparing `cdsspy-1.2.68/LICENSE` & `cdsspy-1.2.69/LICENSE`

 * *Files identical despite different names*

### Comparing `cdsspy-1.2.68/PKG-INFO` & `cdsspy-1.2.69/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdsspy
-Version: 1.2.68
+Version: 1.2.69
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
-Metadata-Version: 2.1 Name: cdsspy Version: 1.2.68 Summary: Provides Python
+Metadata-Version: 2.1 Name: cdsspy Version: 1.2.69 Summary: Provides Python
 functions for discovering and requesting data from the CDSS REST API. Author:
 Angus Watters Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
 License-File: LICENSE # **cdsspy** [https://cdsspy-images.s3.us-west-
 1.amazonaws.com/co_dnr_div_cdss_cwcbdwr_transparent.png]  [![Dependencies]
 (https://img.shields.io/badge/dependencies-12/01-orange?style=flat)](#) [!
```

### Comparing `cdsspy-1.2.68/README.md` & `cdsspy-1.2.69/README.md`

 * *Files identical despite different names*

### Comparing `cdsspy-1.2.68/cdsspy/src/cdsspy.egg-info/PKG-INFO` & `cdsspy-1.2.69/cdsspy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdsspy
-Version: 1.2.68
+Version: 1.2.69
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
-Metadata-Version: 2.1 Name: cdsspy Version: 1.2.68 Summary: Provides Python
+Metadata-Version: 2.1 Name: cdsspy Version: 1.2.69 Summary: Provides Python
 functions for discovering and requesting data from the CDSS REST API. Author:
 Angus Watters Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
 License-File: LICENSE # **cdsspy** [https://cdsspy-images.s3.us-west-
 1.amazonaws.com/co_dnr_div_cdss_cwcbdwr_transparent.png]  [![Dependencies]
 (https://img.shields.io/badge/dependencies-12/01-orange?style=flat)](#) [!
```

### Comparing `cdsspy-1.2.68/setup.py` & `cdsspy-1.2.69/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="cdsspy",                     # This is the name of the package
-    version="1.2.68",                        # The initial release version
+    version="1.2.69",                        # The initial release version
     author="Angus Watters",                     # Full name of the author
     description="Provides Python functions for discovering and requesting data from the CDSS REST API.",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     # packages=setuptools.find_packages(exclude=["cdsspy.egg_info"]),    # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],                                      # Information to filter the project on PyPi website
     python_requires='>=3.6',                # Minimum version requirement of the package
-    py_modules=["cdsspy"],             # Name of the python package
-    package_dir={'':'cdsspy/src'},     # Directory of the source code of the package
+    # py_modules=["cdsspy"],             # Name of the python package
+    # package_dir={'':'cdsspy/cdsspy'},     # Directory of the source code of the package
     install_requires=['pandas', 'datetime', 'requests', 'geopandas', 'shapely', 'pyproj']
 )
```

