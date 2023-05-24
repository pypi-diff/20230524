# Comparing `tmp/nbdocs-0.0.41.tar.gz` & `tmp/nbdocs-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbdocs-0.0.41.tar", last modified: Thu Mar 31 07:09:37 2022, max compression
+gzip compressed data, was "nbdocs-0.2.2.tar", last modified: Wed May 24 10:52:15 2023, max compression
```

## Comparing `nbdocs-0.0.41.tar` & `nbdocs-0.2.2.tar`

### file list

```diff
@@ -1,29 +1,45 @@
-drwxrwxr-x   0 jzz       (1000) jzz       (1000)        0 2022-03-31 07:09:37.092671 nbdocs-0.0.41/
--rw-rw-r--   0 jzz       (1000) jzz       (1000)    11348 2022-03-30 19:52:21.000000 nbdocs-0.0.41/LICENSE
--rw-rw-r--   0 jzz       (1000) jzz       (1000)      539 2022-03-31 07:09:37.092671 nbdocs-0.0.41/PKG-INFO
--rw-rw-r--   0 jzz       (1000) jzz       (1000)       45 2022-03-02 06:29:32.000000 nbdocs-0.0.41/README.md
--rw-rw-r--   0 jzz       (1000) jzz       (1000)      245 2022-03-30 19:52:21.000000 nbdocs-0.0.41/pyproject.toml
--rw-rw-r--   0 jzz       (1000) jzz       (1000)      822 2022-03-31 07:09:37.096671 nbdocs-0.0.41/setup.cfg
--rw-rw-r--   0 jzz       (1000) jzz       (1000)      820 2022-03-30 19:52:21.000000 nbdocs-0.0.41/setup.py
-drwxrwxr-x   0 jzz       (1000) jzz       (1000)        0 2022-03-31 07:09:37.080670 nbdocs-0.0.41/src/
-drwxrwxr-x   0 jzz       (1000) jzz       (1000)        0 2022-03-31 07:09:37.088671 nbdocs-0.0.41/src/nbdocs/
--rw-rw-r--   0 jzz       (1000) jzz       (1000)       33 2022-03-30 19:52:21.000000 nbdocs-0.0.41/src/nbdocs/__init__.py
--rw-rw-r--   0 jzz       (1000) jzz       (1000)       46 2022-03-30 19:52:21.000000 nbdocs-0.0.41/src/nbdocs/__main__.py
-drwxrwxr-x   0 jzz       (1000) jzz       (1000)        0 2022-03-31 07:09:37.092671 nbdocs-0.0.41/src/nbdocs/apps/
--rw-rw-r--   0 jzz       (1000) jzz       (1000)        0 2022-03-30 19:52:21.000000 nbdocs-0.0.41/src/nbdocs/apps/__init__.py
--rw-rw-r--   0 jzz       (1000) jzz       (1000)     1417 2022-03-31 06:44:55.000000 nbdocs-0.0.41/src/nbdocs/apps/app_nb2md.py
--rw-rw-r--   0 jzz       (1000) jzz       (1000)      817 2022-03-31 06:44:55.000000 nbdocs-0.0.41/src/nbdocs/apps/app_nbclean.py
--rw-rw-r--   0 jzz       (1000) jzz       (1000)     1712 2022-03-31 06:44:55.000000 nbdocs-0.0.41/src/nbdocs/apps/app_nbdocs.py
--rw-rw-r--   0 jzz       (1000) jzz       (1000)     1800 2022-03-31 06:44:55.000000 nbdocs-0.0.41/src/nbdocs/clean.py
--rw-rw-r--   0 jzz       (1000) jzz       (1000)     1451 2022-03-31 06:44:55.000000 nbdocs-0.0.41/src/nbdocs/convert.py
--rw-rw-r--   0 jzz       (1000) jzz       (1000)     3115 2022-03-31 06:44:55.000000 nbdocs-0.0.41/src/nbdocs/core.py
--rw-rw-r--   0 jzz       (1000) jzz       (1000)     8118 2022-03-31 06:44:55.000000 nbdocs-0.0.41/src/nbdocs/process.py
--rw-rw-r--   0 jzz       (1000) jzz       (1000)      116 2022-03-31 06:44:55.000000 nbdocs-0.0.41/src/nbdocs/settings.py
--rw-rw-r--   0 jzz       (1000) jzz       (1000)       23 2022-03-31 07:09:20.000000 nbdocs-0.0.41/src/nbdocs/version.py
-drwxrwxr-x   0 jzz       (1000) jzz       (1000)        0 2022-03-31 07:09:37.092671 nbdocs-0.0.41/src/nbdocs.egg-info/
--rw-rw-r--   0 jzz       (1000) jzz       (1000)      539 2022-03-31 07:09:36.000000 nbdocs-0.0.41/src/nbdocs.egg-info/PKG-INFO
--rw-rw-r--   0 jzz       (1000) jzz       (1000)      549 2022-03-31 07:09:36.000000 nbdocs-0.0.41/src/nbdocs.egg-info/SOURCES.txt
--rw-rw-r--   0 jzz       (1000) jzz       (1000)        1 2022-03-31 07:09:36.000000 nbdocs-0.0.41/src/nbdocs.egg-info/dependency_links.txt
--rw-rw-r--   0 jzz       (1000) jzz       (1000)      247 2022-03-31 07:09:36.000000 nbdocs-0.0.41/src/nbdocs.egg-info/entry_points.txt
--rw-rw-r--   0 jzz       (1000) jzz       (1000)       82 2022-03-31 07:09:36.000000 nbdocs-0.0.41/src/nbdocs.egg-info/requires.txt
--rw-rw-r--   0 jzz       (1000) jzz       (1000)        7 2022-03-31 07:09:36.000000 nbdocs-0.0.41/src/nbdocs.egg-info/top_level.txt
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-05-24 10:52:15.247217 nbdocs-0.2.2/
+-rw-rw-r--   0 aya       (1000) aya       (1000)    11348 2022-05-11 12:40:15.000000 nbdocs-0.2.2/LICENSE
+-rw-rw-r--   0 aya       (1000) aya       (1000)      518 2023-05-24 10:52:15.247217 nbdocs-0.2.2/PKG-INFO
+-rw-rw-r--   0 aya       (1000) aya       (1000)       45 2022-02-09 06:21:26.000000 nbdocs-0.2.2/README.md
+-rw-rw-r--   0 aya       (1000) aya       (1000)      229 2022-05-30 14:55:48.000000 nbdocs-0.2.2/pyproject.toml
+-rw-rw-r--   0 aya       (1000) aya       (1000)      871 2023-05-24 10:52:15.247217 nbdocs-0.2.2/setup.cfg
+-rw-rw-r--   0 aya       (1000) aya       (1000)      597 2022-05-27 11:09:38.000000 nbdocs-0.2.2/setup.py
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-05-24 10:52:15.239217 nbdocs-0.2.2/src/
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-05-24 10:52:15.243217 nbdocs-0.2.2/src/nbdocs/
+-rw-rw-r--   0 aya       (1000) aya       (1000)       39 2022-05-27 11:09:38.000000 nbdocs-0.2.2/src/nbdocs/__init__.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)       48 2023-05-23 08:14:45.000000 nbdocs-0.2.2/src/nbdocs/__main__.py
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-05-24 10:52:15.247217 nbdocs-0.2.2/src/nbdocs/apps/
+-rw-rw-r--   0 aya       (1000) aya       (1000)        0 2022-05-11 12:40:15.000000 nbdocs-0.2.2/src/nbdocs/apps/__init__.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     2737 2023-05-24 10:48:02.000000 nbdocs-0.2.2/src/nbdocs/apps/app_nb2md.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     1434 2023-05-24 10:48:02.000000 nbdocs-0.2.2/src/nbdocs/apps/app_nbclean.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     3224 2023-05-24 10:48:02.000000 nbdocs-0.2.2/src/nbdocs/apps/app_nbdocs.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     2697 2023-05-24 10:48:02.000000 nbdocs-0.2.2/src/nbdocs/cfg_tools.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     5077 2023-05-17 15:24:05.000000 nbdocs-0.2.2/src/nbdocs/clean.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     4520 2023-05-24 10:48:02.000000 nbdocs-0.2.2/src/nbdocs/convert.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     2014 2023-05-23 08:14:45.000000 nbdocs-0.2.2/src/nbdocs/core.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     1188 2023-05-24 10:48:02.000000 nbdocs-0.2.2/src/nbdocs/default_settings.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)    11541 2023-05-24 10:48:02.000000 nbdocs-0.2.2/src/nbdocs/process.py
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-05-24 10:52:15.247217 nbdocs-0.2.2/src/nbdocs/tests/
+-rw-rw-r--   0 aya       (1000) aya       (1000)        0 2022-05-29 14:45:46.000000 nbdocs-0.2.2/src/nbdocs/tests/__init__.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     4066 2023-05-22 08:43:58.000000 nbdocs-0.2.2/src/nbdocs/tests/base.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     2746 2023-05-22 08:43:58.000000 nbdocs-0.2.2/src/nbdocs/typing.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)       22 2023-05-24 10:50:59.000000 nbdocs-0.2.2/src/nbdocs/version.py
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-05-24 10:52:15.243217 nbdocs-0.2.2/src/nbdocs.egg-info/
+-rw-rw-r--   0 aya       (1000) aya       (1000)      518 2023-05-24 10:52:15.000000 nbdocs-0.2.2/src/nbdocs.egg-info/PKG-INFO
+-rw-rw-r--   0 aya       (1000) aya       (1000)      889 2023-05-24 10:52:15.000000 nbdocs-0.2.2/src/nbdocs.egg-info/SOURCES.txt
+-rw-rw-r--   0 aya       (1000) aya       (1000)        1 2023-05-24 10:52:15.000000 nbdocs-0.2.2/src/nbdocs.egg-info/dependency_links.txt
+-rw-rw-r--   0 aya       (1000) aya       (1000)      252 2023-05-24 10:52:15.000000 nbdocs-0.2.2/src/nbdocs.egg-info/entry_points.txt
+-rw-rw-r--   0 aya       (1000) aya       (1000)       88 2023-05-24 10:52:15.000000 nbdocs-0.2.2/src/nbdocs.egg-info/requires.txt
+-rw-rw-r--   0 aya       (1000) aya       (1000)        7 2023-05-24 10:52:15.000000 nbdocs-0.2.2/src/nbdocs.egg-info/top_level.txt
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-05-24 10:52:15.247217 nbdocs-0.2.2/tests/
+-rw-rw-r--   0 aya       (1000) aya       (1000)     3332 2023-05-23 08:14:45.000000 nbdocs-0.2.2/tests/test_apps.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     3108 2023-05-22 08:43:36.000000 nbdocs-0.2.2/tests/test_base.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     1499 2023-05-22 08:43:36.000000 nbdocs-0.2.2/tests/test_clean.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     3697 2023-05-24 10:48:02.000000 nbdocs-0.2.2/tests/test_convert.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     2123 2023-05-24 10:48:02.000000 nbdocs-0.2.2/tests/test_core.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     1665 2023-05-03 13:42:07.000000 nbdocs-0.2.2/tests/test_process_collapse.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     2433 2023-05-03 13:42:07.000000 nbdocs-0.2.2/tests/test_process_hide.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     4577 2023-05-24 10:48:02.000000 nbdocs-0.2.2/tests/test_process_links.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     1053 2023-05-03 08:06:54.000000 nbdocs-0.2.2/tests/test_process_re.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     2102 2023-05-24 10:48:02.000000 nbdocs-0.2.2/tests/test_settings.py
```

### Comparing `nbdocs-0.0.41/LICENSE` & `nbdocs-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nbdocs-0.0.41/setup.cfg` & `nbdocs-0.2.2/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 [metadata]
 name = nbdocs
