# Comparing `tmp/error_suggester-0.1.1.tar.gz` & `tmp/error_suggester-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "error_suggester-0.1.1.tar", last modified: Wed May 24 09:12:16 2023, max compression
+gzip compressed data, was "error_suggester-0.1.2.tar", last modified: Wed May 24 09:22:26 2023, max compression
```

## Comparing `error_suggester-0.1.1.tar` & `error_suggester-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 harisbinsaif   (501) staff       (20)        0 2023-05-24 09:12:16.501307 error_suggester-0.1.1/
--rw-r--r--   0 harisbinsaif   (501) staff       (20)     1071 2023-05-24 07:31:52.000000 error_suggester-0.1.1/LICENSE
--rw-r--r--   0 harisbinsaif   (501) staff       (20)      894 2023-05-24 09:12:16.501197 error_suggester-0.1.1/PKG-INFO
--rw-r--r--   0 harisbinsaif   (501) staff       (20)      563 2023-05-24 07:45:36.000000 error_suggester-0.1.1/README.md
-drwxr-xr-x   0 harisbinsaif   (501) staff       (20)        0 2023-05-24 09:12:16.500459 error_suggester-0.1.1/error_suggester/
--rw-r--r--   0 harisbinsaif   (501) staff       (20)      140 2023-05-23 17:29:51.000000 error_suggester-0.1.1/error_suggester/__init__.py
--rw-r--r--   0 harisbinsaif   (501) staff       (20)     1165 2023-05-24 07:45:36.000000 error_suggester-0.1.1/error_suggester/error_suggester.py
-drwxr-xr-x   0 harisbinsaif   (501) staff       (20)        0 2023-05-24 09:12:16.501034 error_suggester-0.1.1/error_suggester.egg-info/
--rw-r--r--   0 harisbinsaif   (501) staff       (20)      894 2023-05-24 09:12:16.000000 error_suggester-0.1.1/error_suggester.egg-info/PKG-INFO
--rw-r--r--   0 harisbinsaif   (501) staff       (20)      283 2023-05-24 09:12:16.000000 error_suggester-0.1.1/error_suggester.egg-info/SOURCES.txt
--rw-r--r--   0 harisbinsaif   (501) staff       (20)        1 2023-05-24 09:12:16.000000 error_suggester-0.1.1/error_suggester.egg-info/dependency_links.txt
--rw-r--r--   0 harisbinsaif   (501) staff       (20)        7 2023-05-24 09:12:16.000000 error_suggester-0.1.1/error_suggester.egg-info/requires.txt
--rw-r--r--   0 harisbinsaif   (501) staff       (20)       16 2023-05-24 09:12:16.000000 error_suggester-0.1.1/error_suggester.egg-info/top_level.txt
--rw-r--r--   0 harisbinsaif   (501) staff       (20)       38 2023-05-24 09:12:16.501345 error_suggester-0.1.1/setup.cfg
--rw-r--r--   0 harisbinsaif   (501) staff       (20)      646 2023-05-24 09:12:07.000000 error_suggester-0.1.1/setup.py
+drwxr-xr-x   0 harisbinsaif   (501) staff       (20)        0 2023-05-24 09:22:26.198444 error_suggester-0.1.2/
+-rw-r--r--   0 harisbinsaif   (501) staff       (20)     1071 2023-05-24 07:31:52.000000 error_suggester-0.1.2/LICENSE
+-rw-r--r--   0 harisbinsaif   (501) staff       (20)      894 2023-05-24 09:22:26.198314 error_suggester-0.1.2/PKG-INFO
+-rw-r--r--   0 harisbinsaif   (501) staff       (20)      563 2023-05-24 07:45:36.000000 error_suggester-0.1.2/README.md
+drwxr-xr-x   0 harisbinsaif   (501) staff       (20)        0 2023-05-24 09:22:26.197382 error_suggester-0.1.2/error_suggester/
+-rw-r--r--   0 harisbinsaif   (501) staff       (20)      331 2023-05-24 09:21:55.000000 error_suggester-0.1.2/error_suggester/__init__.py
+-rw-r--r--   0 harisbinsaif   (501) staff       (20)     1165 2023-05-24 07:45:36.000000 error_suggester-0.1.2/error_suggester/error_suggester.py
+drwxr-xr-x   0 harisbinsaif   (501) staff       (20)        0 2023-05-24 09:22:26.198131 error_suggester-0.1.2/error_suggester.egg-info/
+-rw-r--r--   0 harisbinsaif   (501) staff       (20)      894 2023-05-24 09:22:26.000000 error_suggester-0.1.2/error_suggester.egg-info/PKG-INFO
+-rw-r--r--   0 harisbinsaif   (501) staff       (20)      283 2023-05-24 09:22:26.000000 error_suggester-0.1.2/error_suggester.egg-info/SOURCES.txt
+-rw-r--r--   0 harisbinsaif   (501) staff       (20)        1 2023-05-24 09:22:26.000000 error_suggester-0.1.2/error_suggester.egg-info/dependency_links.txt
+-rw-r--r--   0 harisbinsaif   (501) staff       (20)        7 2023-05-24 09:22:26.000000 error_suggester-0.1.2/error_suggester.egg-info/requires.txt
+-rw-r--r--   0 harisbinsaif   (501) staff       (20)       16 2023-05-24 09:22:26.000000 error_suggester-0.1.2/error_suggester.egg-info/top_level.txt
+-rw-r--r--   0 harisbinsaif   (501) staff       (20)       38 2023-05-24 09:22:26.198486 error_suggester-0.1.2/setup.cfg
+-rw-r--r--   0 harisbinsaif   (501) staff       (20)      646 2023-05-24 09:22:01.000000 error_suggester-0.1.2/setup.py
```

### Comparing `error_suggester-0.1.1/LICENSE` & `error_suggester-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `error_suggester-0.1.1/PKG-INFO` & `error_suggester-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: error_suggester
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python library for error suggestions using ChatGPT
 Home-page: https://github.com/HarisBinSaif/ErrorSuggester
 Author: HarisBinSaif
 Project-URL: GitHub, https://github.com/HarisBinSaif/ErrorSuggester
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `error_suggester-0.1.1/README.md` & `error_suggester-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `error_suggester-0.1.1/error_suggester/error_suggester.py` & `error_suggester-0.1.2/error_suggester/error_suggester.py`

 * *Files identical despite different names*

### Comparing `error_suggester-0.1.1/error_suggester.egg-info/PKG-INFO` & `error_suggester-0.1.2/error_suggester.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: error-suggester
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python library for error suggestions using ChatGPT
 Home-page: https://github.com/HarisBinSaif/ErrorSuggester
 Author: HarisBinSaif
 Project-URL: GitHub, https://github.com/HarisBinSaif/ErrorSuggester
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `error_suggester-0.1.1/setup.py` & `error_suggester-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='error_suggester',
-    version='0.1.1',
+    version='0.1.2',
     url='https://github.com/HarisBinSaif/ErrorSuggester',
     project_urls={
         'GitHub': 'https://github.com/HarisBinSaif/ErrorSuggester',
     },
     description='A Python library for error suggestions using ChatGPT',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

