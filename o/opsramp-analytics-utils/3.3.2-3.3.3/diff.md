# Comparing `tmp/opsramp-analytics-utils-3.3.2.tar.gz` & `tmp/opsramp-analytics-utils-3.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opsramp-analytics-utils-3.3.2.tar", last modified: Mon May 15 10:44:18 2023, max compression
+gzip compressed data, was "opsramp-analytics-utils-3.3.3.tar", last modified: Wed May 24 07:22:04 2023, max compression
```

## Comparing `opsramp-analytics-utils-3.3.2.tar` & `opsramp-analytics-utils-3.3.3.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxr-x   0 rajumummidi  (1001) rajumummidi  (1001)        0 2023-05-15 10:44:18.120164 opsramp-analytics-utils-3.3.2/
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     1073 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.2/LICENSE
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      186 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.2/MANIFEST.in
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     1361 2023-05-15 10:44:18.120164 opsramp-analytics-utils-3.3.2/PKG-INFO
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      711 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.2/README.md
-drwxrwxr-x   0 rajumummidi  (1001) rajumummidi  (1001)        0 2023-05-15 10:44:17.700126 opsramp-analytics-utils-3.3.2/analytics_sdk/
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)       30 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.2/analytics_sdk/__init__.py
-drwxrwxr-x   0 rajumummidi  (1001) rajumummidi  (1001)        0 2023-05-15 10:44:17.868141 opsramp-analytics-utils-3.3.2/analytics_sdk/analysis-wrapper/
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      921 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.2/analytics_sdk/analysis-wrapper/main.js
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)  3321723 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.2/analytics_sdk/analysis-wrapper/main.wrapper.css
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)  2628164 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.2/analytics_sdk/analysis-wrapper/main.wrapper.js
-drwxrwxr-x   0 rajumummidi  (1001) rajumummidi  (1001)        0 2023-05-15 10:44:18.088161 opsramp-analytics-utils-3.3.2/analytics_sdk/analysis-wrapper/media/
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      320 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.2/analytics_sdk/analysis-wrapper/media/close.82b1ae2d.svg
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    34172 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.2/analytics_sdk/analysis-wrapper/media/fontello.487f60cd.woff
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)   148200 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.2/analytics_sdk/analysis-wrapper/media/fontello.52a41d35.svg
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    64440 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.2/analytics_sdk/analysis-wrapper/media/fontello.8be26641.ttf
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    29136 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.2/analytics_sdk/analysis-wrapper/media/fontello.8fcd07de.woff2
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    64608 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.2/analytics_sdk/analysis-wrapper/media/fontello.d35868c4.eot
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      602 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.2/analytics_sdk/analysis-wrapper/media/icon-copy.c16adda9.svg
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      861 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.2/analytics_sdk/analysis-wrapper/media/icon-edit.ae3b1e05.svg
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     1403 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.2/analytics_sdk/analysis-wrapper/media/icon-remove.184d1ffb.svg
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     7536 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.2/analytics_sdk/analysis-wrapper/media/revicons.04eb8fc5.woff
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    11968 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.2/analytics_sdk/analysis-wrapper/media/revicons.17629a5d.ttf
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    12136 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.2/analytics_sdk/analysis-wrapper/media/revicons.2feb69cc.eot
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      733 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.2/analytics_sdk/analysis-wrapper/media/transparent-bg.5f803547.svg
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     4129 2022-07-11 05:34:48.000000 opsramp-analytics-utils-3.3.2/analytics_sdk/components.py
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)       38 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.2/analytics_sdk/constants.py
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    10055 2023-01-25 12:47:16.000000 opsramp-analytics-utils-3.3.2/analytics_sdk/oap_dash.py
-drwxrwxr-x   0 rajumummidi  (1001) rajumummidi  (1001)        0 2023-05-15 10:44:18.108162 opsramp-analytics-utils-3.3.2/analytics_sdk/process/
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)        0 2022-07-27 14:35:38.000000 opsramp-analytics-utils-3.3.2/analytics_sdk/process/__init__.py
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     5809 2023-04-10 11:19:33.000000 opsramp-analytics-utils-3.3.2/analytics_sdk/process/process.py
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     3287 2022-09-28 12:26:39.000000 opsramp-analytics-utils-3.3.2/analytics_sdk/process/querybuilder.py
-drwxrwxr-x   0 rajumummidi  (1001) rajumummidi  (1001)        0 2023-05-15 10:44:18.112163 opsramp-analytics-utils-3.3.2/analytics_sdk/renderer/
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)        0 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.2/analytics_sdk/renderer/__init__.py
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    31171 2023-05-15 10:20:48.000000 opsramp-analytics-utils-3.3.2/analytics_sdk/renderer/excel.py
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     2887 2022-10-28 05:58:48.000000 opsramp-analytics-utils-3.3.2/analytics_sdk/renderer/pdf.py
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    40307 2023-05-15 10:31:47.000000 opsramp-analytics-utils-3.3.2/analytics_sdk/utilities.py
-drwxrwxr-x   0 rajumummidi  (1001) rajumummidi  (1001)        0 2023-05-15 10:44:18.120164 opsramp-analytics-utils-3.3.2/opsramp_analytics_utils.egg-info/
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     1361 2023-05-15 10:44:17.000000 opsramp-analytics-utils-3.3.2/opsramp_analytics_utils.egg-info/PKG-INFO
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     1542 2023-05-15 10:44:17.000000 opsramp-analytics-utils-3.3.2/opsramp_analytics_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)        1 2023-05-15 10:44:17.000000 opsramp-analytics-utils-3.3.2/opsramp_analytics_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      108 2023-05-15 10:44:17.000000 opsramp-analytics-utils-3.3.2/opsramp_analytics_utils.egg-info/requires.txt
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)       14 2023-05-15 10:44:17.000000 opsramp-analytics-utils-3.3.2/opsramp_analytics_utils.egg-info/top_level.txt
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      108 2023-04-03 11:09:31.000000 opsramp-analytics-utils-3.3.2/requires-install.txt
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)       38 2023-05-15 10:44:18.120164 opsramp-analytics-utils-3.3.2/setup.cfg
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      941 2023-05-15 10:41:37.000000 opsramp-analytics-utils-3.3.2/setup.py
+drwxrwxr-x   0 rajumummidi  (1001) rajumummidi  (1001)        0 2023-05-24 07:22:04.320447 opsramp-analytics-utils-3.3.3/
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     1073 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.3/LICENSE
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      186 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.3/MANIFEST.in
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     1361 2023-05-24 07:22:04.320447 opsramp-analytics-utils-3.3.3/PKG-INFO
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      711 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.3/README.md
+drwxrwxr-x   0 rajumummidi  (1001) rajumummidi  (1001)        0 2023-05-24 07:22:03.932376 opsramp-analytics-utils-3.3.3/analytics_sdk/
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)       30 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.3/analytics_sdk/__init__.py
+drwxrwxr-x   0 rajumummidi  (1001) rajumummidi  (1001)        0 2023-05-24 07:22:04.092405 opsramp-analytics-utils-3.3.3/analytics_sdk/analysis-wrapper/
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      921 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.3/analytics_sdk/analysis-wrapper/main.js
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)  3321723 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.3/analytics_sdk/analysis-wrapper/main.wrapper.css
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)  2628164 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.3/analytics_sdk/analysis-wrapper/main.wrapper.js
+drwxrwxr-x   0 rajumummidi  (1001) rajumummidi  (1001)        0 2023-05-24 07:22:04.280439 opsramp-analytics-utils-3.3.3/analytics_sdk/analysis-wrapper/media/
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      320 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.3/analytics_sdk/analysis-wrapper/media/close.82b1ae2d.svg
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    34172 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.3/analytics_sdk/analysis-wrapper/media/fontello.487f60cd.woff
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)   148200 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.3/analytics_sdk/analysis-wrapper/media/fontello.52a41d35.svg
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    64440 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.3/analytics_sdk/analysis-wrapper/media/fontello.8be26641.ttf
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    29136 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.3/analytics_sdk/analysis-wrapper/media/fontello.8fcd07de.woff2
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    64608 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.3/analytics_sdk/analysis-wrapper/media/fontello.d35868c4.eot
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      602 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.3/analytics_sdk/analysis-wrapper/media/icon-copy.c16adda9.svg
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      861 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.3/analytics_sdk/analysis-wrapper/media/icon-edit.ae3b1e05.svg
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     1403 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.3/analytics_sdk/analysis-wrapper/media/icon-remove.184d1ffb.svg
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     7536 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.3/analytics_sdk/analysis-wrapper/media/revicons.04eb8fc5.woff
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    11968 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.3/analytics_sdk/analysis-wrapper/media/revicons.17629a5d.ttf
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    12136 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.3/analytics_sdk/analysis-wrapper/media/revicons.2feb69cc.eot
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      733 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.3/analytics_sdk/analysis-wrapper/media/transparent-bg.5f803547.svg
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     4129 2022-07-11 05:34:48.000000 opsramp-analytics-utils-3.3.3/analytics_sdk/components.py
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)       38 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.3/analytics_sdk/constants.py
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    10055 2023-01-25 12:47:16.000000 opsramp-analytics-utils-3.3.3/analytics_sdk/oap_dash.py
+drwxrwxr-x   0 rajumummidi  (1001) rajumummidi  (1001)        0 2023-05-24 07:22:04.300443 opsramp-analytics-utils-3.3.3/analytics_sdk/process/
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)        0 2022-07-27 14:35:38.000000 opsramp-analytics-utils-3.3.3/analytics_sdk/process/__init__.py
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     5809 2023-04-10 11:19:33.000000 opsramp-analytics-utils-3.3.3/analytics_sdk/process/process.py
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     3287 2022-09-28 12:26:39.000000 opsramp-analytics-utils-3.3.3/analytics_sdk/process/querybuilder.py
+drwxrwxr-x   0 rajumummidi  (1001) rajumummidi  (1001)        0 2023-05-24 07:22:04.312445 opsramp-analytics-utils-3.3.3/analytics_sdk/renderer/
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)        0 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.3/analytics_sdk/renderer/__init__.py
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    32062 2023-05-23 12:05:54.000000 opsramp-analytics-utils-3.3.3/analytics_sdk/renderer/excel.py
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     2887 2022-10-28 05:58:48.000000 opsramp-analytics-utils-3.3.3/analytics_sdk/renderer/pdf.py
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    40307 2023-05-15 10:31:47.000000 opsramp-analytics-utils-3.3.3/analytics_sdk/utilities.py
+drwxrwxr-x   0 rajumummidi  (1001) rajumummidi  (1001)        0 2023-05-24 07:22:04.320447 opsramp-analytics-utils-3.3.3/opsramp_analytics_utils.egg-info/
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     1361 2023-05-24 07:22:03.000000 opsramp-analytics-utils-3.3.3/opsramp_analytics_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     1542 2023-05-24 07:22:03.000000 opsramp-analytics-utils-3.3.3/opsramp_analytics_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)        1 2023-05-24 07:22:03.000000 opsramp-analytics-utils-3.3.3/opsramp_analytics_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      108 2023-05-24 07:22:03.000000 opsramp-analytics-utils-3.3.3/opsramp_analytics_utils.egg-info/requires.txt
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)       14 2023-05-24 07:22:03.000000 opsramp-analytics-utils-3.3.3/opsramp_analytics_utils.egg-info/top_level.txt
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      108 2023-04-03 11:09:31.000000 opsramp-analytics-utils-3.3.3/requires-install.txt
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)       38 2023-05-24 07:22:04.320447 opsramp-analytics-utils-3.3.3/setup.cfg
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      941 2023-05-23 12:12:30.000000 opsramp-analytics-utils-3.3.3/setup.py
```

### Comparing `opsramp-analytics-utils-3.3.2/LICENSE` & `opsramp-analytics-utils-3.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.2/PKG-INFO` & `opsramp-analytics-utils-3.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opsramp-analytics-utils
-Version: 3.3.2
+Version: 3.3.3
 Summary: OpsRamp Analytics SDK
 Home-page: https://github.com/opsramp/analytics-sdk
 Author: OpsRamp
 Author-email: opsramp@support.com
 License: UNKNOWN
 Description: ## OpsRamp Analytics Utilities
