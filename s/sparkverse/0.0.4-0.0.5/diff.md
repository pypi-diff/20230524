# Comparing `tmp/sparkverse-0.0.4.tar.gz` & `tmp/sparkverse-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparkverse-0.0.4.tar", last modified: Tue May 23 07:41:40 2023, max compression
+gzip compressed data, was "sparkverse-0.0.5.tar", last modified: Wed May 24 08:07:27 2023, max compression
```

## Comparing `sparkverse-0.0.4.tar` & `sparkverse-0.0.5.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-23 07:41:40.756348 sparkverse-0.0.4/
--rw-r--r--   0 root         (0) staff       (20)     1070 2023-05-22 07:25:35.000000 sparkverse-0.0.4/LICENSE
--rw-r--r--   0 root         (0) staff       (20)       37 2023-05-22 07:25:35.000000 sparkverse-0.0.4/MANIFEST.in
--rw-r--r--   0 root         (0) staff       (20)      423 2023-05-22 07:25:35.000000 sparkverse-0.0.4/NEWS.txt
--rw-r--r--   0 root         (0) staff       (20)     1031 2023-05-23 07:41:40.755661 sparkverse-0.0.4/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     4191 2023-05-22 07:25:35.000000 sparkverse-0.0.4/README.md
--rw-r--r--   0 root         (0) staff       (20)       38 2023-05-23 07:41:40.756454 sparkverse-0.0.4/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)     1427 2023-05-23 07:41:34.000000 sparkverse-0.0.4/setup.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-23 07:41:40.724466 sparkverse-0.0.4/src/
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-23 07:41:40.734655 sparkverse-0.0.4/src/sparkverse/
--rw-r--r--   0 root         (0) staff       (20)        0 2023-05-22 07:25:35.000000 sparkverse-0.0.4/src/sparkverse/__init__.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-23 07:41:40.739346 sparkverse-0.0.4/src/sparkverse/components/
--rw-r--r--   0 root         (0) staff       (20)        0 2023-05-22 07:25:35.000000 sparkverse-0.0.4/src/sparkverse/components/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     1577 2023-05-22 23:16:20.000000 sparkverse-0.0.4/src/sparkverse/components/log.py
--rw-r--r--   0 root         (0) staff       (20)     1005 2023-05-22 07:25:35.000000 sparkverse-0.0.4/src/sparkverse/components/video.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-23 07:41:40.752447 sparkverse-0.0.4/src/sparkverse/data/
--rwxr-xr-x   0 root         (0) staff       (20)    28453 2023-05-22 07:25:35.000000 sparkverse-0.0.4/src/sparkverse/data/Cropps1.png
--rwxr-xr-x   0 root         (0) staff       (20)    28684 2023-05-22 07:25:35.000000 sparkverse-0.0.4/src/sparkverse/data/Cropps2.png
--rwxr-xr-x   0 root         (0) staff       (20)    26184 2023-05-22 07:25:35.000000 sparkverse-0.0.4/src/sparkverse/data/LaneKeeper1.png
--rwxr-xr-x   0 root         (0) staff       (20)    26228 2023-05-22 07:25:35.000000 sparkverse-0.0.4/src/sparkverse/data/LaneKeeper2.png
--rwxr-xr-x   0 root         (0) staff       (20)    25273 2023-05-22 07:25:35.000000 sparkverse-0.0.4/src/sparkverse/data/LaneKeeper3.png
--rwxr-xr-x   0 root         (0) staff       (20)    76717 2023-05-22 07:25:35.000000 sparkverse-0.0.4/src/sparkverse/data/LineFollower1.png
--rwxr-xr-x   0 root         (0) staff       (20)    17710 2023-05-22 07:25:35.000000 sparkverse-0.0.4/src/sparkverse/data/LineFollower2.png
--rw-r--r--   0 root         (0) staff       (20)    74172 2023-05-22 07:25:35.000000 sparkverse-0.0.4/src/sparkverse/data/logo.png
--rw-r--r--   0 root         (0) staff       (20)    83117 2023-05-22 07:25:35.000000 sparkverse-0.0.4/src/sparkverse/data/logo1.png
--rwxr-xr-x   0 root         (0) staff       (20)      152 2023-05-22 07:25:35.000000 sparkverse-0.0.4/src/sparkverse/data/player.png
--rw-r--r--   0 root         (0) staff       (20)     1248 2023-05-22 23:01:12.000000 sparkverse-0.0.4/src/sparkverse/external_data.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-23 07:41:40.754444 sparkverse-0.0.4/src/sparkverse/gui/
--rw-r--r--   0 root         (0) staff       (20)        0 2023-05-22 07:25:35.000000 sparkverse-0.0.4/src/sparkverse/gui/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     8033 2023-05-22 07:25:35.000000 sparkverse-0.0.4/src/sparkverse/gui/help_bar.py
--rw-r--r--   0 root         (0) staff       (20)     3855 2023-05-22 07:25:35.000000 sparkverse-0.0.4/src/sparkverse/gui/sensor_bar.py
--rw-r--r--   0 root         (0) staff       (20)     3532 2023-05-22 22:59:21.000000 sparkverse-0.0.4/src/sparkverse/player.py
--rw-r--r--   0 root         (0) staff       (20)    12198 2023-05-22 22:44:56.000000 sparkverse-0.0.4/src/sparkverse/sensor.py
--rw-r--r--   0 root         (0) staff       (20)     2971 2023-05-22 23:04:06.000000 sparkverse-0.0.4/src/sparkverse/simulator.py
--rw-r--r--   0 root         (0) staff       (20)     9801 2023-05-22 23:14:10.000000 sparkverse-0.0.4/src/sparkverse/utils.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-23 07:41:40.737948 sparkverse-0.0.4/src/sparkverse.egg-info/
--rw-r--r--   0 root         (0) staff       (20)     1031 2023-05-23 07:41:40.000000 sparkverse-0.0.4/src/sparkverse.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     1014 2023-05-23 07:41:40.000000 sparkverse-0.0.4/src/sparkverse.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-05-23 07:41:40.000000 sparkverse-0.0.4/src/sparkverse.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       48 2023-05-23 07:41:40.000000 sparkverse-0.0.4/src/sparkverse.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-05-22 07:25:43.000000 sparkverse-0.0.4/src/sparkverse.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) staff       (20)       21 2023-05-23 07:41:40.000000 sparkverse-0.0.4/src/sparkverse.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)       11 2023-05-23 07:41:40.000000 sparkverse-0.0.4/src/sparkverse.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-24 08:07:27.373096 sparkverse-0.0.5/
+-rw-r--r--   0 root         (0) staff       (20)     1070 2023-05-22 07:25:35.000000 sparkverse-0.0.5/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)       37 2023-05-22 07:25:35.000000 sparkverse-0.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) staff       (20)      423 2023-05-22 07:25:35.000000 sparkverse-0.0.5/NEWS.txt
+-rw-r--r--   0 root         (0) staff       (20)     1031 2023-05-24 08:07:27.371994 sparkverse-0.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     4191 2023-05-22 07:25:35.000000 sparkverse-0.0.5/README.md
+-rw-r--r--   0 root         (0) staff       (20)       38 2023-05-24 08:07:27.373623 sparkverse-0.0.5/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)     1427 2023-05-24 08:06:59.000000 sparkverse-0.0.5/setup.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-24 08:07:27.346528 sparkverse-0.0.5/src/
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-24 08:07:27.352869 sparkverse-0.0.5/src/sparkverse/
+-rw-r--r--   0 root         (0) staff       (20)        0 2023-05-22 07:25:35.000000 sparkverse-0.0.5/src/sparkverse/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-24 08:07:27.360187 sparkverse-0.0.5/src/sparkverse/components/
+-rw-r--r--   0 root         (0) staff       (20)        0 2023-05-22 07:25:35.000000 sparkverse-0.0.5/src/sparkverse/components/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     1577 2023-05-22 23:16:20.000000 sparkverse-0.0.5/src/sparkverse/components/log.py
+-rw-r--r--   0 root         (0) staff       (20)     1005 2023-05-22 07:25:35.000000 sparkverse-0.0.5/src/sparkverse/components/video.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-24 08:07:27.369300 sparkverse-0.0.5/src/sparkverse/data/
+-rwxr-xr-x   0 root         (0) staff       (20)    28453 2023-05-22 07:25:35.000000 sparkverse-0.0.5/src/sparkverse/data/Cropps1.png
+-rwxr-xr-x   0 root         (0) staff       (20)    28684 2023-05-22 07:25:35.000000 sparkverse-0.0.5/src/sparkverse/data/Cropps2.png
+-rwxr-xr-x   0 root         (0) staff       (20)    26184 2023-05-22 07:25:35.000000 sparkverse-0.0.5/src/sparkverse/data/LaneKeeper1.png
+-rwxr-xr-x   0 root         (0) staff       (20)    26228 2023-05-22 07:25:35.000000 sparkverse-0.0.5/src/sparkverse/data/LaneKeeper2.png
+-rwxr-xr-x   0 root         (0) staff       (20)    25273 2023-05-22 07:25:35.000000 sparkverse-0.0.5/src/sparkverse/data/LaneKeeper3.png
+-rwxr-xr-x   0 root         (0) staff       (20)    76717 2023-05-22 07:25:35.000000 sparkverse-0.0.5/src/sparkverse/data/LineFollower1.png
+-rwxr-xr-x   0 root         (0) staff       (20)    17710 2023-05-22 07:25:35.000000 sparkverse-0.0.5/src/sparkverse/data/LineFollower2.png
+-rw-r--r--   0 root         (0) staff       (20)    74172 2023-05-22 07:25:35.000000 sparkverse-0.0.5/src/sparkverse/data/logo.png
+-rw-r--r--   0 root         (0) staff       (20)    83117 2023-05-22 07:25:35.000000 sparkverse-0.0.5/src/sparkverse/data/logo1.png
+-rwxr-xr-x   0 root         (0) staff       (20)      152 2023-05-22 07:25:35.000000 sparkverse-0.0.5/src/sparkverse/data/player.png
+-rw-r--r--   0 root         (0) staff       (20)     1248 2023-05-22 23:01:12.000000 sparkverse-0.0.5/src/sparkverse/external_data.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-24 08:07:27.371157 sparkverse-0.0.5/src/sparkverse/gui/
+-rw-r--r--   0 root         (0) staff       (20)        0 2023-05-22 07:25:35.000000 sparkverse-0.0.5/src/sparkverse/gui/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     8033 2023-05-22 07:25:35.000000 sparkverse-0.0.5/src/sparkverse/gui/help_bar.py
+-rw-r--r--   0 root         (0) staff       (20)     3855 2023-05-22 07:25:35.000000 sparkverse-0.0.5/src/sparkverse/gui/sensor_bar.py
+-rw-r--r--   0 root         (0) staff       (20)     3532 2023-05-22 22:59:21.000000 sparkverse-0.0.5/src/sparkverse/player.py
+-rw-r--r--   0 root         (0) staff       (20)    12198 2023-05-22 22:44:56.000000 sparkverse-0.0.5/src/sparkverse/sensor.py
+-rw-r--r--   0 root         (0) staff       (20)     2971 2023-05-22 23:04:06.000000 sparkverse-0.0.5/src/sparkverse/simulator.py
+-rw-r--r--   0 root         (0) staff       (20)     9801 2023-05-22 23:14:10.000000 sparkverse-0.0.5/src/sparkverse/utils.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-24 08:07:27.358415 sparkverse-0.0.5/src/sparkverse.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)     1031 2023-05-24 08:07:27.000000 sparkverse-0.0.5/src/sparkverse.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     1014 2023-05-24 08:07:27.000000 sparkverse-0.0.5/src/sparkverse.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-05-24 08:07:27.000000 sparkverse-0.0.5/src/sparkverse.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       48 2023-05-24 08:07:27.000000 sparkverse-0.0.5/src/sparkverse.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-05-22 07:25:43.000000 sparkverse-0.0.5/src/sparkverse.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) staff       (20)       21 2023-05-24 08:07:27.000000 sparkverse-0.0.5/src/sparkverse.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)       11 2023-05-24 08:07:27.000000 sparkverse-0.0.5/src/sparkverse.egg-info/top_level.txt
```

### Comparing `sparkverse-0.0.4/LICENSE` & `sparkverse-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sparkverse-0.0.4/PKG-INFO` & `sparkverse-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparkverse
-Version: 0.0.4
+Version: 0.0.5
 Summary: Simple python3 simulator for advance driving systems
 Home-page: https://github.com/Amporu/SparkVerse
 Author: Tucudean Adrian-Ionut
 Author-email: Tucudean.Adrian.Ionut0@gmail.com
 License: MIT
 Keywords: Simulator computer vision Advanced Driving
 Classifier: Development Status :: 1 - Planning
