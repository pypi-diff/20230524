# Comparing `tmp/edman_cli-2023.5.23.tar.gz` & `tmp/edman_cli-2023.5.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edman_cli-2023.5.23.tar", last modified: Tue May 23 00:42:37 2023, max compression
+gzip compressed data, was "edman_cli-2023.5.24.tar", last modified: Wed May 24 05:54:16 2023, max compression
```

## Comparing `edman_cli-2023.5.23.tar` & `edman_cli-2023.5.24.tar`

### file list

```diff
@@ -1,66 +1,67 @@
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-23 00:42:37.130031 edman_cli-2023.5.23/
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1100 2023-03-15 06:38:21.000000 edman_cli-2023.5.23/LICENSE.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)     4934 2023-05-23 00:42:37.130031 edman_cli-2023.5.23/PKG-INFO
--rw-r--r--   0 ohno      (1000) ohno      (1000)     3345 2023-01-20 03:57:51.000000 edman_cli-2023.5.23/README.rst
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-23 00:42:37.120031 edman_cli-2023.5.23/edman_cli.egg-info/
--rw-r--r--   0 ohno      (1000) ohno      (1000)     4934 2023-05-23 00:42:37.000000 edman_cli-2023.5.23/edman_cli.egg-info/PKG-INFO
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1495 2023-05-23 00:42:37.000000 edman_cli-2023.5.23/edman_cli.egg-info/SOURCES.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)        1 2023-05-23 00:42:37.000000 edman_cli-2023.5.23/edman_cli.egg-info/dependency_links.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)      512 2023-05-23 00:42:37.000000 edman_cli-2023.5.23/edman_cli.egg-info/entry_points.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)       71 2023-05-23 00:42:37.000000 edman_cli-2023.5.23/edman_cli.egg-info/requires.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)       36 2023-05-23 00:42:37.000000 edman_cli-2023.5.23/edman_cli.egg-info/top_level.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1468 2023-05-23 00:41:39.000000 edman_cli-2023.5.23/pyproject.toml
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-23 00:42:37.120031 edman_cli-2023.5.23/scripts/
--rw-r--r--   0 ohno      (1000) ohno      (1000)    16460 2023-05-12 07:08:01.000000 edman_cli-2023.5.23/scripts/action.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2229 2022-03-23 07:12:34.000000 edman_cli-2023.5.23/scripts/assign_bson_type.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     3510 2022-11-21 07:40:05.000000 edman_cli-2023.5.23/scripts/db_create.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2722 2022-11-21 07:40:05.000000 edman_cli-2023.5.23/scripts/db_destroy.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1573 2022-02-03 08:34:28.000000 edman_cli-2023.5.23/scripts/delete.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2557 2022-02-03 08:34:28.000000 edman_cli-2023.5.23/scripts/entry.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2328 2023-05-12 07:08:01.000000 edman_cli-2023.5.23/scripts/file_add.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2947 2022-02-03 08:34:28.000000 edman_cli-2023.5.23/scripts/file_delete.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2513 2023-05-12 07:08:01.000000 edman_cli-2023.5.23/scripts/file_dl.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2374 2022-04-13 08:48:24.000000 edman_cli-2023.5.23/scripts/find.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2628 2022-02-03 08:34:28.000000 edman_cli-2023.5.23/scripts/item_delete.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1907 2022-02-03 08:34:28.000000 edman_cli-2023.5.23/scripts/pullout.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2403 2022-02-03 08:34:28.000000 edman_cli-2023.5.23/scripts/structure_convert.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2096 2022-02-03 08:34:28.000000 edman_cli-2023.5.23/scripts/update.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)       38 2023-05-23 00:42:37.130031 edman_cli-2023.5.23/setup.cfg
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-23 00:42:37.120031 edman_cli-2023.5.23/tests/
--rw-r--r--   0 ohno      (1000) ohno      (1000)    10946 2022-11-21 07:40:05.000000 edman_cli-2023.5.23/tests/test_action.py
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-23 00:42:37.120031 edman_cli-2023.5.23/venv/
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-23 00:42:37.130031 edman_cli-2023.5.23/venv/bin/
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)     1729 2023-04-07 00:41:13.000000 edman_cli-2023.5.23/venv/bin/jp.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      636 2023-05-18 02:30:36.000000 edman_cli-2023.5.23/venv/bin/rst2html.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      758 2023-05-18 02:30:36.000000 edman_cli-2023.5.23/venv/bin/rst2html4.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)     1093 2023-05-18 02:30:36.000000 edman_cli-2023.5.23/venv/bin/rst2html5.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      835 2023-05-18 02:30:36.000000 edman_cli-2023.5.23/venv/bin/rst2latex.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      658 2023-05-18 02:30:36.000000 edman_cli-2023.5.23/venv/bin/rst2man.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      824 2023-05-18 02:30:36.000000 edman_cli-2023.5.23/venv/bin/rst2odt.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      630 2023-05-18 02:30:36.000000 edman_cli-2023.5.23/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      643 2023-05-18 02:30:36.000000 edman_cli-2023.5.23/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      679 2023-05-18 02:30:36.000000 edman_cli-2023.5.23/venv/bin/rst2s5.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      915 2023-05-18 02:30:36.000000 edman_cli-2023.5.23/venv/bin/rst2xetex.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      644 2023-05-18 02:30:36.000000 edman_cli-2023.5.23/venv/bin/rst2xml.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      712 2023-05-18 02:30:36.000000 edman_cli-2023.5.23/venv/bin/rstpep2html.py
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-23 00:42:37.120031 edman_cli-2023.5.23/venv/src/
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-23 00:42:37.130031 edman_cli-2023.5.23/venv/src/edman-cli/
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-23 00:42:37.130031 edman_cli-2023.5.23/venv/src/edman-cli/scripts/
--rw-r--r--   0 ohno      (1000) ohno      (1000)    16618 2023-04-07 00:41:06.000000 edman_cli-2023.5.23/venv/src/edman-cli/scripts/action.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2287 2023-04-07 00:41:06.000000 edman_cli-2023.5.23/venv/src/edman-cli/scripts/assign_bson_type.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     3510 2023-04-07 00:41:06.000000 edman_cli-2023.5.23/venv/src/edman-cli/scripts/db_create.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2722 2023-04-07 00:41:06.000000 edman_cli-2023.5.23/venv/src/edman-cli/scripts/db_destroy.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1618 2023-04-07 00:41:06.000000 edman_cli-2023.5.23/venv/src/edman-cli/scripts/delete.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2624 2023-04-07 00:41:06.000000 edman_cli-2023.5.23/venv/src/edman-cli/scripts/entry.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2266 2023-04-07 00:41:06.000000 edman_cli-2023.5.23/venv/src/edman-cli/scripts/file_add.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     3027 2023-04-07 00:41:06.000000 edman_cli-2023.5.23/venv/src/edman-cli/scripts/file_delete.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     3177 2023-04-07 00:41:06.000000 edman_cli-2023.5.23/venv/src/edman-cli/scripts/file_dl.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2374 2023-04-07 00:41:06.000000 edman_cli-2023.5.23/venv/src/edman-cli/scripts/find.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2702 2023-04-07 00:41:06.000000 edman_cli-2023.5.23/venv/src/edman-cli/scripts/item_delete.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1960 2023-04-07 00:41:06.000000 edman_cli-2023.5.23/venv/src/edman-cli/scripts/pullout.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2462 2023-04-07 00:41:06.000000 edman_cli-2023.5.23/venv/src/edman-cli/scripts/structure_convert.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2156 2023-04-07 00:41:06.000000 edman_cli-2023.5.23/venv/src/edman-cli/scripts/update.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)      855 2023-04-07 00:41:06.000000 edman_cli-2023.5.23/venv/src/edman-cli/setup.py
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-23 00:42:37.130031 edman_cli-2023.5.23/venv/src/edman-cli/tests/
--rw-r--r--   0 ohno      (1000) ohno      (1000)        0 2023-04-07 00:41:06.000000 edman_cli-2023.5.23/venv/src/edman-cli/tests/__init__.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)    10946 2023-04-07 00:41:06.000000 edman_cli-2023.5.23/venv/src/edman-cli/tests/test_action.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-24 05:54:16.364302 edman_cli-2023.5.24/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1100 2023-03-15 06:38:21.000000 edman_cli-2023.5.24/LICENSE.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     4934 2023-05-24 05:54:16.364302 edman_cli-2023.5.24/PKG-INFO
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     3345 2023-01-20 03:57:51.000000 edman_cli-2023.5.24/README.rst
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-24 05:54:16.364302 edman_cli-2023.5.24/edman_cli.egg-info/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     4934 2023-05-24 05:54:16.000000 edman_cli-2023.5.24/edman_cli.egg-info/PKG-INFO
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1515 2023-05-24 05:54:16.000000 edman_cli-2023.5.24/edman_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)        1 2023-05-24 05:54:16.000000 edman_cli-2023.5.24/edman_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      512 2023-05-24 05:54:16.000000 edman_cli-2023.5.24/edman_cli.egg-info/entry_points.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       71 2023-05-24 05:54:16.000000 edman_cli-2023.5.24/edman_cli.egg-info/requires.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       36 2023-05-24 05:54:16.000000 edman_cli-2023.5.24/edman_cli.egg-info/top_level.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1468 2023-05-24 05:52:45.000000 edman_cli-2023.5.24/pyproject.toml
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-24 05:54:16.364302 edman_cli-2023.5.24/scripts/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)        0 2023-05-24 05:52:45.000000 edman_cli-2023.5.24/scripts/__init__.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    16621 2023-05-24 05:52:45.000000 edman_cli-2023.5.24/scripts/action.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2305 2023-05-24 05:52:45.000000 edman_cli-2023.5.24/scripts/assign_bson_type.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     3523 2023-05-24 05:52:45.000000 edman_cli-2023.5.24/scripts/db_create.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2757 2023-05-24 05:52:45.000000 edman_cli-2023.5.24/scripts/db_destroy.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1626 2023-05-24 05:52:45.000000 edman_cli-2023.5.24/scripts/delete.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2666 2023-05-24 05:52:45.000000 edman_cli-2023.5.24/scripts/entry.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2332 2023-05-24 05:52:45.000000 edman_cli-2023.5.24/scripts/file_add.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     3033 2023-05-24 05:52:45.000000 edman_cli-2023.5.24/scripts/file_delete.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2519 2023-05-24 05:52:45.000000 edman_cli-2023.5.24/scripts/file_dl.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2406 2023-05-24 05:52:45.000000 edman_cli-2023.5.24/scripts/find.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2708 2023-05-24 05:52:45.000000 edman_cli-2023.5.24/scripts/item_delete.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2166 2023-05-24 05:52:45.000000 edman_cli-2023.5.24/scripts/pullout.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2492 2023-05-24 05:52:45.000000 edman_cli-2023.5.24/scripts/structure_convert.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2163 2023-05-24 05:52:45.000000 edman_cli-2023.5.24/scripts/update.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       38 2023-05-24 05:54:16.364302 edman_cli-2023.5.24/setup.cfg
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-24 05:54:16.364302 edman_cli-2023.5.24/tests/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    10960 2023-05-24 05:52:45.000000 edman_cli-2023.5.24/tests/test_action.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-24 05:54:16.364302 edman_cli-2023.5.24/venv/
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-24 05:54:16.364302 edman_cli-2023.5.24/venv/bin/
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)     1729 2023-04-07 00:41:13.000000 edman_cli-2023.5.24/venv/bin/jp.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      636 2023-05-18 02:30:36.000000 edman_cli-2023.5.24/venv/bin/rst2html.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      758 2023-05-18 02:30:36.000000 edman_cli-2023.5.24/venv/bin/rst2html4.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)     1093 2023-05-18 02:30:36.000000 edman_cli-2023.5.24/venv/bin/rst2html5.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      835 2023-05-18 02:30:36.000000 edman_cli-2023.5.24/venv/bin/rst2latex.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      658 2023-05-18 02:30:36.000000 edman_cli-2023.5.24/venv/bin/rst2man.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      824 2023-05-18 02:30:36.000000 edman_cli-2023.5.24/venv/bin/rst2odt.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      630 2023-05-18 02:30:36.000000 edman_cli-2023.5.24/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      643 2023-05-18 02:30:36.000000 edman_cli-2023.5.24/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      679 2023-05-18 02:30:36.000000 edman_cli-2023.5.24/venv/bin/rst2s5.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      915 2023-05-18 02:30:36.000000 edman_cli-2023.5.24/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      644 2023-05-18 02:30:36.000000 edman_cli-2023.5.24/venv/bin/rst2xml.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      712 2023-05-18 02:30:36.000000 edman_cli-2023.5.24/venv/bin/rstpep2html.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-24 05:54:16.364302 edman_cli-2023.5.24/venv/src/
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-24 05:54:16.364302 edman_cli-2023.5.24/venv/src/edman-cli/
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-24 05:54:16.364302 edman_cli-2023.5.24/venv/src/edman-cli/scripts/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    16618 2023-04-07 00:41:06.000000 edman_cli-2023.5.24/venv/src/edman-cli/scripts/action.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2287 2023-04-07 00:41:06.000000 edman_cli-2023.5.24/venv/src/edman-cli/scripts/assign_bson_type.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     3510 2023-04-07 00:41:06.000000 edman_cli-2023.5.24/venv/src/edman-cli/scripts/db_create.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2722 2023-04-07 00:41:06.000000 edman_cli-2023.5.24/venv/src/edman-cli/scripts/db_destroy.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1618 2023-04-07 00:41:06.000000 edman_cli-2023.5.24/venv/src/edman-cli/scripts/delete.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2624 2023-04-07 00:41:06.000000 edman_cli-2023.5.24/venv/src/edman-cli/scripts/entry.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2266 2023-04-07 00:41:06.000000 edman_cli-2023.5.24/venv/src/edman-cli/scripts/file_add.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     3027 2023-04-07 00:41:06.000000 edman_cli-2023.5.24/venv/src/edman-cli/scripts/file_delete.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     3177 2023-04-07 00:41:06.000000 edman_cli-2023.5.24/venv/src/edman-cli/scripts/file_dl.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2374 2023-04-07 00:41:06.000000 edman_cli-2023.5.24/venv/src/edman-cli/scripts/find.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2702 2023-04-07 00:41:06.000000 edman_cli-2023.5.24/venv/src/edman-cli/scripts/item_delete.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1960 2023-04-07 00:41:06.000000 edman_cli-2023.5.24/venv/src/edman-cli/scripts/pullout.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2462 2023-04-07 00:41:06.000000 edman_cli-2023.5.24/venv/src/edman-cli/scripts/structure_convert.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2156 2023-04-07 00:41:06.000000 edman_cli-2023.5.24/venv/src/edman-cli/scripts/update.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      855 2023-04-07 00:41:06.000000 edman_cli-2023.5.24/venv/src/edman-cli/setup.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-24 05:54:16.364302 edman_cli-2023.5.24/venv/src/edman-cli/tests/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)        0 2023-04-07 00:41:06.000000 edman_cli-2023.5.24/venv/src/edman-cli/tests/__init__.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    10946 2023-04-07 00:41:06.000000 edman_cli-2023.5.24/venv/src/edman-cli/tests/test_action.py
```

### Comparing `edman_cli-2023.5.23/LICENSE.txt` & `edman_cli-2023.5.24/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.23/PKG-INFO` & `edman_cli-2023.5.24/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edman_cli
-Version: 2023.5.23
+Version: 2023.5.24
 Summary: Sub-package of edman for cli applications and scripts.
 Author-email: Masaki Ohno <masakio@post.kek.jp>
 License: MIT License
         
         Copyright (c) 2019-2023 KEK IMSS SBRC/PF, Masaki Ohno
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `edman_cli-2023.5.23/README.rst` & `edman_cli-2023.5.24/README.rst`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.23/edman_cli.egg-info/PKG-INFO` & `edman_cli-2023.5.24/edman_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edman-cli
-Version: 2023.5.23
+Version: 2023.5.24
 Summary: Sub-package of edman for cli applications and scripts.
 Author-email: Masaki Ohno <masakio@post.kek.jp>
 License: MIT License
         
         Copyright (c) 2019-2023 KEK IMSS SBRC/PF, Masaki Ohno
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `edman_cli-2023.5.23/edman_cli.egg-info/SOURCES.txt` & `edman_cli-2023.5.24/edman_cli.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 pyproject.toml
 edman_cli.egg-info/PKG-INFO
 edman_cli.egg-info/SOURCES.txt
 edman_cli.egg-info/dependency_links.txt
 edman_cli.egg-info/entry_points.txt
 edman_cli.egg-info/requires.txt
 edman_cli.egg-info/top_level.txt
+scripts/__init__.py
 scripts/action.py
 scripts/assign_bson_type.py
 scripts/db_create.py
 scripts/db_destroy.py
 scripts/delete.py
 scripts/entry.py
 scripts/file_add.py
```

