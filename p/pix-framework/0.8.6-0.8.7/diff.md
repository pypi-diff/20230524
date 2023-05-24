# Comparing `tmp/pix_framework-0.8.6.tar.gz` & `tmp/pix_framework-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pix_framework-0.8.6.tar", max compression
+gzip compressed data, was "pix_framework-0.8.7.tar", max compression
```

## Comparing `pix_framework-0.8.6.tar` & `pix_framework-0.8.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    11357 2023-05-23 14:36:37.819071 pix_framework-0.8.6/LICENSE
--rw-r--r--   0        0        0      549 2023-05-23 14:36:37.819071 pix_framework-0.8.6/README.md
--rw-r--r--   0        0        0      761 2023-05-23 14:36:37.819071 pix_framework-0.8.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-23 14:36:37.819071 pix_framework-0.8.6/src/pix_framework/__init__.py
--rw-r--r--   0        0        0       32 2023-05-23 14:36:37.819071 pix_framework-0.8.6/src/pix_framework/calendar/__init__.py
--rw-r--r--   0        0        0     7524 2023-05-23 14:36:37.819071 pix_framework-0.8.6/src/pix_framework/calendar/availability.py
--rw-r--r--   0        0        0    31790 2023-05-23 14:36:37.823071 pix_framework-0.8.6/src/pix_framework/calendar/resource_calendar.py
--rw-r--r--   0        0        0        0 2023-05-23 14:36:37.823071 pix_framework-0.8.6/src/pix_framework/discovery/__init__.py
--rw-r--r--   0        0        0     5835 2023-05-23 14:36:37.823071 pix_framework-0.8.6/src/pix_framework/discovery/calendar_factory.py
--rw-r--r--   0        0        0     6967 2023-05-23 14:36:37.823071 pix_framework-0.8.6/src/pix_framework/discovery/case_arrival.py
--rw-r--r--   0        0        0     4903 2023-05-23 14:36:37.823071 pix_framework-0.8.6/src/pix_framework/discovery/gateway_probabilities.py
--rw-r--r--   0        0        0        0 2023-05-23 14:36:37.823071 pix_framework-0.8.6/src/pix_framework/enhancement/__init__.py
--rw-r--r--   0        0        0     5444 2023-05-23 14:36:37.823071 pix_framework-0.8.6/src/pix_framework/enhancement/multitasking.py
--rw-r--r--   0        0        0       27 2023-05-23 14:36:37.823071 pix_framework-0.8.6/src/pix_framework/filesystem/__init__.py
--rw-r--r--   0        0        0     1088 2023-05-23 14:36:37.823071 pix_framework-0.8.6/src/pix_framework/filesystem/file_manager.py
--rw-r--r--   0        0        0     2498 2023-05-23 14:36:37.823071 pix_framework-0.8.6/src/pix_framework/input.py
--rw-r--r--   0        0        0        0 2023-05-23 14:36:37.823071 pix_framework-0.8.6/src/pix_framework/io/__init__.py
--rw-r--r--   0        0        0    38314 2023-05-23 14:36:37.823071 pix_framework-0.8.6/src/pix_framework/io/bpm_graph.py
--rw-r--r--   0        0        0     2058 2023-05-23 14:36:37.823071 pix_framework-0.8.6/src/pix_framework/log_ids.py
--rw-r--r--   0        0        0        0 2023-05-23 14:36:37.823071 pix_framework-0.8.6/src/pix_framework/log_split/__init__.py
--rw-r--r--   0        0        0     4414 2023-05-23 14:36:37.823071 pix_framework-0.8.6/src/pix_framework/log_split/log_split.py
--rw-r--r--   0        0        0       27 2023-05-23 14:36:37.823071 pix_framework-0.8.6/src/pix_framework/statistics/__init__.py
--rw-r--r--   0        0        0    13047 2023-05-23 14:36:37.823071 pix_framework-0.8.6/src/pix_framework/statistics/distribution.py
--rw-r--r--   0        0        0      970 2023-05-23 14:36:37.823071 pix_framework-0.8.6/src/pix_framework/statistics/utils.py
--rw-r--r--   0        0        0     1220 1970-01-01 00:00:00.000000 pix_framework-0.8.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-24 09:27:37.084466 pix_framework-0.8.7/LICENSE
+-rw-r--r--   0        0        0      549 2023-05-24 09:27:37.084466 pix_framework-0.8.7/README.md
+-rw-r--r--   0        0        0      761 2023-05-24 09:27:37.084466 pix_framework-0.8.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-24 09:27:37.084466 pix_framework-0.8.7/src/pix_framework/__init__.py
+-rw-r--r--   0        0        0       32 2023-05-24 09:27:37.088466 pix_framework-0.8.7/src/pix_framework/calendar/__init__.py
+-rw-r--r--   0        0        0     7524 2023-05-24 09:27:37.088466 pix_framework-0.8.7/src/pix_framework/calendar/availability.py
+-rw-r--r--   0        0        0    31886 2023-05-24 09:27:37.088466 pix_framework-0.8.7/src/pix_framework/calendar/resource_calendar.py
+-rw-r--r--   0        0        0        0 2023-05-24 09:27:37.088466 pix_framework-0.8.7/src/pix_framework/discovery/__init__.py
+-rw-r--r--   0        0        0     5835 2023-05-24 09:27:37.088466 pix_framework-0.8.7/src/pix_framework/discovery/calendar_factory.py
+-rw-r--r--   0        0        0     6967 2023-05-24 09:27:37.088466 pix_framework-0.8.7/src/pix_framework/discovery/case_arrival.py
+-rw-r--r--   0        0        0     4903 2023-05-24 09:27:37.088466 pix_framework-0.8.7/src/pix_framework/discovery/gateway_probabilities.py
+-rw-r--r--   0        0        0        0 2023-05-24 09:27:37.088466 pix_framework-0.8.7/src/pix_framework/enhancement/__init__.py
+-rw-r--r--   0        0        0     5444 2023-05-24 09:27:37.088466 pix_framework-0.8.7/src/pix_framework/enhancement/multitasking.py
+-rw-r--r--   0        0        0       27 2023-05-24 09:27:37.088466 pix_framework-0.8.7/src/pix_framework/filesystem/__init__.py
+-rw-r--r--   0        0        0     1088 2023-05-24 09:27:37.088466 pix_framework-0.8.7/src/pix_framework/filesystem/file_manager.py
+-rw-r--r--   0        0        0     2498 2023-05-24 09:27:37.088466 pix_framework-0.8.7/src/pix_framework/input.py
+-rw-r--r--   0        0        0        0 2023-05-24 09:27:37.088466 pix_framework-0.8.7/src/pix_framework/io/__init__.py
+-rw-r--r--   0        0        0    38314 2023-05-24 09:27:37.088466 pix_framework-0.8.7/src/pix_framework/io/bpm_graph.py
+-rw-r--r--   0        0        0     2058 2023-05-24 09:27:37.088466 pix_framework-0.8.7/src/pix_framework/log_ids.py
+-rw-r--r--   0        0        0        0 2023-05-24 09:27:37.088466 pix_framework-0.8.7/src/pix_framework/log_split/__init__.py
+-rw-r--r--   0        0        0     4414 2023-05-24 09:27:37.088466 pix_framework-0.8.7/src/pix_framework/log_split/log_split.py
+-rw-r--r--   0        0        0       27 2023-05-24 09:27:37.088466 pix_framework-0.8.7/src/pix_framework/statistics/__init__.py
+-rw-r--r--   0        0        0    13047 2023-05-24 09:27:37.088466 pix_framework-0.8.7/src/pix_framework/statistics/distribution.py
+-rw-r--r--   0        0        0      970 2023-05-24 09:27:37.088466 pix_framework-0.8.7/src/pix_framework/statistics/utils.py
+-rw-r--r--   0        0        0     1220 1970-01-01 00:00:00.000000 pix_framework-0.8.7/PKG-INFO
```

### Comparing `pix_framework-0.8.6/LICENSE` & `pix_framework-0.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.6/README.md` & `pix_framework-0.8.7/README.md`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.6/pyproject.toml` & `pix_framework-0.8.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pix-framework"
-version = "0.8.6"
+version = "0.8.7"
 description = "Process Improvement Explorer Framework contains process discovery and improvement modules of the Process Improvement Explorer project."
 authors = ["David Chapela de la Campa <david.chapela.delacampa@gmail.com>", "Ihar Suvorau <ihar.suvorau@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "pix_framework", from = "src" },
 ]
```

