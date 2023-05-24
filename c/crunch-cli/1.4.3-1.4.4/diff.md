# Comparing `tmp/crunch-cli-1.4.3.tar.gz` & `tmp/crunch-cli-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crunch-cli-1.4.3.tar", last modified: Fri May 19 13:53:42 2023, max compression
+gzip compressed data, was "crunch-cli-1.4.4.tar", last modified: Wed May 24 15:16:45 2023, max compression
```

## Comparing `crunch-cli-1.4.3.tar` & `crunch-cli-1.4.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:53:42.661653 crunch-cli-1.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-19 13:53:42.661653 crunch-cli-1.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-19 13:53:37.000000 crunch-cli-1.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:53:42.661653 crunch-cli-1.4.3/crunch/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-19 13:53:37.000000 crunch-cli-1.4.3/crunch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-19 13:53:37.000000 crunch-cli-1.4.3/crunch/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-19 13:53:37.000000 crunch-cli-1.4.3/crunch/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:53:42.661653 crunch-cli-1.4.3/crunch/command/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-19 13:53:37.000000 crunch-cli-1.4.3/crunch/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-19 13:53:37.000000 crunch-cli-1.4.3/crunch/command/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-05-19 13:53:37.000000 crunch-cli-1.4.3/crunch/command/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-05-19 13:53:37.000000 crunch-cli-1.4.3/crunch/command/push.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-19 13:53:37.000000 crunch-cli-1.4.3/crunch/command/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-19 13:53:37.000000 crunch-cli-1.4.3/crunch/command/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-19 13:53:37.000000 crunch-cli-1.4.3/crunch/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:53:42.661653 crunch-cli-1.4.3/crunch/demo-project/
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-05-19 13:53:37.000000 crunch-cli-1.4.3/crunch/demo-project/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-19 13:53:37.000000 crunch-cli-1.4.3/crunch/demo-project/files.json
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-19 13:53:37.000000 crunch-cli-1.4.3/crunch/demo-project/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-19 13:53:37.000000 crunch-cli-1.4.3/crunch/demo-project/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-19 13:53:37.000000 crunch-cli-1.4.3/crunch/ensure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-05-19 13:53:37.000000 crunch-cli-1.4.3/crunch/inline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-05-19 13:53:37.000000 crunch-cli-1.4.3/crunch/library.py
--rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-05-19 13:53:37.000000 crunch-cli-1.4.3/crunch/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-05-19 13:53:37.000000 crunch-cli-1.4.3/crunch/tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-05-19 13:53:37.000000 crunch-cli-1.4.3/crunch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:53:42.661653 crunch-cli-1.4.3/crunch_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-19 13:53:42.000000 crunch-cli-1.4.3/crunch_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-19 13:53:42.000000 crunch-cli-1.4.3/crunch_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 13:53:42.000000 crunch-cli-1.4.3/crunch_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-19 13:53:42.000000 crunch-cli-1.4.3/crunch_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 13:53:42.000000 crunch-cli-1.4.3/crunch_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-19 13:53:42.000000 crunch-cli-1.4.3/crunch_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-19 13:53:42.000000 crunch-cli-1.4.3/crunch_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 13:53:42.661653 crunch-cli-1.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-19 13:53:37.000000 crunch-cli-1.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:16:45.948294 crunch-cli-1.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-24 15:16:45.948294 crunch-cli-1.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-24 15:16:40.000000 crunch-cli-1.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:16:45.940294 crunch-cli-1.4.4/crunch/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-24 15:16:40.000000 crunch-cli-1.4.4/crunch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-24 15:16:40.000000 crunch-cli-1.4.4/crunch/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-24 15:16:40.000000 crunch-cli-1.4.4/crunch/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:16:45.944294 crunch-cli-1.4.4/crunch/command/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-24 15:16:40.000000 crunch-cli-1.4.4/crunch/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-24 15:16:40.000000 crunch-cli-1.4.4/crunch/command/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-05-24 15:16:40.000000 crunch-cli-1.4.4/crunch/command/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-05-24 15:16:40.000000 crunch-cli-1.4.4/crunch/command/push.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-24 15:16:40.000000 crunch-cli-1.4.4/crunch/command/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-24 15:16:40.000000 crunch-cli-1.4.4/crunch/command/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-24 15:16:40.000000 crunch-cli-1.4.4/crunch/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:16:45.944294 crunch-cli-1.4.4/crunch/demo-project/
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-05-24 15:16:40.000000 crunch-cli-1.4.4/crunch/demo-project/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-24 15:16:40.000000 crunch-cli-1.4.4/crunch/demo-project/files.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-24 15:16:40.000000 crunch-cli-1.4.4/crunch/demo-project/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-24 15:16:40.000000 crunch-cli-1.4.4/crunch/demo-project/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-24 15:16:40.000000 crunch-cli-1.4.4/crunch/ensure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-05-24 15:16:40.000000 crunch-cli-1.4.4/crunch/inline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-05-24 15:16:40.000000 crunch-cli-1.4.4/crunch/library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-05-24 15:16:40.000000 crunch-cli-1.4.4/crunch/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-05-24 15:16:40.000000 crunch-cli-1.4.4/crunch/tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-05-24 15:16:40.000000 crunch-cli-1.4.4/crunch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:16:45.948294 crunch-cli-1.4.4/crunch_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-24 15:16:45.000000 crunch-cli-1.4.4/crunch_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-24 15:16:45.000000 crunch-cli-1.4.4/crunch_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:16:45.000000 crunch-cli-1.4.4/crunch_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-24 15:16:45.000000 crunch-cli-1.4.4/crunch_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:16:45.000000 crunch-cli-1.4.4/crunch_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-24 15:16:45.000000 crunch-cli-1.4.4/crunch_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-24 15:16:45.000000 crunch-cli-1.4.4/crunch_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 15:16:45.948294 crunch-cli-1.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-24 15:16:40.000000 crunch-cli-1.4.4/setup.py
```

### Comparing `crunch-cli-1.4.3/crunch/command/convert.py` & `crunch-cli-1.4.4/crunch/command/convert.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.4.3/crunch/command/download.py` & `crunch-cli-1.4.4/crunch/command/download.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.4.3/crunch/command/push.py` & `crunch-cli-1.4.4/crunch/command/push.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,19 +69,18 @@
     try:
         with tempfile.NamedTemporaryFile(prefix="submission-", suffix=".tar", dir=constants.DOT_CRUNCHDAO_DIRECTORY) as tmp:
             with tarfile.open(fileobj=tmp, mode="w") as tar:
                 for file in _list_code_files(model_directory_path):
                     print(f"compress {file}")
                     tar.add(file)
 
