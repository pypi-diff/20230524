# Comparing `tmp/redfin-scraper-0.2.0.tar.gz` & `tmp/redfin-scraper-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redfin-scraper-0.2.0.tar", last modified: Sat May 20 17:18:43 2023, max compression
+gzip compressed data, was "redfin-scraper-0.2.1.tar", last modified: Wed May 24 17:52:42 2023, max compression
```

## Comparing `redfin-scraper-0.2.0.tar` & `redfin-scraper-0.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 17:18:43.846596 redfin-scraper-0.2.0/
--rw-rw-rw-   0        0        0     1087 2023-03-18 00:15:21.000000 redfin-scraper-0.2.0/LICENSE.txt
--rw-rw-rw-   0        0        0     4232 2023-05-20 17:18:43.845597 redfin-scraper-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     2366 2023-05-20 17:17:34.000000 redfin-scraper-0.2.0/README.md
--rw-rw-rw-   0        0        0      904 2023-05-20 17:02:08.000000 redfin-scraper-0.2.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-20 17:18:43.816437 redfin-scraper-0.2.0/redfin_scraper/
--rw-rw-rw-   0        0        0      120 2023-05-20 17:02:04.000000 redfin-scraper-0.2.0/redfin_scraper/__init__.py
--rw-rw-rw-   0        0        0      381 2023-05-20 17:01:49.000000 redfin-scraper-0.2.0/redfin_scraper/config.py
-drwxrwxrwx   0        0        0        0 2023-05-20 17:18:43.839595 redfin-scraper-0.2.0/redfin_scraper/core/
--rw-rw-rw-   0        0        0        0 2023-03-11 03:00:34.000000 redfin-scraper-0.2.0/redfin_scraper/core/__init__.py
--rw-rw-rw-   0        0        0    12326 2023-05-20 17:01:58.000000 redfin-scraper-0.2.0/redfin_scraper/core/redfin_scraper.py
-drwxrwxrwx   0        0        0        0 2023-05-20 17:18:43.844596 redfin-scraper-0.2.0/redfin_scraper/resources/
--rw-rw-rw-   0        0        0        0 2023-02-25 20:03:01.000000 redfin-scraper-0.2.0/redfin_scraper/resources/__init__.py
--rw-rw-rw-   0        0        0     1116 2023-03-11 03:00:17.000000 redfin-scraper-0.2.0/redfin_scraper/resources/json_tools.py
--rw-rw-rw-   0        0        0     2462 2023-04-04 15:04:28.000000 redfin-scraper-0.2.0/redfin_scraper/resources/logging.py
-drwxrwxrwx   0        0        0        0 2023-05-20 17:18:43.835589 redfin-scraper-0.2.0/redfin_scraper.egg-info/
--rw-rw-rw-   0        0        0     4232 2023-05-20 17:18:43.000000 redfin-scraper-0.2.0/redfin_scraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      459 2023-05-20 17:18:43.000000 redfin-scraper-0.2.0/redfin_scraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 17:18:43.000000 redfin-scraper-0.2.0/redfin_scraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-05-20 17:18:43.000000 redfin-scraper-0.2.0/redfin_scraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-20 17:18:43.000000 redfin-scraper-0.2.0/redfin_scraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-20 17:18:43.847596 redfin-scraper-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-24 17:52:42.198446 redfin-scraper-0.2.1/
+-rw-rw-rw-   0        0        0     1087 2023-03-18 00:15:21.000000 redfin-scraper-0.2.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     4232 2023-05-24 17:52:42.197442 redfin-scraper-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2366 2023-05-20 17:17:34.000000 redfin-scraper-0.2.1/README.md
+-rw-rw-rw-   0        0        0      904 2023-05-24 17:51:29.000000 redfin-scraper-0.2.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-24 17:52:42.162021 redfin-scraper-0.2.1/redfin_scraper/
+-rw-rw-rw-   0        0        0      120 2023-05-24 17:51:32.000000 redfin-scraper-0.2.1/redfin_scraper/__init__.py
+-rw-rw-rw-   0        0        0      381 2023-05-20 17:01:49.000000 redfin-scraper-0.2.1/redfin_scraper/config.py
+drwxrwxrwx   0        0        0        0 2023-05-24 17:52:42.190448 redfin-scraper-0.2.1/redfin_scraper/core/
+-rw-rw-rw-   0        0        0        0 2023-03-11 03:00:34.000000 redfin-scraper-0.2.1/redfin_scraper/core/__init__.py
+-rw-rw-rw-   0        0        0    12424 2023-05-24 17:51:55.000000 redfin-scraper-0.2.1/redfin_scraper/core/redfin_scraper.py
+drwxrwxrwx   0        0        0        0 2023-05-24 17:52:42.195452 redfin-scraper-0.2.1/redfin_scraper/resources/
+-rw-rw-rw-   0        0        0        0 2023-02-25 20:03:01.000000 redfin-scraper-0.2.1/redfin_scraper/resources/__init__.py
+-rw-rw-rw-   0        0        0     1116 2023-03-11 03:00:17.000000 redfin-scraper-0.2.1/redfin_scraper/resources/json_tools.py
+-rw-rw-rw-   0        0        0     2445 2023-05-24 17:51:24.000000 redfin-scraper-0.2.1/redfin_scraper/resources/logging.py
+drwxrwxrwx   0        0        0        0 2023-05-24 17:52:42.187450 redfin-scraper-0.2.1/redfin_scraper.egg-info/
+-rw-rw-rw-   0        0        0     4232 2023-05-24 17:52:42.000000 redfin-scraper-0.2.1/redfin_scraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      459 2023-05-24 17:52:42.000000 redfin-scraper-0.2.1/redfin_scraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 17:52:42.000000 redfin-scraper-0.2.1/redfin_scraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-05-24 17:52:42.000000 redfin-scraper-0.2.1/redfin_scraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-24 17:52:42.000000 redfin-scraper-0.2.1/redfin_scraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-24 17:52:42.198446 redfin-scraper-0.2.1/setup.cfg
```

### Comparing `redfin-scraper-0.2.0/LICENSE.txt` & `redfin-scraper-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `redfin-scraper-0.2.0/PKG-INFO` & `redfin-scraper-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redfin-scraper
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python library used to scrape data from Redfin.com using the unofficial Stringray API.
 Author-email: Ryan Sherby <ryan.m.sherby@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Ryan Sherby
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `redfin-scraper-0.2.0/README.md` & `redfin-scraper-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `redfin-scraper-0.2.0/pyproject.toml` & `redfin-scraper-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "redfin-scraper"
-version = "0.2.0"
+version = "0.2.1"
 description = "A Python library used to scrape data from Redfin.com using the unofficial Stringray API."
 readme = "README.md"
 authors = [{ name = "Ryan Sherby", email = "ryan.m.sherby@gmail.com" }]
 license = { file = "LICENSE.txt" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `redfin-scraper-0.2.0/redfin_scraper/core/redfin_scraper.py` & `redfin-scraper-0.2.1/redfin_scraper/core/redfin_scraper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-import re
