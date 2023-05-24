# Comparing `tmp/llnl-hatchet-2022.2.2.tar.gz` & `tmp/llnl-hatchet-2023.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/llnl-hatchet-2022.2.2.tar", last modified: Wed Apr 19 21:25:06 2023, max compression
+gzip compressed data, was "llnl-hatchet-2023.1.0.tar", last modified: Wed May 24 20:30:19 2023, max compression
```

## Comparing `llnl-hatchet-2022.2.2.tar` & `llnl-hatchet-2023.1.0.tar`

### file list

```diff
@@ -1,80 +1,123 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 21:25:05.000000 llnl-hatchet-2022.2.2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 21:25:05.000000 llnl-hatchet-2022.2.2/hatchet/
--rw-r--r--   0 root         (0) root         (0)      261 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/version.py
--rw-r--r--   0 root         (0) root         (0)    68856 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/query.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 21:25:05.000000 llnl-hatchet-2022.2.2/hatchet/writers/
--rw-r--r--   0 root         (0) root         (0)     2364 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/writers/dataframe_writer.py
--rw-r--r--   0 root         (0) root         (0)      181 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/writers/__init__.py
--rw-r--r--   0 root         (0) root         (0)      844 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/writers/hdf5_writer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 21:25:05.000000 llnl-hatchet-2022.2.2/hatchet/util/
--rw-r--r--   0 root         (0) root         (0)      256 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/util/config.py
--rw-r--r--   0 root         (0) root         (0)     1522 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/util/timer.py
--rw-r--r--   0 root         (0) root         (0)     1363 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/util/deprecated.py
--rw-r--r--   0 root         (0) root         (0)      181 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4097 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/util/colormaps.py
--rw-r--r--   0 root         (0) root         (0)      639 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/util/executable.py
--rw-r--r--   0 root         (0) root         (0)     3512 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/util/dot.py
--rw-r--r--   0 root         (0) root         (0)     3274 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/util/profiler.py
--rw-r--r--   0 root         (0) root         (0)    14363 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/graph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 21:25:05.000000 llnl-hatchet-2022.2.2/hatchet/tests/
--rw-r--r--   0 root         (0) root         (0)    43179 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/tests/conftest.py
--rw-r--r--   0 root         (0) root         (0)     7619 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/tests/dataframe_ops.py
--rw-r--r--   0 root         (0) root         (0)    10497 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/tests/caliper.py
--rw-r--r--   0 root         (0) root         (0)     1500 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/tests/timemory_func.py
--rw-r--r--   0 root         (0) root         (0)     2092 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/tests/cprofile.py
--rw-r--r--   0 root         (0) root         (0)     2176 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/tests/spotdb_test.py
--rw-r--r--   0 root         (0) root         (0)    45936 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/tests/query.py
--rw-r--r--   0 root         (0) root         (0)     7547 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/tests/hpctoolkit.py
--rw-r--r--   0 root         (0) root         (0)     4234 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/tests/pyinstrument.py
--rw-r--r--   0 root         (0) root         (0)     2455 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/tests/graph.py
--rw-r--r--   0 root         (0) root         (0)     4632 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/tests/graph_literal.py
--rw-r--r--   0 root         (0) root         (0)     1363 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/tests/callgrind.py
--rw-r--r--   0 root         (0) root         (0)     3143 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/tests/timemory_test.py
--rw-r--r--   0 root         (0) root         (0)      920 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/tests/executable.py
--rw-r--r--   0 root         (0) root         (0)     2353 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/tests/frame.py
--rw-r--r--   0 root         (0) root         (0)    40391 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/tests/graphframe.py
--rw-r--r--   0 root         (0) root         (0)     1211 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/tests/graph_ops.py
--rw-r--r--   0 root         (0) root         (0)     2988 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/tests/tau.py
--rw-r--r--   0 root         (0) root         (0)      839 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/tests/json_test.py
--rw-r--r--   0 root         (0) root         (0)     3362 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/tests/node.py
--rw-r--r--   0 root         (0) root         (0)     2454 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/tests/profiler.py
--rw-r--r--   0 root         (0) root         (0)      345 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 21:25:05.000000 llnl-hatchet-2022.2.2/hatchet/cython_modules/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 21:25:05.000000 llnl-hatchet-2022.2.2/hatchet/cython_modules/libs/
--rw-r--r--   0 root         (0) root         (0)      181 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/cython_modules/libs/__init__.py
--rw-r--r--   0 root         (0) root         (0)   800770 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/cython_modules/graphframe_modules.c
--rw-r--r--   0 root         (0) root         (0)   763943 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/cython_modules/reader_modules.c
--rw-r--r--   0 root         (0) root         (0)     2831 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/frame.py
--rw-r--r--   0 root         (0) root         (0)    61311 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/graphframe.py
--rw-r--r--   0 root         (0) root         (0)     7033 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/node.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 21:25:05.000000 llnl-hatchet-2022.2.2/hatchet/readers/
--rw-r--r--   0 root         (0) root         (0)     4154 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/readers/gprof_dot_reader.py
--rw-r--r--   0 root         (0) root         (0)    16534 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/readers/caliper_reader.py
--rw-r--r--   0 root         (0) root         (0)     3565 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/readers/pyinstrument_reader.py
--rw-r--r--   0 root         (0) root         (0)      804 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/readers/hdf5_reader.py
--rw-r--r--   0 root         (0) root         (0)     3061 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/readers/dataframe_reader.py
--rw-r--r--   0 root         (0) root         (0)      181 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/readers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5744 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/readers/literal_reader.py
--rw-r--r--   0 root         (0) root         (0)     4515 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/readers/cprofile_reader.py
--rw-r--r--   0 root         (0) root         (0)    25694 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/readers/timemory_reader.py
--rw-r--r--   0 root         (0) root         (0)    23415 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/readers/tau_reader.py
--rw-r--r--   0 root         (0) root         (0)    16325 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/readers/hpctoolkit_reader.py
--rw-r--r--   0 root         (0) root         (0)    18371 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/readers/caliper_native_reader.py
--rw-r--r--   0 root         (0) root         (0)     5976 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/readers/spotdb_reader.py
--rw-r--r--   0 root         (0) root         (0)     2060 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/readers/json_reader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 21:25:05.000000 llnl-hatchet-2022.2.2/hatchet/external/
--rw-r--r--   0 root         (0) root         (0)    13290 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/external/console.py
--rw-r--r--   0 root         (0) root         (0)      285 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/hatchet/external/__init__.py
--rw-r--r--   0 root         (0) root         (0)      385 2023-04-19 21:25:05.000000 llnl-hatchet-2022.2.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1092 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      534 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1167 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/NOTICE
--rw-r--r--   0 root         (0) root         (0)     4370 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/README.md
--rw-r--r--   0 root         (0) root         (0)     1880 2022-10-25 04:17:02.000000 llnl-hatchet-2022.2.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 21:25:05.000000 llnl-hatchet-2022.2.2/llnl_hatchet.egg-info/
--rw-r--r--   0 root         (0) root         (0)      385 2023-04-19 21:25:04.000000 llnl-hatchet-2022.2.2/llnl_hatchet.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1869 2023-04-19 21:25:05.000000 llnl-hatchet-2022.2.2/llnl_hatchet.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       71 2023-04-19 21:25:04.000000 llnl-hatchet-2022.2.2/llnl_hatchet.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-19 21:25:04.000000 llnl-hatchet-2022.2.2/llnl_hatchet.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 21:25:04.000000 llnl-hatchet-2022.2.2/llnl_hatchet.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-19 21:25:05.000000 llnl-hatchet-2022.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 20:30:19.568215 llnl-hatchet-2023.1.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-05-24 20:30:06.000000 llnl-hatchet-2023.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      262 2023-05-24 20:30:06.000000 llnl-hatchet-2023.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1167 2023-05-24 20:30:06.000000 llnl-hatchet-2023.1.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (122)     4996 2023-05-24 20:30:19.568215 llnl-hatchet-2023.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4370 2023-05-24 20:30:06.000000 llnl-hatchet-2023.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 20:30:19.544215 llnl-hatchet-2023.1.0/hatchet/
+-rw-r--r--   0 runner    (1001) docker     (122)      345 2023-05-24 20:30:06.000000 llnl-hatchet-2023.1.0/hatchet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 20:30:19.544215 llnl-hatchet-2023.1.0/hatchet/cython_modules/
+-rw-r--r--   0 runner    (1001) docker     (122)     2496 2023-05-24 20:30:06.000000 llnl-hatchet-2023.1.0/hatchet/cython_modules/graphframe_modules.pyx
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 20:30:19.544215 llnl-hatchet-2023.1.0/hatchet/cython_modules/libs/
+-rw-r--r--   0 runner    (1001) docker     (122)      181 2023-05-24 20:30:06.000000 llnl-hatchet-2023.1.0/hatchet/cython_modules/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      667 2023-05-24 20:30:06.000000 llnl-hatchet-2023.1.0/hatchet/cython_modules/reader_modules.pyx
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 20:30:19.544215 llnl-hatchet-2023.1.0/hatchet/external/
+-rw-r--r--   0 runner    (1001) docker     (122)      285 2023-05-24 20:30:06.000000 llnl-hatchet-2023.1.0/hatchet/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13290 2023-05-24 20:30:06.000000 llnl-hatchet-2023.1.0/hatchet/external/console.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2831 2023-05-24 20:30:06.000000 llnl-hatchet-2023.1.0/hatchet/frame.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14363 2023-05-24 20:30:06.000000 llnl-hatchet-2023.1.0/hatchet/graph.py
+-rw-r--r--   0 runner    (1001) docker     (122)    63094 2023-05-24 20:30:06.000000 llnl-hatchet-2023.1.0/hatchet/graphframe.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7033 2023-05-24 20:30:06.000000 llnl-hatchet-2023.1.0/hatchet/node.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 20:30:19.548215 llnl-hatchet-2023.1.0/hatchet/query/
+-rw-r--r--   0 runner    (1001) docker     (122)     2283 2023-05-24 20:30:06.000000 llnl-hatchet-2023.1.0/hatchet/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13191 2023-05-24 20:30:06.000000 llnl-hatchet-2023.1.0/hatchet/query/compat.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6655 2023-05-24 20:30:06.000000 llnl-hatchet-2023.1.0/hatchet/query/compound.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11501 2023-05-24 20:30:06.000000 llnl-hatchet-2023.1.0/hatchet/query/engine.py
+-rw-r--r--   0 runner    (1001) docker     (122)      789 2023-05-24 20:30:06.000000 llnl-hatchet-2023.1.0/hatchet/query/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11045 2023-05-24 20:30:06.000000 llnl-hatchet-2023.1.0/hatchet/query/object_dialect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3654 2023-05-24 20:30:06.000000 llnl-hatchet-2023.1.0/hatchet/query/query.py
+-rw-r--r--   0 runner    (1001) docker     (122)    57905 2023-05-24 20:30:06.000000 llnl-hatchet-2023.1.0/hatchet/query/string_dialect.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 20:30:19.552215 llnl-hatchet-2023.1.0/hatchet/readers/
+-rw-r--r--   0 runner    (1001) docker     (122)      181 2023-05-24 20:30:06.000000 llnl-hatchet-2023.1.0/hatchet/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20177 2023-05-24 20:30:06.000000 llnl-hatchet-2023.1.0/hatchet/readers/caliper_native_reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16534 2023-05-24 20:30:06.000000 llnl-hatchet-2023.1.0/hatchet/readers/caliper_reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4515 2023-05-24 20:30:06.000000 llnl-hatchet-2023.1.0/hatchet/readers/cprofile_reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3061 2023-05-24 20:30:06.000000 llnl-hatchet-2023.1.0/hatchet/readers/dataframe_reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4154 2023-05-24 20:30:06.000000 llnl-hatchet-2023.1.0/hatchet/readers/gprof_dot_reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)      804 2023-05-24 20:30:06.000000 llnl-hatchet-2023.1.0/hatchet/readers/hdf5_reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16325 2023-05-24 20:30:06.000000 llnl-hatchet-2023.1.0/hatchet/readers/hpctoolkit_reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2060 2023-05-24 20:30:06.000000 llnl-hatchet-2023.1.0/hatchet/readers/json_reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5744 2023-05-24 20:30:06.000000 llnl-hatchet-2023.1.0/hatchet/readers/literal_reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3565 2023-05-24 20:30:06.000000 llnl-hatchet-2023.1.0/hatchet/readers/pyinstrument_reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5976 2023-05-24 20:30:06.000000 llnl-hatchet-2023.1.0/hatchet/readers/spotdb_reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23415 2023-05-24 20:30:06.000000 llnl-hatchet-2023.1.0/hatchet/readers/tau_reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25695 2023-05-24 20:30:06.000000 llnl-hatchet-2023.1.0/hatchet/readers/timemory_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 20:30:19.556215 llnl-hatchet-2023.1.0/hatchet/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)    10497 2023-05-24 20:30:06.000000 llnl-hatchet-2023.1.0/hatchet/tests/caliper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1363 2023-05-24 20:30:06.000000 llnl-hatchet-2023.1.0/hatchet/tests/callgrind.py
+-rw-r--r--   0 runner    (1001) docker     (122)    43181 2023-05-24 20:30:06.000000 llnl-hatchet-2023.1.0/hatchet/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2092 2023-05-24 20:30:06.000000 llnl-hatchet-2023.1.0/hatchet/tests/cprofile.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7619 2023-05-24 20:30:07.000000 llnl-hatchet-2023.1.0/hatchet/tests/dataframe_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)      920 2023-05-24 20:30:07.000000 llnl-hatchet-2023.1.0/hatchet/tests/executable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2353 2023-05-24 20:30:07.000000 llnl-hatchet-2023.1.0/hatchet/tests/frame.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2455 2023-05-24 20:30:07.000000 llnl-hatchet-2023.1.0/hatchet/tests/graph.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4632 2023-05-24 20:30:07.000000 llnl-hatchet-2023.1.0/hatchet/tests/graph_literal.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1211 2023-05-24 20:30:07.000000 llnl-hatchet-2023.1.0/hatchet/tests/graph_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)    40391 2023-05-24 20:30:07.000000 llnl-hatchet-2023.1.0/hatchet/tests/graphframe.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7547 2023-05-24 20:30:07.000000 llnl-hatchet-2023.1.0/hatchet/tests/hpctoolkit.py
+-rw-r--r--   0 runner    (1001) docker     (122)      839 2023-05-24 20:30:07.000000 llnl-hatchet-2023.1.0/hatchet/tests/json_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3362 2023-05-24 20:30:07.000000 llnl-hatchet-2023.1.0/hatchet/tests/node.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2454 2023-05-24 20:30:07.000000 llnl-hatchet-2023.1.0/hatchet/tests/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4234 2023-05-24 20:30:07.000000 llnl-hatchet-2023.1.0/hatchet/tests/pyinstrument.py
+-rw-r--r--   0 runner    (1001) docker     (122)    49299 2023-05-24 20:30:07.000000 llnl-hatchet-2023.1.0/hatchet/tests/query.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23130 2023-05-24 20:30:07.000000 llnl-hatchet-2023.1.0/hatchet/tests/query_compat.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2176 2023-05-24 20:30:07.000000 llnl-hatchet-2023.1.0/hatchet/tests/spotdb_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2988 2023-05-24 20:30:07.000000 llnl-hatchet-2023.1.0/hatchet/tests/tau.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1500 2023-05-24 20:30:07.000000 llnl-hatchet-2023.1.0/hatchet/tests/timemory_func.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3143 2023-05-24 20:30:07.000000 llnl-hatchet-2023.1.0/hatchet/tests/timemory_test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 20:30:19.556215 llnl-hatchet-2023.1.0/hatchet/util/
+-rw-r--r--   0 runner    (1001) docker     (122)      181 2023-05-24 20:30:07.000000 llnl-hatchet-2023.1.0/hatchet/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4097 2023-05-24 20:30:07.000000 llnl-hatchet-2023.1.0/hatchet/util/colormaps.py
+-rw-r--r--   0 runner    (1001) docker     (122)      256 2023-05-24 20:30:07.000000 llnl-hatchet-2023.1.0/hatchet/util/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1363 2023-05-24 20:30:07.000000 llnl-hatchet-2023.1.0/hatchet/util/deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3512 2023-05-24 20:30:07.000000 llnl-hatchet-2023.1.0/hatchet/util/dot.py
+-rw-r--r--   0 runner    (1001) docker     (122)      639 2023-05-24 20:30:07.000000 llnl-hatchet-2023.1.0/hatchet/util/executable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3274 2023-05-24 20:30:07.000000 llnl-hatchet-2023.1.0/hatchet/util/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1522 2023-05-24 20:30:07.000000 llnl-hatchet-2023.1.0/hatchet/util/timer.py
+-rw-r--r--   0 runner    (1001) docker     (122)      261 2023-05-24 20:30:07.000000 llnl-hatchet-2023.1.0/hatchet/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 20:30:19.560215 llnl-hatchet-2023.1.0/hatchet/vis/
+-rw-r--r--   0 runner    (1001) docker     (122)     1473 2023-05-24 20:30:07.000000 llnl-hatchet-2023.1.0/hatchet/vis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1790 2023-05-24 20:30:07.000000 llnl-hatchet-2023.1.0/hatchet/vis/loader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1238 2023-05-24 20:30:07.000000 llnl-hatchet-2023.1.0/hatchet/vis/package.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 20:30:19.560215 llnl-hatchet-2023.1.0/hatchet/vis/scripts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 20:30:07.000000 llnl-hatchet-2023.1.0/hatchet/vis/scripts/boxplot.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 20:30:19.560215 llnl-hatchet-2023.1.0/hatchet/vis/scripts/cct/
+-rw-r--r--   0 runner    (1001) docker     (122)    46419 2023-05-24 20:30:07.000000 llnl-hatchet-2023.1.0/hatchet/vis/scripts/cct/cct_chart_view.js
+-rw-r--r--   0 runner    (1001) docker     (122)    10171 2023-05-24 20:30:07.000000 llnl-hatchet-2023.1.0/hatchet/vis/scripts/cct/cct_color_manager.js
+-rw-r--r--   0 runner    (1001) docker     (122)     3017 2023-05-24 20:30:07.000000 llnl-hatchet-2023.1.0/hatchet/vis/scripts/cct/cct_controller.js
+-rw-r--r--   0 runner    (1001) docker     (122)     2542 2023-05-24 20:30:07.000000 llnl-hatchet-2023.1.0/hatchet/vis/scripts/cct/cct_globals.js
+-rw-r--r--   0 runner    (1001) docker     (122)    22694 2023-05-24 20:30:07.000000 llnl-hatchet-2023.1.0/hatchet/vis/scripts/cct/cct_menu_view.js
+-rw-r--r--   0 runner    (1001) docker     (122)    23701 2023-05-24 20:30:07.000000 llnl-hatchet-2023.1.0/hatchet/vis/scripts/cct/cct_model.js
+-rw-r--r--   0 runner    (1001) docker     (122)    18207 2023-05-24 20:30:07.000000 llnl-hatchet-2023.1.0/hatchet/vis/scripts/cct/cct_repr.js
+-rw-r--r--   0 runner    (1001) docker     (122)    26303 2023-05-24 20:30:07.000000 llnl-hatchet-2023.1.0/hatchet/vis/scripts/cct/cct_scented_slider_popup.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1234 2023-05-24 20:30:07.000000 llnl-hatchet-2023.1.0/hatchet/vis/scripts/cct/cct_stats.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1881 2023-05-24 20:30:07.000000 llnl-hatchet-2023.1.0/hatchet/vis/scripts/cct/cct_tooltip_view.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1169 2023-05-24 20:30:07.000000 llnl-hatchet-2023.1.0/hatchet/vis/scripts/cct.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 20:30:19.560215 llnl-hatchet-2023.1.0/hatchet/vis/scripts/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      504 2023-05-24 20:30:07.000000 llnl-hatchet-2023.1.0/hatchet/vis/scripts/utils/view.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 20:30:19.564215 llnl-hatchet-2023.1.0/hatchet/vis/static/
+-rw-r--r--   0 runner    (1001) docker     (122)      138 2023-05-24 20:30:07.000000 llnl-hatchet-2023.1.0/hatchet/vis/static/boxplot_bundle.html
+-rw-r--r--   0 runner    (1001) docker     (122)   181961 2023-05-24 20:30:07.000000 llnl-hatchet-2023.1.0/hatchet/vis/static/boxplot_bundle.js
+-rw-r--r--   0 runner    (1001) docker     (122)      290 2023-05-24 20:30:07.000000 llnl-hatchet-2023.1.0/hatchet/vis/static/cct_bundle.html
+-rw-r--r--   0 runner    (1001) docker     (122)   750167 2023-05-24 20:30:07.000000 llnl-hatchet-2023.1.0/hatchet/vis/static/cct_bundle.js
+-rw-r--r--   0 runner    (1001) docker     (122)      733 2023-05-24 20:30:07.000000 llnl-hatchet-2023.1.0/hatchet/vis/static_fixer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 20:30:19.564215 llnl-hatchet-2023.1.0/hatchet/vis/styles/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 20:30:07.000000 llnl-hatchet-2023.1.0/hatchet/vis/styles/boxplot.css
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 20:30:07.000000 llnl-hatchet-2023.1.0/hatchet/vis/styles/cct.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 20:30:19.564215 llnl-hatchet-2023.1.0/hatchet/vis/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 20:30:07.000000 llnl-hatchet-2023.1.0/hatchet/vis/templates/boxplot.html
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 20:30:07.000000 llnl-hatchet-2023.1.0/hatchet/vis/templates/cct.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1005 2023-05-24 20:30:07.000000 llnl-hatchet-2023.1.0/hatchet/vis/webpack.config.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 20:30:19.564215 llnl-hatchet-2023.1.0/hatchet/writers/
+-rw-r--r--   0 runner    (1001) docker     (122)      181 2023-05-24 20:30:07.000000 llnl-hatchet-2023.1.0/hatchet/writers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2364 2023-05-24 20:30:07.000000 llnl-hatchet-2023.1.0/hatchet/writers/dataframe_writer.py
+-rw-r--r--   0 runner    (1001) docker     (122)      844 2023-05-24 20:30:07.000000 llnl-hatchet-2023.1.0/hatchet/writers/hdf5_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 20:30:19.568215 llnl-hatchet-2023.1.0/llnl_hatchet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4996 2023-05-24 20:30:19.000000 llnl-hatchet-2023.1.0/llnl_hatchet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3013 2023-05-24 20:30:19.000000 llnl-hatchet-2023.1.0/llnl_hatchet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-24 20:30:19.000000 llnl-hatchet-2023.1.0/llnl_hatchet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      145 2023-05-24 20:30:19.000000 llnl-hatchet-2023.1.0/llnl_hatchet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-05-24 20:30:19.000000 llnl-hatchet-2023.1.0/llnl_hatchet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      650 2023-05-24 20:30:07.000000 llnl-hatchet-2023.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-24 20:30:19.568215 llnl-hatchet-2023.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     3471 2023-05-24 20:30:07.000000 llnl-hatchet-2023.1.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `llnl-hatchet-2022.2.2/hatchet/writers/dataframe_writer.py` & `llnl-hatchet-2023.1.0/hatchet/writers/dataframe_writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017-2022 Lawrence Livermore National Security, LLC and other
+# Copyright 2017-2023 Lawrence Livermore National Security, LLC and other
 # Hatchet Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: MIT
 
 from hatchet.node import Node
 
 from abc import abstractmethod
```

