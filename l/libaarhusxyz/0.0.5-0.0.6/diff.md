# Comparing `tmp/libaarhusxyz-0.0.5.tar.gz` & `tmp/libaarhusxyz-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/libaarhusxyz-0.0.5.tar", last modified: Fri Apr 29 08:08:30 2022, max compression
+gzip compressed data, was "dist/libaarhusxyz-0.0.6.tar", last modified: Tue May 10 14:02:42 2022, max compression
```

## Comparing `libaarhusxyz-0.0.5.tar` & `libaarhusxyz-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2022-04-29 08:08:30.000000 libaarhusxyz-0.0.5/
--rw-rw-r--   0 redhog    (1000) redhog    (1000)      635 2022-04-29 08:07:38.000000 libaarhusxyz-0.0.5/setup.py
--rw-rw-r--   0 redhog    (1000) redhog    (1000)      455 2022-04-29 08:08:30.000000 libaarhusxyz-0.0.5/PKG-INFO
-drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2022-04-29 08:08:30.000000 libaarhusxyz-0.0.5/libaarhusxyz/
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     6886 2022-04-27 09:03:49.000000 libaarhusxyz-0.0.5/libaarhusxyz/vtk.py
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     2079 2022-01-06 11:17:32.000000 libaarhusxyz-0.0.5/libaarhusxyz/gex.py
--rw-rw-r--   0 redhog    (1000) redhog    (1000)      118 2022-01-06 11:17:32.000000 libaarhusxyz-0.0.5/libaarhusxyz/__init__.py
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     1958 2021-11-11 08:18:52.000000 libaarhusxyz-0.0.5/libaarhusxyz/transforms.py
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     2241 2022-04-28 14:05:56.000000 libaarhusxyz-0.0.5/libaarhusxyz/alc.py
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     1074 2022-01-06 11:17:32.000000 libaarhusxyz-0.0.5/libaarhusxyz/sr2.py
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     5787 2022-04-29 08:06:37.000000 libaarhusxyz-0.0.5/libaarhusxyz/xyz.py
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     1077 2021-07-29 09:04:04.000000 libaarhusxyz-0.0.5/LICENSE
--rw-rw-r--   0 redhog    (1000) redhog    (1000)       38 2022-04-29 08:08:30.000000 libaarhusxyz-0.0.5/setup.cfg
-drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2022-04-29 08:08:30.000000 libaarhusxyz-0.0.5/libaarhusxyz.egg-info/
--rw-rw-r--   0 redhog    (1000) redhog    (1000)      455 2022-04-29 08:08:30.000000 libaarhusxyz-0.0.5/libaarhusxyz.egg-info/PKG-INFO
--rw-rw-r--   0 redhog    (1000) redhog    (1000)        1 2022-04-29 08:08:30.000000 libaarhusxyz-0.0.5/libaarhusxyz.egg-info/dependency_links.txt
--rw-rw-r--   0 redhog    (1000) redhog    (1000)       13 2022-04-29 08:08:30.000000 libaarhusxyz-0.0.5/libaarhusxyz.egg-info/top_level.txt
--rw-rw-r--   0 redhog    (1000) redhog    (1000)       13 2022-04-29 08:08:30.000000 libaarhusxyz-0.0.5/libaarhusxyz.egg-info/requires.txt
--rw-rw-r--   0 redhog    (1000) redhog    (1000)      357 2022-04-29 08:08:30.000000 libaarhusxyz-0.0.5/libaarhusxyz.egg-info/SOURCES.txt
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     3283 2022-04-28 14:06:26.000000 libaarhusxyz-0.0.5/README.md
+drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2022-05-10 14:02:42.665254 libaarhusxyz-0.0.6/
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     1077 2021-07-29 09:04:04.000000 libaarhusxyz-0.0.6/LICENSE
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)      466 2022-05-10 14:02:42.665254 libaarhusxyz-0.0.6/PKG-INFO
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     3283 2022-04-28 14:06:26.000000 libaarhusxyz-0.0.6/README.md
+drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2022-05-10 14:02:42.665254 libaarhusxyz-0.0.6/libaarhusxyz/
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)      139 2022-04-29 13:14:30.000000 libaarhusxyz-0.0.6/libaarhusxyz/__init__.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     2241 2022-04-28 14:05:56.000000 libaarhusxyz-0.0.6/libaarhusxyz/alc.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     2079 2022-01-06 11:17:32.000000 libaarhusxyz-0.0.6/libaarhusxyz/gex.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     1074 2022-01-06 11:17:32.000000 libaarhusxyz-0.0.6/libaarhusxyz/sr2.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     1958 2021-11-11 08:18:52.000000 libaarhusxyz-0.0.6/libaarhusxyz/transforms.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     6886 2022-04-27 09:03:49.000000 libaarhusxyz-0.0.6/libaarhusxyz/vtk.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)    10135 2022-05-10 13:57:57.000000 libaarhusxyz-0.0.6/libaarhusxyz/xyz.py
+drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2022-05-10 14:02:42.665254 libaarhusxyz-0.0.6/libaarhusxyz.egg-info/
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)      466 2022-05-10 14:02:42.000000 libaarhusxyz-0.0.6/libaarhusxyz.egg-info/PKG-INFO
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)      357 2022-05-10 14:02:42.000000 libaarhusxyz-0.0.6/libaarhusxyz.egg-info/SOURCES.txt
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)        1 2022-05-10 14:02:42.000000 libaarhusxyz-0.0.6/libaarhusxyz.egg-info/dependency_links.txt
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)       13 2022-05-10 14:02:42.000000 libaarhusxyz-0.0.6/libaarhusxyz.egg-info/requires.txt
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)       13 2022-05-10 14:02:42.000000 libaarhusxyz-0.0.6/libaarhusxyz.egg-info/top_level.txt
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)       38 2022-05-10 14:02:42.665254 libaarhusxyz-0.0.6/setup.cfg
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)      635 2022-05-10 14:01:59.000000 libaarhusxyz-0.0.6/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `libaarhusxyz-0.0.5/setup.py` & `libaarhusxyz-0.0.6/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 
 import setuptools
 import os
 
 setuptools.setup(
     name='libaarhusxyz',
-    version='0.0.5',
+    version='0.0.6',
     description='Parser for the Aarhus Workbench XYZ format for geophysical data',
     long_description="""Parser for the Aarhus Workbench XYZ format for geophysical data""",
     long_description_content_type="text/markdown",
     author='Egil Moeller, Craig William Christensen and others ',
     author_email='em@emeraldgeo.no, cch@emeraldgeo.no',
     url='https://github.com/emerald-geomodelling/libaarhusxyz',
     packages=setuptools.find_packages(),
```

### Comparing `libaarhusxyz-0.0.5/libaarhusxyz/vtk.py` & `libaarhusxyz-0.0.6/libaarhusxyz/vtk.py`

 * *Files identical despite different names*

### Comparing `libaarhusxyz-0.0.5/libaarhusxyz/gex.py` & `libaarhusxyz-0.0.6/libaarhusxyz/gex.py`

 * *Files identical despite different names*

### Comparing `libaarhusxyz-0.0.5/libaarhusxyz/transforms.py` & `libaarhusxyz-0.0.6/libaarhusxyz/transforms.py`

 * *Files identical despite different names*

### Comparing `libaarhusxyz-0.0.5/libaarhusxyz/alc.py` & `libaarhusxyz-0.0.6/libaarhusxyz/alc.py`

 * *Files identical despite different names*

### Comparing `libaarhusxyz-0.0.5/libaarhusxyz/sr2.py` & `libaarhusxyz-0.0.6/libaarhusxyz/sr2.py`

 * *Files identical despite different names*

### Comparing `libaarhusxyz-0.0.5/LICENSE` & `libaarhusxyz-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `libaarhusxyz-0.0.5/README.md` & `libaarhusxyz-0.0.6/README.md`

 * *Files identical despite different names*

