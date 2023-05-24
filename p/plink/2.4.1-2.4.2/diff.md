# Comparing `tmp/plink-2.4.1.tar.gz` & `tmp/plink-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/plink-2.4.1.tar", last modified: Wed Nov 10 15:47:32 2021, max compression
+gzip compressed data, was "plink-2.4.2.tar", last modified: Tue May 23 19:36:55 2023, max compression
```

## Comparing `plink-2.4.1.tar` & `plink-2.4.2.tar`

### file list

```diff
@@ -1,62 +1,64 @@
-drwxr-xr-x   0 nmd      (444129884) UOFI\Domain Users (1233727573)        0 2021-11-10 15:47:32.423804 plink-2.4.1/
--rw-r--r--   0 nmd      (444129884) UOFI\Domain Users (1233727573)     1308 2021-11-10 15:47:32.423510 plink-2.4.1/PKG-INFO
--rw-r--r--   0 nmd      (444129884) UOFI\Domain Users (1233727573)     1148 2020-02-11 16:06:51.000000 plink-2.4.1/README.rst
-drwxr-xr-x   0 nmd      (444129884) UOFI\Domain Users (1233727573)        0 2021-11-10 15:47:32.408531 plink-2.4.1/plink.egg-info/
--rw-r--r--   0 nmd      (444129884) UOFI\Domain Users (1233727573)     1308 2021-11-10 15:47:32.000000 plink-2.4.1/plink.egg-info/PKG-INFO
--rw-r--r--   0 nmd      (444129884) UOFI\Domain Users (1233727573)     1514 2021-11-10 15:47:32.000000 plink-2.4.1/plink.egg-info/SOURCES.txt
--rw-r--r--   0 nmd      (444129884) UOFI\Domain Users (1233727573)        1 2021-11-10 15:47:32.000000 plink-2.4.1/plink.egg-info/dependency_links.txt
--rw-r--r--   0 nmd      (444129884) UOFI\Domain Users (1233727573)       42 2021-11-10 15:47:32.000000 plink-2.4.1/plink.egg-info/entry_points.txt
--rw-r--r--   0 nmd      (444129884) UOFI\Domain Users (1233727573)        1 2021-11-10 15:45:37.000000 plink-2.4.1/plink.egg-info/not-zip-safe
--rw-r--r--   0 nmd      (444129884) UOFI\Domain Users (1233727573)        6 2021-11-10 15:47:32.000000 plink-2.4.1/plink.egg-info/top_level.txt
-drwxr-xr-x   0 nmd      (444129884) UOFI\Domain Users (1233727573)        0 2021-11-10 15:47:32.413856 plink-2.4.1/plink_src/
--rw-r--r--   0 nmd      (444129884) UOFI\Domain Users (1233727573)      952 2020-02-11 16:06:51.000000 plink-2.4.1/plink_src/__init__.py
--rw-r--r--   0 nmd      (444129884) UOFI\Domain Users (1233727573)     1028 2020-02-11 16:06:51.000000 plink-2.4.1/plink_src/app.py
--rw-r--r--   0 nmd      (444129884) UOFI\Domain Users (1233727573)     8457 2020-02-11 16:06:51.000000 plink-2.4.1/plink_src/arrow.py
--rw-r--r--   0 nmd      (444129884) UOFI\Domain Users (1233727573)    20501 2021-01-18 03:28:09.000000 plink-2.4.1/plink_src/canvasvg.py
--rw-r--r--   0 nmd      (444129884) UOFI\Domain Users (1233727573)     2457 2020-02-11 16:06:51.000000 plink-2.4.1/plink_src/colors.py
--rw-r--r--   0 nmd      (444129884) UOFI\Domain Users (1233727573)     4839 2021-02-12 16:15:32.000000 plink-2.4.1/plink_src/crossings.py
--rw-r--r--   0 nmd      (444129884) UOFI\Domain Users (1233727573)     2380 2020-02-11 16:06:51.000000 plink-2.4.1/plink_src/dialog.py
-drwxr-xr-x   0 nmd      (444129884) UOFI\Domain Users (1233727573)        0 2021-11-10 15:47:32.416403 plink-2.4.1/plink_src/doc/
--rw-r--r--   0 nmd      (444129884) UOFI\Domain Users (1233727573)      230 2021-11-10 15:47:31.000000 plink-2.4.1/plink_src/doc/.buildinfo
-drwxr-xr-x   0 nmd      (444129884) UOFI\Domain Users (1233727573)        0 2021-11-10 15:47:32.416700 plink-2.4.1/plink_src/doc/_images/
--rw-r--r--   0 nmd      (444129884) UOFI\Domain Users (1233727573)    34337 2020-02-11 16:06:51.000000 plink-2.4.1/plink_src/doc/_images/plink-action.png
-drwxr-xr-x   0 nmd      (444129884) UOFI\Domain Users (1233727573)        0 2021-11-10 15:47:32.417580 plink-2.4.1/plink_src/doc/_sources/
--rw-r--r--   0 nmd      (444129884) UOFI\Domain Users (1233727573)     5554 2020-02-11 16:06:51.000000 plink-2.4.1/plink_src/doc/_sources/index.rst.txt
--rw-r--r--   0 nmd      (444129884) UOFI\Domain Users (1233727573)     1231 2020-08-17 22:05:38.000000 plink-2.4.1/plink_src/doc/_sources/installing.rst.txt
--rw-r--r--   0 nmd      (444129884) UOFI\Domain Users (1233727573)      591 2020-02-11 16:06:51.000000 plink-2.4.1/plink_src/doc/_sources/plink.rst.txt
-drwxr-xr-x   0 nmd      (444129884) UOFI\Domain Users (1233727573)        0 2021-11-10 15:47:32.423079 plink-2.4.1/plink_src/doc/_static/
--rw-r--r--   0 nmd      (444129884) UOFI\Domain Users (1233727573)    14638 2021-11-10 15:47:31.000000 plink-2.4.1/plink_src/doc/_static/basic.css
--rw-r--r--   0 nmd      (444129884) UOFI\Domain Users (1233727573)     4256 2021-11-10 15:47:31.000000 plink-2.4.1/plink_src/doc/_static/classic.css
--rw-r--r--   0 nmd      (444129884) UOFI\Domain Users (1233727573)       28 2020-11-09 03:35:31.000000 plink-2.4.1/plink_src/doc/_static/default.css
--rw-r--r--   0 nmd      (444129884) UOFI\Domain Users (1233727573)     9630 2021-11-10 15:47:25.000000 plink-2.4.1/plink_src/doc/_static/doctools.js
--rw-r--r--   0 nmd      (444129884) UOFI\Domain Users (1233727573)      355 2021-11-10 15:47:31.000000 plink-2.4.1/plink_src/doc/_static/documentation_options.js
--rw-r--r--   0 nmd      (444129884) UOFI\Domain Users (1233727573)      286 2020-11-09 03:35:31.000000 plink-2.4.1/plink_src/doc/_static/file.png
--rw-r--r--   0 nmd      (444129884) UOFI\Domain Users (1233727573)   287630 2020-11-09 03:35:31.000000 plink-2.4.1/plink_src/doc/_static/jquery-3.5.1.js
--rw-r--r--   0 nmd      (444129884) UOFI\Domain Users (1233727573)    89476 2020-11-09 03:35:31.000000 plink-2.4.1/plink_src/doc/_static/jquery.js
--rw-r--r--   0 nmd      (444129884) UOFI\Domain Users (1233727573)    10854 2021-11-10 15:47:31.000000 plink-2.4.1/plink_src/doc/_static/language_data.js
--rw-r--r--   0 nmd      (444129884) UOFI\Domain Users (1233727573)       90 2020-11-09 03:35:31.000000 plink-2.4.1/plink_src/doc/_static/minus.png
--rw-r--r--   0 nmd      (444129884) UOFI\Domain Users (1233727573)       90 2020-11-09 03:35:31.000000 plink-2.4.1/plink_src/doc/_static/plus.png
--rw-r--r--   0 nmd      (444129884) UOFI\Domain Users (1233727573)     4846 2021-11-10 15:47:31.000000 plink-2.4.1/plink_src/doc/_static/pygments.css
--rw-r--r--   0 nmd      (444129884) UOFI\Domain Users (1233727573)    16733 2021-11-10 15:47:25.000000 plink-2.4.1/plink_src/doc/_static/searchtools.js
--rw-r--r--   0 nmd      (444129884) UOFI\Domain Users (1233727573)     4803 2021-11-10 15:47:31.000000 plink-2.4.1/plink_src/doc/_static/sidebar.js
--rw-r--r--   0 nmd      (444129884) UOFI\Domain Users (1233727573)    68420 2021-11-10 15:47:25.000000 plink-2.4.1/plink_src/doc/_static/underscore-1.13.1.js
--rw-r--r--   0 nmd      (444129884) UOFI\Domain Users (1233727573)    35168 2020-11-09 03:35:31.000000 plink-2.4.1/plink_src/doc/_static/underscore-1.3.1.js
--rw-r--r--   0 nmd      (444129884) UOFI\Domain Users (1233727573)    19530 2021-11-10 15:47:25.000000 plink-2.4.1/plink_src/doc/_static/underscore.js
--rw-r--r--   0 nmd      (444129884) UOFI\Domain Users (1233727573)    14200 2021-11-10 15:47:31.000000 plink-2.4.1/plink_src/doc/genindex.html
--rw-r--r--   0 nmd      (444129884) UOFI\Domain Users (1233727573)    11016 2021-11-10 15:47:31.000000 plink-2.4.1/plink_src/doc/index.html
--rw-r--r--   0 nmd      (444129884) UOFI\Domain Users (1233727573)     7217 2021-11-10 15:47:31.000000 plink-2.4.1/plink_src/doc/installing.html
--rw-r--r--   0 nmd      (444129884) UOFI\Domain Users (1233727573)      786 2021-11-10 15:47:31.000000 plink-2.4.1/plink_src/doc/objects.inv
--rw-r--r--   0 nmd      (444129884) UOFI\Domain Users (1233727573)    33984 2021-11-10 15:47:31.000000 plink-2.4.1/plink_src/doc/plink.html
--rw-r--r--   0 nmd      (444129884) UOFI\Domain Users (1233727573)     4021 2021-11-10 15:47:31.000000 plink-2.4.1/plink_src/doc/py-modindex.html
--rw-r--r--   0 nmd      (444129884) UOFI\Domain Users (1233727573)     3392 2021-11-10 15:47:31.000000 plink-2.4.1/plink_src/doc/search.html
--rw-r--r--   0 nmd      (444129884) UOFI\Domain Users (1233727573)     6431 2021-11-10 15:47:31.000000 plink-2.4.1/plink_src/doc/searchindex.js
--rw-r--r--   0 nmd      (444129884) UOFI\Domain Users (1233727573)    50981 2020-08-17 22:05:38.000000 plink-2.4.1/plink_src/editor.py
--rw-r--r--   0 nmd      (444129884) UOFI\Domain Users (1233727573)     3831 2021-01-18 03:29:11.000000 plink-2.4.1/plink_src/gui.py
--rw-r--r--   0 nmd      (444129884) UOFI\Domain Users (1233727573)     3786 2021-02-24 02:14:23.000000 plink-2.4.1/plink_src/ipython_tools.py
--rw-r--r--   0 nmd      (444129884) UOFI\Domain Users (1233727573)    28031 2021-01-18 03:27:44.000000 plink-2.4.1/plink_src/manager.py
--rw-r--r--   0 nmd      (444129884) UOFI\Domain Users (1233727573)    13476 2020-02-11 16:06:51.000000 plink-2.4.1/plink_src/smooth.py
--rw-r--r--   0 nmd      (444129884) UOFI\Domain Users (1233727573)      680 2021-11-10 15:23:13.000000 plink-2.4.1/plink_src/version.py
--rw-r--r--   0 nmd      (444129884) UOFI\Domain Users (1233727573)     5860 2020-02-11 16:06:51.000000 plink-2.4.1/plink_src/vertex.py
--rw-r--r--   0 nmd      (444129884) UOFI\Domain Users (1233727573)     5342 2020-02-11 16:06:51.000000 plink-2.4.1/plink_src/viewer.py
--rw-r--r--   0 nmd      (444129884) UOFI\Domain Users (1233727573)       38 2021-11-10 15:47:32.423905 plink-2.4.1/setup.cfg
--rw-r--r--   0 nmd      (444129884) UOFI\Domain Users (1233727573)     5591 2021-11-10 15:44:14.000000 plink-2.4.1/setup.py
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-05-23 19:36:55.848146 plink-2.4.2/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1764 2023-05-23 19:36:55.848393 plink-2.4.2/PKG-INFO
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1125 2023-03-05 19:33:56.000000 plink-2.4.2/README.rst
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-05-23 19:36:55.813546 plink-2.4.2/plink.egg-info/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1764 2023-05-23 19:36:55.000000 plink-2.4.2/plink.egg-info/PKG-INFO
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1614 2023-05-23 19:36:55.000000 plink-2.4.2/plink.egg-info/SOURCES.txt
+-rw-r--r--   0 nmd      (444129884) staff       (20)        1 2023-05-23 19:36:55.000000 plink-2.4.2/plink.egg-info/dependency_links.txt
+-rw-r--r--   0 nmd      (444129884) staff       (20)       41 2023-05-23 19:36:55.000000 plink-2.4.2/plink.egg-info/entry_points.txt
+-rw-r--r--   0 nmd      (444129884) staff       (20)        1 2023-05-23 19:36:55.000000 plink-2.4.2/plink.egg-info/not-zip-safe
+-rw-r--r--   0 nmd      (444129884) staff       (20)        6 2023-05-23 19:36:55.000000 plink-2.4.2/plink.egg-info/top_level.txt
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-05-23 19:36:55.822856 plink-2.4.2/plink_src/
+-rw-r--r--   0 nmd      (444129884) staff       (20)      952 2020-02-11 16:06:51.000000 plink-2.4.2/plink_src/__init__.py
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1028 2020-02-11 16:06:51.000000 plink-2.4.2/plink_src/app.py
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8457 2020-02-11 16:06:51.000000 plink-2.4.2/plink_src/arrow.py
+-rw-r--r--   0 nmd      (444129884) staff       (20)    20501 2021-01-18 03:28:09.000000 plink-2.4.2/plink_src/canvasvg.py
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2457 2020-02-11 16:06:51.000000 plink-2.4.2/plink_src/colors.py
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4839 2022-11-23 22:15:42.000000 plink-2.4.2/plink_src/crossings.py
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2380 2020-02-11 16:06:51.000000 plink-2.4.2/plink_src/dialog.py
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-05-23 19:36:55.825935 plink-2.4.2/plink_src/doc/
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-05-23 19:36:55.826337 plink-2.4.2/plink_src/doc/_images/
+-rw-r--r--   0 nmd      (444129884) staff       (20)    34337 2020-02-11 16:06:51.000000 plink-2.4.2/plink_src/doc/_images/plink-action.png
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-05-23 19:36:55.828787 plink-2.4.2/plink_src/doc/_sources/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5554 2020-02-11 16:06:51.000000 plink-2.4.2/plink_src/doc/_sources/index.rst.txt
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1231 2020-08-17 22:05:38.000000 plink-2.4.2/plink_src/doc/_sources/installing.rst.txt
+-rw-r--r--   0 nmd      (444129884) staff       (20)      591 2020-02-11 16:06:51.000000 plink-2.4.2/plink_src/doc/_sources/plink.rst.txt
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-05-23 19:36:55.847458 plink-2.4.2/plink_src/doc/_static/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4418 2022-10-29 23:53:26.000000 plink-2.4.2/plink_src/doc/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--   0 nmd      (444129884) staff       (20)    14813 2023-05-23 19:35:39.000000 plink-2.4.2/plink_src/doc/_static/basic.css
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4302 2023-05-23 19:35:39.000000 plink-2.4.2/plink_src/doc/_static/classic.css
+-rw-r--r--   0 nmd      (444129884) staff       (20)       28 2022-03-10 03:05:24.000000 plink-2.4.2/plink_src/doc/_static/default.css
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4472 2023-04-17 20:58:02.000000 plink-2.4.2/plink_src/doc/_static/doctools.js
+-rw-r--r--   0 nmd      (444129884) staff       (20)      420 2023-05-23 19:35:39.000000 plink-2.4.2/plink_src/doc/_static/documentation_options.js
+-rw-r--r--   0 nmd      (444129884) staff       (20)      286 2022-03-10 03:05:24.000000 plink-2.4.2/plink_src/doc/_static/file.png
+-rw-r--r--   0 nmd      (444129884) staff       (20)   287630 2022-03-10 03:05:24.000000 plink-2.4.2/plink_src/doc/_static/jquery-3.5.1.js
+-rw-r--r--   0 nmd      (444129884) staff       (20)   288580 2022-10-29 23:53:26.000000 plink-2.4.2/plink_src/doc/_static/jquery-3.6.0.js
+-rw-r--r--   0 nmd      (444129884) staff       (20)    89501 2023-02-11 15:10:50.000000 plink-2.4.2/plink_src/doc/_static/jquery.js
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4758 2023-05-23 19:35:39.000000 plink-2.4.2/plink_src/doc/_static/language_data.js
+-rw-r--r--   0 nmd      (444129884) staff       (20)       90 2022-03-10 03:05:24.000000 plink-2.4.2/plink_src/doc/_static/minus.png
+-rw-r--r--   0 nmd      (444129884) staff       (20)       90 2022-03-10 03:05:24.000000 plink-2.4.2/plink_src/doc/_static/plus.png
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4846 2023-05-23 19:35:39.000000 plink-2.4.2/plink_src/doc/_static/pygments.css
+-rw-r--r--   0 nmd      (444129884) staff       (20)    18215 2023-04-17 20:58:02.000000 plink-2.4.2/plink_src/doc/_static/searchtools.js
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2540 2023-05-23 19:35:39.000000 plink-2.4.2/plink_src/doc/_static/sidebar.js
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4712 2022-10-29 23:53:26.000000 plink-2.4.2/plink_src/doc/_static/sphinx_highlight.js
+-rw-r--r--   0 nmd      (444129884) staff       (20)    68420 2022-03-10 03:05:24.000000 plink-2.4.2/plink_src/doc/_static/underscore-1.13.1.js
+-rw-r--r--   0 nmd      (444129884) staff       (20)    19530 2022-03-10 03:05:24.000000 plink-2.4.2/plink_src/doc/_static/underscore.js
+-rw-r--r--   0 nmd      (444129884) staff       (20)    14206 2023-05-23 19:35:39.000000 plink-2.4.2/plink_src/doc/genindex.html
+-rw-r--r--   0 nmd      (444129884) staff       (20)    11860 2023-05-23 19:35:38.000000 plink-2.4.2/plink_src/doc/index.html
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7340 2023-05-23 19:35:39.000000 plink-2.4.2/plink_src/doc/installing.html
+-rw-r--r--   0 nmd      (444129884) staff       (20)      786 2023-05-23 19:35:39.000000 plink-2.4.2/plink_src/doc/objects.inv
+-rw-r--r--   0 nmd      (444129884) staff       (20)    44767 2023-05-23 19:35:39.000000 plink-2.4.2/plink_src/doc/plink.html
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4027 2023-05-23 19:35:39.000000 plink-2.4.2/plink_src/doc/py-modindex.html
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3362 2023-05-23 19:35:39.000000 plink-2.4.2/plink_src/doc/search.html
+-rw-r--r--   0 nmd      (444129884) staff       (20)    14312 2023-05-23 19:35:39.000000 plink-2.4.2/plink_src/doc/searchindex.js
+-rw-r--r--   0 nmd      (444129884) staff       (20)    50981 2020-08-17 22:05:38.000000 plink-2.4.2/plink_src/editor.py
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3831 2021-01-18 03:29:11.000000 plink-2.4.2/plink_src/gui.py
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3786 2021-02-24 02:14:23.000000 plink-2.4.2/plink_src/ipython_tools.py
+-rw-r--r--   0 nmd      (444129884) staff       (20)    28299 2022-11-23 22:14:18.000000 plink-2.4.2/plink_src/manager.py
+-rw-r--r--   0 nmd      (444129884) staff       (20)    13476 2020-02-11 16:06:51.000000 plink-2.4.2/plink_src/smooth.py
+-rw-r--r--   0 nmd      (444129884) staff       (20)      680 2023-01-02 21:35:17.000000 plink-2.4.2/plink_src/version.py
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5860 2020-02-11 16:06:51.000000 plink-2.4.2/plink_src/vertex.py
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5342 2020-02-11 16:06:51.000000 plink-2.4.2/plink_src/viewer.py
+-rw-r--r--   0 nmd      (444129884) staff       (20)       99 2022-03-09 22:45:14.000000 plink-2.4.2/pyproject.toml
+-rw-r--r--   0 nmd      (444129884) staff       (20)      895 2023-05-23 19:36:55.849475 plink-2.4.2/setup.cfg
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3619 2023-05-23 16:19:22.000000 plink-2.4.2/setup.py
```

### Comparing `plink-2.4.1/PKG-INFO` & `plink-2.4.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,49 @@
 Metadata-Version: 2.1
 Name: plink
-Version: 2.4.1
+Version: 2.4.2
 Summary: A full featured Tk-based knot and link editor
-Home-page: https://www.math.uic.edu/t3m/plink/doc/
+Home-page: https://github.com/3-manifolds/PLink
 Author: Marc Culler and Nathan M. Dunfield
 Author-email: culler@uic.edu, nathan@dunfield.info
 License: GPLv2+
 Keywords: knot,link,editor,SnapPy
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Mathematics
-Requires-Python: >=3
 
 PLink is a full featured graphical editor for knot and link projections,
 using the cross-platform GUI toolkit Tk.  The primary focus is on
 piecewise-linear link projections, but it also supports a "smooth
 mode" and can export images in PostScript, PDF, SVG, and TikZ formats.
-See the `PLink home page <https://t3m.math.uic.edu/plink/doc>`_
+See the `PLink home page <https://3-manifolds.github.io/PLink>`_
 for complete details.
 
 This is a pure Python module and you can install it via
 `pip <https://pip.pypa.io/en/latest/>`_.
 See `the documentation
-<https://t3m.math.uic.edu/plink/doc/installing>`_
+<https://3-manifolds.github.io/PLink/installing>`_
 for more.
 
 You can browse the source code `here <https://github.com/3-manifolds/PLink>`_.
 
 
+License
+=======
 
+Copyright 2008-present by Marc Culler, Nathan Dunfield, and others.
 
+All parts of this package are released under the
+`GNU General Public License, version 2 <http://www.gnu.org/licenses/gpl-2.0.txt>`_
+or (at your discretion) any later version as
+published by the Free Software Foundation.
+
+
+Acknowledgements
+================
+
+The development of this program was partially supported by the US
+National Science Foundation under grants DMS0608567, DMS0504975,
+DMS0204142, and others.
```

### Comparing `plink-2.4.1/README.rst` & `plink-2.4.2/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 PLink is a full featured graphical editor for knot and link projections,
 using the cross-platform GUI toolkit Tk.  The primary focus is on
 piecewise-linear link projections, but it also supports a "smooth
 mode" and can export images in PostScript, PDF, SVG, and TikZ formats.
-See the `PLink home page <https://t3m.math.uic.edu/plink/doc>`_
+See the `PLink home page <https://3-manifolds.github.io/PLink>`_
 for complete details.
 
 This is a pure Python module and you can install it via
 `pip <https://pip.pypa.io/en/latest/>`_.
 See `the documentation
-<https://t3m.math.uic.edu/plink/doc/installing>`_
+<https://3-manifolds.github.io/PLink/installing>`_
 for more.
 
 You can browse the source code `here <https://github.com/3-manifolds/PLink>`_.
 
 
 License
-========================
+=======
 
 Copyright 2008-present by Marc Culler, Nathan Dunfield, and others.
 
 All parts of this package are released under the
 `GNU General Public License, version 2 <http://www.gnu.org/licenses/gpl-2.0.txt>`_
 or (at your discretion) any later version as
 published by the Free Software Foundation.
 
 
 Acknowledgements
-========================
+================
 
 The development of this program was partially supported by the US
 National Science Foundation under grants DMS0608567, DMS0504975,
 DMS0204142, and others.
```

### Comparing `plink-2.4.1/plink.egg-info/PKG-INFO` & `plink-2.4.2/plink.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,49 @@
 Metadata-Version: 2.1
 Name: plink
-Version: 2.4.1
+Version: 2.4.2
 Summary: A full featured Tk-based knot and link editor
-Home-page: https://www.math.uic.edu/t3m/plink/doc/
+Home-page: https://github.com/3-manifolds/PLink
 Author: Marc Culler and Nathan M. Dunfield
 Author-email: culler@uic.edu, nathan@dunfield.info
 License: GPLv2+
 Keywords: knot,link,editor,SnapPy
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Mathematics
-Requires-Python: >=3
 
 PLink is a full featured graphical editor for knot and link projections,
 using the cross-platform GUI toolkit Tk.  The primary focus is on
 piecewise-linear link projections, but it also supports a "smooth
 mode" and can export images in PostScript, PDF, SVG, and TikZ formats.
-See the `PLink home page <https://t3m.math.uic.edu/plink/doc>`_
+See the `PLink home page <https://3-manifolds.github.io/PLink>`_
 for complete details.
 
 This is a pure Python module and you can install it via
 `pip <https://pip.pypa.io/en/latest/>`_.
 See `the documentation
-<https://t3m.math.uic.edu/plink/doc/installing>`_
+<https://3-manifolds.github.io/PLink/installing>`_
 for more.
 
 You can browse the source code `here <https://github.com/3-manifolds/PLink>`_.
 
 
+License
+=======
 
+Copyright 2008-present by Marc Culler, Nathan Dunfield, and others.
 
+All parts of this package are released under the
+`GNU General Public License, version 2 <http://www.gnu.org/licenses/gpl-2.0.txt>`_
+or (at your discretion) any later version as
+published by the Free Software Foundation.
+
+
+Acknowledgements
+================
+
+The development of this program was partially supported by the US
+National Science Foundation under grants DMS0608567, DMS0504975,
+DMS0204142, and others.
```

### Comparing `plink-2.4.1/plink.egg-info/SOURCES.txt` & `plink-2.4.2/plink.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 README.rst
+pyproject.toml
+setup.cfg
 setup.py
 plink.egg-info/PKG-INFO
 plink.egg-info/SOURCES.txt
 plink.egg-info/dependency_links.txt
 plink.egg-info/entry_points.txt
 plink.egg-info/not-zip-safe
 plink.egg-info/top_level.txt
@@ -17,37 +19,38 @@
 plink_src/gui.py
 plink_src/ipython_tools.py
 plink_src/manager.py
 plink_src/smooth.py
 plink_src/version.py
 plink_src/vertex.py
 plink_src/viewer.py
-plink_src/doc/.buildinfo
 plink_src/doc/genindex.html
 plink_src/doc/index.html
 plink_src/doc/installing.html
 plink_src/doc/objects.inv
 plink_src/doc/plink.html
 plink_src/doc/py-modindex.html
 plink_src/doc/search.html
 plink_src/doc/searchindex.js
 plink_src/doc/_images/plink-action.png
 plink_src/doc/_sources/index.rst.txt
 plink_src/doc/_sources/installing.rst.txt
 plink_src/doc/_sources/plink.rst.txt
+plink_src/doc/_static/_sphinx_javascript_frameworks_compat.js
 plink_src/doc/_static/basic.css
 plink_src/doc/_static/classic.css
 plink_src/doc/_static/default.css
 plink_src/doc/_static/doctools.js
 plink_src/doc/_static/documentation_options.js
 plink_src/doc/_static/file.png
 plink_src/doc/_static/jquery-3.5.1.js
