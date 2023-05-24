# Comparing `tmp/ewoksserver-0.1.0rc0.tar.gz` & `tmp/ewoksserver-0.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ewoksserver-0.1.0rc0.tar", last modified: Tue May 23 16:58:12 2023, max compression
+gzip compressed data, was "dist/ewoksserver-0.1.0rc1.tar", last modified: Wed May 24 09:24:07 2023, max compression
```

## Comparing `ewoksserver-0.1.0rc0.tar` & `ewoksserver-0.1.0rc1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 16:58:12.000000 ewoksserver-0.1.0rc0/
--rw-rw-rw-   0 root         (0) root         (0)     1102 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     2201 2023-05-23 16:58:12.000000 ewoksserver-0.1.0rc0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1468 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1439 2023-05-23 16:58:12.000000 ewoksserver-0.1.0rc0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 16:58:12.000000 ewoksserver-0.1.0rc0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 16:58:12.000000 ewoksserver-0.1.0rc0/src/ewoksserver/
--rw-rw-rw-   0 root         (0) root         (0)       25 2023-05-23 16:55:36.000000 ewoksserver-0.1.0rc0/src/ewoksserver/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 16:58:12.000000 ewoksserver-0.1.0rc0/src/ewoksserver/events/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-23 16:58:06.000000 ewoksserver-0.1.0rc0/src/ewoksserver/events/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1058 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/events/ewoks_events.py
--rw-rw-rw-   0 root         (0) root         (0)     2697 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/events/websocket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 16:58:12.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/
--rw-rw-rw-   0 root         (0) root         (0)      731 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9807 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 16:58:12.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/binary/
--rw-rw-rw-   0 root         (0) root         (0)      413 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/binary/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1140 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/binary/icons.py
--rw-rw-rw-   0 root         (0) root         (0)     3834 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/binary/resource.py
--rw-rw-rw-   0 root         (0) root         (0)     3472 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/binary/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 16:58:12.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/data/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 16:58:12.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/data/icons/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-23 16:58:06.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/data/icons/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1348 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/data/icons/default.png
--rw-rw-rw-   0 root         (0) root         (0)      133 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/data/icons/graphInput.svg
--rw-rw-rw-   0 root         (0) root         (0)      149 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/data/icons/graphOutput.svg
--rw-rw-rw-   0 root         (0) root         (0)     3070 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/data/icons/sum.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 16:58:12.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/data/tasks/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-23 16:58:06.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/data/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      295 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/data/tasks/ewokscore.tests.examples.tasks.sumlist.SumList.json
--rw-rw-rw-   0 root         (0) root         (0)      300 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/data/tasks/ewokscore.tests.examples.tasks.sumtask.SumTask.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 16:58:12.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/data/workflows/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-23 16:58:06.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/data/workflows/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12315 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/data/workflows/demo.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 16:58:12.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/events/
--rw-rw-rw-   0 root         (0) root         (0)      360 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/events/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      880 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/events/resource.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 16:58:12.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/json/
--rw-rw-rw-   0 root         (0) root         (0)      952 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/json/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4691 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/json/resource.py
--rw-rw-rw-   0 root         (0) root         (0)     3052 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/json/tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     3332 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/json/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3371 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/json/workflows.py
--rw-rw-rw-   0 root         (0) root         (0)      403 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     5963 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 16:58:12.000000 ewoksserver-0.1.0rc0/src/ewoksserver/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-23 16:58:06.000000 ewoksserver-0.1.0rc0/src/ewoksserver/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3053 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 16:58:12.000000 ewoksserver-0.1.0rc0/src/ewoksserver/tests/data/
--rw-rw-rw-   0 root         (0) root         (0)      292 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/tests/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2730 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/tests/data/icon1.png
--rw-rw-rw-   0 root         (0) root         (0)      133 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/tests/data/icon1.svg
--rw-rw-rw-   0 root         (0) root         (0)     1698 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/tests/data/icon2.png
--rw-rw-rw-   0 root         (0) root         (0)      493 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/tests/data/icon2.svg
--rw-rw-rw-   0 root         (0) root         (0)       91 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/tests/dummy_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     2040 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/tests/test_data.py
--rw-rw-rw-   0 root         (0) root         (0)     3137 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/tests/test_events.py
--rw-rw-rw-   0 root         (0) root         (0)     1797 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/tests/test_execute.py
--rw-rw-rw-   0 root         (0) root         (0)     2612 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/tests/test_icons.py
--rw-rw-rw-   0 root         (0) root         (0)     5844 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/tests/test_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)      807 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/tests/test_websocket_connection.py
--rw-rw-rw-   0 root         (0) root         (0)     4013 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/tests/test_workflows.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 16:58:12.000000 ewoksserver-0.1.0rc0/src/ewoksserver.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2201 2023-05-23 16:58:12.000000 ewoksserver-0.1.0rc0/src/ewoksserver.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2221 2023-05-23 16:58:12.000000 ewoksserver-0.1.0rc0/src/ewoksserver.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 16:58:12.000000 ewoksserver-0.1.0rc0/src/ewoksserver.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-05-23 16:58:12.000000 ewoksserver-0.1.0rc0/src/ewoksserver.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      355 2023-05-23 16:58:12.000000 ewoksserver-0.1.0rc0/src/ewoksserver.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-05-23 16:58:12.000000 ewoksserver-0.1.0rc0/src/ewoksserver.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:24:07.000000 ewoksserver-0.1.0rc1/
+-rw-rw-rw-   0 root         (0) root         (0)     1102 2023-05-24 07:03:13.000000 ewoksserver-0.1.0rc1/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     2201 2023-05-24 09:24:07.000000 ewoksserver-0.1.0rc1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1468 2023-05-24 07:03:13.000000 ewoksserver-0.1.0rc1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-05-24 07:03:13.000000 ewoksserver-0.1.0rc1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1445 2023-05-24 09:24:07.000000 ewoksserver-0.1.0rc1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-05-24 07:03:13.000000 ewoksserver-0.1.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:24:07.000000 ewoksserver-0.1.0rc1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:24:07.000000 ewoksserver-0.1.0rc1/src/ewoksserver/
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-05-24 09:21:30.000000 ewoksserver-0.1.0rc1/src/ewoksserver/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:24:07.000000 ewoksserver-0.1.0rc1/src/ewoksserver/events/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 09:24:00.000000 ewoksserver-0.1.0rc1/src/ewoksserver/events/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1058 2023-05-24 07:03:13.000000 ewoksserver-0.1.0rc1/src/ewoksserver/events/ewoks_events.py
+-rw-rw-rw-   0 root         (0) root         (0)     2697 2023-05-24 07:03:13.000000 ewoksserver-0.1.0rc1/src/ewoksserver/events/websocket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:24:07.000000 ewoksserver-0.1.0rc1/src/ewoksserver/resources/
+-rw-rw-rw-   0 root         (0) root         (0)      731 2023-05-24 07:03:13.000000 ewoksserver-0.1.0rc1/src/ewoksserver/resources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9807 2023-05-24 07:03:13.000000 ewoksserver-0.1.0rc1/src/ewoksserver/resources/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:24:07.000000 ewoksserver-0.1.0rc1/src/ewoksserver/resources/binary/
+-rw-rw-rw-   0 root         (0) root         (0)      413 2023-05-24 07:03:13.000000 ewoksserver-0.1.0rc1/src/ewoksserver/resources/binary/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1140 2023-05-24 07:03:13.000000 ewoksserver-0.1.0rc1/src/ewoksserver/resources/binary/icons.py
+-rw-rw-rw-   0 root         (0) root         (0)     3834 2023-05-24 07:03:13.000000 ewoksserver-0.1.0rc1/src/ewoksserver/resources/binary/resource.py
+-rw-rw-rw-   0 root         (0) root         (0)     3472 2023-05-24 07:03:13.000000 ewoksserver-0.1.0rc1/src/ewoksserver/resources/binary/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:24:07.000000 ewoksserver-0.1.0rc1/src/ewoksserver/resources/data/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-05-24 07:03:13.000000 ewoksserver-0.1.0rc1/src/ewoksserver/resources/data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:24:07.000000 ewoksserver-0.1.0rc1/src/ewoksserver/resources/data/icons/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 09:24:00.000000 ewoksserver-0.1.0rc1/src/ewoksserver/resources/data/icons/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1348 2023-05-24 07:03:13.000000 ewoksserver-0.1.0rc1/src/ewoksserver/resources/data/icons/default.png
+-rw-rw-rw-   0 root         (0) root         (0)      133 2023-05-24 07:03:13.000000 ewoksserver-0.1.0rc1/src/ewoksserver/resources/data/icons/graphInput.svg
+-rw-rw-rw-   0 root         (0) root         (0)      149 2023-05-24 07:03:13.000000 ewoksserver-0.1.0rc1/src/ewoksserver/resources/data/icons/graphOutput.svg
+-rw-rw-rw-   0 root         (0) root         (0)     3070 2023-05-24 07:03:13.000000 ewoksserver-0.1.0rc1/src/ewoksserver/resources/data/icons/sum.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:24:07.000000 ewoksserver-0.1.0rc1/src/ewoksserver/resources/data/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 09:24:00.000000 ewoksserver-0.1.0rc1/src/ewoksserver/resources/data/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      295 2023-05-24 07:03:13.000000 ewoksserver-0.1.0rc1/src/ewoksserver/resources/data/tasks/ewokscore.tests.examples.tasks.sumlist.SumList.json
+-rw-rw-rw-   0 root         (0) root         (0)      300 2023-05-24 07:03:13.000000 ewoksserver-0.1.0rc1/src/ewoksserver/resources/data/tasks/ewokscore.tests.examples.tasks.sumtask.SumTask.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:24:07.000000 ewoksserver-0.1.0rc1/src/ewoksserver/resources/data/workflows/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 09:24:00.000000 ewoksserver-0.1.0rc1/src/ewoksserver/resources/data/workflows/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12315 2023-05-24 07:03:13.000000 ewoksserver-0.1.0rc1/src/ewoksserver/resources/data/workflows/demo.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:24:07.000000 ewoksserver-0.1.0rc1/src/ewoksserver/resources/events/
+-rw-rw-rw-   0 root         (0) root         (0)      360 2023-05-24 07:03:13.000000 ewoksserver-0.1.0rc1/src/ewoksserver/resources/events/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      880 2023-05-24 07:03:13.000000 ewoksserver-0.1.0rc1/src/ewoksserver/resources/events/resource.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:24:07.000000 ewoksserver-0.1.0rc1/src/ewoksserver/resources/json/
+-rw-rw-rw-   0 root         (0) root         (0)      952 2023-05-24 07:03:13.000000 ewoksserver-0.1.0rc1/src/ewoksserver/resources/json/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4691 2023-05-24 07:03:13.000000 ewoksserver-0.1.0rc1/src/ewoksserver/resources/json/resource.py
+-rw-rw-rw-   0 root         (0) root         (0)     3052 2023-05-24 07:03:13.000000 ewoksserver-0.1.0rc1/src/ewoksserver/resources/json/tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     3332 2023-05-24 07:03:13.000000 ewoksserver-0.1.0rc1/src/ewoksserver/resources/json/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3371 2023-05-24 07:03:13.000000 ewoksserver-0.1.0rc1/src/ewoksserver/resources/json/workflows.py
+-rw-rw-rw-   0 root         (0) root         (0)      403 2023-05-24 07:03:13.000000 ewoksserver-0.1.0rc1/src/ewoksserver/resources/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     5963 2023-05-24 07:03:13.000000 ewoksserver-0.1.0rc1/src/ewoksserver/server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:24:07.000000 ewoksserver-0.1.0rc1/src/ewoksserver/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 09:24:00.000000 ewoksserver-0.1.0rc1/src/ewoksserver/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3053 2023-05-24 07:03:13.000000 ewoksserver-0.1.0rc1/src/ewoksserver/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:24:07.000000 ewoksserver-0.1.0rc1/src/ewoksserver/tests/data/
+-rw-rw-rw-   0 root         (0) root         (0)      292 2023-05-24 07:03:13.000000 ewoksserver-0.1.0rc1/src/ewoksserver/tests/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2730 2023-05-24 07:03:13.000000 ewoksserver-0.1.0rc1/src/ewoksserver/tests/data/icon1.png
+-rw-rw-rw-   0 root         (0) root         (0)      133 2023-05-24 07:03:13.000000 ewoksserver-0.1.0rc1/src/ewoksserver/tests/data/icon1.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1698 2023-05-24 07:03:13.000000 ewoksserver-0.1.0rc1/src/ewoksserver/tests/data/icon2.png
+-rw-rw-rw-   0 root         (0) root         (0)      493 2023-05-24 07:03:13.000000 ewoksserver-0.1.0rc1/src/ewoksserver/tests/data/icon2.svg
+-rw-rw-rw-   0 root         (0) root         (0)       91 2023-05-24 07:03:13.000000 ewoksserver-0.1.0rc1/src/ewoksserver/tests/dummy_tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2040 2023-05-24 07:03:13.000000 ewoksserver-0.1.0rc1/src/ewoksserver/tests/test_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     3137 2023-05-24 07:03:13.000000 ewoksserver-0.1.0rc1/src/ewoksserver/tests/test_events.py
+-rw-rw-rw-   0 root         (0) root         (0)     1797 2023-05-24 07:03:13.000000 ewoksserver-0.1.0rc1/src/ewoksserver/tests/test_execute.py
+-rw-rw-rw-   0 root         (0) root         (0)     2612 2023-05-24 07:03:13.000000 ewoksserver-0.1.0rc1/src/ewoksserver/tests/test_icons.py
+-rw-rw-rw-   0 root         (0) root         (0)     5844 2023-05-24 07:03:13.000000 ewoksserver-0.1.0rc1/src/ewoksserver/tests/test_tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)      807 2023-05-24 07:03:13.000000 ewoksserver-0.1.0rc1/src/ewoksserver/tests/test_websocket_connection.py
+-rw-rw-rw-   0 root         (0) root         (0)     4013 2023-05-24 07:03:13.000000 ewoksserver-0.1.0rc1/src/ewoksserver/tests/test_workflows.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:24:07.000000 ewoksserver-0.1.0rc1/src/ewoksserver.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2201 2023-05-24 09:24:07.000000 ewoksserver-0.1.0rc1/src/ewoksserver.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2221 2023-05-24 09:24:07.000000 ewoksserver-0.1.0rc1/src/ewoksserver.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 09:24:07.000000 ewoksserver-0.1.0rc1/src/ewoksserver.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-05-24 09:24:07.000000 ewoksserver-0.1.0rc1/src/ewoksserver.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      360 2023-05-24 09:24:07.000000 ewoksserver-0.1.0rc1/src/ewoksserver.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-05-24 09:24:07.000000 ewoksserver-0.1.0rc1/src/ewoksserver.egg-info/top_level.txt
```

### Comparing `ewoksserver-0.1.0rc0/LICENSE.md` & `ewoksserver-0.1.0rc1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.1.0rc0/PKG-INFO` & `ewoksserver-0.1.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewoksserver
-Version: 0.1.0rc0
+Version: 0.1.0rc1
 Summary: Backend for ewoksweb
 Home-page: https://gitlab.esrf.fr/workflow/ewoks/ewoksserver
 Author: ESRF
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoks/ewoksserver
 Project-URL: Documentation, https://workflow.gitlab-pages.esrf.fr/ewoks/ewoksserver
 Project-URL: Tracker, https://gitlab.esrf.fr/workflow/ewoks/ewoksserver/issues