### Comparing `edman_cli-2023.5.23/edman_cli.egg-info/entry_points.txt` & `edman_cli-2023.5.24/edman_cli.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.23/pyproject.toml` & `edman_cli-2023.5.24/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -17,17 +17,17 @@
     "License :: OSI Approved :: MIT License",
     "Topic :: Database :: Front-Ends",
 ]
 dependencies = [
     "pymongo~=4.3.3",
     " python-dateutil~=2.8.2",
     "jmespath~=1.0.1",
-    "edman~=2023.5.23",
+    "edman~=2023.5.24",
 ]
-version = "2023.5.23"
+version = "2023.5.24"
 
 [project.urls]
 "repository" = "https://github.com/ryde/edman_cli"
 
 [tool.setuptools.packages.find]
 exclude = ["tests"]
```

### Comparing `edman_cli-2023.5.23/scripts/action.py` & `edman_cli-2023.5.24/venv/src/edman-cli/scripts/action.py`

 * *Files 1% similar despite different names*

```diff
@@ -438,14 +438,15 @@
         パス文字列からパスオブジェクト生成
         パス文字列がなければデフォルトのiniディレクトリパスを返す
 
         :param str or None filepath:
         :return: result
         :rtype: Path
         """
+
         if filepath is not None:
             p = Path(filepath)
             if p.exists():
                 result = p
             else:
                 sys.exit(f'{filepath}は存在しません')
         else:
@@ -460,10 +461,17 @@
 
         :param str or None input_file:
         :return:
         :rtype: dict
         """
         settings = configparser.ConfigParser()
         settings.read(Action.generate_config_path(input_file))
-        result = {k: json.loads(v) if k == 'options' else v for k, v in
-                  settings['DB'].items()}
+
+        result = {}
+        for k, v in settings['DB'].items():
+            if k == 'options':
+                s = json.loads(v)
+            else:
+                s = v
+            result.update({k: s})
         return result
