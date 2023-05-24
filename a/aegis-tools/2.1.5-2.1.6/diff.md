# Comparing `tmp/aegis-tools-2.1.5.tar.gz` & `tmp/aegis-tools-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aegis-tools-2.1.5.tar", last modified: Fri May 12 16:03:16 2023, max compression
+gzip compressed data, was "aegis-tools-2.1.6.tar", last modified: Wed May 24 02:40:42 2023, max compression
```

## Comparing `aegis-tools-2.1.5.tar` & `aegis-tools-2.1.6.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-05-12 16:03:16.109043 aegis-tools-2.1.5/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1073 2022-10-24 18:25:55.000000 aegis-tools-2.1.5/LICENSE
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       38 2022-10-24 18:25:55.000000 aegis-tools-2.1.5/MANIFEST.in
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      808 2023-05-12 16:03:16.109043 aegis-tools-2.1.5/PKG-INFO
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      881 2022-10-24 18:25:55.000000 aegis-tools-2.1.5/README.md
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-05-12 16:03:16.093043 aegis-tools-2.1.5/aegis/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       57 2022-10-24 18:25:55.000000 aegis-tools-2.1.5/aegis/__init__.py
--rwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)    17334 2022-11-21 05:05:18.000000 aegis-tools-2.1.5/aegis/aegis_.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    18804 2023-05-12 16:02:53.000000 aegis-tools-2.1.5/aegis/build.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2380 2023-01-12 20:56:01.000000 aegis-tools-2.1.5/aegis/config.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    25757 2023-04-02 20:38:42.000000 aegis-tools-2.1.5/aegis/database.py
--rwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)    25692 2023-04-04 22:56:26.000000 aegis-tools-2.1.5/aegis/hydra.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     7276 2023-04-24 22:47:56.000000 aegis-tools-2.1.5/aegis/mailer.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    42564 2023-05-05 18:15:10.000000 aegis-tools-2.1.5/aegis/model.py
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-05-12 16:03:16.101043 aegis-tools-2.1.5/aegis/sql/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1089 2022-11-22 01:51:27.000000 aegis-tools-2.1.5/aegis/sql/auditing-mysql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     4271 2023-02-05 03:12:16.000000 aegis-tools-2.1.5/aegis/sql/auditing-pgsql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1051 2022-10-24 18:25:55.000000 aegis-tools-2.1.5/aegis/sql/build-mysql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1672 2022-11-16 03:24:54.000000 aegis-tools-2.1.5/aegis/sql/build-pgsql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      450 2022-10-24 18:25:55.000000 aegis-tools-2.1.5/aegis/sql/cache_system.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1839 2023-04-02 17:24:35.000000 aegis-tools-2.1.5/aegis/sql/email_system-pgsql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1252 2023-03-13 22:09:08.000000 aegis-tools-2.1.5/aegis/sql/google_signin.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3409 2022-10-24 18:25:55.000000 aegis-tools-2.1.5/aegis/sql/hydra-mysql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3195 2022-10-24 18:25:55.000000 aegis-tools-2.1.5/aegis/sql/hydra-pgsql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1535 2022-10-24 18:25:55.000000 aegis-tools-2.1.5/aegis/sql/member_auth.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      616 2022-10-24 18:25:55.000000 aegis-tools-2.1.5/aegis/sql/monitor-mysql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      579 2022-10-24 18:25:55.000000 aegis-tools-2.1.5/aegis/sql/reports.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    31593 2023-04-24 21:25:57.000000 aegis-tools-2.1.5/aegis/stdlib.py
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-05-12 16:03:16.109043 aegis-tools-2.1.5/aegis/templates/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3083 2023-03-11 00:56:38.000000 aegis-tools-2.1.5/aegis/templates/build.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1549 2023-03-11 00:57:54.000000 aegis-tools-2.1.5/aegis/templates/build_confirm.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1187 2023-03-11 00:57:33.000000 aegis-tools-2.1.5/aegis/templates/build_form.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1217 2023-03-11 01:00:56.000000 aegis-tools-2.1.5/aegis/templates/build_view.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      253 2022-10-24 18:25:55.000000 aegis-tools-2.1.5/aegis/templates/error_message.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3297 2023-04-27 02:34:36.000000 aegis-tools-2.1.5/aegis/templates/frame.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2107 2023-03-11 00:53:08.000000 aegis-tools-2.1.5/aegis/templates/hydra.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2652 2023-03-11 00:52:58.000000 aegis-tools-2.1.5/aegis/templates/hydra_form.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1660 2023-03-11 00:55:55.000000 aegis-tools-2.1.5/aegis/templates/hydra_queue.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      109 2023-03-11 01:02:04.000000 aegis-tools-2.1.5/aegis/templates/index.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1954 2023-03-26 04:27:55.000000 aegis-tools-2.1.5/aegis/templates/report.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1909 2023-03-20 03:03:26.000000 aegis-tools-2.1.5/aegis/templates/report_form.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      745 2023-03-20 02:52:01.000000 aegis-tools-2.1.5/aegis/templates/reports.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    23427 2023-03-11 00:09:55.000000 aegis-tools-2.1.5/aegis/templates/w3.css
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2681 2022-10-24 18:25:55.000000 aegis-tools-2.1.5/aegis/threadpool.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    73309 2023-05-05 18:28:25.000000 aegis-tools-2.1.5/aegis/webapp.py
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-05-12 16:03:16.109043 aegis-tools-2.1.5/aegis_tools.egg-info/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      808 2023-05-12 16:03:16.000000 aegis-tools-2.1.5/aegis_tools.egg-info/PKG-INFO
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1176 2023-05-12 16:03:16.000000 aegis-tools-2.1.5/aegis_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)        1 2023-05-12 16:03:16.000000 aegis-tools-2.1.5/aegis_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       45 2023-05-12 16:03:16.000000 aegis-tools-2.1.5/aegis_tools.egg-info/entry_points.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       85 2023-05-12 16:03:16.000000 aegis-tools-2.1.5/aegis_tools.egg-info/requires.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)        6 2023-05-12 16:03:16.000000 aegis-tools-2.1.5/aegis_tools.egg-info/top_level.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       38 2023-05-12 16:03:16.109043 aegis-tools-2.1.5/setup.cfg
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1676 2023-05-12 16:03:01.000000 aegis-tools-2.1.5/setup.py
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-05-24 02:40:42.593545 aegis-tools-2.1.6/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1073 2022-10-24 18:25:55.000000 aegis-tools-2.1.6/LICENSE
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       38 2022-10-24 18:25:55.000000 aegis-tools-2.1.6/MANIFEST.in
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      808 2023-05-24 02:40:42.593545 aegis-tools-2.1.6/PKG-INFO
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      881 2022-10-24 18:25:55.000000 aegis-tools-2.1.6/README.md
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-05-24 02:40:42.565545 aegis-tools-2.1.6/aegis/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       57 2022-10-24 18:25:55.000000 aegis-tools-2.1.6/aegis/__init__.py
+-rwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)    17334 2022-11-21 05:05:18.000000 aegis-tools-2.1.6/aegis/aegis_.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    18804 2023-05-12 16:02:53.000000 aegis-tools-2.1.6/aegis/build.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2380 2023-01-12 20:56:01.000000 aegis-tools-2.1.6/aegis/config.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    25757 2023-04-02 20:38:42.000000 aegis-tools-2.1.6/aegis/database.py
+-rwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)    25692 2023-05-24 02:10:52.000000 aegis-tools-2.1.6/aegis/hydra.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     7276 2023-04-24 22:47:56.000000 aegis-tools-2.1.6/aegis/mailer.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    42782 2023-05-24 01:47:27.000000 aegis-tools-2.1.6/aegis/model.py
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-05-24 02:40:42.573545 aegis-tools-2.1.6/aegis/sql/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1089 2022-11-22 01:51:27.000000 aegis-tools-2.1.6/aegis/sql/auditing-mysql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     4271 2023-02-05 03:12:16.000000 aegis-tools-2.1.6/aegis/sql/auditing-pgsql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1051 2022-10-24 18:25:55.000000 aegis-tools-2.1.6/aegis/sql/build-mysql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1672 2022-11-16 03:24:54.000000 aegis-tools-2.1.6/aegis/sql/build-pgsql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      450 2022-10-24 18:25:55.000000 aegis-tools-2.1.6/aegis/sql/cache_system.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1839 2023-04-02 17:24:35.000000 aegis-tools-2.1.6/aegis/sql/email_system-pgsql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1252 2023-05-22 20:40:27.000000 aegis-tools-2.1.6/aegis/sql/google_signin.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3409 2022-10-24 18:25:55.000000 aegis-tools-2.1.6/aegis/sql/hydra-mysql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3195 2022-10-24 18:25:55.000000 aegis-tools-2.1.6/aegis/sql/hydra-pgsql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1535 2022-10-24 18:25:55.000000 aegis-tools-2.1.6/aegis/sql/member_auth.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      616 2022-10-24 18:25:55.000000 aegis-tools-2.1.6/aegis/sql/monitor-mysql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      579 2022-10-24 18:25:55.000000 aegis-tools-2.1.6/aegis/sql/reports.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    31593 2023-04-24 21:25:57.000000 aegis-tools-2.1.6/aegis/stdlib.py
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-05-24 02:40:42.585545 aegis-tools-2.1.6/aegis/templates/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3083 2023-03-11 00:56:38.000000 aegis-tools-2.1.6/aegis/templates/build.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1549 2023-03-11 00:57:54.000000 aegis-tools-2.1.6/aegis/templates/build_confirm.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1187 2023-03-11 00:57:33.000000 aegis-tools-2.1.6/aegis/templates/build_form.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1217 2023-03-11 01:00:56.000000 aegis-tools-2.1.6/aegis/templates/build_view.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      253 2022-10-24 18:25:55.000000 aegis-tools-2.1.6/aegis/templates/error_message.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3297 2023-04-27 02:34:36.000000 aegis-tools-2.1.6/aegis/templates/frame.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2107 2023-03-11 00:53:08.000000 aegis-tools-2.1.6/aegis/templates/hydra.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2652 2023-03-11 00:52:58.000000 aegis-tools-2.1.6/aegis/templates/hydra_form.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1660 2023-03-11 00:55:55.000000 aegis-tools-2.1.6/aegis/templates/hydra_queue.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      109 2023-03-11 01:02:04.000000 aegis-tools-2.1.6/aegis/templates/index.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1954 2023-03-26 04:27:55.000000 aegis-tools-2.1.6/aegis/templates/report.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1909 2023-03-20 03:03:26.000000 aegis-tools-2.1.6/aegis/templates/report_form.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      745 2023-03-20 02:52:01.000000 aegis-tools-2.1.6/aegis/templates/reports.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    23427 2023-03-11 00:09:55.000000 aegis-tools-2.1.6/aegis/templates/w3.css
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2681 2022-10-24 18:25:55.000000 aegis-tools-2.1.6/aegis/threadpool.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    73800 2023-05-24 02:36:08.000000 aegis-tools-2.1.6/aegis/webapp.py
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-05-24 02:40:42.593545 aegis-tools-2.1.6/aegis_tools.egg-info/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      808 2023-05-24 02:40:42.000000 aegis-tools-2.1.6/aegis_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1176 2023-05-24 02:40:42.000000 aegis-tools-2.1.6/aegis_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)        1 2023-05-24 02:40:42.000000 aegis-tools-2.1.6/aegis_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       45 2023-05-24 02:40:42.000000 aegis-tools-2.1.6/aegis_tools.egg-info/entry_points.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       85 2023-05-24 02:40:42.000000 aegis-tools-2.1.6/aegis_tools.egg-info/requires.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)        6 2023-05-24 02:40:42.000000 aegis-tools-2.1.6/aegis_tools.egg-info/top_level.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       38 2023-05-24 02:40:42.593545 aegis-tools-2.1.6/setup.cfg
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1676 2023-05-22 20:48:40.000000 aegis-tools-2.1.6/setup.py
```

### Comparing `aegis-tools-2.1.5/LICENSE` & `aegis-tools-2.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.5/PKG-INFO` & `aegis-tools-2.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aegis-tools
-Version: 2.1.5
+Version: 2.1.6
 Summary: Aegis is a set of battle-tested tools and tricks to help everyone make better software
 Home-page: https://github.com/mdagosta/aegis
 Author: Michael D'Agosta
 Author-email: mdagosta@codebug.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aegis-tools-2.1.5/README.md` & `aegis-tools-2.1.6/README.md`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.5/aegis/aegis_.py` & `aegis-tools-2.1.6/aegis/aegis_.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.5/aegis/build.py` & `aegis-tools-2.1.6/aegis/build.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.5/aegis/config.py` & `aegis-tools-2.1.6/aegis/config.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.5/aegis/database.py` & `aegis-tools-2.1.6/aegis/database.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.5/aegis/hydra.py` & `aegis-tools-2.1.6/aegis/hydra.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.5/aegis/mailer.py` & `aegis-tools-2.1.6/aegis/mailer.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.5/aegis/model.py` & `aegis-tools-2.1.6/aegis/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,18 +192,19 @@
     def insert(email_id):
         sql = "INSERT INTO member (email_id) VALUES (%s)"
         if type(db()) is aegis.database.PostgresConnection:
             sql += ' RETURNING member_id'
         return db().execute(sql, email_id)
 
     @classmethod
-    def set_member(cls, email_id, marketing_id=None):
+    def set_member(cls, email_id, marketing_id=None, **kwargs):
         member = cls.get_email_id(email_id)
         if not member:
             columns = {'email_id': email_id}
+            columns.update(kwargs)
             if marketing_id:
                 columns['marketing_id'] = marketing_id
             member_id = cls.insert_columns(**columns)
             member = cls.get_id(member_id)
         return member
 
     @classmethod
@@ -327,14 +328,18 @@
         sql = "SELECT * FROM google_user WHERE member_id=%s"
         return db().get(sql, member_id, cls=cls)
 
     def hard_delete(self):
         sql = "DELETE FROM google_user WHERE google_user_id=%s"
         return db().execute(sql, self['google_user_id'])
 
+    def set_scopes(self, scopes):
+        sql = "UPDATE google_user SET scopes=%s WHERE google_user_id=%s"
+        return db().execute(sql, scopes, self['google_user_id'])
+
 
 class GoogleAccess(aegis.database.Row):
     table_name = 'google_access'
     id_column = 'google_access_id'
     primary_key = ('google_access_id')
 
     @classmethod
```

