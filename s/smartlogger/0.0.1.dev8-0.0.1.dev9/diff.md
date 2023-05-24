# Comparing `tmp/smartlogger-0.0.1.dev8.tar.gz` & `tmp/smartlogger-0.0.1.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartlogger-0.0.1.dev8.tar", last modified: Mon May 22 11:31:55 2023, max compression
+gzip compressed data, was "smartlogger-0.0.1.dev9.tar", last modified: Wed May 24 13:50:36 2023, max compression
```

## Comparing `smartlogger-0.0.1.dev8.tar` & `smartlogger-0.0.1.dev9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:31:55.414636 smartlogger-0.0.1.dev8/
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-22 11:31:55.414636 smartlogger-0.0.1.dev8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-22 11:31:44.000000 smartlogger-0.0.1.dev8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 11:31:55.414636 smartlogger-0.0.1.dev8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-05-22 11:31:44.000000 smartlogger-0.0.1.dev8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:31:55.414636 smartlogger-0.0.1.dev8/smartlogger/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-22 11:31:44.000000 smartlogger-0.0.1.dev8/smartlogger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-22 11:31:44.000000 smartlogger-0.0.1.dev8/smartlogger/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-05-22 11:31:44.000000 smartlogger-0.0.1.dev8/smartlogger/smartlogger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:31:55.414636 smartlogger-0.0.1.dev8/smartlogger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-22 11:31:55.000000 smartlogger-0.0.1.dev8/smartlogger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-22 11:31:55.000000 smartlogger-0.0.1.dev8/smartlogger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 11:31:55.000000 smartlogger-0.0.1.dev8/smartlogger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-22 11:31:55.000000 smartlogger-0.0.1.dev8/smartlogger.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-22 11:31:55.000000 smartlogger-0.0.1.dev8/smartlogger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-22 11:31:55.000000 smartlogger-0.0.1.dev8/smartlogger.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:50:36.428397 smartlogger-0.0.1.dev9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-24 13:50:36.428397 smartlogger-0.0.1.dev9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-24 13:50:27.000000 smartlogger-0.0.1.dev9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 13:50:36.428397 smartlogger-0.0.1.dev9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-05-24 13:50:27.000000 smartlogger-0.0.1.dev9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:50:36.424397 smartlogger-0.0.1.dev9/smartlogger/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-24 13:50:27.000000 smartlogger-0.0.1.dev9/smartlogger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-24 13:50:27.000000 smartlogger-0.0.1.dev9/smartlogger/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-05-24 13:50:27.000000 smartlogger-0.0.1.dev9/smartlogger/smartlogger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:50:36.428397 smartlogger-0.0.1.dev9/smartlogger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-24 13:50:36.000000 smartlogger-0.0.1.dev9/smartlogger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-24 13:50:36.000000 smartlogger-0.0.1.dev9/smartlogger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 13:50:36.000000 smartlogger-0.0.1.dev9/smartlogger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-24 13:50:36.000000 smartlogger-0.0.1.dev9/smartlogger.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-24 13:50:36.000000 smartlogger-0.0.1.dev9/smartlogger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-24 13:50:36.000000 smartlogger-0.0.1.dev9/smartlogger.egg-info/top_level.txt
```

### Comparing `smartlogger-0.0.1.dev8/PKG-INFO` & `smartlogger-0.0.1.dev9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartlogger
-Version: 0.0.1.dev8
+Version: 0.0.1.dev9
 Summary: python logging client for SmartDash
 Home-page: https://github.com/notAI-tech/smartdash
 Author: BEDAPUDI PRANEETH
 Author-email: praneeth@bpraneeth.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `smartlogger-0.0.1.dev8/README.md` & `smartlogger-0.0.1.dev9/README.md`

 * *Files identical despite different names*

