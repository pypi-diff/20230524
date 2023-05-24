# Comparing `tmp/nonecorn-0.14.1.dev1.tar.gz` & `tmp/nonecorn-0.14.3.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonecorn-0.14.1.dev1.tar", last modified: Tue Aug 30 15:33:03 2022, max compression
+gzip compressed data, was "nonecorn-0.14.3.dev1.tar", last modified: Wed May 24 10:08:42 2023, max compression
```

## Comparing `nonecorn-0.14.1.dev1.tar` & `nonecorn-0.14.3.dev1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2022-08-30 15:33:03.174720 nonecorn-0.14.1.dev1/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1050 2022-08-30 15:28:56.000000 nonecorn-0.14.1.dev1/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       30 2022-08-30 15:28:56.000000 nonecorn-0.14.1.dev1/MANIFEST.in
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4753 2022-08-30 15:33:03.174720 nonecorn-0.14.1.dev1/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3680 2022-08-30 15:28:56.000000 nonecorn-0.14.1.dev1/README.rst
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2801 2022-08-30 15:28:56.000000 nonecorn-0.14.1.dev1/pyproject.toml
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      146 2022-08-30 15:33:03.174720 nonecorn-0.14.1.dev1/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2077 2022-08-30 15:28:56.000000 nonecorn-0.14.1.dev1/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2022-08-30 15:33:03.166720 nonecorn-0.14.1.dev1/src/
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2022-08-30 15:33:03.166720 nonecorn-0.14.1.dev1/src/hypercorn/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       86 2022-08-30 15:28:56.000000 nonecorn-0.14.1.dev1/src/hypercorn/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10295 2022-08-30 15:28:56.000000 nonecorn-0.14.1.dev1/src/hypercorn/__main__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4742 2022-08-30 15:28:56.000000 nonecorn-0.14.1.dev1/src/hypercorn/app_wrappers.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2022-08-30 15:33:03.166720 nonecorn-0.14.1.dev1/src/hypercorn/asyncio/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1556 2022-08-30 15:28:56.000000 nonecorn-0.14.1.dev1/src/hypercorn/asyncio/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3582 2022-08-30 15:28:56.000000 nonecorn-0.14.1.dev1/src/hypercorn/asyncio/lifespan.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8841 2022-08-30 15:28:56.000000 nonecorn-0.14.1.dev1/src/hypercorn/asyncio/run.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      769 2022-08-30 15:28:56.000000 nonecorn-0.14.1.dev1/src/hypercorn/asyncio/statsd.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2313 2022-08-30 15:28:56.000000 nonecorn-0.14.1.dev1/src/hypercorn/asyncio/task_group.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6074 2022-08-30 15:28:56.000000 nonecorn-0.14.1.dev1/src/hypercorn/asyncio/tcp_server.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2960 2022-08-30 15:28:56.000000 nonecorn-0.14.1.dev1/src/hypercorn/asyncio/udp_server.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      811 2022-08-30 15:28:56.000000 nonecorn-0.14.1.dev1/src/hypercorn/asyncio/worker_context.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    13569 2022-08-30 15:28:56.000000 nonecorn-0.14.1.dev1/src/hypercorn/config.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      525 2022-08-30 15:28:56.000000 nonecorn-0.14.1.dev1/src/hypercorn/events.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7116 2022-08-30 15:28:56.000000 nonecorn-0.14.1.dev1/src/hypercorn/logging.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2022-08-30 15:33:03.170720 nonecorn-0.14.1.dev1/src/hypercorn/middleware/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      333 2022-08-30 15:28:56.000000 nonecorn-0.14.1.dev1/src/hypercorn/middleware/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4306 2022-08-30 15:28:56.000000 nonecorn-0.14.1.dev1/src/hypercorn/middleware/dispatcher.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2619 2022-08-30 15:28:56.000000 nonecorn-0.14.1.dev1/src/hypercorn/middleware/http_to_https.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1281 2022-08-30 15:28:56.000000 nonecorn-0.14.1.dev1/src/hypercorn/middleware/wsgi.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2022-08-30 15:33:03.170720 nonecorn-0.14.1.dev1/src/hypercorn/protocol/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2919 2022-08-30 15:28:56.000000 nonecorn-0.14.1.dev1/src/hypercorn/protocol/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1465 2022-08-30 15:28:56.000000 nonecorn-0.14.1.dev1/src/hypercorn/protocol/events.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12821 2022-08-30 15:28:56.000000 nonecorn-0.14.1.dev1/src/hypercorn/protocol/h11.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    16252 2022-08-30 15:28:56.000000 nonecorn-0.14.1.dev1/src/hypercorn/protocol/h2.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5782 2022-08-30 15:28:56.000000 nonecorn-0.14.1.dev1/src/hypercorn/protocol/h3.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12418 2022-08-30 15:28:56.000000 nonecorn-0.14.1.dev1/src/hypercorn/protocol/http_stream.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5097 2022-08-30 15:28:56.000000 nonecorn-0.14.1.dev1/src/hypercorn/protocol/quic.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15490 2022-08-30 15:28:56.000000 nonecorn-0.14.1.dev1/src/hypercorn/protocol/ws_stream.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        7 2022-08-30 15:28:56.000000 nonecorn-0.14.1.dev1/src/hypercorn/py.typed
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2881 2022-08-30 15:28:56.000000 nonecorn-0.14.1.dev1/src/hypercorn/run.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3832 2022-08-30 15:28:56.000000 nonecorn-0.14.1.dev1/src/hypercorn/statsd.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2022-08-30 15:33:03.170720 nonecorn-0.14.1.dev1/src/hypercorn/trio/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1665 2022-08-30 15:28:56.000000 nonecorn-0.14.1.dev1/src/hypercorn/trio/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3391 2022-08-30 15:28:56.000000 nonecorn-0.14.1.dev1/src/hypercorn/trio/lifespan.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4397 2022-08-30 15:28:56.000000 nonecorn-0.14.1.dev1/src/hypercorn/trio/run.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      493 2022-08-30 15:28:56.000000 nonecorn-0.14.1.dev1/src/hypercorn/trio/statsd.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2266 2022-08-30 15:28:56.000000 nonecorn-0.14.1.dev1/src/hypercorn/trio/task_group.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5015 2022-08-30 15:28:56.000000 nonecorn-0.14.1.dev1/src/hypercorn/trio/tcp_server.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1514 2022-08-30 15:28:56.000000 nonecorn-0.14.1.dev1/src/hypercorn/trio/udp_server.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      798 2022-08-30 15:28:56.000000 nonecorn-0.14.1.dev1/src/hypercorn/trio/worker_context.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7720 2022-08-30 15:28:56.000000 nonecorn-0.14.1.dev1/src/hypercorn/typing.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9487 2022-08-30 15:28:56.000000 nonecorn-0.14.1.dev1/src/hypercorn/utils.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5738 2022-08-30 15:28:56.000000 nonecorn-0.14.1.dev1/src/hypercorn/workers.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2022-08-30 15:33:03.174720 nonecorn-0.14.1.dev1/src/nonecorn.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4753 2022-08-30 15:33:03.000000 nonecorn-0.14.1.dev1/src/nonecorn.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1519 2022-08-30 15:33:03.000000 nonecorn-0.14.1.dev1/src/nonecorn.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2022-08-30 15:33:03.000000 nonecorn-0.14.1.dev1/src/nonecorn.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       55 2022-08-30 15:33:03.000000 nonecorn-0.14.1.dev1/src/nonecorn.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      235 2022-08-30 15:33:03.000000 nonecorn-0.14.1.dev1/src/nonecorn.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       10 2022-08-30 15:33:03.000000 nonecorn-0.14.1.dev1/src/nonecorn.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-24 10:08:42.313403 nonecorn-0.14.3.dev1/
+-rw-rw-rw-   0        0        0     1072 2023-03-10 03:15:15.000000 nonecorn-0.14.3.dev1/LICENSE
+-rw-rw-rw-   0        0        0       30 2023-05-24 06:47:35.000000 nonecorn-0.14.3.dev1/MANIFEST.in
+-rw-rw-rw-   0        0        0     4879 2023-05-24 10:08:42.313914 nonecorn-0.14.3.dev1/PKG-INFO
+-rw-rw-rw-   0        0        0     3798 2023-05-24 06:47:35.000000 nonecorn-0.14.3.dev1/README.rst
+-rw-rw-rw-   0        0        0     2934 2023-05-24 06:47:35.000000 nonecorn-0.14.3.dev1/pyproject.toml
+-rw-rw-rw-   0        0        0      156 2023-05-24 10:08:42.314293 nonecorn-0.14.3.dev1/setup.cfg
+-rw-rw-rw-   0        0        0     2148 2023-05-24 10:08:28.000000 nonecorn-0.14.3.dev1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 10:08:42.264329 nonecorn-0.14.3.dev1/src/
+drwxrwxrwx   0        0        0        0 2023-05-24 10:08:42.280967 nonecorn-0.14.3.dev1/src/hypercorn/
+-rw-rw-rw-   0        0        0       91 2023-03-10 03:15:15.000000 nonecorn-0.14.3.dev1/src/hypercorn/__init__.py
+-rw-rw-rw-   0        0        0    10631 2023-03-10 03:15:15.000000 nonecorn-0.14.3.dev1/src/hypercorn/__main__.py
+-rw-rw-rw-   0        0        0     5262 2023-03-10 03:15:15.000000 nonecorn-0.14.3.dev1/src/hypercorn/app_wrappers.py
+drwxrwxrwx   0        0        0        0 2023-05-24 10:08:42.288621 nonecorn-0.14.3.dev1/src/hypercorn/asyncio/
+-rw-rw-rw-   0        0        0     1607 2023-03-10 03:15:15.000000 nonecorn-0.14.3.dev1/src/hypercorn/asyncio/__init__.py
+-rw-rw-rw-   0        0        0     4069 2023-05-24 05:53:19.000000 nonecorn-0.14.3.dev1/src/hypercorn/asyncio/lifespan.py
+-rw-rw-rw-   0        0        0     9160 2023-05-24 05:53:19.000000 nonecorn-0.14.3.dev1/src/hypercorn/asyncio/run.py
+-rw-rw-rw-   0        0        0      795 2023-03-10 03:15:15.000000 nonecorn-0.14.3.dev1/src/hypercorn/asyncio/statsd.py
+-rw-rw-rw-   0        0        0     2636 2023-03-10 03:15:15.000000 nonecorn-0.14.3.dev1/src/hypercorn/asyncio/task_group.py
+-rw-rw-rw-   0        0        0     6360 2023-05-24 06:47:35.000000 nonecorn-0.14.3.dev1/src/hypercorn/asyncio/tcp_server.py
+-rw-rw-rw-   0        0        0     3139 2023-05-24 06:47:35.000000 nonecorn-0.14.3.dev1/src/hypercorn/asyncio/udp_server.py
+-rw-rw-rw-   0        0        0      849 2023-03-10 03:15:15.000000 nonecorn-0.14.3.dev1/src/hypercorn/asyncio/worker_context.py
+-rw-rw-rw-   0        0        0    14098 2023-05-24 06:47:35.000000 nonecorn-0.14.3.dev1/src/hypercorn/config.py
+-rw-rw-rw-   0        0        0      557 2023-05-24 06:47:35.000000 nonecorn-0.14.3.dev1/src/hypercorn/events.py
+-rw-rw-rw-   0        0        0     7397 2023-03-10 03:15:16.000000 nonecorn-0.14.3.dev1/src/hypercorn/logging.py
+drwxrwxrwx   0        0        0        0 2023-05-24 10:08:42.292166 nonecorn-0.14.3.dev1/src/hypercorn/middleware/
+-rw-rw-rw-   0        0        0      345 2023-03-10 03:15:16.000000 nonecorn-0.14.3.dev1/src/hypercorn/middleware/__init__.py
+-rw-rw-rw-   0        0        0     4414 2023-03-10 03:15:16.000000 nonecorn-0.14.3.dev1/src/hypercorn/middleware/dispatcher.py
+-rw-rw-rw-   0        0        0     2686 2023-03-10 03:15:16.000000 nonecorn-0.14.3.dev1/src/hypercorn/middleware/http_to_https.py
+-rw-rw-rw-   0        0        0     1538 2023-03-10 03:15:16.000000 nonecorn-0.14.3.dev1/src/hypercorn/middleware/wsgi.py
+drwxrwxrwx   0        0        0        0 2023-05-24 10:08:42.299716 nonecorn-0.14.3.dev1/src/hypercorn/protocol/
+-rw-rw-rw-   0        0        0     3235 2023-05-24 06:47:35.000000 nonecorn-0.14.3.dev1/src/hypercorn/protocol/__init__.py
+-rw-rw-rw-   0        0        0     1539 2023-05-24 06:47:35.000000 nonecorn-0.14.3.dev1/src/hypercorn/protocol/events.py
+-rw-rw-rw-   0        0        0    13330 2023-05-24 06:47:35.000000 nonecorn-0.14.3.dev1/src/hypercorn/protocol/h11.py
+-rw-rw-rw-   0        0        0    16826 2023-05-24 06:47:35.000000 nonecorn-0.14.3.dev1/src/hypercorn/protocol/h2.py
+-rw-rw-rw-   0        0        0     6082 2023-05-24 06:47:35.000000 nonecorn-0.14.3.dev1/src/hypercorn/protocol/h3.py
+-rw-rw-rw-   0        0        0    12487 2023-05-24 06:47:35.000000 nonecorn-0.14.3.dev1/src/hypercorn/protocol/http_stream.py
+-rw-rw-rw-   0        0        0     5346 2023-05-24 05:53:19.000000 nonecorn-0.14.3.dev1/src/hypercorn/protocol/quic.py
+-rw-rw-rw-   0        0        0    16039 2023-05-24 06:47:35.000000 nonecorn-0.14.3.dev1/src/hypercorn/protocol/ws_stream.py
+-rw-rw-rw-   0        0        0        8 2023-03-10 03:15:16.000000 nonecorn-0.14.3.dev1/src/hypercorn/py.typed
+-rw-rw-rw-   0        0        0     3454 2023-05-24 06:47:35.000000 nonecorn-0.14.3.dev1/src/hypercorn/run.py
+-rw-rw-rw-   0        0        0     3927 2023-03-10 03:15:16.000000 nonecorn-0.14.3.dev1/src/hypercorn/statsd.py
+drwxrwxrwx   0        0        0        0 2023-05-24 10:08:42.306961 nonecorn-0.14.3.dev1/src/hypercorn/trio/
+-rw-rw-rw-   0        0        0     1722 2023-03-10 03:15:16.000000 nonecorn-0.14.3.dev1/src/hypercorn/trio/__init__.py
+-rw-rw-rw-   0        0        0     3726 2023-05-24 05:53:19.000000 nonecorn-0.14.3.dev1/src/hypercorn/trio/lifespan.py
+-rw-rw-rw-   0        0        0     4569 2023-05-24 06:47:42.000000 nonecorn-0.14.3.dev1/src/hypercorn/trio/run.py
+-rw-rw-rw-   0        0        0      509 2023-03-10 03:15:16.000000 nonecorn-0.14.3.dev1/src/hypercorn/trio/statsd.py
+-rw-rw-rw-   0        0        0     2485 2023-03-10 03:15:16.000000 nonecorn-0.14.3.dev1/src/hypercorn/trio/task_group.py
+-rw-rw-rw-   0        0        0     5267 2023-05-24 05:53:19.000000 nonecorn-0.14.3.dev1/src/hypercorn/trio/tcp_server.py
+-rw-rw-rw-   0        0        0     1678 2023-05-24 05:53:19.000000 nonecorn-0.14.3.dev1/src/hypercorn/trio/udp_server.py
+-rw-rw-rw-   0        0        0      837 2023-03-10 03:15:16.000000 nonecorn-0.14.3.dev1/src/hypercorn/trio/worker_context.py
+-rw-rw-rw-   0        0        0     8138 2023-05-24 06:47:35.000000 nonecorn-0.14.3.dev1/src/hypercorn/typing.py
+-rw-rw-rw-   0        0        0     9813 2023-05-24 06:47:35.000000 nonecorn-0.14.3.dev1/src/hypercorn/utils.py
+-rw-rw-rw-   0        0        0     6305 2023-05-24 06:47:35.000000 nonecorn-0.14.3.dev1/src/hypercorn/workers.py
+drwxrwxrwx   0        0        0        0 2023-05-24 10:08:42.312510 nonecorn-0.14.3.dev1/src/nonecorn.egg-info/
+-rw-rw-rw-   0        0        0     4879 2023-05-24 10:08:42.000000 nonecorn-0.14.3.dev1/src/nonecorn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1519 2023-05-24 10:08:42.000000 nonecorn-0.14.3.dev1/src/nonecorn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 10:08:42.000000 nonecorn-0.14.3.dev1/src/nonecorn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-05-24 10:08:42.000000 nonecorn-0.14.3.dev1/src/nonecorn.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      235 2023-05-24 10:08:42.000000 nonecorn-0.14.3.dev1/src/nonecorn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-24 10:08:42.000000 nonecorn-0.14.3.dev1/src/nonecorn.egg-info/top_level.txt
```

### Comparing `nonecorn-0.14.1.dev1/LICENSE` & `nonecorn-0.14.3.dev1/LICENSE`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-Copyright P G Jones 2018.
-
-Permission is hereby granted, free of charge, to any person
-obtaining a copy of this software and associated documentation
-files (the "Software"), to deal in the Software without
-restriction, including without limitation the rights to use,
-copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the
-Software is furnished to do so, subject to the following
-conditions:
-
-The above copyright notice and this permission notice shall be
-included in all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
-EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES
-OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
-NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
-HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
-WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
-FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
-OTHER DEALINGS IN THE SOFTWARE.
+Copyright P G Jones 2018.
+
+Permission is hereby granted, free of charge, to any person
+obtaining a copy of this software and associated documentation
+files (the "Software"), to deal in the Software without
+restriction, including without limitation the rights to use,
+copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the
+Software is furnished to do so, subject to the following
+conditions:
+
+The above copyright notice and this permission notice shall be
+included in all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES
+OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
+NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
+HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
+WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
+OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `nonecorn-0.14.1.dev1/PKG-INFO` & `nonecorn-0.14.3.dev1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,149 +1,146 @@
-Metadata-Version: 2.1
-Name: nonecorn
-Version: 0.14.1.dev1
-Summary: A ASGI Server forked from hypercorn with more extra feature beyond ASGI
-Home-page: https://gitlab.com/pgjones/hypercorn/
-Author: P G Jones
-Author-email: philip.graham.jones@googlemail.com
-License: MIT
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
-Provides-Extra: h3
-Provides-Extra: tests
-Provides-Extra: trio
-Provides-Extra: uvloop
-License-File: LICENSE
-
-Hypercorn is now hosted at `github.com/pgjones/hypercorn
-<https://github.com/pgjones/hypercorn>`_.
-
-
-Hypercorn
-=========
-
-.. image:: https://github.com/pgjones/hypercorn/raw/main/artwork/logo.png
-   :alt: Hypercorn logo
-
-|Build Status| |docs| |pypi| |http| |python| |license|
-
-Hypercorn is an `ASGI
-<https://github.com/django/asgiref/blob/main/specs/asgi.rst>`_ and
-WSGI web server based on the sans-io hyper, `h11
-<https://github.com/python-hyper/h11>`_, `h2
-<https://github.com/python-hyper/hyper-h2>`_, and `wsproto
-<https://github.com/python-hyper/wsproto>`_ libraries and inspired by
-Gunicorn. Hypercorn supports HTTP/1, HTTP/2, WebSockets (over HTTP/1
-and HTTP/2), ASGI, and WSGI specifications. Hypercorn can utilise
-asyncio, uvloop, or trio worker types.
-
-Hypercorn can optionally serve the current draft of the HTTP/3
-specification using the `aioquic
-<https://github.com/aiortc/aioquic/>`_ library. To enable this install
-the ``h3`` optional extra, ``pip install hypercorn[h3]`` and then
-choose a quic binding e.g. ``hypercorn --quic-bind localhost:4433
-...``.
-
-Hypercorn was initially part of `Quart
-<https://github.com/pgjones/quart>`_ before being separated out into a
-standalone server. Hypercorn forked from version 0.5.0 of Quart.
-
-Quickstart
-----------
-
-Hypercorn can be installed via `pip
-<https://docs.python.org/3/installing/index.html>`_,
-
-.. code-block:: console
-
-    $ pip install hypercorn
-
-and requires Python 3.7.0 or higher.
-
-With hypercorn installed ASGI frameworks (or apps) can be served via
-Hypercorn via the command line,
-
-.. code-block:: console
-
-    $ hypercorn module:app
-
-Alternatively Hypercorn can be used programatically,
-
-.. code-block:: python
-
-    import asyncio
-    from hypercorn.config import Config
-    from hypercorn.asyncio import serve
-
-    from module import app
-
-    asyncio.run(serve(app, Config()))
-
-learn more (including a Trio example of the above) in the `API usage
-<https://hypercorn.readthedocs.io/en/latest/how_to_guides/api_usage.html>`_
-docs.
-
-Contributing
-------------
-
-Hypercorn is developed on `Github
-<https://github.com/pgjones/hypercorn>`_. If you come across an issue,
-or have a feature request please open an `issue
-<https://github.com/pgjones/hypercorn/issues>`_.  If you want to
-contribute a fix or the feature-implementation please do (typo fixes
-welcome), by proposing a `pull request
-<https://github.com/pgjones/hypercorn/merge_requests>`_.
-
-Testing
-~~~~~~~
-
-The best way to test Hypercorn is with `Tox
-<https://tox.readthedocs.io>`_,
-
-.. code-block:: console
-
-    $ pipenv install tox
-    $ tox
-
-this will check the code style and run the tests.
-
-Help
-----
-
-The Hypercorn `documentation <https://hypercorn.readthedocs.io>`_ is
-the best place to start, after that try searching stack overflow, if
-you still can't find an answer please `open an issue
-<https://github.com/pgjones/hypercorn/issues>`_.
-
-
-.. |Build Status| image:: https://github.com/pgjones/hypercorn/actions/workflows/ci.yml/badge.svg
-   :target: https://github.com/pgjones/hypercorn/commits/main
-
-.. |docs| image:: https://img.shields.io/badge/docs-passing-brightgreen.svg
-   :target: https://hypercorn.readthedocs.io
-
-.. |pypi| image:: https://img.shields.io/pypi/v/hypercorn.svg
-   :target: https://pypi.python.org/pypi/Hypercorn/
-
-.. |http| image:: https://img.shields.io/badge/http-1.0,1.1,2-orange.svg
-   :target: https://en.wikipedia.org/wiki/Hypertext_Transfer_Protocol
-
-.. |python| image:: https://img.shields.io/pypi/pyversions/hypercorn.svg
-   :target: https://pypi.python.org/pypi/Hypercorn/
-
-.. |license| image:: https://img.shields.io/badge/license-MIT-blue.svg
-   :target: https://github.com/pgjones/hypercorn/blob/main/LICENSE
-
-
+Metadata-Version: 2.1
+Name: nonecorn
+Version: 0.14.3.dev1
+Summary: A ASGI Server forked from hypercorn with more extra feature beyond ASGI
+Home-page: https://gitlab.com/pgjones/hypercorn/
+Author: P G Jones
+Author-email: philip.graham.jones@googlemail.com
+License: MIT
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.7
+Provides-Extra: h3
+Provides-Extra: tests
+Provides-Extra: trio
+Provides-Extra: uvloop
+License-File: LICENSE
+
+Hypercorn is now hosted at `github.com/pgjones/hypercorn
+<https://github.com/pgjones/hypercorn>`_.
+
+
+Hypercorn
+=========
+
+.. image:: https://github.com/pgjones/hypercorn/raw/main/artwork/logo.png
+   :alt: Hypercorn logo
+
+|Build Status| |docs| |pypi| |http| |python| |license|
+
+Hypercorn is an `ASGI
+<https://github.com/django/asgiref/blob/main/specs/asgi.rst>`_ and
+WSGI web server based on the sans-io hyper, `h11
+<https://github.com/python-hyper/h11>`_, `h2
+<https://github.com/python-hyper/hyper-h2>`_, and `wsproto
+<https://github.com/python-hyper/wsproto>`_ libraries and inspired by
+Gunicorn. Hypercorn supports HTTP/1, HTTP/2, WebSockets (over HTTP/1
+and HTTP/2), ASGI, and WSGI specifications. Hypercorn can utilise
+asyncio, uvloop, or trio worker types.
+
+Hypercorn can optionally serve the current draft of the HTTP/3
+specification using the `aioquic
+<https://github.com/aiortc/aioquic/>`_ library. To enable this install
+the ``h3`` optional extra, ``pip install hypercorn[h3]`` and then
+choose a quic binding e.g. ``hypercorn --quic-bind localhost:4433
+...``.
+
+Hypercorn was initially part of `Quart
+<https://github.com/pgjones/quart>`_ before being separated out into a
+standalone server. Hypercorn forked from version 0.5.0 of Quart.
+
+Quickstart
+----------
+
+Hypercorn can be installed via `pip
+<https://docs.python.org/3/installing/index.html>`_,
+
+.. code-block:: console
+
+    $ pip install hypercorn
+
+and requires Python 3.7.0 or higher.
+
+With hypercorn installed ASGI frameworks (or apps) can be served via
+Hypercorn via the command line,
+
+.. code-block:: console
+
+    $ hypercorn module:app
+
+Alternatively Hypercorn can be used programatically,
+
+.. code-block:: python
+
+    import asyncio
+    from hypercorn.config import Config
+    from hypercorn.asyncio import serve
+
+    from module import app
+
+    asyncio.run(serve(app, Config()))
+
+learn more (including a Trio example of the above) in the `API usage
+<https://hypercorn.readthedocs.io/en/latest/how_to_guides/api_usage.html>`_
+docs.
+
+Contributing
+------------
+
+Hypercorn is developed on `Github
+<https://github.com/pgjones/hypercorn>`_. If you come across an issue,
+or have a feature request please open an `issue
+<https://github.com/pgjones/hypercorn/issues>`_.  If you want to
+contribute a fix or the feature-implementation please do (typo fixes
+welcome), by proposing a `pull request
+<https://github.com/pgjones/hypercorn/merge_requests>`_.
+
+Testing
+~~~~~~~
+
+The best way to test Hypercorn is with `Tox
+<https://tox.readthedocs.io>`_,
+
+.. code-block:: console
+
+    $ pipenv install tox
+    $ tox
+
+this will check the code style and run the tests.
+
+Help
+----
+
+The Hypercorn `documentation <https://hypercorn.readthedocs.io>`_ is
+the best place to start, after that try searching stack overflow, if
+you still can't find an answer please `open an issue
+<https://github.com/pgjones/hypercorn/issues>`_.
+
+
+.. |Build Status| image:: https://github.com/pgjones/hypercorn/actions/workflows/ci.yml/badge.svg
+   :target: https://github.com/pgjones/hypercorn/commits/main
+
+.. |docs| image:: https://img.shields.io/badge/docs-passing-brightgreen.svg
+   :target: https://hypercorn.readthedocs.io
+
+.. |pypi| image:: https://img.shields.io/pypi/v/hypercorn.svg
+   :target: https://pypi.python.org/pypi/Hypercorn/
+
+.. |http| image:: https://img.shields.io/badge/http-1.0,1.1,2-orange.svg
+   :target: https://en.wikipedia.org/wiki/Hypertext_Transfer_Protocol
+
+.. |python| image:: https://img.shields.io/pypi/pyversions/hypercorn.svg
+   :target: https://pypi.python.org/pypi/Hypercorn/
+
+.. |license| image:: https://img.shields.io/badge/license-MIT-blue.svg
+   :target: https://github.com/pgjones/hypercorn/blob/main/LICENSE
```

### Comparing `nonecorn-0.14.1.dev1/README.rst` & `nonecorn-0.14.3.dev1/README.rst`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,118 +1,118 @@
-Hypercorn is now hosted at `github.com/pgjones/hypercorn
-<https://github.com/pgjones/hypercorn>`_.
-
-
-Hypercorn
-=========
-
-.. image:: https://github.com/pgjones/hypercorn/raw/main/artwork/logo.png
-   :alt: Hypercorn logo
-
-|Build Status| |docs| |pypi| |http| |python| |license|
-
-Hypercorn is an `ASGI
-<https://github.com/django/asgiref/blob/main/specs/asgi.rst>`_ and
-WSGI web server based on the sans-io hyper, `h11
-<https://github.com/python-hyper/h11>`_, `h2
-<https://github.com/python-hyper/hyper-h2>`_, and `wsproto
-<https://github.com/python-hyper/wsproto>`_ libraries and inspired by
-Gunicorn. Hypercorn supports HTTP/1, HTTP/2, WebSockets (over HTTP/1
-and HTTP/2), ASGI, and WSGI specifications. Hypercorn can utilise
-asyncio, uvloop, or trio worker types.
-
-Hypercorn can optionally serve the current draft of the HTTP/3
-specification using the `aioquic
-<https://github.com/aiortc/aioquic/>`_ library. To enable this install
-the ``h3`` optional extra, ``pip install hypercorn[h3]`` and then
-choose a quic binding e.g. ``hypercorn --quic-bind localhost:4433
-...``.
-
-Hypercorn was initially part of `Quart
-<https://github.com/pgjones/quart>`_ before being separated out into a
-standalone server. Hypercorn forked from version 0.5.0 of Quart.
-
-Quickstart
-----------
-
-Hypercorn can be installed via `pip
-<https://docs.python.org/3/installing/index.html>`_,
-
-.. code-block:: console
-
-    $ pip install hypercorn
-
-and requires Python 3.7.0 or higher.
-
-With hypercorn installed ASGI frameworks (or apps) can be served via
-Hypercorn via the command line,
-
-.. code-block:: console
-
-    $ hypercorn module:app
-
-Alternatively Hypercorn can be used programatically,
-
-.. code-block:: python
-
-    import asyncio
-    from hypercorn.config import Config
-    from hypercorn.asyncio import serve
-
-    from module import app
-
-    asyncio.run(serve(app, Config()))
-
-learn more (including a Trio example of the above) in the `API usage
-<https://hypercorn.readthedocs.io/en/latest/how_to_guides/api_usage.html>`_
-docs.
-
-Contributing
-------------
-
-Hypercorn is developed on `Github
-<https://github.com/pgjones/hypercorn>`_. If you come across an issue,
-or have a feature request please open an `issue
-<https://github.com/pgjones/hypercorn/issues>`_.  If you want to
-contribute a fix or the feature-implementation please do (typo fixes
-welcome), by proposing a `pull request
-<https://github.com/pgjones/hypercorn/merge_requests>`_.
-
-Testing
-~~~~~~~
-
-The best way to test Hypercorn is with `Tox
-<https://tox.readthedocs.io>`_,
-
-.. code-block:: console
-
-    $ pipenv install tox
-    $ tox
-
-this will check the code style and run the tests.
-
-Help
-----
-
-The Hypercorn `documentation <https://hypercorn.readthedocs.io>`_ is
-the best place to start, after that try searching stack overflow, if
-you still can't find an answer please `open an issue
-<https://github.com/pgjones/hypercorn/issues>`_.
-
-
-.. |Build Status| image:: https://github.com/pgjones/hypercorn/actions/workflows/ci.yml/badge.svg
-   :target: https://github.com/pgjones/hypercorn/commits/main
-
-.. |docs| image:: https://img.shields.io/badge/docs-passing-brightgreen.svg
-   :target: https://hypercorn.readthedocs.io
-
-.. |pypi| image:: https://img.shields.io/pypi/v/hypercorn.svg
-   :target: https://pypi.python.org/pypi/Hypercorn/
-
-.. |http| image:: https://img.shields.io/badge/http-1.0,1.1,2-orange.svg
-   :target: https://en.wikipedia.org/wiki/Hypertext_Transfer_Protocol
-
-.. |python| image:: https://img.shields.io/pypi/pyversions/hypercorn.svg
-   :target: https://pypi.python.org/pypi/Hypercorn/
-
-.. |license| image:: https://img.shields.io/badge/license-MIT-blue.svg
-   :target: https://github.com/pgjones/hypercorn/blob/main/LICENSE
+Hypercorn is now hosted at `github.com/pgjones/hypercorn
+<https://github.com/pgjones/hypercorn>`_.
+
+
+Hypercorn
+=========
+
+.. image:: https://github.com/pgjones/hypercorn/raw/main/artwork/logo.png
+   :alt: Hypercorn logo
+
+|Build Status| |docs| |pypi| |http| |python| |license|
+
+Hypercorn is an `ASGI
+<https://github.com/django/asgiref/blob/main/specs/asgi.rst>`_ and
+WSGI web server based on the sans-io hyper, `h11
+<https://github.com/python-hyper/h11>`_, `h2
+<https://github.com/python-hyper/hyper-h2>`_, and `wsproto
+<https://github.com/python-hyper/wsproto>`_ libraries and inspired by
+Gunicorn. Hypercorn supports HTTP/1, HTTP/2, WebSockets (over HTTP/1
+and HTTP/2), ASGI, and WSGI specifications. Hypercorn can utilise
+asyncio, uvloop, or trio worker types.
+
+Hypercorn can optionally serve the current draft of the HTTP/3
+specification using the `aioquic
+<https://github.com/aiortc/aioquic/>`_ library. To enable this install
+the ``h3`` optional extra, ``pip install hypercorn[h3]`` and then
+choose a quic binding e.g. ``hypercorn --quic-bind localhost:4433
+...``.
+
+Hypercorn was initially part of `Quart
+<https://github.com/pgjones/quart>`_ before being separated out into a
+standalone server. Hypercorn forked from version 0.5.0 of Quart.
+
+Quickstart
+----------
+
+Hypercorn can be installed via `pip
+<https://docs.python.org/3/installing/index.html>`_,
+
+.. code-block:: console
+
+    $ pip install hypercorn
+
+and requires Python 3.7.0 or higher.
+
+With hypercorn installed ASGI frameworks (or apps) can be served via
+Hypercorn via the command line,
+
+.. code-block:: console
+
+    $ hypercorn module:app
+
+Alternatively Hypercorn can be used programatically,
+
+.. code-block:: python
+
+    import asyncio
+    from hypercorn.config import Config
+    from hypercorn.asyncio import serve
+
+    from module import app
+
+    asyncio.run(serve(app, Config()))
+
+learn more (including a Trio example of the above) in the `API usage
+<https://hypercorn.readthedocs.io/en/latest/how_to_guides/api_usage.html>`_
+docs.
+
+Contributing
+------------
+
+Hypercorn is developed on `Github
+<https://github.com/pgjones/hypercorn>`_. If you come across an issue,
+or have a feature request please open an `issue
+<https://github.com/pgjones/hypercorn/issues>`_.  If you want to
+contribute a fix or the feature-implementation please do (typo fixes
+welcome), by proposing a `pull request
+<https://github.com/pgjones/hypercorn/merge_requests>`_.
+
+Testing
+~~~~~~~
+
+The best way to test Hypercorn is with `Tox
+<https://tox.readthedocs.io>`_,
+
+.. code-block:: console
+
+    $ pipenv install tox
+    $ tox
+
+this will check the code style and run the tests.
+
+Help
+----
+
+The Hypercorn `documentation <https://hypercorn.readthedocs.io>`_ is
+the best place to start, after that try searching stack overflow, if
+you still can't find an answer please `open an issue
+<https://github.com/pgjones/hypercorn/issues>`_.
+
+
+.. |Build Status| image:: https://github.com/pgjones/hypercorn/actions/workflows/ci.yml/badge.svg
+   :target: https://github.com/pgjones/hypercorn/commits/main
+
+.. |docs| image:: https://img.shields.io/badge/docs-passing-brightgreen.svg
+   :target: https://hypercorn.readthedocs.io
+
+.. |pypi| image:: https://img.shields.io/pypi/v/hypercorn.svg
+   :target: https://pypi.python.org/pypi/Hypercorn/
+
+.. |http| image:: https://img.shields.io/badge/http-1.0,1.1,2-orange.svg
+   :target: https://en.wikipedia.org/wiki/Hypertext_Transfer_Protocol
+
+.. |python| image:: https://img.shields.io/pypi/pyversions/hypercorn.svg
+   :target: https://pypi.python.org/pypi/Hypercorn/
+
+.. |license| image:: https://img.shields.io/badge/license-MIT-blue.svg
+   :target: https://github.com/pgjones/hypercorn/blob/main/LICENSE
```

### Comparing `nonecorn-0.14.1.dev1/pyproject.toml` & `nonecorn-0.14.3.dev1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,100 +1,100 @@
-[tool.poetry]
-name = "nonecorn"
-version = "0.14.1dev1"
-description = "A ASGI Server based on Hyper libraries and inspired by Gunicorn"
-authors = ["pgjones <philip.graham.jones@googlemail.com>"]
-classifiers = [
-    "Development Status :: 4 - Beta",
-    "Environment :: Web Environment",
-    "Intended Audience :: Developers",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
-    "Topic :: Software Development :: Libraries :: Python Modules",
-]
-include = ["src/hypercorn/py.typed"]
-license = "MIT"
-readme = "README.rst"
-repository = "https://github.com/pgjones/hypercorn/"
-documentation = "https://hypercorn.readthedocs.io"
-
-[tool.poetry.dependencies]
-python = ">=3.7"
-aioquic = { version = ">= 0.9.0, < 1.0", optional = true }
-h11 = "*"
-h2 = ">=3.1.0"
-priority = "*"
-pydata_sphinx_theme = { version = "*", optional = true }
-toml = "*"
-trio = { version = ">=0.11.0", optional = true }
-typing_extensions = { version = ">=3.7.4", python = "<3.8" }
-uvloop = { version = "*", markers = "platform_system != 'Windows'", optional = true }
-wsproto = ">=0.14.0"
-
-[tool.poetry.dev-dependencies]
-hypothesis = "*"
-mock = "*"
-pytest = "*"
-pytest-asyncio = "*"
-pytest-trio = "*"
-trio = "*"
-
-[tool.poetry.scripts]
-hypercorn = "hypercorn.__main__:main"
-
-[tool.poetry.extras]
-docs = ["pydata_sphinx_theme"]
-h3 = ["aioquic"]
-trio = ["trio"]
-uvloop = ["uvloop"]
-
-[tool.black]
-line-length = 100
-target-version = ["py37"]
-
-[tool.isort]
-combine_as_imports = true
-force_grid_wrap = 0
-include_trailing_comma = true
-known_first_party = "hypercorn, tests"
-line_length = 100
-multi_line_output = 3
-no_lines_before = "LOCALFOLDER"
-order_by_type = false
-reverse_relative = true
-
-[tool.mypy]
-allow_redefinition = true
-disallow_any_generics = false
-disallow_subclassing_any = true
-disallow_untyped_calls = false
-disallow_untyped_defs = true
-implicit_reexport = true
-no_implicit_optional = true
-show_error_codes = true
-strict = true
-strict_equality = true
-strict_optional = false
-warn_redundant_casts = true
-warn_return_any = false
-warn_unused_configs = true
-warn_unused_ignores = true
-
-[[tool.mypy.overrides]]
-module =["aioquic.*", "cryptography.*", "h11.*", "h2.*", "priority.*", "pytest_asyncio.*", "trio.*", "uvloop.*"]
-ignore_missing_imports = true
-
-[tool.pytest.ini_options]
-addopts = "--no-cov-on-fail --showlocals --strict-markers"
-asyncio_mode = "strict"
-testpaths = ["tests"]
-
-[build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "nonecorn"
+version = "0.14.3dev1"
+description = "A ASGI Server based on Hyper libraries and inspired by Gunicorn"
+authors = ["pgjones <philip.graham.jones@googlemail.com>"]
+classifiers = [
+    "Development Status :: 4 - Beta",
+    "Environment :: Web Environment",
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
+    "Topic :: Software Development :: Libraries :: Python Modules",
+]
+include = ["src/hypercorn/py.typed"]
+license = "MIT"
+readme = "README.rst"
+repository = "https://github.com/pgjones/hypercorn/"
+documentation = "https://hypercorn.readthedocs.io"
+
+[tool.poetry.dependencies]
+python = ">=3.7"
+aioquic = { version = ">= 0.9.0, < 1.0", optional = true }
+h11 = "*"
+h2 = ">=3.1.0"
+priority = "*"
+pydata_sphinx_theme = { version = "*", optional = true }
+tomli = { version = "*", python = "<3.11" }
+trio = { version = ">=0.11.0", optional = true }
+typing_extensions = { version = ">=3.7.4", python = "<3.8" }
+uvloop = { version = "*", markers = "platform_system != 'Windows'", optional = true }
+wsproto = ">=0.14.0"
+
+[tool.poetry.dev-dependencies]
+hypothesis = "*"
+mock = "*"
+pytest = "*"
+pytest-asyncio = "*"
+pytest-trio = "*"
+trio = "*"
+
+[tool.poetry.scripts]
+hypercorn = "hypercorn.__main__:main"
+
+[tool.poetry.extras]
+docs = ["pydata_sphinx_theme"]
+h3 = ["aioquic"]
+trio = ["trio"]
+uvloop = ["uvloop"]
+
+[tool.black]
+line-length = 100
+target-version = ["py37"]
+
+[tool.isort]
+combine_as_imports = true
+force_grid_wrap = 0
+include_trailing_comma = true
+known_first_party = "hypercorn, tests"
+line_length = 100
+multi_line_output = 3
+no_lines_before = "LOCALFOLDER"
+order_by_type = false
+reverse_relative = true
+
+[tool.mypy]
+allow_redefinition = true
+disallow_any_generics = false
+disallow_subclassing_any = true
+disallow_untyped_calls = false
+disallow_untyped_defs = true
+implicit_reexport = true
+no_implicit_optional = true
+show_error_codes = true
+strict = true
+strict_equality = true
+strict_optional = false
+warn_redundant_casts = true
+warn_return_any = false
+warn_unused_configs = true
+warn_unused_ignores = true
+
+[[tool.mypy.overrides]]
+module =["aioquic.*", "cryptography.*", "h11.*", "h2.*", "priority.*", "pytest_asyncio.*", "trio.*", "uvloop.*"]
+ignore_missing_imports = true
+
+[tool.pytest.ini_options]
+addopts = "--no-cov-on-fail --showlocals --strict-markers"
+asyncio_mode = "strict"
+testpaths = ["tests"]
+
+[build-system]
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `nonecorn-0.14.1.dev1/src/hypercorn/asyncio/__init__.py` & `nonecorn-0.14.3.dev1/src/hypercorn/asyncio/__init__.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-from __future__ import annotations
-
-import warnings
-from typing import Awaitable, Callable, Optional
-
-from .run import worker_serve
-from ..config import Config
-from ..typing import Framework
-from ..utils import wrap_app
-
-try:
-    from typing import Literal
-except ImportError:
-    from typing_extensions import Literal  # type: ignore
-
-
-async def serve(
-    app: Framework,
-    config: Config,
-    *,
-    shutdown_trigger: Optional[Callable[..., Awaitable[None]]] = None,
-    mode: Optional[Literal["asgi", "wsgi"]] = None,
-) -> None:
-    """Serve an ASGI or WSGI framework app given the config.
-
-    This allows for a programmatic way to serve an ASGI or WSGI
-    framework, it can be used via,
-
-    .. code-block:: python
-
-        asyncio.run(serve(app, config))
-
-    It is assumed that the event-loop is configured before calling
-    this function, therefore configuration values that relate to loop
-    setup or process setup are ignored.
-
-    Arguments:
-        app: The ASGI or WSGI application to serve.
-        config: A Hypercorn configuration object.
-        shutdown_trigger: This should return to trigger a graceful
-            shutdown.
-        mode: Specify if the app is WSGI or ASGI.
-    """
-    if config.debug:
-        warnings.warn("The config `debug` has no affect when using serve", Warning)
-    if config.workers != 1:
-        warnings.warn("The config `workers` has no affect when using serve", Warning)
-
-    await worker_serve(
-        wrap_app(app, config.wsgi_max_body_size, mode), config, shutdown_trigger=shutdown_trigger
-    )
+from __future__ import annotations
+
+import warnings
+from typing import Awaitable, Callable, Optional
+
+from .run import worker_serve
+from ..config import Config
+from ..typing import Framework
+from ..utils import wrap_app
+
+try:
+    from typing import Literal
+except ImportError:
+    from typing_extensions import Literal  # type: ignore
+
+
+async def serve(
+    app: Framework,
+    config: Config,
+    *,
+    shutdown_trigger: Optional[Callable[..., Awaitable[None]]] = None,
+    mode: Optional[Literal["asgi", "wsgi"]] = None,
+) -> None:
+    """Serve an ASGI or WSGI framework app given the config.
+
+    This allows for a programmatic way to serve an ASGI or WSGI
+    framework, it can be used via,
+
+    .. code-block:: python
+
+        asyncio.run(serve(app, config))
+
+    It is assumed that the event-loop is configured before calling
+    this function, therefore configuration values that relate to loop
+    setup or process setup are ignored.
+
+    Arguments:
+        app: The ASGI or WSGI application to serve.
+        config: A Hypercorn configuration object.
+        shutdown_trigger: This should return to trigger a graceful
+            shutdown.
+        mode: Specify if the app is WSGI or ASGI.
+    """
+    if config.debug:
+        warnings.warn("The config `debug` has no affect when using serve", Warning)
+    if config.workers != 1:
+        warnings.warn("The config `workers` has no affect when using serve", Warning)
+
+    await worker_serve(
+        wrap_app(app, config.wsgi_max_body_size, mode), config, shutdown_trigger=shutdown_trigger
+    )
```

### Comparing `nonecorn-0.14.1.dev1/src/hypercorn/asyncio/lifespan.py` & `nonecorn-0.14.3.dev1/src/hypercorn/asyncio/lifespan.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,96 +1,108 @@
-from __future__ import annotations
-
-import asyncio
-from functools import partial
-
-from ..config import Config
-from ..typing import AppWrapper, ASGIReceiveEvent, ASGISendEvent, LifespanScope
-from ..utils import LifespanFailureError, LifespanTimeoutError
-
-
-class UnexpectedMessageError(Exception):
-    pass
-
-
-class Lifespan:
-    def __init__(self, app: AppWrapper, config: Config, loop: asyncio.AbstractEventLoop) -> None:
-        self.app = app
-        self.config = config
-        self.startup = asyncio.Event()
-        self.shutdown = asyncio.Event()
-        self.app_queue: asyncio.Queue = asyncio.Queue(config.max_app_queue_size)
-        self.supported = True
-        self.loop = loop
-
-        # This mimics the Trio nursery.start task_status and is
-        # required to ensure the support has been checked before
-        # waiting on timeouts.
-        self._started = asyncio.Event()
-
-    async def handle_lifespan(self) -> None:
-        self._started.set()
-        scope: LifespanScope = {
-            "type": "lifespan",
-            "asgi": {"spec_version": "2.0", "version": "3.0"},
-        }
-        try:
-            await self.app(
-                scope, self.asgi_receive, self.asgi_send, partial(self.loop.run_in_executor, None)
-            )
-        except LifespanFailureError:
-            # Lifespan failures should crash the server
-            raise
-        except Exception:
-            self.supported = False
-            if not self.startup.is_set():
-                await self.config.log.warning(
-                    "ASGI Framework Lifespan error, continuing without Lifespan support"
-                )
-            elif not self.shutdown.is_set():
-                await self.config.log.exception(
-                    "ASGI Framework Lifespan error, shutdown without Lifespan support"
-                )
-            else:
-                await self.config.log.exception("ASGI Framework Lifespan errored after shutdown.")
-        finally:
-            self.startup.set()
-            self.shutdown.set()
-
-    async def wait_for_startup(self) -> None:
-        await self._started.wait()
-        if not self.supported:
-            return
-
-        await self.app_queue.put({"type": "lifespan.startup"})
-        try:
-            await asyncio.wait_for(self.startup.wait(), timeout=self.config.startup_timeout)
-        except asyncio.TimeoutError as error:
-            raise LifespanTimeoutError("startup") from error
-
-    async def wait_for_shutdown(self) -> None:
-        await self._started.wait()
-        if not self.supported:
-            return
-
-        await self.app_queue.put({"type": "lifespan.shutdown"})
-        try:
-            await asyncio.wait_for(self.shutdown.wait(), timeout=self.config.shutdown_timeout)
-        except asyncio.TimeoutError as error:
-            raise LifespanTimeoutError("shutdown") from error
-
-    async def asgi_receive(self) -> ASGIReceiveEvent:
-        return await self.app_queue.get()
-
-    async def asgi_send(self, message: ASGISendEvent) -> None:
-        if message["type"] == "lifespan.startup.complete":
-            self.startup.set()
-        elif message["type"] == "lifespan.shutdown.complete":
-            self.shutdown.set()
-        elif message["type"] == "lifespan.startup.failed":
-            self.startup.set()
-            raise LifespanFailureError("startup", message["message"])
-        elif message["type"] == "lifespan.shutdown.failed":
-            self.shutdown.set()
-            raise LifespanFailureError("shutdown", message["message"])
-        else:
-            raise UnexpectedMessageError(message["type"])
+from __future__ import annotations
+
+import asyncio
+from functools import partial
+from typing import Any, Callable, Dict
+
+from ..config import Config
+from ..typing import AppWrapper, ASGIReceiveEvent, ASGISendEvent, LifespanScope
+from ..utils import LifespanFailureError, LifespanTimeoutError
+
+
+class UnexpectedMessageError(Exception):
+    pass
+
+
+class Lifespan:
+    def __init__(self, app: AppWrapper, config: Config, loop: asyncio.AbstractEventLoop) -> None:
+        self.app = app
+        self.config = config
+        self.startup = asyncio.Event()
+        self.shutdown = asyncio.Event()
+        self.app_queue: asyncio.Queue = asyncio.Queue(config.max_app_queue_size)
+        self.supported = True
+        self.loop = loop
+
+        # This mimics the Trio nursery.start task_status and is
+        # required to ensure the support has been checked before
+        # waiting on timeouts.
+        self._started = asyncio.Event()
+        self.state: Dict[str, Any] = {}
+
+    async def handle_lifespan(self) -> None:
+        self._started.set()
+        scope: LifespanScope = {
+            "type": "lifespan",
+            "asgi": {"spec_version": "2.0", "version": "3.0"},
+            "state": self.state,
+        }
+
+        def _call_soon(func: Callable, *args: Any) -> Any:
+            future = asyncio.run_coroutine_threadsafe(func(*args), self.loop)
+            return future.result()
+
+        try:
+            await self.app(
+                scope,
+                self.asgi_receive,
+                self.asgi_send,
+                partial(self.loop.run_in_executor, None),
+                _call_soon,
+            )
+        except LifespanFailureError:
+            # Lifespan failures should crash the server
+            raise
+        except Exception:
+            self.supported = False
+            if not self.startup.is_set():
+                await self.config.log.warning(
+                    "ASGI Framework Lifespan error, continuing without Lifespan support"
+                )
+            elif not self.shutdown.is_set():
+                await self.config.log.exception(
+                    "ASGI Framework Lifespan error, shutdown without Lifespan support"
+                )
+            else:
+                await self.config.log.exception("ASGI Framework Lifespan errored after shutdown.")
+        finally:
+            self.startup.set()
+            self.shutdown.set()
+
+    async def wait_for_startup(self) -> None:
+        await self._started.wait()
+        if not self.supported:
+            return
+
+        await self.app_queue.put({"type": "lifespan.startup"})
+        try:
+            await asyncio.wait_for(self.startup.wait(), timeout=self.config.startup_timeout)
+        except asyncio.TimeoutError as error:
+            raise LifespanTimeoutError("startup") from error
+
+    async def wait_for_shutdown(self) -> None:
+        await self._started.wait()
+        if not self.supported:
+            return
+
+        await self.app_queue.put({"type": "lifespan.shutdown"})
+        try:
+            await asyncio.wait_for(self.shutdown.wait(), timeout=self.config.shutdown_timeout)
+        except asyncio.TimeoutError as error:
+            raise LifespanTimeoutError("shutdown") from error
+
+    async def asgi_receive(self) -> ASGIReceiveEvent:
+        return await self.app_queue.get()
+
+    async def asgi_send(self, message: ASGISendEvent) -> None:
+        if message["type"] == "lifespan.startup.complete":
+            self.startup.set()
+        elif message["type"] == "lifespan.shutdown.complete":
+            self.shutdown.set()
+        elif message["type"] == "lifespan.startup.failed":
+            self.startup.set()
+            raise LifespanFailureError("startup", message.get("message", ""))
+        elif message["type"] == "lifespan.shutdown.failed":
+            self.shutdown.set()
+            raise LifespanFailureError("shutdown", message.get("message", ""))
+        else:
+            raise UnexpectedMessageError(message["type"])
```

### Comparing `nonecorn-0.14.1.dev1/src/hypercorn/asyncio/run.py` & `nonecorn-0.14.3.dev1/src/hypercorn/asyncio/run.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,273 +1,273 @@
-from __future__ import annotations
-
-import asyncio
-import platform
-import signal
-import ssl
-from functools import partial
-from multiprocessing.synchronize import Event as EventType
-from os import getpid
-from socket import socket
-from typing import Any, Awaitable, Callable, Optional
-from weakref import WeakSet
-
-from .lifespan import Lifespan
-from .statsd import StatsdLogger
-from .tcp_server import TCPServer
-from .udp_server import UDPServer
-from .worker_context import WorkerContext
-from ..config import Config, Sockets
-from ..typing import AppWrapper
-from ..utils import (
-    check_multiprocess_shutdown_event,
-    load_application,
-    raise_shutdown,
-    repr_socket_addr,
-    ShutdownError,
-)
-
-
-async def _windows_signal_support() -> None:
-    # See https://bugs.python.org/issue23057, to catch signals on
-    # Windows it is necessary for an IO event to happen periodically.
-    # Fixed by Python 3.8
-    while True:
-        await asyncio.sleep(1)
-
-
-def _share_socket(sock: socket) -> socket:
-    # Windows requires the socket be explicitly shared across
-    # multiple workers (processes).
-    from socket import fromshare  # type: ignore
-
-    sock_data = sock.share(getpid())  # type: ignore
-    return fromshare(sock_data)
-
-
-async def worker_serve(
-    app: AppWrapper,
-    config: Config,
-    *,
-    sockets: Optional[Sockets] = None,
-    shutdown_trigger: Optional[Callable[..., Awaitable[None]]] = None,
-) -> None:
-    config.set_statsd_logger_class(StatsdLogger)
-
-    loop = asyncio.get_event_loop()
-
-    if shutdown_trigger is None:
-        signal_event = asyncio.Event()
-
-        def _signal_handler(*_: Any) -> None:  # noqa: N803
-            signal_event.set()
-
-        for signal_name in {"SIGINT", "SIGTERM", "SIGBREAK"}:
-            if hasattr(signal, signal_name):
-                try:
-                    loop.add_signal_handler(getattr(signal, signal_name), _signal_handler)
-                except NotImplementedError:
-                    # Add signal handler may not be implemented on Windows
-                    signal.signal(getattr(signal, signal_name), _signal_handler)
-
-        shutdown_trigger = signal_event.wait  # type: ignore
-
-    lifespan = Lifespan(app, config, loop)
-
-    lifespan_task = loop.create_task(lifespan.handle_lifespan())
-    await lifespan.wait_for_startup()
-    if lifespan_task.done():
-        exception = lifespan_task.exception()
-        if exception is not None:
-            raise exception
-
-    if sockets is None:
-        sockets = config.create_sockets()
-
-    ssl_handshake_timeout = None
-    if config.ssl_enabled:
-        ssl_context = config.create_ssl_context()
-        ssl_handshake_timeout = config.ssl_handshake_timeout
-
-    context = WorkerContext()
-    server_tasks: WeakSet = WeakSet()
-
-    async def _server_callback(reader: asyncio.StreamReader, writer: asyncio.StreamWriter) -> None:
-        server_tasks.add(asyncio.current_task(loop))
-        await TCPServer(app, loop, config, context, reader, writer)
-
-    servers = []
-    for sock in sockets.secure_sockets:
-        if config.workers > 1 and platform.system() == "Windows":
-            sock = _share_socket(sock)
-
-        servers.append(
-            await asyncio.start_server(
-                _server_callback,
-                backlog=config.backlog,
-                ssl=ssl_context,
-                sock=sock,
-                ssl_handshake_timeout=ssl_handshake_timeout,
-            )
-        )
-        bind = repr_socket_addr(sock.family, sock.getsockname())
-        await config.log.info(f"Running on https://{bind} (CTRL + C to quit)")
-
-    for sock in sockets.insecure_sockets:
-        if config.workers > 1 and platform.system() == "Windows":
-            sock = _share_socket(sock)
-
-        servers.append(
-            await asyncio.start_server(_server_callback, backlog=config.backlog, sock=sock)
-        )
-        bind = repr_socket_addr(sock.family, sock.getsockname())
-        await config.log.info(f"Running on http://{bind} (CTRL + C to quit)")
-
-    for sock in sockets.quic_sockets:
-        if config.workers > 1 and platform.system() == "Windows":
-            sock = _share_socket(sock)
-
-        _, protocol = await loop.create_datagram_endpoint(
-            lambda: UDPServer(app, loop, config, context), sock=sock
-        )
-        server_tasks.add(loop.create_task(protocol.run()))
-        bind = repr_socket_addr(sock.family, sock.getsockname())
-        await config.log.info(f"Running on https://{bind} (QUIC) (CTRL + C to quit)")
-
-    tasks = []
-    if platform.system() == "Windows":
-        tasks.append(loop.create_task(_windows_signal_support()))
-
-    tasks.append(loop.create_task(raise_shutdown(shutdown_trigger)))
-
-    try:
-        if len(tasks):
-            gathered_tasks = asyncio.gather(*tasks)
-            await gathered_tasks
-        else:
-            loop.run_forever()
-    except (ShutdownError, KeyboardInterrupt):
-        pass
-    finally:
-        await context.terminated.set()
-
-        for server in servers:
-            server.close()
-            await server.wait_closed()
-
-        # Retrieve the Gathered Tasks Cancelled Exception, to
-        # prevent a warning that this hasn't been done.
-        gathered_tasks.exception()
-
-        try:
-            gathered_server_tasks = asyncio.gather(*server_tasks)
-            await asyncio.wait_for(gathered_server_tasks, config.graceful_timeout)
-        except asyncio.TimeoutError:
-            pass
-        finally:
-            # Retrieve the Gathered Tasks Cancelled Exception, to
-            # prevent a warning that this hasn't been done.
-            gathered_server_tasks.exception()
-
-            await lifespan.wait_for_shutdown()
-            lifespan_task.cancel()
-            await lifespan_task
-
-
-def asyncio_worker(
-    config: Config, sockets: Optional[Sockets] = None, shutdown_event: Optional[EventType] = None
-) -> None:
-    app = load_application(config.application_path, config.wsgi_max_body_size)
-
-    shutdown_trigger = None
-    if shutdown_event is not None:
-        shutdown_trigger = partial(check_multiprocess_shutdown_event, shutdown_event, asyncio.sleep)
-
-    if config.workers > 1 and platform.system() == "Windows":
-        asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())  # type: ignore
-
-    _run(
-        partial(worker_serve, app, config, sockets=sockets),
-        debug=config.debug,
-        shutdown_trigger=shutdown_trigger,
-    )
-
-
-def uvloop_worker(
-    config: Config, sockets: Optional[Sockets] = None, shutdown_event: Optional[EventType] = None
-) -> None:
-    try:
-        import uvloop
-    except ImportError as error:
-        raise Exception("uvloop is not installed") from error
-    else:
-        asyncio.set_event_loop_policy(uvloop.EventLoopPolicy())
-
-    app = load_application(config.application_path, config.wsgi_max_body_size)
-
-    shutdown_trigger = None
-    if shutdown_event is not None:
-        shutdown_trigger = partial(check_multiprocess_shutdown_event, shutdown_event, asyncio.sleep)
-
-    _run(
-        partial(worker_serve, app, config, sockets=sockets),
-        debug=config.debug,
-        shutdown_trigger=shutdown_trigger,
-    )
-
-
-def _run(
-    main: Callable,
-    *,
-    debug: bool = False,
-    shutdown_trigger: Optional[Callable[..., Awaitable[None]]] = None,
-) -> None:
-    loop = asyncio.new_event_loop()
-    asyncio.set_event_loop(loop)
-    loop.set_debug(debug)
-    loop.set_exception_handler(_exception_handler)
-
-    try:
-        loop.run_until_complete(main(shutdown_trigger=shutdown_trigger))
-    except KeyboardInterrupt:
-        pass
-    finally:
-        try:
-            _cancel_all_tasks(loop)
-            loop.run_until_complete(loop.shutdown_asyncgens())
-
-            try:
-                loop.run_until_complete(loop.shutdown_default_executor())
-            except AttributeError:
-                pass  # shutdown_default_executor is new to Python 3.9
-
-        finally:
-            asyncio.set_event_loop(None)
-            loop.close()
-
-
-def _cancel_all_tasks(loop: asyncio.AbstractEventLoop) -> None:
-    tasks = [task for task in asyncio.all_tasks(loop) if not task.done()]
-    if not tasks:
-        return
-
-    for task in tasks:
-        task.cancel()
-    loop.run_until_complete(asyncio.gather(*tasks, return_exceptions=True))
-
-    for task in tasks:
-        if not task.cancelled() and task.exception() is not None:
-            loop.call_exception_handler(
-                {
-                    "message": "unhandled exception during shutdown",
-                    "exception": task.exception(),
-                    "task": task,
-                }
-            )
-
-
-def _exception_handler(loop: asyncio.AbstractEventLoop, context: dict) -> None:
-    exception = context.get("exception")
-    if isinstance(exception, ssl.SSLError):
-        pass  # Handshake failure
-    else:
-        loop.default_exception_handler(context)
+from __future__ import annotations
+
+import asyncio
+import platform
+import signal
+import ssl
+from functools import partial
+from multiprocessing.synchronize import Event as EventType
+from os import getpid
+from socket import socket
+from typing import Any, Awaitable, Callable, Optional
+from weakref import WeakSet
+
+from .lifespan import Lifespan
+from .statsd import StatsdLogger
+from .tcp_server import TCPServer
+from .udp_server import UDPServer
+from .worker_context import WorkerContext
+from ..config import Config, Sockets
+from ..typing import AppWrapper
+from ..utils import (
+    check_multiprocess_shutdown_event,
+    load_application,
+    raise_shutdown,
+    repr_socket_addr,
+    ShutdownError,
+)
+
+
+async def _windows_signal_support() -> None:
+    # See https://bugs.python.org/issue23057, to catch signals on
+    # Windows it is necessary for an IO event to happen periodically.
+    # Fixed by Python 3.8
+    while True:
+        await asyncio.sleep(1)
+
+
+def _share_socket(sock: socket) -> socket:
+    # Windows requires the socket be explicitly shared across
+    # multiple workers (processes).
+    from socket import fromshare  # type: ignore
+
+    sock_data = sock.share(getpid())  # type: ignore
+    return fromshare(sock_data)
+
+
+async def worker_serve(
+    app: AppWrapper,
+    config: Config,
+    *,
+    sockets: Optional[Sockets] = None,
+    shutdown_trigger: Optional[Callable[..., Awaitable[None]]] = None,
+) -> None:
+    config.set_statsd_logger_class(StatsdLogger)
+
+    loop = asyncio.get_event_loop()
+
+    if shutdown_trigger is None:
+        signal_event = asyncio.Event()
+
+        def _signal_handler(*_: Any) -> None:  # noqa: N803
+            signal_event.set()
+
+        for signal_name in {"SIGINT", "SIGTERM", "SIGBREAK"}:
+            if hasattr(signal, signal_name):
+                try:
+                    loop.add_signal_handler(getattr(signal, signal_name), _signal_handler)
+                except NotImplementedError:
+                    # Add signal handler may not be implemented on Windows
+                    signal.signal(getattr(signal, signal_name), _signal_handler)
+
+        shutdown_trigger = signal_event.wait  # type: ignore
+
+    lifespan = Lifespan(app, config, loop)
+
+    lifespan_task = loop.create_task(lifespan.handle_lifespan())
+    await lifespan.wait_for_startup()
+    if lifespan_task.done():
+        exception = lifespan_task.exception()
+        if exception is not None:
+            raise exception
+
+    if sockets is None:
+        sockets = config.create_sockets()
+
+    ssl_handshake_timeout = None
+    if config.ssl_enabled:
+        ssl_context = config.create_ssl_context()
+        ssl_handshake_timeout = config.ssl_handshake_timeout
+
+    context = WorkerContext()
+    server_tasks: WeakSet = WeakSet()
+
+    async def _server_callback(reader: asyncio.StreamReader, writer: asyncio.StreamWriter) -> None:
+        server_tasks.add(asyncio.current_task(loop))
+        await TCPServer(app, loop, config, context, reader, writer, lifespan.state.copy())
+
+    servers = []
+    for sock in sockets.secure_sockets:
+        if config.workers > 1 and platform.system() == "Windows":
+            sock = _share_socket(sock)
+
+        servers.append(
+            await asyncio.start_server(
+                _server_callback,
+                backlog=config.backlog,
+                ssl=ssl_context,
+                sock=sock,
+                ssl_handshake_timeout=ssl_handshake_timeout,
+            )
+        )
+        bind = repr_socket_addr(sock.family, sock.getsockname())
+        await config.log.info(f"Running on https://{bind} (CTRL + C to quit)")
+
+    for sock in sockets.insecure_sockets:
+        if config.workers > 1 and platform.system() == "Windows":
+            sock = _share_socket(sock)
+
+        servers.append(
+            await asyncio.start_server(_server_callback, backlog=config.backlog, sock=sock)
+        )
+        bind = repr_socket_addr(sock.family, sock.getsockname())
+        await config.log.info(f"Running on http://{bind} (CTRL + C to quit)")
+
+    for sock in sockets.quic_sockets:
+        if config.workers > 1 and platform.system() == "Windows":
+            sock = _share_socket(sock)
+
+        _, protocol = await loop.create_datagram_endpoint(
+            lambda: UDPServer(app, loop, config, context, lifespan.state.copy()), sock=sock
+        )
+        server_tasks.add(loop.create_task(protocol.run()))
+        bind = repr_socket_addr(sock.family, sock.getsockname())
+        await config.log.info(f"Running on https://{bind} (QUIC) (CTRL + C to quit)")
+
+    tasks = []
+    if platform.system() == "Windows":
+        tasks.append(loop.create_task(_windows_signal_support()))
+
+    tasks.append(loop.create_task(raise_shutdown(shutdown_trigger)))
+
+    try:
+        if len(tasks):
+            gathered_tasks = asyncio.gather(*tasks)
+            await gathered_tasks
+        else:
+            loop.run_forever()
+    except (ShutdownError, KeyboardInterrupt):
+        pass
+    finally:
+        await context.terminated.set()
+
+        for server in servers:
+            server.close()
+            await server.wait_closed()
+
+        # Retrieve the Gathered Tasks Cancelled Exception, to
+        # prevent a warning that this hasn't been done.
+        gathered_tasks.exception()
+
+        try:
+            gathered_server_tasks = asyncio.gather(*server_tasks)
+            await asyncio.wait_for(gathered_server_tasks, config.graceful_timeout)
+        except asyncio.TimeoutError:
+            pass
+        finally:
+            # Retrieve the Gathered Tasks Cancelled Exception, to
+            # prevent a warning that this hasn't been done.
+            gathered_server_tasks.exception()
+
+            await lifespan.wait_for_shutdown()
+            lifespan_task.cancel()
+            await lifespan_task
+
+
+def asyncio_worker(
+    config: Config, sockets: Optional[Sockets] = None, shutdown_event: Optional[EventType] = None
+) -> None:
+    app = load_application(config.application_path, config.wsgi_max_body_size)
+
+    shutdown_trigger = None
+    if shutdown_event is not None:
+        shutdown_trigger = partial(check_multiprocess_shutdown_event, shutdown_event, asyncio.sleep)
+
+    if config.workers > 1 and platform.system() == "Windows":
+        asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())  # type: ignore
+
+    _run(
+        partial(worker_serve, app, config, sockets=sockets),
+        debug=config.debug,
+        shutdown_trigger=shutdown_trigger,
+    )
+
+
+def uvloop_worker(
+    config: Config, sockets: Optional[Sockets] = None, shutdown_event: Optional[EventType] = None
+) -> None:
+    try:
+        import uvloop
+    except ImportError as error:
+        raise Exception("uvloop is not installed") from error
+    else:
+        asyncio.set_event_loop_policy(uvloop.EventLoopPolicy())
+
+    app = load_application(config.application_path, config.wsgi_max_body_size)
+
+    shutdown_trigger = None
+    if shutdown_event is not None:
+        shutdown_trigger = partial(check_multiprocess_shutdown_event, shutdown_event, asyncio.sleep)
+
+    _run(
+        partial(worker_serve, app, config, sockets=sockets),
+        debug=config.debug,
+        shutdown_trigger=shutdown_trigger,
+    )
+
+
+def _run(
+    main: Callable,
+    *,
+    debug: bool = False,
+    shutdown_trigger: Optional[Callable[..., Awaitable[None]]] = None,
+) -> None:
+    loop = asyncio.new_event_loop()
+    asyncio.set_event_loop(loop)
+    loop.set_debug(debug)
+    loop.set_exception_handler(_exception_handler)
+
+    try:
+        loop.run_until_complete(main(shutdown_trigger=shutdown_trigger))
+    except KeyboardInterrupt:
+        pass
+    finally:
+        try:
+            _cancel_all_tasks(loop)
+            loop.run_until_complete(loop.shutdown_asyncgens())
+
+            try:
+                loop.run_until_complete(loop.shutdown_default_executor())
+            except AttributeError:
+                pass  # shutdown_default_executor is new to Python 3.9
+
+        finally:
+            asyncio.set_event_loop(None)
+            loop.close()
+
+
+def _cancel_all_tasks(loop: asyncio.AbstractEventLoop) -> None:
+    tasks = [task for task in asyncio.all_tasks(loop) if not task.done()]
+    if not tasks:
+        return
+
+    for task in tasks:
+        task.cancel()
+    loop.run_until_complete(asyncio.gather(*tasks, return_exceptions=True))
+
+    for task in tasks:
+        if not task.cancelled() and task.exception() is not None:
+            loop.call_exception_handler(
+                {
+                    "message": "unhandled exception during shutdown",
+                    "exception": task.exception(),
+                    "task": task,
+                }
+            )
+
+
+def _exception_handler(loop: asyncio.AbstractEventLoop, context: dict) -> None:
+    exception = context.get("exception")
+    if isinstance(exception, ssl.SSLError):
+        pass  # Handshake failure
+    else:
+        loop.default_exception_handler(context)
```

### Comparing `nonecorn-0.14.1.dev1/src/hypercorn/asyncio/tcp_server.py` & `nonecorn-0.14.3.dev1/src/hypercorn/trio/tcp_server.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,177 +1,149 @@
-from __future__ import annotations
-
-import asyncio
-import os
-from ssl import SSLError
-from typing import Any, Generator, IO, Optional
-
-from .task_group import TaskGroup
-from .worker_context import WorkerContext
-from ..config import Config
-from ..events import Closed, Event, RawData, Updated, ZeroCopySend
-from ..protocol import ProtocolWrapper
-from ..typing import AppWrapper
-from ..utils import can_sendfile, get_tls_info, is_ssl, parse_socket_addr
-
-MAX_RECV = 2**16
-
-
-class TCPServer:
-    def __init__(
-        self,
-        app: AppWrapper,
-        loop: asyncio.AbstractEventLoop,
-        config: Config,
-        context: WorkerContext,
-        reader: asyncio.StreamReader,
-        writer: asyncio.StreamWriter,
-    ) -> None:
-        self.app = app
-        self.config = config
-        self.context = context
-        self.loop = loop
-        self.protocol: ProtocolWrapper
-        self.reader = reader
-        self.writer = writer
-        # Set the buffer to 0 to avoid the problem of sending file before headers.
-        if can_sendfile(loop, is_ssl(writer.transport)):
-            self.writer.transport.set_write_buffer_limits(0)
-        self.send_lock = asyncio.Lock()
-        self.idle_lock = asyncio.Lock()
-
-        self._idle_handle: Optional[asyncio.Task] = None
-
-    def __await__(self) -> Generator[Any, None, None]:
-        return self.run().__await__()
-
-    async def run(self) -> None:
-        socket = self.writer.get_extra_info("socket")
-        tls = None
-
-        try:
-            client = parse_socket_addr(socket.family, socket.getpeername())
-            server = parse_socket_addr(socket.family, socket.getsockname())
-            ssl_object = self.writer.get_extra_info("ssl_object")
-            if ssl_object is not None:
-                ssl = True
-                alpn_protocol = ssl_object.selected_alpn_protocol()
-                tls = get_tls_info(self.writer)
-                if tls:
-                    tls["server_cert"] = self.config.cert_pem
-            else:
-                ssl = False
-                alpn_protocol = "http/1.1"
-
-            async with TaskGroup(self.loop) as task_group:
-                self.protocol = ProtocolWrapper(
-                    self.app,
-                    self.config,
-                    self.context,
-                    task_group,
-                    ssl,
-                    client,
-                    server,
-                    self.protocol_send,
-                    alpn_protocol,
-                    tls,
-                )
-                await self.protocol.initiate()
-                await self._start_idle()
-                await self._read_data()
-        except OSError:
-            pass
-        finally:
-            await self._close()
-
-    async def protocol_send(self, event: Event) -> None:
-        if isinstance(event, RawData):
-            async with self.send_lock:
-                try:
-                    self.writer.write(event.data)
-                    await self.writer.drain()
-                except (ConnectionError, RuntimeError):
-                    await self.protocol.handle(Closed())
-        elif isinstance(event, ZeroCopySend):
-            await self.writer.drain()
-            await self.zerocopysend(event.file, event.offset, event.count)
-        elif isinstance(event, Closed):
-            await self._close()
-            await self.protocol.handle(Closed())
-        elif isinstance(event, Updated):
-            if event.idle:
-                await self._start_idle()
-            else:
-                await self._stop_idle()
-
-    async def zerocopysend(
-        self, file: IO[bytes], offset: Optional[int] = None, count: Optional[int] = None
-    ) -> None:
-        if offset is None:
-            offset = os.lseek(file.fileno(), 0, os.SEEK_CUR)
-        if count is None:
-            count = os.stat(file.fileno()).st_size - offset
-        try:
-            await self.loop.sendfile(self.writer.transport, file, offset, count)
-        except (NotImplementedError, AttributeError):  # for uvloop
-            os.sendfile(
-                self.writer.transport.get_extra_info("socket").fileno(),
-                file.fileno(),
-                offset,
-                count,
-            )
-
-    async def _read_data(self) -> None:
-        while not self.reader.at_eof():
-            try:
-                data = await asyncio.wait_for(self.reader.read(MAX_RECV), self.config.read_timeout)
-            except (
-                ConnectionError,
-                OSError,
-                asyncio.TimeoutError,
-                TimeoutError,
-                SSLError,
-            ):
-                await self.protocol.handle(Closed())
-                break
-            else:
-                await self.protocol.handle(RawData(data))
-
-    async def _close(self) -> None:
-        try:
-            self.writer.write_eof()
-        except (NotImplementedError, OSError, RuntimeError):
-            pass  # Likely SSL connection
-
-        try:
-            self.writer.close()
-            await self.writer.wait_closed()
-        except (BrokenPipeError, ConnectionResetError, RuntimeError):
-            pass  # Already closed
-
-        await self._stop_idle()
-
-    async def _initiate_server_close(self) -> None:
-        await self.protocol.handle(Closed())
-        self.writer.close()
-
-    async def _start_idle(self) -> None:
-        async with self.idle_lock:
-            if self._idle_handle is None:
-                self._idle_handle = self.loop.create_task(self._run_idle())
-
-    async def _stop_idle(self) -> None:
-        async with self.idle_lock:
-            if self._idle_handle is not None:
-                self._idle_handle.cancel()
-                try:
-                    await self._idle_handle
-                except asyncio.CancelledError:
-                    pass
-            self._idle_handle = None
-
-    async def _run_idle(self) -> None:
-        try:
-            await asyncio.wait_for(self.context.terminated.wait(), self.config.keep_alive_timeout)
-        except asyncio.TimeoutError:
-            pass
-        await asyncio.shield(self._initiate_server_close())
+from __future__ import annotations
+
+from math import inf
+from typing import Any, Generator, Optional, Dict
+
+import trio
+
+from .task_group import TaskGroup
+from .worker_context import WorkerContext
+from ..config import Config
+from ..events import Closed, Event, RawData, Updated
+from ..protocol import ProtocolWrapper
+from ..typing import AppWrapper
+from ..utils import parse_socket_addr
+
+MAX_RECV = 2**16
+
+
+class TCPServer:
+    def __init__(
+        self, app: AppWrapper, config: Config, context: WorkerContext, stream: trio.abc.Stream, app_state: Dict[str, Any]
+    ) -> None:
+        self.app = app
+        self.config = config
+        self.context = context
+        self.protocol: ProtocolWrapper
+        self.send_lock = trio.Lock()
+        self.idle_lock = trio.Lock()
+        self.stream = stream
+
+        self._idle_handle: Optional[trio.CancelScope] = None
+        self.app_state = app_state
+
+    def __await__(self) -> Generator[Any, None, None]:
+        return self.run().__await__()
+
+    async def run(self) -> None:
+        try:
+            try:
+                with trio.fail_after(self.config.ssl_handshake_timeout):
+                    await self.stream.do_handshake()
+            except (trio.BrokenResourceError, trio.TooSlowError):
+                return  # Handshake failed
+            alpn_protocol = self.stream.selected_alpn_protocol()
+            socket = self.stream.transport_stream.socket
+            ssl = True
+        except AttributeError:  # Not SSL
+            alpn_protocol = "http/1.1"
+            socket = self.stream.socket
+            ssl = False
+
+        try:
+            client = parse_socket_addr(socket.family, socket.getpeername())
+            server = parse_socket_addr(socket.family, socket.getsockname())
+
+            async with TaskGroup() as task_group:
+                self._task_group = task_group
+                self.protocol = ProtocolWrapper(
+                    self.app,
+                    self.config,
+                    self.context,
+                    task_group,
+                    ssl,
+                    client,
+                    server,
+                    self.protocol_send,
+                    alpn_protocol,
+                    self.app_state
+                )
+                await self.protocol.initiate()
+                await self._start_idle()
+                await self._read_data()
+        except (trio.MultiError, OSError):
+            pass
+        finally:
+            await self._close()
+
+    async def protocol_send(self, event: Event) -> None:
+        if isinstance(event, RawData):
+            async with self.send_lock:
+                try:
+                    with trio.CancelScope() as cancel_scope:
+                        cancel_scope.shield = True
+                        await self.stream.send_all(event.data)
+                except (trio.BrokenResourceError, trio.ClosedResourceError):
+                    await self.protocol.handle(Closed())
+        elif isinstance(event, Closed):
+            await self._close()
+            await self.protocol.handle(Closed())
+        elif isinstance(event, Updated):
+            if event.idle:
+                await self._start_idle()
+            else:
+                await self._stop_idle()
+
+    async def _read_data(self) -> None:
+        while True:
+            try:
+                with trio.fail_after(self.config.read_timeout or inf):
+                    data = await self.stream.receive_some(MAX_RECV)
+            except (trio.ClosedResourceError, trio.BrokenResourceError):
+                await self.protocol.handle(Closed())
+                break
+            else:
+                await self.protocol.handle(RawData(data))
+                if data == b"":
+                    break
+
+    async def _close(self) -> None:
+        try:
+            await self.stream.send_eof()
+        except (
+            trio.BrokenResourceError,
+            AttributeError,
+            trio.BusyResourceError,
+            trio.ClosedResourceError,
+        ):
+            # They're already gone, nothing to do
+            # Or it is a SSL stream
+            pass
+        await self.stream.aclose()
+
+    async def _initiate_server_close(self) -> None:
+        await self.protocol.handle(Closed())
+        await self.stream.aclose()
+
+    async def _start_idle(self) -> None:
+        async with self.idle_lock:
+            if self._idle_handle is None:
+                self._idle_handle = await self._task_group._nursery.start(self._run_idle)
+
+    async def _stop_idle(self) -> None:
+        async with self.idle_lock:
+            if self._idle_handle is not None:
+                self._idle_handle.cancel()
+            self._idle_handle = None
+
+    async def _run_idle(
+        self,
+        task_status: trio._core._run._TaskStatus = trio.TASK_STATUS_IGNORED,
+    ) -> None:
+        cancel_scope = trio.CancelScope()
+        task_status.started(cancel_scope)
+        with cancel_scope:
+            with trio.move_on_after(self.config.keep_alive_timeout):
+                await self.context.terminated.wait()
+
+            cancel_scope.shield = True
+            await self._initiate_server_close()
```

### Comparing `nonecorn-0.14.1.dev1/src/hypercorn/asyncio/udp_server.py` & `nonecorn-0.14.3.dev1/src/hypercorn/asyncio/udp_server.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,80 +1,82 @@
-from __future__ import annotations
-
-import asyncio
-import os
-from typing import IO, Optional, Tuple, TYPE_CHECKING
-
-from .task_group import TaskGroup
-from .worker_context import WorkerContext
-from ..config import Config
-from ..events import Event, RawData, ZeroCopySend
-from ..typing import AppWrapper
-from ..utils import parse_socket_addr
-
-if TYPE_CHECKING:
-    # h3/Quic is an optional part of Hypercorn
-    from ..protocol.quic import QuicProtocol  # noqa: F401
-
-
-class UDPServer(asyncio.DatagramProtocol):
-    def __init__(
-        self,
-        app: AppWrapper,
-        loop: asyncio.AbstractEventLoop,
-        config: Config,
-        context: WorkerContext,
-    ) -> None:
-        self.app = app
-        self.config = config
-        self.context = context
-        self.loop = loop
-        self.protocol: "QuicProtocol"
-        self.protocol_queue: asyncio.Queue = asyncio.Queue(10)
-        self.transport: Optional[asyncio.DatagramTransport] = None
-
-    def connection_made(self, transport: asyncio.DatagramTransport) -> None:  # type: ignore
-        self.transport = transport
-
-    def datagram_received(self, data: bytes, address: Tuple[bytes, str]) -> None:  # type: ignore
-        try:
-            self.protocol_queue.put_nowait(RawData(data=data, address=address))  # type: ignore
-        except asyncio.QueueFull:
-            pass  # Just throw the data away, is UDP
-
-    async def run(self) -> None:
-        # h3/Quic is an optional part of Hypercorn
-        from ..protocol.quic import QuicProtocol  # noqa: F811
-
-        socket = self.transport.get_extra_info("socket")
-        server = parse_socket_addr(socket.family, socket.getsockname())
-        async with TaskGroup(self.loop) as task_group:
-            self.protocol = QuicProtocol(
-                self.app, self.config, self.context, task_group, server, self.protocol_send
-            )
-
-            while not self.context.terminated.is_set() or not self.protocol.idle:
-                event = await self.protocol_queue.get()
-                await self.protocol.handle(event)
-
-    async def protocol_send(self, event: Event) -> None:
-        if isinstance(event, RawData):
-            self.transport.sendto(event.data, event.address)
-        elif isinstance(event, ZeroCopySend):
-            await self.zerocopysend(event.file, event.offset, event.count)
-
-    async def zerocopysend(
-        self, file: IO[bytes], offset: int = 0, count: Optional[int] = None
-    ) -> None:
-        if offset is None:
-            offset = os.lseek(file.fileno(), 0, os.SEEK_CUR)
-        if count is None:
-            count = os.stat(file.fileno()).st_size - offset
-        try:
-            await self.loop.sendfile(self.writer.transport, file, offset, count)
-        except (NotImplementedError, AttributeError):
-            os.sendfile(
-                self.writer.transport.get_extra_info("socket").fileno(),
-                file.fileno(),
-                offset,
-                count,
-            )
+from __future__ import annotations
+
+import asyncio
+import os
+from typing import IO, Optional, Tuple, Dict, Any, TYPE_CHECKING
+
+from .task_group import TaskGroup
+from .worker_context import WorkerContext
+from ..config import Config
+from ..events import Event, RawData, ZeroCopySend
+from ..typing import AppWrapper
+from ..utils import parse_socket_addr
+
+if TYPE_CHECKING:
+    # h3/Quic is an optional part of Hypercorn
+    from ..protocol.quic import QuicProtocol  # noqa: F401
+
+
+class UDPServer(asyncio.DatagramProtocol):
+    def __init__(
+        self,
+        app: AppWrapper,
+        loop: asyncio.AbstractEventLoop,
+        config: Config,
+        context: WorkerContext,
+        app_state: Dict[str, Any],
+    ) -> None:
+        self.app = app
+        self.config = config
+        self.context = context
+        self.loop = loop
+        self.protocol: "QuicProtocol"
+        self.protocol_queue: asyncio.Queue = asyncio.Queue(10)
+        self.transport: Optional[asyncio.DatagramTransport] = None
+        self.app_state = app_state
+
+    def connection_made(self, transport: asyncio.DatagramTransport) -> None:  # type: ignore
+        self.transport = transport
+
+    def datagram_received(self, data: bytes, address: Tuple[bytes, str]) -> None:  # type: ignore
+        try:
+            self.protocol_queue.put_nowait(RawData(data=data, address=address))  # type: ignore
+        except asyncio.QueueFull:
+            pass  # Just throw the data away, is UDP
+
+    async def run(self) -> None:
+        # h3/Quic is an optional part of Hypercorn
+        from ..protocol.quic import QuicProtocol  # noqa: F811
+
+        socket = self.transport.get_extra_info("socket")
+        server = parse_socket_addr(socket.family, socket.getsockname())
+        async with TaskGroup(self.loop) as task_group:
+            self.protocol = QuicProtocol(
+                self.app, self.config, self.context, task_group, server, self.protocol_send, self.app_state
+            )
+
+            while not self.context.terminated.is_set() or not self.protocol.idle:
+                event = await self.protocol_queue.get()
+                await self.protocol.handle(event)
+
+    async def protocol_send(self, event: Event) -> None:
+        if isinstance(event, RawData):
+            self.transport.sendto(event.data, event.address)
+        elif isinstance(event, ZeroCopySend):
+            await self.zerocopysend(event.file, event.offset, event.count)
+
+    async def zerocopysend(
+        self, file: IO[bytes], offset: int = 0, count: Optional[int] = None
+    ) -> None:
+        if offset is None:
+            offset = os.lseek(file.fileno(), 0, os.SEEK_CUR)
+        if count is None:
+            count = os.stat(file.fileno()).st_size - offset
+        try:
+            await self.loop.sendfile(self.writer.transport, file, offset, count)
+        except (NotImplementedError, AttributeError):
+            os.sendfile(
+                self.writer.transport.get_extra_info("socket").fileno(),
+                file.fileno(),
+                offset,
+                count,
+            )
```

### Comparing `nonecorn-0.14.1.dev1/src/hypercorn/asyncio/worker_context.py` & `nonecorn-0.14.3.dev1/src/hypercorn/asyncio/worker_context.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-from __future__ import annotations
-
-import asyncio
-from typing import Type, Union
-
-from ..typing import Event
-
-
-class EventWrapper:
-    def __init__(self) -> None:
-        self._event = asyncio.Event()
-
-    async def clear(self) -> None:
-        self._event.clear()
-
-    async def wait(self) -> None:
-        await self._event.wait()
-
-    async def set(self) -> None:
-        self._event.set()
-
-    def is_set(self) -> bool:
-        return self._event.is_set()
-
-
-class WorkerContext:
-    event_class: Type[Event] = EventWrapper
-
-    def __init__(self) -> None:
-        self.terminated = self.event_class()
-
-    @staticmethod
-    async def sleep(wait: Union[float, int]) -> None:
-        return await asyncio.sleep(wait)
-
-    @staticmethod
-    def time() -> float:
-        return asyncio.get_event_loop().time()
+from __future__ import annotations
+
+import asyncio
+from typing import Type, Union
+
+from ..typing import Event
+
+
+class EventWrapper:
+    def __init__(self) -> None:
+        self._event = asyncio.Event()
+
+    async def clear(self) -> None:
+        self._event.clear()
+
+    async def wait(self) -> None:
+        await self._event.wait()
+
+    async def set(self) -> None:
+        self._event.set()
+
+    def is_set(self) -> bool:
+        return self._event.is_set()
+
+
+class WorkerContext:
+    event_class: Type[Event] = EventWrapper
+
+    def __init__(self) -> None:
+        self.terminated = self.event_class()
+
+    @staticmethod
+    async def sleep(wait: Union[float, int]) -> None:
+        return await asyncio.sleep(wait)
+
+    @staticmethod
+    def time() -> float:
+        return asyncio.get_event_loop().time()
```

### Comparing `nonecorn-0.14.1.dev1/src/hypercorn/config.py` & `nonecorn-0.14.3.dev1/src/hypercorn/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,403 +1,407 @@
-from __future__ import annotations
-
-import importlib
-import importlib.util
-import logging
-import os
-import socket
-import stat
-import types
-import warnings
-from dataclasses import dataclass
-from ssl import (
-    create_default_context,
-    OP_NO_COMPRESSION,
-    Purpose,
-    SSLContext,
-    TLSVersion,
-    VerifyFlags,
-    VerifyMode,
-)
-from time import time
-from typing import Any, AnyStr, Dict, List, Mapping, Optional, Sequence, Tuple, Type, Union
-from wsgiref.handlers import format_date_time
-
-import toml
-
-from .logging import Logger
-
-BYTES = 1
-OCTETS = 1
-SECONDS = 1.0
-
-FilePath = Union[AnyStr, os.PathLike]
-SocketKind = Union[int, socket.SocketKind]
-
-
-@dataclass
-class Sockets:
-    secure_sockets: List[socket.socket]
-    insecure_sockets: List[socket.socket]
-    quic_sockets: List[socket.socket]
-
-
-class SocketTypeError(Exception):
-    def __init__(self, expected: SocketKind, actual: SocketKind) -> None:
-        super().__init__(
-            f'Unexpected socket type, wanted "{socket.SocketKind(expected)}" got '
-            f'"{socket.SocketKind(actual)}"'
-        )
-
-
-class Config:
-    _bind = ["127.0.0.1:8000"]
-    _insecure_bind: List[str] = []
-    _quic_bind: List[str] = []
-    _quic_addresses: List[Tuple] = []
-    _log: Optional[Logger] = None
-    _root_path: str = ""
-
-    access_log_format = '%(h)s %(l)s %(l)s %(t)s "%(r)s" %(s)s %(b)s "%(f)s" "%(a)s"'
-    accesslog: Union[logging.Logger, str, None] = None
-    alpn_protocols = ["h2", "http/1.1"]
-    alt_svc_headers: List[str] = []
-    application_path: str
-    backlog = 100
-    ca_certs: Optional[Union[str, os.PathLike, Sequence[Union[str, os.PathLike]]]] = None
-    certfile: Optional[str] = None
-    cert_pem: Optional[str] = None
-    ciphers: str = "ECDHE+AESGCM"
-    debug = False
-    dogstatsd_tags = ""
-    errorlog: Union[logging.Logger, str, None] = "-"
-    graceful_timeout: float = 3 * SECONDS
-    read_timeout: Optional[int] = None
-    group: Optional[int] = None
-    h11_max_incomplete_size = 16 * 1024 * BYTES
-    h2_max_concurrent_streams = 100
-    h2_max_header_list_size = 2**16
-    h2_max_inbound_frame_size = 2**14 * OCTETS
-    include_date_header = True
-    include_server_header = True
-    keep_alive_timeout = 5 * SECONDS
-    keyfile: Optional[str] = None
-    keyfile_password: Optional[str] = None
-    logconfig: Optional[str] = None
-    logconfig_dict: Optional[dict] = None
-    logger_class = Logger
-    loglevel: str = "INFO"
-    max_app_queue_size: int = 10
-    pid_path: Optional[str] = None
-    server_names: List[str] = []
-    shutdown_timeout = 60 * SECONDS
-    ssl_handshake_timeout = 60 * SECONDS
-    startup_timeout = 60 * SECONDS
-    statsd_host: Optional[str] = None
-    statsd_prefix = ""
-    umask: Optional[int] = None
-    use_reloader = False
-    user: Optional[int] = None
-    verify_flags: Optional[VerifyFlags] = None
-    verify_mode: Optional[VerifyMode] = None
-    websocket_max_message_size = 16 * 1024 * 1024 * BYTES
-    websocket_ping_interval: Optional[float] = None
-    worker_class = "asyncio"
-    workers = 1
-    wsgi_max_body_size = 16 * 1024 * 1024 * BYTES
-
-    def set_cert_reqs(self, value: int) -> None:
-        warnings.warn("Please use verify_mode instead", Warning)
-        self.verify_mode = VerifyMode(value)
-
-    cert_reqs = property(None, set_cert_reqs)
-
-    @property
-    def log(self) -> Logger:
-        if self._log is None:
-            self._log = self.logger_class(self)
-        return self._log
-
-    @property
-    def bind(self) -> List[str]:
-        return self._bind
-
-    @bind.setter
-    def bind(self, value: Union[List[str], str]) -> None:
-        if isinstance(value, str):
-            self._bind = [value]
-        else:
-            self._bind = value
-
-    @property
-    def insecure_bind(self) -> List[str]:
-        return self._insecure_bind
-
-    @insecure_bind.setter
-    def insecure_bind(self, value: Union[List[str], str]) -> None:
-        if isinstance(value, str):
-            self._insecure_bind = [value]
-        else:
-            self._insecure_bind = value
-
-    @property
-    def quic_bind(self) -> List[str]:
-        return self._quic_bind
-
-    @quic_bind.setter
-    def quic_bind(self, value: Union[List[str], str]) -> None:
-        if isinstance(value, str):
-            self._quic_bind = [value]
-        else:
-            self._quic_bind = value
-
-    @property
-    def root_path(self) -> str:
-        return self._root_path
-
-    @root_path.setter
-    def root_path(self, value: str) -> None:
-        self._root_path = value.rstrip("/")
-
-    def create_ssl_context(self) -> Optional[SSLContext]:
-        if not self.ssl_enabled:
-            return None
-
-        context = create_default_context(Purpose.CLIENT_AUTH)
-        context.set_ciphers(self.ciphers)
-        context.minimum_version = TLSVersion.TLSv1_2  # RFC 7540 Section 9.2: MUST be TLS >=1.2
-        context.options = OP_NO_COMPRESSION  # RFC 7540 Section 9.2.1: MUST disable compression
-        context.set_alpn_protocols(self.alpn_protocols)
-
-        if self.certfile is not None and self.keyfile is not None:
-            context.load_cert_chain(
-                certfile=self.certfile,
-                keyfile=self.keyfile,
-                password=self.keyfile_password,
-            )
-
-        if self.ca_certs is not None:
-            if isinstance(self.ca_certs, (str, os.PathLike)):
-                context.load_verify_locations(self.ca_certs)
-            else:
-                for ca_cert in self.ca_certs:
-                    context.load_verify_locations(ca_cert)
-        if self.verify_mode is not None:
-            context.verify_mode = self.verify_mode
-        if self.verify_flags is not None:
-            context.verify_flags = self.verify_flags
-
-        return context
-
-    @property
-    def ssl_enabled(self) -> bool:
-        return self.certfile is not None and self.keyfile is not None
-
-    def create_sockets(self) -> Sockets:
-        if self.ssl_enabled:
-            secure_sockets = self._create_sockets(self.bind)
-            insecure_sockets = self._create_sockets(self.insecure_bind)
-            quic_sockets = self._create_sockets(self.quic_bind, socket.SOCK_DGRAM)
-            self._set_quic_addresses(quic_sockets)
-        else:
-            secure_sockets = []
-            insecure_sockets = self._create_sockets(self.bind)
-            quic_sockets = []
-        return Sockets(secure_sockets, insecure_sockets, quic_sockets)
-
-    def _set_quic_addresses(self, sockets: List[socket.socket]) -> None:
-        self._quic_addresses = []
-        for sock in sockets:
-            name = sock.getsockname()
-            if type(name) is not str and len(name) >= 2:
-                self._quic_addresses.append(name)
-            else:
-                warnings.warn(
-                    f'Cannot create a alt-svc header for the QUIC socket with address "{name}"',
-                    Warning,
-                )
-
-    def _create_sockets(
-        self, binds: List[str], type_: int = socket.SOCK_STREAM
-    ) -> List[socket.socket]:
-        sockets: List[socket.socket] = []
-        for bind in binds:
-            binding: Any = None
-            if bind.startswith("unix:"):
-                sock = socket.socket(socket.AF_UNIX, type_)
-                binding = bind[5:]
-                try:
-                    if stat.S_ISSOCK(os.stat(binding).st_mode):
-                        os.remove(binding)
-                except FileNotFoundError:
-                    pass
-            elif bind.startswith("fd://"):
-                sock = socket.socket(fileno=int(bind[5:]))
-                actual_type = sock.getsockopt(socket.SOL_SOCKET, socket.SO_TYPE)
-                if actual_type != type_:
-                    raise SocketTypeError(type_, actual_type)
-            else:
-                bind = bind.replace("[", "").replace("]", "")
-                try:
-                    value = bind.rsplit(":", 1)
-                    host, port = value[0], int(value[1])
-                except (ValueError, IndexError):
-                    host, port = bind, 8000
-                sock = socket.socket(socket.AF_INET6 if ":" in host else socket.AF_INET, type_)
-                if self.workers > 1:
-                    try:
-                        sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEPORT, 1)
-                    except AttributeError:
-                        pass
-                binding = (host, port)
-
-            sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
-
-            if bind.startswith("unix:"):
-                if self.umask is not None:
-                    current_umask = os.umask(self.umask)
-                sock.bind(binding)
-                if self.user is not None and self.group is not None:
-                    os.chown(binding, self.user, self.group)
-                if self.umask is not None:
-                    os.umask(current_umask)
-            elif bind.startswith("fd://"):
-                pass
-            else:
-                sock.bind(binding)
-
-            sock.setblocking(False)
-            try:
-                sock.set_inheritable(True)
-            except AttributeError:
-                pass
-            sockets.append(sock)
-        return sockets
-
-    def response_headers(self, protocol: str) -> List[Tuple[bytes, bytes]]:
-        headers = []
-        if self.include_date_header:
-            headers.append((b"date", format_date_time(time()).encode("ascii")))
-        if self.include_server_header:
-            headers.append((b"server", f"hypercorn-{protocol}".encode("ascii")))
-
-        for alt_svc_header in self.alt_svc_headers:
-            headers.append((b"alt-svc", alt_svc_header.encode()))
-        if len(self.alt_svc_headers) == 0 and self._quic_addresses:
-            from aioquic.h3.connection import H3_ALPN
-
-            for version in H3_ALPN:
-                for addr in self._quic_addresses:
-                    port = addr[1]
-                    headers.append((b"alt-svc", b'%s=":%d"; ma=3600' % (version.encode(), port)))
-
-        return headers
-
-    def set_statsd_logger_class(self, statsd_logger: Type[Logger]) -> None:
-        if self.logger_class == Logger and self.statsd_host is not None:
-            self.logger_class = statsd_logger
-
-    @classmethod
-    def from_mapping(
-        cls: Type["Config"], mapping: Optional[Mapping[str, Any]] = None, **kwargs: Any
-    ) -> "Config":
-        """Create a configuration from a mapping.
-
-        This allows either a mapping to be directly passed or as
-        keyword arguments, for example,
-
-        .. code-block:: python
-
-            config = {'keep_alive_timeout': 10}
-            Config.from_mapping(config)
-            Config.from_mapping(keep_alive_timeout=10)
-
-        Arguments:
-            mapping: Optionally a mapping object.
-            kwargs: Optionally a collection of keyword arguments to
-                form a mapping.
-        """
-        mappings: Dict[str, Any] = {}
-        if mapping is not None:
-            mappings.update(mapping)
-        mappings.update(kwargs)
-        config = cls()
-        for key, value in mappings.items():
-            try:
-                setattr(config, key, value)
-            except AttributeError:
-                pass
-        if config.certfile is not None:
-            with open(config.certfile) as file:
-                config.cert_pem = file.read()
-        return config
-
-    @classmethod
-    def from_pyfile(cls: Type["Config"], filename: FilePath) -> "Config":
-        """Create a configuration from a Python file.
-
-        .. code-block:: python
-
-            Config.from_pyfile('hypercorn_config.py')
-
-        Arguments:
-            filename: The filename which gives the path to the file.
-        """
-        file_path = os.fspath(filename)
-        spec = importlib.util.spec_from_file_location("module.name", file_path)
-        module = importlib.util.module_from_spec(spec)
-        spec.loader.exec_module(module)
-        return cls.from_object(module)
-
-    @classmethod
-    def from_toml(cls: Type["Config"], filename: FilePath) -> "Config":
-        """Load the configuration values from a TOML formatted file.
-
-        This allows configuration to be loaded as so
-
-        .. code-block:: python
-
-            Config.from_toml('config.toml')
-
-        Arguments:
-            filename: The filename which gives the path to the file.
-        """
-        file_path = os.fspath(filename)
-        with open(file_path) as file_:
-            data = toml.load(file_)
-        return cls.from_mapping(data)
-
-    @classmethod
-    def from_object(cls: Type["Config"], instance: Union[object, str]) -> "Config":
-        """Create a configuration from a Python object.
-
-        This can be used to reference modules or objects within
-        modules for example,
-
-        .. code-block:: python
-
-            Config.from_object('module')
-            Config.from_object('module.instance')
-            from module import instance
-            Config.from_object(instance)
-
-        are valid.
-
-        Arguments:
-            instance: Either a str referencing a python object or the
-                object itself.
-
-        """
-        if isinstance(instance, str):
-            try:
-                instance = importlib.import_module(instance)
-            except ImportError:
-                path, config = instance.rsplit(".", 1)
-                module = importlib.import_module(path)
-                instance = getattr(module, config)
-
-        mapping = {
-            key: getattr(instance, key)
-            for key in dir(instance)
-            if not isinstance(getattr(instance, key), types.ModuleType)
-        }
-        return cls.from_mapping(mapping)
+from __future__ import annotations
+
+import importlib
+import importlib.util
+import logging
+import os
+import socket
+import stat
+import sys
+import types
+import warnings
+from dataclasses import dataclass
+from ssl import (
+    create_default_context,
+    OP_NO_COMPRESSION,
+    Purpose,
+    SSLContext,
+    TLSVersion,
+    VerifyFlags,
+    VerifyMode,
+)
+from time import time
+from typing import Any, AnyStr, Dict, List, Mapping, Optional, Sequence, Tuple, Type, Union
+from wsgiref.handlers import format_date_time
+
+if sys.version_info >= (3, 11):
+    import tomllib
+else:
+    import tomli as tomllib
+
+from .logging import Logger
+
+BYTES = 1
+OCTETS = 1
+SECONDS = 1.0
+
+FilePath = Union[AnyStr, os.PathLike]
+SocketKind = Union[int, socket.SocketKind]
+
+
+@dataclass
+class Sockets:
+    secure_sockets: List[socket.socket]
+    insecure_sockets: List[socket.socket]
+    quic_sockets: List[socket.socket]
+
+
+class SocketTypeError(Exception):
+    def __init__(self, expected: SocketKind, actual: SocketKind) -> None:
+        super().__init__(
+            f'Unexpected socket type, wanted "{socket.SocketKind(expected)}" got '
+            f'"{socket.SocketKind(actual)}"'
+        )
+
+
+class Config:
+    _bind = ["127.0.0.1:8000"]
+    _insecure_bind: List[str] = []
+    _quic_bind: List[str] = []
+    _quic_addresses: List[Tuple] = []
+    _log: Optional[Logger] = None
+    _root_path: str = ""
+
+    access_log_format = '%(h)s %(l)s %(l)s %(t)s "%(r)s" %(s)s %(b)s "%(f)s" "%(a)s"'
+    accesslog: Union[logging.Logger, str, None] = None
+    alpn_protocols = ["h2", "http/1.1"]
+    alt_svc_headers: List[str] = []
+    application_path: str
+    backlog = 100
+    ca_certs: Optional[Union[str, os.PathLike, Sequence[Union[str, os.PathLike]]]] = None
+    certfile: Optional[str] = None
+    cert_pem: Optional[str] = None
+    ciphers: str = "ECDHE+AESGCM"
+    debug = False
+    dogstatsd_tags = ""
+    errorlog: Union[logging.Logger, str, None] = "-"
+    graceful_timeout: float = 3 * SECONDS
+    read_timeout: Optional[int] = None
+    group: Optional[int] = None
+    h11_max_incomplete_size = 16 * 1024 * BYTES
+    h2_max_concurrent_streams = 100
+    h2_max_header_list_size = 2**16
+    h2_max_inbound_frame_size = 2**14 * OCTETS
+    include_date_header = True
+    include_server_header = True
+    keep_alive_timeout = 5 * SECONDS
+    keyfile: Optional[str] = None
+    keyfile_password: Optional[str] = None
+    logconfig: Optional[str] = None
+    logconfig_dict: Optional[dict] = None
+    logger_class = Logger
+    loglevel: str = "INFO"
+    max_app_queue_size: int = 10
+    pid_path: Optional[str] = None
+    server_names: List[str] = []
+    shutdown_timeout = 60 * SECONDS
+    ssl_handshake_timeout = 60 * SECONDS
+    startup_timeout = 60 * SECONDS
+    statsd_host: Optional[str] = None
+    statsd_prefix = ""
+    umask: Optional[int] = None
+    use_reloader = False
+    user: Optional[int] = None
+    verify_flags: Optional[VerifyFlags] = None
+    verify_mode: Optional[VerifyMode] = None
+    websocket_max_message_size = 16 * 1024 * 1024 * BYTES
+    websocket_ping_interval: Optional[float] = None
+    worker_class = "asyncio"
+    workers = 1
+    wsgi_max_body_size = 16 * 1024 * 1024 * BYTES
+
+    def set_cert_reqs(self, value: int) -> None:
+        warnings.warn("Please use verify_mode instead", Warning)
+        self.verify_mode = VerifyMode(value)
+
+    cert_reqs = property(None, set_cert_reqs)
+
+    @property
+    def log(self) -> Logger:
+        if self._log is None:
+            self._log = self.logger_class(self)
+        return self._log
+
+    @property
+    def bind(self) -> List[str]:
+        return self._bind
+
+    @bind.setter
+    def bind(self, value: Union[List[str], str]) -> None:
+        if isinstance(value, str):
+            self._bind = [value]
+        else:
+            self._bind = value
+
+    @property
+    def insecure_bind(self) -> List[str]:
+        return self._insecure_bind
+
+    @insecure_bind.setter
+    def insecure_bind(self, value: Union[List[str], str]) -> None:
+        if isinstance(value, str):
+            self._insecure_bind = [value]
+        else:
+            self._insecure_bind = value
+
+    @property
+    def quic_bind(self) -> List[str]:
+        return self._quic_bind
+
+    @quic_bind.setter
+    def quic_bind(self, value: Union[List[str], str]) -> None:
+        if isinstance(value, str):
+            self._quic_bind = [value]
+        else:
+            self._quic_bind = value
+
+    @property
+    def root_path(self) -> str:
+        return self._root_path
+
+    @root_path.setter
+    def root_path(self, value: str) -> None:
+        self._root_path = value.rstrip("/")
+
+    def create_ssl_context(self) -> Optional[SSLContext]:
+        if not self.ssl_enabled:
+            return None
+
+        context = create_default_context(Purpose.CLIENT_AUTH)
+        context.set_ciphers(self.ciphers)
+        context.minimum_version = TLSVersion.TLSv1_2  # RFC 7540 Section 9.2: MUST be TLS >=1.2
+        context.options = OP_NO_COMPRESSION  # RFC 7540 Section 9.2.1: MUST disable compression
+        context.set_alpn_protocols(self.alpn_protocols)
+
+        if self.certfile is not None and self.keyfile is not None:
+            context.load_cert_chain(
+                certfile=self.certfile,
+                keyfile=self.keyfile,
+                password=self.keyfile_password,
+            )
+
+        if self.ca_certs is not None:
+            if isinstance(self.ca_certs, (str, os.PathLike)):
+                context.load_verify_locations(self.ca_certs)
+            else:
+                for ca_cert in self.ca_certs:
+                    context.load_verify_locations(ca_cert)
+        if self.verify_mode is not None:
+            context.verify_mode = self.verify_mode
+        if self.verify_flags is not None:
+            context.verify_flags = self.verify_flags
+
+        return context
+
+    @property
+    def ssl_enabled(self) -> bool:
+        return self.certfile is not None and self.keyfile is not None
+
+    def create_sockets(self) -> Sockets:
+        if self.ssl_enabled:
+            secure_sockets = self._create_sockets(self.bind)
+            insecure_sockets = self._create_sockets(self.insecure_bind)
+            quic_sockets = self._create_sockets(self.quic_bind, socket.SOCK_DGRAM)
+            self._set_quic_addresses(quic_sockets)
+        else:
+            secure_sockets = []
+            insecure_sockets = self._create_sockets(self.bind)
+            quic_sockets = []
+        return Sockets(secure_sockets, insecure_sockets, quic_sockets)
+
+    def _set_quic_addresses(self, sockets: List[socket.socket]) -> None:
+        self._quic_addresses = []
+        for sock in sockets:
+            name = sock.getsockname()
+            if type(name) is not str and len(name) >= 2:
+                self._quic_addresses.append(name)
+            else:
+                warnings.warn(
+                    f'Cannot create a alt-svc header for the QUIC socket with address "{name}"',
+                    Warning,
+                )
+
+    def _create_sockets(
+        self, binds: List[str], type_: int = socket.SOCK_STREAM
+    ) -> List[socket.socket]:
+        sockets: List[socket.socket] = []
+        for bind in binds:
+            binding: Any = None
+            if bind.startswith("unix:"):
+                sock = socket.socket(socket.AF_UNIX, type_)
+                binding = bind[5:]
+                try:
+                    if stat.S_ISSOCK(os.stat(binding).st_mode):
+                        os.remove(binding)
+                except FileNotFoundError:
+                    pass
+            elif bind.startswith("fd://"):
+                sock = socket.socket(fileno=int(bind[5:]))
+                actual_type = sock.getsockopt(socket.SOL_SOCKET, socket.SO_TYPE)
+                if actual_type != type_:
+                    raise SocketTypeError(type_, actual_type)
+            else:
+                bind = bind.replace("[", "").replace("]", "")
+                try:
+                    value = bind.rsplit(":", 1)
+                    host, port = value[0], int(value[1])
+                except (ValueError, IndexError):
+                    host, port = bind, 8000
+                sock = socket.socket(socket.AF_INET6 if ":" in host else socket.AF_INET, type_)
+                if self.workers > 1:
+                    try:
+                        sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEPORT, 1)
+                    except AttributeError:
+                        pass
+                binding = (host, port)
+
+            sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+
+            if bind.startswith("unix:"):
+                if self.umask is not None:
+                    current_umask = os.umask(self.umask)
+                sock.bind(binding)
+                if self.user is not None and self.group is not None:
+                    os.chown(binding, self.user, self.group)
+                if self.umask is not None:
+                    os.umask(current_umask)
+            elif bind.startswith("fd://"):
+                pass
+            else:
+                sock.bind(binding)
+
+            sock.setblocking(False)
+            try:
+                sock.set_inheritable(True)
+            except AttributeError:
+                pass
+            sockets.append(sock)
+        return sockets
+
+    def response_headers(self, protocol: str) -> List[Tuple[bytes, bytes]]:
+        headers = []
+        if self.include_date_header:
+            headers.append((b"date", format_date_time(time()).encode("ascii")))
+        if self.include_server_header:
+            headers.append((b"server", f"hypercorn-{protocol}".encode("ascii")))
+
+        for alt_svc_header in self.alt_svc_headers:
+            headers.append((b"alt-svc", alt_svc_header.encode()))
+        if len(self.alt_svc_headers) == 0 and self._quic_addresses:
+            from aioquic.h3.connection import H3_ALPN
+
+            for version in H3_ALPN:
+                for addr in self._quic_addresses:
+                    port = addr[1]
+                    headers.append((b"alt-svc", b'%s=":%d"; ma=3600' % (version.encode(), port)))
+
+        return headers
+
+    def set_statsd_logger_class(self, statsd_logger: Type[Logger]) -> None:
+        if self.logger_class == Logger and self.statsd_host is not None:
+            self.logger_class = statsd_logger
+
+    @classmethod
+    def from_mapping(
+        cls: Type["Config"], mapping: Optional[Mapping[str, Any]] = None, **kwargs: Any
+    ) -> "Config":
+        """Create a configuration from a mapping.
+
+        This allows either a mapping to be directly passed or as
+        keyword arguments, for example,
+
+        .. code-block:: python
+
+            config = {'keep_alive_timeout': 10}
+            Config.from_mapping(config)
+            Config.from_mapping(keep_alive_timeout=10)
+
+        Arguments:
+            mapping: Optionally a mapping object.
+            kwargs: Optionally a collection of keyword arguments to
+                form a mapping.
+        """
+        mappings: Dict[str, Any] = {}
+        if mapping is not None:
+            mappings.update(mapping)
+        mappings.update(kwargs)
+        config = cls()
+        for key, value in mappings.items():
+            try:
+                setattr(config, key, value)
+            except AttributeError:
+                pass
+        if config.certfile is not None:
+            with open(config.certfile) as file:
+                config.cert_pem = file.read()
+        return config
+
+    @classmethod
+    def from_pyfile(cls: Type["Config"], filename: FilePath) -> "Config":
+        """Create a configuration from a Python file.
+
+        .. code-block:: python
+
+            Config.from_pyfile('hypercorn_config.py')
+
+        Arguments:
+            filename: The filename which gives the path to the file.
+        """
+        file_path = os.fspath(filename)
+        spec = importlib.util.spec_from_file_location("module.name", file_path)
+        module = importlib.util.module_from_spec(spec)
+        spec.loader.exec_module(module)
+        return cls.from_object(module)
+
+    @classmethod
+    def from_toml(cls: Type["Config"], filename: FilePath) -> "Config":
+        """Load the configuration values from a TOML formatted file.
+
+        This allows configuration to be loaded as so
+
+        .. code-block:: python
+
+            Config.from_toml('config.toml')
+
+        Arguments:
+            filename: The filename which gives the path to the file.
+        """
+        file_path = os.fspath(filename)
+        with open(file_path, "rb") as file_:
+            data = tomllib.load(file_)
+        return cls.from_mapping(data)
+
+    @classmethod
+    def from_object(cls: Type["Config"], instance: Union[object, str]) -> "Config":
+        """Create a configuration from a Python object.
+
+        This can be used to reference modules or objects within
+        modules for example,
+
+        .. code-block:: python
+
+            Config.from_object('module')
+            Config.from_object('module.instance')
+            from module import instance
+            Config.from_object(instance)
+
+        are valid.
+
+        Arguments:
+            instance: Either a str referencing a python object or the
+                object itself.
+
+        """
+        if isinstance(instance, str):
+            try:
+                instance = importlib.import_module(instance)
+            except ImportError:
+                path, config = instance.rsplit(".", 1)
+                module = importlib.import_module(path)
+                instance = getattr(module, config)
+
+        mapping = {
+            key: getattr(instance, key)
+            for key in dir(instance)
+            if not isinstance(getattr(instance, key), types.ModuleType) and not key.startswith("__")
+        }
+        return cls.from_mapping(mapping)
```

### Comparing `nonecorn-0.14.1.dev1/src/hypercorn/logging.py` & `nonecorn-0.14.3.dev1/src/hypercorn/logging.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,194 +1,198 @@
-from __future__ import annotations
-
-import json
-import logging
-import os
-import sys
-import time
-from http import HTTPStatus
-from logging.config import dictConfig, fileConfig
-from typing import Any, IO, Mapping, Optional, TYPE_CHECKING, Union
-
-import toml
-
-if TYPE_CHECKING:
-    from .config import Config
-    from .typing import ResponseSummary, WWWScope
-
-
-def _create_logger(
-    name: str,
-    target: Union[logging.Logger, str, None],
-    level: Optional[str],
-    sys_default: IO,
-    *,
-    propagate: bool = True,
-) -> Optional[logging.Logger]:
-    if isinstance(target, logging.Logger):
-        return target
-
-    if target:
-        logger = logging.getLogger(name)
-        logger.handlers = [
-            logging.StreamHandler(sys_default) if target == "-" else logging.FileHandler(target)  # type: ignore # noqa: E501
-        ]
-        logger.propagate = propagate
-        formatter = logging.Formatter(
-            "%(asctime)s [%(process)d] [%(levelname)s] %(message)s",
-            "[%Y-%m-%d %H:%M:%S %z]",
-        )
-        logger.handlers[0].setFormatter(formatter)
-        if level is not None:
-            logger.setLevel(logging.getLevelName(level.upper()))
-        return logger
-    else:
-        return None
-
-
-class Logger:
-    def __init__(self, config: "Config") -> None:
-        self.access_log_format = config.access_log_format
-
-        self.access_logger = _create_logger(
-            "hypercorn.access",
-            config.accesslog,
-            config.loglevel,
-            sys.stdout,
-            propagate=False,
-        )
-        self.error_logger = _create_logger(
-            "hypercorn.error", config.errorlog, config.loglevel, sys.stderr
-        )
-
-        if config.logconfig is not None:
-            if config.logconfig.startswith("json:"):
-                with open(config.logconfig[5:]) as file_:
-                    dictConfig(json.load(file_))
-            elif config.logconfig.startswith("toml:"):
-                with open(config.logconfig[5:]) as file_:
-                    dictConfig(toml.load(file_))
-            else:
-                log_config = {
-                    "__file__": config.logconfig,
-                    "here": os.path.dirname(config.logconfig),
-                }
-                fileConfig(config.logconfig, defaults=log_config, disable_existing_loggers=False)
-        else:
-            if config.logconfig_dict is not None:
-                dictConfig(config.logconfig_dict)
-
-    async def access(
-        self, request: "WWWScope", response: "ResponseSummary", request_time: float
-    ) -> None:
-        if self.access_logger is not None:
-            self.access_logger.info(
-                self.access_log_format, self.atoms(request, response, request_time)
-            )
-
-    async def critical(self, message: str, *args: Any, **kwargs: Any) -> None:
-        if self.error_logger is not None:
-            self.error_logger.critical(message, *args, **kwargs)
-
-    async def error(self, message: str, *args: Any, **kwargs: Any) -> None:
-        if self.error_logger is not None:
-            self.error_logger.error(message, *args, **kwargs)
-
-    async def warning(self, message: str, *args: Any, **kwargs: Any) -> None:
-        if self.error_logger is not None:
-            self.error_logger.warning(message, *args, **kwargs)
-
-    async def info(self, message: str, *args: Any, **kwargs: Any) -> None:
-        if self.error_logger is not None:
-            self.error_logger.info(message, *args, **kwargs)
-
-    async def debug(self, message: str, *args: Any, **kwargs: Any) -> None:
-        if self.error_logger is not None:
-            self.error_logger.debug(message, *args, **kwargs)
-
-    async def exception(self, message: str, *args: Any, **kwargs: Any) -> None:
-        if self.error_logger is not None:
-            self.error_logger.exception(message, *args, **kwargs)
-
-    async def log(self, level: int, message: str, *args: Any, **kwargs: Any) -> None:
-        if self.error_logger is not None:
-            self.error_logger.log(level, message, *args, **kwargs)
-
-    def atoms(
-        self, request: "WWWScope", response: "ResponseSummary", request_time: float
-    ) -> Mapping[str, str]:
-        """Create and return an access log atoms dictionary.
-
-        This can be overidden and customised if desired. It should
-        return a mapping between an access log format key and a value.
-        """
-        return AccessLogAtoms(request, response, request_time)
-
-    def __getattr__(self, name: str) -> Any:
-        return getattr(self.error_logger, name)
-
-
-class AccessLogAtoms(dict):
-    def __init__(
-        self, request: "WWWScope", response: "ResponseSummary", request_time: float
-    ) -> None:
-        for name, value in request["headers"]:
-            self[f"{{{name.decode('latin1').lower()}}}i"] = value.decode("latin1")
-        for name, value in response.get("headers", []):
-            self[f"{{{name.decode('latin1').lower()}}}o"] = value.decode("latin1")
-        for name, value in os.environ.items():
-            self[f"{{{name.lower()}}}e"] = value
-        protocol = request.get("http_version", "ws")
-        client = request.get("client")
-        if client is None:
-            remote_addr = None
-        elif len(client) == 2:
-            remote_addr = f"{client[0]}:{client[1]}"
-        elif len(client) == 1:
-            remote_addr = client[0]
-        else:  # make sure not to throw UnboundLocalError
-            remote_addr = f"<???{client}???>"
-        if request["type"] == "http":
-            method = request["method"]
-        else:
-            method = "GET"
-        query_string = request["query_string"].decode()
-        path_with_qs = request["path"] + ("?" + query_string if query_string else "")
-        status_code = response["status"]
-        try:
-            status_phrase = HTTPStatus(status_code).phrase
-        except ValueError:
-            status_phrase = f"<???{status_code}???>"
-        self.update(
-            {
-                "h": remote_addr,
-                "l": "-",
-                "t": time.strftime("[%d/%b/%Y:%H:%M:%S %z]"),
-                "r": f"{method} {request['path']} {protocol}",
-                "R": f"{method} {path_with_qs} {protocol}",
-                "s": response["status"],
-                "st": status_phrase,
-                "S": request["scheme"],
-                "m": method,
-                "U": request["path"],
-                "Uq": path_with_qs,
-                "q": query_string,
-                "H": protocol,
-                "b": self["{Content-Length}o"],
-                "B": self["{Content-Length}o"],
-                "f": self["{Referer}i"],
-                "a": self["{User-Agent}i"],
-                "T": int(request_time),
-                "D": int(request_time * 1_000_000),
-                "L": f"{request_time:.6f}",
-                "p": f"<{os.getpid()}>",
-            }
-        )
-
-    def __getitem__(self, key: str) -> str:
-        try:
-            if key.startswith("{"):
-                return super().__getitem__(key.lower())
-            else:
-                return super().__getitem__(key)
-        except KeyError:
-            return "-"
+from __future__ import annotations
+
+import json
+import logging
+import os
+import sys
+import time
+from http import HTTPStatus
+from logging.config import dictConfig, fileConfig
+from typing import Any, IO, Mapping, Optional, TYPE_CHECKING, Union
+
+if sys.version_info >= (3, 11):
+    import tomllib
+else:
+    import tomli as tomllib
+
+
+if TYPE_CHECKING:
+    from .config import Config
+    from .typing import ResponseSummary, WWWScope
+
+
+def _create_logger(
+    name: str,
+    target: Union[logging.Logger, str, None],
+    level: Optional[str],
+    sys_default: IO,
+    *,
+    propagate: bool = True,
+) -> Optional[logging.Logger]:
+    if isinstance(target, logging.Logger):
+        return target
+
+    if target:
+        logger = logging.getLogger(name)
+        logger.handlers = [
+            logging.StreamHandler(sys_default) if target == "-" else logging.FileHandler(target)  # type: ignore # noqa: E501
+        ]
+        logger.propagate = propagate
+        formatter = logging.Formatter(
+            "%(asctime)s [%(process)d] [%(levelname)s] %(message)s",
+            "[%Y-%m-%d %H:%M:%S %z]",
+        )
+        logger.handlers[0].setFormatter(formatter)
+        if level is not None:
+            logger.setLevel(logging.getLevelName(level.upper()))
+        return logger
+    else:
+        return None
+
+
+class Logger:
+    def __init__(self, config: "Config") -> None:
+        self.access_log_format = config.access_log_format
+
+        self.access_logger = _create_logger(
+            "hypercorn.access",
+            config.accesslog,
+            config.loglevel,
+            sys.stdout,
+            propagate=False,
+        )
+        self.error_logger = _create_logger(
+            "hypercorn.error", config.errorlog, config.loglevel, sys.stderr
+        )
+
+        if config.logconfig is not None:
+            if config.logconfig.startswith("json:"):
+                with open(config.logconfig[5:]) as file_:
+                    dictConfig(json.load(file_))
+            elif config.logconfig.startswith("toml:"):
+                with open(config.logconfig[5:], "rb") as file_:
+                    dictConfig(tomllib.load(file_))
+            else:
+                log_config = {
+                    "__file__": config.logconfig,
+                    "here": os.path.dirname(config.logconfig),
+                }
+                fileConfig(config.logconfig, defaults=log_config, disable_existing_loggers=False)
+        else:
+            if config.logconfig_dict is not None:
+                dictConfig(config.logconfig_dict)
+
+    async def access(
+        self, request: "WWWScope", response: "ResponseSummary", request_time: float
+    ) -> None:
+        if self.access_logger is not None:
+            self.access_logger.info(
+                self.access_log_format, self.atoms(request, response, request_time)
+            )
+
+    async def critical(self, message: str, *args: Any, **kwargs: Any) -> None:
+        if self.error_logger is not None:
+            self.error_logger.critical(message, *args, **kwargs)
+
+    async def error(self, message: str, *args: Any, **kwargs: Any) -> None:
+        if self.error_logger is not None:
+            self.error_logger.error(message, *args, **kwargs)
+
+    async def warning(self, message: str, *args: Any, **kwargs: Any) -> None:
+        if self.error_logger is not None:
+            self.error_logger.warning(message, *args, **kwargs)
+
+    async def info(self, message: str, *args: Any, **kwargs: Any) -> None:
+        if self.error_logger is not None:
+            self.error_logger.info(message, *args, **kwargs)
+
+    async def debug(self, message: str, *args: Any, **kwargs: Any) -> None:
+        if self.error_logger is not None:
+            self.error_logger.debug(message, *args, **kwargs)
+
+    async def exception(self, message: str, *args: Any, **kwargs: Any) -> None:
+        if self.error_logger is not None:
+            self.error_logger.exception(message, *args, **kwargs)
+
+    async def log(self, level: int, message: str, *args: Any, **kwargs: Any) -> None:
+        if self.error_logger is not None:
+            self.error_logger.log(level, message, *args, **kwargs)
+
+    def atoms(
+        self, request: "WWWScope", response: "ResponseSummary", request_time: float
+    ) -> Mapping[str, str]:
+        """Create and return an access log atoms dictionary.
+
+        This can be overidden and customised if desired. It should
+        return a mapping between an access log format key and a value.
+        """
+        return AccessLogAtoms(request, response, request_time)
+
+    def __getattr__(self, name: str) -> Any:
+        return getattr(self.error_logger, name)
+
+
+class AccessLogAtoms(dict):
+    def __init__(
+        self, request: "WWWScope", response: "ResponseSummary", request_time: float
+    ) -> None:
+        for name, value in request["headers"]:
+            self[f"{{{name.decode('latin1').lower()}}}i"] = value.decode("latin1")
+        for name, value in response.get("headers", []):
+            self[f"{{{name.decode('latin1').lower()}}}o"] = value.decode("latin1")
+        for name, value in os.environ.items():
+            self[f"{{{name.lower()}}}e"] = value
+        protocol = request.get("http_version", "ws")
+        client = request.get("client")
+        if client is None:
+            remote_addr = None
+        elif len(client) == 2:
+            remote_addr = f"{client[0]}:{client[1]}"
+        elif len(client) == 1:
+            remote_addr = client[0]
+        else:  # make sure not to throw UnboundLocalError
+            remote_addr = f"<???{client}???>"
+        if request["type"] == "http":
+            method = request["method"]
+        else:
+            method = "GET"
+        query_string = request["query_string"].decode()
+        path_with_qs = request["path"] + ("?" + query_string if query_string else "")
+        status_code = response["status"]
+        try:
+            status_phrase = HTTPStatus(status_code).phrase
+        except ValueError:
+            status_phrase = f"<???{status_code}???>"
+        self.update(
+            {
+                "h": remote_addr,
+                "l": "-",
+                "t": time.strftime("[%d/%b/%Y:%H:%M:%S %z]"),
+                "r": f"{method} {request['path']} {protocol}",
+                "R": f"{method} {path_with_qs} {protocol}",
+                "s": response["status"],
+                "st": status_phrase,
+                "S": request["scheme"],
+                "m": method,
+                "U": request["path"],
+                "Uq": path_with_qs,
+                "q": query_string,
+                "H": protocol,
+                "b": self["{Content-Length}o"],
+                "B": self["{Content-Length}o"],
+                "f": self["{Referer}i"],
+                "a": self["{User-Agent}i"],
+                "T": int(request_time),
+                "D": int(request_time * 1_000_000),
+                "L": f"{request_time:.6f}",
+                "p": f"<{os.getpid()}>",
+            }
+        )
+
+    def __getitem__(self, key: str) -> str:
+        try:
+            if key.startswith("{"):
+                return super().__getitem__(key.lower())
+            else:
+                return super().__getitem__(key)
+        except KeyError:
+            return "-"
```

### Comparing `nonecorn-0.14.1.dev1/src/hypercorn/middleware/dispatcher.py` & `nonecorn-0.14.3.dev1/src/hypercorn/middleware/dispatcher.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,108 +1,108 @@
-from __future__ import annotations
-
-import asyncio
-from functools import partial
-from typing import Callable, Dict
-
-from ..asyncio.task_group import TaskGroup
-from ..typing import ASGIFramework, Scope
-
-MAX_QUEUE_SIZE = 10
-
-
-class _DispatcherMiddleware:
-    def __init__(self, mounts: Dict[str, ASGIFramework]) -> None:
-        self.mounts = mounts
-
-    async def __call__(self, scope: Scope, receive: Callable, send: Callable) -> None:
-        if scope["type"] == "lifespan":
-            await self._handle_lifespan(scope, receive, send)
-        else:
-            for path, app in self.mounts.items():
-                if scope["path"].startswith(path):
-                    scope["path"] = scope["path"][len(path) :] or "/"
-                    return await app(scope, receive, send)
-            await send(
-                {
-                    "type": "http.response.start",
-                    "status": 404,
-                    "headers": [(b"content-length", b"0")],
-                }
-            )
-            await send({"type": "http.response.body"})
-
-    async def _handle_lifespan(self, scope: Scope, receive: Callable, send: Callable) -> None:
-        pass
-
-
-class AsyncioDispatcherMiddleware(_DispatcherMiddleware):
-    async def _handle_lifespan(self, scope: Scope, receive: Callable, send: Callable) -> None:
-        self.app_queues: Dict[str, asyncio.Queue] = {
-            path: asyncio.Queue(MAX_QUEUE_SIZE) for path in self.mounts
-        }
-        self.startup_complete = {path: False for path in self.mounts}
-        self.shutdown_complete = {path: False for path in self.mounts}
-
-        async with TaskGroup(asyncio.get_event_loop()) as task_group:
-            for path, app in self.mounts.items():
-                task_group.spawn(
-                    app,
-                    scope,
-                    self.app_queues[path].get,
-                    partial(self.send, path, send),
-                )
-
-            while True:
-                message = await receive()
-                for queue in self.app_queues.values():
-                    await queue.put(message)
-                if message["type"] == "lifespan.shutdown":
-                    break
-
-    async def send(self, path: str, send: Callable, message: dict) -> None:
-        if message["type"] == "lifespan.startup.complete":
-            self.startup_complete[path] = True
-            if all(self.startup_complete.values()):
-                await send({"type": "lifespan.startup.complete"})
-        elif message["type"] == "lifespan.shutdown.complete":
-            self.shutdown_complete[path] = True
-            if all(self.shutdown_complete.values()):
-                await send({"type": "lifespan.shutdown.complete"})
-
-
-class TrioDispatcherMiddleware(_DispatcherMiddleware):
-    async def _handle_lifespan(self, scope: Scope, receive: Callable, send: Callable) -> None:
-        import trio
-
-        self.app_queues = {path: trio.open_memory_channel(MAX_QUEUE_SIZE) for path in self.mounts}
-        self.startup_complete = {path: False for path in self.mounts}
-        self.shutdown_complete = {path: False for path in self.mounts}
-
-        async with trio.open_nursery() as nursery:
-            for path, app in self.mounts.items():
-                nursery.start_soon(
-                    app,
-                    scope,
-                    self.app_queues[path][1].receive,
-                    partial(self.send, path, send),
-                )
-
-            while True:
-                message = await receive()
-                for channels in self.app_queues.values():
-                    await channels[0].send(message)
-                if message["type"] == "lifespan.shutdown":
-                    break
-
-    async def send(self, path: str, send: Callable, message: dict) -> None:
-        if message["type"] == "lifespan.startup.complete":
-            self.startup_complete[path] = True
-            if all(self.startup_complete.values()):
-                await send({"type": "lifespan.startup.complete"})
-        elif message["type"] == "lifespan.shutdown.complete":
-            self.shutdown_complete[path] = True
-            if all(self.shutdown_complete.values()):
-                await send({"type": "lifespan.shutdown.complete"})
-
-
-DispatcherMiddleware = AsyncioDispatcherMiddleware  # Remove with version 0.11
+from __future__ import annotations
+
+import asyncio
+from functools import partial
+from typing import Callable, Dict
+
+from ..asyncio.task_group import TaskGroup
+from ..typing import ASGIFramework, Scope
+
+MAX_QUEUE_SIZE = 10
+
+
+class _DispatcherMiddleware:
+    def __init__(self, mounts: Dict[str, ASGIFramework]) -> None:
+        self.mounts = mounts
+
+    async def __call__(self, scope: Scope, receive: Callable, send: Callable) -> None:
+        if scope["type"] == "lifespan":
+            await self._handle_lifespan(scope, receive, send)
+        else:
+            for path, app in self.mounts.items():
+                if scope["path"].startswith(path):
+                    scope["path"] = scope["path"][len(path) :] or "/"
+                    return await app(scope, receive, send)
+            await send(
+                {
+                    "type": "http.response.start",
+                    "status": 404,
+                    "headers": [(b"content-length", b"0")],
+                }
+            )
+            await send({"type": "http.response.body"})
+
+    async def _handle_lifespan(self, scope: Scope, receive: Callable, send: Callable) -> None:
+        pass
+
+
+class AsyncioDispatcherMiddleware(_DispatcherMiddleware):
+    async def _handle_lifespan(self, scope: Scope, receive: Callable, send: Callable) -> None:
+        self.app_queues: Dict[str, asyncio.Queue] = {
+            path: asyncio.Queue(MAX_QUEUE_SIZE) for path in self.mounts
+        }
+        self.startup_complete = {path: False for path in self.mounts}
+        self.shutdown_complete = {path: False for path in self.mounts}
+
+        async with TaskGroup(asyncio.get_event_loop()) as task_group:
+            for path, app in self.mounts.items():
+                task_group.spawn(
+                    app,
+                    scope,
+                    self.app_queues[path].get,
+                    partial(self.send, path, send),
+                )
+
+            while True:
+                message = await receive()
+                for queue in self.app_queues.values():
+                    await queue.put(message)
+                if message["type"] == "lifespan.shutdown":
+                    break
+
+    async def send(self, path: str, send: Callable, message: dict) -> None:
+        if message["type"] == "lifespan.startup.complete":
+            self.startup_complete[path] = True
+            if all(self.startup_complete.values()):
+                await send({"type": "lifespan.startup.complete"})
+        elif message["type"] == "lifespan.shutdown.complete":
+            self.shutdown_complete[path] = True
+            if all(self.shutdown_complete.values()):
+                await send({"type": "lifespan.shutdown.complete"})
+
+
+class TrioDispatcherMiddleware(_DispatcherMiddleware):
+    async def _handle_lifespan(self, scope: Scope, receive: Callable, send: Callable) -> None:
+        import trio
+
+        self.app_queues = {path: trio.open_memory_channel(MAX_QUEUE_SIZE) for path in self.mounts}
+        self.startup_complete = {path: False for path in self.mounts}
+        self.shutdown_complete = {path: False for path in self.mounts}
+
+        async with trio.open_nursery() as nursery:
+            for path, app in self.mounts.items():
+                nursery.start_soon(
+                    app,
+                    scope,
+                    self.app_queues[path][1].receive,
+                    partial(self.send, path, send),
+                )
+
+            while True:
+                message = await receive()
+                for channels in self.app_queues.values():
+                    await channels[0].send(message)
+                if message["type"] == "lifespan.shutdown":
+                    break
+
+    async def send(self, path: str, send: Callable, message: dict) -> None:
+        if message["type"] == "lifespan.startup.complete":
+            self.startup_complete[path] = True
+            if all(self.startup_complete.values()):
+                await send({"type": "lifespan.startup.complete"})
+        elif message["type"] == "lifespan.shutdown.complete":
+            self.shutdown_complete[path] = True
+            if all(self.shutdown_complete.values()):
+                await send({"type": "lifespan.shutdown.complete"})
+
+
+DispatcherMiddleware = AsyncioDispatcherMiddleware  # Remove with version 0.11
```

### Comparing `nonecorn-0.14.1.dev1/src/hypercorn/middleware/wsgi.py` & `nonecorn-0.14.3.dev1/src/hypercorn/middleware/wsgi.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,49 @@
-from __future__ import annotations
-
-import asyncio
-from functools import partial
-from typing import Callable, Iterable
-
-from ..app_wrappers import WSGIWrapper
-from ..typing import ASGIReceiveCallable, ASGISendCallable, Scope, WSGIFramework
-
-MAX_BODY_SIZE = 2**16
-
-WSGICallable = Callable[[dict, Callable], Iterable[bytes]]
-
-
-class InvalidPathError(Exception):
-    pass
-
-
-class _WSGIMiddleware:
-    def __init__(self, wsgi_app: WSGIFramework, max_body_size: int = MAX_BODY_SIZE) -> None:
-        self.wsgi_app = WSGIWrapper(wsgi_app, max_body_size)
-        self.max_body_size = max_body_size
-
-    async def __call__(
-        self, scope: Scope, receive: ASGIReceiveCallable, send: ASGISendCallable
-    ) -> None:
-        pass
-
-
-class AsyncioWSGIMiddleware(_WSGIMiddleware):
-    async def __call__(
-        self, scope: Scope, receive: ASGIReceiveCallable, send: ASGISendCallable
-    ) -> None:
-        loop = asyncio.get_event_loop()
-        await self.wsgi_app(scope, receive, send, partial(loop.run_in_executor, None))
-
-
-class TrioWSGIMiddleware(_WSGIMiddleware):
-    async def __call__(
-        self, scope: Scope, receive: ASGIReceiveCallable, send: ASGISendCallable
-    ) -> None:
-        import trio
-
-        await self.wsgi_app(scope, receive, send, trio.to_thread.run_sync)
+from __future__ import annotations
+
+import asyncio
+from functools import partial
+from typing import Any, Callable, Iterable
+
+from ..app_wrappers import WSGIWrapper
+from ..typing import ASGIReceiveCallable, ASGISendCallable, Scope, WSGIFramework
+
+MAX_BODY_SIZE = 2**16
+
+WSGICallable = Callable[[dict, Callable], Iterable[bytes]]
+
+
+class InvalidPathError(Exception):
+    pass
+
+
+class _WSGIMiddleware:
+    def __init__(self, wsgi_app: WSGIFramework, max_body_size: int = MAX_BODY_SIZE) -> None:
+        self.wsgi_app = WSGIWrapper(wsgi_app, max_body_size)
+        self.max_body_size = max_body_size
+
+    async def __call__(
+        self, scope: Scope, receive: ASGIReceiveCallable, send: ASGISendCallable
+    ) -> None:
+        pass
+
+
+class AsyncioWSGIMiddleware(_WSGIMiddleware):
+    async def __call__(
+        self, scope: Scope, receive: ASGIReceiveCallable, send: ASGISendCallable
+    ) -> None:
+        loop = asyncio.get_event_loop()
+
+        def _call_soon(func: Callable, *args: Any) -> Any:
+            future = asyncio.run_coroutine_threadsafe(func(*args), loop)
+            return future.result()
+
+        await self.wsgi_app(scope, receive, send, partial(loop.run_in_executor, None), _call_soon)
+
+
+class TrioWSGIMiddleware(_WSGIMiddleware):
+    async def __call__(
+        self, scope: Scope, receive: ASGIReceiveCallable, send: ASGISendCallable
+    ) -> None:
+        import trio
+
+        await self.wsgi_app(scope, receive, send, trio.to_thread.run_sync, trio.from_thread.run)
```

### Comparing `nonecorn-0.14.1.dev1/src/hypercorn/protocol/__init__.py` & `nonecorn-0.14.3.dev1/src/hypercorn/protocol/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,94 +1,100 @@
-from __future__ import annotations
-
-from typing import Awaitable, Callable, Optional, Tuple, Union
-
-from .h2 import H2Protocol
-from .h11 import H2CProtocolRequiredError, H2ProtocolAssumedError, H11Protocol
-from ..config import Config
-from ..events import Event, RawData
-from ..typing import AppWrapper, TaskGroup, WorkerContext
-
-
-class ProtocolWrapper:
-    def __init__(
-        self,
-        app: AppWrapper,
-        config: Config,
-        context: WorkerContext,
-        task_group: TaskGroup,
-        ssl: bool,
-        client: Optional[Tuple[str, int]],
-        server: Optional[Tuple[str, int]],
-        send: Callable[[Event], Awaitable[None]],
-        alpn_protocol: Optional[str] = None,
-        tls: Optional[dict] = None,
-    ) -> None:
-        self.app = app
-        self.config = config
-        self.context = context
-        self.task_group = task_group
-        self.ssl = ssl
-        self.client = client
-        self.server = server
-        self.send = send
-        self.protocol: Union[H11Protocol, H2Protocol]
-        self.tls = tls
-        if alpn_protocol == "h2":
-            self.protocol = H2Protocol(
-                self.app,
-                self.config,
-                self.context,
-                self.task_group,
-                self.ssl,
-                self.client,
-                self.server,
-                self.send,
-                self.tls,
-            )
-        else:
-            self.protocol = H11Protocol(
-                self.app,
-                self.config,
-                self.context,
-                self.task_group,
-                self.ssl,
-                self.client,
-                self.server,
-                self.send,
-                self.tls,
-            )
-
-    async def initiate(self) -> None:
-        return await self.protocol.initiate()
-
-    async def handle(self, event: Event) -> None:
-        try:
-            return await self.protocol.handle(event)
-        except H2ProtocolAssumedError as error:
-            self.protocol = H2Protocol(
-                self.app,
-                self.config,
-                self.context,
-                self.task_group,
-                self.ssl,
-                self.client,
-                self.server,
-                self.send,
-            )
-            await self.protocol.initiate()
-            if error.data != b"":
-                return await self.protocol.handle(RawData(data=error.data))
-        except H2CProtocolRequiredError as error:
-            self.protocol = H2Protocol(
-                self.app,
-                self.config,
-                self.context,
-                self.task_group,
-                self.ssl,
-                self.client,
-                self.server,
-                self.send,
-            )
-            await self.protocol.initiate(error.headers, error.settings)
-            if error.data != b"":
-                return await self.protocol.handle(RawData(data=error.data))
+from __future__ import annotations
+
+from typing import Awaitable, Callable, Optional, Tuple, Union, Dict, Any
+
+from .h2 import H2Protocol
+from .h11 import H2CProtocolRequiredError, H2ProtocolAssumedError, H11Protocol
+from ..config import Config
+from ..events import Event, RawData
+from ..typing import AppWrapper, TaskGroup, WorkerContext
+
+
+class ProtocolWrapper:
+    def __init__(
+        self,
+        app: AppWrapper,
+        config: Config,
+        context: WorkerContext,
+        task_group: TaskGroup,
+        ssl: bool,
+        client: Optional[Tuple[str, int]],
+        server: Optional[Tuple[str, int]],
+        send: Callable[[Event], Awaitable[None]],
+        alpn_protocol: Optional[str] = None,
+        tls: Optional[dict] = None,
+        app_state: Dict[str, Any] = None,
+    ) -> None:
+        self.app = app
+        self.config = config
+        self.context = context
+        self.task_group = task_group
+        self.ssl = ssl
+        self.client = client
+        self.server = server
+        self.send = send
+        self.protocol: Union[H11Protocol, H2Protocol]
+        self.tls = tls
+        self.app_state = app_state
+        if alpn_protocol == "h2":
+            self.protocol = H2Protocol(
+                self.app,
+                self.config,
+                self.context,
+                self.task_group,
+                self.ssl,
+                self.client,
+                self.server,
+                self.send,
+                self.tls,
+                self.app_state,
+            )
+        else:
+            self.protocol = H11Protocol(
+                self.app,
+                self.config,
+                self.context,
+                self.task_group,
+                self.ssl,
+                self.client,
+                self.server,
+                self.send,
+                self.tls,
+                self.app_state,
+            )
+
+    async def initiate(self) -> None:
+        return await self.protocol.initiate()
+
+    async def handle(self, event: Event) -> None:
+        try:
+            return await self.protocol.handle(event)
+        except H2ProtocolAssumedError as error:
+            self.protocol = H2Protocol(
+                self.app,
+                self.config,
+                self.context,
+                self.task_group,
+                self.ssl,
+                self.client,
+                self.server,
+                self.send,
+                self.app_state,
+            )
+            await self.protocol.initiate()
+            if error.data != b"":
+                return await self.protocol.handle(RawData(data=error.data))
+        except H2CProtocolRequiredError as error:
+            self.protocol = H2Protocol(
+                self.app,
+                self.config,
+                self.context,
+                self.task_group,
+                self.ssl,
+                self.client,
+                self.server,
+                self.send,
+                self.app_state,
+            )
+            await self.protocol.initiate(error.headers, error.settings)
+            if error.data != b"":
+                return await self.protocol.handle(RawData(data=error.data))
```

### Comparing `nonecorn-0.14.1.dev1/src/hypercorn/protocol/http_stream.py` & `nonecorn-0.14.3.dev1/src/hypercorn/protocol/http_stream.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,316 +1,307 @@
-from __future__ import annotations
-
-import asyncio
-from enum import auto, Enum
-from time import time
-from typing import Awaitable, Callable, Optional, Tuple
-from urllib.parse import unquote
-
-from .events import (
-    Body,
-    EndBody,
-    Event,
-    InformationalResponse,
-    Request,
-    Response,
-    StreamClosed,
-    TrailerHeadersSend,
-    ZeroCopySend,
-)
-from ..config import Config
-from ..typing import (
-    AppWrapper,
-    ASGISendEvent,
-    HTTPResponseStartEvent,
-    HTTPScope,
-    TaskGroup,
-    WorkerContext,
-)
-from ..utils import (
-    build_and_validate_headers,
-    can_sendfile,
-    suppress_body,
-    UnexpectedMessageError,
-    valid_server_name,
-)
-
-PUSH_VERSIONS = {"2", "3"}
-EARLY_HINTS_VERSIONS = {"2", "3"}
-
-
-class ASGIHTTPState(Enum):
-    # The ASGI Spec is clear that a response should not start till the
-    # framework has sent at least one body message hence why this
-    # state tracking is required.
-    REQUEST = auto()
-    RESPONSE = auto()
-    CLOSED = auto()
-
-
-class HTTPStream:
-    def __init__(
-        self,
-        app: AppWrapper,
-        config: Config,
-        context: WorkerContext,
-        task_group: TaskGroup,
-        ssl: bool,
-        client: Optional[Tuple[str, int]],
-        server: Optional[Tuple[str, int]],
-        send: Callable[[Event], Awaitable[None]],
-        stream_id: int,
-        tls: Optional[dict] = None,
-    ) -> None:
-        self.app = app
-        self.client = client
-        self.closed = False
-        self.config = config
-        self.context = context
-        self.response: HTTPResponseStartEvent
-        self.scope: HTTPScope
-        self.send = send
-        self.scheme = "https" if ssl else "http"
-        self.server = server
-        self.start_time: float
-        self.state = ASGIHTTPState.REQUEST
-        self.stream_id = stream_id
-        self.task_group = task_group
-        self.tls = tls
-
-    @property
-    def idle(self) -> bool:
-        return False
-
-    async def handle(self, event: Event) -> None:
-        if self.closed:
-            return
-        elif isinstance(event, Request):
-            self.start_time = time()
-            path, _, query_string = event.raw_path.partition(b"?")
-            self.scope = {
-                "type": "http",
-                "http_version": event.http_version,
-                "asgi": {"spec_version": "2.1", "version": "3.0"},
-                "method": event.method,
-                "scheme": self.scheme,
-                "path": unquote(path.decode("ascii")),
-                "raw_path": path,
-                "query_string": query_string,
-                "root_path": self.config.root_path,
-                "headers": event.headers,
-                "client": self.client,
-                "server": self.server,
-                "extensions": {},
-            }
-            self.scope["extensions"]["http.response.trailers"] = {}
-            if event.http_version in PUSH_VERSIONS:
-                self.scope["extensions"]["http.response.push"] = {}
-            if (
-                can_sendfile(asyncio.get_event_loop(), self.scheme == "https")
-                and event.http_version not in PUSH_VERSIONS
-            ):
-                self.scope["extensions"]["http.response.zerocopysend"] = {}
-            if self.scheme == "https" and self.tls:
-                self.scope["extensions"]["tls"] = self.tls
-
-            if event.http_version in EARLY_HINTS_VERSIONS:
-                self.scope["extensions"]["http.response.early_hint"] = {}
-
-            if valid_server_name(self.config, event):
-                self.app_put = await self.task_group.spawn_app(
-                    self.app, self.config, self.scope, self.app_send
-                )
-            else:
-                await self._send_error_response(404)
-                self.closed = True
-
-        elif isinstance(event, Body):
-            await self.app_put(
-                {"type": "http.request", "body": bytes(event.data), "more_body": True}
-            )
-        elif isinstance(event, EndBody):
-            await self.app_put({"type": "http.request", "body": b"", "more_body": False})
-        elif isinstance(event, StreamClosed):
-            self.closed = True
-            if self.app_put is not None:
-                await self.app_put({"type": "http.disconnect"})  # type: ignore
-
-    async def app_send(self, message: Optional[ASGISendEvent]) -> None:
-        if self.closed:
-            # Allow app to finish after close
-            return
-
-        if message is None:  # ASGI App has finished sending messages
-            # Cleanup if required
-            if self.state == ASGIHTTPState.REQUEST:
-                await self._send_error_response(500)
-            await self.send(StreamClosed(stream_id=self.stream_id))
-        else:
-            if message["type"] == "http.response.start" and self.state == ASGIHTTPState.REQUEST:
-                self.response = message
-            elif (
-                message["type"] == "http.response.push"
-                and self.scope["http_version"] in PUSH_VERSIONS
-            ):
-                if not isinstance(message["path"], str):
-                    raise TypeError(f"{message['path']} should be a str")
-                headers = [(b":scheme", self.scope["scheme"].encode())]
-                for name, value in self.scope["headers"]:
-                    if name == b"host":
-                        headers.append((b":authority", value))
-                headers.extend(build_and_validate_headers(message["headers"]))
-                await self.send(
-                    Request(
-                        stream_id=self.stream_id,
-                        headers=headers,
-                        http_version=self.scope["http_version"],
-                        method="GET",
-                        raw_path=message["path"].encode(),
-                    )
-                )
-            elif (
-                message["type"] == "http.response.early_hint"
-                and self.scope["http_version"] in EARLY_HINTS_VERSIONS
-                and self.state == ASGIHTTPState.REQUEST
-            ):
-                headers = [(b"link", bytes(link).strip()) for link in message["links"]]
-                await self.send(
-                    InformationalResponse(
-                        stream_id=self.stream_id,
-                        headers=headers,
-                        status_code=103,
-                    )
-                )
-            elif message["type"] == "http.response.body" and self.state in {
-                ASGIHTTPState.REQUEST,
-                ASGIHTTPState.RESPONSE,
-            }:
-                if self.state == ASGIHTTPState.REQUEST:
-                    headers = build_and_validate_headers(self.response.get("headers", []))
-                    reason = (
-                        self.response["meta"].get("reason", "") if "meta" in self.response else ""
-                    )
-                    await self.send(
-                        Response(
-                            stream_id=self.stream_id,
-                            headers=headers,
-                            status_code=int(self.response["status"]),
-                            reason=reason,
-                        )
-                    )
-                    self.state = ASGIHTTPState.RESPONSE
-
-                if (
-                    not suppress_body(self.scope["method"], int(self.response["status"]))
-                    and message.get("body", b"") != b""
-                ):
-                    await self.send(
-                        Body(
-                            stream_id=self.stream_id,
-                            data=bytes(message.get("body", b"")),
-                            flush=message["meta"].get("flush", False)
-                            if "meta" in message
-                            else False,
-                        )
-                    )
-
-                if not message.get("more_body", False):
-                    if self.state != ASGIHTTPState.CLOSED:
-                        self.state = ASGIHTTPState.CLOSED
-                        await self.config.log.access(
-                            self.scope, self.response, time() - self.start_time
-                        )
-                        await self.send(
-                            EndBody(
-                                stream_id=self.stream_id,
-                                headers=message["meta"].get("headers", [])
-                                if "meta" in message
-                                else [],
-                            )
-                        )
-                        await self.send(StreamClosed(stream_id=self.stream_id))
-            elif message["type"] == "http.response.zerocopysend" and self.state in {
-                ASGIHTTPState.REQUEST,
-                ASGIHTTPState.RESPONSE,
-            }:
-                if self.state == ASGIHTTPState.REQUEST:
-                    headers = build_and_validate_headers(self.response.get("headers", []))
-                    reason = (
-                        self.response["meta"].get("reason", "") if "meta" in self.response else ""
-                    )
-                    await self.send(
-                        Response(
-                            stream_id=self.stream_id,
-                            headers=headers,
-                            status_code=int(self.response["status"]),
-                            reason=reason,
-                        )
-                    )
-                    self.state = ASGIHTTPState.RESPONSE
-
-                if (
-                    not suppress_body(self.scope["method"], int(self.response["status"]))
-                    and message.get("file") is not None
-                ):
-                    await self.send(
-                        ZeroCopySend(
-                            stream_id=self.stream_id,
-                            file=message.get("file"),
-                            offset=message.get("offset"),
-                            count=message.get("count"),
-                        )
-                    )
-
-                if not message.get("more_body", False):
-                    if self.state != ASGIHTTPState.CLOSED:
-                        self.state = ASGIHTTPState.CLOSED
-                        await self.config.log.access(
-                            self.scope, self.response, time() - self.start_time
-                        )
-                        await self.send(
-                            EndBody(
-                                stream_id=self.stream_id,
-                                headers=message["meta"].get("headers") if "meta" in message else [],
-                            )
-                        )
-                        await self.send(StreamClosed(stream_id=self.stream_id))
-            elif message["type"] == "http.response.trailers" and self.state in {
-                ASGIHTTPState.REQUEST,
-                ASGIHTTPState.RESPONSE,
-            }:
-                headers = message.get("headers", [])
-                more_body = message.get("more_body", False)
-                if not more_body:
-                    await self.config.log.access(
-                        self.scope, self.response, time() - self.start_time
-                    )
-                await self.send(
-                    TrailerHeadersSend(
-                        stream_id=self.stream_id, headers=headers, end_stream=not more_body
-                    )
-                )
-                if not more_body:
-                    if self.scope["http_version"] == "2":
-                        await self.send(
-                            EndBody(
-                                stream_id=self.stream_id,
-                                headers=[],
-                            )
-                        )
-                    await self.send(StreamClosed(stream_id=self.stream_id))
-            else:
-                raise UnexpectedMessageError(self.state, message["type"])
-
-    async def _send_error_response(self, status_code: int) -> None:
-        await self.send(
-            Response(
-                stream_id=self.stream_id,
-                headers=[(b"content-length", b"0"), (b"connection", b"close")],
-                status_code=status_code,
-            )
-        )
-        await self.send(EndBody(stream_id=self.stream_id))
-        self.state = ASGIHTTPState.CLOSED
-        await self.config.log.access(
-            self.scope, {"status": status_code, "headers": []}, time() - self.start_time
-        )
+from __future__ import annotations
+
+import asyncio
+from enum import auto, Enum
+from time import time
+from typing import Awaitable, Callable, Optional, Tuple, Dict, Any
+from urllib.parse import unquote
+
+from .events import (
+    Body,
+    EndBody,
+    Event,
+    InformationalResponse,
+    Request,
+    Response,
+    StreamClosed,
+    TrailerHeadersSend,
+    ZeroCopySend,
+)
+from ..config import Config
+from ..typing import (
+    AppWrapper,
+    ASGISendEvent,
+    HTTPResponseStartEvent,
+    HTTPScope,
+    TaskGroup,
+    WorkerContext,
+)
+from ..utils import (
+    build_and_validate_headers,
+    can_sendfile,
+    suppress_body,
+    UnexpectedMessageError,
+    valid_server_name,
+)
+
+PUSH_VERSIONS = {"2", "3"}
+EARLY_HINTS_VERSIONS = {"2", "3"}
+
+
+class ASGIHTTPState(Enum):
+    # The ASGI Spec is clear that a response should not start till the
+    # framework has sent at least one body message hence why this
+    # state tracking is required.
+    REQUEST = auto()
+    RESPONSE = auto()
+    CLOSED = auto()
+
+
+class HTTPStream:
+    def __init__(
+        self,
+        app: AppWrapper,
+        config: Config,
+        context: WorkerContext,
+        task_group: TaskGroup,
+        ssl: bool,
+        client: Optional[Tuple[str, int]],
+        server: Optional[Tuple[str, int]],
+        send: Callable[[Event], Awaitable[None]],
+        stream_id: int,
+        tls: Optional[dict] = None,
+        app_state: Optional[Dict[str, Any]] = None,
+    ) -> None:
+        self.app = app
+        self.client = client
+        self.closed = False
+        self.config = config
+        self.context = context
+        self.response: HTTPResponseStartEvent
+        self.scope: HTTPScope
+        self.send = send
+        self.scheme = "https" if ssl else "http"
+        self.server = server
+        self.start_time: float
+        self.state = ASGIHTTPState.REQUEST
+        self.stream_id = stream_id
+        self.task_group = task_group
+        self.tls = tls
+        self.trailers_expected: bool = False
+        self.app_state = app_state
+
+    @property
+    def idle(self) -> bool:
+        return False
+
+    async def handle(self, event: Event) -> None:
+        if self.closed:
+            return
+        elif isinstance(event, Request):
+            self.start_time = time()
+            path, _, query_string = event.raw_path.partition(b"?")
+            self.scope = {
+                "type": "http",
+                "http_version": event.http_version,
+                "asgi": {"spec_version": "2.1", "version": "3.0"},
+                "method": event.method,
+                "scheme": self.scheme,
+                "path": unquote(path.decode("ascii")),
+                "raw_path": path,
+                "query_string": query_string,
+                "root_path": self.config.root_path,
+                "headers": event.headers,
+                "client": self.client,
+                "server": self.server,
+                "extensions": {},
+                "state": self.app_state,
+            }
+            self.scope["extensions"]["http.response.trailers"] = {}
+            if event.http_version in PUSH_VERSIONS:
+                self.scope["extensions"]["http.response.push"] = {}
+            if (
+                can_sendfile(asyncio.get_event_loop(), self.scheme == "https")
+                and event.http_version not in PUSH_VERSIONS
+            ):
+                self.scope["extensions"]["http.response.zerocopysend"] = {}
+            if self.scheme == "https" and self.tls:
+                self.scope["extensions"]["tls"] = self.tls
+
+            if event.http_version in EARLY_HINTS_VERSIONS:
+                self.scope["extensions"]["http.response.early_hint"] = {}
+
+            if valid_server_name(self.config, event):
+                self.app_put = await self.task_group.spawn_app(
+                    self.app, self.config, self.scope, self.app_send
+                )
+            else:
+                await self._send_error_response(404)
+                self.closed = True
+
+        elif isinstance(event, Body):
+            await self.app_put(
+                {"type": "http.request", "body": bytes(event.data), "more_body": True}
+            )
+        elif isinstance(event, EndBody):
+            await self.app_put({"type": "http.request", "body": b"", "more_body": False})
+        elif isinstance(event, StreamClosed):
+            self.closed = True
+            if self.app_put is not None:
+                await self.app_put({"type": "http.disconnect"})  # type: ignore
+
+    async def app_send(self, message: Optional[ASGISendEvent]) -> None:
+        if self.closed:
+            # Allow app to finish after close
+            return
+
+        if message is None:  # ASGI App has finished sending messages
+            # Cleanup if required
+            if self.state == ASGIHTTPState.REQUEST:
+                await self._send_error_response(500)
+            await self.send(StreamClosed(stream_id=self.stream_id))
+        else:
+            if message["type"] == "http.response.start" and self.state == ASGIHTTPState.REQUEST:
+                self.response = message
+                self.trailers_expected = message.get("trailers", False)
+            elif (
+                message["type"] == "http.response.push"
+                and self.scope["http_version"] in PUSH_VERSIONS
+            ):
+                if not isinstance(message["path"], str):
+                    raise TypeError(f"{message['path']} should be a str")
+                headers = [(b":scheme", self.scope["scheme"].encode())]
+                for name, value in self.scope["headers"]:
+                    if name == b"host":
+                        headers.append((b":authority", value))
+                headers.extend(build_and_validate_headers(message["headers"]))
+                await self.send(
+                    Request(
+                        stream_id=self.stream_id,
+                        headers=headers,
+                        http_version=self.scope["http_version"],
+                        method="GET",
+                        raw_path=message["path"].encode(),
+                    )
+                )
+            elif (
+                message["type"] == "http.response.early_hint"
+                and self.scope["http_version"] in EARLY_HINTS_VERSIONS
+                and self.state == ASGIHTTPState.REQUEST
+            ):
+                headers = [(b"link", bytes(link).strip()) for link in message["links"]]
+                await self.send(
+                    InformationalResponse(
+                        stream_id=self.stream_id,
+                        headers=headers,
+                        status_code=103,
+                    )
+                )
+            elif message["type"] == "http.response.body" and self.state in {
+                ASGIHTTPState.REQUEST,
+                ASGIHTTPState.RESPONSE,
+            }:
+                if self.state == ASGIHTTPState.REQUEST:
+                    headers = build_and_validate_headers(self.response.get("headers", []))
+                    reason = self.response.get("reason", "")
+                    await self.send(
+                        Response(
+                            stream_id=self.stream_id,
+                            headers=headers,
+                            status_code=int(self.response["status"]),
+                            reason=reason,
+                        )
+                    )
+                    self.state = ASGIHTTPState.RESPONSE
+
+                if (
+                    not suppress_body(self.scope["method"], int(self.response["status"]))
+                    and message.get("body", b"") != b""
+                ):
+                    await self.send(
+                        Body(
+                            stream_id=self.stream_id,
+                            data=bytes(message.get("body", b"")),
+                            flush=message.get("flush", False) or self.trailers_expected,
+                        )
+                    )
+
+                if not message.get("more_body", False) and not self.trailers_expected:
+                    if self.state != ASGIHTTPState.CLOSED:
+                        self.state = ASGIHTTPState.CLOSED
+                        await self.config.log.access(
+                            self.scope, self.response, time() - self.start_time
+                        )
+                        await self.send(
+                            EndBody(stream_id=self.stream_id, headers=message.get("headers", []))
+                        )
+                        await self.send(StreamClosed(stream_id=self.stream_id))
+            elif message["type"] == "http.response.zerocopysend" and self.state in {
+                ASGIHTTPState.REQUEST,
+                ASGIHTTPState.RESPONSE,
+            }:
+                if self.state == ASGIHTTPState.REQUEST:
+                    headers = build_and_validate_headers(self.response.get("headers", []))
+                    reason = self.response.get("reason", "")
+                    await self.send(
+                        Response(
+                            stream_id=self.stream_id,
+                            headers=headers,
+                            status_code=int(self.response["status"]),
+                            reason=reason,
+                        )
+                    )
+                    self.state = ASGIHTTPState.RESPONSE
+
+                if (
+                    not suppress_body(self.scope["method"], int(self.response["status"]))
+                    and message.get("file") is not None
+                ):
+                    await self.send(
+                        ZeroCopySend(
+                            stream_id=self.stream_id,
+                            file=message.get("file"),
+                            offset=message.get("offset"),
+                            count=message.get("count"),
+                        )
+                    )
+
+                if not message.get("more_body", False) and not self.trailers_expected:
+                    if self.state != ASGIHTTPState.CLOSED:
+                        self.state = ASGIHTTPState.CLOSED
+                        await self.config.log.access(
+                            self.scope, self.response, time() - self.start_time
+                        )
+                        await self.send(
+                            EndBody(stream_id=self.stream_id, headers=message.get("headers", []))
+                        )
+                        await self.send(StreamClosed(stream_id=self.stream_id))
+            elif message["type"] == "http.response.trailers" and self.state in {
+                ASGIHTTPState.REQUEST,
+                ASGIHTTPState.RESPONSE,
+            }:
+                headers = message.get("headers", [])
+                more_trailers = message.get("more_trailers", False)
+                if not more_trailers:
+                    await self.config.log.access(
+                        self.scope, self.response, time() - self.start_time
+                    )
+                await self.send(
+                    TrailerHeadersSend(
+                        stream_id=self.stream_id, headers=headers, end_stream=not more_trailers
+                    )
+                )
+                if not more_trailers:
+                    if self.scope["http_version"] == "2":
+                        await self.send(
+                            EndBody(
+                                stream_id=self.stream_id,
+                                headers=[],
+                            )
+                        )
+                    await self.send(StreamClosed(stream_id=self.stream_id))
+            else:
+                raise UnexpectedMessageError(self.state, message["type"])
+
+    async def _send_error_response(self, status_code: int) -> None:
+        await self.send(
+            Response(
+                stream_id=self.stream_id,
+                headers=[(b"content-length", b"0"), (b"connection", b"close")],
+                status_code=status_code,
+            )
+        )
+        await self.send(EndBody(stream_id=self.stream_id))
+        self.state = ASGIHTTPState.CLOSED
+        await self.config.log.access(
+            self.scope, {"status": status_code, "headers": []}, time() - self.start_time
+        )
```

### Comparing `nonecorn-0.14.1.dev1/src/hypercorn/protocol/quic.py` & `nonecorn-0.14.3.dev1/src/hypercorn/protocol/quic.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,135 +1,138 @@
-from __future__ import annotations
-
-from functools import partial
-from typing import Awaitable, Callable, Dict, Optional, Tuple
-
-from aioquic.buffer import Buffer
-from aioquic.h3.connection import H3_ALPN
-from aioquic.quic.configuration import QuicConfiguration
-from aioquic.quic.connection import QuicConnection
-from aioquic.quic.events import (
-    ConnectionIdIssued,
-    ConnectionIdRetired,
-    ConnectionTerminated,
-    ProtocolNegotiated,
-)
-from aioquic.quic.packet import (
-    encode_quic_version_negotiation,
-    PACKET_TYPE_INITIAL,
-    pull_quic_header,
-)
-
-from .h3 import H3Protocol
-from ..config import Config
-from ..events import Closed, Event, RawData
-from ..typing import AppWrapper, TaskGroup, WorkerContext
-
-
-class QuicProtocol:
-    def __init__(
-        self,
-        app: AppWrapper,
-        config: Config,
-        context: WorkerContext,
-        task_group: TaskGroup,
-        server: Optional[Tuple[str, int]],
-        send: Callable[[Event], Awaitable[None]],
-    ) -> None:
-        self.app = app
-        self.config = config
-        self.context = context
-        self.connections: Dict[bytes, QuicConnection] = {}
-        self.http_connections: Dict[QuicConnection, H3Protocol] = {}
-        self.send = send
-        self.server = server
-        self.task_group = task_group
-
-        self.quic_config = QuicConfiguration(alpn_protocols=H3_ALPN, is_client=False)
-        self.quic_config.load_cert_chain(certfile=config.certfile, keyfile=config.keyfile)
-
-    @property
-    def idle(self) -> bool:
-        return len(self.connections) == 0 and len(self.http_connections) == 0
-
-    async def handle(self, event: Event) -> None:
-        if isinstance(event, RawData):
-            try:
-                header = pull_quic_header(Buffer(data=event.data), host_cid_length=8)
-            except ValueError:
-                return
-            if (
-                header.version is not None
-                and header.version not in self.quic_config.supported_versions
-            ):
-                data = encode_quic_version_negotiation(
-                    source_cid=header.destination_cid,
-                    destination_cid=header.source_cid,
-                    supported_versions=self.quic_config.supported_versions,
-                )
-                await self.send(RawData(data=data, address=event.address))
-                return
-
-            connection = self.connections.get(header.destination_cid)
-            if (
-                connection is None
-                and len(event.data) >= 1200
-                and header.packet_type == PACKET_TYPE_INITIAL
-                and not self.context.terminated.is_set()
-            ):
-                connection = QuicConnection(
-                    configuration=self.quic_config,
-                    original_destination_connection_id=header.destination_cid,
-                )
-                self.connections[header.destination_cid] = connection
-                self.connections[connection.host_cid] = connection
-
-            if connection is not None:
-                connection.receive_datagram(event.data, event.address, now=self.context.time())
-                await self._handle_events(connection, event.address)
-        elif isinstance(event, Closed):
-            pass
-
-    async def send_all(self, connection: QuicConnection) -> None:
-        for data, address in connection.datagrams_to_send(now=self.context.time()):
-            await self.send(RawData(data=data, address=address))
-
-    async def _handle_events(
-        self, connection: QuicConnection, client: Optional[Tuple[str, int]] = None
-    ) -> None:
-        event = connection.next_event()
-        while event is not None:
-            if isinstance(event, ConnectionTerminated):
-                pass
-            elif isinstance(event, ProtocolNegotiated):
-                self.http_connections[connection] = H3Protocol(
-                    self.app,
-                    self.config,
-                    self.context,
-                    self.task_group,
-                    client,
-                    self.server,
-                    connection,
-                    partial(self.send_all, connection),
-                )
-            elif isinstance(event, ConnectionIdIssued):
-                self.connections[event.connection_id] = connection
-            elif isinstance(event, ConnectionIdRetired):
-                del self.connections[event.connection_id]
-
-            if connection in self.http_connections:
-                await self.http_connections[connection].handle(event)
-
-            event = connection.next_event()
-
-        await self.send_all(connection)
-
-        timer = connection.get_timer()
-        if timer is not None:
-            self.task_group.spawn(self._handle_timer, timer, connection)
-
-    async def _handle_timer(self, timer: float, connection: QuicConnection) -> None:
-        wait = max(0, timer - self.context.time())
-        await self.context.sleep(wait)
-        if connection._close_at is not None:
-            connection.handle_timer(now=self.context.time())
-            await self._handle_events(connection, None)
+from __future__ import annotations
+
+from functools import partial
+from typing import Awaitable, Callable, Dict, Optional, Tuple, Any
+
+from aioquic.buffer import Buffer
+from aioquic.h3.connection import H3_ALPN
+from aioquic.quic.configuration import QuicConfiguration
+from aioquic.quic.connection import QuicConnection
+from aioquic.quic.events import (
+    ConnectionIdIssued,
+    ConnectionIdRetired,
+    ConnectionTerminated,
+    ProtocolNegotiated,
+)
+from aioquic.quic.packet import (
+    encode_quic_version_negotiation,
+    PACKET_TYPE_INITIAL,
+    pull_quic_header,
+)
+
+from .h3 import H3Protocol
+from ..config import Config
+from ..events import Closed, Event, RawData
+from ..typing import AppWrapper, TaskGroup, WorkerContext
+
+
+class QuicProtocol:
+    def __init__(
+        self,
+        app: AppWrapper,
+        config: Config,
+        context: WorkerContext,
+        task_group: TaskGroup,
+        server: Optional[Tuple[str, int]],
+        send: Callable[[Event], Awaitable[None]],
+        app_state: Dict[str, Any],
+    ) -> None:
+        self.app = app
+        self.config = config
+        self.context = context
+        self.connections: Dict[bytes, QuicConnection] = {}
+        self.http_connections: Dict[QuicConnection, H3Protocol] = {}
+        self.send = send
+        self.server = server
+        self.task_group = task_group
+
+        self.quic_config = QuicConfiguration(alpn_protocols=H3_ALPN, is_client=False)
+        self.quic_config.load_cert_chain(certfile=config.certfile, keyfile=config.keyfile)
+        self.app_state = app_state
+
+    @property
+    def idle(self) -> bool:
+        return len(self.connections) == 0 and len(self.http_connections) == 0
+
+    async def handle(self, event: Event) -> None:
+        if isinstance(event, RawData):
+            try:
+                header = pull_quic_header(Buffer(data=event.data), host_cid_length=8)
+            except ValueError:
+                return
+            if (
+                header.version is not None
+                and header.version not in self.quic_config.supported_versions
+            ):
+                data = encode_quic_version_negotiation(
+                    source_cid=header.destination_cid,
+                    destination_cid=header.source_cid,
+                    supported_versions=self.quic_config.supported_versions,
+                )
+                await self.send(RawData(data=data, address=event.address))
+                return
+
+            connection = self.connections.get(header.destination_cid)
+            if (
+                connection is None
+                and len(event.data) >= 1200
+                and header.packet_type == PACKET_TYPE_INITIAL
+                and not self.context.terminated.is_set()
+            ):
+                connection = QuicConnection(
+                    configuration=self.quic_config,
+                    original_destination_connection_id=header.destination_cid,
+                )
+                self.connections[header.destination_cid] = connection
+                self.connections[connection.host_cid] = connection
+
+            if connection is not None:
+                connection.receive_datagram(event.data, event.address, now=self.context.time())
+                await self._handle_events(connection, event.address)
+        elif isinstance(event, Closed):
+            pass
+
+    async def send_all(self, connection: QuicConnection) -> None:
+        for data, address in connection.datagrams_to_send(now=self.context.time()):
+            await self.send(RawData(data=data, address=address))
+
+    async def _handle_events(
+        self, connection: QuicConnection, client: Optional[Tuple[str, int]] = None
+    ) -> None:
+        event = connection.next_event()
+        while event is not None:
+            if isinstance(event, ConnectionTerminated):
+                pass
+            elif isinstance(event, ProtocolNegotiated):
+                self.http_connections[connection] = H3Protocol(
+                    self.app,
+                    self.config,
+                    self.context,
+                    self.task_group,
+                    client,
+                    self.server,
+                    connection,
+                    partial(self.send_all, connection),
+                    self.app_state,
+                )
+            elif isinstance(event, ConnectionIdIssued):
+                self.connections[event.connection_id] = connection
+            elif isinstance(event, ConnectionIdRetired):
+                del self.connections[event.connection_id]
+
+            if connection in self.http_connections:
+                await self.http_connections[connection].handle(event)
+
+            event = connection.next_event()
+
+        await self.send_all(connection)
+
+        timer = connection.get_timer()
+        if timer is not None:
+            self.task_group.spawn(self._handle_timer, timer, connection)
+
+    async def _handle_timer(self, timer: float, connection: QuicConnection) -> None:
+        wait = max(0, timer - self.context.time())
+        await self.context.sleep(wait)
+        if connection._close_at is not None:
+            connection.handle_timer(now=self.context.time())
+            await self._handle_events(connection, None)
```

### Comparing `nonecorn-0.14.1.dev1/src/hypercorn/protocol/ws_stream.py` & `nonecorn-0.14.3.dev1/src/hypercorn/protocol/ws_stream.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,391 +1,394 @@
-from __future__ import annotations
-
-from enum import auto, Enum
-from io import BytesIO, StringIO
-from time import time
-from typing import Awaitable, Callable, Iterable, List, Optional, Tuple, Union
-from urllib.parse import unquote
-
-from wsproto.connection import Connection, ConnectionState, ConnectionType
-from wsproto.events import (
-    BytesMessage,
-    CloseConnection,
-    Event as WSProtoEvent,
-    Message,
-    Ping,
-    TextMessage,
-)
-from wsproto.extensions import Extension, PerMessageDeflate
-from wsproto.frame_protocol import CloseReason
-from wsproto.handshake import server_extensions_handshake, WEBSOCKET_VERSION
-from wsproto.utilities import generate_accept_token, split_comma_header
-
-from .events import Body, Data, EndBody, EndData, Event, Request, Response, StreamClosed
-from ..config import Config
-from ..typing import (
-    AppWrapper,
-    ASGISendEvent,
-    TaskGroup,
-    WebsocketAcceptEvent,
-    WebsocketResponseBodyEvent,
-    WebsocketResponseStartEvent,
-    WebsocketScope,
-    WorkerContext,
-)
-from ..utils import (
-    build_and_validate_headers,
-    suppress_body,
-    UnexpectedMessageError,
-    valid_server_name,
-)
-
-
-class ASGIWebsocketState(Enum):
-    # Hypercorn supports the ASGI websocket HTTP response extension,
-    # which allows HTTP responses rather than acceptance.
-    HANDSHAKE = auto()
-    CONNECTED = auto()
-    RESPONSE = auto()
-    CLOSED = auto()
-    HTTPCLOSED = auto()
-
-
-class FrameTooLargeError(Exception):
-    pass
-
-
-class Handshake:
-    def __init__(self, headers: List[Tuple[bytes, bytes]], http_version: str) -> None:
-        self.http_version = http_version
-        self.connection_tokens: Optional[List[str]] = None
-        self.extensions: Optional[List[str]] = None
-        self.key: Optional[bytes] = None
-        self.subprotocols: Optional[List[str]] = None
-        self.upgrade: Optional[bytes] = None
-        self.version: Optional[bytes] = None
-        for name, value in headers:
-            name = name.lower()
-            if name == b"connection":
-                self.connection_tokens = split_comma_header(value)
-            elif name == b"sec-websocket-extensions":
-                self.extensions = split_comma_header(value)
-            elif name == b"sec-websocket-key":
-                self.key = value
-            elif name == b"sec-websocket-protocol":
-                self.subprotocols = split_comma_header(value)
-            elif name == b"sec-websocket-version":
-                self.version = value
-            elif name == b"upgrade":
-                self.upgrade = value
-
-    def is_valid(self) -> bool:
-        if self.http_version < "1.1":
-            return False
-        elif self.http_version == "1.1":
-            if self.key is None:
-                return False
-            if self.connection_tokens is None or not any(
-                token.lower() == "upgrade" for token in self.connection_tokens
-            ):
-                return False
-            if self.upgrade.lower() != b"websocket":
-                return False
-
-        if self.version != WEBSOCKET_VERSION:
-            return False
-        return True
-
-    def accept(
-        self,
-        subprotocol: Optional[str],
-        additional_headers: Iterable[Tuple[bytes, bytes]],
-    ) -> Tuple[int, List[Tuple[bytes, bytes]], Connection]:
-        headers = []
-        if subprotocol is not None:
-            if subprotocol not in self.subprotocols:
-                raise Exception("Invalid Subprotocol")
-            else:
-                headers.append((b"sec-websocket-protocol", subprotocol.encode()))
-
-        extensions: List[Extension] = [PerMessageDeflate()]
-        accepts = None
-        if self.extensions is not None:
-            accepts = server_extensions_handshake(self.extensions, extensions)
-
-        if accepts:
-            headers.append((b"sec-websocket-extensions", accepts))
-
-        if self.key is not None:
-            headers.append((b"sec-websocket-accept", generate_accept_token(self.key)))
-
-        status_code = 200
-        if self.http_version == "1.1":
-            headers.extend([(b"upgrade", b"WebSocket"), (b"connection", b"Upgrade")])
-            status_code = 101
-
-        for name, value in additional_headers:
-            if b"sec-websocket-protocol" == name or name.startswith(b":"):
-                raise Exception(f"Invalid additional header, {name.decode()}")
-
-            headers.append((name, value))
-
-        return status_code, headers, Connection(ConnectionType.SERVER, extensions)
-
-
-class WebsocketBuffer:
-    def __init__(self, max_length: int) -> None:
-        self.value: Optional[Union[BytesIO, StringIO]] = None
-        self.length = 0
-        self.max_length = max_length
-
-    def extend(self, event: Message) -> None:
-        if self.value is None:
-            if isinstance(event, TextMessage):
-                self.value = StringIO()
-            else:
-                self.value = BytesIO()
-        self.length += self.value.write(event.data)
-        if self.length > self.max_length:
-            raise FrameTooLargeError()
-
-    def clear(self) -> None:
-        self.value = None
-        self.length = 0
-
-    def to_message(self) -> dict:
-        return {
-            "type": "websocket.receive",
-            "bytes": self.value.getvalue() if isinstance(self.value, BytesIO) else None,
-            "text": self.value.getvalue() if isinstance(self.value, StringIO) else None,
-        }
-
-
-class WSStream:
-    def __init__(
-        self,
-        app: AppWrapper,
-        config: Config,
-        context: WorkerContext,
-        task_group: TaskGroup,
-        ssl: bool,
-        client: Optional[Tuple[str, int]],
-        server: Optional[Tuple[str, int]],
-        send: Callable[[Event], Awaitable[None]],
-        stream_id: int,
-        tls: Optional[dict] = None,
-    ) -> None:
-        self.app = app
-        self.app_put: Optional[Callable] = None
-        self.buffer = WebsocketBuffer(config.websocket_max_message_size)
-        self.client = client
-        self.closed = False
-        self.config = config
-        self.context = context
-        self.task_group = task_group
-        self.response: WebsocketResponseStartEvent
-        self.scope: WebsocketScope
-        self.send = send
-        # RFC 8441 for HTTP/2 says use http or https, ASGI says ws or wss
-        self.scheme = "wss" if ssl else "ws"
-        self.server = server
-        self.start_time: float
-        self.state = ASGIWebsocketState.HANDSHAKE
-        self.stream_id = stream_id
-        self.tls = tls
-
-        self.connection: Connection
-        self.handshake: Handshake
-
-    @property
-    def idle(self) -> bool:
-        return self.state in {ASGIWebsocketState.CLOSED, ASGIWebsocketState.HTTPCLOSED}
-
-    async def handle(self, event: Event) -> None:
-        if self.closed:
-            return
-        elif isinstance(event, Request):
-            self.start_time = time()
-            self.handshake = Handshake(event.headers, event.http_version)
-            path, _, query_string = event.raw_path.partition(b"?")
-            self.scope = {
-                "type": "websocket",
-                "asgi": {"spec_version": "2.3", "version": "3.0"},
-                "scheme": self.scheme,
-                "http_version": event.http_version,
-                "path": unquote(path.decode("ascii")),
-                "raw_path": path,
-                "query_string": query_string,
-                "root_path": self.config.root_path,
-                "headers": event.headers,
-                "client": self.client,
-                "server": self.server,
-                "subprotocols": self.handshake.subprotocols or [],
-                "extensions": {"websocket.http.response": {}, "websocket.multiframe": {}},
-            }
-            if self.scheme == "wss" and self.tls:
-                self.scope["extensions"]["tls"] = self.tls
-
-            if not valid_server_name(self.config, event):
-                await self._send_error_response(404)
-                self.closed = True
-            elif not self.handshake.is_valid():
-                await self._send_error_response(400)
-                self.closed = True
-            else:
-                self.app_put = await self.task_group.spawn_app(
-                    self.app, self.config, self.scope, self.app_send
-                )
-                await self.app_put({"type": "websocket.connect"})  # type: ignore
-        elif isinstance(event, (Body, Data)):
-            self.connection.receive_data(event.data)
-            await self._handle_events()
-        elif isinstance(event, StreamClosed):
-            self.closed = True
-            if self.app_put is not None:
-                if self.state in {ASGIWebsocketState.HTTPCLOSED, ASGIWebsocketState.CLOSED}:
-                    code = CloseReason.NORMAL_CLOSURE.value
-                else:
-                    code = CloseReason.ABNORMAL_CLOSURE.value
-                await self.app_put({"type": "websocket.disconnect", "code": code})
-
-    async def app_send(self, message: Optional[ASGISendEvent]) -> None:
-        if self.closed:
-            # Allow app to finish after close
-            return
-
-        if message is None:  # ASGI App has finished sending messages
-            # Cleanup if required
-            if self.state == ASGIWebsocketState.HANDSHAKE:
-                await self._send_error_response(500)
-                await self.config.log.access(
-                    self.scope, {"status": 500, "headers": []}, time() - self.start_time
-                )
-            elif self.state == ASGIWebsocketState.CONNECTED:
-                await self._send_wsproto_event(CloseConnection(code=CloseReason.ABNORMAL_CLOSURE))
-            await self.send(StreamClosed(stream_id=self.stream_id))
-        else:
-            if message["type"] == "websocket.accept" and self.state == ASGIWebsocketState.HANDSHAKE:
-                await self._accept(message)
-            elif (
-                message["type"] == "websocket.http.response.start"
-                and self.state == ASGIWebsocketState.HANDSHAKE
-            ):
-                self.response = message
-            elif message["type"] == "websocket.http.response.body" and self.state in {
-                ASGIWebsocketState.HANDSHAKE,
-                ASGIWebsocketState.RESPONSE,
-            }:
-                await self._send_rejection(message)
-            elif message["type"] == "websocket.send" and self.state == ASGIWebsocketState.CONNECTED:
-                event: WSProtoEvent
-                if message.get("bytes") is not None:
-                    event = BytesMessage(
-                        data=bytes(message["bytes"]),
-                        message_finished=message.get("message_finished", True),
-                    )
-                elif not isinstance(message["text"], str):
-                    raise TypeError(f"{message['text']} should be a str")
-                else:
-                    event = TextMessage(
-                        data=message["text"], message_finished=message.get("message_finished", True)
-                    )
-                await self._send_wsproto_event(event)
-            elif (
-                message["type"] == "websocket.close" and self.state == ASGIWebsocketState.HANDSHAKE
-            ):
-                self.state = ASGIWebsocketState.HTTPCLOSED
-                await self._send_error_response(403)
-            elif message["type"] == "websocket.close":
-                self.state = ASGIWebsocketState.CLOSED
-                await self._send_wsproto_event(
-                    CloseConnection(
-                        code=int(message.get("code", CloseReason.NORMAL_CLOSURE)),
-                        reason=message.get("reason"),
-                    )
-                )
-                await self.send(EndData(stream_id=self.stream_id))
-            else:
-                raise UnexpectedMessageError(self.state, message["type"])
-
-    async def _handle_events(self) -> None:
-        for event in self.connection.events():
-            if isinstance(event, Message):
-                try:
-                    self.buffer.extend(event)
-                except FrameTooLargeError:
-                    await self._send_wsproto_event(
-                        CloseConnection(code=CloseReason.MESSAGE_TOO_BIG)
-                    )
-                    break
-
-                if event.message_finished:
-                    await self.app_put(self.buffer.to_message())
-                    self.buffer.clear()
-            elif isinstance(event, Ping):
-                await self._send_wsproto_event(event.response())
-            elif isinstance(event, CloseConnection):
-                if self.connection.state == ConnectionState.REMOTE_CLOSING:
-                    await self._send_wsproto_event(event.response())
-                await self.send(StreamClosed(stream_id=self.stream_id))
-
-    async def _send_error_response(self, status_code: int) -> None:
-        await self.send(
-            Response(
-                stream_id=self.stream_id,
-                status_code=status_code,
-                headers=[(b"content-length", b"0"), (b"connection", b"close")],
-            )
-        )
-        await self.send(EndBody(stream_id=self.stream_id))
-        await self.config.log.access(
-            self.scope, {"status": status_code, "headers": []}, time() - self.start_time
-        )
-
-    async def _send_wsproto_event(self, event: WSProtoEvent) -> None:
-        data = self.connection.send(event)
-        await self.send(Data(stream_id=self.stream_id, data=data))
-
-    async def _accept(self, message: WebsocketAcceptEvent) -> None:
-        self.state = ASGIWebsocketState.CONNECTED
-        status_code, headers, self.connection = self.handshake.accept(
-            message.get("subprotocol"), message.get("headers", [])
-        )
-        await self.send(
-            Response(
-                stream_id=self.stream_id,
-                status_code=status_code,
-                headers=headers,
-                reason="Switching Protocols",
-            )
-        )
-        await self.config.log.access(
-            self.scope, {"status": status_code, "headers": []}, time() - self.start_time
-        )
-        if self.config.websocket_ping_interval is not None:
-            self.task_group.spawn(self._send_pings)
-
-    async def _send_rejection(self, message: WebsocketResponseBodyEvent) -> None:
-        body_suppressed = suppress_body("GET", self.response["status"])
-        if self.state == ASGIWebsocketState.HANDSHAKE:
-            headers = build_and_validate_headers(self.response["headers"])
-            reason = self.response["meta"].get("reason", "") if "meta" in self.response else ""
-            await self.send(
-                Response(
-                    stream_id=self.stream_id,
-                    status_code=int(self.response["status"]),
-                    headers=headers,
-                    reason=reason,
-                )
-            )
-            self.state = ASGIWebsocketState.RESPONSE
-        if not body_suppressed:
-            await self.send(Body(stream_id=self.stream_id, data=bytes(message.get("body", b""))))
-        if not message.get("more_body", False):
-            self.state = ASGIWebsocketState.HTTPCLOSED
-            await self.send(EndBody(stream_id=self.stream_id))
-            await self.config.log.access(self.scope, self.response, time() - self.start_time)
-
-    async def _send_pings(self) -> None:
-        while not self.closed:
-            await self._send_wsproto_event(Ping())
-            await self.context.sleep(self.config.websocket_ping_interval)
+from __future__ import annotations
+
+from enum import auto, Enum
+from io import BytesIO, StringIO
+from time import time
+from typing import Awaitable, Callable, Iterable, List, Optional, Tuple, Union, Dict, Any
+from urllib.parse import unquote
+
+from wsproto.connection import Connection, ConnectionState, ConnectionType
+from wsproto.events import (
+    BytesMessage,
+    CloseConnection,
+    Event as WSProtoEvent,
+    Message,
+    Ping,
+    TextMessage,
+)
+from wsproto.extensions import Extension, PerMessageDeflate
+from wsproto.frame_protocol import CloseReason
+from wsproto.handshake import server_extensions_handshake, WEBSOCKET_VERSION
+from wsproto.utilities import generate_accept_token, split_comma_header
+
+from .events import Body, Data, EndBody, EndData, Event, Request, Response, StreamClosed
+from ..config import Config
+from ..typing import (
+    AppWrapper,
+    ASGISendEvent,
+    TaskGroup,
+    WebsocketAcceptEvent,
+    WebsocketResponseBodyEvent,
+    WebsocketResponseStartEvent,
+    WebsocketScope,
+    WorkerContext,
+)
+from ..utils import (
+    build_and_validate_headers,
+    suppress_body,
+    UnexpectedMessageError,
+    valid_server_name,
+)
+
+
+class ASGIWebsocketState(Enum):
+    # Hypercorn supports the ASGI websocket HTTP response extension,
+    # which allows HTTP responses rather than acceptance.
+    HANDSHAKE = auto()
+    CONNECTED = auto()
+    RESPONSE = auto()
+    CLOSED = auto()
+    HTTPCLOSED = auto()
+
+
+class FrameTooLargeError(Exception):
+    pass
+
+
+class Handshake:
+    def __init__(self, headers: List[Tuple[bytes, bytes]], http_version: str) -> None:
+        self.http_version = http_version
+        self.connection_tokens: Optional[List[str]] = None
+        self.extensions: Optional[List[str]] = None
+        self.key: Optional[bytes] = None
+        self.subprotocols: Optional[List[str]] = None
+        self.upgrade: Optional[bytes] = None
+        self.version: Optional[bytes] = None
+        for name, value in headers:
+            name = name.lower()
+            if name == b"connection":
+                self.connection_tokens = split_comma_header(value)
+            elif name == b"sec-websocket-extensions":
+                self.extensions = split_comma_header(value)
+            elif name == b"sec-websocket-key":
+                self.key = value
+            elif name == b"sec-websocket-protocol":
+                self.subprotocols = split_comma_header(value)
+            elif name == b"sec-websocket-version":
+                self.version = value
+            elif name == b"upgrade":
+                self.upgrade = value
+
+    def is_valid(self) -> bool:
+        if self.http_version < "1.1":
+            return False
+        elif self.http_version == "1.1":
+            if self.key is None:
+                return False
+            if self.connection_tokens is None or not any(
+                token.lower() == "upgrade" for token in self.connection_tokens
+            ):
+                return False
+            if self.upgrade.lower() != b"websocket":
+                return False
+
+        if self.version != WEBSOCKET_VERSION:
+            return False
+        return True
+
+    def accept(
+        self,
+        subprotocol: Optional[str],
+        additional_headers: Iterable[Tuple[bytes, bytes]],
+    ) -> Tuple[int, List[Tuple[bytes, bytes]], Connection]:
+        headers = []
+        if subprotocol is not None:
+            if self.subprotocols is None or subprotocol not in self.subprotocols:
+                raise Exception("Invalid Subprotocol")
+            else:
+                headers.append((b"sec-websocket-protocol", subprotocol.encode()))
+
+        extensions: List[Extension] = [PerMessageDeflate()]
+        accepts = None
+        if self.extensions is not None:
+            accepts = server_extensions_handshake(self.extensions, extensions)
+
+        if accepts:
+            headers.append((b"sec-websocket-extensions", accepts))
+
+        if self.key is not None:
+            headers.append((b"sec-websocket-accept", generate_accept_token(self.key)))
+
+        status_code = 200
+        if self.http_version == "1.1":
+            headers.extend([(b"upgrade", b"WebSocket"), (b"connection", b"Upgrade")])
+            status_code = 101
+
+        for name, value in additional_headers:
+            if b"sec-websocket-protocol" == name or name.startswith(b":"):
+                raise Exception(f"Invalid additional header, {name.decode()}")
+
+            headers.append((name, value))
+
+        return status_code, headers, Connection(ConnectionType.SERVER, extensions)
+
+
+class WebsocketBuffer:
+    def __init__(self, max_length: int) -> None:
+        self.value: Optional[Union[BytesIO, StringIO]] = None
+        self.length = 0
+        self.max_length = max_length
+
+    def extend(self, event: Message) -> None:
+        if self.value is None:
+            if isinstance(event, TextMessage):
+                self.value = StringIO()
+            else:
+                self.value = BytesIO()
+        self.length += self.value.write(event.data)
+        if self.length > self.max_length:
+            raise FrameTooLargeError()
+
+    def clear(self) -> None:
+        self.value = None
+        self.length = 0
+
+    def to_message(self) -> dict:
+        return {
+            "type": "websocket.receive",
+            "bytes": self.value.getvalue() if isinstance(self.value, BytesIO) else None,
+            "text": self.value.getvalue() if isinstance(self.value, StringIO) else None,
+        }
+
+
+class WSStream:
+    def __init__(
+        self,
+        app: AppWrapper,
+        config: Config,
+        context: WorkerContext,
+        task_group: TaskGroup,
+        ssl: bool,
+        client: Optional[Tuple[str, int]],
+        server: Optional[Tuple[str, int]],
+        send: Callable[[Event], Awaitable[None]],
+        stream_id: int,
+        tls: Optional[dict] = None,
+        app_state: Optional[Dict[str, Any]] = None,
+    ) -> None:
+        self.app = app
+        self.app_put: Optional[Callable] = None
+        self.buffer = WebsocketBuffer(config.websocket_max_message_size)
+        self.client = client
+        self.closed = False
+        self.config = config
+        self.context = context
+        self.task_group = task_group
+        self.response: WebsocketResponseStartEvent
+        self.scope: WebsocketScope
+        self.send = send
+        # RFC 8441 for HTTP/2 says use http or https, ASGI says ws or wss
+        self.scheme = "wss" if ssl else "ws"
+        self.server = server
+        self.start_time: float
+        self.state = ASGIWebsocketState.HANDSHAKE
+        self.stream_id = stream_id
+        self.tls = tls
+
+        self.connection: Connection
+        self.handshake: Handshake
+        self.app_state = app_state
+
+    @property
+    def idle(self) -> bool:
+        return self.state in {ASGIWebsocketState.CLOSED, ASGIWebsocketState.HTTPCLOSED}
+
+    async def handle(self, event: Event) -> None:
+        if self.closed:
+            return
+        elif isinstance(event, Request):
+            self.start_time = time()
+            self.handshake = Handshake(event.headers, event.http_version)
+            path, _, query_string = event.raw_path.partition(b"?")
+            self.scope = {
+                "type": "websocket",
+                "asgi": {"spec_version": "2.3", "version": "3.0"},
+                "scheme": self.scheme,
+                "http_version": event.http_version,
+                "path": unquote(path.decode("ascii")),
+                "raw_path": path,
+                "query_string": query_string,
+                "root_path": self.config.root_path,
+                "headers": event.headers,
+                "client": self.client,
+                "server": self.server,
+                "subprotocols": self.handshake.subprotocols or [],
+                "extensions": {"websocket.http.response": {}, "websocket.multiframe": {}},
+                "state": self.app_state,
+            }
+            if self.scheme == "wss" and self.tls:
+                self.scope["extensions"]["tls"] = self.tls
+
+            if not valid_server_name(self.config, event):
+                await self._send_error_response(404)
+                self.closed = True
+            elif not self.handshake.is_valid():
+                await self._send_error_response(400)
+                self.closed = True
+            else:
+                self.app_put = await self.task_group.spawn_app(
+                    self.app, self.config, self.scope, self.app_send
+                )
+                await self.app_put({"type": "websocket.connect"})  # type: ignore
+        elif isinstance(event, (Body, Data)):
+            self.connection.receive_data(event.data)
+            await self._handle_events()
+        elif isinstance(event, StreamClosed):
+            self.closed = True
+            if self.app_put is not None:
+                if self.state in {ASGIWebsocketState.HTTPCLOSED, ASGIWebsocketState.CLOSED}:
+                    code = CloseReason.NORMAL_CLOSURE.value
+                else:
+                    code = CloseReason.ABNORMAL_CLOSURE.value
+                await self.app_put({"type": "websocket.disconnect", "code": code})
+
+    async def app_send(self, message: Optional[ASGISendEvent]) -> None:
+        if self.closed:
+            # Allow app to finish after close
+            return
+
+        if message is None:  # ASGI App has finished sending messages
+            # Cleanup if required
+            if self.state == ASGIWebsocketState.HANDSHAKE:
+                await self._send_error_response(500)
+                await self.config.log.access(
+                    self.scope, {"status": 500, "headers": []}, time() - self.start_time
+                )
+            elif self.state == ASGIWebsocketState.CONNECTED:
+                await self._send_wsproto_event(CloseConnection(code=CloseReason.ABNORMAL_CLOSURE))
+            await self.send(StreamClosed(stream_id=self.stream_id))
+        else:
+            if message["type"] == "websocket.accept" and self.state == ASGIWebsocketState.HANDSHAKE:
+                await self._accept(message)
+            elif (
+                message["type"] == "websocket.http.response.start"
+                and self.state == ASGIWebsocketState.HANDSHAKE
+            ):
+                self.response = message
+            elif message["type"] == "websocket.http.response.body" and self.state in {
+                ASGIWebsocketState.HANDSHAKE,
+                ASGIWebsocketState.RESPONSE,
+            }:
+                await self._send_rejection(message)
+            elif message["type"] == "websocket.send" and self.state == ASGIWebsocketState.CONNECTED:
+                event: WSProtoEvent
+                if message.get("bytes") is not None:
+                    event = BytesMessage(
+                        data=bytes(message["bytes"]),
+                        message_finished=message.get("message_finished", True),
+                    )
+                elif not isinstance(message["text"], str):
+                    raise TypeError(f"{message['text']} should be a str")
+                else:
+                    event = TextMessage(
+                        data=message["text"], message_finished=message.get("message_finished", True)
+                    )
+                await self._send_wsproto_event(event)
+            elif (
+                message["type"] == "websocket.close" and self.state == ASGIWebsocketState.HANDSHAKE
+            ):
+                self.state = ASGIWebsocketState.HTTPCLOSED
+                await self._send_error_response(403)
+            elif message["type"] == "websocket.close":
+                self.state = ASGIWebsocketState.CLOSED
+                await self._send_wsproto_event(
+                    CloseConnection(
+                        code=int(message.get("code", CloseReason.NORMAL_CLOSURE)),
+                        reason=message.get("reason"),
+                    )
+                )
+                await self.send(EndData(stream_id=self.stream_id))
+            else:
+                raise UnexpectedMessageError(self.state, message["type"])
+
+    async def _handle_events(self) -> None:
+        for event in self.connection.events():
+            if isinstance(event, Message):
+                try:
+                    self.buffer.extend(event)
+                except FrameTooLargeError:
+                    await self._send_wsproto_event(
+                        CloseConnection(code=CloseReason.MESSAGE_TOO_BIG)
+                    )
+                    break
+
+                if event.message_finished:
+                    await self.app_put(self.buffer.to_message())
+                    self.buffer.clear()
+            elif isinstance(event, Ping):
+                await self._send_wsproto_event(event.response())
+            elif isinstance(event, CloseConnection):
+                if self.connection.state == ConnectionState.REMOTE_CLOSING:
+                    await self._send_wsproto_event(event.response())
+                await self.send(StreamClosed(stream_id=self.stream_id))
+
+    async def _send_error_response(self, status_code: int) -> None:
+        await self.send(
+            Response(
+                stream_id=self.stream_id,
+                status_code=status_code,
+                headers=[(b"content-length", b"0"), (b"connection", b"close")],
+            )
+        )
+        await self.send(EndBody(stream_id=self.stream_id))
+        await self.config.log.access(
+            self.scope, {"status": status_code, "headers": []}, time() - self.start_time
+        )
+
+    async def _send_wsproto_event(self, event: WSProtoEvent) -> None:
+        data = self.connection.send(event)
+        await self.send(Data(stream_id=self.stream_id, data=data))
+
+    async def _accept(self, message: WebsocketAcceptEvent) -> None:
+        self.state = ASGIWebsocketState.CONNECTED
+        status_code, headers, self.connection = self.handshake.accept(
+            message.get("subprotocol"), message.get("headers", [])
+        )
+        await self.send(
+            Response(
+                stream_id=self.stream_id,
+                status_code=status_code,
+                headers=headers,
+                reason="Switching Protocols" if status_code == 101 else "",
+            )
+        )
+        await self.config.log.access(
+            self.scope, {"status": status_code, "headers": []}, time() - self.start_time
+        )
+        if self.config.websocket_ping_interval is not None:
+            self.task_group.spawn(self._send_pings)
+
+    async def _send_rejection(self, message: WebsocketResponseBodyEvent) -> None:
+        body_suppressed = suppress_body("GET", self.response["status"])
+        if self.state == ASGIWebsocketState.HANDSHAKE:
+            headers = build_and_validate_headers(self.response["headers"])
+            reason = self.response.get("reason", "")
+            await self.send(
+                Response(
+                    stream_id=self.stream_id,
+                    status_code=int(self.response["status"]),
+                    headers=headers,
+                    reason=reason,
+                )
+            )
+            self.state = ASGIWebsocketState.RESPONSE
+        if not body_suppressed:
+            await self.send(Body(stream_id=self.stream_id, data=bytes(message.get("body", b""))))
+        if not message.get("more_body", False):
+            self.state = ASGIWebsocketState.HTTPCLOSED
+            await self.send(EndBody(stream_id=self.stream_id))
+            await self.config.log.access(self.scope, self.response, time() - self.start_time)
+
+    async def _send_pings(self) -> None:
+        while not self.closed:
+            await self._send_wsproto_event(Ping())
+            await self.context.sleep(self.config.websocket_ping_interval)
```

### Comparing `nonecorn-0.14.1.dev1/src/hypercorn/run.py` & `nonecorn-0.14.3.dev1/src/hypercorn/run.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,95 +1,109 @@
-from __future__ import annotations
-
-import multiprocessing
-import platform
-import signal
-import time
-from multiprocessing import Event, Process
-from multiprocessing.synchronize import Event as EventType
-from typing import Any, List
-
-from .config import Config, Sockets
-from .typing import WorkerFunc
-from .utils import load_application, wait_for_changes, write_pid_file
-
-multiprocessing.allow_connection_pickling()
-spawn = multiprocessing.get_context("spawn")
-
-
-def run(config: Config) -> None:
-    if config.pid_path is not None:
-        write_pid_file(config.pid_path)
-
-    worker_func: WorkerFunc
-    if config.worker_class == "asyncio":
-        from .asyncio.run import asyncio_worker
-
-        worker_func = asyncio_worker
-    elif config.worker_class == "uvloop":
-        from .asyncio.run import uvloop_worker
-
-        worker_func = uvloop_worker
-    elif config.worker_class == "trio":
-        from .trio.run import trio_worker
-
-        worker_func = trio_worker
-    else:
-        raise ValueError(f"No worker of class {config.worker_class} exists")
-
-    sockets = config.create_sockets()
-
-    # Load the application so that the correct paths are checked for
-    # changes.
-    load_application(config.application_path, config.wsgi_max_body_size)
-
-    active = True
-    while active:
-        # Ignore SIGINT before creating the processes, so that they
-        # inherit the signal handling. This means that the shutdown
-        # function controls the shutdown.
-        signal.signal(signal.SIGINT, signal.SIG_IGN)
-
-        shutdown_event = Event()
-        processes = start_processes(config, worker_func, sockets, shutdown_event)
-
-        def shutdown(*args: Any) -> None:
-            nonlocal active, shutdown_event
-            shutdown_event.set()
-            active = False
-
-        for signal_name in {"SIGINT", "SIGTERM", "SIGBREAK"}:
-            if hasattr(signal, signal_name):
-                signal.signal(getattr(signal, signal_name), shutdown)
-
-        if config.use_reloader:
-            wait_for_changes(shutdown_event)
-            shutdown_event.set()
-        else:
-            active = False
-
-    for process in processes:
-        process.join()
-    for process in processes:
-        process.terminate()
-
-    for sock in sockets.secure_sockets:
-        sock.close()
-    for sock in sockets.insecure_sockets:
-        sock.close()
-
-
-def start_processes(
-    config: Config, worker_func: WorkerFunc, sockets: Sockets, shutdown_event: EventType
-) -> List[Process]:
-    processes = []
-    for _ in range(config.workers):
-        process = Process(
-            target=worker_func,
-            kwargs={"config": config, "shutdown_event": shutdown_event, "sockets": sockets},
-        )
-        process.daemon = True
-        process.start()
-        processes.append(process)
-        if platform.system() == "Windows":
-            time.sleep(0.1)
-    return processes
+from __future__ import annotations
+
+import multiprocessing
+import platform
+import signal
+import time
+from multiprocessing import get_context
+from multiprocessing.context import BaseContext
+from multiprocessing.process import BaseProcess
+from multiprocessing.synchronize import Event as EventType
+from pickle import PicklingError
+from typing import Any, List
+
+from .config import Config, Sockets
+from .typing import WorkerFunc
+from .utils import load_application, wait_for_changes, write_pid_file
+
+multiprocessing.allow_connection_pickling()
+spawn = multiprocessing.get_context("spawn")
+
+
+def run(config: Config) -> None:
+    if config.pid_path is not None:
+        write_pid_file(config.pid_path)
+
+    worker_func: WorkerFunc
+    if config.worker_class == "asyncio":
+        from .asyncio.run import asyncio_worker
+
+        worker_func = asyncio_worker
+    elif config.worker_class == "uvloop":
+        from .asyncio.run import uvloop_worker
+
+        worker_func = uvloop_worker
+    elif config.worker_class == "trio":
+        from .trio.run import trio_worker
+
+        worker_func = trio_worker
+    else:
+        raise ValueError(f"No worker of class {config.worker_class} exists")
+
+    sockets = config.create_sockets()
+
+    # Load the application so that the correct paths are checked for
+    # changes.
+    load_application(config.application_path, config.wsgi_max_body_size)
+
+    ctx = get_context("spawn")
+
+    active = True
+    while active:
+        # Ignore SIGINT before creating the processes, so that they
+        # inherit the signal handling. This means that the shutdown
+        # function controls the shutdown.
+        signal.signal(signal.SIGINT, signal.SIG_IGN)
+
+        shutdown_event = ctx.Event()
+        processes = start_processes(config, worker_func, sockets, shutdown_event, ctx)
+
+        def shutdown(*args: Any) -> None:
+            nonlocal active, shutdown_event
+            shutdown_event.set()
+            active = False
+
+        for signal_name in {"SIGINT", "SIGTERM", "SIGBREAK"}:
+            if hasattr(signal, signal_name):
+                signal.signal(getattr(signal, signal_name), shutdown)
+
+        if config.use_reloader:
+            wait_for_changes(shutdown_event)
+            shutdown_event.set()
+        else:
+            active = False
+
+    for process in processes:
+        process.join()
+    for process in processes:
+        process.terminate()
+
+    for sock in sockets.secure_sockets:
+        sock.close()
+    for sock in sockets.insecure_sockets:
+        sock.close()
+
+
+def start_processes(
+    config: Config,
+    worker_func: WorkerFunc,
+    sockets: Sockets,
+    shutdown_event: EventType,
+    ctx: BaseContext,
+) -> List[BaseProcess]:
+    processes = []
+    for _ in range(config.workers):
+        process = ctx.Process(  # type: ignore
+            target=worker_func,
+            kwargs={"config": config, "shutdown_event": shutdown_event, "sockets": sockets},
+        )
+        process.daemon = True
+        try:
+            process.start()
+        except PicklingError as error:
+            raise RuntimeError(
+                "Cannot pickle the config, see https://docs.python.org/3/library/pickle.html#pickle-picklable"  # noqa: E501
+            ) from error
+        processes.append(process)
+        if platform.system() == "Windows":
+            time.sleep(0.1)
+    return processes
```

### Comparing `nonecorn-0.14.1.dev1/src/hypercorn/trio/__init__.py` & `nonecorn-0.14.3.dev1/src/hypercorn/trio/__init__.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-from __future__ import annotations
-
-import warnings
-from typing import Awaitable, Callable, Optional
-
-import trio
-
-from .run import worker_serve
-from ..config import Config
-from ..typing import Framework
-from ..utils import wrap_app
-
-try:
-    from typing import Literal
-except ImportError:
-    from typing_extensions import Literal  # type: ignore
-
-
-async def serve(
-    app: Framework,
-    config: Config,
-    *,
-    shutdown_trigger: Optional[Callable[..., Awaitable[None]]] = None,
-    task_status: trio._core._run._TaskStatus = trio.TASK_STATUS_IGNORED,
-    mode: Optional[Literal["asgi", "wsgi"]] = None,
-) -> None:
-    """Serve an ASGI framework app given the config.
-
-    This allows for a programmatic way to serve an ASGI framework, it
-    can be used via,
-
-    .. code-block:: python
-
-        trio.run(serve, app, config)
-
-    It is assumed that the event-loop is configured before calling
-    this function, therefore configuration values that relate to loop
-    setup or process setup are ignored.
-
-    Arguments:
-        app: The ASGI application to serve.
-        config: A Hypercorn configuration object.
-        shutdown_trigger: This should return to trigger a graceful
-            shutdown.
-        mode: Specify if the app is WSGI or ASGI.
-    """
-    if config.debug:
-        warnings.warn("The config `debug` has no affect when using serve", Warning)
-    if config.workers != 1:
-        warnings.warn("The config `workers` has no affect when using serve", Warning)
-
-    await worker_serve(
-        wrap_app(app, config.wsgi_max_body_size, mode),
-        config,
-        shutdown_trigger=shutdown_trigger,
-        task_status=task_status,
-    )
+from __future__ import annotations
+
+import warnings
+from typing import Awaitable, Callable, Optional
+
+import trio
+
+from .run import worker_serve
+from ..config import Config
+from ..typing import Framework
+from ..utils import wrap_app
+
+try:
+    from typing import Literal
+except ImportError:
+    from typing_extensions import Literal  # type: ignore
+
+
+async def serve(
+    app: Framework,
+    config: Config,
+    *,
+    shutdown_trigger: Optional[Callable[..., Awaitable[None]]] = None,
+    task_status: trio._core._run._TaskStatus = trio.TASK_STATUS_IGNORED,
+    mode: Optional[Literal["asgi", "wsgi"]] = None,
+) -> None:
+    """Serve an ASGI framework app given the config.
+
+    This allows for a programmatic way to serve an ASGI framework, it
+    can be used via,
+
+    .. code-block:: python
+
+        trio.run(serve, app, config)
+
+    It is assumed that the event-loop is configured before calling
+    this function, therefore configuration values that relate to loop
+    setup or process setup are ignored.
+
+    Arguments:
+        app: The ASGI application to serve.
+        config: A Hypercorn configuration object.
+        shutdown_trigger: This should return to trigger a graceful
+            shutdown.
+        mode: Specify if the app is WSGI or ASGI.
+    """
+    if config.debug:
+        warnings.warn("The config `debug` has no affect when using serve", Warning)
+    if config.workers != 1:
+        warnings.warn("The config `workers` has no affect when using serve", Warning)
+
+    await worker_serve(
+        wrap_app(app, config.wsgi_max_body_size, mode),
+        config,
+        shutdown_trigger=shutdown_trigger,
+        task_status=task_status,
+    )
```

### Comparing `nonecorn-0.14.1.dev1/src/hypercorn/trio/lifespan.py` & `nonecorn-0.14.3.dev1/src/hypercorn/trio/lifespan.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,91 +1,100 @@
-from __future__ import annotations
-
-import trio
-
-from ..config import Config
-from ..typing import AppWrapper, ASGIReceiveEvent, ASGISendEvent, LifespanScope
-from ..utils import LifespanFailureError, LifespanTimeoutError
-
-
-class UnexpectedMessageError(Exception):
-    pass
-
-
-class Lifespan:
-    def __init__(self, app: AppWrapper, config: Config) -> None:
-        self.app = app
-        self.config = config
-        self.startup = trio.Event()
-        self.shutdown = trio.Event()
-        self.app_send_channel, self.app_receive_channel = trio.open_memory_channel(
-            config.max_app_queue_size
-        )
-        self.supported = True
-
-    async def handle_lifespan(
-        self, *, task_status: trio._core._run._TaskStatus = trio.TASK_STATUS_IGNORED
-    ) -> None:
-        task_status.started()
-        scope: LifespanScope = {
-            "type": "lifespan",
-            "asgi": {"spec_version": "2.0", "version": "3.0"},
-        }
-        try:
-            await self.app(scope, self.asgi_receive, self.asgi_send, trio.to_thread.run_sync)
-        except LifespanFailureError:
-            # Lifespan failures should crash the server
-            raise
-        except Exception:
-            self.supported = False
-            if not self.startup.is_set():
-                await self.config.log.warning(
-                    "ASGI Framework Lifespan error, continuing without Lifespan support"
-                )
-            elif not self.shutdown.is_set():
-                await self.config.log.exception(
-                    "ASGI Framework Lifespan error, shutdown without Lifespan support"
-                )
-            else:
-                await self.config.log.exception("ASGI Framework Lifespan errored after shutdown.")
-        finally:
-            self.startup.set()
-            self.shutdown.set()
-            await self.app_send_channel.aclose()
-            await self.app_receive_channel.aclose()
-
-    async def wait_for_startup(self) -> None:
-        if not self.supported:
-            return
-
-        await self.app_send_channel.send({"type": "lifespan.startup"})
-        try:
-            with trio.fail_after(self.config.startup_timeout):
-                await self.startup.wait()
-        except trio.TooSlowError as error:
-            raise LifespanTimeoutError("startup") from error
-
-    async def wait_for_shutdown(self) -> None:
-        if not self.supported:
-            return
-
-        await self.app_send_channel.send({"type": "lifespan.shutdown"})
-        try:
-            with trio.fail_after(self.config.shutdown_timeout):
-                await self.shutdown.wait()
-        except trio.TooSlowError as error:
-            raise LifespanTimeoutError("startup") from error
-
-    async def asgi_receive(self) -> ASGIReceiveEvent:
-        return await self.app_receive_channel.receive()
-
-    async def asgi_send(self, message: ASGISendEvent) -> None:
-        if message["type"] == "lifespan.startup.complete":
-            self.startup.set()
-        elif message["type"] == "lifespan.shutdown.complete":
-            self.shutdown.set()
-        elif message["type"] == "lifespan.startup.failed":
-            raise LifespanFailureError("startup", message["message"])
-        elif message["type"] == "lifespan.shutdown.failed":
-            raise LifespanFailureError("shutdown", message["message"])
-        else:
-            raise UnexpectedMessageError(message["type"])
+from __future__ import annotations
+
+from typing import Dict, Any
+import trio
+
+from ..config import Config
+from ..typing import AppWrapper, ASGIReceiveEvent, ASGISendEvent, LifespanScope
+from ..utils import LifespanFailureError, LifespanTimeoutError
+
+
+class UnexpectedMessageError(Exception):
+    pass
+
+
+class Lifespan:
+    def __init__(self, app: AppWrapper, config: Config) -> None:
+        self.app = app
+        self.config = config
+        self.startup = trio.Event()
+        self.shutdown = trio.Event()
+        self.app_send_channel, self.app_receive_channel = trio.open_memory_channel(
+            config.max_app_queue_size
+        )
+        self.supported = True
+        self.state: Dict[str, Any] = {}
+
+    async def handle_lifespan(
+        self, *, task_status: trio._core._run._TaskStatus = trio.TASK_STATUS_IGNORED
+    ) -> None:
+        task_status.started()
+        scope: LifespanScope = {
+            "type": "lifespan",
+            "asgi": {"spec_version": "2.0", "version": "3.0"},
+            "state": self.state,
+        }
+        try:
+            await self.app(
+                scope,
+                self.asgi_receive,
+                self.asgi_send,
+                trio.to_thread.run_sync,
+                trio.from_thread.run,
+            )
+        except LifespanFailureError:
+            # Lifespan failures should crash the server
+            raise
+        except Exception:
+            self.supported = False
+            if not self.startup.is_set():
+                await self.config.log.warning(
+                    "ASGI Framework Lifespan error, continuing without Lifespan support"
+                )
+            elif not self.shutdown.is_set():
+                await self.config.log.exception(
+                    "ASGI Framework Lifespan error, shutdown without Lifespan support"
+                )
+            else:
+                await self.config.log.exception("ASGI Framework Lifespan errored after shutdown.")
+        finally:
+            self.startup.set()
+            self.shutdown.set()
+            await self.app_send_channel.aclose()
+            await self.app_receive_channel.aclose()
+
+    async def wait_for_startup(self) -> None:
+        if not self.supported:
+            return
+
+        await self.app_send_channel.send({"type": "lifespan.startup"})
+        try:
+            with trio.fail_after(self.config.startup_timeout):
+                await self.startup.wait()
+        except trio.TooSlowError as error:
+            raise LifespanTimeoutError("startup") from error
+
+    async def wait_for_shutdown(self) -> None:
+        if not self.supported:
+            return
+
+        await self.app_send_channel.send({"type": "lifespan.shutdown"})
+        try:
+            with trio.fail_after(self.config.shutdown_timeout):
+                await self.shutdown.wait()
+        except trio.TooSlowError as error:
+            raise LifespanTimeoutError("startup") from error
+
+    async def asgi_receive(self) -> ASGIReceiveEvent:
+        return await self.app_receive_channel.receive()
+
+    async def asgi_send(self, message: ASGISendEvent) -> None:
+        if message["type"] == "lifespan.startup.complete":
+            self.startup.set()
+        elif message["type"] == "lifespan.shutdown.complete":
+            self.shutdown.set()
+        elif message["type"] == "lifespan.startup.failed":
+            raise LifespanFailureError("startup", message.get("message", ""))
+        elif message["type"] == "lifespan.shutdown.failed":
+            raise LifespanFailureError("shutdown", message.get("message", ""))
+        else:
+            raise UnexpectedMessageError(message["type"])
```

### Comparing `nonecorn-0.14.1.dev1/src/hypercorn/trio/run.py` & `nonecorn-0.14.3.dev1/src/hypercorn/trio/run.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,116 +1,116 @@
-from __future__ import annotations
-
-from functools import partial
-from multiprocessing.synchronize import Event as EventType
-from typing import Awaitable, Callable, Optional
-
-import trio
-
-from .lifespan import Lifespan
-from .statsd import StatsdLogger
-from .tcp_server import TCPServer
-from .udp_server import UDPServer
-from .worker_context import WorkerContext
-from ..config import Config, Sockets
-from ..typing import AppWrapper
-from ..utils import (
-    check_multiprocess_shutdown_event,
-    load_application,
-    raise_shutdown,
-    repr_socket_addr,
-    ShutdownError,
-)
-
-
-async def worker_serve(
-    app: AppWrapper,
-    config: Config,
-    *,
-    sockets: Optional[Sockets] = None,
-    shutdown_trigger: Optional[Callable[..., Awaitable[None]]] = None,
-    task_status: trio._core._run._TaskStatus = trio.TASK_STATUS_IGNORED,
-) -> None:
-    config.set_statsd_logger_class(StatsdLogger)
-
-    lifespan = Lifespan(app, config)
-    context = WorkerContext()
-
-    async with trio.open_nursery() as lifespan_nursery:
-        await lifespan_nursery.start(lifespan.handle_lifespan)
-        await lifespan.wait_for_startup()
-
-        async with trio.open_nursery() as server_nursery:
-            if sockets is None:
-                sockets = config.create_sockets()
-                for sock in sockets.secure_sockets:
-                    sock.listen(config.backlog)
-                for sock in sockets.insecure_sockets:
-                    sock.listen(config.backlog)
-
-            ssl_context = config.create_ssl_context()
-            listeners = []
-            binds = []
-            for sock in sockets.secure_sockets:
-                listeners.append(
-                    trio.SSLListener(
-                        trio.SocketListener(trio.socket.from_stdlib_socket(sock)),
-                        ssl_context,
-                        https_compatible=True,
-                    )
-                )
-                bind = repr_socket_addr(sock.family, sock.getsockname())
-                binds.append(f"https://{bind}")
-                await config.log.info(f"Running on https://{bind} (CTRL + C to quit)")
-
-            for sock in sockets.insecure_sockets:
-                listeners.append(trio.SocketListener(trio.socket.from_stdlib_socket(sock)))
-                bind = repr_socket_addr(sock.family, sock.getsockname())
-                binds.append(f"http://{bind}")
-                await config.log.info(f"Running on http://{bind} (CTRL + C to quit)")
-
-            for sock in sockets.quic_sockets:
-                await server_nursery.start(UDPServer(app, config, context, sock).run)
-                bind = repr_socket_addr(sock.family, sock.getsockname())
-                await config.log.info(f"Running on https://{bind} (QUIC) (CTRL + C to quit)")
-
-            task_status.started(binds)
-            try:
-                async with trio.open_nursery() as nursery:
-                    if shutdown_trigger is not None:
-                        nursery.start_soon(raise_shutdown, shutdown_trigger)
-
-                    nursery.start_soon(
-                        partial(
-                            trio.serve_listeners,
-                            partial(TCPServer, app, config, context),
-                            listeners,
-                            handler_nursery=server_nursery,
-                        ),
-                    )
-
-                    await trio.sleep_forever()
-            except (ShutdownError, KeyboardInterrupt):
-                pass
-            finally:
-                await context.terminated.set()
-                server_nursery.cancel_scope.deadline = trio.current_time() + config.graceful_timeout
-
-        await lifespan.wait_for_shutdown()
-        lifespan_nursery.cancel_scope.cancel()
-
-
-def trio_worker(
-    config: Config, sockets: Optional[Sockets] = None, shutdown_event: Optional[EventType] = None
-) -> None:
-    if sockets is not None:
-        for sock in sockets.secure_sockets:
-            sock.listen(config.backlog)
-        for sock in sockets.insecure_sockets:
-            sock.listen(config.backlog)
-    app = load_application(config.application_path, config.wsgi_max_body_size)
-
-    shutdown_trigger = None
-    if shutdown_event is not None:
-        shutdown_trigger = partial(check_multiprocess_shutdown_event, shutdown_event, trio.sleep)
-
-    trio.run(partial(worker_serve, app, config, sockets=sockets, shutdown_trigger=shutdown_trigger))
+from __future__ import annotations
+
+from functools import partial
+from multiprocessing.synchronize import Event as EventType
+from typing import Awaitable, Callable, Optional
+
+import trio
+
+from .lifespan import Lifespan
+from .statsd import StatsdLogger
+from .tcp_server import TCPServer
+from .udp_server import UDPServer
+from .worker_context import WorkerContext
+from ..config import Config, Sockets
+from ..typing import AppWrapper
+from ..utils import (
+    check_multiprocess_shutdown_event,
+    load_application,
+    raise_shutdown,
+    repr_socket_addr,
+    ShutdownError,
+)
+
+
+async def worker_serve(
+    app: AppWrapper,
+    config: Config,
+    *,
+    sockets: Optional[Sockets] = None,
+    shutdown_trigger: Optional[Callable[..., Awaitable[None]]] = None,
+    task_status: trio._core._run._TaskStatus = trio.TASK_STATUS_IGNORED,
+) -> None:
+    config.set_statsd_logger_class(StatsdLogger)
+
+    lifespan = Lifespan(app, config)
+    context = WorkerContext()
+
+    async with trio.open_nursery() as lifespan_nursery:
+        await lifespan_nursery.start(lifespan.handle_lifespan)
+        await lifespan.wait_for_startup()
+
+        async with trio.open_nursery() as server_nursery:
+            if sockets is None:
+                sockets = config.create_sockets()
+                for sock in sockets.secure_sockets:
+                    sock.listen(config.backlog)
+                for sock in sockets.insecure_sockets:
+                    sock.listen(config.backlog)
+
+            ssl_context = config.create_ssl_context()
+            listeners = []
+            binds = []
+            for sock in sockets.secure_sockets:
+                listeners.append(
+                    trio.SSLListener(
+                        trio.SocketListener(trio.socket.from_stdlib_socket(sock)),
+                        ssl_context,
+                        https_compatible=True,
+                    )
+                )
+                bind = repr_socket_addr(sock.family, sock.getsockname())
+                binds.append(f"https://{bind}")
+                await config.log.info(f"Running on https://{bind} (CTRL + C to quit)")
+
+            for sock in sockets.insecure_sockets:
+                listeners.append(trio.SocketListener(trio.socket.from_stdlib_socket(sock)))
+                bind = repr_socket_addr(sock.family, sock.getsockname())
+                binds.append(f"http://{bind}")
+                await config.log.info(f"Running on http://{bind} (CTRL + C to quit)")
+
+            for sock in sockets.quic_sockets:
+                await server_nursery.start(UDPServer(app, config, context, sock, lifespan.state.copy()).run)
+                bind = repr_socket_addr(sock.family, sock.getsockname())
+                await config.log.info(f"Running on https://{bind} (QUIC) (CTRL + C to quit)")
+
+            task_status.started(binds)
+            try:
+                async with trio.open_nursery() as nursery:
+                    if shutdown_trigger is not None:
+                        nursery.start_soon(raise_shutdown, shutdown_trigger)
+
+                    nursery.start_soon(
+                        partial(
+                            trio.serve_listeners,
+                            partial(TCPServer, app, config, context, app_state=lifespan.state.copy()),
+                            listeners,
+                            handler_nursery=server_nursery,
+                        ),
+                    )
+
+                    await trio.sleep_forever()
+            except (ShutdownError, KeyboardInterrupt):
+                pass
+            finally:
+                await context.terminated.set()
+                server_nursery.cancel_scope.deadline = trio.current_time() + config.graceful_timeout
+
+        await lifespan.wait_for_shutdown()
+        lifespan_nursery.cancel_scope.cancel()
+
+
+def trio_worker(
+    config: Config, sockets: Optional[Sockets] = None, shutdown_event: Optional[EventType] = None
+) -> None:
+    if sockets is not None:
+        for sock in sockets.secure_sockets:
+            sock.listen(config.backlog)
+        for sock in sockets.insecure_sockets:
+            sock.listen(config.backlog)
+    app = load_application(config.application_path, config.wsgi_max_body_size)
+
+    shutdown_trigger = None
+    if shutdown_event is not None:
+        shutdown_trigger = partial(check_multiprocess_shutdown_event, shutdown_event, trio.sleep)
+
+    trio.run(partial(worker_serve, app, config, sockets=sockets, shutdown_trigger=shutdown_trigger))
```

### Comparing `nonecorn-0.14.1.dev1/src/hypercorn/trio/task_group.py` & `nonecorn-0.14.3.dev1/src/hypercorn/trio/task_group.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,68 +1,76 @@
-from __future__ import annotations
-
-from types import TracebackType
-from typing import Any, Awaitable, Callable, Optional
-
-import trio
-
-from ..config import Config
-from ..typing import AppWrapper, ASGIReceiveCallable, ASGIReceiveEvent, ASGISendEvent, Scope
-
-
-async def _handle(
-    app: AppWrapper,
-    config: Config,
-    scope: Scope,
-    receive: ASGIReceiveCallable,
-    send: Callable[[Optional[ASGISendEvent]], Awaitable[None]],
-    sync_spawn: Callable,
-) -> None:
-    try:
-        await app(scope, receive, send, sync_spawn)
-    except trio.Cancelled:
-        raise
-    except trio.MultiError as error:
-        errors = trio.MultiError.filter(
-            lambda exc: None if isinstance(exc, trio.Cancelled) else exc, root_exc=error
-        )
-        if errors is not None:
-            await config.log.exception("Error in ASGI Framework")
-            await send(None)
-        else:
-            raise
-    except Exception:
-        await config.log.exception("Error in ASGI Framework")
-    finally:
-        await send(None)
-
-
-class TaskGroup:
-    def __init__(self) -> None:
-        self._nursery: Optional[trio._core._run.Nursery] = None
-        self._nursery_manager: Optional[trio._core._run.NurseryManager] = None
-
-    async def spawn_app(
-        self,
-        app: AppWrapper,
-        config: Config,
-        scope: Scope,
-        send: Callable[[Optional[ASGISendEvent]], Awaitable[None]],
-    ) -> Callable[[ASGIReceiveEvent], Awaitable[None]]:
-        app_send_channel, app_receive_channel = trio.open_memory_channel(config.max_app_queue_size)
-        self._nursery.start_soon(
-            _handle, app, config, scope, app_receive_channel.receive, send, trio.to_thread.run_sync
-        )
-        return app_send_channel.send
-
-    def spawn(self, func: Callable, *args: Any) -> None:
-        self._nursery.start_soon(func, *args)
-
-    async def __aenter__(self) -> TaskGroup:
-        self._nursery_manager = trio.open_nursery()
-        self._nursery = await self._nursery_manager.__aenter__()
-        return self
-
-    async def __aexit__(self, exc_type: type, exc_value: BaseException, tb: TracebackType) -> None:
-        await self._nursery_manager.__aexit__(exc_type, exc_value, tb)
-        self._nursery_manager = None
-        self._nursery = None
+from __future__ import annotations
+
+from types import TracebackType
+from typing import Any, Awaitable, Callable, Optional
+
+import trio
+
+from ..config import Config
+from ..typing import AppWrapper, ASGIReceiveCallable, ASGIReceiveEvent, ASGISendEvent, Scope
+
+
+async def _handle(
+    app: AppWrapper,
+    config: Config,
+    scope: Scope,
+    receive: ASGIReceiveCallable,
+    send: Callable[[Optional[ASGISendEvent]], Awaitable[None]],
+    sync_spawn: Callable,
+    call_soon: Callable,
+) -> None:
+    try:
+        await app(scope, receive, send, sync_spawn, call_soon)
+    except trio.Cancelled:
+        raise
+    except trio.MultiError as error:
+        errors = trio.MultiError.filter(
+            lambda exc: None if isinstance(exc, trio.Cancelled) else exc, root_exc=error
+        )
+        if errors is not None:
+            await config.log.exception("Error in ASGI Framework")
+            await send(None)
+        else:
+            raise
+    except Exception:
+        await config.log.exception("Error in ASGI Framework")
+    finally:
+        await send(None)
+
+
+class TaskGroup:
+    def __init__(self) -> None:
+        self._nursery: Optional[trio._core._run.Nursery] = None
+        self._nursery_manager: Optional[trio._core._run.NurseryManager] = None
+
+    async def spawn_app(
+        self,
+        app: AppWrapper,
+        config: Config,
+        scope: Scope,
+        send: Callable[[Optional[ASGISendEvent]], Awaitable[None]],
+    ) -> Callable[[ASGIReceiveEvent], Awaitable[None]]:
+        app_send_channel, app_receive_channel = trio.open_memory_channel(config.max_app_queue_size)
+        self._nursery.start_soon(
+            _handle,
+            app,
+            config,
+            scope,
+            app_receive_channel.receive,
+            send,
+            trio.to_thread.run_sync,
+            trio.from_thread.run,
+        )
+        return app_send_channel.send
+
+    def spawn(self, func: Callable, *args: Any) -> None:
+        self._nursery.start_soon(func, *args)
+
+    async def __aenter__(self) -> TaskGroup:
+        self._nursery_manager = trio.open_nursery()
+        self._nursery = await self._nursery_manager.__aenter__()
+        return self
+
+    async def __aexit__(self, exc_type: type, exc_value: BaseException, tb: TracebackType) -> None:
+        await self._nursery_manager.__aexit__(exc_type, exc_value, tb)
+        self._nursery_manager = None
+        self._nursery = None
```

### Comparing `nonecorn-0.14.1.dev1/src/hypercorn/trio/udp_server.py` & `nonecorn-0.14.3.dev1/src/hypercorn/trio/udp_server.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,49 @@
-from __future__ import annotations
-
-import trio
-
-from .task_group import TaskGroup
-from .worker_context import WorkerContext
-from ..config import Config
-from ..events import Event, RawData
-from ..typing import AppWrapper
-from ..utils import parse_socket_addr
-
-MAX_RECV = 2**16
-
-
-class UDPServer:
-    def __init__(
-        self,
-        app: AppWrapper,
-        config: Config,
-        context: WorkerContext,
-        socket: trio.socket.socket,
-    ) -> None:
-        self.app = app
-        self.config = config
-        self.context = context
-        self.socket = trio.socket.from_stdlib_socket(socket)
-
-    async def run(
-        self, task_status: trio._core._run._TaskStatus = trio.TASK_STATUS_IGNORED
-    ) -> None:
-        from ..protocol.quic import QuicProtocol  # h3/Quic is an optional part of Hypercorn
-
-        task_status.started()
-        server = parse_socket_addr(self.socket.family, self.socket.getsockname())
-        async with TaskGroup() as task_group:
-            self.protocol = QuicProtocol(
-                self.app, self.config, self.context, task_group, server, self.protocol_send
-            )
-
-            while not self.context.terminated.is_set() or not self.protocol.idle:
-                data, address = await self.socket.recvfrom(MAX_RECV)
-                await self.protocol.handle(RawData(data=data, address=address))
-
-    async def protocol_send(self, event: Event) -> None:
-        if isinstance(event, RawData):
-            await self.socket.sendto(event.data, event.address)
+from __future__ import annotations
+
+from typing import Dict, Any
+import trio
+
+from .task_group import TaskGroup
+from .worker_context import WorkerContext
+from ..config import Config
+from ..events import Event, RawData
+from ..typing import AppWrapper
+from ..utils import parse_socket_addr
+
+MAX_RECV = 2**16
+
+
+class UDPServer:
+    def __init__(
+        self,
+        app: AppWrapper,
+        config: Config,
+        context: WorkerContext,
+        socket: trio.socket.socket,
+        app_state: Dict[str, Any],
+    ) -> None:
+        self.app = app
+        self.config = config
+        self.context = context
+        self.socket = trio.socket.from_stdlib_socket(socket)
+        self.app_state = app_state
+
+    async def run(
+        self, task_status: trio._core._run._TaskStatus = trio.TASK_STATUS_IGNORED
+    ) -> None:
+        from ..protocol.quic import QuicProtocol  # h3/Quic is an optional part of Hypercorn
+
+        task_status.started()
+        server = parse_socket_addr(self.socket.family, self.socket.getsockname())
+        async with TaskGroup() as task_group:
+            self.protocol = QuicProtocol(
+                self.app, self.config, self.context, task_group, server, self.protocol_send, self.app_state
+            )
+
+            while not self.context.terminated.is_set() or not self.protocol.idle:
+                data, address = await self.socket.recvfrom(MAX_RECV)
+                await self.protocol.handle(RawData(data=data, address=address))
+
+    async def protocol_send(self, event: Event) -> None:
+        if isinstance(event, RawData):
+            await self.socket.sendto(event.data, event.address)
```

### Comparing `nonecorn-0.14.1.dev1/src/hypercorn/trio/worker_context.py` & `nonecorn-0.14.3.dev1/src/hypercorn/trio/worker_context.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-from __future__ import annotations
-
-from typing import Type, Union
-
-import trio
-
-from ..typing import Event
-
-
-class EventWrapper:
-    def __init__(self) -> None:
-        self._event = trio.Event()
-
-    async def clear(self) -> None:
-        self._event = trio.Event()
-
-    async def wait(self) -> None:
-        await self._event.wait()
-
-    async def set(self) -> None:
-        self._event.set()
-
-    def is_set(self) -> bool:
-        return self._event.is_set()
-
-
-class WorkerContext:
-    event_class: Type[Event] = EventWrapper
-
-    def __init__(self) -> None:
-        self.terminated = self.event_class()
-
-    @staticmethod
-    async def sleep(wait: Union[float, int]) -> None:
-        return await trio.sleep(wait)
-
-    @staticmethod
-    def time() -> float:
-        return trio.current_time()
+from __future__ import annotations
+
+from typing import Type, Union
+
+import trio
+
+from ..typing import Event
+
+
+class EventWrapper:
+    def __init__(self) -> None:
+        self._event = trio.Event()
+
+    async def clear(self) -> None:
+        self._event = trio.Event()
+
+    async def wait(self) -> None:
+        await self._event.wait()
+
+    async def set(self) -> None:
+        self._event.set()
+
+    def is_set(self) -> bool:
+        return self._event.is_set()
+
+
+class WorkerContext:
+    event_class: Type[Event] = EventWrapper
+
+    def __init__(self) -> None:
+        self.terminated = self.event_class()
+
+    @staticmethod
+    async def sleep(wait: Union[float, int]) -> None:
+        return await trio.sleep(wait)
+
+    @staticmethod
+    def time() -> float:
+        return trio.current_time()
```

### Comparing `nonecorn-0.14.1.dev1/src/hypercorn/typing.py` & `nonecorn-0.14.3.dev1/src/hypercorn/typing.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,347 +1,349 @@
-from __future__ import annotations
-
-from multiprocessing.synchronize import Event as EventType
-from types import TracebackType
-from typing import Any, Awaitable, Callable, Dict, Iterable, Optional, Tuple, Type, Union
-
-import h2.events
-import h11
-
-# Till PEP 544 is accepted
-try:
-    from typing import Literal, Protocol, TypedDict
-except ImportError:
-    from typing_extensions import Literal, Protocol, TypedDict  # type: ignore
-
-from .config import Config, Sockets
-
-H11SendableEvent = Union[h11.Data, h11.EndOfMessage, h11.InformationalResponse, h11.Response]
-
-WorkerFunc = Callable[[Config, Optional[Sockets], Optional[EventType]], None]
-
-
-class ASGIVersions(TypedDict, total=False):
-    spec_version: str
-    version: Union[Literal["2.0"], Literal["3.0"]]
-
-
-class HTTPScope(TypedDict):
-    type: Literal["http"]
-    asgi: ASGIVersions
-    http_version: str
-    method: str
-    scheme: str
-    path: str
-    raw_path: bytes
-    query_string: bytes
-    root_path: str
-    headers: Iterable[Tuple[bytes, bytes]]
-    client: Optional[Tuple[str, int]]
-    server: Optional[Tuple[str, Optional[int]]]
-    extensions: Dict[str, dict]
-
-
-class WebsocketScope(TypedDict):
-    type: Literal["websocket"]
-    asgi: ASGIVersions
-    http_version: str
-    scheme: str
-    path: str
-    raw_path: bytes
-    query_string: bytes
-    root_path: str
-    headers: Iterable[Tuple[bytes, bytes]]
-    client: Optional[Tuple[str, int]]
-    server: Optional[Tuple[str, Optional[int]]]
-    subprotocols: Iterable[str]
-    extensions: Dict[str, dict]
-
-
-class LifespanScope(TypedDict):
-    type: Literal["lifespan"]
-    asgi: ASGIVersions
-
-
-WWWScope = Union[HTTPScope, WebsocketScope]
-Scope = Union[HTTPScope, WebsocketScope, LifespanScope]
-
-
-class HTTPRequestEvent(TypedDict):
-    type: Literal["http.request"]
-    body: bytes
-    more_body: bool
-
-
-class HTTPResponseStartEvent(TypedDict):
-    type: Literal["http.response.start"]
-    status: int
-    headers: Iterable[Tuple[bytes, bytes]]
-    meta: dict
-
-
-class HTTPResponseBodyEvent(TypedDict):
-    type: Literal["http.response.body"]
-    body: bytes
-    more_body: bool
-    headers: Optional[Iterable[Tuple[bytes, bytes]]] = None
-    meta: dict
-
-
-class HTTPServerPushEvent(TypedDict):
-    type: Literal["http.response.push"]
-    path: str
-    headers: Iterable[Tuple[bytes, bytes]]
-
-
-class HTTPZeroCopySendEvent(TypedDict):
-    type: Literal["http.response.zerocopysend"]
-    file: int
-    offset: Optional[int]
-    count: Optional[int]
-    more_body: Optional[bool]
-
-
-class HTTPTrailerHeadersSendEvent(TypedDict):
-    type: Literal["http.response.trailers"]  # todo
-    headers: Iterable[Tuple[bytes, bytes]]
-    more_body: Optional[bool] = False
-
-
-class HTTPEarlyHintEvent(TypedDict):
-    type: Literal["http.response.early_hint"]
-    links: Iterable[bytes]
-
-
-class HTTPDisconnectEvent(TypedDict):
-    type: Literal["http.disconnect"]
-
-
-class WebsocketConnectEvent(TypedDict):
-    type: Literal["websocket.connect"]
-
-
-class WebsocketAcceptEvent(TypedDict):
-    type: Literal["websocket.accept"]
-    subprotocol: Optional[str]
-    headers: Iterable[Tuple[bytes, bytes]]
-
-
-class WebsocketReceiveEvent(TypedDict):
-    type: Literal["websocket.receive"]
-    bytes: Optional[bytes]
-    text: Optional[str]
-
-
-class WebsocketSendEvent(TypedDict):
-    type: Literal["websocket.send"]
-    bytes: Optional[bytes]
-    text: Optional[str]
-
-
-class WebsocketResponseStartEvent(TypedDict):
-    type: Literal["websocket.http.response.start"]
-    status: int
-    headers: Iterable[Tuple[bytes, bytes]]
-
-
-class WebsocketResponseBodyEvent(TypedDict):
-    type: Literal["websocket.http.response.body"]
-    body: bytes
-    more_body: bool
-
-
-class WebsocketDisconnectEvent(TypedDict):
-    type: Literal["websocket.disconnect"]
-    code: int
-
-
-class WebsocketCloseEvent(TypedDict):
-    type: Literal["websocket.close"]
-    code: int
-    reason: Optional[str]
-
-
-class LifespanStartupEvent(TypedDict):
-    type: Literal["lifespan.startup"]
-
-
-class LifespanShutdownEvent(TypedDict):
-    type: Literal["lifespan.shutdown"]
-
-
-class LifespanStartupCompleteEvent(TypedDict):
-    type: Literal["lifespan.startup.complete"]
-
-
-class LifespanStartupFailedEvent(TypedDict):
-    type: Literal["lifespan.startup.failed"]
-    message: str
-
-
-class LifespanShutdownCompleteEvent(TypedDict):
-    type: Literal["lifespan.shutdown.complete"]
-
-
-class LifespanShutdownFailedEvent(TypedDict):
-    type: Literal["lifespan.shutdown.failed"]
-    message: str
-
-
-ASGIReceiveEvent = Union[
-    HTTPRequestEvent,
-    HTTPDisconnectEvent,
-    WebsocketConnectEvent,
-    WebsocketReceiveEvent,
-    WebsocketDisconnectEvent,
-    LifespanStartupEvent,
-    LifespanShutdownEvent,
-]
-
-ASGISendEvent = Union[
-    HTTPResponseStartEvent,
-    HTTPResponseBodyEvent,
-    HTTPServerPushEvent,
-    HTTPZeroCopySendEvent,
-    HTTPTrailerHeadersSendEvent,
-    HTTPEarlyHintEvent,
-    HTTPDisconnectEvent,
-    WebsocketAcceptEvent,
-    WebsocketSendEvent,
-    WebsocketResponseStartEvent,
-    WebsocketResponseBodyEvent,
-    WebsocketCloseEvent,
-    LifespanStartupCompleteEvent,
-    LifespanStartupFailedEvent,
-    LifespanShutdownCompleteEvent,
-    LifespanShutdownFailedEvent,
-]
-
-ASGIReceiveCallable = Callable[[], Awaitable[ASGIReceiveEvent]]
-ASGISendCallable = Callable[[ASGISendEvent], Awaitable[None]]
-
-ASGIFramework = Callable[
-    [
-        Scope,
-        ASGIReceiveCallable,
-        ASGISendCallable,
-    ],
-    Awaitable[None],
-]
-WSGIFramework = Callable[[dict, Callable], Iterable[bytes]]
-Framework = Union[ASGIFramework, WSGIFramework]
-
-
-class H2SyncStream(Protocol):
-    scope: dict
-
-    def data_received(self, data: bytes) -> None:
-        ...
-
-    def ended(self) -> None:
-        ...
-
-    def reset(self) -> None:
-        ...
-
-    def close(self) -> None:
-        ...
-
-    async def handle_request(
-        self,
-        event: h2.events.RequestReceived,
-        scheme: str,
-        client: Tuple[str, int],
-        server: Tuple[str, int],
-    ) -> None:
-        ...
-
-
-class H2AsyncStream(Protocol):
-    scope: dict
-
-    async def data_received(self, data: bytes) -> None:
-        ...
-
-    async def ended(self) -> None:
-        ...
-
-    async def reset(self) -> None:
-        ...
-
-    async def close(self) -> None:
-        ...
-
-    async def handle_request(
-        self,
-        event: h2.events.RequestReceived,
-        scheme: str,
-        client: Tuple[str, int],
-        server: Tuple[str, int],
-    ) -> None:
-        ...
-
-
-class Event(Protocol):
-    def __init__(self) -> None:
-        ...
-
-    async def clear(self) -> None:
-        ...
-
-    async def set(self) -> None:
-        ...
-
-    async def wait(self) -> None:
-        ...
-
-    def is_set(self) -> bool:
-        ...
-
-
-class WorkerContext(Protocol):
-    event_class: Type[Event]
-    terminated: Event
-
-    @staticmethod
-    async def sleep(wait: Union[float, int]) -> None:
-        ...
-
-    @staticmethod
-    def time() -> float:
-        ...
-
-
-class TaskGroup(Protocol):
-    async def spawn_app(
-        self,
-        app: AppWrapper,
-        config: Config,
-        scope: Scope,
-        send: Callable[[Optional[ASGISendEvent]], Awaitable[None]],
-    ) -> Callable[[ASGIReceiveEvent], Awaitable[None]]:
-        ...
-
-    def spawn(self, func: Callable, *args: Any) -> None:
-        ...
-
-    async def __aenter__(self) -> TaskGroup:
-        ...
-
-    async def __aexit__(self, exc_type: type, exc_value: BaseException, tb: TracebackType) -> None:
-        ...
-
-
-class ResponseSummary(TypedDict):
-    status: int
-    headers: Iterable[Tuple[bytes, bytes]]
-
-
-class AppWrapper(Protocol):
-    async def __call__(
-        self,
-        scope: Scope,
-        receive: ASGIReceiveCallable,
-        send: ASGISendCallable,
-        sync_spawn: Callable,
-    ) -> None:
-        ...
+from __future__ import annotations
+
+from multiprocessing.synchronize import Event as EventType
+from types import TracebackType
+from typing import Any, Awaitable, Callable, Dict, Iterable, Optional, Tuple, Type, Union
+
+import h2.events
+import h11
+
+# Till PEP 544 is accepted
+try:
+    from typing import Literal, Protocol, TypedDict
+except ImportError:
+    from typing_extensions import Literal, Protocol, TypedDict  # type: ignore
+
+from .config import Config, Sockets
+
+H11SendableEvent = Union[h11.Data, h11.EndOfMessage, h11.InformationalResponse, h11.Response]
+
+WorkerFunc = Callable[[Config, Optional[Sockets], Optional[EventType]], None]
+
+
+class ASGIVersions(TypedDict, total=False):
+    spec_version: str
+    version: Union[Literal["2.0"], Literal["3.0"]]
+
+
+class HTTPScope(TypedDict):
+    type: Literal["http"]
+    asgi: ASGIVersions
+    http_version: str
+    method: str
+    scheme: str
+    path: str
+    raw_path: bytes
+    query_string: bytes
+    root_path: str
+    headers: Iterable[Tuple[bytes, bytes]]
+    client: Optional[Tuple[str, int]]
+    server: Optional[Tuple[str, Optional[int]]]
+    extensions: Dict[str, dict]
+    state: Dict[str, Any]
+
+
+class WebsocketScope(TypedDict):
+    type: Literal["websocket"]
+    asgi: ASGIVersions
+    http_version: str
+    scheme: str
+    path: str
+    raw_path: bytes
+    query_string: bytes
+    root_path: str
+    headers: Iterable[Tuple[bytes, bytes]]
+    client: Optional[Tuple[str, int]]
+    server: Optional[Tuple[str, Optional[int]]]
+    subprotocols: Iterable[str]
+    extensions: Dict[str, dict]
+    state: Dict[str, Any]
+
+
+class LifespanScope(TypedDict):
+    type: Literal["lifespan"]
+    asgi: ASGIVersions
+    state: Dict[str, Any]
+
+
+WWWScope = Union[HTTPScope, WebsocketScope]
+Scope = Union[HTTPScope, WebsocketScope, LifespanScope]
+
+
+class HTTPRequestEvent(TypedDict):
+    type: Literal["http.request"]
+    body: bytes
+    more_body: bool
+
+
+class HTTPResponseStartEvent(TypedDict):
+    type: Literal["http.response.start"]
+    status: int
+    headers: Iterable[Tuple[bytes, bytes]]
+    trailers: bool
+
+class HTTPResponseBodyEvent(TypedDict):
+    type: Literal["http.response.body"]
+    body: bytes
+    more_body: bool
+    headers: Optional[Iterable[Tuple[bytes, bytes]]] = None
+
+
+class HTTPServerPushEvent(TypedDict):
+    type: Literal["http.response.push"]
+    path: str
+    headers: Iterable[Tuple[bytes, bytes]]
+
+
+class HTTPZeroCopySendEvent(TypedDict):
+    type: Literal["http.response.zerocopysend"]
+    file: int
+    offset: Optional[int]
+    count: Optional[int]
+    more_body: Optional[bool]
+
+
+class HTTPResponseTrailersEvent(TypedDict):
+    type: Literal["http.response.trailers"]
+    headers: Iterable[Tuple[bytes, bytes]]
+    more_trailers: bool
+
+
+class HTTPEarlyHintEvent(TypedDict):
+    type: Literal["http.response.early_hint"]
+    links: Iterable[bytes]
+
+
+class HTTPDisconnectEvent(TypedDict):
+    type: Literal["http.disconnect"]
+
+
+class WebsocketConnectEvent(TypedDict):
+    type: Literal["websocket.connect"]
+
+
+class WebsocketAcceptEvent(TypedDict):
+    type: Literal["websocket.accept"]
+    subprotocol: Optional[str]
+    headers: Iterable[Tuple[bytes, bytes]]
+
+
+class WebsocketReceiveEvent(TypedDict):
+    type: Literal["websocket.receive"]
+    bytes: Optional[bytes]
+    text: Optional[str]
+
+
+class WebsocketSendEvent(TypedDict):
+    type: Literal["websocket.send"]
+    bytes: Optional[bytes]
+    text: Optional[str]
+
+
+class WebsocketResponseStartEvent(TypedDict):
+    type: Literal["websocket.http.response.start"]
+    status: int
+    headers: Iterable[Tuple[bytes, bytes]]
+
+
+class WebsocketResponseBodyEvent(TypedDict):
+    type: Literal["websocket.http.response.body"]
+    body: bytes
+    more_body: bool
+
+
+class WebsocketDisconnectEvent(TypedDict):
+    type: Literal["websocket.disconnect"]
+    code: int
+
+
+class WebsocketCloseEvent(TypedDict):
+    type: Literal["websocket.close"]
+    code: int
+    reason: Optional[str]
+
+
+class LifespanStartupEvent(TypedDict):
+    type: Literal["lifespan.startup"]
+
+
+class LifespanShutdownEvent(TypedDict):
+    type: Literal["lifespan.shutdown"]
+
+
+class LifespanStartupCompleteEvent(TypedDict):
+    type: Literal["lifespan.startup.complete"]
+
+
+class LifespanStartupFailedEvent(TypedDict):
+    type: Literal["lifespan.startup.failed"]
+    message: str
+
+
+class LifespanShutdownCompleteEvent(TypedDict):
+    type: Literal["lifespan.shutdown.complete"]
+
+
+class LifespanShutdownFailedEvent(TypedDict):
+    type: Literal["lifespan.shutdown.failed"]
+    message: str
+
+
+ASGIReceiveEvent = Union[
+    HTTPRequestEvent,
+    HTTPDisconnectEvent,
+    WebsocketConnectEvent,
+    WebsocketReceiveEvent,
+    WebsocketDisconnectEvent,
+    LifespanStartupEvent,
+    LifespanShutdownEvent,
+]
+
+ASGISendEvent = Union[
+    HTTPResponseStartEvent,
+    HTTPResponseBodyEvent,
+    HTTPServerPushEvent,
+    HTTPZeroCopySendEvent,
+    HTTPResponseTrailersEvent,
+    HTTPEarlyHintEvent,
+    HTTPDisconnectEvent,
+    WebsocketAcceptEvent,
+    WebsocketSendEvent,
+    WebsocketResponseStartEvent,
+    WebsocketResponseBodyEvent,
+    WebsocketCloseEvent,
+    LifespanStartupCompleteEvent,
+    LifespanStartupFailedEvent,
+    LifespanShutdownCompleteEvent,
+    LifespanShutdownFailedEvent,
+]
+
+ASGIReceiveCallable = Callable[[], Awaitable[ASGIReceiveEvent]]
+ASGISendCallable = Callable[[ASGISendEvent], Awaitable[None]]
+
+ASGIFramework = Callable[
+    [
+        Scope,
+        ASGIReceiveCallable,
+        ASGISendCallable,
+    ],
+    Awaitable[None],
+]
+WSGIFramework = Callable[[dict, Callable], Iterable[bytes]]
+Framework = Union[ASGIFramework, WSGIFramework]
+
+
+class H2SyncStream(Protocol):
+    scope: dict
+
+    def data_received(self, data: bytes) -> None:
+        ...
+
+    def ended(self) -> None:
+        ...
+
+    def reset(self) -> None:
+        ...
+
+    def close(self) -> None:
+        ...
+
+    async def handle_request(
+        self,
+        event: h2.events.RequestReceived,
+        scheme: str,
+        client: Tuple[str, int],
+        server: Tuple[str, int],
+    ) -> None:
+        ...
+
+
+class H2AsyncStream(Protocol):
+    scope: dict
+
+    async def data_received(self, data: bytes) -> None:
+        ...
+
+    async def ended(self) -> None:
+        ...
+
+    async def reset(self) -> None:
+        ...
+
+    async def close(self) -> None:
+        ...
+
+    async def handle_request(
+        self,
+        event: h2.events.RequestReceived,
+        scheme: str,
+        client: Tuple[str, int],
+        server: Tuple[str, int],
+    ) -> None:
+        ...
+
+
+class Event(Protocol):
+    def __init__(self) -> None:
+        ...
+
+    async def clear(self) -> None:
+        ...
+
+    async def set(self) -> None:
+        ...
+
+    async def wait(self) -> None:
+        ...
+
+    def is_set(self) -> bool:
+        ...
+
+
+class WorkerContext(Protocol):
+    event_class: Type[Event]
+    terminated: Event
+
+    @staticmethod
+    async def sleep(wait: Union[float, int]) -> None:
+        ...
+
+    @staticmethod
+    def time() -> float:
+        ...
+
+
+class TaskGroup(Protocol):
+    async def spawn_app(
+        self,
+        app: AppWrapper,
+        config: Config,
+        scope: Scope,
+        send: Callable[[Optional[ASGISendEvent]], Awaitable[None]],
+    ) -> Callable[[ASGIReceiveEvent], Awaitable[None]]:
+        ...
+
+    def spawn(self, func: Callable, *args: Any) -> None:
+        ...
+
+    async def __aenter__(self) -> TaskGroup:
+        ...
+
+    async def __aexit__(self, exc_type: type, exc_value: BaseException, tb: TracebackType) -> None:
+        ...
+
+
+class ResponseSummary(TypedDict):
+    status: int
+    headers: Iterable[Tuple[bytes, bytes]]
+
+
+class AppWrapper(Protocol):
+    async def __call__(
+        self,
+        scope: Scope,
+        receive: ASGIReceiveCallable,
+        send: ASGISendCallable,
+        sync_spawn: Callable,
+        call_soon: Callable,
+    ) -> None:
+        ...
```

### Comparing `nonecorn-0.14.1.dev1/src/hypercorn/utils.py` & `nonecorn-0.14.3.dev1/src/hypercorn/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,324 +1,325 @@
-from __future__ import annotations
-
-import asyncio
-import inspect
-import os
-import socket
-import ssl
-import sys
-import time
-from enum import Enum
-from functools import lru_cache
-from importlib import import_module
-from multiprocessing.synchronize import Event as EventType
-from pathlib import Path
-from typing import (
-    Any,
-    Awaitable,
-    Callable,
-    cast,
-    Dict,
-    Iterable,
-    List,
-    Optional,
-    Tuple,
-    TYPE_CHECKING,
-)
-
-try:
-    from uvloop import Loop
-except ImportError:
-    Loop = None
-
-from .app_wrappers import ASGIWrapper, WSGIWrapper
-from .config import Config
-from .typing import AppWrapper, ASGIFramework, Framework, WSGIFramework
-
-try:
-    from typing import Literal
-except ImportError:
-    from typing_extensions import Literal  # type: ignore
-
-if TYPE_CHECKING:
-    from .protocol.events import Request
-
-
-class ShutdownError(Exception):
-    pass
-
-
-class NoAppError(Exception):
-    pass
-
-
-class LifespanTimeoutError(Exception):
-    def __init__(self, stage: str) -> None:
-        super().__init__(
-            f"Timeout whilst awaiting {stage}. Your application may not support the ASGI Lifespan "
-            f"protocol correctly, alternatively the {stage}_timeout configuration is incorrect."
-        )
-
-
-class LifespanFailureError(Exception):
-    def __init__(self, stage: str, message: str) -> None:
-        super().__init__(f"Lifespan failure in {stage}. '{message}'")
-
-
-class UnexpectedMessageError(Exception):
-    def __init__(self, state: Enum, message_type: str) -> None:
-        super().__init__(f"Unexpected message type, {message_type} given the state {state}")
-
-
-class FrameTooLargeError(Exception):
-    pass
-
-
-def suppress_body(method: str, status_code: int) -> bool:
-    return method == "HEAD" or 100 <= status_code < 200 or status_code in {204, 304}
-
-
-def build_and_validate_headers(headers: Iterable[Tuple[bytes, bytes]]) -> List[Tuple[bytes, bytes]]:
-    # Validates that the header name and value are bytes
-    validated_headers: List[Tuple[bytes, bytes]] = []
-    for name, value in headers:
-        if name[0] == b":"[0]:
-            raise ValueError("Pseudo headers are not valid")
-        validated_headers.append((bytes(name).strip(), bytes(value).strip()))
-    return validated_headers
-
-
-def filter_pseudo_headers(headers: List[Tuple[bytes, bytes]]) -> List[Tuple[bytes, bytes]]:
-    filtered_headers: List[Tuple[bytes, bytes]] = [(b"host", b"")]  # Placeholder
-    authority = None
-    host = b""
-    for name, value in headers:
-        if name == b":authority":  # h2 & h3 libraries validate this is present
-            authority = value
-        elif name == b"host":
-            host = value
-        elif name[0] != b":"[0]:
-            filtered_headers.append((name, value))
-    filtered_headers[0] = (b"host", authority if authority is not None else host)
-    return filtered_headers
-
-
-def load_application(path: str, wsgi_max_body_size: int) -> AppWrapper:
-    mode: Optional[Literal["asgi", "wsgi"]] = None
-    if ":" not in path:
-        module_name, app_name = path, "app"
-    elif path.count(":") == 2:
-        mode, module_name, app_name = path.split(":", 2)  # type: ignore
-        if mode not in {"asgi", "wsgi"}:
-            raise ValueError("Invalid mode, must be 'asgi', or 'wsgi'")
-    else:
-        module_name, app_name = path.split(":", 1)
-
-    module_path = Path(module_name).resolve()
-    sys.path.insert(0, str(module_path.parent))
-    if module_path.is_file():
-        import_name = module_path.with_suffix("").name
-    else:
-        import_name = module_path.name
-    try:
-        module = import_module(import_name)
-    except ModuleNotFoundError as error:
-        if error.name == import_name:
-            raise NoAppError()
-        else:
-            raise
-    try:
-        app = eval(app_name, vars(module))
-    except NameError:
-        raise NoAppError()
-    else:
-        return wrap_app(app, wsgi_max_body_size, mode)
-
-
-def wrap_app(
-    app: Framework, wsgi_max_body_size: int, mode: Optional[Literal["asgi", "wsgi"]]
-) -> AppWrapper:
-    if mode is None:
-        mode = "asgi" if is_asgi(app) else "wsgi"
-    if mode == "asgi":
-        return ASGIWrapper(cast(ASGIFramework, app))
-    else:
-        return WSGIWrapper(cast(WSGIFramework, app), wsgi_max_body_size)
-
-
-def wait_for_changes(shutdown_event: EventType) -> None:
-    last_updates: Dict[Path, float] = {}
-    for module in list(sys.modules.values()):
-        filename = getattr(module, "__file__", None)
-        if filename is None:
-            continue
-        path = Path(filename)
-        try:
-            last_updates[Path(filename)] = path.stat().st_mtime
-        except (FileNotFoundError, NotADirectoryError):
-            pass
-
-    while not shutdown_event.is_set():
-        time.sleep(1)
-
-        for index, (path, last_mtime) in enumerate(last_updates.items()):
-            if index % 10 == 0:
-                # Yield to the event loop
-                time.sleep(0)
-
-            try:
-                mtime = path.stat().st_mtime
-            except FileNotFoundError:
-                return
-            else:
-                if mtime > last_mtime:
-                    return
-                else:
-                    last_updates[path] = mtime
-
-
-async def raise_shutdown(shutdown_event: Callable[..., Awaitable[None]]) -> None:
-    await shutdown_event()
-    raise ShutdownError()
-
-
-async def check_multiprocess_shutdown_event(
-    shutdown_event: EventType, sleep: Callable[[float], Awaitable[Any]]
-) -> None:
-    while True:
-        if shutdown_event.is_set():
-            return
-        await sleep(0.1)
-
-
-def write_pid_file(pid_path: str) -> None:
-    with open(pid_path, "w") as file_:
-        file_.write(f"{os.getpid()}")
-
-
-def parse_socket_addr(family: int, address: tuple) -> Optional[Tuple[str, int]]:
-    if family == socket.AF_INET:
-        return address  # type: ignore
-    elif family == socket.AF_INET6:
-        return (address[0], address[1])
-    else:
-        return None
-
-
-def repr_socket_addr(family: int, address: tuple) -> str:
-    if family == socket.AF_INET:
-        return f"{address[0]}:{address[1]}"
-    elif family == socket.AF_INET6:
-        return f"[{address[0]}]:{address[1]}"
-    elif family == socket.AF_UNIX:
-        return f"unix:{address}"
-    else:
-        return f"{address}"
-
-
-def valid_server_name(config: Config, request: "Request") -> bool:
-    if len(config.server_names) == 0:
-        return True
-
-    host = ""
-    for name, value in request.headers:
-        if name.lower() == b"host":
-            host = value.decode()
-            break
-    return host in config.server_names
-
-
-RDNS_MAPPING: Dict[str, str] = {
-    "commonName": "CN",
-    "localityName": "L",
-    "stateOrProvinceName": "ST",
-    "organizationName": "O",
-    "organizationalUnitName": "OU",
-    "countryName": "C",
-    "streetAddress": "STREET",
-    "domainComponent": "DC",
-    "userId": "UID",
-}
-
-TLS_VERSION_MAP: Dict[str, int] = {
-    "TLSv1": 0x0301,
-    "TLSv1.1": 0x0302,
-    "TLSv1.2": 0x0303,
-    "TLSv1.3": 0x0304,
-}
-
-
-def get_tls_info(writer: asyncio.StreamWriter) -> Optional[Dict]:
-    """
-    # server_cert: Unable to set from transport information
-    # client_cert_chain: Just the peercert, currently no access to the full cert chain
-    # client_cert_name:
-    # client_cert_error: No access to this
-    # tls_version:
-    # cipher_suite: Too hard to convert without direct access to openssl
-    """
-    ssl_info: Dict[str, Any] = {
-        "server_cert": None,
-        "client_cert_chain": [],
-        "client_cert_name": None,
-        "client_cert_error": None,
-        "tls_version": None,
-        "cipher_suite": None,
-    }
-
-    ssl_object = writer.get_extra_info("ssl_object", default=None)
-    peercert = ssl_object.getpeercert()
-
-    if peercert:
-        rdn_strings = []
-        for rdn in peercert["subject"]:
-            rdn_strings.append(
-                "+".join(
-                    [
-                        "%s = %s" % (RDNS_MAPPING[entry[0]], entry[1])
-                        for entry in reversed(rdn)
-                        if entry[0] in RDNS_MAPPING
-                    ]
-                )
-            )
-        ssl_info["client_cert_chain"] = [
-            ssl.DER_cert_to_PEM_cert(ssl_object.getpeercert(binary_form=True))
-        ]
-        ssl_info["client_cert_name"] = ", ".join(rdn_strings) if rdn_strings else ""
-        ssl_info["tls_version"] = (
-            TLS_VERSION_MAP[ssl_object.version()]
-            if ssl_object.version() in TLS_VERSION_MAP
-            else None
-        )
-        ssl_info["cipher_suite"] = list(ssl_object.cipher())
-        return ssl_info
-    return None
-
-
-def is_ssl(transport: asyncio.Transport) -> bool:
-    return bool(transport.get_extra_info("sslcontext"))
-
-
-def check_uvloop(loop) -> bool:
-    return isinstance(loop, Loop) if Loop else False
-
-
-@lru_cache(2, typed=False)
-def can_sendfile(loop: asyncio.AbstractEventLoop, https: bool = False) -> bool:
-    """
-    Judge loop.sendfile available. Uvloop not included.
-    """
-    return (
-        sys.version_info[:2] >= (3, 7)
-        and (
-            (hasattr(asyncio, "ProactorEventLoop") and isinstance(loop, asyncio.ProactorEventLoop))
-            or (isinstance(loop, asyncio.SelectorEventLoop) and hasattr(os, "sendfile"))
-        )
-        and not https
-    )
-
-def is_asgi(app: Any) -> bool:
-    if inspect.iscoroutinefunction(app):
-        return True
-    elif hasattr(app, "__call__"):
-        return inspect.iscoroutinefunction(app.__call__)
-    return False
+from __future__ import annotations
+
+import asyncio
+import inspect
+import os
+import socket
+import ssl
+import sys
+import time
+from enum import Enum
+from functools import lru_cache
+from importlib import import_module
+from multiprocessing.synchronize import Event as EventType
+from pathlib import Path
+from typing import (
+    Any,
+    Awaitable,
+    Callable,
+    cast,
+    Dict,
+    Iterable,
+    List,
+    Optional,
+    Tuple,
+    TYPE_CHECKING,
+)
+
+try:
+    from uvloop import Loop
+except ImportError:
+    Loop = None
+
+from .app_wrappers import ASGIWrapper, WSGIWrapper
+from .config import Config
+from .typing import AppWrapper, ASGIFramework, Framework, WSGIFramework
+
+try:
+    from typing import Literal
+except ImportError:
+    from typing_extensions import Literal  # type: ignore
+
+if TYPE_CHECKING:
+    from .protocol.events import Request
+
+
+class ShutdownError(Exception):
+    pass
+
+
+class NoAppError(Exception):
+    pass
+
+
+class LifespanTimeoutError(Exception):
+    def __init__(self, stage: str) -> None:
+        super().__init__(
+            f"Timeout whilst awaiting {stage}. Your application may not support the ASGI Lifespan "
+            f"protocol correctly, alternatively the {stage}_timeout configuration is incorrect."
+        )
+
+
+class LifespanFailureError(Exception):
+    def __init__(self, stage: str, message: str) -> None:
+        super().__init__(f"Lifespan failure in {stage}. '{message}'")
+
+
+class UnexpectedMessageError(Exception):
+    def __init__(self, state: Enum, message_type: str) -> None:
+        super().__init__(f"Unexpected message type, {message_type} given the state {state}")
+
+
+class FrameTooLargeError(Exception):
+    pass
+
+
+def suppress_body(method: str, status_code: int) -> bool:
+    return method == "HEAD" or 100 <= status_code < 200 or status_code in {204, 304}
+
+
+def build_and_validate_headers(headers: Iterable[Tuple[bytes, bytes]]) -> List[Tuple[bytes, bytes]]:
+    # Validates that the header name and value are bytes
+    validated_headers: List[Tuple[bytes, bytes]] = []
+    for name, value in headers:
+        if name[0] == b":"[0]:
+            raise ValueError("Pseudo headers are not valid")
+        validated_headers.append((bytes(name).strip(), bytes(value).strip()))
+    return validated_headers
+
+
+def filter_pseudo_headers(headers: List[Tuple[bytes, bytes]]) -> List[Tuple[bytes, bytes]]:
+    filtered_headers: List[Tuple[bytes, bytes]] = [(b"host", b"")]  # Placeholder
+    authority = None
+    host = b""
+    for name, value in headers:
+        if name == b":authority":  # h2 & h3 libraries validate this is present
+            authority = value
+        elif name == b"host":
+            host = value
+        elif name[0] != b":"[0]:
+            filtered_headers.append((name, value))
+    filtered_headers[0] = (b"host", authority if authority is not None else host)
+    return filtered_headers
+
+
+def load_application(path: str, wsgi_max_body_size: int) -> AppWrapper:
+    mode: Optional[Literal["asgi", "wsgi"]] = None
+    if ":" not in path:
+        module_name, app_name = path, "app"
+    elif path.count(":") == 2:
+        mode, module_name, app_name = path.split(":", 2)  # type: ignore
+        if mode not in {"asgi", "wsgi"}:
+            raise ValueError("Invalid mode, must be 'asgi', or 'wsgi'")
+    else:
+        module_name, app_name = path.split(":", 1)
+
+    module_path = Path(module_name).resolve()
+    sys.path.insert(0, str(module_path.parent))
+    if module_path.is_file():
+        import_name = module_path.with_suffix("").name
+    else:
+        import_name = module_path.name
+    try:
+        module = import_module(import_name)
+    except ModuleNotFoundError as error:
+        if error.name == import_name:
+            raise NoAppError()
+        else:
+            raise
+    try:
+        app = eval(app_name, vars(module))
+    except NameError:
+        raise NoAppError()
+    else:
+        return wrap_app(app, wsgi_max_body_size, mode)
+
+
+def wrap_app(
+    app: Framework, wsgi_max_body_size: int, mode: Optional[Literal["asgi", "wsgi"]]
+) -> AppWrapper:
+    if mode is None:
+        mode = "asgi" if is_asgi(app) else "wsgi"
+    if mode == "asgi":
+        return ASGIWrapper(cast(ASGIFramework, app))
+    else:
+        return WSGIWrapper(cast(WSGIFramework, app), wsgi_max_body_size)
+
+
+def wait_for_changes(shutdown_event: EventType) -> None:
+    last_updates: Dict[Path, float] = {}
+    for module in list(sys.modules.values()):
+        filename = getattr(module, "__file__", None)
+        if filename is None:
+            continue
+        path = Path(filename)
+        try:
+            last_updates[Path(filename)] = path.stat().st_mtime
+        except (FileNotFoundError, NotADirectoryError):
+            pass
+
+    while not shutdown_event.is_set():
+        time.sleep(1)
+
+        for index, (path, last_mtime) in enumerate(last_updates.items()):
+            if index % 10 == 0:
+                # Yield to the event loop
+                time.sleep(0)
+
+            try:
+                mtime = path.stat().st_mtime
+            except FileNotFoundError:
+                return
+            else:
+                if mtime > last_mtime:
+                    return
+                else:
+                    last_updates[path] = mtime
+
+
+async def raise_shutdown(shutdown_event: Callable[..., Awaitable[None]]) -> None:
+    await shutdown_event()
+    raise ShutdownError()
+
+
+async def check_multiprocess_shutdown_event(
+    shutdown_event: EventType, sleep: Callable[[float], Awaitable[Any]]
+) -> None:
+    while True:
+        if shutdown_event.is_set():
+            return
+        await sleep(0.1)
+
+
+def write_pid_file(pid_path: str) -> None:
+    with open(pid_path, "w") as file_:
+        file_.write(f"{os.getpid()}")
+
+
+def parse_socket_addr(family: int, address: tuple) -> Optional[Tuple[str, int]]:
+    if family == socket.AF_INET:
+        return address  # type: ignore
+    elif family == socket.AF_INET6:
+        return (address[0], address[1])
+    else:
+        return None
+
+
+def repr_socket_addr(family: int, address: tuple) -> str:
+    if family == socket.AF_INET:
+        return f"{address[0]}:{address[1]}"
+    elif family == socket.AF_INET6:
+        return f"[{address[0]}]:{address[1]}"
+    elif family == socket.AF_UNIX:
+        return f"unix:{address}"
+    else:
+        return f"{address}"
+
+
+def valid_server_name(config: Config, request: "Request") -> bool:
+    if len(config.server_names) == 0:
+        return True
+
+    host = ""
+    for name, value in request.headers:
+        if name.lower() == b"host":
+            host = value.decode()
+            break
+    return host in config.server_names
+
+
+RDNS_MAPPING: Dict[str, str] = {
+    "commonName": "CN",
+    "localityName": "L",
+    "stateOrProvinceName": "ST",
+    "organizationName": "O",
+    "organizationalUnitName": "OU",
+    "countryName": "C",
+    "streetAddress": "STREET",
+    "domainComponent": "DC",
+    "userId": "UID",
+}
+
+TLS_VERSION_MAP: Dict[str, int] = {
+    "TLSv1": 0x0301,
+    "TLSv1.1": 0x0302,
+    "TLSv1.2": 0x0303,
+    "TLSv1.3": 0x0304,
+}
+
+
+def get_tls_info(writer: asyncio.StreamWriter) -> Optional[Dict]:
+    """
+    # server_cert: Unable to set from transport information
+    # client_cert_chain: Just the peercert, currently no access to the full cert chain
+    # client_cert_name:
+    # client_cert_error: No access to this
+    # tls_version:
+    # cipher_suite: Too hard to convert without direct access to openssl
+    """
+    ssl_info: Dict[str, Any] = {
+        "server_cert": None,
+        "client_cert_chain": [],
+        "client_cert_name": None,
+        "client_cert_error": None,
+        "tls_version": None,
+        "cipher_suite": None,
+    }
+
+    ssl_object = writer.get_extra_info("ssl_object", default=None)
+    peercert = ssl_object.getpeercert()
+
+    if peercert:
+        rdn_strings = []
+        for rdn in peercert["subject"]:
+            rdn_strings.append(
+                "+".join(
+                    [
+                        "%s = %s" % (RDNS_MAPPING[entry[0]], entry[1])
+                        for entry in reversed(rdn)
+                        if entry[0] in RDNS_MAPPING
+                    ]
+                )
+            )
+        ssl_info["client_cert_chain"] = [
+            ssl.DER_cert_to_PEM_cert(ssl_object.getpeercert(binary_form=True))
+        ]
+        ssl_info["client_cert_name"] = ", ".join(rdn_strings) if rdn_strings else ""
+        ssl_info["tls_version"] = (
+            TLS_VERSION_MAP[ssl_object.version()]
+            if ssl_object.version() in TLS_VERSION_MAP
+            else None
+        )
+        ssl_info["cipher_suite"] = list(ssl_object.cipher())
+        return ssl_info
+    return None
+
+
+def is_ssl(transport: asyncio.Transport) -> bool:
+    return bool(transport.get_extra_info("sslcontext"))
+
+
+def check_uvloop(loop) -> bool:
+    return isinstance(loop, Loop) if Loop else False
+
+
+@lru_cache(2, typed=False)
+def can_sendfile(loop: asyncio.AbstractEventLoop, https: bool = False) -> bool:
+    """
+    Judge loop.sendfile available. Uvloop not included.
+    """
+    return (
+        sys.version_info[:2] >= (3, 7)
+        and (
+            (hasattr(asyncio, "ProactorEventLoop") and isinstance(loop, asyncio.ProactorEventLoop))
+            or (isinstance(loop, asyncio.SelectorEventLoop) and hasattr(os, "sendfile"))
+        )
+        and not https
+    )
+
+
+def is_asgi(app: Any) -> bool:
+    if inspect.iscoroutinefunction(app):
+        return True
+    elif hasattr(app, "__call__"):
+        return inspect.iscoroutinefunction(app.__call__)
+    return False
```

### Comparing `nonecorn-0.14.1.dev1/src/nonecorn.egg-info/PKG-INFO` & `nonecorn-0.14.3.dev1/src/nonecorn.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,149 +1,146 @@
-Metadata-Version: 2.1
-Name: nonecorn
-Version: 0.14.1.dev1
-Summary: A ASGI Server forked from hypercorn with more extra feature beyond ASGI
-Home-page: https://gitlab.com/pgjones/hypercorn/
-Author: P G Jones
-Author-email: philip.graham.jones@googlemail.com
-License: MIT
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
-Provides-Extra: h3
-Provides-Extra: tests
-Provides-Extra: trio
-Provides-Extra: uvloop
-License-File: LICENSE
-
-Hypercorn is now hosted at `github.com/pgjones/hypercorn
-<https://github.com/pgjones/hypercorn>`_.
-
-
-Hypercorn
-=========
-
-.. image:: https://github.com/pgjones/hypercorn/raw/main/artwork/logo.png
-   :alt: Hypercorn logo
-
-|Build Status| |docs| |pypi| |http| |python| |license|
-
-Hypercorn is an `ASGI
-<https://github.com/django/asgiref/blob/main/specs/asgi.rst>`_ and
-WSGI web server based on the sans-io hyper, `h11
-<https://github.com/python-hyper/h11>`_, `h2
-<https://github.com/python-hyper/hyper-h2>`_, and `wsproto
-<https://github.com/python-hyper/wsproto>`_ libraries and inspired by
-Gunicorn. Hypercorn supports HTTP/1, HTTP/2, WebSockets (over HTTP/1
-and HTTP/2), ASGI, and WSGI specifications. Hypercorn can utilise
-asyncio, uvloop, or trio worker types.
-
-Hypercorn can optionally serve the current draft of the HTTP/3
-specification using the `aioquic
-<https://github.com/aiortc/aioquic/>`_ library. To enable this install
-the ``h3`` optional extra, ``pip install hypercorn[h3]`` and then
-choose a quic binding e.g. ``hypercorn --quic-bind localhost:4433
-...``.
-
-Hypercorn was initially part of `Quart
-<https://github.com/pgjones/quart>`_ before being separated out into a
-standalone server. Hypercorn forked from version 0.5.0 of Quart.
-
-Quickstart
-----------
-
-Hypercorn can be installed via `pip
-<https://docs.python.org/3/installing/index.html>`_,
-
-.. code-block:: console
-
-    $ pip install hypercorn
-
-and requires Python 3.7.0 or higher.
-
-With hypercorn installed ASGI frameworks (or apps) can be served via
-Hypercorn via the command line,
-
-.. code-block:: console
-
-    $ hypercorn module:app
-
-Alternatively Hypercorn can be used programatically,
-
-.. code-block:: python
-
-    import asyncio
-    from hypercorn.config import Config
-    from hypercorn.asyncio import serve
-
-    from module import app
-
-    asyncio.run(serve(app, Config()))
-
-learn more (including a Trio example of the above) in the `API usage
-<https://hypercorn.readthedocs.io/en/latest/how_to_guides/api_usage.html>`_
-docs.
-
-Contributing
-------------
-
-Hypercorn is developed on `Github
-<https://github.com/pgjones/hypercorn>`_. If you come across an issue,
-or have a feature request please open an `issue
-<https://github.com/pgjones/hypercorn/issues>`_.  If you want to
-contribute a fix or the feature-implementation please do (typo fixes
-welcome), by proposing a `pull request
-<https://github.com/pgjones/hypercorn/merge_requests>`_.
-
-Testing
-~~~~~~~
-
-The best way to test Hypercorn is with `Tox
-<https://tox.readthedocs.io>`_,
-
-.. code-block:: console
-
-    $ pipenv install tox
-    $ tox
-
-this will check the code style and run the tests.
-
-Help
-----
-
-The Hypercorn `documentation <https://hypercorn.readthedocs.io>`_ is
-the best place to start, after that try searching stack overflow, if
-you still can't find an answer please `open an issue
-<https://github.com/pgjones/hypercorn/issues>`_.
-
-
-.. |Build Status| image:: https://github.com/pgjones/hypercorn/actions/workflows/ci.yml/badge.svg
-   :target: https://github.com/pgjones/hypercorn/commits/main
-
-.. |docs| image:: https://img.shields.io/badge/docs-passing-brightgreen.svg
-   :target: https://hypercorn.readthedocs.io
-
-.. |pypi| image:: https://img.shields.io/pypi/v/hypercorn.svg
-   :target: https://pypi.python.org/pypi/Hypercorn/
-
-.. |http| image:: https://img.shields.io/badge/http-1.0,1.1,2-orange.svg
-   :target: https://en.wikipedia.org/wiki/Hypertext_Transfer_Protocol
-
-.. |python| image:: https://img.shields.io/pypi/pyversions/hypercorn.svg
-   :target: https://pypi.python.org/pypi/Hypercorn/
-
-.. |license| image:: https://img.shields.io/badge/license-MIT-blue.svg
-   :target: https://github.com/pgjones/hypercorn/blob/main/LICENSE
-
-
+Metadata-Version: 2.1
+Name: nonecorn
+Version: 0.14.3.dev1
+Summary: A ASGI Server forked from hypercorn with more extra feature beyond ASGI
+Home-page: https://gitlab.com/pgjones/hypercorn/
+Author: P G Jones
+Author-email: philip.graham.jones@googlemail.com
+License: MIT
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.7
+Provides-Extra: h3
+Provides-Extra: tests
+Provides-Extra: trio
+Provides-Extra: uvloop
+License-File: LICENSE
+
+Hypercorn is now hosted at `github.com/pgjones/hypercorn
+<https://github.com/pgjones/hypercorn>`_.
+
+
+Hypercorn
+=========
+
+.. image:: https://github.com/pgjones/hypercorn/raw/main/artwork/logo.png
+   :alt: Hypercorn logo
+
+|Build Status| |docs| |pypi| |http| |python| |license|
+
+Hypercorn is an `ASGI
+<https://github.com/django/asgiref/blob/main/specs/asgi.rst>`_ and
+WSGI web server based on the sans-io hyper, `h11
+<https://github.com/python-hyper/h11>`_, `h2
+<https://github.com/python-hyper/hyper-h2>`_, and `wsproto
+<https://github.com/python-hyper/wsproto>`_ libraries and inspired by
+Gunicorn. Hypercorn supports HTTP/1, HTTP/2, WebSockets (over HTTP/1
+and HTTP/2), ASGI, and WSGI specifications. Hypercorn can utilise
+asyncio, uvloop, or trio worker types.
+
+Hypercorn can optionally serve the current draft of the HTTP/3
+specification using the `aioquic
+<https://github.com/aiortc/aioquic/>`_ library. To enable this install
+the ``h3`` optional extra, ``pip install hypercorn[h3]`` and then
+choose a quic binding e.g. ``hypercorn --quic-bind localhost:4433
+...``.
+
+Hypercorn was initially part of `Quart
+<https://github.com/pgjones/quart>`_ before being separated out into a
+standalone server. Hypercorn forked from version 0.5.0 of Quart.
+
+Quickstart
+----------
+
+Hypercorn can be installed via `pip
+<https://docs.python.org/3/installing/index.html>`_,
+
+.. code-block:: console
+
+    $ pip install hypercorn
+
+and requires Python 3.7.0 or higher.
+
+With hypercorn installed ASGI frameworks (or apps) can be served via
+Hypercorn via the command line,
+
+.. code-block:: console
+
+    $ hypercorn module:app
+
+Alternatively Hypercorn can be used programatically,
+
+.. code-block:: python
+
+    import asyncio
+    from hypercorn.config import Config
+    from hypercorn.asyncio import serve
+
+    from module import app
+
+    asyncio.run(serve(app, Config()))
+
+learn more (including a Trio example of the above) in the `API usage
+<https://hypercorn.readthedocs.io/en/latest/how_to_guides/api_usage.html>`_
+docs.
+
+Contributing
+------------
+
+Hypercorn is developed on `Github
+<https://github.com/pgjones/hypercorn>`_. If you come across an issue,
+or have a feature request please open an `issue
+<https://github.com/pgjones/hypercorn/issues>`_.  If you want to
+contribute a fix or the feature-implementation please do (typo fixes
+welcome), by proposing a `pull request
+<https://github.com/pgjones/hypercorn/merge_requests>`_.
+
+Testing
+~~~~~~~
+
+The best way to test Hypercorn is with `Tox
+<https://tox.readthedocs.io>`_,
+
+.. code-block:: console
+
+    $ pipenv install tox
+    $ tox
+
+this will check the code style and run the tests.
+
+Help
+----
+
+The Hypercorn `documentation <https://hypercorn.readthedocs.io>`_ is
+the best place to start, after that try searching stack overflow, if
+you still can't find an answer please `open an issue
+<https://github.com/pgjones/hypercorn/issues>`_.
+
+
+.. |Build Status| image:: https://github.com/pgjones/hypercorn/actions/workflows/ci.yml/badge.svg
+   :target: https://github.com/pgjones/hypercorn/commits/main
+
+.. |docs| image:: https://img.shields.io/badge/docs-passing-brightgreen.svg
+   :target: https://hypercorn.readthedocs.io
+
+.. |pypi| image:: https://img.shields.io/pypi/v/hypercorn.svg
+   :target: https://pypi.python.org/pypi/Hypercorn/
+
+.. |http| image:: https://img.shields.io/badge/http-1.0,1.1,2-orange.svg
+   :target: https://en.wikipedia.org/wiki/Hypertext_Transfer_Protocol
+
+.. |python| image:: https://img.shields.io/pypi/pyversions/hypercorn.svg
+   :target: https://pypi.python.org/pypi/Hypercorn/
+
+.. |license| image:: https://img.shields.io/badge/license-MIT-blue.svg
+   :target: https://github.com/pgjones/hypercorn/blob/main/LICENSE
```

### Comparing `nonecorn-0.14.1.dev1/src/nonecorn.egg-info/SOURCES.txt` & `nonecorn-0.14.3.dev1/src/nonecorn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