### Comparing `llnl-hatchet-2022.2.2/hatchet/writers/hdf5_writer.py` & `llnl-hatchet-2023.1.0/hatchet/writers/hdf5_writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017-2022 Lawrence Livermore National Security, LLC and other
+# Copyright 2017-2023 Lawrence Livermore National Security, LLC and other
 # Hatchet Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: MIT
 
 import warnings
 import sys
```

### Comparing `llnl-hatchet-2022.2.2/hatchet/util/timer.py` & `llnl-hatchet-2023.1.0/hatchet/util/timer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017-2022 Lawrence Livermore National Security, LLC and other
+# Copyright 2017-2023 Lawrence Livermore National Security, LLC and other
 # Hatchet Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: MIT
 
 from collections import OrderedDict
 from contextlib import contextmanager
 from datetime import datetime
```

### Comparing `llnl-hatchet-2022.2.2/hatchet/util/deprecated.py` & `llnl-hatchet-2023.1.0/hatchet/util/deprecated.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017-2022 Lawrence Livermore National Security, LLC and other
+# Copyright 2017-2023 Lawrence Livermore National Security, LLC and other
 # Hatchet Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: MIT
 
 import functools
```

### Comparing `llnl-hatchet-2022.2.2/hatchet/util/colormaps.py` & `llnl-hatchet-2023.1.0/hatchet/util/colormaps.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017-2022 Lawrence Livermore National Security, LLC and other
+# Copyright 2017-2023 Lawrence Livermore National Security, LLC and other
 # Hatchet Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: MIT
 
 
 class ColorMaps:
     # RdYlGn (Default) color map
```

### Comparing `llnl-hatchet-2022.2.2/hatchet/util/executable.py` & `llnl-hatchet-2023.1.0/hatchet/util/executable.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017-2022 Lawrence Livermore National Security, LLC and other
+# Copyright 2017-2023 Lawrence Livermore National Security, LLC and other
 # Hatchet Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: MIT
 
 import os
```

### Comparing `llnl-hatchet-2022.2.2/hatchet/util/dot.py` & `llnl-hatchet-2023.1.0/hatchet/util/dot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017-2022 Lawrence Livermore National Security, LLC and other
+# Copyright 2017-2023 Lawrence Livermore National Security, LLC and other
 # Hatchet Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: MIT
 
 import matplotlib.cm
 import matplotlib.colors
```

### Comparing `llnl-hatchet-2022.2.2/hatchet/util/profiler.py` & `llnl-hatchet-2023.1.0/hatchet/util/profiler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017-2022 Lawrence Livermore National Security, LLC and other
+# Copyright 2017-2023 Lawrence Livermore National Security, LLC and other
 # Hatchet Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: MIT
 
 import cProfile
 import traceback
 import sys
```

### Comparing `llnl-hatchet-2022.2.2/hatchet/graph.py` & `llnl-hatchet-2023.1.0/hatchet/graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017-2022 Lawrence Livermore National Security, LLC and other
+# Copyright 2017-2023 Lawrence Livermore National Security, LLC and other
 # Hatchet Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: MIT
 
 from collections import defaultdict
 
 from .node import Node, traversal_order
```

### Comparing `llnl-hatchet-2022.2.2/hatchet/tests/conftest.py` & `llnl-hatchet-2023.1.0/hatchet/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017-2022 Lawrence Livermore National Security, LLC and other
+# Copyright 2017-2023 Lawrence Livermore National Security, LLC and other
 # Hatchet Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: MIT
 
 import os
 import sys
 import shutil
@@ -1002,15 +1002,15 @@
     timemory.settings.flat_profile = True
 
     with marker(components, key="main"):
         nx = 10
         ny = 10
         tol = 5.0e-2
         profl_arr = np.random.rand(nx, ny)
-        trace_arr = np.zeros([nx, ny], dtype=np.float)
+        trace_arr = np.zeros([nx, ny], dtype=np.float64)
         trace_arr[:, :] = profl_arr[:, :]
 
         # restrict the scope of the profiler
         ProfilerConfig.only_filenames = ["timemory_func.py", "_methods.py"]
         ProfilerConfig.include_line = False
         prof_func(profl_arr, tol)
```

### Comparing `llnl-hatchet-2022.2.2/hatchet/tests/dataframe_ops.py` & `llnl-hatchet-2023.1.0/hatchet/tests/dataframe_ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017-2022 Lawrence Livermore National Security, LLC and other
+# Copyright 2017-2023 Lawrence Livermore National Security, LLC and other
 # Hatchet Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: MIT
 
 from __future__ import division
 
 from hatchet import GraphFrame
