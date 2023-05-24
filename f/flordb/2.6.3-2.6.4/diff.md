# Comparing `tmp/flordb-2.6.3.tar.gz` & `tmp/flordb-2.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flordb-2.6.3.tar", last modified: Wed May 17 00:26:37 2023, max compression
+gzip compressed data, was "flordb-2.6.4.tar", last modified: Wed May 24 17:16:24 2023, max compression
```

## Comparing `flordb-2.6.3.tar` & `flordb-2.6.4.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-17 00:26:37.323162 flordb-2.6.3/
--rw-r--r--   0 rogarcia   (501) staff       (20)    11357 2023-03-12 17:55:35.000000 flordb-2.6.3/LICENSE
--rw-r--r--   0 rogarcia   (501) staff       (20)     8099 2023-05-17 00:26:37.323044 flordb-2.6.3/PKG-INFO
--rw-r--r--   0 rogarcia   (501) staff       (20)     7667 2023-03-12 20:12:23.000000 flordb-2.6.3/README.md
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-17 00:26:37.314523 flordb-2.6.3/flor/
--rw-r--r--   0 rogarcia   (501) staff       (20)      269 2023-05-17 00:21:40.000000 flordb-2.6.3/flor/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     1779 2023-05-17 00:21:40.000000 flordb-2.6.3/flor/__main__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      922 2023-05-17 00:21:40.000000 flordb-2.6.3/flor/batch.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      544 2023-03-12 17:55:35.000000 flordb-2.6.3/flor/constants.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     4416 2023-05-17 00:21:40.000000 flordb-2.6.3/flor/database.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     6283 2023-05-17 00:21:40.000000 flordb-2.6.3/flor/flags.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-17 00:26:37.315228 flordb-2.6.3/flor/hlast/
--rw-r--r--   0 rogarcia   (501) staff       (20)     4159 2023-03-23 13:19:05.000000 flordb-2.6.3/flor/hlast/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     8884 2023-03-12 17:55:35.000000 flordb-2.6.3/flor/hlast/gtpropagate.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-17 00:26:37.316408 flordb-2.6.3/flor/hlast/gumtree/
--rw-r--r--   0 rogarcia   (501) staff       (20)     6322 2023-03-12 17:55:35.000000 flordb-2.6.3/flor/hlast/gumtree/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2916 2023-03-12 17:55:35.000000 flordb-2.6.3/flor/hlast/gumtree/adapter.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      876 2023-03-12 17:55:35.000000 flordb-2.6.3/flor/hlast/gumtree/idmap.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     1085 2023-03-12 17:55:35.000000 flordb-2.6.3/flor/hlast/gumtree/priorityq.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2110 2023-03-12 17:55:35.000000 flordb-2.6.3/flor/hlast/gumtree/python.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     8350 2023-03-12 17:55:35.000000 flordb-2.6.3/flor/hlast/gumtree/test.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      903 2023-03-12 17:55:35.000000 flordb-2.6.3/flor/hlast/gumtree/tree.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2273 2023-03-23 13:19:05.000000 flordb-2.6.3/flor/hlast/visitors.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2634 2023-03-22 14:08:08.000000 flordb-2.6.3/flor/iterator.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-17 00:26:37.316544 flordb-2.6.3/flor/journal/
--rw-r--r--   0 rogarcia   (501) staff       (20)     2946 2023-03-22 14:08:08.000000 flordb-2.6.3/flor/journal/__init__.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-17 00:26:37.317005 flordb-2.6.3/flor/journal/entry/
--rw-r--r--   0 rogarcia   (501) staff       (20)      876 2023-03-12 17:55:35.000000 flordb-2.6.3/flor/journal/entry/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      710 2023-03-12 17:55:35.000000 flordb-2.6.3/flor/journal/entry/abstract.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      284 2023-03-12 17:55:35.000000 flordb-2.6.3/flor/journal/entry/constants.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-17 00:26:37.318059 flordb-2.6.3/flor/journal/entry/data/
--rw-r--r--   0 rogarcia   (501) staff       (20)      427 2023-03-12 17:55:35.000000 flordb-2.6.3/flor/journal/entry/data/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      588 2023-03-12 17:55:35.000000 flordb-2.6.3/flor/journal/entry/data/abstract.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2073 2023-03-23 13:19:05.000000 flordb-2.6.3/flor/journal/entry/data/dataframe.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2093 2023-03-12 17:55:35.000000 flordb-2.6.3/flor/journal/entry/data/reference.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     1904 2023-03-12 17:55:35.000000 flordb-2.6.3/flor/journal/entry/data/torch_chkpt.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      711 2023-03-12 17:55:35.000000 flordb-2.6.3/flor/journal/entry/data/value.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-17 00:26:37.318828 flordb-2.6.3/flor/journal/entry/metadata/
--rw-r--r--   0 rogarcia   (501) staff       (20)      149 2023-03-12 17:55:35.000000 flordb-2.6.3/flor/journal/entry/metadata/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      461 2023-03-12 17:55:35.000000 flordb-2.6.3/flor/journal/entry/metadata/abstract.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      741 2023-03-12 17:55:35.000000 flordb-2.6.3/flor/journal/entry/metadata/bracket.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     1032 2023-03-12 17:55:35.000000 flordb-2.6.3/flor/journal/entry/metadata/eof.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-17 00:26:37.319429 flordb-2.6.3/flor/journal/tree/
--rw-r--r--   0 rogarcia   (501) staff       (20)       23 2023-03-12 17:55:35.000000 flordb-2.6.3/flor/journal/tree/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     1285 2023-03-12 17:55:35.000000 flordb-2.6.3/flor/journal/tree/block.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      929 2023-03-12 17:55:35.000000 flordb-2.6.3/flor/journal/tree/group.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     3472 2023-03-12 17:55:35.000000 flordb-2.6.3/flor/journal/tree/tree.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     4231 2023-03-22 14:08:08.000000 flordb-2.6.3/flor/journal/tree/window.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     1998 2023-04-14 18:08:18.000000 flordb-2.6.3/flor/kits.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-17 00:26:37.320338 flordb-2.6.3/flor/logger/
--rw-r--r--   0 rogarcia   (501) staff       (20)     2219 2023-05-10 13:18:25.000000 flordb-2.6.3/flor/logger/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2179 2023-03-12 17:55:35.000000 flordb-2.6.3/flor/logger/checkpoint_logger.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     1592 2023-05-04 17:16:10.000000 flordb-2.6.3/flor/logger/exp_json.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      536 2023-03-12 17:55:35.000000 flordb-2.6.3/flor/logger/future.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2013 2023-03-16 16:35:51.000000 flordb-2.6.3/flor/logger/log_records.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-17 00:26:37.321045 flordb-2.6.3/flor/query/
--rw-r--r--   0 rogarcia   (501) staff       (20)     7946 2023-05-17 00:21:40.000000 flordb-2.6.3/flor/query/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     3716 2023-05-17 00:21:40.000000 flordb-2.6.3/flor/query/database.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     1862 2023-03-12 17:55:35.000000 flordb-2.6.3/flor/query/engine.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2503 2023-03-12 17:55:35.000000 flordb-2.6.3/flor/query/pivot.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     9180 2023-05-17 00:21:40.000000 flordb-2.6.3/flor/query/unpack.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-17 00:26:37.321380 flordb-2.6.3/flor/shelf/
--rw-r--r--   0 rogarcia   (501) staff       (20)        0 2023-03-12 17:55:35.000000 flordb-2.6.3/flor/shelf/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2558 2023-05-17 00:21:40.000000 flordb-2.6.3/flor/shelf/cwd_shelf.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     3176 2023-05-10 13:18:25.000000 flordb-2.6.3/flor/shelf/home_shelf.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-17 00:26:37.322153 flordb-2.6.3/flor/skipblock/
--rw-r--r--   0 rogarcia   (501) staff       (20)       32 2023-03-12 17:55:36.000000 flordb-2.6.3/flor/skipblock/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      689 2023-03-12 17:55:36.000000 flordb-2.6.3/flor/skipblock/abstract.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2623 2023-03-22 14:08:08.000000 flordb-2.6.3/flor/skipblock/readblock.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      349 2023-03-12 17:55:36.000000 flordb-2.6.3/flor/skipblock/seemblock.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     3819 2023-04-14 18:08:18.000000 flordb-2.6.3/flor/skipblock/writeblock.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      600 2023-03-22 14:08:08.000000 flordb-2.6.3/flor/state.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      564 2023-04-04 22:53:53.000000 flordb-2.6.3/flor/utils.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-17 00:26:37.322899 flordb-2.6.3/flordb.egg-info/
--rw-r--r--   0 rogarcia   (501) staff       (20)     8099 2023-05-17 00:26:37.000000 flordb-2.6.3/flordb.egg-info/PKG-INFO
--rw-r--r--   0 rogarcia   (501) staff       (20)     1684 2023-05-17 00:26:37.000000 flordb-2.6.3/flordb.egg-info/SOURCES.txt
--rw-r--r--   0 rogarcia   (501) staff       (20)        1 2023-05-17 00:26:37.000000 flordb-2.6.3/flordb.egg-info/dependency_links.txt
--rw-r--r--   0 rogarcia   (501) staff       (20)       91 2023-05-17 00:26:37.000000 flordb-2.6.3/flordb.egg-info/requires.txt
--rw-r--r--   0 rogarcia   (501) staff       (20)        5 2023-05-17 00:26:37.000000 flordb-2.6.3/flordb.egg-info/top_level.txt
--rw-r--r--   0 rogarcia   (501) staff       (20)       38 2023-05-17 00:26:37.323193 flordb-2.6.3/setup.cfg
--rw-r--r--   0 rogarcia   (501) staff       (20)      904 2023-05-17 00:26:19.000000 flordb-2.6.3/setup.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-24 17:16:24.368499 flordb-2.6.4/
+-rw-r--r--   0 rogarcia   (501) staff       (20)    11357 2023-03-12 17:55:35.000000 flordb-2.6.4/LICENSE
+-rw-r--r--   0 rogarcia   (501) staff       (20)     8299 2023-05-24 17:16:24.368264 flordb-2.6.4/PKG-INFO
+-rw-r--r--   0 rogarcia   (501) staff       (20)     7867 2023-05-24 17:15:50.000000 flordb-2.6.4/README.md
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-24 17:16:24.360337 flordb-2.6.4/flor/
+-rw-r--r--   0 rogarcia   (501) staff       (20)      281 2023-05-24 17:15:50.000000 flordb-2.6.4/flor/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     1779 2023-05-17 00:21:40.000000 flordb-2.6.4/flor/__main__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      922 2023-05-17 00:21:40.000000 flordb-2.6.4/flor/batch.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      544 2023-03-12 17:55:35.000000 flordb-2.6.4/flor/constants.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     4416 2023-05-17 00:21:40.000000 flordb-2.6.4/flor/database.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     6299 2023-05-24 17:15:50.000000 flordb-2.6.4/flor/flags.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-24 17:16:24.360918 flordb-2.6.4/flor/hlast/
+-rw-r--r--   0 rogarcia   (501) staff       (20)     4159 2023-03-23 13:19:05.000000 flordb-2.6.4/flor/hlast/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     8884 2023-03-12 17:55:35.000000 flordb-2.6.4/flor/hlast/gtpropagate.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-24 17:16:24.362059 flordb-2.6.4/flor/hlast/gumtree/
+-rw-r--r--   0 rogarcia   (501) staff       (20)     6322 2023-03-12 17:55:35.000000 flordb-2.6.4/flor/hlast/gumtree/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2916 2023-03-12 17:55:35.000000 flordb-2.6.4/flor/hlast/gumtree/adapter.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      876 2023-03-12 17:55:35.000000 flordb-2.6.4/flor/hlast/gumtree/idmap.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     1085 2023-03-12 17:55:35.000000 flordb-2.6.4/flor/hlast/gumtree/priorityq.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2110 2023-03-12 17:55:35.000000 flordb-2.6.4/flor/hlast/gumtree/python.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     8350 2023-03-12 17:55:35.000000 flordb-2.6.4/flor/hlast/gumtree/test.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      903 2023-03-12 17:55:35.000000 flordb-2.6.4/flor/hlast/gumtree/tree.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2273 2023-03-23 13:19:05.000000 flordb-2.6.4/flor/hlast/visitors.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2634 2023-03-22 14:08:08.000000 flordb-2.6.4/flor/iterator.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-24 17:16:24.362175 flordb-2.6.4/flor/journal/
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2946 2023-03-22 14:08:08.000000 flordb-2.6.4/flor/journal/__init__.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-24 17:16:24.362537 flordb-2.6.4/flor/journal/entry/
+-rw-r--r--   0 rogarcia   (501) staff       (20)      876 2023-03-12 17:55:35.000000 flordb-2.6.4/flor/journal/entry/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      710 2023-03-12 17:55:35.000000 flordb-2.6.4/flor/journal/entry/abstract.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      284 2023-03-12 17:55:35.000000 flordb-2.6.4/flor/journal/entry/constants.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-24 17:16:24.363531 flordb-2.6.4/flor/journal/entry/data/
+-rw-r--r--   0 rogarcia   (501) staff       (20)      427 2023-03-12 17:55:35.000000 flordb-2.6.4/flor/journal/entry/data/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      588 2023-03-12 17:55:35.000000 flordb-2.6.4/flor/journal/entry/data/abstract.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2073 2023-03-23 13:19:05.000000 flordb-2.6.4/flor/journal/entry/data/dataframe.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2093 2023-03-12 17:55:35.000000 flordb-2.6.4/flor/journal/entry/data/reference.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     1904 2023-03-12 17:55:35.000000 flordb-2.6.4/flor/journal/entry/data/torch_chkpt.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      711 2023-03-12 17:55:35.000000 flordb-2.6.4/flor/journal/entry/data/value.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-24 17:16:24.364278 flordb-2.6.4/flor/journal/entry/metadata/
+-rw-r--r--   0 rogarcia   (501) staff       (20)      149 2023-03-12 17:55:35.000000 flordb-2.6.4/flor/journal/entry/metadata/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      461 2023-03-12 17:55:35.000000 flordb-2.6.4/flor/journal/entry/metadata/abstract.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      741 2023-03-12 17:55:35.000000 flordb-2.6.4/flor/journal/entry/metadata/bracket.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     1032 2023-03-12 17:55:35.000000 flordb-2.6.4/flor/journal/entry/metadata/eof.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-24 17:16:24.364895 flordb-2.6.4/flor/journal/tree/
+-rw-r--r--   0 rogarcia   (501) staff       (20)       23 2023-03-12 17:55:35.000000 flordb-2.6.4/flor/journal/tree/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     1285 2023-03-12 17:55:35.000000 flordb-2.6.4/flor/journal/tree/block.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      929 2023-03-12 17:55:35.000000 flordb-2.6.4/flor/journal/tree/group.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     3472 2023-03-12 17:55:35.000000 flordb-2.6.4/flor/journal/tree/tree.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     4231 2023-03-22 14:08:08.000000 flordb-2.6.4/flor/journal/tree/window.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2116 2023-05-24 17:15:50.000000 flordb-2.6.4/flor/kits.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-24 17:16:24.365884 flordb-2.6.4/flor/logger/
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2219 2023-05-10 13:18:25.000000 flordb-2.6.4/flor/logger/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2179 2023-03-12 17:55:35.000000 flordb-2.6.4/flor/logger/checkpoint_logger.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     1592 2023-05-04 17:16:10.000000 flordb-2.6.4/flor/logger/exp_json.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      536 2023-03-12 17:55:35.000000 flordb-2.6.4/flor/logger/future.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2013 2023-03-16 16:35:51.000000 flordb-2.6.4/flor/logger/log_records.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-24 17:16:24.366497 flordb-2.6.4/flor/query/
+-rw-r--r--   0 rogarcia   (501) staff       (20)     8042 2023-05-24 17:15:50.000000 flordb-2.6.4/flor/query/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     3721 2023-05-24 17:15:50.000000 flordb-2.6.4/flor/query/database.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     1752 2023-05-24 17:15:50.000000 flordb-2.6.4/flor/query/engine.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2503 2023-03-12 17:55:35.000000 flordb-2.6.4/flor/query/pivot.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     9458 2023-05-24 17:15:50.000000 flordb-2.6.4/flor/query/unpack.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-24 17:16:24.366775 flordb-2.6.4/flor/shelf/
+-rw-r--r--   0 rogarcia   (501) staff       (20)        0 2023-03-12 17:55:35.000000 flordb-2.6.4/flor/shelf/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2558 2023-05-17 00:21:40.000000 flordb-2.6.4/flor/shelf/cwd_shelf.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     3176 2023-05-10 13:18:25.000000 flordb-2.6.4/flor/shelf/home_shelf.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-24 17:16:24.367548 flordb-2.6.4/flor/skipblock/
+-rw-r--r--   0 rogarcia   (501) staff       (20)       32 2023-03-12 17:55:36.000000 flordb-2.6.4/flor/skipblock/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      689 2023-03-12 17:55:36.000000 flordb-2.6.4/flor/skipblock/abstract.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2623 2023-03-22 14:08:08.000000 flordb-2.6.4/flor/skipblock/readblock.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      349 2023-03-12 17:55:36.000000 flordb-2.6.4/flor/skipblock/seemblock.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     3819 2023-04-14 18:08:18.000000 flordb-2.6.4/flor/skipblock/writeblock.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      600 2023-03-22 14:08:08.000000 flordb-2.6.4/flor/state.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     1078 2023-05-24 17:15:50.000000 flordb-2.6.4/flor/utils.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-24 17:16:24.368132 flordb-2.6.4/flordb.egg-info/
+-rw-r--r--   0 rogarcia   (501) staff       (20)     8299 2023-05-24 17:16:24.000000 flordb-2.6.4/flordb.egg-info/PKG-INFO
+-rw-r--r--   0 rogarcia   (501) staff       (20)     1684 2023-05-24 17:16:24.000000 flordb-2.6.4/flordb.egg-info/SOURCES.txt
+-rw-r--r--   0 rogarcia   (501) staff       (20)        1 2023-05-24 17:16:24.000000 flordb-2.6.4/flordb.egg-info/dependency_links.txt
+-rw-r--r--   0 rogarcia   (501) staff       (20)       91 2023-05-24 17:16:24.000000 flordb-2.6.4/flordb.egg-info/requires.txt
+-rw-r--r--   0 rogarcia   (501) staff       (20)        5 2023-05-24 17:16:24.000000 flordb-2.6.4/flordb.egg-info/top_level.txt
+-rw-r--r--   0 rogarcia   (501) staff       (20)       38 2023-05-24 17:16:24.368554 flordb-2.6.4/setup.cfg
+-rw-r--r--   0 rogarcia   (501) staff       (20)      904 2023-05-24 17:15:50.000000 flordb-2.6.4/setup.py
```

### Comparing `flordb-2.6.3/LICENSE` & `flordb-2.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `flordb-2.6.3/PKG-INFO` & `flordb-2.6.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flordb
-Version: 2.6.3
+Version: 2.6.4
 Summary: Fast Low-Overhead Recovery
 Home-page: https://github.com/ucbrise/flor
 Author: Rolando Garcia
 Author-email: rogarcia@berkeley.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -21,14 +21,21 @@
 
 Flor and FlorDB are software developed at UC Berkeley's [RISE](https://rise.cs.berkeley.edu/) Lab.
 # Installation
 
 ```bash
 pip install flordb
 ```
+# Demo
+
+[![Napa Retreat Demo](https://i.ytimg.com/vi/TNSt5-i7kR4/sddefault.jpg)](https://youtu.be/TNSt5-i7kR4)
+
+<!-- https://i.ytimg.com/vi/TNSt5-i7kR4/sddefault.jpg
+https://youtu.be/TNSt5-i7kR4
+ -->
 
 # First run
 
 Run the ``examples/rnn.py`` script to test your installation. 
 This script will train a small linear model on MNIST.
 FLOR shadow branches permit us to commit your work
 automatically on every run, without interfering with your
```