```

### Comparing `opsramp-analytics-utils-3.3.2/README.md` & `opsramp-analytics-utils-3.3.3/README.md`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.2/analytics_sdk/analysis-wrapper/main.js` & `opsramp-analytics-utils-3.3.3/analytics_sdk/analysis-wrapper/main.js`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.2/analytics_sdk/analysis-wrapper/main.wrapper.css` & `opsramp-analytics-utils-3.3.3/analytics_sdk/analysis-wrapper/main.wrapper.css`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.2/analytics_sdk/analysis-wrapper/main.wrapper.js` & `opsramp-analytics-utils-3.3.3/analytics_sdk/analysis-wrapper/main.wrapper.js`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.2/analytics_sdk/analysis-wrapper/media/fontello.487f60cd.woff` & `opsramp-analytics-utils-3.3.3/analytics_sdk/analysis-wrapper/media/fontello.487f60cd.woff`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.2/analytics_sdk/analysis-wrapper/media/fontello.52a41d35.svg` & `opsramp-analytics-utils-3.3.3/analytics_sdk/analysis-wrapper/media/fontello.52a41d35.svg`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.2/analytics_sdk/analysis-wrapper/media/fontello.8be26641.ttf` & `opsramp-analytics-utils-3.3.3/analytics_sdk/analysis-wrapper/media/fontello.8be26641.ttf`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.2/analytics_sdk/analysis-wrapper/media/fontello.8fcd07de.woff2` & `opsramp-analytics-utils-3.3.3/analytics_sdk/analysis-wrapper/media/fontello.8fcd07de.woff2`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.2/analytics_sdk/analysis-wrapper/media/fontello.d35868c4.eot` & `opsramp-analytics-utils-3.3.3/analytics_sdk/analysis-wrapper/media/fontello.d35868c4.eot`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.2/analytics_sdk/analysis-wrapper/media/icon-copy.c16adda9.svg` & `opsramp-analytics-utils-3.3.3/analytics_sdk/analysis-wrapper/media/icon-copy.c16adda9.svg`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.2/analytics_sdk/analysis-wrapper/media/icon-edit.ae3b1e05.svg` & `opsramp-analytics-utils-3.3.3/analytics_sdk/analysis-wrapper/media/icon-edit.ae3b1e05.svg`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.2/analytics_sdk/analysis-wrapper/media/icon-remove.184d1ffb.svg` & `opsramp-analytics-utils-3.3.3/analytics_sdk/analysis-wrapper/media/icon-remove.184d1ffb.svg`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.2/analytics_sdk/analysis-wrapper/media/revicons.04eb8fc5.woff` & `opsramp-analytics-utils-3.3.3/analytics_sdk/analysis-wrapper/media/revicons.04eb8fc5.woff`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.2/analytics_sdk/analysis-wrapper/media/revicons.17629a5d.ttf` & `opsramp-analytics-utils-3.3.3/analytics_sdk/analysis-wrapper/media/revicons.17629a5d.ttf`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.2/analytics_sdk/analysis-wrapper/media/revicons.2feb69cc.eot` & `opsramp-analytics-utils-3.3.3/analytics_sdk/analysis-wrapper/media/revicons.2feb69cc.eot`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.2/analytics_sdk/analysis-wrapper/media/transparent-bg.5f803547.svg` & `opsramp-analytics-utils-3.3.3/analytics_sdk/analysis-wrapper/media/transparent-bg.5f803547.svg`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.2/analytics_sdk/components.py` & `opsramp-analytics-utils-3.3.3/analytics_sdk/components.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.2/analytics_sdk/oap_dash.py` & `opsramp-analytics-utils-3.3.3/analytics_sdk/oap_dash.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.2/analytics_sdk/process/process.py` & `opsramp-analytics-utils-3.3.3/analytics_sdk/process/process.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.2/analytics_sdk/process/querybuilder.py` & `opsramp-analytics-utils-3.3.3/analytics_sdk/process/querybuilder.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.2/analytics_sdk/renderer/excel.py` & `opsramp-analytics-utils-3.3.3/analytics_sdk/renderer/excel.py`

 * *Files 4% similar despite different names*

```diff
@@ -291,20 +291,33 @@
         chart.width = chart_data.get('width', 17)
         chart.height = chart_data.get('height', 8.5)
 
         s1 = chart.series[0]
         s1.graphicalProperties.line.solidFill = "0077C8"
         s1.graphicalProperties.solidFill = "0077C8"
 
