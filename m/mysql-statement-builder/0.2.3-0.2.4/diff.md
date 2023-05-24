# Comparing `tmp/mysql-statement-builder-0.2.3.tar.gz` & `tmp/mysql-statement-builder-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mysql-statement-builder-0.2.3.tar", last modified: Tue May 23 10:41:27 2023, max compression
+gzip compressed data, was "mysql-statement-builder-0.2.4.tar", last modified: Wed May 24 19:03:31 2023, max compression
```

## Comparing `mysql-statement-builder-0.2.3.tar` & `mysql-statement-builder-0.2.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 10:41:27.212502 mysql-statement-builder-0.2.3/
--rw-rw-rw-   0        0        0     1101 2023-05-23 08:20:23.000000 mysql-statement-builder-0.2.3/LICENSE
--rw-rw-rw-   0        0        0     2169 2023-05-23 10:41:27.212502 mysql-statement-builder-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     1564 2023-05-23 10:36:35.000000 mysql-statement-builder-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-23 10:41:27.195504 mysql-statement-builder-0.2.3/mysql_statement_builder.egg-info/
--rw-rw-rw-   0        0        0     2169 2023-05-23 10:41:27.000000 mysql-statement-builder-0.2.3/mysql_statement_builder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      450 2023-05-23 10:41:27.000000 mysql-statement-builder-0.2.3/mysql_statement_builder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 10:41:27.000000 mysql-statement-builder-0.2.3/mysql_statement_builder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-05-23 10:41:27.000000 mysql-statement-builder-0.2.3/mysql_statement_builder.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-23 10:41:27.000000 mysql-statement-builder-0.2.3/mysql_statement_builder.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-23 10:41:27.205496 mysql-statement-builder-0.2.3/mysqlsb/
--rw-rw-rw-   0        0        0      188 2023-05-23 10:41:12.000000 mysql-statement-builder-0.2.3/mysqlsb/__init__.py
--rw-rw-rw-   0        0        0     7560 2023-05-23 09:07:28.000000 mysql-statement-builder-0.2.3/mysqlsb/builder.py
--rw-rw-rw-   0        0        0      219 2023-05-23 07:45:37.000000 mysql-statement-builder-0.2.3/mysqlsb/configuration.py
--rw-rw-rw-   0        0        0       59 2023-05-22 15:16:44.000000 mysql-statement-builder-0.2.3/mysqlsb/exceptions.py
--rw-rw-rw-   0        0        0     2259 2023-05-23 08:48:54.000000 mysql-statement-builder-0.2.3/mysqlsb/statements.py
--rw-rw-rw-   0        0        0      612 2021-12-08 13:05:41.000000 mysql-statement-builder-0.2.3/mysqlsb/utils.py
--rw-rw-rw-   0        0        0       42 2023-05-23 10:41:27.213504 mysql-statement-builder-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0      949 2023-05-23 10:41:17.000000 mysql-statement-builder-0.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-23 10:41:27.210493 mysql-statement-builder-0.2.3/tests/
--rw-rw-rw-   0        0        0        0 2023-05-23 07:33:30.000000 mysql-statement-builder-0.2.3/tests/__init__.py
--rw-rw-rw-   0        0        0      491 2023-05-23 08:55:28.000000 mysql-statement-builder-0.2.3/tests/test_builder.py
--rw-rw-rw-   0        0        0      506 2023-05-23 08:49:25.000000 mysql-statement-builder-0.2.3/tests/test_statements.py
+drwxrwxrwx   0        0        0        0 2023-05-24 19:03:31.370955 mysql-statement-builder-0.2.4/
+-rw-rw-rw-   0        0        0     1101 2023-05-23 08:20:23.000000 mysql-statement-builder-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0     2169 2023-05-24 19:03:31.369953 mysql-statement-builder-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1564 2023-05-23 10:36:35.000000 mysql-statement-builder-0.2.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-24 19:03:31.310176 mysql-statement-builder-0.2.4/mysql_statement_builder.egg-info/
+-rw-rw-rw-   0        0        0     2169 2023-05-24 19:03:31.000000 mysql-statement-builder-0.2.4/mysql_statement_builder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      450 2023-05-24 19:03:31.000000 mysql-statement-builder-0.2.4/mysql_statement_builder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 19:03:31.000000 mysql-statement-builder-0.2.4/mysql_statement_builder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-05-24 19:03:31.000000 mysql-statement-builder-0.2.4/mysql_statement_builder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-24 19:03:31.000000 mysql-statement-builder-0.2.4/mysql_statement_builder.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-24 19:03:31.351093 mysql-statement-builder-0.2.4/mysqlsb/
+-rw-rw-rw-   0        0        0      188 2023-05-23 10:41:12.000000 mysql-statement-builder-0.2.4/mysqlsb/__init__.py
+-rw-rw-rw-   0        0        0     7560 2023-05-23 09:07:28.000000 mysql-statement-builder-0.2.4/mysqlsb/builder.py
+-rw-rw-rw-   0        0        0      219 2023-05-23 07:45:37.000000 mysql-statement-builder-0.2.4/mysqlsb/configuration.py
+-rw-rw-rw-   0        0        0      112 2023-05-24 19:02:23.000000 mysql-statement-builder-0.2.4/mysqlsb/exceptions.py
+-rw-rw-rw-   0        0        0     2259 2023-05-23 08:48:54.000000 mysql-statement-builder-0.2.4/mysqlsb/statements.py
+-rw-rw-rw-   0        0        0     1517 2023-05-24 19:02:43.000000 mysql-statement-builder-0.2.4/mysqlsb/utils.py
+-rw-rw-rw-   0        0        0       42 2023-05-24 19:03:31.370955 mysql-statement-builder-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      949 2023-05-24 19:02:58.000000 mysql-statement-builder-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 19:03:31.368970 mysql-statement-builder-0.2.4/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-23 07:33:30.000000 mysql-statement-builder-0.2.4/tests/__init__.py
+-rw-rw-rw-   0        0        0      491 2023-05-23 08:55:28.000000 mysql-statement-builder-0.2.4/tests/test_builder.py
+-rw-rw-rw-   0        0        0      506 2023-05-23 08:49:25.000000 mysql-statement-builder-0.2.4/tests/test_statements.py
```

### Comparing `mysql-statement-builder-0.2.3/LICENSE` & `mysql-statement-builder-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mysql-statement-builder-0.2.3/PKG-INFO` & `mysql-statement-builder-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysql-statement-builder
-Version: 0.2.3
+Version: 0.2.4
 Summary: Simplifies writing MySQL statements in non-ORM environments.
 Home-page: https://github.com/johnmartins/mysql-statement-builder
 Author: Julian Martinsson Bonde
 Author-email: julianm@chalmers.se
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mysql-statement-builder-0.2.3/README.md` & `mysql-statement-builder-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `mysql-statement-builder-0.2.3/mysql_statement_builder.egg-info/PKG-INFO` & `mysql-statement-builder-0.2.4/mysql_statement_builder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysql-statement-builder
-Version: 0.2.3
+Version: 0.2.4
 Summary: Simplifies writing MySQL statements in non-ORM environments.
 Home-page: https://github.com/johnmartins/mysql-statement-builder
 Author: Julian Martinsson Bonde
 Author-email: julianm@chalmers.se
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mysql-statement-builder-0.2.3/mysqlsb/builder.py` & `mysql-statement-builder-0.2.4/mysqlsb/builder.py`

 * *Files identical despite different names*

### Comparing `mysql-statement-builder-0.2.3/mysqlsb/statements.py` & `mysql-statement-builder-0.2.4/mysqlsb/statements.py`

 * *Files identical despite different names*

### Comparing `mysql-statement-builder-0.2.3/setup.py` & `mysql-statement-builder-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.2.3'
+VERSION = '0.2.4'
 DESCRIPTION = 'Simplifies writing MySQL statements in non-ORM environments.'
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='mysql-statement-builder',
```