```

### Comparing `llnl-hatchet-2022.2.2/hatchet/tests/caliper.py` & `llnl-hatchet-2023.1.0/hatchet/tests/caliper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017-2022 Lawrence Livermore National Security, LLC and other
+# Copyright 2017-2023 Lawrence Livermore National Security, LLC and other
 # Hatchet Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: MIT
 
 import subprocess
 import numpy as np
```

### Comparing `llnl-hatchet-2022.2.2/hatchet/tests/timemory_func.py` & `llnl-hatchet-2023.1.0/hatchet/tests/timemory_func.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017-2022 Lawrence Livermore National Security, LLC and other
+# Copyright 2017-2023 Lawrence Livermore National Security, LLC and other
 # Hatchet Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: MIT
 
 import numpy as np
 
 timemory_avail = True
```

### Comparing `llnl-hatchet-2022.2.2/hatchet/tests/cprofile.py` & `llnl-hatchet-2023.1.0/hatchet/tests/cprofile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017-2022 Lawrence Livermore National Security, LLC and other
+# Copyright 2017-2023 Lawrence Livermore National Security, LLC and other
 # Hatchet Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: MIT
 
 import numpy as np
 import re
```

### Comparing `llnl-hatchet-2022.2.2/hatchet/tests/spotdb_test.py` & `llnl-hatchet-2023.1.0/hatchet/tests/spotdb_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017-2022 Lawrence Livermore National Security, LLC and other
+# Copyright 2017-2023 Lawrence Livermore National Security, LLC and other
 # Hatchet Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: MIT
 
 import pytest
 
 from hatchet import GraphFrame
```

### Comparing `llnl-hatchet-2022.2.2/hatchet/tests/query.py` & `llnl-hatchet-2023.1.0/hatchet/tests/query.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-# Copyright 2017-2022 Lawrence Livermore National Security, LLC and other
+# Copyright 2017-2023 Lawrence Livermore National Security, LLC and other
 # Hatchet Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: MIT
 
 import pytest
 
 import re
 
 import numpy as np
 
 from hatchet import GraphFrame
 from hatchet.node import traversal_order
 from hatchet.query import (
-    QueryMatcher,
+    Query,
+    ObjectQuery,
+    StringQuery,
+    parse_string_dialect,
+    QueryEngine,
     InvalidQueryFilter,
     InvalidQueryPath,
-    AbstractQuery,
-    NaryQuery,
-    AndQuery,
-    OrQuery,
-    XorQuery,
-    IntersectionQuery,
-    UnionQuery,
-    SymDifferenceQuery,
-    CypherQuery,
-    parse_cypher_query,
+    CompoundQuery,
+    ConjunctionQuery,
+    DisjunctionQuery,
+    ExclusiveDisjunctionQuery,
+    NegationQuery,
 )
+from hatchet.query.errors import MultiIndexModeMismatch
 
 
-def test_construct_high_level_api():
+def test_construct_object_dialect():
     mock_node_mpi = {"name": "MPI_Bcast"}
     mock_node_ibv = {"name": "ibv_reg_mr"}
     mock_node_time_true = {"time (inc)": 0.1}
     mock_node_time_false = {"time (inc)": 0.001}
     path1 = [{"name": "MPI_[_a-zA-Z]*"}, "*", {"name": "ibv[_a-zA-Z]*"}]
     path2 = [{"name": "MPI_[_a-zA-Z]*"}, 2, {"name": "ibv[_a-zA-Z]*"}]
     path3 = [
@@ -41,18 +41,18 @@
         {"name": "ibv[_a-zA-Z]*"},
     ]
     path4 = [
         {"name": "MPI_[_a-zA-Z]*"},
         (3, {"time (inc)": 0.1}),
         {"name": "ibv[_a-zA-Z]*"},
     ]
-    query1 = QueryMatcher(path1)
-    query2 = QueryMatcher(path2)
-    query3 = QueryMatcher(path3)
-    query4 = QueryMatcher(path4)
+    query1 = ObjectQuery(path1)
+    query2 = ObjectQuery(path2)
+    query3 = ObjectQuery(path3)
+    query4 = ObjectQuery(path4)
 
     assert query1.query_pattern[0][0] == "."
     assert query1.query_pattern[0][1](mock_node_mpi)
     assert not query1.query_pattern[0][1](mock_node_ibv)
     assert not query1.query_pattern[0][1](mock_node_time_true)
     assert query1.query_pattern[1][0] == "*"
     assert query1.query_pattern[1][1](mock_node_mpi)
@@ -107,22 +107,22 @@
 
     invalid_path = [
         {"name": "MPI_[_a-zA-Z]*"},
         ({"bad": "wildcard"}, {"time (inc)": 0.1}),
         {"name": "ibv[_a-zA-Z]*"},
     ]
     with pytest.raises(InvalidQueryPath):
-        _ = QueryMatcher(invalid_path)
+        _ = ObjectQuery(invalid_path)
 
     invalid_path = [["name", "MPI_[_a-zA-Z]*"], "*", {"name": "ibv[_a-zA-Z]*"}]
     with pytest.raises(InvalidQueryPath):
-        _ = QueryMatcher(invalid_path)
+        _ = ObjectQuery(invalid_path)
 
 
-def test_construct_low_level_api():
+def test_construct_base_query():
     mock_node_mpi = {"name": "MPI_Bcast"}
     mock_node_ibv = {"name": "ibv_reg_mr"}
     mock_node_time_true = {"time (inc)": 0.1}
     mock_node_time_false = {"time (inc)": 0.001}
 
     def mpi_filter(df_row):
         if "name" not in df_row:
@@ -144,61 +144,57 @@
         return df_row["time (inc)"] >= 0.1
 
     def time_eq_filter(df_row):
         if "time (inc)" not in df_row:
             return False
         return df_row["time (inc)"] == 0.1
 
-    query = QueryMatcher()
+    query = Query()
 
-    query.match(filter_func=mpi_filter).rel("*").rel(filter_func=ibv_filter)
+    query.match(predicate=mpi_filter).rel("*").rel(predicate=ibv_filter)
     assert query.query_pattern[0][0] == "."
     assert query.query_pattern[0][1](mock_node_mpi)
     assert not query.query_pattern[0][1](mock_node_ibv)
     assert not query.query_pattern[0][1](mock_node_time_true)
     assert query.query_pattern[1][0] == "*"
     assert query.query_pattern[1][1](mock_node_mpi)
     assert query.query_pattern[1][1](mock_node_ibv)
     assert query.query_pattern[1][1](mock_node_time_true)
     assert query.query_pattern[1][1](mock_node_time_false)
     assert query.query_pattern[2][0] == "."
 
-    query.match(filter_func=mpi_filter).rel(2).rel(filter_func=ibv_filter)
+    query.match(predicate=mpi_filter).rel(2).rel(predicate=ibv_filter)
     assert query.query_pattern[0][0] == "."
     assert query.query_pattern[1][0] == "."
     assert query.query_pattern[1][1](mock_node_mpi)
     assert query.query_pattern[1][1](mock_node_ibv)
     assert query.query_pattern[1][1](mock_node_time_true)
     assert query.query_pattern[1][1](mock_node_time_false)
     assert query.query_pattern[2][0] == "."
     assert query.query_pattern[2][1](mock_node_mpi)
     assert query.query_pattern[2][1](mock_node_ibv)
     assert query.query_pattern[2][1](mock_node_time_true)
     assert query.query_pattern[2][1](mock_node_time_false)
     assert query.query_pattern[3][0] == "."
 
-    query.match(filter_func=mpi_filter).rel("+", time_ge_filter).rel(
-        filter_func=ibv_filter
-    )
+    query.match(predicate=mpi_filter).rel("+", time_ge_filter).rel(predicate=ibv_filter)
     assert query.query_pattern[0][0] == "."
     assert query.query_pattern[1][0] == "."
     assert query.query_pattern[2][0] == "*"
     assert not query.query_pattern[1][1](mock_node_mpi)
     assert not query.query_pattern[1][1](mock_node_ibv)
     assert query.query_pattern[1][1](mock_node_time_true)
     assert not query.query_pattern[1][1](mock_node_time_false)
     assert not query.query_pattern[2][1](mock_node_mpi)
     assert not query.query_pattern[2][1](mock_node_ibv)
     assert query.query_pattern[2][1](mock_node_time_true)
     assert not query.query_pattern[2][1](mock_node_time_false)
     assert query.query_pattern[3][0] == "."
 
-    query.match(filter_func=mpi_filter).rel(3, time_eq_filter).rel(
-        filter_func=ibv_filter
-    )
+    query.match(predicate=mpi_filter).rel(3, time_eq_filter).rel(predicate=ibv_filter)
     assert query.query_pattern[0][0] == "."
     assert query.query_pattern[1][0] == "."
     assert not query.query_pattern[1][1](mock_node_mpi)
     assert not query.query_pattern[1][1](mock_node_ibv)
     assert query.query_pattern[1][1](mock_node_time_true)
     assert not query.query_pattern[1][1](mock_node_time_false)
     assert query.query_pattern[2][0] == "."
@@ -210,29 +206,30 @@
     assert not query.query_pattern[3][1](mock_node_mpi)
     assert not query.query_pattern[3][1](mock_node_ibv)
     assert query.query_pattern[3][1](mock_node_time_true)
     assert not query.query_pattern[3][1](mock_node_time_false)
     assert query.query_pattern[4][0] == "."
 
     with pytest.raises(InvalidQueryPath):
-        _ = QueryMatcher().rel(".", lambda row: True)
+        _ = Query().rel(".", lambda row: True)
 
 
 def test_node_caching(mock_graph_literal):
     path = [{"name": "fr[a-z]+"}, ("+", {"time (inc)": ">= 25.0"}), {"name": "baz"}]
     gf = GraphFrame.from_literal(mock_graph_literal)
     node = gf.graph.roots[0].children[2].children[0]
 
-    query = QueryMatcher(path)
-    query._cache_node(gf, node)
-
-    assert 0 in query.search_cache[node._hatchet_nid]
-    assert 1 in query.search_cache[node._hatchet_nid]
-    assert 2 in query.search_cache[node._hatchet_nid]
-    assert 3 not in query.search_cache[node._hatchet_nid]
+    query = ObjectQuery(path)
+    engine = QueryEngine()
+    engine._cache_node(node, query, gf.dataframe)
+
+    assert 0 in engine.search_cache[node._hatchet_nid]
+    assert 1 in engine.search_cache[node._hatchet_nid]
+    assert 2 in engine.search_cache[node._hatchet_nid]
+    assert 3 not in engine.search_cache[node._hatchet_nid]
 
 
 def test_match_0_or_more_wildcard(mock_graph_literal):
     path = [
         {"name": "qux"},
         ("*", {"time (inc)": "> 10"}),
         {"name": "gr[a-z]+", "time (inc)": "<= 10"},
@@ -246,38 +243,40 @@
             node.children[0],
             node.children[0].children[0],
             node.children[0].children[0].children[0],
         ],
         [node.children[0], node.children[0].children[0]],
     ]
 
-    query = QueryMatcher(path)
+    query = ObjectQuery(path)
+    engine = QueryEngine()
     matched_paths = []
     for child in sorted(node.children, key=traversal_order):
-        match = query._match_0_or_more(gf, child, 1)
+        match = engine._match_0_or_more(query, gf.dataframe, child, 1)
         if match is not None:
             matched_paths.extend(match)
 
     assert sorted(matched_paths, key=len) == sorted(correct_paths, key=len)
-    assert query._match_0_or_more(gf, none_node, 1) is None
+    assert engine._match_0_or_more(query, gf.dataframe, none_node, 1) is None
 
 
 def test_match_1(mock_graph_literal):
     gf = GraphFrame.from_literal(mock_graph_literal)
     path = [
         {"name": "qux"},
         ("*", {"time (inc)": "> 10"}),
         {"name": "gr[a-z]+", "time (inc)": "<= 10.0"},
     ]
-    query = QueryMatcher(path)
+    query = ObjectQuery(path)
+    engine = QueryEngine()
 
-    assert query._match_1(gf, gf.graph.roots[0].children[0], 2) == [
+    assert engine._match_1(query, gf.dataframe, gf.graph.roots[0].children[0], 2) == [
         [gf.graph.roots[0].children[0].children[1]]
     ]
-    assert query._match_1(gf, gf.graph.roots[0], 2) is None
+    assert engine._match_1(query, gf.dataframe, gf.graph.roots[0], 2) is None
 
 
 def test_match(mock_graph_literal):
     gf = GraphFrame.from_literal(mock_graph_literal)
     root = gf.graph.roots[0].children[2]
 
     path0 = [
@@ -292,26 +291,29 @@
             root,
             root.children[0],
             root.children[0].children[1],
             root.children[0].children[1].children[0],
             root.children[0].children[1].children[0].children[0],
         ]
     ]
-    query0 = QueryMatcher(path0)
-    assert query0._match_pattern(gf, root, 0) == match0
+    query0 = ObjectQuery(path0)
+    engine = QueryEngine()
+    assert engine._match_pattern(query0, gf.dataframe, root, 0) == match0
+
+    engine.reset_cache()
 
     path1 = [
         {"name": "waldo"},
         ("+", {}),
         {"time (inc)": ">= 20.0"},
         "+",
         {"time (inc)": 7.5, "time": 7.5},
     ]
