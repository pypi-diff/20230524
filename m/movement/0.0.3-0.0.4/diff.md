# Comparing `tmp/movement-0.0.3.tar.gz` & `tmp/movement-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/movement-0.0.3.tar", last modified: Wed Apr  8 13:42:38 2020, max compression
+gzip compressed data, was "movement-0.0.4.tar", last modified: Wed May 24 15:44:17 2023, max compression
```

## Comparing `movement-0.0.3.tar` & `movement-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,35 @@
-drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2020-04-08 13:42:38.924372 movement-0.0.3/
--rw-r--r--   0 adam      (1000) adam      (1000)        0 2020-04-03 14:26:04.000000 movement-0.0.3/MANIFEST.in
--rw-r--r--   0 adam      (1000) adam      (1000)      660 2020-04-08 13:42:38.924372 movement-0.0.3/PKG-INFO
--rw-r--r--   0 adam      (1000) adam      (1000)      151 2020-04-03 17:55:16.000000 movement-0.0.3/README.md
-drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2020-04-08 13:42:38.924372 movement-0.0.3/movement/
--rw-r--r--   0 adam      (1000) adam      (1000)        0 2020-04-03 14:25:20.000000 movement-0.0.3/movement/__init__.py
-drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2020-04-08 13:42:38.924372 movement-0.0.3/movement/io/
--rw-r--r--   0 adam      (1000) adam      (1000)        0 2020-04-06 09:36:45.000000 movement-0.0.3/movement/io/__init__.py
--rw-r--r--   0 adam      (1000) adam      (1000)     2507 2020-04-08 09:54:02.000000 movement-0.0.3/movement/io/dlc.py
-drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2020-04-08 13:42:38.924372 movement-0.0.3/movement/movement/
--rw-r--r--   0 adam      (1000) adam      (1000)        0 2020-04-06 09:11:44.000000 movement-0.0.3/movement/movement/__init__.py
--rw-r--r--   0 adam      (1000) adam      (1000)     1575 2020-04-06 09:54:51.000000 movement-0.0.3/movement/movement/velocity.py
-drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2020-04-08 13:42:38.924372 movement-0.0.3/movement/position/
--rw-r--r--   0 adam      (1000) adam      (1000)        0 2020-04-03 16:13:24.000000 movement-0.0.3/movement/position/__init__.py
--rw-r--r--   0 adam      (1000) adam      (1000)      704 2020-04-03 17:53:18.000000 movement-0.0.3/movement/position/angles.py
-drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2020-04-08 13:42:38.924372 movement-0.0.3/movement.egg-info/
--rw-r--r--   0 adam      (1000) adam      (1000)      660 2020-04-08 13:42:38.000000 movement-0.0.3/movement.egg-info/PKG-INFO
--rw-r--r--   0 adam      (1000) adam      (1000)      402 2020-04-08 13:42:38.000000 movement-0.0.3/movement.egg-info/SOURCES.txt
--rw-r--r--   0 adam      (1000) adam      (1000)        1 2020-04-08 13:42:38.000000 movement-0.0.3/movement.egg-info/dependency_links.txt
--rw-r--r--   0 adam      (1000) adam      (1000)        1 2020-04-03 14:29:53.000000 movement-0.0.3/movement.egg-info/not-zip-safe
--rw-r--r--   0 adam      (1000) adam      (1000)      131 2020-04-08 13:42:38.000000 movement-0.0.3/movement.egg-info/requires.txt
--rw-r--r--   0 adam      (1000) adam      (1000)       16 2020-04-08 13:42:38.000000 movement-0.0.3/movement.egg-info/top_level.txt
--rw-r--r--   0 adam      (1000) adam      (1000)       38 2020-04-08 13:42:38.924372 movement-0.0.3/setup.cfg
--rw-r--r--   0 adam      (1000) adam      (1000)     1187 2020-04-08 13:42:26.000000 movement-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:44:17.049431 movement-0.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:44:17.045431 movement-0.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:44:17.049431 movement-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-24 15:44:07.000000 movement-0.0.4/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-24 15:44:07.000000 movement-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-24 15:44:07.000000 movement-0.0.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-24 15:44:07.000000 movement-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-24 15:44:07.000000 movement-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-05-24 15:44:17.049431 movement-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-05-24 15:44:07.000000 movement-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:44:17.049431 movement-0.0.4/movement/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-24 15:44:07.000000 movement-0.0.4/movement/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:44:17.049431 movement-0.0.4/movement/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:44:07.000000 movement-0.0.4/movement/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-05-24 15:44:07.000000 movement-0.0.4/movement/io/load_poses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-24 15:44:07.000000 movement-0.0.4/movement/io/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-24 15:44:07.000000 movement-0.0.4/movement/log_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:44:17.049431 movement-0.0.4/movement.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-05-24 15:44:17.000000 movement-0.0.4/movement.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-24 15:44:17.000000 movement-0.0.4/movement.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:44:17.000000 movement-0.0.4/movement.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-24 15:44:17.000000 movement-0.0.4/movement.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-24 15:44:17.000000 movement-0.0.4/movement.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-05-24 15:44:07.000000 movement-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 15:44:17.049431 movement-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:44:17.049431 movement-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:44:07.000000 movement-0.0.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-24 15:44:07.000000 movement-0.0.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:44:17.049431 movement-0.0.4/tests/test_integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:44:07.000000 movement-0.0.4/tests/test_integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:44:17.049431 movement-0.0.4/tests/test_unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:44:07.000000 movement-0.0.4/tests/test_unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-05-24 15:44:07.000000 movement-0.0.4/tests/test_unit/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-24 15:44:07.000000 movement-0.0.4/tests/test_unit/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-24 15:44:07.000000 movement-0.0.4/tox.ini
```

