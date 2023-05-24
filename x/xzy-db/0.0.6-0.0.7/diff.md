# Comparing `tmp/xzy-db-0.0.6.tar.gz` & `tmp/xzy-db-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xzy-db-0.0.6.tar", last modified: Mon May 22 08:26:20 2023, max compression
+gzip compressed data, was "xzy-db-0.0.7.tar", last modified: Wed May 24 07:48:45 2023, max compression
```

## Comparing `xzy-db-0.0.6.tar` & `xzy-db-0.0.7.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2023-05-22 08:26:20.039002 xzy-db-0.0.6/
--rw-r--r--   0 liubola   (1000) liubola   (1000)      523 2023-05-22 08:26:20.039002 xzy-db-0.0.6/PKG-INFO
--rw-r--r--   0 liubola   (1000) liubola   (1000)       40 2023-05-22 08:05:17.000000 xzy-db-0.0.6/README.md
--rw-r--r--   0 liubola   (1000) liubola   (1000)       38 2023-05-22 08:26:20.039002 xzy-db-0.0.6/setup.cfg
--rw-r--r--   0 liubola   (1000) liubola   (1000)      904 2023-05-22 08:26:19.000000 xzy-db-0.0.6/setup.py
-drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2023-05-22 08:26:20.029002 xzy-db-0.0.6/xzy_db/
--rw-r--r--   0 liubola   (1000) liubola   (1000)       62 2023-05-22 08:05:17.000000 xzy-db-0.0.6/xzy_db/__init__.py
-drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2023-05-22 08:26:20.029002 xzy-db-0.0.6/xzy_db/api/
--rw-r--r--   0 liubola   (1000) liubola   (1000)      322 2023-05-22 08:05:17.000000 xzy-db-0.0.6/xzy_db/api/__init__.py
--rw-r--r--   0 liubola   (1000) liubola   (1000)     2174 2023-05-22 08:05:17.000000 xzy-db-0.0.6/xzy_db/api/get_fund_data.py
--rw-r--r--   0 liubola   (1000) liubola   (1000)     2781 2023-05-22 08:05:17.000000 xzy-db-0.0.6/xzy_db/api/get_fund_list.py
--rw-r--r--   0 liubola   (1000) liubola   (1000)     3262 2023-05-22 08:05:17.000000 xzy-db-0.0.6/xzy_db/api/get_index_data.py
--rw-r--r--   0 liubola   (1000) liubola   (1000)     2021 2023-05-22 08:05:17.000000 xzy-db-0.0.6/xzy_db/api/get_index_weight.py
--rw-r--r--   0 liubola   (1000) liubola   (1000)     4470 2023-05-22 08:05:17.000000 xzy-db-0.0.6/xzy_db/api/get_industry.py
--rw-r--r--   0 liubola   (1000) liubola   (1000)     3534 2023-05-22 08:05:17.000000 xzy-db-0.0.6/xzy_db/api/get_ret.py
--rw-r--r--   0 liubola   (1000) liubola   (1000)     5845 2023-05-22 08:26:16.000000 xzy-db-0.0.6/xzy_db/api/get_universe.py
-drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2023-05-22 08:26:20.029002 xzy-db-0.0.6/xzy_db/crawler/
--rw-r--r--   0 liubola   (1000) liubola   (1000)       46 2023-05-22 08:05:17.000000 xzy-db-0.0.6/xzy_db/crawler/__init__.py
-drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2023-05-22 08:26:20.029002 xzy-db-0.0.6/xzy_db/crawler/futures/
--rw-r--r--   0 liubola   (1000) liubola   (1000)        0 2023-05-22 08:05:17.000000 xzy-db-0.0.6/xzy_db/crawler/futures/__init__.py
--rw-r--r--   0 liubola   (1000) liubola   (1000)    17469 2023-05-22 08:05:17.000000 xzy-db-0.0.6/xzy_db/crawler/futures/domestic.py
--rw-r--r--   0 liubola   (1000) liubola   (1000)     5254 2023-05-22 08:05:17.000000 xzy-db-0.0.6/xzy_db/crawler/futures/domestic_cons.py
-drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2023-05-22 08:26:20.039002 xzy-db-0.0.6/xzy_db/hk_sangreal_calendar/
--rw-r--r--   0 liubola   (1000) liubola   (1000)      399 2023-05-22 08:05:17.000000 xzy-db-0.0.6/xzy_db/hk_sangreal_calendar/__init__.py
-drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2023-05-22 08:26:20.039002 xzy-db-0.0.6/xzy_db/sangreal_calendar/
--rw-r--r--   0 liubola   (1000) liubola   (1000)      397 2023-05-22 08:05:17.000000 xzy-db-0.0.6/xzy_db/sangreal_calendar/__init__.py
-drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2023-05-22 08:26:20.039002 xzy-db-0.0.6/xzy_db/utils/
--rw-r--r--   0 liubola   (1000) liubola   (1000)      112 2023-05-22 08:05:17.000000 xzy-db-0.0.6/xzy_db/utils/__init__.py
--rw-r--r--   0 liubola   (1000) liubola   (1000)     2277 2023-05-22 08:05:17.000000 xzy-db-0.0.6/xzy_db/utils/commons.py
--rw-r--r--   0 liubola   (1000) liubola   (1000)       93 2023-05-22 08:05:17.000000 xzy-db-0.0.6/xzy_db/utils/datetime_handle.py
--rw-r--r--   0 liubola   (1000) liubola   (1000)     2436 2023-05-22 08:05:17.000000 xzy-db-0.0.6/xzy_db/utils/engines.py
--rw-r--r--   0 liubola   (1000) liubola   (1000)      419 2023-05-22 08:05:17.000000 xzy-db-0.0.6/xzy_db/utils/fund_type.py
-drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2023-05-22 08:26:20.029002 xzy-db-0.0.6/xzy_db.egg-info/
--rw-r--r--   0 liubola   (1000) liubola   (1000)      523 2023-05-22 08:26:19.000000 xzy-db-0.0.6/xzy_db.egg-info/PKG-INFO
--rw-r--r--   0 liubola   (1000) liubola   (1000)      746 2023-05-22 08:26:19.000000 xzy-db-0.0.6/xzy_db.egg-info/SOURCES.txt
--rw-r--r--   0 liubola   (1000) liubola   (1000)        1 2023-05-22 08:26:19.000000 xzy-db-0.0.6/xzy_db.egg-info/dependency_links.txt
--rw-r--r--   0 liubola   (1000) liubola   (1000)       47 2023-05-22 08:26:19.000000 xzy-db-0.0.6/xzy_db.egg-info/requires.txt
--rw-r--r--   0 liubola   (1000) liubola   (1000)        7 2023-05-22 08:26:19.000000 xzy-db-0.0.6/xzy_db.egg-info/top_level.txt
+drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2023-05-24 07:48:45.190104 xzy-db-0.0.7/
+-rw-r--r--   0 liubola   (1000) liubola   (1000)      523 2023-05-24 07:48:45.190104 xzy-db-0.0.7/PKG-INFO
+-rw-r--r--   0 liubola   (1000) liubola   (1000)       40 2023-05-22 08:05:17.000000 xzy-db-0.0.7/README.md
+-rw-r--r--   0 liubola   (1000) liubola   (1000)       38 2023-05-24 07:48:45.190104 xzy-db-0.0.7/setup.cfg
+-rw-r--r--   0 liubola   (1000) liubola   (1000)      904 2023-05-24 07:48:44.000000 xzy-db-0.0.7/setup.py
+drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2023-05-24 07:48:45.180104 xzy-db-0.0.7/xzy_db/
+-rw-r--r--   0 liubola   (1000) liubola   (1000)       62 2023-05-22 08:05:17.000000 xzy-db-0.0.7/xzy_db/__init__.py
+drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2023-05-24 07:48:45.180104 xzy-db-0.0.7/xzy_db/api/
+-rw-r--r--   0 liubola   (1000) liubola   (1000)      322 2023-05-22 08:05:17.000000 xzy-db-0.0.7/xzy_db/api/__init__.py
+-rw-r--r--   0 liubola   (1000) liubola   (1000)     2174 2023-05-22 08:05:17.000000 xzy-db-0.0.7/xzy_db/api/get_fund_data.py
+-rw-r--r--   0 liubola   (1000) liubola   (1000)     2781 2023-05-22 08:05:17.000000 xzy-db-0.0.7/xzy_db/api/get_fund_list.py
+-rw-r--r--   0 liubola   (1000) liubola   (1000)     3262 2023-05-22 08:05:17.000000 xzy-db-0.0.7/xzy_db/api/get_index_data.py
+-rw-r--r--   0 liubola   (1000) liubola   (1000)     2021 2023-05-22 08:05:17.000000 xzy-db-0.0.7/xzy_db/api/get_index_weight.py
+-rw-r--r--   0 liubola   (1000) liubola   (1000)     4470 2023-05-22 08:05:17.000000 xzy-db-0.0.7/xzy_db/api/get_industry.py
+-rw-r--r--   0 liubola   (1000) liubola   (1000)     3534 2023-05-22 08:05:17.000000 xzy-db-0.0.7/xzy_db/api/get_ret.py
+-rw-r--r--   0 liubola   (1000) liubola   (1000)     5845 2023-05-22 08:26:16.000000 xzy-db-0.0.7/xzy_db/api/get_universe.py
+drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2023-05-24 07:48:45.180104 xzy-db-0.0.7/xzy_db/crawler/
+-rw-r--r--   0 liubola   (1000) liubola   (1000)       46 2023-05-22 08:05:17.000000 xzy-db-0.0.7/xzy_db/crawler/__init__.py
+drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2023-05-24 07:48:45.180104 xzy-db-0.0.7/xzy_db/crawler/futures/
+-rw-r--r--   0 liubola   (1000) liubola   (1000)        0 2023-05-22 08:05:17.000000 xzy-db-0.0.7/xzy_db/crawler/futures/__init__.py
+-rw-r--r--   0 liubola   (1000) liubola   (1000)    17469 2023-05-22 08:05:17.000000 xzy-db-0.0.7/xzy_db/crawler/futures/domestic.py
+-rw-r--r--   0 liubola   (1000) liubola   (1000)     5254 2023-05-22 08:05:17.000000 xzy-db-0.0.7/xzy_db/crawler/futures/domestic_cons.py
+drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2023-05-24 07:48:45.180104 xzy-db-0.0.7/xzy_db/hk_sangreal_calendar/
+-rw-r--r--   0 liubola   (1000) liubola   (1000)      399 2023-05-22 08:05:17.000000 xzy-db-0.0.7/xzy_db/hk_sangreal_calendar/__init__.py
+drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2023-05-24 07:48:45.180104 xzy-db-0.0.7/xzy_db/sangreal_calendar/
+-rw-r--r--   0 liubola   (1000) liubola   (1000)      397 2023-05-22 08:05:17.000000 xzy-db-0.0.7/xzy_db/sangreal_calendar/__init__.py
+drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2023-05-24 07:48:45.190104 xzy-db-0.0.7/xzy_db/utils/
+-rw-r--r--   0 liubola   (1000) liubola   (1000)      112 2023-05-22 08:05:17.000000 xzy-db-0.0.7/xzy_db/utils/__init__.py
+-rw-r--r--   0 liubola   (1000) liubola   (1000)     2277 2023-05-22 08:05:17.000000 xzy-db-0.0.7/xzy_db/utils/commons.py
+-rw-r--r--   0 liubola   (1000) liubola   (1000)       93 2023-05-22 08:05:17.000000 xzy-db-0.0.7/xzy_db/utils/datetime_handle.py
+-rw-r--r--   0 liubola   (1000) liubola   (1000)     2436 2023-05-22 08:05:17.000000 xzy-db-0.0.7/xzy_db/utils/engines.py
+-rw-r--r--   0 liubola   (1000) liubola   (1000)      419 2023-05-22 08:05:17.000000 xzy-db-0.0.7/xzy_db/utils/fund_type.py
+drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2023-05-24 07:48:45.180104 xzy-db-0.0.7/xzy_db.egg-info/
+-rw-r--r--   0 liubola   (1000) liubola   (1000)      523 2023-05-24 07:48:45.000000 xzy-db-0.0.7/xzy_db.egg-info/PKG-INFO
+-rw-r--r--   0 liubola   (1000) liubola   (1000)      746 2023-05-24 07:48:45.000000 xzy-db-0.0.7/xzy_db.egg-info/SOURCES.txt
+-rw-r--r--   0 liubola   (1000) liubola   (1000)        1 2023-05-24 07:48:45.000000 xzy-db-0.0.7/xzy_db.egg-info/dependency_links.txt
+-rw-r--r--   0 liubola   (1000) liubola   (1000)       47 2023-05-24 07:48:45.000000 xzy-db-0.0.7/xzy_db.egg-info/requires.txt
+-rw-r--r--   0 liubola   (1000) liubola   (1000)        7 2023-05-24 07:48:45.000000 xzy-db-0.0.7/xzy_db.egg-info/top_level.txt
```

### Comparing `xzy-db-0.0.6/PKG-INFO` & `xzy-db-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: xzy-db
-Version: 0.0.6
+Version: 0.0.7
 Summary: short cut api for wind
 Home-page: https://gitee.com/liubola/xzy-db
 Author: liubola
 Author-email: lby3523@gmail.com
 License: GNU General Public License v3.0
 Description: UNKNOWN
 Platform: all
