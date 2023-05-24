# Comparing `tmp/json2csv-0.0.1.tar.gz` & `tmp/json2csv-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json2csv-0.0.1.tar", last modified: Wed May 24 12:53:21 2023, max compression
+gzip compressed data, was "json2csv-0.0.2.tar", last modified: Wed May 24 13:34:12 2023, max compression
```

## Comparing `json2csv-0.0.1.tar` & `json2csv-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 agaba     (1000) agaba     (1000)        0 2023-05-24 12:53:21.881709 json2csv-0.0.1/
--rw-r--r--   0 agaba     (1000) agaba     (1000)      203 2023-05-24 12:53:21.881709 json2csv-0.0.1/PKG-INFO
-drwxr-xr-x   0 agaba     (1000) agaba     (1000)        0 2023-05-24 12:53:21.881709 json2csv-0.0.1/json2csv/
--rw-r--r--   0 agaba     (1000) agaba     (1000)        0 2023-05-24 12:30:00.000000 json2csv-0.0.1/json2csv/__init__.py
--rw-r--r--   0 agaba     (1000) agaba     (1000)      906 2023-05-24 12:33:15.000000 json2csv-0.0.1/json2csv/json2csv.py
-drwxr-xr-x   0 agaba     (1000) agaba     (1000)        0 2023-05-24 12:53:21.881709 json2csv-0.0.1/json2csv.egg-info/
--rw-r--r--   0 agaba     (1000) agaba     (1000)      203 2023-05-24 12:53:21.000000 json2csv-0.0.1/json2csv.egg-info/PKG-INFO
--rw-r--r--   0 agaba     (1000) agaba     (1000)      178 2023-05-24 12:53:21.000000 json2csv-0.0.1/json2csv.egg-info/SOURCES.txt
--rw-r--r--   0 agaba     (1000) agaba     (1000)        1 2023-05-24 12:53:21.000000 json2csv-0.0.1/json2csv.egg-info/dependency_links.txt
--rw-r--r--   0 agaba     (1000) agaba     (1000)        9 2023-05-24 12:53:21.000000 json2csv-0.0.1/json2csv.egg-info/top_level.txt
--rw-r--r--   0 agaba     (1000) agaba     (1000)       38 2023-05-24 12:53:21.881709 json2csv-0.0.1/setup.cfg
--rw-r--r--   0 agaba     (1000) agaba     (1000)      321 2023-05-24 12:45:13.000000 json2csv-0.0.1/setup.py
+drwxr-xr-x   0 agaba     (1000) agaba     (1000)        0 2023-05-24 13:34:12.839486 json2csv-0.0.2/
+-rw-r--r--   0 agaba     (1000) agaba     (1000)      203 2023-05-24 13:34:12.839486 json2csv-0.0.2/PKG-INFO
+-rw-r--r--   0 agaba     (1000) agaba     (1000)      790 2023-05-24 13:32:50.000000 json2csv-0.0.2/README.md
+drwxr-xr-x   0 agaba     (1000) agaba     (1000)        0 2023-05-24 13:34:12.839486 json2csv-0.0.2/json2csv/
+-rw-r--r--   0 agaba     (1000) agaba     (1000)        0 2023-05-24 12:30:00.000000 json2csv-0.0.2/json2csv/__init__.py
+-rw-r--r--   0 agaba     (1000) agaba     (1000)      950 2023-05-24 13:32:04.000000 json2csv-0.0.2/json2csv/json2csv.py
+drwxr-xr-x   0 agaba     (1000) agaba     (1000)        0 2023-05-24 13:34:12.839486 json2csv-0.0.2/json2csv.egg-info/
+-rw-r--r--   0 agaba     (1000) agaba     (1000)      203 2023-05-24 13:34:12.000000 json2csv-0.0.2/json2csv.egg-info/PKG-INFO
+-rw-r--r--   0 agaba     (1000) agaba     (1000)      188 2023-05-24 13:34:12.000000 json2csv-0.0.2/json2csv.egg-info/SOURCES.txt
+-rw-r--r--   0 agaba     (1000) agaba     (1000)        1 2023-05-24 13:34:12.000000 json2csv-0.0.2/json2csv.egg-info/dependency_links.txt
+-rw-r--r--   0 agaba     (1000) agaba     (1000)        9 2023-05-24 13:34:12.000000 json2csv-0.0.2/json2csv.egg-info/top_level.txt
+-rw-r--r--   0 agaba     (1000) agaba     (1000)       38 2023-05-24 13:34:12.839486 json2csv-0.0.2/setup.cfg
+-rw-r--r--   0 agaba     (1000) agaba     (1000)      321 2023-05-24 13:33:33.000000 json2csv-0.0.2/setup.py
```

