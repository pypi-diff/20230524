# Comparing `tmp/prometheus_client-0.8.0.tar.gz` & `tmp/prometheus_client-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/prometheus_client-0.8.0.tar", last modified: Mon May 25 12:11:13 2020, max compression
+gzip compressed data, was "dist/prometheus_client-0.9.0.tar", last modified: Mon Nov 16 13:33:35 2020, max compression
```

## Comparing `prometheus_client-0.8.0.tar` & `prometheus_client-0.9.0.tar`

### file list

```diff
@@ -1,95 +1,71 @@
-drwxrwxr-x   0 bbrazil   (1000) bbrazil   (1000)        0 2020-05-25 12:11:13.000000 prometheus_client-0.8.0/
-drwxrwxr-x   0 bbrazil   (1000) bbrazil   (1000)        0 2020-05-25 12:11:13.000000 prometheus_client-0.8.0/prometheus_client.egg-info/
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)       19 2020-05-25 12:11:13.000000 prometheus_client-0.8.0/prometheus_client.egg-info/requires.txt
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)       18 2020-05-25 12:11:13.000000 prometheus_client-0.8.0/prometheus_client.egg-info/top_level.txt
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)        1 2020-05-25 12:11:13.000000 prometheus_client-0.8.0/prometheus_client.egg-info/dependency_links.txt
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)    22825 2020-05-25 12:11:13.000000 prometheus_client-0.8.0/prometheus_client.egg-info/PKG-INFO
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)     2546 2020-05-25 12:11:13.000000 prometheus_client-0.8.0/prometheus_client.egg-info/SOURCES.txt
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)       38 2020-05-25 12:11:13.000000 prometheus_client-0.8.0/setup.cfg
-drwxrwxr-x   0 bbrazil   (1000) bbrazil   (1000)        0 2020-05-25 12:11:13.000000 prometheus_client-0.8.0/prometheus_client/
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)     1458 2019-12-19 12:56:41.000000 prometheus_client-0.8.0/prometheus_client/gc_collector.py
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)     1817 2020-04-22 11:40:32.000000 prometheus_client-0.8.0/prometheus_client/__init__.py
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)     1358 2019-12-19 12:56:41.000000 prometheus_client-0.8.0/prometheus_client/samples.py
-drwxrwxr-x   0 bbrazil   (1000) bbrazil   (1000)        0 2020-05-25 12:11:13.000000 prometheus_client-0.8.0/prometheus_client/twisted/
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)       72 2018-08-23 15:38:57.000000 prometheus_client-0.8.0/prometheus_client/twisted/__init__.py
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)      308 2020-04-22 11:40:32.000000 prometheus_client-0.8.0/prometheus_client/twisted/_exposition.py
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)     5357 2019-12-19 12:56:41.000000 prometheus_client-0.8.0/prometheus_client/registry.py
-drwxrwxr-x   0 bbrazil   (1000) bbrazil   (1000)        0 2020-05-25 12:11:13.000000 prometheus_client-0.8.0/prometheus_client/openmetrics/
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)    21527 2020-05-20 16:24:40.000000 prometheus_client-0.8.0/prometheus_client/openmetrics/parser.py
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)        0 2018-09-07 16:26:49.000000 prometheus_client-0.8.0/prometheus_client/openmetrics/__init__.py
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)     2860 2019-12-19 12:56:41.000000 prometheus_client-0.8.0/prometheus_client/openmetrics/exposition.py
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)    15283 2020-05-20 16:24:40.000000 prometheus_client-0.8.0/prometheus_client/exposition.py
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)      895 2019-12-19 12:56:40.000000 prometheus_client-0.8.0/prometheus_client/core.py
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)      621 2020-04-22 11:40:32.000000 prometheus_client-0.8.0/prometheus_client/utils.py
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)     3836 2020-04-22 11:40:32.000000 prometheus_client-0.8.0/prometheus_client/values.py
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)     5264 2020-04-22 11:40:32.000000 prometheus_client-0.8.0/prometheus_client/mmap_dict.py
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)    11881 2020-04-22 11:40:32.000000 prometheus_client-0.8.0/prometheus_client/metrics_core.py
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)     1691 2019-12-19 12:56:40.000000 prometheus_client-0.8.0/prometheus_client/context_managers.py
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)     1735 2019-12-19 12:56:41.000000 prometheus_client-0.8.0/prometheus_client/platform_collector.py
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)     3654 2020-04-22 11:40:32.000000 prometheus_client-0.8.0/prometheus_client/process_collector.py
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)     7256 2019-12-19 12:56:41.000000 prometheus_client-0.8.0/prometheus_client/parser.py
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)    22184 2020-05-20 16:24:40.000000 prometheus_client-0.8.0/prometheus_client/metrics.py
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)     1185 2020-04-22 11:40:32.000000 prometheus_client-0.8.0/prometheus_client/asgi.py
-drwxrwxr-x   0 bbrazil   (1000) bbrazil   (1000)        0 2020-05-25 12:11:13.000000 prometheus_client-0.8.0/prometheus_client/bridge/
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)        0 2018-08-23 15:38:57.000000 prometheus_client-0.8.0/prometheus_client/bridge/__init__.py
--rwxrwxr-x   0 bbrazil   (1000) bbrazil   (1000)     2485 2019-12-19 12:56:40.000000 prometheus_client-0.8.0/prometheus_client/bridge/graphite.py
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)     6474 2019-12-19 12:56:41.000000 prometheus_client-0.8.0/prometheus_client/multiprocess.py
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)    15802 2019-12-19 12:56:41.000000 prometheus_client-0.8.0/prometheus_client/decorator.py
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)       50 2020-04-22 11:40:32.000000 prometheus_client-0.8.0/MANIFEST.in
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)    16931 2020-04-22 11:40:32.000000 prometheus_client-0.8.0/README.md
-drwxrwxr-x   0 bbrazil   (1000) bbrazil   (1000)        0 2020-05-25 12:11:13.000000 prometheus_client-0.8.0/tests/
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)     2049 2018-09-07 16:26:49.000000 prometheus_client-0.8.0/tests/test_platform_collector.py
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)    15309 2020-04-22 12:10:45.000000 prometheus_client-0.8.0/tests/test_parser.pyc
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)    17060 2020-05-20 16:24:40.000000 prometheus_client-0.8.0/tests/test_exposition.py
-drwxrwxr-x   0 bbrazil   (1000) bbrazil   (1000)        0 2020-05-25 12:11:13.000000 prometheus_client-0.8.0/tests/proc/
-drwxrwxr-x   0 bbrazil   (1000) bbrazil   (1000)        0 2020-05-25 12:11:13.000000 prometheus_client-0.8.0/tests/proc/26231/
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)      330 2015-07-12 20:17:06.000000 prometheus_client-0.8.0/tests/proc/26231/stat
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)     1093 2015-07-12 20:17:06.000000 prometheus_client-0.8.0/tests/proc/26231/limits
-drwxrwxr-x   0 bbrazil   (1000) bbrazil   (1000)        0 2020-05-25 12:11:13.000000 prometheus_client-0.8.0/tests/proc/26231/fd/
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)        0 2015-07-12 20:17:06.000000 prometheus_client-0.8.0/tests/proc/26231/fd/1
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)        0 2015-07-12 20:17:06.000000 prometheus_client-0.8.0/tests/proc/26231/fd/2
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)        0 2015-07-12 20:17:06.000000 prometheus_client-0.8.0/tests/proc/26231/fd/0
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)        0 2015-07-12 20:17:06.000000 prometheus_client-0.8.0/tests/proc/26231/fd/4
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)        0 2015-07-12 20:17:06.000000 prometheus_client-0.8.0/tests/proc/26231/fd/3
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)     2094 2015-07-12 20:17:06.000000 prometheus_client-0.8.0/tests/proc/stat
-drwxrwxr-x   0 bbrazil   (1000) bbrazil   (1000)        0 2020-05-25 12:11:13.000000 prometheus_client-0.8.0/tests/proc/584/
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)      314 2015-07-12 20:17:06.000000 prometheus_client-0.8.0/tests/proc/584/stat
-drwxrwxr-x   0 bbrazil   (1000) bbrazil   (1000)        0 2020-05-25 12:11:13.000000 prometheus_client-0.8.0/tests/openmetrics/
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)    32377 2020-05-20 16:24:40.000000 prometheus_client-0.8.0/tests/openmetrics/test_parser.py
-drwxrwxr-x   0 bbrazil   (1000) bbrazil   (1000)        0 2020-05-25 12:11:13.000000 prometheus_client-0.8.0/tests/openmetrics/__pycache__/
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)    11412 2019-06-07 10:37:29.000000 prometheus_client-0.8.0/tests/openmetrics/__pycache__/test_exposition.cpython-35.pyc
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)    29118 2020-05-25 12:03:52.000000 prometheus_client-0.8.0/tests/openmetrics/__pycache__/test_parser.cpython-36.pyc
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)      144 2019-09-03 12:47:00.000000 prometheus_client-0.8.0/tests/openmetrics/__pycache__/__init__.cpython-36.pyc
--rw-------   0 bbrazil   (1000) bbrazil   (1000)    33684 2019-12-19 16:55:28.000000 prometheus_client-0.8.0/tests/openmetrics/__pycache__/test_parser.cpython-27-PYTEST.pyc
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)      144 2018-11-22 12:04:14.000000 prometheus_client-0.8.0/tests/openmetrics/__pycache__/__init__.cpython-35.pyc
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)    11714 2020-04-22 12:10:54.000000 prometheus_client-0.8.0/tests/openmetrics/__pycache__/test_exposition.cpython-36.pyc
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)    27794 2019-07-25 13:26:19.000000 prometheus_client-0.8.0/tests/openmetrics/__pycache__/test_parser.cpython-35.pyc
--rw-------   0 bbrazil   (1000) bbrazil   (1000)    13927 2019-12-19 16:55:28.000000 prometheus_client-0.8.0/tests/openmetrics/__pycache__/test_exposition.cpython-27-PYTEST.pyc
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)    33753 2020-05-25 12:03:59.000000 prometheus_client-0.8.0/tests/openmetrics/test_parser.pyc
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)        0 2018-09-07 16:26:49.000000 prometheus_client-0.8.0/tests/openmetrics/__init__.py
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)    13785 2020-04-22 12:10:45.000000 prometheus_client-0.8.0/tests/openmetrics/test_exposition.pyc
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)      148 2018-11-22 12:02:35.000000 prometheus_client-0.8.0/tests/openmetrics/__init__.pyc
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)     8949 2020-04-22 11:40:32.000000 prometheus_client-0.8.0/tests/openmetrics/test_exposition.py
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)    23387 2020-05-25 12:03:59.000000 prometheus_client-0.8.0/tests/test_exposition.pyc
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)     2490 2020-04-22 11:40:32.000000 prometheus_client-0.8.0/tests/test_wsgi.py
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)    12786 2020-04-22 11:58:36.000000 prometheus_client-0.8.0/tests/test_parser.py
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)     2016 2019-12-19 12:56:41.000000 prometheus_client-0.8.0/tests/test_gc_collector.py
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)     5448 2020-04-22 12:10:45.000000 prometheus_client-0.8.0/tests/test_asgi.pyc
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)     1577 2020-05-06 13:52:38.000000 prometheus_client-0.8.0/tests/test_twisted.py
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)      136 2018-11-22 12:02:35.000000 prometheus_client-0.8.0/tests/__init__.pyc
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)     3948 2018-11-22 12:02:35.000000 prometheus_client-0.8.0/tests/test_platform_collector.pyc
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)     4563 2020-04-22 12:10:45.000000 prometheus_client-0.8.0/tests/test_process_collector.pyc
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)     3873 2019-12-19 16:32:48.000000 prometheus_client-0.8.0/tests/test_graphite_bridge.pyc
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)    40625 2020-05-25 12:03:59.000000 prometheus_client-0.8.0/tests/test_core.pyc
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)     4013 2020-04-22 11:40:32.000000 prometheus_client-0.8.0/tests/test_asgi.py
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)     3708 2020-04-22 11:40:32.000000 prometheus_client-0.8.0/tests/test_process_collector.py
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)     2398 2020-05-15 10:40:12.000000 prometheus_client-0.8.0/tests/test_twisted.pyc
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)        0 2015-02-09 21:44:24.000000 prometheus_client-0.8.0/tests/__init__.py
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)     2084 2019-12-19 12:56:41.000000 prometheus_client-0.8.0/tests/test_graphite_bridge.py
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)     3486 2020-04-22 12:10:45.000000 prometheus_client-0.8.0/tests/test_wsgi.pyc
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)    18238 2019-12-19 16:32:48.000000 prometheus_client-0.8.0/tests/test_multiprocess.pyc
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)    35239 2020-05-20 16:24:40.000000 prometheus_client-0.8.0/tests/test_core.py
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)     2402 2019-12-19 16:32:48.000000 prometheus_client-0.8.0/tests/test_gc_collector.pyc
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)    13565 2019-12-19 12:56:41.000000 prometheus_client-0.8.0/tests/test_multiprocess.py
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)    22825 2020-05-25 12:11:13.000000 prometheus_client-0.8.0/PKG-INFO
--rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)     2011 2020-05-25 12:11:11.000000 prometheus_client-0.8.0/setup.py
+drwxrwxr-x   0 bbrazil   (1000) bbrazil   (1000)        0 2020-11-16 13:33:35.000000 prometheus_client-0.9.0/
+-rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)     2062 2020-11-16 13:26:23.000000 prometheus_client-0.9.0/setup.py
+drwxrwxr-x   0 bbrazil   (1000) bbrazil   (1000)        0 2020-11-16 13:33:35.000000 prometheus_client-0.9.0/prometheus_client.egg-info/
+-rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)       18 2020-11-16 13:33:35.000000 prometheus_client-0.9.0/prometheus_client.egg-info/top_level.txt
+-rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)       19 2020-11-16 13:33:35.000000 prometheus_client-0.9.0/prometheus_client.egg-info/requires.txt
+-rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)     1663 2020-11-16 13:33:35.000000 prometheus_client-0.9.0/prometheus_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)        1 2020-11-16 13:33:35.000000 prometheus_client-0.9.0/prometheus_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)    23347 2020-11-16 13:33:35.000000 prometheus_client-0.9.0/prometheus_client.egg-info/PKG-INFO
+-rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)    23347 2020-11-16 13:33:35.000000 prometheus_client-0.9.0/PKG-INFO
+-rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)       38 2020-11-16 13:33:35.000000 prometheus_client-0.9.0/setup.cfg
+drwxrwxr-x   0 bbrazil   (1000) bbrazil   (1000)        0 2020-11-16 13:33:35.000000 prometheus_client-0.9.0/tests/
+-rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)     2433 2020-11-03 19:33:29.000000 prometheus_client-0.9.0/tests/test_wsgi.py
+-rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)     2016 2019-12-19 12:56:41.000000 prometheus_client-0.9.0/tests/test_gc_collector.py
+-rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)     3998 2020-11-03 19:33:29.000000 prometheus_client-0.9.0/tests/test_asgi.py
+drwxrwxr-x   0 bbrazil   (1000) bbrazil   (1000)        0 2020-11-16 13:33:35.000000 prometheus_client-0.9.0/tests/proc/
+drwxrwxr-x   0 bbrazil   (1000) bbrazil   (1000)        0 2020-11-16 13:33:35.000000 prometheus_client-0.9.0/tests/proc/584/
+-rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)      314 2015-07-12 20:17:06.000000 prometheus_client-0.9.0/tests/proc/584/stat
+-rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)     2094 2015-07-12 20:17:06.000000 prometheus_client-0.9.0/tests/proc/stat
+drwxrwxr-x   0 bbrazil   (1000) bbrazil   (1000)        0 2020-11-16 13:33:35.000000 prometheus_client-0.9.0/tests/proc/26231/
+drwxrwxr-x   0 bbrazil   (1000) bbrazil   (1000)        0 2020-11-16 13:33:35.000000 prometheus_client-0.9.0/tests/proc/26231/fd/
+-rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)        0 2015-07-12 20:17:06.000000 prometheus_client-0.9.0/tests/proc/26231/fd/2
+-rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)        0 2015-07-12 20:17:06.000000 prometheus_client-0.9.0/tests/proc/26231/fd/1
+-rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)        0 2015-07-12 20:17:06.000000 prometheus_client-0.9.0/tests/proc/26231/fd/4
+-rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)        0 2015-07-12 20:17:06.000000 prometheus_client-0.9.0/tests/proc/26231/fd/3
+-rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)        0 2015-07-12 20:17:06.000000 prometheus_client-0.9.0/tests/proc/26231/fd/0
+-rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)     1093 2015-07-12 20:17:06.000000 prometheus_client-0.9.0/tests/proc/26231/limits
+-rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)      330 2015-07-12 20:17:06.000000 prometheus_client-0.9.0/tests/proc/26231/stat
+-rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)        0 2015-02-09 21:44:24.000000 prometheus_client-0.9.0/tests/__init__.py
+-rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)    12786 2020-04-22 11:58:36.000000 prometheus_client-0.9.0/tests/test_parser.py
+-rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)     3708 2020-04-22 11:40:32.000000 prometheus_client-0.9.0/tests/test_process_collector.py
+-rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)     1543 2020-11-03 19:33:29.000000 prometheus_client-0.9.0/tests/test_twisted.py
+-rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)     2049 2018-09-07 16:26:49.000000 prometheus_client-0.9.0/tests/test_platform_collector.py
+-rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)     2084 2019-12-19 12:56:41.000000 prometheus_client-0.9.0/tests/test_graphite_bridge.py
+drwxrwxr-x   0 bbrazil   (1000) bbrazil   (1000)        0 2020-11-16 13:33:35.000000 prometheus_client-0.9.0/tests/openmetrics/
+-rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)    32706 2020-11-13 21:19:44.000000 prometheus_client-0.9.0/tests/openmetrics/test_parser.py
+-rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)     8949 2020-09-15 23:04:40.000000 prometheus_client-0.9.0/tests/openmetrics/test_exposition.py
+-rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)        0 2018-09-07 16:26:49.000000 prometheus_client-0.9.0/tests/openmetrics/__init__.py
+-rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)    16975 2020-11-03 19:33:29.000000 prometheus_client-0.9.0/tests/test_exposition.py
+-rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)    13565 2019-12-19 12:56:41.000000 prometheus_client-0.9.0/tests/test_multiprocess.py
+-rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)    35205 2020-11-13 21:19:44.000000 prometheus_client-0.9.0/tests/test_core.py
+-rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)    17315 2020-11-03 19:33:29.000000 prometheus_client-0.9.0/README.md
+-rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)       50 2020-04-22 11:40:32.000000 prometheus_client-0.9.0/MANIFEST.in
+drwxrwxr-x   0 bbrazil   (1000) bbrazil   (1000)        0 2020-11-16 13:33:35.000000 prometheus_client-0.9.0/prometheus_client/
+-rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)     6474 2019-12-19 12:56:41.000000 prometheus_client-0.9.0/prometheus_client/multiprocess.py
+-rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)      621 2020-04-22 11:40:32.000000 prometheus_client-0.9.0/prometheus_client/utils.py
+drwxrwxr-x   0 bbrazil   (1000) bbrazil   (1000)        0 2020-11-16 13:33:35.000000 prometheus_client-0.9.0/prometheus_client/bridge/
+-rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)        0 2018-08-23 15:38:57.000000 prometheus_client-0.9.0/prometheus_client/bridge/__init__.py
+-rwxrwxr-x   0 bbrazil   (1000) bbrazil   (1000)     2485 2019-12-19 12:56:40.000000 prometheus_client-0.9.0/prometheus_client/bridge/graphite.py
+-rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)     1358 2019-12-19 12:56:41.000000 prometheus_client-0.9.0/prometheus_client/samples.py
+-rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)     1185 2020-04-22 11:40:32.000000 prometheus_client-0.9.0/prometheus_client/asgi.py
+-rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)     7258 2020-11-03 19:33:29.000000 prometheus_client-0.9.0/prometheus_client/parser.py
+-rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)    11900 2020-11-13 21:19:44.000000 prometheus_client-0.9.0/prometheus_client/metrics_core.py
+-rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)     1691 2019-12-19 12:56:40.000000 prometheus_client-0.9.0/prometheus_client/context_managers.py
+-rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)     1735 2019-12-19 12:56:41.000000 prometheus_client-0.9.0/prometheus_client/platform_collector.py
+-rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)     5262 2020-11-03 19:33:29.000000 prometheus_client-0.9.0/prometheus_client/mmap_dict.py
+drwxrwxr-x   0 bbrazil   (1000) bbrazil   (1000)        0 2020-11-16 13:33:35.000000 prometheus_client-0.9.0/prometheus_client/openmetrics/
+-rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)    22004 2020-11-13 21:19:44.000000 prometheus_client-0.9.0/prometheus_client/openmetrics/parser.py
+-rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)        0 2018-09-07 16:26:49.000000 prometheus_client-0.9.0/prometheus_client/openmetrics/__init__.py
+-rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)     2860 2020-09-15 13:16:16.000000 prometheus_client-0.9.0/prometheus_client/openmetrics/exposition.py
+drwxrwxr-x   0 bbrazil   (1000) bbrazil   (1000)        0 2020-11-16 13:33:35.000000 prometheus_client-0.9.0/prometheus_client/twisted/
+-rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)       72 2018-08-23 15:38:57.000000 prometheus_client-0.9.0/prometheus_client/twisted/__init__.py
+-rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)      308 2020-11-03 19:33:29.000000 prometheus_client-0.9.0/prometheus_client/twisted/_exposition.py
+-rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)     5407 2020-11-13 21:19:44.000000 prometheus_client-0.9.0/prometheus_client/registry.py
+-rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)     3836 2020-04-22 11:40:32.000000 prometheus_client-0.9.0/prometheus_client/values.py
+-rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)    22184 2020-05-20 16:24:40.000000 prometheus_client-0.9.0/prometheus_client/metrics.py
+-rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)     3654 2020-04-22 11:40:32.000000 prometheus_client-0.9.0/prometheus_client/process_collector.py
+-rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)     1458 2019-12-19 12:56:41.000000 prometheus_client-0.9.0/prometheus_client/gc_collector.py
+-rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)     1752 2020-11-03 19:33:29.000000 prometheus_client-0.9.0/prometheus_client/__init__.py
+-rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)    15267 2020-11-03 19:33:29.000000 prometheus_client-0.9.0/prometheus_client/exposition.py
+-rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)      901 2020-11-03 19:33:29.000000 prometheus_client-0.9.0/prometheus_client/core.py
+-rw-rw-r--   0 bbrazil   (1000) bbrazil   (1000)    15802 2019-12-19 12:56:41.000000 prometheus_client-0.9.0/prometheus_client/decorator.py
```

### Comparing `prometheus_client-0.8.0/prometheus_client.egg-info/PKG-INFO` & `prometheus_client-0.9.0/prometheus_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prometheus-client
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python client for the Prometheus monitoring system.
 Home-page: https://github.com/prometheus/client_python
 Author: Brian Brazil
 Author-email: brian.brazil@robustperception.io
 License: Apache Software License 2.0
 Description: # Prometheus Python Client
         
