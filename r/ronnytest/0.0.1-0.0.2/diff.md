# Comparing `tmp/ronnytest-0.0.1.tar.gz` & `tmp/ronnytest-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ronnytest-0.0.1.tar", last modified: Wed May 24 11:34:50 2023, max compression
+gzip compressed data, was "dist/ronnytest-0.0.2.tar", last modified: Wed May 24 11:43:42 2023, max compression
```

## Comparing `ronnytest-0.0.1.tar` & `ronnytest-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 11:34:50.000000 ronnytest-0.0.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 11:34:50.000000 ronnytest-0.0.1/ronnytest.egg-info/
--rw-r--r--   0 root         (0) root         (0)      422 2023-05-24 11:34:50.000000 ronnytest-0.0.1/ronnytest.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 11:34:50.000000 ronnytest-0.0.1/ronnytest.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      158 2023-05-24 11:34:50.000000 ronnytest-0.0.1/ronnytest.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 11:34:50.000000 ronnytest-0.0.1/ronnytest.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 11:30:26.000000 ronnytest-0.0.1/README.md
--rw-r--r--   0 root         (0) root         (0)     1073 2023-05-15 11:35:28.000000 ronnytest-0.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      422 2023-05-24 11:34:50.000000 ronnytest-0.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-24 11:34:50.000000 ronnytest-0.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      560 2023-05-24 11:32:50.000000 ronnytest-0.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 11:43:42.000000 ronnytest-0.0.2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 11:43:42.000000 ronnytest-0.0.2/ronnytest.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      434 2023-05-24 11:43:42.000000 ronnytest-0.0.2/ronnytest.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 11:43:42.000000 ronnytest-0.0.2/ronnytest.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      158 2023-05-24 11:43:42.000000 ronnytest-0.0.2/ronnytest.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 11:43:42.000000 ronnytest-0.0.2/ronnytest.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 11:30:26.000000 ronnytest-0.0.2/README.md
+-rw-r--r--   0 root         (0) root         (0)     1073 2023-05-15 11:35:28.000000 ronnytest-0.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      434 2023-05-24 11:43:42.000000 ronnytest-0.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-24 11:43:42.000000 ronnytest-0.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1049 2023-05-24 11:43:34.000000 ronnytest-0.0.2/setup.py
```

### Comparing `ronnytest-0.0.1/LICENSE` & `ronnytest-0.0.2/LICENSE`

 * *Files identical despite different names*

