# Comparing `tmp/eobi-1.1.2.tar.gz` & `tmp/eobi-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eobi-1.1.2.tar", last modified: Wed May 24 08:59:20 2023, max compression
+gzip compressed data, was "eobi-1.1.4.tar", last modified: Wed May 24 11:17:03 2023, max compression
```

## Comparing `eobi-1.1.2.tar` & `eobi-1.1.4.tar`

### file list

```diff
@@ -1,32 +1,30 @@
-drwxr-xr-x   0 ebukaobi   (501) staff       (20)        0 2023-05-24 08:59:20.223446 eobi-1.1.2/
--rw-r--r--   0 ebukaobi   (501) staff       (20)      415 2023-05-24 08:59:20.223189 eobi-1.1.2/PKG-INFO
--rw-r--r--   0 ebukaobi   (501) staff       (20)       15 2023-05-03 08:46:26.000000 eobi-1.1.2/README.md
-drwxr-xr-x   0 ebukaobi   (501) staff       (20)        0 2023-05-24 08:59:20.218504 eobi-1.1.2/autogon_ml/
--rw-r--r--   0 ebukaobi   (501) staff       (20)        0 2023-05-03 08:46:26.000000 eobi-1.1.2/autogon_ml/__init__.py
-drwxr-xr-x   0 ebukaobi   (501) staff       (20)        0 2023-05-24 08:59:20.218943 eobi-1.1.2/autogon_ml/autoClassification/
--rw-r--r--   0 ebukaobi   (501) staff       (20)        0 2023-05-03 08:46:26.000000 eobi-1.1.2/autogon_ml/autoClassification/__init__.py
--rw-r--r--   0 ebukaobi   (501) staff       (20)     3987 2023-05-03 08:46:26.000000 eobi-1.1.2/autogon_ml/autoClassification/base.py
-drwxr-xr-x   0 ebukaobi   (501) staff       (20)        0 2023-05-24 08:59:20.219344 eobi-1.1.2/autogon_ml/autoFeatureEngineering/
--rw-r--r--   0 ebukaobi   (501) staff       (20)        0 2023-05-03 08:46:26.000000 eobi-1.1.2/autogon_ml/autoFeatureEngineering/__init__.py
--rw-r--r--   0 ebukaobi   (501) staff       (20)    17276 2023-05-04 07:15:17.000000 eobi-1.1.2/autogon_ml/autoFeatureEngineering/base.py
-drwxr-xr-x   0 ebukaobi   (501) staff       (20)        0 2023-05-24 08:59:20.219967 eobi-1.1.2/autogon_ml/autoRegression/
--rw-r--r--   0 ebukaobi   (501) staff       (20)        0 2023-05-03 08:46:26.000000 eobi-1.1.2/autogon_ml/autoRegression/__init__.py
--rw-r--r--   0 ebukaobi   (501) staff       (20)     2809 2023-05-03 08:46:26.000000 eobi-1.1.2/autogon_ml/autoRegression/base.py
-drwxr-xr-x   0 ebukaobi   (501) staff       (20)        0 2023-05-24 08:59:20.220224 eobi-1.1.2/autogon_ml/auto_data_preprocessing/
-drwxr-xr-x   0 ebukaobi   (501) staff       (20)        0 2023-05-24 08:59:20.220984 eobi-1.1.2/autogon_ml/auto_data_preprocessing/AutoClean/
--rw-r--r--   0 ebukaobi   (501) staff       (20)       41 2023-05-07 18:50:08.000000 eobi-1.1.2/autogon_ml/auto_data_preprocessing/AutoClean/__init__.py
--rw-r--r--   0 ebukaobi   (501) staff       (20)     9245 2023-05-24 08:46:20.000000 eobi-1.1.2/autogon_ml/auto_data_preprocessing/AutoClean/autoclean.py
--rw-r--r--   0 ebukaobi   (501) staff       (20)    27739 2023-05-07 18:50:08.000000 eobi-1.1.2/autogon_ml/auto_data_preprocessing/AutoClean/modules.py
--rw-r--r--   0 ebukaobi   (501) staff       (20)        0 2023-05-07 19:50:13.000000 eobi-1.1.2/autogon_ml/auto_data_preprocessing/__init__.py
-drwxr-xr-x   0 ebukaobi   (501) staff       (20)        0 2023-05-24 08:59:20.221702 eobi-1.1.2/autogon_ml/auto_data_preprocessing/feature_engineering/
--rw-r--r--   0 ebukaobi   (501) staff       (20)        0 2023-05-07 18:50:08.000000 eobi-1.1.2/autogon_ml/auto_data_preprocessing/feature_engineering/__init__.py
--rw-r--r--   0 ebukaobi   (501) staff       (20)    26597 2023-05-24 08:49:54.000000 eobi-1.1.2/autogon_ml/auto_data_preprocessing/feature_engineering/base.py
--rw-r--r--   0 ebukaobi   (501) staff       (20)      614 2023-05-24 08:54:26.000000 eobi-1.1.2/autogon_ml/test.py
-drwxr-xr-x   0 ebukaobi   (501) staff       (20)        0 2023-05-24 08:59:20.222916 eobi-1.1.2/eobi.egg-info/
--rw-r--r--   0 ebukaobi   (501) staff       (20)      415 2023-05-24 08:59:20.000000 eobi-1.1.2/eobi.egg-info/PKG-INFO
--rw-r--r--   0 ebukaobi   (501) staff       (20)      787 2023-05-24 08:59:20.000000 eobi-1.1.2/eobi.egg-info/SOURCES.txt
--rw-r--r--   0 ebukaobi   (501) staff       (20)        1 2023-05-24 08:59:20.000000 eobi-1.1.2/eobi.egg-info/dependency_links.txt
--rw-r--r--   0 ebukaobi   (501) staff       (20)      234 2023-05-24 08:59:20.000000 eobi-1.1.2/eobi.egg-info/requires.txt
--rw-r--r--   0 ebukaobi   (501) staff       (20)       11 2023-05-24 08:59:20.000000 eobi-1.1.2/eobi.egg-info/top_level.txt
--rw-r--r--   0 ebukaobi   (501) staff       (20)       38 2023-05-24 08:59:20.223516 eobi-1.1.2/setup.cfg
--rw-r--r--   0 ebukaobi   (501) staff       (20)     1182 2023-05-24 08:56:25.000000 eobi-1.1.2/setup.py
+drwxr-xr-x   0 ebukaobi   (501) staff       (20)        0 2023-05-24 11:17:03.759472 eobi-1.1.4/
+-rw-r--r--   0 ebukaobi   (501) staff       (20)      415 2023-05-24 11:17:03.759293 eobi-1.1.4/PKG-INFO
+-rw-r--r--   0 ebukaobi   (501) staff       (20)       15 2023-05-03 08:46:26.000000 eobi-1.1.4/README.md
+drwxr-xr-x   0 ebukaobi   (501) staff       (20)        0 2023-05-24 11:17:03.755783 eobi-1.1.4/autogon_ml/
+-rw-r--r--   0 ebukaobi   (501) staff       (20)        0 2023-05-03 08:46:26.000000 eobi-1.1.4/autogon_ml/__init__.py
+drwxr-xr-x   0 ebukaobi   (501) staff       (20)        0 2023-05-24 11:17:03.756270 eobi-1.1.4/autogon_ml/autoClassification/
+-rw-r--r--   0 ebukaobi   (501) staff       (20)        0 2023-05-03 08:46:26.000000 eobi-1.1.4/autogon_ml/autoClassification/__init__.py
+-rw-r--r--   0 ebukaobi   (501) staff       (20)     3987 2023-05-03 08:46:26.000000 eobi-1.1.4/autogon_ml/autoClassification/base.py
+drwxr-xr-x   0 ebukaobi   (501) staff       (20)        0 2023-05-24 11:17:03.756661 eobi-1.1.4/autogon_ml/autoRegression/
+-rw-r--r--   0 ebukaobi   (501) staff       (20)        0 2023-05-03 08:46:26.000000 eobi-1.1.4/autogon_ml/autoRegression/__init__.py
+-rw-r--r--   0 ebukaobi   (501) staff       (20)     2809 2023-05-03 08:46:26.000000 eobi-1.1.4/autogon_ml/autoRegression/base.py
+drwxr-xr-x   0 ebukaobi   (501) staff       (20)        0 2023-05-24 11:17:03.756887 eobi-1.1.4/autogon_ml/auto_data_preprocessing/
+drwxr-xr-x   0 ebukaobi   (501) staff       (20)        0 2023-05-24 11:17:03.757516 eobi-1.1.4/autogon_ml/auto_data_preprocessing/AutoClean/
+-rw-r--r--   0 ebukaobi   (501) staff       (20)       41 2023-05-07 18:50:08.000000 eobi-1.1.4/autogon_ml/auto_data_preprocessing/AutoClean/__init__.py
+-rw-r--r--   0 ebukaobi   (501) staff       (20)     9245 2023-05-24 08:46:20.000000 eobi-1.1.4/autogon_ml/auto_data_preprocessing/AutoClean/autoclean.py
+-rw-r--r--   0 ebukaobi   (501) staff       (20)    27739 2023-05-07 18:50:08.000000 eobi-1.1.4/autogon_ml/auto_data_preprocessing/AutoClean/modules.py
+-rw-r--r--   0 ebukaobi   (501) staff       (20)        0 2023-05-07 19:50:13.000000 eobi-1.1.4/autogon_ml/auto_data_preprocessing/__init__.py
+drwxr-xr-x   0 ebukaobi   (501) staff       (20)        0 2023-05-24 11:17:03.758388 eobi-1.1.4/autogon_ml/auto_data_preprocessing/feature_engineering/
+-rw-r--r--   0 ebukaobi   (501) staff       (20)        0 2023-05-07 18:50:08.000000 eobi-1.1.4/autogon_ml/auto_data_preprocessing/feature_engineering/__init__.py
+-rw-r--r--   0 ebukaobi   (501) staff       (20)    26597 2023-05-24 10:20:53.000000 eobi-1.1.4/autogon_ml/auto_data_preprocessing/feature_engineering/base.py
+-rw-r--r--   0 ebukaobi   (501) staff       (20)     3967 2023-05-24 10:13:46.000000 eobi-1.1.4/autogon_ml/auto_data_preprocessing/feature_engineering/util.py
+-rw-r--r--   0 ebukaobi   (501) staff       (20)      898 2023-05-24 10:22:27.000000 eobi-1.1.4/autogon_ml/test.py
+drwxr-xr-x   0 ebukaobi   (501) staff       (20)        0 2023-05-24 11:17:03.759112 eobi-1.1.4/eobi.egg-info/
+-rw-r--r--   0 ebukaobi   (501) staff       (20)      415 2023-05-24 11:17:03.000000 eobi-1.1.4/eobi.egg-info/PKG-INFO
+-rw-r--r--   0 ebukaobi   (501) staff       (20)      762 2023-05-24 11:17:03.000000 eobi-1.1.4/eobi.egg-info/SOURCES.txt
+-rw-r--r--   0 ebukaobi   (501) staff       (20)        1 2023-05-24 11:17:03.000000 eobi-1.1.4/eobi.egg-info/dependency_links.txt
+-rw-r--r--   0 ebukaobi   (501) staff       (20)      234 2023-05-24 11:17:03.000000 eobi-1.1.4/eobi.egg-info/requires.txt
+-rw-r--r--   0 ebukaobi   (501) staff       (20)       11 2023-05-24 11:17:03.000000 eobi-1.1.4/eobi.egg-info/top_level.txt
+-rw-r--r--   0 ebukaobi   (501) staff       (20)       38 2023-05-24 11:17:03.759510 eobi-1.1.4/setup.cfg
+-rw-r--r--   0 ebukaobi   (501) staff       (20)     1182 2023-05-24 11:15:56.000000 eobi-1.1.4/setup.py
```

### Comparing `eobi-1.1.2/autogon_ml/autoClassification/base.py` & `eobi-1.1.4/autogon_ml/autoClassification/base.py`

 * *Files identical despite different names*

### Comparing `eobi-1.1.2/autogon_ml/autoRegression/base.py` & `eobi-1.1.4/autogon_ml/autoRegression/base.py`

 * *Files identical despite different names*

### Comparing `eobi-1.1.2/autogon_ml/auto_data_preprocessing/AutoClean/autoclean.py` & `eobi-1.1.4/autogon_ml/auto_data_preprocessing/AutoClean/autoclean.py`

 * *Files identical despite different names*

### Comparing `eobi-1.1.2/autogon_ml/auto_data_preprocessing/AutoClean/modules.py` & `eobi-1.1.4/autogon_ml/auto_data_preprocessing/AutoClean/modules.py`

 * *Files identical despite different names*

### Comparing `eobi-1.1.2/autogon_ml/auto_data_preprocessing/feature_engineering/base.py` & `eobi-1.1.4/autogon_ml/auto_data_preprocessing/feature_engineering/base.py`

 * *Files identical despite different names*

### Comparing `eobi-1.1.2/eobi.egg-info/SOURCES.txt` & `eobi-1.1.4/eobi.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 README.md
 setup.py
 autogon_ml/__init__.py
 autogon_ml/test.py
 autogon_ml/autoClassification/__init__.py
 autogon_ml/autoClassification/base.py
