# Comparing `tmp/inspirational_quotes-0.0.7.tar.gz` & `tmp/inspirational_quotes-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inspirational_quotes-0.0.7.tar", last modified: Tue Mar 14 10:49:44 2023, max compression
+gzip compressed data, was "inspirational_quotes-0.0.8.tar", last modified: Wed May 24 12:19:42 2023, max compression
```

## Comparing `inspirational_quotes-0.0.7.tar` & `inspirational_quotes-0.0.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 ssambarathi  (1000) ssambarathi  (1000)        0 2023-03-14 10:49:44.660481 inspirational_quotes-0.0.7/
--rw-rw-r--   0 ssambarathi  (1000) ssambarathi  (1000)     1070 2023-03-13 11:47:41.000000 inspirational_quotes-0.0.7/LICENSE
--rw-rw-r--   0 ssambarathi  (1000) ssambarathi  (1000)      598 2023-03-14 10:49:44.660481 inspirational_quotes-0.0.7/PKG-INFO
--rw-rw-r--   0 ssambarathi  (1000) ssambarathi  (1000)       89 2023-03-14 04:43:03.000000 inspirational_quotes-0.0.7/README.md
-drwxrwxr-x   0 ssambarathi  (1000) ssambarathi  (1000)        0 2023-03-14 10:49:44.652481 inspirational_quotes-0.0.7/inspirational_quotes/
--rw-rw-r--   0 ssambarathi  (1000) ssambarathi  (1000)       39 2023-03-14 04:43:03.000000 inspirational_quotes-0.0.7/inspirational_quotes/__init__.py
--rw-rw-r--   0 ssambarathi  (1000) ssambarathi  (1000)      128 2023-03-14 04:43:03.000000 inspirational_quotes-0.0.7/inspirational_quotes/example.py
--rw-rw-r--   0 ssambarathi  (1000) ssambarathi  (1000)      310 2023-03-14 10:29:24.000000 inspirational_quotes-0.0.7/inspirational_quotes/inspirational_quotes.py
-drwxrwxr-x   0 ssambarathi  (1000) ssambarathi  (1000)        0 2023-03-14 10:49:44.656481 inspirational_quotes-0.0.7/inspirational_quotes/quotes/
--rw-rw-r--   0 ssambarathi  (1000) ssambarathi  (1000)        0 2023-03-14 10:41:04.000000 inspirational_quotes-0.0.7/inspirational_quotes/quotes/__init__.py
--rw-rw-r--   0 ssambarathi  (1000) ssambarathi  (1000)    50378 2023-03-14 04:43:03.000000 inspirational_quotes-0.0.7/inspirational_quotes/quotes/quotes.json
-drwxrwxr-x   0 ssambarathi  (1000) ssambarathi  (1000)        0 2023-03-14 10:49:44.656481 inspirational_quotes-0.0.7/inspirational_quotes/tests/
--rw-rw-r--   0 ssambarathi  (1000) ssambarathi  (1000)        0 2023-03-14 10:41:25.000000 inspirational_quotes-0.0.7/inspirational_quotes/tests/__init__.py
--rw-rw-r--   0 ssambarathi  (1000) ssambarathi  (1000)       18 2023-03-14 04:43:03.000000 inspirational_quotes-0.0.7/inspirational_quotes/tests/test.py
-drwxrwxr-x   0 ssambarathi  (1000) ssambarathi  (1000)        0 2023-03-14 10:49:44.656481 inspirational_quotes-0.0.7/inspirational_quotes.egg-info/
--rw-rw-r--   0 ssambarathi  (1000) ssambarathi  (1000)      598 2023-03-14 10:49:44.000000 inspirational_quotes-0.0.7/inspirational_quotes.egg-info/PKG-INFO
--rw-rw-r--   0 ssambarathi  (1000) ssambarathi  (1000)      509 2023-03-14 10:49:44.000000 inspirational_quotes-0.0.7/inspirational_quotes.egg-info/SOURCES.txt
--rw-rw-r--   0 ssambarathi  (1000) ssambarathi  (1000)        1 2023-03-14 10:49:44.000000 inspirational_quotes-0.0.7/inspirational_quotes.egg-info/dependency_links.txt
--rw-rw-r--   0 ssambarathi  (1000) ssambarathi  (1000)        6 2023-03-14 10:49:44.000000 inspirational_quotes-0.0.7/inspirational_quotes.egg-info/requires.txt
--rw-rw-r--   0 ssambarathi  (1000) ssambarathi  (1000)       21 2023-03-14 10:49:44.000000 inspirational_quotes-0.0.7/inspirational_quotes.egg-info/top_level.txt
--rw-rw-r--   0 ssambarathi  (1000) ssambarathi  (1000)       38 2023-03-14 10:49:44.660481 inspirational_quotes-0.0.7/setup.cfg
--rw-rw-r--   0 ssambarathi  (1000) ssambarathi  (1000)      876 2023-03-14 10:49:24.000000 inspirational_quotes-0.0.7/setup.py
+drwxrwxr-x   0 ssambarathi  (1000) ssambarathi  (1000)        0 2023-05-24 12:19:42.606927 inspirational_quotes-0.0.8/
+-rw-rw-r--   0 ssambarathi  (1000) ssambarathi  (1000)     1070 2023-05-24 11:58:44.000000 inspirational_quotes-0.0.8/LICENSE
+-rw-rw-r--   0 ssambarathi  (1000) ssambarathi  (1000)     1571 2023-05-24 12:19:42.606927 inspirational_quotes-0.0.8/PKG-INFO
+-rw-rw-r--   0 ssambarathi  (1000) ssambarathi  (1000)     1064 2023-05-24 11:58:44.000000 inspirational_quotes-0.0.8/README.md
+drwxrwxr-x   0 ssambarathi  (1000) ssambarathi  (1000)        0 2023-05-24 12:19:42.602928 inspirational_quotes-0.0.8/inspirational_quotes/
+-rw-rw-r--   0 ssambarathi  (1000) ssambarathi  (1000)       39 2023-05-24 11:58:44.000000 inspirational_quotes-0.0.8/inspirational_quotes/__init__.py
+-rw-rw-r--   0 ssambarathi  (1000) ssambarathi  (1000)      128 2023-05-24 11:58:44.000000 inspirational_quotes-0.0.8/inspirational_quotes/example.py
+-rw-rw-r--   0 ssambarathi  (1000) ssambarathi  (1000)      343 2023-05-24 12:02:14.000000 inspirational_quotes-0.0.8/inspirational_quotes/inspirational_quotes.py
+drwxrwxr-x   0 ssambarathi  (1000) ssambarathi  (1000)        0 2023-05-24 12:19:42.606927 inspirational_quotes-0.0.8/inspirational_quotes/quotes/
+-rw-rw-r--   0 ssambarathi  (1000) ssambarathi  (1000)        0 2023-05-24 11:58:44.000000 inspirational_quotes-0.0.8/inspirational_quotes/quotes/__init__.py
+-rw-rw-r--   0 ssambarathi  (1000) ssambarathi  (1000)    50378 2023-05-24 11:58:44.000000 inspirational_quotes-0.0.8/inspirational_quotes/quotes/quotes.json
+drwxrwxr-x   0 ssambarathi  (1000) ssambarathi  (1000)        0 2023-05-24 12:19:42.606927 inspirational_quotes-0.0.8/inspirational_quotes/tests/
+-rw-rw-r--   0 ssambarathi  (1000) ssambarathi  (1000)        0 2023-05-24 11:58:44.000000 inspirational_quotes-0.0.8/inspirational_quotes/tests/__init__.py
+-rw-rw-r--   0 ssambarathi  (1000) ssambarathi  (1000)       18 2023-05-24 11:58:44.000000 inspirational_quotes-0.0.8/inspirational_quotes/tests/test.py
+drwxrwxr-x   0 ssambarathi  (1000) ssambarathi  (1000)        0 2023-05-24 12:19:42.606927 inspirational_quotes-0.0.8/inspirational_quotes.egg-info/
+-rw-rw-r--   0 ssambarathi  (1000) ssambarathi  (1000)     1571 2023-05-24 12:19:42.000000 inspirational_quotes-0.0.8/inspirational_quotes.egg-info/PKG-INFO
+-rw-rw-r--   0 ssambarathi  (1000) ssambarathi  (1000)      509 2023-05-24 12:19:42.000000 inspirational_quotes-0.0.8/inspirational_quotes.egg-info/SOURCES.txt
+-rw-rw-r--   0 ssambarathi  (1000) ssambarathi  (1000)        1 2023-05-24 12:19:42.000000 inspirational_quotes-0.0.8/inspirational_quotes.egg-info/dependency_links.txt
+-rw-rw-r--   0 ssambarathi  (1000) ssambarathi  (1000)        6 2023-05-24 12:19:42.000000 inspirational_quotes-0.0.8/inspirational_quotes.egg-info/requires.txt
+-rw-rw-r--   0 ssambarathi  (1000) ssambarathi  (1000)       21 2023-05-24 12:19:42.000000 inspirational_quotes-0.0.8/inspirational_quotes.egg-info/top_level.txt
+-rw-rw-r--   0 ssambarathi  (1000) ssambarathi  (1000)       38 2023-05-24 12:19:42.606927 inspirational_quotes-0.0.8/setup.cfg
+-rw-rw-r--   0 ssambarathi  (1000) ssambarathi  (1000)      876 2023-05-24 12:17:27.000000 inspirational_quotes-0.0.8/setup.py
```

### Comparing `inspirational_quotes-0.0.7/LICENSE` & `inspirational_quotes-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `inspirational_quotes-0.0.7/inspirational_quotes/quotes/quotes.json` & `inspirational_quotes-0.0.8/inspirational_quotes/quotes/quotes.json`

 * *Files identical despite different names*

### Comparing `inspirational_quotes-0.0.7/setup.py` & `inspirational_quotes-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="inspirational_quotes",
-    version="0.0.7",
+    version="0.0.8",
     author="saip007",
     author_email="saip4622@outlook.com",
     description="inspirational quotes package",
     license='MIT',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/saip007/inspirational_quotes",
```

