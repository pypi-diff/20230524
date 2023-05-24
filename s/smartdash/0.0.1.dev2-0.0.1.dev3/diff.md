# Comparing `tmp/smartdash-0.0.1.dev2.tar.gz` & `tmp/smartdash-0.0.1.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartdash-0.0.1.dev2.tar", last modified: Wed May 24 15:29:25 2023, max compression
+gzip compressed data, was "smartdash-0.0.1.dev3.tar", last modified: Wed May 24 15:33:37 2023, max compression
```

## Comparing `smartdash-0.0.1.dev2.tar` & `smartdash-0.0.1.dev3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:29:25.781545 smartdash-0.0.1.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-24 15:29:25.777544 smartdash-0.0.1.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 15:29:25.781545 smartdash-0.0.1.dev2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-05-24 15:29:14.000000 smartdash-0.0.1.dev2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:29:25.777544 smartdash-0.0.1.dev2/smartdash/
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-24 15:29:14.000000 smartdash-0.0.1.dev2/smartdash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-24 15:29:14.000000 smartdash-0.0.1.dev2/smartdash/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-05-24 15:29:14.000000 smartdash-0.0.1.dev2/smartdash/dash.py
--rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-05-24 15:29:14.000000 smartdash-0.0.1.dev2/smartdash/smartdash_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:29:25.777544 smartdash-0.0.1.dev2/smartdash.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-24 15:29:25.000000 smartdash-0.0.1.dev2/smartdash.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-24 15:29:25.000000 smartdash-0.0.1.dev2/smartdash.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:29:25.000000 smartdash-0.0.1.dev2/smartdash.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-24 15:29:25.000000 smartdash-0.0.1.dev2/smartdash.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-24 15:29:25.000000 smartdash-0.0.1.dev2/smartdash.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-24 15:29:25.000000 smartdash-0.0.1.dev2/smartdash.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:33:37.067944 smartdash-0.0.1.dev3/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-24 15:33:37.067944 smartdash-0.0.1.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 15:33:37.067944 smartdash-0.0.1.dev3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-05-24 15:33:23.000000 smartdash-0.0.1.dev3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:33:37.067944 smartdash-0.0.1.dev3/smartdash/
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-24 15:33:23.000000 smartdash-0.0.1.dev3/smartdash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-24 15:33:23.000000 smartdash-0.0.1.dev3/smartdash/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-05-24 15:33:23.000000 smartdash-0.0.1.dev3/smartdash/dash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-05-24 15:33:23.000000 smartdash-0.0.1.dev3/smartdash/smartdash_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:33:37.067944 smartdash-0.0.1.dev3/smartdash.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-24 15:33:37.000000 smartdash-0.0.1.dev3/smartdash.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-24 15:33:37.000000 smartdash-0.0.1.dev3/smartdash.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:33:37.000000 smartdash-0.0.1.dev3/smartdash.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-24 15:33:37.000000 smartdash-0.0.1.dev3/smartdash.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-24 15:33:37.000000 smartdash-0.0.1.dev3/smartdash.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-24 15:33:37.000000 smartdash-0.0.1.dev3/smartdash.egg-info/top_level.txt
```

### Comparing `smartdash-0.0.1.dev2/PKG-INFO` & `smartdash-0.0.1.dev3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartdash
-Version: 0.0.1.dev2
+Version: 0.0.1.dev3
 Summary: python logging client for SmartDash
 Home-page: https://github.com/notAI-tech/smartdash
 Author: BEDAPUDI PRANEETH
 Author-email: praneeth@bpraneeth.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `smartdash-0.0.1.dev2/setup.py` & `smartdash-0.0.1.dev3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = "smartdash"
 DESCRIPTION = "python logging client for SmartDash"
 URL = "https://github.com/notAI-tech/smartdash"
 EMAIL = "praneeth@bpraneeth.com"
 AUTHOR = "BEDAPUDI PRANEETH"
 REQUIRES_PYTHON = ">=3.6.0"
-VERSION = "0.0.1.dev2"
+VERSION = "0.0.1.dev3"
 
 # What packages are required for this module to be executed?
 REQUIRED = ["requests", "liteindex", "streamlit", "plotly"]
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
```

### Comparing `smartdash-0.0.1.dev2/smartdash/__init__.py` & `smartdash-0.0.1.dev3/smartdash/__init__.py`

 * *Files identical despite different names*

### Comparing `smartdash-0.0.1.dev2/smartdash/dash.py` & `smartdash-0.0.1.dev3/smartdash/dash.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,41 +3,45 @@
 import pandas as pd
 import requests
 import json
 import plotly.express as px
 import plotly.graph_objects as go
 from datetime import datetime
 
+SERVER_URL = os.getenv("SERVER_URL")
+if not SERVER_URL:
+    print("--server_url is must of --dash")
+    exit()
 
 # Function to fetch logs data
 def fetch_logs(app_name, last_n_hours):
     logs_data = requests.get(
-        f"http://localhost:8080/logs?app_name={app_name}&last_n_hours={last_n_hours}"
+        f"{SERVER_URL}logs?app_name={app_name}&last_n_hours={last_n_hours}"
     ).json()
     # Convert timestamp to datetime format
     for log in logs_data:
         log["timestamp"] = datetime.fromtimestamp(log["timestamp"])
     return logs_data
 
 
 # Function to fetch logs data
 def fetch_ml_inputs_outputs(app_name, last_n_hours):
     logs_data = requests.get(
-        f"http://localhost:8080/ml_inputs_outputs?app_name={app_name}&last_n_hours={last_n_hours}"
+        f"{SERVER_URL}ml_inputs_outputs?app_name={app_name}&last_n_hours={last_n_hours}"
     ).json()
     # Convert timestamp to datetime format
     for log in logs_data:
         log["timestamp"] = datetime.fromtimestamp(log["timestamp"])
     return logs_data
 
 
 # Function to fetch timers data
 def fetch_timers(app_name, last_n_hours):
     timers_data = requests.get(
-        f"http://localhost:8080/timers?app_name={app_name}&last_n_hours={last_n_hours}"
+        f"{SERVER_URL}timers?app_name={app_name}&last_n_hours={last_n_hours}"
     ).json()
     return timers_data
 
 
 # Function to group timers data by u_id
 def group_timers(timers_data):
     grouped_timers = {}
@@ -153,15 +157,15 @@
 
     st.sidebar.title("SmartDash - App Dashboard")
 
     # Dropdowns for app_name and last_n_hours in the sidebar
     st.sidebar.markdown("## Settings")
     app_name = st.sidebar.selectbox(
         "Select App",
-        requests.get("http://localhost:8080/app_names").json()["app_names"],
+        requests.get("{SERVER_URL}app_names").json()["app_names"],
         index=0,
     )
     time_range = st.sidebar.selectbox(
         "Select Time Range", ["8 hours", "12 hours", "Last day", "Last week"], index=0
     )
 
     time_mapping = {"8 hours": 8, "12 hours": 12, "Last day": 24, "Last week": 168}
```

### Comparing `smartdash-0.0.1.dev2/smartdash/smartdash_server.py` & `smartdash-0.0.1.dev3/smartdash/smartdash_server.py`

 * *Files identical despite different names*

### Comparing `smartdash-0.0.1.dev2/smartdash.egg-info/PKG-INFO` & `smartdash-0.0.1.dev3/smartdash.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartdash
-Version: 0.0.1.dev2
+Version: 0.0.1.dev3
 Summary: python logging client for SmartDash
 Home-page: https://github.com/notAI-tech/smartdash
 Author: BEDAPUDI PRANEETH
 Author-email: praneeth@bpraneeth.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