```

### Comparing `sparkverse-0.0.4/README.md` & `sparkverse-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `sparkverse-0.0.4/setup.py` & `sparkverse-0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 here = os.path.abspath(os.path.dirname(__file__))
 #README = open(os.path.join(here, 'README-pypi.rst')).read()
 NEWS = open(os.path.join(here, 'NEWS.txt')).read()
 
 
-version = '0.0.4'
+version = '0.0.5'
 
 install_requires = [
     # List your project dependencies here.
     # For more details, see:
     # http://packages.python.org/distribute/setuptools.html#declaring-dependencies
     'requests'	
 ]
```

### Comparing `sparkverse-0.0.4/src/sparkverse/components/log.py` & `sparkverse-0.0.5/src/sparkverse/components/log.py`

 * *Files identical despite different names*

### Comparing `sparkverse-0.0.4/src/sparkverse/components/video.py` & `sparkverse-0.0.5/src/sparkverse/components/video.py`

 * *Files identical despite different names*

### Comparing `sparkverse-0.0.4/src/sparkverse/data/Cropps1.png` & `sparkverse-0.0.5/src/sparkverse/data/Cropps1.png`

 * *Files identical despite different names*

### Comparing `sparkverse-0.0.4/src/sparkverse/data/Cropps2.png` & `sparkverse-0.0.5/src/sparkverse/data/Cropps2.png`

 * *Files identical despite different names*