+        # return dict([i for i in settings['DB'].items()])
```

### Comparing `edman_cli-2023.5.23/scripts/assign_bson_type.py` & `edman_cli-2023.5.24/scripts/assign_bson_type.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,59 +1,63 @@
-def main():
-    import sys
-    import signal
-    import argparse
-    from pathlib import Path
-    from edman import DB, JsonManager
-    from scripts.action import Action
-
-    # Ctrl-Cを押下された時の対策
-    signal.signal(signal.SIGINT, lambda sig, frame: sys.exit('\n'))
-
-    # コマンドライン引数処理
-    parser = argparse.ArgumentParser(description='DB内のRefドキュメントに型を適応するスクリプト')
-    parser.add_argument('path', help='JSON file path.')
-    parser.add_argument('-l', '--logfile',
-                        help='Output logfile path. default is current dir.')
-    parser.add_argument('-n', '--no_logfile', help='Do not output log file.',
-                        action='store_true')
-    parser.add_argument('-i', '--inifile', help='DB connect file path.')
-
-    # 引数を付けなかった場合はヘルプを表示して終了する
-    if len(sys.argv) == 1:
-        parser.parse_args(["-h"])
-        sys.exit(0)
-    args = parser.parse_args()
-
-    # 結果を記録する場合はパスの存在を調べる
-    log_p = Path(args.logfile) if args.logfile is not None else Path.cwd()
-    if not log_p.exists() or not log_p.is_dir():
-        sys.exit('指定のログファイル用ディレクトリパスが不正です')
-
-    # JSONのパスを取得
-    p = Path(args.path)
-    if not p.exists() or not p.is_file() or p.suffix != '.json':
-        sys.exit('指定のJSONファイルがありません')
-
-    try:
-        # 接続用iniファイル読み込み
-        con = Action.reading_config_file(args.inifile)
-        db = DB(con)
-        process_data = {}
-
-        # ファイル読み込み、実行
-        # ファイル単体の場合でもジェネレータなのでループを使用する
-        for i in Action.file_gen((p,)):
-            process_data = db.bson_type(i)
-
-        # ログファイル書き出し処理
-        if not args.no_logfile:
-            jm = JsonManager()
-            jm.save(process_data, log_p, name='type_assigned_log', date=True)
-
-    except Exception as e:
-        tb = sys.exc_info()[2]
-        sys.stderr.write(f'{type(e).__name__}: {e.with_traceback(tb)}\n')
-        sys.exit(1)
-
-if __name__ == "__main__":
-    main()
+def main():
+    import argparse
+    import signal
+    import sys
+    from pathlib import Path
+
+    from edman import DB, JsonManager
+
+    from scripts.action import Action
+
+    # Ctrl-Cを押下された時の対策
+    signal.signal(signal.SIGINT, lambda sig, frame: sys.exit('\n'))
+
+    # コマンドライン引数処理
+    parser = argparse.ArgumentParser(
+        description='DB内のRefドキュメントに型を適応するスクリプト')
+    parser.add_argument('path', help='JSON file path.')
+    parser.add_argument('-l', '--logfile',
+                        help='Output logfile path. default is current dir.')
+    parser.add_argument('-n', '--no_logfile', help='Do not output log file.',
+                        action='store_true')
+    parser.add_argument('-i', '--inifile', help='DB connect file path.')
+
+    # 引数を付けなかった場合はヘルプを表示して終了する
+    if len(sys.argv) == 1:
+        parser.parse_args(["-h"])
+        sys.exit(0)
+    args = parser.parse_args()
+
+    # 結果を記録する場合はパスの存在を調べる
+    log_p = Path(args.logfile) if args.logfile is not None else Path.cwd()
+    if not log_p.exists() or not log_p.is_dir():
+        sys.exit('指定のログファイル用ディレクトリパスが不正です')
+
+    # JSONのパスを取得
+    p = Path(args.path)
+    if not p.exists() or not p.is_file() or p.suffix != '.json':
+        sys.exit('指定のJSONファイルがありません')
+
+    try:
+        # 接続用iniファイル読み込み
+        con = Action.reading_config_file(args.inifile)
+        db = DB(con)
+        process_data = {}
+
+        # ファイル読み込み、実行
+        # ファイル単体の場合でもジェネレータなのでループを使用する
+        for i in Action.file_gen((p,)):
+            process_data = db.bson_type(i)
+
+        # ログファイル書き出し処理
+        if not args.no_logfile:
+            jm = JsonManager()
+            jm.save(process_data, log_p, name='type_assigned_log', date=True)
+
+    except Exception as e:
+        tb = sys.exc_info()[2]
+        sys.stderr.write(f'{type(e).__name__}: {e.with_traceback(tb)}\n')
+        sys.exit(1)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `edman_cli-2023.5.23/scripts/db_create.py` & `edman_cli-2023.5.24/venv/src/edman-cli/scripts/db_create.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.23/scripts/db_destroy.py` & `edman_cli-2023.5.24/venv/src/edman-cli/scripts/db_destroy.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.23/scripts/delete.py` & `edman_cli-2023.5.24/scripts/delete.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,46 +1,49 @@
-def main():
-    import sys
-    import signal
-    import argparse
-    from edman import DB
-    from scripts.action import Action
-
-    # Ctrl-Cを押下された時の対策
-    signal.signal(signal.SIGINT, lambda sig, frame: sys.exit('\n'))
-
-    # コマンドライン引数処理
-    parser = argparse.ArgumentParser(description='ドキュメントを削除するスクリプト')
-    # parser.add_argument('-c', '--collection', help='collection name.')
-    parser.add_argument('objectid', help='objectid str.')
-    parser.add_argument('-i', '--inifile', help='DB connect file path.')
-
-    # 引数を付けなかった場合はヘルプを表示して終了する
-    if len(sys.argv) == 1:
-        parser.parse_args(["-h"])
-        sys.exit(0)
-    args = parser.parse_args()
-
-    try:
-        # iniファイル読み込み
-        con = Action.reading_config_file(args.inifile)
-
-        db = DB(con)
-        # 対象oidの所属コレクションを自動的に取得 ※動作が遅い場合は使用しないこと
-        collection = db.find_collection_from_objectid(args.objectid)
-
-        # 指定のドキュメントの文書構造を取得
-        structure = db.get_structure(collection, args.objectid)
-
-        # 削除処理
-        if db.delete(args.objectid, collection, structure):
-            print('削除成功')
-        else:
-            print('削除失敗')
-
-    except Exception as e:
-        tb = sys.exc_info()[2]
-        sys.stderr.write(f'{type(e).__name__}: {e.with_traceback(tb)}\n')
-        sys.exit(1)
-
-if __name__ == "__main__":
-    main()
+def main():
+    import argparse
+    import signal
+    import sys
+
+    from edman import DB
+
+    from scripts.action import Action
+
+    # Ctrl-Cを押下された時の対策
+    signal.signal(signal.SIGINT, lambda sig, frame: sys.exit('\n'))
+
+    # コマンドライン引数処理
+    parser = argparse.ArgumentParser(description='ドキュメントを削除するスクリプト')
+    # parser.add_argument('-c', '--collection', help='collection name.')
+    parser.add_argument('objectid', help='objectid str.')
+    parser.add_argument('-i', '--inifile', help='DB connect file path.')
+
+    # 引数を付けなかった場合はヘルプを表示して終了する
+    if len(sys.argv) == 1:
+        parser.parse_args(["-h"])
+        sys.exit(0)
+    args = parser.parse_args()
+
+    try:
+        # iniファイル読み込み
+        con = Action.reading_config_file(args.inifile)
+
+        db = DB(con)
+        # 対象oidの所属コレクションを自動的に取得 ※動作が遅い場合は使用しないこと
+        collection = db.find_collection_from_objectid(args.objectid)
+
+        # 指定のドキュメントの文書構造を取得
+        structure = db.get_structure(collection, args.objectid)
+
+        # 削除処理
+        if db.delete(args.objectid, collection, structure):
+            print('削除成功')
+        else:
+            print('削除失敗')
+
+    except Exception as e:
+        tb = sys.exc_info()[2]
+        sys.stderr.write(f'{type(e).__name__}: {e.with_traceback(tb)}\n')
+        sys.exit(1)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `edman_cli-2023.5.23/scripts/entry.py` & `edman_cli-2023.5.24/scripts/entry.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,68 +1,71 @@
-def main():
-
-    import sys
-    import signal
-    import argparse
-    from pathlib import Path
-    from edman import DB, Convert, JsonManager
-    from scripts.action import Action
-
-    # Ctrl-Cを押下された時の対策
-    signal.signal(signal.SIGINT, lambda sig, frame: sys.exit('\n'))
-
-    # コマンドライン引数処理
-    parser = argparse.ArgumentParser(description='JSONからDBに投入するスクリプト')
-    parser.add_argument('path', help='file or Dir path.')
-    parser.add_argument('-rd', '--result_dir',
-                        help='Dir of report files. default is current dir.',
-                        default=None)
-    parser.add_argument('-s', '--structure', default='ref',
-                        help='Select ref(Reference, default) or emb(embedded).')
-    parser.add_argument('-i', '--inifile', help='DB connect file path.')
-
-    # 引数を付けなかった場合はヘルプを表示して終了する
-    if len(sys.argv) == 1:
-        parser.parse_args(["-h"])
-        sys.exit(0)
-    args = parser.parse_args()
-
-    # 構造はrefかembのどちらか ※モジュール内でも判断できる
-    if not (args.structure == 'ref' or args.structure == 'emb'):
-        parser.error("--structure requires 'ref' or 'emb'.")
-
-    # 結果を記録する場合はパスの存在を調べる
-    if args.result_dir is not None:
-        p = Path(args.result_dir)
-        if not p.exists() and not p.is_dir():
-            sys.exit('パスが不正です')
-
-    try:
-        # iniファイル読み込み
-        con = Action.reading_config_file(args.inifile)
-
-        db = DB(con)
-        jm = JsonManager()
-        convert = Convert()
-        json_files = Action.files_read(args.path, 'json')
-
-        for file in Action.file_gen(json_files):
-            # Edman用にjsonをコンバート
-            converted_edman = convert.dict_to_edman(file, mode=args.structure)
-            # コンバート結果を保存する場合
-            # jm.save({'converted_edman': converted_edman}, args.result_dir,
-            #         name='edman_json_list', date=True)
-
-            # DBへインサート
-            inserted_report = db.insert(converted_edman)
-
-            if args.result_dir is not None:
-                jm.save({'inserted_report': inserted_report}, args.result_dir,
-                        name='inserted', date=True)
-
-    except Exception as e:
-        tb = sys.exc_info()[2]
-        sys.stderr.write(f'{type(e).__name__}: {e.with_traceback(tb)}\n')
-        sys.exit(1)
-
-if __name__ == "__main__":
-    main()
+def main():
+    import argparse
+    import signal
+    import sys
+    from pathlib import Path
+
+    from edman import DB, Convert, JsonManager
+
+    from scripts.action import Action
+
+    # Ctrl-Cを押下された時の対策
+    signal.signal(signal.SIGINT, lambda sig, frame: sys.exit('\n'))
+
+    # コマンドライン引数処理
+    parser = argparse.ArgumentParser(description='JSONからDBに投入するスクリプト')
+    parser.add_argument('path', help='file or Dir path.')
+    parser.add_argument('-rd', '--result_dir',
+                        help='Dir of report files. default is current dir.',
+                        default=None)
+    parser.add_argument('-s', '--structure', default='ref',
+                        help=('Select ref(Reference, default) '
+                              'or emb(embedded).'))
+    parser.add_argument('-i', '--inifile', help='DB connect file path.')
+
+    # 引数を付けなかった場合はヘルプを表示して終了する
+    if len(sys.argv) == 1:
+        parser.parse_args(["-h"])
+        sys.exit(0)
+    args = parser.parse_args()
+
+    # 構造はrefかembのどちらか ※モジュール内でも判断できる
+    if not (args.structure == 'ref' or args.structure == 'emb'):
+        parser.error("--structure requires 'ref' or 'emb'.")
+
+    # 結果を記録する場合はパスの存在を調べる
+    if args.result_dir is not None:
+        p = Path(args.result_dir)
+        if not p.exists() and not p.is_dir():
+            sys.exit('パスが不正です')
+
+    try:
+        # iniファイル読み込み
+        con = Action.reading_config_file(args.inifile)
+
+        db = DB(con)
+        jm = JsonManager()
+        convert = Convert()
+        json_files = Action.files_read(args.path, 'json')
+
+        for file in Action.file_gen(json_files):
+            # Edman用にjsonをコンバート
+            converted_edman = convert.dict_to_edman(file, mode=args.structure)
+            # コンバート結果を保存する場合
+            # jm.save({'converted_edman': converted_edman}, args.result_dir,
+            #         name='edman_json_list', date=True)
+
+            # DBへインサート
+            inserted_report = db.insert(converted_edman)
+
+            if args.result_dir is not None:
+                jm.save({'inserted_report': inserted_report}, args.result_dir,
+                        name='inserted', date=True)
+
+    except Exception as e:
+        tb = sys.exc_info()[2]
+        sys.stderr.write(f'{type(e).__name__}: {e.with_traceback(tb)}\n')
+        sys.exit(1)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `edman_cli-2023.5.23/scripts/file_add.py` & `edman_cli-2023.5.24/scripts/file_add.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 def main():
-    import sys
-    import signal
     import argparse
+    import signal
+    import sys
+
     from edman import DB, File
+
     from scripts.action import Action
 
     # Ctrl-Cを押下された時の対策
     signal.signal(signal.SIGINT, lambda sig, frame: sys.exit('\n'))
 
     # コマンドライン引数処理
     parser = argparse.ArgumentParser(description='ファイルを実験データに追加するスクリプト')
```

