# Comparing `tmp/mapfun-0.0.2.tar.gz` & `tmp/mapfun-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapfun-0.0.2.tar", last modified: Tue May 23 17:26:45 2023, max compression
+gzip compressed data, was "mapfun-0.0.3.tar", last modified: Wed May 24 15:11:47 2023, max compression
```

## Comparing `mapfun-0.0.2.tar` & `mapfun-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 17:26:45.687098 mapfun-0.0.2/
--rw-rw-rw-   0        0        0     1094 2023-05-23 16:05:12.000000 mapfun-0.0.2/LICENCE
--rw-rw-rw-   0        0        0     1393 2023-05-23 17:26:45.687098 mapfun-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      884 2023-05-23 16:05:12.000000 mapfun-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-23 17:26:45.671459 mapfun-0.0.2/mapfun.egg-info/
--rw-rw-rw-   0        0        0     1393 2023-05-23 17:26:44.000000 mapfun-0.0.2/mapfun.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      169 2023-05-23 17:26:45.000000 mapfun-0.0.2/mapfun.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 17:26:44.000000 mapfun-0.0.2/mapfun.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-05-23 17:26:45.000000 mapfun-0.0.2/mapfun.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-23 17:26:45.687098 mapfun-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1005 2023-05-23 17:23:35.000000 mapfun-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-23 17:26:45.671459 mapfun-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-23 17:26:45.671459 mapfun-0.0.2/src/mapfun/
--rw-rw-rw-   0        0        0     1085 2023-05-23 16:05:12.000000 mapfun-0.0.2/src/mapfun/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:11:47.456429 mapfun-0.0.3/
+-rw-rw-rw-   0        0        0     1094 2023-05-24 15:08:54.000000 mapfun-0.0.3/LICENCE
+-rw-rw-rw-   0        0        0      523 2023-05-24 15:11:47.456429 mapfun-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2258 2023-05-24 15:08:54.000000 mapfun-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-24 15:11:47.451463 mapfun-0.0.3/mapfun.egg-info/
+-rw-rw-rw-   0        0        0      523 2023-05-24 15:11:46.000000 mapfun-0.0.3/mapfun.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      160 2023-05-24 15:11:47.000000 mapfun-0.0.3/mapfun.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 15:11:46.000000 mapfun-0.0.3/mapfun.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-05-24 15:11:46.000000 mapfun-0.0.3/mapfun.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-24 15:11:47.456429 mapfun-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      701 2023-05-24 15:11:35.000000 mapfun-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:11:47.454568 mapfun-0.0.3/src/
+-rw-rw-rw-   0        0        0     1085 2023-05-24 15:08:54.000000 mapfun-0.0.3/src/mapfun.py
```

### Comparing `mapfun-0.0.2/LICENCE` & `mapfun-0.0.3/LICENCE`

 * *Files identical despite different names*

### Comparing `mapfun-0.0.2/src/mapfun/__init__.py` & `mapfun-0.0.3/src/mapfun.py`

 * *Files identical despite different names*

