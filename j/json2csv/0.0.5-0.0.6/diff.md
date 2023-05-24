# Comparing `tmp/json2csv-0.0.5.tar.gz` & `tmp/json2csv-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json2csv-0.0.5.tar", last modified: Wed May 24 14:29:31 2023, max compression
+gzip compressed data, was "json2csv-0.0.6.tar", last modified: Wed May 24 14:32:26 2023, max compression
```

## Comparing `json2csv-0.0.5.tar` & `json2csv-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxr-xr-x   0 agaba     (1000) agaba     (1000)        0 2023-05-24 14:29:31.214818 json2csv-0.0.5/
--rw-r--r--   0 agaba     (1000) agaba     (1000)      203 2023-05-24 14:29:31.214818 json2csv-0.0.5/PKG-INFO
--rw-r--r--   0 agaba     (1000) agaba     (1000)      790 2023-05-24 13:32:50.000000 json2csv-0.0.5/README.md
-drwxr-xr-x   0 agaba     (1000) agaba     (1000)        0 2023-05-24 14:29:31.214818 json2csv-0.0.5/json2csv/
--rw-r--r--   0 agaba     (1000) agaba     (1000)       30 2023-05-24 14:24:05.000000 json2csv-0.0.5/json2csv/__init__.py
--rw-r--r--   0 agaba     (1000) agaba     (1000)      950 2023-05-24 13:32:04.000000 json2csv-0.0.5/json2csv/json2csv.py
-drwxr-xr-x   0 agaba     (1000) agaba     (1000)        0 2023-05-24 14:29:31.214818 json2csv-0.0.5/json2csv.egg-info/
--rw-r--r--   0 agaba     (1000) agaba     (1000)      203 2023-05-24 14:29:31.000000 json2csv-0.0.5/json2csv.egg-info/PKG-INFO
--rw-r--r--   0 agaba     (1000) agaba     (1000)      219 2023-05-24 14:29:31.000000 json2csv-0.0.5/json2csv.egg-info/SOURCES.txt
--rw-r--r--   0 agaba     (1000) agaba     (1000)        1 2023-05-24 14:29:31.000000 json2csv-0.0.5/json2csv.egg-info/dependency_links.txt
--rw-r--r--   0 agaba     (1000) agaba     (1000)        5 2023-05-24 14:29:31.000000 json2csv-0.0.5/json2csv.egg-info/requires.txt
--rw-r--r--   0 agaba     (1000) agaba     (1000)        9 2023-05-24 14:29:31.000000 json2csv-0.0.5/json2csv.egg-info/top_level.txt
--rw-r--r--   0 agaba     (1000) agaba     (1000)       38 2023-05-24 14:29:31.214818 json2csv-0.0.5/setup.cfg
--rw-r--r--   0 agaba     (1000) agaba     (1000)      248 2023-05-24 14:26:35.000000 json2csv-0.0.5/setup.py
+drwxr-xr-x   0 agaba     (1000) agaba     (1000)        0 2023-05-24 14:32:26.889228 json2csv-0.0.6/
+-rw-r--r--   0 agaba     (1000) agaba     (1000)      203 2023-05-24 14:32:26.889228 json2csv-0.0.6/PKG-INFO
+-rw-r--r--   0 agaba     (1000) agaba     (1000)      790 2023-05-24 13:32:50.000000 json2csv-0.0.6/README.md
+drwxr-xr-x   0 agaba     (1000) agaba     (1000)        0 2023-05-24 14:32:26.889228 json2csv-0.0.6/json2csv/
+-rw-r--r--   0 agaba     (1000) agaba     (1000)       30 2023-05-24 14:24:05.000000 json2csv-0.0.6/json2csv/__init__.py
+-rw-r--r--   0 agaba     (1000) agaba     (1000)      950 2023-05-24 13:32:04.000000 json2csv-0.0.6/json2csv/json2csv.py
+drwxr-xr-x   0 agaba     (1000) agaba     (1000)        0 2023-05-24 14:32:26.889228 json2csv-0.0.6/json2csv.egg-info/
+-rw-r--r--   0 agaba     (1000) agaba     (1000)      203 2023-05-24 14:32:26.000000 json2csv-0.0.6/json2csv.egg-info/PKG-INFO
+-rw-r--r--   0 agaba     (1000) agaba     (1000)      188 2023-05-24 14:32:26.000000 json2csv-0.0.6/json2csv.egg-info/SOURCES.txt
+-rw-r--r--   0 agaba     (1000) agaba     (1000)        1 2023-05-24 14:32:26.000000 json2csv-0.0.6/json2csv.egg-info/dependency_links.txt
+-rw-r--r--   0 agaba     (1000) agaba     (1000)        9 2023-05-24 14:32:26.000000 json2csv-0.0.6/json2csv.egg-info/top_level.txt
+-rw-r--r--   0 agaba     (1000) agaba     (1000)       38 2023-05-24 14:32:26.889228 json2csv-0.0.6/setup.cfg
+-rw-r--r--   0 agaba     (1000) agaba     (1000)      242 2023-05-24 14:31:57.000000 json2csv-0.0.6/setup.py
```

### Comparing `json2csv-0.0.5/README.md` & `json2csv-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `json2csv-0.0.5/json2csv/json2csv.py` & `json2csv-0.0.6/json2csv/json2csv.py`

 * *Files identical despite different names*