@@ -224,14 +224,25 @@
         ```python
         from prometheus_client import Counter
         c = Counter('my_requests_total', 'HTTP Failures', ['method', 'endpoint'])
         c.labels(method='get', endpoint='/').inc()
         c.labels(method='post', endpoint='/submit').inc()
         ```
         
+        Metrics with labels are not initialized when declared, because the client can't
+        know what values the label can have. It is recommended to initialize the label
+        values by calling the `.labels()` method alone:
+        
+        ```python
+        from prometheus_client import Counter
+        c = Counter('my_requests_total', 'HTTP Failures', ['method', 'endpoint'])
+        c.labels('get', '/')
+        c.labels('post', '/submit')
+        ```
+        
         ### Process Collector
         
         The Python client automatically exports metrics about process CPU usage, RAM,
         file descriptors and start time. These all have the prefix `process`, and
         are only currently available on Linux.
         
         The namespace and pid constructor arguments allows for exporting metrics about
@@ -338,25 +349,25 @@
         from werkzeug.middleware.dispatcher import DispatcherMiddleware
         from prometheus_client import make_wsgi_app
         
         # Create my app
         app = Flask(__name__)
         
         # Add prometheus wsgi middleware to route /metrics requests
-        app_dispatch = DispatcherMiddleware(app, {
+        app.wsgi_app = DispatcherMiddleware(app.wsgi_app, {
             '/metrics': make_wsgi_app()
         })
         ```
         
         Run the example web application like this
         
         ```bash
         # Install uwsgi if you do not have it
         pip install uwsgi
-        uwsgi --http 127.0.0.1:8000 --wsgi-file myapp.py --callable app_dispatch
+        uwsgi --http 127.0.0.1:8000 --wsgi-file myapp.py --callable app
         ```
         
         Visit http://localhost:8000/metrics to see the metrics
         
         ### Node exporter textfile collector
         
         The [textfile collector](https://github.com/prometheus/node_exporter#textfile-collector)
@@ -585,13 +596,14 @@
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: System :: Monitoring
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
 Provides-Extra: twisted
```

### Comparing `prometheus_client-0.8.0/prometheus_client/gc_collector.py` & `prometheus_client-0.9.0/prometheus_client/gc_collector.py`

 * *Files identical despite different names*

### Comparing `prometheus_client-0.8.0/prometheus_client/__init__.py` & `prometheus_client-0.9.0/prometheus_client/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 #!/usr/bin/python
 
-from . import exposition
-from . import gc_collector
-from . import metrics
-from . import metrics_core
-from . import platform_collector
-from . import process_collector
-from . import registry
+from . import (
+    exposition, gc_collector, metrics, metrics_core, platform_collector,
+    process_collector, registry,
+)
 
 __all__ = ['Counter', 'Gauge', 'Summary', 'Histogram', 'Info', 'Enum']
 
 CollectorRegistry = registry.CollectorRegistry
 REGISTRY = registry.REGISTRY
 Metric = metrics_core.Metric
 Counter = metrics.Counter
```

### Comparing `prometheus_client-0.8.0/prometheus_client/samples.py` & `prometheus_client-0.9.0/prometheus_client/samples.py`

 * *Files identical despite different names*

### Comparing `prometheus_client-0.8.0/prometheus_client/registry.py` & `prometheus_client-0.9.0/prometheus_client/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         """Remove a collector from the registry."""
         with self._lock:
             for name in self._collector_to_names[collector]:
                 del self._names_to_collectors[name]
             del self._collector_to_names[collector]
 
     def _get_names(self, collector):
-        """Get names of timeseries the collector produces."""
+        """Get names of timeseries the collector produces and clashes with."""
         desc_func = None
         # If there's a describe function, use it.
         try:
             desc_func = collector.describe
         except AttributeError:
             pass
         # Otherwise, if auto describe is enabled use the collect function.
@@ -54,21 +54,22 @@
 
         if not desc_func:
             return []
 
         result = []
         type_suffixes = {
             'counter': ['_total', '_created'],
-            'summary': ['', '_sum', '_count', '_created'],
+            'summary': ['_sum', '_count', '_created'],
             'histogram': ['_bucket', '_sum', '_count', '_created'],
             'gaugehistogram': ['_bucket', '_gsum', '_gcount'],
             'info': ['_info'],
         }
         for metric in desc_func():
-            for suffix in type_suffixes.get(metric.type, ['']):
+            result.append(metric.name)
+            for suffix in type_suffixes.get(metric.type, []):
                 result.append(metric.name + suffix)
         return result
 
     def collect(self):
         """Yields metrics from the collectors in the registry."""
         collectors = None
         ti = None
```

### Comparing `prometheus_client-0.8.0/prometheus_client/openmetrics/parser.py` & `prometheus_client-0.9.0/prometheus_client/openmetrics/parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,24 +11,25 @@
 
 try:
     import StringIO
 except ImportError:
     # Python 3
     import io as StringIO
 
+
 def text_string_to_metric_families(text):
     """Parse Openmetrics text format from a unicode string.
 
     See text_fd_to_metric_families.
     """
     for metric_family in text_fd_to_metric_families(StringIO.StringIO(text)):
         yield metric_family
 
 
-_CANONICAL_NUMBERS = set([i / 1000.0 for i in range(10000)] + [10.0**i for i in range(-10, 11)] + [float("inf")])
+_CANONICAL_NUMBERS = set([float("inf")])
 
 
 def _isUncanonicalNumber(s):
     f = float(s)
     if f not in _CANONICAL_NUMBERS:
         return False  # Only the canonical numbers are required to be canonical.
     return s != floatToGoString(f)
@@ -109,16 +110,16 @@
             if math.isnan(ts) or math.isinf(ts):
                 raise ValueError("Invalid timestamp: {0!r}".format(timestamp))
             return ts
 
 
 def _is_character_escaped(s, charpos):
     num_bslashes = 0
-    while (charpos > num_bslashes and
-           s[charpos - 1 - num_bslashes] == '\\'):
+    while (charpos > num_bslashes
+           and s[charpos - 1 - num_bslashes] == '\\'):
         num_bslashes += 1
     return num_bslashes % 2 == 1
 
 
 def _parse_labels_with_state_machine(text):
     # The { has already been parsed.
     state = 'startoflabelname'
@@ -355,15 +356,15 @@
     if state in ['exemplarhash', 'exemplarspace', 'exemplarstartoflabels', 'exemplarparsedlabels']:
         raise ValueError("Invalid line: " + text)
 
     ts = _parse_timestamp(timestamp)
     exemplar = None
     if exemplar_labels is not None:
         exemplar_length = sum([len(k) + len(v) for k, v in exemplar_labels.items()])
-        if exemplar_length > 64:
+        if exemplar_length > 128:
             raise ValueError("Exmplar labels are too long: " + text)
         exemplar = Exemplar(
             exemplar_labels,
             _parse_value(exemplar_value),
             _parse_timestamp(exemplar_timestamp),
         )
 
@@ -394,14 +395,20 @@
     timestamp = None
 
     def do_checks():
         if bucket != float('+Inf'):
             raise ValueError("+Inf bucket missing: " + name)
         if count is not None and value != count:
             raise ValueError("Count does not match +Inf value: " + name)
+        if has_sum and count is None:
+            raise ValueError("_count must be present if _sum is present: " + name)
+        if has_gsum and count is None:
+            raise ValueError("_gcount must be present if _gsum is present: " + name)
+        if not (has_sum or has_gsum) and count is not None:
+            raise ValueError("_sum/_gsum must be present if _count is present: " + name)
         if has_negative_buckets and has_sum:
             raise ValueError("Cannot have _sum with negative buckets: " + name)
         if not has_negative_buckets and has_negative_gsum:
             raise ValueError("Cannot have negative _gsum with non-negative buckets: " + name)
 
     for s in samples:
         suffix = s.name[len(name):]
@@ -409,14 +416,15 @@
         if g != group or s.timestamp != timestamp:
             if group is not None:
                 do_checks()
             count = None
             bucket = None
             has_negative_buckets = False
             has_sum = False
+            has_gsum = False
             has_negative_gsum = False
             value = 0
         group = g
         timestamp = s.timestamp
 
         if suffix == '_bucket':
             b = float(s.labels['le'])
@@ -428,16 +436,18 @@
                 raise ValueError("Bucket values out of order: " + name)
             bucket = b
             value = s.value
         elif suffix in ['_count', '_gcount']:
             count = s.value
         elif suffix in ['_sum']:
             has_sum = True
-        elif suffix in ['_gsum'] and s.value < 0:
-            has_negative_gsum = True
+        elif suffix in ['_gsum']:
+            has_gsum = True
+            if s.value < 0:
+                has_negative_gsum = True
 
     if group is not None:
         do_checks()
 
 
 def text_fd_to_metric_families(fd):
     """Parse Prometheus text format from a file descriptor.
@@ -448,22 +458,30 @@
 
     Yields Metric's.
     """
     name = None
     allowed_names = []
     eof = False
 
-    seen_metrics = set()
+    seen_names = set()
+    type_suffixes = {
+        'counter': ['_total', '_created'],
+        'summary': ['', '_count', '_sum', '_created'],
+        'histogram': ['_count', '_sum', '_bucket', '_created'],
+        'gaugehistogram': ['_gcount', '_gsum', '_bucket'],
+        'info': ['_info'],
+    }
 
     def build_metric(name, documentation, typ, unit, samples):
-        if name in seen_metrics:
-            raise ValueError("Duplicate metric: " + name)
-        seen_metrics.add(name)
         if typ is None:
             typ = 'unknown'
+        for suffix in set(type_suffixes.get(typ, []) + [""]):
+            if name + suffix in seen_names:
+                raise ValueError("Clashing name: " + name + suffix)
+            seen_names.add(name + suffix)
         if documentation is None:
             documentation = ''
         if unit is None:
             unit = ''
         if unit and not name.endswith("_" + unit):
             raise ValueError("Unit does not match metric name: " + name)
         if unit and typ in ['info', 'stateset']:
@@ -478,14 +496,17 @@
     for line in fd:
         if line[-1] == '\n':
             line = line[:-1]
 
         if eof:
             raise ValueError("Received line after # EOF: " + line)
 
+        if not line:
+            raise ValueError("Received blank line")
+
         if line == '# EOF':
             eof = True
         elif line.startswith('#'):
             parts = line.split(' ', 3)
             if len(parts) < 4:
                 raise ValueError("Invalid line: " + line)
             if parts[2] == name and samples:
@@ -514,22 +535,15 @@
                     raise ValueError("Invalid line: " + line)
             elif parts[1] == 'TYPE':
                 if typ is not None:
                     raise ValueError("More than one TYPE for metric: " + line)
                 typ = parts[3]
                 if typ == 'untyped':
                     raise ValueError("Invalid TYPE for metric: " + line)
-                allowed_names = {
-                    'counter': ['_total', '_created'],
-                    'summary': ['_count', '_sum', '', '_created'],
-                    'histogram': ['_count', '_sum', '_bucket', '_created'],
-                    'gaugehistogram': ['_gcount', '_gsum', '_bucket'],
-                    'info': ['_info'],
-                }.get(typ, [''])
-                allowed_names = [name + n for n in allowed_names]
+                allowed_names = [name + n for n in type_suffixes.get(typ, [''])]
             elif parts[1] == 'UNIT':
                 if unit is not None:
                     raise ValueError("More than one UNIT for metric: " + line)
                 unit = parts[3]
             else:
                 raise ValueError("Invalid line: " + line)
         else:
@@ -553,15 +567,15 @@
                 raise ValueError("Stateset missing label: " + line)
             if (typ in ['histogram', 'gaugehistogram'] and name + '_bucket' == sample.name
                     and (sample.labels.get('le', "NaN") == "NaN"
                          or _isUncanonicalNumber(sample.labels['le']))):
                 raise ValueError("Invalid le label: " + line)
             if (typ == 'summary' and name == sample.name
                     and (not (0 <= float(sample.labels.get('quantile', -1)) <= 1)
-                          or _isUncanonicalNumber(sample.labels['quantile']))):
+                         or _isUncanonicalNumber(sample.labels['quantile']))):
                 raise ValueError("Invalid quantile label: " + line)
 
             g = tuple(sorted(_group_for_sample(sample, name, typ).items()))
             if group is not None and g != group and g in seen_groups:
                 raise ValueError("Invalid metric grouping: " + line)
             if group is not None and g == group:
                 if (sample.timestamp is None) != (group_timestamp is None):
