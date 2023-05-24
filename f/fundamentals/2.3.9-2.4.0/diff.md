# Comparing `tmp/fundamentals-2.3.9.tar.gz` & `tmp/fundamentals-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fundamentals-2.3.9.tar", last modified: Mon Nov  8 17:01:19 2021, max compression
+gzip compressed data, was "fundamentals-2.4.0.tar", last modified: Wed May 24 11:19:31 2023, max compression
```

## Comparing `fundamentals-2.3.9.tar` & `fundamentals-2.4.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2021-11-08 17:01:18.000000 fundamentals-2.3.9/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      412 2021-11-08 16:59:06.000000 fundamentals-2.3.9/.readthedocs.yaml
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2993 2021-11-08 16:59:06.000000 fundamentals-2.3.9/CHANGES.md
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    35149 2021-11-08 16:59:06.000000 fundamentals-2.3.9/LICENSE
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      304 2021-11-08 16:59:06.000000 fundamentals-2.3.9/MANIFEST.in
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2865 2021-11-08 17:01:18.000000 fundamentals-2.3.9/PKG-INFO
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2100 2021-11-08 16:59:06.000000 fundamentals-2.3.9/README.md
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2021-11-08 17:01:18.000000 fundamentals-2.3.9/fundamentals/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      318 2021-11-08 16:59:06.000000 fundamentals-2.3.9/fundamentals/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       22 2021-11-08 16:59:06.000000 fundamentals-2.3.9/fundamentals/__version__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3944 2021-11-08 16:59:06.000000 fundamentals-2.3.9/fundamentals/cl_utils.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2021-11-08 17:01:18.000000 fundamentals-2.3.9/fundamentals/commonutils/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      106 2021-11-08 16:59:06.000000 fundamentals-2.3.9/fundamentals/commonutils/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      375 2021-11-08 16:59:06.000000 fundamentals-2.3.9/fundamentals/commonutils/getpackagepath.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6521 2021-11-08 16:59:06.000000 fundamentals-2.3.9/fundamentals/docstring_test.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2021-11-08 17:01:18.000000 fundamentals-2.3.9/fundamentals/download/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      477 2021-11-08 16:59:06.000000 fundamentals-2.3.9/fundamentals/download/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1192 2021-11-08 16:59:06.000000 fundamentals-2.3.9/fundamentals/download/_dump_files_to_local_drive.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1790 2021-11-08 16:59:06.000000 fundamentals-2.3.9/fundamentals/download/_fetch.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1564 2021-11-08 16:59:06.000000 fundamentals-2.3.9/fundamentals/download/append_now_datestamp_to_filename.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1369 2021-11-08 16:59:06.000000 fundamentals-2.3.9/fundamentals/download/extract_filename_from_url.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      997 2021-11-08 16:59:06.000000 fundamentals-2.3.9/fundamentals/download/get_now_datetime_filestamp.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6824 2021-11-08 16:59:06.000000 fundamentals-2.3.9/fundamentals/download/multiobject_download.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2021-11-08 17:01:18.000000 fundamentals-2.3.9/fundamentals/files/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      306 2021-11-08 16:59:06.000000 fundamentals-2.3.9/fundamentals/files/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1765 2021-11-08 16:59:06.000000 fundamentals-2.3.9/fundamentals/files/fileChunker.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2121 2021-11-08 16:59:06.000000 fundamentals-2.3.9/fundamentals/files/list_of_dictionaries_to_mysql_inserts.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2929 2021-11-08 16:59:06.000000 fundamentals-2.3.9/fundamentals/files/recursive_directory_listing.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6445 2021-11-08 16:59:06.000000 fundamentals-2.3.9/fundamentals/files/tag.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2520 2021-11-08 16:59:06.000000 fundamentals-2.3.9/fundamentals/fmultiprocess.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     7274 2021-11-08 16:59:06.000000 fundamentals-2.3.9/fundamentals/logs.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2021-11-08 17:01:18.000000 fundamentals-2.3.9/fundamentals/mysql/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      742 2021-11-08 16:59:06.000000 fundamentals-2.3.9/fundamentals/mysql/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    21529 2021-11-08 16:59:06.000000 fundamentals-2.3.9/fundamentals/mysql/convert_dictionary_to_mysql_table.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5579 2021-11-08 16:59:06.000000 fundamentals-2.3.9/fundamentals/mysql/database.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    13993 2021-11-08 16:59:06.000000 fundamentals-2.3.9/fundamentals/mysql/directory_script_runner.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1584 2021-11-08 16:59:06.000000 fundamentals-2.3.9/fundamentals/mysql/get_database_table_column_names.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    13232 2021-11-08 16:59:06.000000 fundamentals-2.3.9/fundamentals/mysql/insert_list_of_dictionaries_into_database_tables.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2801 2021-11-08 16:59:06.000000 fundamentals-2.3.9/fundamentals/mysql/readquery.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2483 2021-11-08 16:59:06.000000 fundamentals-2.3.9/fundamentals/mysql/setup_database_connection.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    10966 2021-11-08 16:59:06.000000 fundamentals-2.3.9/fundamentals/mysql/sqlite2mysql.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1406 2021-11-08 16:59:06.000000 fundamentals-2.3.9/fundamentals/mysql/table_exists.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     7384 2021-11-08 16:59:06.000000 fundamentals-2.3.9/fundamentals/mysql/writequery.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     9717 2021-11-08 16:59:06.000000 fundamentals-2.3.9/fundamentals/mysql/yaml_to_database.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2021-11-08 17:01:18.000000 fundamentals-2.3.9/fundamentals/nose2_plugins/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       41 2021-11-08 16:59:06.000000 fundamentals-2.3.9/fundamentals/nose2_plugins/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1384 2021-11-08 16:59:06.000000 fundamentals-2.3.9/fundamentals/nose2_plugins/cprof.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2021-11-08 17:01:18.000000 fundamentals-2.3.9/fundamentals/renderer/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      162 2021-11-08 16:59:06.000000 fundamentals-2.3.9/fundamentals/renderer/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    20625 2021-11-08 16:59:06.000000 fundamentals-2.3.9/fundamentals/renderer/list_of_dictionaries.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2021-11-08 17:01:18.000000 fundamentals-2.3.9/fundamentals/stats/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      109 2021-11-08 16:59:06.000000 fundamentals-2.3.9/fundamentals/stats/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2854 2021-11-08 16:59:06.000000 fundamentals-2.3.9/fundamentals/stats/rolling_window_sigma_clip.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3137 2021-11-08 16:59:06.000000 fundamentals-2.3.9/fundamentals/times.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    22991 2021-11-08 16:59:06.000000 fundamentals-2.3.9/fundamentals/tools.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5328 2021-11-08 16:59:06.000000 fundamentals-2.3.9/fundamentals/utKit.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2021-11-08 17:01:18.000000 fundamentals-2.3.9/fundamentals.egg-info/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2865 2021-11-08 17:01:18.000000 fundamentals-2.3.9/fundamentals.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1907 2021-11-08 17:01:18.000000 fundamentals-2.3.9/fundamentals.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2021-11-08 17:01:18.000000 fundamentals-2.3.9/fundamentals.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      184 2021-11-08 17:01:18.000000 fundamentals-2.3.9/fundamentals.egg-info/entry_points.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2021-11-08 16:59:58.000000 fundamentals-2.3.9/fundamentals.egg-info/not-zip-safe
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       78 2021-11-08 17:01:18.000000 fundamentals-2.3.9/fundamentals.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       13 2021-11-08 17:01:18.000000 fundamentals-2.3.9/fundamentals.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       79 2021-11-08 17:01:18.000000 fundamentals-2.3.9/setup.cfg
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2210 2021-11-08 16:59:06.000000 fundamentals-2.3.9/setup.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-24 11:19:31.638472 fundamentals-2.4.0/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      412 2023-05-24 11:11:35.000000 fundamentals-2.4.0/.readthedocs.yaml
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3406 2023-05-24 11:11:35.000000 fundamentals-2.4.0/CHANGES.md
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    35149 2023-05-24 11:11:35.000000 fundamentals-2.4.0/LICENSE
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      363 2023-05-24 11:11:35.000000 fundamentals-2.4.0/MANIFEST.in
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2845 2023-05-24 11:19:31.638472 fundamentals-2.4.0/PKG-INFO
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2100 2023-05-24 11:11:35.000000 fundamentals-2.4.0/README.md
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-24 11:19:31.626472 fundamentals-2.4.0/fundamentals/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      351 2023-05-24 11:11:35.000000 fundamentals-2.4.0/fundamentals/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       22 2023-05-24 11:11:35.000000 fundamentals-2.4.0/fundamentals/__version__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3944 2023-05-24 11:11:35.000000 fundamentals-2.4.0/fundamentals/cl_utils.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-24 11:19:31.630472 fundamentals-2.4.0/fundamentals/commonutils/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      106 2023-05-24 11:11:35.000000 fundamentals-2.4.0/fundamentals/commonutils/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      375 2023-05-24 11:11:35.000000 fundamentals-2.4.0/fundamentals/commonutils/getpackagepath.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5224 2023-05-24 11:11:35.000000 fundamentals-2.4.0/fundamentals/daemonise.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-24 11:19:31.634472 fundamentals-2.4.0/fundamentals/download/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      477 2023-05-24 11:11:35.000000 fundamentals-2.4.0/fundamentals/download/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1192 2023-05-24 11:11:35.000000 fundamentals-2.4.0/fundamentals/download/_dump_files_to_local_drive.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1790 2023-05-24 11:11:35.000000 fundamentals-2.4.0/fundamentals/download/_fetch.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1564 2023-05-24 11:11:35.000000 fundamentals-2.4.0/fundamentals/download/append_now_datestamp_to_filename.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1369 2023-05-24 11:11:35.000000 fundamentals-2.4.0/fundamentals/download/extract_filename_from_url.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      997 2023-05-24 11:11:35.000000 fundamentals-2.4.0/fundamentals/download/get_now_datetime_filestamp.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6824 2023-05-24 11:11:35.000000 fundamentals-2.4.0/fundamentals/download/multiobject_download.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-24 11:19:31.634472 fundamentals-2.4.0/fundamentals/files/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      306 2023-05-24 11:11:35.000000 fundamentals-2.4.0/fundamentals/files/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1765 2023-05-24 11:11:35.000000 fundamentals-2.4.0/fundamentals/files/fileChunker.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2121 2023-05-24 11:11:35.000000 fundamentals-2.4.0/fundamentals/files/list_of_dictionaries_to_mysql_inserts.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2929 2023-05-24 11:11:35.000000 fundamentals-2.4.0/fundamentals/files/recursive_directory_listing.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6445 2023-05-24 11:11:35.000000 fundamentals-2.4.0/fundamentals/files/tag.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3087 2023-05-24 11:11:35.000000 fundamentals-2.4.0/fundamentals/fmultiprocess.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     7274 2023-05-24 11:11:35.000000 fundamentals-2.4.0/fundamentals/logs.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-24 11:19:31.634472 fundamentals-2.4.0/fundamentals/mysql/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      742 2023-05-24 11:11:35.000000 fundamentals-2.4.0/fundamentals/mysql/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    21529 2023-05-24 11:11:35.000000 fundamentals-2.4.0/fundamentals/mysql/convert_dictionary_to_mysql_table.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5579 2023-05-24 11:11:35.000000 fundamentals-2.4.0/fundamentals/mysql/database.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    13993 2023-05-24 11:11:35.000000 fundamentals-2.4.0/fundamentals/mysql/directory_script_runner.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1584 2023-05-24 11:11:35.000000 fundamentals-2.4.0/fundamentals/mysql/get_database_table_column_names.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    13232 2023-05-24 11:11:35.000000 fundamentals-2.4.0/fundamentals/mysql/insert_list_of_dictionaries_into_database_tables.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2801 2023-05-24 11:11:35.000000 fundamentals-2.4.0/fundamentals/mysql/readquery.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2483 2023-05-24 11:11:35.000000 fundamentals-2.4.0/fundamentals/mysql/setup_database_connection.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    10966 2023-05-24 11:11:35.000000 fundamentals-2.4.0/fundamentals/mysql/sqlite2mysql.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1406 2023-05-24 11:11:35.000000 fundamentals-2.4.0/fundamentals/mysql/table_exists.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     7416 2023-05-24 11:11:35.000000 fundamentals-2.4.0/fundamentals/mysql/writequery.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     9717 2023-05-24 11:11:35.000000 fundamentals-2.4.0/fundamentals/mysql/yaml_to_database.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-24 11:19:31.638472 fundamentals-2.4.0/fundamentals/nose2_plugins/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       41 2023-05-24 11:11:35.000000 fundamentals-2.4.0/fundamentals/nose2_plugins/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1384 2023-05-24 11:11:35.000000 fundamentals-2.4.0/fundamentals/nose2_plugins/cprof.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-24 11:19:31.638472 fundamentals-2.4.0/fundamentals/renderer/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      162 2023-05-24 11:11:35.000000 fundamentals-2.4.0/fundamentals/renderer/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    20625 2023-05-24 11:11:35.000000 fundamentals-2.4.0/fundamentals/renderer/list_of_dictionaries.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-24 11:19:31.638472 fundamentals-2.4.0/fundamentals/stats/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      109 2023-05-24 11:11:35.000000 fundamentals-2.4.0/fundamentals/stats/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2854 2023-05-24 11:11:35.000000 fundamentals-2.4.0/fundamentals/stats/rolling_window_sigma_clip.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3137 2023-05-24 11:11:35.000000 fundamentals-2.4.0/fundamentals/times.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    23090 2023-05-24 11:11:35.000000 fundamentals-2.4.0/fundamentals/tools.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5328 2023-05-24 11:11:35.000000 fundamentals-2.4.0/fundamentals/utKit.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-24 11:19:31.630472 fundamentals-2.4.0/fundamentals.egg-info/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2845 2023-05-24 11:19:31.000000 fundamentals-2.4.0/fundamentals.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1902 2023-05-24 11:19:31.000000 fundamentals-2.4.0/fundamentals.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2023-05-24 11:19:31.000000 fundamentals-2.4.0/fundamentals.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      183 2023-05-24 11:19:31.000000 fundamentals-2.4.0/fundamentals.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2023-05-24 11:15:43.000000 fundamentals-2.4.0/fundamentals.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       92 2023-05-24 11:19:31.000000 fundamentals-2.4.0/fundamentals.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       13 2023-05-24 11:19:31.000000 fundamentals-2.4.0/fundamentals.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       79 2023-05-24 11:19:31.638472 fundamentals-2.4.0/setup.cfg
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2251 2023-05-24 11:11:35.000000 fundamentals-2.4.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `fundamentals-2.3.9/CHANGES.md` & `fundamentals-2.4.0/CHANGES.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,38 @@
 
 ## Release Notes
 
-**v2.3.9 - November 8, 2021**
+**v2.4.0 - May 24, 2023**
 
-* **FIXED:** moved depreciated calls to yaml `load` to `safe_load`
+* **FEATURE** added a class to help daemonise code
 
-**v2.3.8 - September 29, 2021**
+**v2.3.12 - May 10, 2022**
 
-* **ENHANCEMENT:** fundamentals is now on conda-forge
+* **FIXED** doc fixes
 
-**v2.3.7 - September 27, 2021**
 
-* **ENHANCEMENT:** some speed improvements in multi-downloads
+**v2.3.11 - March 17, 2022**  
+
+* **FIXED**: deadlocked connections now attempt to reconnect.
+
+**v2.3.10 - March 7, 2022**  
+
+* **ENHANCEMENT:** can now turn off multiprocessing with the `turnOffMP` parameter of `fmultiprocessing`. Needed for full profiling of code.  
+
+**v2.3.9 - November 8, 2021**  
+
+* **FIXED:** moved depreciated calls to yaml `load` to `safe_load`  
+
+**v2.3.8 - September 29, 2021**  
+
+* **ENHANCEMENT:** fundamentals is now on conda-forge  
+
+**v2.3.7 - September 27, 2021**  
+
+* **ENHANCEMENT:** some speed improvements in multi-downloads  
 
 **v2.3.6 - August 16, 2021**
 
 * **FIXED:** no longer crashing for scripts where no settings file is passed in via CL arguments
 * **FIXED:** database credentials can now be passed to the command-line again
 
 **v2.3.5 - July 30, 2021**
```