### Comparing `smartlogger-0.0.1.dev8/setup.py` & `smartlogger-0.0.1.dev9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = "smartlogger"
 DESCRIPTION = "python logging client for SmartDash"
 URL = "https://github.com/notAI-tech/smartdash"
 EMAIL = "praneeth@bpraneeth.com"
 AUTHOR = "BEDAPUDI PRANEETH"
 REQUIRES_PYTHON = ">=3.6.0"
-VERSION = "0.0.1.dev8"
+VERSION = "0.0.1.dev9"
 
 # What packages are required for this module to be executed?
 REQUIRED = ["requests", "liteindex"]
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
```

### Comparing `smartlogger-0.0.1.dev8/smartlogger/smartlogger.py` & `smartlogger-0.0.1.dev9/smartlogger/smartlogger.py`

 * *Files 12% similar despite different names*

```diff
@@ -118,28 +118,31 @@
                 "failed": True,
                 "start": False,
             }
         )
 
 
 class SmartLogger:
-    def __init__(self, name, save_to_dir="./"):
+    def __init__(self, name, save_to_dir="./", log_to_console=True):
         self.name = name
+        self.log_to_console = log_to_console
+
         self.logs_index = DefinedIndex(
             f"{self.name}_logs",
             schema={
                 "u_id": "",
                 "level": "",
                 "messages": [],
                 "timestamp": 0,
                 "stage": "",
             },
             db_path=os.path.join(save_to_dir, f"{self.name}_logs.db"),
             auto_key=True,
         )
+
         self.ml_inputs_outputs_index = DefinedIndex(
             f"{self.name}_ml_inputs_outputs",
             schema={
                 "u_id": "",
                 "inputs": [],
                 "outputs": [],
                 "model_type": "",
@@ -158,24 +161,49 @@
                 "level": level,
                 "messages": [str(_) for _ in messages],
                 "timestamp": timestamp,
                 "stage": stage,
             }
         )
 
+        if self.log_to_console:
+            self._print_to_console(timestamp, id, level, messages, stage)
+
+    def _print_to_console(self, timestamp, id, level, messages, stage):
+        timestamp = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(timestamp))
+        log_colors = {
+            "INFO": "\033[94m",
+            "WARNING": "\033[93m",
+            "ERROR": "\033[91m",
+            "EXCEPTION": "\033[91m",
+            "DEBUG": "\033[92m",
+        }
+        stage_color = "\033[95m"
+        reset_color = "\033[0m"
+
+        formatted_message = f"{log_colors[level]}{timestamp} {id} {stage_color}{stage}: {level}: {reset_color}"
+        for message in messages:
+            formatted_message += f"{message} "
+
+        print(formatted_message)
+
     def debug(self, id, *messages, stage=None):
         self._log(id, "DEBUG", *messages, stage=stage)
 
     def info(self, id, *messages, stage=None):
         self._log(id, "INFO", *messages, stage=stage)
 
     def warning(self, id, *messages, stage=None):
         self._log(id, "WARNING", *messages, stage=stage)
 
-    def exception(self, id, *messages, stage=None):
+    def error(self, id, *messages, stage=None):
+        self._log(id, "ERROR", *messages, stage=stage)
+
+    def exception(self, id, exc, *messages, stage=None):
+        messages = (str(exc),) + messages
         self._log(id, "EXCEPTION", *messages, stage=stage)
 
     def ml_inputs_outputs(self, id, inputs, outputs, model_type, stage=None):
         if not isinstance(inputs, (list, tuple)):
             raise ValueError("inputs must be a list or tuple")
         if not isinstance(outputs, (list, tuple)):
             raise ValueError("outputs must be a list or tuple")
```

### Comparing `smartlogger-0.0.1.dev8/smartlogger.egg-info/PKG-INFO` & `smartlogger-0.0.1.dev9/smartlogger.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartlogger
-Version: 0.0.1.dev8
+Version: 0.0.1.dev9
 Summary: python logging client for SmartDash
 Home-page: https://github.com/notAI-tech/smartdash
 Author: BEDAPUDI PRANEETH
 Author-email: praneeth@bpraneeth.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