### Comparing `edman_cli-2023.5.23/scripts/file_delete.py` & `edman_cli-2023.5.24/venv/src/edman-cli/scripts/file_dl.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,81 +1,82 @@
-def main():
-
-    import sys
-    import signal
-    import argparse
-    from edman import DB, File
-    from scripts.action import Action
-
-    # Ctrl-Cを押下された時の対策
-    signal.signal(signal.SIGINT, lambda sig, frame: sys.exit('\n'))
-
-    # コマンドライン引数処理
-    parser = argparse.ArgumentParser(
-        description='ファイルを実験データから削除するスクリプト')
-    # parser.add_argument('-c', '--collection', help='collection name.')
-    parser.add_argument('objectid', help='objectid str.')
-    # クエリは structureがembの時だけ
-    parser.add_argument('-q', '--query', default=None,
-                        help='Ref is ObjectId or Emb is query list strings.')
-    parser.add_argument('-i', '--inifile', help='DB connect file path.')
-
-    # 引数を付けなかった場合はヘルプを表示して終了する
-    if len(sys.argv) == 1:
-        parser.parse_args(["-h"])
-        sys.exit(0)
-    args = parser.parse_args()
-
-    try:
-        # iniファイル読み込み
-        con = Action.reading_config_file(args.inifile)
-
-        db = DB(con)
-        file = File(db.get_db)
-
-        # 対象oidの所属コレクションを自動的に取得 ※動作が遅い場合は使用しないこと
-        collection = db.find_collection_from_objectid(args.objectid)
-
-        # ドキュメント構造の取得
-        structure = db.get_structure(collection, args.objectid)
-
-        # クエリの変換
-        query = Action.file_query_eval(args.query, structure)
-
-        # ファイル名一覧を取得
-        file_names = file.get_file_names(collection, args.objectid, structure,
-                                         query)
-        if not file_names:
-            sys.exit('ファイルは存在しません')
-
-        file_oids = []
-        # ファイル名一覧を画面表示&file_oid用リスト作成
-        for idx, (oid, filename) in enumerate(file_names.items()):
-            print('(' + str(idx) + ')', filename, oid)
-            file_oids.append(oid)
-
-        # 表示されている選択番号を入力
-        if len(file_names) > 0:
-            while True:
-                selected_idx = input('0 - ' + str(len(file_names) - 1) + ' > ')
-                if selected_idx.isdecimal() and (
-                        0 <= int(selected_idx) < len(file_names)):
-                    break
-                else:
-                    print('Required!')
-        else:
-            sys.exit('インデックスが不正です')
-
-        # 該当するファイルを削除
-        if file.delete(file_oids[int(selected_idx)], collection, args.objectid,
-                       structure, query):
-            print('削除完了')
-        else:
-            print('削除失敗')
-
-    except Exception as e:
-        tb = sys.exc_info()[2]
-        sys.stderr.write(f'{type(e).__name__}: {e.with_traceback(tb)}\n')
-        sys.exit(1)
-
-if __name__ == "__main__":
+def main():
+
+    import sys
+    import signal
+    import argparse
+    from edman import DB, File
+    from scripts.action import Action
+
+    # Ctrl-Cを押下された時の対策
+    signal.signal(signal.SIGINT, lambda sig, frame: sys.exit('\n'))
+
+    # コマンドライン引数処理
+    parser = argparse.ArgumentParser(
+        description='ファイルを実験データからダウンロードするスクリプト')
+    # parser.add_argument('-c', '--collection', help='collection name.')
+    parser.add_argument('objectid', help='objectid str.')
+    parser.add_argument('path', help='Download Dir path.')
+    # クエリは structureがembの時だけ
+    parser.add_argument('-q', '--query', default=None,
+                        help='Ref is ObjectId or Emb is query list strings.')
+    parser.add_argument('-i', '--inifile', help='DB connect file path.')
+
+    # 引数を付けなかった場合はヘルプを表示して終了する
+    if len(sys.argv) == 1:
+        parser.parse_args(["-h"])
+        sys.exit(0)
+    args = parser.parse_args()
+
+    try:
+        # iniファイル読み込み
+        con = Action.reading_config_file(args.inifile)
+
+        db = DB(con)
+        file = File(db.get_db)
+
+        # 対象oidの所属コレクションを自動的に取得 ※動作が遅い場合は使用しないこと
+        collection = db.find_collection_from_objectid(args.objectid)
+
+        # ドキュメント構造の取得
+        structure = db.get_structure(collection, args.objectid)
+
+        # クエリの変換
+        query = Action.file_query_eval(args.query, structure)
+
+        # ファイル名一覧を取得
+        file_names = file.get_file_names(collection, args.objectid, structure,
+                                         query)
+        if not file_names:
+            sys.exit('ファイルは存在しません')
+
+        file_oids = []
+        # ファイル名一覧を画面表示&file_oid用リスト作成
+        for idx, (oid, filename) in enumerate(file_names.items()):
+            print('(' + str(idx) + ')', filename, oid)
+            file_oids.append(oid)
+
+        # 複数ファイルの場合、表示されている選択番号を入力
+        if len(file_names) > 1:
+            while True:
+                selected_idx = input('0 - ' + str(len(file_names) - 1) + ' > ')
+                if selected_idx.isdecimal() and (
+                        0 <= int(selected_idx) < len(file_names)):
+                    break
+                else:
+                    print('Required!')
+        # ファイルが一つしかない場合は選択無しでDL
+        elif len(file_names) == 1:
+            selected_idx = 0
+        else:
+            sys.exit('インデックスが不正です')
+
+        # 指定のディレクトリにダウンロード
+        if file.download(file_oids[int(selected_idx)], args.path):
+            print('DLしました')
+
+    except Exception as e:
+        tb = sys.exc_info()[2]
+        sys.stderr.write(f'{type(e).__name__}: {e.with_traceback(tb)}\n')
+        sys.exit(1)
+
+if __name__ == "__main__":
     main()
```

### Comparing `edman_cli-2023.5.23/scripts/file_dl.py` & `edman_cli-2023.5.24/scripts/file_dl.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 def main():
-
-    import sys
-    import signal
     import argparse
+    import signal
+    import sys
+
     from edman import DB, File
