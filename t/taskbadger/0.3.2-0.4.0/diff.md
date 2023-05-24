# Comparing `tmp/taskbadger-0.3.2.tar.gz` & `tmp/taskbadger-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskbadger-0.3.2.tar", max compression
+gzip compressed data, was "taskbadger-0.4.0.tar", max compression
```

## Comparing `taskbadger-0.3.2.tar` & `taskbadger-0.4.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0    11357 2023-04-01 18:07:49.396917 taskbadger-0.3.2/LICENSE
--rw-r--r--   0        0        0     1650 2023-04-04 19:59:48.817874 taskbadger-0.3.2/README.md
--rw-r--r--   0        0        0     1751 2023-04-04 20:00:06.714013 taskbadger-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      405 2023-04-04 19:58:44.625340 taskbadger-0.3.2/taskbadger/__init__.py
--rw-r--r--   0        0        0     5174 2023-04-04 19:58:48.329372 taskbadger-0.3.2/taskbadger/cli.py
--rw-r--r--   0        0        0     3253 2023-04-04 19:58:48.329372 taskbadger-0.3.2/taskbadger/config.py
--rw-r--r--   0        0        0      250 2023-04-01 18:07:49.396917 taskbadger-0.3.2/taskbadger/exceptions.py
--rw-r--r--   0        0        0     1008 2023-04-04 19:37:59.419308 taskbadger-0.3.2/taskbadger/integrations.py
--rw-r--r--   0        0        0      155 2023-04-03 15:10:25.786742 taskbadger-0.3.2/taskbadger/internal/__init__.py
--rw-r--r--   0        0        0       47 2023-04-03 15:10:26.042799 taskbadger-0.3.2/taskbadger/internal/api/__init__.py
--rw-r--r--   0        0        0        0 2023-04-03 15:10:26.126818 taskbadger-0.3.2/taskbadger/internal/api/action_endpoints/__init__.py
--rw-r--r--   0        0        0     3318 2023-04-03 15:10:27.351088 taskbadger-0.3.2/taskbadger/internal/api/action_endpoints/action_cancel.py
--rw-r--r--   0        0        0     5393 2023-04-03 15:10:27.363091 taskbadger-0.3.2/taskbadger/internal/api/action_endpoints/action_create.py
--rw-r--r--   0        0        0     5005 2023-04-03 15:10:27.371092 taskbadger-0.3.2/taskbadger/internal/api/action_endpoints/action_get.py
--rw-r--r--   0        0        0     5097 2023-04-03 15:10:27.359090 taskbadger-0.3.2/taskbadger/internal/api/action_endpoints/action_list.py
--rw-r--r--   0        0        0     5676 2023-04-03 15:10:27.439107 taskbadger-0.3.2/taskbadger/internal/api/action_endpoints/action_partial_update.py
--rw-r--r--   0        0        0     5556 2023-04-03 15:10:27.399098 taskbadger-0.3.2/taskbadger/internal/api/action_endpoints/action_update.py
--rw-r--r--   0        0        0        0 2023-04-03 15:10:26.066805 taskbadger-0.3.2/taskbadger/internal/api/task_endpoints/__init__.py
--rw-r--r--   0        0        0     3123 2023-04-03 15:10:27.339085 taskbadger-0.3.2/taskbadger/internal/api/task_endpoints/task_cancel.py
--rw-r--r--   0        0        0     5770 2023-04-04 19:37:59.419308 taskbadger-0.3.2/taskbadger/internal/api/task_endpoints/task_create.py
--rw-r--r--   0        0        0     4662 2023-04-03 15:10:27.543130 taskbadger-0.3.2/taskbadger/internal/api/task_endpoints/task_get.py
--rw-r--r--   0        0        0     5872 2023-04-03 15:10:27.615146 taskbadger-0.3.2/taskbadger/internal/api/task_endpoints/task_list.py
--rw-r--r--   0        0        0     5359 2023-04-03 15:10:27.619147 taskbadger-0.3.2/taskbadger/internal/api/task_endpoints/task_partial_update.py
--rw-r--r--   0        0        0     5167 2023-04-03 15:10:27.567135 taskbadger-0.3.2/taskbadger/internal/api/task_endpoints/task_update.py
--rw-r--r--   0        0        0     2673 2023-04-03 15:10:27.495119 taskbadger-0.3.2/taskbadger/internal/client.py
--rw-r--r--   0        0        0      282 2023-04-03 15:10:27.463112 taskbadger-0.3.2/taskbadger/internal/errors.py
--rw-r--r--   0        0        0     1022 2023-04-03 15:10:26.038798 taskbadger-0.3.2/taskbadger/internal/models/__init__.py
--rw-r--r--   0        0        0     3234 2023-04-03 15:10:27.599142 taskbadger-0.3.2/taskbadger/internal/models/action.py
--rw-r--r--   0        0        0     1152 2023-04-03 15:10:27.563134 taskbadger-0.3.2/taskbadger/internal/models/action_config.py
--rw-r--r--   0        0        0     2405 2023-04-03 15:10:27.615146 taskbadger-0.3.2/taskbadger/internal/models/action_request.py
--rw-r--r--   0        0        0     1190 2023-04-03 15:10:27.607144 taskbadger-0.3.2/taskbadger/internal/models/action_request_config.py
--rw-r--r--   0        0        0     2590 2023-04-03 15:10:27.691162 taskbadger-0.3.2/taskbadger/internal/models/paginated_task_list.py
--rw-r--r--   0        0        0     2638 2023-04-03 15:10:27.719169 taskbadger-0.3.2/taskbadger/internal/models/patched_action_request.py
--rw-r--r--   0        0        0     1228 2023-04-03 15:10:27.647153 taskbadger-0.3.2/taskbadger/internal/models/patched_action_request_config.py
--rw-r--r--   0        0        0     6107 2023-04-04 19:37:59.419308 taskbadger-0.3.2/taskbadger/internal/models/patched_task_request.py
--rw-r--r--   0        0        0     1222 2023-04-03 15:10:27.675159 taskbadger-0.3.2/taskbadger/internal/models/patched_task_request_data.py
--rw-r--r--   0        0        0      339 2023-04-04 19:37:59.419308 taskbadger-0.3.2/taskbadger/internal/models/status_enum.py
--rw-r--r--   0        0        0     7435 2023-04-04 19:37:59.419308 taskbadger-0.3.2/taskbadger/internal/models/task.py
--rw-r--r--   0        0        0     1146 2023-04-03 15:10:27.683161 taskbadger-0.3.2/taskbadger/internal/models/task_data.py
--rw-r--r--   0        0        0     5965 2023-04-04 19:37:59.419308 taskbadger-0.3.2/taskbadger/internal/models/task_request.py
--rw-r--r--   0        0        0     1184 2023-04-03 15:10:27.723169 taskbadger-0.3.2/taskbadger/internal/models/task_request_data.py
--rw-r--r--   0        0        0       25 2023-04-04 19:37:59.419308 taskbadger-0.3.2/taskbadger/internal/py.typed
--rw-r--r--   0        0        0      974 2023-04-03 15:10:27.723169 taskbadger-0.3.2/taskbadger/internal/types.py
--rw-r--r--   0        0        0     9802 2023-04-04 19:37:59.419308 taskbadger-0.3.2/taskbadger/sdk.py
--rw-r--r--   0        0        0     2882 1970-01-01 00:00:00.000000 taskbadger-0.3.2/setup.py
--rw-r--r--   0        0        0     3191 1970-01-01 00:00:00.000000 taskbadger-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-01 18:07:49.396917 taskbadger-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1649 2023-05-24 06:53:11.963809 taskbadger-0.4.0/README.md
+-rw-r--r--   0        0        0     1751 2023-05-24 06:53:11.963809 taskbadger-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      405 2023-04-07 06:55:09.353665 taskbadger-0.4.0/taskbadger/__init__.py
+-rw-r--r--   0        0        0     5175 2023-05-24 06:53:11.963809 taskbadger-0.4.0/taskbadger/cli.py
+-rw-r--r--   0        0        0     3253 2023-04-04 19:58:48.329372 taskbadger-0.4.0/taskbadger/config.py
+-rw-r--r--   0        0        0      250 2023-04-01 18:07:49.396917 taskbadger-0.4.0/taskbadger/exceptions.py
+-rw-r--r--   0        0        0     1008 2023-04-04 19:37:59.419308 taskbadger-0.4.0/taskbadger/integrations.py
+-rw-r--r--   0        0        0      155 2023-04-03 15:10:25.786742 taskbadger-0.4.0/taskbadger/internal/__init__.py
+-rw-r--r--   0        0        0       47 2023-04-03 15:10:26.042799 taskbadger-0.4.0/taskbadger/internal/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-03 15:10:26.126818 taskbadger-0.4.0/taskbadger/internal/api/action_endpoints/__init__.py
+-rw-r--r--   0        0        0     3318 2023-04-03 15:10:27.351088 taskbadger-0.4.0/taskbadger/internal/api/action_endpoints/action_cancel.py
+-rw-r--r--   0        0        0     5393 2023-04-03 15:10:27.363091 taskbadger-0.4.0/taskbadger/internal/api/action_endpoints/action_create.py
+-rw-r--r--   0        0        0     5005 2023-04-03 15:10:27.371092 taskbadger-0.4.0/taskbadger/internal/api/action_endpoints/action_get.py
+-rw-r--r--   0        0        0     5097 2023-04-03 15:10:27.359090 taskbadger-0.4.0/taskbadger/internal/api/action_endpoints/action_list.py
+-rw-r--r--   0        0        0     5676 2023-04-03 15:10:27.439107 taskbadger-0.4.0/taskbadger/internal/api/action_endpoints/action_partial_update.py
+-rw-r--r--   0        0        0     5556 2023-04-03 15:10:27.399098 taskbadger-0.4.0/taskbadger/internal/api/action_endpoints/action_update.py
+-rw-r--r--   0        0        0        0 2023-04-03 15:10:26.066805 taskbadger-0.4.0/taskbadger/internal/api/task_endpoints/__init__.py
+-rw-r--r--   0        0        0     3123 2023-04-03 15:10:27.339085 taskbadger-0.4.0/taskbadger/internal/api/task_endpoints/task_cancel.py
+-rw-r--r--   0        0        0     5770 2023-04-04 19:37:59.419308 taskbadger-0.4.0/taskbadger/internal/api/task_endpoints/task_create.py
+-rw-r--r--   0        0        0     4662 2023-04-03 15:10:27.543130 taskbadger-0.4.0/taskbadger/internal/api/task_endpoints/task_get.py
+-rw-r--r--   0        0        0     5872 2023-04-03 15:10:27.615146 taskbadger-0.4.0/taskbadger/internal/api/task_endpoints/task_list.py
+-rw-r--r--   0        0        0     5359 2023-04-03 15:10:27.619147 taskbadger-0.4.0/taskbadger/internal/api/task_endpoints/task_partial_update.py
+-rw-r--r--   0        0        0     5167 2023-04-03 15:10:27.567135 taskbadger-0.4.0/taskbadger/internal/api/task_endpoints/task_update.py
+-rw-r--r--   0        0        0     2673 2023-04-03 15:10:27.495119 taskbadger-0.4.0/taskbadger/internal/client.py
+-rw-r--r--   0        0        0      282 2023-04-03 15:10:27.463112 taskbadger-0.4.0/taskbadger/internal/errors.py
+-rw-r--r--   0        0        0     1022 2023-04-03 15:10:26.038798 taskbadger-0.4.0/taskbadger/internal/models/__init__.py
+-rw-r--r--   0        0        0     3234 2023-04-03 15:10:27.599142 taskbadger-0.4.0/taskbadger/internal/models/action.py
+-rw-r--r--   0        0        0     1152 2023-04-03 15:10:27.563134 taskbadger-0.4.0/taskbadger/internal/models/action_config.py
+-rw-r--r--   0        0        0     2405 2023-04-03 15:10:27.615146 taskbadger-0.4.0/taskbadger/internal/models/action_request.py
+-rw-r--r--   0        0        0     1190 2023-04-03 15:10:27.607144 taskbadger-0.4.0/taskbadger/internal/models/action_request_config.py
+-rw-r--r--   0        0        0     2590 2023-04-03 15:10:27.691162 taskbadger-0.4.0/taskbadger/internal/models/paginated_task_list.py
+-rw-r--r--   0        0        0     2638 2023-04-03 15:10:27.719169 taskbadger-0.4.0/taskbadger/internal/models/patched_action_request.py
+-rw-r--r--   0        0        0     1228 2023-04-03 15:10:27.647153 taskbadger-0.4.0/taskbadger/internal/models/patched_action_request_config.py
+-rw-r--r--   0        0        0     6107 2023-04-04 19:37:59.419308 taskbadger-0.4.0/taskbadger/internal/models/patched_task_request.py
+-rw-r--r--   0        0        0     1222 2023-04-03 15:10:27.675159 taskbadger-0.4.0/taskbadger/internal/models/patched_task_request_data.py
+-rw-r--r--   0        0        0      339 2023-04-04 19:37:59.419308 taskbadger-0.4.0/taskbadger/internal/models/status_enum.py
+-rw-r--r--   0        0        0     7435 2023-04-04 19:37:59.419308 taskbadger-0.4.0/taskbadger/internal/models/task.py
+-rw-r--r--   0        0        0     1146 2023-04-03 15:10:27.683161 taskbadger-0.4.0/taskbadger/internal/models/task_data.py
+-rw-r--r--   0        0        0     5965 2023-04-04 19:37:59.419308 taskbadger-0.4.0/taskbadger/internal/models/task_request.py
+-rw-r--r--   0        0        0     1184 2023-04-03 15:10:27.723169 taskbadger-0.4.0/taskbadger/internal/models/task_request_data.py
+-rw-r--r--   0        0        0       26 2023-05-24 06:53:11.963809 taskbadger-0.4.0/taskbadger/internal/py.typed
+-rw-r--r--   0        0        0      974 2023-04-03 15:10:27.723169 taskbadger-0.4.0/taskbadger/internal/types.py
+-rw-r--r--   0        0        0    10426 2023-05-24 06:53:11.963809 taskbadger-0.4.0/taskbadger/sdk.py
+-rw-r--r--   0        0        0     2880 1970-01-01 00:00:00.000000 taskbadger-0.4.0/setup.py
+-rw-r--r--   0        0        0     3190 1970-01-01 00:00:00.000000 taskbadger-0.4.0/PKG-INFO
```

### Comparing `taskbadger-0.3.2/LICENSE` & `taskbadger-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `taskbadger-0.3.2/README.md` & `taskbadger-0.4.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -85,8 +85,7 @@
 The CLI `run` command executes your command whilst creating and updating a Task Badger task.
 
 ```shell
 $ taskbadger run "demo task" --action "error email to:me@test.com" -- path/to/script.sh
 
 Task created: https://taskbadger.net/public/tasks/xyz/
 ```
-
```

