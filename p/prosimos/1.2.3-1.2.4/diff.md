# Comparing `tmp/prosimos-1.2.3.tar.gz` & `tmp/prosimos-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prosimos-1.2.3.tar", max compression
+gzip compressed data, was "prosimos-1.2.4.tar", max compression
```

## Comparing `prosimos-1.2.3.tar` & `prosimos-1.2.4.tar`

### file list

```diff
@@ -1,32 +1,31 @@
--rw-r--r--   0        0        0    14755 2023-05-15 07:00:12.329363 prosimos-1.2.3/README.md
--rw-r--r--   0        0        0        0 2023-05-15 07:00:12.345364 prosimos-1.2.3/bpdfr_discovery/__init__.py
--rw-r--r--   0        0        0     3478 2023-05-15 07:00:12.345364 prosimos-1.2.3/bpdfr_discovery/emd_metric.py
--rw-r--r--   0        0        0      489 2023-05-15 07:00:12.345364 prosimos-1.2.3/bpdfr_discovery/exceptions.py
--rw-r--r--   0        0        0     7248 2023-05-15 07:00:12.345364 prosimos-1.2.3/bpdfr_discovery/inter_arrival_cases_discovery.py
--rw-r--r--   0        0        0     5615 2023-05-15 07:00:12.345364 prosimos-1.2.3/bpdfr_discovery/log_comparison_metrics.py
--rw-r--r--   0        0        0    44018 2023-05-15 07:00:12.345364 prosimos-1.2.3/bpdfr_discovery/log_parser.py
--rw-r--r--   0        0        0        0 2023-05-15 07:00:12.345364 prosimos-1.2.3/cli/__init__.py
--rw-r--r--   0        0        0     3539 2023-05-15 07:00:12.345364 prosimos-1.2.3/cli/diff_res_bpsim.py
--rw-r--r--   0        0        0        0 2023-05-15 07:00:12.449369 prosimos-1.2.3/prosimos/__init__.py
--rw-r--r--   0        0        0    44562 2023-05-15 07:00:12.449369 prosimos-1.2.3/prosimos/batch_processing.py
--rw-r--r--   0        0        0     4383 2023-05-15 07:00:12.449369 prosimos-1.2.3/prosimos/batch_processing_parser.py
--rw-r--r--   0        0        0     2626 2023-05-15 07:00:12.449369 prosimos-1.2.3/prosimos/case_attributes.py
--rw-r--r--   0        0        0    48440 2023-05-15 07:00:12.449369 prosimos-1.2.3/prosimos/control_flow_manager.py
--rw-r--r--   0        0        0      487 2023-05-15 07:00:12.449369 prosimos-1.2.3/prosimos/exceptions.py
--rw-r--r--   0        0        0     7340 2023-05-15 07:00:12.449369 prosimos-1.2.3/prosimos/execution_info.py
--rw-r--r--   0        0        0     1109 2023-05-15 07:00:12.449369 prosimos-1.2.3/prosimos/file_manager.py
--rw-r--r--   0        0        0     3147 2023-05-15 07:00:12.449369 prosimos-1.2.3/prosimos/prioritisation.py
--rw-r--r--   0        0        0     1345 2023-05-15 07:00:12.449369 prosimos-1.2.3/prosimos/prioritisation_parser.py
--rw-r--r--   0        0        0     3009 2023-05-15 07:00:12.449369 prosimos-1.2.3/prosimos/prioritisation_rules.py
--rw-r--r--   0        0        0     8585 2023-05-15 07:00:12.449369 prosimos-1.2.3/prosimos/probability_distributions.py
--rw-r--r--   0        0        0    41729 2023-05-15 07:00:12.449369 prosimos-1.2.3/prosimos/resource_calendar.py
--rw-r--r--   0        0        0      467 2023-05-15 07:00:12.449369 prosimos-1.2.3/prosimos/resource_profile.py
--rw-r--r--   0        0        0    28588 2023-05-15 07:00:12.449369 prosimos-1.2.3/prosimos/simulation_engine.py
--rw-r--r--   0        0        0    22058 2023-05-15 07:00:12.449369 prosimos-1.2.3/prosimos/simulation_properties_parser.py
--rw-r--r--   0        0        0     6298 2023-05-15 07:00:12.449369 prosimos-1.2.3/prosimos/simulation_queues_ds.py
--rw-r--r--   0        0        0     6003 2023-05-15 07:00:12.449369 prosimos-1.2.3/prosimos/simulation_setup.py
--rw-r--r--   0        0        0    15565 2023-05-15 07:00:12.453369 prosimos-1.2.3/prosimos/simulation_stats.py
--rw-r--r--   0        0        0    14157 2023-05-15 07:00:12.453369 prosimos-1.2.3/prosimos/simulation_stats_calculator.py
--rw-r--r--   0        0        0     1714 2023-05-15 07:00:12.453369 prosimos-1.2.3/prosimos/weekday_helper.py
--rw-r--r--   0        0        0      612 2023-05-15 07:00:12.453369 prosimos-1.2.3/pyproject.toml
--rw-r--r--   0        0        0    15464 1970-01-01 00:00:00.000000 prosimos-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0    15059 2023-05-24 09:38:28.436268 prosimos-1.2.4/README.md
+-rw-r--r--   0        0        0        0 2023-05-24 09:38:28.456268 prosimos-1.2.4/bpdfr_discovery/__init__.py
+-rw-r--r--   0        0        0     3478 2023-05-24 09:38:28.456268 prosimos-1.2.4/bpdfr_discovery/emd_metric.py
+-rw-r--r--   0        0        0      489 2023-05-24 09:38:28.456268 prosimos-1.2.4/bpdfr_discovery/exceptions.py
+-rw-r--r--   0        0        0     7248 2023-05-24 09:38:28.456268 prosimos-1.2.4/bpdfr_discovery/inter_arrival_cases_discovery.py
+-rw-r--r--   0        0        0     5615 2023-05-24 09:38:28.456268 prosimos-1.2.4/bpdfr_discovery/log_comparison_metrics.py
+-rw-r--r--   0        0        0    44084 2023-05-24 09:38:28.456268 prosimos-1.2.4/bpdfr_discovery/log_parser.py
+-rw-r--r--   0        0        0        0 2023-05-24 09:38:28.456268 prosimos-1.2.4/cli/__init__.py
+-rw-r--r--   0        0        0     3539 2023-05-24 09:38:28.456268 prosimos-1.2.4/cli/diff_res_bpsim.py
+-rw-r--r--   0        0        0        0 2023-05-24 09:38:28.556268 prosimos-1.2.4/prosimos/__init__.py
+-rw-r--r--   0        0        0    44577 2023-05-24 09:38:28.556268 prosimos-1.2.4/prosimos/batch_processing.py
+-rw-r--r--   0        0        0     4383 2023-05-24 09:38:28.556268 prosimos-1.2.4/prosimos/batch_processing_parser.py
+-rw-r--r--   0        0        0     2626 2023-05-24 09:38:28.556268 prosimos-1.2.4/prosimos/case_attributes.py
+-rw-r--r--   0        0        0    48440 2023-05-24 09:38:28.556268 prosimos-1.2.4/prosimos/control_flow_manager.py
+-rw-r--r--   0        0        0      487 2023-05-24 09:38:28.556268 prosimos-1.2.4/prosimos/exceptions.py
+-rw-r--r--   0        0        0     7340 2023-05-24 09:38:28.556268 prosimos-1.2.4/prosimos/execution_info.py
+-rw-r--r--   0        0        0     1109 2023-05-24 09:38:28.556268 prosimos-1.2.4/prosimos/file_manager.py
+-rw-r--r--   0        0        0     3147 2023-05-24 09:38:28.556268 prosimos-1.2.4/prosimos/prioritisation.py
+-rw-r--r--   0        0        0     1345 2023-05-24 09:38:28.556268 prosimos-1.2.4/prosimos/prioritisation_parser.py
+-rw-r--r--   0        0        0     3009 2023-05-24 09:38:28.556268 prosimos-1.2.4/prosimos/prioritisation_rules.py
+-rw-r--r--   0        0        0     8585 2023-05-24 09:38:28.556268 prosimos-1.2.4/prosimos/probability_distributions.py
+-rw-r--r--   0        0        0      467 2023-05-24 09:38:28.556268 prosimos-1.2.4/prosimos/resource_profile.py
+-rw-r--r--   0        0        0    29275 2023-05-24 09:38:28.556268 prosimos-1.2.4/prosimos/simulation_engine.py
+-rw-r--r--   0        0        0    22072 2023-05-24 09:38:28.556268 prosimos-1.2.4/prosimos/simulation_properties_parser.py
+-rw-r--r--   0        0        0     6298 2023-05-24 09:38:28.560268 prosimos-1.2.4/prosimos/simulation_queues_ds.py
+-rw-r--r--   0        0        0     6005 2023-05-24 09:38:28.560268 prosimos-1.2.4/prosimos/simulation_setup.py
+-rw-r--r--   0        0        0    15565 2023-05-24 09:38:28.560268 prosimos-1.2.4/prosimos/simulation_stats.py
+-rw-r--r--   0        0        0    14171 2023-05-24 09:38:28.560268 prosimos-1.2.4/prosimos/simulation_stats_calculator.py
+-rw-r--r--   0        0        0     1730 2023-05-24 09:38:28.560268 prosimos-1.2.4/prosimos/weekday_helper.py
+-rw-r--r--   0        0        0      637 2023-05-24 09:38:28.560268 prosimos-1.2.4/pyproject.toml
+-rw-r--r--   0        0        0    15764 1970-01-01 00:00:00.000000 prosimos-1.2.4/PKG-INFO
```

### Comparing `prosimos-1.2.3/README.md` & `prosimos-1.2.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 # Prosimos
 