### Comparing `flordb-2.6.3/README.md` & `flordb-2.6.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,21 @@
 
 Flor and FlorDB are software developed at UC Berkeley's [RISE](https://rise.cs.berkeley.edu/) Lab.
 # Installation
 
 ```bash
 pip install flordb
 ```
+# Demo
+
+[![Napa Retreat Demo](https://i.ytimg.com/vi/TNSt5-i7kR4/sddefault.jpg)](https://youtu.be/TNSt5-i7kR4)
+
+<!-- https://i.ytimg.com/vi/TNSt5-i7kR4/sddefault.jpg
+https://youtu.be/TNSt5-i7kR4
+ -->
 
 # First run
 
 Run the ``examples/rnn.py`` script to test your installation. 
 This script will train a small linear model on MNIST.
 FLOR shadow branches permit us to commit your work
 automatically on every run, without interfering with your
```

### Comparing `flordb-2.6.3/flor/__main__.py` & `flordb-2.6.4/flor/__main__.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.3/flor/batch.py` & `flordb-2.6.4/flor/batch.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.3/flor/constants.py` & `flordb-2.6.4/flor/constants.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.3/flor/database.py` & `flordb-2.6.4/flor/database.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.3/flor/flags.py` & `flordb-2.6.4/flor/flags.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,15 +188,15 @@
 
 
 parser = CLI_Args()
 
 
 def is_interactive():
     try:
-        get_ipython()
+        get_ipython()  # type: ignore
         return True
     except:
         return False
 
 
 def parse():
     State.import_time = time()
```

### Comparing `flordb-2.6.3/flor/hlast/__init__.py` & `flordb-2.6.4/flor/hlast/__init__.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.3/flor/hlast/gtpropagate.py` & `flordb-2.6.4/flor/hlast/gtpropagate.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.3/flor/hlast/gumtree/__init__.py` & `flordb-2.6.4/flor/hlast/gumtree/__init__.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.3/flor/hlast/gumtree/adapter.py` & `flordb-2.6.4/flor/hlast/gumtree/adapter.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.3/flor/hlast/gumtree/idmap.py` & `flordb-2.6.4/flor/hlast/gumtree/idmap.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.3/flor/hlast/gumtree/priorityq.py` & `flordb-2.6.4/flor/hlast/gumtree/priorityq.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.3/flor/hlast/gumtree/python.py` & `flordb-2.6.4/flor/hlast/gumtree/python.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.3/flor/hlast/gumtree/test.py` & `flordb-2.6.4/flor/hlast/gumtree/test.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.3/flor/hlast/gumtree/tree.py` & `flordb-2.6.4/flor/hlast/gumtree/tree.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.3/flor/hlast/visitors.py` & `flordb-2.6.4/flor/hlast/visitors.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.3/flor/iterator.py` & `flordb-2.6.4/flor/iterator.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.3/flor/journal/__init__.py` & `flordb-2.6.4/flor/journal/__init__.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.3/flor/journal/entry/__init__.py` & `flordb-2.6.4/flor/journal/entry/__init__.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.3/flor/journal/entry/abstract.py` & `flordb-2.6.4/flor/journal/entry/abstract.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.3/flor/journal/entry/data/abstract.py` & `flordb-2.6.4/flor/journal/entry/data/abstract.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.3/flor/journal/entry/data/dataframe.py` & `flordb-2.6.4/flor/journal/entry/data/dataframe.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.3/flor/journal/entry/data/reference.py` & `flordb-2.6.4/flor/journal/entry/data/reference.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.3/flor/journal/entry/data/torch_chkpt.py` & `flordb-2.6.4/flor/journal/entry/data/torch_chkpt.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.3/flor/journal/entry/data/value.py` & `flordb-2.6.4/flor/journal/entry/data/value.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.3/flor/journal/entry/metadata/bracket.py` & `flordb-2.6.4/flor/journal/entry/metadata/bracket.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.3/flor/journal/entry/metadata/eof.py` & `flordb-2.6.4/flor/journal/entry/metadata/eof.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.3/flor/journal/tree/block.py` & `flordb-2.6.4/flor/journal/tree/block.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.3/flor/journal/tree/group.py` & `flordb-2.6.4/flor/journal/tree/group.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.3/flor/journal/tree/tree.py` & `flordb-2.6.4/flor/journal/tree/tree.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.3/flor/journal/tree/window.py` & `flordb-2.6.4/flor/journal/tree/window.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.3/flor/kits.py` & `flordb-2.6.4/flor/kits.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,20 +32,22 @@
             name = str(static_id) if name is None else name
             if State.loop_nesting_level == 1:
                 # Outer loop
                 assert State.import_time is not None
                 State.seconds["PREP"] = time() - State.import_time
                 State.seconds["EPOCHS"] = []
                 State.epoch = 0
+                State.seconds["EVAL"] = time()
                 for each in it(iter8r):
                     start_time = time()
                     State.step = 0
                     State.epoch += 1
                     yield each
                     State.seconds["EPOCHS"].append(time() - start_time)
+                State.seconds["EVAL"] = time() - State.seconds["EVAL"]
             else:
                 assert State.loop_nesting_level > 1
                 # Nested loop
                 if SkipBlock.step_into(name, probed):
                     assert State.step is not None
                     try:
                         while True:
```

### Comparing `flordb-2.6.3/flor/logger/__init__.py` & `flordb-2.6.4/flor/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.3/flor/logger/checkpoint_logger.py` & `flordb-2.6.4/flor/logger/checkpoint_logger.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.3/flor/logger/exp_json.py` & `flordb-2.6.4/flor/logger/exp_json.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.3/flor/logger/future.py` & `flordb-2.6.4/flor/logger/future.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.3/flor/logger/log_records.py` & `flordb-2.6.4/flor/logger/log_records.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.3/flor/query/__init__.py` & `flordb-2.6.4/flor/query/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,15 +46,15 @@
                 "value",
             ],
         )
         .astype(
             {
                 "projid": str,
                 "runid": str,
-                "tstamp": 'datetime64[ns]',
+                "tstamp": "datetime64[ns]",
                 "vid": str,
                 "epoch": int,
                 "step": int,
                 "name": str,
                 "value": object,
             }
         )
