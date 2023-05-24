# Comparing `tmp/psa_utils-0.2.3.tar.gz` & `tmp/psa_utils-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/psa_utils/psa_utils/dist/tmponza2yvy/psa_utils-0.2.3.tar", last modified: Thu Sep  2 12:16:34 2021, max compression
+gzip compressed data, was "psa_utils-0.2.4.tar", last modified: Wed May 24 07:32:43 2023, max compression
```

## Comparing `psa_utils-0.2.3.tar` & `psa_utils-0.2.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-09-02 12:16:34.000000 psa_utils-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (116)    35149 2021-09-02 12:16:21.000000 psa_utils-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     2163 2021-09-02 12:16:34.000000 psa_utils-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1912 2021-09-02 12:16:21.000000 psa_utils-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-09-02 12:16:34.000000 psa_utils-0.2.3/psa_utils/
--rw-r--r--   0 runner    (1001) docker     (116)      353 2021-09-02 12:16:21.000000 psa_utils-0.2.3/psa_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1552 2021-09-02 12:16:21.000000 psa_utils-0.2.3/psa_utils/common.py
--rw-r--r--   0 runner    (1001) docker     (116)     7970 2021-09-02 12:16:21.000000 psa_utils-0.2.3/psa_utils/download.py
--rw-r--r--   0 runner    (1001) docker     (116)     2786 2021-09-02 12:16:21.000000 psa_utils-0.2.3/psa_utils/geogen.py
--rw-r--r--   0 runner    (1001) docker     (116)    13907 2021-09-02 12:16:21.000000 psa_utils-0.2.3/psa_utils/internal.py
--rw-r--r--   0 runner    (1001) docker     (116)    13895 2021-09-02 12:16:21.000000 psa_utils-0.2.3/psa_utils/packager.py
--rw-r--r--   0 runner    (1001) docker     (116)     3732 2021-09-02 12:16:21.000000 psa_utils-0.2.3/psa_utils/pdap.py
--rw-r--r--   0 runner    (1001) docker     (116)     4404 2021-09-02 12:16:21.000000 psa_utils-0.2.3/psa_utils/tap.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-09-02 12:16:34.000000 psa_utils-0.2.3/psa_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     2163 2021-09-02 12:16:34.000000 psa_utils-0.2.3/psa_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      410 2021-09-02 12:16:34.000000 psa_utils-0.2.3/psa_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-09-02 12:16:34.000000 psa_utils-0.2.3/psa_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-09-02 12:16:34.000000 psa_utils-0.2.3/psa_utils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)      107 2021-09-02 12:16:34.000000 psa_utils-0.2.3/psa_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       10 2021-09-02 12:16:34.000000 psa_utils-0.2.3/psa_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      100 2021-09-02 12:16:21.000000 psa_utils-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)      469 2021-09-02 12:16:34.000000 psa_utils-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)       69 2021-09-02 12:16:21.000000 psa_utils-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:32:43.630484 psa_utils-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-24 07:32:31.000000 psa_utils-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-05-24 07:32:43.630484 psa_utils-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-05-24 07:32:31.000000 psa_utils-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:32:43.626484 psa_utils-0.2.4/psa_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-24 07:32:31.000000 psa_utils-0.2.4/psa_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-24 07:32:31.000000 psa_utils-0.2.4/psa_utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-05-24 07:32:31.000000 psa_utils-0.2.4/psa_utils/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-24 07:32:31.000000 psa_utils-0.2.4/psa_utils/geogen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29839 2023-05-24 07:32:31.000000 psa_utils-0.2.4/psa_utils/internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13894 2023-05-24 07:32:31.000000 psa_utils-0.2.4/psa_utils/packager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-05-24 07:32:31.000000 psa_utils-0.2.4/psa_utils/pdap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-05-24 07:32:31.000000 psa_utils-0.2.4/psa_utils/tap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:32:43.630484 psa_utils-0.2.4/psa_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-05-24 07:32:43.000000 psa_utils-0.2.4/psa_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-24 07:32:43.000000 psa_utils-0.2.4/psa_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 07:32:43.000000 psa_utils-0.2.4/psa_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 07:32:43.000000 psa_utils-0.2.4/psa_utils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-24 07:32:43.000000 psa_utils-0.2.4/psa_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-24 07:32:43.000000 psa_utils-0.2.4/psa_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-24 07:32:31.000000 psa_utils-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-24 07:32:43.630484 psa_utils-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-24 07:32:31.000000 psa_utils-0.2.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `psa_utils-0.2.3/LICENSE` & `psa_utils-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `psa_utils-0.2.3/PKG-INFO` & `psa_utils-0.2.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 Metadata-Version: 2.1
 Name: psa_utils