+
     from scripts.action import Action
 
     # Ctrl-Cを押下された時の対策
     signal.signal(signal.SIGINT, lambda sig, frame: sys.exit('\n'))
 
     # コマンドライン引数処理
     parser = argparse.ArgumentParser(
@@ -59,9 +60,10 @@
             print('DLしました')
 
     except Exception as e:
         tb = sys.exc_info()[2]
         sys.stderr.write(f'{type(e).__name__}: {e.with_traceback(tb)}\n')
         sys.exit(1)
 
+
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `edman_cli-2023.5.23/scripts/find.py` & `edman_cli-2023.5.24/venv/src/edman-cli/scripts/find.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.23/scripts/item_delete.py` & `edman_cli-2023.5.24/venv/src/edman-cli/scripts/item_delete.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-def main():
-
-    import sys
-    import signal
-    import argparse
-    from edman import DB
-    from scripts.action import Action
-
-    # Ctrl-Cを押下された時の対策
-    signal.signal(signal.SIGINT, lambda sig, frame: sys.exit('\n'))
-
-    # コマンドライン引数処理
-    parser = argparse.ArgumentParser(description='ドキュメントの項目を削除するスクリプト')
-    # parser.add_argument('-c', '--collection', help='collection name.')
-    parser.add_argument('objectid', help='objectid str.')
-    # クエリは structureがembの時だけ
-    parser.add_argument('-q', '--query', default=None,
-                        help='Ref is ObjectId or Emb is query list strings.')
-    parser.add_argument('-i', '--inifile', help='DB connect file path.')
-
-    # 引数を付けなかった場合はヘルプを表示して終了する
-    if len(sys.argv) == 1:
-        parser.parse_args(["-h"])
-        sys.exit(0)
-    args = parser.parse_args()
-
-    try:
-        # iniファイル読み込み
-        con = Action.reading_config_file(args.inifile)
-
-        db = DB(con)
-
-        # 対象oidの所属コレクションを自動的に取得 ※動作が遅い場合は使用しないこと
-        collection = db.find_collection_from_objectid(args.objectid)
-
-        # ドキュメント構造の取得
-        structure = db.get_structure(collection, args.objectid)
-
-        # クエリの変換
-        query = Action.file_query_eval(args.query, structure)
-
-        # ドキュメント取得
-        doc = db.doc(collection, args.objectid, query)
-        doc_keys = list(doc.keys())
-
-        # 項目を画面表示
-        for idx, (key, value) in enumerate(doc.items()):
-            print('(' + str(idx) + ')', key, ':', value)
-
-        # 表示されている選択番号を入力
-        if len(doc) > 0:
-            while True:
-                selected_idx = input('0 - ' + str(len(doc) - 1) + ' > ')
-                if selected_idx.isdecimal() and (
-                        0 <= int(selected_idx) < len(doc)):
-                    break
-                else:
-                    print('Required!')
-        else:
-            sys.exit('ドキュメントが取得できていません')
-
-        # 削除処理
-        if db.item_delete(collection, args.objectid,
-                          doc_keys[int(selected_idx)], query):
-            print('削除成功')
-        else:
-            print('削除失敗')
-
-    except Exception as e:
-        tb = sys.exc_info()[2]
-        sys.stderr.write(f'{type(e).__name__}: {e.with_traceback(tb)}\n')
-        sys.exit(1)
-
-if __name__ == "__main__":
+def main():
+
+    import sys
+    import signal
+    import argparse
+    from edman import DB
+    from scripts.action import Action
+
+    # Ctrl-Cを押下された時の対策
+    signal.signal(signal.SIGINT, lambda sig, frame: sys.exit('\n'))
+
+    # コマンドライン引数処理
+    parser = argparse.ArgumentParser(description='ドキュメントの項目を削除するスクリプト')
+    # parser.add_argument('-c', '--collection', help='collection name.')
+    parser.add_argument('objectid', help='objectid str.')
+    # クエリは structureがembの時だけ
+    parser.add_argument('-q', '--query', default=None,
+                        help='Ref is ObjectId or Emb is query list strings.')
+    parser.add_argument('-i', '--inifile', help='DB connect file path.')
+
+    # 引数を付けなかった場合はヘルプを表示して終了する
+    if len(sys.argv) == 1:
+        parser.parse_args(["-h"])
+        sys.exit(0)
+    args = parser.parse_args()
+
+    try:
+        # iniファイル読み込み
+        con = Action.reading_config_file(args.inifile)
+
+        db = DB(con)
+
+        # 対象oidの所属コレクションを自動的に取得 ※動作が遅い場合は使用しないこと
+        collection = db.find_collection_from_objectid(args.objectid)
+
+        # ドキュメント構造の取得
+        structure = db.get_structure(collection, args.objectid)
+
+        # クエリの変換
+        query = Action.file_query_eval(args.query, structure)
+
+        # ドキュメント取得
+        doc = db.doc(collection, args.objectid, query)
+        doc_keys = list(doc.keys())
+
+        # 項目を画面表示
+        for idx, (key, value) in enumerate(doc.items()):
+            print('(' + str(idx) + ')', key, ':', value)
+
+        # 表示されている選択番号を入力
+        if len(doc) > 0:
+            while True:
+                selected_idx = input('0 - ' + str(len(doc) - 1) + ' > ')
+                if selected_idx.isdecimal() and (
+                        0 <= int(selected_idx) < len(doc)):
+                    break
+                else:
+                    print('Required!')
+        else:
+            sys.exit('ドキュメントが取得できていません')
+
+        # 削除処理
+        if db.item_delete(collection, args.objectid,
+                          doc_keys[int(selected_idx)], query):
+            print('削除成功')
+        else:
+            print('削除失敗')
+
+    except Exception as e:
+        tb = sys.exc_info()[2]
+        sys.stderr.write(f'{type(e).__name__}: {e.with_traceback(tb)}\n')
+        sys.exit(1)
+
+if __name__ == "__main__":
     main()
```

### Comparing `edman_cli-2023.5.23/scripts/pullout.py` & `edman_cli-2023.5.24/venv/src/edman-cli/scripts/pullout.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-def main():
-    import sys
-    import signal
-    import argparse
-    from edman import DB
-    # from edman import DB, JsonManager
-    from scripts.action import Action
-
-    # Ctrl-Cを押下された時の対策
-    signal.signal(signal.SIGINT, lambda sig, frame: sys.exit('\n'))
-
-    # コマンドライン引数処理
-    parser = argparse.ArgumentParser(
-        description='特定コレクション内のembデータの特定のキーに対してref化を行うスクリプト')
-    parser.add_argument('collection')
-    parser.add_argument('pullout_key')
-    parser.add_argument('-e', '--exclusion_keys', nargs='*')
-    parser.add_argument('-i', '--inifile', help='DB connect file path.')
-    # parser.add_argument('-d', '--dir',
-    #                     help='Dir of report files.',
-    #                     default=None)
-
-    # 引数を付けなかった場合はヘルプを表示して終了する
-    if len(sys.argv) == 1:
-        parser.parse_args(["-h"])
-        sys.exit(0)
-    args = parser.parse_args()
-
-    # 結果を記録する場合はパスの存在を調べる
-    # if args.dir is not None:
-    #     p = Path(args.dir)
-    #     if not p.exists() and not p.is_dir():
-    #         sys.exit('パスが不正です')
-
-    try:
-        # iniファイル読み込み
-        con = Action.reading_config_file(args.inifile)
-
-        db = DB(con)
-        exclusion = tuple(args.exclusion_keys if args.exclusion_keys is not None else [])
-        result = db.loop_exclusion_key_and_ref(args.collection, args.pullout_key, exclusion)
-
-        # 結果を保存する
-        # if args.dir is not None:
-        #     jm = JsonManager()
-        #     jm.save(result, args.dir, 'pullout', date=True)
-
-    except Exception as e:
-        tb = sys.exc_info()[2]
-        sys.stderr.write(f'{type(e).__name__}: {e.with_traceback(tb)}\n')
-        sys.exit(1)
-
-if __name__ == "__main__":
+def main():
+    import sys
+    import signal
+    import argparse
+    from edman import DB
+    # from edman import DB, JsonManager
+    from scripts.action import Action
+
+    # Ctrl-Cを押下された時の対策
+    signal.signal(signal.SIGINT, lambda sig, frame: sys.exit('\n'))
+
+    # コマンドライン引数処理
+    parser = argparse.ArgumentParser(
+        description='特定コレクション内のembデータの特定のキーに対してref化を行うスクリプト')
+    parser.add_argument('collection')
+    parser.add_argument('pullout_key')
+    parser.add_argument('-e', '--exclusion_keys', nargs='*')
+    parser.add_argument('-i', '--inifile', help='DB connect file path.')
+    # parser.add_argument('-d', '--dir',
+    #                     help='Dir of report files.',
+    #                     default=None)
+
+    # 引数を付けなかった場合はヘルプを表示して終了する
+    if len(sys.argv) == 1:
+        parser.parse_args(["-h"])
+        sys.exit(0)
+    args = parser.parse_args()
+
+    # 結果を記録する場合はパスの存在を調べる
+    # if args.dir is not None:
+    #     p = Path(args.dir)
+    #     if not p.exists() and not p.is_dir():
+    #         sys.exit('パスが不正です')
+
+    try:
+        # iniファイル読み込み
+        con = Action.reading_config_file(args.inifile)
+
+        db = DB(con)
+        exclusion = tuple(args.exclusion_keys if args.exclusion_keys is not None else [])
+        result = db.loop_exclusion_key_and_ref(args.collection, args.pullout_key, exclusion)
+
+        # 結果を保存する
+        # if args.dir is not None:
+        #     jm = JsonManager()
+        #     jm.save(result, args.dir, 'pullout', date=True)
+
+    except Exception as e:
+        tb = sys.exc_info()[2]
+        sys.stderr.write(f'{type(e).__name__}: {e.with_traceback(tb)}\n')
+        sys.exit(1)
+
+if __name__ == "__main__":
     main()
```

### Comparing `edman_cli-2023.5.23/scripts/structure_convert.py` & `edman_cli-2023.5.24/venv/src/edman-cli/scripts/structure_convert.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-def main():
-
-    import sys
-    import signal
-    import argparse
-    from edman import DB
-    from scripts.action import Action
-
-    # Ctrl-Cを押下された時の対策
-    signal.signal(signal.SIGINT, lambda sig, frame: sys.exit('\n'))
-
-    # コマンドライン引数処理
-    parser = argparse.ArgumentParser(description='DBから検索したデータをコンバートしてDBに入れるスクリプト')
-    # parser.add_argument('-c', '--collection', help='collection name.')
-    parser.add_argument('objectid', help='objectid str.')
-    # parser.add_argument('-s', '--structure', default='ref',
-    #                     help='Select ref(Reference, default) or emb(embedded).')
-    parser.add_argument('new_collection', help='new collection name.')
-    parser.add_argument('-i', '--inifile', help='DB connect file path.')
-
-    # 引数を付けなかった場合はヘルプを表示して終了する
-    if len(sys.argv) == 1:
-        parser.parse_args(["-h"])
-        sys.exit(0)
-    args = parser.parse_args()
-
-    try:
-        # iniファイル読み込み
-        con = Action.reading_config_file(args.inifile)
-
-        db = DB(con)
-        # 対象oidの所属コレクションを自動的に取得 ※動作が遅い場合は使用しないこと
-        collection = db.find_collection_from_objectid(args.objectid)
-
-        # 対象のドキュメントがrefかembかを調べる
-        # (ただし、子要素が存在しないドキュメントの場合は必ずembと表示される)
-        current_structure = db.get_structure(collection, args.objectid)
-        print(f'このドキュメントは {current_structure} 形式です')
-        structures = ['emb', 'ref']
-        structures.remove(current_structure)
-
-        while True:
-            convert_selected = input(f'{structures[0]}に変更しますか？ y/n(exit) >> ')
-            if convert_selected == 'y':
-                result = db.structure(collection, args.objectid, structures[0],
-                                      args.new_collection)
-                print('\n', result)
-                break
-            elif convert_selected == 'n':
-                sys.exit()
-            else:
-                continue
-
-    except Exception as e:
-        tb = sys.exc_info()[2]
-        sys.stderr.write(f'{type(e).__name__}: {e.with_traceback(tb)}\n')
-        sys.exit(1)
-
-if __name__ == "__main__":
+def main():
+
+    import sys
+    import signal
+    import argparse
+    from edman import DB
+    from scripts.action import Action
+
+    # Ctrl-Cを押下された時の対策
+    signal.signal(signal.SIGINT, lambda sig, frame: sys.exit('\n'))
+
+    # コマンドライン引数処理
+    parser = argparse.ArgumentParser(description='DBから検索したデータをコンバートしてDBに入れるスクリプト')
+    # parser.add_argument('-c', '--collection', help='collection name.')
+    parser.add_argument('objectid', help='objectid str.')
+    # parser.add_argument('-s', '--structure', default='ref',
+    #                     help='Select ref(Reference, default) or emb(embedded).')
+    parser.add_argument('new_collection', help='new collection name.')
+    parser.add_argument('-i', '--inifile', help='DB connect file path.')
+
+    # 引数を付けなかった場合はヘルプを表示して終了する
+    if len(sys.argv) == 1:
+        parser.parse_args(["-h"])
+        sys.exit(0)
+    args = parser.parse_args()
+
+    try:
+        # iniファイル読み込み
+        con = Action.reading_config_file(args.inifile)
+
+        db = DB(con)
+        # 対象oidの所属コレクションを自動的に取得 ※動作が遅い場合は使用しないこと
+        collection = db.find_collection_from_objectid(args.objectid)
+
+        # 対象のドキュメントがrefかembかを調べる
+        # (ただし、子要素が存在しないドキュメントの場合は必ずembと表示される)
+        current_structure = db.get_structure(collection, args.objectid)
+        print(f'このドキュメントは {current_structure} 形式です')
+        structures = ['emb', 'ref']
+        structures.remove(current_structure)
+
+        while True:
+            convert_selected = input(f'{structures[0]}に変更しますか？ y/n(exit) >> ')
+            if convert_selected == 'y':
+                result = db.structure(collection, args.objectid, structures[0],
+                                      args.new_collection)
+                print('\n', result)
+                break
+            elif convert_selected == 'n':
+                sys.exit()
+            else:
+                continue
+
+    except Exception as e:
+        tb = sys.exc_info()[2]
+        sys.stderr.write(f'{type(e).__name__}: {e.with_traceback(tb)}\n')
+        sys.exit(1)
+
+if __name__ == "__main__":
     main()
```

### Comparing `edman_cli-2023.5.23/scripts/update.py` & `edman_cli-2023.5.24/scripts/file_delete.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,61 +1,83 @@
-def main():
-    import sys
-    import signal
-    import argparse
-    import json
-    from edman import DB
-    from scripts.action import Action
-
-    # Ctrl-Cを押下された時の対策
-    signal.signal(signal.SIGINT, lambda sig, frame: sys.exit('\n'))
-
-    # コマンドライン引数処理
-    parser = argparse.ArgumentParser(description='ドキュメントの項目を修正するスクリプト')
-    # parser.add_argument('-c', '--collection', help='collection name.')
-    parser.add_argument('objectid', help='objectid str.')
-    parser.add_argument('amend_file', type=open, help='JSON file.')
-    parser.add_argument('structure', help='Select ref or emb.')
-    parser.add_argument('-i', '--inifile', help='DB connect file path.')
-
-    # 引数を付けなかった場合はヘルプを表示して終了する
-    if len(sys.argv) == 1:
-        parser.parse_args(["-h"])
-        sys.exit(0)
-    args = parser.parse_args()
-
-    # 構造はrefかembのどちらか
-    if not (args.structure == 'ref' or args.structure == 'emb'):
-        parser.error("structure requires 'ref' or 'emb'.")
-
-    try:
-        # iniファイル読み込み
-        con = Action.reading_config_file(args.inifile)
-
-        # ファイル読み込み
-        try:
-
-            amend_data = json.load(args.amend_file)
-        except json.JSONDecodeError:
-            sys.exit(f'File is not json format.')
-        except IOError:
-            sys.exit('file read error.')
-
-        #  DB接続
-        db = DB(con)
-
-        # 対象oidの所属コレクションを自動的に取得 ※動作が遅い場合は使用しないこと
-        collection = db.find_collection_from_objectid(args.objectid)
-
-        # アップデート処理
-        if db.update(collection, args.objectid, amend_data, args.structure):
-            print('アップデート成功')
-        else:
-            print('アップデート失敗')
-
-    except Exception as e:
-        tb = sys.exc_info()[2]
-        sys.stderr.write(f'{type(e).__name__}: {e.with_traceback(tb)}\n')
-        sys.exit(1)
-
-if __name__ == "__main__":
-    main()
+def main():
+    import argparse
+    import signal
+    import sys
+
+    from edman import DB, File
+
+    from scripts.action import Action
+
+    # Ctrl-Cを押下された時の対策
+    signal.signal(signal.SIGINT, lambda sig, frame: sys.exit('\n'))
+
+    # コマンドライン引数処理
+    parser = argparse.ArgumentParser(
+        description='ファイルを実験データから削除するスクリプト')
+    # parser.add_argument('-c', '--collection', help='collection name.')
+    parser.add_argument('objectid', help='objectid str.')
+    # クエリは structureがembの時だけ
+    parser.add_argument('-q', '--query', default=None,
+                        help='Ref is ObjectId or Emb is query list strings.')
+    parser.add_argument('-i', '--inifile', help='DB connect file path.')
+
+    # 引数を付けなかった場合はヘルプを表示して終了する
+    if len(sys.argv) == 1:
+        parser.parse_args(["-h"])
+        sys.exit(0)
+    args = parser.parse_args()
+
+    try:
+        # iniファイル読み込み
+        con = Action.reading_config_file(args.inifile)
+
+        db = DB(con)
+        file = File(db.get_db)
+
+        # 対象oidの所属コレクションを自動的に取得 ※動作が遅い場合は使用しないこと
+        collection = db.find_collection_from_objectid(args.objectid)
+
+        # ドキュメント構造の取得
+        structure = db.get_structure(collection, args.objectid)
+
+        # クエリの変換
+        query = Action.file_query_eval(args.query, structure)
+
+        # ファイル名一覧を取得
+        file_names = file.get_file_names(collection, args.objectid, structure,
+                                         query)
+        if not file_names:
+            sys.exit('ファイルは存在しません')
+
+        file_oids = []
+        # ファイル名一覧を画面表示&file_oid用リスト作成
+        for idx, (oid, filename) in enumerate(file_names.items()):
+            print('(' + str(idx) + ')', filename, oid)
+            file_oids.append(oid)
+
+        # 表示されている選択番号を入力
+        if len(file_names) > 0:
+            while True:
+                selected_idx = input('0 - ' + str(len(file_names) - 1) + ' > ')
+                if selected_idx.isdecimal() and (
+                        0 <= int(selected_idx) < len(file_names)):
+                    break
+                else:
+                    print('Required!')
+        else:
+            sys.exit('インデックスが不正です')
+
+        # 該当するファイルを削除
+        if file.delete(file_oids[int(selected_idx)], collection, args.objectid,
+                       structure, query):
+            print('削除完了')
+        else:
+            print('削除失敗')
+
+    except Exception as e:
+        tb = sys.exc_info()[2]
+        sys.stderr.write(f'{type(e).__name__}: {e.with_traceback(tb)}\n')
+        sys.exit(1)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `edman_cli-2023.5.23/tests/test_action.py` & `edman_cli-2023.5.24/venv/src/edman-cli/tests/test_action.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.23/venv/bin/jp.py` & `edman_cli-2023.5.24/venv/bin/jp.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.23/venv/bin/rst2html.py` & `edman_cli-2023.5.24/venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.23/venv/bin/rst2html4.py` & `edman_cli-2023.5.24/venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.23/venv/bin/rst2html5.py` & `edman_cli-2023.5.24/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.23/venv/bin/rst2latex.py` & `edman_cli-2023.5.24/venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.23/venv/bin/rst2man.py` & `edman_cli-2023.5.24/venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.23/venv/bin/rst2odt.py` & `edman_cli-2023.5.24/venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.23/venv/bin/rst2odt_prepstyles.py` & `edman_cli-2023.5.24/venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.23/venv/bin/rst2pseudoxml.py` & `edman_cli-2023.5.24/venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.23/venv/bin/rst2s5.py` & `edman_cli-2023.5.24/venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.23/venv/bin/rst2xetex.py` & `edman_cli-2023.5.24/venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.23/venv/bin/rst2xml.py` & `edman_cli-2023.5.24/venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.23/venv/bin/rstpep2html.py` & `edman_cli-2023.5.24/venv/bin/rstpep2html.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.23/venv/src/edman-cli/scripts/action.py` & `edman_cli-2023.5.24/scripts/action.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-import sys
-import os
-import json
 import ast
-import getpass
 import configparser
-from pathlib import Path
+import getpass
+import json
+import os
+import sys
 from collections import OrderedDict
+from pathlib import Path
 from typing import Iterator, Union
+
 from edman import DB
 from edman.exceptions import EdmanDbConnectError, EdmanDbProcessError
 
 
 class Action:
     """
     ラッパーやファイル読み込み操作、書き出しなどの操作用
@@ -108,23 +109,23 @@
         except SyntaxError:
             sys.exit(error_message)
         if not isinstance(query, dict):
             sys.exit(error_message)
         return query
 
     @staticmethod
-    def file_query_eval(raw_query: str, structure: str) -> list:
+    def file_query_eval(raw_query: str, structure: str) -> list | None:
         """
         embの場合文字列のクエリを受け取り、リストに変換する
         refの場合はNoneを返す
 
         :param str raw_query:
         :param str structure:
         :return: query
-        :rtype: list
+        :rtype: list or None
         """
         # embのときだけクエリが必須
         if 'ref' in structure:
             query = None
         elif 'emb' in structure:
             if raw_query is None:
                 sys.exit('クエリがありません')
@@ -251,15 +252,15 @@
                 f"user = {ini_data['username']}",
                 f"password = {ini_data['userpwd']}",
                 f"database = {ini_data['dbname']}",
                 f'options = ["{authsource}"]' + '\n'
             ]
 
         # iniファイルの書き出し
-        savefile = ini_dir / filename
+        savefile = ini_dir / filename  # type: ignore
         try:
             with savefile.open("w") as file:
                 file.writelines('\n'.join(put_data))
                 file.flush()
                 os.fsync(file.fileno())
 
                 print(f'Create {savefile}')
@@ -314,16 +315,18 @@
                 db.delete_role(user['name'], user['dbname'])
                 db.delete_db(user['dbname'])
             else:
                 db.delete_user_and_role(user['name'], user['dbname'])
                 db.delete_db(user['dbname'])
         except EdmanDbProcessError:
             sys.exit('DB,User/Role delete failed.')
-        except:
-            sys.exit('DB,User/Role delete failed for unknown reason.')
+        except EdmanDbConnectError:
+            sys.exit('DB not connect.')
+        except Exception as e:
+            sys.exit(str(e))
         else:
             print('DB,User/Role delete OK.')
 
     @staticmethod
     def is_duplicate_filename(ini_dir: Path) -> tuple[bool, Union[str, None]]:
         """
         ini_dirのパスに指定のファイルが存在していれば重複のフラグ、
@@ -356,18 +359,18 @@
         """
         acc = OrderedDict()
         acc['name'] = f"MongoDB's {user} name >> "
         acc['dbname'] = f"MongoDB's {user} DB >> "
 
         if not ldap:
             acc['pwd'] = f"MongoDB's {user} password >> "
-            acc[
-                'pwd_verification'] = f"MongoDB's {user} Verification password >> "
+            acc['pwd_verification'] = (f"MongoDB's {user} "
+                                       f"Verification password >> ")
 
-        account = {}
+        account: dict = {}
         for key, value in acc.items():
             buff = ""
             if 'name' == key or 'dbname' == key:
                 while True:
                     if not (buff := input(value)):
                         print('Required!')
                     else:
@@ -406,15 +409,15 @@
         print(f'[{user}]')
         for key, value in user_data.items():
             print(key + ' : ' + '*' * len(
                 value) if key == 'pwd' else key + ' : ' + value)
 
     @staticmethod
     def outputs(users: dict, host: str, port: int,
-                ini_dir: Union[Path, None]) -> None:
+                ini_dir: Path | None) -> None:
         """
             DB入力項目の確認表示(サーバ項目)
 
         :param dict users:
         :param str host:
         :param int port:
         :param Path or None ini_dir:
@@ -426,27 +429,27 @@
         print(f"""
         host : {host}
         port : {port}
         """)
         if ini_dir is not None:
             dup_flg, proposal_filename = Action.is_duplicate_filename(ini_dir)
             filename = proposal_filename if dup_flg else Action.default_ini
-            print(f"ini path : {ini_dir / filename}")
+            ini_path = ini_dir / filename  # type: ignore
+            print(f"ini path : {ini_path}")
 
     @staticmethod
     def generate_config_path(filepath: Union[str, None]) -> Path:
         """
         パス文字列からパスオブジェクト生成
         パス文字列がなければデフォルトのiniディレクトリパスを返す
 
         :param str or None filepath:
         :return: result
         :rtype: Path
         """
-
         if filepath is not None:
             p = Path(filepath)
             if p.exists():
                 result = p
             else:
                 sys.exit(f'{filepath}は存在しません')
         else:
@@ -461,17 +464,10 @@
 
         :param str or None input_file:
         :return:
         :rtype: dict
         """
         settings = configparser.ConfigParser()
         settings.read(Action.generate_config_path(input_file))
-
-        result = {}
-        for k, v in settings['DB'].items():
-            if k == 'options':
-                s = json.loads(v)
-            else:
-                s = v
-            result.update({k: s})
+        result = {k: json.loads(v) if k == 'options' else v for k, v in
+                  settings['DB'].items()}
         return result
-        # return dict([i for i in settings['DB'].items()])
```

### Comparing `edman_cli-2023.5.23/venv/src/edman-cli/scripts/assign_bson_type.py` & `edman_cli-2023.5.24/venv/src/edman-cli/scripts/assign_bson_type.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.23/venv/src/edman-cli/scripts/db_create.py` & `edman_cli-2023.5.24/scripts/db_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 def main():
     """
     新しいユーザ権限のDBを作成
     """
-    import sys
-    import signal
     import argparse
+    import signal
+    import sys
     from pathlib import Path
+
     from scripts.action import Action
 
     # Ctrl-Cを押下された時の対策
     signal.signal(signal.SIGINT, lambda sig, frame: sys.exit('\n'))
 
     # コマンドライン引数処理
     parser = argparse.ArgumentParser(description='MongoDBのユーザとDBを作成するスクリプト')
@@ -84,15 +85,16 @@
                 continue
 
         # DB作成
         Action.create(admin_account, user_account, ini_dir, host, port,
                       ldap=args.db_only)
 
         # テスト用のためにここに置く
-        # db.destroy(user_account, host, port, admin=admin_account, del_user=True)
+        # db.destroy(user_account, host, port, admin=admin_account,
+        # del_user=True)
 
     except Exception as e:
         tb = sys.exc_info()[2]
         sys.stderr.write(f'{type(e).__name__}: {e.with_traceback(tb)}\n')
         sys.exit(1)
```

### Comparing `edman_cli-2023.5.23/venv/src/edman-cli/scripts/db_destroy.py` & `edman_cli-2023.5.24/scripts/db_destroy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 def main():
     """
     DBと認証ユーザを削除する
     """
-    import sys
-    import signal
     import argparse
+    import signal
+    import sys
+
     from scripts.action import Action
 
     # Ctrl-Cを押下された時の対策
     signal.signal(signal.SIGINT, lambda sig, frame: sys.exit('\n'))
 
     # コマンドライン引数処理
     parser = argparse.ArgumentParser(
         description='DB及びDB管理ユーザ/管理ロール削除スクリプト')
     parser.add_argument('-r', '--remove_role',
-                        help='Remove DB and role(LDAP User),MongoDB Admin account required.',
+                        help='Remove DB and role(LDAP User),'
+                             'MongoDB Admin account required.',
                         action='store_true')
 
     # 引数を付けなかった場合はヘルプを表示して終了する
     # if len(sys.argv) == 1:
     #     parser.parse_args(["-h"])
     #     sys.exit(0)
```

### Comparing `edman_cli-2023.5.23/venv/src/edman-cli/scripts/delete.py` & `edman_cli-2023.5.24/venv/src/edman-cli/scripts/delete.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.23/venv/src/edman-cli/scripts/entry.py` & `edman_cli-2023.5.24/venv/src/edman-cli/scripts/entry.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.23/venv/src/edman-cli/scripts/file_add.py` & `edman_cli-2023.5.24/venv/src/edman-cli/scripts/file_add.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.23/venv/src/edman-cli/scripts/file_delete.py` & `edman_cli-2023.5.24/venv/src/edman-cli/scripts/file_delete.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.23/venv/src/edman-cli/scripts/file_dl.py` & `edman_cli-2023.5.24/scripts/item_delete.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 def main():
-
-    import sys
-    import signal
     import argparse
-    from edman import DB, File
+    import signal
+    import sys
+
+    from edman import DB
+
     from scripts.action import Action
 
     # Ctrl-Cを押下された時の対策
     signal.signal(signal.SIGINT, lambda sig, frame: sys.exit('\n'))
 
     # コマンドライン引数処理
-    parser = argparse.ArgumentParser(
-        description='ファイルを実験データからダウンロードするスクリプト')
+    parser = argparse.ArgumentParser(description='ドキュメントの項目を削除するスクリプト')
     # parser.add_argument('-c', '--collection', help='collection name.')
     parser.add_argument('objectid', help='objectid str.')
-    parser.add_argument('path', help='Download Dir path.')
     # クエリは structureがembの時だけ
     parser.add_argument('-q', '--query', default=None,
                         help='Ref is ObjectId or Emb is query list strings.')
     parser.add_argument('-i', '--inifile', help='DB connect file path.')
 
     # 引数を付けなかった場合はヘルプを表示して終了する
     if len(sys.argv) == 1:
@@ -27,56 +26,52 @@
     args = parser.parse_args()
 
     try:
         # iniファイル読み込み
         con = Action.reading_config_file(args.inifile)
 
         db = DB(con)
-        file = File(db.get_db)
 
         # 対象oidの所属コレクションを自動的に取得 ※動作が遅い場合は使用しないこと
         collection = db.find_collection_from_objectid(args.objectid)
 
         # ドキュメント構造の取得
         structure = db.get_structure(collection, args.objectid)
 
         # クエリの変換
         query = Action.file_query_eval(args.query, structure)
 
-        # ファイル名一覧を取得
-        file_names = file.get_file_names(collection, args.objectid, structure,
-                                         query)
-        if not file_names:
-            sys.exit('ファイルは存在しません')
-
-        file_oids = []
-        # ファイル名一覧を画面表示&file_oid用リスト作成
-        for idx, (oid, filename) in enumerate(file_names.items()):
-            print('(' + str(idx) + ')', filename, oid)
-            file_oids.append(oid)
+        # ドキュメント取得
+        doc = db.doc(collection, args.objectid, query)
+        doc_keys = list(doc.keys())
+
+        # 項目を画面表示
+        for idx, (key, value) in enumerate(doc.items()):
+            print('(' + str(idx) + ')', key, ':', value)
 
-        # 複数ファイルの場合、表示されている選択番号を入力
-        if len(file_names) > 1:
+        # 表示されている選択番号を入力
+        if len(doc) > 0:
             while True:
-                selected_idx = input('0 - ' + str(len(file_names) - 1) + ' > ')
+                selected_idx = input('0 - ' + str(len(doc) - 1) + ' > ')
                 if selected_idx.isdecimal() and (
-                        0 <= int(selected_idx) < len(file_names)):
+                        0 <= int(selected_idx) < len(doc)):
                     break
                 else:
                     print('Required!')
