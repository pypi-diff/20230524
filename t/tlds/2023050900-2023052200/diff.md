# Comparing `tmp/tlds-2023050900.tar.gz` & `tmp/tlds-2023052200.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tlds-2023050900.tar", last modified: Tue May  9 21:19:57 2023, max compression
+gzip compressed data, was "tlds-2023052200.tar", last modified: Tue May 23 23:59:42 2023, max compression
```

## Comparing `tlds-2023050900.tar` & `tlds-2023052200.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:19:57.414707 tlds-2023050900/
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-09 21:19:51.000000 tlds-2023050900/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-09 21:19:57.414707 tlds-2023050900/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-09 21:19:51.000000 tlds-2023050900/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-09 21:19:57.414707 tlds-2023050900/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-09 21:19:51.000000 tlds-2023050900/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:19:57.410706 tlds-2023050900/tlds/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-09 21:19:51.000000 tlds-2023050900/tlds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14301 2023-05-09 21:19:51.000000 tlds-2023050900/tlds/_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:19:57.414707 tlds-2023050900/tlds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-09 21:19:57.000000 tlds-2023050900/tlds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-09 21:19:57.000000 tlds-2023050900/tlds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 21:19:57.000000 tlds-2023050900/tlds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-09 21:19:57.000000 tlds-2023050900/tlds.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 21:19:57.000000 tlds-2023050900/tlds.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:59:42.907643 tlds-2023052200/
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-23 23:59:36.000000 tlds-2023052200/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-23 23:59:42.907643 tlds-2023052200/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-23 23:59:36.000000 tlds-2023052200/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-23 23:59:42.907643 tlds-2023052200/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-23 23:59:36.000000 tlds-2023052200/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:59:42.907643 tlds-2023052200/tlds/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-23 23:59:36.000000 tlds-2023052200/tlds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14301 2023-05-23 23:59:36.000000 tlds-2023052200/tlds/_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:59:42.907643 tlds-2023052200/tlds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-23 23:59:42.000000 tlds-2023052200/tlds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-23 23:59:42.000000 tlds-2023052200/tlds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 23:59:42.000000 tlds-2023052200/tlds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-23 23:59:42.000000 tlds-2023052200/tlds.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 23:59:42.000000 tlds-2023052200/tlds.egg-info/zip-safe
```

### Comparing `tlds-2023050900/LICENSE` & `tlds-2023052200/LICENSE`

 * *Files identical despite different names*

### Comparing `tlds-2023050900/PKG-INFO` & `tlds-2023052200/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tlds
-Version: 2023050900
+Version: 2023052200
 Summary: Automatically updated list of valid TLDs taken directly from IANA
 Home-page: https://github.com/kichik/tlds
 Author: Amir Szekely
 Author-email: kichik@gmail.com
 License: MIT
 Keywords: tld
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `tlds-2023050900/README.rst` & `tlds-2023052200/README.rst`

 * *Files identical despite different names*

### Comparing `tlds-2023050900/setup.py` & `tlds-2023052200/setup.py`

 * *Files identical despite different names*

### Comparing `tlds-2023050900/tlds/_data.py` & `tlds-2023052200/tlds/_data.py`

 * *Files identical despite different names*

### Comparing `tlds-2023050900/tlds.egg-info/PKG-INFO` & `tlds-2023052200/tlds.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tlds
-Version: 2023050900
+Version: 2023052200
 Summary: Automatically updated list of valid TLDs taken directly from IANA
 Home-page: https://github.com/kichik/tlds
 Author: Amir Szekely
 Author-email: kichik@gmail.com
 License: MIT
 Keywords: tld
 Classifier: Development Status :: 5 - Production/Stable
```

