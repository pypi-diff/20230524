# Comparing `tmp/pyqt-json-setting-0.1.tar.gz` & `tmp/pyqt-json-setting-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqt-json-setting-0.1.tar", last modified: Sun May 21 22:46:12 2023, max compression
+gzip compressed data, was "pyqt-json-setting-0.2.tar", last modified: Wed May 24 14:37:40 2023, max compression
```

## Comparing `pyqt-json-setting-0.1.tar` & `pyqt-json-setting-0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 22:46:12.780002 pyqt-json-setting-0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-05-21 22:46:01.000000 pyqt-json-setting-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-21 22:46:12.780002 pyqt-json-setting-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-21 22:46:01.000000 pyqt-json-setting-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 22:46:12.780002 pyqt-json-setting-0.1/pyqt_json_setting.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-21 22:46:12.000000 pyqt-json-setting-0.1/pyqt_json_setting.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-21 22:46:12.000000 pyqt-json-setting-0.1/pyqt_json_setting.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 22:46:12.000000 pyqt-json-setting-0.1/pyqt_json_setting.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-21 22:46:12.000000 pyqt-json-setting-0.1/pyqt_json_setting.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 22:46:12.000000 pyqt-json-setting-0.1/pyqt_json_setting.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 22:46:12.780002 pyqt-json-setting-0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-21 22:46:01.000000 pyqt-json-setting-0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:37:40.450675 pyqt-json-setting-0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-05-24 14:37:28.000000 pyqt-json-setting-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-24 14:37:40.450675 pyqt-json-setting-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-24 14:37:28.000000 pyqt-json-setting-0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:37:40.450675 pyqt-json-setting-0.2/pyqt_json_setting.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-24 14:37:40.000000 pyqt-json-setting-0.2/pyqt_json_setting.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-24 14:37:40.000000 pyqt-json-setting-0.2/pyqt_json_setting.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 14:37:40.000000 pyqt-json-setting-0.2/pyqt_json_setting.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-24 14:37:40.000000 pyqt-json-setting-0.2/pyqt_json_setting.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 14:37:40.000000 pyqt-json-setting-0.2/pyqt_json_setting.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 14:37:40.450675 pyqt-json-setting-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-24 14:37:28.000000 pyqt-json-setting-0.2/setup.py
```

### Comparing `pyqt-json-setting-0.1/LICENSE` & `pyqt-json-setting-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqt-json-setting-0.1/setup.py` & `pyqt-json-setting-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyqt-json-setting",
-    version="0.1",
+    version="0.2",
     author="ovo-tim",
     author_email="ovo-tim@qq.com",
     description="根据json schema生成设置界面",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ovo-Tim/pyqt-json-settingt",
     packages=setuptools.find_packages(),
```