### Comparing `fundamentals-2.3.9/LICENSE` & `fundamentals-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fundamentals-2.3.9/PKG-INFO` & `fundamentals-2.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: fundamentals
-Version: 2.3.9
+Version: 2.4.0
 Summary: Some fundamental tools required by most self-respecting python-packages bundled in one place. Very opinionated project setup tools including logging, plain-text settings files and database connections.
 Home-page: https://github.com/thespacedoctor/fundamentals
+Download-URL: https://github.com/thespacedoctor/fundamentals/archive/v2.4.0.zip
 Author: David Young
 Author-email: davidrobertyoung@gmail.com
 License: MIT
-Download-URL: https://github.com/thespacedoctor/fundamentals/archive/v2.3.9.zip
 Keywords: logging, database
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # fundamentals
 
 <!-- INFO BADGES -->  
@@ -40,9 +39,7 @@
 
 ## Features
 
 * 
 
 
 
-
-
```

### Comparing `fundamentals-2.3.9/README.md` & `fundamentals-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `fundamentals-2.3.9/fundamentals/cl_utils.py` & `fundamentals-2.4.0/fundamentals/cl_utils.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.3.9/fundamentals/download/_dump_files_to_local_drive.py` & `fundamentals-2.4.0/fundamentals/download/_dump_files_to_local_drive.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.3.9/fundamentals/download/_fetch.py` & `fundamentals-2.4.0/fundamentals/download/_fetch.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.3.9/fundamentals/download/append_now_datestamp_to_filename.py` & `fundamentals-2.4.0/fundamentals/download/append_now_datestamp_to_filename.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.3.9/fundamentals/download/extract_filename_from_url.py` & `fundamentals-2.4.0/fundamentals/download/extract_filename_from_url.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.3.9/fundamentals/download/get_now_datetime_filestamp.py` & `fundamentals-2.4.0/fundamentals/download/get_now_datetime_filestamp.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.3.9/fundamentals/download/multiobject_download.py` & `fundamentals-2.4.0/fundamentals/download/multiobject_download.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.3.9/fundamentals/files/fileChunker.py` & `fundamentals-2.4.0/fundamentals/files/fileChunker.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.3.9/fundamentals/files/list_of_dictionaries_to_mysql_inserts.py` & `fundamentals-2.4.0/fundamentals/files/list_of_dictionaries_to_mysql_inserts.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.3.9/fundamentals/files/recursive_directory_listing.py` & `fundamentals-2.4.0/fundamentals/files/recursive_directory_listing.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.3.9/fundamentals/files/tag.py` & `fundamentals-2.4.0/fundamentals/files/tag.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.3.9/fundamentals/fmultiprocess.py` & `fundamentals-2.4.0/fundamentals/fmultiprocess.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,39 +3,41 @@
 """
 *A function to quickly add multiprocessing to any program*
 
 :Author:
     David Young
 """
 from __future__ import division
+import inspect
+from functools import partial
+from fundamentals import tools
 from past.utils import old_div
 import sys
 import os
 os.environ['TERM'] = 'vt100'
-from fundamentals import tools
-from functools import partial
-import inspect
 
 
 def fmultiprocess(
         log,
         function,
         inputArray,
         poolSize=False,
         timeout=3600,
+        turnOffMP=False,
         **kwargs):
     """multiprocess pool
 
     **Key Arguments**
 
     - ``log`` -- logger
     - ``function`` -- the function to multiprocess
     - ``inputArray`` -- the array to be iterated over
     - ``poolSize`` -- limit the number of CPU that are used in multiprocess job
     - ``timeout`` -- time in sec after which to raise a timeout error if the processes have not completed
+    - ``turnOffMP`` -- turn off multiprocessing. Useful for profiling and debugging. Default **False**
 
 
     **Return**
 
     - ``resultArray`` -- the array of results
 
 
@@ -47,53 +49,67 @@
     inputArray = range(10000)
     results = multiprocess(log=log, function=functionName, poolSize=10, timeout=300,
                           inputArray=inputArray, otherFunctionKeyword="cheese")
     ```
 
     """
     log.debug('starting the ``multiprocess`` function')
-    import psutil
-    # import multiprocess as mp
-    # mp.set_start_method('forkserver')
-    from multiprocess import cpu_count, Pool
-
-    # DEFINTE POOL SIZE - NUMBER OF CPU CORES TO USE (BEST = ALL - 1)
-    if not poolSize:
-        poolSize = psutil.cpu_count()
-
-    if poolSize:
-        p = Pool(processes=poolSize)
-    else:
-        p = Pool()
-
-    cpuCount = psutil.cpu_count()
-    chunksize = int(old_div((len(inputArray) + 1), (cpuCount * 3)))
-
-    if chunksize == 0:
-        chunksize = 1
-
-    # chunksize = 1
 
-    # MAP-REDUCE THE WORK OVER MULTIPLE CPU CORES
     logFound = False
     # PYTHON 3 VS 2 ..
     try:
         if "log" in inspect.getfullargspec(function)[0]:
             logFound = True
     except:
         if "log" in inspect.getargspec(function)[0]:
             logFound = True
-    if logFound:
-        mapfunc = partial(function, log=log, **kwargs)
-        resultArray = p.map_async(mapfunc, inputArray, chunksize=chunksize)
-    else:
-        mapfunc = partial(function, **kwargs)
-        resultArray = p.map_async(mapfunc, inputArray, chunksize=chunksize)
 
-    resultArray = resultArray.get(timeout=timeout)
+    if turnOffMP == False:
+        import psutil
+        # import multiprocess as mp
+        # mp.set_start_method('forkserver')
+        from multiprocess import cpu_count, Pool
+
+        # DEFINTE POOL SIZE - NUMBER OF CPU CORES TO USE (BEST = ALL - 1)
+        if not poolSize:
+            poolSize = psutil.cpu_count()
+
+        if poolSize:
+            p = Pool(processes=poolSize)
+        else:
+            p = Pool()
+
+        cpuCount = psutil.cpu_count()
+        chunksize = int(old_div((len(inputArray) + 1), (cpuCount * 3)))
+
+        if chunksize == 0:
+            chunksize = 1
+
+        # chunksize = 1
+        # MAP-REDUCE THE WORK OVER MULTIPLE CPU CORES
+        if logFound:
+            mapfunc = partial(function, log=log, **kwargs)
+            resultArray = p.map_async(mapfunc, inputArray, chunksize=chunksize)
+        else:
+            mapfunc = partial(function, **kwargs)
+            resultArray = p.map_async(mapfunc, inputArray, chunksize=chunksize)
+
+        resultArray = resultArray.get(timeout=timeout)
+
+        p.close()
+        p.join()
+        # p.terminate()
+
+    else:
+        resultArray = []
 
-    p.close()
-    p.join()
-    # p.terminate()
+        if logFound:
+            for i in inputArray:
+                r = function(log, i, **kwargs)
+                resultArray.append(r)
+        else:
+            for i in inputArray:
+                r = function(i, **kwargs)
+                resultArray.append(r)
 
     log.debug('completed the ``multiprocess`` function')
     return resultArray
```

### Comparing `fundamentals-2.3.9/fundamentals/logs.py` & `fundamentals-2.4.0/fundamentals/logs.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.3.9/fundamentals/mysql/__init__.py` & `fundamentals-2.4.0/fundamentals/mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.3.9/fundamentals/mysql/convert_dictionary_to_mysql_table.py` & `fundamentals-2.4.0/fundamentals/mysql/convert_dictionary_to_mysql_table.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.3.9/fundamentals/mysql/database.py` & `fundamentals-2.4.0/fundamentals/mysql/database.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.3.9/fundamentals/mysql/directory_script_runner.py` & `fundamentals-2.4.0/fundamentals/mysql/directory_script_runner.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.3.9/fundamentals/mysql/get_database_table_column_names.py` & `fundamentals-2.4.0/fundamentals/mysql/get_database_table_column_names.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.3.9/fundamentals/mysql/insert_list_of_dictionaries_into_database_tables.py` & `fundamentals-2.4.0/fundamentals/mysql/insert_list_of_dictionaries_into_database_tables.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.3.9/fundamentals/mysql/readquery.py` & `fundamentals-2.4.0/fundamentals/mysql/readquery.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.3.9/fundamentals/mysql/setup_database_connection.py` & `fundamentals-2.4.0/fundamentals/mysql/setup_database_connection.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.3.9/fundamentals/mysql/sqlite2mysql.py` & `fundamentals-2.4.0/fundamentals/mysql/sqlite2mysql.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.3.9/fundamentals/mysql/table_exists.py` & `fundamentals-2.4.0/fundamentals/mysql/table_exists.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.3.9/fundamentals/mysql/writequery.py` & `fundamentals-2.4.0/fundamentals/mysql/writequery.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,15 +101,15 @@
                     thisList = manyValueList[offset:offset + batch]
                     offset += batch
                     a = len(thisList)
                     cursor.executemany(sqlQuery, thisList)
                     dbConn.commit()
                     if len(thisList) < batch:
                         stop = 1
-        except pymysql.err.InternalError as e:
+        except (pymysql.err.InternalError, pymysql.err.OperationalError) as e:
             if tries < 61:
                 tryAgain = True
                 log.warning(f"MySQL error: {e}. Attempt {tries}/60.")
                 tries += 1
             else:
                 log.warning(f"MySQL error: {e}. Attempt {tries}/60 failed. ")
                 raise
```

### Comparing `fundamentals-2.3.9/fundamentals/mysql/yaml_to_database.py` & `fundamentals-2.4.0/fundamentals/mysql/yaml_to_database.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.3.9/fundamentals/nose2_plugins/cprof.py` & `fundamentals-2.4.0/fundamentals/nose2_plugins/cprof.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.3.9/fundamentals/renderer/list_of_dictionaries.py` & `fundamentals-2.4.0/fundamentals/renderer/list_of_dictionaries.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.3.9/fundamentals/stats/rolling_window_sigma_clip.py` & `fundamentals-2.4.0/fundamentals/stats/rolling_window_sigma_clip.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.3.9/fundamentals/times.py` & `fundamentals-2.4.0/fundamentals/times.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.3.9/fundamentals/tools.py` & `fundamentals-2.4.0/fundamentals/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,16 @@
             arguments,
             docString,
             logLevel="WARNING",
             options_first=False,
             projectName=False,
             distributionName=False,
             orderedSettings=False,
-            defaultSettingsFile=False
+            defaultSettingsFile=False,
+            quitIfRunning=True
     ):
         self.arguments = arguments
         self.docString = docString
         self.logLevel = logLevel
 
         if not distributionName:
             distributionName = projectName
@@ -157,25 +158,26 @@
         self.arguments = arguments
 
         # BUILD A STRING FOR THE PROCESS TO MATCH RUNNING PROCESSES AGAINST
         lockname = "".join(sys.argv)
 
         # TEST IF THE PROCESS IS ALREADY RUNNING WITH THE SAME ARGUMENTS (e.g.
         # FROM CRON) - QUIT IF MATCH FOUND
-        for q in psutil.process_iter():
-            try:
-                this = q.cmdline()
-            except:
-                continue
-
-            test = "".join(this[1:])
-            if q.pid != os.getpid() and lockname == test and "--reload" not in test:
-                thisId = q.pid
-                print("This command is already running (see PID %(thisId)s)" % locals())
-                sys.exit(0)
+        if quitIfRunning:
+            for q in psutil.process_iter():
+                try:
+                    this = q.cmdline()
+                except:
+                    continue
+
+                test = "".join(this[1:])
+                if q.pid != os.getpid() and lockname == test and "--reload" not in test:
+                    thisId = q.pid
+                    print("This command is already running (see PID %(thisId)s)" % locals())
+                    sys.exit(0)
 
         try:
             if "tests.test" in arguments["<pathToSettingsFile>"]:
                 del arguments["<pathToSettingsFile>"]
         except:
             pass
 
@@ -579,9 +581,10 @@
         loader.flatten_mapping(node)
         return object_pairs_hook(loader.construct_pairs(node))
     OrderedLoader.add_constructor(
         yaml.resolver.BaseResolver.DEFAULT_MAPPING_TAG,
         construct_mapping)
     return yaml.safe_load(stream, OrderedLoader)
 
+
 if __name__ == '__main__':
     main()
```

### Comparing `fundamentals-2.3.9/fundamentals/utKit.py` & `fundamentals-2.4.0/fundamentals/utKit.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.3.9/fundamentals.egg-info/PKG-INFO` & `fundamentals-2.4.0/fundamentals.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: fundamentals
-Version: 2.3.9
+Version: 2.4.0
 Summary: Some fundamental tools required by most self-respecting python-packages bundled in one place. Very opinionated project setup tools including logging, plain-text settings files and database connections.
 Home-page: https://github.com/thespacedoctor/fundamentals
+Download-URL: https://github.com/thespacedoctor/fundamentals/archive/v2.4.0.zip
 Author: David Young
 Author-email: davidrobertyoung@gmail.com
 License: MIT
-Download-URL: https://github.com/thespacedoctor/fundamentals/archive/v2.3.9.zip
 Keywords: logging, database
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # fundamentals
 
 <!-- INFO BADGES -->  
@@ -40,9 +39,7 @@
 
 ## Features
 
 * 
 
 
 
-
-
```

### Comparing `fundamentals-2.3.9/fundamentals.egg-info/SOURCES.txt` & `fundamentals-2.4.0/fundamentals.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 fundamentals/__init__.py
 fundamentals/__version__.py
 fundamentals/cl_utils.py
-fundamentals/docstring_test.py
+fundamentals/daemonise.py
 fundamentals/fmultiprocess.py
 fundamentals/logs.py
 fundamentals/times.py
 fundamentals/tools.py
 fundamentals/utKit.py
 fundamentals.egg-info/PKG-INFO
 fundamentals.egg-info/SOURCES.txt
```

### Comparing `fundamentals-2.3.9/setup.py` & `fundamentals-2.4.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,23 +5,25 @@
 exec(open(moduleDirectory + "/fundamentals/__version__.py").read())
 
 
 def readme():
     with open(moduleDirectory + '/README.md') as f:
         return f.read()
 
+
 install_requires = [
     'pyyaml',
     'fundamentals',
     'future',
     'docopt',
     'psutil',
     'python-dateutil',
     'coloredlogs',
-    'requests'
+    'requests',
+    'python-daemon'
 ]
 
 # READ THE DOCS SERVERS
 exists = os.path.exists("/home/docs/")
 if exists:
     c_exclude_list = ['healpy', 'astropy',
                       'numpy', 'sherlock', 'wcsaxes', 'HMpTy', 'ligo-gracedb']
@@ -35,25 +37,25 @@
       version=__version__,
       description="Some fundamental tools required by most self-respecting python-packages bundled in one place. Very opinionated project setup tools including logging, plain-text settings files and database connections.",
       long_description=readme(),
       long_description_content_type='text/markdown',
       classifiers=[
           'Development Status :: 4 - Beta',
           'License :: OSI Approved :: MIT License',
-          'Programming Language :: Python :: 3.7',
+          'Programming Language :: Python :: 3.9',
           'Topic :: Utilities',
       ],
       keywords=['logging, database'],
       url='https://github.com/thespacedoctor/fundamentals',
       download_url='https://github.com/thespacedoctor/fundamentals/archive/v%(__version__)s.zip' % locals(
       ),
       author='David Young',
       author_email='davidrobertyoung@gmail.com',
       license='MIT',
-      packages=find_packages(),
+      packages=find_packages(exclude=["*tests*"]),
       include_package_data=True,
       install_requires=install_requires,
       test_suite='nose2.collector.collector',
       tests_require=['nose2', 'cov-core'],
       entry_points={
           'console_scripts': ['mysqlSucker=fundamentals.mysql.directory_script_runner:main',
                               'yaml2db=fundamentals.mysql.yaml_to_database:main',
```