```

### Comparing `xzy-db-0.0.6/setup.py` & `xzy-db-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='xzy-db',
-    version='0.0.6',
+    version='0.0.7',
     description=('short cut api for wind'),
     install_requires=[
         'sangreal-db',
         'sangreal-calendar',
         'sqlalchemy',
         'attrs',
     ],
```

### Comparing `xzy-db-0.0.6/xzy_db/api/get_fund_data.py` & `xzy-db-0.0.7/xzy_db/api/get_fund_data.py`

 * *Files identical despite different names*

### Comparing `xzy-db-0.0.6/xzy_db/api/get_fund_list.py` & `xzy-db-0.0.7/xzy_db/api/get_fund_list.py`

 * *Files identical despite different names*

### Comparing `xzy-db-0.0.6/xzy_db/api/get_index_data.py` & `xzy-db-0.0.7/xzy_db/api/get_index_data.py`

 * *Files identical despite different names*

### Comparing `xzy-db-0.0.6/xzy_db/api/get_index_weight.py` & `xzy-db-0.0.7/xzy_db/api/get_index_weight.py`

 * *Files identical despite different names*

### Comparing `xzy-db-0.0.6/xzy_db/api/get_industry.py` & `xzy-db-0.0.7/xzy_db/api/get_industry.py`

 * *Files identical despite different names*

### Comparing `xzy-db-0.0.6/xzy_db/api/get_ret.py` & `xzy-db-0.0.7/xzy_db/api/get_ret.py`

 * *Files identical despite different names*

### Comparing `xzy-db-0.0.6/xzy_db/api/get_universe.py` & `xzy-db-0.0.7/xzy_db/api/get_universe.py`

 * *Files identical despite different names*

### Comparing `xzy-db-0.0.6/xzy_db/crawler/futures/domestic.py` & `xzy-db-0.0.7/xzy_db/crawler/futures/domestic.py`

 * *Files identical despite different names*

### Comparing `xzy-db-0.0.6/xzy_db/crawler/futures/domestic_cons.py` & `xzy-db-0.0.7/xzy_db/crawler/futures/domestic_cons.py`

 * *Files identical despite different names*

### Comparing `xzy-db-0.0.6/xzy_db/utils/commons.py` & `xzy-db-0.0.7/xzy_db/utils/commons.py`

 * *Files identical despite different names*

### Comparing `xzy-db-0.0.6/xzy_db/utils/engines.py` & `xzy-db-0.0.7/xzy_db/utils/engines.py`

 * *Files identical despite different names*

### Comparing `xzy-db-0.0.6/xzy_db.egg-info/PKG-INFO` & `xzy-db-0.0.7/xzy_db.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: xzy-db
-Version: 0.0.6
+Version: 0.0.7
 Summary: short cut api for wind
 Home-page: https://gitee.com/liubola/xzy-db
 Author: liubola
 Author-email: lby3523@gmail.com
 License: GNU General Public License v3.0
 Description: UNKNOWN
 Platform: all
```

### Comparing `xzy-db-0.0.6/xzy_db.egg-info/SOURCES.txt` & `xzy-db-0.0.7/xzy_db.egg-info/SOURCES.txt`

 * *Files identical despite different names*

