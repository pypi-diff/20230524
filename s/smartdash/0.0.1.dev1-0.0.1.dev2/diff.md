# Comparing `tmp/smartdash-0.0.1.dev1.tar.gz` & `tmp/smartdash-0.0.1.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartdash-0.0.1.dev1.tar", last modified: Mon May 22 12:25:19 2023, max compression
+gzip compressed data, was "smartdash-0.0.1.dev2.tar", last modified: Wed May 24 15:29:25 2023, max compression
```

## Comparing `smartdash-0.0.1.dev1.tar` & `smartdash-0.0.1.dev2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:25:19.721297 smartdash-0.0.1.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-22 12:25:19.721297 smartdash-0.0.1.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 12:25:19.721297 smartdash-0.0.1.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-05-22 12:25:07.000000 smartdash-0.0.1.dev1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:25:19.717297 smartdash-0.0.1.dev1/smartdash/
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-22 12:25:07.000000 smartdash-0.0.1.dev1/smartdash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-22 12:25:07.000000 smartdash-0.0.1.dev1/smartdash/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-05-22 12:25:07.000000 smartdash-0.0.1.dev1/smartdash/dash.py
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-05-22 12:25:07.000000 smartdash-0.0.1.dev1/smartdash/smartdash_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:25:19.721297 smartdash-0.0.1.dev1/smartdash.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-22 12:25:19.000000 smartdash-0.0.1.dev1/smartdash.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-22 12:25:19.000000 smartdash-0.0.1.dev1/smartdash.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 12:25:19.000000 smartdash-0.0.1.dev1/smartdash.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-22 12:25:19.000000 smartdash-0.0.1.dev1/smartdash.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-22 12:25:19.000000 smartdash-0.0.1.dev1/smartdash.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-22 12:25:19.000000 smartdash-0.0.1.dev1/smartdash.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:29:25.781545 smartdash-0.0.1.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-24 15:29:25.777544 smartdash-0.0.1.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 15:29:25.781545 smartdash-0.0.1.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-05-24 15:29:14.000000 smartdash-0.0.1.dev2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:29:25.777544 smartdash-0.0.1.dev2/smartdash/
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-24 15:29:14.000000 smartdash-0.0.1.dev2/smartdash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-24 15:29:14.000000 smartdash-0.0.1.dev2/smartdash/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-05-24 15:29:14.000000 smartdash-0.0.1.dev2/smartdash/dash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-05-24 15:29:14.000000 smartdash-0.0.1.dev2/smartdash/smartdash_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:29:25.777544 smartdash-0.0.1.dev2/smartdash.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-24 15:29:25.000000 smartdash-0.0.1.dev2/smartdash.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-24 15:29:25.000000 smartdash-0.0.1.dev2/smartdash.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:29:25.000000 smartdash-0.0.1.dev2/smartdash.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-24 15:29:25.000000 smartdash-0.0.1.dev2/smartdash.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-24 15:29:25.000000 smartdash-0.0.1.dev2/smartdash.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-24 15:29:25.000000 smartdash-0.0.1.dev2/smartdash.egg-info/top_level.txt
```

### Comparing `smartdash-0.0.1.dev1/PKG-INFO` & `smartdash-0.0.1.dev2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartdash
-Version: 0.0.1.dev1
+Version: 0.0.1.dev2
 Summary: python logging client for SmartDash
 Home-page: https://github.com/notAI-tech/smartdash
 Author: BEDAPUDI PRANEETH
 Author-email: praneeth@bpraneeth.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `smartdash-0.0.1.dev1/setup.py` & `smartdash-0.0.1.dev2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = "smartdash"
 DESCRIPTION = "python logging client for SmartDash"
 URL = "https://github.com/notAI-tech/smartdash"
 EMAIL = "praneeth@bpraneeth.com"
 AUTHOR = "BEDAPUDI PRANEETH"
 REQUIRES_PYTHON = ">=3.6.0"
-VERSION = "0.0.1.dev1"
+VERSION = "0.0.1.dev2"
 
 # What packages are required for this module to be executed?
 REQUIRED = ["requests", "liteindex", "streamlit", "plotly"]
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
@@ -113,11 +113,9 @@
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: Implementation :: CPython",
     ],
     # $ setup.py publish support.
-    cmdclass={
-        "upload": UploadCommand,
-    },
+    cmdclass={"upload": UploadCommand,},
 )
```

### Comparing `smartdash-0.0.1.dev1/smartdash/dash.py` & `smartdash-0.0.1.dev2/smartdash/dash.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,15 +151,19 @@
 def main():
     st.set_page_config(page_title="SmartDash", layout="wide")  # Add layout parameter
 
     st.sidebar.title("SmartDash - App Dashboard")
 
     # Dropdowns for app_name and last_n_hours in the sidebar
     st.sidebar.markdown("## Settings")
-    app_name = st.sidebar.selectbox("Select App", requests.get("http://localhost:8080/app_names").json()['app_names'], index=0)
+    app_name = st.sidebar.selectbox(
+        "Select App",
+        requests.get("http://localhost:8080/app_names").json()["app_names"],
+        index=0,
+    )
     time_range = st.sidebar.selectbox(
         "Select Time Range", ["8 hours", "12 hours", "Last day", "Last week"], index=0
     )
 
     time_mapping = {"8 hours": 8, "12 hours": 12, "Last day": 24, "Last week": 168}
     last_n_hours = time_mapping[time_range]
```

### Comparing `smartdash-0.0.1.dev1/smartdash/smartdash_server.py` & `smartdash-0.0.1.dev2/smartdash/smartdash_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,19 +51,30 @@
         "timestamp": 0,
         "stage": "",
     },
     "smartdash.db",
     auto_key=True,
 )
 
+
 class AppNames(object):
     def on_get(self, req, resp):
-        resp.media = {"success": True, "app_names": list(set(LOG_INDEX.distinct("app_name") + TIMERS_INDEX.distinct("app_name") + ML_INPUTS_OUTPUTS_INDEX.distinct("app_name")))}
+        resp.media = {
+            "success": True,
+            "app_names": list(
+                set(
+                    LOG_INDEX.distinct("app_name")
+                    + TIMERS_INDEX.distinct("app_name")
+                    + ML_INPUTS_OUTPUTS_INDEX.distinct("app_name")
+                )
+            ),
+        }
         resp.status = falcon.HTTP_200
 
+
 class AddLogs(object):
     def on_post(self, req, resp):
         data = req.media
         id = LOG_INDEX.add(data)
         resp.media = {"success": True, "id": id}
         resp.status = falcon.HTTP_200
```

### Comparing `smartdash-0.0.1.dev1/smartdash.egg-info/PKG-INFO` & `smartdash-0.0.1.dev2/smartdash.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartdash
-Version: 0.0.1.dev1
+Version: 0.0.1.dev2
 Summary: python logging client for SmartDash
 Home-page: https://github.com/notAI-tech/smartdash
 Author: BEDAPUDI PRANEETH
 Author-email: praneeth@bpraneeth.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