-        # ファイルが一つしかない場合は選択無しでDL
-        elif len(file_names) == 1:
-            selected_idx = 0
         else:
-            sys.exit('インデックスが不正です')
+            sys.exit('ドキュメントが取得できていません')
 
-        # 指定のディレクトリにダウンロード
-        if file.download(file_oids[int(selected_idx)], args.path):
-            print('DLしました')
+        # 削除処理
+        if db.item_delete(collection, args.objectid,
+                          doc_keys[int(selected_idx)], query):
+            print('削除成功')
+        else:
+            print('削除失敗')
 
     except Exception as e:
         tb = sys.exc_info()[2]
         sys.stderr.write(f'{type(e).__name__}: {e.with_traceback(tb)}\n')
         sys.exit(1)
 
+
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `edman_cli-2023.5.23/venv/src/edman-cli/scripts/find.py` & `edman_cli-2023.5.24/scripts/find.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 def main():
-    import sys
-    import signal
     import argparse
+    import signal
+    import sys
+
     from edman import DB, JsonManager, Search
+
     from scripts.action import Action
 
     # Ctrl-Cを押下された時の対策
     signal.signal(signal.SIGINT, lambda sig, frame: sys.exit('\n'))
     # コマンドライン引数処理
-    parser = argparse.ArgumentParser(description='DBから検索して結果をJSONファイルにするスクリプト')
+    parser = argparse.ArgumentParser(
+        description='DBから検索して結果をJSONファイルにするスクリプト')
     parser.add_argument('collection')
     # コマンドもしくはファイルでの検索文字列を選択
     group = parser.add_mutually_exclusive_group()
     group.add_argument('-q', '--query')
     group.add_argument('-f', '--query_file', type=open)
     parser.add_argument('-p', '--parent_depth', type=int, default=0)
     parser.add_argument('-c', '--child_depth', type=int, default=0)
@@ -31,15 +34,16 @@
 
     # クエリおよびクエリファイルはどちらかは必須
     if not args.query and not args.query_file:
         parser.error("query or query_file is mandatory.")
 
     try:
         # クエリ入力値変換
-        query = Action.query_eval(args.query if args.query else args.query_file.read())
+        query = Action.query_eval(
+            args.query if args.query else args.query_file.read())
 
         # iniファイル読み込み
         con = Action.reading_config_file(args.inifile)
 
         db = DB(con)
         search = Search(db)
 
@@ -52,9 +56,10 @@
         jm.save(search_result, args.dir, name=args.out_file_name, date=True)
 
     except Exception as e:
         tb = sys.exc_info()[2]
         sys.stderr.write(f'{type(e).__name__}: {e.with_traceback(tb)}\n')
         sys.exit(1)
 
+
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `edman_cli-2023.5.23/venv/src/edman-cli/scripts/item_delete.py` & `edman_cli-2023.5.24/venv/src/edman-cli/scripts/update.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,74 +1,60 @@
 def main():
