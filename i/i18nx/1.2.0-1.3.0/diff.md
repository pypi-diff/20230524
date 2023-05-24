# Comparing `tmp/i18nx-1.2.0.tar.gz` & `tmp/i18nx-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "i18nx-1.2.0.tar", last modified: Sat Mar 25 11:09:57 2023, max compression
+gzip compressed data, was "i18nx-1.3.0.tar", last modified: Wed May 24 17:18:39 2023, max compression
```

## Comparing `i18nx-1.2.0.tar` & `i18nx-1.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-25 11:09:57.014686 i18nx-1.2.0/
--rw-rw-rw-   0 root         (0) root         (0)     1075 2023-03-25 11:09:24.000000 i18nx-1.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4703 2023-03-25 11:09:57.013686 i18nx-1.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3767 2023-03-25 11:09:24.000000 i18nx-1.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-25 11:09:57.011686 i18nx-1.2.0/i18nx/
--rw-rw-rw-   0 root         (0) root         (0)     3429 2023-03-25 11:09:24.000000 i18nx-1.2.0/i18nx/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-25 11:09:57.013686 i18nx-1.2.0/i18nx.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4703 2023-03-25 11:09:56.000000 i18nx-1.2.0/i18nx.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      160 2023-03-25 11:09:56.000000 i18nx-1.2.0/i18nx.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-25 11:09:56.000000 i18nx-1.2.0/i18nx.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-03-25 11:09:56.000000 i18nx-1.2.0/i18nx.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-25 11:09:57.014686 i18nx-1.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1248 2023-03-25 11:09:24.000000 i18nx-1.2.0/setup.py
+drwxrwxr-x   0 demsking  (1000) demsking  (1000)        0 2023-05-24 17:18:39.392127 i18nx-1.3.0/
+-rw-rw-r--   0 demsking  (1000) demsking  (1000)     1075 2023-03-22 13:48:37.000000 i18nx-1.3.0/LICENSE
+-rw-rw-r--   0 demsking  (1000) demsking  (1000)     4703 2023-05-24 17:18:39.392127 i18nx-1.3.0/PKG-INFO
+-rw-rw-r--   0 demsking  (1000) demsking  (1000)     3767 2023-03-23 22:07:54.000000 i18nx-1.3.0/README.md
+drwxrwxr-x   0 demsking  (1000) demsking  (1000)        0 2023-05-24 17:18:39.392127 i18nx-1.3.0/i18nx/
+-rw-rw-r--   0 demsking  (1000) demsking  (1000)     4347 2023-05-24 15:22:45.000000 i18nx-1.3.0/i18nx/__init__.py
+drwxrwxr-x   0 demsking  (1000) demsking  (1000)        0 2023-05-24 17:18:39.392127 i18nx-1.3.0/i18nx.egg-info/
+-rw-rw-r--   0 demsking  (1000) demsking  (1000)     4703 2023-05-24 17:18:39.000000 i18nx-1.3.0/i18nx.egg-info/PKG-INFO
+-rw-rw-r--   0 demsking  (1000) demsking  (1000)      160 2023-05-24 17:18:39.000000 i18nx-1.3.0/i18nx.egg-info/SOURCES.txt
+-rw-rw-r--   0 demsking  (1000) demsking  (1000)        1 2023-05-24 17:18:39.000000 i18nx-1.3.0/i18nx.egg-info/dependency_links.txt
+-rw-rw-r--   0 demsking  (1000) demsking  (1000)        6 2023-05-24 17:18:39.000000 i18nx-1.3.0/i18nx.egg-info/top_level.txt
+-rw-rw-r--   0 demsking  (1000) demsking  (1000)       38 2023-05-24 17:18:39.392127 i18nx-1.3.0/setup.cfg
+-rw-rw-r--   0 demsking  (1000) demsking  (1000)     1248 2023-05-24 17:16:00.000000 i18nx-1.3.0/setup.py
```

### Comparing `i18nx-1.2.0/LICENSE` & `i18nx-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `i18nx-1.2.0/PKG-INFO` & `i18nx-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i18nx
-Version: 1.2.0
+Version: 1.3.0
 Summary: Lightweight i18n for Python
 Home-page: https://gitlab.com/demsking/i18nx
 Author: Sébastien Demanou
 Author-email: demsking@gmail.com
 License: MIT
 Project-URL: Documentation, https://gitlab.com/demsking/i18nx/-/blob/main/README.md
 Project-URL: Say Thanks!, https://www.buymeacoffee.com/demsking
```

### Comparing `i18nx-1.2.0/README.md` & `i18nx-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `i18nx-1.2.0/i18nx.egg-info/PKG-INFO` & `i18nx-1.3.0/i18nx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i18nx
-Version: 1.2.0
+Version: 1.3.0
 Summary: Lightweight i18n for Python
 Home-page: https://gitlab.com/demsking/i18nx
 Author: Sébastien Demanou
 Author-email: demsking@gmail.com
 License: MIT
 Project-URL: Documentation, https://gitlab.com/demsking/i18nx/-/blob/main/README.md
 Project-URL: Say Thanks!, https://www.buymeacoffee.com/demsking
```

### Comparing `i18nx-1.2.0/setup.py` & `i18nx-1.3.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', encoding='utf-8') as f:
   readme = f.read()
 
 setup(
   name = 'i18nx',
-  version = '1.2.0',
+  version = '1.3.0',
   description = "Lightweight i18n for Python",
   long_description = readme,
   long_description_content_type = 'text/markdown',
   keywords = 'i18n internationalization translate',
   readme = 'README.md',
   python_requires = '>=3.9',
   license = 'MIT',
```