+        multicolor_check = False
+        multi_colors = chart_colors
+        if 'is-multicolored-chart' in chart_data:
+            multicolor_check = chart_data['is-multicolored-chart']
+        if 'colors' in chart_data and chart_data['colors']:
+            multi_colors = chart_data['colors']
+
         for idx, s in enumerate(chart.series):
-            index = len(chart_colors)%(idx+1)
-            if index >= len(chart_colors):
-                index = 0
-            s.graphicalProperties.line.solidFill = chart_colors[index]
-            s.graphicalProperties.solidFill = chart_colors[index]
+            if multicolor_check:
+                for i in range(len(multi_colors)):
+                    pt = DataPoint(idx=i)
+                    pt.graphicalProperties.solidFill = multi_colors[i]
+                    s.dPt.append(pt)
+            else:
+                index = len(chart_colors)%(idx+1)
+                if index >= len(chart_colors):
+                    index = 0
+                s.graphicalProperties.line.solidFill = chart_colors[index]
+                s.graphicalProperties.solidFill = chart_colors[index]
 
         ws.add_chart(chart, chart_data['chart-position'])
 
     def add_stack_bar_chart(self, ws, chart_data):
         """
         add stack bar chart component
         """
@@ -332,21 +345,29 @@
         chart.grouping = "stacked"
         chart.width = chart_data.get('width', 20)
         chart.height = chart_data.get('height', 10)
 
         s1 = chart.series[0]
         s1.graphicalProperties.line.solidFill = "0077C8"
         s1.graphicalProperties.solidFill = "0077C8"
