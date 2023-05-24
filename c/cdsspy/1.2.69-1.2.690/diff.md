# Comparing `tmp/cdsspy-1.2.69.tar.gz` & `tmp/cdsspy-1.2.690.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdsspy-1.2.69.tar", last modified: Wed May 24 16:51:40 2023, max compression
+gzip compressed data, was "cdsspy-1.2.690.tar", last modified: Wed May 24 17:35:55 2023, max compression
```

## Comparing `cdsspy-1.2.69.tar` & `cdsspy-1.2.690.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 16:51:40.360302 cdsspy-1.2.69/
--rw-rw-rw-   0        0        0     1059 2023-01-10 16:17:56.000000 cdsspy-1.2.69/LICENSE
--rw-rw-rw-   0        0        0    19401 2023-05-24 16:51:40.359301 cdsspy-1.2.69/PKG-INFO
--rw-rw-rw-   0        0        0    18980 2023-01-12 17:46:31.000000 cdsspy-1.2.69/README.md
-drwxrwxrwx   0        0        0        0 2023-05-24 16:51:40.341303 cdsspy-1.2.69/cdsspy/
--rw-rw-rw-   0        0        0      293 2023-05-24 16:49:46.000000 cdsspy-1.2.69/cdsspy/__init__.py
--rw-rw-rw-   0        0        0     5079 2023-05-20 13:48:43.000000 cdsspy-1.2.69/cdsspy/admin_calls.py
--rw-rw-rw-   0        0        0    34260 2023-05-24 14:28:36.000000 cdsspy-1.2.69/cdsspy/analysis_services.py
--rw-rw-rw-   0        0        0    23277 2023-05-20 13:48:50.000000 cdsspy-1.2.69/cdsspy/climate.py
--rw-rw-rw-   0        0        0    15846 2023-05-20 13:48:51.000000 cdsspy-1.2.69/cdsspy/gw.py
--rw-rw-rw-   0        0        0    25374 2023-05-20 13:48:53.000000 cdsspy-1.2.69/cdsspy/reference_tbl.py
--rw-rw-rw-   0        0        0    34635 2023-05-20 13:48:53.000000 cdsspy-1.2.69/cdsspy/structures.py
--rw-rw-rw-   0        0        0    24840 2023-05-20 13:48:54.000000 cdsspy-1.2.69/cdsspy/sw.py
--rw-rw-rw-   0        0        0    11248 2023-05-20 13:48:55.000000 cdsspy-1.2.69/cdsspy/telemetry.py
--rw-rw-rw-   0        0        0    33575 2023-05-24 14:30:00.000000 cdsspy-1.2.69/cdsspy/utils.py
--rw-rw-rw-   0        0        0     9924 2023-05-20 13:48:57.000000 cdsspy-1.2.69/cdsspy/water_rights.py
-drwxrwxrwx   0        0        0        0 2023-05-24 16:51:40.358302 cdsspy-1.2.69/cdsspy.egg-info/
--rw-rw-rw-   0        0        0    19401 2023-05-24 16:51:40.000000 cdsspy-1.2.69/cdsspy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      392 2023-05-24 16:51:40.000000 cdsspy-1.2.69/cdsspy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 16:51:40.000000 cdsspy-1.2.69/cdsspy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-24 16:51:40.000000 cdsspy-1.2.69/cdsspy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-24 16:51:40.000000 cdsspy-1.2.69/cdsspy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-24 16:51:40.360302 cdsspy-1.2.69/setup.cfg
--rw-rw-rw-   0        0        0     1356 2023-05-24 16:50:36.000000 cdsspy-1.2.69/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 17:35:55.519964 cdsspy-1.2.690/
+-rw-rw-rw-   0        0        0     1059 2023-01-10 16:17:56.000000 cdsspy-1.2.690/LICENSE
+-rw-rw-rw-   0        0        0    19402 2023-05-24 17:35:55.519964 cdsspy-1.2.690/PKG-INFO
+-rw-rw-rw-   0        0        0    18980 2023-01-12 17:46:31.000000 cdsspy-1.2.690/README.md
+drwxrwxrwx   0        0        0        0 2023-05-24 17:35:55.482965 cdsspy-1.2.690/cdsspy/
+-rw-rw-rw-   0        0        0      294 2023-05-24 17:35:42.000000 cdsspy-1.2.690/cdsspy/__init__.py
+-rw-rw-rw-   0        0        0     5075 2023-05-24 17:35:14.000000 cdsspy-1.2.690/cdsspy/admin_calls.py
+-rw-rw-rw-   0        0        0    34256 2023-05-24 17:34:52.000000 cdsspy-1.2.690/cdsspy/analysis_services.py
+-rw-rw-rw-   0        0        0    23273 2023-05-24 17:35:03.000000 cdsspy-1.2.690/cdsspy/climate.py
+-rw-rw-rw-   0        0        0    15842 2023-05-24 17:34:51.000000 cdsspy-1.2.690/cdsspy/gw.py
+-rw-rw-rw-   0        0        0    25370 2023-05-24 17:34:49.000000 cdsspy-1.2.690/cdsspy/reference_tbl.py
+-rw-rw-rw-   0        0        0    34631 2023-05-24 17:34:50.000000 cdsspy-1.2.690/cdsspy/structures.py
+-rw-rw-rw-   0        0        0    24836 2023-05-24 17:34:18.000000 cdsspy-1.2.690/cdsspy/sw.py
+-rw-rw-rw-   0        0        0    11244 2023-05-24 17:34:21.000000 cdsspy-1.2.690/cdsspy/telemetry.py
+-rw-rw-rw-   0        0        0    33575 2023-05-24 14:30:00.000000 cdsspy-1.2.690/cdsspy/utils.py
+-rw-rw-rw-   0        0        0     9956 2023-05-24 17:34:33.000000 cdsspy-1.2.690/cdsspy/water_rights.py
+drwxrwxrwx   0        0        0        0 2023-05-24 17:35:55.516962 cdsspy-1.2.690/cdsspy.egg-info/
+-rw-rw-rw-   0        0        0    19402 2023-05-24 17:35:55.000000 cdsspy-1.2.690/cdsspy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      392 2023-05-24 17:35:55.000000 cdsspy-1.2.690/cdsspy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 17:35:55.000000 cdsspy-1.2.690/cdsspy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-24 17:35:55.000000 cdsspy-1.2.690/cdsspy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-24 17:35:55.000000 cdsspy-1.2.690/cdsspy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-24 17:35:55.520964 cdsspy-1.2.690/setup.cfg
+-rw-rw-rw-   0        0        0     1357 2023-05-24 17:35:44.000000 cdsspy-1.2.690/setup.py
```

### Comparing `cdsspy-1.2.69/LICENSE` & `cdsspy-1.2.690/LICENSE`

 * *Files identical despite different names*

### Comparing `cdsspy-1.2.69/PKG-INFO` & `cdsspy-1.2.690/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdsspy
-Version: 1.2.69
+Version: 1.2.690
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
-Metadata-Version: 2.1 Name: cdsspy Version: 1.2.69 Summary: Provides Python
+Metadata-Version: 2.1 Name: cdsspy Version: 1.2.690 Summary: Provides Python
 functions for discovering and requesting data from the CDSS REST API. Author:
 Angus Watters Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
 License-File: LICENSE # **cdsspy** [https://cdsspy-images.s3.us-west-
 1.amazonaws.com/co_dnr_div_cdss_cwcbdwr_transparent.png]  [![Dependencies]
 (https://img.shields.io/badge/dependencies-12/01-orange?style=flat)](#) [!
```

### Comparing `cdsspy-1.2.69/README.md` & `cdsspy-1.2.690/README.md`

 * *Files identical despite different names*

### Comparing `cdsspy-1.2.69/cdsspy/admin_calls.py` & `cdsspy-1.2.690/cdsspy/admin_calls.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import requests
 import datetime
 import geopandas
 import shapely
 import pyproj
 
 # from cdsspy.utils import utils2
-from src.cdsspy import utils
+from cdsspy import utils
 
 def get_admin_calls(
     division            = None,
     location_wdid       = None,
     call_number         = None,
     start_date          = None,
     end_date            = None,
```

### Comparing `cdsspy-1.2.69/cdsspy/analysis_services.py` & `cdsspy-1.2.690/cdsspy/analysis_services.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import requests
 import datetime
 import geopandas
 import shapely
 import pyproj
 
 # from cdsspy.utils import utils2
-from src.cdsspy import utils
+from cdsspy import utils
 
 def get_call_analysis_wdid(
     wdid                = None,
     admin_no            = None,
     start_date          = None,
     end_date            = None,
     batch               = False,
```

### Comparing `cdsspy-1.2.69/cdsspy/climate.py` & `cdsspy-1.2.690/cdsspy/climate.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import requests
 import datetime
 import geopandas
 import shapely
 import pyproj
 
 # from cdsspy.utils import utils2
-from src.cdsspy import utils
-
 # from .utils import shared_function
+from cdsspy import utils
+
 def get_climate_stations(
     aoi                 = None,
     radius              = None,
     county              = None,
     division            = None,
     station_name        = None,
     site_id             = None,
```

### Comparing `cdsspy-1.2.69/cdsspy/gw.py` & `cdsspy-1.2.690/cdsspy/gw.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import requests
 import datetime
 import geopandas
 import shapely
 import pyproj
 
 # from cdsspy.utils import utils2
-from src.cdsspy import utils
+from cdsspy import utils
 
 def get_gw_wl_wells(
     county              = None,
     designated_basin    = None,
     division            = None,
     management_district = None,
     water_district      = None,
```

### Comparing `cdsspy-1.2.69/cdsspy/reference_tbl.py` & `cdsspy-1.2.690/cdsspy/reference_tbl.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import requests
 import datetime
 import geopandas
 import shapely
 import pyproj
 
 # from cdsspy.utils import utils2
-from src.cdsspy import utils
+from cdsspy import utils
 
 def get_reference_tbl(
     table_name = None,
     api_key    = None
     ):
     """Return Reference Table reference table
```

### Comparing `cdsspy-1.2.69/cdsspy/structures.py` & `cdsspy-1.2.690/cdsspy/structures.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import requests
 import datetime
 import geopandas
 import shapely
 import pyproj
 
 # from cdsspy.utils import utils2
-from src.cdsspy import utils
+from cdsspy import utils
 
 def _get_structures_divrecday(
     wdid          = None,
     wc_identifier = None,
     start_date    = None,
     end_date      = None,
     api_key       = None
```

### Comparing `cdsspy-1.2.69/cdsspy/sw.py` & `cdsspy-1.2.690/cdsspy/sw.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import requests
 import datetime
 import geopandas
 import shapely
 import pyproj
 
 # from cdsspy.utils import utils2
-from src.cdsspy import utils
+from cdsspy import utils
 
 def get_sw_stations(
     aoi                 = None,
     radius              = None,
     abbrev              = None,
     county              = None,
     division            = None,
```

### Comparing `cdsspy-1.2.69/cdsspy/telemetry.py` & `cdsspy-1.2.690/cdsspy/telemetry.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import requests
 import datetime
 import geopandas
 import shapely
 import pyproj
 
 # from cdsspy.utils import utils2
-from src.cdsspy import utils
+from cdsspy import utils
 
 def get_telemetry_stations(
     aoi            = None,
     radius         = None,
     abbrev         = None,
     county         = None,
     division       = None,
```

### Comparing `cdsspy-1.2.69/cdsspy/utils.py` & `cdsspy-1.2.690/cdsspy/utils.py`

 * *Files identical despite different names*

### Comparing `cdsspy-1.2.69/cdsspy/water_rights.py` & `cdsspy-1.2.690/cdsspy/water_rights.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 import requests
 import datetime
 import geopandas
 import shapely
 import pyproj
 
 # from cdsspy.utils import utils2
-from src.cdsspy import utils
+# from cdsspy.cdsspy2 import utils
+from cdsspy import utils
 
 def get_water_rights_netamount(
     aoi                 = None,
     radius              = None, 
     county              = None,
     division            = None,
     water_district      = None,
```

### Comparing `cdsspy-1.2.69/cdsspy.egg-info/PKG-INFO` & `cdsspy-1.2.690/cdsspy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdsspy
-Version: 1.2.69
+Version: 1.2.690
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
-Metadata-Version: 2.1 Name: cdsspy Version: 1.2.69 Summary: Provides Python
+Metadata-Version: 2.1 Name: cdsspy Version: 1.2.690 Summary: Provides Python
 functions for discovering and requesting data from the CDSS REST API. Author:
 Angus Watters Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
 License-File: LICENSE # **cdsspy** [https://cdsspy-images.s3.us-west-
 1.amazonaws.com/co_dnr_div_cdss_cwcbdwr_transparent.png]  [![Dependencies]
 (https://img.shields.io/badge/dependencies-12/01-orange?style=flat)](#) [!
```

### Comparing `cdsspy-1.2.69/setup.py` & `cdsspy-1.2.690/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="cdsspy",                     # This is the name of the package
-    version="1.2.69",                        # The initial release version
+    version="1.2.690",                        # The initial release version
     author="Angus Watters",                     # Full name of the author
     description="Provides Python functions for discovering and requesting data from the CDSS REST API.",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     # packages=setuptools.find_packages(exclude=["cdsspy.egg_info"]),    # List of all python modules to be installed
     classifiers=[
```

