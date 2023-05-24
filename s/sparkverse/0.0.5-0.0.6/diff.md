# Comparing `tmp/sparkverse-0.0.5.tar.gz` & `tmp/sparkverse-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparkverse-0.0.5.tar", last modified: Wed May 24 08:07:27 2023, max compression
+gzip compressed data, was "sparkverse-0.0.6.tar", last modified: Wed May 24 19:50:57 2023, max compression
```

## Comparing `sparkverse-0.0.5.tar` & `sparkverse-0.0.6.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-24 08:07:27.373096 sparkverse-0.0.5/
--rw-r--r--   0 root         (0) staff       (20)     1070 2023-05-22 07:25:35.000000 sparkverse-0.0.5/LICENSE
--rw-r--r--   0 root         (0) staff       (20)       37 2023-05-22 07:25:35.000000 sparkverse-0.0.5/MANIFEST.in
--rw-r--r--   0 root         (0) staff       (20)      423 2023-05-22 07:25:35.000000 sparkverse-0.0.5/NEWS.txt
--rw-r--r--   0 root         (0) staff       (20)     1031 2023-05-24 08:07:27.371994 sparkverse-0.0.5/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     4191 2023-05-22 07:25:35.000000 sparkverse-0.0.5/README.md
--rw-r--r--   0 root         (0) staff       (20)       38 2023-05-24 08:07:27.373623 sparkverse-0.0.5/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)     1427 2023-05-24 08:06:59.000000 sparkverse-0.0.5/setup.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-24 08:07:27.346528 sparkverse-0.0.5/src/
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-24 08:07:27.352869 sparkverse-0.0.5/src/sparkverse/
--rw-r--r--   0 root         (0) staff       (20)        0 2023-05-22 07:25:35.000000 sparkverse-0.0.5/src/sparkverse/__init__.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-24 08:07:27.360187 sparkverse-0.0.5/src/sparkverse/components/
--rw-r--r--   0 root         (0) staff       (20)        0 2023-05-22 07:25:35.000000 sparkverse-0.0.5/src/sparkverse/components/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     1577 2023-05-22 23:16:20.000000 sparkverse-0.0.5/src/sparkverse/components/log.py
--rw-r--r--   0 root         (0) staff       (20)     1005 2023-05-22 07:25:35.000000 sparkverse-0.0.5/src/sparkverse/components/video.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-24 08:07:27.369300 sparkverse-0.0.5/src/sparkverse/data/
--rwxr-xr-x   0 root         (0) staff       (20)    28453 2023-05-22 07:25:35.000000 sparkverse-0.0.5/src/sparkverse/data/Cropps1.png
--rwxr-xr-x   0 root         (0) staff       (20)    28684 2023-05-22 07:25:35.000000 sparkverse-0.0.5/src/sparkverse/data/Cropps2.png
--rwxr-xr-x   0 root         (0) staff       (20)    26184 2023-05-22 07:25:35.000000 sparkverse-0.0.5/src/sparkverse/data/LaneKeeper1.png
--rwxr-xr-x   0 root         (0) staff       (20)    26228 2023-05-22 07:25:35.000000 sparkverse-0.0.5/src/sparkverse/data/LaneKeeper2.png
--rwxr-xr-x   0 root         (0) staff       (20)    25273 2023-05-22 07:25:35.000000 sparkverse-0.0.5/src/sparkverse/data/LaneKeeper3.png
--rwxr-xr-x   0 root         (0) staff       (20)    76717 2023-05-22 07:25:35.000000 sparkverse-0.0.5/src/sparkverse/data/LineFollower1.png
--rwxr-xr-x   0 root         (0) staff       (20)    17710 2023-05-22 07:25:35.000000 sparkverse-0.0.5/src/sparkverse/data/LineFollower2.png
--rw-r--r--   0 root         (0) staff       (20)    74172 2023-05-22 07:25:35.000000 sparkverse-0.0.5/src/sparkverse/data/logo.png
--rw-r--r--   0 root         (0) staff       (20)    83117 2023-05-22 07:25:35.000000 sparkverse-0.0.5/src/sparkverse/data/logo1.png
--rwxr-xr-x   0 root         (0) staff       (20)      152 2023-05-22 07:25:35.000000 sparkverse-0.0.5/src/sparkverse/data/player.png
--rw-r--r--   0 root         (0) staff       (20)     1248 2023-05-22 23:01:12.000000 sparkverse-0.0.5/src/sparkverse/external_data.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-24 08:07:27.371157 sparkverse-0.0.5/src/sparkverse/gui/
--rw-r--r--   0 root         (0) staff       (20)        0 2023-05-22 07:25:35.000000 sparkverse-0.0.5/src/sparkverse/gui/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     8033 2023-05-22 07:25:35.000000 sparkverse-0.0.5/src/sparkverse/gui/help_bar.py
--rw-r--r--   0 root         (0) staff       (20)     3855 2023-05-22 07:25:35.000000 sparkverse-0.0.5/src/sparkverse/gui/sensor_bar.py
--rw-r--r--   0 root         (0) staff       (20)     3532 2023-05-22 22:59:21.000000 sparkverse-0.0.5/src/sparkverse/player.py
--rw-r--r--   0 root         (0) staff       (20)    12198 2023-05-22 22:44:56.000000 sparkverse-0.0.5/src/sparkverse/sensor.py
--rw-r--r--   0 root         (0) staff       (20)     2971 2023-05-22 23:04:06.000000 sparkverse-0.0.5/src/sparkverse/simulator.py
--rw-r--r--   0 root         (0) staff       (20)     9801 2023-05-22 23:14:10.000000 sparkverse-0.0.5/src/sparkverse/utils.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-24 08:07:27.358415 sparkverse-0.0.5/src/sparkverse.egg-info/
--rw-r--r--   0 root         (0) staff       (20)     1031 2023-05-24 08:07:27.000000 sparkverse-0.0.5/src/sparkverse.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     1014 2023-05-24 08:07:27.000000 sparkverse-0.0.5/src/sparkverse.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-05-24 08:07:27.000000 sparkverse-0.0.5/src/sparkverse.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       48 2023-05-24 08:07:27.000000 sparkverse-0.0.5/src/sparkverse.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-05-22 07:25:43.000000 sparkverse-0.0.5/src/sparkverse.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) staff       (20)       21 2023-05-24 08:07:27.000000 sparkverse-0.0.5/src/sparkverse.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)       11 2023-05-24 08:07:27.000000 sparkverse-0.0.5/src/sparkverse.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-24 19:50:56.999997 sparkverse-0.0.6/
+-rw-r--r--   0 root         (0) staff       (20)     1070 2023-05-22 07:25:35.000000 sparkverse-0.0.6/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)       37 2023-05-22 07:25:35.000000 sparkverse-0.0.6/MANIFEST.in
+-rw-r--r--   0 root         (0) staff       (20)      423 2023-05-22 07:25:35.000000 sparkverse-0.0.6/NEWS.txt
+-rw-r--r--   0 root         (0) staff       (20)     1031 2023-05-24 19:50:56.999521 sparkverse-0.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     4191 2023-05-22 07:25:35.000000 sparkverse-0.0.6/README.md
+-rw-r--r--   0 root         (0) staff       (20)       38 2023-05-24 19:50:57.000137 sparkverse-0.0.6/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)     1456 2023-05-24 19:47:17.000000 sparkverse-0.0.6/setup.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-24 19:50:56.953870 sparkverse-0.0.6/src/
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-24 19:50:56.972179 sparkverse-0.0.6/src/sparkverse/
+-rw-r--r--   0 root         (0) staff       (20)        0 2023-05-22 07:25:35.000000 sparkverse-0.0.6/src/sparkverse/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-24 19:50:56.981393 sparkverse-0.0.6/src/sparkverse/components/
+-rw-r--r--   0 root         (0) staff       (20)        0 2023-05-22 07:25:35.000000 sparkverse-0.0.6/src/sparkverse/components/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     1577 2023-05-22 23:16:20.000000 sparkverse-0.0.6/src/sparkverse/components/log.py
+-rw-r--r--   0 root         (0) staff       (20)     1005 2023-05-22 07:25:35.000000 sparkverse-0.0.6/src/sparkverse/components/video.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-24 19:50:56.996891 sparkverse-0.0.6/src/sparkverse/data/
+-rwxr-xr-x   0 root         (0) staff       (20)    28453 2023-05-22 07:25:35.000000 sparkverse-0.0.6/src/sparkverse/data/Cropps1.png
+-rwxr-xr-x   0 root         (0) staff       (20)    28684 2023-05-22 07:25:35.000000 sparkverse-0.0.6/src/sparkverse/data/Cropps2.png
+-rwxr-xr-x   0 root         (0) staff       (20)    26184 2023-05-22 07:25:35.000000 sparkverse-0.0.6/src/sparkverse/data/LaneKeeper1.png
+-rwxr-xr-x   0 root         (0) staff       (20)    26228 2023-05-22 07:25:35.000000 sparkverse-0.0.6/src/sparkverse/data/LaneKeeper2.png
+-rwxr-xr-x   0 root         (0) staff       (20)    25273 2023-05-22 07:25:35.000000 sparkverse-0.0.6/src/sparkverse/data/LaneKeeper3.png
+-rwxr-xr-x   0 root         (0) staff       (20)    76717 2023-05-22 07:25:35.000000 sparkverse-0.0.6/src/sparkverse/data/LineFollower1.png
+-rwxr-xr-x   0 root         (0) staff       (20)    17710 2023-05-22 07:25:35.000000 sparkverse-0.0.6/src/sparkverse/data/LineFollower2.png
+-rw-r--r--   0 root         (0) staff       (20)    74172 2023-05-22 07:25:35.000000 sparkverse-0.0.6/src/sparkverse/data/logo.png
+-rw-r--r--   0 root         (0) staff       (20)    83117 2023-05-22 07:25:35.000000 sparkverse-0.0.6/src/sparkverse/data/logo1.png
+-rwxr-xr-x   0 root         (0) staff       (20)      152 2023-05-22 07:25:35.000000 sparkverse-0.0.6/src/sparkverse/data/player.png
+-rw-r--r--   0 root         (0) staff       (20)     1298 2023-05-24 19:47:56.000000 sparkverse-0.0.6/src/sparkverse/external_data.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-24 19:50:56.998887 sparkverse-0.0.6/src/sparkverse/gui/
+-rw-r--r--   0 root         (0) staff       (20)        0 2023-05-22 07:25:35.000000 sparkverse-0.0.6/src/sparkverse/gui/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     8033 2023-05-22 07:25:35.000000 sparkverse-0.0.6/src/sparkverse/gui/help_bar.py
+-rw-r--r--   0 root         (0) staff       (20)     3855 2023-05-22 07:25:35.000000 sparkverse-0.0.6/src/sparkverse/gui/sensor_bar.py
+-rw-r--r--   0 root         (0) staff       (20)     3532 2023-05-22 22:59:21.000000 sparkverse-0.0.6/src/sparkverse/player.py
+-rw-r--r--   0 root         (0) staff       (20)    12198 2023-05-22 22:44:56.000000 sparkverse-0.0.6/src/sparkverse/sensor.py
+-rw-r--r--   0 root         (0) staff       (20)     3003 2023-05-24 19:50:21.000000 sparkverse-0.0.6/src/sparkverse/simulator.py
+-rw-r--r--   0 root         (0) staff       (20)     9801 2023-05-22 23:14:10.000000 sparkverse-0.0.6/src/sparkverse/utils.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-24 19:50:56.979239 sparkverse-0.0.6/src/sparkverse.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)     1031 2023-05-24 19:50:56.000000 sparkverse-0.0.6/src/sparkverse.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     1014 2023-05-24 19:50:56.000000 sparkverse-0.0.6/src/sparkverse.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-05-24 19:50:56.000000 sparkverse-0.0.6/src/sparkverse.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       48 2023-05-24 19:50:56.000000 sparkverse-0.0.6/src/sparkverse.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-05-22 07:25:43.000000 sparkverse-0.0.6/src/sparkverse.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) staff       (20)       21 2023-05-24 19:50:56.000000 sparkverse-0.0.6/src/sparkverse.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)       11 2023-05-24 19:50:56.000000 sparkverse-0.0.6/src/sparkverse.egg-info/top_level.txt
```

### Comparing `sparkverse-0.0.5/LICENSE` & `sparkverse-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sparkverse-0.0.5/PKG-INFO` & `sparkverse-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparkverse
-Version: 0.0.5
+Version: 0.0.6
 Summary: Simple python3 simulator for advance driving systems
 Home-page: https://github.com/Amporu/SparkVerse
 Author: Tucudean Adrian-Ionut
 Author-email: Tucudean.Adrian.Ionut0@gmail.com
 License: MIT
 Keywords: Simulator computer vision Advanced Driving
 Classifier: Development Status :: 1 - Planning