```

### Comparing `prometheus_client-0.8.0/prometheus_client/openmetrics/exposition.py` & `prometheus_client-0.9.0/prometheus_client/openmetrics/exposition.py`

 * *Files identical despite different names*

### Comparing `prometheus_client-0.8.0/prometheus_client/exposition.py` & `prometheus_client-0.9.0/prometheus_client/exposition.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,32 +2,33 @@
 
 import base64
 from contextlib import closing
 import os
 import socket
 import sys
 import threading
-from wsgiref.simple_server import make_server, WSGIServer, WSGIRequestHandler
+from wsgiref.simple_server import make_server, WSGIRequestHandler, WSGIServer
 
 from .openmetrics import exposition as openmetrics
 from .registry import REGISTRY
 from .utils import floatToGoString
 
 try:
-    from BaseHTTPServer import BaseHTTPRequestHandler, HTTPServer
-    from SocketServer import ThreadingMixIn
-    from urllib2 import build_opener, Request, HTTPHandler
     from urllib import quote_plus
+
+    from BaseHTTPServer import BaseHTTPRequestHandler
+    from SocketServer import ThreadingMixIn
+    from urllib2 import build_opener, HTTPHandler, Request
     from urlparse import parse_qs, urlparse
 except ImportError:
     # Python 3