@@ -145,48 +145,44 @@
         df.query(where_clause)[list(DATA_PREP)]
         .drop_duplicates()
         .merge(
             pd.DataFrame(database.get_schedule(DATA_PREP)).astype(
                 {
                     "projid": str,
                     "runid": str,
-                    "tstamp": 'datetime64[ns]',
+                    "tstamp": "datetime64[ns]",
                     "vid": str,
-                    "seconds": float,
+                    "prep_secs": float,
+                    "eval_secs": float,
                 }
             ),
             how="inner",
             on=DATA_PREP,
-        )[
-            list(DATA_PREP)
-            + [
-                "seconds",
-            ]
-        ]
+        )[list(DATA_PREP) + ["prep_secs", "eval_secs"]]
     )
     if loglvl == DATA_PREP:
         versions = dp_schedule["vid"].drop_duplicates()
         display(dp_schedule)
         print(
-            f"Continue replaying {len(versions)} versions at DATA_PREP level for {'{:.2f}'.format(3 * len(versions) + sum(dp_schedule['seconds']))} seconds?"
+            f"Continue replaying {len(versions)} versions at DATA_PREP level for {'{:.2f}'.format(3 * len(versions) + sum(dp_schedule['prep_secs']) + sum(dp_schedule['eval_secs']))} seconds?"
         )
         res = input("Continue [Y/n]? ")
         if res.strip().lower() != "n":
             batch_replay(apply_vars, path, versions, DATA_PREP)
     elif loglvl == OUTR_LOOP:
         size_bytes = home_shelf.get_checkpoint_bytes_per_epoch(cwd_shelf.get_projid())
         schedule = (
             df.query(where_clause)[list(OUTR_LOOP)]
             .drop_duplicates()
             .merge(
                 pd.DataFrame(database.get_schedule(OUTR_LOOP)).astype(
                     {
                         "projid": str,
                         "runid": str,
-                        "tstamp": 'datetime64[ns]',
+                        "tstamp": "datetime64[ns]",
                         "vid": str,
                         "epoch": int,
                         "seconds": float,
                     }
                 ),
                 how="inner",
                 on=OUTR_LOOP,
@@ -197,29 +193,29 @@
                 ]
             ]
         )
         schedule["seconds"] = size_bytes * DESERIALIZATION_COEFF
         versions = schedule["vid"].drop_duplicates()
         display(schedule)
         print(
-            f"Continue replaying {len(versions)} versions at OUTR_LOOP level for {'{:.2f}'.format((3 * len(versions) + sum(dp_schedule['seconds'])) + sum(schedule['seconds']))} seconds?"
+            f"Continue replaying {len(versions)} versions at OUTR_LOOP level for {'{:.2f}'.format((3 * len(versions) + sum(dp_schedule['prep_secs']) + sum(dp_schedule['eval_secs'])) + sum(schedule['seconds']))} seconds?"
         )
         res = input("Continue [Y/n]? ")
         if res.strip().lower() != "n":
             batch_replay(apply_vars, path, versions, OUTR_LOOP)
     elif loglvl == INNR_LOOP:
         schedule = (
             df.query(where_clause)[list(OUTR_LOOP)]
             .drop_duplicates()
             .merge(
                 pd.DataFrame(database.get_schedule(OUTR_LOOP)).astype(
                     {
                         "projid": str,
                         "runid": str,
-                        "tstamp": 'datetime64[ns]',
+                        "tstamp": "datetime64[ns]",
                         "vid": str,
                         "epoch": int,
                         "seconds": float,
                     }
                 ),
                 how="inner",
                 on=OUTR_LOOP,
@@ -229,15 +225,15 @@
                     "seconds",
                 ]
             ]
         )
         versions = schedule["vid"].drop_duplicates()
         display(schedule)
         print(
-            f"Continue replaying {len(versions)} versions at INNR_LOOP level for {'{:.2f}'.format(sum(3 * len(versions) + dp_schedule['seconds']) + sum(schedule['seconds']))} seconds?"
+            f"Continue replaying {len(versions)} versions at INNR_LOOP level for {'{:.2f}'.format((3 * len(versions) + sum(dp_schedule['prep_secs']) + sum(dp_schedule['eval_secs'])) + sum(schedule['seconds']))} seconds?"
         )
         res = input("Continue [Y/n]? ")
         if res.strip().lower() != "n":
             batch_replay(apply_vars, path, versions, INNR_LOOP)
     else:
         raise
