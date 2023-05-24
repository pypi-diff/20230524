# Comparing `tmp/vcorelib-1.6.4.tar.gz` & `tmp/vcorelib-1.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vcorelib-1.6.4.tar", last modified: Sat May 13 06:25:00 2023, max compression
+gzip compressed data, was "vcorelib-1.6.5.tar", last modified: Mon May 15 22:31:44 2023, max compression
```

## Comparing `vcorelib-1.6.4.tar` & `vcorelib-1.6.5.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 06:25:00.326831 vcorelib-1.6.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-13 06:23:09.000000 vcorelib-1.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-13 06:25:00.326831 vcorelib-1.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-05-13 06:23:09.000000 vcorelib-1.6.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-13 06:23:09.000000 vcorelib-1.6.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-13 06:25:00.326831 vcorelib-1.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-13 06:23:09.000000 vcorelib-1.6.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 06:25:00.314831 vcorelib-1.6.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-13 06:23:09.000000 vcorelib-1.6.4/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-13 06:23:09.000000 vcorelib-1.6.4/tests/test_names.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-13 06:23:09.000000 vcorelib-1.6.4/tests/test_namespace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 06:25:00.314831 vcorelib-1.6.4/vcorelib/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 06:25:00.318831 vcorelib-1.6.4/vcorelib/args/
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/args/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/args/newline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 06:25:00.318831 vcorelib-1.6.4/vcorelib/asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/asyncio/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/asyncio/subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/dev_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 06:25:00.318831 vcorelib-1.6.4/vcorelib/dict/
--rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/dict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/dict/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/dict/codec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/dict/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/dict/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 06:25:00.318831 vcorelib-1.6.4/vcorelib/graph/
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7436 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/graph/abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/graph/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/graph/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/graph/port.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 06:25:00.322831 vcorelib-1.6.4/vcorelib/io/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/io/abc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 06:25:00.322831 vcorelib-1.6.4/vcorelib/io/arbiter/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/io/arbiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/io/arbiter/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/io/arbiter/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/io/arbiter/directory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 06:25:00.322831 vcorelib-1.6.4/vcorelib/io/archive/
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/io/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/io/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/io/decode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/io/encode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/io/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/io/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 06:25:00.322831 vcorelib-1.6.4/vcorelib/math/
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/math/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 06:25:00.322831 vcorelib-1.6.4/vcorelib/math/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/math/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/math/analysis/average.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 06:25:00.322831 vcorelib-1.6.4/vcorelib/math/analysis/rate/
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/math/analysis/rate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/math/analysis/rate/limiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/math/time.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/names.py
--rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/namespace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 06:25:00.322831 vcorelib-1.6.4/vcorelib/paths/
--rw-r--r--   0 runner    (1001) docker     (123)     6054 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/paths/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/paths/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/paths/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/paths/info_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 06:25:00.322831 vcorelib-1.6.4/vcorelib/platform/
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 06:25:00.322831 vcorelib-1.6.4/vcorelib/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/schemas/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/schemas/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/schemas/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 06:25:00.326831 vcorelib-1.6.4/vcorelib/script/
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/script/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 06:25:00.326831 vcorelib-1.6.4/vcorelib/target/
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/target/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/target/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/target/expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/target/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 06:25:00.326831 vcorelib-1.6.4/vcorelib/task/
--rw-r--r--   0 runner    (1001) docker     (123)    11913 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/task/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 06:25:00.326831 vcorelib-1.6.4/vcorelib/task/dict/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/task/dict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/task/dict/melder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/task/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 06:25:00.326831 vcorelib-1.6.4/vcorelib/task/subprocess/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/task/subprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/task/subprocess/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 06:25:00.326831 vcorelib-1.6.4/vcorelib/task/time/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/task/time/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-13 06:23:09.000000 vcorelib-1.6.4/vcorelib/task/time/sleep.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 06:25:00.314831 vcorelib-1.6.4/vcorelib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-13 06:25:00.000000 vcorelib-1.6.4/vcorelib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-13 06:25:00.000000 vcorelib-1.6.4/vcorelib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 06:25:00.000000 vcorelib-1.6.4/vcorelib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-13 06:25:00.000000 vcorelib-1.6.4/vcorelib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-13 06:25:00.000000 vcorelib-1.6.4/vcorelib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:31:44.943096 vcorelib-1.6.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-15 22:30:21.000000 vcorelib-1.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-15 22:31:44.943096 vcorelib-1.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-05-15 22:30:21.000000 vcorelib-1.6.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-15 22:30:21.000000 vcorelib-1.6.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 22:31:44.943096 vcorelib-1.6.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-15 22:30:21.000000 vcorelib-1.6.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:31:44.935097 vcorelib-1.6.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-15 22:30:21.000000 vcorelib-1.6.5/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-15 22:30:21.000000 vcorelib-1.6.5/tests/test_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-15 22:30:21.000000 vcorelib-1.6.5/tests/test_namespace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:31:44.935097 vcorelib-1.6.5/vcorelib/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:31:44.939097 vcorelib-1.6.5/vcorelib/args/
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/args/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/args/newline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:31:44.939097 vcorelib-1.6.5/vcorelib/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/asyncio/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/asyncio/subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/dev_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:31:44.939097 vcorelib-1.6.5/vcorelib/dict/
+-rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/dict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/dict/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/dict/codec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/dict/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/dict/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:31:44.939097 vcorelib-1.6.5/vcorelib/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7436 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/graph/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/graph/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/graph/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/graph/port.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:31:44.939097 vcorelib-1.6.5/vcorelib/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/io/abc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:31:44.939097 vcorelib-1.6.5/vcorelib/io/arbiter/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/io/arbiter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/io/arbiter/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/io/arbiter/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/io/arbiter/directory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:31:44.939097 vcorelib-1.6.5/vcorelib/io/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/io/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/io/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/io/decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/io/encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/io/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/io/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:31:44.939097 vcorelib-1.6.5/vcorelib/math/
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/math/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:31:44.939097 vcorelib-1.6.5/vcorelib/math/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/math/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/math/analysis/average.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:31:44.943096 vcorelib-1.6.5/vcorelib/math/analysis/rate/
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/math/analysis/rate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/math/analysis/rate/limiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/math/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/namespace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:31:44.943096 vcorelib-1.6.5/vcorelib/paths/
+-rw-r--r--   0 runner    (1001) docker     (123)     6054 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/paths/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/paths/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/paths/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6913 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/paths/info_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:31:44.943096 vcorelib-1.6.5/vcorelib/platform/
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:31:44.943096 vcorelib-1.6.5/vcorelib/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/schemas/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/schemas/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/schemas/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:31:44.943096 vcorelib-1.6.5/vcorelib/script/
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/script/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:31:44.943096 vcorelib-1.6.5/vcorelib/target/
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/target/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/target/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/target/expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/target/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:31:44.943096 vcorelib-1.6.5/vcorelib/task/
+-rw-r--r--   0 runner    (1001) docker     (123)    11913 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/task/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:31:44.943096 vcorelib-1.6.5/vcorelib/task/dict/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/task/dict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/task/dict/melder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/task/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:31:44.943096 vcorelib-1.6.5/vcorelib/task/subprocess/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/task/subprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/task/subprocess/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:31:44.943096 vcorelib-1.6.5/vcorelib/task/time/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/task/time/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-15 22:30:21.000000 vcorelib-1.6.5/vcorelib/task/time/sleep.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:31:44.939097 vcorelib-1.6.5/vcorelib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-15 22:31:44.000000 vcorelib-1.6.5/vcorelib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-15 22:31:44.000000 vcorelib-1.6.5/vcorelib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 22:31:44.000000 vcorelib-1.6.5/vcorelib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-15 22:31:44.000000 vcorelib-1.6.5/vcorelib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-15 22:31:44.000000 vcorelib-1.6.5/vcorelib.egg-info/top_level.txt
```

### Comparing `vcorelib-1.6.4/LICENSE` & `vcorelib-1.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.4/PKG-INFO` & `vcorelib-1.6.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vcorelib
-Version: 1.6.4
+Version: 1.6.5
 Summary: A collection of core Python utilities.
 Home-page: https://github.com/vkottler/vcorelib
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=66904405c5937dfd140eee634412d8a1
+    hash=65da3e0aa71cb6e20ca639beab16e65d
     =====================================
 -->
 
