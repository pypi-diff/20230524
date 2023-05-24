# Comparing `tmp/deepdataspace-0.0.2.tar.gz` & `tmp/deepdataspace-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepdataspace-0.0.2.tar", last modified: Wed May 10 07:50:49 2023, max compression
+gzip compressed data, was "deepdataspace-0.0.3.tar", last modified: Wed May 24 14:14:50 2023, max compression
```

## Comparing `deepdataspace-0.0.2.tar` & `deepdataspace-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,203 @@
-drwxr-xr-x   0 johnhu     (501) staff       (20)        0 2023-05-10 07:50:49.652689 deepdataspace-0.0.2/
--rw-r--r--   0 johnhu     (501) staff       (20)      584 2023-05-10 07:19:32.000000 deepdataspace-0.0.2/LICENSE
--rw-r--r--   0 johnhu     (501) staff       (20)      149 2023-03-02 01:14:06.000000 deepdataspace-0.0.2/MANIFEST.in
--rw-r--r--   0 johnhu     (501) staff       (20)     1967 2023-05-10 07:50:49.652384 deepdataspace-0.0.2/PKG-INFO
--rw-r--r--   0 johnhu     (501) staff       (20)      770 2023-05-10 07:15:20.000000 deepdataspace-0.0.2/README.md
--rwxr-xr-x   0 johnhu     (501) staff       (20)      941 2023-05-10 07:17:08.000000 deepdataspace-0.0.2/dds.py
-drwxr-xr-x   0 johnhu     (501) staff       (20)        0 2023-05-10 07:50:49.650010 deepdataspace-0.0.2/deepdataspace/
--rw-r--r--   0 johnhu     (501) staff       (20)        0 2023-05-10 07:15:48.000000 deepdataspace-0.0.2/deepdataspace/__init__.py
-drwxr-xr-x   0 johnhu     (501) staff       (20)        0 2023-05-10 07:50:49.651940 deepdataspace-0.0.2/deepdataspace.egg-info/
--rw-r--r--   0 johnhu     (501) staff       (20)     1967 2023-05-10 07:50:49.000000 deepdataspace-0.0.2/deepdataspace.egg-info/PKG-INFO
--rw-r--r--   0 johnhu     (501) staff       (20)      295 2023-05-10 07:50:49.000000 deepdataspace-0.0.2/deepdataspace.egg-info/SOURCES.txt
--rw-r--r--   0 johnhu     (501) staff       (20)        1 2023-05-10 07:50:49.000000 deepdataspace-0.0.2/deepdataspace.egg-info/dependency_links.txt
--rw-r--r--   0 johnhu     (501) staff       (20)       34 2023-05-10 07:50:49.000000 deepdataspace-0.0.2/deepdataspace.egg-info/entry_points.txt
--rw-r--r--   0 johnhu     (501) staff       (20)      378 2023-05-10 07:50:49.000000 deepdataspace-0.0.2/deepdataspace.egg-info/requires.txt
--rw-r--r--   0 johnhu     (501) staff       (20)       18 2023-05-10 07:50:49.000000 deepdataspace-0.0.2/deepdataspace.egg-info/top_level.txt
--rw-r--r--   0 johnhu     (501) staff       (20)       38 2023-05-10 07:50:49.652789 deepdataspace-0.0.2/setup.cfg
--rw-r--r--   0 johnhu     (501) staff       (20)     2981 2023-05-10 07:50:45.000000 deepdataspace-0.0.2/setup.py
+drwxr-xr-x   0 johnhu     (501) staff       (20)        0 2023-05-24 14:14:50.691448 deepdataspace-0.0.3/
+-rw-r--r--   0 johnhu     (501) staff       (20)    11310 2023-05-23 01:21:27.000000 deepdataspace-0.0.3/LICENSE
+-rw-r--r--   0 johnhu     (501) staff       (20)      149 2023-05-23 01:21:27.000000 deepdataspace-0.0.3/MANIFEST.in
+-rw-r--r--   0 johnhu     (501) staff       (20)     6595 2023-05-24 14:14:50.691048 deepdataspace-0.0.3/PKG-INFO
+-rw-r--r--   0 johnhu     (501) staff       (20)     4465 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/README.md
+-rwxr-xr-x   0 johnhu     (501) staff       (20)     1203 2023-05-23 01:21:27.000000 deepdataspace-0.0.3/dds.py
+-rwxr-xr-x   0 johnhu     (501) staff       (20)     1088 2023-05-23 01:21:27.000000 deepdataspace-0.0.3/ddsop.py
+drwxr-xr-x   0 johnhu     (501) staff       (20)        0 2023-05-24 14:14:50.540615 deepdataspace-0.0.3/deepdataspace/
+-rw-r--r--   0 johnhu     (501) staff       (20)      847 2023-05-23 01:21:27.000000 deepdataspace-0.0.3/deepdataspace/__init__.py
+drwxr-xr-x   0 johnhu     (501) staff       (20)        0 2023-05-24 14:14:50.544215 deepdataspace-0.0.3/deepdataspace/algos/
+-rw-r--r--   0 johnhu     (501) staff       (20)       94 2023-05-23 01:21:27.000000 deepdataspace-0.0.3/deepdataspace/algos/__init__.py
+-rw-r--r--   0 johnhu     (501) staff       (20)     7596 2023-05-23 01:21:27.000000 deepdataspace-0.0.3/deepdataspace/algos/calculate_fnfp.py
+-rw-r--r--   0 johnhu     (501) staff       (20)     5606 2023-05-23 01:21:27.000000 deepdataspace-0.0.3/deepdataspace/algos/graph.py
+-rw-r--r--   0 johnhu     (501) staff       (20)     5611 2023-05-23 01:21:27.000000 deepdataspace-0.0.3/deepdataspace/algos/refine_by_seed.py
+-rw-r--r--   0 johnhu     (501) staff       (20)    10683 2023-05-23 01:21:27.000000 deepdataspace-0.0.3/deepdataspace/constants.py
+-rw-r--r--   0 johnhu     (501) staff       (20)     3725 2023-05-23 01:21:27.000000 deepdataspace-0.0.3/deepdataspace/environs.py
+-rw-r--r--   0 johnhu     (501) staff       (20)     1838 2023-05-23 01:21:27.000000 deepdataspace-0.0.3/deepdataspace/globals.py
+drwxr-xr-x   0 johnhu     (501) staff       (20)        0 2023-05-24 14:14:50.545132 deepdataspace-0.0.3/deepdataspace/io/
+-rw-r--r--   0 johnhu     (501) staff       (20)      134 2023-05-23 01:21:27.000000 deepdataspace-0.0.3/deepdataspace/io/__init__.py
+-rw-r--r--   0 johnhu     (501) staff       (20)    16806 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/io/importer.py
+drwxr-xr-x   0 johnhu     (501) staff       (20)        0 2023-05-24 14:14:50.550081 deepdataspace-0.0.3/deepdataspace/model/
+-rw-r--r--   0 johnhu     (501) staff       (20)      814 2023-05-23 01:21:27.000000 deepdataspace-0.0.3/deepdataspace/model/__init__.py
+-rw-r--r--   0 johnhu     (501) staff       (20)    11913 2023-05-23 01:21:27.000000 deepdataspace-0.0.3/deepdataspace/model/_base.py
+-rw-r--r--   0 johnhu     (501) staff       (20)      543 2023-05-23 01:21:27.000000 deepdataspace-0.0.3/deepdataspace/model/category.py
+-rw-r--r--   0 johnhu     (501) staff       (20)    12823 2023-05-23 01:21:27.000000 deepdataspace-0.0.3/deepdataspace/model/dataset.py
+-rw-r--r--   0 johnhu     (501) staff       (20)    15481 2023-05-23 01:21:27.000000 deepdataspace-0.0.3/deepdataspace/model/image.py
+-rw-r--r--   0 johnhu     (501) staff       (20)      871 2023-05-23 01:21:27.000000 deepdataspace-0.0.3/deepdataspace/model/label.py
+-rw-r--r--   0 johnhu     (501) staff       (20)    62460 2023-05-23 01:21:27.000000 deepdataspace-0.0.3/deepdataspace/model/label_task.py
+-rw-r--r--   0 johnhu     (501) staff       (20)     1955 2023-05-24 13:49:53.000000 deepdataspace-0.0.3/deepdataspace/model/object.py
+-rw-r--r--   0 johnhu     (501) staff       (20)     4426 2023-05-23 01:21:27.000000 deepdataspace-0.0.3/deepdataspace/model/user.py
+drwxr-xr-x   0 johnhu     (501) staff       (20)        0 2023-05-24 14:14:50.550448 deepdataspace-0.0.3/deepdataspace/plugins/
+-rw-r--r--   0 johnhu     (501) staff       (20)     1043 2023-05-23 01:21:27.000000 deepdataspace-0.0.3/deepdataspace/plugins/__init__.py
+drwxr-xr-x   0 johnhu     (501) staff       (20)        0 2023-05-24 14:14:50.551195 deepdataspace-0.0.3/deepdataspace/plugins/coco2017/
+-rw-r--r--   0 johnhu     (501) staff       (20)      230 2023-05-23 01:21:27.000000 deepdataspace-0.0.3/deepdataspace/plugins/coco2017/__init__.py
+-rw-r--r--   0 johnhu     (501) staff       (20)    10909 2023-05-23 01:21:27.000000 deepdataspace-0.0.3/deepdataspace/plugins/coco2017/importer.py
+drwxr-xr-x   0 johnhu     (501) staff       (20)        0 2023-05-24 14:14:50.552938 deepdataspace-0.0.3/deepdataspace/plugins/tsv/
+-rw-r--r--   0 johnhu     (501) staff       (20)      475 2023-05-23 01:21:27.000000 deepdataspace-0.0.3/deepdataspace/plugins/tsv/__init__.py
+-rw-r--r--   0 johnhu     (501) staff       (20)    11622 2023-05-23 01:21:27.000000 deepdataspace-0.0.3/deepdataspace/plugins/tsv/importer.py
+-rw-r--r--   0 johnhu     (501) staff       (20)     1790 2023-05-23 01:21:27.000000 deepdataspace-0.0.3/deepdataspace/plugins/tsv/process.py
+-rw-r--r--   0 johnhu     (501) staff       (20)     2796 2023-05-23 01:21:27.000000 deepdataspace-0.0.3/deepdataspace/plugins/tsv/server.py
+drwxr-xr-x   0 johnhu     (501) staff       (20)        0 2023-05-24 14:14:50.555274 deepdataspace-0.0.3/deepdataspace/process/
+-rw-r--r--   0 johnhu     (501) staff       (20)      238 2023-05-23 01:21:27.000000 deepdataspace-0.0.3/deepdataspace/process/__init__.py
+-rw-r--r--   0 johnhu     (501) staff       (20)     9346 2023-05-23 01:21:27.000000 deepdataspace-0.0.3/deepdataspace/process/calculate_fnfp.py
+-rw-r--r--   0 johnhu     (501) staff       (20)     9954 2023-05-23 01:21:27.000000 deepdataspace-0.0.3/deepdataspace/process/processor.py
+drwxr-xr-x   0 johnhu     (501) staff       (20)        0 2023-05-24 14:14:50.558817 deepdataspace-0.0.3/deepdataspace/scripts/
+-rw-r--r--   0 johnhu     (501) staff       (20)      850 2023-05-23 01:21:27.000000 deepdataspace-0.0.3/deepdataspace/scripts/__init__.py
+-rw-r--r--   0 johnhu     (501) staff       (20)     3389 2023-05-23 01:21:27.000000 deepdataspace-0.0.3/deepdataspace/scripts/dataset_cmds.py
+-rw-r--r--   0 johnhu     (501) staff       (20)      798 2023-05-23 01:21:27.000000 deepdataspace-0.0.3/deepdataspace/scripts/enter_shell.py
+-rw-r--r--   0 johnhu     (501) staff       (20)     4408 2023-05-23 01:21:27.000000 deepdataspace-0.0.3/deepdataspace/scripts/label_project_cmds.py
+-rw-r--r--   0 johnhu     (501) staff       (20)     2313 2023-05-23 01:21:27.000000 deepdataspace-0.0.3/deepdataspace/scripts/start.py
+-rw-r--r--   0 johnhu     (501) staff       (20)     2910 2023-05-23 01:21:27.000000 deepdataspace-0.0.3/deepdataspace/scripts/user_cmds.py
+drwxr-xr-x   0 johnhu     (501) staff       (20)        0 2023-05-24 14:14:50.563154 deepdataspace-0.0.3/deepdataspace/server/
+-rw-r--r--   0 johnhu     (501) staff       (20)       75 2023-05-23 01:21:28.000000 deepdataspace-0.0.3/deepdataspace/server/__init__.py
+-rw-r--r--   0 johnhu     (501) staff       (20)      594 2023-05-23 01:21:28.000000 deepdataspace-0.0.3/deepdataspace/server/apps.py
+-rw-r--r--   0 johnhu     (501) staff       (20)      602 2023-05-23 01:21:28.000000 deepdataspace-0.0.3/deepdataspace/server/manage.py
+drwxr-xr-x   0 johnhu     (501) staff       (20)        0 2023-05-24 14:14:50.564457 deepdataspace-0.0.3/deepdataspace/server/middlewares/
+-rw-r--r--   0 johnhu     (501) staff       (20)      147 2023-05-23 01:21:28.000000 deepdataspace-0.0.3/deepdataspace/server/middlewares/__init__.py
+-rw-r--r--   0 johnhu     (501) staff       (20)      571 2023-05-23 01:21:28.000000 deepdataspace-0.0.3/deepdataspace/server/middlewares/request_perf.py
+drwxr-xr-x   0 johnhu     (501) staff       (20)        0 2023-05-24 14:14:50.565731 deepdataspace-0.0.3/deepdataspace/server/resources/
+-rw-r--r--   0 johnhu     (501) staff       (20)      163 2023-05-23 01:21:28.000000 deepdataspace-0.0.3/deepdataspace/server/resources/__init__.py
+drwxr-xr-x   0 johnhu     (501) staff       (20)        0 2023-05-24 14:14:50.576756 deepdataspace-0.0.3/deepdataspace/server/resources/api_v1/
+-rw-r--r--   0 johnhu     (501) staff       (20)     2860 2023-05-23 01:21:28.000000 deepdataspace-0.0.3/deepdataspace/server/resources/api_v1/__init__.py
+-rw-r--r--   0 johnhu     (501) staff       (20)     5802 2023-05-23 01:21:28.000000 deepdataspace-0.0.3/deepdataspace/server/resources/api_v1/annotations.py
+-rw-r--r--   0 johnhu     (501) staff       (20)     7088 2023-05-23 01:21:28.000000 deepdataspace-0.0.3/deepdataspace/server/resources/api_v1/comparisons.py
+-rw-r--r--   0 johnhu     (501) staff       (20)     2958 2023-05-23 01:21:28.000000 deepdataspace-0.0.3/deepdataspace/server/resources/api_v1/datasets.py
+-rw-r--r--   0 johnhu     (501) staff       (20)     2972 2023-05-23 01:21:28.000000 deepdataspace-0.0.3/deepdataspace/server/resources/api_v1/image_flags.py
+-rw-r--r--   0 johnhu     (501) staff       (20)     4806 2023-05-23 01:21:28.000000 deepdataspace-0.0.3/deepdataspace/server/resources/api_v1/images.py
+-rw-r--r--   0 johnhu     (501) staff       (20)     7298 2023-05-23 01:21:28.000000 deepdataspace-0.0.3/deepdataspace/server/resources/api_v1/label_clone.py
+-rw-r--r--   0 johnhu     (501) staff       (20)    36250 2023-05-23 01:21:28.000000 deepdataspace-0.0.3/deepdataspace/server/resources/api_v1/label_tasks.py
+-rw-r--r--   0 johnhu     (501) staff       (20)     2518 2023-05-23 01:21:28.000000 deepdataspace-0.0.3/deepdataspace/server/resources/api_v1/lints.py
+-rw-r--r--   0 johnhu     (501) staff       (20)     2165 2023-05-23 01:21:28.000000 deepdataspace-0.0.3/deepdataspace/server/resources/api_v1/login.py
+-rw-r--r--   0 johnhu     (501) staff       (20)     2938 2023-05-23 01:21:28.000000 deepdataspace-0.0.3/deepdataspace/server/resources/api_v1/object_confirm.py
+-rw-r--r--   0 johnhu     (501) staff       (20)     1782 2023-05-23 01:21:28.000000 deepdataspace-0.0.3/deepdataspace/server/resources/api_v1/ping.py
+-rw-r--r--   0 johnhu     (501) staff       (20)     8875 2023-05-23 01:21:28.000000 deepdataspace-0.0.3/deepdataspace/server/resources/common.py
+drwxr-xr-x   0 johnhu     (501) staff       (20)        0 2023-05-24 14:14:50.579286 deepdataspace-0.0.3/deepdataspace/server/resources/files/
+-rw-r--r--   0 johnhu     (501) staff       (20)      493 2023-05-23 01:21:28.000000 deepdataspace-0.0.3/deepdataspace/server/resources/files/__init__.py
+-rw-r--r--   0 johnhu     (501) staff       (20)     1382 2023-05-23 01:21:28.000000 deepdataspace-0.0.3/deepdataspace/server/resources/files/dataset_flags.py
+-rw-r--r--   0 johnhu     (501) staff       (20)     2355 2023-05-23 01:21:28.000000 deepdataspace-0.0.3/deepdataspace/server/resources/files/local_file.py
+-rw-r--r--   0 johnhu     (501) staff       (20)     4454 2023-05-23 01:21:28.000000 deepdataspace-0.0.3/deepdataspace/server/settings.py
+drwxr-xr-x   0 johnhu     (501) staff       (20)        0 2023-05-24 14:14:50.669537 deepdataspace-0.0.3/deepdataspace/server/static/
+-rw-r--r--   0 johnhu     (501) staff       (20)    46189 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/14.dae06833.async.js
+-rw-r--r--   0 johnhu     (501) staff       (20)   514040 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/146.455dc60d.async.js
+-rw-r--r--   0 johnhu     (501) staff       (20)   111434 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/146.455dc60d.async.js.map
+-rw-r--r--   0 johnhu     (501) staff       (20)    10284 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/212.1ee4b28f.async.js
+-rw-r--r--   0 johnhu     (501) staff       (20)      266 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/274.3ab3bcc6.async.js
+-rw-r--r--   0 johnhu     (501) staff       (20)    39583 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/288.ebd2cb40.async.js
+-rw-r--r--   0 johnhu     (501) staff       (20)     3746 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/288.ebd2cb40.async.js.map
+-rw-r--r--   0 johnhu     (501) staff       (20)     8446 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/394.67ea71c7.async.js
+-rw-r--r--   0 johnhu     (501) staff       (20)    41761 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/510.80710ae7.async.js
+-rw-r--r--   0 johnhu     (501) staff       (20)    17950 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/510.80710ae7.async.js.map
+-rw-r--r--   0 johnhu     (501) staff       (20)    12587 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/56.652c60d5.async.js
+-rw-r--r--   0 johnhu     (501) staff       (20)    19725 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/666.3345b426.async.js
+-rw-r--r--   0 johnhu     (501) staff       (20)    23132 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/666.3345b426.async.js.map
+-rw-r--r--   0 johnhu     (501) staff       (20)    57580 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/698.c6248ea2.async.js
+-rw-r--r--   0 johnhu     (501) staff       (20)    31004 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/698.c6248ea2.async.js.map
+-rw-r--r--   0 johnhu     (501) staff       (20)    77742 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/699.92205a61.async.js
+-rw-r--r--   0 johnhu     (501) staff       (20)     1713 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/699.92205a61.async.js.map
+-rw-r--r--   0 johnhu     (501) staff       (20)     8465 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/730.e3f88aee.async.js
+-rw-r--r--   0 johnhu     (501) staff       (20)    12547 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/741.2fe47ad4.async.js
+-rw-r--r--   0 johnhu     (501) staff       (20)   294435 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/799.fcb64d08.async.js
+-rw-r--r--   0 johnhu     (501) staff       (20)    78446 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/799.fcb64d08.async.js.map
+-rw-r--r--   0 johnhu     (501) staff       (20)   126115 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/812.6f477ebe.async.js
+-rw-r--r--   0 johnhu     (501) staff       (20)    61229 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/812.6f477ebe.async.js.map
+-rw-r--r--   0 johnhu     (501) staff       (20)    19183 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/867.60365366.async.js
+-rw-r--r--   0 johnhu     (501) staff       (20)    34791 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/911.87792508.async.js
+-rw-r--r--   0 johnhu     (501) staff       (20)    19649 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/911.87792508.async.js.map
+-rw-r--r--   0 johnhu     (501) staff       (20)    38647 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/998.06c6f229.async.js
+-rw-r--r--   0 johnhu     (501) staff       (20)    13344 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/998.06c6f229.async.js.map
+-rw-r--r--   0 johnhu     (501) staff       (20)     4914 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/favicon.png
+-rw-r--r--   0 johnhu     (501) staff       (20)      498 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/index.html
+-rw-r--r--   0 johnhu     (501) staff       (20)    22202 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/layouts__index.6f82fbf8.async.js
+-rw-r--r--   0 johnhu     (501) staff       (20)     5808 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/layouts__index.90fa8c8a.chunk.css
+-rw-r--r--   0 johnhu     (501) staff       (20)    14619 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/layouts__index.90fa8c8a.chunk.css.map
+-rw-r--r--   0 johnhu     (501) staff       (20)      580 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/p__404.87cb0239.async.js
+-rw-r--r--   0 johnhu     (501) staff       (20)     8350 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/p__Annotator__index.4c4249ee.async.js
+-rw-r--r--   0 johnhu     (501) staff       (20)    11767 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/p__Annotator__index.4c4249ee.async.js.map
+-rw-r--r--   0 johnhu     (501) staff       (20)     1534 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/p__Annotator__index.648f5c31.chunk.css
+-rw-r--r--   0 johnhu     (501) staff       (20)     9132 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/p__Annotator__index.648f5c31.chunk.css.map
+-rw-r--r--   0 johnhu     (501) staff       (20)     2446 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/p__DatasetList__index.4108f691.chunk.css
+-rw-r--r--   0 johnhu     (501) staff       (20)     9164 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/p__DatasetList__index.4108f691.chunk.css.map
+-rw-r--r--   0 johnhu     (501) staff       (20)     1338 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/p__DatasetList__index.754a7df2.async.js
+-rw-r--r--   0 johnhu     (501) staff       (20)     9448 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/p__Dataset__index.4b0b9915.chunk.css
+-rw-r--r--   0 johnhu     (501) staff       (20)     8815 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/p__Dataset__index.4b0b9915.chunk.css.map
+-rw-r--r--   0 johnhu     (501) staff       (20)    11330 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/p__Dataset__index.abafc0e0.async.js
+-rw-r--r--   0 johnhu     (501) staff       (20)     4046 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/p__Lab__Datasets__index.2dc8934d.chunk.css
+-rw-r--r--   0 johnhu     (501) staff       (20)    11249 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/p__Lab__Datasets__index.2dc8934d.chunk.css.map
+-rw-r--r--   0 johnhu     (501) staff       (20)     1490 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/p__Lab__Datasets__index.f22cadfa.async.js
+-rw-r--r--   0 johnhu     (501) staff       (20)     8638 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/p__Lab__FlagTool__index.7ed03066.chunk.css
+-rw-r--r--   0 johnhu     (501) staff       (20)     8821 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/p__Lab__FlagTool__index.7ed03066.chunk.css.map
+-rw-r--r--   0 johnhu     (501) staff       (20)     7770 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/p__Lab__FlagTool__index.af45538a.async.js
+-rw-r--r--   0 johnhu     (501) staff       (20)      518 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/p__Lab__index.133bb551.chunk.css
+-rw-r--r--   0 johnhu     (501) staff       (20)     9178 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/p__Lab__index.133bb551.chunk.css.map
+-rw-r--r--   0 johnhu     (501) staff       (20)     1121 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/p__Lab__index.185b5038.async.js
+-rw-r--r--   0 johnhu     (501) staff       (20)    22169 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/p__Login__index.bfa83139.async.js
+-rw-r--r--   0 johnhu     (501) staff       (20)      214 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/p__Login__index.e3ef503c.chunk.css
+-rw-r--r--   0 johnhu     (501) staff       (20)     8909 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/p__Login__index.e3ef503c.chunk.css.map
+-rw-r--r--   0 johnhu     (501) staff       (20)     1040 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/p__Project__Detail__index.85029923.chunk.css
+-rw-r--r--   0 johnhu     (501) staff       (20)     8823 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/p__Project__Detail__index.85029923.chunk.css.map
+-rw-r--r--   0 johnhu     (501) staff       (20)    13005 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/p__Project__Detail__index.91b86861.async.js
+-rw-r--r--   0 johnhu     (501) staff       (20)     2338 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/p__Project__Workspace__index.17ab0171.chunk.css
+-rw-r--r--   0 johnhu     (501) staff       (20)    11129 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/p__Project__Workspace__index.17ab0171.chunk.css.map
+-rw-r--r--   0 johnhu     (501) staff       (20)     8152 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/p__Project__Workspace__index.bd227a15.async.js
+-rw-r--r--   0 johnhu     (501) staff       (20)    18455 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/p__Project__index.1fd5dda2.async.js
+-rw-r--r--   0 johnhu     (501) staff       (20)     5401 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/p__Project__index.1fd5dda2.async.js.map
+-rw-r--r--   0 johnhu     (501) staff       (20)      495 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/p__Project__index.c088bdc3.chunk.css
+-rw-r--r--   0 johnhu     (501) staff       (20)     8815 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/p__Project__index.c088bdc3.chunk.css.map
+drwxr-xr-x   0 johnhu     (501) staff       (20)        0 2023-05-24 14:14:50.673214 deepdataspace-0.0.3/deepdataspace/server/static/static/
+-rw-r--r--   0 johnhu     (501) staff       (20)    58216 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/static/annotate_coop.44ac433d.png
+-rw-r--r--   0 johnhu     (501) staff       (20)    82163 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/static/annotate_quick.b8733d56.png
+-rw-r--r--   0 johnhu     (501) staff       (20)    14013 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/static/card_cover_4.b81bbca8.png
+-rw-r--r--   0 johnhu     (501) staff       (20)    52425 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/static/flagtool.a991e5bd.png
+-rw-r--r--   0 johnhu     (501) staff       (20)    24577 2023-05-23 01:21:28.000000 deepdataspace-0.0.3/deepdataspace/server/static/static/home_banner.0fcae71f.png
+-rw-r--r--   0 johnhu     (501) staff       (20)     1037 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/t__plugin-layout__Layout.58f1aeb4.chunk.css
+-rw-r--r--   0 johnhu     (501) staff       (20)     9815 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/t__plugin-layout__Layout.58f1aeb4.chunk.css.map
+-rw-r--r--   0 johnhu     (501) staff       (20)     7591 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/t__plugin-layout__Layout.8d55c430.async.js
+-rw-r--r--   0 johnhu     (501) staff       (20)  1795344 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/umi.b78a4ca1.js
+-rw-r--r--   0 johnhu     (501) staff       (20)  1420708 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/umi.b78a4ca1.js.map
+-rw-r--r--   0 johnhu     (501) staff       (20)    15007 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/umi.dfabe2b1.css
+-rw-r--r--   0 johnhu     (501) staff       (20)    10163 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/umi.dfabe2b1.css.map
+-rw-r--r--   0 johnhu     (501) staff       (20)      358 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/static/wrappers__auth.3cb2bc7c.async.js
+drwxr-xr-x   0 johnhu     (501) staff       (20)        0 2023-05-24 14:14:50.674190 deepdataspace-0.0.3/deepdataspace/server/templates/
+-rw-r--r--   0 johnhu     (501) staff       (20)      498 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/server/templates/index.html
+-rw-r--r--   0 johnhu     (501) staff       (20)      524 2023-05-23 01:21:28.000000 deepdataspace-0.0.3/deepdataspace/server/urls.py
+-rw-r--r--   0 johnhu     (501) staff       (20)     1013 2023-05-23 01:21:28.000000 deepdataspace-0.0.3/deepdataspace/server/utils.py
+drwxr-xr-x   0 johnhu     (501) staff       (20)        0 2023-05-24 14:14:50.675007 deepdataspace-0.0.3/deepdataspace/server/views/
+-rw-r--r--   0 johnhu     (501) staff       (20)      132 2023-05-23 01:21:28.000000 deepdataspace-0.0.3/deepdataspace/server/views/__init__.py
+-rw-r--r--   0 johnhu     (501) staff       (20)      213 2023-05-23 01:21:28.000000 deepdataspace-0.0.3/deepdataspace/server/views/index.py
+-rw-r--r--   0 johnhu     (501) staff       (20)      247 2023-05-23 01:21:28.000000 deepdataspace-0.0.3/deepdataspace/server/wsgi.py
+drwxr-xr-x   0 johnhu     (501) staff       (20)        0 2023-05-24 14:14:50.682005 deepdataspace-0.0.3/deepdataspace/services/
+-rw-r--r--   0 johnhu     (501) staff       (20)      229 2023-05-23 01:21:28.000000 deepdataspace-0.0.3/deepdataspace/services/__init__.py
+-rw-r--r--   0 johnhu     (501) staff       (20)      934 2023-05-23 01:21:28.000000 deepdataspace-0.0.3/deepdataspace/services/celery.py
+-rw-r--r--   0 johnhu     (501) staff       (20)     7564 2023-05-24 13:18:00.000000 deepdataspace-0.0.3/deepdataspace/services/config.py
+-rw-r--r--   0 johnhu     (501) staff       (20)    18409 2023-05-23 01:21:28.000000 deepdataspace-0.0.3/deepdataspace/services/dds.py
+-rw-r--r--   0 johnhu     (501) staff       (20)     1711 2023-05-23 01:21:28.000000 deepdataspace-0.0.3/deepdataspace/services/django.py
+-rw-r--r--   0 johnhu     (501) staff       (20)     4265 2023-05-23 01:21:28.000000 deepdataspace-0.0.3/deepdataspace/services/mongodb.py
+-rw-r--r--   0 johnhu     (501) staff       (20)     1812 2023-05-23 01:21:28.000000 deepdataspace-0.0.3/deepdataspace/services/redis.py
+-rw-r--r--   0 johnhu     (501) staff       (20)     4965 2023-05-23 01:21:28.000000 deepdataspace-0.0.3/deepdataspace/services/service.py
+-rw-r--r--   0 johnhu     (501) staff       (20)      669 2023-05-23 01:21:28.000000 deepdataspace-0.0.3/deepdataspace/services/sqlite.py
+drwxr-xr-x   0 johnhu     (501) staff       (20)        0 2023-05-24 14:14:50.684609 deepdataspace-0.0.3/deepdataspace/task/
+-rw-r--r--   0 johnhu     (501) staff       (20)     2635 2023-05-23 01:21:28.000000 deepdataspace-0.0.3/deepdataspace/task/__init__.py
+-rw-r--r--   0 johnhu     (501) staff       (20)      168 2023-05-23 01:21:28.000000 deepdataspace-0.0.3/deepdataspace/task/celery.py
+-rw-r--r--   0 johnhu     (501) staff       (20)      487 2023-05-23 01:21:28.000000 deepdataspace-0.0.3/deepdataspace/task/import_dataset.py
+-rw-r--r--   0 johnhu     (501) staff       (20)      192 2023-05-23 01:21:28.000000 deepdataspace-0.0.3/deepdataspace/task/ping.py
+-rw-r--r--   0 johnhu     (501) staff       (20)      563 2023-05-23 01:21:28.000000 deepdataspace-0.0.3/deepdataspace/task/process_dataset.py
+-rw-r--r--   0 johnhu     (501) staff       (20)      195 2023-05-23 01:21:28.000000 deepdataspace-0.0.3/deepdataspace/task/settings.py
+drwxr-xr-x   0 johnhu     (501) staff       (20)        0 2023-05-24 14:14:50.689601 deepdataspace-0.0.3/deepdataspace/utils/
+-rw-r--r--   0 johnhu     (501) staff       (20)       50 2023-05-23 01:21:28.000000 deepdataspace-0.0.3/deepdataspace/utils/__init__.py
+-rw-r--r--   0 johnhu     (501) staff       (20)     2547 2023-05-23 01:21:28.000000 deepdataspace-0.0.3/deepdataspace/utils/classes.py
+-rw-r--r--   0 johnhu     (501) staff       (20)     5099 2023-05-23 01:21:28.000000 deepdataspace-0.0.3/deepdataspace/utils/file.py
+-rw-r--r--   0 johnhu     (501) staff       (20)     1493 2023-05-23 01:21:28.000000 deepdataspace-0.0.3/deepdataspace/utils/function.py
+-rw-r--r--   0 johnhu     (501) staff       (20)     1036 2023-05-23 01:21:28.000000 deepdataspace-0.0.3/deepdataspace/utils/import_utils.py
+-rw-r--r--   0 johnhu     (501) staff       (20)     1231 2023-05-23 01:21:28.000000 deepdataspace-0.0.3/deepdataspace/utils/network.py
+-rw-r--r--   0 johnhu     (501) staff       (20)     5939 2023-05-23 01:21:28.000000 deepdataspace-0.0.3/deepdataspace/utils/os.py
+-rw-r--r--   0 johnhu     (501) staff       (20)     1734 2023-05-23 01:21:28.000000 deepdataspace-0.0.3/deepdataspace/utils/string.py
+drwxr-xr-x   0 johnhu     (501) staff       (20)        0 2023-05-24 14:14:50.542567 deepdataspace-0.0.3/deepdataspace.egg-info/
+-rw-r--r--   0 johnhu     (501) staff       (20)     6595 2023-05-24 14:14:50.000000 deepdataspace-0.0.3/deepdataspace.egg-info/PKG-INFO
+-rw-r--r--   0 johnhu     (501) staff       (20)     8195 2023-05-24 14:14:50.000000 deepdataspace-0.0.3/deepdataspace.egg-info/SOURCES.txt
+-rw-r--r--   0 johnhu     (501) staff       (20)        1 2023-05-24 14:14:50.000000 deepdataspace-0.0.3/deepdataspace.egg-info/dependency_links.txt
+-rw-r--r--   0 johnhu     (501) staff       (20)       54 2023-05-24 14:14:50.000000 deepdataspace-0.0.3/deepdataspace.egg-info/entry_points.txt
+-rw-r--r--   0 johnhu     (501) staff       (20)      290 2023-05-24 14:14:50.000000 deepdataspace-0.0.3/deepdataspace.egg-info/requires.txt
+-rw-r--r--   0 johnhu     (501) staff       (20)      453 2023-05-24 14:14:50.000000 deepdataspace-0.0.3/deepdataspace.egg-info/top_level.txt
+-rw-r--r--   0 johnhu     (501) staff       (20)       38 2023-05-24 14:14:50.691563 deepdataspace-0.0.3/setup.cfg
+-rw-r--r--   0 johnhu     (501) staff       (20)     2380 2023-05-24 14:11:39.000000 deepdataspace-0.0.3/setup.py
```

### Comparing `deepdataspace-0.0.2/dds.py` & `deepdataspace-0.0.3/dds.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 #! python
-
-import click
-
 """
 dds.py
 
 This script starts the dds tool.
 
 Usage: dds.py [OPTIONS] [DATA_DIR]
 
 Options:
-  --quickstart    Quick start dds with sample datasets instead of a specified
-                  DATA_DIR, default false. This overwrites the DATA_DIR
-                  argument.
-  -V, --verbose   Display detailed logs on console, default false.
-  -P, --public    Enable public access from your network neighbors, default
-                  false. This sets the service host by an auto-detected
-                  outward IP address.
-  --host TEXT     Set the http service host. This overwrites the '--public'
-                  flag.
-  --port INTEGER  Set the http service port, default 8765.
-  --reload        Auto reload service on code change, for development only.
-  --help          Show this message and exit.
+  --quickstart       Quick start dds with sample datasets instead of a
+                     specified DATA_DIR, default false. This overwrites the
+                     DATA_DIR argument.
+  -V, --verbose      Display detailed logs on console, default false.
+  -P, --public       Enable public access from your network neighbors, default
+                     false. This sets the service host by an auto-detected
+                     outward IP address.
+  --host TEXT        Set the http service host. This overwrites the '--public'
+                     flag.
+  --port TEXT        Set the http service port, default 8765.
+  --reload           Auto reload service on code change, for development only.
+  --configfile TEXT  Load the target yaml file to initialize more
+                     configurations. The command line options take precedence
+                     of the config file.
+  --help             Show this message and exit.
 """
