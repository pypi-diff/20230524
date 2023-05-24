# Comparing `tmp/wordlink-1.0.5.tar.gz` & `tmp/wordlink-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wordlink-1.0.5.tar", last modified: Wed May 24 21:16:56 2023, max compression
+gzip compressed data, was "wordlink-1.0.7.tar", last modified: Wed May 24 21:48:05 2023, max compression
```

## Comparing `wordlink-1.0.5.tar` & `wordlink-1.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 bloom      (501) staff       (20)        0 2023-05-24 21:16:56.719028 wordlink-1.0.5/
--rw-r--r--   0 bloom      (501) staff       (20)     1048 2023-05-24 20:43:31.000000 wordlink-1.0.5/LICENSE
--rw-r--r--   0 bloom      (501) staff       (20)      523 2023-05-24 21:16:56.719096 wordlink-1.0.5/PKG-INFO
--rw-r--r--   0 bloom      (501) staff       (20)     3641 2023-05-24 21:00:09.000000 wordlink-1.0.5/README
--rw-r--r--   0 bloom      (501) staff       (20)      746 2023-05-24 21:16:56.719330 wordlink-1.0.5/setup.cfg
--rw-r--r--   0 bloom      (501) staff       (20)      713 2023-05-24 20:57:22.000000 wordlink-1.0.5/setup.py
-drwxr-xr-x   0 bloom      (501) staff       (20)        0 2023-05-24 21:16:56.717798 wordlink-1.0.5/tests/
--rw-r--r--   0 bloom      (501) staff       (20)        0 2023-05-24 20:48:47.000000 wordlink-1.0.5/tests/__init__.py
--rw-r--r--   0 bloom      (501) staff       (20)     3758 2023-05-24 20:43:31.000000 wordlink-1.0.5/tests/main_test.py
-drwxr-xr-x   0 bloom      (501) staff       (20)        0 2023-05-24 21:16:56.718147 wordlink-1.0.5/wordlink/
--rw-r--r--   0 bloom      (501) staff       (20)        0 2023-05-24 20:43:31.000000 wordlink-1.0.5/wordlink/__init__.py
--rw-r--r--   0 bloom      (501) staff       (20)     3582 2023-05-24 20:43:31.000000 wordlink-1.0.5/wordlink/__main__.py
-drwxr-xr-x   0 bloom      (501) staff       (20)        0 2023-05-24 21:16:56.718935 wordlink-1.0.5/wordlink.egg-info/
--rw-r--r--   0 bloom      (501) staff       (20)      523 2023-05-24 21:16:56.000000 wordlink-1.0.5/wordlink.egg-info/PKG-INFO
--rw-r--r--   0 bloom      (501) staff       (20)      306 2023-05-24 21:16:56.000000 wordlink-1.0.5/wordlink.egg-info/SOURCES.txt
--rw-r--r--   0 bloom      (501) staff       (20)        1 2023-05-24 21:16:56.000000 wordlink-1.0.5/wordlink.egg-info/dependency_links.txt
--rw-r--r--   0 bloom      (501) staff       (20)       43 2023-05-24 21:16:56.000000 wordlink-1.0.5/wordlink.egg-info/entry_points.txt
--rw-r--r--   0 bloom      (501) staff       (20)       24 2023-05-24 21:16:56.000000 wordlink-1.0.5/wordlink.egg-info/requires.txt
--rw-r--r--   0 bloom      (501) staff       (20)       15 2023-05-24 21:16:56.000000 wordlink-1.0.5/wordlink.egg-info/top_level.txt
+drwxr-xr-x   0 bloom      (501) staff       (20)        0 2023-05-24 21:48:05.674206 wordlink-1.0.7/
+-rw-r--r--   0 bloom      (501) staff       (20)     1048 2023-05-24 20:43:31.000000 wordlink-1.0.7/LICENSE
+-rw-r--r--   0 bloom      (501) staff       (20)     4165 2023-05-24 21:48:05.674302 wordlink-1.0.7/PKG-INFO
+-rw-r--r--   0 bloom      (501) staff       (20)     3641 2023-05-24 21:44:10.000000 wordlink-1.0.7/README.md
+-rw-r--r--   0 bloom      (501) staff       (20)      746 2023-05-24 21:48:05.674720 wordlink-1.0.7/setup.cfg
+-rw-r--r--   0 bloom      (501) staff       (20)      713 2023-05-24 21:47:56.000000 wordlink-1.0.7/setup.py
+drwxr-xr-x   0 bloom      (501) staff       (20)        0 2023-05-24 21:48:05.673035 wordlink-1.0.7/tests/
+-rw-r--r--   0 bloom      (501) staff       (20)        0 2023-05-24 20:48:47.000000 wordlink-1.0.7/tests/__init__.py
+-rw-r--r--   0 bloom      (501) staff       (20)     3758 2023-05-24 20:43:31.000000 wordlink-1.0.7/tests/main_test.py
+drwxr-xr-x   0 bloom      (501) staff       (20)        0 2023-05-24 21:48:05.673434 wordlink-1.0.7/wordlink/
+-rw-r--r--   0 bloom      (501) staff       (20)        0 2023-05-24 20:43:31.000000 wordlink-1.0.7/wordlink/__init__.py
+-rw-r--r--   0 bloom      (501) staff       (20)     3582 2023-05-24 20:43:31.000000 wordlink-1.0.7/wordlink/__main__.py
+drwxr-xr-x   0 bloom      (501) staff       (20)        0 2023-05-24 21:48:05.674126 wordlink-1.0.7/wordlink.egg-info/
+-rw-r--r--   0 bloom      (501) staff       (20)     4165 2023-05-24 21:48:05.000000 wordlink-1.0.7/wordlink.egg-info/PKG-INFO
+-rw-r--r--   0 bloom      (501) staff       (20)      319 2023-05-24 21:48:05.000000 wordlink-1.0.7/wordlink.egg-info/SOURCES.txt
+-rw-r--r--   0 bloom      (501) staff       (20)        1 2023-05-24 21:48:05.000000 wordlink-1.0.7/wordlink.egg-info/dependency_links.txt
+-rw-r--r--   0 bloom      (501) staff       (20)       43 2023-05-24 21:48:05.000000 wordlink-1.0.7/wordlink.egg-info/entry_points.txt
+-rw-r--r--   0 bloom      (501) staff       (20)       24 2023-05-24 21:48:05.000000 wordlink-1.0.7/wordlink.egg-info/requires.txt
+-rw-r--r--   0 bloom      (501) staff       (20)       15 2023-05-24 21:48:05.000000 wordlink-1.0.7/wordlink.egg-info/top_level.txt
```

### Comparing `wordlink-1.0.5/LICENSE` & `wordlink-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `wordlink-1.0.5/README` & `wordlink-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `wordlink-1.0.5/setup.cfg` & `wordlink-1.0.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = wordlink
-version = 1.0.5
+version = 1.0.7
 author = Trevor Bloomfield
 author_email = bloomfieldtm@gmail.com
 description = A Word Link Generator that searches for a given term in multiple text files within a specified directory and generates links to the matched occurrences.
 long_description = file: readme.md
 long_description_content_type = text/markdown
 url = https://github.com/psibir/wordlink
 classifiers =
```

### Comparing `wordlink-1.0.5/setup.py` & `wordlink-1.0.7/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='wordlink',
-    version='1.0.5',
+    version='1.0.7',
     author='Trevor Bloomfield',
     author_email='bloomfieldtm@gmail.com',
     description='Word Link Generator',
     py_modules=['wordlink'],
     url = 'https://github.com/psibir/wordlink',   # Provide either the link to your github or to your website
     download_url = 'https://github.com/psibir/wordlink/archive/v_01.tar.gz',    # I explain this later on
     keywords = ['word', 'link', 'html', 'console'],   # Keywords that define your package best
```

### Comparing `wordlink-1.0.5/tests/main_test.py` & `wordlink-1.0.7/tests/main_test.py`

 * *Files identical despite different names*

### Comparing `wordlink-1.0.5/wordlink/__main__.py` & `wordlink-1.0.7/wordlink/__main__.py`

 * *Files identical despite different names*