+plink_src/doc/_static/jquery-3.6.0.js
 plink_src/doc/_static/jquery.js
 plink_src/doc/_static/language_data.js
 plink_src/doc/_static/minus.png
 plink_src/doc/_static/plus.png
 plink_src/doc/_static/pygments.css
 plink_src/doc/_static/searchtools.js
 plink_src/doc/_static/sidebar.js
+plink_src/doc/_static/sphinx_highlight.js
 plink_src/doc/_static/underscore-1.13.1.js
-plink_src/doc/_static/underscore-1.3.1.js
 plink_src/doc/_static/underscore.js
```

### Comparing `plink-2.4.1/plink_src/__init__.py` & `plink-2.4.2/plink_src/__init__.py`

 * *Files identical despite different names*

### Comparing `plink-2.4.1/plink_src/app.py` & `plink-2.4.2/plink_src/app.py`

 * *Files identical despite different names*

### Comparing `plink-2.4.1/plink_src/arrow.py` & `plink-2.4.2/plink_src/arrow.py`

 * *Files identical despite different names*

### Comparing `plink-2.4.1/plink_src/canvasvg.py` & `plink-2.4.2/plink_src/canvasvg.py`

 * *Files identical despite different names*

### Comparing `plink-2.4.1/plink_src/colors.py` & `plink-2.4.2/plink_src/colors.py`

 * *Files identical despite different names*

### Comparing `plink-2.4.1/plink_src/crossings.py` & `plink-2.4.2/plink_src/crossings.py`

 * *Files identical despite different names*

### Comparing `plink-2.4.1/plink_src/dialog.py` & `plink-2.4.2/plink_src/dialog.py`

 * *Files identical despite different names*

### Comparing `plink-2.4.1/plink_src/doc/_images/plink-action.png` & `plink-2.4.2/plink_src/doc/_images/plink-action.png`

 * *Files identical despite different names*

### Comparing `plink-2.4.1/plink_src/doc/_sources/index.rst.txt` & `plink-2.4.2/plink_src/doc/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `plink-2.4.1/plink_src/doc/_sources/installing.rst.txt` & `plink-2.4.2/plink_src/doc/_sources/installing.rst.txt`

 * *Files identical despite different names*

### Comparing `plink-2.4.1/plink_src/doc/_sources/plink.rst.txt` & `plink-2.4.2/plink_src/doc/_sources/plink.rst.txt`

 * *Files identical despite different names*

### Comparing `plink-2.4.1/plink_src/doc/_static/basic.css` & `plink-2.4.2/plink_src/doc/_static/basic.css`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 /*
  * basic.css
  * ~~~~~~~~~
  *
  * Sphinx stylesheet -- basic theme.
  *
- * :copyright: Copyright 2007-2021 by the Sphinx team, see AUTHORS.
+ * :copyright: Copyright 2007-2023 by the Sphinx team, see AUTHORS.
  * :license: BSD, see LICENSE for details.
  *
  */
 
 /* -- main layout ----------------------------------------------------------- */
 
 div.clearer {
@@ -218,39 +218,29 @@
     padding: 2px;
     border-collapse: collapse;
 }
 
 /* -- general body styles --------------------------------------------------- */
 
 div.body {
-    min-width: 450px;
+    min-width: 360px;
     max-width: 800px;
 }
 
 div.body p, div.body dd, div.body li, div.body blockquote {
     -moz-hyphens: auto;
     -ms-hyphens: auto;
     -webkit-hyphens: auto;
     hyphens: auto;
 }
 
 a.headerlink {
     visibility: hidden;
 }
 
-a.brackets:before,
-span.brackets > a:before{
-    content: "[";
-}
-
-a.brackets:after,
-span.brackets > a:after {
-    content: "]";
-}
-
 h1:hover > a.headerlink,
 h2:hover > a.headerlink,
 h3:hover > a.headerlink,
 h4:hover > a.headerlink,
 h5:hover > a.headerlink,
 h6:hover > a.headerlink,
 dt:hover > a.headerlink,
@@ -331,20 +321,24 @@
     overflow-x: auto;
 }
 
 p.sidebar-title {
     font-weight: bold;
 }
 
+nav.contents,
+aside.topic,
 div.admonition, div.topic, blockquote {
     clear: left;
 }
 
 /* -- topics ---------------------------------------------------------------- */
 
+nav.contents,
+aside.topic,
 div.topic {
     border: 1px solid #ccc;
     padding: 7px;
     margin: 10px 0 10px 0;
 }
 
 p.topic-title {
@@ -375,21 +369,25 @@
     margin-top: 25px;
 }
 
 /* -- content of sidebars/topics/admonitions -------------------------------- */
 
 div.sidebar > :last-child,
 aside.sidebar > :last-child,
+nav.contents > :last-child,
+aside.topic > :last-child,
 div.topic > :last-child,
 div.admonition > :last-child {
     margin-bottom: 0;
 }
 
 div.sidebar::after,
 aside.sidebar::after,
+nav.contents::after,
+aside.topic::after,
 div.topic::after,
 div.admonition::after,
 blockquote::after {
     display: block;
     content: '';
     clear: both;
 }
@@ -424,18 +422,14 @@
     padding: 1px 8px 1px 5px;
     border-top: 0;
     border-left: 0;
     border-right: 0;
     border-bottom: 1px solid #aaa;
 }
 
-table.footnote td, table.footnote th {
-    border: 0 !important;
-}
-
 th {
     text-align: left;
     padding-right: 5px;
 }
 
 table.citation {
     border-left: solid 1px gray;
@@ -611,27 +605,34 @@
 }
 
 ol.simple p,
 ul.simple p {
     margin-bottom: 0;
 }
 
