# Comparing `tmp/dart-tools-0.2.0.tar.gz` & `tmp/dart-tools-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dart-tools-0.2.0.tar", last modified: Sat May 13 07:21:37 2023, max compression
+gzip compressed data, was "dart-tools-0.3.0.tar", last modified: Tue May 23 22:12:46 2023, max compression
```

## Comparing `dart-tools-0.2.0.tar` & `dart-tools-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-05-13 07:21:37.184260 dart-tools-0.2.0/
--rw-r--r--   0 zack       (501) staff       (20)     1061 2023-02-28 02:56:19.000000 dart-tools-0.2.0/LICENSE
--rw-r--r--   0 zack       (501) staff       (20)     4358 2023-05-13 07:21:37.183916 dart-tools-0.2.0/PKG-INFO
--rw-r--r--   0 zack       (501) staff       (20)     1510 2023-04-03 00:03:57.000000 dart-tools-0.2.0/README.md
-drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-05-13 07:21:37.181131 dart-tools-0.2.0/dart/
--rw-r--r--   0 zack       (501) staff       (20)       64 2023-02-28 04:01:58.000000 dart-tools-0.2.0/dart/__init__.py
--rwxr-xr-x   0 zack       (501) staff       (20)    11703 2023-05-13 07:20:34.000000 dart-tools-0.2.0/dart/dart.py
--rw-r--r--   0 zack       (501) staff       (20)     1709 2023-02-28 02:57:20.000000 dart-tools-0.2.0/dart/order_manager.py
-drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-05-13 07:21:37.183406 dart-tools-0.2.0/dart_tools.egg-info/
--rw-r--r--   0 zack       (501) staff       (20)     4358 2023-05-13 07:21:37.000000 dart-tools-0.2.0/dart_tools.egg-info/PKG-INFO
--rw-r--r--   0 zack       (501) staff       (20)      290 2023-05-13 07:21:37.000000 dart-tools-0.2.0/dart_tools.egg-info/SOURCES.txt
--rw-r--r--   0 zack       (501) staff       (20)        1 2023-05-13 07:21:37.000000 dart-tools-0.2.0/dart_tools.egg-info/dependency_links.txt
--rw-r--r--   0 zack       (501) staff       (20)       34 2023-05-13 07:21:37.000000 dart-tools-0.2.0/dart_tools.egg-info/entry_points.txt
--rw-r--r--   0 zack       (501) staff       (20)       14 2023-05-13 07:21:37.000000 dart-tools-0.2.0/dart_tools.egg-info/requires.txt
--rw-r--r--   0 zack       (501) staff       (20)        5 2023-05-13 07:21:37.000000 dart-tools-0.2.0/dart_tools.egg-info/top_level.txt
--rw-r--r--   0 zack       (501) staff       (20)     1744 2023-05-13 07:20:34.000000 dart-tools-0.2.0/pyproject.toml
--rw-r--r--   0 zack       (501) staff       (20)       38 2023-05-13 07:21:37.184370 dart-tools-0.2.0/setup.cfg
+drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-05-23 22:12:46.047203 dart-tools-0.3.0/
+-rw-r--r--   0 zack       (501) staff       (20)     1061 2023-02-28 02:56:19.000000 dart-tools-0.3.0/LICENSE
+-rw-r--r--   0 zack       (501) staff       (20)     4358 2023-05-23 22:12:46.046810 dart-tools-0.3.0/PKG-INFO
+-rw-r--r--   0 zack       (501) staff       (20)     1510 2023-04-03 00:03:57.000000 dart-tools-0.3.0/README.md
+drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-05-23 22:12:46.042158 dart-tools-0.3.0/dart/
+-rw-r--r--   0 zack       (501) staff       (20)       64 2023-02-28 04:01:58.000000 dart-tools-0.3.0/dart/__init__.py
+-rwxr-xr-x   0 zack       (501) staff       (20)    11987 2023-05-23 22:10:51.000000 dart-tools-0.3.0/dart/dart.py
+-rw-r--r--   0 zack       (501) staff       (20)     1709 2023-02-28 02:57:20.000000 dart-tools-0.3.0/dart/order_manager.py
+drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-05-23 22:12:46.045940 dart-tools-0.3.0/dart_tools.egg-info/
+-rw-r--r--   0 zack       (501) staff       (20)     4358 2023-05-23 22:12:45.000000 dart-tools-0.3.0/dart_tools.egg-info/PKG-INFO
+-rw-r--r--   0 zack       (501) staff       (20)      290 2023-05-23 22:12:45.000000 dart-tools-0.3.0/dart_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 zack       (501) staff       (20)        1 2023-05-23 22:12:45.000000 dart-tools-0.3.0/dart_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 zack       (501) staff       (20)       34 2023-05-23 22:12:45.000000 dart-tools-0.3.0/dart_tools.egg-info/entry_points.txt
+-rw-r--r--   0 zack       (501) staff       (20)       14 2023-05-23 22:12:45.000000 dart-tools-0.3.0/dart_tools.egg-info/requires.txt
+-rw-r--r--   0 zack       (501) staff       (20)        5 2023-05-23 22:12:45.000000 dart-tools-0.3.0/dart_tools.egg-info/top_level.txt
+-rw-r--r--   0 zack       (501) staff       (20)     1744 2023-05-23 22:01:53.000000 dart-tools-0.3.0/pyproject.toml
+-rw-r--r--   0 zack       (501) staff       (20)       38 2023-05-23 22:12:46.047360 dart-tools-0.3.0/setup.cfg
```

### Comparing `dart-tools-0.2.0/LICENSE` & `dart-tools-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dart-tools-0.2.0/PKG-INFO` & `dart-tools-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dart-tools
-Version: 0.2.0
+Version: 0.3.0
 Summary: The Dart CLI and Python Library
 Author-email: Dart Software Team <software@itsdart.com>
 License: MIT License
         
         Copyright (c) 2023 Dart
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dart-tools Version: 0.2.0 Summary: The Dart CLI and
+Metadata-Version: 2.1 Name: dart-tools Version: 0.3.0 Summary: The Dart CLI and
 Python Library Author-email: Dart Software Team
 itsdart.com> License: MIT License Copyright (c) 2023 Dart Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `dart-tools-0.2.0/README.md` & `dart-tools-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `dart-tools-0.2.0/dart/dart.py` & `dart-tools-0.3.0/dart/dart.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,14 +75,18 @@
     return "".join(random.choices(_DUID_CHARS, k=12))
 
 
 def _run_cmd(cmd):
     return subprocess.check_output(cmd, shell=True).decode()
 
 