```

### Comparing `flordb-2.6.3/flor/query/database.py` & `flordb-2.6.4/flor/query/database.py`

 * *Files 10% similar despite different names*

```diff
@@ -47,15 +47,16 @@
             value text
             );
         CREATE TABLE data_prep(
             projid text,
             runid text,
             tstamp text,
             vid text,
-            seconds real
+            prep_secs real,
+            eval_secs real
         );
         CREATE TABLE outr_loop(
             projid text,
             runid text,
             tstamp text,
             vid text,
             epoch integer,
@@ -74,29 +75,27 @@
     if not res:
         return None
     cur.close()
     return [str(row[0]) for row in res]
 
 
 def get_schedule(keys):
+    # TODO: repair and test
     assert State.db_conn is not None
     cur = State.db_conn.cursor()
     if keys == DATA_PREP:
         res = []
         for r in cur.execute(
-            "SELECT " + ", ".join(DATA_PREP) + ", seconds FROM data_prep;"
+            "SELECT " + ", ".join(DATA_PREP) + ", prep_secs, eval_secs FROM data_prep;"
         ).fetchall():
             res.append(
                 {
                     c: v
                     for c, v in zip(
-                        list(DATA_PREP)
-                        + [
-                            "seconds",
-                        ],
+                        list(DATA_PREP) + ["prep_secs", "eval_secs"],
                         r,
                     )
                 }
             )
     elif keys == OUTR_LOOP:
         res = []
         for r in cur.execute(
@@ -147,9 +146,9 @@
                 d["name"],
                 d["value"],
             )
             for d in list_of_dicts
         ],
     )
     State.db_conn.commit()
