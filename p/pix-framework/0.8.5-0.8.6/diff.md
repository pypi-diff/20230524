# Comparing `tmp/pix_framework-0.8.5.tar.gz` & `tmp/pix_framework-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pix_framework-0.8.5.tar", max compression
+gzip compressed data, was "pix_framework-0.8.6.tar", max compression
```

## Comparing `pix_framework-0.8.5.tar` & `pix_framework-0.8.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    11357 2023-05-23 14:06:14.723423 pix_framework-0.8.5/LICENSE
--rw-r--r--   0        0        0      549 2023-05-23 14:06:14.723423 pix_framework-0.8.5/README.md
--rw-r--r--   0        0        0      761 2023-05-23 14:06:14.723423 pix_framework-0.8.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-23 14:06:14.723423 pix_framework-0.8.5/src/pix_framework/__init__.py
--rw-r--r--   0        0        0       32 2023-05-23 14:06:14.723423 pix_framework-0.8.5/src/pix_framework/calendar/__init__.py
--rw-r--r--   0        0        0     7524 2023-05-23 14:06:14.723423 pix_framework-0.8.5/src/pix_framework/calendar/availability.py
--rw-r--r--   0        0        0    31488 2023-05-23 14:06:14.723423 pix_framework-0.8.5/src/pix_framework/calendar/resource_calendar.py
--rw-r--r--   0        0        0        0 2023-05-23 14:06:14.723423 pix_framework-0.8.5/src/pix_framework/discovery/__init__.py
--rw-r--r--   0        0        0     5835 2023-05-23 14:06:14.723423 pix_framework-0.8.5/src/pix_framework/discovery/calendar_factory.py
--rw-r--r--   0        0        0     6967 2023-05-23 14:06:14.723423 pix_framework-0.8.5/src/pix_framework/discovery/case_arrival.py
--rw-r--r--   0        0        0     4903 2023-05-23 14:06:14.723423 pix_framework-0.8.5/src/pix_framework/discovery/gateway_probabilities.py
--rw-r--r--   0        0        0        0 2023-05-23 14:06:14.723423 pix_framework-0.8.5/src/pix_framework/enhancement/__init__.py
--rw-r--r--   0        0        0     5444 2023-05-23 14:06:14.723423 pix_framework-0.8.5/src/pix_framework/enhancement/multitasking.py
--rw-r--r--   0        0        0       27 2023-05-23 14:06:14.723423 pix_framework-0.8.5/src/pix_framework/filesystem/__init__.py
--rw-r--r--   0        0        0     1088 2023-05-23 14:06:14.723423 pix_framework-0.8.5/src/pix_framework/filesystem/file_manager.py
--rw-r--r--   0        0        0     2498 2023-05-23 14:06:14.723423 pix_framework-0.8.5/src/pix_framework/input.py
--rw-r--r--   0        0        0        0 2023-05-23 14:06:14.723423 pix_framework-0.8.5/src/pix_framework/io/__init__.py
--rw-r--r--   0        0        0    38314 2023-05-23 14:06:14.723423 pix_framework-0.8.5/src/pix_framework/io/bpm_graph.py
--rw-r--r--   0        0        0     2058 2023-05-23 14:06:14.723423 pix_framework-0.8.5/src/pix_framework/log_ids.py
--rw-r--r--   0        0        0        0 2023-05-23 14:06:14.723423 pix_framework-0.8.5/src/pix_framework/log_split/__init__.py
--rw-r--r--   0        0        0     4414 2023-05-23 14:06:14.723423 pix_framework-0.8.5/src/pix_framework/log_split/log_split.py
--rw-r--r--   0        0        0       27 2023-05-23 14:06:14.723423 pix_framework-0.8.5/src/pix_framework/statistics/__init__.py
--rw-r--r--   0        0        0    13047 2023-05-23 14:06:14.723423 pix_framework-0.8.5/src/pix_framework/statistics/distribution.py
--rw-r--r--   0        0        0      970 2023-05-23 14:06:14.723423 pix_framework-0.8.5/src/pix_framework/statistics/utils.py
--rw-r--r--   0        0        0     1220 1970-01-01 00:00:00.000000 pix_framework-0.8.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-23 14:36:37.819071 pix_framework-0.8.6/LICENSE
+-rw-r--r--   0        0        0      549 2023-05-23 14:36:37.819071 pix_framework-0.8.6/README.md
+-rw-r--r--   0        0        0      761 2023-05-23 14:36:37.819071 pix_framework-0.8.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-23 14:36:37.819071 pix_framework-0.8.6/src/pix_framework/__init__.py
+-rw-r--r--   0        0        0       32 2023-05-23 14:36:37.819071 pix_framework-0.8.6/src/pix_framework/calendar/__init__.py
+-rw-r--r--   0        0        0     7524 2023-05-23 14:36:37.819071 pix_framework-0.8.6/src/pix_framework/calendar/availability.py
+-rw-r--r--   0        0        0    31790 2023-05-23 14:36:37.823071 pix_framework-0.8.6/src/pix_framework/calendar/resource_calendar.py
+-rw-r--r--   0        0        0        0 2023-05-23 14:36:37.823071 pix_framework-0.8.6/src/pix_framework/discovery/__init__.py
+-rw-r--r--   0        0        0     5835 2023-05-23 14:36:37.823071 pix_framework-0.8.6/src/pix_framework/discovery/calendar_factory.py
+-rw-r--r--   0        0        0     6967 2023-05-23 14:36:37.823071 pix_framework-0.8.6/src/pix_framework/discovery/case_arrival.py
+-rw-r--r--   0        0        0     4903 2023-05-23 14:36:37.823071 pix_framework-0.8.6/src/pix_framework/discovery/gateway_probabilities.py
+-rw-r--r--   0        0        0        0 2023-05-23 14:36:37.823071 pix_framework-0.8.6/src/pix_framework/enhancement/__init__.py
+-rw-r--r--   0        0        0     5444 2023-05-23 14:36:37.823071 pix_framework-0.8.6/src/pix_framework/enhancement/multitasking.py
+-rw-r--r--   0        0        0       27 2023-05-23 14:36:37.823071 pix_framework-0.8.6/src/pix_framework/filesystem/__init__.py
+-rw-r--r--   0        0        0     1088 2023-05-23 14:36:37.823071 pix_framework-0.8.6/src/pix_framework/filesystem/file_manager.py
+-rw-r--r--   0        0        0     2498 2023-05-23 14:36:37.823071 pix_framework-0.8.6/src/pix_framework/input.py
+-rw-r--r--   0        0        0        0 2023-05-23 14:36:37.823071 pix_framework-0.8.6/src/pix_framework/io/__init__.py
+-rw-r--r--   0        0        0    38314 2023-05-23 14:36:37.823071 pix_framework-0.8.6/src/pix_framework/io/bpm_graph.py
+-rw-r--r--   0        0        0     2058 2023-05-23 14:36:37.823071 pix_framework-0.8.6/src/pix_framework/log_ids.py
+-rw-r--r--   0        0        0        0 2023-05-23 14:36:37.823071 pix_framework-0.8.6/src/pix_framework/log_split/__init__.py
+-rw-r--r--   0        0        0     4414 2023-05-23 14:36:37.823071 pix_framework-0.8.6/src/pix_framework/log_split/log_split.py
+-rw-r--r--   0        0        0       27 2023-05-23 14:36:37.823071 pix_framework-0.8.6/src/pix_framework/statistics/__init__.py
+-rw-r--r--   0        0        0    13047 2023-05-23 14:36:37.823071 pix_framework-0.8.6/src/pix_framework/statistics/distribution.py
+-rw-r--r--   0        0        0      970 2023-05-23 14:36:37.823071 pix_framework-0.8.6/src/pix_framework/statistics/utils.py
+-rw-r--r--   0        0        0     1220 1970-01-01 00:00:00.000000 pix_framework-0.8.6/PKG-INFO
```

### Comparing `pix_framework-0.8.5/LICENSE` & `pix_framework-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.5/README.md` & `pix_framework-0.8.6/README.md`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.5/pyproject.toml` & `pix_framework-0.8.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pix-framework"
-version = "0.8.5"
+version = "0.8.6"
 description = "Process Improvement Explorer Framework contains process discovery and improvement modules of the Process Improvement Explorer project."
 authors = ["David Chapela de la Campa <david.chapela.delacampa@gmail.com>", "Ihar Suvorau <ihar.suvorau@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "pix_framework", from = "src" },
 ]
```