### Comparing `sparkverse-0.0.4/src/sparkverse/data/LaneKeeper1.png` & `sparkverse-0.0.5/src/sparkverse/data/LaneKeeper1.png`

 * *Files identical despite different names*

### Comparing `sparkverse-0.0.4/src/sparkverse/data/LaneKeeper2.png` & `sparkverse-0.0.5/src/sparkverse/data/LaneKeeper2.png`

 * *Files identical despite different names*

### Comparing `sparkverse-0.0.4/src/sparkverse/data/LaneKeeper3.png` & `sparkverse-0.0.5/src/sparkverse/data/LaneKeeper3.png`

 * *Files identical despite different names*

### Comparing `sparkverse-0.0.4/src/sparkverse/data/LineFollower1.png` & `sparkverse-0.0.5/src/sparkverse/data/LineFollower1.png`

 * *Files identical despite different names*

### Comparing `sparkverse-0.0.4/src/sparkverse/data/LineFollower2.png` & `sparkverse-0.0.5/src/sparkverse/data/LineFollower2.png`

 * *Files identical despite different names*

### Comparing `sparkverse-0.0.4/src/sparkverse/data/logo.png` & `sparkverse-0.0.5/src/sparkverse/data/logo.png`

 * *Files identical despite different names*

### Comparing `sparkverse-0.0.4/src/sparkverse/data/logo1.png` & `sparkverse-0.0.5/src/sparkverse/data/logo1.png`

 * *Files identical despite different names*