-    print("Flor wrote log records to SqliteDB")
+    print("Flor wrote log records to sqlite")
     cur.close()
```

### Comparing `flordb-2.6.3/flor/query/engine.py` & `flordb-2.6.4/flor/query/engine.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,18 +19,16 @@
         return INNR_LOOP
     if any([applied_v in pivot_vars["OUTR_LOOP"] for applied_v in apply_vars]):
         return OUTR_LOOP
     return DATA_PREP
 
 
 def batch_replay(apply_vars: List[str], path: str, versions: pd.Series, loglvl):
-    # TODO: argv processing
     base_cmd = ["python", path, "--replay_flor"]
 
-    start_time = time()
     assert State.repo is not None
     for hexsha in versions:
         State.repo.git.checkout(hexsha)
         apply(diff_vars(apply_vars, path), path)
 
         if loglvl == DATA_PREP:
             subprocess.run(
@@ -53,15 +51,14 @@
                 + [
                     "2/2",
                 ]
             )
         else:
             raise
         State.repo.git.stash()
-    print(f"Time elapsed: {time() - start_time} seconds")
 
 
 def diff_vars(apply_vars: List[str], path: str):
     with open(path, "r") as f:
         tree = ast.parse(f.read())
     visitor = LoggedExpVisitor()
     visitor.visit(tree)