-    from http.server import BaseHTTPRequestHandler, HTTPServer
+    from http.server import BaseHTTPRequestHandler
     from socketserver import ThreadingMixIn
-    from urllib.request import build_opener, Request, HTTPHandler
-    from urllib.parse import quote_plus, parse_qs, urlparse
+    from urllib.parse import parse_qs, quote_plus, urlparse
+    from urllib.request import build_opener, HTTPHandler, Request
 
 CONTENT_TYPE_LATEST = str('text/plain; version=0.0.4; charset=utf-8')
 """Content type of the latest text format"""
 
 PYTHON26_OR_OLDER = sys.version_info < (2, 7)
 PYTHON376_OR_NEWER = sys.version_info > (3, 7, 5)
 
@@ -358,15 +359,15 @@
     handler(
         url=url, method=method, timeout=timeout,
         headers=[('Content-Type', CONTENT_TYPE_LATEST)], data=data,
     )()
 
 
 def _escape_grouping_key(k, v):
-    if v == "" :
+    if v == "":
         # Per https://github.com/prometheus/pushgateway/pull/346.
         return k + "@base64", "="
     elif '/' in v:
         # Added in Pushgateway 0.9.0.
         return k + "@base64", base64.urlsafe_b64encode(v.encode("utf-8")).decode("utf-8")
     else:
         return k, quote_plus(v)
@@ -377,10 +378,10 @@
     with closing(socket.socket(socket.AF_INET, socket.SOCK_DGRAM)) as s:
         s.connect(('localhost', 0))
         return {'instance': s.getsockname()[0]}
 
 
 try:
     # Python >3.5 only