```

### Comparing `ewoksserver-0.1.0rc0/README.md` & `ewoksserver-0.1.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.1.0rc0/setup.cfg` & `ewoksserver-0.1.0rc1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 	=src
 packages = find:
 python_requires = >=3.7
 install_requires = 
 	flask
 	flask-restful
 	flask-cors
-	flask-socketio
+	flask-socketio <=5.2
 	flask-apispec
 	werkzeug <2.3  # until flask-socketio issue #1982 is solved
 	simple-websocket
 	ewokscore >=0.3.2
 	ewoksjob[worker]
 
 [options.packages.find]
```

### Comparing `ewoksserver-0.1.0rc0/src/ewoksserver/events/ewoks_events.py` & `ewoksserver-0.1.0rc1/src/ewoksserver/events/ewoks_events.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.1.0rc0/src/ewoksserver/events/websocket.py` & `ewoksserver-0.1.0rc1/src/ewoksserver/events/websocket.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.1.0rc0/src/ewoksserver/resources/__init__.py` & `ewoksserver-0.1.0rc1/src/ewoksserver/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.1.0rc0/src/ewoksserver/resources/api.py` & `ewoksserver-0.1.0rc1/src/ewoksserver/resources/api.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.1.0rc0/src/ewoksserver/resources/binary/icons.py` & `ewoksserver-0.1.0rc1/src/ewoksserver/resources/binary/icons.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.1.0rc0/src/ewoksserver/resources/binary/resource.py` & `ewoksserver-0.1.0rc1/src/ewoksserver/resources/binary/resource.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.1.0rc0/src/ewoksserver/resources/binary/utils.py` & `ewoksserver-0.1.0rc1/src/ewoksserver/resources/binary/utils.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.1.0rc0/src/ewoksserver/resources/data/icons/default.png` & `ewoksserver-0.1.0rc1/src/ewoksserver/resources/data/icons/default.png`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.1.0rc0/src/ewoksserver/resources/data/icons/sum.png` & `ewoksserver-0.1.0rc1/src/ewoksserver/resources/data/icons/sum.png`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.1.0rc0/src/ewoksserver/resources/data/workflows/demo.json` & `ewoksserver-0.1.0rc1/src/ewoksserver/resources/data/workflows/demo.json`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.1.0rc0/src/ewoksserver/resources/events/resource.py` & `ewoksserver-0.1.0rc1/src/ewoksserver/resources/events/resource.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.1.0rc0/src/ewoksserver/resources/json/__init__.py` & `ewoksserver-0.1.0rc1/src/ewoksserver/resources/json/__init__.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.1.0rc0/src/ewoksserver/resources/json/resource.py` & `ewoksserver-0.1.0rc1/src/ewoksserver/resources/json/resource.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.1.0rc0/src/ewoksserver/resources/json/tasks.py` & `ewoksserver-0.1.0rc1/src/ewoksserver/resources/json/tasks.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.1.0rc0/src/ewoksserver/resources/json/utils.py` & `ewoksserver-0.1.0rc1/src/ewoksserver/resources/json/utils.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.1.0rc0/src/ewoksserver/resources/json/workflows.py` & `ewoksserver-0.1.0rc1/src/ewoksserver/resources/json/workflows.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.1.0rc0/src/ewoksserver/server.py` & `ewoksserver-0.1.0rc1/src/ewoksserver/server.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.1.0rc0/src/ewoksserver/tests/conftest.py` & `ewoksserver-0.1.0rc1/src/ewoksserver/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.1.0rc0/src/ewoksserver/tests/data/icon1.png` & `ewoksserver-0.1.0rc1/src/ewoksserver/tests/data/icon1.png`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.1.0rc0/src/ewoksserver/tests/data/icon2.png` & `ewoksserver-0.1.0rc1/src/ewoksserver/tests/data/icon2.png`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.1.0rc0/src/ewoksserver/tests/test_data.py` & `ewoksserver-0.1.0rc1/src/ewoksserver/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.1.0rc0/src/ewoksserver/tests/test_events.py` & `ewoksserver-0.1.0rc1/src/ewoksserver/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.1.0rc0/src/ewoksserver/tests/test_execute.py` & `ewoksserver-0.1.0rc1/src/ewoksserver/tests/test_execute.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.1.0rc0/src/ewoksserver/tests/test_icons.py` & `ewoksserver-0.1.0rc1/src/ewoksserver/tests/test_icons.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.1.0rc0/src/ewoksserver/tests/test_tasks.py` & `ewoksserver-0.1.0rc1/src/ewoksserver/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.1.0rc0/src/ewoksserver/tests/test_websocket_connection.py` & `ewoksserver-0.1.0rc1/src/ewoksserver/tests/test_websocket_connection.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.1.0rc0/src/ewoksserver/tests/test_workflows.py` & `ewoksserver-0.1.0rc1/src/ewoksserver/tests/test_workflows.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.1.0rc0/src/ewoksserver.egg-info/PKG-INFO` & `ewoksserver-0.1.0rc1/src/ewoksserver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewoksserver
-Version: 0.1.0rc0
+Version: 0.1.0rc1
 Summary: Backend for ewoksweb
 Home-page: https://gitlab.esrf.fr/workflow/ewoks/ewoksserver
 Author: ESRF
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoks/ewoksserver
 Project-URL: Documentation, https://workflow.gitlab-pages.esrf.fr/ewoks/ewoksserver
 Project-URL: Tracker, https://gitlab.esrf.fr/workflow/ewoks/ewoksserver/issues
```

### Comparing `ewoksserver-0.1.0rc0/src/ewoksserver.egg-info/SOURCES.txt` & `ewoksserver-0.1.0rc1/src/ewoksserver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