### Comparing `aegis-tools-2.1.5/aegis/sql/auditing-mysql.sql` & `aegis-tools-2.1.6/aegis/sql/auditing-mysql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.5/aegis/sql/auditing-pgsql.sql` & `aegis-tools-2.1.6/aegis/sql/auditing-pgsql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.5/aegis/sql/build-mysql.sql` & `aegis-tools-2.1.6/aegis/sql/build-mysql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.5/aegis/sql/build-pgsql.sql` & `aegis-tools-2.1.6/aegis/sql/build-pgsql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.5/aegis/sql/email_system-pgsql.sql` & `aegis-tools-2.1.6/aegis/sql/email_system-pgsql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.5/aegis/sql/google_signin.sql` & `aegis-tools-2.1.6/aegis/sql/google_signin.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.5/aegis/sql/hydra-mysql.sql` & `aegis-tools-2.1.6/aegis/sql/hydra-mysql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.5/aegis/sql/hydra-pgsql.sql` & `aegis-tools-2.1.6/aegis/sql/hydra-pgsql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.5/aegis/sql/member_auth.sql` & `aegis-tools-2.1.6/aegis/sql/member_auth.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.5/aegis/sql/monitor-mysql.sql` & `aegis-tools-2.1.6/aegis/sql/monitor-mysql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.5/aegis/sql/reports.sql` & `aegis-tools-2.1.6/aegis/sql/reports.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.5/aegis/stdlib.py` & `aegis-tools-2.1.6/aegis/stdlib.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.5/aegis/templates/build.html` & `aegis-tools-2.1.6/aegis/templates/build.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.5/aegis/templates/build_confirm.html` & `aegis-tools-2.1.6/aegis/templates/build_confirm.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.5/aegis/templates/build_form.html` & `aegis-tools-2.1.6/aegis/templates/build_form.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.5/aegis/templates/build_view.html` & `aegis-tools-2.1.6/aegis/templates/build_view.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.5/aegis/templates/frame.html` & `aegis-tools-2.1.6/aegis/templates/frame.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.5/aegis/templates/hydra.html` & `aegis-tools-2.1.6/aegis/templates/hydra.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.5/aegis/templates/hydra_form.html` & `aegis-tools-2.1.6/aegis/templates/hydra_form.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.5/aegis/templates/hydra_queue.html` & `aegis-tools-2.1.6/aegis/templates/hydra_queue.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.5/aegis/templates/report.html` & `aegis-tools-2.1.6/aegis/templates/report.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.5/aegis/templates/report_form.html` & `aegis-tools-2.1.6/aegis/templates/report_form.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.5/aegis/templates/reports.html` & `aegis-tools-2.1.6/aegis/templates/reports.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.5/aegis/templates/w3.css` & `aegis-tools-2.1.6/aegis/templates/w3.css`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.5/aegis/threadpool.py` & `aegis-tools-2.1.6/aegis/threadpool.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.5/aegis/webapp.py` & `aegis-tools-2.1.6/aegis/webapp.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,14 +65,15 @@
             # Ignore hostnames not in config.py. Only use the ones we have specified.
             if self.tmpl['host'] not in config.hostnames.keys():
                 logging.warning("Ignore hostname not specified in config.py: %s", self.tmpl['host'])
                 raise tornado.web.HTTPError(404)
         config.apply_hostname(self.tmpl['host'])
         if not aegis.config.get('skip_hostname_check'):
             self.tmpl['domain'] = options.domain