```

### Comparing `flordb-2.6.3/flor/query/pivot.py` & `flordb-2.6.4/flor/query/pivot.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.3/flor/query/unpack.py` & `flordb-2.6.4/flor/query/unpack.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,30 +30,34 @@
     assert r is not None
 
     all_versions = [version for version in r.iter_commits()]
     flor_versions = [
         version for version in all_versions if "::" in str(version.message)
     ]
     record_versions = [
-        version for version in flor_versions if "RECORD::" in str(version.message)
+        version
+        for version in flor_versions
+        if str(version.message).count("RECORD::") == 1
     ]
 
     return {"ALL": all_versions, "FLOR": flor_versions, "RECORD": record_versions}
 
 
 def resolve_cache(cache_short_path):
     assert cwd_shelf.in_shadow_branch()
     return Path.home() / ".flor" / cwd_shelf.get_projid() / cache_short_path
 
 
 def unpack():
     """
     MAIN FUNCTION
     """
-    assert cwd_shelf.in_shadow_branch()
+    assert (
+        cwd_shelf.in_shadow_branch()
+    ), "Please unpack log records from within a `flor.shadow` branch"
     clear_stash()
 
     r = State.repo
     assert r is not None
     if State.db_conn is None:
         database.start_db(cwd_shelf.get_projid())
     wmrk = database.get_watermark()