```

### Comparing `sparkverse-0.0.5/README.md` & `sparkverse-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `sparkverse-0.0.5/setup.py` & `sparkverse-0.0.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 import os
 from setuptools import setup, find_packages
 
 here = os.path.abspath(os.path.dirname(__file__))
 #README = open(os.path.join(here, 'README-pypi.rst')).read()
 NEWS = open(os.path.join(here, 'NEWS.txt')).read()
-
-
-version = '0.0.5'
+from src.sparkverse.external_data import VERSION
 
 install_requires = [
     # List your project dependencies here.
     # For more details, see:
     # http://packages.python.org/distribute/setuptools.html#declaring-dependencies
     'requests'	
 ]
 
 
 setup(name='sparkverse',
-    version=version,
+    version=VERSION,
     description="Simple python3 simulator for advance driving systems",
     long_description= NEWS,
     keywords='Simulator computer vision Advanced Driving',
     author='Tucudean Adrian-Ionut',
     author_email='Tucudean.Adrian.Ionut0@gmail.com',
     url='https://github.com/Amporu/SparkVerse',
     license='MIT',
```

### Comparing `sparkverse-0.0.5/src/sparkverse/components/log.py` & `sparkverse-0.0.6/src/sparkverse/components/log.py`

 * *Files identical despite different names*

