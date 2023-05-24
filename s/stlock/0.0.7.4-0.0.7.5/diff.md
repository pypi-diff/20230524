# Comparing `tmp/stlock-0.0.7.4.tar.gz` & `tmp/stlock-0.0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stlock-0.0.7.4.tar", last modified: Wed May 24 10:37:43 2023, max compression
+gzip compressed data, was "stlock-0.0.7.5.tar", last modified: Wed May 24 10:38:53 2023, max compression
```

## Comparing `stlock-0.0.7.4.tar` & `stlock-0.0.7.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-24 10:37:43.790477 stlock-0.0.7.4/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     5749 2023-05-24 10:37:43.790477 stlock-0.0.7.4/PKG-INFO
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     5180 2023-05-24 10:37:34.000000 stlock-0.0.7.4/README.md
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       38 2023-05-24 10:37:43.790477 stlock-0.0.7.4/setup.cfg
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      933 2023-05-24 10:37:42.000000 stlock-0.0.7.4/setup.py
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-24 10:37:43.790477 stlock-0.0.7.4/stlock/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       31 2023-05-22 16:05:24.000000 stlock-0.0.7.4/stlock/__init__.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     2138 2023-05-23 15:50:14.000000 stlock-0.0.7.4/stlock/stlock.py
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-24 10:37:43.790477 stlock-0.0.7.4/stlock.egg-info/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     5749 2023-05-24 10:37:43.000000 stlock-0.0.7.4/stlock.egg-info/PKG-INFO
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      242 2023-05-24 10:37:43.000000 stlock-0.0.7.4/stlock.egg-info/SOURCES.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        1 2023-05-24 10:37:43.000000 stlock-0.0.7.4/stlock.egg-info/dependency_links.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        1 2023-05-22 16:50:38.000000 stlock-0.0.7.4/stlock.egg-info/not-zip-safe
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       15 2023-05-24 10:37:43.000000 stlock-0.0.7.4/stlock.egg-info/requires.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        7 2023-05-24 10:37:43.000000 stlock-0.0.7.4/stlock.egg-info/top_level.txt
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-24 10:38:53.490804 stlock-0.0.7.5/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     5759 2023-05-24 10:38:53.490804 stlock-0.0.7.5/PKG-INFO
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     5190 2023-05-24 10:38:43.000000 stlock-0.0.7.5/README.md
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       38 2023-05-24 10:38:53.490804 stlock-0.0.7.5/setup.cfg
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      933 2023-05-24 10:38:52.000000 stlock-0.0.7.5/setup.py
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-24 10:38:53.490804 stlock-0.0.7.5/stlock/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       31 2023-05-22 16:05:24.000000 stlock-0.0.7.5/stlock/__init__.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     2138 2023-05-23 15:50:14.000000 stlock-0.0.7.5/stlock/stlock.py
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-24 10:38:53.490804 stlock-0.0.7.5/stlock.egg-info/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     5759 2023-05-24 10:38:53.000000 stlock-0.0.7.5/stlock.egg-info/PKG-INFO
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      242 2023-05-24 10:38:53.000000 stlock-0.0.7.5/stlock.egg-info/SOURCES.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        1 2023-05-24 10:38:53.000000 stlock-0.0.7.5/stlock.egg-info/dependency_links.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        1 2023-05-22 16:50:38.000000 stlock-0.0.7.5/stlock.egg-info/not-zip-safe
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       15 2023-05-24 10:38:53.000000 stlock-0.0.7.5/stlock.egg-info/requires.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        7 2023-05-24 10:38:53.000000 stlock-0.0.7.5/stlock.egg-info/top_level.txt
```

### Comparing `stlock-0.0.7.4/PKG-INFO` & `stlock-0.0.7.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: stlock
-Version: 0.0.7.4
+Version: 0.0.7.5
 Summary: oauth2.0 stlock
 Author: Smart Techno Lab
 Author-email: office@stl.im
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 3 - Alpha
 Description-Content-Type: text/markdown
 
-Библиотека для сервиса авторизации STLock (powered by SmartTechnoLab)
+Библиотека для сервиса авторизации **STLock** *(powered by **SmartTechnoLab**)*
 
 **Статус:** *В разработке*
 
 # Библиотека Python STLock
 
 
 # Быстрый старт
```

### Comparing `stlock-0.0.7.4/README.md` & `stlock-0.0.7.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Библиотека для сервиса авторизации STLock (powered by SmartTechnoLab)
+Библиотека для сервиса авторизации **STLock** *(powered by **SmartTechnoLab**)*
 
 **Статус:** *В разработке*
 
 # Библиотека Python STLock
 
 
 # Быстрый старт
```

### Comparing `stlock-0.0.7.4/setup.py` & `stlock-0.0.7.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 setup(name='stlock',
-      version='0.0.7.4',
+      version='0.0.7.5',
       description='oauth2.0 stlock\nTest description\nBlah blah blah',
       packages=['stlock'],
       author="Smart Techno Lab",
       author_email='office@stl.im',
       zip_safe=False,
       install_requires=["requests", "pyjwt"],
       long_description=long_description,
```

### Comparing `stlock-0.0.7.4/stlock/stlock.py` & `stlock-0.0.7.5/stlock/stlock.py`

 * *Files identical despite different names*

### Comparing `stlock-0.0.7.4/stlock.egg-info/PKG-INFO` & `stlock-0.0.7.5/stlock.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: stlock
-Version: 0.0.7.4
+Version: 0.0.7.5
 Summary: oauth2.0 stlock
 Author: Smart Techno Lab
 Author-email: office@stl.im
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 3 - Alpha
 Description-Content-Type: text/markdown
 
-Библиотека для сервиса авторизации STLock (powered by SmartTechnoLab)
+Библиотека для сервиса авторизации **STLock** *(powered by **SmartTechnoLab**)*
 
 **Статус:** *В разработке*
 
 # Библиотека Python STLock
 
 
 # Быстрый старт
```