-    from .asgi import make_asgi_app
+    from .asgi import make_asgi_app  # noqa
 except:
     pass
```

### Comparing `prometheus_client-0.8.0/prometheus_client/core.py` & `prometheus_client-0.9.0/prometheus_client/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from __future__ import unicode_literals
 
 from .metrics import Counter, Enum, Gauge, Histogram, Info, Summary
 from .metrics_core import (
-    CounterMetricFamily, GaugeHistogramMetricFamily, GaugeMetricFamily, HistogramMetricFamily, InfoMetricFamily,
-    Metric, StateSetMetricFamily, SummaryMetricFamily, UnknownMetricFamily, UntypedMetricFamily)
+    CounterMetricFamily, GaugeHistogramMetricFamily, GaugeMetricFamily,
+    HistogramMetricFamily, InfoMetricFamily, Metric, StateSetMetricFamily,
+    SummaryMetricFamily, UnknownMetricFamily, UntypedMetricFamily,
+)
 from .registry import CollectorRegistry, REGISTRY
 from .samples import Exemplar, Sample, Timestamp
 
 __all__ = (
     'CollectorRegistry',
     'Counter',
     'CounterMetricFamily',
```

### Comparing `prometheus_client-0.8.0/prometheus_client/utils.py` & `prometheus_client-0.9.0/prometheus_client/utils.py`

 * *Files identical despite different names*

### Comparing `prometheus_client-0.8.0/prometheus_client/values.py` & `prometheus_client-0.9.0/prometheus_client/values.py`

 * *Files identical despite different names*

### Comparing `prometheus_client-0.8.0/prometheus_client/mmap_dict.py` & `prometheus_client-0.9.0/prometheus_client/mmap_dict.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
     while pos < used:
         encoded_len = _unpack_integer(data, pos)[0]
         # check we are not reading beyond bounds
         if encoded_len + pos > used:
             raise RuntimeError('Read beyond file size detected, file is corrupted.')
         pos += 4
-        encoded_key = data[pos : pos + encoded_len]
+        encoded_key = data[pos:pos + encoded_len]
         padded_len = encoded_len + (8 - (encoded_len + 4) % 8)
         pos += padded_len
         value = _unpack_double(data, pos)[0]
         yield encoded_key.decode('utf-8'), value, pos
         pos += 8
```

### Comparing `prometheus_client-0.8.0/prometheus_client/metrics_core.py` & `prometheus_client-0.9.0/prometheus_client/metrics_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,20 +38,20 @@
     def add_sample(self, name, labels, value, timestamp=None, exemplar=None):
         """Add a sample to the metric.
 
         Internal-only, do not use."""
         self.samples.append(Sample(name, labels, value, timestamp, exemplar))
 
     def __eq__(self, other):
-        return (isinstance(other, Metric) and
-                self.name == other.name and
-                self.documentation == other.documentation and
-                self.type == other.type and
-                self.unit == other.unit and
-                self.samples == other.samples)
+        return (isinstance(other, Metric)
+                and self.name == other.name 
+                and self.documentation == other.documentation
+                and self.type == other.type
+                and self.unit == other.unit
+                and self.samples == other.samples)
 
     def __repr__(self):
         return "Metric(%s, %s, %s, %s, %s)" % (
             self.name,
             self.documentation,
             self.type,
             self.unit,
@@ -212,21 +212,21 @@
             self.samples.append(Sample(
                 self.name + '_bucket',
                 dict(list(zip(self._labelnames, labels)) + [('le', bucket)]),
                 value,
                 timestamp,
                 exemplar,
             ))
-        # +Inf is last and provides the count value.
-        self.samples.append(
-                Sample(self.name + '_count', dict(zip(self._labelnames, labels)), buckets[-1][1], timestamp))
-        # Don't iunclude sum if there's negative buckets.
+        # Don't include sum and thus count if there's negative buckets.
         if float(buckets[0][0]) >= 0 and sum_value is not None:
+            # +Inf is last and provides the count value.
+            self.samples.append(
+                Sample(self.name + '_count', dict(zip(self._labelnames, labels)), buckets[-1][1], timestamp))
             self.samples.append(
-                    Sample(self.name + '_sum', dict(zip(self._labelnames, labels)), sum_value, timestamp))
+                Sample(self.name + '_sum', dict(zip(self._labelnames, labels)), sum_value, timestamp))
 
 
 
 class GaugeHistogramMetricFamily(Metric):
     """A single gauge histogram and its samples.
 
     For use by custom collectors.
```

### Comparing `prometheus_client-0.8.0/prometheus_client/context_managers.py` & `prometheus_client-0.9.0/prometheus_client/context_managers.py`

 * *Files identical despite different names*

### Comparing `prometheus_client-0.8.0/prometheus_client/platform_collector.py` & `prometheus_client-0.9.0/prometheus_client/platform_collector.py`

 * *Files identical despite different names*

### Comparing `prometheus_client-0.8.0/prometheus_client/process_collector.py` & `prometheus_client-0.9.0/prometheus_client/process_collector.py`

 * *Files identical despite different names*

### Comparing `prometheus_client-0.8.0/prometheus_client/parser.py` & `prometheus_client-0.9.0/prometheus_client/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,16 +42,16 @@
 
 def _replace_escaping(s):
     return ESCAPING_RE.sub(replace_escape_sequence, s)
 
 
 def _is_character_escaped(s, charpos):
     num_bslashes = 0
-    while (charpos > num_bslashes and
-           s[charpos - 1 - num_bslashes] == '\\'):
+    while (charpos > num_bslashes
+           and s[charpos - 1 - num_bslashes] == '\\'):
         num_bslashes += 1
     return num_bslashes % 2 == 1
 
 
 def _parse_labels(labels_string):
     labels = {}
     # Return if we don't have valid labels
@@ -108,15 +108,15 @@
     separator = " "
     if separator not in s:
         separator = "\t"
     values = [value.strip() for value in s.split(separator) if value.strip()]
     if not values:
         return float(s), None
     value = float(values[0])
-    timestamp = (float(values[-1])/1000) if len(values) > 1 else None
+    timestamp = (float(values[-1]) / 1000) if len(values) > 1 else None
     return value, timestamp
 
 
 def _parse_sample(text):
     # Detect the labels in the text
     try:
         label_start, label_end = text.index("{"), text.rindex("}")
```

### Comparing `prometheus_client-0.8.0/prometheus_client/metrics.py` & `prometheus_client-0.9.0/prometheus_client/metrics.py`

 * *Files identical despite different names*

### Comparing `prometheus_client-0.8.0/prometheus_client/asgi.py` & `prometheus_client-0.9.0/prometheus_client/asgi.py`

 * *Files identical despite different names*

### Comparing `prometheus_client-0.8.0/prometheus_client/bridge/graphite.py` & `prometheus_client-0.9.0/prometheus_client/bridge/graphite.py`

 * *Files identical despite different names*

### Comparing `prometheus_client-0.8.0/prometheus_client/multiprocess.py` & `prometheus_client-0.9.0/prometheus_client/multiprocess.py`

 * *Files identical despite different names*

### Comparing `prometheus_client-0.8.0/prometheus_client/decorator.py` & `prometheus_client-0.9.0/prometheus_client/decorator.py`

 * *Files identical despite different names*

### Comparing `prometheus_client-0.8.0/README.md` & `prometheus_client-0.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -216,14 +216,25 @@
 ```python
 from prometheus_client import Counter
 c = Counter('my_requests_total', 'HTTP Failures', ['method', 'endpoint'])
 c.labels(method='get', endpoint='/').inc()
 c.labels(method='post', endpoint='/submit').inc()
 ```
 
+Metrics with labels are not initialized when declared, because the client can't
+know what values the label can have. It is recommended to initialize the label
+values by calling the `.labels()` method alone:
+
+```python
+from prometheus_client import Counter
+c = Counter('my_requests_total', 'HTTP Failures', ['method', 'endpoint'])
+c.labels('get', '/')
+c.labels('post', '/submit')
+```
+
 ### Process Collector
 
 The Python client automatically exports metrics about process CPU usage, RAM,
 file descriptors and start time. These all have the prefix `process`, and
 are only currently available on Linux.
 
 The namespace and pid constructor arguments allows for exporting metrics about
@@ -330,25 +341,25 @@
 from werkzeug.middleware.dispatcher import DispatcherMiddleware
 from prometheus_client import make_wsgi_app
 
 # Create my app
 app = Flask(__name__)
 
 # Add prometheus wsgi middleware to route /metrics requests
-app_dispatch = DispatcherMiddleware(app, {
+app.wsgi_app = DispatcherMiddleware(app.wsgi_app, {
     '/metrics': make_wsgi_app()
 })
 ```
 
 Run the example web application like this
 
 ```bash
 # Install uwsgi if you do not have it
 pip install uwsgi
-uwsgi --http 127.0.0.1:8000 --wsgi-file myapp.py --callable app_dispatch
+uwsgi --http 127.0.0.1:8000 --wsgi-file myapp.py --callable app
 ```
 
 Visit http://localhost:8000/metrics to see the metrics
 
 ### Node exporter textfile collector
 
 The [textfile collector](https://github.com/prometheus/node_exporter#textfile-collector)
```

### Comparing `prometheus_client-0.8.0/tests/test_platform_collector.py` & `prometheus_client-0.9.0/tests/test_platform_collector.py`

 * *Files identical despite different names*

### Comparing `prometheus_client-0.8.0/tests/test_exposition.py` & `prometheus_client-0.9.0/tests/test_exposition.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,37 +3,34 @@
 import sys
 import threading
 import time
 
 import pytest
 
 from prometheus_client import (
-    CollectorRegistry, CONTENT_TYPE_LATEST, Counter, delete_from_gateway, Enum,
-    Gauge, generate_latest, Histogram, Info, instance_ip_grouping_key, Metric,
-    push_to_gateway, pushadd_to_gateway, Summary,
+    CollectorRegistry, CONTENT_TYPE_LATEST, core, Counter, delete_from_gateway,
+    Enum, Gauge, generate_latest, Histogram, Info, instance_ip_grouping_key,
+    Metric, push_to_gateway, pushadd_to_gateway, Summary,
 )
-from prometheus_client import core
 from prometheus_client.core import GaugeHistogramMetricFamily, Timestamp
 from prometheus_client.exposition import (
-    basic_auth_handler, default_handler, MetricsHandler
+    basic_auth_handler, default_handler, MetricsHandler,
 )
 
 if sys.version_info < (2, 7):
     # We need the skip decorators from unittest2 on Python 2.6.
     import unittest2 as unittest
 else:
     import unittest
 
 try:
-    from BaseHTTPServer import BaseHTTPRequestHandler
-    from BaseHTTPServer import HTTPServer
+    from BaseHTTPServer import BaseHTTPRequestHandler, HTTPServer
 except ImportError:
     # Python 3
-    from http.server import BaseHTTPRequestHandler
-    from http.server import HTTPServer
+    from http.server import BaseHTTPRequestHandler, HTTPServer
 
 
 class TestGenerateText(unittest.TestCase):
     def setUp(self):
         self.registry = CollectorRegistry()
 
         # Mock time so _created values are fixed.
```

### Comparing `prometheus_client-0.8.0/tests/proc/26231/limits` & `prometheus_client-0.9.0/tests/proc/26231/limits`

 * *Files identical despite different names*

### Comparing `prometheus_client-0.8.0/tests/proc/stat` & `prometheus_client-0.9.0/tests/proc/stat`

 * *Files identical despite different names*

### Comparing `prometheus_client-0.8.0/tests/openmetrics/test_parser.py` & `prometheus_client-0.9.0/tests/openmetrics/test_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,20 +98,22 @@
 
     def test_summary_quantiles(self):
         families = text_string_to_metric_families("""# TYPE a summary
 # HELP a help
 a_count 1
 a_sum 2
 a{quantile="0.5"} 0.7
+a{quantile="1"} 0.8
 # EOF
 """)
         # The Python client doesn't support quantiles, but we
         # still need to be able to parse them.
         metric_family = SummaryMetricFamily("a", "help", count_value=1, sum_value=2)
         metric_family.add_sample("a", {"quantile": "0.5"}, 0.7)
+        metric_family.add_sample("a", {"quantile": "1"}, 0.8)
         self.assertEqual([metric_family], list(families))
 
     def test_simple_histogram(self):
         families = text_string_to_metric_families("""# TYPE a histogram
 # HELP a help
 a_bucket{le="1.0"} 0
 a_bucket{le="+Inf"} 3
@@ -121,50 +123,56 @@
 """)
         self.assertEqual([HistogramMetricFamily("a", "help", sum_value=2, buckets=[("1.0", 0.0), ("+Inf", 3.0)])],
                          list(families))
 
     def test_histogram_noncanonical(self):
         families = text_string_to_metric_families("""# TYPE a histogram
 # HELP a help
+a_bucket{le="0"} 0
 a_bucket{le="0.00000000001"} 0
+a_bucket{le="0.0000000001"} 0
+a_bucket{le="1e-04"} 0
 a_bucket{le="1.1e-4"} 0
 a_bucket{le="1.1e-3"} 0
+a_bucket{le="1.1e-2"} 0
+a_bucket{le="1"} 0
+a_bucket{le="1e+05"} 0
+a_bucket{le="10000000000"} 0
 a_bucket{le="100000000000.0"} 0
 a_bucket{le="+Inf"} 3
 a_count 3
 a_sum 2
 # EOF
 """)
         list(families)
 
     def test_negative_bucket_histogram(self):
         families = text_string_to_metric_families("""# TYPE a histogram
 # HELP a help
 a_bucket{le="-1.0"} 0
 a_bucket{le="1.0"} 1
 a_bucket{le="+Inf"} 3
-a_count 3
 # EOF
 """)
         self.assertEqual([HistogramMetricFamily("a", "help", buckets=[("-1.0", 0.0), ("1.0", 1.0), ("+Inf", 3.0)])],
                          list(families))
 
     def test_histogram_exemplars(self):
         families = text_string_to_metric_families("""# TYPE a histogram
 # HELP a help
 a_bucket{le="1.0"} 0 # {a="b"} 0.5
 a_bucket{le="2.0"} 2 # {a="c"} 0.5
-a_bucket{le="+Inf"} 3 # {a="1234567890123456789012345678901234567890123456789012345678"} 4 123
+a_bucket{le="+Inf"} 3 # {a="2345678901234567890123456789012345678901234567890123456789012345678901234567890123456789012345678901234567890123456789012345678"} 4 123
 # EOF
 """)
         hfm = HistogramMetricFamily("a", "help")
         hfm.add_sample("a_bucket", {"le": "1.0"}, 0.0, None, Exemplar({"a": "b"}, 0.5))
         hfm.add_sample("a_bucket", {"le": "2.0"}, 2.0, None, Exemplar({"a": "c"}, 0.5)),
         hfm.add_sample("a_bucket", {"le": "+Inf"}, 3.0, None,
-                       Exemplar({"a": "1234567890123456789012345678901234567890123456789012345678"}, 4,
+                       Exemplar({"a": "2345678901234567890123456789012345678901234567890123456789012345678901234567890123456789012345678901234567890123456789012345678"}, 4,
                                 Timestamp(123, 0)))
         self.assertEqual([hfm], list(families))
 
     def test_simple_gaugehistogram(self):
         families = text_string_to_metric_families("""# TYPE a gaugehistogram
 # HELP a help
 a_bucket{le="1.0"} 0
@@ -464,14 +472,15 @@
         hfm.add_sample("a_bucket", {"le": "2.0", "foo": "bar # "}, 2.0, None, Exemplar({"a": "c", "foo": "bar # bar"}, 0.5))
         hfm.add_sample("a_bucket", {"le": "+Inf", "foo": "bar # "}, 3.0, None, Exemplar({"a": "d", "foo": "bar # bar"}, 4))
         self.assertEqual([hfm], list(families))
 
     @unittest.skipIf(sys.version_info < (3, 3), "Test requires Python 3.3+.")
     def test_fallback_to_state_machine_label_parsing(self):
         from unittest.mock import patch
+
         from prometheus_client.openmetrics.parser import _parse_sample
 
         parse_sample_function = "prometheus_client.openmetrics.parser._parse_sample"
         parse_labels_function = "prometheus_client.openmetrics.parser._parse_labels"
         parse_remaining_function = "prometheus_client.openmetrics.parser._parse_remaining_text"
         state_machine_function = "prometheus_client.openmetrics.parser._parse_labels_with_state_machine"
 
@@ -594,14 +603,16 @@
         registry.register(TextCollector())
         self.assertEqual(text.encode('utf-8'), generate_latest(registry))
 
     def test_invalid_input(self):
         for case in [
             # No EOF.
             (''),
+            # Blank line
+            ('a 1\n\n# EOF\n'),
             # Text after EOF.
             ('a 1\n# EOF\nblah'),
             ('a 1\n# EOFblah'),
             # Missing or wrong quotes on label value.
             ('a{a=1} 1\n# EOF\n'),
             ('a{a="1} 1\n# EOF\n'),
             ('a{a=\'1\'} 1\n# EOF\n'),
@@ -688,15 +699,15 @@
             ('# TYPE a histogram\na_bucket{le="+Inf"} 1 #\n# EOF\n'),
             ('# TYPE a histogram\na_bucket{le="+Inf"} 1# {} 1\n# EOF\n'),
             ('# TYPE a histogram\na_bucket{le="+Inf"} 1 #{} 1\n# EOF\n'),
             ('# TYPE a histogram\na_bucket{le="+Inf"} 1 # {}1\n# EOF\n'),
             ('# TYPE a histogram\na_bucket{le="+Inf"} 1 # {} 1 \n# EOF\n'),
             ('# TYPE a histogram\na_bucket{le="+Inf"} 1 # {} 1 1 \n# EOF\n'),
             ('# TYPE a histogram\na_bucket{le="+Inf"} 1 # '
-             '{a="2345678901234567890123456789012345678901234567890123456789012345"} 1 1\n# EOF\n'),
+             '{a="23456789012345678901234567890123456789012345678901234567890123456789012345678901234567890123456789012345678901234567890123456789"} 1 1\n# EOF\n'),
             ('# TYPE a histogram\na_bucket{le="+Inf"} 1 # {} 0x1p-3\n# EOF\n'),
             ('# TYPE a histogram\na_bucket{le="+Inf"} 1 # {} 1 0x1p-3\n# EOF\n'),
             # Exemplars on unallowed samples.
             ('# TYPE a histogram\na_sum 1 # {a="b"} 0.5\n# EOF\n'),
             ('# TYPE a gaugehistogram\na_sum 1 # {a="b"} 0.5\n# EOF\n'),
             ('# TYPE a_bucket gauge\na_bucket 1 # {a="b"} 0.5\n# EOF\n'),
             ('# TYPE a counter\na_created 1 # {a="b"} 0.5\n# EOF\n'),
@@ -711,15 +722,14 @@
             ('# TYPE a info\na 2.0\n# EOF\n'),
             # Missing or invalid labels for a type.
             ('# TYPE a summary\na 0\n# EOF\n'),
             ('# TYPE a summary\na{quantile="-1"} 0\n# EOF\n'),
             ('# TYPE a summary\na{quantile="foo"} 0\n# EOF\n'),
             ('# TYPE a summary\na{quantile="1.01"} 0\n# EOF\n'),
             ('# TYPE a summary\na{quantile="NaN"} 0\n# EOF\n'),
-            ('# TYPE a summary\na{quantile="1"} 0\n# EOF\n'),
             ('# TYPE a histogram\na_bucket 0\n# EOF\n'),
             ('# TYPE a gaugehistogram\na_bucket 0\n# EOF\n'),
             ('# TYPE a stateset\na 0\n# EOF\n'),
             # Bad counter values.
             ('# TYPE a counter\na_total NaN\n# EOF\n'),
             ('# TYPE a counter\na_total -1\n# EOF\n'),
             ('# TYPE a histogram\na_sum NaN\n# EOF\n'),
@@ -738,24 +748,21 @@
             ('# TYPE a summary\na_sum NaN\n# EOF\n'),
             ('# TYPE a summary\na_count NaN\n# EOF\n'),
             ('# TYPE a summary\na_sum -1\n# EOF\n'),
             ('# TYPE a summary\na_count -1\n# EOF\n'),
             ('# TYPE a summary\na{quantile="0.5"} -1\n# EOF\n'),
             # Bad histograms.
             ('# TYPE a histogram\na_sum 1\n# EOF\n'),
+            ('# TYPE a histogram\na_bucket{le="+Inf"} 0\n#a_sum 0\n# EOF\n'),
+            ('# TYPE a histogram\na_bucket{le="+Inf"} 0\n#a_count 0\n# EOF\n'),
             ('# TYPE a gaugehistogram\na_gsum 1\n# EOF\n'),
+            ('# TYPE a gaugehistogram\na_bucket{le="+Inf"} 0\na_gsum 0\n# EOF\n'),
+            ('# TYPE a gaugehistogram\na_bucket{le="+Inf"} 0\na_gcount 0\n# EOF\n'),
             ('# TYPE a histogram\na_count 1\na_bucket{le="+Inf"} 0\n# EOF\n'),
             ('# TYPE a histogram\na_bucket{le="+Inf"} 0\na_count 1\n# EOF\n'),
-            ('# TYPE a histogram\na_bucket{le="0"} 0\na_bucket{le="+Inf"} 0\n# EOF\n'),
-            ('# TYPE a histogram\na_bucket{le="1"} 0\na_bucket{le="+Inf"} 0\n# EOF\n'),
-            ('# TYPE a histogram\na_bucket{le="0.0000000001"} 0\na_bucket{le="+Inf"} 0\n# EOF\n'),
-            ('# TYPE a histogram\na_bucket{le="1.1e-2"} 0\na_bucket{le="+Inf"} 0\n# EOF\n'),
-            ('# TYPE a histogram\na_bucket{le="1e-04"} 0\na_bucket{le="+Inf"} 0\n# EOF\n'),
-            ('# TYPE a histogram\na_bucket{le="1e+05"} 0\na_bucket{le="+Inf"} 0\n# EOF\n'),
-            ('# TYPE a histogram\na_bucket{le="10000000000"} 0\na_bucket{le="+Inf"} 0\n# EOF\n'),
             ('# TYPE a histogram\na_bucket{le="+INF"} 0\n# EOF\n'),
             ('# TYPE a histogram\na_bucket{le="2"} 0\na_bucket{le="1"} 0\na_bucket{le="+Inf"} 0\n# EOF\n'),
             ('# TYPE a histogram\na_bucket{le="1"} 1\na_bucket{le="2"} 1\na_bucket{le="+Inf"} 0\n# EOF\n'),
             # Bad grouping or ordering.
             ('# TYPE a histogram\na_sum{a="1"} 0\na_sum{a="2"} 0\na_count{a="1"} 0\n# EOF\n'),
             ('# TYPE a histogram\na_bucket{a="1",le="1"} 0\na_bucket{a="2",le="+Inf""} '
              '0\na_bucket{a="1",le="+Inf"} 0\n# EOF\n'),
@@ -764,14 +771,18 @@
             ('# TYPE a gauge\na 0 -1\na 0 -2\n# EOF\n'),
             ('# TYPE a gauge\na 0 -1\na 0 -1.1\n# EOF\n'),
             ('# TYPE a gauge\na 0 1\na 0 -1\n# EOF\n'),
             ('# TYPE a gauge\na 0 1.1\na 0 1\n# EOF\n'),
             ('# TYPE a gauge\na 0 1\na 0 0\n# EOF\n'),
             ('# TYPE a gauge\na 0\na 0 0\n# EOF\n'),
             ('# TYPE a gauge\na 0 0\na 0\n# EOF\n'),
+            # Clashing names.
+            ('# TYPE a counter\n# TYPE a counter\n# EOF\n'),
+            ('# TYPE a info\n# TYPE a counter\n# EOF\n'),
+            ('# TYPE a_created gauge\n# TYPE a counter\n# EOF\n'),
         ]:
             with self.assertRaises(ValueError, msg=case):
                 list(text_string_to_metric_families(case))
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `prometheus_client-0.8.0/tests/openmetrics/test_exposition.py` & `prometheus_client-0.9.0/tests/openmetrics/test_exposition.py`

 * *Files identical despite different names*