-
     import sys
     import signal
     import argparse
+    import json
     from edman import DB
     from scripts.action import Action
 
     # Ctrl-Cを押下された時の対策
     signal.signal(signal.SIGINT, lambda sig, frame: sys.exit('\n'))
 
     # コマンドライン引数処理
-    parser = argparse.ArgumentParser(description='ドキュメントの項目を削除するスクリプト')
+    parser = argparse.ArgumentParser(description='ドキュメントの項目を修正するスクリプト')
     # parser.add_argument('-c', '--collection', help='collection name.')
     parser.add_argument('objectid', help='objectid str.')
-    # クエリは structureがembの時だけ
-    parser.add_argument('-q', '--query', default=None,
-                        help='Ref is ObjectId or Emb is query list strings.')
+    parser.add_argument('amend_file', type=open, help='JSON file.')
+    parser.add_argument('structure', help='Select ref or emb.')
     parser.add_argument('-i', '--inifile', help='DB connect file path.')
 
     # 引数を付けなかった場合はヘルプを表示して終了する
     if len(sys.argv) == 1:
         parser.parse_args(["-h"])
         sys.exit(0)
     args = parser.parse_args()
 
+    # 構造はrefかembのどちらか
+    if not (args.structure == 'ref' or args.structure == 'emb'):
+        parser.error("structure requires 'ref' or 'emb'.")
+
     try:
         # iniファイル読み込み
         con = Action.reading_config_file(args.inifile)
 
