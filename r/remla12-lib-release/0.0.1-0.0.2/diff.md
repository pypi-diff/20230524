# Comparing `tmp/remla12-lib-release-0.0.1.tar.gz` & `tmp/remla12-lib-release-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remla12-lib-release-0.0.1.tar", last modified: Fri May  5 11:06:27 2023, max compression
+gzip compressed data, was "remla12-lib-release-0.0.2.tar", last modified: Wed May 24 13:07:59 2023, max compression
```

## Comparing `remla12-lib-release-0.0.1.tar` & `remla12-lib-release-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:06:27.358149 remla12-lib-release-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-05 11:06:27.358149 remla12-lib-release-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-05 11:06:09.000000 remla12-lib-release-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:06:27.358149 remla12-lib-release-0.0.1/remla12_lib_release.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-05 11:06:27.000000 remla12-lib-release-0.0.1/remla12_lib_release.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-05 11:06:27.000000 remla12-lib-release-0.0.1/remla12_lib_release.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 11:06:27.000000 remla12-lib-release-0.0.1/remla12_lib_release.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 11:06:27.000000 remla12-lib-release-0.0.1/remla12_lib_release.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 11:06:27.358149 remla12-lib-release-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-05 11:06:09.000000 remla12-lib-release-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:07:59.264257 remla12-lib-release-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-24 13:07:59.264257 remla12-lib-release-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-24 13:07:45.000000 remla12-lib-release-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:07:59.264257 remla12-lib-release-0.0.2/remla12_lib_release.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-24 13:07:59.000000 remla12-lib-release-0.0.2/remla12_lib_release.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-24 13:07:59.000000 remla12-lib-release-0.0.2/remla12_lib_release.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 13:07:59.000000 remla12-lib-release-0.0.2/remla12_lib_release.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 13:07:59.000000 remla12-lib-release-0.0.2/remla12_lib_release.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 13:07:59.264257 remla12-lib-release-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-24 13:07:45.000000 remla12-lib-release-0.0.2/setup.py
```

