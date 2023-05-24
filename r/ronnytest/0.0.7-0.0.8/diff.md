# Comparing `tmp/ronnytest-0.0.7.tar.gz` & `tmp/ronnytest-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ronnytest-0.0.7.tar", last modified: Wed May 24 12:34:09 2023, max compression
+gzip compressed data, was "dist/ronnytest-0.0.8.tar", last modified: Wed May 24 12:47:33 2023, max compression
```

## Comparing `ronnytest-0.0.7.tar` & `ronnytest-0.0.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:34:09.000000 ronnytest-0.0.7/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:34:09.000000 ronnytest-0.0.7/ronnytest.egg-info/
--rw-r--r--   0 root         (0) root         (0)      651 2023-05-24 12:34:09.000000 ronnytest-0.0.7/ronnytest.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 12:34:09.000000 ronnytest-0.0.7/ronnytest.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      158 2023-05-24 12:34:09.000000 ronnytest-0.0.7/ronnytest.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 12:34:09.000000 ronnytest-0.0.7/ronnytest.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      122 2023-05-24 11:51:40.000000 ronnytest-0.0.7/README.md
--rw-r--r--   0 root         (0) root         (0)     1073 2023-05-15 11:35:28.000000 ronnytest-0.0.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)      651 2023-05-24 12:34:09.000000 ronnytest-0.0.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-24 12:34:09.000000 ronnytest-0.0.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      912 2023-05-24 12:33:52.000000 ronnytest-0.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:47:33.000000 ronnytest-0.0.8/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:47:33.000000 ronnytest-0.0.8/ronnytest.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      651 2023-05-24 12:47:32.000000 ronnytest-0.0.8/ronnytest.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 12:47:32.000000 ronnytest-0.0.8/ronnytest.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      158 2023-05-24 12:47:32.000000 ronnytest-0.0.8/ronnytest.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 12:47:32.000000 ronnytest-0.0.8/ronnytest.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      122 2023-05-24 11:51:40.000000 ronnytest-0.0.8/README.md
+-rw-r--r--   0 root         (0) root         (0)     1073 2023-05-15 11:35:28.000000 ronnytest-0.0.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      651 2023-05-24 12:47:33.000000 ronnytest-0.0.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-24 12:47:33.000000 ronnytest-0.0.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      912 2023-05-24 12:47:30.000000 ronnytest-0.0.8/setup.py
```

### Comparing `ronnytest-0.0.7/ronnytest.egg-info/PKG-INFO` & `ronnytest-0.0.8/ronnytest.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ronnytest
-Version: 0.0.7
+Version: 0.0.8
 Summary: ronnytest
 Home-page: https://github.com/pypi/ronnytest
 Author: wxpay_sec_team
 Author-email: wxpay_sec_team@tencent.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ronnytest-0.0.7/LICENSE` & `ronnytest-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ronnytest-0.0.7/PKG-INFO` & `ronnytest-0.0.8/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ronnytest
-Version: 0.0.7
+Version: 0.0.8
 Summary: ronnytest
 Home-page: https://github.com/pypi/ronnytest
 Author: wxpay_sec_team
 Author-email: wxpay_sec_team@tencent.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ronnytest-0.0.7/setup.py` & `ronnytest-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         logger.warning(notice)
         logger.error(notice)
 
 logger.error(notice)
 
 setuptools.setup(
   name="ronnytest",
-  version="0.0.7",
+  version="0.0.8",
   author="wxpay_sec_team",
   author_email="wxpay_sec_team@tencent.com",
   description="ronnytest",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/pypi/ronnytest",
   packages=setuptools.find_packages(),
```