+        self.tmpl['host_config'] = config.hostnames[self.tmpl['host']]
         self.tmpl['options'] = options
         self.tmpl['program_name'] = options.program_name
         self.tmpl['app_name'] = options.app_name
         self.tmpl['env'] = config.get_env()
         self.tmpl['referer'] = self.request.headers.get('Referer')
         self.tmpl['user_agent'] = self.request.headers.get('User-Agent')
         self.tmpl['scheme'] = 'https://'
@@ -109,16 +110,16 @@
         self.tmpl['next_url'] = self.get_next_url()
         self.request.args = dict([(key, self.get_argument(key, strip=False)) for key, val in self.request.arguments.items()])
         self.setup_user()
         self.track_email()
         # Enable/Disable auditing. Allow for host-specific override in config.py hostnames. Else just use from options.use_audit, or False.
         self.use_audit = False
         if aegis.config.exists('use_audit'):
-            if hasattr(config, 'hostnames') and 'use_audit' in config.hostnames[self.tmpl['host']]:
-                self.use_audit = config.hostnames[self.tmpl['host']].get('use_audit')
+            if hasattr(config, 'hostnames') and 'use_audit' in self.tmpl['host_config']:
+                self.use_audit = self.tmpl['host_config'].get('use_audit')
             else:
                 self.use_audit = options.use_audit
         if self.use_audit:
             self.set_marketing_id()
             self.audit_start()
         super(AegisHandler, self).prepare()
         if self._parent_timer:
