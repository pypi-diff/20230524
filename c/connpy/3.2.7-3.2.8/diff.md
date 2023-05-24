# Comparing `tmp/connpy-3.2.7.tar.gz` & `tmp/connpy-3.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connpy-3.2.7.tar", last modified: Tue May 23 19:16:09 2023, max compression
+gzip compressed data, was "connpy-3.2.8.tar", last modified: Wed May 24 21:15:10 2023, max compression
```

## Comparing `connpy-3.2.7.tar` & `connpy-3.2.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:16:09.755095 connpy-3.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-23 19:15:57.000000 connpy-3.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-05-23 19:16:09.755095 connpy-3.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-05-23 19:15:57.000000 connpy-3.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:16:09.755095 connpy-3.2.7/connpy/
--rw-r--r--   0 runner    (1001) docker     (123)     8384 2023-05-23 19:15:57.000000 connpy-3.2.7/connpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-23 19:15:57.000000 connpy-3.2.7/connpy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-23 19:15:57.000000 connpy-3.2.7/connpy/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22109 2023-05-23 19:15:57.000000 connpy-3.2.7/connpy/ai.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5102 2023-05-23 19:15:57.000000 connpy-3.2.7/connpy/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-05-23 19:15:57.000000 connpy-3.2.7/connpy/completion.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15540 2023-05-23 19:15:57.000000 connpy-3.2.7/connpy/configfile.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    50300 2023-05-23 19:15:57.000000 connpy-3.2.7/connpy/connapp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    28719 2023-05-23 19:15:57.000000 connpy-3.2.7/connpy/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:16:09.755095 connpy-3.2.7/connpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-05-23 19:16:09.000000 connpy-3.2.7/connpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-23 19:16:09.000000 connpy-3.2.7/connpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 19:16:09.000000 connpy-3.2.7/connpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-23 19:16:09.000000 connpy-3.2.7/connpy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-23 19:16:09.000000 connpy-3.2.7/connpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-23 19:16:09.000000 connpy-3.2.7/connpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-23 19:16:09.755095 connpy-3.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-23 19:15:57.000000 connpy-3.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:15:10.386407 connpy-3.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-24 21:14:54.000000 connpy-3.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-05-24 21:15:10.386407 connpy-3.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-05-24 21:14:54.000000 connpy-3.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:15:10.386407 connpy-3.2.8/connpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     8384 2023-05-24 21:14:54.000000 connpy-3.2.8/connpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-24 21:14:54.000000 connpy-3.2.8/connpy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-24 21:14:54.000000 connpy-3.2.8/connpy/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22046 2023-05-24 21:14:54.000000 connpy-3.2.8/connpy/ai.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5102 2023-05-24 21:14:54.000000 connpy-3.2.8/connpy/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-05-24 21:14:54.000000 connpy-3.2.8/connpy/completion.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15540 2023-05-24 21:14:54.000000 connpy-3.2.8/connpy/configfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    50300 2023-05-24 21:14:54.000000 connpy-3.2.8/connpy/connapp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28719 2023-05-24 21:14:54.000000 connpy-3.2.8/connpy/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:15:10.386407 connpy-3.2.8/connpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-05-24 21:15:10.000000 connpy-3.2.8/connpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-24 21:15:10.000000 connpy-3.2.8/connpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 21:15:10.000000 connpy-3.2.8/connpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-24 21:15:10.000000 connpy-3.2.8/connpy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-24 21:15:10.000000 connpy-3.2.8/connpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-24 21:15:10.000000 connpy-3.2.8/connpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-24 21:15:10.386407 connpy-3.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-24 21:14:54.000000 connpy-3.2.8/setup.py
```

### Comparing `connpy-3.2.7/LICENSE` & `connpy-3.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `connpy-3.2.7/PKG-INFO` & `connpy-3.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connpy
-Version: 3.2.7
+Version: 3.2.8
 Summary: Connpy is a SSH/Telnet connection manager and automation module
 Home-page: https://github.com/fluzzi/connpy
 Author: Federico Luzzi
 Author-email: fluzzi@gmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/fluzzi/connpy/issues
 Project-URL: Documentation, https://fluzzi.github.io/connpy/
```

### Comparing `connpy-3.2.7/README.md` & `connpy-3.2.8/README.md`

 * *Files identical despite different names*

### Comparing `connpy-3.2.7/connpy/__init__.py` & `connpy-3.2.8/connpy/__init__.py`

 * *Files identical despite different names*

### Comparing `connpy-3.2.7/connpy/ai.py` & `connpy-3.2.8/connpy/ai.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,15 @@
     def _retry_function(self, function, max_retries, backoff_num, *args):
         #Retry openai requests
         retries = 0
         while retries < max_retries:
             try:
                 myfunction = function(*args)
                 break
-            except (openai.error.APIConnectionError, openai.error.RateLimitError):
+            except:
                 wait_time = backoff_num * (2 ** retries)
                 time.sleep(wait_time)
                 retries += 1
                 continue
         if retries == max_retries:
             myfunction = False
         return myfunction
```

### Comparing `connpy-3.2.7/connpy/api.py` & `connpy-3.2.8/connpy/api.py`

 * *Files identical despite different names*

### Comparing `connpy-3.2.7/connpy/completion.py` & `connpy-3.2.8/connpy/completion.py`

 * *Files identical despite different names*

### Comparing `connpy-3.2.7/connpy/configfile.py` & `connpy-3.2.8/connpy/configfile.py`

 * *Files identical despite different names*

### Comparing `connpy-3.2.7/connpy/connapp.py` & `connpy-3.2.8/connpy/connapp.py`

 * *Files identical despite different names*

### Comparing `connpy-3.2.7/connpy/core.py` & `connpy-3.2.8/connpy/core.py`

 * *Files identical despite different names*

### Comparing `connpy-3.2.7/connpy.egg-info/PKG-INFO` & `connpy-3.2.8/connpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connpy
-Version: 3.2.7
+Version: 3.2.8
 Summary: Connpy is a SSH/Telnet connection manager and automation module
 Home-page: https://github.com/fluzzi/connpy
 Author: Federico Luzzi
 Author-email: fluzzi@gmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/fluzzi/connpy/issues
 Project-URL: Documentation, https://fluzzi.github.io/connpy/
```

### Comparing `connpy-3.2.7/setup.cfg` & `connpy-3.2.8/setup.cfg`

 * *Files identical despite different names*