-    query1 = QueryMatcher(path1)
-    assert query1._match_pattern(gf, root, 0) is None
+    query1 = ObjectQuery(path1)
+    assert engine._match_pattern(query1, gf.dataframe, root, 0) is None
 
 
 def test_apply(mock_graph_literal):
     gf = GraphFrame.from_literal(mock_graph_literal)
     path = [
         {"time (inc)": ">= 30.0"},
         (2, {"name": "[^b][a-z]+"}),
@@ -322,75 +324,76 @@
     match = [
         root,
         root.children[1],
         root.children[1].children[0],
         root.children[1].children[0].children[0],
         root.children[1].children[0].children[0].children[1],
     ]
-    query = QueryMatcher(path)
+    query = ObjectQuery(path)
+    engine = QueryEngine()
 
-    assert sorted(query.apply(gf)) == sorted(match)
+    assert sorted(engine.apply(query, gf.graph, gf.dataframe)) == sorted(match)
 
     path = [{"time (inc)": ">= 30.0"}, ".", {"name": "bar"}, "*"]
     match = [
         root.children[1].children[0],
         root.children[1].children[0].children[0],
         root.children[1].children[0].children[0].children[0],
         root.children[1].children[0].children[0].children[0].children[0],
         root.children[1].children[0].children[0].children[0].children[1],
     ]
-    query = QueryMatcher(path)
-    assert sorted(query.apply(gf)) == sorted(match)
+    query = ObjectQuery(path)
+    assert sorted(engine.apply(query, gf.graph, gf.dataframe)) == sorted(match)
 
     path = [{"name": "foo"}, {"name": "bar"}, {"time": 5.0}]
     match = [root, root.children[0], root.children[0].children[0]]
-    query = QueryMatcher(path)
-    assert sorted(query.apply(gf)) == sorted(match)
+    query = ObjectQuery(path)
+    assert sorted(engine.apply(query, gf.graph, gf.dataframe)) == sorted(match)
 
     path = [{"name": "foo"}, {"name": "qux"}, ("+", {"time (inc)": "> 15.0"})]
     match = [
         root,
         root.children[1],
         root.children[1].children[0],
         root.children[1].children[0].children[0],
         root.children[1].children[0].children[0].children[0],
     ]
-    query = QueryMatcher(path)
-    assert sorted(query.apply(gf)) == sorted(match)
+    query = ObjectQuery(path)
+    assert sorted(engine.apply(query, gf.graph, gf.dataframe)) == sorted(match)
 
     path = [{"name": "this"}, ("*", {"name": "is"}), {"name": "nonsense"}]
 
-    query = QueryMatcher(path)
-    assert query.apply(gf) == []
+    query = ObjectQuery(path)
+    assert engine.apply(query, gf.graph, gf.dataframe) == []
 
     path = [{"name": 5}, "*", {"name": "whatever"}]
-    query = QueryMatcher(path)
+    query = ObjectQuery(path)
     with pytest.raises(InvalidQueryFilter):
-        query.apply(gf)
+        engine.apply(query, gf.graph, gf.dataframe)
 
     path = [{"time": "badstring"}, "*", {"name": "whatever"}]
-    query = QueryMatcher(path)
+    query = ObjectQuery(path)
     with pytest.raises(InvalidQueryFilter):
-        query.apply(gf)
+        engine.apply(query, gf.graph, gf.dataframe)
 
     class DummyType:
         def __init__(self):
             self.x = 5.0
             self.y = -1
             self.z = "hello"
 
     bad_field_test_dict = list(mock_graph_literal)
     bad_field_test_dict[0]["children"][0]["children"][0]["metrics"][
         "list"
     ] = DummyType()
     gf = GraphFrame.from_literal(bad_field_test_dict)
     path = [{"name": "foo"}, {"name": "bar"}, {"list": DummyType()}]
-    query = QueryMatcher(path)
+    query = ObjectQuery(path)
     with pytest.raises(InvalidQueryFilter):
-        query.apply(gf)
+        engine.apply(query, gf.graph, gf.dataframe)
 
     path = ["*", {"name": "bar"}, {"name": "grault"}, "*"]
     match = [
         [root, root.children[0], root.children[0].children[1]],
         [root.children[0], root.children[0].children[1]],
         [
             root,
@@ -426,20 +429,20 @@
             gf.graph.roots[1],
             gf.graph.roots[1].children[0],
             gf.graph.roots[1].children[0].children[1],
         ],
         [gf.graph.roots[1].children[0], gf.graph.roots[1].children[0].children[1]],
     ]
     match = list(set().union(*match))
-    query = QueryMatcher(path)
-    assert sorted(query.apply(gf)) == sorted(match)
+    query = ObjectQuery(path)
+    assert sorted(engine.apply(query, gf.graph, gf.dataframe)) == sorted(match)
 
     path = ["*", {"name": "bar"}, {"name": "grault"}, "+"]
-    query = QueryMatcher(path)
-    assert query.apply(gf) == []
+    query = ObjectQuery(path)
+    assert engine.apply(query, gf.graph, gf.dataframe) == []
 
     # Test a former edge case with the + quantifier/wildcard
     match = [
         [gf.graph.roots[0].children[0], gf.graph.roots[0].children[0].children[0]],
         [
             gf.graph.roots[0].children[1].children[0].children[0].children[0],
             gf.graph.roots[0]
@@ -460,16 +463,16 @@
             .children[1]
             .children[0]
             .children[0],
         ],
     ]
     match = list(set().union(*match))
     path = [("+", {"name": "ba.*"})]
-    query = QueryMatcher(path)
-    assert sorted(query.apply(gf)) == sorted(match)
+    query = ObjectQuery(path)
+    assert sorted(engine.apply(query, gf.graph, gf.dataframe)) == sorted(match)
 
 
 def test_apply_indices(calc_pi_hpct_db):
     gf = GraphFrame.from_hpctoolkit(str(calc_pi_hpct_db))
     main = gf.graph.roots[0].children[0]
     path = [
         {"name": "[0-9]*:?MPI_.*"},
@@ -486,29 +489,31 @@
         [
             main.children[1],
             main.children[1].children[0],
             main.children[1].children[0].children[0],
         ],
     ]
     matches = list(set().union(*matches))
-    query = QueryMatcher(path)
-    assert sorted(query.apply(gf)) == sorted(matches)
+    query = ObjectQuery(path, multi_index_mode="all")
+    engine = QueryEngine()
+    assert sorted(engine.apply(query, gf.graph, gf.dataframe)) == sorted(matches)
 
     gf.drop_index_levels()
-    assert query.apply(gf) == matches
+    assert engine.apply(query, gf.graph, gf.dataframe) == matches
 
 
-def test_high_level_depth(mock_graph_literal):
+def test_object_dialect_depth(mock_graph_literal):
     gf = GraphFrame.from_literal(mock_graph_literal)
-    query = QueryMatcher([("*", {"depth": 1})])
+    query = ObjectQuery([("*", {"depth": 1})])
+    engine = QueryEngine()
     roots = gf.graph.roots
     matches = [c for r in roots for c in r.children]
-    assert sorted(query.apply(gf)) == sorted(matches)
+    assert sorted(engine.apply(query, gf.graph, gf.dataframe)) == sorted(matches)
 
-    query = QueryMatcher([("*", {"depth": "<= 2"})])
+    query = ObjectQuery([("*", {"depth": "<= 2"})])
     matches = [
         [roots[0], roots[0].children[0], roots[0].children[0].children[0]],
         [roots[0].children[0], roots[0].children[0].children[0]],
         [roots[0].children[0].children[0]],
         [roots[0], roots[0].children[0], roots[0].children[0].children[1]],
         [roots[0].children[0], roots[0].children[0].children[1]],
         [roots[0].children[0].children[1]],
@@ -525,96 +530,100 @@
         [roots[1].children[0], roots[1].children[0].children[0]],
         [roots[1].children[0].children[0]],
         [roots[1], roots[1].children[0], roots[1].children[0].children[1]],
         [roots[1].children[0], roots[1].children[0].children[1]],
         [roots[1].children[0].children[1]],
     ]
     matches = list(set().union(*matches))
-    assert sorted(query.apply(gf)) == sorted(matches)
+    assert sorted(engine.apply(query, gf.graph, gf.dataframe)) == sorted(matches)
 
     with pytest.raises(InvalidQueryFilter):
-        query = QueryMatcher([{"depth": "hello"}])
-        query.apply(gf)
+        query = ObjectQuery([{"depth": "hello"}])
+        engine.apply(query, gf.graph, gf.dataframe)
 
 
-def test_high_level_hatchet_nid(mock_graph_literal):
+def test_object_dialect_hatchet_nid(mock_graph_literal):
     gf = GraphFrame.from_literal(mock_graph_literal)
-    query = QueryMatcher([("*", {"node_id": ">= 20"})])
+    query = ObjectQuery([("*", {"node_id": ">= 20"})])
+    engine = QueryEngine()
     root = gf.graph.roots[1]
     matches = [
         [root, root.children[0], root.children[0].children[0]],
         [root.children[0], root.children[0].children[0]],
         [root.children[0].children[0]],
         [root, root.children[0], root.children[0].children[1]],
         [root.children[0], root.children[0].children[1]],
         [root.children[0].children[1]],
     ]
     matches = list(set().union(*matches))
-    assert sorted(query.apply(gf)) == sorted(matches)
+    assert sorted(engine.apply(query, gf.graph, gf.dataframe)) == sorted(matches)
 
-    query = QueryMatcher([{"node_id": 0}])
-    assert query.apply(gf) == [gf.graph.roots[0]]
+    query = ObjectQuery([{"node_id": 0}])
+    assert engine.apply(query, gf.graph, gf.dataframe) == [gf.graph.roots[0]]
 
     with pytest.raises(InvalidQueryFilter):
-        query = QueryMatcher([{"node_id": "hello"}])
-        query.apply(gf)
+        query = ObjectQuery([{"node_id": "hello"}])
+        engine.apply(query, gf.graph, gf.dataframe)
 
 
-def test_high_level_depth_index_levels(calc_pi_hpct_db):
+def test_object_dialect_depth_index_levels(calc_pi_hpct_db):
     gf = GraphFrame.from_hpctoolkit(str(calc_pi_hpct_db))
     root = gf.graph.roots[0]
 
-    query = QueryMatcher([("*", {"depth": "<= 2"})])
+    query = ObjectQuery([("*", {"depth": "<= 2"})], multi_index_mode="all")
+    engine = QueryEngine()
     matches = [
         [root, root.children[0], root.children[0].children[0]],
         [root.children[0], root.children[0].children[0]],
         [root.children[0].children[0]],
         [root, root.children[0], root.children[0].children[1]],
         [root.children[0], root.children[0].children[1]],
         [root.children[0].children[1]],
     ]
     matches = list(set().union(*matches))
-    assert sorted(query.apply(gf)) == sorted(matches)
+    assert sorted(engine.apply(query, gf.graph, gf.dataframe)) == sorted(matches)
 
-    query = QueryMatcher([("*", {"depth": 0})])
+    query = ObjectQuery([("*", {"depth": 0})], multi_index_mode="all")
     matches = [root]
-    assert query.apply(gf) == matches
+    assert engine.apply(query, gf.graph, gf.dataframe) == matches
 
     with pytest.raises(InvalidQueryFilter):
-        query = QueryMatcher([{"depth": "hello"}])
-        query.apply(gf)
+        query = ObjectQuery([{"depth": "hello"}], multi_index_mode="all")
+        engine.apply(query, gf.graph, gf.dataframe)
 
 
-def test_high_level_node_id_index_levels(calc_pi_hpct_db):
+def test_object_dialect_node_id_index_levels(calc_pi_hpct_db):
     gf = GraphFrame.from_hpctoolkit(str(calc_pi_hpct_db))
     root = gf.graph.roots[0]
 
-    query = QueryMatcher([("*", {"node_id": "<= 2"})])
+    query = ObjectQuery([("*", {"node_id": "<= 2"})], multi_index_mode="all")
+    engine = QueryEngine()
     matches = [
         [root, root.children[0]],
         [root.children[0]],
         [root, root.children[0], root.children[0].children[0]],
         [root.children[0], root.children[0].children[0]],
         [root.children[0].children[0]],
     ]
     matches = list(set().union(*matches))
-    assert sorted(query.apply(gf)) == sorted(matches)
+    assert sorted(engine.apply(query, gf.graph, gf.dataframe)) == sorted(matches)
 
-    query = QueryMatcher([("*", {"node_id": 0})])
+    query = ObjectQuery([("*", {"node_id": 0})], multi_index_mode="all")
     matches = [root]
-    assert query.apply(gf) == matches
+    assert engine.apply(query, gf.graph, gf.dataframe) == matches
 
     with pytest.raises(InvalidQueryFilter):
-        query = QueryMatcher([{"node_id": "hello"}])
-        query.apply(gf)
+        query = ObjectQuery([{"node_id": "hello"}], multi_index_mode="all")
+        engine.apply(query, gf.graph, gf.dataframe)
 
 
-def test_high_level_multi_condition_one_attribute(mock_graph_literal):
+def test_object_dialect_multi_condition_one_attribute(mock_graph_literal):
     gf = GraphFrame.from_literal(mock_graph_literal)
-    query = QueryMatcher([("*", {"time (inc)": [">= 20", "<= 60"]})])
+    query = ObjectQuery([("*", {"time (inc)": [">= 20", "<= 60"]})])
+    engine = QueryEngine()
     roots = gf.graph.roots
     matches = [
         [roots[0].children[0]],
         [
             roots[0].children[1],
             roots[0].children[1].children[0],
             roots[0].children[1].children[0].children[0],
@@ -659,195 +668,159 @@
             roots[0].children[2].children[0].children[1].children[0],
         ],
         [roots[0].children[2].children[0].children[1].children[0]],
         [roots[1], roots[1].children[0]],
         [roots[1].children[0]],
     ]
     matches = list(set().union(*matches))
-    assert sorted(query.apply(gf)) == sorted(matches)
+    assert sorted(engine.apply(query, gf.graph, gf.dataframe)) == sorted(matches)
+
+
+def test_obj_query_is_query():
+    assert issubclass(ObjectQuery, Query)
 
 
-def test_query_matcher_is_abstract_query():
-    assert issubclass(QueryMatcher, AbstractQuery)
+def test_str_query_is_query():
+    assert issubclass(StringQuery, Query)
 
 
-def test_nary_query_is_abstract_query():
-    assert issubclass(NaryQuery, AbstractQuery)
+def test_conj_query_is_compound_query():
+    assert issubclass(ConjunctionQuery, CompoundQuery)
 
 
-def test_and_query_is_nary_query():
-    assert issubclass(AndQuery, NaryQuery)
+def test_disj_query_is_compound_query():
+    assert issubclass(DisjunctionQuery, CompoundQuery)
 
 
-def test_or_query_is_nary_query():
-    assert issubclass(OrQuery, NaryQuery)
+def test_exc_disj_query_is_compound_query():
+    assert issubclass(ExclusiveDisjunctionQuery, CompoundQuery)
 
 
-def test_xor_query_is_nary_query():
-    assert issubclass(XorQuery, NaryQuery)
+def test_negation_query_is_compound_query():
+    assert issubclass(NegationQuery, CompoundQuery)
 
 
-def test_nary_query_high_level_construction(mock_graph_literal):
+def test_compound_query_object_dialect_construction(mock_graph_literal):
     gf = GraphFrame.from_literal(mock_graph_literal)
     query1 = [("*", {"time (inc)": [">= 20", "<= 60"]})]
     query2 = [("*", {"time (inc)": ">= 60"})]
     q1_node = gf.graph.roots[0].children[1].children[0].children[0]
     q2_node = gf.graph.roots[0]
-    compound_query = AndQuery(query1, query2)
+    compound_query = ConjunctionQuery(query1, query2)
     assert compound_query.subqueries[0].query_pattern[0][0] == "*"
     assert compound_query.subqueries[0].query_pattern[0][1](gf.dataframe.loc[q1_node])
     assert not compound_query.subqueries[0].query_pattern[0][1](
         gf.dataframe.loc[q2_node]
     )
     assert compound_query.subqueries[1].query_pattern[0][0] == "*"
     assert compound_query.subqueries[1].query_pattern[0][1](gf.dataframe.loc[q2_node])
     assert not compound_query.subqueries[1].query_pattern[0][1](
         gf.dataframe.loc[q1_node]
     )
 
 
-def test_nary_query_low_level_construction(mock_graph_literal):
+def test_compound_query_base_query_construction(mock_graph_literal):
     gf = GraphFrame.from_literal(mock_graph_literal)
-    query1 = QueryMatcher().match(
+    query1 = Query().match(
         "*", lambda x: x["time (inc)"] >= 20 and x["time (inc)"] <= 60
     )
-    query2 = QueryMatcher().match("*", lambda x: x["time (inc)"] >= 60)
+    query2 = Query().match("*", lambda x: x["time (inc)"] >= 60)
     q1_node = gf.graph.roots[0].children[1].children[0].children[0]
     q2_node = gf.graph.roots[0]
-    compound_query = AndQuery(query1, query2)
+    compound_query = ConjunctionQuery(query1, query2)
     assert compound_query.subqueries[0].query_pattern[0][0] == "*"
     assert compound_query.subqueries[0].query_pattern[0][1](gf.dataframe.loc[q1_node])
     assert not compound_query.subqueries[0].query_pattern[0][1](
         gf.dataframe.loc[q2_node]
     )
     assert compound_query.subqueries[1].query_pattern[0][0] == "*"
     assert compound_query.subqueries[1].query_pattern[0][1](gf.dataframe.loc[q2_node])
     assert not compound_query.subqueries[1].query_pattern[0][1](
         gf.dataframe.loc[q1_node]
     )
 
 
-def test_nary_query_mixed_level_construction(mock_graph_literal):
+def test_compound_query_mixed_syntax_construction(mock_graph_literal):
     gf = GraphFrame.from_literal(mock_graph_literal)
     query1 = [("*", {"time (inc)": [">= 20", "<= 60"]})]
-    query2 = QueryMatcher().match("*", lambda x: x["time (inc)"] >= 60)
+    query2 = Query().match("*", lambda x: x["time (inc)"] >= 60)
     q1_node = gf.graph.roots[0].children[1].children[0].children[0]
     q2_node = gf.graph.roots[0]
-    compound_query = AndQuery(query1, query2)
+    compound_query = ConjunctionQuery(query1, query2)
     assert compound_query.subqueries[0].query_pattern[0][0] == "*"
     assert compound_query.subqueries[0].query_pattern[0][1](gf.dataframe.loc[q1_node])
     assert not compound_query.subqueries[0].query_pattern[0][1](
         gf.dataframe.loc[q2_node]
     )
     assert compound_query.subqueries[1].query_pattern[0][0] == "*"
     assert compound_query.subqueries[1].query_pattern[0][1](gf.dataframe.loc[q2_node])
     assert not compound_query.subqueries[1].query_pattern[0][1](
         gf.dataframe.loc[q1_node]
     )
 
 
-def test_and_query(mock_graph_literal):
-    gf = GraphFrame.from_literal(mock_graph_literal)
-    query1 = [("*", {"time (inc)": [">= 20", "<= 60"]})]
-    query2 = [("*", {"time (inc)": ">= 60"})]
-    compound_query = AndQuery(query1, query2)
-    roots = gf.graph.roots
-    matches = [
-        roots[0].children[1],
-        roots[0].children[1].children[0],
-    ]
-    assert sorted(compound_query.apply(gf)) == sorted(matches)
-
-
-def test_intersection_query(mock_graph_literal):
+def test_conjunction_query(mock_graph_literal):
     gf = GraphFrame.from_literal(mock_graph_literal)
     query1 = [("*", {"time (inc)": [">= 20", "<= 60"]})]
     query2 = [("*", {"time (inc)": ">= 60"})]
-    compound_query = IntersectionQuery(query1, query2)
+    compound_query = ConjunctionQuery(query1, query2)
+    engine = QueryEngine()
     roots = gf.graph.roots
     matches = [
         roots[0].children[1],
         roots[0].children[1].children[0],
     ]
-    assert sorted(compound_query.apply(gf)) == sorted(matches)
-
-
-def test_or_query(mock_graph_literal):
-    gf = GraphFrame.from_literal(mock_graph_literal)
-    query1 = [("*", {"time (inc)": 5.0})]
-    query2 = [("*", {"time (inc)": 10.0})]
-    compound_query = OrQuery(query1, query2)
-    roots = gf.graph.roots
-    matches = [
-        roots[0].children[0].children[0],
-        roots[0].children[0].children[1],
-        roots[0].children[1].children[0].children[0].children[0].children[0],
-        roots[0].children[1].children[0].children[0].children[0].children[1],
-        roots[0].children[1].children[0].children[0].children[1],
-        roots[0].children[2].children[0].children[0],
-        roots[0].children[2].children[0].children[1].children[0].children[0],
-        roots[1].children[0].children[0],
-        roots[1].children[0].children[1],
-    ]
-    assert sorted(compound_query.apply(gf)) == sorted(matches)
+    assert sorted(engine.apply(compound_query, gf.graph, gf.dataframe)) == sorted(
+        matches
+    )
 
 
-def test_union_query(mock_graph_literal):
+def test_disjunction_query(mock_graph_literal):
     gf = GraphFrame.from_literal(mock_graph_literal)
     query1 = [("*", {"time (inc)": 5.0})]
     query2 = [("*", {"time (inc)": 10.0})]
-    compound_query = UnionQuery(query1, query2)
+    compound_query = DisjunctionQuery(query1, query2)
+    engine = QueryEngine()
     roots = gf.graph.roots
     matches = [
         roots[0].children[0].children[0],
         roots[0].children[0].children[1],
         roots[0].children[1].children[0].children[0].children[0].children[0],
         roots[0].children[1].children[0].children[0].children[0].children[1],
         roots[0].children[1].children[0].children[0].children[1],
         roots[0].children[2].children[0].children[0],
         roots[0].children[2].children[0].children[1].children[0].children[0],
         roots[1].children[0].children[0],
         roots[1].children[0].children[1],
     ]
-    assert sorted(compound_query.apply(gf)) == sorted(matches)
-
-
-def test_xor_query(mock_graph_literal):
-    gf = GraphFrame.from_literal(mock_graph_literal)
-    query1 = [("*", {"time (inc)": [">= 5.0", "<= 10.0"]})]
-    query2 = [("*", {"time (inc)": 10.0})]
-    compound_query = XorQuery(query1, query2)
-    roots = gf.graph.roots
-    matches = [
-        roots[0].children[0].children[0],
-        roots[0].children[1].children[0].children[0].children[0].children[0],
-        roots[0].children[2].children[0].children[0],
-        roots[0].children[2].children[0].children[1].children[0].children[0],
-        roots[1].children[0].children[0],
-    ]
-    assert sorted(compound_query.apply(gf)) == sorted(matches)
+    assert sorted(engine.apply(compound_query, gf.graph, gf.dataframe)) == sorted(
+        matches
+    )
 
 
-def test_sym_diff_query(mock_graph_literal):
+def test_exc_disjunction_query(mock_graph_literal):
     gf = GraphFrame.from_literal(mock_graph_literal)
     query1 = [("*", {"time (inc)": [">= 5.0", "<= 10.0"]})]
     query2 = [("*", {"time (inc)": 10.0})]
-    compound_query = SymDifferenceQuery(query1, query2)
+    compound_query = ExclusiveDisjunctionQuery(query1, query2)
+    engine = QueryEngine()
     roots = gf.graph.roots
     matches = [
         roots[0].children[0].children[0],
         roots[0].children[1].children[0].children[0].children[0].children[0],
         roots[0].children[2].children[0].children[0],
         roots[0].children[2].children[0].children[1].children[0].children[0],
         roots[1].children[0].children[0],
     ]
-    assert sorted(compound_query.apply(gf)) == sorted(matches)
+    assert sorted(engine.apply(compound_query, gf.graph, gf.dataframe)) == sorted(
+        matches
+    )
 
 
-def test_construct_cypher_api():
+def test_construct_string_dialect():
     mock_node_mpi = {"name": "MPI_Bcast"}
     mock_node_ibv = {"name": "ibv_reg_mr"}
     mock_node_time_true = {"time (inc)": 0.1}
     mock_node_time_false = {"time (inc)": 0.001}
     path1 = u"""MATCH (p)->("*")->(q)
     WHERE p."name" STARTS WITH "MPI_" AND q."name" STARTS WITH "ibv"
     """
@@ -856,18 +829,18 @@
     """
     path3 = u"""MATCH (p)->("+", a)->(q)
     WHERE p."name" STARTS WITH "MPI" AND a."time (inc)" >= 0.1 AND q."name" STARTS WITH "ibv"
     """
     path4 = u"""MATCH (p)->(3, a)->(q)
     WHERE p."name" STARTS WITH "MPI" AND a."time (inc)" = 0.1 AND q."name" STARTS WITH "ibv"
     """
-    query1 = CypherQuery(path1)
-    query2 = CypherQuery(path2)
-    query3 = CypherQuery(path3)
-    query4 = CypherQuery(path4)
+    query1 = StringQuery(path1)
+    query2 = StringQuery(path2)
+    query3 = StringQuery(path3)
+    query4 = StringQuery(path4)
 
     assert query1.query_pattern[0][0] == "."
     assert query1.query_pattern[0][1](mock_node_mpi)
     assert not query1.query_pattern[0][1](mock_node_ibv)
     assert not query1.query_pattern[0][1](mock_node_time_true)
     assert query1.query_pattern[1][0] == "*"
     assert query1.query_pattern[1][1](mock_node_mpi)
@@ -921,101 +894,102 @@
     assert query4.query_pattern[4][0] == "."
 
     invalid_path = u"""MATCH (p)->({"bad": "wildcard"}, a)->(q)
     WHERE p."name" STARTS WITH "MPI" AND a."time (inc)" = 0.1 AND
     q."name" STARTS WITH "ibv"
     """
     with pytest.raises(InvalidQueryPath):
-        _ = CypherQuery(invalid_path)
+        _ = StringQuery(invalid_path)
 
 
-def test_apply_cypher(mock_graph_literal):
+def test_apply_string_dialect(mock_graph_literal):
     gf = GraphFrame.from_literal(mock_graph_literal)
     path = u"""MATCH (p)->(2, q)->("*", r)->(s)
     WHERE p."time (inc)" >= 30.0 AND NOT q."name" STARTS WITH "b"
     AND r."name" =~ "[^b][a-z]+" AND s."name" STARTS WITH "gr"
     """
     root = gf.graph.roots[0]
     match = [
         root,
         root.children[1],
         root.children[1].children[0],
         root.children[1].children[0].children[0],
         root.children[1].children[0].children[0].children[1],
     ]
-    query = CypherQuery(path)
+    query = StringQuery(path)
+    engine = QueryEngine()
 
-    assert sorted(query.apply(gf)) == sorted(match)
+    assert sorted(engine.apply(query, gf.graph, gf.dataframe)) == sorted(match)
 
     path = u"""MATCH (p)->(".")->(q)->("*")
     WHERE p."time (inc)" >= 30.0 AND q."name" = "bar"
     """
     match = [
         root.children[1].children[0],
         root.children[1].children[0].children[0],
         root.children[1].children[0].children[0].children[0],
         root.children[1].children[0].children[0].children[0].children[0],
         root.children[1].children[0].children[0].children[0].children[1],
     ]
-    query = CypherQuery(path)
-    assert sorted(query.apply(gf)) == sorted(match)
+    query = StringQuery(path)
+    assert sorted(engine.apply(query, gf.graph, gf.dataframe)) == sorted(match)
 
     path = u"""MATCH (p)->(q)->(r)
     WHERE p."name" = "foo" AND q."name" = "bar" AND r."time" = 5.0
     """
     match = [root, root.children[0], root.children[0].children[0]]
-    query = CypherQuery(path)
-    assert sorted(query.apply(gf)) == sorted(match)
+    query = StringQuery(path)
+    assert sorted(engine.apply(query, gf.graph, gf.dataframe)) == sorted(match)
 
     path = u"""MATCH (p)->(q)->("+", r)
     WHERE p."name" = "foo" AND q."name" = "qux" AND r."time (inc)" > 15.0
     """
     match = [
         root,
         root.children[1],
         root.children[1].children[0],
         root.children[1].children[0].children[0],
         root.children[1].children[0].children[0].children[0],
     ]
-    query = CypherQuery(path)
-    assert sorted(query.apply(gf)) == sorted(match)
+    query = StringQuery(path)
+    assert sorted(engine.apply(query, gf.graph, gf.dataframe)) == sorted(match)
 
     path = u"""MATCH (p)->(q)
     WHERE p."time (inc)" > 100 OR p."time (inc)" <= 30 AND q."time (inc)" = 20
     """
     roots = gf.graph.roots
     match = [
         roots[0],
         roots[0].children[0],
         roots[1],
         roots[1].children[0],
     ]
-    query = CypherQuery(path)
-    assert sorted(query.apply(gf)) == sorted(match)
+    query = StringQuery(path)
+    assert sorted(engine.apply(query, gf.graph, gf.dataframe)) == sorted(match)
 
     path = u"""MATCH (p)->("*", q)->(r)
     WHERE p."name" = "this" AND q."name" = "is" AND r."name" = "nonsense"
     """
 
-    query = CypherQuery(path)
-    assert query.apply(gf) == []
+    query = StringQuery(path)
+    assert engine.apply(query, gf.graph, gf.dataframe) == []
 
     path = u"""MATCH (p)->("*")->(q)
     WHERE p."name" = 5 AND q."name" = "whatever"
     """
     with pytest.raises(InvalidQueryFilter):
-        query = CypherQuery(path)
-        query.apply(gf)
+        query = StringQuery(path)
+        engine.apply(query, gf.graph, gf.dataframe)
 
     path = u"""MATCH (p)->("*")->(q)
     WHERE p."time" = "badstring" AND q."name" = "whatever"
     """
-    query = CypherQuery(path)
+    query = StringQuery(path)
     with pytest.raises(InvalidQueryFilter):
-        query.apply(gf)
+        engine.apply(query, gf.graph, gf.dataframe)
 
     class DummyType:
         def __init__(self):
             self.x = 5.0
             self.y = -1
             self.z = "hello"
 
@@ -1024,16 +998,16 @@
         "list"
     ] = DummyType()
     gf = GraphFrame.from_literal(bad_field_test_dict)
     path = u"""MATCH (p)->(q)->(r)
     WHERE p."name" = "foo" AND q."name" = "bar" AND p."list" = DummyType()
     """
     with pytest.raises(InvalidQueryPath):
-        query = CypherQuery(path)
-        query.apply(gf)
+        query = StringQuery(path)
+        engine.apply(query, gf.graph, gf.dataframe)
 
     path = u"""MATCH ("*")->(p)->(q)->("*")
     WHERE p."name" = "bar" AND q."name" = "grault"
     """
     match = [
         [root, root.children[0], root.children[0].children[1]],
         [root.children[0], root.children[0].children[1]],
@@ -1071,179 +1045,284 @@
             gf.graph.roots[1],
             gf.graph.roots[1].children[0],
             gf.graph.roots[1].children[0].children[1],
         ],
         [gf.graph.roots[1].children[0], gf.graph.roots[1].children[0].children[1]],
     ]
     match = list(set().union(*match))
-    query = CypherQuery(path)
-    assert sorted(query.apply(gf)) == sorted(match)
+    query = StringQuery(path)
+    assert sorted(engine.apply(query, gf.graph, gf.dataframe)) == sorted(match)
 
     path = u"""MATCH ("*")->(p)->(q)->("+")
     WHERE p."name" = "bar" AND q."name" = "grault"
     """
-    query = CypherQuery(path)
-    assert query.apply(gf) == []
+    query = StringQuery(path)
+    assert engine.apply(query, gf.graph, gf.dataframe) == []
 
     gf.dataframe["time"] = np.NaN
     gf.dataframe.at[gf.graph.roots[0], "time"] = 5.0
     path = u"""MATCH ("*", p)
     WHERE p."time" IS NOT NAN"""
     match = [gf.graph.roots[0]]
-    query = CypherQuery(path)
-    assert query.apply(gf) == match
+    query = StringQuery(path)
+    assert engine.apply(query, gf.graph, gf.dataframe) == match
 
     gf.dataframe["time"] = 5.0
     gf.dataframe.at[gf.graph.roots[0], "time"] = np.NaN
     path = u"""MATCH ("*", p)
     WHERE p."time" IS NAN"""
     match = [gf.graph.roots[0]]
-    query = CypherQuery(path)
-    assert query.apply(gf) == match
+    query = StringQuery(path)
+    assert engine.apply(query, gf.graph, gf.dataframe) == match
 
     gf.dataframe["time"] = np.Inf
     gf.dataframe.at[gf.graph.roots[0], "time"] = 5.0
     path = u"""MATCH ("*", p)
     WHERE p."time" IS NOT INF"""
     match = [gf.graph.roots[0]]
-    query = CypherQuery(path)
-    assert query.apply(gf) == match
+    query = StringQuery(path)
+    assert engine.apply(query, gf.graph, gf.dataframe) == match
 
     gf.dataframe["time"] = 5.0
     gf.dataframe.at[gf.graph.roots[0], "time"] = np.Inf
     path = u"""MATCH ("*", p)
     WHERE p."time" IS INF"""
     match = [gf.graph.roots[0]]
-    query = CypherQuery(path)
-    assert query.apply(gf) == match
+    query = StringQuery(path)
+    assert engine.apply(query, gf.graph, gf.dataframe) == match
 
     names = gf.dataframe["name"].copy()
     gf.dataframe["name"] = None
     gf.dataframe.at[gf.graph.roots[0], "name"] = names.iloc[0]
     path = u"""MATCH ("*", p)
     WHERE p."name" IS NOT NONE"""
     match = [gf.graph.roots[0]]
-    query = CypherQuery(path)
-    assert query.apply(gf) == match
+    query = StringQuery(path)
+    assert engine.apply(query, gf.graph, gf.dataframe) == match
 
     gf.dataframe["name"] = names
     gf.dataframe.at[gf.graph.roots[0], "name"] = None
     path = u"""MATCH ("*", p)
     WHERE p."name" IS NONE"""
     match = [gf.graph.roots[0]]
-    query = CypherQuery(path)
-    assert query.apply(gf) == match
+    query = StringQuery(path)
+    assert engine.apply(query, gf.graph, gf.dataframe) == match
 
 
-def test_cypher_and_compound_query(mock_graph_literal):
+def test_string_conj_compound_query(mock_graph_literal):
     gf = GraphFrame.from_literal(mock_graph_literal)
-    compound_query1 = parse_cypher_query(
+    compound_query1 = parse_string_dialect(
         u"""
         {MATCH ("*", p) WHERE p."time (inc)" >= 20 AND p."time (inc)" <= 60}
         AND {MATCH ("*", p) WHERE p."time (inc)" >= 60}
         """
     )
-    compound_query2 = parse_cypher_query(
+    compound_query2 = parse_string_dialect(
         u"""
         MATCH ("*", p)
         WHERE {p."time (inc)" >= 20 AND p."time (inc)" <= 60} AND {p."time (inc)" >= 60}
         """
     )
+    engine = QueryEngine()
     roots = gf.graph.roots
     matches = [
         roots[0].children[1],
         roots[0].children[1].children[0],
     ]
-    assert sorted(compound_query1.apply(gf)) == sorted(matches)
-    assert sorted(compound_query2.apply(gf)) == sorted(matches)
+    assert sorted(engine.apply(compound_query1, gf.graph, gf.dataframe)) == sorted(
+        matches
+    )
+    assert sorted(engine.apply(compound_query2, gf.graph, gf.dataframe)) == sorted(
+        matches
+    )
 
 
-def test_cypher_or_compound_query(mock_graph_literal):
+def test_string_disj_compound_query(mock_graph_literal):
     gf = GraphFrame.from_literal(mock_graph_literal)
-    compound_query1 = parse_cypher_query(
+    compound_query1 = parse_string_dialect(
         u"""
         {MATCH ("*", p) WHERE p."time (inc)" = 5.0}
         OR {MATCH ("*", p) WHERE p."time (inc)" = 10.0}
         """
     )
-    compound_query2 = parse_cypher_query(
+    compound_query2 = parse_string_dialect(
         u"""
         MATCH ("*", p)
         WHERE {p."time (inc)" = 5.0} OR {p."time (inc)" = 10.0}
         """
     )
+    engine = QueryEngine()
     roots = gf.graph.roots
     matches = [
         roots[0].children[0].children[0],
         roots[0].children[0].children[1],
         roots[0].children[1].children[0].children[0].children[0].children[0],
         roots[0].children[1].children[0].children[0].children[0].children[1],
         roots[0].children[1].children[0].children[0].children[1],
         roots[0].children[2].children[0].children[0],
         roots[0].children[2].children[0].children[1].children[0].children[0],
         roots[1].children[0].children[0],
         roots[1].children[0].children[1],
     ]
-    assert sorted(compound_query1.apply(gf)) == sorted(matches)
-    assert sorted(compound_query2.apply(gf)) == sorted(matches)
+    assert sorted(engine.apply(compound_query1, gf.graph, gf.dataframe)) == sorted(
+        matches
+    )
+    assert sorted(engine.apply(compound_query2, gf.graph, gf.dataframe)) == sorted(
+        matches
+    )
 
 
-def test_cypher_xor_compound_query(mock_graph_literal):
+def test_cypher_exc_disj_compound_query(mock_graph_literal):
     gf = GraphFrame.from_literal(mock_graph_literal)
-    compound_query1 = parse_cypher_query(
+    compound_query1 = parse_string_dialect(
         u"""
         {MATCH ("*", p) WHERE p."time (inc)" >= 5.0 AND p."time (inc)" <= 10.0}
         XOR {MATCH ("*", p) WHERE p."time (inc)" = 10.0}
         """
     )
-    compound_query2 = parse_cypher_query(
+    compound_query2 = parse_string_dialect(
         u"""
         MATCH ("*", p)
         WHERE {p."time (inc)" >= 5.0 AND p."time (inc)" <= 10.0} XOR {p."time (inc)" = 10.0}
         """
     )
+    engine = QueryEngine()
     roots = gf.graph.roots
     matches = [
         roots[0].children[0].children[0],
         roots[0].children[1].children[0].children[0].children[0].children[0],
         roots[0].children[2].children[0].children[0],
         roots[0].children[2].children[0].children[1].children[0].children[0],
         roots[1].children[0].children[0],
     ]
-    assert sorted(compound_query1.apply(gf)) == sorted(matches)
-    assert sorted(compound_query2.apply(gf)) == sorted(matches)
+    assert sorted(engine.apply(compound_query1, gf.graph, gf.dataframe)) == sorted(
+        matches
+    )
+    assert sorted(engine.apply(compound_query2, gf.graph, gf.dataframe)) == sorted(
+        matches
+    )
 
 
 def test_leaf_query(small_mock2):
     gf = GraphFrame.from_literal(small_mock2)
     roots = gf.graph.roots
     matches = [
         roots[0].children[0].children[0],
         roots[0].children[0].children[1],
         roots[0].children[1].children[0],
         roots[0].children[1].children[1],
     ]
     nodes = set(gf.graph.traverse())
     nonleaves = list(nodes - set(matches))
-    obj_query = QueryMatcher([{"depth": -1}])
-    str_query_numeric = parse_cypher_query(
+    obj_query = ObjectQuery([{"depth": -1}])
+    str_query_numeric = parse_string_dialect(
         u"""
         MATCH (p)
         WHERE p."depth" = -1
         """
     )
-    str_query_is_leaf = parse_cypher_query(
+    str_query_is_leaf = parse_string_dialect(
         u"""
         MATCH (p)
         WHERE p IS LEAF
         """
     )
-    str_query_is_not_leaf = parse_cypher_query(
+    str_query_is_not_leaf = parse_string_dialect(
         u"""
         MATCH (p)
         WHERE p IS NOT LEAF
         """
     )
-    assert sorted(obj_query.apply(gf)) == sorted(matches)
-    assert sorted(str_query_numeric.apply(gf)) == sorted(matches)
-    assert sorted(str_query_is_leaf.apply(gf)) == sorted(matches)
-    assert sorted(str_query_is_not_leaf.apply(gf)) == sorted(nonleaves)
+    engine = QueryEngine()
+    assert sorted(engine.apply(obj_query, gf.graph, gf.dataframe)) == sorted(matches)
+    assert sorted(engine.apply(str_query_numeric, gf.graph, gf.dataframe)) == sorted(
+        matches
+    )
+    assert sorted(engine.apply(str_query_is_leaf, gf.graph, gf.dataframe)) == sorted(
+        matches
+    )
+    assert sorted(
+        engine.apply(str_query_is_not_leaf, gf.graph, gf.dataframe)
+    ) == sorted(nonleaves)
+
+
+def test_object_dialect_all_mode(tau_profile_dir):
+    gf = GraphFrame.from_tau(tau_profile_dir)
+    engine = QueryEngine()
+    query = ObjectQuery(
+        [".", ("+", {"time (inc)": ">= 17983.0"})], multi_index_mode="all"
+    )
+    roots = gf.graph.roots
+    matches = [
+        roots[0],
+        roots[0].children[6],
+        roots[0].children[6].children[1],
+        roots[0].children[0],
+    ]
+    assert sorted(engine.apply(query, gf.graph, gf.dataframe)) == sorted(matches)
+
+
+def test_string_dialect_all_mode(tau_profile_dir):
+    gf = GraphFrame.from_tau(tau_profile_dir)
+    engine = QueryEngine()
+    query = StringQuery(
+        u"""MATCH (".")->("+", p)
+        WHERE p."time (inc)" >= 17983.0
+        """,
+        multi_index_mode="all",
+    )
+    roots = gf.graph.roots
+    matches = [
+        roots[0],
+        roots[0].children[6],
+        roots[0].children[6].children[1],
+        roots[0].children[0],
+    ]
+    assert sorted(engine.apply(query, gf.graph, gf.dataframe)) == sorted(matches)
+
+
+def test_object_dialect_any_mode(tau_profile_dir):
+    gf = GraphFrame.from_tau(tau_profile_dir)
+    engine = QueryEngine()
+    query = ObjectQuery([{"time": "< 24.0"}], multi_index_mode="any")
+    roots = gf.graph.roots
+    matches = [
+        roots[0].children[2],
+        roots[0].children[6].children[3],
+    ]
+    assert sorted(engine.apply(query, gf.graph, gf.dataframe)) == sorted(matches)
+
+
+def test_string_dialect_any_mode(tau_profile_dir):
+    gf = GraphFrame.from_tau(tau_profile_dir)
+    engine = QueryEngine()
+    query = StringQuery(
+        u"""MATCH (".", p)
+        WHERE p."time" < 24.0
+        """,
+        multi_index_mode="any",
+    )
+    roots = gf.graph.roots
+    matches = [
+        roots[0].children[2],
+        roots[0].children[6].children[3],
+    ]
+    assert sorted(engine.apply(query, gf.graph, gf.dataframe)) == sorted(matches)
+
+
+def test_multi_index_mode_assertion_error(tau_profile_dir):
+    with pytest.raises(AssertionError):
+        _ = ObjectQuery([".", ("*", {"name": "test"})], multi_index_mode="foo")
+    with pytest.raises(AssertionError):
+        _ = StringQuery(
+            u""" MATCH (".")->("*", p)
+            WHERE p."name" = "test"
+            """,
+            multi_index_mode="foo",
+        )
+    gf = GraphFrame.from_tau(tau_profile_dir)
+    query = ObjectQuery(
+        [".", ("*", {"time (inc)": "> 17983.0"})], multi_index_mode="off"
+    )
+    engine = QueryEngine()
+    with pytest.raises(MultiIndexModeMismatch):
+        engine.apply(query, gf.graph, gf.dataframe)
```

### Comparing `llnl-hatchet-2022.2.2/hatchet/tests/hpctoolkit.py` & `llnl-hatchet-2023.1.0/hatchet/tests/hpctoolkit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017-2022 Lawrence Livermore National Security, LLC and other
+# Copyright 2017-2023 Lawrence Livermore National Security, LLC and other
 # Hatchet Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: MIT
 
 import numpy as np
 import pandas as pd
 import os
```

### Comparing `llnl-hatchet-2022.2.2/hatchet/tests/pyinstrument.py` & `llnl-hatchet-2023.1.0/hatchet/tests/pyinstrument.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017-2022 Lawrence Livermore National Security, LLC and other
+# Copyright 2017-2023 Lawrence Livermore National Security, LLC and other
 # Hatchet Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: MIT
 
 import json
 
 import numpy as np
```

### Comparing `llnl-hatchet-2022.2.2/hatchet/tests/graph.py` & `llnl-hatchet-2023.1.0/hatchet/tests/graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017-2022 Lawrence Livermore National Security, LLC and other
+# Copyright 2017-2023 Lawrence Livermore National Security, LLC and other
 # Hatchet Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: MIT
 
 from hatchet.node import Node
 from hatchet.frame import Frame
 from hatchet.graph import Graph
```

### Comparing `llnl-hatchet-2022.2.2/hatchet/tests/graph_literal.py` & `llnl-hatchet-2023.1.0/hatchet/tests/graph_literal.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017-2022 Lawrence Livermore National Security, LLC and other
+# Copyright 2017-2023 Lawrence Livermore National Security, LLC and other
 # Hatchet Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: MIT
 
 from hatchet import GraphFrame
```

### Comparing `llnl-hatchet-2022.2.2/hatchet/tests/callgrind.py` & `llnl-hatchet-2023.1.0/hatchet/tests/callgrind.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017-2022 Lawrence Livermore National Security, LLC and other
+# Copyright 2017-2023 Lawrence Livermore National Security, LLC and other
 # Hatchet Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: MIT
 
 import numpy as np
 
 from hatchet import GraphFrame
```

### Comparing `llnl-hatchet-2022.2.2/hatchet/tests/timemory_test.py` & `llnl-hatchet-2023.1.0/hatchet/tests/timemory_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017-2022 Lawrence Livermore National Security, LLC and other
+# Copyright 2017-2023 Lawrence Livermore National Security, LLC and other
 # Hatchet Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: MIT
 
 import numpy as np
 
 from hatchet import GraphFrame
```

### Comparing `llnl-hatchet-2022.2.2/hatchet/tests/executable.py` & `llnl-hatchet-2023.1.0/hatchet/tests/executable.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017-2022 Lawrence Livermore National Security, LLC and other
+# Copyright 2017-2023 Lawrence Livermore National Security, LLC and other
 # Hatchet Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: MIT
 
 import os
 import stat
```

### Comparing `llnl-hatchet-2022.2.2/hatchet/tests/frame.py` & `llnl-hatchet-2023.1.0/hatchet/tests/frame.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017-2022 Lawrence Livermore National Security, LLC and other
+# Copyright 2017-2023 Lawrence Livermore National Security, LLC and other
 # Hatchet Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: MIT
 
 import pytest
 
 from hatchet.frame import Frame
```

### Comparing `llnl-hatchet-2022.2.2/hatchet/tests/graphframe.py` & `llnl-hatchet-2023.1.0/hatchet/tests/graphframe.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2017-2022 Lawrence Livermore National Security, LLC and other
+# Copyright 2017-2023 Lawrence Livermore National Security, LLC and other
 # Hatchet Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: MIT
 
 from __future__ import division
 
 import os
```

### Comparing `llnl-hatchet-2022.2.2/hatchet/tests/graph_ops.py` & `llnl-hatchet-2023.1.0/hatchet/tests/graph_ops.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017-2022 Lawrence Livermore National Security, LLC and other
+# Copyright 2017-2023 Lawrence Livermore National Security, LLC and other
 # Hatchet Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: MIT
 
 from hatchet import GraphFrame
```

### Comparing `llnl-hatchet-2022.2.2/hatchet/tests/tau.py` & `llnl-hatchet-2023.1.0/hatchet/tests/tau.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017-2022 Lawrence Livermore National Security, LLC and other
+# Copyright 2017-2023 Lawrence Livermore National Security, LLC and other
 # Hatchet Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: MIT
 
 import numpy as np
 
 from hatchet import GraphFrame
```

### Comparing `llnl-hatchet-2022.2.2/hatchet/tests/json_test.py` & `llnl-hatchet-2023.1.0/hatchet/tests/json_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017-2022 Lawrence Livermore National Security, LLC and other
+# Copyright 2017-2023 Lawrence Livermore National Security, LLC and other
 # Hatchet Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: MIT
 
 from hatchet import GraphFrame
```

### Comparing `llnl-hatchet-2022.2.2/hatchet/tests/node.py` & `llnl-hatchet-2023.1.0/hatchet/tests/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017-2022 Lawrence Livermore National Security, LLC and other
+# Copyright 2017-2023 Lawrence Livermore National Security, LLC and other
 # Hatchet Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: MIT
 
 import pytest
 
 from hatchet.node import Node, MultiplePathError
```

### Comparing `llnl-hatchet-2022.2.2/hatchet/tests/profiler.py` & `llnl-hatchet-2023.1.0/hatchet/tests/profiler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017-2022 Lawrence Livermore National Security, LLC and other
+# Copyright 2017-2023 Lawrence Livermore National Security, LLC and other
 # Hatchet Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: MIT
 
 import hatchet as ht
 import pstats
 import os
```

### Comparing `llnl-hatchet-2022.2.2/hatchet/frame.py` & `llnl-hatchet-2023.1.0/hatchet/frame.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017-2022 Lawrence Livermore National Security, LLC and other
+# Copyright 2017-2023 Lawrence Livermore National Security, LLC and other
 # Hatchet Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: MIT
 
 from functools import total_ordering
```

### Comparing `llnl-hatchet-2022.2.2/hatchet/graphframe.py` & `llnl-hatchet-2023.1.0/hatchet/graphframe.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017-2022 Lawrence Livermore National Security, LLC and other
+# Copyright 2017-2023 Lawrence Livermore National Security, LLC and other
 # Hatchet Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: MIT
 
 import copy
 import sys
 import traceback
@@ -13,15 +13,21 @@
 import numpy as np
 import multiprocess as mp
 import json
 
 from .node import Node
 from .graph import Graph
 from .frame import Frame
-from .query import AbstractQuery, QueryMatcher, parse_cypher_query
+from .query import (
+    is_hatchet_query,
+    ObjectQuery,
+    parse_string_dialect,
+    QueryEngine,
+    AbstractQuery,
+)
 from .external.console import ConsoleRenderer
 from .util.dot import trees_to_dot
 from .util.deprecated import deprecated_params
 
 try:
     from .cython_modules.libs import graphframe_modules as _gfm_cy
 except ImportError:
@@ -82,14 +88,15 @@
 
         self.graph = graph
         self.dataframe = dataframe
         self.exc_metrics = [] if exc_metrics is None else exc_metrics
         self.inc_metrics = [] if inc_metrics is None else inc_metrics
         self.default_metric = default_metric
         self.metadata = metadata
+        self.query_engine = QueryEngine()
 
     @staticmethod
     def from_hpctoolkit(dirname):
         """Read an HPCToolkit database directory into a new GraphFrame.
 
         Arguments:
             dirname (str): parent directory of an HPCToolkit
@@ -115,25 +122,32 @@
         """
         # import this lazily to avoid circular dependencies
         from .readers.caliper_reader import CaliperReader
 
         return CaliperReader(filename_or_stream, query).read()
 
     @staticmethod
-    def from_caliperreader(filename_or_caliperreader):
+    def from_caliperreader(
+        filename_or_caliperreader, native=False, string_attributes=[]
+    ):
         """Read in a native Caliper `cali` file using Caliper's python reader.
 
         Args:
             filename_or_caliperreader (str or CaliperReader): name of a Caliper
                 output file in `.cali` format, or a CaliperReader object
+            native (bool): use native or user-readable metric names (default)
+            string_attributes (str or list, optional): Adds existing string
+                attributes from within the caliper file to the dataframe
         """
         # import this lazily to avoid circular dependencies
         from .readers.caliper_native_reader import CaliperNativeReader
 
-        return CaliperNativeReader(filename_or_caliperreader).read()
+        return CaliperNativeReader(
+            filename_or_caliperreader, native, string_attributes
+        ).read()
 
     @staticmethod
     def from_spotdb(db_key, list_of_ids=None):
         """Read multiple graph frames from a SpotDB instance
 
         Args:
             db_key (str or SpotDB object): locator for SpotDB instance
@@ -396,22 +410,31 @@
 
         # perform a groupby to merge nodes that just differ in index columns
         self.dataframe.reset_index(level="node", inplace=True)
         agg_df = self.dataframe.groupby("node").agg(agg_dict)
 
         self.dataframe = agg_df
 
-    def filter(self, filter_obj, squash=True, num_procs=mp.cpu_count(), rec_limit=1000):
+    def filter(
+        self,
+        filter_obj,
+        squash=True,
+        update_inc_cols=True,
+        num_procs=mp.cpu_count(),
+        rec_limit=1000,
+        multi_index_mode="off",
+    ):
         """Filter the dataframe using a user-supplied function.
 
         Note: Operates in parallel on user-supplied lambda functions.
 
         Arguments:
             filter_obj (callable, list, or QueryMatcher): the filter to apply to the GraphFrame.
             squash (boolean, optional): if True, automatically call squash for the user.
+            update_inc_cols (boolean, optional): if True, update inclusive columns when performing squash.
             rec_limit: set Python recursion limit, increase if running into
                 recursion depth errors) (default: 1000).
         """
         sys.setrecursionlimit(rec_limit)
 
         dataframe_copy = self.dataframe.copy()
 
@@ -453,24 +476,29 @@
                 filtered_df = pd.concat(returned_frames)
 
             else:
                 # perform filter sequentiually if num_procs = 1
                 filtered_rows = dataframe_copy.apply(filter_obj, axis=1)
                 filtered_df = dataframe_copy[filtered_rows]
 
-        elif isinstance(filter_obj, (list, str)) or issubclass(
-            type(filter_obj), AbstractQuery
-        ):
+        elif isinstance(filter_obj, (list, str)) or is_hatchet_query(filter_obj):
             # use a callpath query to apply the filter
             query = filter_obj
+            # If a raw Object-dialect query is provided (not already passed to ObjectQuery),
+            # create a new ObjectQuery object.
             if isinstance(filter_obj, list):
-                query = QueryMatcher(filter_obj)
+                query = ObjectQuery(filter_obj, multi_index_mode)
+            # If a raw String-dialect query is provided (not already passed to StringQuery),
+            # create a new StringQuery object.
             elif isinstance(filter_obj, str):
-                query = parse_cypher_query(filter_obj)
-            query_matches = query.apply(self)
+                query = parse_string_dialect(filter_obj, multi_index_mode)
+            # If an old-style query is provided, extract the underlying new-style query.
+            elif issubclass(type(filter_obj), AbstractQuery):
+                query = filter_obj._get_new_query()
+            query_matches = self.query_engine.apply(query, self.graph, self.dataframe)
             # match_set = list(set().union(*query_matches))
             # filtered_df = dataframe_copy.loc[dataframe_copy["node"].isin(match_set)]
             filtered_df = dataframe_copy.loc[dataframe_copy["node"].isin(query_matches)]
         else:
             raise InvalidFilter(
                 "The argument passed to filter must be a callable, a query path list, or a QueryMatcher object."
             )
@@ -485,22 +513,25 @@
         filtered_gf = GraphFrame(self.graph, filtered_df)
         filtered_gf.exc_metrics = self.exc_metrics
         filtered_gf.inc_metrics = self.inc_metrics
         filtered_gf.default_metric = self.default_metric
         filtered_gf.metadata = self.metadata
 
         if squash:
-            return filtered_gf.squash()
+            return filtered_gf.squash(update_inc_cols)
         return filtered_gf
 
-    def squash(self):
+    def squash(self, update_inc_cols=True):
         """Rewrite the Graph to include only nodes present in the DataFrame's rows.
 
         This can be used to simplify the Graph, or to normalize Graph
         indexes between two GraphFrames.
+
+        Arguments:
+            update_inc_cols (boolean, optional): if True, update inclusive columns.
         """
         index_names = self.dataframe.index.names
         self.dataframe.reset_index(inplace=True)
 
         # create new nodes for each unique node in the old dataframe
         old_to_new = {n: n.copy() for n in set(self.dataframe["node"])}
         for i in old_to_new:
@@ -584,15 +615,16 @@
             graph,
             agg_df,
             self.exc_metrics,
             self.inc_metrics,
             self.default_metric,
             self.metadata,
         )
-        new_gf.update_inclusive_columns()
+        if update_inc_cols:
+            new_gf.update_inclusive_columns()
         return new_gf
 
     def _init_sum_columns(self, columns, out_columns):
         """Helper function for subtree_sum and subgraph_sum."""
         if out_columns is None:
             out_columns = columns
         else:
@@ -825,18 +857,28 @@
 
         # TODO When Python 2.7 support is dropped, change this line to the more idiomatic:
         # old_inc_metrics = self.inc_metrics.copy()
         old_inc_metrics = list(self.inc_metrics)
         # TODO Change this logic when inc_metrics and exc_metrics are changed
         new_inc_metrics = []
         for exc in self.exc_metrics:
-            if exc.endswith("(exc)"):
-                new_inc_metrics.append(exc[: -len("(exc)")].strip())
+            if isinstance(exc, tuple):
+                if exc[-1].endswith("(exc)"):
+                    temp = list(exc)
+                    temp[-1] = temp[-1][: -len("(exc)")].strip()
+                    new_inc_metrics.append(tuple(temp))
+                else:
+                    temp = list(exc)
+                    temp[-1] = "%s (inc)" % temp[-1]
+                    new_inc_metrics.append(tuple(temp))
             else:
-                new_inc_metrics.append("%s (inc)" % exc)
+                if exc.endswith("(exc)"):
+                    new_inc_metrics.append(exc[: -len("(exc)")].strip())
+                else:
+                    new_inc_metrics.append("%s (inc)" % exc)
         self.inc_metrics = new_inc_metrics
 
         self.subgraph_sum(self.exc_metrics, self.inc_metrics)
         self.inc_metrics = list(set(self.inc_metrics + old_inc_metrics))
 
     def show_metric_columns(self):
         """Returns a list of dataframe column labels."""
```

### Comparing `llnl-hatchet-2022.2.2/hatchet/node.py` & `llnl-hatchet-2023.1.0/hatchet/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017-2022 Lawrence Livermore National Security, LLC and other
+# Copyright 2017-2023 Lawrence Livermore National Security, LLC and other
 # Hatchet Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: MIT
 
 from functools import total_ordering
 
 from .frame import Frame
```

### Comparing `llnl-hatchet-2022.2.2/hatchet/readers/gprof_dot_reader.py` & `llnl-hatchet-2023.1.0/hatchet/readers/gprof_dot_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017-2022 Lawrence Livermore National Security, LLC and other
+# Copyright 2017-2023 Lawrence Livermore National Security, LLC and other
 # Hatchet Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: MIT
 
 import re
 
 import pandas as pd
```

### Comparing `llnl-hatchet-2022.2.2/hatchet/readers/caliper_reader.py` & `llnl-hatchet-2023.1.0/hatchet/readers/caliper_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017-2022 Lawrence Livermore National Security, LLC and other
+# Copyright 2017-2023 Lawrence Livermore National Security, LLC and other
 # Hatchet Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: MIT
 
 import json
 import sys
 import re
```

### Comparing `llnl-hatchet-2022.2.2/hatchet/readers/pyinstrument_reader.py` & `llnl-hatchet-2023.1.0/hatchet/readers/pyinstrument_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017-2022 Lawrence Livermore National Security, LLC and other
+# Copyright 2017-2023 Lawrence Livermore National Security, LLC and other
 # Hatchet Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: MIT
 
 import json
 
 import pandas as pd
```

### Comparing `llnl-hatchet-2022.2.2/hatchet/readers/hdf5_reader.py` & `llnl-hatchet-2023.1.0/hatchet/readers/hdf5_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017-2022 Lawrence Livermore National Security, LLC and other
+# Copyright 2017-2023 Lawrence Livermore National Security, LLC and other
 # Hatchet Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: MIT
 
 import warnings
 import pandas as pd
 import sys
```

### Comparing `llnl-hatchet-2022.2.2/hatchet/readers/dataframe_reader.py` & `llnl-hatchet-2023.1.0/hatchet/readers/dataframe_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017-2022 Lawrence Livermore National Security, LLC and other
+# Copyright 2017-2023 Lawrence Livermore National Security, LLC and other
 # Hatchet Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: MIT
 
 import hatchet.graphframe
 from hatchet.node import Node
 from hatchet.graph import Graph
```

### Comparing `llnl-hatchet-2022.2.2/hatchet/readers/literal_reader.py` & `llnl-hatchet-2023.1.0/hatchet/readers/literal_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017-2022 Lawrence Livermore National Security, LLC and other
+# Copyright 2017-2023 Lawrence Livermore National Security, LLC and other
 # Hatchet Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: MIT
 
 import pandas as pd
 
 import hatchet.graphframe
```

### Comparing `llnl-hatchet-2022.2.2/hatchet/readers/cprofile_reader.py` & `llnl-hatchet-2023.1.0/hatchet/readers/cprofile_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017-2022 Lawrence Livermore National Security, LLC and other
+# Copyright 2017-2023 Lawrence Livermore National Security, LLC and other
 # Hatchet Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: MIT
 
 import pstats
 import sys
 import pandas as pd
```

### Comparing `llnl-hatchet-2022.2.2/hatchet/readers/timemory_reader.py` & `llnl-hatchet-2023.1.0/hatchet/readers/timemory_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017-2022 Lawrence Livermore National Security, LLC and other
+# Copyright 2017-2023 Lawrence Livermore National Security, LLC and other
 # Hatchet Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: MIT
 
 import json
 import pandas as pd
 import os
@@ -355,15 +355,15 @@
             # check if we saw this (callpath, rank, thread) before
             if node_dict is None:
                 # if no, create a new dict.
                 self.callpath_to_node_dict[callpath_rank_thread] = dict(
                     {"node": _hnode, **_frame_attrs},
                     **_extra,
                     **_exc_stats,
-                    **_inc_stats
+                    **_inc_stats,
                 )
             else:
                 # if yes, don't create a new dict, just add the new metrics to
                 # the existing node_dict using update().
                 # we are doing this to combine different metrics on a single dataframe.
                 self.callpath_to_node_dict[callpath_rank_thread].update(
                     dict(**_exc_stats, **_inc_stats)
```

### Comparing `llnl-hatchet-2022.2.2/hatchet/readers/tau_reader.py` & `llnl-hatchet-2023.1.0/hatchet/readers/tau_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017-2022 Lawrence Livermore National Security, LLC and other
+# Copyright 2017-2023 Lawrence Livermore National Security, LLC and other
 # Hatchet Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: MIT
 
 import re
 import os
 import glob
```

### Comparing `llnl-hatchet-2022.2.2/hatchet/readers/hpctoolkit_reader.py` & `llnl-hatchet-2023.1.0/hatchet/readers/hpctoolkit_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017-2022 Lawrence Livermore National Security, LLC and other
+# Copyright 2017-2023 Lawrence Livermore National Security, LLC and other
 # Hatchet Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: MIT
 
 import glob
 import struct
 import re
```

### Comparing `llnl-hatchet-2022.2.2/hatchet/readers/caliper_native_reader.py` & `llnl-hatchet-2023.1.0/hatchet/readers/caliper_native_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017-2022 Lawrence Livermore National Security, LLC and other
+# Copyright 2017-2023 Lawrence Livermore National Security, LLC and other
 # Hatchet Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: MIT
 
 
 import pandas as pd
 import os
@@ -15,23 +15,27 @@
 from hatchet.frame import Frame
 from hatchet.util.timer import Timer
 
 
 class CaliperNativeReader:
     """Read in a native `.cali` file using Caliper's python reader."""
 
-    def __init__(self, filename_or_caliperreader):
+    def __init__(self, filename_or_caliperreader, native, string_attributes):
         """Read in a native cali using Caliper's python reader.
 
         Args:
             filename_or_caliperreader (str or CaliperReader): name of a `cali` file OR
                 a CaliperReader object
+            native (bool): use native metric names or user-readable metric names
+            string_attributes (str or list): Adds existing string attributes from within the caliper file to the dataframe
         """
         self.filename_or_caliperreader = filename_or_caliperreader
         self.filename_ext = ""
+        self.use_native_metric_names = native
+        self.string_attributes = string_attributes
 
         self.df_nodes = {}
         self.metric_cols = []
         self.record_data_cols = []
         self.node_dicts = []
         self.callpath_to_node = {}
         self.idx_to_node = {}
@@ -41,14 +45,17 @@
         self.default_metric = None
 
         self.timer = Timer()
 
         if isinstance(self.filename_or_caliperreader, str):
             _, self.filename_ext = os.path.splitext(filename_or_caliperreader)
 
+        if isinstance(self.string_attributes, str):
+            self.string_attributes = [self.string_attributes]
+
     def read_metrics(self, ctx="path"):
         all_metrics = []
         records = self.filename_or_caliperreader.records
 
         # read metadata from the caliper reader
         for record in records:
             node_dict = {}
@@ -98,24 +105,35 @@
                                     item
                                 ).attribute_type()
                                 == "int"
                             ):
                                 node_dict[item] = int(record[item])
                                 if item not in self.record_data_cols:
                                     self.record_data_cols.append(item)
