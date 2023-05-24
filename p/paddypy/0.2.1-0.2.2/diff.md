# Comparing `tmp/paddypy-0.2.1.tar.gz` & `tmp/paddypy-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paddypy-0.2.1.tar", last modified: Fri May  5 09:10:26 2023, max compression
+gzip compressed data, was "paddypy-0.2.2.tar", last modified: Wed May 24 09:00:33 2023, max compression
```

## Comparing `paddypy-0.2.1.tar` & `paddypy-0.2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 09:10:26.633408 paddypy-0.2.1/
--rw-rw-rw-   0        0        0     1150 2022-05-16 06:26:09.000000 paddypy-0.2.1/LICENSE
--rw-rw-rw-   0        0        0     1795 2023-05-05 09:10:26.632910 paddypy-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      918 2023-04-17 10:33:45.000000 paddypy-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 09:10:26.619409 paddypy-0.2.1/paddypy/
--rw-rw-rw-   0        0        0      102 2023-04-17 12:26:22.000000 paddypy-0.2.1/paddypy/__init__.py
--rw-rw-rw-   0        0        0     5772 2023-04-17 12:26:22.000000 paddypy-0.2.1/paddypy/access.py
--rw-rw-rw-   0        0        0     5064 2023-05-05 09:10:04.000000 paddypy-0.2.1/paddypy/log.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:10:26.631408 paddypy-0.2.1/paddypy.egg-info/
--rw-rw-rw-   0        0        0     1795 2023-05-05 09:10:26.000000 paddypy-0.2.1/paddypy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-05-05 09:10:26.000000 paddypy-0.2.1/paddypy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 09:10:26.000000 paddypy-0.2.1/paddypy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      127 2023-05-05 09:10:26.000000 paddypy-0.2.1/paddypy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-05 09:10:26.000000 paddypy-0.2.1/paddypy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-05 09:10:26.633408 paddypy-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1480 2023-05-05 09:07:24.000000 paddypy-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:00:33.163735 paddypy-0.2.2/
+-rw-rw-rw-   0        0        0     1150 2022-05-16 06:26:09.000000 paddypy-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0     1795 2023-05-24 09:00:33.163232 paddypy-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0      918 2023-04-17 10:33:45.000000 paddypy-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-24 09:00:33.143235 paddypy-0.2.2/paddypy/
+-rw-rw-rw-   0        0        0      102 2023-04-17 12:26:22.000000 paddypy-0.2.2/paddypy/__init__.py
+-rw-rw-rw-   0        0        0     5772 2023-04-17 12:26:22.000000 paddypy-0.2.2/paddypy/access.py
+-rw-rw-rw-   0        0        0     8275 2023-05-24 08:59:47.000000 paddypy-0.2.2/paddypy/log.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:00:33.162231 paddypy-0.2.2/paddypy.egg-info/
+-rw-rw-rw-   0        0        0     1795 2023-05-24 09:00:32.000000 paddypy-0.2.2/paddypy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-05-24 09:00:33.000000 paddypy-0.2.2/paddypy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 09:00:32.000000 paddypy-0.2.2/paddypy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      127 2023-05-24 09:00:32.000000 paddypy-0.2.2/paddypy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-24 09:00:32.000000 paddypy-0.2.2/paddypy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-24 09:00:33.163735 paddypy-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1480 2023-05-24 08:46:28.000000 paddypy-0.2.2/setup.py
```

### Comparing `paddypy-0.2.1/LICENSE` & `paddypy-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `paddypy-0.2.1/PKG-INFO` & `paddypy-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paddypy
-Version: 0.2.1
+Version: 0.2.2
 Summary: Collection of helpfull extensions
 Author: Patrik
 Author-email: <patrikhartl@gmail.com>
 Keywords: python,appconfiguration,azure
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `paddypy-0.2.1/README.md` & `paddypy-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `paddypy-0.2.1/paddypy/access.py` & `paddypy-0.2.2/paddypy/access.py`

 * *Files identical despite different names*

### Comparing `paddypy-0.2.1/paddypy.egg-info/PKG-INFO` & `paddypy-0.2.2/paddypy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paddypy
-Version: 0.2.1
+Version: 0.2.2
 Summary: Collection of helpfull extensions
 Author: Patrik
 Author-email: <patrikhartl@gmail.com>
 Keywords: python,appconfiguration,azure
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `paddypy-0.2.1/setup.py` & `paddypy-0.2.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.2.1'
+VERSION = '0.2.2'
 DESCRIPTION = 'Collection of helpfull extensions'
 LONG_DESCRIPTION = 'Collection of helpfull extensions'
 
 # Setting up
 setup(
     name="paddypy",
     version=VERSION,
```