+import os
+
+os.environ["DDS_STARTING"] = "1"
+
+from deepdataspace.scripts.start import start_dds
 
 
-@click.command("dds")
 def main():
-    click.echo("coming soon...")
+    start_dds()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `deepdataspace-0.0.2/setup.py` & `deepdataspace-0.0.3/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,42 @@
 import os
+
 from setuptools import setup
 
-version = "0.0.2"
+version = "0.0.3"
+
 description = "A tool for CV dataset labeling, visualizing and analysing"
 with open("README.md", "r") as fp:
     long_description = fp.read()
-url = "https://idea.edu.cn/cvr.html"
+
+url = "https://github.com/IDEA-Research/deepdataspace"
 author = "cvr@idea"
+
+install_requires = [
+    "celery==5.2.7",
+    "click==8.1.3",
+    "cryptography==39.0.1",
+    "Django==4.1.9",
+    "djangorestframework==3.14.0",
+    "django-cors-headers==3.13.0",
+    "numpy==1.22.0",
+    "psutil==5.9.2",
+    "pydantic==1.10.2",
+    "pymongo==4.2.0",
+    "PyYAML==6.0",
+    "redis==4.4.4",
+    "requests==2.31.0",
+    "scikit-learn==1.0.2",
+    "sentry-sdk==1.19.1",
+    "tqdm==4.64.1",
+    "whitenoise==6.2.0",
+]
+
 classifiers = [
     "Development Status :: 4 - Beta",
-    "Intended Audience :: Information Technology",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Scientific/Engineering :: Image Processing",
     "Topic :: Scientific/Engineering :: Image Recognition",
     "Topic :: Scientific/Engineering :: Information Analysis",
     "Topic :: Scientific/Engineering :: Visualization",
     "Operating System :: MacOS :: MacOS X",
@@ -22,26 +45,15 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 
 
-def get_version():
-    ver = os.environ.get("DDS_PACKAGE_VERSION", None)
-    if ver is not None:
-        return ver
-    return str(version)
-
-
 def find_packages(pkg_dir: str):
-    """
-    把 pkg_dir 目录下所有 python package 都找出来并返回
-    所谓 python package，是至少包含 __init__.py 的文件目录
-    """
     found = []
 
     for top, dirs, files in os.walk(pkg_dir):
         has_init = False
         has_python = False
         for file in files:
             if file == "__init__.py":
@@ -52,46 +64,25 @@
         if has_init and has_python:
             found.append(top)
 
     return found
 
 
 setup(name="deepdataspace",
-      version=get_version(),  # the package version, it may be different from the release version
+      version=version,
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url=url,
       author=author,
-      author_email="huweiqiang@idea.edu.cn",
       packages=find_packages("deepdataspace"),
       include_package_data=True,
-      py_modules=["dds"],
+      py_modules=["dds", "ddsop"],
       entry_points={
           "console_scripts": [
               "dds=dds:main",
+              "ddsop=ddsop:ddsop",
           ],
       },
-      install_requires=[
-          "celery==5.2.7",
-          "click==8.1.3",
-          "cryptography==39.0.1",
-          "Django==4.1.1",
-          "djangorestframework==3.14.0",
-          "django-cors-headers==3.13.0",
-          "numpy==1.21.5",
-          "opencv-contrib-python-headless==4.6.0.66",
-          "opencv-python-headless==4.6.0.66",
-          "psutil==5.9.2",
-          "pydantic==1.10.2",
-          "pymongo==4.2.0",
-          "PyYAML==6.0",
-          "Pillow==8.4.0",
-          "redis==4.3.4",
-          "requests==2.28.1",
-          "scikit-learn==1.0.2",
-          "sentry-sdk==1.19.1",
-          "tqdm==4.64.1",
-          "whitenoise==6.2.0"
-      ],
+      install_requires=install_requires,
       classifiers=classifiers,
       )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