### Comparing `sparkverse-0.0.4/src/sparkverse/external_data.py` & `sparkverse-0.0.5/src/sparkverse/external_data.py`

 * *Files identical despite different names*

### Comparing `sparkverse-0.0.4/src/sparkverse/gui/help_bar.py` & `sparkverse-0.0.5/src/sparkverse/gui/help_bar.py`

 * *Files identical despite different names*

### Comparing `sparkverse-0.0.4/src/sparkverse/gui/sensor_bar.py` & `sparkverse-0.0.5/src/sparkverse/gui/sensor_bar.py`

 * *Files identical despite different names*

### Comparing `sparkverse-0.0.4/src/sparkverse/player.py` & `sparkverse-0.0.5/src/sparkverse/player.py`

 * *Files identical despite different names*

### Comparing `sparkverse-0.0.4/src/sparkverse/sensor.py` & `sparkverse-0.0.5/src/sparkverse/sensor.py`

 * *Files identical despite different names*

### Comparing `sparkverse-0.0.4/src/sparkverse/simulator.py` & `sparkverse-0.0.5/src/sparkverse/simulator.py`

 * *Files identical despite different names*

### Comparing `sparkverse-0.0.4/src/sparkverse/utils.py` & `sparkverse-0.0.5/src/sparkverse/utils.py`

 * *Files identical despite different names*

### Comparing `sparkverse-0.0.4/src/sparkverse.egg-info/PKG-INFO` & `sparkverse-0.0.5/src/sparkverse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparkverse
-Version: 0.0.4
+Version: 0.0.5
 Summary: Simple python3 simulator for advance driving systems
 Home-page: https://github.com/Amporu/SparkVerse
 Author: Tucudean Adrian-Ionut
 Author-email: Tucudean.Adrian.Ionut0@gmail.com
 License: MIT
 Keywords: Simulator computer vision Advanced Driving
 Classifier: Development Status :: 1 - Planning
```

### Comparing `sparkverse-0.0.4/src/sparkverse.egg-info/SOURCES.txt` & `sparkverse-0.0.5/src/sparkverse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