-dl.footnote > dt,
-dl.citation > dt {
+aside.footnote > span,
+div.citation > span {
     float: left;
-    margin-right: 0.5em;
 }
-
-dl.footnote > dd,
-dl.citation > dd {
+aside.footnote > span:last-of-type,
+div.citation > span:last-of-type {
+  padding-right: 0.5em;
+}
+aside.footnote > p {
+  margin-left: 2em;
+}
+div.citation > p {
+  margin-left: 4em;
+}
+aside.footnote > p:last-of-type,
+div.citation > p:last-of-type {
     margin-bottom: 0em;
 }
-
-dl.footnote > dd:after,
-dl.citation > dd:after {
+aside.footnote > p:last-of-type:after,
+div.citation > p:last-of-type:after {
     content: "";
     clear: both;
 }
 
 dl.field-list {
     display: grid;
     grid-template-columns: fit-content(30%) auto;
@@ -640,18 +641,14 @@
 dl.field-list > dt {
     font-weight: bold;
     word-break: break-word;
     padding-left: 0.5em;
     padding-right: 5px;
 }
 
-dl.field-list > dt:after {
-    content: ":";
-}
-
 dl.field-list > dd {
     padding-left: 0.5em;
     margin-top: 0em;
     margin-left: 0em;
     margin-bottom: 0em;
 }
 
@@ -727,16 +724,17 @@
 
 .classifier {
     font-style: oblique;
 }
 
 .classifier:before {
     font-style: normal;
-    margin: 0.5em;
+    margin: 0 0.5em;
     content: ":";
+    display: inline-block;
 }
 
 abbr, acronym {
     border-bottom: dotted 1px;
     cursor: help;
 }
 
@@ -752,14 +750,15 @@
 }
 
 span.pre {
     -moz-hyphens: none;
     -ms-hyphens: none;
     -webkit-hyphens: none;
     hyphens: none;
+    white-space: nowrap;
 }
 
 div[class*="highlight-"] {
     margin: 1em 0;
 }
 
 td.linenos pre {
```

### Comparing `plink-2.4.1/plink_src/doc/_static/classic.css` & `plink-2.4.2/plink_src/doc/_static/classic.css`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 /*
  * classic.css_t
  * ~~~~~~~~~~~~~
  *
  * Sphinx stylesheet -- classic theme.
  *
- * :copyright: Copyright 2007-2021 by the Sphinx team, see AUTHORS.
+ * :copyright: Copyright 2007-2023 by the Sphinx team, see AUTHORS.
  * :license: BSD, see LICENSE for details.
  *
  */
 
 @import url("basic.css");
 
 /* -- page layout ----------------------------------------------------------- */
@@ -24,14 +24,15 @@
     background-color: #11303d;
     color: #000;
     margin: 0;
     padding: 0;
 }
 
 div.document {
+    display: flex;
     background-color: #1c4e63;
 }
 
 div.documentwrapper {
     float: left;
     width: 100%;
 }
@@ -201,14 +202,16 @@
 }
 
 div.seealso {
     background-color: #ffc;
     border: 1px solid #ff6;
 }
 
+nav.contents,
+aside.topic,
 div.topic {
     background-color: #eee;
 }
 
 div.warning {
     background-color: #ffe4e4;
     border: 1px solid #f66;
```

### Comparing `plink-2.4.1/plink_src/doc/_static/jquery-3.5.1.js` & `plink-2.4.2/plink_src/doc/_static/jquery-3.5.1.js`

 * *Files identical despite different names*

### Comparing `plink-2.4.1/plink_src/doc/_static/jquery.js` & `plink-2.4.2/plink_src/doc/_static/jquery.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! jQuery v3.5.1 | (c) JS Foundation and other contributors | jquery.org/license */ ! function(e, t) {
+/*! jQuery v3.6.0 | (c) OpenJS Foundation and other contributors | jquery.org/license */ ! function(e, t) {
     "use strict";
     "object" == typeof module && "object" == typeof module.exports ? module.exports = e.document ? t(e, !0) : function(e) {
         if (!e.document) throw new Error("jQuery requires a window with a document");
         return t(e)
     } : t(e)
 }("undefined" != typeof window ? window : this, function(C, e) {
     "use strict";
@@ -19,15 +19,15 @@
         n = {},
         o = n.toString,
         v = n.hasOwnProperty,
         a = v.toString,
         l = a.call(Object),
         y = {},
         m = function(e) {
-            return "function" == typeof e && "number" != typeof e.nodeType
+            return "function" == typeof e && "number" != typeof e.nodeType && "function" != typeof e.item
         },
         x = function(e) {
             return null != e && e === e.window
         },
         E = C.document,
         c = {
             type: !0,
@@ -42,15 +42,15 @@
             for (r in c)(i = t[r] || t.getAttribute && t.getAttribute(r)) && o.setAttribute(r, i);
         n.head.appendChild(o).parentNode.removeChild(o)
     }
 
     function w(e) {
         return null == e ? e + "" : "object" == typeof e || "function" == typeof e ? n[o.call(e)] || "object" : typeof e
     }
-    var f = "3.5.1",
+    var f = "3.6.0",
         S = function(e, t) {
             return new S.fn.init(e, t)
         };
 
     function p(e) {
         var t = !!e && "length" in e && e.length,
             n = w(e);
@@ -182,18 +182,18 @@
             p = n.document,
             k = 0,
             r = 0,
             m = ue(),
             x = ue(),
             A = ue(),
             N = ue(),
-            D = function(e, t) {
+            j = function(e, t) {
                 return e === t && (l = !0), 0
             },
-            j = {}.hasOwnProperty,
+            D = {}.hasOwnProperty,
             t = [],
             q = t.pop,
             L = t.push,
             H = t.push,
             O = t.slice,
             P = function(e, t) {
                 for (var n = 0, r = e.length; n < r; n++)
@@ -360,16 +360,16 @@
             })
         }
 
         function ye(e) {
             return e && "undefined" != typeof e.getElementsByTagName && e
         }
         for (e in d = se.support = {}, i = se.isXML = function(e) {
-                var t = e.namespaceURI,
-                    n = (e.ownerDocument || e).documentElement;
+                var t = e && e.namespaceURI,
+                    n = e && (e.ownerDocument || e).documentElement;
                 return !Y.test(t || n && n.nodeName || "HTML")
             }, T = se.setDocument = function(e) {
                 var t, n, r = e ? e.ownerDocument || e : p;
                 return r != C && 9 === r.nodeType && r.documentElement && (a = (C = r).documentElement, E = !i(C), p != C && (n = C.defaultView) && n.top !== n && (n.addEventListener ? n.addEventListener("unload", oe, !1) : n.attachEvent && n.attachEvent("onunload", oe)), d.scope = ce(function(e) {
                     return a.appendChild(e).appendChild(C.createElement("div")), "undefined" != typeof e.querySelectorAll && !e.querySelectorAll(":scope fieldset div").length
                 }), d.attributes = ce(function(e) {
                     return e.className = "i", !e.getAttribute("className")
@@ -431,15 +431,15 @@
                         r = t && t.parentNode;
                     return e === r || !(!r || 1 !== r.nodeType || !(n.contains ? n.contains(r) : e.compareDocumentPosition && 16 & e.compareDocumentPosition(r)))
                 } : function(e, t) {
                     if (t)
                         while (t = t.parentNode)
                             if (t === e) return !0;
                     return !1
-                }, D = t ? function(e, t) {
+                }, j = t ? function(e, t) {
                     if (e === t) return l = !0, 0;
                     var n = !e.compareDocumentPosition - !t.compareDocumentPosition;
                     return n || (1 & (n = (e.ownerDocument || e) == (t.ownerDocument || t) ? e.compareDocumentPosition(t) : 1) || !d.sortDetached && t.compareDocumentPosition(e) === n ? e == C || e.ownerDocument == p && y(p, e) ? -1 : t == C || t.ownerDocument == p && y(p, t) ? 1 : u ? P(u, e) - P(u, t) : 0 : 4 & n ? -1 : 1)
                 } : function(e, t) {
                     if (e === t) return l = !0, 0;
                     var n, r = 0,
                         i = e.parentNode,
@@ -466,25 +466,25 @@
                 }
                 return 0 < se(t, C, null, [e]).length
             }, se.contains = function(e, t) {
                 return (e.ownerDocument || e) != C && T(e), y(e, t)
             }, se.attr = function(e, t) {
                 (e.ownerDocument || e) != C && T(e);
                 var n = b.attrHandle[t.toLowerCase()],
-                    r = n && j.call(b.attrHandle, t.toLowerCase()) ? n(e, t, !E) : void 0;
+                    r = n && D.call(b.attrHandle, t.toLowerCase()) ? n(e, t, !E) : void 0;
                 return void 0 !== r ? r : d.attributes || !E ? e.getAttribute(t) : (r = e.getAttributeNode(t)) && r.specified ? r.value : null
             }, se.escape = function(e) {
                 return (e + "").replace(re, ie)
             }, se.error = function(e) {
                 throw new Error("Syntax error, unrecognized expression: " + e)
             }, se.uniqueSort = function(e) {
                 var t, n = [],
                     r = 0,
                     i = 0;
-                if (l = !d.detectDuplicates, u = !d.sortStable && e.slice(0), e.sort(D), l) {
+                if (l = !d.detectDuplicates, u = !d.sortStable && e.slice(0), e.sort(j), l) {
                     while (t = e[i++]) t === e[i] && (r = n.push(i));
                     while (r--) e.splice(n[r], 1)
                 }
                 return u = null, e
             }, o = se.getText = function(e) {
                 var t, n = "",
                     r = 0,
@@ -880,15 +880,15 @@
                     if ((u = b.find[s]) && (r = u(a.matches[0].replace(te, ne), ee.test(o[0].type) && ye(t.parentNode) || t))) {
                         if (o.splice(i, 1), !(e = r.length && xe(o))) return H.apply(n, r), n;
                         break
                     }
                 }
             }
             return (l || f(e, c))(r, t, !E, n, !t || ee.test(e) && ye(t.parentNode) || t), n
-        }, d.sortStable = S.split("").sort(D).join("") === S, d.detectDuplicates = !!l, T(), d.sortDetached = ce(function(e) {
+        }, d.sortStable = S.split("").sort(j).join("") === S, d.detectDuplicates = !!l, T(), d.sortDetached = ce(function(e) {
             return 1 & e.compareDocumentPosition(C.createElement("fieldset"))
         }), ce(function(e) {
             return e.innerHTML = "<a href='#'></a>", "#" === e.firstChild.getAttribute("href")
         }) || fe("type|href|height|width", function(e, t, n) {
             if (!n) return e.getAttribute(t, "type" === t.toLowerCase() ? 1 : 2)
         }), d.attributes && ce(function(e) {
             return e.innerHTML = "<input/>", e.firstChild.setAttribute("value", ""), "" === e.firstChild.getAttribute("value")
@@ -918,15 +918,15 @@
         k = S.expr.match.needsContext;
 
     function A(e, t) {
         return e.nodeName && e.nodeName.toLowerCase() === t.toLowerCase()
     }
     var N = /^<([a-z][^\/\0>:\x20\t\r\n\f]*)[\x20\t\r\n\f]*\/?>(?:<\/\1>|)$/i;
 
-    function D(e, n, r) {
+    function j(e, n, r) {
         return m(n) ? S.grep(e, function(e, t) {
             return !!n.call(e, t, e) !== r
         }) : n.nodeType ? S.grep(e, function(e) {
             return e === n !== r
         }) : "string" != typeof n ? S.grep(e, function(e) {
             return -1 < i.call(n, e) !== r
         }) : S.filter(n, e, r)
@@ -944,38 +944,38 @@
                 for (t = 0; t < r; t++)
                     if (S.contains(i[t], this)) return !0
             }));
             for (n = this.pushStack([]), t = 0; t < r; t++) S.find(e, i[t], n);
             return 1 < r ? S.uniqueSort(n) : n
         },
         filter: function(e) {
-            return this.pushStack(D(this, e || [], !1))
+            return this.pushStack(j(this, e || [], !1))
         },
         not: function(e) {
-            return this.pushStack(D(this, e || [], !0))
+            return this.pushStack(j(this, e || [], !0))
         },
         is: function(e) {
-            return !!D(this, "string" == typeof e && k.test(e) ? S(e) : e || [], !1).length
+            return !!j(this, "string" == typeof e && k.test(e) ? S(e) : e || [], !1).length
         }
     });
-    var j, q = /^(?:\s*(<[\w\W]+>)[^>]*|#([\w-]+))$/;
+    var D, q = /^(?:\s*(<[\w\W]+>)[^>]*|#([\w-]+))$/;
     (S.fn.init = function(e, t, n) {
         var r, i;
         if (!e) return this;
-        if (n = n || j, "string" == typeof e) {
+        if (n = n || D, "string" == typeof e) {
             if (!(r = "<" === e[0] && ">" === e[e.length - 1] && 3 <= e.length ? [null, e, null] : q.exec(e)) || !r[1] && t) return !t || t.jquery ? (t || n).find(e) : this.constructor(t).find(e);
             if (r[1]) {
                 if (t = t instanceof S ? t[0] : t, S.merge(this, S.parseHTML(r[1], t && t.nodeType ? t.ownerDocument || t : E, !0)), N.test(r[1]) && S.isPlainObject(t))
                     for (r in t) m(this[r]) ? this[r](t[r]) : this.attr(r, t[r]);
                 return this
             }
             return (i = E.getElementById(r[2])) && (this[0] = i, this.length = 1), this
         }
         return e.nodeType ? (this[0] = e, this.length = 1, this) : m(e) ? void 0 !== n.ready ? n.ready(e) : e(S) : S.makeArray(e, this)
-    }).prototype = S.fn, j = S(E);
+    }).prototype = S.fn, D = S(E);
     var L = /^(?:parents|prev(?:Until|All))/,
         H = {
             children: !0,
             contents: !0,
             next: !0,
             prev: !0
         };
@@ -1514,72 +1514,70 @@
             if (r && -1 < S.inArray(o, r)) i && i.push(o);
             else if (l = ie(o), a = ve(f.appendChild(o), "script"), l && ye(a), n) {
             c = 0;
             while (o = a[c++]) he.test(o.type || "") && n.push(o)
         }
         return f
     }
-    var be = /^key/,
-        we = /^(?:mouse|pointer|contextmenu|drag|drop)|click/,
-        Te = /^([^.]*)(?:\.(.+)|)/;
+    var be = /^([^.]*)(?:\.(.+)|)/;
 
-    function Ce() {
+    function we() {
         return !0
     }
 
-    function Ee() {
+    function Te() {
         return !1
     }
 
-    function Se(e, t) {
+    function Ce(e, t) {
         return e === function() {
             try {
                 return E.activeElement
             } catch (e) {}
         }() == ("focus" === t)
     }
 
-    function ke(e, t, n, r, i, o) {
+    function Ee(e, t, n, r, i, o) {
         var a, s;
         if ("object" == typeof t) {
-            for (s in "string" != typeof n && (r = r || n, n = void 0), t) ke(e, s, n, r, t[s], o);
+            for (s in "string" != typeof n && (r = r || n, n = void 0), t) Ee(e, s, n, r, t[s], o);
             return e
         }
-        if (null == r && null == i ? (i = n, r = n = void 0) : null == i && ("string" == typeof n ? (i = r, r = void 0) : (i = r, r = n, n = void 0)), !1 === i) i = Ee;
+        if (null == r && null == i ? (i = n, r = n = void 0) : null == i && ("string" == typeof n ? (i = r, r = void 0) : (i = r, r = n, n = void 0)), !1 === i) i = Te;
         else if (!i) return e;
         return 1 === o && (a = i, (i = function(e) {
             return S().off(e), a.apply(this, arguments)
         }).guid = a.guid || (a.guid = S.guid++)), e.each(function() {
             S.event.add(this, t, i, r, n)
         })
     }
 
-    function Ae(e, i, o) {
+    function Se(e, i, o) {
         o ? (Y.set(e, i, !1), S.event.add(e, i, {
             namespace: !1,
             handler: function(e) {
                 var t, n, r = Y.get(this, i);
                 if (1 & e.isTrigger && this[i]) {
                     if (r.length)(S.event.special[i] || {}).delegateType && e.stopPropagation();
-                    else if (r = s.call(arguments), Y.set(this, i, r), t = o(this, i), this[i](), r !== (n = Y.get(this, i)) || t ? Y.set(this, i, !1) : n = {}, r !== n) return e.stopImmediatePropagation(), e.preventDefault(), n.value
+                    else if (r = s.call(arguments), Y.set(this, i, r), t = o(this, i), this[i](), r !== (n = Y.get(this, i)) || t ? Y.set(this, i, !1) : n = {}, r !== n) return e.stopImmediatePropagation(), e.preventDefault(), n && n.value
                 } else r.length && (Y.set(this, i, {
                     value: S.event.trigger(S.extend(r[0], S.Event.prototype), r.slice(1), this)
                 }), e.stopImmediatePropagation())
             }
-        })) : void 0 === Y.get(e, i) && S.event.add(e, i, Ce)
+        })) : void 0 === Y.get(e, i) && S.event.add(e, i, we)
     }
     S.event = {
         global: {},
         add: function(t, e, n, r, i) {
             var o, a, s, u, l, c, f, p, d, h, g, v = Y.get(t);
             if (V(t)) {
                 n.handler && (n = (o = n).handler, i = o.selector), i && S.find.matchesSelector(re, i), n.guid || (n.guid = S.guid++), (u = v.events) || (u = v.events = Object.create(null)), (a = v.handle) || (a = v.handle = function(e) {
                     return "undefined" != typeof S && S.event.triggered !== e.type ? S.event.dispatch.apply(t, arguments) : void 0
                 }), l = (e = (e || "").match(P) || [""]).length;
-                while (l--) d = g = (s = Te.exec(e[l]) || [])[1], h = (s[2] || "").split(".").sort(), d && (f = S.event.special[d] || {}, d = (i ? f.delegateType : f.bindType) || d, f = S.event.special[d] || {}, c = S.extend({
+                while (l--) d = g = (s = be.exec(e[l]) || [])[1], h = (s[2] || "").split(".").sort(), d && (f = S.event.special[d] || {}, d = (i ? f.delegateType : f.bindType) || d, f = S.event.special[d] || {}, c = S.extend({
                     type: d,
                     origType: g,
                     data: r,
                     handler: n,
                     guid: n.guid,
                     selector: i,
                     needsContext: i && S.expr.match.needsContext.test(i),
@@ -1588,15 +1586,15 @@
             }
         },
         remove: function(e, t, n, r, i) {
             var o, a, s, u, l, c, f, p, d, h, g, v = Y.hasData(e) && Y.get(e);
             if (v && (u = v.events)) {
                 l = (t = (t || "").match(P) || [""]).length;
                 while (l--)
-                    if (d = g = (s = Te.exec(t[l]) || [])[1], h = (s[2] || "").split(".").sort(), d) {
+                    if (d = g = (s = be.exec(t[l]) || [])[1], h = (s[2] || "").split(".").sort(), d) {
                         f = S.event.special[d] || {}, p = u[d = (r ? f.delegateType : f.bindType) || d] || [], s = s[2] && new RegExp("(^|\\.)" + h.join("\\.(?:.*\\.|)") + "(\\.|$)"), a = o = p.length;
                         while (o--) c = p[o], !i && g !== c.origType || n && n.guid !== c.guid || s && !s.test(c.namespace) || r && r !== c.selector && ("**" !== r || !c.selector) || (p.splice(o, 1), c.selector && p.delegateCount--, f.remove && f.remove.call(e, c));
                         a && !p.length && (f.teardown && !1 !== f.teardown.call(e, h, v.handle) || S.removeEvent(e, d, v.handle), delete u[d])
                     } else
                         for (d in u) S.event.remove(e, d + t[l], n, r, !0);
                 S.isEmptyObject(u) && Y.remove(e, "handle events")
             }
@@ -1658,19 +1656,19 @@
         special: {
             load: {
                 noBubble: !0
             },
             click: {
                 setup: function(e) {
                     var t = this || e;
-                    return pe.test(t.type) && t.click && A(t, "input") && Ae(t, "click", Ce), !1
+                    return pe.test(t.type) && t.click && A(t, "input") && Se(t, "click", we), !1
                 },
                 trigger: function(e) {
                     var t = this || e;
-                    return pe.test(t.type) && t.click && A(t, "input") && Ae(t, "click"), !0
+                    return pe.test(t.type) && t.click && A(t, "input") && Se(t, "click"), !0
                 },
                 _default: function(e) {
                     var t = e.target;
                     return pe.test(t.type) && t.click && A(t, "input") && Y.get(t, "click") || A(t, "a")
                 }
             },
             beforeunload: {
@@ -1679,32 +1677,32 @@
                 }
             }
         }
     }, S.removeEvent = function(e, t, n) {
         e.removeEventListener && e.removeEventListener(t, n)
     }, S.Event = function(e, t) {
         if (!(this instanceof S.Event)) return new S.Event(e, t);
-        e && e.type ? (this.originalEvent = e, this.type = e.type, this.isDefaultPrevented = e.defaultPrevented || void 0 === e.defaultPrevented && !1 === e.returnValue ? Ce : Ee, this.target = e.target && 3 === e.target.nodeType ? e.target.parentNode : e.target, this.currentTarget = e.currentTarget, this.relatedTarget = e.relatedTarget) : this.type = e, t && S.extend(this, t), this.timeStamp = e && e.timeStamp || Date.now(), this[S.expando] = !0
+        e && e.type ? (this.originalEvent = e, this.type = e.type, this.isDefaultPrevented = e.defaultPrevented || void 0 === e.defaultPrevented && !1 === e.returnValue ? we : Te, this.target = e.target && 3 === e.target.nodeType ? e.target.parentNode : e.target, this.currentTarget = e.currentTarget, this.relatedTarget = e.relatedTarget) : this.type = e, t && S.extend(this, t), this.timeStamp = e && e.timeStamp || Date.now(), this[S.expando] = !0
     }, S.Event.prototype = {
         constructor: S.Event,
-        isDefaultPrevented: Ee,
-        isPropagationStopped: Ee,
-        isImmediatePropagationStopped: Ee,
+        isDefaultPrevented: Te,
+        isPropagationStopped: Te,
+        isImmediatePropagationStopped: Te,
         isSimulated: !1,
         preventDefault: function() {
             var e = this.originalEvent;
-            this.isDefaultPrevented = Ce, e && !this.isSimulated && e.preventDefault()
+            this.isDefaultPrevented = we, e && !this.isSimulated && e.preventDefault()
         },
         stopPropagation: function() {
             var e = this.originalEvent;
-            this.isPropagationStopped = Ce, e && !this.isSimulated && e.stopPropagation()
+            this.isPropagationStopped = we, e && !this.isSimulated && e.stopPropagation()
         },
         stopImmediatePropagation: function() {
             var e = this.originalEvent;
-            this.isImmediatePropagationStopped = Ce, e && !this.isSimulated && e.stopImmediatePropagation(), this.stopPropagation()
+            this.isImmediatePropagationStopped = we, e && !this.isSimulated && e.stopImmediatePropagation(), this.stopPropagation()
         }
     }, S.each({
         altKey: !0,
         bubbles: !0,
         cancelable: !0,
         changedTouches: !0,
         ctrlKey: !0,
@@ -1729,28 +1727,28 @@
         pointerId: !0,
         pointerType: !0,
         screenX: !0,
         screenY: !0,
         targetTouches: !0,
         toElement: !0,
         touches: !0,
-        which: function(e) {
-            var t = e.button;
-            return null == e.which && be.test(e.type) ? null != e.charCode ? e.charCode : e.keyCode : !e.which && void 0 !== t && we.test(e.type) ? 1 & t ? 1 : 2 & t ? 3 : 4 & t ? 2 : 0 : e.which
-        }
+        which: !0
     }, S.event.addProp), S.each({
         focus: "focusin",
         blur: "focusout"
     }, function(e, t) {
         S.event.special[e] = {
             setup: function() {
-                return Ae(this, e, Se), !1
+                return Se(this, e, Ce), !1
             },
             trigger: function() {
-                return Ae(this, e), !0
+                return Se(this, e), !0
+            },
+            _default: function() {
+                return !0
             },
             delegateType: t
         }
     }), S.each({
         mouseenter: "mouseover",
         mouseleave: "mouseout",
         pointerenter: "pointerover",
@@ -1763,95 +1761,95 @@
                 var t, n = e.relatedTarget,
                     r = e.handleObj;
                 return n && (n === this || S.contains(this, n)) || (e.type = r.origType, t = r.handler.apply(this, arguments), e.type = i), t
             }
         }
     }), S.fn.extend({
         on: function(e, t, n, r) {
-            return ke(this, e, t, n, r)
+            return Ee(this, e, t, n, r)
         },
         one: function(e, t, n, r) {
-            return ke(this, e, t, n, r, 1)
+            return Ee(this, e, t, n, r, 1)
         },
         off: function(e, t, n) {
             var r, i;
             if (e && e.preventDefault && e.handleObj) return r = e.handleObj, S(e.delegateTarget).off(r.namespace ? r.origType + "." + r.namespace : r.origType, r.selector, r.handler), this;
             if ("object" == typeof e) {
                 for (i in e) this.off(i, t, e[i]);
                 return this
             }
-            return !1 !== t && "function" != typeof t || (n = t, t = void 0), !1 === n && (n = Ee), this.each(function() {
+            return !1 !== t && "function" != typeof t || (n = t, t = void 0), !1 === n && (n = Te), this.each(function() {
                 S.event.remove(this, e, n, t)
             })
         }
     });
-    var Ne = /<script|<style|<link/i,
-        De = /checked\s*(?:[^=]|=\s*.checked.)/i,
-        je = /^\s*<!(?:\[CDATA\[|--)|(?:\]\]|--)>\s*$/g;
+    var ke = /<script|<style|<link/i,
+        Ae = /checked\s*(?:[^=]|=\s*.checked.)/i,
+        Ne = /^\s*<!(?:\[CDATA\[|--)|(?:\]\]|--)>\s*$/g;
 
-    function qe(e, t) {
+    function je(e, t) {
         return A(e, "table") && A(11 !== t.nodeType ? t : t.firstChild, "tr") && S(e).children("tbody")[0] || e
     }
 
-    function Le(e) {
+    function De(e) {
         return e.type = (null !== e.getAttribute("type")) + "/" + e.type, e
     }
 
-    function He(e) {
+    function qe(e) {
         return "true/" === (e.type || "").slice(0, 5) ? e.type = e.type.slice(5) : e.removeAttribute("type"), e
     }
 
-    function Oe(e, t) {
+    function Le(e, t) {
         var n, r, i, o, a, s;
         if (1 === t.nodeType) {
             if (Y.hasData(e) && (s = Y.get(e).events))
                 for (i in Y.remove(t, "handle events"), s)
                     for (n = 0, r = s[i].length; n < r; n++) S.event.add(t, i, s[i][n]);
             Q.hasData(e) && (o = Q.access(e), a = S.extend({}, o), Q.set(t, a))
         }
     }
 
-    function Pe(n, r, i, o) {
+    function He(n, r, i, o) {
         r = g(r);
         var e, t, a, s, u, l, c = 0,
             f = n.length,
             p = f - 1,
             d = r[0],
             h = m(d);
-        if (h || 1 < f && "string" == typeof d && !y.checkClone && De.test(d)) return n.each(function(e) {
+        if (h || 1 < f && "string" == typeof d && !y.checkClone && Ae.test(d)) return n.each(function(e) {
             var t = n.eq(e);
-            h && (r[0] = d.call(this, e, t.html())), Pe(t, r, i, o)
+            h && (r[0] = d.call(this, e, t.html())), He(t, r, i, o)
         });
         if (f && (t = (e = xe(r, n[0].ownerDocument, !1, n, o)).firstChild, 1 === e.childNodes.length && (e = t), t || o)) {
-            for (s = (a = S.map(ve(e, "script"), Le)).length; c < f; c++) u = e, c !== p && (u = S.clone(u, !0, !0), s && S.merge(a, ve(u, "script"))), i.call(n[c], u, c);
+            for (s = (a = S.map(ve(e, "script"), De)).length; c < f; c++) u = e, c !== p && (u = S.clone(u, !0, !0), s && S.merge(a, ve(u, "script"))), i.call(n[c], u, c);
             if (s)
-                for (l = a[a.length - 1].ownerDocument, S.map(a, He), c = 0; c < s; c++) u = a[c], he.test(u.type || "") && !Y.access(u, "globalEval") && S.contains(l, u) && (u.src && "module" !== (u.type || "").toLowerCase() ? S._evalUrl && !u.noModule && S._evalUrl(u.src, {
+                for (l = a[a.length - 1].ownerDocument, S.map(a, qe), c = 0; c < s; c++) u = a[c], he.test(u.type || "") && !Y.access(u, "globalEval") && S.contains(l, u) && (u.src && "module" !== (u.type || "").toLowerCase() ? S._evalUrl && !u.noModule && S._evalUrl(u.src, {
                     nonce: u.nonce || u.getAttribute("nonce")
-                }, l) : b(u.textContent.replace(je, ""), u, l))
+                }, l) : b(u.textContent.replace(Ne, ""), u, l))
         }
         return n
     }
 
-    function Re(e, t, n) {
+    function Oe(e, t, n) {
         for (var r, i = t ? S.filter(t, e) : e, o = 0; null != (r = i[o]); o++) n || 1 !== r.nodeType || S.cleanData(ve(r)), r.parentNode && (n && ie(r) && ye(ve(r, "script")), r.parentNode.removeChild(r));
         return e
     }
     S.extend({
         htmlPrefilter: function(e) {
             return e
         },
         clone: function(e, t, n) {
             var r, i, o, a, s, u, l, c = e.cloneNode(!0),
                 f = ie(e);
             if (!(y.noCloneChecked || 1 !== e.nodeType && 11 !== e.nodeType || S.isXMLDoc(e)))
                 for (a = ve(c), r = 0, i = (o = ve(e)).length; r < i; r++) s = o[r], u = a[r], void 0, "input" === (l = u.nodeName.toLowerCase()) && pe.test(s.type) ? u.checked = s.checked : "input" !== l && "textarea" !== l || (u.defaultValue = s.defaultValue);
             if (t)
                 if (n)
-                    for (o = o || ve(e), a = a || ve(c), r = 0, i = o.length; r < i; r++) Oe(o[r], a[r]);
-                else Oe(e, c);
+                    for (o = o || ve(e), a = a || ve(c), r = 0, i = o.length; r < i; r++) Le(o[r], a[r]);
+                else Le(e, c);
             return 0 < (a = ve(c, "script")).length && ye(a, !f && ve(e, "script")), c
         },
         cleanData: function(e) {
             for (var t, n, r, i = S.event.special, o = 0; void 0 !== (n = e[o]); o++)
                 if (V(n)) {
                     if (t = n[Y.expando]) {
                         if (t.events)
@@ -1859,46 +1857,46 @@
                         n[Y.expando] = void 0
                     }
                     n[Q.expando] && (n[Q.expando] = void 0)
                 }
         }
     }), S.fn.extend({
         detach: function(e) {
-            return Re(this, e, !0)
+            return Oe(this, e, !0)
         },
         remove: function(e) {
-            return Re(this, e)
+            return Oe(this, e)
         },
         text: function(e) {
             return $(this, function(e) {
                 return void 0 === e ? S.text(this) : this.empty().each(function() {
                     1 !== this.nodeType && 11 !== this.nodeType && 9 !== this.nodeType || (this.textContent = e)
                 })
             }, null, e, arguments.length)
         },
         append: function() {
-            return Pe(this, arguments, function(e) {
-                1 !== this.nodeType && 11 !== this.nodeType && 9 !== this.nodeType || qe(this, e).appendChild(e)
+            return He(this, arguments, function(e) {
+                1 !== this.nodeType && 11 !== this.nodeType && 9 !== this.nodeType || je(this, e).appendChild(e)
             })
         },
         prepend: function() {
-            return Pe(this, arguments, function(e) {
+            return He(this, arguments, function(e) {
                 if (1 === this.nodeType || 11 === this.nodeType || 9 === this.nodeType) {
-                    var t = qe(this, e);
+                    var t = je(this, e);
                     t.insertBefore(e, t.firstChild)
                 }
             })
         },
         before: function() {
-            return Pe(this, arguments, function(e) {
+            return He(this, arguments, function(e) {
                 this.parentNode && this.parentNode.insertBefore(e, this)
             })
         },
         after: function() {
-            return Pe(this, arguments, function(e) {
+            return He(this, arguments, function(e) {
                 this.parentNode && this.parentNode.insertBefore(e, this.nextSibling)
             })
         },
         empty: function() {
             for (var e, t = 0; null != (e = this[t]); t++) 1 === e.nodeType && (S.cleanData(ve(e, !1)), e.textContent = "");
             return this
         },
@@ -1909,27 +1907,27 @@
         },
         html: function(e) {
             return $(this, function(e) {
                 var t = this[0] || {},
                     n = 0,
                     r = this.length;
                 if (void 0 === e && 1 === t.nodeType) return t.innerHTML;
-                if ("string" == typeof e && !Ne.test(e) && !ge[(de.exec(e) || ["", ""])[1].toLowerCase()]) {
+                if ("string" == typeof e && !ke.test(e) && !ge[(de.exec(e) || ["", ""])[1].toLowerCase()]) {
                     e = S.htmlPrefilter(e);
                     try {
                         for (; n < r; n++) 1 === (t = this[n] || {}).nodeType && (S.cleanData(ve(t, !1)), t.innerHTML = e);
                         t = 0
                     } catch (e) {}
                 }
                 t && this.empty().append(e)
             }, null, e, arguments.length)
         },
         replaceWith: function() {
             var n = [];
-            return Pe(this, arguments, function(e) {
+            return He(this, arguments, function(e) {
                 var t = this.parentNode;
                 S.inArray(this, n) < 0 && (S.cleanData(ve(this)), t && t.replaceChild(e, this))
             }, n)
         }
     }), S.each({
         appendTo: "append",
         prependTo: "prepend",
@@ -1938,33 +1936,33 @@
         replaceAll: "replaceWith"
     }, function(e, a) {
         S.fn[e] = function(e) {
             for (var t, n = [], r = S(e), i = r.length - 1, o = 0; o <= i; o++) t = o === i ? this : this.clone(!0), S(r[o])[a](t), u.apply(n, t.get());
             return this.pushStack(n)
         }
     });
-    var Me = new RegExp("^(" + ee + ")(?!px)[a-z%]+$", "i"),
-        Ie = function(e) {
+    var Pe = new RegExp("^(" + ee + ")(?!px)[a-z%]+$", "i"),
+        Re = function(e) {
             var t = e.ownerDocument.defaultView;
             return t && t.opener || (t = C), t.getComputedStyle(e)
         },
-        We = function(e, t, n) {
+        Me = function(e, t, n) {
             var r, i, o = {};
             for (i in t) o[i] = e.style[i], e.style[i] = t[i];
             for (i in r = n.call(e), t) e.style[i] = o[i];
             return r
         },
-        Fe = new RegExp(ne.join("|"), "i");
+        Ie = new RegExp(ne.join("|"), "i");
 
-    function Be(e, t, n) {
+    function We(e, t, n) {
         var r, i, o, a, s = e.style;
-        return (n = n || Ie(e)) && ("" !== (a = n.getPropertyValue(t) || n[t]) || ie(e) || (a = S.style(e, t)), !y.pixelBoxStyles() && Me.test(a) && Fe.test(t) && (r = s.width, i = s.minWidth, o = s.maxWidth, s.minWidth = s.maxWidth = s.width = a, a = n.width, s.width = r, s.minWidth = i, s.maxWidth = o)), void 0 !== a ? a + "" : a
+        return (n = n || Re(e)) && ("" !== (a = n.getPropertyValue(t) || n[t]) || ie(e) || (a = S.style(e, t)), !y.pixelBoxStyles() && Pe.test(a) && Ie.test(t) && (r = s.width, i = s.minWidth, o = s.maxWidth, s.minWidth = s.maxWidth = s.width = a, a = n.width, s.width = r, s.minWidth = i, s.maxWidth = o)), void 0 !== a ? a + "" : a
     }
 
-    function $e(e, t) {
+    function Fe(e, t) {
         return {
             get: function() {
                 if (!e()) return (this.get = t).apply(this, arguments);
                 delete this.get
             }
         }
     }! function() {
@@ -1995,79 +1993,79 @@
                 return e(), s
             },
             scrollboxSize: function() {
                 return e(), i
             },
             reliableTrDimensions: function() {
                 var e, t, n, r;
-                return null == a && (e = E.createElement("table"), t = E.createElement("tr"), n = E.createElement("div"), e.style.cssText = "position:absolute;left:-11111px", t.style.height = "1px", n.style.height = "9px", re.appendChild(e).appendChild(t).appendChild(n), r = C.getComputedStyle(t), a = 3 < parseInt(r.height), re.removeChild(e)), a
+                return null == a && (e = E.createElement("table"), t = E.createElement("tr"), n = E.createElement("div"), e.style.cssText = "position:absolute;left:-11111px;border-collapse:separate", t.style.cssText = "border:1px solid", t.style.height = "1px", n.style.height = "9px", n.style.display = "block", re.appendChild(e).appendChild(t).appendChild(n), r = C.getComputedStyle(t), a = parseInt(r.height, 10) + parseInt(r.borderTopWidth, 10) + parseInt(r.borderBottomWidth, 10) === t.offsetHeight, re.removeChild(e)), a
             }
         }))
     }();
-    var _e = ["Webkit", "Moz", "ms"],
-        ze = E.createElement("div").style,
-        Ue = {};
-
-    function Xe(e) {
-        var t = S.cssProps[e] || Ue[e];
-        return t || (e in ze ? e : Ue[e] = function(e) {
+    var Be = ["Webkit", "Moz", "ms"],
+        $e = E.createElement("div").style,
+        _e = {};
+
+    function ze(e) {
+        var t = S.cssProps[e] || _e[e];
+        return t || (e in $e ? e : _e[e] = function(e) {
             var t = e[0].toUpperCase() + e.slice(1),
-                n = _e.length;
+                n = Be.length;
             while (n--)
-                if ((e = _e[n] + t) in ze) return e
+                if ((e = Be[n] + t) in $e) return e
         }(e) || e)
     }
-    var Ve = /^(none|table(?!-c[ea]).+)/,
-        Ge = /^--/,
-        Ye = {
+    var Ue = /^(none|table(?!-c[ea]).+)/,
+        Xe = /^--/,
+        Ve = {
             position: "absolute",
             visibility: "hidden",
             display: "block"
         },
-        Qe = {
+        Ge = {
             letterSpacing: "0",
             fontWeight: "400"
         };
 
-    function Je(e, t, n) {
+    function Ye(e, t, n) {
         var r = te.exec(t);
         return r ? Math.max(0, r[2] - (n || 0)) + (r[3] || "px") : t
     }
 
-    function Ke(e, t, n, r, i, o) {
+    function Qe(e, t, n, r, i, o) {
         var a = "width" === t ? 1 : 0,
             s = 0,
             u = 0;
         if (n === (r ? "border" : "content")) return 0;
         for (; a < 4; a += 2) "margin" === n && (u += S.css(e, n + ne[a], !0, i)), r ? ("content" === n && (u -= S.css(e, "padding" + ne[a], !0, i)), "margin" !== n && (u -= S.css(e, "border" + ne[a] + "Width", !0, i))) : (u += S.css(e, "padding" + ne[a], !0, i), "padding" !== n ? u += S.css(e, "border" + ne[a] + "Width", !0, i) : s += S.css(e, "border" + ne[a] + "Width", !0, i));
         return !r && 0 <= o && (u += Math.max(0, Math.ceil(e["offset" + t[0].toUpperCase() + t.slice(1)] - o - u - s - .5)) || 0), u
     }
 
-    function Ze(e, t, n) {
-        var r = Ie(e),
+    function Je(e, t, n) {
+        var r = Re(e),
             i = (!y.boxSizingReliable() || n) && "border-box" === S.css(e, "boxSizing", !1, r),
             o = i,
-            a = Be(e, t, r),
+            a = We(e, t, r),
             s = "offset" + t[0].toUpperCase() + t.slice(1);
-        if (Me.test(a)) {
+        if (Pe.test(a)) {
             if (!n) return a;
             a = "auto"
         }
-        return (!y.boxSizingReliable() && i || !y.reliableTrDimensions() && A(e, "tr") || "auto" === a || !parseFloat(a) && "inline" === S.css(e, "display", !1, r)) && e.getClientRects().length && (i = "border-box" === S.css(e, "boxSizing", !1, r), (o = s in e) && (a = e[s])), (a = parseFloat(a) || 0) + Ke(e, t, n || (i ? "border" : "content"), o, r, a) + "px"
+        return (!y.boxSizingReliable() && i || !y.reliableTrDimensions() && A(e, "tr") || "auto" === a || !parseFloat(a) && "inline" === S.css(e, "display", !1, r)) && e.getClientRects().length && (i = "border-box" === S.css(e, "boxSizing", !1, r), (o = s in e) && (a = e[s])), (a = parseFloat(a) || 0) + Qe(e, t, n || (i ? "border" : "content"), o, r, a) + "px"
     }
 
-    function et(e, t, n, r, i) {
-        return new et.prototype.init(e, t, n, r, i)
+    function Ke(e, t, n, r, i) {
+        return new Ke.prototype.init(e, t, n, r, i)
     }
     S.extend({
         cssHooks: {
             opacity: {
                 get: function(e, t) {
                     if (t) {
-                        var n = Be(e, "opacity");
+                        var n = We(e, "opacity");
                         return "" === n ? "1" : n
                     }
                 }
             }
         },
         cssNumber: {
             animationIterationCount: !0,
@@ -2091,152 +2089,152 @@
             zIndex: !0,
             zoom: !0
         },
         cssProps: {},
         style: function(e, t, n, r) {
             if (e && 3 !== e.nodeType && 8 !== e.nodeType && e.style) {
                 var i, o, a, s = X(t),
-                    u = Ge.test(t),
+                    u = Xe.test(t),
                     l = e.style;
-                if (u || (t = Xe(s)), a = S.cssHooks[t] || S.cssHooks[s], void 0 === n) return a && "get" in a && void 0 !== (i = a.get(e, !1, r)) ? i : l[t];
+                if (u || (t = ze(s)), a = S.cssHooks[t] || S.cssHooks[s], void 0 === n) return a && "get" in a && void 0 !== (i = a.get(e, !1, r)) ? i : l[t];
                 "string" === (o = typeof n) && (i = te.exec(n)) && i[1] && (n = se(e, t, i), o = "number"), null != n && n == n && ("number" !== o || u || (n += i && i[3] || (S.cssNumber[s] ? "" : "px")), y.clearCloneStyle || "" !== n || 0 !== t.indexOf("background") || (l[t] = "inherit"), a && "set" in a && void 0 === (n = a.set(e, n, r)) || (u ? l.setProperty(t, n) : l[t] = n))
             }
         },
         css: function(e, t, n, r) {
             var i, o, a, s = X(t);
-            return Ge.test(t) || (t = Xe(s)), (a = S.cssHooks[t] || S.cssHooks[s]) && "get" in a && (i = a.get(e, !0, n)), void 0 === i && (i = Be(e, t, r)), "normal" === i && t in Qe && (i = Qe[t]), "" === n || n ? (o = parseFloat(i), !0 === n || isFinite(o) ? o || 0 : i) : i
+            return Xe.test(t) || (t = ze(s)), (a = S.cssHooks[t] || S.cssHooks[s]) && "get" in a && (i = a.get(e, !0, n)), void 0 === i && (i = We(e, t, r)), "normal" === i && t in Ge && (i = Ge[t]), "" === n || n ? (o = parseFloat(i), !0 === n || isFinite(o) ? o || 0 : i) : i
         }
     }), S.each(["height", "width"], function(e, u) {
         S.cssHooks[u] = {
             get: function(e, t, n) {
-                if (t) return !Ve.test(S.css(e, "display")) || e.getClientRects().length && e.getBoundingClientRect().width ? Ze(e, u, n) : We(e, Ye, function() {
-                    return Ze(e, u, n)
+                if (t) return !Ue.test(S.css(e, "display")) || e.getClientRects().length && e.getBoundingClientRect().width ? Je(e, u, n) : Me(e, Ve, function() {
+                    return Je(e, u, n)
                 })
             },
             set: function(e, t, n) {
-                var r, i = Ie(e),
+                var r, i = Re(e),
                     o = !y.scrollboxSize() && "absolute" === i.position,
                     a = (o || n) && "border-box" === S.css(e, "boxSizing", !1, i),
-                    s = n ? Ke(e, u, n, a, i) : 0;
-                return a && o && (s -= Math.ceil(e["offset" + u[0].toUpperCase() + u.slice(1)] - parseFloat(i[u]) - Ke(e, u, "border", !1, i) - .5)), s && (r = te.exec(t)) && "px" !== (r[3] || "px") && (e.style[u] = t, t = S.css(e, u)), Je(0, t, s)
+                    s = n ? Qe(e, u, n, a, i) : 0;
+                return a && o && (s -= Math.ceil(e["offset" + u[0].toUpperCase() + u.slice(1)] - parseFloat(i[u]) - Qe(e, u, "border", !1, i) - .5)), s && (r = te.exec(t)) && "px" !== (r[3] || "px") && (e.style[u] = t, t = S.css(e, u)), Ye(0, t, s)
             }
         }
-    }), S.cssHooks.marginLeft = $e(y.reliableMarginLeft, function(e, t) {
-        if (t) return (parseFloat(Be(e, "marginLeft")) || e.getBoundingClientRect().left - We(e, {
+    }), S.cssHooks.marginLeft = Fe(y.reliableMarginLeft, function(e, t) {
+        if (t) return (parseFloat(We(e, "marginLeft")) || e.getBoundingClientRect().left - Me(e, {
             marginLeft: 0
         }, function() {
             return e.getBoundingClientRect().left
         })) + "px"
     }), S.each({
         margin: "",
         padding: "",
         border: "Width"
     }, function(i, o) {
         S.cssHooks[i + o] = {
             expand: function(e) {
                 for (var t = 0, n = {}, r = "string" == typeof e ? e.split(" ") : [e]; t < 4; t++) n[i + ne[t] + o] = r[t] || r[t - 2] || r[0];
                 return n
             }
-        }, "margin" !== i && (S.cssHooks[i + o].set = Je)
+        }, "margin" !== i && (S.cssHooks[i + o].set = Ye)
     }), S.fn.extend({
         css: function(e, t) {
             return $(this, function(e, t, n) {
                 var r, i, o = {},
                     a = 0;
                 if (Array.isArray(t)) {
-                    for (r = Ie(e), i = t.length; a < i; a++) o[t[a]] = S.css(e, t[a], !1, r);
+                    for (r = Re(e), i = t.length; a < i; a++) o[t[a]] = S.css(e, t[a], !1, r);
                     return o
                 }
                 return void 0 !== n ? S.style(e, t, n) : S.css(e, t)
             }, e, t, 1 < arguments.length)
         }
-    }), ((S.Tween = et).prototype = {
-        constructor: et,
+    }), ((S.Tween = Ke).prototype = {
+        constructor: Ke,
         init: function(e, t, n, r, i, o) {
             this.elem = e, this.prop = n, this.easing = i || S.easing._default, this.options = t, this.start = this.now = this.cur(), this.end = r, this.unit = o || (S.cssNumber[n] ? "" : "px")
         },
         cur: function() {
-            var e = et.propHooks[this.prop];
-            return e && e.get ? e.get(this) : et.propHooks._default.get(this)
+            var e = Ke.propHooks[this.prop];
+            return e && e.get ? e.get(this) : Ke.propHooks._default.get(this)
         },
         run: function(e) {
-            var t, n = et.propHooks[this.prop];
-            return this.options.duration ? this.pos = t = S.easing[this.easing](e, this.options.duration * e, 0, 1, this.options.duration) : this.pos = t = e, this.now = (this.end - this.start) * t + this.start, this.options.step && this.options.step.call(this.elem, this.now, this), n && n.set ? n.set(this) : et.propHooks._default.set(this), this
+            var t, n = Ke.propHooks[this.prop];
+            return this.options.duration ? this.pos = t = S.easing[this.easing](e, this.options.duration * e, 0, 1, this.options.duration) : this.pos = t = e, this.now = (this.end - this.start) * t + this.start, this.options.step && this.options.step.call(this.elem, this.now, this), n && n.set ? n.set(this) : Ke.propHooks._default.set(this), this
         }
-    }).init.prototype = et.prototype, (et.propHooks = {
+    }).init.prototype = Ke.prototype, (Ke.propHooks = {
         _default: {
             get: function(e) {
                 var t;
                 return 1 !== e.elem.nodeType || null != e.elem[e.prop] && null == e.elem.style[e.prop] ? e.elem[e.prop] : (t = S.css(e.elem, e.prop, "")) && "auto" !== t ? t : 0
             },
             set: function(e) {
-                S.fx.step[e.prop] ? S.fx.step[e.prop](e) : 1 !== e.elem.nodeType || !S.cssHooks[e.prop] && null == e.elem.style[Xe(e.prop)] ? e.elem[e.prop] = e.now : S.style(e.elem, e.prop, e.now + e.unit)
+                S.fx.step[e.prop] ? S.fx.step[e.prop](e) : 1 !== e.elem.nodeType || !S.cssHooks[e.prop] && null == e.elem.style[ze(e.prop)] ? e.elem[e.prop] = e.now : S.style(e.elem, e.prop, e.now + e.unit)
             }
         }
-    }).scrollTop = et.propHooks.scrollLeft = {
+    }).scrollTop = Ke.propHooks.scrollLeft = {
         set: function(e) {
             e.elem.nodeType && e.elem.parentNode && (e.elem[e.prop] = e.now)
         }
     }, S.easing = {
         linear: function(e) {
             return e
         },
         swing: function(e) {
             return .5 - Math.cos(e * Math.PI) / 2
         },
         _default: "swing"
-    }, S.fx = et.prototype.init, S.fx.step = {};
-    var tt, nt, rt, it, ot = /^(?:toggle|show|hide)$/,
-        at = /queueHooks$/;
+    }, S.fx = Ke.prototype.init, S.fx.step = {};
+    var Ze, et, tt, nt, rt = /^(?:toggle|show|hide)$/,
+        it = /queueHooks$/;
 
-    function st() {
-        nt && (!1 === E.hidden && C.requestAnimationFrame ? C.requestAnimationFrame(st) : C.setTimeout(st, S.fx.interval), S.fx.tick())
+    function ot() {
+        et && (!1 === E.hidden && C.requestAnimationFrame ? C.requestAnimationFrame(ot) : C.setTimeout(ot, S.fx.interval), S.fx.tick())
     }
 
-    function ut() {
+    function at() {
         return C.setTimeout(function() {
-            tt = void 0
-        }), tt = Date.now()
+            Ze = void 0
+        }), Ze = Date.now()
     }
 
-    function lt(e, t) {
+    function st(e, t) {
         var n, r = 0,
             i = {
                 height: e
             };
         for (t = t ? 1 : 0; r < 4; r += 2 - t) i["margin" + (n = ne[r])] = i["padding" + n] = e;
         return t && (i.opacity = i.width = e), i
     }
 
-    function ct(e, t, n) {
-        for (var r, i = (ft.tweeners[t] || []).concat(ft.tweeners["*"]), o = 0, a = i.length; o < a; o++)
+    function ut(e, t, n) {
+        for (var r, i = (lt.tweeners[t] || []).concat(lt.tweeners["*"]), o = 0, a = i.length; o < a; o++)
             if (r = i[o].call(n, t, e)) return r
     }
 
-    function ft(o, e, t) {
+    function lt(o, e, t) {
         var n, a, r = 0,
-            i = ft.prefilters.length,
+            i = lt.prefilters.length,
             s = S.Deferred().always(function() {
                 delete u.elem
             }),
             u = function() {
                 if (a) return !1;
-                for (var e = tt || ut(), t = Math.max(0, l.startTime + l.duration - e), n = 1 - (t / l.duration || 0), r = 0, i = l.tweens.length; r < i; r++) l.tweens[r].run(n);
+                for (var e = Ze || at(), t = Math.max(0, l.startTime + l.duration - e), n = 1 - (t / l.duration || 0), r = 0, i = l.tweens.length; r < i; r++) l.tweens[r].run(n);
                 return s.notifyWith(o, [l, n, t]), n < 1 && i ? t : (i || s.notifyWith(o, [l, 1, 0]), s.resolveWith(o, [l]), !1)
             },
             l = s.promise({
                 elem: o,
                 props: S.extend({}, e),
                 opts: S.extend(!0, {
                     specialEasing: {},
                     easing: S.easing._default
                 }, t),
                 originalProperties: e,
                 originalOptions: t,
-                startTime: tt || ut(),
+                startTime: Ze || at(),
                 duration: t.duration,
                 tweens: [],
                 createTween: function(e, t) {
                     var n = S.Tween(o, l.opts, e, t, l.opts.specialEasing[e] || l.opts.easing);
                     return l.tweens.push(n), n
                 },
                 stop: function(e) {
@@ -2251,31 +2249,31 @@
         for (! function(e, t) {
                 var n, r, i, o, a;
                 for (n in e)
                     if (i = t[r = X(n)], o = e[n], Array.isArray(o) && (i = o[1], o = e[n] = o[0]), n !== r && (e[r] = o, delete e[n]), (a = S.cssHooks[r]) && "expand" in a)
                         for (n in o = a.expand(o), delete e[r], o) n in e || (e[n] = o[n], t[n] = i);
                     else t[r] = i
             }(c, l.opts.specialEasing); r < i; r++)
-            if (n = ft.prefilters[r].call(l, o, c, l.opts)) return m(n.stop) && (S._queueHooks(l.elem, l.opts.queue).stop = n.stop.bind(n)), n;
-        return S.map(c, ct, l), m(l.opts.start) && l.opts.start.call(o, l), l.progress(l.opts.progress).done(l.opts.done, l.opts.complete).fail(l.opts.fail).always(l.opts.always), S.fx.timer(S.extend(u, {
+            if (n = lt.prefilters[r].call(l, o, c, l.opts)) return m(n.stop) && (S._queueHooks(l.elem, l.opts.queue).stop = n.stop.bind(n)), n;
+        return S.map(c, ut, l), m(l.opts.start) && l.opts.start.call(o, l), l.progress(l.opts.progress).done(l.opts.done, l.opts.complete).fail(l.opts.fail).always(l.opts.always), S.fx.timer(S.extend(u, {
             elem: o,
             anim: l,
             queue: l.opts.queue
         })), l
     }
-    S.Animation = S.extend(ft, {
+    S.Animation = S.extend(lt, {
         tweeners: {
             "*": [function(e, t) {
                 var n = this.createTween(e, t);
                 return se(n.elem, e, te.exec(t), n), n
             }]
         },
         tweener: function(e, t) {
             m(e) ? (t = e, e = ["*"]) : e = e.match(P);
-            for (var n, r = 0, i = e.length; r < i; r++) n = e[r], ft.tweeners[n] = ft.tweeners[n] || [], ft.tweeners[n].unshift(t)
+            for (var n, r = 0, i = e.length; r < i; r++) n = e[r], lt.tweeners[n] = lt.tweeners[n] || [], lt.tweeners[n].unshift(t)
         },
         prefilters: [function(e, t, n) {
             var r, i, o, a, s, u, l, c, f = "width" in t || "height" in t,
                 p = this,
                 d = {},
                 h = e.style,
                 g = e.nodeType && ae(e),
@@ -2283,33 +2281,33 @@
             for (r in n.queue || (null == (a = S._queueHooks(e, "fx")).unqueued && (a.unqueued = 0, s = a.empty.fire, a.empty.fire = function() {
                     a.unqueued || s()
                 }), a.unqueued++, p.always(function() {
                     p.always(function() {
                         a.unqueued--, S.queue(e, "fx").length || a.empty.fire()
                     })
                 })), t)
-                if (i = t[r], ot.test(i)) {
+                if (i = t[r], rt.test(i)) {
                     if (delete t[r], o = o || "toggle" === i, i === (g ? "hide" : "show")) {
                         if ("show" !== i || !v || void 0 === v[r]) continue;
                         g = !0
                     }
                     d[r] = v && v[r] || S.style(e, r)
                 } if ((u = !S.isEmptyObject(t)) || !S.isEmptyObject(d))
                 for (r in f && 1 === e.nodeType && (n.overflow = [h.overflow, h.overflowX, h.overflowY], null == (l = v && v.display) && (l = Y.get(e, "display")), "none" === (c = S.css(e, "display")) && (l ? c = l : (le([e], !0), l = e.style.display || l, c = S.css(e, "display"), le([e]))), ("inline" === c || "inline-block" === c && null != l) && "none" === S.css(e, "float") && (u || (p.done(function() {
                         h.display = l
                     }), null == l && (c = h.display, l = "none" === c ? "" : c)), h.display = "inline-block")), n.overflow && (h.overflow = "hidden", p.always(function() {
                         h.overflow = n.overflow[0], h.overflowX = n.overflow[1], h.overflowY = n.overflow[2]
                     })), u = !1, d) u || (v ? "hidden" in v && (g = v.hidden) : v = Y.access(e, "fxshow", {
                     display: l
                 }), o && (v.hidden = !g), g && le([e], !0), p.done(function() {
                     for (r in g || le([e]), Y.remove(e, "fxshow"), d) S.style(e, r, d[r])
-                })), u = ct(g ? v[r] : 0, r, p), r in v || (v[r] = u.start, g && (u.end = u.start, u.start = 0))
+                })), u = ut(g ? v[r] : 0, r, p), r in v || (v[r] = u.start, g && (u.end = u.start, u.start = 0))
         }],
         prefilter: function(e, t) {
-            t ? ft.prefilters.unshift(e) : ft.prefilters.push(e)
+            t ? lt.prefilters.unshift(e) : lt.prefilters.push(e)
         }
     }), S.speed = function(e, t, n) {
         var r = e && "object" == typeof e ? S.extend({}, e) : {
             complete: n || !n && t || m(e) && e,
             duration: e,
             easing: n && t || t && !m(t) && t
         };
@@ -2322,15 +2320,15 @@
                 opacity: t
             }, e, n, r)
         },
         animate: function(t, e, n, r) {
             var i = S.isEmptyObject(t),
                 o = S.speed(e, n, r),
                 a = function() {
-                    var e = ft(this, S.extend({}, t), o);
+                    var e = lt(this, S.extend({}, t), o);
                     (i || Y.get(this, "finish")) && e.stop(!0)
                 };
             return a.finish = a, i || !1 === o.queue ? this.each(a) : this.queue(o.queue, a)
         },
         stop: function(i, e, o) {
             var a = function(e) {
                 var t = e.stop;
@@ -2339,15 +2337,15 @@
             return "string" != typeof i && (o = e, e = i, i = void 0), e && this.queue(i || "fx", []), this.each(function() {
                 var e = !0,
                     t = null != i && i + "queueHooks",
                     n = S.timers,
                     r = Y.get(this);
                 if (t) r[t] && r[t].stop && a(r[t]);
                 else
-                    for (t in r) r[t] && r[t].stop && at.test(t) && a(r[t]);
+                    for (t in r) r[t] && r[t].stop && it.test(t) && a(r[t]);
                 for (t = n.length; t--;) n[t].elem !== this || null != i && n[t].queue !== i || (n[t].anim.stop(o), e = !1, n.splice(t, 1));
                 !e && o || S.dequeue(this, i)
             })
         },
         finish: function(a) {
             return !1 !== a && (a = a || "fx"), this.each(function() {
                 var e, t = Y.get(this),
@@ -2359,20 +2357,20 @@
                 for (e = 0; e < o; e++) n[e] && n[e].finish && n[e].finish.call(this);
                 delete t.finish
             })
         }
     }), S.each(["toggle", "show", "hide"], function(e, r) {
         var i = S.fn[r];
         S.fn[r] = function(e, t, n) {
-            return null == e || "boolean" == typeof e ? i.apply(this, arguments) : this.animate(lt(r, !0), e, t, n)
+            return null == e || "boolean" == typeof e ? i.apply(this, arguments) : this.animate(st(r, !0), e, t, n)
         }
     }), S.each({
-        slideDown: lt("show"),
-        slideUp: lt("hide"),
-        slideToggle: lt("toggle"),
+        slideDown: st("show"),
+        slideUp: st("hide"),
+        slideToggle: st("toggle"),
         fadeIn: {
             opacity: "show"
         },
         fadeOut: {
             opacity: "hide"
         },
         fadeToggle: {
@@ -2381,48 +2379,48 @@
     }, function(e, r) {
         S.fn[e] = function(e, t, n) {
             return this.animate(r, e, t, n)
         }
     }), S.timers = [], S.fx.tick = function() {
         var e, t = 0,
             n = S.timers;
-        for (tt = Date.now(); t < n.length; t++)(e = n[t])() || n[t] !== e || n.splice(t--, 1);
-        n.length || S.fx.stop(), tt = void 0
+        for (Ze = Date.now(); t < n.length; t++)(e = n[t])() || n[t] !== e || n.splice(t--, 1);
+        n.length || S.fx.stop(), Ze = void 0
     }, S.fx.timer = function(e) {
         S.timers.push(e), S.fx.start()
     }, S.fx.interval = 13, S.fx.start = function() {
-        nt || (nt = !0, st())
+        et || (et = !0, ot())
     }, S.fx.stop = function() {
-        nt = null
+        et = null
     }, S.fx.speeds = {
         slow: 600,
         fast: 200,
         _default: 400
     }, S.fn.delay = function(r, e) {
         return r = S.fx && S.fx.speeds[r] || r, e = e || "fx", this.queue(e, function(e, t) {
             var n = C.setTimeout(e, r);
             t.stop = function() {
                 C.clearTimeout(n)
             }
         })
-    }, rt = E.createElement("input"), it = E.createElement("select").appendChild(E.createElement("option")), rt.type = "checkbox", y.checkOn = "" !== rt.value, y.optSelected = it.selected, (rt = E.createElement("input")).value = "t", rt.type = "radio", y.radioValue = "t" === rt.value;
-    var pt, dt = S.expr.attrHandle;
+    }, tt = E.createElement("input"), nt = E.createElement("select").appendChild(E.createElement("option")), tt.type = "checkbox", y.checkOn = "" !== tt.value, y.optSelected = nt.selected, (tt = E.createElement("input")).value = "t", tt.type = "radio", y.radioValue = "t" === tt.value;
+    var ct, ft = S.expr.attrHandle;
     S.fn.extend({
         attr: function(e, t) {
             return $(this, S.attr, e, t, 1 < arguments.length)
         },
         removeAttr: function(e) {
             return this.each(function() {
                 S.removeAttr(this, e)
             })
         }
     }), S.extend({
         attr: function(e, t, n) {
             var r, i, o = e.nodeType;
-            if (3 !== o && 8 !== o && 2 !== o) return "undefined" == typeof e.getAttribute ? S.prop(e, t, n) : (1 === o && S.isXMLDoc(e) || (i = S.attrHooks[t.toLowerCase()] || (S.expr.match.bool.test(t) ? pt : void 0)), void 0 !== n ? null === n ? void S.removeAttr(e, t) : i && "set" in i && void 0 !== (r = i.set(e, n, t)) ? r : (e.setAttribute(t, n + ""), n) : i && "get" in i && null !== (r = i.get(e, t)) ? r : null == (r = S.find.attr(e, t)) ? void 0 : r)
+            if (3 !== o && 8 !== o && 2 !== o) return "undefined" == typeof e.getAttribute ? S.prop(e, t, n) : (1 === o && S.isXMLDoc(e) || (i = S.attrHooks[t.toLowerCase()] || (S.expr.match.bool.test(t) ? ct : void 0)), void 0 !== n ? null === n ? void S.removeAttr(e, t) : i && "set" in i && void 0 !== (r = i.set(e, n, t)) ? r : (e.setAttribute(t, n + ""), n) : i && "get" in i && null !== (r = i.get(e, t)) ? r : null == (r = S.find.attr(e, t)) ? void 0 : r)
         },
         attrHooks: {
             type: {
                 set: function(e, t) {
                     if (!y.radioValue && "radio" === t && A(e, "input")) {
                         var n = e.value;
                         return e.setAttribute("type", t), n && (e.value = n), t
@@ -2432,37 +2430,37 @@
         },
         removeAttr: function(e, t) {
             var n, r = 0,
                 i = t && t.match(P);
             if (i && 1 === e.nodeType)
                 while (n = i[r++]) e.removeAttribute(n)
         }
-    }), pt = {
+    }), ct = {
         set: function(e, t, n) {
             return !1 === t ? S.removeAttr(e, n) : e.setAttribute(n, n), n
         }
     }, S.each(S.expr.match.bool.source.match(/\w+/g), function(e, t) {
-        var a = dt[t] || S.find.attr;
-        dt[t] = function(e, t, n) {
+        var a = ft[t] || S.find.attr;
+        ft[t] = function(e, t, n) {
             var r, i, o = t.toLowerCase();
-            return n || (i = dt[o], dt[o] = r, r = null != a(e, t, n) ? o : null, dt[o] = i), r
+            return n || (i = ft[o], ft[o] = r, r = null != a(e, t, n) ? o : null, ft[o] = i), r
         }
     });
-    var ht = /^(?:input|select|textarea|button)$/i,
-        gt = /^(?:a|area)$/i;
+    var pt = /^(?:input|select|textarea|button)$/i,
+        dt = /^(?:a|area)$/i;
 
-    function vt(e) {
+    function ht(e) {
         return (e.match(P) || []).join(" ")
     }
 
-    function yt(e) {
+    function gt(e) {
         return e.getAttribute && e.getAttribute("class") || ""
     }
 
-    function mt(e) {
+    function vt(e) {
         return Array.isArray(e) ? e : "string" == typeof e && e.match(P) || []
     }
     S.fn.extend({
         prop: function(e, t) {
             return $(this, S.prop, e, t, 1 < arguments.length)
         },
         removeProp: function(e) {
@@ -2475,15 +2473,15 @@
             var r, i, o = e.nodeType;
             if (3 !== o && 8 !== o && 2 !== o) return 1 === o && S.isXMLDoc(e) || (t = S.propFix[t] || t, i = S.propHooks[t]), void 0 !== n ? i && "set" in i && void 0 !== (r = i.set(e, n, t)) ? r : e[t] = n : i && "get" in i && null !== (r = i.get(e, t)) ? r : e[t]
         },
         propHooks: {
             tabIndex: {
                 get: function(e) {
                     var t = S.find.attr(e, "tabindex");
-                    return t ? parseInt(t, 10) : ht.test(e.nodeName) || gt.test(e.nodeName) && e.href ? 0 : -1
+                    return t ? parseInt(t, 10) : pt.test(e.nodeName) || dt.test(e.nodeName) && e.href ? 0 : -1
                 }
             }
         },
         propFix: {
             "for": "htmlFor",
             "class": "className"
         }
@@ -2498,77 +2496,77 @@
         }
     }), S.each(["tabIndex", "readOnly", "maxLength", "cellSpacing", "cellPadding", "rowSpan", "colSpan", "useMap", "frameBorder", "contentEditable"], function() {
         S.propFix[this.toLowerCase()] = this
     }), S.fn.extend({
         addClass: function(t) {
             var e, n, r, i, o, a, s, u = 0;
             if (m(t)) return this.each(function(e) {
-                S(this).addClass(t.call(this, e, yt(this)))
+                S(this).addClass(t.call(this, e, gt(this)))
             });
-            if ((e = mt(t)).length)
+            if ((e = vt(t)).length)
                 while (n = this[u++])
-                    if (i = yt(n), r = 1 === n.nodeType && " " + vt(i) + " ") {
+                    if (i = gt(n), r = 1 === n.nodeType && " " + ht(i) + " ") {
                         a = 0;
                         while (o = e[a++]) r.indexOf(" " + o + " ") < 0 && (r += o + " ");
-                        i !== (s = vt(r)) && n.setAttribute("class", s)
+                        i !== (s = ht(r)) && n.setAttribute("class", s)
                     } return this
         },
         removeClass: function(t) {
             var e, n, r, i, o, a, s, u = 0;
             if (m(t)) return this.each(function(e) {
-                S(this).removeClass(t.call(this, e, yt(this)))
+                S(this).removeClass(t.call(this, e, gt(this)))
             });
             if (!arguments.length) return this.attr("class", "");
-            if ((e = mt(t)).length)
+            if ((e = vt(t)).length)
                 while (n = this[u++])
-                    if (i = yt(n), r = 1 === n.nodeType && " " + vt(i) + " ") {
+                    if (i = gt(n), r = 1 === n.nodeType && " " + ht(i) + " ") {
                         a = 0;
                         while (o = e[a++])
                             while (-1 < r.indexOf(" " + o + " ")) r = r.replace(" " + o + " ", " ");
-                        i !== (s = vt(r)) && n.setAttribute("class", s)
+                        i !== (s = ht(r)) && n.setAttribute("class", s)
                     } return this
         },
         toggleClass: function(i, t) {
             var o = typeof i,
                 a = "string" === o || Array.isArray(i);
             return "boolean" == typeof t && a ? t ? this.addClass(i) : this.removeClass(i) : m(i) ? this.each(function(e) {
-                S(this).toggleClass(i.call(this, e, yt(this), t), t)
+                S(this).toggleClass(i.call(this, e, gt(this), t), t)
             }) : this.each(function() {
                 var e, t, n, r;
                 if (a) {
-                    t = 0, n = S(this), r = mt(i);
+                    t = 0, n = S(this), r = vt(i);
                     while (e = r[t++]) n.hasClass(e) ? n.removeClass(e) : n.addClass(e)
-                } else void 0 !== i && "boolean" !== o || ((e = yt(this)) && Y.set(this, "__className__", e), this.setAttribute && this.setAttribute("class", e || !1 === i ? "" : Y.get(this, "__className__") || ""))
+                } else void 0 !== i && "boolean" !== o || ((e = gt(this)) && Y.set(this, "__className__", e), this.setAttribute && this.setAttribute("class", e || !1 === i ? "" : Y.get(this, "__className__") || ""))
             })
         },
         hasClass: function(e) {
             var t, n, r = 0;
             t = " " + e + " ";
             while (n = this[r++])
-                if (1 === n.nodeType && -1 < (" " + vt(yt(n)) + " ").indexOf(t)) return !0;
+                if (1 === n.nodeType && -1 < (" " + ht(gt(n)) + " ").indexOf(t)) return !0;
             return !1
         }
     });
-    var xt = /\r/g;
+    var yt = /\r/g;
     S.fn.extend({
         val: function(n) {
             var r, e, i, t = this[0];
             return arguments.length ? (i = m(n), this.each(function(e) {
                 var t;
                 1 === this.nodeType && (null == (t = i ? n.call(this, e, S(this).val()) : n) ? t = "" : "number" == typeof t ? t += "" : Array.isArray(t) && (t = S.map(t, function(e) {
                     return null == e ? "" : e + ""
                 })), (r = S.valHooks[this.type] || S.valHooks[this.nodeName.toLowerCase()]) && "set" in r && void 0 !== r.set(this, t, "value") || (this.value = t))
-            })) : t ? (r = S.valHooks[t.type] || S.valHooks[t.nodeName.toLowerCase()]) && "get" in r && void 0 !== (e = r.get(t, "value")) ? e : "string" == typeof(e = t.value) ? e.replace(xt, "") : null == e ? "" : e : void 0
+            })) : t ? (r = S.valHooks[t.type] || S.valHooks[t.nodeName.toLowerCase()]) && "get" in r && void 0 !== (e = r.get(t, "value")) ? e : "string" == typeof(e = t.value) ? e.replace(yt, "") : null == e ? "" : e : void 0
         }
     }), S.extend({
         valHooks: {
             option: {
                 get: function(e) {
                     var t = S.find.attr(e, "value");
-                    return null != t ? t : vt(S.text(e))
+                    return null != t ? t : ht(S.text(e))
                 }
             },
             select: {
                 get: function(e) {
                     var t, n, r, i = e.options,
                         o = e.selectedIndex,
                         a = "select-one" === e.type,
@@ -2594,31 +2592,31 @@
             set: function(e, t) {
                 if (Array.isArray(t)) return e.checked = -1 < S.inArray(S(e).val(), t)
             }
         }, y.checkOn || (S.valHooks[this].get = function(e) {
             return null === e.getAttribute("value") ? "on" : e.value
         })
     }), y.focusin = "onfocusin" in C;
-    var bt = /^(?:focusinfocus|focusoutblur)$/,
-        wt = function(e) {
+    var mt = /^(?:focusinfocus|focusoutblur)$/,
+        xt = function(e) {
             e.stopPropagation()
         };
     S.extend(S.event, {
         trigger: function(e, t, n, r) {
             var i, o, a, s, u, l, c, f, p = [n || E],
                 d = v.call(e, "type") ? e.type : e,
                 h = v.call(e, "namespace") ? e.namespace.split(".") : [];
-            if (o = f = a = n = n || E, 3 !== n.nodeType && 8 !== n.nodeType && !bt.test(d + S.event.triggered) && (-1 < d.indexOf(".") && (d = (h = d.split(".")).shift(), h.sort()), u = d.indexOf(":") < 0 && "on" + d, (e = e[S.expando] ? e : new S.Event(d, "object" == typeof e && e)).isTrigger = r ? 2 : 3, e.namespace = h.join("."), e.rnamespace = e.namespace ? new RegExp("(^|\\.)" + h.join("\\.(?:.*\\.|)") + "(\\.|$)") : null, e.result = void 0, e.target || (e.target = n), t = null == t ? [e] : S.makeArray(t, [e]), c = S.event.special[d] || {}, r || !c.trigger || !1 !== c.trigger.apply(n, t))) {
+            if (o = f = a = n = n || E, 3 !== n.nodeType && 8 !== n.nodeType && !mt.test(d + S.event.triggered) && (-1 < d.indexOf(".") && (d = (h = d.split(".")).shift(), h.sort()), u = d.indexOf(":") < 0 && "on" + d, (e = e[S.expando] ? e : new S.Event(d, "object" == typeof e && e)).isTrigger = r ? 2 : 3, e.namespace = h.join("."), e.rnamespace = e.namespace ? new RegExp("(^|\\.)" + h.join("\\.(?:.*\\.|)") + "(\\.|$)") : null, e.result = void 0, e.target || (e.target = n), t = null == t ? [e] : S.makeArray(t, [e]), c = S.event.special[d] || {}, r || !c.trigger || !1 !== c.trigger.apply(n, t))) {
                 if (!r && !c.noBubble && !x(n)) {
-                    for (s = c.delegateType || d, bt.test(s + d) || (o = o.parentNode); o; o = o.parentNode) p.push(o), a = o;
+                    for (s = c.delegateType || d, mt.test(s + d) || (o = o.parentNode); o; o = o.parentNode) p.push(o), a = o;
                     a === (n.ownerDocument || E) && p.push(a.defaultView || a.parentWindow || C)
                 }
                 i = 0;
                 while ((o = p[i++]) && !e.isPropagationStopped()) f = o, e.type = 1 < i ? s : c.bindType || d, (l = (Y.get(o, "events") || Object.create(null))[e.type] && Y.get(o, "handle")) && l.apply(o, t), (l = u && o[u]) && l.apply && V(o) && (e.result = l.apply(o, t), !1 === e.result && e.preventDefault());
-                return e.type = d, r || e.isDefaultPrevented() || c._default && !1 !== c._default.apply(p.pop(), t) || !V(n) || u && m(n[d]) && !x(n) && ((a = n[u]) && (n[u] = null), S.event.triggered = d, e.isPropagationStopped() && f.addEventListener(d, wt), n[d](), e.isPropagationStopped() && f.removeEventListener(d, wt), S.event.triggered = void 0, a && (n[u] = a)), e.result
+                return e.type = d, r || e.isDefaultPrevented() || c._default && !1 !== c._default.apply(p.pop(), t) || !V(n) || u && m(n[d]) && !x(n) && ((a = n[u]) && (n[u] = null), S.event.triggered = d, e.isPropagationStopped() && f.addEventListener(d, xt), n[d](), e.isPropagationStopped() && f.removeEventListener(d, xt), S.event.triggered = void 0, a && (n[u] = a)), e.result
             }
         },
         simulate: function(e, t, n) {
             var r = S.extend(new S.Event, n, {
                 type: e,
                 isSimulated: !0
             });
@@ -2650,135 +2648,135 @@
             teardown: function() {
                 var e = this.ownerDocument || this.document || this,
                     t = Y.access(e, r) - 1;
                 t ? Y.access(e, r, t) : (e.removeEventListener(n, i, !0), Y.remove(e, r))
             }
         }
     });
-    var Tt = C.location,
-        Ct = {
+    var bt = C.location,
+        wt = {
             guid: Date.now()
         },
-        Et = /\?/;
+        Tt = /\?/;
     S.parseXML = function(e) {
-        var t;
+        var t, n;
         if (!e || "string" != typeof e) return null;
         try {
             t = (new C.DOMParser).parseFromString(e, "text/xml")
-        } catch (e) {
-            t = void 0
-        }
-        return t && !t.getElementsByTagName("parsererror").length || S.error("Invalid XML: " + e), t
+        } catch (e) {}
+        return n = t && t.getElementsByTagName("parsererror")[0], t && !n || S.error("Invalid XML: " + (n ? S.map(n.childNodes, function(e) {
+            return e.textContent
+        }).join("\n") : e)), t
     };
-    var St = /\[\]$/,
-        kt = /\r?\n/g,
-        At = /^(?:submit|button|image|reset|file)$/i,
-        Nt = /^(?:input|select|textarea|keygen)/i;
+    var Ct = /\[\]$/,
+        Et = /\r?\n/g,
+        St = /^(?:submit|button|image|reset|file)$/i,
+        kt = /^(?:input|select|textarea|keygen)/i;
 
-    function Dt(n, e, r, i) {
+    function At(n, e, r, i) {
         var t;
         if (Array.isArray(e)) S.each(e, function(e, t) {
-            r || St.test(n) ? i(n, t) : Dt(n + "[" + ("object" == typeof t && null != t ? e : "") + "]", t, r, i)
+            r || Ct.test(n) ? i(n, t) : At(n + "[" + ("object" == typeof t && null != t ? e : "") + "]", t, r, i)
         });
         else if (r || "object" !== w(e)) i(n, e);
         else
-            for (t in e) Dt(n + "[" + t + "]", e[t], r, i)
+            for (t in e) At(n + "[" + t + "]", e[t], r, i)
     }
     S.param = function(e, t) {
         var n, r = [],
             i = function(e, t) {
                 var n = m(t) ? t() : t;
                 r[r.length] = encodeURIComponent(e) + "=" + encodeURIComponent(null == n ? "" : n)
             };
         if (null == e) return "";
         if (Array.isArray(e) || e.jquery && !S.isPlainObject(e)) S.each(e, function() {
             i(this.name, this.value)
         });
         else
-            for (n in e) Dt(n, e[n], t, i);
+            for (n in e) At(n, e[n], t, i);
         return r.join("&")
     }, S.fn.extend({
         serialize: function() {
             return S.param(this.serializeArray())
         },
         serializeArray: function() {
             return this.map(function() {
                 var e = S.prop(this, "elements");
                 return e ? S.makeArray(e) : this
             }).filter(function() {
                 var e = this.type;
-                return this.name && !S(this).is(":disabled") && Nt.test(this.nodeName) && !At.test(e) && (this.checked || !pe.test(e))
+                return this.name && !S(this).is(":disabled") && kt.test(this.nodeName) && !St.test(e) && (this.checked || !pe.test(e))
             }).map(function(e, t) {
                 var n = S(this).val();
                 return null == n ? null : Array.isArray(n) ? S.map(n, function(e) {
                     return {
                         name: t.name,
-                        value: e.replace(kt, "\r\n")
+                        value: e.replace(Et, "\r\n")
                     }
                 }) : {
                     name: t.name,
-                    value: n.replace(kt, "\r\n")
+                    value: n.replace(Et, "\r\n")
                 }
             }).get()
         }
     });
-    var jt = /%20/g,
-        qt = /#.*$/,
-        Lt = /([?&])_=[^&]*/,
-        Ht = /^(.*?):[ \t]*([^\r\n]*)$/gm,
-        Ot = /^(?:GET|HEAD)$/,
-        Pt = /^\/\//,
-        Rt = {},
-        Mt = {},
-        It = "*/".concat("*"),
-        Wt = E.createElement("a");
+    var Nt = /%20/g,
+        jt = /#.*$/,
+        Dt = /([?&])_=[^&]*/,
+        qt = /^(.*?):[ \t]*([^\r\n]*)$/gm,
+        Lt = /^(?:GET|HEAD)$/,
+        Ht = /^\/\//,
+        Ot = {},
+        Pt = {},
+        Rt = "*/".concat("*"),
+        Mt = E.createElement("a");
 
-    function Ft(o) {
+    function It(o) {
         return function(e, t) {
             "string" != typeof e && (t = e, e = "*");
             var n, r = 0,
                 i = e.toLowerCase().match(P) || [];
             if (m(t))
                 while (n = i[r++]) "+" === n[0] ? (n = n.slice(1) || "*", (o[n] = o[n] || []).unshift(t)) : (o[n] = o[n] || []).push(t)
         }
     }
 
-    function Bt(t, i, o, a) {
+    function Wt(t, i, o, a) {
         var s = {},
-            u = t === Mt;
+            u = t === Pt;
 
         function l(e) {
             var r;
             return s[e] = !0, S.each(t[e] || [], function(e, t) {
                 var n = t(i, o, a);
                 return "string" != typeof n || u || s[n] ? u ? !(r = n) : void 0 : (i.dataTypes.unshift(n), l(n), !1)
             }), r
         }
         return l(i.dataTypes[0]) || !s["*"] && l("*")
     }
 
-    function $t(e, t) {
+    function Ft(e, t) {
         var n, r, i = S.ajaxSettings.flatOptions || {};
         for (n in t) void 0 !== t[n] && ((i[n] ? e : r || (r = {}))[n] = t[n]);
         return r && S.extend(!0, e, r), e
     }
-    Wt.href = Tt.href, S.extend({
+    Mt.href = bt.href, S.extend({
         active: 0,
         lastModified: {},
         etag: {},
         ajaxSettings: {
-            url: Tt.href,
+            url: bt.href,
             type: "GET",
-            isLocal: /^(?:about|app|app-storage|.+-extension|file|res|widget):$/.test(Tt.protocol),
+            isLocal: /^(?:about|app|app-storage|.+-extension|file|res|widget):$/.test(bt.protocol),
             global: !0,
             processData: !0,
             async: !0,
             contentType: "application/x-www-form-urlencoded; charset=UTF-8",
             accepts: {
-                "*": It,
+                "*": Rt,
                 text: "text/plain",
                 html: "text/html",
                 xml: "application/xml, text/xml",
                 json: "application/json, text/javascript"
             },
             contents: {
                 xml: /\bxml\b/,
@@ -2798,18 +2796,18 @@
             },
             flatOptions: {
                 url: !0,
                 context: !0
             }
         },
         ajaxSetup: function(e, t) {
-            return t ? $t($t(e, S.ajaxSettings), t) : $t(S.ajaxSettings, e)
+            return t ? Ft(Ft(e, S.ajaxSettings), t) : Ft(S.ajaxSettings, e)
         },
-        ajaxPrefilter: Ft(Rt),
-        ajaxTransport: Ft(Mt),
+        ajaxPrefilter: It(Ot),
+        ajaxTransport: It(Pt),
         ajax: function(e, t) {
             "object" == typeof e && (t = e, e = void 0), t = t || {};
             var c, f, p, n, d, r, h, g, i, o, v = S.ajaxSetup({}, t),
                 y = v.context || v,
                 m = v.context && (y.nodeType || y.jquery) ? S(y) : S.event,
                 x = S.Deferred(),
                 b = S.Callbacks("once memory"),
@@ -2820,15 +2818,15 @@
                 T = {
                     readyState: 0,
                     getResponseHeader: function(e) {
                         var t;
                         if (h) {
                             if (!n) {
                                 n = {};
-                                while (t = Ht.exec(p)) n[t[1].toLowerCase() + " "] = (n[t[1].toLowerCase() + " "] || []).concat(t[2])
+                                while (t = qt.exec(p)) n[t[1].toLowerCase() + " "] = (n[t[1].toLowerCase() + " "] || []).concat(t[2])
                             }
                             t = n[e.toLowerCase() + " "]
                         }
                         return null == t ? null : t.join(", ")
                     },
                     getAllResponseHeaders: function() {
                         return h ? p : null
@@ -2848,26 +2846,26 @@
                         return this
                     },
                     abort: function(e) {
                         var t = e || u;
                         return c && c.abort(t), l(0, t), this
                     }
                 };
-            if (x.promise(T), v.url = ((e || v.url || Tt.href) + "").replace(Pt, Tt.protocol + "//"), v.type = t.method || t.type || v.method || v.type, v.dataTypes = (v.dataType || "*").toLowerCase().match(P) || [""], null == v.crossDomain) {
+            if (x.promise(T), v.url = ((e || v.url || bt.href) + "").replace(Ht, bt.protocol + "//"), v.type = t.method || t.type || v.method || v.type, v.dataTypes = (v.dataType || "*").toLowerCase().match(P) || [""], null == v.crossDomain) {
                 r = E.createElement("a");
                 try {
-                    r.href = v.url, r.href = r.href, v.crossDomain = Wt.protocol + "//" + Wt.host != r.protocol + "//" + r.host
+                    r.href = v.url, r.href = r.href, v.crossDomain = Mt.protocol + "//" + Mt.host != r.protocol + "//" + r.host
                 } catch (e) {
                     v.crossDomain = !0
                 }
             }
-            if (v.data && v.processData && "string" != typeof v.data && (v.data = S.param(v.data, v.traditional)), Bt(Rt, v, t, T), h) return T;
-            for (i in (g = S.event && v.global) && 0 == S.active++ && S.event.trigger("ajaxStart"), v.type = v.type.toUpperCase(), v.hasContent = !Ot.test(v.type), f = v.url.replace(qt, ""), v.hasContent ? v.data && v.processData && 0 === (v.contentType || "").indexOf("application/x-www-form-urlencoded") && (v.data = v.data.replace(jt, "+")) : (o = v.url.slice(f.length), v.data && (v.processData || "string" == typeof v.data) && (f += (Et.test(f) ? "&" : "?") + v.data, delete v.data), !1 === v.cache && (f = f.replace(Lt, "$1"), o = (Et.test(f) ? "&" : "?") + "_=" + Ct.guid++ + o), v.url = f + o), v.ifModified && (S.lastModified[f] && T.setRequestHeader("If-Modified-Since", S.lastModified[f]), S.etag[f] && T.setRequestHeader("If-None-Match", S.etag[f])), (v.data && v.hasContent && !1 !== v.contentType || t.contentType) && T.setRequestHeader("Content-Type", v.contentType), T.setRequestHeader("Accept", v.dataTypes[0] && v.accepts[v.dataTypes[0]] ? v.accepts[v.dataTypes[0]] + ("*" !== v.dataTypes[0] ? ", " + It + "; q=0.01" : "") : v.accepts["*"]), v.headers) T.setRequestHeader(i, v.headers[i]);
+            if (v.data && v.processData && "string" != typeof v.data && (v.data = S.param(v.data, v.traditional)), Wt(Ot, v, t, T), h) return T;
+            for (i in (g = S.event && v.global) && 0 == S.active++ && S.event.trigger("ajaxStart"), v.type = v.type.toUpperCase(), v.hasContent = !Lt.test(v.type), f = v.url.replace(jt, ""), v.hasContent ? v.data && v.processData && 0 === (v.contentType || "").indexOf("application/x-www-form-urlencoded") && (v.data = v.data.replace(Nt, "+")) : (o = v.url.slice(f.length), v.data && (v.processData || "string" == typeof v.data) && (f += (Tt.test(f) ? "&" : "?") + v.data, delete v.data), !1 === v.cache && (f = f.replace(Dt, "$1"), o = (Tt.test(f) ? "&" : "?") + "_=" + wt.guid++ + o), v.url = f + o), v.ifModified && (S.lastModified[f] && T.setRequestHeader("If-Modified-Since", S.lastModified[f]), S.etag[f] && T.setRequestHeader("If-None-Match", S.etag[f])), (v.data && v.hasContent && !1 !== v.contentType || t.contentType) && T.setRequestHeader("Content-Type", v.contentType), T.setRequestHeader("Accept", v.dataTypes[0] && v.accepts[v.dataTypes[0]] ? v.accepts[v.dataTypes[0]] + ("*" !== v.dataTypes[0] ? ", " + Rt + "; q=0.01" : "") : v.accepts["*"]), v.headers) T.setRequestHeader(i, v.headers[i]);
             if (v.beforeSend && (!1 === v.beforeSend.call(y, T, v) || h)) return T.abort();
-            if (u = "abort", b.add(v.complete), T.done(v.success), T.fail(v.error), c = Bt(Mt, v, t, T)) {
+            if (u = "abort", b.add(v.complete), T.done(v.success), T.fail(v.error), c = Wt(Pt, v, t, T)) {
                 if (T.readyState = 1, g && m.trigger("ajaxSend", [T, v]), h) return T;
                 v.async && 0 < v.timeout && (d = C.setTimeout(function() {
                     T.abort("timeout")
                 }, v.timeout));
                 try {
                     h = !1, c.send(a, l)
                 } catch (e) {
@@ -2895,15 +2893,15 @@
                                 break
                             }
                             a || (a = i)
                         }
                         o = o || a
                     }
                     if (o) return o !== u[0] && u.unshift(o), n[o]
-                }(v, T, n)), !i && -1 < S.inArray("script", v.dataTypes) && (v.converters["text script"] = function() {}), s = function(e, t, n, r) {
+                }(v, T, n)), !i && -1 < S.inArray("script", v.dataTypes) && S.inArray("json", v.dataTypes) < 0 && (v.converters["text script"] = function() {}), s = function(e, t, n, r) {
                     var i, o, a, s, u, l = {},
                         c = e.dataTypes.slice();
                     if (c[1])
                         for (a in e.converters) l[a.toLowerCase()] = e.converters[a];
                     o = c.shift();
                     while (o)
                         if (e.responseFields[o] && (n[e.responseFields[o]] = t), !u && r && e.dataFilter && (t = e.dataFilter(t, e.dataType)), u = o, o = c.shift())
@@ -3001,30 +2999,30 @@
     }, S.expr.pseudos.visible = function(e) {
         return !!(e.offsetWidth || e.offsetHeight || e.getClientRects().length)
     }, S.ajaxSettings.xhr = function() {
         try {
             return new C.XMLHttpRequest
         } catch (e) {}
     };
-    var _t = {
+    var Bt = {
             0: 200,
             1223: 204
         },
-        zt = S.ajaxSettings.xhr();
-    y.cors = !!zt && "withCredentials" in zt, y.ajax = zt = !!zt, S.ajaxTransport(function(i) {
+        $t = S.ajaxSettings.xhr();
+    y.cors = !!$t && "withCredentials" in $t, y.ajax = $t = !!$t, S.ajaxTransport(function(i) {
         var o, a;
-        if (y.cors || zt && !i.crossDomain) return {
+        if (y.cors || $t && !i.crossDomain) return {
             send: function(e, t) {
                 var n, r = i.xhr();
                 if (r.open(i.type, i.url, i.async, i.username, i.password), i.xhrFields)
                     for (n in i.xhrFields) r[n] = i.xhrFields[n];
                 for (n in i.mimeType && r.overrideMimeType && r.overrideMimeType(i.mimeType), i.crossDomain || e["X-Requested-With"] || (e["X-Requested-With"] = "XMLHttpRequest"), e) r.setRequestHeader(n, e[n]);
                 o = function(e) {
                     return function() {
-                        o && (o = a = r.onload = r.onerror = r.onabort = r.ontimeout = r.onreadystatechange = null, "abort" === e ? r.abort() : "error" === e ? "number" != typeof r.status ? t(0, "error") : t(r.status, r.statusText) : t(_t[r.status] || r.status, r.statusText, "text" !== (r.responseType || "text") || "string" != typeof r.responseText ? {
+                        o && (o = a = r.onload = r.onerror = r.onabort = r.ontimeout = r.onreadystatechange = null, "abort" === e ? r.abort() : "error" === e ? "number" != typeof r.status ? t(0, "error") : t(r.status, r.statusText) : t(Bt[r.status] || r.status, r.statusText, "text" !== (r.responseType || "text") || "string" != typeof r.responseText ? {
                             binary: r.response
                         } : {
                             text: r.responseText
                         }, r.getAllResponseHeaders()))
                     }
                 }, r.onload = o(), a = r.onerror = r.ontimeout = o("error"), void 0 !== r.onabort ? r.onabort = a : r.onreadystatechange = function() {
                     4 === r.readyState && C.setTimeout(function() {
@@ -3069,38 +3067,38 @@
                 }), E.head.appendChild(r[0])
             },
             abort: function() {
                 i && i()
             }
         }
     });
-    var Ut, Xt = [],
-        Vt = /(=)\?(?=&|$)|\?\?/;
+    var _t, zt = [],
+        Ut = /(=)\?(?=&|$)|\?\?/;
     S.ajaxSetup({
         jsonp: "callback",
         jsonpCallback: function() {
-            var e = Xt.pop() || S.expando + "_" + Ct.guid++;
+            var e = zt.pop() || S.expando + "_" + wt.guid++;
             return this[e] = !0, e
         }
     }), S.ajaxPrefilter("json jsonp", function(e, t, n) {
-        var r, i, o, a = !1 !== e.jsonp && (Vt.test(e.url) ? "url" : "string" == typeof e.data && 0 === (e.contentType || "").indexOf("application/x-www-form-urlencoded") && Vt.test(e.data) && "data");
-        if (a || "jsonp" === e.dataTypes[0]) return r = e.jsonpCallback = m(e.jsonpCallback) ? e.jsonpCallback() : e.jsonpCallback, a ? e[a] = e[a].replace(Vt, "$1" + r) : !1 !== e.jsonp && (e.url += (Et.test(e.url) ? "&" : "?") + e.jsonp + "=" + r), e.converters["script json"] = function() {
+        var r, i, o, a = !1 !== e.jsonp && (Ut.test(e.url) ? "url" : "string" == typeof e.data && 0 === (e.contentType || "").indexOf("application/x-www-form-urlencoded") && Ut.test(e.data) && "data");
+        if (a || "jsonp" === e.dataTypes[0]) return r = e.jsonpCallback = m(e.jsonpCallback) ? e.jsonpCallback() : e.jsonpCallback, a ? e[a] = e[a].replace(Ut, "$1" + r) : !1 !== e.jsonp && (e.url += (Tt.test(e.url) ? "&" : "?") + e.jsonp + "=" + r), e.converters["script json"] = function() {
             return o || S.error(r + " was not called"), o[0]
         }, e.dataTypes[0] = "json", i = C[r], C[r] = function() {
             o = arguments
         }, n.always(function() {
-            void 0 === i ? S(C).removeProp(r) : C[r] = i, e[r] && (e.jsonpCallback = t.jsonpCallback, Xt.push(r)), o && m(i) && i(o[0]), o = i = void 0
+            void 0 === i ? S(C).removeProp(r) : C[r] = i, e[r] && (e.jsonpCallback = t.jsonpCallback, zt.push(r)), o && m(i) && i(o[0]), o = i = void 0
         }), "script"
-    }), y.createHTMLDocument = ((Ut = E.implementation.createHTMLDocument("").body).innerHTML = "<form></form><form></form>", 2 === Ut.childNodes.length), S.parseHTML = function(e, t, n) {
+    }), y.createHTMLDocument = ((_t = E.implementation.createHTMLDocument("").body).innerHTML = "<form></form><form></form>", 2 === _t.childNodes.length), S.parseHTML = function(e, t, n) {
         return "string" != typeof e ? [] : ("boolean" == typeof t && (n = t, t = !1), t || (y.createHTMLDocument ? ((r = (t = E.implementation.createHTMLDocument("")).createElement("base")).href = E.location.href, t.head.appendChild(r)) : t = E), o = !n && [], (i = N.exec(e)) ? [t.createElement(i[1])] : (i = xe([e], t, o), o && o.length && S(o).remove(), S.merge([], i.childNodes)));
         var r, i, o
     }, S.fn.load = function(e, t, n) {
         var r, i, o, a = this,
             s = e.indexOf(" ");
-        return -1 < s && (r = vt(e.slice(s)), e = e.slice(0, s)), m(t) ? (n = t, t = void 0) : t && "object" == typeof t && (i = "POST"), 0 < a.length && S.ajax({
+        return -1 < s && (r = ht(e.slice(s)), e = e.slice(0, s)), m(t) ? (n = t, t = void 0) : t && "object" == typeof t && (i = "POST"), 0 < a.length && S.ajax({
             url: e,
             type: i || "GET",
             dataType: "html",
             data: t
         }).done(function(e) {
             o = arguments, a.html(r ? S("<div>").append(S.parseHTML(e)).find(r) : e)
         }).always(n && function(e, t) {
@@ -3113,15 +3111,15 @@
             return t === e.elem
         }).length
     }, S.offset = {
         setOffset: function(e, t, n) {
             var r, i, o, a, s, u, l = S.css(e, "position"),
                 c = S(e),
                 f = {};
-            "static" === l && (e.style.position = "relative"), s = c.offset(), o = S.css(e, "top"), u = S.css(e, "left"), ("absolute" === l || "fixed" === l) && -1 < (o + u).indexOf("auto") ? (a = (r = c.position()).top, i = r.left) : (a = parseFloat(o) || 0, i = parseFloat(u) || 0), m(t) && (t = t.call(e, n, S.extend({}, s))), null != t.top && (f.top = t.top - s.top + a), null != t.left && (f.left = t.left - s.left + i), "using" in t ? t.using.call(e, f) : ("number" == typeof f.top && (f.top += "px"), "number" == typeof f.left && (f.left += "px"), c.css(f))
+            "static" === l && (e.style.position = "relative"), s = c.offset(), o = S.css(e, "top"), u = S.css(e, "left"), ("absolute" === l || "fixed" === l) && -1 < (o + u).indexOf("auto") ? (a = (r = c.position()).top, i = r.left) : (a = parseFloat(o) || 0, i = parseFloat(u) || 0), m(t) && (t = t.call(e, n, S.extend({}, s))), null != t.top && (f.top = t.top - s.top + a), null != t.left && (f.left = t.left - s.left + i), "using" in t ? t.using.call(e, f) : c.css(f)
         }
     }, S.fn.extend({
         offset: function(t) {
             if (arguments.length) return void 0 === t ? this : this.each(function(e) {
                 S.offset.setOffset(this, t, e)
             });
             var e, n, r = this[0];
@@ -3168,16 +3166,16 @@
             return $(this, function(e, t, n) {
                 var r;
                 if (x(e) ? r = e : 9 === e.nodeType && (r = e.defaultView), void 0 === n) return r ? r[i] : e[t];
                 r ? r.scrollTo(o ? r.pageXOffset : n, o ? n : r.pageYOffset) : e[t] = n
             }, t, e, arguments.length)
         }
     }), S.each(["top", "left"], function(e, n) {
-        S.cssHooks[n] = $e(y.pixelPosition, function(e, t) {
-            if (t) return t = Be(e, n), Me.test(t) ? S(e).position()[n] + "px" : t
+        S.cssHooks[n] = Fe(y.pixelPosition, function(e, t) {
+            if (t) return t = We(e, n), Pe.test(t) ? S(e).position()[n] + "px" : t
         })
     }), S.each({
         Height: "height",
         Width: "width"
     }, function(a, s) {
         S.each({
             padding: "inner" + a,
@@ -3214,29 +3212,29 @@
             return this.mouseenter(e).mouseleave(t || e)
         }
     }), S.each("blur focus focusin focusout resize scroll click dblclick mousedown mouseup mousemove mouseover mouseout mouseenter mouseleave change select submit keydown keypress keyup contextmenu".split(" "), function(e, n) {
         S.fn[n] = function(e, t) {
             return 0 < arguments.length ? this.on(n, null, e, t) : this.trigger(n)
         }
     });
-    var Gt = /^[\s\uFEFF\xA0]+|[\s\uFEFF\xA0]+$/g;
+    var Xt = /^[\s\uFEFF\xA0]+|[\s\uFEFF\xA0]+$/g;
     S.proxy = function(e, t) {
         var n, r, i;
         if ("string" == typeof t && (n = e[t], t = e, e = n), m(e)) return r = s.call(arguments, 2), (i = function() {
             return e.apply(t || this, r.concat(s.call(arguments)))
         }).guid = e.guid = e.guid || S.guid++, i
     }, S.holdReady = function(e) {
         e ? S.readyWait++ : S.ready(!0)
     }, S.isArray = Array.isArray, S.parseJSON = JSON.parse, S.nodeName = A, S.isFunction = m, S.isWindow = x, S.camelCase = X, S.type = w, S.now = Date.now, S.isNumeric = function(e) {
         var t = S.type(e);
         return ("number" === t || "string" === t) && !isNaN(e - parseFloat(e))
     }, S.trim = function(e) {
-        return null == e ? "" : (e + "").replace(Gt, "")
+        return null == e ? "" : (e + "").replace(Xt, "")
     }, "function" == typeof define && define.amd && define("jquery", [], function() {
         return S
     });
-    var Yt = C.jQuery,
-        Qt = C.$;
+    var Vt = C.jQuery,
+        Gt = C.$;
     return S.noConflict = function(e) {
-        return C.$ === S && (C.$ = Qt), e && C.jQuery === S && (C.jQuery = Yt), S
+        return C.$ === S && (C.$ = Gt), e && C.jQuery === S && (C.jQuery = Vt), S
     }, "undefined" == typeof e && (C.jQuery = C.$ = S), S
 });
```

### Comparing `plink-2.4.1/plink_src/doc/_static/pygments.css` & `plink-2.4.2/plink_src/doc/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `plink-2.4.1/plink_src/doc/_static/searchtools.js` & `plink-2.4.2/plink_src/doc/_static/searchtools.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -1,553 +1,577 @@
 /*
  * searchtools.js
  * ~~~~~~~~~~~~~~~~
  *
  * Sphinx JavaScript utilities for the full-text search.
  *
- * :copyright: Copyright 2007-2021 by the Sphinx team, see AUTHORS.
+ * :copyright: Copyright 2007-2023 by the Sphinx team, see AUTHORS.
  * :license: BSD, see LICENSE for details.
  *
  */
+"use strict";
 
-if (!Scorer) {
-    /**
-     * Simple result scoring code.
-     */
+/**
+ * Simple result scoring code.
+ */
+if (typeof Scorer === "undefined") {
     var Scorer = {
         // Implement the following function to further tweak the score for each result
-        // The function takes a result array [filename, title, anchor, descr, score]
+        // The function takes a result array [docname, title, anchor, descr, score, filename]
         // and returns the new score.
         /*
-        score: function(result) {
-          return result[4];
+        score: result => {
+          const [docname, title, anchor, descr, score, filename] = result
+          return score
         },
         */
 
         // query matches the full name of an object
         objNameMatch: 11,
         // or matches in the last dotted part of the object name
         objPartialMatch: 6,
         // Additive scores depending on the priority of the object
         objPrio: {
             0: 15, // used to be importantResults
             1: 5, // used to be objectResults
-            2: -5
-        }, // used to be unimportantResults
+            2: -5, // used to be unimportantResults
+        },
         //  Used when the priority is not in the mapping.
         objPrioDefault: 0,
 
         // query found in title
         title: 15,
         partialTitle: 7,
         // query found in terms
         term: 5,
-        partialTerm: 2
+        partialTerm: 2,
     };
 }
 
-if (!splitQuery) {
-    function splitQuery(query) {
-        return query.split(/\s+/);
+const _removeChildren = (element) => {
+    while (element && element.lastChild) element.removeChild(element.lastChild);
+};
+
+/**
+ * See https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions#escaping
+ */
+const _escapeRegExp = (string) =>
+    string.replace(/[.*+\-?^${}()|[\]\\]/g, "\\$&"); // $& means the whole matched string
+
+const _displayItem = (item, searchTerms) => {
+    const docBuilder = DOCUMENTATION_OPTIONS.BUILDER;
+    const docUrlRoot = DOCUMENTATION_OPTIONS.URL_ROOT;
+    const docFileSuffix = DOCUMENTATION_OPTIONS.FILE_SUFFIX;
+    const docLinkSuffix = DOCUMENTATION_OPTIONS.LINK_SUFFIX;
+    const showSearchSummary = DOCUMENTATION_OPTIONS.SHOW_SEARCH_SUMMARY;
+
+    const [docName, title, anchor, descr, score, _filename] = item;
+
+    let listItem = document.createElement("li");
+    let requestUrl;
+    let linkUrl;
+    if (docBuilder === "dirhtml") {
+        // dirhtml builder
+        let dirname = docName + "/";
+        if (dirname.match(/\/index\/$/))
+            dirname = dirname.substring(0, dirname.length - 6);
+        else if (dirname === "index/") dirname = "";
+        requestUrl = docUrlRoot + dirname;
+        linkUrl = requestUrl;
+    } else {
+        // normal html builders
+        requestUrl = docUrlRoot + docName + docFileSuffix;
+        linkUrl = docName + docLinkSuffix;
+    }
+    let linkEl = listItem.appendChild(document.createElement("a"));
+    linkEl.href = linkUrl + anchor;
+    linkEl.dataset.score = score;
+    linkEl.innerHTML = title;
+    if (descr)
+        listItem.appendChild(document.createElement("span")).innerHTML =
+        " (" + descr + ")";
+    else if (showSearchSummary)
+        fetch(requestUrl)
+        .then((responseData) => responseData.text())
+        .then((data) => {
+            if (data)
+                listItem.appendChild(
+                    Search.makeSearchSummary(data, searchTerms)
+                );
+        });
+    Search.output.appendChild(listItem);
+};
+const _finishSearch = (resultCount) => {
+    Search.stopPulse();
+    Search.title.innerText = _("Search Results");
+    if (!resultCount)
+        Search.status.innerText = Documentation.gettext(
+            "Your search did not match any documents. Please make sure that all words are spelled correctly and that you've selected enough categories."
+        );
+    else
+        Search.status.innerText = _(
+            `Search finished, found ${resultCount} page(s) matching the search query.`
+        );
+};
+const _displayNextItem = (
+    results,
+    resultCount,
+    searchTerms
+) => {
+    // results left, load the summary and display it
+    // this is intended to be dynamic (don't sub resultsCount)
+    if (results.length) {
+        _displayItem(results.pop(), searchTerms);
+        setTimeout(
+            () => _displayNextItem(results, resultCount, searchTerms),
+            5
+        );
     }
+    // search finished, update title and status message
+    else _finishSearch(resultCount);
+};
+
+/**
+ * Default splitQuery function. Can be overridden in ``sphinx.search`` with a
+ * custom function per language.
+ *
+ * The regular expression works by splitting the string on consecutive characters
+ * that are not Unicode letters, numbers, underscores, or emoji characters.
+ * This is the same as ``\W+`` in Python, preserving the surrogate pair area.
+ */
+if (typeof splitQuery === "undefined") {
+    var splitQuery = (query) => query
+        .split(/[^\p{Letter}\p{Number}_\p{Emoji_Presentation}]+/gu)
+        .filter(term => term) // remove remaining empty strings
 }
 
 /**
  * Search Module
  */
-var Search = {
-
+const Search = {
     _index: null,
     _queued_query: null,
     _pulse_status: -1,
 
-    htmlToText: function(htmlString) {
-        var virtualDocument = document.implementation.createHTMLDocument('virtual');
-        var htmlElement = $(htmlString, virtualDocument);
-        htmlElement.find('.headerlink').remove();
-        docContent = htmlElement.find('[role=main]')[0];
-        if (docContent === undefined) {
-            console.warn("Content block not found. Sphinx search tries to obtain it " +
-                "via '[role=main]'. Could you check your theme or template.");
-            return "";
-        }
-        return docContent.textContent || docContent.innerText;
+    htmlToText: (htmlString) => {
+        const htmlElement = new DOMParser().parseFromString(htmlString, 'text/html');
+        htmlElement.querySelectorAll(".headerlink").forEach((el) => {
+            el.remove()
+        });
+        const docContent = htmlElement.querySelector('[role="main"]');
+        if (docContent !== undefined) return docContent.textContent;
+        console.warn(
+            "Content block not found. Sphinx search tries to obtain it via '[role=main]'. Could you check your theme or template."
+        );
+        return "";
     },
 
-    init: function() {
-        var params = $.getQueryParameters();
-        if (params.q) {
-            var query = params.q[0];
-            $('input[name="q"]')[0].value = query;
-            this.performSearch(query);
-        }
+    init: () => {
+        const query = new URLSearchParams(window.location.search).get("q");
+        document
+            .querySelectorAll('input[name="q"]')
+            .forEach((el) => (el.value = query));
+        if (query) Search.performSearch(query);
     },
 
-    loadIndex: function(url) {
-        $.ajax({
-            type: "GET",
-            url: url,
-            data: null,
-            dataType: "script",
-            cache: true,
-            complete: function(jqxhr, textstatus) {
-                if (textstatus != "success") {
-                    document.getElementById("searchindexloader").src = url;
-                }
-            }
-        });
-    },
+    loadIndex: (url) =>
+        (document.body.appendChild(document.createElement("script")).src = url),
 
-    setIndex: function(index) {
-        var q;
-        this._index = index;
-        if ((q = this._queued_query) !== null) {
-            this._queued_query = null;
-            Search.query(q);
+    setIndex: (index) => {
+        Search._index = index;
+        if (Search._queued_query !== null) {
+            const query = Search._queued_query;
+            Search._queued_query = null;
+            Search.query(query);
         }
     },
 
-    hasIndex: function() {
-        return this._index !== null;
-    },
+    hasIndex: () => Search._index !== null,
 
-    deferQuery: function(query) {
-        this._queued_query = query;
-    },
+    deferQuery: (query) => (Search._queued_query = query),
 
-    stopPulse: function() {
-        this._pulse_status = 0;
-    },
+    stopPulse: () => (Search._pulse_status = -1),
 
-    startPulse: function() {
-        if (this._pulse_status >= 0)
-            return;
+    startPulse: () => {
+        if (Search._pulse_status >= 0) return;
 
-        function pulse() {
-            var i;
+        const pulse = () => {
             Search._pulse_status = (Search._pulse_status + 1) % 4;
-            var dotString = '';
-            for (i = 0; i < Search._pulse_status; i++)
-                dotString += '.';
-            Search.dots.text(dotString);
-            if (Search._pulse_status > -1)
-                window.setTimeout(pulse, 500);
-        }
+            Search.dots.innerText = ".".repeat(Search._pulse_status);
+            if (Search._pulse_status >= 0) window.setTimeout(pulse, 500);
+        };
         pulse();
     },
 
     /**
      * perform a search for something (or wait until index is loaded)
      */
-    performSearch: function(query) {
+    performSearch: (query) => {
         // create the required interface elements
-        this.out = $('#search-results');
-        this.title = $('<h2>' + _('Searching') + '</h2>').appendTo(this.out);
-        this.dots = $('<span></span>').appendTo(this.title);
-        this.status = $('<p class="search-summary">&nbsp;</p>').appendTo(this.out);
-        this.output = $('<ul class="search"/>').appendTo(this.out);
-
-        $('#search-progress').text(_('Preparing search...'));
-        this.startPulse();
+        const searchText = document.createElement("h2");
+        searchText.textContent = _("Searching");
+        const searchSummary = document.createElement("p");
+        searchSummary.classList.add("search-summary");
+        searchSummary.innerText = "";
+        const searchList = document.createElement("ul");
+        searchList.classList.add("search");
+
+        const out = document.getElementById("search-results");
+        Search.title = out.appendChild(searchText);
+        Search.dots = Search.title.appendChild(document.createElement("span"));
+        Search.status = out.appendChild(searchSummary);
+        Search.output = out.appendChild(searchList);
+
+        const searchProgress = document.getElementById("search-progress");
+        // Some themes don't use the search progress node
+        if (searchProgress) {
+            searchProgress.innerText = _("Preparing search...");
+        }
+        Search.startPulse();
 
         // index already loaded, the browser was quick!
-        if (this.hasIndex())
-            this.query(query);
-        else
-            this.deferQuery(query);
+        if (Search.hasIndex()) Search.query(query);
+        else Search.deferQuery(query);
     },
 
     /**
      * execute search (requires search index to be loaded)
      */
-    query: function(query) {
-        var i;
+    query: (query) => {
+        const filenames = Search._index.filenames;
+        const docNames = Search._index.docnames;
+        const titles = Search._index.titles;
+        const allTitles = Search._index.alltitles;
+        const indexEntries = Search._index.indexentries;
+
+        // stem the search terms and add them to the correct list
+        const stemmer = new Stemmer();
+        const searchTerms = new Set();
+        const excludedTerms = new Set();
+        const highlightTerms = new Set();
+        const objectTerms = new Set(splitQuery(query.toLowerCase().trim()));
+        splitQuery(query.trim()).forEach((queryTerm) => {
+            const queryTermLower = queryTerm.toLowerCase();
 
-        // stem the searchterms and add them to the correct list
-        var stemmer = new Stemmer();
-        var searchterms = [];
-        var excluded = [];
-        var hlterms = [];
-        var tmp = splitQuery(query);
-        var objectterms = [];
-        for (i = 0; i < tmp.length; i++) {
-            if (tmp[i] !== "") {
-                objectterms.push(tmp[i].toLowerCase());
-            }
+            // maybe skip this "word"
+            // stopwords array is from language_data.js
+            if (
+                stopwords.indexOf(queryTermLower) !== -1 ||
+                queryTerm.match(/^\d+$/)
+            )
+                return;
 
-            if ($u.indexOf(stopwords, tmp[i].toLowerCase()) != -1 || tmp[i] === "") {
-                // skip this "word"
-                continue;
-            }
             // stem the word
-            var word = stemmer.stemWord(tmp[i].toLowerCase());
-            // prevent stemmer from cutting word smaller than two chars
-            if (word.length < 3 && tmp[i].length >= 3) {
-                word = tmp[i];
-            }
-            var toAppend;
+            let word = stemmer.stemWord(queryTermLower);
             // select the correct list
-            if (word[0] == '-') {
-                toAppend = excluded;
-                word = word.substr(1);
-            } else {
-                toAppend = searchterms;
-                hlterms.push(tmp[i].toLowerCase());
+            if (word[0] === "-") excludedTerms.add(word.substr(1));
+            else {
+                searchTerms.add(word);
+                highlightTerms.add(queryTermLower);
             }
-            // only add if not already in the list
-            if (!$u.contains(toAppend, word))
-                toAppend.push(word);
-        }
-        var highlightstring = '?highlight=' + $.urlencode(hlterms.join(" "));
+        });
 
-        // console.debug('SEARCH: searching for:');
-        // console.info('required: ', searchterms);
-        // console.info('excluded: ', excluded);
+        if (SPHINX_HIGHLIGHT_ENABLED) { // set in sphinx_highlight.js
+            localStorage.setItem("sphinx_highlight_terms", [...highlightTerms].join(" "))
+        }
 
-        // prepare search
-        var terms = this._index.terms;
-        var titleterms = this._index.titleterms;
+        // console.debug("SEARCH: searching for:");
+        // console.info("required: ", [...searchTerms]);
+        // console.info("excluded: ", [...excludedTerms]);
+
+        // array of [docname, title, anchor, descr, score, filename]
+        let results = [];
+        _removeChildren(document.getElementById("search-progress"));
+
+        const queryLower = query.toLowerCase();
+        for (const [title, foundTitles] of Object.entries(allTitles)) {
+            if (title.toLowerCase().includes(queryLower) && (queryLower.length >= title.length / 2)) {
+                for (const [file, id] of foundTitles) {
+                    let score = Math.round(100 * queryLower.length / title.length)
+                    results.push([
+                        docNames[file],
+                        titles[file] !== title ? `${titles[file]} > ${title}` : title,
+                        id !== null ? "#" + id : "",
+                        null,
+                        score,
+                        filenames[file],
+                    ]);
+                }
+            }
+        }
 
-        // array of [filename, title, anchor, descr, score]
-        var results = [];
-        $('#search-progress').empty();
+        // search for explicit entries in index directives
+        for (const [entry, foundEntries] of Object.entries(indexEntries)) {
+            if (entry.includes(queryLower) && (queryLower.length >= entry.length / 2)) {
+                for (const [file, id] of foundEntries) {
+                    let score = Math.round(100 * queryLower.length / entry.length)
+                    results.push([
+                        docNames[file],
+                        titles[file],
+                        id ? "#" + id : "",
+                        null,
+                        score,
+                        filenames[file],
+                    ]);
+                }
+            }
+        }
 
         // lookup as object
-        for (i = 0; i < objectterms.length; i++) {
-            var others = [].concat(objectterms.slice(0, i),
-                objectterms.slice(i + 1, objectterms.length));
-            results = results.concat(this.performObjectSearch(objectterms[i], others));
-        }
+        objectTerms.forEach((term) =>
+            results.push(...Search.performObjectSearch(term, objectTerms))
+        );
 
         // lookup as search terms in fulltext
-        results = results.concat(this.performTermsSearch(searchterms, excluded, terms, titleterms));
+        results.push(...Search.performTermsSearch(searchTerms, excludedTerms));
 
         // let the scorer override scores with a custom scoring function
-        if (Scorer.score) {
-            for (i = 0; i < results.length; i++)
-                results[i][4] = Scorer.score(results[i]);
-        }
+        if (Scorer.score) results.forEach((item) => (item[4] = Scorer.score(item)));
 
         // now sort the results by score (in opposite order of appearance, since the
         // display function below uses pop() to retrieve items) and then
         // alphabetically
-        results.sort(function(a, b) {
-            var left = a[4];
-            var right = b[4];
-            if (left > right) {
-                return 1;
-            } else if (left < right) {
-                return -1;
-            } else {
+        results.sort((a, b) => {
+            const leftScore = a[4];
+            const rightScore = b[4];
+            if (leftScore === rightScore) {
                 // same score: sort alphabetically
-                left = a[1].toLowerCase();
-                right = b[1].toLowerCase();
-                return (left > right) ? -1 : ((left < right) ? 1 : 0);
+                const leftTitle = a[1].toLowerCase();
+                const rightTitle = b[1].toLowerCase();
+                if (leftTitle === rightTitle) return 0;
+                return leftTitle > rightTitle ? -1 : 1; // inverted is intentional
             }
+            return leftScore > rightScore ? 1 : -1;
         });
 
+        // remove duplicate search results
+        // note the reversing of results, so that in the case of duplicates, the highest-scoring entry is kept
+        let seen = new Set();
+        results = results.reverse().reduce((acc, result) => {
+            let resultStr = result.slice(0, 4).concat([result[5]]).map(v => String(v)).join(',');
+            if (!seen.has(resultStr)) {
+                acc.push(result);
+                seen.add(resultStr);
+            }
+            return acc;
+        }, []);
+
+        results = results.reverse();
+
         // for debugging
         //Search.lastresults = results.slice();  // a copy
-        //console.info('search results:', Search.lastresults);
+        // console.info("search results:", Search.lastresults);
 
         // print the results
-        var resultCount = results.length;
-
-        function displayNextItem() {
-            // results left, load the summary and display it
-            if (results.length) {
-                var item = results.pop();
-                var listItem = $('<li></li>');
-                var requestUrl = "";
-                var linkUrl = "";
-                if (DOCUMENTATION_OPTIONS.BUILDER === 'dirhtml') {
-                    // dirhtml builder
-                    var dirname = item[0] + '/';
-                    if (dirname.match(/\/index\/$/)) {
-                        dirname = dirname.substring(0, dirname.length - 6);
-                    } else if (dirname == 'index/') {
-                        dirname = '';
-                    }
-                    requestUrl = DOCUMENTATION_OPTIONS.URL_ROOT + dirname;
-                    linkUrl = requestUrl;
-
-                } else {
-                    // normal html builders
-                    requestUrl = DOCUMENTATION_OPTIONS.URL_ROOT + item[0] + DOCUMENTATION_OPTIONS.FILE_SUFFIX;
-                    linkUrl = item[0] + DOCUMENTATION_OPTIONS.LINK_SUFFIX;
-                }
-                listItem.append($('<a/>').attr('href',
-                    linkUrl +
-                    highlightstring + item[2]).html(item[1]));
-                if (item[3]) {
-                    listItem.append($('<span> (' + item[3] + ')</span>'));
-                    Search.output.append(listItem);
-                    setTimeout(function() {
-                        displayNextItem();
-                    }, 5);
-                } else if (DOCUMENTATION_OPTIONS.HAS_SOURCE) {
-                    $.ajax({
-                        url: requestUrl,
-                        dataType: "text",
-                        complete: function(jqxhr, textstatus) {
-                            var data = jqxhr.responseText;
-                            if (data !== '' && data !== undefined) {
-                                var summary = Search.makeSearchSummary(data, searchterms, hlterms);
-                                if (summary) {
-                                    listItem.append(summary);
-                                }
-                            }
-                            Search.output.append(listItem);
-                            setTimeout(function() {
-                                displayNextItem();
-                            }, 5);
-                        }
-                    });
-                } else {
-                    // no source available, just display title
-                    Search.output.append(listItem);
-                    setTimeout(function() {
-                        displayNextItem();
-                    }, 5);
-                }
-            }
-            // search finished, update title and status message
-            else {
-                Search.stopPulse();
-                Search.title.text(_('Search Results'));
-                if (!resultCount)
-                    Search.status.text(_('Your search did not match any documents. Please make sure that all words are spelled correctly and that you\'ve selected enough categories.'));
-                else
-                    Search.status.text(_('Search finished, found %s page(s) matching the search query.').replace('%s', resultCount));
-                Search.status.fadeIn(500);
-            }
-        }
-        displayNextItem();
+        _displayNextItem(results, results.length, searchTerms);
     },
 
     /**
      * search for object names
      */
-    performObjectSearch: function(object, otherterms) {
-        var filenames = this._index.filenames;
-        var docnames = this._index.docnames;
-        var objects = this._index.objects;
-        var objnames = this._index.objnames;
-        var titles = this._index.titles;
-
-        var i;
-        var results = [];
-
-        for (var prefix in objects) {
-            for (var name in objects[prefix]) {
-                var fullname = (prefix ? prefix + '.' : '') + name;
-                var fullnameLower = fullname.toLowerCase()
-                if (fullnameLower.indexOf(object) > -1) {
-                    var score = 0;
-                    var parts = fullnameLower.split('.');
-                    // check for different match types: exact matches of full name or
-                    // "last name" (i.e. last dotted part)
-                    if (fullnameLower == object || parts[parts.length - 1] == object) {
-                        score += Scorer.objNameMatch;
-                        // matches in last name
-                    } else if (parts[parts.length - 1].indexOf(object) > -1) {
-                        score += Scorer.objPartialMatch;
-                    }
-                    var match = objects[prefix][name];
-                    var objname = objnames[match[1]][2];
-                    var title = titles[match[0]];
-                    // If more than one term searched for, we require other words to be
-                    // found in the name/title/description
-                    if (otherterms.length > 0) {
-                        var haystack = (prefix + ' ' + name + ' ' +
-                            objname + ' ' + title).toLowerCase();
-                        var allfound = true;
-                        for (i = 0; i < otherterms.length; i++) {
-                            if (haystack.indexOf(otherterms[i]) == -1) {
-                                allfound = false;
-                                break;
-                            }
-                        }
-                        if (!allfound) {
-                            continue;
-                        }
-                    }
-                    var descr = objname + _(', in ') + title;
-
-                    var anchor = match[3];
-                    if (anchor === '')
-                        anchor = fullname;
-                    else if (anchor == '-')
-                        anchor = objnames[match[1]][1] + '-' + fullname;
-                    // add custom score for some objects according to scorer
-                    if (Scorer.objPrio.hasOwnProperty(match[2])) {
-                        score += Scorer.objPrio[match[2]];
-                    } else {
-                        score += Scorer.objPrioDefault;
-                    }
-                    results.push([docnames[match[0]], fullname, '#' + anchor, descr, score, filenames[match[0]]]);
-                }
-            }
-        }
-
+    performObjectSearch: (object, objectTerms) => {
+        const filenames = Search._index.filenames;
+        const docNames = Search._index.docnames;
+        const objects = Search._index.objects;
+        const objNames = Search._index.objnames;
+        const titles = Search._index.titles;
+
+        const results = [];
+
+        const objectSearchCallback = (prefix, match) => {
+            const name = match[4]
+            const fullname = (prefix ? prefix + "." : "") + name;
+            const fullnameLower = fullname.toLowerCase();
+            if (fullnameLower.indexOf(object) < 0) return;
+
+            let score = 0;
+            const parts = fullnameLower.split(".");
+
+            // check for different match types: exact matches of full name or
+            // "last name" (i.e. last dotted part)
+            if (fullnameLower === object || parts.slice(-1)[0] === object)
+                score += Scorer.objNameMatch;
+            else if (parts.slice(-1)[0].indexOf(object) > -1)
+                score += Scorer.objPartialMatch; // matches in last name
+
+            const objName = objNames[match[1]][2];
+            const title = titles[match[0]];
+
+            // If more than one term searched for, we require other words to be
+            // found in the name/title/description
+            const otherTerms = new Set(objectTerms);
+            otherTerms.delete(object);
+            if (otherTerms.size > 0) {
+                const haystack = `${prefix} ${name} ${objName} ${title}`.toLowerCase();
+                if (
+                    [...otherTerms].some((otherTerm) => haystack.indexOf(otherTerm) < 0)
+                )
+                    return;
+            }
+
+            let anchor = match[3];
+            if (anchor === "") anchor = fullname;
+            else if (anchor === "-") anchor = objNames[match[1]][1] + "-" + fullname;
+
+            const descr = objName + _(", in ") + title;
+
+            // add custom score for some objects according to scorer
+            if (Scorer.objPrio.hasOwnProperty(match[2]))
+                score += Scorer.objPrio[match[2]];
+            else score += Scorer.objPrioDefault;
+
+            results.push([
+                docNames[match[0]],
+                fullname,
+                "#" + anchor,
+                descr,
+                score,
+                filenames[match[0]],
+            ]);
+        };
+        Object.keys(objects).forEach((prefix) =>
+            objects[prefix].forEach((array) =>
+                objectSearchCallback(prefix, array)
+            )
+        );
         return results;
     },
 
     /**
-     * See https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions
-     */
-    escapeRegExp: function(string) {
-        return string.replace(/[.*+\-?^${}()|[\]\\]/g, '\\$&'); // $& means the whole matched string
-    },
-
-    /**
      * search for full-text terms in the index
      */
-    performTermsSearch: function(searchterms, excluded, terms, titleterms) {
-        var docnames = this._index.docnames;
-        var filenames = this._index.filenames;
-        var titles = this._index.titles;
-
-        var i, j, file;
-        var fileMap = {};
-        var scoreMap = {};
-        var results = [];
+    performTermsSearch: (searchTerms, excludedTerms) => {
+        // prepare search
+        const terms = Search._index.terms;
+        const titleTerms = Search._index.titleterms;
+        const filenames = Search._index.filenames;
+        const docNames = Search._index.docnames;
+        const titles = Search._index.titles;
+
+        const scoreMap = new Map();
+        const fileMap = new Map();
 
         // perform the search on the required terms
-        for (i = 0; i < searchterms.length; i++) {
-            var word = searchterms[i];
-            var files = [];
-            var _o = [{
+        searchTerms.forEach((word) => {
+            const files = [];
+            const arr = [{
                 files: terms[word],
                 score: Scorer.term
             }, {
-                files: titleterms[word],
+                files: titleTerms[word],
                 score: Scorer.title
-            }];
+            }, ];
             // add support for partial matches
             if (word.length > 2) {
-                var word_regex = this.escapeRegExp(word);
-                for (var w in terms) {
-                    if (w.match(word_regex) && !terms[word]) {
-                        _o.push({
-                            files: terms[w],
+                const escapedWord = _escapeRegExp(word);
+                Object.keys(terms).forEach((term) => {
+                    if (term.match(escapedWord) && !terms[word])
+                        arr.push({
+                            files: terms[term],
                             score: Scorer.partialTerm
-                        })
-                    }
-                }
-                for (var w in titleterms) {
-                    if (w.match(word_regex) && !titleterms[word]) {
-                        _o.push({
-                            files: titleterms[w],
+                        });
+                });
+                Object.keys(titleTerms).forEach((term) => {
+                    if (term.match(escapedWord) && !titleTerms[word])
+                        arr.push({
+                            files: titleTerms[word],
                             score: Scorer.partialTitle
-                        })
-                    }
-                }
+                        });
+                });
             }
 
             // no match but word was a required one
-            if ($u.every(_o, function(o) {
-                    return o.files === undefined;
-                })) {
-                break;
-            }
+            if (arr.every((record) => record.files === undefined)) return;
+
             // found search word in contents
-            $u.each(_o, function(o) {
-                var _files = o.files;
-                if (_files === undefined)
-                    return
-
-                if (_files.length === undefined)
-                    _files = [_files];
-                files = files.concat(_files);
-
-                // set score for the word in each file to Scorer.term
-                for (j = 0; j < _files.length; j++) {
-                    file = _files[j];
-                    if (!(file in scoreMap))
-                        scoreMap[file] = {};
-                    scoreMap[file][word] = o.score;
-                }
+            arr.forEach((record) => {
+                if (record.files === undefined) return;
+
+                let recordFiles = record.files;
+                if (recordFiles.length === undefined) recordFiles = [recordFiles];
+                files.push(...recordFiles);
+
+                // set score for the word in each file
+                recordFiles.forEach((file) => {
+                    if (!scoreMap.has(file)) scoreMap.set(file, {});
+                    scoreMap.get(file)[word] = record.score;
+                });
             });
 
             // create the mapping
-            for (j = 0; j < files.length; j++) {
-                file = files[j];
-                if (file in fileMap && fileMap[file].indexOf(word) === -1)
-                    fileMap[file].push(word);
-                else
-                    fileMap[file] = [word];
-            }
-        }
+            files.forEach((file) => {
+                if (fileMap.has(file) && fileMap.get(file).indexOf(word) === -1)
+                    fileMap.get(file).push(word);
+                else fileMap.set(file, [word]);
+            });
+        });
 
         // now check if the files don't contain excluded terms
-        for (file in fileMap) {
-            var valid = true;
-
+        const results = [];
+        for (const [file, wordList] of fileMap) {
             // check if all requirements are matched
-            var filteredTermCount = // as search terms with length < 3 are discarded: ignore
-                searchterms.filter(function(term) {
-                    return term.length > 2
-                }).length
+
+            // as search terms with length < 3 are discarded
+            const filteredTermCount = [...searchTerms].filter(
+                (term) => term.length > 2
+            ).length;
             if (
-                fileMap[file].length != searchterms.length &&
-                fileMap[file].length != filteredTermCount
-            ) continue;
+                wordList.length !== searchTerms.size &&
+                wordList.length !== filteredTermCount
+            )
+                continue;
 
             // ensure that none of the excluded terms is in the search result
-            for (i = 0; i < excluded.length; i++) {
-                if (terms[excluded[i]] == file ||
-                    titleterms[excluded[i]] == file ||
-                    $u.contains(terms[excluded[i]] || [], file) ||
-                    $u.contains(titleterms[excluded[i]] || [], file)) {
-                    valid = false;
-                    break;
-                }
-            }
+            if (
+                [...excludedTerms].some(
+                    (term) =>
+                    terms[term] === file ||
+                    titleTerms[term] === file ||
+                    (terms[term] || []).includes(file) ||
+                    (titleTerms[term] || []).includes(file)
+                )
+            )
+                break;
 
-            // if we have still a valid result we can add it to the result list
-            if (valid) {
-                // select one (max) score for the file.
-                // for better ranking, we should calculate ranking by using words statistics like basic tf-idf...
-                var score = $u.max($u.map(fileMap[file], function(w) {
-                    return scoreMap[file][w]
-                }));
-                results.push([docnames[file], titles[file], '', null, score, filenames[file]]);
-            }
+            // select one (max) score for the file.
+            const score = Math.max(...wordList.map((w) => scoreMap.get(file)[w]));
+            // add result to the result list
+            results.push([
+                docNames[file],
+                titles[file],
+                "",
+                null,
+                score,
+                filenames[file],
+            ]);
         }
         return results;
     },
 
     /**
      * helper function to return a node containing the
      * search summary for a given text. keywords is a list
-     * of stemmed words, hlwords is the list of normal, unstemmed
-     * words. the first one is used to find the occurrence, the
-     * latter for highlighting it.
+     * of stemmed words.
      */
-    makeSearchSummary: function(htmlText, keywords, hlwords) {
-        var text = Search.htmlToText(htmlText);
-        if (text == "") {
-            return null;
-        }
-        var textLower = text.toLowerCase();
-        var start = 0;
-        $.each(keywords, function() {
-            var i = textLower.indexOf(this.toLowerCase());
-            if (i > -1)
-                start = i;
-        });
-        start = Math.max(start - 120, 0);
-        var excerpt = ((start > 0) ? '...' : '') +
-            $.trim(text.substr(start, 240)) +
-            ((start + 240 - text.length) ? '...' : '');
-        var rv = $('<p class="context"></p>').text(excerpt);
-        $.each(hlwords, function() {
-            rv = rv.highlightText(this, 'highlighted');
-        });
-        return rv;
-    }
+    makeSearchSummary: (htmlText, keywords) => {
+        const text = Search.htmlToText(htmlText);
+        if (text === "") return null;
+
+        const textLower = text.toLowerCase();
+        const actualStartPosition = [...keywords]
+            .map((k) => textLower.indexOf(k.toLowerCase()))
+            .filter((i) => i > -1)
+            .slice(-1)[0];
+        const startWithContext = Math.max(actualStartPosition - 120, 0);
+
+        const top = startWithContext === 0 ? "" : "...";
+        const tail = startWithContext + 240 < text.length ? "..." : "";
+
+        let summary = document.createElement("p");
+        summary.classList.add("context");
+        summary.textContent = top + text.substr(startWithContext, 240).trim() + tail;
+
+        return summary;
+    },
 };
 
-$(document).ready(function() {
-    Search.init();
-});
+_ready(Search.init);
```

### Comparing `plink-2.4.1/plink_src/doc/_static/underscore-1.13.1.js` & `plink-2.4.2/plink_src/doc/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `plink-2.4.1/plink_src/doc/_static/underscore.js` & `plink-2.4.2/plink_src/doc/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `plink-2.4.1/plink_src/doc/genindex.html` & `plink-2.4.2/plink_src/doc/genindex.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 
 <!DOCTYPE html>
 
-<html>
+<html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Index &#8212; PLink 2.4.1 documentation</title>
+    <title>Index &#8212; PLink 2.4.2 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/classic.css" />
     
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
-    <script src="_static/jquery.js"></script>
-    <script src="_static/underscore.js"></script>
     <script src="_static/doctools.js"></script>
+    <script src="_static/sphinx_highlight.js"></script>
     
     <link rel="index" title="Index" href="#" />
     <link rel="search" title="Search" href="search.html" /> 
   </head><body>
     <div class="related" role="navigation" aria-label="related navigation">
       <h3>Navigation</h3>
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="#" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">PLink 2.4.1 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">PLink 2.4.2 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Index</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -343,31 +342,31 @@
     <div class="searchformwrapper">
     <form class="search" action="search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
 </div>
-<script>$('#searchbox').show(0);</script>
+<script>document.getElementById('searchbox').style.display = "block"</script>
         </div>
       </div>
       <div class="clearer"></div>
     </div>
     <div class="related" role="navigation" aria-label="related navigation">
       <h3>Navigation</h3>
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="#" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">PLink 2.4.1 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">PLink 2.4.2 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Index</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2009-present, Marc Culler, Nathan Dunfield and others.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 4.2.0.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.1.3.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 
 
 
 
 **** Navigation ****
     * index
     * modules |
-    * PLink_2.4.1_documentation »
+    * PLink_2.4.2_documentation »
     * Index
 ****** Index ******
 A | C | D | E | F | G | H | L | M | N | P | R | S | T | U | V
 ***** A *****
     * active_crossing_data()_       * Arrow_(class_in_plink.arrow)
       (plink.LinkEditor_method)     * attach_cursor()_(plink.LinkEditor
                                       method)
@@ -94,11 +94,11 @@
     * vectorize()_(plink.arrow.Arrow     * verify_drag()_(plink.LinkEditor
       method)                              method)
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
-    * PLink_2.4.1_documentation »
+    * PLink_2.4.2_documentation »
     * Index
 © Copyright 2009-present, Marc Culler, Nathan Dunfield and others. Created
-using Sphinx 4.2.0.
+using Sphinx 6.1.3.
```

### Comparing `plink-2.4.1/plink_src/doc/index.html` & `plink-2.4.2/plink_src/doc/index.html`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 
 <!DOCTYPE html>
 
-<html>
+<html lang="en">
   <head>
     <meta charset="utf-8" />
-    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>How to use PLink &#8212; PLink 2.4.1 documentation</title>
+    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
+
+    <title>How to use PLink &#8212; PLink 2.4.2 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/classic.css" />
     
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
-    <script src="_static/jquery.js"></script>
-    <script src="_static/underscore.js"></script>
     <script src="_static/doctools.js"></script>
+    <script src="_static/sphinx_highlight.js"></script>
     
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="Installing and running PLink" href="installing.html" /> 
   </head><body>
     <div class="related" role="navigation" aria-label="related navigation">
       <h3>Navigation</h3>
@@ -26,32 +26,32 @@
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
           <a href="installing.html" title="Installing and running PLink"
              accesskey="N">next</a> |</li>
-        <li class="nav-item nav-item-0"><a href="#">PLink 2.4.1 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="#">PLink 2.4.2 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">How to use PLink</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
           <div class="body" role="main">
             
-  <div class="section" id="how-to-use-plink">
-<h1>How to use PLink<a class="headerlink" href="#how-to-use-plink" title="Permalink to this headline">¶</a></h1>
+  <section id="how-to-use-plink">
+<h1>How to use PLink<a class="headerlink" href="#how-to-use-plink" title="Permalink to this heading">¶</a></h1>
 <p>PLink draws piecewise linear link projections.  Components may be
 points, PL arcs, or PL circles.  Line segments are oriented consistently in
 each component.  Different components are different colors.</p>
 <img alt="_images/plink-action.png" src="_images/plink-action.png" />
-<div class="section" id="drawing-basics">
-<h2>Drawing Basics<a class="headerlink" href="#drawing-basics" title="Permalink to this headline">¶</a></h2>
+<section id="drawing-basics">
+<h2>Drawing Basics<a class="headerlink" href="#drawing-basics" title="Permalink to this heading">¶</a></h2>
 <ul class="simple">
 <li><p>When using the mouse to draw a link with PLink, you should always
 <em>click-and-release</em>.  Do not hold the mouse button down while drawing.
 PLink requires only the left mouse button.</p></li>
 <li><p>The default state of the editor is indicated by the arrow cursor.
 In this state, click-and-release the left mouse button on the
 background to place a starting vertex and begin drawing.  The vertex
@@ -89,34 +89,34 @@
 Delete to remove the incoming segment at that vertex; then click the
 vertex again to reconnect.</p></li>
 <li><p>You will not be allowed to create edges that pass too close to a
 vertex or a crossing, or to place vertices too close to edges or to
 crossings or to other vertices.  If you attempt to do any of these
 things, <em>PLink will beep at you</em>.</p></li>
 </ul>
-</div>
-<div class="section" id="miscellaneous-features">
-<h2>Miscellaneous Features<a class="headerlink" href="#miscellaneous-features" title="Permalink to this headline">¶</a></h2>
+</section>
+<section id="miscellaneous-features">
+<h2>Miscellaneous Features<a class="headerlink" href="#miscellaneous-features" title="Permalink to this heading">¶</a></h2>
 <p>The window can be resized to allow for different sizes of link
 projections, and the arrow keys can be used to slide the projection
 around in order to make more room on one side or another.  The keys
-‘+’, ‘-‘, and ‘0’ can be used to zoom in, zoom out, or resize the
+‘+’, ‘-’, and ‘0’ can be used to zoom in, zoom out, or resize the
 diagram to fit the size of the window.</p>
 <p>The “Tools” menu can be used to make the projection alternating
 (provided that all components are circles), or to clear the screen, or
 to reflect the projection in the xy-plane, changing all crossings.
 The “Preserve diagram” option disables any operation which could
 change the combinatorics of the diagram; a vertex can be moved, but it
 cannot be moved across an edge and its adjacent edges cannot be moved
 across a vertex. The “Smooth” option opens a new window with a smooth
 version of the diagram, rendered with cubic Bezier splines.  When used
 within SnapPy, the “Tools” menu includes the “Send to SnapPy” command.</p>
 <p>There also are options in the “Tools” menu for zooming or panning
 the diagram, but these operations are usually more easily done with
-the arrow keys or the ‘+’, ‘-‘, and ‘0’ keys.</p>
+the arrow keys or the ‘+’, ‘-’, and ‘0’ keys.</p>
 <p>The “File” menu can be used to save the projection as a SnapPea
 link projection file.  (This can be done from the drawing state as
 well, in which case the “hot vertex” is remembered in the file!).  The
 “File-&gt;Open File” command will read a SnapPea link projection file,
 and restart drawing if the projection was saved while drawing.</p>
 <p>The “Info” menu selects information about the link projection to be
 displayed in the info line at the bottom.  Various encoding schemes
@@ -125,56 +125,66 @@
 pasting from the info line is supported.  The numerical and
 alphabetical Dowker-Thistlethwaite codes are displayed in an extended
 form which includes a full description of the planar embedding.  The
 string printed in the info line is also accepted as input to SnapPy’s
 Manifold constructor.  Paste the DT code between the apostrophes in
 Manifold(‘’).  The “DT labels” option displays the indexing used in
 computing the Dowker-Thistlethwaite codes.</p>
-</div>
-</div>
-<div class="section" id="credits">
-<h1>Credits<a class="headerlink" href="#credits" title="Permalink to this headline">¶</a></h1>
+</section>
+</section>
+<section id="credits">
+<h1>Credits<a class="headerlink" href="#credits" title="Permalink to this heading">¶</a></h1>
 <p>Written by <a class="reference external" href="http://math.uic.edu/~culler">Marc Culler</a> and <a class="reference external" href="http://dunfield.info">Nathan Dunfield</a>.</p>
-</div>
-<div class="section" id="contents">
-<h1>Contents<a class="headerlink" href="#contents" title="Permalink to this headline">¶</a></h1>
+</section>
+<section id="contents">
+<h1>Contents<a class="headerlink" href="#contents" title="Permalink to this heading">¶</a></h1>
 <div class="toctree-wrapper compound">
 <ul>
 <li class="toctree-l1"><a class="reference internal" href="installing.html">Installing and running PLink</a><ul>
 <li class="toctree-l2"><a class="reference internal" href="installing.html#mac-os-x">Mac OS X</a></li>
 <li class="toctree-l2"><a class="reference internal" href="installing.html#windows">Windows</a></li>
 <li class="toctree-l2"><a class="reference internal" href="installing.html#source-code">Source code</a></li>
 </ul>
 </li>
-<li class="toctree-l1"><a class="reference internal" href="plink.html">plink – A Python/Tk link editor</a></li>
+<li class="toctree-l1"><a class="reference internal" href="plink.html">plink – A Python/Tk link editor</a><ul>
+<li class="toctree-l2"><a class="reference internal" href="plink.html#plink.LinkEditor"><code class="docutils literal notranslate"><span class="pre">LinkEditor</span></code></a></li>
+<li class="toctree-l2"><a class="reference internal" href="plink.html#plink.arrow.Arrow"><code class="docutils literal notranslate"><span class="pre">Arrow</span></code></a></li>
+<li class="toctree-l2"><a class="reference internal" href="plink.html#plink.crossings.Crossing"><code class="docutils literal notranslate"><span class="pre">Crossing</span></code></a></li>
+<li class="toctree-l2"><a class="reference internal" href="plink.html#plink.crossings.ECrossing"><code class="docutils literal notranslate"><span class="pre">ECrossing</span></code></a></li>
+</ul>
+</li>
 </ul>
 </div>
-</div>
+</section>
 
 
             <div class="clearer"></div>
           </div>
         </div>
       </div>
       <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
         <div class="sphinxsidebarwrapper">
-  <h3><a href="#">Table of Contents</a></h3>
-  <ul>
+  <div>
+    <h3><a href="#">Table of Contents</a></h3>
+    <ul>
 <li><a class="reference internal" href="#">How to use PLink</a><ul>
 <li><a class="reference internal" href="#drawing-basics">Drawing Basics</a></li>
 <li><a class="reference internal" href="#miscellaneous-features">Miscellaneous Features</a></li>
 </ul>
 </li>
 <li><a class="reference internal" href="#credits">Credits</a></li>
 <li><a class="reference internal" href="#contents">Contents</a></li>
 </ul>
 
-  <h4>Next topic</h4>
-  <p class="topless"><a href="installing.html"
-                        title="next chapter">Installing and running PLink</a></p>
+  </div>
+  <div>
+    <h4>Next topic</h4>
+    <p class="topless"><a href="installing.html"
+                          title="next chapter">Installing and running PLink</a></p>
+  </div>
   <div role="note" aria-label="source link">
     <h3>This Page</h3>
     <ul class="this-page-menu">
       <li><a href="_sources/index.rst.txt"
             rel="nofollow">Show Source</a></li>
     </ul>
    </div>
@@ -183,15 +193,15 @@
     <div class="searchformwrapper">
     <form class="search" action="search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
 </div>
-<script>$('#searchbox').show(0);</script>
+<script>document.getElementById('searchbox').style.display = "block"</script>
         </div>
       </div>
       <div class="clearer"></div>
     </div>
     <div class="related" role="navigation" aria-label="related navigation">
       <h3>Navigation</h3>
       <ul>
@@ -200,17 +210,17 @@
              >index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
           <a href="installing.html" title="Installing and running PLink"
              >next</a> |</li>
-        <li class="nav-item nav-item-0"><a href="#">PLink 2.4.1 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="#">PLink 2.4.2 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">How to use PLink</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2009-present, Marc Culler, Nathan Dunfield and others.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 4.2.0.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.1.3.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -4,15 +4,15 @@
 
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
-    * PLink_2.4.1_documentation »
+    * PLink_2.4.2_documentation »
     * How to use PLink
 ****** How to use PLinkÂ¶ ******
 PLink draws piecewise linear link projections. Components may be points, PL
 arcs, or PL circles. Line segments are oriented consistently in each component.
 Different components are different colors.
 [_images/plink-action.png]
 ***** Drawing BasicsÂ¶ *****
@@ -51,31 +51,32 @@
       active component is removed. This can be used to remove a segment from
       the diagram. Double-click a vertex; hit Delete to remove the incoming
       segment at that vertex; then click the vertex again to reconnect.
     * You will not be allowed to create edges that pass too close to a vertex
       or a crossing, or to place vertices too close to edges or to crossings or
       to other vertices. If you attempt to do any of these things, PLink will
       beep at you.
+
 ***** Miscellaneous FeaturesÂ¶ *****
 The window can be resized to allow for different sizes of link projections, and
 the arrow keys can be used to slide the projection around in order to make more
-room on one side or another. The keys â+â, â-â, and â0â can be used
+room on one side or another. The keys â+â, â-â, and â0â can be used
 to zoom in, zoom out, or resize the diagram to fit the size of the window.
 The âToolsâ menu can be used to make the projection alternating (provided
 that all components are circles), or to clear the screen, or to reflect the
 projection in the xy-plane, changing all crossings. The âPreserve diagramâ
 option disables any operation which could change the combinatorics of the
 diagram; a vertex can be moved, but it cannot be moved across an edge and its
 adjacent edges cannot be moved across a vertex. The âSmoothâ option opens a
 new window with a smooth version of the diagram, rendered with cubic Bezier
 splines. When used within SnapPy, the âToolsâ menu includes the âSend to
 SnapPyâ command.
 There also are options in the âToolsâ menu for zooming or panning the
 diagram, but these operations are usually more easily done with the arrow keys
-or the â+â, â-â, and â0â keys.
+or the â+â, â-â, and â0â keys.
 The âFileâ menu can be used to save the projection as a SnapPea link
 projection file. (This can be done from the drawing state as well, in which
 case the âhot vertexâ is remembered in the file!). The âFile->Open
 Fileâ command will read a SnapPea link projection file, and restart drawing
 if the projection was saved while drawing.
 The âInfoâ menu selects information about the link projection to be
 displayed in the info line at the bottom. Various encoding schemes for link
@@ -83,22 +84,28 @@
 in meridian-longitude coordinates. Cutting and pasting from the info line is
 supported. The numerical and alphabetical Dowker-Thistlethwaite codes are
 displayed in an extended form which includes a full description of the planar
 embedding. The string printed in the info line is also accepted as input to
 SnapPyâs Manifold constructor. Paste the DT code between the apostrophes in
 Manifold(ââ). The âDT labelsâ option displays the indexing used in
 computing the Dowker-Thistlethwaite codes.
+
 ****** CreditsÂ¶ ******
 Written by Marc_Culler and Nathan_Dunfield.
+
 ****** ContentsÂ¶ ******
     * Installing_and_running_PLink
           o Mac_OS_X
           o Windows
           o Source_code
     * plink_â_A_Python/Tk_link_editor
+          o LinkEditor
+          o Arrow
+          o Crossing
+          o ECrossing
 **** Table_of_Contents ****
     * How_to_use_PLink
           o Drawing_Basics
           o Miscellaneous_Features
     * Credits
     * Contents
 *** Next topic ***
@@ -107,11 +114,11 @@
     * Show_Source
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
     * next |
-    * PLink_2.4.1_documentation »
+    * PLink_2.4.2_documentation »
     * How to use PLink
 © Copyright 2009-present, Marc Culler, Nathan Dunfield and others. Created
-using Sphinx 4.2.0.
+using Sphinx 6.1.3.
```

### Comparing `plink-2.4.1/plink_src/doc/installing.html` & `plink-2.4.2/plink_src/doc/installing.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 
 <!DOCTYPE html>
 
-<html>
+<html lang="en">
   <head>
     <meta charset="utf-8" />
-    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Installing and running PLink &#8212; PLink 2.4.1 documentation</title>
+    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
+
+    <title>Installing and running PLink &#8212; PLink 2.4.2 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/classic.css" />
     
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
-    <script src="_static/jquery.js"></script>
-    <script src="_static/underscore.js"></script>
     <script src="_static/doctools.js"></script>
+    <script src="_static/sphinx_highlight.js"></script>
     
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="plink – A Python/Tk link editor" href="plink.html" />
     <link rel="prev" title="How to use PLink" href="index.html" /> 
   </head><body>
     <div class="related" role="navigation" aria-label="related navigation">
@@ -30,34 +30,34 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="plink.html" title="plink – A Python/Tk link editor"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="index.html" title="How to use PLink"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">PLink 2.4.1 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">PLink 2.4.2 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Installing and running PLink</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
           <div class="body" role="main">
             
-  <div class="section" id="installing-and-running-plink">
-<h1>Installing and running PLink<a class="headerlink" href="#installing-and-running-plink" title="Permalink to this headline">¶</a></h1>
-<div class="section" id="mac-os-x">
-<h2>Mac OS X<a class="headerlink" href="#mac-os-x" title="Permalink to this headline">¶</a></h2>
+  <section id="installing-and-running-plink">
+<h1>Installing and running PLink<a class="headerlink" href="#installing-and-running-plink" title="Permalink to this heading">¶</a></h1>
+<section id="mac-os-x">
+<h2>Mac OS X<a class="headerlink" href="#mac-os-x" title="Permalink to this heading">¶</a></h2>
 <p>Simply download <a class="reference external" href="http://math.uic.edu/t3m/plink/PLink.dmg">PLink.dmg</a>
 and copy PLink.app to the Applications folder.  Double-click to start
 it, just like any other application.</p>
-</div>
-<div class="section" id="windows">
-<h2>Windows<a class="headerlink" href="#windows" title="Permalink to this headline">¶</a></h2>
+</section>
+<section id="windows">
+<h2>Windows<a class="headerlink" href="#windows" title="Permalink to this heading">¶</a></h2>
 <p>Install <a class="reference external" href="http://python.org">Python</a> and use <a class="reference external" href="https://pip.pypa.io/en/latest/">pip</a> (included in recent versions) to
 get plink.  For example:</p>
 <div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="n">pip</span> <span class="n">install</span> <span class="n">plink</span>
 <span class="n">python</span> <span class="o">-</span><span class="n">m</span> <span class="n">plink</span><span class="o">.</span><span class="n">app</span>
 </pre></div>
 </div>
 <hr class="docutils" />
@@ -70,45 +70,51 @@
 </div>
 <p>This installs a shell-command called “plink” which starts PLink.</p>
 <p>If you don’t have root privileges, add the “–user” flag to the end of
 the above install command.  You can then run plink via:</p>
 <div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="n">python</span> <span class="o">-</span><span class="n">m</span> <span class="n">plink</span><span class="o">.</span><span class="n">app</span>
 </pre></div>
 </div>
-</div>
-<div class="section" id="source-code">
-<h2>Source code<a class="headerlink" href="#source-code" title="Permalink to this headline">¶</a></h2>
+</section>
+<section id="source-code">
+<h2>Source code<a class="headerlink" href="#source-code" title="Permalink to this heading">¶</a></h2>
 <p>You can download and browse the source code
 <a class="reference external" href="https://github.com/3-manifolds/PLink">here</a>.</p>
-</div>
-</div>
+</section>
+</section>
 
 
             <div class="clearer"></div>
           </div>
         </div>
       </div>
       <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
         <div class="sphinxsidebarwrapper">
-  <h3><a href="index.html">Table of Contents</a></h3>
-  <ul>
+  <div>
+    <h3><a href="index.html">Table of Contents</a></h3>
+    <ul>
 <li><a class="reference internal" href="#">Installing and running PLink</a><ul>
 <li><a class="reference internal" href="#mac-os-x">Mac OS X</a></li>
 <li><a class="reference internal" href="#windows">Windows</a></li>
 <li><a class="reference internal" href="#source-code">Source code</a></li>
 </ul>
 </li>
 </ul>
 
-  <h4>Previous topic</h4>
-  <p class="topless"><a href="index.html"
-                        title="previous chapter">How to use PLink</a></p>
-  <h4>Next topic</h4>
-  <p class="topless"><a href="plink.html"
-                        title="next chapter">plink – A Python/Tk link editor</a></p>
+  </div>
+  <div>
+    <h4>Previous topic</h4>
+    <p class="topless"><a href="index.html"
+                          title="previous chapter">How to use PLink</a></p>
+  </div>
+  <div>
+    <h4>Next topic</h4>
+    <p class="topless"><a href="plink.html"
+                          title="next chapter">plink – A Python/Tk link editor</a></p>
+  </div>
   <div role="note" aria-label="source link">
     <h3>This Page</h3>
     <ul class="this-page-menu">
       <li><a href="_sources/installing.rst.txt"
             rel="nofollow">Show Source</a></li>
     </ul>
    </div>
@@ -117,15 +123,15 @@
     <div class="searchformwrapper">
     <form class="search" action="search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
 </div>
-<script>$('#searchbox').show(0);</script>
+<script>document.getElementById('searchbox').style.display = "block"</script>
         </div>
       </div>
       <div class="clearer"></div>
     </div>
     <div class="related" role="navigation" aria-label="related navigation">
       <h3>Navigation</h3>
       <ul>
@@ -137,17 +143,17 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="plink.html" title="plink – A Python/Tk link editor"
              >next</a> |</li>
         <li class="right" >
           <a href="index.html" title="How to use PLink"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">PLink 2.4.1 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">PLink 2.4.2 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Installing and running PLink</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2009-present, Marc Culler, Nathan Dunfield and others.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 4.2.0.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.1.3.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -6,20 +6,21 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * PLink_2.4.1_documentation »
+    * PLink_2.4.2_documentation »
     * Installing and running PLink
 ****** Installing and running PLinkÂ¶ ******
 ***** Mac OS XÂ¶ *****
 Simply download PLink.dmg and copy PLink.app to the Applications folder.
 Double-click to start it, just like any other application.
+
 ***** WindowsÂ¶ *****
 Install Python and use pip (included in recent versions) to get plink. For
 example:
 pip install plink
 python -m plink.app
 ===============================================================================
 You will need to have Python (> 2.4), Tk (>= 8.4), and Tkinter installed to run
@@ -27,16 +28,18 @@
 package âpython-tkâ.
 If you have root privileges and pip, simply do:
 pip install plink
 This installs a shell-command called âplinkâ which starts PLink.
 If you donât have root privileges, add the ââuserâ flag to the end of
 the above install command. You can then run plink via:
 python -m plink.app
+
 ***** Source codeÂ¶ *****
 You can download and browse the source code here.
+
 **** Table_of_Contents ****
     * Installing_and_running_PLink
           o Mac_OS_X
           o Windows
           o Source_code
 *** Previous topic ***
 How_to_use_PLink
@@ -47,11 +50,11 @@
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * PLink_2.4.1_documentation »
+    * PLink_2.4.2_documentation »
     * Installing and running PLink
 © Copyright 2009-present, Marc Culler, Nathan Dunfield and others. Created
-using Sphinx 4.2.0.
+using Sphinx 6.1.3.
```

### Comparing `plink-2.4.1/plink_src/doc/objects.inv` & `plink-2.4.2/plink_src/doc/objects.inv`

 * *Files 15% similar despite different names*

#### Sphinx inventory

```diff
@@ -1,10 +1,10 @@
 # Sphinx inventory version 2
 # Project: PLink
-# Version: 2.4.1
+# Version: 2.4.2
 # The remainder of this file is compressed using zlib.
 
 plink py:module 0 plink.html#module-$ -
 plink.LinkEditor py:class 1 plink.html#$ -
 plink.LinkEditor.active_crossing_data py:method 1 plink.html#$ -
 plink.LinkEditor.attach_cursor py:method 1 plink.html#$ -
 plink.LinkEditor.clear py:method 1 plink.html#$ -
```

### Comparing `plink-2.4.1/plink_src/doc/plink.html` & `plink-2.4.2/plink_src/doc/plink.html`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 
 <!DOCTYPE html>
 
-<html>
+<html lang="en">
   <head>
     <meta charset="utf-8" />
-    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>plink – A Python/Tk link editor &#8212; PLink 2.4.1 documentation</title>
+    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
+
+    <title>plink – A Python/Tk link editor &#8212; PLink 2.4.2 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/classic.css" />
     
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
-    <script src="_static/jquery.js"></script>
-    <script src="_static/underscore.js"></script>
     <script src="_static/doctools.js"></script>
+    <script src="_static/sphinx_highlight.js"></script>
     
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="prev" title="Installing and running PLink" href="installing.html" /> 
   </head><body>
     <div class="related" role="navigation" aria-label="related navigation">
       <h3>Navigation</h3>
@@ -26,31 +26,31 @@
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
           <a href="installing.html" title="Installing and running PLink"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">PLink 2.4.1 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">PLink 2.4.2 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">plink – A Python/Tk link editor</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
           <div class="body" role="main">
             
-  <div class="section" id="plink-a-python-tk-link-editor">
-<h1>plink – A Python/Tk link editor<a class="headerlink" href="#plink-a-python-tk-link-editor" title="Permalink to this headline">¶</a></h1>
+  <section id="plink-a-python-tk-link-editor">
+<h1>plink – A Python/Tk link editor<a class="headerlink" href="#plink-a-python-tk-link-editor" title="Permalink to this heading">¶</a></h1>
 <p>Technical documentation of the Python objects that underly PLink.  Of
 interest only to Marc, Nathan, or similar folks.</p>
 <span class="target" id="module-plink"></span><dl class="py class">
 <dt class="sig sig-object py" id="plink.LinkEditor">
-<em class="property"><span class="pre">class</span> </em><span class="sig-prename descclassname"><span class="pre">plink.</span></span><span class="sig-name descname"><span class="pre">LinkEditor</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="o"><span class="pre">*</span></span><span class="n"><span class="pre">args</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">**</span></span><span class="n"><span class="pre">kwargs</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#plink.LinkEditor" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">plink.</span></span><span class="sig-name descname"><span class="pre">LinkEditor</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="o"><span class="pre">*</span></span><span class="n"><span class="pre">args</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">**</span></span><span class="n"><span class="pre">kwargs</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#plink.LinkEditor" title="Permalink to this definition">¶</a></dt>
 <dd><p>A complete graphical link drawing tool based on the one embedded in Jeff Weeks’
 original SnapPea program.</p>
 <dl class="py method">
 <dt class="sig sig-object py" id="plink.LinkEditor.active_crossing_data">
 <span class="sig-name descname"><span class="pre">active_crossing_data</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="headerlink" href="#plink.LinkEditor.active_crossing_data" title="Permalink to this definition">¶</a></dt>
 <dd><p>Return the tuple of edges crossed by the in and out
 arrows of the active vertex.</p>
@@ -202,24 +202,24 @@
 
 </dd></dl>
 
 <span class="target" id="module-plink.arrow"></span><p>This module exports the class Arrow which represents a (directed)
 line segment in a PL link diagram.</p>
 <dl class="py class">
 <dt class="sig sig-object py" id="plink.arrow.Arrow">
-<em class="property"><span class="pre">class</span> </em><span class="sig-prename descclassname"><span class="pre">plink.arrow.</span></span><span class="sig-name descname"><span class="pre">Arrow</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">start</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">end</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">canvas</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">style</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'normal'</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">color</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'black'</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">other_params</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#plink.arrow.Arrow" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">plink.arrow.</span></span><span class="sig-name descname"><span class="pre">Arrow</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">start</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">end</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">canvas</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">style</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'normal'</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">color</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'black'</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">other_params</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#plink.arrow.Arrow" title="Permalink to this definition">¶</a></dt>
 <dd><p>An arrow in a PL link diagram.</p>
 <dl class="py method">
 <dt class="sig sig-object py" id="plink.arrow.Arrow.draw">
 <span class="sig-name descname"><span class="pre">draw</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">crossings</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">[]</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">recurse</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">True</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">skip_frozen</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">True</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#plink.arrow.Arrow.draw" title="Permalink to this definition">¶</a></dt>
 <dd></dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="plink.arrow.Arrow.epsilon">
-<span class="sig-name descname"><span class="pre">epsilon</span></span><em class="property"> <span class="pre">=</span> <span class="pre">8</span></em><a class="headerlink" href="#plink.arrow.Arrow.epsilon" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">epsilon</span></span><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">8</span></em><a class="headerlink" href="#plink.arrow.Arrow.epsilon" title="Permalink to this definition">¶</a></dt>
 <dd></dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="plink.arrow.Arrow.erase">
 <span class="sig-name descname"><span class="pre">erase</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="headerlink" href="#plink.arrow.Arrow.erase" title="Permalink to this definition">¶</a></dt>
 <dd><p>Prepare the arrow for the garbage collector.</p>
 </dd></dl>
@@ -245,20 +245,20 @@
 <dl class="py method">
 <dt class="sig sig-object py" id="plink.arrow.Arrow.freeze">
 <span class="sig-name descname"><span class="pre">freeze</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="headerlink" href="#plink.arrow.Arrow.freeze" title="Permalink to this definition">¶</a></dt>
 <dd></dd></dl>
 
 <dl class="py property">
 <dt class="sig sig-object py" id="plink.arrow.Arrow.frozen">
-<em class="property"><span class="pre">property</span> </em><span class="sig-name descname"><span class="pre">frozen</span></span><a class="headerlink" href="#plink.arrow.Arrow.frozen" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">frozen</span></span><a class="headerlink" href="#plink.arrow.Arrow.frozen" title="Permalink to this definition">¶</a></dt>
 <dd></dd></dl>
 
 <dl class="py property">
 <dt class="sig sig-object py" id="plink.arrow.Arrow.hidden">
-<em class="property"><span class="pre">property</span> </em><span class="sig-name descname"><span class="pre">hidden</span></span><a class="headerlink" href="#plink.arrow.Arrow.hidden" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">hidden</span></span><a class="headerlink" href="#plink.arrow.Arrow.hidden" title="Permalink to this definition">¶</a></dt>
 <dd></dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="plink.arrow.Arrow.hide">
 <span class="sig-name descname"><span class="pre">hide</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="headerlink" href="#plink.arrow.Arrow.hide" title="Permalink to this definition">¶</a></dt>
 <dd></dd></dl>
 
@@ -300,15 +300,15 @@
 </dd></dl>
 
 <span class="target" id="module-plink.crossings"></span><p>This module exports the Crossing class, which represents a crossing
 in a link diagram, and the ECrossing class which represents an edge
 of the diagram passing through a crossing.</p>
 <dl class="py class">
 <dt class="sig sig-object py" id="plink.crossings.Crossing">
-<em class="property"><span class="pre">class</span> </em><span class="sig-prename descclassname"><span class="pre">plink.crossings.</span></span><span class="sig-name descname"><span class="pre">Crossing</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">over</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">under</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">is_virtual</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">label</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#plink.crossings.Crossing" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">plink.crossings.</span></span><span class="sig-name descname"><span class="pre">Crossing</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">over</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">under</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">is_virtual</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">label</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#plink.crossings.Crossing" title="Permalink to this definition">¶</a></dt>
 <dd><p>A pair of crossing arrows in a PL link diagram.</p>
 <dl class="py method">
 <dt class="sig sig-object py" id="plink.crossings.Crossing.DT_hit">
 <span class="sig-name descname"><span class="pre">DT_hit</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">count</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">ecrossing</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#plink.crossings.Crossing.DT_hit" title="Permalink to this definition">¶</a></dt>
 <dd><p>Count the crossing, using DT conventions.  Return True on the
 first hit if the count is odd and the crossing is shared by
 two components of the diagram.  As a side effect, set the
@@ -350,41 +350,118 @@
 <span class="sig-name descname"><span class="pre">strand</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">arrow</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#plink.crossings.Crossing.strand" title="Permalink to this definition">¶</a></dt>
 <dd></dd></dl>
 
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="plink.crossings.ECrossing">
-<em class="property"><span class="pre">class</span> </em><span class="sig-prename descclassname"><span class="pre">plink.crossings.</span></span><span class="sig-name descname"><span class="pre">ECrossing</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">crossing</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">arrow</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#plink.crossings.ECrossing" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">plink.crossings.</span></span><span class="sig-name descname"><span class="pre">ECrossing</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">crossing</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">arrow</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#plink.crossings.ECrossing" title="Permalink to this definition">¶</a></dt>
 <dd><p>A pair: (Crossing, Arrow), where the Arrow is involved in the Crossing.
 The ECrossings correspond 1-1 with edges of the link diagram.</p>
 <dl class="py method">
 <dt class="sig sig-object py" id="plink.crossings.ECrossing.goes_over">
 <span class="sig-name descname"><span class="pre">goes_over</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="headerlink" href="#plink.crossings.ECrossing.goes_over" title="Permalink to this definition">¶</a></dt>
 <dd></dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="plink.crossings.ECrossing.pair">
 <span class="sig-name descname"><span class="pre">pair</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="headerlink" href="#plink.crossings.ECrossing.pair" title="Permalink to this definition">¶</a></dt>
 <dd></dd></dl>
 
 </dd></dl>
 
-</div>
+</section>
 
 
             <div class="clearer"></div>
           </div>
         </div>
       </div>
       <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
         <div class="sphinxsidebarwrapper">
-  <h4>Previous topic</h4>
-  <p class="topless"><a href="installing.html"
-                        title="previous chapter">Installing and running PLink</a></p>
+  <div>
+    <h3><a href="index.html">Table of Contents</a></h3>
+    <ul>
+<li><a class="reference internal" href="#">plink – A Python/Tk link editor</a><ul>
+<li><a class="reference internal" href="#plink.LinkEditor"><code class="docutils literal notranslate"><span class="pre">LinkEditor</span></code></a><ul>
+<li><a class="reference internal" href="#plink.LinkEditor.active_crossing_data"><code class="docutils literal notranslate"><span class="pre">LinkEditor.active_crossing_data()</span></code></a></li>
+<li><a class="reference internal" href="#plink.LinkEditor.attach_cursor"><code class="docutils literal notranslate"><span class="pre">LinkEditor.attach_cursor()</span></code></a></li>
+<li><a class="reference internal" href="#plink.LinkEditor.clear"><code class="docutils literal notranslate"><span class="pre">LinkEditor.clear()</span></code></a></li>
+<li><a class="reference internal" href="#plink.LinkEditor.clicked_on_arrow"><code class="docutils literal notranslate"><span class="pre">LinkEditor.clicked_on_arrow()</span></code></a></li>
+<li><a class="reference internal" href="#plink.LinkEditor.crossed_arrows"><code class="docutils literal notranslate"><span class="pre">LinkEditor.crossed_arrows()</span></code></a></li>
+<li><a class="reference internal" href="#plink.LinkEditor.cursor_on_arrow"><code class="docutils literal notranslate"><span class="pre">LinkEditor.cursor_on_arrow()</span></code></a></li>
+<li><a class="reference internal" href="#plink.LinkEditor.destroy_arrow"><code class="docutils literal notranslate"><span class="pre">LinkEditor.destroy_arrow()</span></code></a></li>
+<li><a class="reference internal" href="#plink.LinkEditor.detach_cursor"><code class="docutils literal notranslate"><span class="pre">LinkEditor.detach_cursor()</span></code></a></li>
+<li><a class="reference internal" href="#plink.LinkEditor.done"><code class="docutils literal notranslate"><span class="pre">LinkEditor.done()</span></code></a></li>
+<li><a class="reference internal" href="#plink.LinkEditor.double_click"><code class="docutils literal notranslate"><span class="pre">LinkEditor.double_click()</span></code></a></li>
+<li><a class="reference internal" href="#plink.LinkEditor.end_dragging_state"><code class="docutils literal notranslate"><span class="pre">LinkEditor.end_dragging_state()</span></code></a></li>
+<li><a class="reference internal" href="#plink.LinkEditor.focus_in"><code class="docutils literal notranslate"><span class="pre">LinkEditor.focus_in()</span></code></a></li>
+<li><a class="reference internal" href="#plink.LinkEditor.focus_out"><code class="docutils literal notranslate"><span class="pre">LinkEditor.focus_out()</span></code></a></li>
+<li><a class="reference internal" href="#plink.LinkEditor.generic_arrow"><code class="docutils literal notranslate"><span class="pre">LinkEditor.generic_arrow()</span></code></a></li>
+<li><a class="reference internal" href="#plink.LinkEditor.generic_vertex"><code class="docutils literal notranslate"><span class="pre">LinkEditor.generic_vertex()</span></code></a></li>
+<li><a class="reference internal" href="#plink.LinkEditor.goto_drawing_state"><code class="docutils literal notranslate"><span class="pre">LinkEditor.goto_drawing_state()</span></code></a></li>
+<li><a class="reference internal" href="#plink.LinkEditor.goto_start_state"><code class="docutils literal notranslate"><span class="pre">LinkEditor.goto_start_state()</span></code></a></li>
+<li><a class="reference internal" href="#plink.LinkEditor.make_alternating"><code class="docutils literal notranslate"><span class="pre">LinkEditor.make_alternating()</span></code></a></li>
+<li><a class="reference internal" href="#plink.LinkEditor.mouse_moved"><code class="docutils literal notranslate"><span class="pre">LinkEditor.mouse_moved()</span></code></a></li>
+<li><a class="reference internal" href="#plink.LinkEditor.move_active"><code class="docutils literal notranslate"><span class="pre">LinkEditor.move_active()</span></code></a></li>
+<li><a class="reference internal" href="#plink.LinkEditor.move_is_ok"><code class="docutils literal notranslate"><span class="pre">LinkEditor.move_is_ok()</span></code></a></li>
+<li><a class="reference internal" href="#plink.LinkEditor.notice_focus"><code class="docutils literal notranslate"><span class="pre">LinkEditor.notice_focus()</span></code></a></li>
+<li><a class="reference internal" href="#plink.LinkEditor.reflect"><code class="docutils literal notranslate"><span class="pre">LinkEditor.reflect()</span></code></a></li>
+<li><a class="reference internal" href="#plink.LinkEditor.set_start_cursor"><code class="docutils literal notranslate"><span class="pre">LinkEditor.set_start_cursor()</span></code></a></li>
+<li><a class="reference internal" href="#plink.LinkEditor.shift_click"><code class="docutils literal notranslate"><span class="pre">LinkEditor.shift_click()</span></code></a></li>
+<li><a class="reference internal" href="#plink.LinkEditor.single_click"><code class="docutils literal notranslate"><span class="pre">LinkEditor.single_click()</span></code></a></li>
+<li><a class="reference internal" href="#plink.LinkEditor.update_crossings"><code class="docutils literal notranslate"><span class="pre">LinkEditor.update_crossings()</span></code></a></li>
+<li><a class="reference internal" href="#plink.LinkEditor.verify_drag"><code class="docutils literal notranslate"><span class="pre">LinkEditor.verify_drag()</span></code></a></li>
+</ul>
+</li>
+<li><a class="reference internal" href="#plink.arrow.Arrow"><code class="docutils literal notranslate"><span class="pre">Arrow</span></code></a><ul>
+<li><a class="reference internal" href="#plink.arrow.Arrow.draw"><code class="docutils literal notranslate"><span class="pre">Arrow.draw()</span></code></a></li>
+<li><a class="reference internal" href="#plink.arrow.Arrow.epsilon"><code class="docutils literal notranslate"><span class="pre">Arrow.epsilon</span></code></a></li>
+<li><a class="reference internal" href="#plink.arrow.Arrow.erase"><code class="docutils literal notranslate"><span class="pre">Arrow.erase()</span></code></a></li>
+<li><a class="reference internal" href="#plink.arrow.Arrow.expose"><code class="docutils literal notranslate"><span class="pre">Arrow.expose()</span></code></a></li>
+<li><a class="reference internal" href="#plink.arrow.Arrow.find_segments"><code class="docutils literal notranslate"><span class="pre">Arrow.find_segments()</span></code></a></li>
+<li><a class="reference internal" href="#plink.arrow.Arrow.freeze"><code class="docutils literal notranslate"><span class="pre">Arrow.freeze()</span></code></a></li>
+<li><a class="reference internal" href="#plink.arrow.Arrow.frozen"><code class="docutils literal notranslate"><span class="pre">Arrow.frozen</span></code></a></li>
+<li><a class="reference internal" href="#plink.arrow.Arrow.hidden"><code class="docutils literal notranslate"><span class="pre">Arrow.hidden</span></code></a></li>
+<li><a class="reference internal" href="#plink.arrow.Arrow.hide"><code class="docutils literal notranslate"><span class="pre">Arrow.hide()</span></code></a></li>
+<li><a class="reference internal" href="#plink.arrow.Arrow.make_faint"><code class="docutils literal notranslate"><span class="pre">Arrow.make_faint()</span></code></a></li>
+<li><a class="reference internal" href="#plink.arrow.Arrow.reverse"><code class="docutils literal notranslate"><span class="pre">Arrow.reverse()</span></code></a></li>
+<li><a class="reference internal" href="#plink.arrow.Arrow.set_color"><code class="docutils literal notranslate"><span class="pre">Arrow.set_color()</span></code></a></li>
+<li><a class="reference internal" href="#plink.arrow.Arrow.set_end"><code class="docutils literal notranslate"><span class="pre">Arrow.set_end()</span></code></a></li>
+<li><a class="reference internal" href="#plink.arrow.Arrow.set_start"><code class="docutils literal notranslate"><span class="pre">Arrow.set_start()</span></code></a></li>
+<li><a class="reference internal" href="#plink.arrow.Arrow.too_close"><code class="docutils literal notranslate"><span class="pre">Arrow.too_close()</span></code></a></li>
+<li><a class="reference internal" href="#plink.arrow.Arrow.vectorize"><code class="docutils literal notranslate"><span class="pre">Arrow.vectorize()</span></code></a></li>
+</ul>
+</li>
+<li><a class="reference internal" href="#plink.crossings.Crossing"><code class="docutils literal notranslate"><span class="pre">Crossing</span></code></a><ul>
+<li><a class="reference internal" href="#plink.crossings.Crossing.DT_hit"><code class="docutils literal notranslate"><span class="pre">Crossing.DT_hit()</span></code></a></li>
+<li><a class="reference internal" href="#plink.crossings.Crossing.clear_marks"><code class="docutils literal notranslate"><span class="pre">Crossing.clear_marks()</span></code></a></li>
+<li><a class="reference internal" href="#plink.crossings.Crossing.height"><code class="docutils literal notranslate"><span class="pre">Crossing.height()</span></code></a></li>
+<li><a class="reference internal" href="#plink.crossings.Crossing.locate"><code class="docutils literal notranslate"><span class="pre">Crossing.locate()</span></code></a></li>
+<li><a class="reference internal" href="#plink.crossings.Crossing.mark_component"><code class="docutils literal notranslate"><span class="pre">Crossing.mark_component()</span></code></a></li>
+<li><a class="reference internal" href="#plink.crossings.Crossing.reverse"><code class="docutils literal notranslate"><span class="pre">Crossing.reverse()</span></code></a></li>
+<li><a class="reference internal" href="#plink.crossings.Crossing.sign"><code class="docutils literal notranslate"><span class="pre">Crossing.sign()</span></code></a></li>
+<li><a class="reference internal" href="#plink.crossings.Crossing.strand"><code class="docutils literal notranslate"><span class="pre">Crossing.strand()</span></code></a></li>
+</ul>
+</li>
+<li><a class="reference internal" href="#plink.crossings.ECrossing"><code class="docutils literal notranslate"><span class="pre">ECrossing</span></code></a><ul>
+<li><a class="reference internal" href="#plink.crossings.ECrossing.goes_over"><code class="docutils literal notranslate"><span class="pre">ECrossing.goes_over()</span></code></a></li>
+<li><a class="reference internal" href="#plink.crossings.ECrossing.pair"><code class="docutils literal notranslate"><span class="pre">ECrossing.pair()</span></code></a></li>
+</ul>
+</li>
+</ul>
+</li>
+</ul>
+
+  </div>
+  <div>
+    <h4>Previous topic</h4>
+    <p class="topless"><a href="installing.html"
+                          title="previous chapter">Installing and running PLink</a></p>
+  </div>
   <div role="note" aria-label="source link">
     <h3>This Page</h3>
     <ul class="this-page-menu">
       <li><a href="_sources/plink.rst.txt"
             rel="nofollow">Show Source</a></li>
     </ul>
    </div>
@@ -393,15 +470,15 @@
     <div class="searchformwrapper">
     <form class="search" action="search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
 </div>
-<script>$('#searchbox').show(0);</script>
+<script>document.getElementById('searchbox').style.display = "block"</script>
         </div>
       </div>
       <div class="clearer"></div>
     </div>
     <div class="related" role="navigation" aria-label="related navigation">
       <h3>Navigation</h3>
       <ul>
@@ -410,17 +487,17 @@
              >index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
           <a href="installing.html" title="Installing and running PLink"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">PLink 2.4.1 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">PLink 2.4.2 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">plink – A Python/Tk link editor</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2009-present, Marc Culler, Nathan Dunfield and others.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 4.2.0.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.1.3.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -4,15 +4,15 @@
 
 
 
 **** Navigation ****
     * index
     * modules |
     * previous |
-    * PLink_2.4.1_documentation »
+    * PLink_2.4.2_documentation »
     * plink â A Python/Tk link editor
 ****** plink â A Python/Tk link editorÂ¶ ******
 Technical documentation of the Python objects that underly PLink. Of interest
 only to Marc, Nathan, or similar folks.
   classplink.LinkEditor(*args, **kwargs)Â¶
       A complete graphical link drawing tool based on the one embedded in Jeff
       Weeksâ original SnapPea program.
@@ -102,21 +102,81 @@
         sign()Â¶
         strand(arrow)Â¶
   classplink.crossings.ECrossing(crossing, arrow)Â¶
       A pair: (Crossing, Arrow), where the Arrow is involved in the Crossing.
       The ECrossings correspond 1-1 with edges of the link diagram.
         goes_over()Â¶
         pair()Â¶
+**** Table_of_Contents ****
+    * plink_â_A_Python/Tk_link_editor
+          o LinkEditor
+                # LinkEditor.active_crossing_data()
+                # LinkEditor.attach_cursor()
+                # LinkEditor.clear()
+                # LinkEditor.clicked_on_arrow()
+                # LinkEditor.crossed_arrows()
+                # LinkEditor.cursor_on_arrow()
+                # LinkEditor.destroy_arrow()
+                # LinkEditor.detach_cursor()
+                # LinkEditor.done()
+                # LinkEditor.double_click()
+                # LinkEditor.end_dragging_state()
+                # LinkEditor.focus_in()
+                # LinkEditor.focus_out()
+                # LinkEditor.generic_arrow()
+                # LinkEditor.generic_vertex()
+                # LinkEditor.goto_drawing_state()
+                # LinkEditor.goto_start_state()
+                # LinkEditor.make_alternating()
+                # LinkEditor.mouse_moved()
+                # LinkEditor.move_active()
+                # LinkEditor.move_is_ok()
+                # LinkEditor.notice_focus()
+                # LinkEditor.reflect()
+                # LinkEditor.set_start_cursor()
+                # LinkEditor.shift_click()
+                # LinkEditor.single_click()
+                # LinkEditor.update_crossings()
+                # LinkEditor.verify_drag()
+          o Arrow
+                # Arrow.draw()
+                # Arrow.epsilon
+                # Arrow.erase()
+                # Arrow.expose()
+                # Arrow.find_segments()
+                # Arrow.freeze()
+                # Arrow.frozen
+                # Arrow.hidden
+                # Arrow.hide()
+                # Arrow.make_faint()
+                # Arrow.reverse()
+                # Arrow.set_color()
+                # Arrow.set_end()
+                # Arrow.set_start()
+                # Arrow.too_close()
+                # Arrow.vectorize()
+          o Crossing
+                # Crossing.DT_hit()
+                # Crossing.clear_marks()
+                # Crossing.height()
+                # Crossing.locate()
+                # Crossing.mark_component()
+                # Crossing.reverse()
+                # Crossing.sign()
+                # Crossing.strand()
+          o ECrossing
+                # ECrossing.goes_over()
+                # ECrossing.pair()
 *** Previous topic ***
 Installing_and_running_PLink
 **** This Page ****
     * Show_Source
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
     * previous |
-    * PLink_2.4.1_documentation »
+    * PLink_2.4.2_documentation »
     * plink â A Python/Tk link editor
 © Copyright 2009-present, Marc Culler, Nathan Dunfield and others. Created
-using Sphinx 4.2.0.
+using Sphinx 6.1.3.
```

### Comparing `plink-2.4.1/plink_src/doc/py-modindex.html` & `plink-2.4.2/plink_src/doc/py-modindex.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 
 <!DOCTYPE html>
 
-<html>
+<html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Python Module Index &#8212; PLink 2.4.1 documentation</title>
+    <title>Python Module Index &#8212; PLink 2.4.2 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/classic.css" />
     
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
-    <script src="_static/jquery.js"></script>
-    <script src="_static/underscore.js"></script>
     <script src="_static/doctools.js"></script>
+    <script src="_static/sphinx_highlight.js"></script>
     
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
  
 
 
   </head><body>
@@ -25,15 +24,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="#" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">PLink 2.4.1 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">PLink 2.4.2 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Python Module Index</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -80,31 +79,31 @@
     <div class="searchformwrapper">
     <form class="search" action="search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
 </div>
-<script>$('#searchbox').show(0);</script>
+<script>document.getElementById('searchbox').style.display = "block"</script>
         </div>
       </div>
       <div class="clearer"></div>
     </div>
     <div class="related" role="navigation" aria-label="related navigation">
       <h3>Navigation</h3>
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="#" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">PLink 2.4.1 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">PLink 2.4.2 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Python Module Index</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2009-present, Marc Culler, Nathan Dunfield and others.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 4.2.0.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.1.3.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -2,25 +2,25 @@
 
 
 
 
 **** Navigation ****
     * index
     * modules |
-    * PLink_2.4.1_documentation »
+    * PLink_2.4.2_documentation »
     * Python Module Index
 ****** Python Module Index ******
 p
      
     p
 [-] plink
         plink.arrow
         plink.crossings
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
-    * PLink_2.4.1_documentation »
+    * PLink_2.4.2_documentation »
     * Python Module Index
 © Copyright 2009-present, Marc Culler, Nathan Dunfield and others. Created
-using Sphinx 4.2.0.
+using Sphinx 6.1.3.
```

### Comparing `plink-2.4.1/plink_src/doc/search.html` & `plink-2.4.2/plink_src/doc/search.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 
 <!DOCTYPE html>
 
-<html>
+<html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Search &#8212; PLink 2.4.1 documentation</title>
+    <title>Search &#8212; PLink 2.4.2 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/classic.css" />
     
     
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
-    <script src="_static/jquery.js"></script>
-    <script src="_static/underscore.js"></script>
     <script src="_static/doctools.js"></script>
+    <script src="_static/sphinx_highlight.js"></script>
     
     <script src="_static/searchtools.js"></script>
     <script src="_static/language_data.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="#" />
   <script src="searchindex.js" defer></script>
    
@@ -28,15 +27,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">PLink 2.4.1 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">PLink 2.4.2 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Search</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -88,17 +87,17 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">PLink 2.4.1 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">PLink 2.4.2 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Search</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2009-present, Marc Culler, Nathan Dunfield and others.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 4.2.0.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.1.3.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -2,20 +2,20 @@
 
 
 
 
 **** Navigation ****
     * index
     * modules |
-    * PLink_2.4.1_documentation »
+    * PLink_2.4.2_documentation »
     * Search
 ****** Search ******
 Please activate JavaScript to enable the search functionality.
 Searching for multiple words only shows matches that contain all words.
 [q                   ] [search]
 **** Navigation ****
     * index
     * modules |
-    * PLink_2.4.1_documentation »
+    * PLink_2.4.2_documentation »
     * Search
 © Copyright 2009-present, Marc Culler, Nathan Dunfield and others. Created
-using Sphinx 4.2.0.
+using Sphinx 6.1.3.
```

### Comparing `plink-2.4.1/plink_src/editor.py` & `plink-2.4.2/plink_src/editor.py`

 * *Files identical despite different names*

### Comparing `plink-2.4.1/plink_src/gui.py` & `plink-2.4.2/plink_src/gui.py`

 * *Files identical despite different names*

### Comparing `plink-2.4.1/plink_src/ipython_tools.py` & `plink-2.4.2/plink_src/ipython_tools.py`

 * *Files identical despite different names*

### Comparing `plink-2.4.1/plink_src/manager.py` & `plink-2.4.2/plink_src/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,14 +211,21 @@
             crosses=[]
             for arrow in component:
                 arrow_crosses = [(c.height(arrow), c, arrow)
                                 for c in self.Crossings if arrow in c]
                 arrow_crosses.sort()
                 crosses += arrow_crosses
             result.append([ECrossing(c[1],c[2]) for c in crosses])
+
+        for crossing in self.Crossings:
+            crossing.clear_marks()
+        # Mark which components each crossing belongs to.
+        for component in result:
+            for ecrossing in component:
+                ecrossing.crossing.mark_component(component)
         return result
 
 
     def sorted_components(self):
         """
         Returns a list of crossing components which have been sorted
         and cyclically permuted, following the scheme used in "standard"
```

### Comparing `plink-2.4.1/plink_src/smooth.py` & `plink-2.4.2/plink_src/smooth.py`

 * *Files identical despite different names*

### Comparing `plink-2.4.1/plink_src/version.py` & `plink-2.4.2/plink_src/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 #
 #   The development of this program was partially supported by
 #   the National Science Foundation under grants DMS0608567,
 #   DMS0504975 and DMS0204142.
 
 """The version number for this PLink program."""
 
-version = "2.4.1"
+version = "2.4.2"
```

### Comparing `plink-2.4.1/plink_src/vertex.py` & `plink-2.4.2/plink_src/vertex.py`

 * *Files identical despite different names*

### Comparing `plink-2.4.1/plink_src/viewer.py` & `plink-2.4.2/plink_src/viewer.py`

 * *Files identical despite different names*

