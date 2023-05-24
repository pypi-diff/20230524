# Comparing `tmp/milspend-0.0.2.tar.gz` & `tmp/milspend-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/milspend-0.0.2.tar", last modified: Sun Feb 27 14:22:14 2022, max compression
+gzip compressed data, was "milspend-0.0.3.tar", last modified: Wed May 24 09:50:06 2023, max compression
```

## Comparing `milspend-0.0.2.tar` & `milspend-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2022-02-27 14:22:14.463702 milspend-0.0.2/
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)     1689 2022-02-27 14:22:14.463702 milspend-0.0.2/PKG-INFO
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)     1147 2022-02-27 14:19:58.000000 milspend-0.0.2/README.md
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)       38 2022-02-27 14:22:14.463702 milspend-0.0.2/setup.cfg
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)      962 2022-02-27 14:20:35.000000 milspend-0.0.2/setup.py
-drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2022-02-27 14:22:14.432443 milspend-0.0.2/src/
-drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2022-02-27 14:22:14.448068 milspend-0.0.2/src/milspend.egg-info/
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)     1689 2022-02-27 14:22:13.000000 milspend-0.0.2/src/milspend.egg-info/PKG-INFO
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)      217 2022-02-27 14:22:13.000000 milspend-0.0.2/src/milspend.egg-info/SOURCES.txt
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)        1 2022-02-27 14:22:13.000000 milspend-0.0.2/src/milspend.egg-info/dependency_links.txt
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)       44 2022-02-27 14:22:13.000000 milspend-0.0.2/src/milspend.egg-info/entry_points.txt
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)        9 2022-02-27 14:22:13.000000 milspend-0.0.2/src/milspend.egg-info/top_level.txt
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)     1808 2022-02-27 14:18:27.000000 milspend-0.0.2/src/milspend.py
+drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-05-24 09:50:06.894383 milspend-0.0.3/
+-rw-r--r--   0 yt        (1000) yt        (1000)     1689 2023-05-24 09:50:06.894383 milspend-0.0.3/PKG-INFO
+-rw-r--r--   0 yt        (1000) yt        (1000)     1147 2022-02-27 14:19:58.000000 milspend-0.0.3/README.md
+-rw-r--r--   0 yt        (1000) yt        (1000)       38 2023-05-24 09:50:06.902366 milspend-0.0.3/setup.cfg
+-rw-r--r--   0 yt        (1000) yt        (1000)      962 2023-05-23 23:56:30.000000 milspend-0.0.3/setup.py
+drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-05-24 09:50:06.887504 milspend-0.0.3/src/
+drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-05-24 09:50:06.894383 milspend-0.0.3/src/milspend.egg-info/
+-rw-r--r--   0 yt        (1000) yt        (1000)     1689 2023-05-24 09:50:06.000000 milspend-0.0.3/src/milspend.egg-info/PKG-INFO
+-rw-r--r--   0 yt        (1000) yt        (1000)      227 2023-05-24 09:50:06.000000 milspend-0.0.3/src/milspend.egg-info/SOURCES.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)        1 2023-05-24 09:50:06.000000 milspend-0.0.3/src/milspend.egg-info/dependency_links.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)       44 2023-05-24 09:50:06.000000 milspend-0.0.3/src/milspend.egg-info/entry_points.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)        9 2023-05-24 09:50:06.000000 milspend-0.0.3/src/milspend.egg-info/top_level.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)     1548 2023-05-24 09:49:23.000000 milspend-0.0.3/src/milspend.py
```

### Comparing `milspend-0.0.2/PKG-INFO` & `milspend-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: milspend
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package for visualizing military spending of up to 4 countries
 Home-page: https://github.com/ytakefuji/defense
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ytakefuji/defense
 Platform: UNKNOWN
```

### Comparing `milspend-0.0.2/README.md` & `milspend-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `milspend-0.0.2/setup.py` & `milspend-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="milspend",
-    version="0.0.2",
+    version="0.0.3",
     author="yoshiyasu takefuji",
     author_email="takefuji@keio.jp",
     description="A package for visualizing military spending of up to 4 countries",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ytakefuji/defense",
     project_urls={
```

### Comparing `milspend-0.0.2/src/milspend.egg-info/PKG-INFO` & `milspend-0.0.3/src/milspend.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: milspend
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package for visualizing military spending of up to 4 countries
 Home-page: https://github.com/ytakefuji/defense
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ytakefuji/defense
 Platform: UNKNOWN
```