-import json
-import datetime as dt
-import time
 import itertools
 import multiprocessing
 import concurrent.futures
 import io
 import csv
 
 import requests
@@ -67,15 +63,15 @@
                 temp_zip_database_dtype=temp_zip_database.apply(lambda row:pd.to_numeric(row,errors='ignore'))
 
                 self.zip_database=temp_zip_database_dtype
                 """
 
             else:
                 try:
-                    self.zip_database=pd.read_csv(filepath_or_buffer=zip_database_path)
+                    self.zip_database=pd.read_csv(filepath_or_buffer=zip_database_path,dtype={'zip':str})
                 except:
                     raise Exception("Could not locate zip_database.csv")
 
 
 
         if multiprocessing=='True' or multiprocessing=='true' or multiprocessing == True:
             self._mp=True       
@@ -174,18 +170,19 @@
 
         if len(df_list)==0:
             self.data[self.data_id]=None
             return None
 
 
         concat_df=pd.concat(df_list,axis=0,ignore_index=True)
-        concat_df=concat_df.apply(lambda row:pd.to_numeric(row,errors='ignore'))
-        concat_df.reset_index(inplace=True,drop=True)
+        converted_df=concat_df.drop('ZIP OR POSTAL CODE',axis=1).apply(lambda row:pd.to_numeric(row,errors='ignore'))
+        converted_df.insert(6,'ZIP OR POSTAL CODE',concat_df['ZIP OR POSTAL CODE'].astype(str))
+        converted_df.reset_index(inplace=True,drop=True)
     
-        self.df=concat_df
+        self.df=converted_df
 
         self.data[self.data_id]=self.df
         return self.df
 
 
     def _core(self,zip_list):
         page_urls=self._generate_urls(zip_codes=zip_list)
```

### Comparing `redfin-scraper-0.2.0/redfin_scraper/resources/json_tools.py` & `redfin-scraper-0.2.1/redfin_scraper/resources/json_tools.py`

 * *Files identical despite different names*

### Comparing `redfin-scraper-0.2.0/redfin_scraper/resources/logging.py` & `redfin-scraper-0.2.1/redfin_scraper/resources/logging.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import functools
-import datetime
 import logging
 import time
 from queue import Queue
 
 class OrderedQueueHandler(logging.Handler):
     def __init__(self,filename):
         super().__init__()
```

### Comparing `redfin-scraper-0.2.0/redfin_scraper.egg-info/PKG-INFO` & `redfin-scraper-0.2.1/redfin_scraper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redfin-scraper
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python library used to scrape data from Redfin.com using the unofficial Stringray API.
 Author-email: Ryan Sherby <ryan.m.sherby@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Ryan Sherby
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