-Version: 0.2.3
+Version: 0.2.4
 Summary: A collection of PSA utilities
-Home-page: UNKNOWN
-License: UNKNOWN
 Keywords: PDS,PDS4,archive,data,PSA,ESA
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # psa_utils
 A python package for working with the ESA Planetary Science Archive. The following sub-modules are available:
 ### download
 Provides functions to help with downloading public data products using either PDAP or TAP
@@ -76,9 +73,7 @@
 The URL for the PSA can be specified when instantiating the tap class. If none is given, a default URL is used, which corresponds to the default operational server.
 
 
 
 ## Example
 
 The Jupyter notebook included with this repository shows examples of each function and module. Click [here](https://nbviewer.jupyter.org/github/msbentley/psa_utils/blob/main/psa_utils_demo.ipynb) to access the notebook!
-
-
```

### Comparing `psa_utils-0.2.3/README.md` & `psa_utils-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `psa_utils-0.2.3/psa_utils/common.py` & `psa_utils-0.2.4/psa_utils/common.py`

 * *Files identical despite different names*

### Comparing `psa_utils-0.2.3/psa_utils/download.py` & `psa_utils-0.2.4/psa_utils/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 A module to download public PSA products
 """
 
 import os
 import requests
 import re
 import pathlib
-import pandas as pd
 from lxml import etree
 
 from . import pdap
 from . import tap
 
 import logging
 log = logging.getLogger(__name__)
@@ -153,15 +152,15 @@
     then downloads each label to output_dir
     """
     epn_tap_df = get_label_urls(epn_tap_df)
     for idx, url in epn_tap_df.label_url.iteritems():
         if url is None: # skip PDS3 or proprietary labels
             continue
         filename = os.path.basename(url)
-        download_file(url, output_dir='.', output_file=filename)
+        download_file(url, output_dir=output_dir, output_file=filename)
 
     return
 
 def get_label_urls(epn_tap_df):
     """Accepts a DataFrame as returned by psa_tap.query, filters for
     PDS4 products, and finds the unique bundles.
```

### Comparing `psa_utils-0.2.3/psa_utils/geogen.py` & `psa_utils-0.2.4/psa_utils/geogen.py`

 * *Files identical despite different names*

### Comparing `psa_utils-0.2.3/psa_utils/packager.py` & `psa_utils-0.2.4/psa_utils/packager.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,15 +195,15 @@
                 filepath.append(os.path.join(pathlib.Path(product.path).parent, data_file))
 
         checksum['checksum'] = check
         checksum['filepath'] = filepath
 
         checksum_file = self.delivery_name + '-checksum_manifest.tab'
         self.checksum_file = os.path.join(self.package_dir, checksum_file)
-        checksum.to_csv(self.checksum_file, line_terminator='\r\n', sep='\t', header=False, index=False)
+        checksum.to_csv(self.checksum_file, lineterminator='\r\n', sep='\t', header=False, index=False)
         
         self.checksum_records = len(checksum)
 
         return
 
 
     def create_label(self, template=None):
```

### Comparing `psa_utils-0.2.3/psa_utils/pdap.py` & `psa_utils-0.2.4/psa_utils/pdap.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         r = requests.get(
             self._url('/metadata'),
             params={
                 'RETURN_TYPE': 'VOTABLE',
                 'RESOURE_CLASS': 'DATA_SET'}) 
         r.raise_for_status()
 
-        table = votable.parse_single_table(BytesIO(r.content), pedantic=False)
+        table = votable.parse_single_table(BytesIO(r.content), verify=False)
         data = pd.DataFrame(table.array.data)
         
         return data
 
     @exception
     def get_products(self, dataset_id):
         """Queries the meta-data endpoint for products in the dataset ID
@@ -72,15 +72,15 @@
         r = requests.get(
             self._url('/metadata'),
             params={
                 'RETURN_TYPE': 'VOTABLE',
                 'RESOURCE_CLASS': 'PRODUCT',
                 'DATA_SET_ID': dataset_id}) 
         r.raise_for_status()
-        table = votable.parse_single_table(BytesIO(r.content), pedantic=False)
+        table = votable.parse_single_table(BytesIO(r.content), verify=False)
         data = pd.DataFrame(table.array.data)
 
         # extract VIDs from the download url
         data['VID'] = data['PRODUCT.DATA_ACCESS_REFERENCE'].apply(lambda url: url.split('::')[-1])
         
         return data
 
@@ -90,15 +90,15 @@
         r = requests.get(
             self._url('/metadata'),
             params={
                 'RETURN_TYPE': 'VOTABLE',
                 'RESOURCE_CLASS': 'PRODUCT',
                 'PRODUCT_ID': product_id}) 
         r.raise_for_status()
-        table = votable.parse_single_table(BytesIO(r.content), pedantic=False)
+        table = votable.parse_single_table(BytesIO(r.content), verify=False)
         data = pd.DataFrame(table.array.data)
 
         # extract VIDs from the download url
         data['VID'] = data['PRODUCT.DATA_ACCESS_REFERENCE'].apply(lambda url: url.split('::')[-1])
         
         return data.squeeze()
 
@@ -108,15 +108,15 @@
         r = requests.get(
             self._url('/files'),
             params={
                 'RETURN_TYPE': 'VOTABLE',
                 'RESOURCE_CLASS': 'PRODUCT',
                 'DATA_SET_ID': dataset_id}) 
         r.raise_for_status()
-        table = votable.parse_single_table(BytesIO(r.content), pedantic=False)
+        table = votable.parse_single_table(BytesIO(r.content), verify=False)
         data = pd.DataFrame(table.array.data)
 
         return data
 
 
 def latest_version(lid):
     """Uses PDAP to retrieve the highest VID for a given LID"""
```

### Comparing `psa_utils-0.2.3/psa_utils/tap.py` & `psa_utils-0.2.4/psa_utils/tap.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,19 +10,20 @@
 # from astroquery.utils.tap.core import Tap
 # switching to PyVO since astroquery TAP doesn't support maxrecs
 # see https://github.com/astropy/astroquery/issues/1581
 import pyvo as vo
 import pandas as pd
 from . import common
 import time
+import numpy as np
 from requests.exceptions import HTTPError
 
 job_wait_time = 2 # seconds
 job_wait_cycles = 10
-psa_tap_url = 'https://archives.esac.esa.int/psa/epn-tap/tap/'
+psa_tap_url = 'https://archives.esac.esa.int/psa-tap/tap/'
 import logging
 log = logging.getLogger(__name__)
 logging.getLogger("astroquery").setLevel(logging.WARNING)
 
 
 class PsaTap:
 
@@ -41,15 +42,28 @@
                 data = self.tap.run_sync(q, maxrec=-1).to_table()
             except ValueError as err:
                 log.error('query error: {0}'.format(err))
                 return None
             except HTTPError as err:
                 log.error('http error: {0}'.format(err))
                 return None
+
             data = data.to_pandas()
+
+            if data.empty:
+                log.warn('no results returned')
+                return None
+            
+            # check for byte encoded (object) strings and decode to utf-8
+            for col, dtype in data.dtypes.items():
+                if dtype == np.object_:
+                    # check if we really have bytes here or a string
+                    if not isinstance(data[col].iloc[0], str):
+                        data[col] = data[col].str.decode('utf-8')
+
         else:
             log.error('async jobs currently disabled')
             return None
             job = self.tap.run_async(q, maxrec=-1)
             for i in range(job_wait_cycles):
                 time.sleep(job_wait_time)
                 if job.is_finished():
@@ -86,17 +100,23 @@
     return product_id
 
 
 def get_missions():
     tap = PsaTap()
     return tap.query('SELECT DISTINCT instrument_host_name from EPN_CORE').squeeze().tolist()
 
-def get_instruments():
+def get_instruments(mission=None):
     tap = PsaTap()
-    return tap.query('SELECT DISTINCT instrument_name from EPN_CORE').squeeze().tolist()
+
+    if mission is None:
+        instruments = tap.query('SELECT DISTINCT instrument_name from EPN_CORE').squeeze().tolist()
+    else:
+        instruments = tap.query("SELECT DISTINCT instrument_name from EPN_CORE where instrument_host_name='{:s}'".format(mission)).squeeze().tolist()
+
+    return instruments
 
 def get_collections(bundle_id):
      tap = PsaTap()
      return tap.query("select distinct granule_gid from epn_core where granule_gid like 'urn:esa:psa:{:s}:%%'".format(bundle_id))
 
 
 def summarise_mission(mission_name, pretty=True):
@@ -110,21 +130,25 @@
         tap = PsaTap()
         result = tap.query("SELECT instrument_name, count(*) FROM epn_core WHERE instrument_host_name='{:s}' GROUP BY instrument_name".format(mission[0]))
         if pretty:
             common.printtable(result)
         return result
 
 
-def summarise_instrument(instrument_name, pretty=False):
+def summarise_instrument(instrument_name, ignore_levels=False, pretty=False):
  
     instruments = get_instruments()
     instrument = [name for name in instruments if name.lower()==instrument_name.lower()]
     if len(instrument)==0:
         log.error('instrument name {:s} not found'.format(instrument_name))
         return None
     else:
         tap = PsaTap()
-        result = tap.query("SELECT processing_level, count(*) FROM epn_core WHERE instrument_name='{:s}' AND processing_level IS NOT NULL GROUP BY processing_level ORDER BY processing_level".format(instrument[0]))
+
+        if ignore_levels:
+            result = tap.query("SELECT count(*) FROM epn_core WHERE instrument_name='{:s}'".format(instrument[0]))
+        else:
+            result = tap.query("SELECT processing_level, count(*) FROM epn_core WHERE instrument_name='{:s}' AND processing_level IS NOT NULL GROUP BY processing_level ORDER BY processing_level".format(instrument[0]))
         if pretty:
             common.printtable(result)
         return result
```

### Comparing `psa_utils-0.2.3/psa_utils.egg-info/PKG-INFO` & `psa_utils-0.2.4/psa_utils.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 Metadata-Version: 2.1
 Name: psa-utils
-Version: 0.2.3
+Version: 0.2.4
 Summary: A collection of PSA utilities
-Home-page: UNKNOWN
-License: UNKNOWN
 Keywords: PDS,PDS4,archive,data,PSA,ESA
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # psa_utils
 A python package for working with the ESA Planetary Science Archive. The following sub-modules are available:
 ### download
 Provides functions to help with downloading public data products using either PDAP or TAP
@@ -76,9 +73,7 @@
 The URL for the PSA can be specified when instantiating the tap class. If none is given, a default URL is used, which corresponds to the default operational server.
 
 
 
 ## Example
 
 The Jupyter notebook included with this repository shows examples of each function and module. Click [here](https://nbviewer.jupyter.org/github/msbentley/psa_utils/blob/main/psa_utils_demo.ipynb) to access the notebook!
-
-
```

