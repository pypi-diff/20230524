# Comparing `tmp/pyiir-0.0.5.tar.gz` & `tmp/pyiir-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiir-0.0.5.tar", last modified: Wed May 24 16:09:35 2023, max compression
+gzip compressed data, was "pyiir-0.0.6.tar", last modified: Wed May 24 16:14:38 2023, max compression
```

## Comparing `pyiir-0.0.5.tar` & `pyiir-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:09:35.603247 pyiir-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-24 16:09:35.603247 pyiir-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-24 16:09:20.000000 pyiir-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:09:35.599247 pyiir-0.0.5/pyiir/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 16:09:20.000000 pyiir-0.0.5/pyiir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-05-24 16:09:20.000000 pyiir-0.0.5/pyiir/pyiir.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:09:35.603247 pyiir-0.0.5/pyiir.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-24 16:09:35.000000 pyiir-0.0.5/pyiir.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-24 16:09:35.000000 pyiir-0.0.5/pyiir.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 16:09:35.000000 pyiir-0.0.5/pyiir.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-24 16:09:35.000000 pyiir-0.0.5/pyiir.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-24 16:09:35.000000 pyiir-0.0.5/pyiir.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 16:09:35.603247 pyiir-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-24 16:09:20.000000 pyiir-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:14:38.914247 pyiir-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-24 16:14:38.914247 pyiir-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-24 16:14:28.000000 pyiir-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:14:38.914247 pyiir-0.0.6/pyiir/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 16:14:28.000000 pyiir-0.0.6/pyiir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-05-24 16:14:28.000000 pyiir-0.0.6/pyiir/pyiir.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:14:38.914247 pyiir-0.0.6/pyiir.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-24 16:14:38.000000 pyiir-0.0.6/pyiir.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-24 16:14:38.000000 pyiir-0.0.6/pyiir.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 16:14:38.000000 pyiir-0.0.6/pyiir.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-24 16:14:38.000000 pyiir-0.0.6/pyiir.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-24 16:14:38.000000 pyiir-0.0.6/pyiir.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 16:14:38.914247 pyiir-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-24 16:14:28.000000 pyiir-0.0.6/setup.py
```

### Comparing `pyiir-0.0.5/pyiir/pyiir.py` & `pyiir-0.0.6/pyiir/pyiir.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,17 +91,17 @@
 def tar_to_timeseries(taramount, startdate, enddate, tarname=None):
     dr = pd.date_range("01/01/2000", "12/01/2030")
     ser = pd.Series(0, index=dr)
     ser[startdate:enddate] = taramount
     ser.name = tarname
     return ser
 
-def create_offline_dataset(startdate: str, enddate: str, tradingRegion: str, unitType: str, country: str):
+def create_offline_dataset(startdate: str, enddate: str, tradingRegion: str, unitTypeGroup: str, country: str):
     df = pd.DataFrame()
-    fin = summary_call(startdate, enddate, tradingRegion, unitType, country)
+    fin = summary_call(startdate, enddate, tradingRegion, unitTypeGroup, country)
     for index, row in fin.iterrows():
         row = tar_to_timeseries(row['capacityOffline'], row['eventStartDate'], row['eventEndDate'])
         df = pd.concat([df, row], axis=1)
     df = (df.sum(axis=1)) / 1000
     df = df.rename('capacityOffline')
     df = df.to_frame()
     return df
```

### Comparing `pyiir-0.0.5/setup.py` & `pyiir-0.0.6/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="pyiir",
-    version="0.0.5",
+    version="0.0.6",
     author="jalex1",
     description="Wrapper around IIR",
     url="https://github.com/aeorxc/pyiir",
     project_urls={
         "Source": "https://github.com/aeorxc/pyiir",
     },
     packages=setuptools.find_packages(),
```

