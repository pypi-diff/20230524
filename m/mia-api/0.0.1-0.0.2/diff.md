# Comparing `tmp/mia_api-0.0.1.tar.gz` & `tmp/mia_api-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mia_api-0.0.1.tar", last modified: Thu Mar 17 20:47:39 2022, max compression
+gzip compressed data, was "mia_api-0.0.2.tar", last modified: Mon Jan 16 19:55:09 2023, max compression
```

## Comparing `mia_api-0.0.1.tar` & `mia_api-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 gilly     (1000) gilly     (1000)        0 2022-03-17 20:47:39.828341 mia_api-0.0.1/
--rw-rw-r--   0 gilly     (1000) gilly     (1000)      574 2022-03-17 20:47:39.828341 mia_api-0.0.1/PKG-INFO
--rw-rw-r--   0 gilly     (1000) gilly     (1000)      145 2022-03-17 20:38:13.000000 mia_api-0.0.1/README.md
--rw-rw-r--   0 gilly     (1000) gilly     (1000)       85 2022-03-17 20:38:32.000000 mia_api-0.0.1/pyproject.toml
--rw-rw-r--   0 gilly     (1000) gilly     (1000)      561 2022-03-17 20:47:39.832341 mia_api-0.0.1/setup.cfg
--rw-rw-r--   0 gilly     (1000) gilly     (1000)      613 2022-03-17 20:47:11.000000 mia_api-0.0.1/setup.py
-drwxrwxr-x   0 gilly     (1000) gilly     (1000)        0 2022-03-17 20:47:39.828341 mia_api-0.0.1/src/
-drwxrwxr-x   0 gilly     (1000) gilly     (1000)        0 2022-03-17 20:47:39.828341 mia_api-0.0.1/src/mia_api/
--rw-rw-r--   0 gilly     (1000) gilly     (1000)        0 2022-02-25 21:32:22.000000 mia_api-0.0.1/src/mia_api/__init__.py
--rw-rw-r--   0 gilly     (1000) gilly     (1000)     1187 2022-03-14 15:00:52.000000 mia_api-0.0.1/src/mia_api/bar.py
--rw-rw-r--   0 gilly     (1000) gilly     (1000)       38 2022-02-25 21:34:21.000000 mia_api-0.0.1/src/mia_api/config_file.py
--rw-rw-r--   0 gilly     (1000) gilly     (1000)     2930 2022-03-16 18:34:39.000000 mia_api-0.0.1/src/mia_api/juice.py
--rw-rw-r--   0 gilly     (1000) gilly     (1000)      891 2022-03-17 20:17:57.000000 mia_api-0.0.1/src/mia_api/user.py
--rw-rw-r--   0 gilly     (1000) gilly     (1000)      373 2022-03-14 14:57:41.000000 mia_api-0.0.1/src/mia_api/utils.py
-drwxrwxr-x   0 gilly     (1000) gilly     (1000)        0 2022-03-17 20:47:39.828341 mia_api-0.0.1/src/mia_api.egg-info/
--rw-rw-r--   0 gilly     (1000) gilly     (1000)      574 2022-03-17 20:47:38.000000 mia_api-0.0.1/src/mia_api.egg-info/PKG-INFO
--rw-rw-r--   0 gilly     (1000) gilly     (1000)      315 2022-03-17 20:47:39.000000 mia_api-0.0.1/src/mia_api.egg-info/SOURCES.txt
--rw-rw-r--   0 gilly     (1000) gilly     (1000)        1 2022-03-17 20:47:39.000000 mia_api-0.0.1/src/mia_api.egg-info/dependency_links.txt
--rw-rw-r--   0 gilly     (1000) gilly     (1000)        8 2022-03-17 20:47:39.000000 mia_api-0.0.1/src/mia_api.egg-info/top_level.txt
+drwxrwxr-x   0 gilly     (1000) gilly     (1000)        0 2023-01-16 19:55:09.249084 mia_api-0.0.2/
+-rw-rw-r--   0 gilly     (1000) gilly     (1000)      537 2023-01-16 19:55:09.249084 mia_api-0.0.2/PKG-INFO
+-rwxrwxrwx   0 gilly     (1000) gilly     (1000)      145 2022-07-29 12:38:50.000000 mia_api-0.0.2/README.md
+-rwxrwxrwx   0 gilly     (1000) gilly     (1000)       85 2022-07-29 12:38:50.000000 mia_api-0.0.2/pyproject.toml
+-rwxrwxrwx   0 gilly     (1000) gilly     (1000)      561 2023-01-16 19:55:09.249084 mia_api-0.0.2/setup.cfg
+-rwxrwxrwx   0 gilly     (1000) gilly     (1000)      613 2023-01-16 19:53:12.000000 mia_api-0.0.2/setup.py
+drwxrwxr-x   0 gilly     (1000) gilly     (1000)        0 2023-01-16 19:55:09.249084 mia_api-0.0.2/src/
+drwxrwxr-x   0 gilly     (1000) gilly     (1000)        0 2023-01-16 19:55:09.249084 mia_api-0.0.2/src/mia_api/
+-rwxrwxrwx   0 gilly     (1000) gilly     (1000)       73 2023-01-16 19:51:32.000000 mia_api-0.0.2/src/mia_api/__init__.py
+-rwxrwxrwx   0 gilly     (1000) gilly     (1000)       38 2023-01-16 19:51:32.000000 mia_api-0.0.2/src/mia_api/config_file.py
+-rwxrwxrwx   0 gilly     (1000) gilly     (1000)      775 2023-01-16 19:51:32.000000 mia_api-0.0.2/src/mia_api/connect.py
+-rwxrwxrwx   0 gilly     (1000) gilly     (1000)      735 2023-01-16 19:51:32.000000 mia_api-0.0.2/src/mia_api/juice.py
+-rwxrwxrwx   0 gilly     (1000) gilly     (1000)     3546 2023-01-16 19:51:32.000000 mia_api-0.0.2/src/mia_api/models.py
+-rwxrwxrwx   0 gilly     (1000) gilly     (1000)      373 2023-01-16 19:51:32.000000 mia_api-0.0.2/src/mia_api/utils.py
+drwxrwxr-x   0 gilly     (1000) gilly     (1000)        0 2023-01-16 19:55:09.249084 mia_api-0.0.2/src/mia_api.egg-info/
+-rwxrwxrwx   0 gilly     (1000) gilly     (1000)      537 2023-01-16 19:55:09.000000 mia_api-0.0.2/src/mia_api.egg-info/PKG-INFO
+-rwxrwxrwx   0 gilly     (1000) gilly     (1000)      321 2023-01-16 19:55:09.000000 mia_api-0.0.2/src/mia_api.egg-info/SOURCES.txt
+-rwxrwxrwx   0 gilly     (1000) gilly     (1000)        1 2023-01-16 19:55:09.000000 mia_api-0.0.2/src/mia_api.egg-info/dependency_links.txt
+-rwxrwxrwx   0 gilly     (1000) gilly     (1000)        8 2023-01-16 19:55:09.000000 mia_api-0.0.2/src/mia_api.egg-info/top_level.txt
```

### Comparing `mia_api-0.0.1/setup.cfg` & `mia_api-0.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `mia_api-0.0.1/setup.py` & `mia_api-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name='mia_api',
-  version='0.0.1',
+  version='0.0.2',
   author='MeteoIA',
   author_email='meteoia.consult@meteoia.com',
   description='A package to communicate with MIA API',
   long_description=long_description,
   long_description_content_type="text/markdown",
   url='https://github.com/meteoia-team/mia_api',
   project_urls = {
```

