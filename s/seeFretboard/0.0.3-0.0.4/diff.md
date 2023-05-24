# Comparing `tmp/seeFretboard-0.0.3.tar.gz` & `tmp/seeFretboard-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seeFretboard-0.0.3.tar", last modified: Wed May 24 18:29:22 2023, max compression
+gzip compressed data, was "seeFretboard-0.0.4.tar", last modified: Wed May 24 18:57:15 2023, max compression
```

## Comparing `seeFretboard-0.0.3.tar` & `seeFretboard-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,59 @@
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-24 18:29:22.953337 seeFretboard-0.0.3/
--rw-r--r--   0 lindazhang   (501) staff       (20)     1072 2023-05-24 18:18:02.000000 seeFretboard-0.0.3/LICENSE
--rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-05-24 18:19:53.000000 seeFretboard-0.0.3/MANIFEST.in
--rw-r--r--   0 lindazhang   (501) staff       (20)     1370 2023-05-24 18:29:22.953166 seeFretboard-0.0.3/PKG-INFO
--rw-r--r--   0 lindazhang   (501) staff       (20)     1005 2023-05-02 18:53:11.000000 seeFretboard-0.0.3/README.md
--rw-r--r--   0 lindazhang   (501) staff       (20)      287 2023-05-24 18:17:32.000000 seeFretboard-0.0.3/pyproject.toml
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-24 18:29:22.951982 seeFretboard-0.0.3/seeFretboard/
--rw-r--r--   0 lindazhang   (501) staff       (20)      349 2023-05-23 16:52:09.000000 seeFretboard-0.0.3/seeFretboard/NotePosition.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     1002 2023-05-24 15:44:17.000000 seeFretboard-0.0.3/seeFretboard/PathInfo.py
--rw-r--r--   0 lindazhang   (501) staff       (20)     7371 2023-05-23 15:53:29.000000 seeFretboard-0.0.3/seeFretboard/PitchCollection.py
--rw-r--r--   0 lindazhang   (501) staff       (20)    49032 2023-05-24 17:25:46.000000 seeFretboard-0.0.3/seeFretboard/SeeFretboard.py
--rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-05-23 07:07:14.000000 seeFretboard-0.0.3/seeFretboard/__init__.py
--rw-r--r--   0 lindazhang   (501) staff       (20)      430 2023-05-24 17:03:19.000000 seeFretboard-0.0.3/seeFretboard/generalTest.py
-drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-24 18:29:22.952822 seeFretboard-0.0.3/seeFretboard.egg-info/
--rw-r--r--   0 lindazhang   (501) staff       (20)     1370 2023-05-24 18:29:22.000000 seeFretboard-0.0.3/seeFretboard.egg-info/PKG-INFO
--rw-r--r--   0 lindazhang   (501) staff       (20)      400 2023-05-24 18:29:22.000000 seeFretboard-0.0.3/seeFretboard.egg-info/SOURCES.txt
--rw-r--r--   0 lindazhang   (501) staff       (20)        1 2023-05-24 18:29:22.000000 seeFretboard-0.0.3/seeFretboard.egg-info/dependency_links.txt
--rw-r--r--   0 lindazhang   (501) staff       (20)        9 2023-05-24 18:29:22.000000 seeFretboard-0.0.3/seeFretboard.egg-info/requires.txt
--rw-r--r--   0 lindazhang   (501) staff       (20)       13 2023-05-24 18:29:22.000000 seeFretboard-0.0.3/seeFretboard.egg-info/top_level.txt
--rw-r--r--   0 lindazhang   (501) staff       (20)       38 2023-05-24 18:29:22.953401 seeFretboard-0.0.3/setup.cfg
--rw-r--r--   0 lindazhang   (501) staff       (20)      628 2023-05-24 18:23:48.000000 seeFretboard-0.0.3/setup.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-24 18:57:15.569078 seeFretboard-0.0.4/
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-24 18:57:15.563807 seeFretboard-0.0.4/Designs/
+-rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-05-24 06:03:38.000000 seeFretboard-0.0.4/Designs/Buttons.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2163 2023-05-23 16:51:07.000000 seeFretboard-0.0.4/Designs/CirlceNote.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3207 2023-05-24 16:53:11.000000 seeFretboard-0.0.4/Designs/FretboardFigure.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     6610 2023-05-23 21:33:59.000000 seeFretboard-0.0.4/Designs/FretboardStyle.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-05-23 07:10:21.000000 seeFretboard-0.0.4/Designs/__init__.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-24 18:57:15.565957 seeFretboard-0.0.4/Examples/
+-rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-05-24 18:55:42.000000 seeFretboard-0.0.4/Examples/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      602 2023-05-17 18:35:46.000000 seeFretboard-0.0.4/Examples/arpeggio.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      554 2023-05-23 22:12:06.000000 seeFretboard-0.0.4/Examples/createMidiAudio.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      754 2023-05-24 06:43:40.000000 seeFretboard-0.0.4/Examples/createVideo.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      829 2023-05-24 06:45:32.000000 seeFretboard-0.0.4/Examples/createVideoWithAudio.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1013 2023-05-24 06:41:18.000000 seeFretboard-0.0.4/Examples/createVideoWithMidiAudio.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      416 2023-05-24 13:28:52.000000 seeFretboard-0.0.4/Examples/figureNextToEachOther.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      438 2023-05-24 15:45:15.000000 seeFretboard-0.0.4/Examples/generateScriptAndDiv.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      278 2023-05-24 15:59:25.000000 seeFretboard-0.0.4/Examples/generateStandalone.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      421 2023-05-16 18:33:07.000000 seeFretboard-0.0.4/Examples/groundtruthVPredictionTest.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      239 2023-05-16 18:33:07.000000 seeFretboard-0.0.4/Examples/horizontalFretboard.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      282 2023-05-16 17:18:49.000000 seeFretboard-0.0.4/Examples/horizontalFretboardAddNotes.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      492 2023-05-16 18:32:52.000000 seeFretboard-0.0.4/Examples/interval.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      648 2023-05-23 17:47:04.000000 seeFretboard-0.0.4/Examples/saveVideoWithAudio.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      825 2023-05-17 13:39:03.000000 seeFretboard-0.0.4/Examples/scale.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      980 2023-05-16 18:32:51.000000 seeFretboard-0.0.4/Examples/testText.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      238 2023-05-16 18:32:51.000000 seeFretboard-0.0.4/Examples/verticalFretboard.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      282 2023-05-16 18:32:51.000000 seeFretboard-0.0.4/Examples/verticalFretboardAddNotes.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-24 18:57:15.566068 seeFretboard-0.0.4/GuitarSet/
+-rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-05-24 18:56:04.000000 seeFretboard-0.0.4/GuitarSet/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1072 2023-05-24 18:18:02.000000 seeFretboard-0.0.4/LICENSE
+-rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-05-24 18:19:53.000000 seeFretboard-0.0.4/MANIFEST.in
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-24 18:57:15.566156 seeFretboard-0.0.4/Outputs/
+-rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-05-24 18:55:54.000000 seeFretboard-0.0.4/Outputs/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1370 2023-05-24 18:57:15.568933 seeFretboard-0.0.4/PKG-INFO
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1005 2023-05-02 18:53:11.000000 seeFretboard-0.0.4/README.md
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-24 18:57:15.566618 seeFretboard-0.0.4/Tests/
+-rw-r--r--   0 lindazhang   (501) staff       (20)     7163 2023-05-24 07:07:44.000000 seeFretboard-0.0.4/Tests/StylesTest.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-05-24 18:56:48.000000 seeFretboard-0.0.4/Tests/__init__.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-24 18:57:15.566964 seeFretboard-0.0.4/Utilities/
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1760 2023-05-24 16:11:25.000000 seeFretboard-0.0.4/Utilities/Constants.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     3532 2023-05-23 05:52:24.000000 seeFretboard-0.0.4/Utilities/Util.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)        0 2023-05-23 21:33:25.000000 seeFretboard-0.0.4/Utilities/__init__.py
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-24 18:57:15.568088 seeFretboard-0.0.4/Videos/
+-rw-r--r--   0 lindazhang   (501) staff       (20)     2731 2023-05-24 04:39:52.000000 seeFretboard-0.0.4/Videos/Audio.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      377 2023-04-26 17:58:37.000000 seeFretboard-0.0.4/Videos/Frame.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1035 2023-05-24 05:48:56.000000 seeFretboard-0.0.4/Videos/Images.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     7079 2023-05-24 06:00:03.000000 seeFretboard-0.0.4/Videos/TabSequence.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4603 2023-05-24 06:46:51.000000 seeFretboard-0.0.4/Videos/Video.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)     4093 2023-05-24 06:41:15.000000 seeFretboard-0.0.4/Videos/VideoManager.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      549 2023-05-24 16:47:03.000000 seeFretboard-0.0.4/Videos/VideoNote.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      212 2023-05-24 05:31:37.000000 seeFretboard-0.0.4/Videos/__init__.py
+-rw-r--r--   0 lindazhang   (501) staff       (20)      287 2023-05-24 18:45:11.000000 seeFretboard-0.0.4/pyproject.toml
+drwxr-xr-x   0 lindazhang   (501) staff       (20)        0 2023-05-24 18:57:15.568740 seeFretboard-0.0.4/seeFretboard.egg-info/
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1370 2023-05-24 18:57:15.000000 seeFretboard-0.0.4/seeFretboard.egg-info/PKG-INFO
+-rw-r--r--   0 lindazhang   (501) staff       (20)     1170 2023-05-24 18:57:15.000000 seeFretboard-0.0.4/seeFretboard.egg-info/SOURCES.txt
+-rw-r--r--   0 lindazhang   (501) staff       (20)        1 2023-05-24 18:57:15.000000 seeFretboard-0.0.4/seeFretboard.egg-info/dependency_links.txt
+-rw-r--r--   0 lindazhang   (501) staff       (20)        9 2023-05-24 18:57:15.000000 seeFretboard-0.0.4/seeFretboard.egg-info/requires.txt
+-rw-r--r--   0 lindazhang   (501) staff       (20)       58 2023-05-24 18:57:15.000000 seeFretboard-0.0.4/seeFretboard.egg-info/top_level.txt
+-rw-r--r--   0 lindazhang   (501) staff       (20)       38 2023-05-24 18:57:15.569225 seeFretboard-0.0.4/setup.cfg
+-rw-r--r--   0 lindazhang   (501) staff       (20)      658 2023-05-24 18:53:52.000000 seeFretboard-0.0.4/setup.py
```

### Comparing `seeFretboard-0.0.3/LICENSE` & `seeFretboard-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.3/PKG-INFO` & `seeFretboard-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seeFretboard
-Version: 0.0.3
+Version: 0.0.4
 Summary: Testing installation of Package
 Home-page: https://github.com/LindaRZhang/seeFretboard
 Author: Linda Rong Zhang
 Author-email: ronglindaz@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/LindaRZhang/seeFretboard/issues
 Description-Content-Type: text/markdown
```

### Comparing `seeFretboard-0.0.3/README.md` & `seeFretboard-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `seeFretboard-0.0.3/seeFretboard.egg-info/PKG-INFO` & `seeFretboard-0.0.4/seeFretboard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seeFretboard
-Version: 0.0.3
+Version: 0.0.4
 Summary: Testing installation of Package
 Home-page: https://github.com/LindaRZhang/seeFretboard
 Author: Linda Rong Zhang
 Author-email: ronglindaz@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/LindaRZhang/seeFretboard/issues
 Description-Content-Type: text/markdown
```

### Comparing `seeFretboard-0.0.3/setup.py` & `seeFretboard-0.0.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-import setuptools
+from setuptools import setuptools, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='seeFretboard',
-    version='0.0.3',
+    version='0.0.4',
     author='Linda Rong Zhang',
     author_email='ronglindaz@gmail.com',
     description='Testing installation of Package',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/LindaRZhang/seeFretboard',
     project_urls = {
         "Bug Tracker": "https://github.com/LindaRZhang/seeFretboard/issues"
     },
     license='MIT',
-    packages=['seeFretboard'],
+    packages=find_packages(),
     install_requires=['requests'],
 )
```

