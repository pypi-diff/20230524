# Comparing `tmp/piwaterflow-0.5.4.tar.gz` & `tmp/piwaterflow-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piwaterflow-0.5.4.tar", last modified: Mon May 22 06:18:58 2023, max compression
+gzip compressed data, was "piwaterflow-0.5.6.tar", last modified: Wed May 24 07:11:35 2023, max compression
```

## Comparing `piwaterflow-0.5.4.tar` & `piwaterflow-0.5.6.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:18:58.631210 piwaterflow-0.5.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-22 06:18:58.631210 piwaterflow-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-22 06:18:43.000000 piwaterflow-0.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:18:58.627210 piwaterflow-0.5.4/piwaterflow/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-22 06:18:43.000000 piwaterflow-0.5.4/piwaterflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-22 06:18:43.000000 piwaterflow-0.5.4/piwaterflow/config-template.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-22 06:18:43.000000 piwaterflow-0.5.4/piwaterflow/config_waterflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:18:58.631210 piwaterflow-0.5.4/piwaterflow/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:18:43.000000 piwaterflow-0.5.4/piwaterflow/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-22 06:18:43.000000 piwaterflow-0.5.4/piwaterflow/tests/test_000.py
--rw-r--r--   0 runner    (1001) docker     (123)    21323 2023-05-22 06:18:43.000000 piwaterflow-0.5.4/piwaterflow/waterflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:18:58.631210 piwaterflow-0.5.4/piwaterflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-22 06:18:58.000000 piwaterflow-0.5.4/piwaterflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-22 06:18:58.000000 piwaterflow-0.5.4/piwaterflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 06:18:58.000000 piwaterflow-0.5.4/piwaterflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-22 06:18:58.000000 piwaterflow-0.5.4/piwaterflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-22 06:18:58.000000 piwaterflow-0.5.4/piwaterflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 06:18:58.631210 piwaterflow-0.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-22 06:18:43.000000 piwaterflow-0.5.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:18:58.631210 piwaterflow-0.5.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:18:43.000000 piwaterflow-0.5.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-22 06:18:43.000000 piwaterflow-0.5.4/tests/test_000_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-05-22 06:18:43.000000 piwaterflow-0.5.4/tests/test_001_forward.py
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-22 06:18:43.000000 piwaterflow-0.5.4/tests/test_002_reverse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-22 06:18:43.000000 piwaterflow-0.5.4/tests/test_003_lock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:11:35.532252 piwaterflow-0.5.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-24 07:11:35.532252 piwaterflow-0.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-24 07:11:23.000000 piwaterflow-0.5.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:11:35.528252 piwaterflow-0.5.6/piwaterflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-24 07:11:23.000000 piwaterflow-0.5.6/piwaterflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-24 07:11:23.000000 piwaterflow-0.5.6/piwaterflow/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-24 07:11:23.000000 piwaterflow-0.5.6/piwaterflow/config-template.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-24 07:11:23.000000 piwaterflow-0.5.6/piwaterflow/config_waterflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:11:35.532252 piwaterflow-0.5.6/piwaterflow/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 07:11:23.000000 piwaterflow-0.5.6/piwaterflow/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-24 07:11:23.000000 piwaterflow-0.5.6/piwaterflow/tests/test_000.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21323 2023-05-24 07:11:23.000000 piwaterflow-0.5.6/piwaterflow/waterflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:11:35.528252 piwaterflow-0.5.6/piwaterflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-24 07:11:35.000000 piwaterflow-0.5.6/piwaterflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-24 07:11:35.000000 piwaterflow-0.5.6/piwaterflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 07:11:35.000000 piwaterflow-0.5.6/piwaterflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-24 07:11:35.000000 piwaterflow-0.5.6/piwaterflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-24 07:11:35.000000 piwaterflow-0.5.6/piwaterflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 07:11:35.532252 piwaterflow-0.5.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-24 07:11:23.000000 piwaterflow-0.5.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:11:35.532252 piwaterflow-0.5.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 07:11:23.000000 piwaterflow-0.5.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-24 07:11:23.000000 piwaterflow-0.5.6/tests/test_000_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-05-24 07:11:23.000000 piwaterflow-0.5.6/tests/test_001_forward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-24 07:11:23.000000 piwaterflow-0.5.6/tests/test_002_reverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-24 07:11:23.000000 piwaterflow-0.5.6/tests/test_003_lock.py
```

### Comparing `piwaterflow-0.5.4/PKG-INFO` & `piwaterflow-0.5.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piwaterflow
-Version: 0.5.4
+Version: 0.5.6
 Summary: Raspberry Pi Waterflow resilient system
 Home-page: https://github.com/Phornee/piwaterflow
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Description: # PiWaterflow
         This is a resilient watering system, executed in a Raspberry Pi to control irrigation valves using relays.
```

### Comparing `piwaterflow-0.5.4/README.md` & `piwaterflow-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `piwaterflow-0.5.4/piwaterflow/config-template.yml` & `piwaterflow-0.5.6/piwaterflow/config-template.yml`

 * *Files identical despite different names*

### Comparing `piwaterflow-0.5.4/piwaterflow/config_waterflow.py` & `piwaterflow-0.5.6/piwaterflow/config_waterflow.py`

 * *Files identical despite different names*

### Comparing `piwaterflow-0.5.4/piwaterflow/tests/test_000.py` & `piwaterflow-0.5.6/piwaterflow/tests/test_000.py`

 * *Files identical despite different names*

### Comparing `piwaterflow-0.5.4/piwaterflow/waterflow.py` & `piwaterflow-0.5.6/piwaterflow/waterflow.py`

 * *Files identical despite different names*

### Comparing `piwaterflow-0.5.4/piwaterflow.egg-info/PKG-INFO` & `piwaterflow-0.5.6/piwaterflow.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piwaterflow
-Version: 0.5.4
+Version: 0.5.6
 Summary: Raspberry Pi Waterflow resilient system
 Home-page: https://github.com/Phornee/piwaterflow
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Description: # PiWaterflow
         This is a resilient watering system, executed in a Raspberry Pi to control irrigation valves using relays.
```

### Comparing `piwaterflow-0.5.4/setup.py` & `piwaterflow-0.5.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="piwaterflow",
-    version="0.5.4",
+    version="0.5.6",
     author="Ismael Raya",
     author_email="phornee@gmail.com",
     description="Raspberry Pi Waterflow resilient system",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Phornee/piwaterflow",
     packages=setuptools.find_packages(),
```

### Comparing `piwaterflow-0.5.4/tests/test_000_loop.py` & `piwaterflow-0.5.6/tests/test_000_loop.py`

 * *Files identical despite different names*

### Comparing `piwaterflow-0.5.4/tests/test_001_forward.py` & `piwaterflow-0.5.6/tests/test_001_forward.py`

 * *Files identical despite different names*

### Comparing `piwaterflow-0.5.4/tests/test_002_reverse.py` & `piwaterflow-0.5.6/tests/test_002_reverse.py`

 * *Files identical despite different names*

### Comparing `piwaterflow-0.5.4/tests/test_003_lock.py` & `piwaterflow-0.5.6/tests/test_003_lock.py`

 * *Files identical despite different names*

