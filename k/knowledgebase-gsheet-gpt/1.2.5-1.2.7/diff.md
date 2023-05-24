# Comparing `tmp/knowledgebase-gsheet-gpt-1.2.5.tar.gz` & `tmp/knowledgebase-gsheet-gpt-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "knowledgebase-gsheet-gpt-1.2.5.tar", last modified: Sun May 21 18:57:42 2023, max compression
+gzip compressed data, was "knowledgebase-gsheet-gpt-1.2.7.tar", last modified: Wed May 24 06:38:45 2023, max compression
```

## Comparing `knowledgebase-gsheet-gpt-1.2.5.tar` & `knowledgebase-gsheet-gpt-1.2.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-21 18:57:42.529444 knowledgebase-gsheet-gpt-1.2.5/
--rw-r--r--   0 chiubowen   (501) staff       (20)     1658 2023-05-21 18:57:42.529301 knowledgebase-gsheet-gpt-1.2.5/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)     1476 2023-05-21 18:57:42.000000 knowledgebase-gsheet-gpt-1.2.5/README.md
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-21 18:57:42.529023 knowledgebase-gsheet-gpt-1.2.5/knowledgebase_gsheet_gpt.egg-info/
--rw-r--r--   0 chiubowen   (501) staff       (20)     1658 2023-05-21 18:57:42.000000 knowledgebase-gsheet-gpt-1.2.5/knowledgebase_gsheet_gpt.egg-info/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)      336 2023-05-21 18:57:42.000000 knowledgebase-gsheet-gpt-1.2.5/knowledgebase_gsheet_gpt.egg-info/SOURCES.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-05-21 18:57:42.000000 knowledgebase-gsheet-gpt-1.2.5/knowledgebase_gsheet_gpt.egg-info/dependency_links.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       76 2023-05-21 18:57:42.000000 knowledgebase-gsheet-gpt-1.2.5/knowledgebase_gsheet_gpt.egg-info/entry_points.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)      112 2023-05-21 18:57:42.000000 knowledgebase-gsheet-gpt-1.2.5/knowledgebase_gsheet_gpt.egg-info/requires.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       25 2023-05-21 18:57:42.000000 knowledgebase-gsheet-gpt-1.2.5/knowledgebase_gsheet_gpt.egg-info/top_level.txt
--rwxr-xr-x   0 chiubowen   (501) staff       (20)     6193 2023-05-21 18:57:42.000000 knowledgebase-gsheet-gpt-1.2.5/knowledgebase_gsheet_gpt.py
--rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-05-21 18:57:42.529497 knowledgebase-gsheet-gpt-1.2.5/setup.cfg
--rw-r--r--   0 chiubowen   (501) staff       (20)      560 2023-05-21 18:57:42.000000 knowledgebase-gsheet-gpt-1.2.5/setup.py
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-24 06:38:45.322763 knowledgebase-gsheet-gpt-1.2.7/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     1658 2023-05-24 06:38:45.322647 knowledgebase-gsheet-gpt-1.2.7/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)     1476 2023-05-24 06:38:45.000000 knowledgebase-gsheet-gpt-1.2.7/README.md
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-24 06:38:45.322474 knowledgebase-gsheet-gpt-1.2.7/knowledgebase_gsheet_gpt.egg-info/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     1658 2023-05-24 06:38:45.000000 knowledgebase-gsheet-gpt-1.2.7/knowledgebase_gsheet_gpt.egg-info/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)      336 2023-05-24 06:38:45.000000 knowledgebase-gsheet-gpt-1.2.7/knowledgebase_gsheet_gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-05-24 06:38:45.000000 knowledgebase-gsheet-gpt-1.2.7/knowledgebase_gsheet_gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       76 2023-05-24 06:38:45.000000 knowledgebase-gsheet-gpt-1.2.7/knowledgebase_gsheet_gpt.egg-info/entry_points.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)      112 2023-05-24 06:38:45.000000 knowledgebase-gsheet-gpt-1.2.7/knowledgebase_gsheet_gpt.egg-info/requires.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       25 2023-05-24 06:38:45.000000 knowledgebase-gsheet-gpt-1.2.7/knowledgebase_gsheet_gpt.egg-info/top_level.txt
+-rwxr-xr-x   0 chiubowen   (501) staff       (20)     6193 2023-05-24 06:38:45.000000 knowledgebase-gsheet-gpt-1.2.7/knowledgebase_gsheet_gpt.py
+-rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-05-24 06:38:45.322798 knowledgebase-gsheet-gpt-1.2.7/setup.cfg
+-rw-r--r--   0 chiubowen   (501) staff       (20)      560 2023-05-24 06:38:45.000000 knowledgebase-gsheet-gpt-1.2.7/setup.py
```

### Comparing `knowledgebase-gsheet-gpt-1.2.5/PKG-INFO` & `knowledgebase-gsheet-gpt-1.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: knowledgebase-gsheet-gpt
-Version: 1.2.5
+Version: 1.2.7
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # Knowledgebase GSheet GPT
```

### Comparing `knowledgebase-gsheet-gpt-1.2.5/README.md` & `knowledgebase-gsheet-gpt-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `knowledgebase-gsheet-gpt-1.2.5/knowledgebase_gsheet_gpt.egg-info/PKG-INFO` & `knowledgebase-gsheet-gpt-1.2.7/knowledgebase_gsheet_gpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: knowledgebase-gsheet-gpt
-Version: 1.2.5
+Version: 1.2.7
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # Knowledgebase GSheet GPT
```

### Comparing `knowledgebase-gsheet-gpt-1.2.5/knowledgebase_gsheet_gpt.py` & `knowledgebase-gsheet-gpt-1.2.7/knowledgebase_gsheet_gpt.py`

 * *Files identical despite different names*

### Comparing `knowledgebase-gsheet-gpt-1.2.5/setup.py` & `knowledgebase-gsheet-gpt-1.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = [line.strip() for line in f.readlines()]
 
 setup(
     name="knowledgebase-gsheet-gpt",
-    version="1.2.5",
+    version="1.2.7",
     packages=find_packages(),
     py_modules=['knowledgebase_gsheet_gpt'],
     install_requires=requirements,
     entry_points={
         'console_scripts': [
             'knowledgebase_gsheet_gpt = knowledgebase_gsheet_gpt:main',
         ],
```

