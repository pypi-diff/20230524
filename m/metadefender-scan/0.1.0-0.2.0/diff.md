# Comparing `tmp/metadefender-scan-0.1.0.tar.gz` & `tmp/metadefender-scan-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metadefender-scan-0.1.0.tar", last modified: Fri May 14 13:40:10 2021, max compression
+gzip compressed data, was "metadefender-scan-0.2.0.tar", last modified: Wed May 24 10:57:31 2023, max compression
```

## Comparing `metadefender-scan-0.1.0.tar` & `metadefender-scan-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxrwx   0        0        0        0 2021-05-14 13:40:10.985924 metadefender-scan-0.1.0/
--rw-rw-rw-   0        0        0      916 2021-05-14 13:40:10.985778 metadefender-scan-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2582 2021-05-14 12:44:27.000000 metadefender-scan-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2021-05-14 13:40:10.986657 metadefender-scan-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1254 2021-05-14 13:40:06.000000 metadefender-scan-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2021-05-14 13:40:10.971198 metadefender-scan-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2021-05-14 13:40:10.976683 metadefender-scan-0.1.0/src/metadefender/
--rw-rw-rw-   0        0        0     4951 2021-05-14 13:28:10.000000 metadefender-scan-0.1.0/src/metadefender/__init__.py
--rw-rw-rw-   0        0        0    11179 2021-05-14 12:36:25.000000 metadefender-scan-0.1.0/src/metadefender/api.py
--rw-rw-rw-   0        0        0     4540 2021-05-14 12:29:49.000000 metadefender-scan-0.1.0/src/metadefender/app.py
-drwxrwxrwx   0        0        0        0 2021-05-14 13:40:10.984663 metadefender-scan-0.1.0/src/metadefender_scan.egg-info/
--rw-rw-rw-   0        0        0      916 2021-05-14 13:40:10.000000 metadefender-scan-0.1.0/src/metadefender_scan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      367 2021-05-14 13:40:10.000000 metadefender-scan-0.1.0/src/metadefender_scan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-05-14 13:40:10.000000 metadefender-scan-0.1.0/src/metadefender_scan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2021-05-14 13:40:10.000000 metadefender-scan-0.1.0/src/metadefender_scan.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       16 2021-05-14 13:40:10.000000 metadefender-scan-0.1.0/src/metadefender_scan.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2021-05-14 13:40:10.000000 metadefender-scan-0.1.0/src/metadefender_scan.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-24 10:57:31.953892 metadefender-scan-0.2.0/
+-rw-rw-rw-   0        0        0     1063 2021-04-02 11:16:41.000000 metadefender-scan-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     6143 2023-05-24 10:57:31.952916 metadefender-scan-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5458 2023-05-24 10:51:10.000000 metadefender-scan-0.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-24 10:57:31.953892 metadefender-scan-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1411 2023-05-24 10:51:10.000000 metadefender-scan-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 10:57:31.924601 metadefender-scan-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-24 10:57:31.934361 metadefender-scan-0.2.0/src/metadefender/
+-rw-rw-rw-   0        0        0     8083 2023-05-24 10:51:10.000000 metadefender-scan-0.2.0/src/metadefender/__init__.py
+-rw-rw-rw-   0        0        0     8229 2023-05-24 10:51:10.000000 metadefender-scan-0.2.0/src/metadefender/api.py
+-rw-rw-rw-   0        0        0    20909 2023-05-24 10:51:10.000000 metadefender-scan-0.2.0/src/metadefender/app.py
+-rw-rw-rw-   0        0        0      756 2023-05-24 10:51:10.000000 metadefender-scan-0.2.0/src/metadefender/logging.py
+drwxrwxrwx   0        0        0        0 2023-05-24 10:57:31.951940 metadefender-scan-0.2.0/src/metadefender_scan.egg-info/
+-rw-rw-rw-   0        0        0     6143 2023-05-24 10:57:31.000000 metadefender-scan-0.2.0/src/metadefender_scan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      403 2023-05-24 10:57:31.000000 metadefender-scan-0.2.0/src/metadefender_scan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 10:57:31.000000 metadefender-scan-0.2.0/src/metadefender_scan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-05-24 10:57:31.000000 metadefender-scan-0.2.0/src/metadefender_scan.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       16 2023-05-24 10:57:31.000000 metadefender-scan-0.2.0/src/metadefender_scan.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-24 10:57:31.000000 metadefender-scan-0.2.0/src/metadefender_scan.egg-info/top_level.txt
```