### Comparing `prometheus_client-0.8.0/tests/test_wsgi.py` & `prometheus_client-0.9.0/tests/test_wsgi.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from __future__ import absolute_import, unicode_literals
 
-import sys
 from unittest import TestCase
 from wsgiref.util import setup_testing_defaults
-from prometheus_client import make_wsgi_app
 
-from prometheus_client import CollectorRegistry, Counter, generate_latest
+from prometheus_client import CollectorRegistry, Counter, make_wsgi_app
 from prometheus_client.exposition import CONTENT_TYPE_LATEST
 
 
 class WSGITest(TestCase):
     def setUp(self):
         self.registry = CollectorRegistry()
         self.captured_status = None
```

### Comparing `prometheus_client-0.8.0/tests/test_parser.py` & `prometheus_client-0.9.0/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `prometheus_client-0.8.0/tests/test_gc_collector.py` & `prometheus_client-0.9.0/tests/test_gc_collector.py`

 * *Files identical despite different names*

### Comparing `prometheus_client-0.8.0/tests/test_twisted.py` & `prometheus_client-0.9.0/tests/test_twisted.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,21 @@
 
 if sys.version_info < (2, 7):
     from unittest2 import skipUnless
 else:
     from unittest import skipUnless
 
 try:
-    from prometheus_client.twisted import MetricsResource
-
+    from twisted.internet import reactor
     from twisted.trial.unittest import TestCase