-# vcorelib ([1.6.4](https://pypi.org/project/vcorelib/))
+# vcorelib ([1.6.5](https://pypi.org/project/vcorelib/))
 
 [![python](https://img.shields.io/pypi/pyversions/vcorelib.svg)](https://pypi.org/project/vcorelib/)
 ![Build Status](https://github.com/vkottler/vcorelib/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/vcorelib/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/vcorelib)
 ![PyPI - Status](https://img.shields.io/pypi/status/vcorelib)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/vcorelib)
```

### Comparing `vcorelib-1.6.4/README.md` & `vcorelib-1.6.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=66904405c5937dfd140eee634412d8a1
+    hash=65da3e0aa71cb6e20ca639beab16e65d
     =====================================
 -->
 
-# vcorelib ([1.6.4](https://pypi.org/project/vcorelib/))
+# vcorelib ([1.6.5](https://pypi.org/project/vcorelib/))
 
 [![python](https://img.shields.io/pypi/pyversions/vcorelib.svg)](https://pypi.org/project/vcorelib/)
 ![Build Status](https://github.com/vkottler/vcorelib/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/vcorelib/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/vcorelib)
 ![PyPI - Status](https://img.shields.io/pypi/status/vcorelib)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/vcorelib)
```

### Comparing `vcorelib-1.6.4/pyproject.toml` & `vcorelib-1.6.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "vcorelib"
-version = "1.6.4"
+version = "1.6.5"
 description = "A collection of core Python utilities."
 readme = "README.md"
 requires-python = ">=3.7"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `vcorelib-1.6.4/setup.py` & `vcorelib-1.6.5/setup.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.4/tests/test_logging.py` & `vcorelib-1.6.5/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.4/tests/test_names.py` & `vcorelib-1.6.5/tests/test_names.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.4/tests/test_namespace.py` & `vcorelib-1.6.5/tests/test_namespace.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.4/vcorelib/args/__init__.py` & `vcorelib-1.6.5/vcorelib/args/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.4/vcorelib/args/newline.py` & `vcorelib-1.6.5/vcorelib/args/newline.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.4/vcorelib/asyncio/__init__.py` & `vcorelib-1.6.5/vcorelib/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.4/vcorelib/asyncio/cli.py` & `vcorelib-1.6.5/vcorelib/asyncio/cli.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.4/vcorelib/asyncio/subprocess.py` & `vcorelib-1.6.5/vcorelib/asyncio/subprocess.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.4/vcorelib/dict/__init__.py` & `vcorelib-1.6.5/vcorelib/dict/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.4/vcorelib/dict/cache.py` & `vcorelib-1.6.5/vcorelib/dict/cache.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.4/vcorelib/dict/codec.py` & `vcorelib-1.6.5/vcorelib/dict/codec.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.4/vcorelib/dict/config.py` & `vcorelib-1.6.5/vcorelib/dict/config.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.4/vcorelib/dict/env.py` & `vcorelib-1.6.5/vcorelib/dict/env.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.4/vcorelib/graph/__init__.py` & `vcorelib-1.6.5/vcorelib/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.4/vcorelib/graph/abc.py` & `vcorelib-1.6.5/vcorelib/graph/abc.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.4/vcorelib/graph/edge.py` & `vcorelib-1.6.5/vcorelib/graph/edge.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.4/vcorelib/graph/node.py` & `vcorelib-1.6.5/vcorelib/graph/node.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.4/vcorelib/graph/port.py` & `vcorelib-1.6.5/vcorelib/graph/port.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.4/vcorelib/io/__init__.py` & `vcorelib-1.6.5/vcorelib/io/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.4/vcorelib/io/abc.py` & `vcorelib-1.6.5/vcorelib/io/abc.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.4/vcorelib/io/arbiter/base.py` & `vcorelib-1.6.5/vcorelib/io/arbiter/base.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.4/vcorelib/io/arbiter/context.py` & `vcorelib-1.6.5/vcorelib/io/arbiter/context.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.4/vcorelib/io/arbiter/directory.py` & `vcorelib-1.6.5/vcorelib/io/arbiter/directory.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.4/vcorelib/io/archive/__init__.py` & `vcorelib-1.6.5/vcorelib/io/archive/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.4/vcorelib/io/cache.py` & `vcorelib-1.6.5/vcorelib/io/cache.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.4/vcorelib/io/decode.py` & `vcorelib-1.6.5/vcorelib/io/decode.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.4/vcorelib/io/encode.py` & `vcorelib-1.6.5/vcorelib/io/encode.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.4/vcorelib/io/mapping.py` & `vcorelib-1.6.5/vcorelib/io/mapping.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.4/vcorelib/io/types.py` & `vcorelib-1.6.5/vcorelib/io/types.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.4/vcorelib/logging.py` & `vcorelib-1.6.5/vcorelib/logging.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.4/vcorelib/math/__init__.py` & `vcorelib-1.6.5/vcorelib/math/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.4/vcorelib/math/analysis/average.py` & `vcorelib-1.6.5/vcorelib/math/analysis/average.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.4/vcorelib/math/analysis/rate/__init__.py` & `vcorelib-1.6.5/vcorelib/math/analysis/rate/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.4/vcorelib/math/analysis/rate/limiter.py` & `vcorelib-1.6.5/vcorelib/math/analysis/rate/limiter.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.4/vcorelib/math/time.py` & `vcorelib-1.6.5/vcorelib/math/time.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.4/vcorelib/names.py` & `vcorelib-1.6.5/vcorelib/names.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.4/vcorelib/namespace.py` & `vcorelib-1.6.5/vcorelib/namespace.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.4/vcorelib/paths/__init__.py` & `vcorelib-1.6.5/vcorelib/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.4/vcorelib/paths/context.py` & `vcorelib-1.6.5/vcorelib/paths/context.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.4/vcorelib/paths/info.py` & `vcorelib-1.6.5/vcorelib/paths/info.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,21 +60,25 @@
         if stats is None:
             stats = _stats(path)
         assert stats is not None
         md5_hex = _file_md5_hex(path)
         return FileInfo(path, stats.st_size, md5_hex, stats.st_mtime_ns)
 
     def poll(
-        self,
+        self, check_contents: bool = True
     ) -> _Tuple[_Optional[FileChangeEvent], _Optional["FileInfo"]]:
         """Determine if this file is in a new state or not."""
 
         if not self.path.is_file():
             return FileChangeEvent.REMOVED, None
 
+        # Skip checking file contents if specified.
+        if not check_contents:
+            return None, self
+
         # If the file hasn't been modified, skip re-reading it for a new
         # checksum.
         stats = _stats(self.path)
         if stats is not None and stats.st_mtime_ns == self.modified_ns:
             return None, self
 
         new_info = FileInfo.from_file(self.path, stats)
```

### Comparing `vcorelib-1.6.4/vcorelib/paths/info_cache.py` & `vcorelib-1.6.5/vcorelib/paths/info_cache.py`

 * *Files 6% similar despite different names*

```diff
@@ -91,25 +91,27 @@
 
     def __init__(
         self,
         poll_cb: FileChangedCallback,
         initial: _Dict[_Path, FileInfo] = None,
         logger: LoggerType = None,
         level: int = _logging.DEBUG,
+        check_contents: bool = True,
     ) -> None:
         """Initialize this file-info manager."""
 
         self.poll = poll_cb
 
         if initial is None:
             initial = {}
         self.infos = initial
 
         self.logger = logger
         self.level = level
+        self.check_contents = check_contents
 
         # If we have initial files, poll them all.
         self.poll_existing()
 
     def _handle_info(self, path: _Path, info: _Optional[FileInfo]) -> None:
         """Update our internal tracking."""
 
@@ -174,17 +176,21 @@
             if path.is_file():
                 change = FileChangeEvent.CREATED
                 file_info = FileInfo.from_file(path)
 
             return change, file_info
 
         # Determine if the existing file has changed.
-        return self.infos[path].poll()
+        return self.infos[path].poll(check_contents=self.check_contents)
 
-    def poll_file(self, path: _Pathlike, base: _Pathlike = None) -> None:
+    def poll_file(
+        self,
+        path: _Pathlike,
+        base: _Pathlike = None,
+    ) -> None:
         """Check if a file has changed and invoke the callback if so."""
 
         norm = _normalize(path).resolve()
         kind, info = self._poll_path(norm)
 
         # Invoke the callback if a change event occured. Update our internal
         # structure if the callback succeeds.
@@ -197,25 +203,27 @@
 
 @_contextmanager
 def file_info_cache(
     cache_path: _Pathlike,
     poll_cb: FileChangedCallback,
     logger: LoggerType = None,
     level: int = _logging.DEBUG,
+    check_contents: bool = True,
 ) -> _Iterator[FileInfoManager]:
     """Obtain a file-info manager as a cached context."""
 
     path = _normalize(cache_path)
     assert not path.is_dir(), f"'{path}' is a directory!"
     with FileCache(path).loaded() as data:
         manager = FileInfoManager(
             poll_cb,
             FileInfo.from_json(data, force=True),
             logger=logger,
             level=level,
+            check_contents=check_contents,
         )
         yield manager
 
         # Update dictionary data with the current cache contents.
         data.clear()
         for info in manager.infos.values():
             info.to_json(data)
```

### Comparing `vcorelib-1.6.4/vcorelib/platform/__init__.py` & `vcorelib-1.6.5/vcorelib/platform/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.4/vcorelib/schemas/__init__.py` & `vcorelib-1.6.5/vcorelib/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.4/vcorelib/schemas/base.py` & `vcorelib-1.6.5/vcorelib/schemas/base.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.4/vcorelib/schemas/json.py` & `vcorelib-1.6.5/vcorelib/schemas/json.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.4/vcorelib/schemas/mixins.py` & `vcorelib-1.6.5/vcorelib/schemas/mixins.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.4/vcorelib/script/__init__.py` & `vcorelib-1.6.5/vcorelib/script/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.4/vcorelib/target/__init__.py` & `vcorelib-1.6.5/vcorelib/target/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.4/vcorelib/target/evaluation.py` & `vcorelib-1.6.5/vcorelib/target/evaluation.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.4/vcorelib/target/expression.py` & `vcorelib-1.6.5/vcorelib/target/expression.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.4/vcorelib/target/resolver.py` & `vcorelib-1.6.5/vcorelib/target/resolver.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.4/vcorelib/task/__init__.py` & `vcorelib-1.6.5/vcorelib/task/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.4/vcorelib/task/dict/melder.py` & `vcorelib-1.6.5/vcorelib/task/dict/melder.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.4/vcorelib/task/manager.py` & `vcorelib-1.6.5/vcorelib/task/manager.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.4/vcorelib/task/subprocess/run.py` & `vcorelib-1.6.5/vcorelib/task/subprocess/run.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.4/vcorelib/task/time/sleep.py` & `vcorelib-1.6.5/vcorelib/task/time/sleep.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.4/vcorelib.egg-info/PKG-INFO` & `vcorelib-1.6.5/vcorelib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vcorelib
-Version: 1.6.4
+Version: 1.6.5
 Summary: A collection of core Python utilities.
 Home-page: https://github.com/vkottler/vcorelib
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=66904405c5937dfd140eee634412d8a1
+    hash=65da3e0aa71cb6e20ca639beab16e65d
     =====================================
 -->
 
-# vcorelib ([1.6.4](https://pypi.org/project/vcorelib/))
+# vcorelib ([1.6.5](https://pypi.org/project/vcorelib/))
 
 [![python](https://img.shields.io/pypi/pyversions/vcorelib.svg)](https://pypi.org/project/vcorelib/)
 ![Build Status](https://github.com/vkottler/vcorelib/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/vcorelib/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/vcorelib)
 ![PyPI - Status](https://img.shields.io/pypi/status/vcorelib)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/vcorelib)
```

### Comparing `vcorelib-1.6.4/vcorelib.egg-info/SOURCES.txt` & `vcorelib-1.6.5/vcorelib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