+                            elif (
+                                self.filename_or_caliperreader.attribute(
+                                    item
+                                ).attribute_type()
+                                == "string"
+                            ):
+                                if item in self.string_attributes:
+                                    node_dict[item] = record[item]
+                                    if item not in self.record_data_cols:
+                                        self.record_data_cols.append(item)
 
                     all_metrics.append(node_dict)
 
         # make list of metric columns
         for col in self.record_data_cols:
             if self.filename_or_caliperreader.attribute(col).is_value():
                 self.metric_cols.append(col)
 
         df_metrics = pd.DataFrame.from_dict(data=all_metrics)
-        return df_metrics
+        df_new = df_metrics.groupby(df_metrics["nid"]).aggregate("first").reset_index()
+        return df_new
 
     def create_graph(self, ctx="path"):
         list_roots = []
 
         def _create_parent(child_node, parent_callpath):
             """We may encounter a parent node in the callpath before we see it
             as a child node. In this case, we need to create a hatchet node for
@@ -359,14 +377,31 @@
                         node_dict["nid"] = row["nid"]
                         node_dict["mpi.rank"] = rank
                         missing_nodes.append(node_dict)
 
         df_missing = pd.DataFrame.from_dict(data=missing_nodes)
         df_metrics = pd.concat([df_fixed_data, df_missing], sort=False)
 
+        # rename columns to user-readable metric names (i.e., aliases)
+        if not self.use_native_metric_names:
+            for col in df_metrics.columns:
+                if col == "nid":
+                    continue
+                alias = self.filename_or_caliperreader.attribute(col).get(
+                    "attribute.alias"
+                )
+                if alias:
+                    # update column name in metrics dataframe
+                    df_metrics.rename(columns={col: alias}, inplace=True)
+
+                    # also update list of metric columns
+                    self.metric_cols = [
+                        alias if item == col else item for item in self.metric_cols
+                    ]
+
         # dict mapping old to new column names to make columns consistent with
         # other readers
         old_to_new = {
             "mpi.rank": "rank",
             "module#cali.sampler.pc": "module",
             "sum#time.duration": "time",
             "sum#avg#sum#time.duration": "time",
```

### Comparing `llnl-hatchet-2022.2.2/hatchet/readers/spotdb_reader.py` & `llnl-hatchet-2023.1.0/hatchet/readers/spotdb_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017-2022 Lawrence Livermore National Security, LLC and other
+# Copyright 2017-2023 Lawrence Livermore National Security, LLC and other
 # Hatchet Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: MIT
 
 import pandas as pd
 
 import hatchet.graphframe
```

### Comparing `llnl-hatchet-2022.2.2/hatchet/readers/json_reader.py` & `llnl-hatchet-2023.1.0/hatchet/readers/json_reader.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017-2022 Lawrence Livermore National Security, LLC and other
+# Copyright 2017-2023 Lawrence Livermore National Security, LLC and other
 # Hatchet Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: MIT
 
 import json
 
 import pandas as pd
```

### Comparing `llnl-hatchet-2022.2.2/hatchet/external/console.py` & `llnl-hatchet-2023.1.0/hatchet/external/console.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2022.2.2/LICENSE` & `llnl-hatchet-2023.1.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2017-2022, Lawrence Livermore National Security, LLC.
+Copyright (c) 2017-2023, Lawrence Livermore National Security, LLC.
 
 Permission is hereby granted, free of charge, to any person obtaining a
 copy of this software and associated documentation files (the "Software"),
 to deal in the Software without restriction, including without limitation
 the rights to use, copy, modify, merge, publish, distribute, sublicense,
 and/or sell copies of the Software, and to permit persons to whom the
 Software is furnished to do so, subject to the following conditions:
```

### Comparing `llnl-hatchet-2022.2.2/pyproject.toml` & `llnl-hatchet-2023.1.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,18 @@
+[build-system]
+requires = [
+    "setuptools",
+    "wheel",
+    "Cython",
+]
+build-backend = "setuptools.build_meta"
+
 [tool.poetry]
 name = "llnl-hatchet"
-version = "2022.2.2"
+version = "2023.1.0"
 description = "A Python library for analyzing hierarchical performance data."
 authors = [
     "Abhinav Bhatele <bhatele@cs.umd.edu>",
     "Stephanie Brink <brink2@llnl.gov>",
     "Todd Gamblin <tgamblin@llnl.gov>",
 ]
 license = "MIT"
```

### Comparing `llnl-hatchet-2022.2.2/NOTICE` & `llnl-hatchet-2023.1.0/NOTICE`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2022.2.2/README.md` & `llnl-hatchet-2023.1.0/README.md`

 * *Files identical despite different names*