### Comparing `taskbadger-0.3.2/pyproject.toml` & `taskbadger-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "taskbadger"
-version = "0.3.2"
+version = "0.4.0"
 description = "The official Python SDK for Task Badger"
 license = "Apache-2.0"
 
 authors = []
 
 readme = "README.md"
 packages = [
```

### Comparing `taskbadger-0.3.2/taskbadger/cli.py` & `taskbadger-0.4.0/taskbadger/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 from datetime import datetime
 from typing import Optional, Tuple
 
 import typer
 from rich import print
 from rich.console import Console
 
-from taskbadger import Action, StatusEnum, Task, integrations, __version__
+from taskbadger import Action, StatusEnum, Task, __version__, integrations
 from taskbadger.config import get_config, write_config
 from taskbadger.exceptions import ConfigurationError
 
 app = typer.Typer(
     rich_markup_mode="rich",
-    context_settings={"help_option_names": ["-h", "--help"]}
+    context_settings={"help_option_names": ["-h", "--help"]},
 )
 
 
 err_console = Console(stderr=True)
 
 
 def version_callback(value: bool):
```

### Comparing `taskbadger-0.3.2/taskbadger/config.py` & `taskbadger-0.4.0/taskbadger/config.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.3.2/taskbadger/integrations.py` & `taskbadger-0.4.0/taskbadger/integrations.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.3.2/taskbadger/internal/api/action_endpoints/action_cancel.py` & `taskbadger-0.4.0/taskbadger/internal/api/action_endpoints/action_cancel.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.3.2/taskbadger/internal/api/action_endpoints/action_create.py` & `taskbadger-0.4.0/taskbadger/internal/api/action_endpoints/action_create.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.3.2/taskbadger/internal/api/action_endpoints/action_get.py` & `taskbadger-0.4.0/taskbadger/internal/api/action_endpoints/action_get.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.3.2/taskbadger/internal/api/action_endpoints/action_list.py` & `taskbadger-0.4.0/taskbadger/internal/api/action_endpoints/action_list.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.3.2/taskbadger/internal/api/action_endpoints/action_partial_update.py` & `taskbadger-0.4.0/taskbadger/internal/api/action_endpoints/action_partial_update.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.3.2/taskbadger/internal/api/action_endpoints/action_update.py` & `taskbadger-0.4.0/taskbadger/internal/api/action_endpoints/action_update.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.3.2/taskbadger/internal/api/task_endpoints/task_cancel.py` & `taskbadger-0.4.0/taskbadger/internal/api/task_endpoints/task_cancel.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.3.2/taskbadger/internal/api/task_endpoints/task_create.py` & `taskbadger-0.4.0/taskbadger/internal/api/task_endpoints/task_create.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.3.2/taskbadger/internal/api/task_endpoints/task_get.py` & `taskbadger-0.4.0/taskbadger/internal/api/task_endpoints/task_get.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.3.2/taskbadger/internal/api/task_endpoints/task_list.py` & `taskbadger-0.4.0/taskbadger/internal/api/task_endpoints/task_list.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.3.2/taskbadger/internal/api/task_endpoints/task_partial_update.py` & `taskbadger-0.4.0/taskbadger/internal/api/task_endpoints/task_partial_update.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.3.2/taskbadger/internal/api/task_endpoints/task_update.py` & `taskbadger-0.4.0/taskbadger/internal/api/task_endpoints/task_update.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.3.2/taskbadger/internal/client.py` & `taskbadger-0.4.0/taskbadger/internal/client.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.3.2/taskbadger/internal/models/__init__.py` & `taskbadger-0.4.0/taskbadger/internal/models/__init__.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.3.2/taskbadger/internal/models/action.py` & `taskbadger-0.4.0/taskbadger/internal/models/action.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.3.2/taskbadger/internal/models/action_config.py` & `taskbadger-0.4.0/taskbadger/internal/models/action_config.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.3.2/taskbadger/internal/models/action_request.py` & `taskbadger-0.4.0/taskbadger/internal/models/action_request.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.3.2/taskbadger/internal/models/action_request_config.py` & `taskbadger-0.4.0/taskbadger/internal/models/action_request_config.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.3.2/taskbadger/internal/models/paginated_task_list.py` & `taskbadger-0.4.0/taskbadger/internal/models/paginated_task_list.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.3.2/taskbadger/internal/models/patched_action_request.py` & `taskbadger-0.4.0/taskbadger/internal/models/patched_action_request.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.3.2/taskbadger/internal/models/patched_action_request_config.py` & `taskbadger-0.4.0/taskbadger/internal/models/patched_action_request_config.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.3.2/taskbadger/internal/models/patched_task_request.py` & `taskbadger-0.4.0/taskbadger/internal/models/patched_task_request.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.3.2/taskbadger/internal/models/patched_task_request_data.py` & `taskbadger-0.4.0/taskbadger/internal/models/patched_task_request_data.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.3.2/taskbadger/internal/models/task.py` & `taskbadger-0.4.0/taskbadger/internal/models/task.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.3.2/taskbadger/internal/models/task_data.py` & `taskbadger-0.4.0/taskbadger/internal/models/task_data.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.3.2/taskbadger/internal/models/task_request.py` & `taskbadger-0.4.0/taskbadger/internal/models/task_request.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.3.2/taskbadger/internal/models/task_request_data.py` & `taskbadger-0.4.0/taskbadger/internal/models/task_request_data.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.3.2/taskbadger/internal/types.py` & `taskbadger-0.4.0/taskbadger/internal/types.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.3.2/taskbadger/sdk.py` & `taskbadger-0.4.0/taskbadger/sdk.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,20 +30,20 @@
     _init(_TB_HOST, organization_slug, project_slug, token)
 
 
 def _init(host: str = None, organization_slug: str = None, project_slug: str = None, token: str = None):
     host = host or os.environ.get("TASKBADGER_HOST", "https://taskbadger.net")
     organization_slug = organization_slug or os.environ.get("TASKBADGER_ORG")
     project_slug = project_slug or os.environ.get("TASKBADGER_PROJECT")
-    token = token or os.environ.get("TASKBADGER_TOKEN")
+    token = token or os.environ.get("TASKBADGER_API_KEY")
 
     if host and organization_slug and project_slug and token:
         client = AuthenticatedClient(host, token)
         settings = Settings(client, organization_slug, project_slug)
-        _local.set(settings)
+        Mug.current.bind(settings)
     else:
         raise ConfigurationError(
             host=host,
             organization_slug=organization_slug,
             project_slug=project_slug,
             token=token,
         )
@@ -157,15 +157,15 @@
     kwargs = _make_args(id=task_id, json_body=body)
     response = task_partial_update.sync_detailed(**kwargs)
     _check_response(response)
     return Task(response.parsed)
 
 
 def _make_args(**kwargs):
-    settings = _local.get()
+    settings = Mug.current.settings
     ret_args = dataclasses.asdict(settings)
     ret_args.update(kwargs)
     return ret_args
 
 
 def _get_settings():
     return _local.get()
@@ -182,14 +182,42 @@
 @dataclasses.dataclass
 class Settings:
     client: AuthenticatedClient
     organization_slug: str
     project_slug: str
 
 
+class MugMeta(type):
+    @property
+    def current(cls):
+        mug = _local.get(None)
+        if mug is None:
+            mug = Mug(GLOBAL_MUG)
+            _local.set(mug)
+        return mug
+
+
+class Mug(metaclass=MugMeta):
+    def __init__(self, settings_or_mug=None):
+        if isinstance(settings_or_mug, Mug):
+            self.settings = settings_or_mug.settings
+        else:
+            self.settings = settings_or_mug
+
+    def bind(self, settings):
+        self.settings = settings
+
+    def is_configured(self):
+        return self.settings is not None
+
+
+GLOBAL_MUG = Mug()
+_local.set(GLOBAL_MUG)
+
+
 class Task:
     """The Task class provides a convenient Python API to interact
     with Task Badger tasks.
     """
 
     @classmethod
     def get(cls, task_id: str) -> "Task":
```

### Comparing `taskbadger-0.3.2/setup.py` & `taskbadger-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,17 +23,17 @@
 {':python_version < "3.8"': ['importlib-metadata>=1.0,<2.0']}
 
 entry_points = \
 {'console_scripts': ['taskbadger = taskbadger.cli:app']}
 
 setup_kwargs = {
     'name': 'taskbadger',
-    'version': '0.3.2',
+    'version': '0.4.0',
     'description': 'The official Python SDK for Task Badger',
-    'long_description': '# Task Badger Python Client\n\nThis is the official Python SDK for [Task Badger](https://taskbadger.net/).\n\nFor full documentation go to https://docs.taskbadger.net/python/.\n\n---\n\n## Getting Started\n\n### Install\n\n```bash\npip install --upgrade taskbadger\n```\n\n### Client Usage\n\n#### Configuration\n\n```python\nimport taskbadger\n\ntaskbadger.init(\n    organization_slug="my-org",\n    project_slug="my-project",\n    token="***"\n)\n```\n\n#### API Example\n\n```python\nfrom taskbadger import Task, Action, EmailIntegration\n\n# create a new task with custom data and an action definition\ntask = Task.create(\n    "task name",\n    data={\n        "custom": "data"\n    },\n    actions=[\n        Action(\n            "*/10%,success,error",\n            integration=EmailIntegration(to="me@example.com")\n        )\n    ]\n)\n\n# update the task status to \'processing\' and set the value to 0\ntask.started()\ntry:\n   for i in range(100):\n      do_something(i)\n      if i!= 0 and i % 10 == 0:\n         # update the progress of the task\n         task.update_progress(i)\nexcept Exception as e:\n    # record task errors\n    task.error(data={\n        "error": str(e)\n    })\n    raise\n\n# record task success\ntask.success()\n```\n\n### CLI USage\n\n#### Configuration\n\n```shell\n$ taskbadger configure\n\nOrganization slug: my-org\nProject slug: project-x\nAPI Key: XYZ.ABC\n\nConfig written to ~/.config/taskbadger/config\n```\n\n#### Usage Examples\n\nThe CLI `run` command executes your command whilst creating and updating a Task Badger task.\n\n```shell\n$ taskbadger run "demo task" --action "error email to:me@test.com" -- path/to/script.sh\n\nTask created: https://taskbadger.net/public/tasks/xyz/\n```\n\n',
+    'long_description': '# Task Badger Python Client\n\nThis is the official Python SDK for [Task Badger](https://taskbadger.net/).\n\nFor full documentation go to https://docs.taskbadger.net/python/.\n\n---\n\n## Getting Started\n\n### Install\n\n```bash\npip install --upgrade taskbadger\n```\n\n### Client Usage\n\n#### Configuration\n\n```python\nimport taskbadger\n\ntaskbadger.init(\n    organization_slug="my-org",\n    project_slug="my-project",\n    token="***"\n)\n```\n\n#### API Example\n\n```python\nfrom taskbadger import Task, Action, EmailIntegration\n\n# create a new task with custom data and an action definition\ntask = Task.create(\n    "task name",\n    data={\n        "custom": "data"\n    },\n    actions=[\n        Action(\n            "*/10%,success,error",\n            integration=EmailIntegration(to="me@example.com")\n        )\n    ]\n)\n\n# update the task status to \'processing\' and set the value to 0\ntask.started()\ntry:\n   for i in range(100):\n      do_something(i)\n      if i!= 0 and i % 10 == 0:\n         # update the progress of the task\n         task.update_progress(i)\nexcept Exception as e:\n    # record task errors\n    task.error(data={\n        "error": str(e)\n    })\n    raise\n\n# record task success\ntask.success()\n```\n\n### CLI USage\n\n#### Configuration\n\n```shell\n$ taskbadger configure\n\nOrganization slug: my-org\nProject slug: project-x\nAPI Key: XYZ.ABC\n\nConfig written to ~/.config/taskbadger/config\n```\n\n#### Usage Examples\n\nThe CLI `run` command executes your command whilst creating and updating a Task Badger task.\n\n```shell\n$ taskbadger run "demo task" --action "error email to:me@test.com" -- path/to/script.sh\n\nTask created: https://taskbadger.net/public/tasks/xyz/\n```\n',
     'author': 'None',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://taskbadger.net/',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `taskbadger-0.3.2/PKG-INFO` & `taskbadger-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskbadger
-Version: 0.3.2
+Version: 0.4.0
 Summary: The official Python SDK for Task Badger
 Home-page: https://taskbadger.net/
 License: Apache-2.0
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -121,8 +121,7 @@
 
 ```shell
 $ taskbadger run "demo task" --action "error email to:me@test.com" -- path/to/script.sh
 
 Task created: https://taskbadger.net/public/tasks/xyz/
 ```
 
-
```