### Comparing `sparkverse-0.0.5/src/sparkverse/components/video.py` & `sparkverse-0.0.6/src/sparkverse/components/video.py`

 * *Files identical despite different names*

### Comparing `sparkverse-0.0.5/src/sparkverse/data/Cropps1.png` & `sparkverse-0.0.6/src/sparkverse/data/Cropps1.png`

 * *Files identical despite different names*

### Comparing `sparkverse-0.0.5/src/sparkverse/data/Cropps2.png` & `sparkverse-0.0.6/src/sparkverse/data/Cropps2.png`

 * *Files identical despite different names*

### Comparing `sparkverse-0.0.5/src/sparkverse/data/LaneKeeper1.png` & `sparkverse-0.0.6/src/sparkverse/data/LaneKeeper1.png`

 * *Files identical despite different names*

### Comparing `sparkverse-0.0.5/src/sparkverse/data/LaneKeeper2.png` & `sparkverse-0.0.6/src/sparkverse/data/LaneKeeper2.png`

 * *Files identical despite different names*

### Comparing `sparkverse-0.0.5/src/sparkverse/data/LaneKeeper3.png` & `sparkverse-0.0.6/src/sparkverse/data/LaneKeeper3.png`

 * *Files identical despite different names*

### Comparing `sparkverse-0.0.5/src/sparkverse/data/LineFollower1.png` & `sparkverse-0.0.6/src/sparkverse/data/LineFollower1.png`

 * *Files identical despite different names*

