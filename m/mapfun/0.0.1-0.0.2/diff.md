# Comparing `tmp/mapfun-0.0.1.tar.gz` & `tmp/mapfun-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapfun-0.0.1.tar", last modified: Tue May 23 15:45:10 2023, max compression
+gzip compressed data, was "mapfun-0.0.2.tar", last modified: Tue May 23 17:26:45 2023, max compression
```

## Comparing `mapfun-0.0.1.tar` & `mapfun-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 15:45:10.533780 mapfun-0.0.1/
--rw-rw-rw-   0        0        0     1094 2023-05-22 09:15:01.000000 mapfun-0.0.1/LICENCE
--rw-rw-rw-   0        0        0      714 2023-05-23 15:45:10.533780 mapfun-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      884 2023-05-22 09:15:01.000000 mapfun-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-23 15:45:10.518139 mapfun-0.0.1/mapfun.egg-info/
--rw-rw-rw-   0        0        0      714 2023-05-23 15:45:09.000000 mapfun-0.0.1/mapfun.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      169 2023-05-23 15:45:10.000000 mapfun-0.0.1/mapfun.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 15:45:09.000000 mapfun-0.0.1/mapfun.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-05-23 15:45:10.000000 mapfun-0.0.1/mapfun.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-23 15:45:10.533780 mapfun-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      927 2023-05-23 15:33:45.000000 mapfun-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-23 15:45:10.501972 mapfun-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-23 15:45:10.533780 mapfun-0.0.1/src/mapfun/
--rw-rw-rw-   0        0        0     1093 2023-05-23 14:54:05.000000 mapfun-0.0.1/src/mapfun/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 17:26:45.687098 mapfun-0.0.2/
+-rw-rw-rw-   0        0        0     1094 2023-05-23 16:05:12.000000 mapfun-0.0.2/LICENCE
+-rw-rw-rw-   0        0        0     1393 2023-05-23 17:26:45.687098 mapfun-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      884 2023-05-23 16:05:12.000000 mapfun-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 17:26:45.671459 mapfun-0.0.2/mapfun.egg-info/
+-rw-rw-rw-   0        0        0     1393 2023-05-23 17:26:44.000000 mapfun-0.0.2/mapfun.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      169 2023-05-23 17:26:45.000000 mapfun-0.0.2/mapfun.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 17:26:44.000000 mapfun-0.0.2/mapfun.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-05-23 17:26:45.000000 mapfun-0.0.2/mapfun.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-23 17:26:45.687098 mapfun-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1005 2023-05-23 17:23:35.000000 mapfun-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 17:26:45.671459 mapfun-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-23 17:26:45.671459 mapfun-0.0.2/src/mapfun/
+-rw-rw-rw-   0        0        0     1085 2023-05-23 16:05:12.000000 mapfun-0.0.2/src/mapfun/__init__.py
```

### Comparing `mapfun-0.0.1/LICENCE` & `mapfun-0.0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `mapfun-0.0.1/README.md` & `mapfun-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `mapfun-0.0.1/setup.py` & `mapfun-0.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from setuptools import setup
-
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'mapfun'
-LONG_DESCRIPTION = 'A function that applies a mapping function to an infinite number of input elements, with options to skip certain elements and selectively apply the mapping to keys and/or values of objects.'
-
+#LONG_DESCRIPTION = 'A function that applies a mapping function to an infinite number of input elements, with options to skip certain elements and selectively apply the mapping to keys and/or values of objects.'
 # Setting up
+from pathlib import Path
+this_directory = Path(__file__).parent
+LONG_DESCRIPTION = (this_directory / "README.md").read_text()
 setup(
     name="mapfun",
     version=VERSION,
     author="Zakaria Elalaoui",
-    author_email="",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages = ['src.mapfun'],
-    install_requires=[],
     keywords=['python', 'map'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

### Comparing `mapfun-0.0.1/src/mapfun/__init__.py` & `mapfun-0.0.2/src/mapfun/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,8 +22,7 @@
         if isinstance(x, (tuple, range)):
             return type(x)(mapRecursive(n) for n in x)
         if isinstance(x, object):
             return fun(x)
         else:
             raise ValueError('Uncategorized data')
     return [mapRecursive(x) for x in X]
-print(1)
```