@@ -65,58 +69,56 @@
                 break
             try:
                 print(f"STEPPING IN {version.hexsha}")
                 r.git.checkout(version)
                 cp_seconds(version)
                 cp_log_records(version)
             except Exception as e:
-                print("Line 72 Exception", e)
+                print("Line Exception", e)
     finally:
         r.git.checkout(active_branch)
 
 
 def cp_seconds(version):
     assert State.db_conn is not None
     hexsha, message = version.hexsha, version.message
-    if "RECORD::" in message and SECONDS_JSON.exists():
+    if message.count("RECORD::") == 1 and SECONDS_JSON.exists():
         with open(REPLAY_JSON, "r") as f:
             replay_json = json.load(f)
         with open(SECONDS_JSON, "r") as f:
             seconds_json = json.load(f)
         assert isinstance(seconds_json, dict) and seconds_json
         assert "PREP" in seconds_json
 
-        def prep_normalize(prep_secs):
-            nonlocal seconds_json, replay_json
+        def prep_normalize(prep_secs, eval_secs):
+            nonlocal replay_json
             data = []
             data.append(
                 {
                     c: v
                     for c, v in zip(
-                        list(DATA_PREP)
-                        + [
-                            "seconds",
-                        ],
+                        list(DATA_PREP) + ["prep_secs", "eval_secs"],
                         [
                             cwd_shelf.get_projid(),
                             replay_json["NAME"],
                             PurePath(replay_json["TSTAMP"]).stem,
                             hexsha,
                             float(prep_secs),
+                            float(eval_secs),
                         ],
                     )
                 }
             )
             return data
 
         def outr_normalize(all_epochs_secs):