### Comparing `sparkverse-0.0.5/src/sparkverse/data/LineFollower2.png` & `sparkverse-0.0.6/src/sparkverse/data/LineFollower2.png`

 * *Files identical despite different names*

### Comparing `sparkverse-0.0.5/src/sparkverse/data/logo.png` & `sparkverse-0.0.6/src/sparkverse/data/logo.png`

 * *Files identical despite different names*

### Comparing `sparkverse-0.0.5/src/sparkverse/data/logo1.png` & `sparkverse-0.0.6/src/sparkverse/data/logo1.png`

 * *Files identical despite different names*

### Comparing `sparkverse-0.0.5/src/sparkverse/external_data.py` & `sparkverse-0.0.6/src/sparkverse/external_data.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 autor: Tucudean Adrian-Ionut
 date: 22.05.2023
 email: Tucudean.Adrian.Ionut@outlook.com
 license: MIT
 """
 import os
 from sparkverse.components.log import logger
-logger.info ("")
-
+VERSION='0.0.6'
+logger.info(f"VERSION : \033[92m{VERSION}\033[0m")
 CAR    = os.path.join(os.path.dirname(__file__), 'data/player.png')
 LEVEL1 = os.path.join(os.path.dirname(__file__), 'data/LineFollower1.png')
 LEVEL2 = os.path.join(os.path.dirname(__file__), 'data/LineFollower2.png')
 LEVEL3 = os.path.join(os.path.dirname(__file__), 'data/LaneKeeper1.png')
 LEVEL4 = os.path.join(os.path.dirname(__file__), 'data/LaneKeeper2.png')
 LEVEL5 = os.path.join(os.path.dirname(__file__), 'data/LaneKeeper3.png')
 LEVEL6 = os.path.join(os.path.dirname(__file__), 'data/Cropps1.png')
@@ -21,8 +21,8 @@
 if os.path.exists(CAR) and os.path.exists(LEVEL1) and os.path.exists(LOGO):
     logger.info("ASSETS : \033[92mOK\033[0m")
     logger.info("TRACK : \033[92mOK\033[0m")
 else:
     logger.error("ASSETS : \033[91mNOT FOUND\033[0m")
 SIMULATOR=os.path.join(os.path.dirname(__file__), 'simulator.py')
 if os.path.exists(SIMULATOR):
-    logger.info("SCRIPTS : \033[92mOK\033[0m")
+    logger.info("SCRIPTS : \033[92mOK\033[0m")
```

### Comparing `sparkverse-0.0.5/src/sparkverse/gui/help_bar.py` & `sparkverse-0.0.6/src/sparkverse/gui/help_bar.py`

 * *Files identical despite different names*

### Comparing `sparkverse-0.0.5/src/sparkverse/gui/sensor_bar.py` & `sparkverse-0.0.6/src/sparkverse/gui/sensor_bar.py`

 * *Files identical despite different names*

### Comparing `sparkverse-0.0.5/src/sparkverse/player.py` & `sparkverse-0.0.6/src/sparkverse/player.py`

 * *Files identical despite different names*

### Comparing `sparkverse-0.0.5/src/sparkverse/sensor.py` & `sparkverse-0.0.6/src/sparkverse/sensor.py`

 * *Files identical despite different names*

### Comparing `sparkverse-0.0.5/src/sparkverse/simulator.py` & `sparkverse-0.0.6/src/sparkverse/simulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,23 @@
 license: MIT
 """
 import pygame
 import sparkverse.external_data as ex
 import sparkverse.player as pl
 from sparkverse.utils import Utils
 from sparkverse.components.log import logger