### Comparing `pix_framework-0.8.6/src/pix_framework/calendar/availability.py` & `pix_framework-0.8.7/src/pix_framework/calendar/availability.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.6/src/pix_framework/calendar/resource_calendar.py` & `pix_framework-0.8.7/src/pix_framework/calendar/resource_calendar.py`

 * *Files 5% similar despite different names*

```diff
@@ -372,19 +372,19 @@
             self.week_day == another_point.week_day
             and self.index == another_point.index
         )
 
 
 @dataclass
 class Interval:
-    start: pd.Timestamp
-    end: pd.Timestamp
+    start: datetime.datetime
+    end: datetime.datetime
     duration: float
 
-    def __init__(self, start: pd.Timestamp, end: pd.Timestamp):
+    def __init__(self, start: datetime.datetime, end: datetime.datetime):
         self.start = start
         if end < start and end.hour == 0 and end.minute == 0:
             end.replace(hour=23, minute=59, second=59, microsecond=999)
         self.end = end
         self.duration = (end - start).total_seconds()
 
     def __eq__(self, other):
@@ -484,15 +484,15 @@
         )
         return res_interval
 
 
 class RCalendar:  # AvailabilityCalendar
     def __init__(self, calendar_id):
         self.calendar_id = calendar_id
-        self.default_date = pd.Timestamp.now().date()
+        self.default_date = None
         self.work_intervals = {}
         self.new_day = None
         self.cumulative_work_durations = {}
         self.work_rest_count = {}
         self.total_weekly_work = 0
         self.total_weekly_rest = to_seconds(1, "WEEKS")
         for i in range(0, 7):
@@ -546,21 +546,22 @@
 
     def add_calendar_item(
         self, from_day: str, to_day: str, begin_time: str, end_time: str
     ):
         if from_day.upper() in str_week_days and to_day.upper() in str_week_days:
             try:
                 t_interval = Interval(
-                    start=pd.Timestamp.combine(
-                        self.default_date, pd.Timestamp(begin_time).time()
-                    ),
-                    end=pd.Timestamp.combine(
-                        self.default_date, pd.Timestamp(end_time).time()
-                    ),
+                    start=pd.Timestamp(begin_time).to_pydatetime(),
+                    end=pd.Timestamp(end_time).to_pydatetime(),
                 )
+                if self.default_date is None:
+                    self.default_date = t_interval.start.date()
+                    self.new_day = datetime.datetime.combine(
+                        self.default_date, datetime.time()
+                    )
                 d_s = str_week_days[from_day]
                 d_e = str_week_days[to_day]
                 while True:
                     self._add_interval(d_s % 7, t_interval)
                     if d_s % 7 == d_e:
                         break
                     d_s += 1
```

