# Comparing `tmp/async-westjr-0.0.1.tar.gz` & `tmp/async-westjr-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/async-westjr-0.0.1.tar", last modified: Thu Dec 16 06:30:43 2021, max compression
+gzip compressed data, was "async-westjr-0.4.tar", last modified: Wed May 24 01:19:34 2023, max compression
```

## Comparing `async-westjr-0.0.1.tar` & `async-westjr-0.4.tar`

### file list

```diff
@@ -1,14 +1,24 @@
-drwxr-xr-x   0 clark      (503) staff       (20)        0 2021-12-16 06:30:43.088021 async-westjr-0.0.1/
--rw-r--r--   0 clark      (503) staff       (20)     3395 2021-12-16 06:30:43.087626 async-westjr-0.0.1/PKG-INFO
--rw-r--r--   0 clark      (503) staff       (20)     2273 2021-12-16 06:21:57.000000 async-westjr-0.0.1/README.md
-drwxr-xr-x   0 clark      (503) staff       (20)        0 2021-12-16 06:30:43.080827 async-westjr-0.0.1/async_westjr/
--rw-r--r--   0 clark      (503) staff       (20)     5178 2021-12-16 05:50:49.000000 async-westjr-0.0.1/async_westjr/__init__.py
--rw-r--r--   0 clark      (503) staff       (20)    18946 2021-12-16 05:30:21.000000 async-westjr-0.0.1/async_westjr/const.py
-drwxr-xr-x   0 clark      (503) staff       (20)        0 2021-12-16 06:30:43.086960 async-westjr-0.0.1/async_westjr.egg-info/
--rw-r--r--   0 clark      (503) staff       (20)     3395 2021-12-16 06:30:42.000000 async-westjr-0.0.1/async_westjr.egg-info/PKG-INFO
--rw-r--r--   0 clark      (503) staff       (20)      244 2021-12-16 06:30:42.000000 async-westjr-0.0.1/async_westjr.egg-info/SOURCES.txt
--rw-r--r--   0 clark      (503) staff       (20)        1 2021-12-16 06:30:42.000000 async-westjr-0.0.1/async_westjr.egg-info/dependency_links.txt
--rw-r--r--   0 clark      (503) staff       (20)        8 2021-12-16 06:30:42.000000 async-westjr-0.0.1/async_westjr.egg-info/requires.txt
--rw-r--r--   0 clark      (503) staff       (20)       13 2021-12-16 06:30:42.000000 async-westjr-0.0.1/async_westjr.egg-info/top_level.txt
--rw-r--r--   0 clark      (503) staff       (20)       38 2021-12-16 06:30:43.088132 async-westjr-0.0.1/setup.cfg
--rw-r--r--   0 clark      (503) staff       (20)      785 2021-12-16 06:27:56.000000 async-westjr-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 01:19:34.891498 async-westjr-0.4/
+-rw-rw-rw-   0        0        0     1235 2023-05-23 04:39:13.000000 async-westjr-0.4/LICENSE
+-rw-rw-rw-   0        0        0     4704 2023-05-24 01:19:34.891498 async-westjr-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4011 2023-05-24 01:12:52.000000 async-westjr-0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-24 01:19:34.851513 async-westjr-0.4/async_westjr/
+-rw-rw-rw-   0        0        0       70 2023-05-23 04:39:13.000000 async-westjr-0.4/async_westjr/__init__.py
+-rw-rw-rw-   0        0        0     6783 2023-05-24 01:15:18.000000 async-westjr-0.4/async_westjr/api.py
+-rw-rw-rw-   0        0        0    27332 2023-05-23 04:39:13.000000 async-westjr-0.4/async_westjr/const.py
+drwxrwxrwx   0        0        0        0 2023-05-24 01:19:34.883512 async-westjr-0.4/async_westjr/response_types/
+-rw-rw-rw-   0        0        0      645 2023-05-23 04:39:13.000000 async-westjr-0.4/async_westjr/response_types/__init__.py
+-rw-rw-rw-   0        0        0      403 2023-05-23 04:39:13.000000 async-westjr-0.4/async_westjr/response_types/area_maintenance.py
+-rw-rw-rw-   0        0        0     1058 2023-05-23 04:39:13.000000 async-westjr-0.4/async_westjr/response_types/area_master.py
+-rw-rw-rw-   0        0        0      942 2023-05-23 04:39:13.000000 async-westjr-0.4/async_westjr/response_types/stations.py
+-rw-rw-rw-   0        0        0      614 2023-05-23 04:39:13.000000 async-westjr-0.4/async_westjr/response_types/train_info.py
+-rw-rw-rw-   0        0        0      386 2023-05-23 04:39:13.000000 async-westjr-0.4/async_westjr/response_types/train_monitor_info.py
+-rw-rw-rw-   0        0        0      470 2023-05-23 04:39:13.000000 async-westjr-0.4/async_westjr/response_types/train_pos.py
+drwxrwxrwx   0        0        0        0 2023-05-24 01:19:34.867502 async-westjr-0.4/async_westjr.egg-info/
+-rw-rw-rw-   0        0        0     4704 2023-05-24 01:19:34.000000 async-westjr-0.4/async_westjr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      586 2023-05-24 01:19:34.000000 async-westjr-0.4/async_westjr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 01:19:34.000000 async-westjr-0.4/async_westjr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      172 2023-05-24 01:19:34.000000 async-westjr-0.4/async_westjr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-24 01:19:34.000000 async-westjr-0.4/async_westjr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1385 2023-05-24 01:19:34.891498 async-westjr-0.4/setup.cfg
+-rw-rw-rw-   0        0        0       66 2023-05-23 04:39:13.000000 async-westjr-0.4/setup.py
```

