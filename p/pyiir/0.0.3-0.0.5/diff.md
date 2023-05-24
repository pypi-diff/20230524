# Comparing `tmp/pyiir-0.0.3.tar.gz` & `tmp/pyiir-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiir-0.0.3.tar", last modified: Fri Nov 11 12:37:13 2022, max compression
+gzip compressed data, was "pyiir-0.0.5.tar", last modified: Wed May 24 16:09:35 2023, max compression
```

## Comparing `pyiir-0.0.3.tar` & `pyiir-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 12:37:13.750682 pyiir-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (121)      402 2022-11-11 12:37:13.750682 pyiir-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-11-11 12:37:03.000000 pyiir-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 12:37:13.750682 pyiir-0.0.3/pyiir/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 12:37:03.000000 pyiir-0.0.3/pyiir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3526 2022-11-11 12:37:03.000000 pyiir-0.0.3/pyiir/pyiir.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 12:37:13.750682 pyiir-0.0.3/pyiir.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      402 2022-11-11 12:37:13.000000 pyiir-0.0.3/pyiir.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      195 2022-11-11 12:37:13.000000 pyiir-0.0.3/pyiir.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-11 12:37:13.000000 pyiir-0.0.3/pyiir.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-11-11 12:37:13.000000 pyiir-0.0.3/pyiir.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-11-11 12:37:13.000000 pyiir-0.0.3/pyiir.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-11 12:37:13.750682 pyiir-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      624 2022-11-11 12:37:03.000000 pyiir-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:09:35.603247 pyiir-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-24 16:09:35.603247 pyiir-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-24 16:09:20.000000 pyiir-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:09:35.599247 pyiir-0.0.5/pyiir/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 16:09:20.000000 pyiir-0.0.5/pyiir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-05-24 16:09:20.000000 pyiir-0.0.5/pyiir/pyiir.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:09:35.603247 pyiir-0.0.5/pyiir.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-24 16:09:35.000000 pyiir-0.0.5/pyiir.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-24 16:09:35.000000 pyiir-0.0.5/pyiir.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 16:09:35.000000 pyiir-0.0.5/pyiir.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-24 16:09:35.000000 pyiir-0.0.5/pyiir.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-24 16:09:35.000000 pyiir-0.0.5/pyiir.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 16:09:35.603247 pyiir-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-24 16:09:20.000000 pyiir-0.0.5/setup.py
```

### Comparing `pyiir-0.0.3/pyiir/pyiir.py` & `pyiir-0.0.5/pyiir/pyiir.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os
 import pandas as pd
 from cachetools.func import ttl_cache
 
 token_url = "https://api.industrialinfo.com/idb/v1.4/token"
 offline_events_summary_url = 'https://api.industrialinfo.com/idb/v1.4/offlineevents/summary'
 
+proxies = {'http': 'proxy-rwest-uk.energy.local:8080', 'https': 'proxy-rwest-uk.energy.local:8080'}
 
 def extract_credential(key: str):
     credentials = os.getenv("IIR_API_CREDENTIALS")
     tokens = credentials.split(";")
     token = [x for x in tokens if x.startswith(key)]
     if len(token) > 0:
         s = token[0].split("=")
@@ -23,15 +24,17 @@
     :return:
     """
     params = {
         "username": extract_credential("username"),
         "password": extract_credential("password"),
         "tokeenLifeTime": 30,
     }
-    token_request = requests.post(token_url, params=params)
+
+
+    token_request = requests.post(token_url, params=params, proxies=proxies)
     req_dic = token_request.headers
     access_token = req_dic["AUTHORIZATION"]
     return access_token
 
 
 def build_header():
     header = {
@@ -39,28 +42,29 @@
         "Authorization": get_access_token(),
     }
     return header
 
 
 @ttl_cache(ttl=10 * 60)
 def summary_call(startdate: str = None, enddate: str = None, tradingRegion: str = None,
-                 unitType: str = None, country: str = None):
+                 unitType: str = None, unitTypeGroup: str = None, country: str = None):
     fin = pd.DataFrame()
     offset = 0
     while True:
         params = {
             "eventStartDateMin": startdate,
             "limit": 1000,
             'offset': offset,
             'eventEndDateMax': enddate,
             "unitTypeDesc": unitType,
+            "unitTypeGroup": unitTypeGroup,
             "physicalAddressCountryName": country,
         }
         headers = build_header()
-        response = requests.post(url=offline_events_summary_url, headers=headers, params=params)
+        response = requests.post(url=offline_events_summary_url, headers=headers, params=params, proxies=proxies)
         summary = response.json()
         if summary['resultCount'] == 0:
             break
         res = pd.DataFrame(summary['offlineEvents'])
         if tradingRegion != None:
             res = res.loc[res['tradingRegionName'] == tradingRegion]
         cols = ['eventStartDate', 'eventEndDate', 'liveDate', 'releaseDate']
@@ -75,15 +79,15 @@
 
 
 def details_call(eventId: str):
     params = {
         "eventId": eventId,
     }
     headers = build_header()
-    response = requests.post(url=offline_events_summary_url, headers=headers, params=params)
+    response = requests.post(url=offline_events_summary_url, headers=headers, params=params, proxies=proxies)
     summary = response.json()
     summary = pd.DataFrame(summary['offlineEvents'])
     return summary
 
 def tar_to_timeseries(taramount, startdate, enddate, tarname=None):
     dr = pd.date_range("01/01/2000", "12/01/2030")
     ser = pd.Series(0, index=dr)
```

