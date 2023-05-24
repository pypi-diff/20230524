# Comparing `tmp/vocabmaster-0.1.5.tar.gz` & `tmp/vocabmaster-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vocabmaster-0.1.5.tar", last modified: Fri May  5 18:15:22 2023, max compression
+gzip compressed data, was "vocabmaster-0.1.6.tar", last modified: Wed May 24 20:40:35 2023, max compression
```

## Comparing `vocabmaster-0.1.5.tar` & `vocabmaster-0.1.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-05-05 18:15:22.743051 vocabmaster-0.1.5/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1079 2023-04-08 02:37:38.000000 vocabmaster-0.1.5/LICENSE
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     2698 2023-05-05 18:15:22.743051 vocabmaster-0.1.5/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     2565 2023-05-04 11:47:01.000000 vocabmaster-0.1.5/README.md
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-05-05 18:15:22.743051 vocabmaster-0.1.5/setup.cfg
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      578 2023-05-05 18:14:40.000000 vocabmaster-0.1.5/setup.py
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-05-05 18:15:22.743051 vocabmaster-0.1.5/vocabmaster/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-04-09 03:24:19.000000 vocabmaster-0.1.5/vocabmaster/__init__.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    18006 2023-05-04 13:07:42.000000 vocabmaster-0.1.5/vocabmaster/cli.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     4200 2023-04-16 12:02:38.000000 vocabmaster-0.1.5/vocabmaster/config_handler.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    10722 2023-05-05 18:12:19.000000 vocabmaster-0.1.5/vocabmaster/csv_handler.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     5646 2023-05-04 16:22:59.000000 vocabmaster-0.1.5/vocabmaster/gpt_integration.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     7264 2023-05-04 13:33:03.000000 vocabmaster-0.1.5/vocabmaster/utils.py
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-05-05 18:15:22.743051 vocabmaster-0.1.5/vocabmaster.egg-info/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     2698 2023-05-05 18:15:22.000000 vocabmaster-0.1.5/vocabmaster.egg-info/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      390 2023-05-05 18:15:22.000000 vocabmaster-0.1.5/vocabmaster.egg-info/SOURCES.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-05-05 18:15:22.000000 vocabmaster-0.1.5/vocabmaster.egg-info/dependency_links.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       60 2023-05-05 18:15:22.000000 vocabmaster-0.1.5/vocabmaster.egg-info/entry_points.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      277 2023-05-05 18:15:22.000000 vocabmaster-0.1.5/vocabmaster.egg-info/requires.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       12 2023-05-05 18:15:22.000000 vocabmaster-0.1.5/vocabmaster.egg-info/top_level.txt
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-05-24 20:40:35.909385 vocabmaster-0.1.6/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1079 2023-04-08 02:37:38.000000 vocabmaster-0.1.6/LICENSE
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     2698 2023-05-24 20:40:35.909385 vocabmaster-0.1.6/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     2565 2023-05-04 11:47:01.000000 vocabmaster-0.1.6/README.md
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-05-24 20:40:35.909385 vocabmaster-0.1.6/setup.cfg
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      578 2023-05-24 20:38:03.000000 vocabmaster-0.1.6/setup.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-05-24 20:40:35.899385 vocabmaster-0.1.6/vocabmaster/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-04-09 03:24:19.000000 vocabmaster-0.1.6/vocabmaster/__init__.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    18006 2023-05-04 13:07:42.000000 vocabmaster-0.1.6/vocabmaster/cli.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     4200 2023-04-16 12:02:38.000000 vocabmaster-0.1.6/vocabmaster/config_handler.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    10722 2023-05-05 18:12:19.000000 vocabmaster-0.1.6/vocabmaster/csv_handler.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     5646 2023-05-04 16:22:59.000000 vocabmaster-0.1.6/vocabmaster/gpt_integration.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     7264 2023-05-04 13:33:03.000000 vocabmaster-0.1.6/vocabmaster/utils.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-05-24 20:40:35.909385 vocabmaster-0.1.6/vocabmaster.egg-info/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     2698 2023-05-24 20:40:35.000000 vocabmaster-0.1.6/vocabmaster.egg-info/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      390 2023-05-24 20:40:35.000000 vocabmaster-0.1.6/vocabmaster.egg-info/SOURCES.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-05-24 20:40:35.000000 vocabmaster-0.1.6/vocabmaster.egg-info/dependency_links.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       60 2023-05-24 20:40:35.000000 vocabmaster-0.1.6/vocabmaster.egg-info/entry_points.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      273 2023-05-24 20:40:35.000000 vocabmaster-0.1.6/vocabmaster.egg-info/requires.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       12 2023-05-24 20:40:35.000000 vocabmaster-0.1.6/vocabmaster.egg-info/top_level.txt
```

### Comparing `vocabmaster-0.1.5/LICENSE` & `vocabmaster-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `vocabmaster-0.1.5/PKG-INFO` & `vocabmaster-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vocabmaster
-Version: 0.1.5
+Version: 0.1.6
 Author: sderev
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # VocabMaster
 
 Master new languages with this user-friendly CLI tool, designed to help you record vocabulary, access translations and examples, and seamlessly import them into Anki for an optimized language learning experience.
```

### Comparing `vocabmaster-0.1.5/README.md` & `vocabmaster-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `vocabmaster-0.1.5/setup.py` & `vocabmaster-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     readme = file.read()
 
 with open("requirements.txt", "r", encoding="utf-8") as file:
     requirements = [line.strip() for line in file]
 
 setup(
     name="vocabmaster",
-    version="0.1.5",
+    version="0.1.6",
     packages=find_packages(),
     install_requires=requirements,
     entry_points={
         "console_scripts": [
             "vocabmaster = vocabmaster.cli:vocabmaster",
         ]
     },
```

### Comparing `vocabmaster-0.1.5/vocabmaster/cli.py` & `vocabmaster-0.1.6/vocabmaster/cli.py`

 * *Files identical despite different names*

### Comparing `vocabmaster-0.1.5/vocabmaster/config_handler.py` & `vocabmaster-0.1.6/vocabmaster/config_handler.py`

 * *Files identical despite different names*

### Comparing `vocabmaster-0.1.5/vocabmaster/csv_handler.py` & `vocabmaster-0.1.6/vocabmaster/csv_handler.py`

 * *Files identical despite different names*

### Comparing `vocabmaster-0.1.5/vocabmaster/gpt_integration.py` & `vocabmaster-0.1.6/vocabmaster/gpt_integration.py`

 * *Files identical despite different names*

### Comparing `vocabmaster-0.1.5/vocabmaster/utils.py` & `vocabmaster-0.1.6/vocabmaster/utils.py`

 * *Files identical despite different names*

### Comparing `vocabmaster-0.1.5/vocabmaster.egg-info/PKG-INFO` & `vocabmaster-0.1.6/vocabmaster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vocabmaster
-Version: 0.1.5
+Version: 0.1.6
 Author: sderev
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # VocabMaster
 
 Master new languages with this user-friendly CLI tool, designed to help you record vocabulary, access translations and examples, and seamlessly import them into Anki for an optimized language learning experience.
```