@@ -241,15 +242,16 @@
         return bool(self.tmpl['user_agent_obj'].is_bot or aegis.stdlib.is_robot(self.tmpl['user_agent']))
 
     def get_template_path(self):
         return options.template_path
 
     def render(self, template_name, **kwargs):
         aegis.stdlib.timer_start(self.timer_obj, 'render')
-        template_path = os.path.join(options.template_path, template_name)
+        template_path = self.tmpl['host_config'].get('template_path') or options.template_path
+        template_path = os.path.join(template_path, template_name)
         # Override parent class render to remove the embeds and instrument a timer here. Copied in from tornado/web.py render()
         if self._finished:
             raise RuntimeError("Cannot render() after finish()")
         html = self.render_string(template_name, **kwargs)
         aegis.stdlib.timer_stop(self.timer_obj, 'render')
         self.finish(html)
 
@@ -282,14 +284,19 @@
             return
 
         # Send errors to chat hooks, based on them being configured for the environment
         header = "`[%s ENV   %s   %s   uid: %s   mid: %s]`" % (config.get_env().upper(), self.request.uri, self.tmpl['request_name'], self.get_user_id() or '-', self.get_member_id() or '-')
         template_opts = {'handler': self, 'traceback': traceback.format_exc(), 'kwargs': {}, 'header': header}
         template_opts['kwargs']['user_agent'] = self.tmpl['user_agent']
         template_opts['kwargs']['remote_ip'] = self.request.remote_ip