-
+        
+        add_chart_colors = chart_colors
+        colors_check = False
+        if 'colors' in chart_data and chart_data['colors']:
+            add_chart_colors = chart_data['colors']+add_chart_colors
+            colors_check = True
+        
         for idx, s in enumerate(chart.series):
-            index = len(chart_colors)%(idx+1)
-            if index >= len(chart_colors):
+            index = idx
+            if not colors_check:
+                index = len(add_chart_colors)%(idx+1)
+            if index >= len(add_chart_colors):
                 index = 0
-            s.graphicalProperties.line.solidFill = chart_colors[index]
-            s.graphicalProperties.solidFill = chart_colors[index]
+            s.graphicalProperties.line.solidFill = add_chart_colors[index]
+            s.graphicalProperties.solidFill = add_chart_colors[index]
 
         ws.add_chart(chart, chart_data['chart-position'])
 
     def add_scatter_chart(self, ws, chart_data):
         """
         add scatter chart component
         """
```

### Comparing `opsramp-analytics-utils-3.3.2/analytics_sdk/renderer/pdf.py` & `opsramp-analytics-utils-3.3.3/analytics_sdk/renderer/pdf.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.2/analytics_sdk/utilities.py` & `opsramp-analytics-utils-3.3.3/analytics_sdk/utilities.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.2/opsramp_analytics_utils.egg-info/PKG-INFO` & `opsramp-analytics-utils-3.3.3/opsramp_analytics_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opsramp-analytics-utils
-Version: 3.3.2
+Version: 3.3.3
 Summary: OpsRamp Analytics SDK
 Home-page: https://github.com/opsramp/analytics-sdk
 Author: OpsRamp
 Author-email: opsramp@support.com
 License: UNKNOWN
 Description: ## OpsRamp Analytics Utilities
```

### Comparing `opsramp-analytics-utils-3.3.2/opsramp_analytics_utils.egg-info/SOURCES.txt` & `opsramp-analytics-utils-3.3.3/opsramp_analytics_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.2/setup.py` & `opsramp-analytics-utils-3.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     with open("requires-{}.txt".format(req_type)) as fp:
         requires = (line.strip() for line in fp)
         return [req for req in requires if req and not req.startswith("#")]
 
 
 setuptools.setup(
     name="opsramp-analytics-utils",
-    version="3.3.2",
+    version="3.3.3",
     author="OpsRamp",
     author_email="opsramp@support.com",
     description="OpsRamp Analytics SDK",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=read_req_file("install"),
     url="https://github.com/opsramp/analytics-sdk",
```