-#pylint: disable=E1101
 
+#pylint: disable=E1101
 class Simulator(Utils):
     """simulator class"""
     logger.info("TRACK PRESET : \033[92mLEVEL1\033[0m")
     TRACK=pygame.image.load(ex.LEVEL1)
     WIDTH, HEIGHT = TRACK.get_width(), TRACK.get_height()
     WIN = pygame.display.set_mode((WIDTH, HEIGHT))#),pygame.NOFRAME | pygame.HIDDEN)
+    pygame.event.set_grab(True)
     TITLE=pygame.display.set_caption("Pygame SIMULATOR")
 
     isRunning = True
     clock = pygame.time.Clock()
     player_car = pl.PlayerCar(2, 2)
     FPS=30
```

### Comparing `sparkverse-0.0.5/src/sparkverse/utils.py` & `sparkverse-0.0.6/src/sparkverse/utils.py`

 * *Files identical despite different names*

### Comparing `sparkverse-0.0.5/src/sparkverse.egg-info/PKG-INFO` & `sparkverse-0.0.6/src/sparkverse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparkverse
-Version: 0.0.5
+Version: 0.0.6
 Summary: Simple python3 simulator for advance driving systems
 Home-page: https://github.com/Amporu/SparkVerse
 Author: Tucudean Adrian-Ionut
 Author-email: Tucudean.Adrian.Ionut0@gmail.com
 License: MIT
 Keywords: Simulator computer vision Advanced Driving
 Classifier: Development Status :: 1 - Planning
```

### Comparing `sparkverse-0.0.5/src/sparkverse.egg-info/SOURCES.txt` & `sparkverse-0.0.6/src/sparkverse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