-            fd = open(tmp.name, "rb")
-            fds.append(fd)
+            tmp.seek(0)
 
             files = [
-                ("codeFile", ('code.tar', fd, "application/x-tar"))
+                ("codeFile", ('code.tar', tmp, "application/x-tar"))
             ]
 
             for path, name in _list_model_files(model_directory_path):
                 print(f"model {name}")
 
                 fd = open(path, "rb")
                 fds.append(fd)
```

### Comparing `crunch-cli-1.4.3/crunch/command/setup.py` & `crunch-cli-1.4.4/crunch/command/setup.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.4.3/crunch/command/test.py` & `crunch-cli-1.4.4/crunch/command/test.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.4.3/crunch/constants.py` & `crunch-cli-1.4.4/crunch/constants.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.4.3/crunch/demo-project/.gitignore` & `crunch-cli-1.4.4/crunch/demo-project/.gitignore`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.4.3/crunch/demo-project/main.py` & `crunch-cli-1.4.4/crunch/demo-project/main.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.4.3/crunch/ensure.py` & `crunch-cli-1.4.4/crunch/ensure.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.4.3/crunch/inline.py` & `crunch-cli-1.4.4/crunch/inline.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.4.3/crunch/library.py` & `crunch-cli-1.4.4/crunch/library.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.4.3/crunch/main.py` & `crunch-cli-1.4.4/crunch/main.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.4.3/crunch/tester.py` & `crunch-cli-1.4.4/crunch/tester.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.4.3/crunch/utils.py` & `crunch-cli-1.4.4/crunch/utils.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.4.3/crunch_cli.egg-info/SOURCES.txt` & `crunch-cli-1.4.4/crunch_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.4.3/setup.py` & `crunch-cli-1.4.4/setup.py`

 * *Files identical despite different names*