-autogon_ml/autoFeatureEngineering/__init__.py
-autogon_ml/autoFeatureEngineering/base.py
 autogon_ml/autoRegression/__init__.py
 autogon_ml/autoRegression/base.py
 autogon_ml/auto_data_preprocessing/__init__.py
 autogon_ml/auto_data_preprocessing/AutoClean/__init__.py
 autogon_ml/auto_data_preprocessing/AutoClean/autoclean.py
 autogon_ml/auto_data_preprocessing/AutoClean/modules.py
 autogon_ml/auto_data_preprocessing/feature_engineering/__init__.py
 autogon_ml/auto_data_preprocessing/feature_engineering/base.py
+autogon_ml/auto_data_preprocessing/feature_engineering/util.py
 eobi.egg-info/PKG-INFO
 eobi.egg-info/SOURCES.txt
 eobi.egg-info/dependency_links.txt
 eobi.egg-info/requires.txt
 eobi.egg-info/top_level.txt
```

### Comparing `eobi-1.1.2/setup.py` & `eobi-1.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_packages
 
 setup(
     name='eobi',
-    version='1.1.2',
+    version='1.1.4',
     description='...',
     author='Autogon Inc',
     author_email='developer@autogon.ai',
     packages=find_packages(),
     install_requires=[
             'catboost',
             'contourpy',
```