+version = attr: nbdocs.version.__version__
 author = Yasyrev Andrei
 author_email = a.yasyrev@gmail.com
 description = Docs from jupyter notebooks.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ayasyrev/nbdocs
 license = apache2
@@ -12,26 +13,26 @@
 	License :: OSI Approved :: Apache Software License
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
 	= src
 packages = find:
-python_requires = >=3.7
+python_requires = >=3.8
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts = 
-	nbdocs=nbdocs.apps.app_nbdocs:app
-	nb2md=nbdocs.apps.app_nb2md:app
-	nbclean=nbdocs.apps.app_nbclean:app
+	nbdocs=nbdocs.apps.app_nbdocs:main
+	nb2md=nbdocs.apps.app_nb2md:main
+	nbclean=nbdocs.apps.app_nbclean:main
 pipx.run = 
-	nbdocs=nbdocs.apps.app_nbdocs:app
-	nb2md=nbdocs.apps.app_nb2md:app
-	nbclean=nbdocs.apps.app_nbclean:app
+	nbdocs=nbdocs.apps.app_nbdocs:main
+	nb2md=nbdocs.apps.app_nb2md:main
+	nbclean=nbdocs.apps.app_nbclean:main
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `nbdocs-0.0.41/setup.py` & `nbdocs-0.2.2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,28 @@
 from setuptools import setup
 
 
-VERSION_FILENAME = 'src/nbdocs/version.py'
 REQUIREMENTS_FILENAME = 'requirements.txt'
 REQUIREMENTS_TEST_FILENAME = 'requirements_test.txt'
 
 
 # Requirements
 try:
-    with open(REQUIREMENTS_FILENAME, encoding="utf-8") as f:
-        REQUIRED = f.read().split("\n")
+    with open(REQUIREMENTS_FILENAME, encoding="utf-8") as fh:
+        REQUIRED = fh.read().split("\n")
 except FileNotFoundError:
     REQUIRED = []
 
 try:
-    with open(REQUIREMENTS_TEST_FILENAME, encoding="utf-8") as f:
-        TEST_REQUIRED = f.read().split("\n")
+    with open(REQUIREMENTS_TEST_FILENAME, encoding="utf-8") as fh:
+        TEST_REQUIRED = fh.read().split("\n")
 except FileNotFoundError:
     TEST_REQUIRED = []
 
 # What packages are optional?
 EXTRAS = {"test": TEST_REQUIRED}
 
-# Load the package's __version__ from version.py
-version = {}
-with open(VERSION_FILENAME, 'r') as f:
-    exec(f.read(), version)
-VERSION = version['__version__']
-
 
 setup(
-    version=VERSION,
     install_requires=REQUIRED,
     extras_require=EXTRAS,
 )
```