+![build](https://github.com/AutomatedProcessImprovement/prosimos/actions/workflows/python.yml/badge.svg)
+![release](https://github.com/AutomatedProcessImprovement/prosimos/actions/workflows/release-pypi.yml/badge.svg)
+![version](https://img.shields.io/github/v/tag/AutomatedProcessImprovement/prosimos)
+
 Prosimos is a Business Process Simulation Engine that supports differentiated resources. 
 Prosimos considers resource pools formed by a set of resources (process participants) with different profiles. 
 For example, each resource has individual calendars, costs, and a differentiated performance to execute the process activities. 
 Besides, pools can share resources, i.e., a resource may play different roles in the organization, thus performing several tasks.
 
 ## Requirements
 
-- Python 3.8+
+- Python 3.9+
 - Poetry 1.4.2
 - For dependencies, please, check `pyproject.toml`
 
 ## Getting Started
 
     git clone https://github.com/AutomatedProcessImprovement/Prosimos.git
```

### Comparing `prosimos-1.2.3/bpdfr_discovery/emd_metric.py` & `prosimos-1.2.4/bpdfr_discovery/emd_metric.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.3/bpdfr_discovery/inter_arrival_cases_discovery.py` & `prosimos-1.2.4/bpdfr_discovery/inter_arrival_cases_discovery.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.3/bpdfr_discovery/log_comparison_metrics.py` & `prosimos-1.2.4/bpdfr_discovery/log_comparison_metrics.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.3/bpdfr_discovery/log_parser.py` & `prosimos-1.2.4/bpdfr_discovery/log_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 import json
 import sys
 from datetime import datetime
 
 import numpy as np
 import pandas as pd
 import pytz
+from pix_framework.calendar.resource_calendar import RCalendar
+from pix_framework.discovery.calendar_factory import CalendarFactory
 
 from bpdfr_discovery.exceptions import InvalidInputDiscoveryParameters
 from prosimos.control_flow_manager import BPMN, BPMNGraph
 from prosimos.exceptions import InvalidBpmnModelException, InvalidLogFileException
 from prosimos.execution_info import Trace, TaskEvent
 from prosimos.file_manager import FileManager
 from prosimos.probability_distributions import best_fit_distribution
-from prosimos.resource_calendar import RCalendar, CalendarFactory
 from prosimos.simulation_properties_parser import parse_simulation_model
 
 print_info = False
 
 
 def event_list_from_xes_log(log_path):
     from pm4py.objects.log.importer.xes import importer as xes_importer
```

### Comparing `prosimos-1.2.3/cli/diff_res_bpsim.py` & `prosimos-1.2.4/cli/diff_res_bpsim.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.3/prosimos/batch_processing.py` & `prosimos-1.2.4/prosimos/batch_processing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-from enum import Enum
 import operator as operator
-from random import choices
 import sys
-from typing import List
 from datetime import date, datetime, time, timedelta
-from prosimos.exceptions import InvalidRuleDefinition
+from enum import Enum
+from random import choices
+from typing import List
 
-from prosimos.resource_calendar import str_week_days
+from pix_framework.calendar.resource_calendar import str_week_days
+
+from prosimos.exceptions import InvalidRuleDefinition
 from prosimos.weekday_helper import CustomDatetimeAndSeconds, get_nearest_abs_day, get_nearest_past_day
 
 
 def _get_operator_symbols(operator_str: str, eq_operator: operator):
     OPERATOR_SYMBOLS = {
         '<': operator.lt,
         '<=': operator.le,
```

### Comparing `prosimos-1.2.3/prosimos/batch_processing_parser.py` & `prosimos-1.2.4/prosimos/batch_processing_parser.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.3/prosimos/case_attributes.py` & `prosimos-1.2.4/prosimos/case_attributes.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.3/prosimos/control_flow_manager.py` & `prosimos-1.2.4/prosimos/control_flow_manager.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.3/prosimos/execution_info.py` & `prosimos-1.2.4/prosimos/execution_info.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.3/prosimos/file_manager.py` & `prosimos-1.2.4/prosimos/file_manager.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.3/prosimos/prioritisation.py` & `prosimos-1.2.4/prosimos/prioritisation.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.3/prosimos/prioritisation_parser.py` & `prosimos-1.2.4/prosimos/prioritisation_parser.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.3/prosimos/prioritisation_rules.py` & `prosimos-1.2.4/prosimos/prioritisation_rules.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.3/prosimos/probability_distributions.py` & `prosimos-1.2.4/prosimos/probability_distributions.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.3/prosimos/simulation_engine.py` & `prosimos-1.2.4/prosimos/simulation_engine.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 import csv
+import datetime
+from datetime import timedelta
 from typing import List
 
 import pytz
-import datetime
-from datetime import timedelta
+from dateutil import parser
+
 from prosimos.control_flow_manager import (
     BPMN,
     CustomDatetimeAndSeconds,
 )
-
-from prosimos.file_manager import FileManager
 from prosimos.execution_info import Trace, TaskEvent, EnabledEvent
+from prosimos.file_manager import FileManager
 from prosimos.prioritisation import CasePrioritisation
-from prosimos.resource_calendar import get_string_from_datetime
-from prosimos.resource_calendar import parse_datetime
 from prosimos.simulation_queues_ds import (
-    PriorityQueue,
     DiffResourceQueue,
     EventQueue,
 )
 from prosimos.simulation_setup import SimDiffSetup
 from prosimos.simulation_stats_calculator import LogInfo
 
 
@@ -720,18 +718,41 @@
 
     return None
 
 
 def verify_miliseconds(array):
     """
     In case of datetime.microsecond = 0, standard converter does not print microseconds
-    So we force the convertation, so that the datetime format is the same for every datetime in the final file
+    So we force the conversion, so that the datetime format is the same for every datetime in the final file
     Indexes correspond to the next values:
         2 - enabled_datetime
         3 - start_datetime
         4 - end_datetime
     """
     for i in range(2, 5):
         if array[i].microsecond == 0:
-            array[i] = get_string_from_datetime(array[i])
+            array[i] = _get_string_from_datetime(array[i])
 
     return array
+
+
+def _get_string_from_datetime(datetime):
+    datetime_without_colon = datetime.strftime("%Y-%m-%d %H:%M:%S.%f%z")
+    return "{0}:{1}".format(
+        datetime_without_colon[:-2],
+        datetime_without_colon[-2:]
+    )
+
+
+def parse_datetime(time, has_date):
+    time_formats = ['%H:%M:%S.%f', '%H:%M', '%I:%M%p', '%H:%M:%S', '%I:%M:%S%p'] if not has_date \
+        else ['%Y-%m-%dT%H:%M:%S.%f%z', '%b %d %Y %I:%M%p', '%b %d %Y at %I:%M%p',
+              '%B %d, %Y, %H:%M:%S', '%a,%d/%m/%y,%I:%M%p', '%a, %d %B, %Y', '%Y-%m-%dT%H:%M:%SZ']
+    try:
+        return parser.parse(time)
+    except:
+        for time_format in time_formats:
+            try:
+                return datetime.datetime.strptime(time, time_format)
+            except ValueError:
+                pass
+    raise ValueError
```

### Comparing `prosimos-1.2.3/prosimos/simulation_properties_parser.py` & `prosimos-1.2.4/prosimos/simulation_properties_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import json
 import xml.etree.ElementTree as ET
 
 from numpy import exp, log, sqrt
+from pix_framework.calendar.resource_calendar import RCalendar
 
 from prosimos.batch_processing_parser import BatchProcessingParser
 from prosimos.case_attributes import AllCaseAttributes, CaseAttribute
 from prosimos.control_flow_manager import (
     BPMN,
     EVENT_TYPE,
     BPMNGraph,
     ElementInfo,
 )
 from prosimos.prioritisation import AllPriorityRules
 from prosimos.prioritisation_parser import PrioritisationParser
 from prosimos.probability_distributions import *
-from prosimos.resource_calendar import RCalendar
 from prosimos.resource_profile import PoolInfo, ResourceProfile
 
 bpmn_schema_url = "http://www.omg.org/spec/BPMN/20100524/MODEL"
 simod_ns = {"qbp": "http://www.qbp-simulator.com/Schema201212"}
 bpmn_element_ns = {"xmlns": bpmn_schema_url}
 
 EVENT_DISTRIBUTION_SECTION = "event_distribution"
```

### Comparing `prosimos-1.2.3/prosimos/simulation_queues_ds.py` & `prosimos-1.2.4/prosimos/simulation_queues_ds.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.3/prosimos/simulation_setup.py` & `prosimos-1.2.4/prosimos/simulation_setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-import pytz
 import datetime
-from datetime import timedelta
 import ntpath
-from prosimos.batch_processing import BatchConfigPerTask
+from datetime import timedelta
 from typing import Optional
 
+import pytz
+from pix_framework.calendar.resource_calendar import RCalendar
+
+from prosimos.batch_processing import BatchConfigPerTask
 from prosimos.control_flow_manager import ProcessState, ElementInfo, BPMN
 from prosimos.probability_distributions import generate_number_from
-from prosimos.resource_calendar import RCalendar
 from prosimos.simulation_properties_parser import parse_simulation_model, parse_json_sim_parameters
 
 
 class SimDiffSetup:
     def __init__(self, bpmn_path, json_path, is_event_added_to_log, total_cases):
         self.process_name = ntpath.basename(bpmn_path).split(".")[0]
         self.start_datetime = datetime.datetime.now(pytz.utc)
@@ -23,15 +24,15 @@
         self.bpmn_graph = parse_simulation_model(bpmn_path)
         self.bpmn_graph.set_additional_fields_from_json(self.element_probability, \
             self.task_resource, self.event_distibution, self.batch_processing)
         if not self.arrival_calendar:
             self.arrival_calendar = self.find_arrival_calendar()
 
         self.is_event_added_to_log = is_event_added_to_log
-        self.total_num_cases = total_cases # how many process cases should be simulated
+        self.total_num_cases = total_cases  # how many process cases should be simulated
 
     def verify_simulation_input(self):
         for e_id in self.bpmn_graph.element_info:
             e_info: ElementInfo = self.bpmn_graph[e_id]
             if e_info.type == BPMN.TASK and e_info.id not in self.task_resource:
                 print("WARNING: No resource assigned to task %s" % e_info.name)
             if e_info.type in [BPMN.INCLUSIVE_GATEWAY, BPMN.EXCLUSIVE_GATEWAY] and e_info.is_split():
@@ -85,28 +86,27 @@
                     continue
                 arrival_calendar.combine_calendar(self.calendars_map[self.resources_map[r_id].calendar_id])
                 starter_resources.add(r_id)
         return arrival_calendar
 
     def ideal_task_duration(self, task_id, resource_id, num_tasks_in_batch):
         val = generate_number_from(self.task_resource[task_id][resource_id]['distribution_name'],
-                        self.task_resource[task_id][resource_id]['distribution_params'])
-                        
+                                   self.task_resource[task_id][resource_id]['distribution_params'])
+
         if num_tasks_in_batch == 0:
             # task executed NOT in batch
             return val
         else:
             # task executed as a part of the batch
             curr_batch_info: Optional[BatchConfigPerTask] = self.batch_processing.get(task_id, None)
             if curr_batch_info == None:
                 print(f"WARNING: Could not find info about batch_processing for task {task_id}")
 
             return curr_batch_info.calculate_ideal_duration(val, num_tasks_in_batch)
 
-
     def real_task_duration(self, task_duration, resource_id, enabled_at):
         return self.calendars_map[self.resources_map[resource_id].calendar_id].find_idle_time(enabled_at, task_duration)
 
     def set_starting_datetime(self, new_datetime):
         (
             is_inside_arrival_calendar,
             _,
```

### Comparing `prosimos-1.2.3/prosimos/simulation_stats.py` & `prosimos-1.2.4/prosimos/simulation_stats.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.3/prosimos/simulation_stats_calculator.py` & `prosimos-1.2.4/prosimos/simulation_stats_calculator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 import datetime
 import pytz
 from prosimos.control_flow_manager import BPMN
 
-from prosimos.resource_calendar import Interval
+from pix_framework.calendar.resource_calendar import Interval
 
 from prosimos.execution_info import TaskEvent, Trace
 from prosimos.simulation_setup import SimDiffSetup
 
 
 class KPIInfo:
     def __init__(self):
```

### Comparing `prosimos-1.2.3/prosimos/weekday_helper.py` & `prosimos-1.2.4/prosimos/weekday_helper.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from datetime import timedelta
-from prosimos.resource_calendar import str_week_days
+
+from pix_framework.calendar.resource_calendar import str_week_days
+
 
 class CustomDatetimeAndSeconds:
     def __init__(self, seconds_from_start, datetime):
         self.seconds_from_start = seconds_from_start
         self.datetime = datetime
 
 def get_nearest_abs_day(weekday, from_datetime):
```

### Comparing `prosimos-1.2.3/pyproject.toml` & `prosimos-1.2.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [tool.poetry]
 name = "prosimos"
-version = "1.2.3"
+version = "1.2.4"
 description = ""
 authors = ["Iryna Halenok, Orlenys López Pintado"]
 readme = "README.md"
 packages = [
     {include = "cli"},
     {include = "prosimos"},
     {include = "bpdfr_discovery"}
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.12"
+python = ">=3.9,<3.12"
 click = "^8.1.3"
 numpy = "^1.24.3"
 pandas = "^2.0.1"
 python-dateutil = "^2.8.2"
 pytz = "^2023.3"
 scipy = "^1.10.1"
 pm4py = "^2.7.4"
+pix-framework = "^0.8.7"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.3.1"
 
 [tool.poetry.scripts]
 prosimos = "cli.diff_res_bpsim:cli"
```

### Comparing `prosimos-1.2.3/PKG-INFO` & `prosimos-1.2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 Metadata-Version: 2.1
 Name: prosimos
-Version: 1.2.3
+Version: 1.2.4
 Summary: 
 Author: Iryna Halenok, Orlenys López Pintado
-Requires-Python: >=3.8,<3.12
+Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
+Requires-Dist: pix-framework (>=0.8.7,<0.9.0)
 Requires-Dist: pm4py (>=2.7.4,<3.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: pytz (>=2023.3,<2024.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Prosimos
 
+![build](https://github.com/AutomatedProcessImprovement/prosimos/actions/workflows/python.yml/badge.svg)
+![release](https://github.com/AutomatedProcessImprovement/prosimos/actions/workflows/release-pypi.yml/badge.svg)
+![version](https://img.shields.io/github/v/tag/AutomatedProcessImprovement/prosimos)
+
 Prosimos is a Business Process Simulation Engine that supports differentiated resources. 
 Prosimos considers resource pools formed by a set of resources (process participants) with different profiles. 
 For example, each resource has individual calendars, costs, and a differentiated performance to execute the process activities. 
 Besides, pools can share resources, i.e., a resource may play different roles in the organization, thus performing several tasks.
 
 ## Requirements
 
-- Python 3.8+
+- Python 3.9+
 - Poetry 1.4.2
 - For dependencies, please, check `pyproject.toml`
 
 ## Getting Started
 
     git clone https://github.com/AutomatedProcessImprovement/Prosimos.git
```

