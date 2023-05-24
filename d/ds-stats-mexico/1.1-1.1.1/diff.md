# Comparing `tmp/ds_stats_mexico-1.1.tar.gz` & `tmp/ds_stats_mexico-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ds_stats_mexico-1.1.tar", last modified: Wed May 24 06:26:23 2023, max compression
+gzip compressed data, was "ds_stats_mexico-1.1.1.tar", last modified: Wed May 24 06:28:08 2023, max compression
```

## Comparing `ds_stats_mexico-1.1.tar` & `ds_stats_mexico-1.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 06:26:23.982703 ds_stats_mexico-1.1/
--rw-rw-rw-   0        0        0      291 2023-05-24 06:26:23.982703 ds_stats_mexico-1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-24 06:26:23.977706 ds_stats_mexico-1.1/ds_stats_mexico/
--rw-rw-rw-   0        0        0      257 2023-05-24 06:07:03.000000 ds_stats_mexico-1.1/ds_stats_mexico/__init__.py
--rw-rw-rw-   0        0        0     1679 2023-05-24 06:17:32.000000 ds_stats_mexico-1.1/ds_stats_mexico/functions.py
-drwxrwxrwx   0        0        0        0 2023-05-24 06:26:23.981703 ds_stats_mexico-1.1/ds_stats_mexico.egg-info/
--rw-rw-rw-   0        0        0      291 2023-05-24 06:26:23.000000 ds_stats_mexico-1.1/ds_stats_mexico.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2023-05-24 06:26:23.000000 ds_stats_mexico-1.1/ds_stats_mexico.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 06:26:23.000000 ds_stats_mexico-1.1/ds_stats_mexico.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-24 06:26:23.000000 ds_stats_mexico-1.1/ds_stats_mexico.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-24 06:26:23.000000 ds_stats_mexico-1.1/ds_stats_mexico.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-24 06:26:23.982703 ds_stats_mexico-1.1/setup.cfg
--rw-rw-rw-   0        0        0      904 2023-05-24 06:26:20.000000 ds_stats_mexico-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 06:28:08.366962 ds_stats_mexico-1.1.1/
+-rw-rw-rw-   0        0        0     1147 2023-05-24 06:28:08.366962 ds_stats_mexico-1.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-24 06:28:08.361839 ds_stats_mexico-1.1.1/ds_stats_mexico/
+-rw-rw-rw-   0        0        0      257 2023-05-24 06:07:03.000000 ds_stats_mexico-1.1.1/ds_stats_mexico/__init__.py
+-rw-rw-rw-   0        0        0     1679 2023-05-24 06:17:32.000000 ds_stats_mexico-1.1.1/ds_stats_mexico/functions.py
+drwxrwxrwx   0        0        0        0 2023-05-24 06:28:08.365957 ds_stats_mexico-1.1.1/ds_stats_mexico.egg-info/
+-rw-rw-rw-   0        0        0     1147 2023-05-24 06:28:08.000000 ds_stats_mexico-1.1.1/ds_stats_mexico.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-05-24 06:28:08.000000 ds_stats_mexico-1.1.1/ds_stats_mexico.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 06:28:08.000000 ds_stats_mexico-1.1.1/ds_stats_mexico.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-24 06:28:08.000000 ds_stats_mexico-1.1.1/ds_stats_mexico.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-24 06:28:08.000000 ds_stats_mexico-1.1.1/ds_stats_mexico.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-24 06:28:08.366962 ds_stats_mexico-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1058 2023-05-24 06:27:58.000000 ds_stats_mexico-1.1.1/setup.py
```

### Comparing `ds_stats_mexico-1.1/ds_stats_mexico/functions.py` & `ds_stats_mexico-1.1.1/ds_stats_mexico/functions.py`

 * *Files identical despite different names*

### Comparing `ds_stats_mexico-1.1/setup.py` & `ds_stats_mexico-1.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '1.1'
+VERSION = '1.1.1'
 PACKAGE_NAME = 'ds_stats_mexico'
 AUTHOR = 'DavichoStar'
 AUTHOR_EMAIL = 'davichostar@protonmail.com'
 URL = 'https://github.com/DavichoStar'
 
 LICENSE = 'MIT'
 DESCRIPTION = 'Librería de estadística (Gráficas) de México (Paises ricos, envejecimiento, mortalidad infantil)'
@@ -18,14 +18,16 @@
     'matplotlib'
 ]
 
 setup(
     name=PACKAGE_NAME,
     version=VERSION,
     description=DESCRIPTION,
+    long_description=LONG_DESCRIPTION,
+    long_description_content_type='text/markdown',  # Este es importante para que se muestre bien el README.md
     author=AUTHOR,
     author_email=AUTHOR_EMAIL,
     url=URL,
     install_requires=INSTALL_REQUIRES,
     license=LICENSE,
     packages=find_packages(),
     include_package_data=True
```

