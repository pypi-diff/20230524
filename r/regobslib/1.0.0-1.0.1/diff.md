# Comparing `tmp/regobslib-1.0.0.tar.gz` & `tmp/regobslib-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regobslib-1.0.0.tar", last modified: Thu Sep  1 13:42:14 2022, max compression
+gzip compressed data, was "regobslib-1.0.1.tar", last modified: Wed Nov 30 15:24:55 2022, max compression
```

## Comparing `regobslib-1.0.0.tar` & `regobslib-1.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 aron      (1000) aron      (1000)        0 2022-09-01 13:42:14.267764 regobslib-1.0.0/
--rw-rw-r--   0 aron      (1000) aron      (1000)        0 2021-08-23 07:22:18.000000 regobslib-1.0.0/LICENSE
--rw-rw-r--   0 aron      (1000) aron      (1000)     3662 2022-09-01 13:42:14.267764 regobslib-1.0.0/PKG-INFO
--rw-rw-r--   0 aron      (1000) aron      (1000)     3188 2022-02-08 10:10:03.000000 regobslib-1.0.0/README.md
--rw-rw-r--   0 aron      (1000) aron      (1000)      103 2021-08-23 11:53:34.000000 regobslib-1.0.0/pyproject.toml
--rw-rw-r--   0 aron      (1000) aron      (1000)      650 2022-09-01 13:42:14.267764 regobslib-1.0.0/setup.cfg
-drwxrwxr-x   0 aron      (1000) aron      (1000)        0 2022-09-01 13:42:14.263764 regobslib-1.0.0/src/
-drwxrwxr-x   0 aron      (1000) aron      (1000)        0 2022-09-01 13:42:14.263764 regobslib-1.0.0/src/regobslib/
--rw-rw-r--   0 aron      (1000) aron      (1000)      540 2022-05-23 10:26:00.000000 regobslib-1.0.0/src/regobslib/__init__.py
--rw-rw-r--   0 aron      (1000) aron      (1000)    19693 2022-08-09 16:36:18.000000 regobslib-1.0.0/src/regobslib/aps.py
--rw-rw-r--   0 aron      (1000) aron      (1000)    18957 2022-05-24 08:19:40.000000 regobslib-1.0.0/src/regobslib/connection.py
--rw-rw-r--   0 aron      (1000) aron      (1000)     3496 2022-08-17 09:10:21.000000 regobslib-1.0.0/src/regobslib/misc.py
--rw-rw-r--   0 aron      (1000) aron      (1000)     3733 2022-05-23 10:27:05.000000 regobslib-1.0.0/src/regobslib/region.py
--rw-rw-r--   0 aron      (1000) aron      (1000)    71566 2022-05-24 07:55:01.000000 regobslib-1.0.0/src/regobslib/submit.py
--rw-rw-r--   0 aron      (1000) aron      (1000)     9351 2022-09-01 13:25:56.000000 regobslib-1.0.0/src/regobslib/types.py
--rw-rw-r--   0 aron      (1000) aron      (1000)    13572 2022-09-01 13:39:19.000000 regobslib-1.0.0/src/regobslib/varsom.py
-drwxrwxr-x   0 aron      (1000) aron      (1000)        0 2022-09-01 13:42:14.267764 regobslib-1.0.0/src/regobslib.egg-info/
--rw-rw-r--   0 aron      (1000) aron      (1000)     3662 2022-09-01 13:42:14.000000 regobslib-1.0.0/src/regobslib.egg-info/PKG-INFO
--rw-rw-r--   0 aron      (1000) aron      (1000)      418 2022-09-01 13:42:14.000000 regobslib-1.0.0/src/regobslib.egg-info/SOURCES.txt
--rw-rw-r--   0 aron      (1000) aron      (1000)        1 2022-09-01 13:42:14.000000 regobslib-1.0.0/src/regobslib.egg-info/dependency_links.txt
--rw-rw-r--   0 aron      (1000) aron      (1000)       27 2022-09-01 13:42:14.000000 regobslib-1.0.0/src/regobslib.egg-info/requires.txt
--rw-rw-r--   0 aron      (1000) aron      (1000)       10 2022-09-01 13:42:14.000000 regobslib-1.0.0/src/regobslib.egg-info/top_level.txt
+drwxrwxr-x   0 aron      (1000) aron      (1000)        0 2022-11-30 15:24:55.201455 regobslib-1.0.1/
+-rw-rw-r--   0 aron      (1000) aron      (1000)        0 2021-08-23 07:22:18.000000 regobslib-1.0.1/LICENSE
+-rw-rw-r--   0 aron      (1000) aron      (1000)     3662 2022-11-30 15:24:55.201455 regobslib-1.0.1/PKG-INFO
+-rw-rw-r--   0 aron      (1000) aron      (1000)     3188 2022-02-08 10:10:03.000000 regobslib-1.0.1/README.md
+-rw-rw-r--   0 aron      (1000) aron      (1000)      103 2021-08-23 11:53:34.000000 regobslib-1.0.1/pyproject.toml
+-rw-rw-r--   0 aron      (1000) aron      (1000)      650 2022-11-30 15:24:55.201455 regobslib-1.0.1/setup.cfg
+drwxrwxr-x   0 aron      (1000) aron      (1000)        0 2022-11-30 15:24:55.197455 regobslib-1.0.1/src/
+drwxrwxr-x   0 aron      (1000) aron      (1000)        0 2022-11-30 15:24:55.197455 regobslib-1.0.1/src/regobslib/
+-rw-rw-r--   0 aron      (1000) aron      (1000)      540 2022-05-23 10:26:00.000000 regobslib-1.0.1/src/regobslib/__init__.py
+-rw-rw-r--   0 aron      (1000) aron      (1000)    19693 2022-08-09 16:36:18.000000 regobslib-1.0.1/src/regobslib/aps.py
+-rw-rw-r--   0 aron      (1000) aron      (1000)    19109 2022-11-30 15:23:31.000000 regobslib-1.0.1/src/regobslib/connection.py
+-rw-rw-r--   0 aron      (1000) aron      (1000)     3496 2022-08-17 09:10:21.000000 regobslib-1.0.1/src/regobslib/misc.py
+-rw-rw-r--   0 aron      (1000) aron      (1000)     3733 2022-05-23 10:27:05.000000 regobslib-1.0.1/src/regobslib/region.py
+-rw-rw-r--   0 aron      (1000) aron      (1000)    71573 2022-09-02 08:03:34.000000 regobslib-1.0.1/src/regobslib/submit.py
+-rw-rw-r--   0 aron      (1000) aron      (1000)     9351 2022-09-01 13:25:56.000000 regobslib-1.0.1/src/regobslib/types.py
+-rw-rw-r--   0 aron      (1000) aron      (1000)    13572 2022-09-01 13:39:19.000000 regobslib-1.0.1/src/regobslib/varsom.py
+drwxrwxr-x   0 aron      (1000) aron      (1000)        0 2022-11-30 15:24:55.201455 regobslib-1.0.1/src/regobslib.egg-info/
+-rw-rw-r--   0 aron      (1000) aron      (1000)     3662 2022-11-30 15:24:55.000000 regobslib-1.0.1/src/regobslib.egg-info/PKG-INFO
+-rw-rw-r--   0 aron      (1000) aron      (1000)      418 2022-11-30 15:24:55.000000 regobslib-1.0.1/src/regobslib.egg-info/SOURCES.txt
+-rw-rw-r--   0 aron      (1000) aron      (1000)        1 2022-11-30 15:24:55.000000 regobslib-1.0.1/src/regobslib.egg-info/dependency_links.txt
+-rw-rw-r--   0 aron      (1000) aron      (1000)       27 2022-11-30 15:24:55.000000 regobslib-1.0.1/src/regobslib.egg-info/requires.txt
+-rw-rw-r--   0 aron      (1000) aron      (1000)       10 2022-11-30 15:24:55.000000 regobslib-1.0.1/src/regobslib.egg-info/top_level.txt
```

### Comparing `regobslib-1.0.0/PKG-INFO` & `regobslib-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regobslib
-Version: 1.0.0
+Version: 1.0.1
 Summary: Client library for Regobs
 Home-page: https://github.com/NVE/regobslib
 Author: Aron Widforss
 Author-email: arwi@nve.no
 Project-URL: API Documentation, http://api.nve.no/doc/regobs/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `regobslib-1.0.0/README.md` & `regobslib-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `regobslib-1.0.0/setup.cfg` & `regobslib-1.0.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = regobslib
