# Comparing `tmp/mapfun-0.0.3.tar.gz` & `tmp/mapfun-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapfun-0.0.3.tar", last modified: Wed May 24 15:11:47 2023, max compression
+gzip compressed data, was "mapfun-0.0.4.tar", last modified: Wed May 24 15:32:36 2023, max compression
```

## Comparing `mapfun-0.0.3.tar` & `mapfun-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 15:11:47.456429 mapfun-0.0.3/
--rw-rw-rw-   0        0        0     1094 2023-05-24 15:08:54.000000 mapfun-0.0.3/LICENCE
--rw-rw-rw-   0        0        0      523 2023-05-24 15:11:47.456429 mapfun-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2258 2023-05-24 15:08:54.000000 mapfun-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-24 15:11:47.451463 mapfun-0.0.3/mapfun.egg-info/
--rw-rw-rw-   0        0        0      523 2023-05-24 15:11:46.000000 mapfun-0.0.3/mapfun.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      160 2023-05-24 15:11:47.000000 mapfun-0.0.3/mapfun.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 15:11:46.000000 mapfun-0.0.3/mapfun.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-05-24 15:11:46.000000 mapfun-0.0.3/mapfun.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-24 15:11:47.456429 mapfun-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      701 2023-05-24 15:11:35.000000 mapfun-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-24 15:11:47.454568 mapfun-0.0.3/src/
--rw-rw-rw-   0        0        0     1085 2023-05-24 15:08:54.000000 mapfun-0.0.3/src/mapfun.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:32:36.757949 mapfun-0.0.4/
+-rw-rw-rw-   0        0        0     1094 2023-05-24 15:08:54.000000 mapfun-0.0.4/LICENCE
+-rw-rw-rw-   0        0        0      523 2023-05-24 15:32:36.750033 mapfun-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2258 2023-05-24 15:08:54.000000 mapfun-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-24 15:32:36.726493 mapfun-0.0.4/mapfun/
+-rw-rw-rw-   0        0        0       32 2023-05-24 15:31:29.000000 mapfun-0.0.4/mapfun/__init__.py
+-rw-rw-rw-   0        0        0     1085 2023-05-24 15:08:54.000000 mapfun-0.0.4/mapfun/mapfun.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:32:36.750033 mapfun-0.0.4/mapfun.egg-info/
+-rw-rw-rw-   0        0        0      523 2023-05-24 15:32:35.000000 mapfun-0.0.4/mapfun.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-05-24 15:32:36.000000 mapfun-0.0.4/mapfun.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 15:32:35.000000 mapfun-0.0.4/mapfun.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-24 15:32:36.000000 mapfun-0.0.4/mapfun.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-24 15:32:36.757949 mapfun-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      704 2023-05-24 15:32:25.000000 mapfun-0.0.4/setup.py
```

### Comparing `mapfun-0.0.3/LICENCE` & `mapfun-0.0.4/LICENCE`

 * *Files identical despite different names*

### Comparing `mapfun-0.0.3/PKG-INFO` & `mapfun-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapfun
-Version: 0.0.3
+Version: 0.0.4
 Summary: mapfun
 Author: Zakaria Elalaoui
 License: UNKNOWN
 Keywords: zikojs,python,map
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `mapfun-0.0.3/README.md` & `mapfun-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `mapfun-0.0.3/mapfun.egg-info/PKG-INFO` & `mapfun-0.0.4/mapfun.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapfun
-Version: 0.0.3
+Version: 0.0.4
 Summary: mapfun
 Author: Zakaria Elalaoui
 License: UNKNOWN
 Keywords: zikojs,python,map
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `mapfun-0.0.3/setup.py` & `mapfun-0.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup
 from pathlib import Path
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 parent = Path(__file__).parent
 setup(
     name="mapfun",
     version=VERSION,
     author="Zakaria Elalaoui",
     description="mapfun",
     long_description_content_type="text/markdown",
     #long_description=(parent / "README.md").read_text(),
-    packages = ['src'],
+    packages = ['mapfun'],
     keywords=['zikojs','python', 'map'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

### Comparing `mapfun-0.0.3/src/mapfun.py` & `mapfun-0.0.4/mapfun/mapfun.py`

 * *Files identical despite different names*

