# Comparing `tmp/error_suggester-0.1.0.tar.gz` & `tmp/error_suggester-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "error_suggester-0.1.0.tar", last modified: Wed May 24 07:50:07 2023, max compression
+gzip compressed data, was "error_suggester-0.1.1.tar", last modified: Wed May 24 09:12:16 2023, max compression
```

## Comparing `error_suggester-0.1.0.tar` & `error_suggester-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 harisbinsaif   (501) staff       (20)        0 2023-05-24 07:50:07.748895 error_suggester-0.1.0/
--rw-r--r--   0 harisbinsaif   (501) staff       (20)     1071 2023-05-24 07:31:52.000000 error_suggester-0.1.0/LICENSE
--rw-r--r--   0 harisbinsaif   (501) staff       (20)      164 2023-05-24 07:50:07.748752 error_suggester-0.1.0/PKG-INFO
--rw-r--r--   0 harisbinsaif   (501) staff       (20)      563 2023-05-24 07:45:36.000000 error_suggester-0.1.0/README.md
-drwxr-xr-x   0 harisbinsaif   (501) staff       (20)        0 2023-05-24 07:50:07.747179 error_suggester-0.1.0/error_suggester/
--rw-r--r--   0 harisbinsaif   (501) staff       (20)      140 2023-05-23 17:29:51.000000 error_suggester-0.1.0/error_suggester/__init__.py
--rw-r--r--   0 harisbinsaif   (501) staff       (20)     1165 2023-05-24 07:45:36.000000 error_suggester-0.1.0/error_suggester/error_suggester.py
-drwxr-xr-x   0 harisbinsaif   (501) staff       (20)        0 2023-05-24 07:50:07.748447 error_suggester-0.1.0/error_suggester.egg-info/
--rw-r--r--   0 harisbinsaif   (501) staff       (20)      164 2023-05-24 07:50:07.000000 error_suggester-0.1.0/error_suggester.egg-info/PKG-INFO
--rw-r--r--   0 harisbinsaif   (501) staff       (20)      283 2023-05-24 07:50:07.000000 error_suggester-0.1.0/error_suggester.egg-info/SOURCES.txt
--rw-r--r--   0 harisbinsaif   (501) staff       (20)        1 2023-05-24 07:50:07.000000 error_suggester-0.1.0/error_suggester.egg-info/dependency_links.txt
--rw-r--r--   0 harisbinsaif   (501) staff       (20)        7 2023-05-24 07:50:07.000000 error_suggester-0.1.0/error_suggester.egg-info/requires.txt
--rw-r--r--   0 harisbinsaif   (501) staff       (20)       16 2023-05-24 07:50:07.000000 error_suggester-0.1.0/error_suggester.egg-info/top_level.txt
--rw-r--r--   0 harisbinsaif   (501) staff       (20)       38 2023-05-24 07:50:07.749022 error_suggester-0.1.0/setup.cfg
--rw-r--r--   0 harisbinsaif   (501) staff       (20)      320 2023-05-24 07:45:36.000000 error_suggester-0.1.0/setup.py
+drwxr-xr-x   0 harisbinsaif   (501) staff       (20)        0 2023-05-24 09:12:16.501307 error_suggester-0.1.1/
+-rw-r--r--   0 harisbinsaif   (501) staff       (20)     1071 2023-05-24 07:31:52.000000 error_suggester-0.1.1/LICENSE
+-rw-r--r--   0 harisbinsaif   (501) staff       (20)      894 2023-05-24 09:12:16.501197 error_suggester-0.1.1/PKG-INFO
+-rw-r--r--   0 harisbinsaif   (501) staff       (20)      563 2023-05-24 07:45:36.000000 error_suggester-0.1.1/README.md
+drwxr-xr-x   0 harisbinsaif   (501) staff       (20)        0 2023-05-24 09:12:16.500459 error_suggester-0.1.1/error_suggester/
+-rw-r--r--   0 harisbinsaif   (501) staff       (20)      140 2023-05-23 17:29:51.000000 error_suggester-0.1.1/error_suggester/__init__.py
+-rw-r--r--   0 harisbinsaif   (501) staff       (20)     1165 2023-05-24 07:45:36.000000 error_suggester-0.1.1/error_suggester/error_suggester.py
+drwxr-xr-x   0 harisbinsaif   (501) staff       (20)        0 2023-05-24 09:12:16.501034 error_suggester-0.1.1/error_suggester.egg-info/
+-rw-r--r--   0 harisbinsaif   (501) staff       (20)      894 2023-05-24 09:12:16.000000 error_suggester-0.1.1/error_suggester.egg-info/PKG-INFO
+-rw-r--r--   0 harisbinsaif   (501) staff       (20)      283 2023-05-24 09:12:16.000000 error_suggester-0.1.1/error_suggester.egg-info/SOURCES.txt
+-rw-r--r--   0 harisbinsaif   (501) staff       (20)        1 2023-05-24 09:12:16.000000 error_suggester-0.1.1/error_suggester.egg-info/dependency_links.txt
+-rw-r--r--   0 harisbinsaif   (501) staff       (20)        7 2023-05-24 09:12:16.000000 error_suggester-0.1.1/error_suggester.egg-info/requires.txt
+-rw-r--r--   0 harisbinsaif   (501) staff       (20)       16 2023-05-24 09:12:16.000000 error_suggester-0.1.1/error_suggester.egg-info/top_level.txt
+-rw-r--r--   0 harisbinsaif   (501) staff       (20)       38 2023-05-24 09:12:16.501345 error_suggester-0.1.1/setup.cfg
+-rw-r--r--   0 harisbinsaif   (501) staff       (20)      646 2023-05-24 09:12:07.000000 error_suggester-0.1.1/setup.py
```

### Comparing `error_suggester-0.1.0/LICENSE` & `error_suggester-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `error_suggester-0.1.0/README.md` & `error_suggester-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `error_suggester-0.1.0/error_suggester/error_suggester.py` & `error_suggester-0.1.1/error_suggester/error_suggester.py`

 * *Files identical despite different names*