+        if hasattr(self, 'audit_request'):
+            template_opts['kwargs']['country_cd'] = self.audit_request['country_cd']
+            template_opts['kwargs']['region_cd'] = self.audit_request['region_cd']
+        if hasattr(self, 'audit_session'):
+            template_opts['kwargs']['audit_session_id'] = self.audit_session.get('audit_session_id')
         template_opts['kwargs']['robot'] = self.user_is_robot()
         template_opts['kwargs']['Python UTC Now'] = self.tmpl['utcnow'].strftime('%Y-%m-%dT%H:%M:%S')
         error_message = self.render_string("error_message.txt", **template_opts).decode('utf-8')
         if config.get_env() == 'prod':
             hooks = ['alerts_chat_hook']
         else:
             hooks = ['debug_chat_hook']
```

### Comparing `aegis-tools-2.1.5/aegis_tools.egg-info/PKG-INFO` & `aegis-tools-2.1.6/aegis_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aegis-tools
-Version: 2.1.5
+Version: 2.1.6
 Summary: Aegis is a set of battle-tested tools and tricks to help everyone make better software
 Home-page: https://github.com/mdagosta/aegis
 Author: Michael D'Agosta
 Author-email: mdagosta@codebug.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aegis-tools-2.1.5/aegis_tools.egg-info/SOURCES.txt` & `aegis-tools-2.1.6/aegis_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.5/setup.py` & `aegis-tools-2.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 """
 
 import os
 import setuptools
 
 setuptools.setup (
     name = 'aegis-tools',
-    version = '2.1.5',
+    version = '2.1.6',
     description = 'Aegis is a set of battle-tested tools and tricks to help everyone make better software',
     long_description = 'A combination of tools and framework, Aegis has multiple different uses. You can import it and use the thoroughly made and tested functions. You can use it as a natural extension for the tornado web framework. And you can use it to quickly create a new web application with the structure already built-in, and follow along.',
     author = "Michael D'Agosta",
     author_email = 'mdagosta@codebug.com',
     url = 'https://github.com/mdagosta/aegis',
     python_requires='>=3.6',
     packages = ['aegis'],
```