-    from twisted.web.server import Site
+    from twisted.web.client import Agent, readBody
     from twisted.web.resource import Resource
-    from twisted.internet import reactor
-    from twisted.web.client import Agent
-    from twisted.web.client import readBody
+    from twisted.web.server import Site
+
+    from prometheus_client.twisted import MetricsResource
 
     HAVE_TWISTED = True
 except ImportError:
     from unittest import TestCase
 
     HAVE_TWISTED = False
```

### Comparing `prometheus_client-0.8.0/tests/test_asgi.py` & `prometheus_client-0.9.0/tests/test_asgi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from __future__ import absolute_import, unicode_literals
 
 import sys
 from unittest import TestCase
 
-from prometheus_client import CollectorRegistry, Counter, generate_latest
+from prometheus_client import CollectorRegistry, Counter
 from prometheus_client.exposition import CONTENT_TYPE_LATEST
 
 if sys.version_info < (2, 7):
     from unittest2 import skipUnless
 else:
     from unittest import skipUnless
 
 try:
     # Python >3.5 only
-    from prometheus_client import make_asgi_app
     import asyncio
+
     from asgiref.testing import ApplicationCommunicator
+
+    from prometheus_client import make_asgi_app
     HAVE_ASYNCIO_AND_ASGI = True
 except ImportError:
     HAVE_ASYNCIO_AND_ASGI = False
 
 
 def setup_testing_defaults(scope):
     scope.update(
```

### Comparing `prometheus_client-0.8.0/tests/test_process_collector.py` & `prometheus_client-0.9.0/tests/test_process_collector.py`

 * *Files identical despite different names*

### Comparing `prometheus_client-0.8.0/tests/test_graphite_bridge.py` & `prometheus_client-0.9.0/tests/test_graphite_bridge.py`

 * *Files identical despite different names*

### Comparing `prometheus_client-0.8.0/tests/test_core.py` & `prometheus_client-0.9.0/tests/test_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import unicode_literals
 
 from concurrent.futures import ThreadPoolExecutor
-import inspect
 import time
 
 import pytest
 
 from prometheus_client.core import (
     CollectorRegistry, Counter, CounterMetricFamily, Enum, Gauge,
     GaugeHistogramMetricFamily, GaugeMetricFamily, Histogram,
     HistogramMetricFamily, Info, InfoMetricFamily, Metric, Sample,
     StateSetMetricFamily, Summary, SummaryMetricFamily, UntypedMetricFamily,
 )
+from prometheus_client.decorator import getargspec
 
 try:
     import unittest2 as unittest
 except ImportError:
     import unittest
 
 
@@ -42,15 +42,15 @@
         @self.counter.count_exceptions(ValueError)
         def f(r):
             if r:
                 raise ValueError
             else:
                 raise TypeError
 
-        self.assertEqual((["r"], None, None, None), inspect.getargspec(f))
+        self.assertEqual((["r"], None, None, None), getargspec(f))
 
         try:
             f(False)
         except TypeError:
             pass
         self.assertEqual(0, self.registry.get_sample_value('c_total'))
 
@@ -103,15 +103,15 @@
     def test_inprogress_function_decorator(self):
         self.assertEqual(0, self.registry.get_sample_value('g'))
 
         @self.gauge.track_inprogress()
         def f():
             self.assertEqual(1, self.registry.get_sample_value('g'))
 
-        self.assertEqual(([], None, None, None), inspect.getargspec(f))
+        self.assertEqual(([], None, None, None), getargspec(f))
 
         f()
         self.assertEqual(0, self.registry.get_sample_value('g'))
 
     def test_inprogress_block_decorator(self):
         self.assertEqual(0, self.registry.get_sample_value('g'))
         with self.gauge.track_inprogress():
@@ -130,15 +130,15 @@
     def test_time_function_decorator(self):
         self.assertEqual(0, self.registry.get_sample_value('g'))
 
         @self.gauge.time()
         def f():
             time.sleep(.001)
 
-        self.assertEqual(([], None, None, None), inspect.getargspec(f))
+        self.assertEqual(([], None, None, None), getargspec(f))
 
         f()
         self.assertNotEqual(0, self.registry.get_sample_value('g'))
 
     def test_function_decorator_multithread(self):
         self.assertEqual(0, self.registry.get_sample_value('g'))
         workers = 2
@@ -200,15 +200,15 @@
     def test_function_decorator(self):
         self.assertEqual(0, self.registry.get_sample_value('s_count'))
 
         @self.summary.time()
         def f():
             pass
 
-        self.assertEqual(([], None, None, None), inspect.getargspec(f))
+        self.assertEqual(([], None, None, None), getargspec(f))
 
         f()
         self.assertEqual(1, self.registry.get_sample_value('s_count'))
 
     def test_function_decorator_multithread(self):
         self.assertEqual(0, self.registry.get_sample_value('s_count'))
         summary2 = Summary('s2', 'help', registry=self.registry)
@@ -341,15 +341,15 @@
         self.assertEqual(0, self.registry.get_sample_value('h_count'))
         self.assertEqual(0, self.registry.get_sample_value('h_bucket', {'le': '+Inf'}))
 
         @self.histogram.time()
         def f():
             pass
 
-        self.assertEqual(([], None, None, None), inspect.getargspec(f))
+        self.assertEqual(([], None, None, None), getargspec(f))
 
         f()
         self.assertEqual(1, self.registry.get_sample_value('h_count'))
         self.assertEqual(1, self.registry.get_sample_value('h_bucket', {'le': '+Inf'}))
 
     def test_function_decorator_multithread(self):
         self.assertEqual(0, self.registry.get_sample_value('h_count'))
@@ -524,17 +524,16 @@
         self.assertEqual(0, self.registry.get_sample_value('h_seconds_sum'))
 
     def test_no_units_for_info_enum(self):
         self.assertRaises(ValueError, Info, 'foo', 'help', unit="x")
         self.assertRaises(ValueError, Enum, 'foo', 'help', unit="x")
 
     def test_name_cleanup_before_unit_append(self):
-        self.assertEqual(self.counter._name, 'c')
-        self.c = Counter('c_total', 'help', unit="total", labelnames=['l'], registry=self.registry)
-        self.assertEqual(self.c._name, 'c_total')
+        c = Counter('b_total', 'help', unit="total", labelnames=['l'], registry=self.registry)
+        self.assertEqual(c._name, 'b_total')
 
 
 class TestMetricFamilies(unittest.TestCase):
     def setUp(self):
         self.registry = CollectorRegistry()
 
     def custom_collector(self, metric_family):
@@ -713,16 +712,16 @@
         self.assertRaises(ValueError, Histogram, 'h', 'help', registry=registry)
         # Clashes aggaint various suffixes.
         self.assertRaises(ValueError, Summary, 'h', 'help', registry=registry)
         self.assertRaises(ValueError, Gauge, 'h_count', 'help', registry=registry)
         self.assertRaises(ValueError, Gauge, 'h_sum', 'help', registry=registry)
         self.assertRaises(ValueError, Gauge, 'h_bucket', 'help', registry=registry)
         self.assertRaises(ValueError, Gauge, 'h_created', 'help', registry=registry)
-        # The name of the histogram itself isn't taken.
-        Gauge('h', 'help', registry=registry)
+        # The name of the histogram itself is also taken.
+        self.assertRaises(ValueError, Gauge, 'h', 'help', registry=registry)
 
         Info('i', 'help', registry=registry)
         self.assertRaises(ValueError, Gauge, 'i_info', 'help', registry=registry)
 
     def test_unregister_works(self):
         registry = CollectorRegistry()
         s = Summary('s', 'help', registry=registry)
@@ -749,15 +748,15 @@
     def test_restricted_registry(self):
         registry = CollectorRegistry()
         Counter('c_total', 'help', registry=registry)
         Summary('s', 'help', registry=registry).observe(7)
 
         m = Metric('s', 'help', 'summary')
         m.samples = [Sample('s_sum', {}, 7)]
-        self.assertEquals([m], registry.restricted_registry(['s_sum']).collect())
+        self.assertEqual([m], registry.restricted_registry(['s_sum']).collect())
 
     def test_target_info_injected(self):
         registry = CollectorRegistry(target_info={'foo': 'bar'})
         self.assertEqual(1, registry.get_sample_value('target_info', {'foo': 'bar'}))
 
     def test_target_info_duplicate_detected(self):
         registry = CollectorRegistry(target_info={'foo': 'bar'})
@@ -773,16 +772,16 @@
 
     def test_target_info_restricted_registry(self):
         registry = CollectorRegistry(target_info={'foo': 'bar'})
         Summary('s', 'help', registry=registry).observe(7)
 
         m = Metric('s', 'help', 'summary')
         m.samples = [Sample('s_sum', {}, 7)]
-        self.assertEquals([m], registry.restricted_registry(['s_sum']).collect())
+        self.assertEqual([m], registry.restricted_registry(['s_sum']).collect())
 
         m = Metric('target', 'Target metadata', 'info')
         m.samples = [Sample('target_info', {'foo': 'bar'}, 1)]
-        self.assertEquals([m], registry.restricted_registry(['target_info']).collect())
+        self.assertEqual([m], registry.restricted_registry(['target_info']).collect())
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `prometheus_client-0.8.0/tests/test_multiprocess.py` & `prometheus_client-0.9.0/tests/test_multiprocess.py`

 * *Files identical despite different names*

### Comparing `prometheus_client-0.8.0/PKG-INFO` & `prometheus_client-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prometheus_client
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python client for the Prometheus monitoring system.
 Home-page: https://github.com/prometheus/client_python
 Author: Brian Brazil
 Author-email: brian.brazil@robustperception.io
 License: Apache Software License 2.0
 Description: # Prometheus Python Client
         
@@ -224,14 +224,25 @@
         ```python
         from prometheus_client import Counter
         c = Counter('my_requests_total', 'HTTP Failures', ['method', 'endpoint'])
         c.labels(method='get', endpoint='/').inc()
         c.labels(method='post', endpoint='/submit').inc()
         ```
         
+        Metrics with labels are not initialized when declared, because the client can't
+        know what values the label can have. It is recommended to initialize the label
+        values by calling the `.labels()` method alone:
+        
+        ```python
+        from prometheus_client import Counter
+        c = Counter('my_requests_total', 'HTTP Failures', ['method', 'endpoint'])
+        c.labels('get', '/')
+        c.labels('post', '/submit')
+        ```
+        
         ### Process Collector
         
         The Python client automatically exports metrics about process CPU usage, RAM,
         file descriptors and start time. These all have the prefix `process`, and
         are only currently available on Linux.
         
         The namespace and pid constructor arguments allows for exporting metrics about
@@ -338,25 +349,25 @@
         from werkzeug.middleware.dispatcher import DispatcherMiddleware
         from prometheus_client import make_wsgi_app
         
         # Create my app
         app = Flask(__name__)
         
         # Add prometheus wsgi middleware to route /metrics requests
-        app_dispatch = DispatcherMiddleware(app, {
+        app.wsgi_app = DispatcherMiddleware(app.wsgi_app, {
             '/metrics': make_wsgi_app()
         })
         ```
         
         Run the example web application like this
         
         ```bash
         # Install uwsgi if you do not have it
         pip install uwsgi
-        uwsgi --http 127.0.0.1:8000 --wsgi-file myapp.py --callable app_dispatch
+        uwsgi --http 127.0.0.1:8000 --wsgi-file myapp.py --callable app
         ```
         
         Visit http://localhost:8000/metrics to see the metrics
         
         ### Node exporter textfile collector
         
         The [textfile collector](https://github.com/prometheus/node_exporter#textfile-collector)
@@ -585,13 +596,14 @@
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: System :: Monitoring
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
 Provides-Extra: twisted
```

### Comparing `prometheus_client-0.8.0/setup.py` & `prometheus_client-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-from setuptools import setup
-import sys
 from os import path
+import sys
+
+from setuptools import setup
 
 if sys.version_info >= (2, 7):
     with open(path.join(path.abspath(path.dirname(__file__)), 'README.md')) as f:
         long_description = f.read()
-else: # Assuming we don't run setup in order to publish under python 2.6
+else:  # Assuming we don't run setup in order to publish under python 2.6
     long_description = "NA"
 
 
 setup(
     name="prometheus_client",
-    version="0.8.0",
+    version="0.9.0",
     author="Brian Brazil",
     author_email="brian.brazil@robustperception.io",
     description="Python client for the Prometheus monitoring system.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="Apache Software License 2.0",
     keywords="prometheus monitoring instrumentation client",
@@ -41,14 +42,15 @@
         "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.4",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Topic :: System :: Monitoring",
         "License :: OSI Approved :: Apache Software License",
     ],
     options={'bdist_wheel': {'universal': '1'}},
 )
```