+        # ファイル読み込み
+        try:
+
+            amend_data = json.load(args.amend_file)
+        except json.JSONDecodeError:
+            sys.exit(f'File is not json format.')
+        except IOError:
+            sys.exit('file read error.')
+
+        #  DB接続
         db = DB(con)
 
         # 対象oidの所属コレクションを自動的に取得 ※動作が遅い場合は使用しないこと
         collection = db.find_collection_from_objectid(args.objectid)
 
-        # ドキュメント構造の取得
-        structure = db.get_structure(collection, args.objectid)
-
-        # クエリの変換
-        query = Action.file_query_eval(args.query, structure)
-
-        # ドキュメント取得
-        doc = db.doc(collection, args.objectid, query)
-        doc_keys = list(doc.keys())
-
-        # 項目を画面表示
-        for idx, (key, value) in enumerate(doc.items()):
-            print('(' + str(idx) + ')', key, ':', value)
-
-        # 表示されている選択番号を入力
-        if len(doc) > 0:
-            while True:
-                selected_idx = input('0 - ' + str(len(doc) - 1) + ' > ')
-                if selected_idx.isdecimal() and (
-                        0 <= int(selected_idx) < len(doc)):
-                    break
-                else:
-                    print('Required!')
-        else:
-            sys.exit('ドキュメントが取得できていません')
-
-        # 削除処理
-        if db.item_delete(collection, args.objectid,
-                          doc_keys[int(selected_idx)], query):
-            print('削除成功')
+        # アップデート処理
+        if db.update(collection, args.objectid, amend_data, args.structure):
+            print('アップデート成功')
         else:
-            print('削除失敗')
+            print('アップデート失敗')
 
     except Exception as e:
         tb = sys.exc_info()[2]
         sys.stderr.write(f'{type(e).__name__}: {e.with_traceback(tb)}\n')
         sys.exit(1)
 
 if __name__ == "__main__":
```

### Comparing `edman_cli-2023.5.23/venv/src/edman-cli/scripts/pullout.py` & `edman_cli-2023.5.24/scripts/pullout.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 def main():
-    import sys
-    import signal
     import argparse
+    import signal
+    import sys
+
     from edman import DB
+
     # from edman import DB, JsonManager
     from scripts.action import Action
 
     # Ctrl-Cを押下された時の対策
     signal.signal(signal.SIGINT, lambda sig, frame: sys.exit('\n'))
 
     # コマンドライン引数処理
@@ -33,22 +35,27 @@
     #         sys.exit('パスが不正です')
 
     try:
         # iniファイル読み込み
         con = Action.reading_config_file(args.inifile)
 
         db = DB(con)
-        exclusion = tuple(args.exclusion_keys if args.exclusion_keys is not None else [])
-        result = db.loop_exclusion_key_and_ref(args.collection, args.pullout_key, exclusion)
+        exclusion = tuple(
+            args.exclusion_keys if args.exclusion_keys is not None else [])
+        _ = db.loop_exclusion_key_and_ref(args.collection,
+                                          args.pullout_key, exclusion)
 
         # 結果を保存する
+        # result = db.loop_exclusion_key_and_ref(args.collection,
+        #                                        args.pullout_key, exclusion)
         # if args.dir is not None:
         #     jm = JsonManager()
         #     jm.save(result, args.dir, 'pullout', date=True)
 
     except Exception as e:
         tb = sys.exc_info()[2]
         sys.stderr.write(f'{type(e).__name__}: {e.with_traceback(tb)}\n')
         sys.exit(1)
 
+
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `edman_cli-2023.5.23/venv/src/edman-cli/scripts/structure_convert.py` & `edman_cli-2023.5.24/scripts/structure_convert.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 def main():
-
-    import sys
-    import signal
     import argparse
+    import signal
+    import sys
+
     from edman import DB
+
     from scripts.action import Action
 
     # Ctrl-Cを押下された時の対策
     signal.signal(signal.SIGINT, lambda sig, frame: sys.exit('\n'))
 
     # コマンドライン引数処理
-    parser = argparse.ArgumentParser(description='DBから検索したデータをコンバートしてDBに入れるスクリプト')
+    parser = argparse.ArgumentParser(
+        description='DBから検索したデータをコンバートしてDBに入れるスクリプト')
     # parser.add_argument('-c', '--collection', help='collection name.')
     parser.add_argument('objectid', help='objectid str.')
     # parser.add_argument('-s', '--structure', default='ref',
-    #                     help='Select ref(Reference, default) or emb(embedded).')
+    #                 help='Select ref(Reference, default) or emb(embedded).')
     parser.add_argument('new_collection', help='new collection name.')
     parser.add_argument('-i', '--inifile', help='DB connect file path.')
 
     # 引数を付けなかった場合はヘルプを表示して終了する
     if len(sys.argv) == 1:
         parser.parse_args(["-h"])
         sys.exit(0)
@@ -36,15 +38,16 @@
         # (ただし、子要素が存在しないドキュメントの場合は必ずembと表示される)
         current_structure = db.get_structure(collection, args.objectid)
         print(f'このドキュメントは {current_structure} 形式です')
         structures = ['emb', 'ref']
         structures.remove(current_structure)
 
         while True:
-            convert_selected = input(f'{structures[0]}に変更しますか？ y/n(exit) >> ')
+            convert_selected = input(
+                f'{structures[0]}に変更しますか？ y/n(exit) >> ')
             if convert_selected == 'y':
                 result = db.structure(collection, args.objectid, structures[0],
                                       args.new_collection)
                 print('\n', result)
                 break
             elif convert_selected == 'n':
                 sys.exit()
@@ -52,9 +55,10 @@
                 continue
 
     except Exception as e:
         tb = sys.exc_info()[2]
         sys.stderr.write(f'{type(e).__name__}: {e.with_traceback(tb)}\n')
         sys.exit(1)
 
+
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `edman_cli-2023.5.23/venv/src/edman-cli/scripts/update.py` & `edman_cli-2023.5.24/scripts/update.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 def main():
-    import sys
-    import signal
     import argparse
     import json
+    import signal
+    import sys
+
     from edman import DB
+
     from scripts.action import Action
 
     # Ctrl-Cを押下された時の対策
     signal.signal(signal.SIGINT, lambda sig, frame: sys.exit('\n'))
 
     # コマンドライン引数処理
     parser = argparse.ArgumentParser(description='ドキュメントの項目を修正するスクリプト')
@@ -32,15 +34,15 @@
         con = Action.reading_config_file(args.inifile)
 
         # ファイル読み込み
         try:
 
             amend_data = json.load(args.amend_file)
         except json.JSONDecodeError:
-            sys.exit(f'File is not json format.')
+            sys.exit('File is not json format.')
         except IOError:
             sys.exit('file read error.')
 
         #  DB接続
         db = DB(con)
 
         # 対象oidの所属コレクションを自動的に取得 ※動作が遅い場合は使用しないこと
@@ -53,9 +55,10 @@
             print('アップデート失敗')
 
     except Exception as e:
         tb = sys.exc_info()[2]
         sys.stderr.write(f'{type(e).__name__}: {e.with_traceback(tb)}\n')
         sys.exit(1)
 
+
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `edman_cli-2023.5.23/venv/src/edman-cli/setup.py` & `edman_cli-2023.5.24/venv/src/edman-cli/setup.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.5.23/venv/src/edman-cli/tests/test_action.py` & `edman_cli-2023.5.24/tests/test_action.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
+import configparser
+import json
+import shutil
 import sys
 import tempfile
-import shutil
-import json
-import configparser
 from pathlib import Path
 from unittest import TestCase, skipIf
 
 # edman/scripts/action.pyが読み込める状態ならテストをする
 # それ以外なら全てのテストをスキップする
 cwd = Path.cwd()
 import_path = cwd.parent / 'scripts'
 import_path_full = import_path / 'action.py'
 if import_path_full.exists():
     sys.path.append(str(import_path))
-    from action import Action
+    from action import Action  # type: ignore
 
     import_flag = True
 else:
     import_flag = False
 
 
 class TestAction(TestCase):
@@ -235,15 +235,14 @@
                 'port': '27017',
                 'host': '127.0.0.1',
                 'user': 'username',
                 'database': 'userdb',
                 'options': ['authMechanism=PLAIN']}
             self.assertDictEqual(actual_db, expected_db)
 
-
     @skipIf(import_flag is False, 'There is no action.py')
     def test_is_duplicate_filename(self):
 
         # 重複しない場合
         with tempfile.TemporaryDirectory() as tmp_dir:
             p = Path(tmp_dir)
             dup_flg, proposal_filename = Action.is_duplicate_filename(p)
```