-            nonlocal seconds_json, replay_json
+            nonlocal replay_json
             data = []
             for i, epoch_secs in enumerate(all_epochs_secs):
-                epoch = i + 1
+                epoch = i + 1  # TODO: confirm not off-by-one
                 data.append(
                     {
                         c: v
                         for c, v in zip(
                             list(OUTR_LOOP)
                             + [
                                 "seconds",
@@ -131,17 +133,20 @@
                             ],
                         )
                     }
                 )
             return data
 
         # ..send PREP to data_prep
-        pd.DataFrame(prep_normalize(seconds_json["PREP"])).to_sql(
-            "data_prep", con=State.db_conn, if_exists="append", index=False
-        )
+        pd.DataFrame(
+            prep_normalize(
+                seconds_json["PREP"],
+                seconds_json["EVAL"] if "EVAL" in seconds_json else -1.0,
+            )
+        ).to_sql("data_prep", con=State.db_conn, if_exists="append", index=False)
 
         # .. send EPOCHS to outr_loop
         if "EPOCHS" in seconds_json:
             pd.DataFrame(outr_normalize(seconds_json["EPOCHS"])).to_sql(
                 "outr_loop", con=State.db_conn, if_exists="append", index=False
             )
 
@@ -213,26 +218,27 @@
                 "epoch": -1,
                 "step": -1,
                 "name": user_var,
                 "value": d[user_var],
             }
         )
     if "CLI" in d:
-        for user_var in d['CLI']:
-            data.append({
-                "projid": cwd_shelf.get_projid(),
-                "runid": d["NAME"],
-                "tstamp": tstamp.stem,
-                "vid": hexsha,
-                "epoch": -1,
-                "step": -1,
-                "name": user_var,
-                "value": d['CLI'][user_var],
-            })
-
+        for user_var in d["CLI"]:
+            data.append(
+                {
+                    "projid": cwd_shelf.get_projid(),
+                    "runid": d["NAME"],
+                    "tstamp": tstamp.stem,
+                    "vid": hexsha,
+                    "epoch": -1,
+                    "step": -1,
+                    "name": user_var,
+                    "value": d["CLI"][user_var],
+                }
+            )
 
     if "KVS" in d:
         # LEGACY
         _kvs = d["KVS"]
 
         for k in _kvs:
             if len(k.split(".")) >= 3:
```

### Comparing `flordb-2.6.3/flor/shelf/cwd_shelf.py` & `flordb-2.6.4/flor/shelf/cwd_shelf.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.3/flor/shelf/home_shelf.py` & `flordb-2.6.4/flor/shelf/home_shelf.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.3/flor/skipblock/abstract.py` & `flordb-2.6.4/flor/skipblock/abstract.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.3/flor/skipblock/readblock.py` & `flordb-2.6.4/flor/skipblock/readblock.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.3/flor/skipblock/writeblock.py` & `flordb-2.6.4/flor/skipblock/writeblock.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.3/flor/state.py` & `flordb-2.6.4/flor/state.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.3/flordb.egg-info/PKG-INFO` & `flordb-2.6.4/flordb.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flordb
-Version: 2.6.3
+Version: 2.6.4
 Summary: Fast Low-Overhead Recovery
 Home-page: https://github.com/ucbrise/flor
 Author: Rolando Garcia
 Author-email: rogarcia@berkeley.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -21,14 +21,21 @@
 
 Flor and FlorDB are software developed at UC Berkeley's [RISE](https://rise.cs.berkeley.edu/) Lab.
 # Installation
 
 ```bash
 pip install flordb
 ```
+# Demo
+
+[![Napa Retreat Demo](https://i.ytimg.com/vi/TNSt5-i7kR4/sddefault.jpg)](https://youtu.be/TNSt5-i7kR4)
+
+<!-- https://i.ytimg.com/vi/TNSt5-i7kR4/sddefault.jpg
+https://youtu.be/TNSt5-i7kR4
+ -->
 
 # First run
 
 Run the ``examples/rnn.py`` script to test your installation. 
 This script will train a small linear model on MNIST.
 FLOR shadow branches permit us to commit your work
 automatically on every run, without interfering with your
```

### Comparing `flordb-2.6.3/flordb.egg-info/SOURCES.txt` & `flordb-2.6.4/flordb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flordb-2.6.3/setup.py` & `flordb-2.6.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import io
 
 with io.open("README.md", mode="r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="flordb",
-    version="2.6.3",
+    version="2.6.4",
     author="Rolando Garcia",
     author_email="rogarcia@berkeley.edu",
     description="Fast Low-Overhead Recovery",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ucbrise/flor",
     packages=setuptools.find_packages(),
```