### Comparing `pix_framework-0.8.6/src/pix_framework/discovery/calendar_factory.py` & `pix_framework-0.8.7/src/pix_framework/discovery/calendar_factory.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.6/src/pix_framework/discovery/case_arrival.py` & `pix_framework-0.8.7/src/pix_framework/discovery/case_arrival.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.6/src/pix_framework/discovery/gateway_probabilities.py` & `pix_framework-0.8.7/src/pix_framework/discovery/gateway_probabilities.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.6/src/pix_framework/enhancement/multitasking.py` & `pix_framework-0.8.7/src/pix_framework/enhancement/multitasking.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.6/src/pix_framework/filesystem/file_manager.py` & `pix_framework-0.8.7/src/pix_framework/filesystem/file_manager.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.6/src/pix_framework/input.py` & `pix_framework-0.8.7/src/pix_framework/input.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.6/src/pix_framework/io/bpm_graph.py` & `pix_framework-0.8.7/src/pix_framework/io/bpm_graph.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.6/src/pix_framework/log_ids.py` & `pix_framework-0.8.7/src/pix_framework/log_ids.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.6/src/pix_framework/log_split/log_split.py` & `pix_framework-0.8.7/src/pix_framework/log_split/log_split.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.6/src/pix_framework/statistics/distribution.py` & `pix_framework-0.8.7/src/pix_framework/statistics/distribution.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.6/src/pix_framework/statistics/utils.py` & `pix_framework-0.8.7/src/pix_framework/statistics/utils.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.6/PKG-INFO` & `pix_framework-0.8.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pix-framework
-Version: 0.8.6
+Version: 0.8.7
 Summary: Process Improvement Explorer Framework contains process discovery and improvement modules of the Process Improvement Explorer project.
 Author: David Chapela de la Campa
 Author-email: david.chapela.delacampa@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