-version = 1.0.0
+version = 1.0.1
 author = Aron Widforss
 author_email = arwi@nve.no
 description = Client library for Regobs
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/NVE/regobslib
 project_urls =
```

### Comparing `regobslib-1.0.0/src/regobslib/__init__.py` & `regobslib-1.0.1/src/regobslib/__init__.py`

 * *Files identical despite different names*

### Comparing `regobslib-1.0.0/src/regobslib/aps.py` & `regobslib-1.0.1/src/regobslib/aps.py`

 * *Files identical despite different names*

### Comparing `regobslib-1.0.0/src/regobslib/connection.py` & `regobslib-1.0.1/src/regobslib/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,20 +210,22 @@
             aps.Temp,
             aps.SnowDepth,
             aps.NewSnow,
             aps.NewSnowMax,
         ]
         for region in regions:
             for data_type in data_types:
-                aps_url = f"{APS_PROD}/{data_type.WEATHER_PARAM}/24/{region}/{from_date}/{to_date - ONE_DAY}"
-                json = get(aps_url).json()
-                if data is None:
-                    data = aps.Aps.deserialize(json, data_type)
-                else:
-                    data = data.assimilate(aps.Aps.deserialize(json, data_type))
+                w_param = data_type.WEATHER_PARAM
+                url_formatter = lambda f, t: f"{APS_PROD}/{w_param}/24/{region}/{f.isoformat()}/{t.isoformat()}"
+                jsons = get_period(from_date, to_date - ONE_DAY, url_formatter, delta=128)
+                for json in jsons:
+                    if data is None:
+                        data = aps.Aps.deserialize(json, data_type)
+                    else:
+                        data = data.assimilate(aps.Aps.deserialize(json, data_type))
             url_formatter = lambda f, t: f"{APS_WIND_PROD}/{region}/{f.isoformat()}/{t.isoformat()}"
             jsons = get_period(from_date, to_date - ONE_DAY, url_formatter, delta=128)
             for json in jsons:
                 data = data.assimilate(aps.Aps.deserialize(json, aps.Wind))
         return data
 
     def search(self,
```

### Comparing `regobslib-1.0.0/src/regobslib/misc.py` & `regobslib-1.0.1/src/regobslib/misc.py`

 * *Files identical despite different names*

### Comparing `regobslib-1.0.0/src/regobslib/region.py` & `regobslib-1.0.1/src/regobslib/region.py`

 * *Files identical despite different names*

### Comparing `regobslib-1.0.0/src/regobslib/submit.py` & `regobslib-1.0.1/src/regobslib/submit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1484,15 +1484,15 @@
         ]
         return f"Position( {', '.join(rep)} )"
 
     def to_dict(self) -> ObsDict:
         return {
             "lat": self.lat,
             "lon": self.lon,
-            "region": None,
+            "region": self.region,
         }
 
 
 class Observer(types.Observer, Dictable):
     nickname = None
     id = None
     competence = None
```

### Comparing `regobslib-1.0.0/src/regobslib/types.py` & `regobslib-1.0.1/src/regobslib/types.py`

 * *Files identical despite different names*

### Comparing `regobslib-1.0.0/src/regobslib/varsom.py` & `regobslib-1.0.1/src/regobslib/varsom.py`

 * *Files identical despite different names*

### Comparing `regobslib-1.0.0/src/regobslib.egg-info/PKG-INFO` & `regobslib-1.0.1/src/regobslib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regobslib
-Version: 1.0.0
+Version: 1.0.1
 Summary: Client library for Regobs
 Home-page: https://github.com/NVE/regobslib
 Author: Aron Widforss
 Author-email: arwi@nve.no
 Project-URL: API Documentation, http://api.nve.no/doc/regobs/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