### Comparing `pix_framework-0.8.5/src/pix_framework/calendar/availability.py` & `pix_framework-0.8.6/src/pix_framework/calendar/availability.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.5/src/pix_framework/calendar/resource_calendar.py` & `pix_framework-0.8.6/src/pix_framework/calendar/resource_calendar.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     2: "WEDNESDAY",
     3: "THURSDAY",
     4: "FRIDAY",
     5: "SATURDAY",
     6: "SUNDAY",
 }
 
-convertion_table = {
+conversion_table = {
     "WEEKS": 604800,
     "DAYS": 86400,
     "HOURS": 3600,
     "MINUTES": 60,
     "SECONDS": 1,
 }
 
@@ -779,10 +779,20 @@
                             interval.start.minute,
                             interval.end.hour,
                             interval.end.minute,
                         )
                     )
 
 
+def build_full_time_calendar(calendar_id) -> RCalendar:
+    r_calendar = RCalendar(calendar_id)
+    for i in range(0, 7):
+        str_weekday = int_week_days[i]
+        r_calendar.add_calendar_item(
+            str_weekday, str_weekday, "00:00:00.000", "23:59:59.999"
+        )
+    return r_calendar
+
+
 def to_seconds(value, from_unit):
     u_from = from_unit.upper()
-    return value * convertion_table[u_from] if u_from in convertion_table else value
+    return value * conversion_table[u_from] if u_from in conversion_table else value
```

### Comparing `pix_framework-0.8.5/src/pix_framework/discovery/calendar_factory.py` & `pix_framework-0.8.6/src/pix_framework/discovery/calendar_factory.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.5/src/pix_framework/discovery/case_arrival.py` & `pix_framework-0.8.6/src/pix_framework/discovery/case_arrival.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.5/src/pix_framework/discovery/gateway_probabilities.py` & `pix_framework-0.8.6/src/pix_framework/discovery/gateway_probabilities.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.5/src/pix_framework/enhancement/multitasking.py` & `pix_framework-0.8.6/src/pix_framework/enhancement/multitasking.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.5/src/pix_framework/filesystem/file_manager.py` & `pix_framework-0.8.6/src/pix_framework/filesystem/file_manager.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.5/src/pix_framework/input.py` & `pix_framework-0.8.6/src/pix_framework/input.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.5/src/pix_framework/io/bpm_graph.py` & `pix_framework-0.8.6/src/pix_framework/io/bpm_graph.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.5/src/pix_framework/log_ids.py` & `pix_framework-0.8.6/src/pix_framework/log_ids.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.5/src/pix_framework/log_split/log_split.py` & `pix_framework-0.8.6/src/pix_framework/log_split/log_split.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.5/src/pix_framework/statistics/distribution.py` & `pix_framework-0.8.6/src/pix_framework/statistics/distribution.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.5/src/pix_framework/statistics/utils.py` & `pix_framework-0.8.6/src/pix_framework/statistics/utils.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.5/PKG-INFO` & `pix_framework-0.8.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pix-framework
-Version: 0.8.5
+Version: 0.8.6
 Summary: Process Improvement Explorer Framework contains process discovery and improvement modules of the Process Improvement Explorer project.
 Author: David Chapela de la Campa
 Author-email: david.chapela.delacampa@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

