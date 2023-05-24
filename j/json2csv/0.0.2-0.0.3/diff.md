# Comparing `tmp/json2csv-0.0.2.tar.gz` & `tmp/json2csv-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json2csv-0.0.2.tar", last modified: Wed May 24 13:34:12 2023, max compression
+gzip compressed data, was "json2csv-0.0.3.tar", last modified: Wed May 24 13:58:38 2023, max compression
```

## Comparing `json2csv-0.0.2.tar` & `json2csv-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 agaba     (1000) agaba     (1000)        0 2023-05-24 13:34:12.839486 json2csv-0.0.2/
--rw-r--r--   0 agaba     (1000) agaba     (1000)      203 2023-05-24 13:34:12.839486 json2csv-0.0.2/PKG-INFO
--rw-r--r--   0 agaba     (1000) agaba     (1000)      790 2023-05-24 13:32:50.000000 json2csv-0.0.2/README.md
-drwxr-xr-x   0 agaba     (1000) agaba     (1000)        0 2023-05-24 13:34:12.839486 json2csv-0.0.2/json2csv/
--rw-r--r--   0 agaba     (1000) agaba     (1000)        0 2023-05-24 12:30:00.000000 json2csv-0.0.2/json2csv/__init__.py
--rw-r--r--   0 agaba     (1000) agaba     (1000)      950 2023-05-24 13:32:04.000000 json2csv-0.0.2/json2csv/json2csv.py
-drwxr-xr-x   0 agaba     (1000) agaba     (1000)        0 2023-05-24 13:34:12.839486 json2csv-0.0.2/json2csv.egg-info/
--rw-r--r--   0 agaba     (1000) agaba     (1000)      203 2023-05-24 13:34:12.000000 json2csv-0.0.2/json2csv.egg-info/PKG-INFO
--rw-r--r--   0 agaba     (1000) agaba     (1000)      188 2023-05-24 13:34:12.000000 json2csv-0.0.2/json2csv.egg-info/SOURCES.txt
--rw-r--r--   0 agaba     (1000) agaba     (1000)        1 2023-05-24 13:34:12.000000 json2csv-0.0.2/json2csv.egg-info/dependency_links.txt
--rw-r--r--   0 agaba     (1000) agaba     (1000)        9 2023-05-24 13:34:12.000000 json2csv-0.0.2/json2csv.egg-info/top_level.txt
--rw-r--r--   0 agaba     (1000) agaba     (1000)       38 2023-05-24 13:34:12.839486 json2csv-0.0.2/setup.cfg
--rw-r--r--   0 agaba     (1000) agaba     (1000)      321 2023-05-24 13:33:33.000000 json2csv-0.0.2/setup.py
+drwxr-xr-x   0 agaba     (1000) agaba     (1000)        0 2023-05-24 13:58:38.544009 json2csv-0.0.3/
+-rw-r--r--   0 agaba     (1000) agaba     (1000)      203 2023-05-24 13:58:38.544009 json2csv-0.0.3/PKG-INFO
+-rw-r--r--   0 agaba     (1000) agaba     (1000)      790 2023-05-24 13:32:50.000000 json2csv-0.0.3/README.md
+drwxr-xr-x   0 agaba     (1000) agaba     (1000)        0 2023-05-24 13:58:38.544009 json2csv-0.0.3/json2csv/
+-rw-r--r--   0 agaba     (1000) agaba     (1000)       29 2023-05-24 13:51:55.000000 json2csv-0.0.3/json2csv/__init__.py
+-rw-r--r--   0 agaba     (1000) agaba     (1000)      950 2023-05-24 13:32:04.000000 json2csv-0.0.3/json2csv/json2csv.py
+drwxr-xr-x   0 agaba     (1000) agaba     (1000)        0 2023-05-24 13:58:38.544009 json2csv-0.0.3/json2csv.egg-info/
+-rw-r--r--   0 agaba     (1000) agaba     (1000)      203 2023-05-24 13:58:38.000000 json2csv-0.0.3/json2csv.egg-info/PKG-INFO
+-rw-r--r--   0 agaba     (1000) agaba     (1000)      219 2023-05-24 13:58:38.000000 json2csv-0.0.3/json2csv.egg-info/SOURCES.txt
+-rw-r--r--   0 agaba     (1000) agaba     (1000)        1 2023-05-24 13:58:38.000000 json2csv-0.0.3/json2csv.egg-info/dependency_links.txt
+-rw-r--r--   0 agaba     (1000) agaba     (1000)        9 2023-05-24 13:58:38.000000 json2csv-0.0.3/json2csv.egg-info/requires.txt
+-rw-r--r--   0 agaba     (1000) agaba     (1000)        9 2023-05-24 13:58:38.000000 json2csv-0.0.3/json2csv.egg-info/top_level.txt
+-rw-r--r--   0 agaba     (1000) agaba     (1000)       38 2023-05-24 13:58:38.544009 json2csv-0.0.3/setup.cfg
+-rw-r--r--   0 agaba     (1000) agaba     (1000)      255 2023-05-24 13:56:46.000000 json2csv-0.0.3/setup.py
```

### Comparing `json2csv-0.0.2/README.md` & `json2csv-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `json2csv-0.0.2/json2csv/json2csv.py` & `json2csv-0.0.3/json2csv/json2csv.py`

 * *Files identical despite different names*