+def _get_task_url(host, duid):
+    return f"{host}/search?t={duid}"
+
+
 class _Config:
     def __init__(self):
         if os.path.isfile(_CONFIG_FPATH):
             with open(_CONFIG_FPATH, "r", encoding="UTF-8") as fin:
                 self._content = json.load(fin)
         self._content = {
             _CLIENT_DUID_KEY: _make_duid(),
@@ -281,89 +285,94 @@
     _Git.ensure_on_main_or_intended()
 
     config = _Config()
     session = _Session(config)
 
     user_bundle = _get_full_user_bundle(session)
 
-    user_email = user_bundle["user"]["email"]
+    user = user_bundle["user"]
+    user_duid = user["duid"]
     active_duid = next(
         e["duid"] for e in user_bundle["dartboards"] if e["kind"] == "Active"
     )
     unterm_status_duids = {
         e["duid"]
         for e in user_bundle["statuses"]
         if e["kind"] not in _COMPLETED_STATUS_KINDS
     }
     filtered_tasks = [
         e
         for e in user_bundle["tasks"]
         if not e["inTrash"]
         and e["dartboardDuid"] == active_duid
-        and user_email in e["assigneeEmails"]
+        and user_duid in e["assigneeDuids"]
         and e["statusDuid"] in unterm_status_duids
-        and e["drafterEmail"] is None
+        and e["drafterDuid"] is None
     ]
     filtered_tasks.sort(key=lambda e: e["order"])
 
     chosen_task = filtered_tasks[
         pick(
             [e["title"] for e in filtered_tasks],
             "Which of your active, unfinalized tasks are you beginning work on?",
             "→",
         )[1]
     ]
+
     response = session.post(_COPY_BRANCH_URL_FRAG, json={"duid": chosen_task["duid"]})
     _check_response_and_maybe_exit(response)
 
-    branch_name = _Git.make_task_name(user_email, chosen_task)
+    branch_name = _Git.make_task_name(user["email"], chosen_task)
     _Git.checkout_branch(branch_name)
 
+    print(
+        f"Started work on [{chosen_task['title']}]({_get_task_url(config.host, chosen_task['duid'])}) on branch {branch_name}"
+    )
     print("Done.")
 
 
 def create_task(title):
     config = _Config()
     session = _Session(config)
 
     user_bundle = _get_full_user_bundle(session)
 
-    user_email = user_bundle["user"]["email"]
+    user_duid = user_bundle["user"]["duid"]
     active_duid = next(
         e["duid"] for e in user_bundle["dartboards"] if e["kind"] == "Active"
     )
     first_order = min(
         e["order"] for e in user_bundle["tasks"] if e["dartboardDuid"] == active_duid
     )
     order = get_orders_between(None, first_order, 1)[0]
     status_duid = next(
         e["duid"]
         for e in user_bundle["statuses"]
         if e["kind"] == "Unstarted" and e["locked"]
     )
 
-    print("Creating task")
     task = {
         "duid": _make_duid(),
-        "drafterEmail": None,
+        "drafterDuid": None,
         "dartboardDuid": active_duid,
         "order": order,
         "title": title,
         "description": _DEFAULT_DESCRIPTION,
         "statusDuid": status_duid,
-        "assigneeEmails": [user_email],
-        "subscriberEmails": [user_email],
+        "assigneeDuids": [user_duid],
+        "subscriberDuids": [user_duid],
         "tagDuids": [],
         "priority": None,
         "size": None,
         "dueAt": None,
     }
     response = session.post(_CREATE_TASK_URL_FRAG, json={"item": task})
     _check_response_and_maybe_exit(response)
 
+    print(f"Created task [{task['title']}]({_get_task_url(config.host, task['duid'])})")
     print("Done.")
 
 
 def cli():
     if _VERSION_CMD in sys.argv:
         print_version()
         sys.exit(0)
```

### Comparing `dart-tools-0.2.0/dart/order_manager.py` & `dart-tools-0.3.0/dart/order_manager.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.2.0/dart_tools.egg-info/PKG-INFO` & `dart-tools-0.3.0/dart_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dart-tools
-Version: 0.2.0
+Version: 0.3.0
 Summary: The Dart CLI and Python Library
 Author-email: Dart Software Team <software@itsdart.com>
 License: MIT License
         
         Copyright (c) 2023 Dart
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dart-tools Version: 0.2.0 Summary: The Dart CLI and
+Metadata-Version: 2.1 Name: dart-tools Version: 0.3.0 Summary: The Dart CLI and
 Python Library Author-email: Dart Software Team
 itsdart.com> License: MIT License Copyright (c) 2023 Dart Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `dart-tools-0.2.0/pyproject.toml` & `dart-tools-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dart-tools"
-version = "0.2.0"
+version = "0.3.0"
 description = "The Dart CLI and Python Library"
 readme = "README.md"
 requires-python = ">=3.8"
 
 license = {file = "LICENSE"}
 keywords = ["dart", "cli", "projectmanagement", "taskmanagement"]
 authors = [
```

