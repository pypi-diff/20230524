# Comparing `tmp/eobi-1.0.0.tar.gz` & `tmp/eobi-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eobi-1.0.0.tar", last modified: Wed May  3 07:53:15 2023, max compression
+gzip compressed data, was "eobi-1.1.0.tar", last modified: Wed May  3 08:20:39 2023, max compression
```

## Comparing `eobi-1.0.0.tar` & `eobi-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 ebukaobi   (501) staff       (20)        0 2023-05-03 07:53:15.168830 eobi-1.0.0/
--rw-r--r--   0 ebukaobi   (501) staff       (20)      415 2023-05-03 07:53:15.168665 eobi-1.0.0/PKG-INFO
-drwxr-xr-x   0 ebukaobi   (501) staff       (20)        0 2023-05-03 07:53:15.166231 eobi-1.0.0/autogon_ml/
--rw-r--r--   0 ebukaobi   (501) staff       (20)        0 2023-05-03 00:26:31.000000 eobi-1.0.0/autogon_ml/__init__.py
-drwxr-xr-x   0 ebukaobi   (501) staff       (20)        0 2023-05-03 07:53:15.166430 eobi-1.0.0/autogon_ml/autoClassification/
--rw-r--r--   0 ebukaobi   (501) staff       (20)        0 2023-05-03 00:46:55.000000 eobi-1.0.0/autogon_ml/autoClassification/__init__.py
--rw-r--r--   0 ebukaobi   (501) staff       (20)     3987 2023-05-01 01:21:50.000000 eobi-1.0.0/autogon_ml/autoClassification/base.py
-drwxr-xr-x   0 ebukaobi   (501) staff       (20)        0 2023-05-03 07:53:15.166921 eobi-1.0.0/autogon_ml/autoFeatureEngineering/
--rw-r--r--   0 ebukaobi   (501) staff       (20)        0 2023-05-03 00:47:22.000000 eobi-1.0.0/autogon_ml/autoFeatureEngineering/__init__.py
--rw-r--r--   0 ebukaobi   (501) staff       (20)    17242 2023-05-01 01:30:22.000000 eobi-1.0.0/autogon_ml/autoFeatureEngineering/base.py
-drwxr-xr-x   0 ebukaobi   (501) staff       (20)        0 2023-05-03 07:53:15.167614 eobi-1.0.0/autogon_ml/autoRegression/
--rw-r--r--   0 ebukaobi   (501) staff       (20)        0 2023-05-03 00:47:06.000000 eobi-1.0.0/autogon_ml/autoRegression/__init__.py
--rw-r--r--   0 ebukaobi   (501) staff       (20)     2809 2023-05-03 00:48:03.000000 eobi-1.0.0/autogon_ml/autoRegression/base.py
-drwxr-xr-x   0 ebukaobi   (501) staff       (20)        0 2023-05-03 07:53:15.168494 eobi-1.0.0/eobi.egg-info/
--rw-r--r--   0 ebukaobi   (501) staff       (20)      415 2023-05-03 07:53:15.000000 eobi-1.0.0/eobi.egg-info/PKG-INFO
--rw-r--r--   0 ebukaobi   (501) staff       (20)      410 2023-05-03 07:53:15.000000 eobi-1.0.0/eobi.egg-info/SOURCES.txt
--rw-r--r--   0 ebukaobi   (501) staff       (20)        1 2023-05-03 07:53:15.000000 eobi-1.0.0/eobi.egg-info/dependency_links.txt
--rw-r--r--   0 ebukaobi   (501) staff       (20)      388 2023-05-03 07:53:15.000000 eobi-1.0.0/eobi.egg-info/requires.txt
--rw-r--r--   0 ebukaobi   (501) staff       (20)       11 2023-05-03 07:53:15.000000 eobi-1.0.0/eobi.egg-info/top_level.txt
--rw-r--r--   0 ebukaobi   (501) staff       (20)       38 2023-05-03 07:53:15.168870 eobi-1.0.0/setup.cfg
--rw-r--r--   0 ebukaobi   (501) staff       (20)     1307 2023-05-03 07:50:07.000000 eobi-1.0.0/setup.py
+drwxr-xr-x   0 ebukaobi   (501) staff       (20)        0 2023-05-03 08:20:39.685567 eobi-1.1.0/
+-rw-r--r--   0 ebukaobi   (501) staff       (20)      415 2023-05-03 08:20:39.685390 eobi-1.1.0/PKG-INFO
+drwxr-xr-x   0 ebukaobi   (501) staff       (20)        0 2023-05-03 08:20:39.682803 eobi-1.1.0/autogon_ml/
+-rw-r--r--   0 ebukaobi   (501) staff       (20)        0 2023-05-03 00:26:31.000000 eobi-1.1.0/autogon_ml/__init__.py
+drwxr-xr-x   0 ebukaobi   (501) staff       (20)        0 2023-05-03 08:20:39.683011 eobi-1.1.0/autogon_ml/autoClassification/
+-rw-r--r--   0 ebukaobi   (501) staff       (20)        0 2023-05-03 00:46:55.000000 eobi-1.1.0/autogon_ml/autoClassification/__init__.py
+-rw-r--r--   0 ebukaobi   (501) staff       (20)     3987 2023-05-01 01:21:50.000000 eobi-1.1.0/autogon_ml/autoClassification/base.py
+drwxr-xr-x   0 ebukaobi   (501) staff       (20)        0 2023-05-03 08:20:39.683526 eobi-1.1.0/autogon_ml/autoFeatureEngineering/
+-rw-r--r--   0 ebukaobi   (501) staff       (20)        0 2023-05-03 00:47:22.000000 eobi-1.1.0/autogon_ml/autoFeatureEngineering/__init__.py
+-rw-r--r--   0 ebukaobi   (501) staff       (20)    17242 2023-05-01 01:30:22.000000 eobi-1.1.0/autogon_ml/autoFeatureEngineering/base.py
+drwxr-xr-x   0 ebukaobi   (501) staff       (20)        0 2023-05-03 08:20:39.684248 eobi-1.1.0/autogon_ml/autoRegression/
+-rw-r--r--   0 ebukaobi   (501) staff       (20)        0 2023-05-03 00:47:06.000000 eobi-1.1.0/autogon_ml/autoRegression/__init__.py
+-rw-r--r--   0 ebukaobi   (501) staff       (20)     2809 2023-05-03 00:48:03.000000 eobi-1.1.0/autogon_ml/autoRegression/base.py
+drwxr-xr-x   0 ebukaobi   (501) staff       (20)        0 2023-05-03 08:20:39.685207 eobi-1.1.0/eobi.egg-info/
+-rw-r--r--   0 ebukaobi   (501) staff       (20)      415 2023-05-03 08:20:39.000000 eobi-1.1.0/eobi.egg-info/PKG-INFO
+-rw-r--r--   0 ebukaobi   (501) staff       (20)      410 2023-05-03 08:20:39.000000 eobi-1.1.0/eobi.egg-info/SOURCES.txt
+-rw-r--r--   0 ebukaobi   (501) staff       (20)        1 2023-05-03 08:20:39.000000 eobi-1.1.0/eobi.egg-info/dependency_links.txt
+-rw-r--r--   0 ebukaobi   (501) staff       (20)      212 2023-05-03 08:20:39.000000 eobi-1.1.0/eobi.egg-info/requires.txt
+-rw-r--r--   0 ebukaobi   (501) staff       (20)       11 2023-05-03 08:20:39.000000 eobi-1.1.0/eobi.egg-info/top_level.txt
+-rw-r--r--   0 ebukaobi   (501) staff       (20)       38 2023-05-03 08:20:39.685606 eobi-1.1.0/setup.cfg
+-rw-r--r--   0 ebukaobi   (501) staff       (20)     1131 2023-05-03 08:20:36.000000 eobi-1.1.0/setup.py
```

### Comparing `eobi-1.0.0/autogon_ml/autoClassification/base.py` & `eobi-1.1.0/autogon_ml/autoClassification/base.py`

 * *Files identical despite different names*

### Comparing `eobi-1.0.0/autogon_ml/autoFeatureEngineering/base.py` & `eobi-1.1.0/autogon_ml/autoFeatureEngineering/base.py`

 * *Files identical despite different names*

### Comparing `eobi-1.0.0/autogon_ml/autoRegression/base.py` & `eobi-1.1.0/autogon_ml/autoRegression/base.py`

 * *Files identical despite different names*

