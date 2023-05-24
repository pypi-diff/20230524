# Comparing `tmp/braintrust-0.0.1.tar.gz` & `tmp/braintrust-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "braintrust-0.0.1.tar", last modified: Wed May 24 03:25:17 2023, max compression
+gzip compressed data, was "braintrust-0.0.2.tar", last modified: Wed May 24 03:34:59 2023, max compression
```

## Comparing `braintrust-0.0.1.tar` & `braintrust-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-05-24 03:25:17.866247 braintrust-0.0.1/
--rw-r--r--   0 ankur      (501) staff       (20)      494 2023-05-24 03:25:17.866085 braintrust-0.0.1/PKG-INFO
--rw-r--r--   0 ankur      (501) staff       (20)       49 2023-04-02 02:49:19.000000 braintrust-0.0.1/README.md
--rw-r--r--   0 ankur      (501) staff       (20)       38 2023-05-24 03:25:17.866293 braintrust-0.0.1/setup.cfg
--rw-r--r--   0 ankur      (501) staff       (20)     1592 2023-05-24 03:21:54.000000 braintrust-0.0.1/setup.py
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-05-24 03:25:17.864517 braintrust-0.0.1/src/
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-05-24 03:25:17.865218 braintrust-0.0.1/src/braintrust/
--rw-r--r--   0 ankur      (501) staff       (20)    10847 2023-05-21 16:20:09.000000 braintrust-0.0.1/src/braintrust/__init__.py
--rw-r--r--   0 ankur      (501) staff       (20)      123 2023-05-14 19:33:59.000000 braintrust-0.0.1/src/braintrust/cache.py
--rw-r--r--   0 ankur      (501) staff       (20)      811 2023-04-15 21:46:41.000000 braintrust-0.0.1/src/braintrust/oai.py
--rw-r--r--   0 ankur      (501) staff       (20)       18 2023-04-02 02:49:19.000000 braintrust-0.0.1/src/braintrust/version.py
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-05-24 03:25:17.865889 braintrust-0.0.1/src/braintrust.egg-info/
--rw-r--r--   0 ankur      (501) staff       (20)      494 2023-05-24 03:25:17.000000 braintrust-0.0.1/src/braintrust.egg-info/PKG-INFO
--rw-r--r--   0 ankur      (501) staff       (20)      347 2023-05-24 03:25:17.000000 braintrust-0.0.1/src/braintrust.egg-info/SOURCES.txt
--rw-r--r--   0 ankur      (501) staff       (20)        1 2023-05-24 03:25:17.000000 braintrust-0.0.1/src/braintrust.egg-info/dependency_links.txt
--rw-r--r--   0 ankur      (501) staff       (20)       60 2023-05-24 03:25:17.000000 braintrust-0.0.1/src/braintrust.egg-info/entry_points.txt
--rw-r--r--   0 ankur      (501) staff       (20)      196 2023-05-24 03:25:17.000000 braintrust-0.0.1/src/braintrust.egg-info/requires.txt
--rw-r--r--   0 ankur      (501) staff       (20)       11 2023-05-24 03:25:17.000000 braintrust-0.0.1/src/braintrust.egg-info/top_level.txt
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-05-24 03:34:59.807954 braintrust-0.0.2/
+-rw-r--r--   0 ankur      (501) staff       (20)      494 2023-05-24 03:34:59.807785 braintrust-0.0.2/PKG-INFO
+-rw-r--r--   0 ankur      (501) staff       (20)       49 2023-04-02 02:49:19.000000 braintrust-0.0.2/README.md
+-rw-r--r--   0 ankur      (501) staff       (20)       38 2023-05-24 03:34:59.808003 braintrust-0.0.2/setup.cfg
+-rw-r--r--   0 ankur      (501) staff       (20)     1592 2023-05-24 03:21:54.000000 braintrust-0.0.2/setup.py
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-05-24 03:34:59.804862 braintrust-0.0.2/src/
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-05-24 03:34:59.806839 braintrust-0.0.2/src/braintrust/
+-rw-r--r--   0 ankur      (501) staff       (20)    10847 2023-05-21 16:20:09.000000 braintrust-0.0.2/src/braintrust/__init__.py
+-rw-r--r--   0 ankur      (501) staff       (20)      123 2023-05-14 19:33:59.000000 braintrust-0.0.2/src/braintrust/cache.py
+-rw-r--r--   0 ankur      (501) staff       (20)      811 2023-04-15 21:46:41.000000 braintrust-0.0.2/src/braintrust/oai.py
+-rw-r--r--   0 ankur      (501) staff       (20)       18 2023-05-24 03:34:51.000000 braintrust-0.0.2/src/braintrust/version.py
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-05-24 03:34:59.807577 braintrust-0.0.2/src/braintrust.egg-info/
+-rw-r--r--   0 ankur      (501) staff       (20)      494 2023-05-24 03:34:59.000000 braintrust-0.0.2/src/braintrust.egg-info/PKG-INFO
+-rw-r--r--   0 ankur      (501) staff       (20)      347 2023-05-24 03:34:59.000000 braintrust-0.0.2/src/braintrust.egg-info/SOURCES.txt
+-rw-r--r--   0 ankur      (501) staff       (20)        1 2023-05-24 03:34:59.000000 braintrust-0.0.2/src/braintrust.egg-info/dependency_links.txt
+-rw-r--r--   0 ankur      (501) staff       (20)       60 2023-05-24 03:34:59.000000 braintrust-0.0.2/src/braintrust.egg-info/entry_points.txt
+-rw-r--r--   0 ankur      (501) staff       (20)      196 2023-05-24 03:34:59.000000 braintrust-0.0.2/src/braintrust.egg-info/requires.txt
+-rw-r--r--   0 ankur      (501) staff       (20)       11 2023-05-24 03:34:59.000000 braintrust-0.0.2/src/braintrust.egg-info/top_level.txt
```

### Comparing `braintrust-0.0.1/setup.py` & `braintrust-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `braintrust-0.0.1/src/braintrust/__init__.py` & `braintrust-0.0.2/src/braintrust/__init__.py`

 * *Files identical despite different names*

### Comparing `braintrust-0.0.1/src/braintrust/oai.py` & `braintrust-0.0.2/src/braintrust/oai.py`

 * *Files identical despite different names*

